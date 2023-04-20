# Comparing `tmp/fringes-0.1.5.tar.gz` & `tmp/fringes-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fringes-0.1.5.tar", max compression
+gzip compressed data, was "fringes-0.1.6.tar", max compression
```

## Comparing `fringes-0.1.5.tar` & `fringes-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      100 2023-04-02 10:36:06.093945 fringes-0.1.5/fringes/__init__.py
--rw-r--r--   0        0        0    15118 2023-04-11 17:47:00.201815 fringes-0.1.5/fringes/decoder.py
--rw-r--r--   0        0        0   103433 2023-04-11 17:50:18.840652 fringes-0.1.5/fringes/fringes.py
--rw-r--r--   0        0        0     4240 2023-03-20 11:38:51.156757 fringes-0.1.5/fringes/grid.py
--rw-r--r--   0        0        0    12901 2023-04-02 11:05:36.206594 fringes-0.1.5/fringes/util.py
--rw-r--r--   0        0        0    21278 2023-01-20 12:12:32.656203 fringes-0.1.5/LICENSE
--rw-r--r--   0        0        0      816 2023-03-31 19:52:30.401871 fringes-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    26112 2023-04-11 17:47:00.199821 fringes-0.1.5/README.md
--rw-r--r--   0        0        0    27109 1970-01-01 00:00:00.000000 fringes-0.1.5/setup.py
--rw-r--r--   0        0        0    26522 1970-01-01 00:00:00.000000 fringes-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      100 2023-04-12 19:36:07.072992 fringes-0.1.6/fringes/__init__.py
+-rw-r--r--   0        0        0    15089 2023-04-20 10:13:33.145944 fringes-0.1.6/fringes/decoder.py
+-rw-r--r--   0        0        0   101502 2023-04-20 17:39:42.888660 fringes-0.1.6/fringes/fringes.py
+-rw-r--r--   0        0        0     3917 2023-04-20 17:25:28.118925 fringes-0.1.6/fringes/grid.py
+-rw-r--r--   0        0        0    12901 2023-04-02 11:05:36.206594 fringes-0.1.6/fringes/util.py
+-rw-r--r--   0        0        0    21278 2023-01-20 12:12:32.656203 fringes-0.1.6/LICENSE
+-rw-r--r--   0        0        0      816 2023-04-19 10:17:47.450559 fringes-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    26825 2023-04-20 20:10:36.865717 fringes-0.1.6/README.md
+-rw-r--r--   0        0        0    27847 1970-01-01 00:00:00.000000 fringes-0.1.6/setup.py
+-rw-r--r--   0        0        0    27266 1970-01-01 00:00:00.000000 fringes-0.1.6/PKG-INFO
```

### Comparing `fringes-0.1.5/fringes/decoder.py` & `fringes-0.1.6/fringes/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 @nb.jit(cache=True, fastmath=True)
 def decode(
     I: np.ndarray,
     N: np.ndarray,
     v: np.ndarray,
     f: np.ndarray,
     R: np.ndarray,  # range
+    a: float = 1,  # alpha
     o: float = np.pi,
     r: float = 0,
     mode: str = "",
     Vmin: float = 0.0,  # 10 / 255  # min fringe contrast i.e. min visibility (can accelerate unwrapping)
     verbose: bool = False,
 ) -> (np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray):
     """Decoding."""
@@ -42,15 +43,15 @@
     assert N.shape == v.shape == f.shape, "N, v, f each must have same shape (D, K)."
     assert False not in [np.any(Nd >= 3) for Nd in N], "Each direction must have at least one set with >= 3 shifts."
     T, Y, X, C = I.shape
     assert np.sum(N) == T, "Sum of shifts must equal number of frames."
     D, K = N.shape
     assert R.size == D, "Screen length must be given for each direction."
 
-    L = max(R)  # length of fringe pattern
+    L = max(R) * a
     l = L / v  # lambda i.e. period lengths in [px]
 
     # precomputations for later use in for-loops
     Nmax = np.max(N)
     sin = np.empty((D, K, Nmax))  # phase shift factors
     cos = np.empty((D, K, Nmax))  # phase shift factors
     for d in nb.prange(D):
@@ -164,26 +165,26 @@
                     if K == 1:
                         if v[d, 0] == 0:  # no spatial modulation
                             if R[d] == 1:
                                 reg[d, y, x, c] = 0  # the only possible value; however this is obsolete as it makes no senso to encode one single coordinate
                                 if verbose:
                                     res[d, y, x, c] = 0
                                     fid[d, 0, y, x, c] = 0
-                            else:  # elif R[d] > 1:
+                            else:
                                 reg[d, y, x, c] = np.nan  # no spatial modulation, therefore we can't compute value
                                 if verbose:
                                     res[d, y, x, c] = np.nan
                                     fid[d, 0, y, x, c] = np.nan
                         elif v[d, 0] <= 1:  # one period covers whole screen: no unwrapping required
                             pn = (p[0] + o) / PI2 % 1  # revert offset and change codomain from [-PI, PI] to [0, 1) -> normalized phi
                             reg[d, y, x, c] = pn * l[d, 0]
                             if verbose:
                                 res[d, y, x, c] = 0  # todo: uncertainty
                                 fid[d, 0, y, x, c] = 0
-                        else:  # v[d, 0] > 1: # spatial phase unwrapping (to be done in a later step)
+                        else:  # spatial phase unwrapping (to be done in a later step)
                             reg[d, y, x, c] = p[0]
                             if verbose:
                                 # todo: residuals are to be received from SPU (spatial phase unwrapping)
                                 fid[d, 0, y, x, c] = np.nan  # unknown
                     else:  # K > 1: temporal phase unwrapping
                         if False:    # todo
                             # cw = np.empty(K)  # fringe visibility (fringe contrast) squared for multiplying into weights
@@ -192,15 +193,15 @@
                             #                         #         cm[k] = 0
                             #                         #     elif B[k] > A[k]:
                             #                         #         cw[k] = np.sqrt(2 - B[k])  # (2 - B[k]) ** (1 / p)  # 1
                             #                         #     else:
                             #                         #         cw[k] = (B[k] / A[k]) ** 2
                             v = A / B  # dim K ?!
                             mask = v < Vmin or B > A or np.isnan(B)  # check for sufficient modulation i.e. fringe contrast
-                            # todo: if umr(v[mask]) < L -> SPU
+                            # todo: if umr(v[mask]) < R -> SPU
                             #     reg[d, y, x, c] = np.nan
                             # if verbose:
                             #   pass  # residuals are to be received from SPU (spatial phase unwrapping)
                             continue
                         else:
                             mn = ssdmax[d] + 0  # adding zero creates a copy
                             pn = (p % PI2 + o) / PI2  # change codomain from [-PI, PI] to [-0.5, 0.5) and revert offset -> normalized phi
```

### Comparing `fringes-0.1.5/fringes/fringes.py` & `fringes-0.1.6/fringes/fringes.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import json
 
 import numpy as np
 import scipy as sp
 import sympy
 import skimage as ski
 import cv2
-# import toml
+import toml
 import yaml
 import asdf
 from si_prefix import si_format as si
 
 from .util import vshape, bilateral, median
 from . import grid
 from .decoder import decode  # todo: fast_decode i.e. fast_unwrap
@@ -57,16 +57,16 @@
         # 'uint64',  # bins = self._xp.arange(mn, mx + 1.01 * step, step, dtype="uint64")
         # "float16",  # numba doesn't handle float16, also most algorithms convert float16 to float32 anyway
         "float32",
         "float64",
     )
     _loader = {
         ".json": json.load,
-        # todo: ".toml": toml.load,
         ".yaml": yaml.safe_load,
+        ".toml": toml.load,
         ".asdf": asdf.open,
     }
 
     # default values are defined here; take care to only use immutable types!
     def __init__(self,
                  Y: int = 1200,
                  X: int = 1920,
@@ -80,15 +80,15 @@
                  v: tuple | np.ndarray = np.array([[13, 7, 89], [13, 7, 89]], float),
                  f: tuple | np.ndarray = np.array([[1, 1, 1], [1, 1, 1]], float),
                  h: tuple | np.ndarray = _hues[0],  # np.array([[255, 255, 255]], int)
                  o: float = np.pi,
                  gamma: float = 1.,
                  A: float = 255 / 2,  # Imax / 2 @ uint8
                  B: float = 255 / 2,  # Imax / 2 @ uint8
-                 V: float = 1.,
+                 V: float = 1.,  # V is inferred from A and B
                  alpha: float = 1.,
                  dtype: str | np.dtype = "uint8",
                  grid: str = "image",
                  angle: float = 0.,
                  axis: int = 0,
                  TDM: bool = True,
                  SDM: bool = False,
@@ -167,15 +167,15 @@
     def __str__(self) -> str:
         return "Fringes"
 
     def __repr__(self) -> str:
         return f"{self.params}"
 
     def __eq__(self, other) -> bool:
-        return self.params == other.params
+        return hasattr(other, "params") and self.params == other.params
 
     def load(self, fname: "") -> dict:
         """Load parameters from file."""
         if not os.path.isfile(fname):
             fname = os.path.dirname(__file__) + os.sep + "params.yaml"
 
         if not fname:
@@ -190,17 +190,16 @@
                 p = f.copy()
         else:
             with open(fname, "r") as f:
                 if ext == ".json":
                     p = json.load(f)
                 elif ext == ".yaml":
                     p = yaml.safe_load(f)
-                # todo:
-                # elif ext == ".toml":
-                #     p = toml.load(f)
+                elif ext == ".toml":
+                    p = toml.load(f)
                 else:
                     self.logger.error(f"Unknown file type '{ext}'.")
                     return {}
 
         if "fringes" in p:
             params = p["fringes"]
             for k in self.params.keys():  # todo: does order in which params are loaded affect final param state?
@@ -227,17 +226,16 @@
             asdf.AsdfFile({"fringes": self.params}).write_to(fname)
         else:
             with open(fname, "w") as f:
                 if ext == ".json":
                     json.dump({"fringes": self.params}, f)
                 elif ext == ".yaml":
                     yaml.dump({"fringes": self.params}, f)
-                # elif ext == ".toml":
-                #     toml.dump({"fringes": self.params}, f)
-                # todo: ".ini"
+                elif ext == ".toml":
+                    toml.dump({"fringes": self.params}, f)
 
         self.logger.info(f"Saved parameters to {fname}.")
 
     def reset(self) -> None:
         """Reset parameters to defaults."""
         # self.__init__()  # attention: config file might be reloaded
 
@@ -313,21 +311,22 @@
         return I.reshape((-1, self.T, X, C)).swapaxes(0, 1)
 
     def coordinates(self) -> np.ndarray:
         """uv-coordinates of grid to encode."""
 
         t0 = time.perf_counter()
 
-        centered = False if self.grid == "image" else True
         sys = "img" if self.grid == "image" else "cart" if self.grid == "Cartesian" else "pol" if self.grid == "polar" else "logpol"
-        uv = np.array(getattr(grid, sys)(self.Y, self.X, self.angle, centered))[self.axis if self.D == 1 else ...]  # * self.L  # todo: numba
+        xi = np.array(getattr(grid, sys)(self.Y, self.X, self.angle))[self.axis if self.D == 1 else ...]
+        if self.grid in ["polar", "log-polar"]:
+            xi *= self.L
 
         self.logger.info(f"{si(time.perf_counter() - t0)}s")
 
-        return uv.reshape((self.D, self.Y, self.X, 1))
+        return xi.reshape((self.D, self.Y, self.X, 1))
 
     def _modulate(self, frame: tuple = None, rint: bool = True) -> np.ndarray:  # todo: rint = False as default? influence on residuals?
         """Encode base fringe patterns by spatio-temporal modulation."""
 
         # dd = [d for d in range(self.D) for k in range(self.K) for n in range(self._N[d, k])]
         # kk = [k for d in range(self.D) for k in range(self.K) for n in range(self._N[d, k])]
         # NN = [self._N[d, k] for d in range(self.D) for k in range(self.K) for n in range(self._N[d, k])]
@@ -354,48 +353,52 @@
             T = len(frame)
         except:
             T = 1
             frame = [frame]
         frames = np.array(frame)
 
         if self.grid != "image" or self.angle != 0:
-            uv = self.coordinates()[..., 0]
-            assert uv.ndim == 3, "uv-coordinates are not three-dimensional with shape (D, Y, X)"
+            xi = self.coordinates()[..., 0]
+            assert xi.ndim == 3, "uv-coordinates are not three-dimensional with shape (D, Y, X)"
         else:
-            uv = None
+            xi = None
 
         # is_pure = all(c == 0 or c == 255 for h in self.h for c in h)
         # dtype = np.dtype("float64") if self.SDM or self.FDM or not is_pure else self.dtype
         dtype = np.dtype("float64") if self.SDM or self.FDM else self.dtype
 
         I = np.empty([T, self.Y, self.X], dtype)
         i = 0
         f = 0
         for d in range(self.D):
-            if uv is None and self.grid == "image":
+            if xi is None and self.grid == "image":
                 x = np.arange(self.R[d]) / self.L  # gets broadcasted
                 if self.D == 2:
                     if d == 0:
                         x = x[None, :]
                     else:
                         x = x[:, None]
                 else:
                     if self.axis == 0:
                         x = x[None, :]
                     else:
                         x = x[:, None]
             else:
-                x = uv[d]
+                x = xi[d] / self.L
 
             for k in range(self.K):
                 q = 2 * np.pi * self._v[d, k]
-                w = 2 * np.pi * self._f[d, k] * (-1 if self.reverse else 1)
+                w = 2 * np.pi * self._f[d, k]
+
+                if self.reverse:
+                    w *= -1
+
                 for n in range(self._N[d, k]):
                     if f in frames:
-                        t = n / 4 if self._N[d, k] == 2 else n / self._N[d, k]  # t = o if N[d, k] == 1
+                        t = n / 4 if self._N[d, k] == 2 else n / self._N[d, k]
                         cos = np.cos(q * x - w * t - self.o)
 
                         if self.gamma == 1:
                             val = self.A + self.B * cos
                         else:
                             val = self.A + self.B * (.5 + .5 * cos) ** self.gamma
 
@@ -406,17 +409,14 @@
                         elif dtype.kind in "b":
                             I[i] = val >= .5
                         else:
                             I[i] = val
                         i += 1
                     f += 1
 
-        # if self.grid in ["polar", "log-polar"]:
-        #     I *= grid.innercirc(self.Y, self.X)[None, None, None, :, :, None]
-
         # dt = np.float64 if self.SDM or self.FDM or np.any((self.h != 0) * (self.h != 255)) else self.dtype
         # I = encode(dt, np.ones(1), frames, self._N, self._v, self._f * (-1 if self.reverse else 1), self.o, self.Y, self.X, 1, self.axis, self.gamma, self.A, self.B)
 
         self.logger.debug(f"{si(time.perf_counter() - t0)}s")
 
         return I.reshape(-1, self.Y, self.X, 1)
 
@@ -514,15 +514,15 @@
             elif self.D == 1:
                 L = max(X, Y)
                 fx = np.fft.fftshift(np.fft.fftfreq(X)) * X * Y / L  # todo: hfft
                 fy = np.fft.fftshift(np.fft.fftfreq(Y)) * Y * X / L
                 fxx, fyy = np.meshgrid(fx, fy)
                 frr = np.sqrt(fxx ** 2 + fyy ** 2)  # todo: normalization of both directions
 
-                mr = frr <= L / 2  # ensure same sampling in all disrections
+                mr = frr <= L / 2  # ensure same sampling in all directions
                 W = 10
                 W = min(max(1, W / 2), L / 20)
                 mr[frr < W] = 0  # remove baseband
                 mr[frr > L / 4] = 0  # remove too high frequencies
 
                 mh = np.empty([Y, X])
                 mh[:, :X // 2] = 1
@@ -584,15 +584,15 @@
             # var = 1 / self._N / self.M / np.sqrt(
             #     self._v)  # / B has to be done in decoder as it depends on captured scene
             # w = 1 / var
             # for d in range(self.D):
             #     w[d] /= np.sum(w[d])
 
             phi, bri, mod, reg, res, fid = decode(
-                I, self._N, self._v, _f, self.R, self.o, r, self.mode, Vmin, self.verbose or verbose
+                I, self._N, self._v, _f, self.R, self.alpha, self.o, r, self.mode, Vmin, self.verbose or verbose
             )
 
         self.logger.debug(f"{si(time.perf_counter() - t0)}s")
 
         return phi, bri, mod, reg, res, fid
 
     def _multiplex(self, I: np.ndarray, rint: bool = True) -> np.ndarray:
@@ -805,36 +805,33 @@
             I = np.moveaxis(I, 0, -2)  # returns a view
             idx = self.h != 0
             I = I[..., idx]  # advanced indexing doesn't return a view
         else:  # fuse colors by weighted averaging
             w = self.h / np.sum(self.h, axis=0)  # normalized weights
             # w[np.isnan(w)] = 0
 
-            if np.all((w == 0) | (w == 1)):
+            if np.all((w == 0) | (w == 1)):  # todo: when does this happen?
                 w = w.astype(bool, copy=False)  # multiplying with bool preserves dtype
                 dtype = I.dtype  # without this, np.sum chooses a dtype which can hold the theoretical maximal sum
             else:
                 dtype = float  # without this, np.sum chooses a dtype which can hold the theoretical maximal sum
 
-
-            # I = I.astype(float, copy=False)
-            # I[w[:, None, None, None, :] == 0] = np.nan
             I = np.sum(I * w[:, None, None, None, :], axis=0, dtype=dtype)
 
         self.logger.debug(f"{si(time.perf_counter() - t0)}s")
 
         return I
 
     def encode(self, frame: int | tuple | list = None, rint: bool = True) -> np.ndarray:
         """Encode fringe patterns."""
 
         t0 = time.perf_counter()
 
         # check UMR
-        if np.any(self.UMR < self.R):
+        if self._isambiguous:
             self.logger.warning(
                 "UMR < R. Unwrapping will not be spatially independent and only yield a relative phase map.")
 
         if frame is not None:  # lazy encoding
             try:  # ensure frame is iterable
                 len(frame)
             except:
@@ -860,14 +857,18 @@
         # modulate
         I = self._modulate(frame, rint)
 
         # multiplex (reduce number of frames)
         if self.SDM or self.WDM or self.FDM:
             I = self._multiplex(I, rint)
 
+        # apply inscribed circle
+        if self.grid in ["polar", "log-polar"]:
+            I *= grid.innercirc(self.Y, self.X)[None, :, :, None]
+
         # colorize (extended averaging)
         if self.H > 1 or np.any(self.h != 255):  # can be used for extended averaging
             I = self._colorize(I, frames)
 
         self.logger.info(f"{si(time.perf_counter() - t0)}s")
 
         return I
@@ -882,18 +883,14 @@
         I = I.reshape((T, Y, X, C))
 
         # assertions
         if T != self.T:
             self.logger.error("Number of frames of parameters and data don't match.")
             return
 
-        if np.any(self.UMR < self.R):
-            self.logger.warning(
-                "UMR < R. Unwrapping will not be spatially independent and only yield a relative phase map.")
-
         if self.FDM:
             assert len(np.unique(self.N)) == 1, "Shifts aren't equal."
 
         # decolorize i.e. fuse hues/colors
         if self.H > 1 or not self._ismono:  # for gray fringes, color fusion is not performed, but extended averaging is
             I = self._decolorize(I)
 
@@ -909,21 +906,31 @@
             if True in idx:  # blacken where color value of hue was black
                 reg[..., idx] = np.nan
                 if self.verbose:
                     res[..., idx] = np.nan
                     fid[..., idx] = -1  # np.nan
 
         # spatial unwrapping
-        if np.any(self.UMR < self.R):
+        if self._isambiguous:
+            self.logger.warning("Unwrapping is not spatially independent and only yields a relative phase map.")
             uwr = self._unwrap(phi if self.verbose or verbose else reg)
 
             if self.verbose:
                 reg, res, fid = uwr
             else:
                 reg = uwr[0]
+        else:
+            # coordiante retransformation
+            if False:  # todo: self.D == 2:
+                if self.grid == "Cartesian":
+                    reg = grid.cart2img(reg, -self.angle)
+                elif self.grid =="polar":
+                    reg = grid.pol2cart(vu, -self.angle)
+                elif self.grid == "log-polar":
+                    reg = grid.logpol2cart(vu, -self.angle)
 
         if denoise:
             reg = bilateral(reg, k=3)
 
         if despike:
             reg = median(reg, k=3)
 
@@ -1054,49 +1061,49 @@
                     # reg[d, :, :, c] = unwrapping_instance.unwrapPhaseMap(phi[d, :, :, c], shadowMask=shadow_mask)
                 else:  # Scikit-image algorithm is slower but delivers better results on edges
                     uwr[t, :, :, c] = ski.restoration.unwrap_phase(phi[t, :, :, c])
 
         return uwr
 
     def remap(self,
-              x: np.ndarray,
+              xi: np.ndarray,
               B: np.ndarray = None,
               Bmin: float = 0,
               scale: float = 1,
               normalize: bool = True) -> np.ndarray:
         """Mapping decoded coordinates (having sub-pixel accuracy)
         from camera grid to (integer) positions on pattern/screen grid
         with weights from modulation.
         This yields a grid representing the screen (light source)
         with the pixel values being a relative measure
         of how much a screen (light source) pixel contributed
         to the exposure of the camera sensor."""
 
         t0 = time.perf_counter()
 
-        T, Y, X, C = vshape(x).shape
+        T, Y, X, C = vshape(xi).shape
 
         if B is not None and B.ndim > 1:
-            assert x.shape[1:] == B.shape[1:], "'x' and 'B' have different width, height or color channels"
+            assert xi.shape[1:] == B.shape[1:], "'xi' and 'B' have different width, height or color channels"
 
             B = B.reshape((-1, Y, X, C))
 
-        x = x.reshape((-1, Y, X, C))
+        xi = xi.reshape((-1, Y, X, C))
 
-        assert np.all(np.round(np.max(x[d])) <= self.R[d] - 1 for d in range(self.D)), \
+        assert np.all(np.round(np.max(xi[d])) <= self.R[d] - 1 for d in range(self.D)), \
             f"Coordinates contain values > {self.R - 1}, decoding might be erroneous."
 
         if T == 1:
             if self.axis == 0:
-                x = np.vstack((x, np.zeros_like(x)))
+                xi = np.vstack((xi, np.zeros_like(xi)))
             else:  # self.axis == 1
-                x = np.vstack((np.zeros_like(x), x))
+                xi = np.vstack((np.zeros_like(xi), xi))
 
         src = np.zeros((int(np.round(self.Y * scale)), int(np.round(self.X * scale)), C), np.float32)
-        idx = np.rint(x.swapaxes(1, 2) * scale).astype(int, copy=False)
+        idx = np.rint(xi.swapaxes(1, 2) * scale).astype(int, copy=False)
         if B is not None:
             val = np.mean(B.swapaxes(1, 2), axis=0)
             if Bmin > 0:
                 val *= val >= Bmin
         else:
             val = np.ones((Y, X, C), np.uint8)
         for c in range(C):
@@ -1117,19 +1124,18 @@
 
         t0 = time.perf_counter()
 
         # f = Fringes(**{k: v for k, v in self.params.items() if k in Fringes.defaults})
         I = self.encode()
         dec = self.decode(I)
 
-        centered = False if self.grid == "image" else True
         sys = "img" if self.grid == "image" else "cart" if self.grid == "Cartesian" else "pol" if self.grid == "polar" else "logpol"
-        uv = np.array(getattr(grid, sys)(self.Y, self.X, self.angle, centered))[:, :, :, None] * self.L
+        xi = np.array(getattr(grid, sys)(self.Y, self.X, self.angle))[:, :, :, None] * self.L
 
-        eps = np.abs(uv - dec.registration)  # / self.L
+        eps = np.abs(xi - dec.registration)  # / self.L
         idxe = np.argwhere(eps.squeeze() > 0.1)
 
         xavg = np.nanmean(eps)
         xmed = np.nanmedian(eps)
         xmax = np.nanmax(eps)
         xstd = np.nanstd(eps)
         SNR = self.L / xstd
@@ -1172,23 +1178,14 @@
             return
 
         if self._grid != _grid and _grid in self._grids:
             self._grid = _grid
             self.logger.debug(f"{self._grid = }")
             self.SDM = self.SDM
 
-            # if self.grid in self._grids[2:]:
-            #     self.angle = 45
-            #     # optional: create quadratic shape of fringe patterns which fit onto screen  # todo
-            #     # L = min(self.X, self.Y)  # max(self.X, self.Y) i.e. self.L  # ... into screen
-            #     # self.X = L
-            #     # self.Y = L
-            # else:
-            #     self.angle = 0
-
     @property
     def angle(self) -> float:
         """Angle of coordinate system's principal axis."""
         return self._angle
 
     @angle.setter
     def angle(self, angle: float):
@@ -1365,19 +1362,15 @@
                 K = _T // self.D - (Nmin - 1)  # Nmin - 1 = 2; i.e. 2 more for first set
                 # Kmax = 2
             else:
                 K = _T // (self.D * Nmin)
             self.K = min(K, Kmax)
 
             # ensure UMR >= R
-            if self.K == 1:
-                self.v = 1
-            if np.any(self.UMR < self.R):
-                # self.v = "auto"
-                # self._v[:, 0] = 1
+            if self._isambiguous:
                 imin = np.argmin(self._v, axis=0)
                 self._v[imin] = 1
 
             # try N >= 4  # todo: try N >= Nmin
             N = np.empty([self.D, self.K], int)
             Navg = _T // (self.D * self.K)
             if Navg < Nmin:  # use N12
@@ -1463,90 +1456,42 @@
     @property
     def P(self) -> int:
         """Number of pixels per color channel and frame."""
         return self.Y * self.X
 
     @property
     def alpha(self) -> float:
-        """Additional relative buffer coding range."""
+        """Factor for extending the coding range 'L'."""
         return self._alpha
 
     @alpha.setter
     def alpha(self, alpha: float):
-        # _alpha = float(min(max(1, alpha), self.alphamax))
-        _alpha = float(max(1, alpha))
+        _alpha = float(min(max(1, alpha), self._alphamax))
 
         if self._alpha != _alpha:
             self._alpha = _alpha
+            self.logger.debug(f"{self._alpha = }")
             self.l = self.L / self._v
 
     @property
     def R(self) -> np.ndarray:
-        """Range of fringe patterns for each direction [px]."""
+        """Lengths of fringe patterns for each direction [px]."""
         if self.D == 2:
             R = np.array([self.X, self.Y])
         else:
             if self.axis == 0:
                 R = np.array([self.X])
             else:
                 R = np.array([self.Y])
-
-        # a = self.angle / 360 * (2 * np.pi)
-        # tan = np.tan(a)
-        # if self.D == 2:
-        #     Rx = self.X + self.Y * tan
-        #     Ry = self.Y + self.X * tan
-        #     R = np.array([Rx, Ry], float)
-        # else:
-        #     if self.axis == 0:
-        #         Rx = self.X + self.Y * tan
-        #         R = np.array([Rx], float)
-        #     else:
-        #         Ry = self.Y + self.X * tan
-        #         R = np.array([Ry], float)
-        # # todo: polar, log-polar coordinates
         return R
 
     @property
     def L(self) -> int | float:
-        """Length of fringe patterns [px]."""
-
-        if True:#self.grid in ["image", "Cartesian"]:
-            if self.angle % 90 == 0:
-                if self.D == 2:
-                    L = max(self.X, self.Y)
-                else:
-                    if self.axis == 0:
-                        L = self.X
-                    else:  # self.axis == 1
-                        L = self.Y
-            else:
-                a = np.deg2rad(self.angle)
-                if self.D == 2:
-                    L = self.X * np.cos(a) + self.Y * np.sin(a)
-                    # Lx = self.X + self.Y * tan
-                    # Ly = self.Y + self.X * tan
-                    # L = max(Lx, Ly)
-                else:
-                    if self.axis == 0:
-                        L = self.X + self.Y * np.tan(a)
-                    else:
-                        L = self.Y + self.X * np.tan(a)
-        elif self.grid == "polar":
-            if self.angle % 90 == 0:
-                L = np.sqrt(self.X ** 2 + self.Y ** 2)  # todo
-            else:
-                L = self.X ** 2 + self.Y ** 2  # todo
-        elif self.grid == "log-polar":
-            if self.angle % 90 == 0:
-                L = np.log(np.sqrt(self.X ** 2 + self.Y ** 2))  # todo
-            else:
-                L = self.X ** 2 + self.Y ** 2  # todo
-
-        return L * self.alpha
+        """Length to be encoded [px]."""
+        return float(self.R.max() * self.alpha)
 
     @property
     def UMR(self) -> np.ndarray:
         """Unambiguous measurement range."""
         # If neither wavelength nor periods are integers, lcm resp. gcd are extended to rational numbers.
 
         if self._UMR is not None:  # cache
@@ -1617,21 +1562,28 @@
                     UMR[d] = np.lcm.reduce(ls) / 10 ** precision
 
         # self._UMR = float(np.min(UMR))  # cast type frm "numpy.core.multiarray.scalar" to "int" or "float"
 
         self._UMR = UMR
         self.logger.debug(f"self.UMR = {str(self.UMR)}")
 
-        if np.any(self.UMR < self.R):
+        if self._isambiguous:
             self.logger.warning(
                 "UMR < R. Unwrapping will not be spatially independent and only yield a relative phase map.")
 
         return self._UMR
 
     @property
+    def eta(self) -> float:
+        """Coding efficiency."""
+        eta = self.R / self.UMR
+        eta[self.UMR < self.R] = 0
+        return eta
+
+    @property
     def M(self) -> int | np.ndarray:
         """Number of averaged intensity samples."""
         M = np.sum(self.h, axis=0) / 255
         if len(set(M)) == 1:
             M = M[0]
         else:
             # todo: M = M[None, None, :]
@@ -1892,21 +1844,14 @@
             l = self.L ** (1 / np.arange(self._l.shape[1] + 1, _K + 1))
             self.l = np.append(self._l, np.tile(l, (self.D, 1)), axis=1)  # l triggers v
             self.f = np.append(self._f, np.tile(self.defaults["f"][0, 0], (self.D, _K - self._f.shape[1])), axis=1)
 
             self.B = self.B
 
     @property
-    def eta(self) -> float:
-        """Coding efficiency."""
-        eta = self.R / self.UMR
-        eta[self.UMR < self.R] = 0
-        return eta
-
-    @property
     def N(self) -> np.ndarray:
         """Number of phase shifts."""
         if self.D == 1 or len(np.unique(self._N, axis=0)) == 1:  # sets in directions are identical
             N = self._N[0]  # 1D
         else:
             N = self._N  # 2D
         return N
@@ -2107,15 +2052,15 @@
             self.logger.debug(f"self._v = {str(self.v.round(3)).replace(chr(10), ',')}")
             self._UMR = None
             self.D, self.K = self._l.shape  # set l before K and K before f
             self.f = self._f
 
     @property
     def v(self) -> np.ndarray:
-        """Spatial frequencies, i.e. number of periods/fringes across maximum length times alpha."""
+        """Spatial frequencies, i.e. number of periods/fringes across maximum coding length."""
         if self.D == 1 or len(np.unique(self._v, axis=0)) == 1:  # sets in directions are identical
             v = self._v[0]  # 1D
         else:
             v = self._v  # 2D
         return v
 
     @v.setter
@@ -2270,14 +2215,19 @@
 
     @property
     def _ismono(self) -> bool:
         """All hues are monochromatic, i.e. RGB values are identical for each hue."""
         return all(len(set(h)) == 1 for h in self.h)
 
     @property
+    def _isambiguous(self) -> bool:
+        """Unambiguous measument range is larger than the screen length."""
+        return np.any(self.UMR < self.R * self.alpha)
+
+    @property
     def Nmin(self) -> int:
         """Minimum number of shifts to (uniformly) sample temporal frequencies."""
         if self.FDM:
             if self.static:
                 Nmin = int(np.ceil(2 * self.f.max() + 1))  # todo: 2 * D * K + 1 -> fractional periods
             else:
                 Nmin = 2 * self.D * self.K + 1
@@ -2357,24 +2307,24 @@
     def PU(self) -> str:
         """Phase unwrapping method."""
 
         if self.SSB:
             PU = "SSB"  # single sideband demodulation
         elif self.K == np.all(self.v <= 1):
             PU = "none"
-        elif np.all(self.UMR >= self.R):
-            PU = "temporal"
-        else:
+        elif self._isambiguous:
             PU = "spatial"
+        else:
+            PU = "temporal"
 
         return PU
 
     @property
     def gamma(self) -> float:
-        """Gamma factor."""
+        """Gamma` correction factor used to compensate the display resonse curve."""
         return self._gamma
 
     @gamma.setter
     def gamma(self, gamma: float):
         _gamma = float(min(max(0, gamma), self._gammamax))
 
         if self._gamma != _gamma and _gamma != 0:
@@ -2572,15 +2522,15 @@
         uxi = upin * self._l  # local positional uncertainties
         ux = np.sqrt(1 / np.sum(1 / uxi ** 2))  # global phase uncertainty (by inverse variance weighting of uxi)
         return float(ux)  # convert Numpy float64 to Python float
 
     @property
     def DR(self) -> float:
         """Dynamic range."""
-        return self.R / self.u
+        return self.UMR / self.u
 
     @property
     def DRdB(self) -> float:
         """Dynamic range [dB]."""
         return 20 * np.log10(self.DR)
 
     @property
@@ -2597,16 +2547,14 @@
                 else:
                     params[p] = getattr(self, p, None)
         return params
 
     # docstrings of properties
     doc = {k: v.__doc__ for k, v in sorted(vars().items()) if isinstance(v, property) and v.__doc__ is not None}
 
-    # amplitude = B
-
     # docstring of __init__()
     __init__.__doc__ = ""
     for __k, __v in sorted(vars().copy().items()):
         if __k in defaults:
             if isinstance(__v, property) and __v.__doc__ is not None:
                 __init__.__doc__ += f"{__k}: {__v.__doc__}\n"
     del __k
```

### Comparing `fringes-0.1.5/fringes/grid.py` & `fringes-0.1.6/fringes/grid.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,45 +33,38 @@
 #     l = np.log(r)
 #
 #     # logpol2pol
 #     p = p
 #     r = np.exp(l)
 
 
-def img(Y: int = 720, X: int = 720, a: float = 0, centered: bool = False):
+def img(Y: int = 720, X: int = 720, a: float = 0):
     # y, x = np.mgrid[:Y, :X]
     y, x = np.indices((Y, X))
     return rot(x, y, a)
 
 
-def cart(Y: int = 720, X: int = 720, a: float = 0, centered: bool = True):
-    L = max(X, Y)
-
-    if centered:
-        x = np.linspace(-X / 2, X / 2, X, endpoint=True)
-        y = np.linspace(Y / 2, -Y / 2, Y, endpoint=True)
-    else:
-        x = np.linspace(0, X, X, endpoint=False)
-        y = np.linspace(Y - 1, 0, -1, X, endpoint=False)
-
+def cart(Y: int = 720, X: int = 720, a: float = 0):
+    x = np.linspace(-(X - 1) / 2, (X - 1) / 2, X, endpoint=True)
+    y = np.linspace((Y - 1) / 2, -(Y - 1) / 2, Y, endpoint=True)
     xx, yy = np.meshgrid(x, y)
     return rot(xx, yy, a)
 
 
-def pol(Y: int = 720, X: int = 720, a: float = 0, centered: bool = True):
+def pol(Y: int = 720, X: int = 720, a: float = 0):
     xx, yy = cart(Y, X)
     pp = np.arctan2(yy, xx) / (2 * np.pi)
     # rr = np.sqrt(xx ** 2 + yy ** 2) * max(X, Y) / min(X, Y)
-    rr = np.sqrt(xx ** 2 + yy ** 2) # / np.sqrt((min(X, Y) / max(X, Y)) ** 2 + 1)
+    rr = np.sqrt(xx ** 2 + yy ** 2) / min(X, Y)
     return rot(pp, rr, a)
 
 
-def logpol(Y: int = 720, X: int = 720, a: float = 0, centered: bool = True):
+def logpol(Y: int = 720, X: int = 720, a: float = 0):
     pp, rr = pol(Y, X)
-    ll = np.log(rr + 1)  # with rr in [0, 1] -> ll in [0, 0.693]; important is only the logarithmical progression
+    ll = np.log(rr) / (2 * np.pi)
     return rot(pp, ll, a)
 
 
 def rot(uu, vv, a):
     # a *= -1
     if a % 360 == 0:
         return uu, vv
@@ -107,37 +100,37 @@
 
 # todo: coordinate transformations, add angle
 def cart2pol(uv, a: float = 0):
     xx = uv[0]
     yy = uv[1]
     pp = np.arctan2(yy, xx)
     rr = np.sqrt(xx ** 2 + yy ** 2)
-    return np.stack((pp, rr), axis=0)
+    return np.stack(rot(pp, rr, a), axis=0)
 
 
 def pol2cart(uv, a: float = 0):
     pp = uv[0] * 2 * np.pi
     rr = uv[1]
     xx = rr * np.cos(pp)
     yy = rr * np.sin(pp)
-    return np.stack((xx, yy), axis=0)
+    return np.stack(rot(xx, yy, a), axis=0)
 
 
 def pol2logpol(uv, a: float = 0):
     pp = uv[0]
     rr = uv[1]
     ll = np.log(rr)
-    return np.stack((pp, ll), axis=0)
+    return np.stack(rot(pp, ll, a), axis=0)
 
 
 def logpol2pol(uv, a: float = 0):
     pp = uv[0]
     ll = uv[1]
-    rr = np.exp(ll)
-    return np.stack((pp, rr), axis=0)
+    rr = np.exp(ll) - 1
+    return np.stack(rot(pp, rr, a), axis=0)
 
 
 def cart2logpol(uv, a: float = 0):
     xx = uv[0]
     yy = uv[1]
     pp = np.arctan2(yy, xx) / (2 * np.pi)
     rr = np.sqrt(xx ** 2 + yy ** 2)
```

### Comparing `fringes-0.1.5/fringes/util.py` & `fringes-0.1.6/fringes/util.py`

 * *Files identical despite different names*

### Comparing `fringes-0.1.5/LICENSE` & `fringes-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fringes-0.1.5/pyproject.toml` & `fringes-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Fringes"
-version = "0.1.5"
+version = "0.1.6"
 description = "Phase shifting algorithms for encoding and decoding sinusoidal fringe patterns."
 license = "CC-BY-NC-SA-4.0"
 authors = ["Christian Kludt"]
 readme = "README.md"
 repository = "https://github.com/comimag/fringes"
 keywords = ["phase shifting", "fringe analysis", "fringe projection", "deflectometry", "computational imaging"]
 
@@ -14,16 +14,16 @@
 numba = "^0.56.4"
 opencv-contrib-python = "^4.7.0"
 pyyaml = "^6.0"
 scikit-image = "^0.19.3"
 scipy = "^1.10.0"
 si-prefix = "^1.2.2"
 sympy = "^1.11.1"
+toml = "^0.10.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 pytest = "^7.2.1"
-toml = "^0.10.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fringes-0.1.5/README.md` & `fringes-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # Fringes
-
 Author: Christian Kludt
 
 [//]: # (![Parameter Interdependencies]&#40;docs/spirals.png&#41;)
+<img src="docs/du-bist-ein-wildschwein.gif">
 
 ## Description
 This package provides the handy `Fringes` class which handles all the required parameters
 for configuring fringe pattern sequences
 and provides methods for fringe analysis.
 <!---
 link to  paper, please cite
 --->
 
 ### Features
-<!---
-- Generalized Temporal Phase Unwrappting (GTPU)[[14](#14-kludt-2024)]
---->
+
 - Generalized Temporal Phase Unwrappting (GTPU)
 - Uncertainty Propagation
 - Optimal Coding Strategy
 - Deinterlacing
 - Multiplexing
 - Filtering Phase Maps
 - Remapping
@@ -135,47 +133,45 @@
 You can change the [logging level](https://docs.python.org/3/library/logging.html#levels) of a `Fringes` instance.
 Changing it to `'DEBUG'` gives you verbose feedback on which parameters are changed
 and how long functions take to execute.
 
 ```python
 f.logger.setLevel("DEBUG")
 ```
-<!---
+
 ## Graphical User Interface
-Do you need a GUI? `Fringes` has a sister project that is called `Fringes GUI`:
-https://pypi.org/project/fringes-gui/
---->
+Do you need a GUI? `Fringes` has a sister project that is called `Fringes-GUI`: https://pypi.org/project/fringes-gui/
+
 ## Attributes
 All parameters are parsed when setting, so usually several input formats are accepted, e.g.
 `bool`, `int`, `float`, `str` for scalars and additionally `list`, `tuple`, `ndarray` for arrays.
 
 Note that parameters might have circular dependencies which are resolved automatically,
-hence dependent parameters might change as well. 
-The attributes in rectangular boxes are readonly, i.e. they are inferred from the others.
-Only the ones in white boxes will never influence others.
+hence dependent parameters might change as well.
 
 ![Parameter Interdependencies](docs/interdependencies.svg)\
 Parameter and their Interdependencies.
 
 ### __Video Shape__
 Standardized `shape` `(T, Y, X, C)` of fringe pattern sequence, with
 - `T`: number of frames
 - `Y`: height
 - `X`: width
 - `C`: number of color channels
 
 `T` depends on the paremeters `H`, `D`, `K`, `N` and the [multiplexing](#multiplexing) methods:\
 If all `N` are identical, then `T = H * D * K * N` with `N` as a scalar,
 else <code>T = H * &sum; N<sub>i</sub></code> with `N` as an array.\
-If a [multiplexing](#multiplexing) methods is activated, `T` reduces further.
-
-The length `L` is the maximum of `X` and `Y`.
+If a [multiplexing](#multiplexing) method is activated, `T` reduces further.
 
 `C` depends on the [coloring](#coloring-and-averaging) and [multiplexing](#multiplexing) methods.
 
+The length `L` is the maximum of `X` and `Y` and denotes the length in [px] to be ancoded.\
+It can be extended by the factor `alpha`.
+
 `size` is the product of `shape`.
 
 ### __Coordinate System__
 The following coordinate systems can be used by setting `grid` to:
 - `'image'`: The top left corner pixel of the grid is the origin (0, 0)
 and positive directions are right- resp. downwards.
 - `'Cartesian'`: The center of grid is the origin (0, 0) and positive directions are right- resp. upwards.
@@ -211,24 +207,14 @@
 Usually `f = 1` and is essentially only changed if [frequency division multiplexing](#multiplexing) `FDM` is activated.
 
 `reverse` is a boolean which reverses the direction of the shifts (by multiplying `f` with `-1`).
 
 `o` denotes the phase offset `φ₀` which can be used to
 e.g. let the fringe patterns start (at the origin) with a gray value of zero.
 
-`UMR` denotes the unambiguous measurement range.
-The coding is only unique in the interval `[0, UMR)`; after that it repeats itself.
-The `UMR` is derived from `l` and `v`:
-- If <code>l &isin; &#8469;</code>, <code>UMR = lcm(l<sub>i</sub>)</code> with `lcm` being the least common multiple.
-- Else, if <code>v &isin; &#8469;</code>,
-  <code>UMR = `L`/ gcd(v<sub>i</sub>)</code> with `gcd` being the greatest common divisor.
-- Else, if <code>l &and; v &isin; &#8474;</code>, `lcm` resp. `gdc` are extended to rational numbers.
-- Else, if <code>l &and; v &isin; &#8477; \ &#8474;</code>, `l` and `v` are approximated by rational numbers
-  with a fixed length of decimal digits.
-
 ### __Coloring and Averaging__
 The fringe pattern sequence `I` can be colorized by setting the hue `h` to any RGB color tuple
 in the interval `[0, 255]`. However, black `(0, 0, 0)` is not allowed. `h` must be in shape `(H, 3)`:\
 `H` is the number of hues and can be set directly; 3 is the length of the RGB color tuple.\
 The hues `h` can also be set by assigning any combination of the following characters as a string:
 - `'r'`: red
 - `'g'`: green
@@ -267,15 +253,15 @@
   If one wants a static pattern, i.e. one that remains congruent when shifted, set `static` to `True`.
 
 `SDM` and `WDM` can be used together [[6]](#6) (reducing `T` by a factor of 2 * 3 = 6), `FDM` with neighter.
 
 By default, the aforementioned multiplexing methods are deactivated,
 so we then only have `TDM`: Time Divison Multiplexing.
 
-### __Data Type__
+### __Values__
 `dtype` denotes the data type of the fringe pattern sequence `I`.\
 Possible values are:
 - `'bool'`
 - `'uint8'` (the default)
 - `'uint16'`
 - `'float32'`
 - `'float64'`
@@ -288,15 +274,18 @@
 `Imax` in turn limits the offset `A` and the amplitude `B`.
 The fringe visibility (also called fringe contrast) is `V = A / B` with <code>V &isin; [0, 1]</code>.
 
 The quantization step size `q` is also derived from `dtype`:
 `q = 1` for `bool` and `Q`-bit `unsigned integers`, 
 and for `float` its corresponding [resolution](https://numpy.org/doc/stable/reference/generated/numpy.finfo.html).
 
-The standard deviation of the quantization noise  is <code>QN = q / &radic; 12</code>.
+The standard deviation of the quantization noise  is <code>quant = q / &radic; 12</code>.
+
+`gamma` denotes the gamma correction factor and can be used to compensate for nonlinearities
+of the display response curve.
 
 ### Unwrapping
 - `PU` denotes the phase unwrapping method and is eihter `'none'`, `'temporal'`, `'spatial'` or `'SSB'`.
 See [spatial demodulation](#spatial-demodulation--phase-unwrapping--pu-) for more details.
 - `mode` denotes the mode used for [temporal phase unwrapping](#temporal-phase-unwrapping--tpu-).
   Choose either `'fast'` (the default) or `'precise'`.
 - `Vmin` denotes the minimal fringe visibility (fringe contrast) required for the measurement to be valid
@@ -304,39 +293,49 @@
 - `verbose` can be set to `True` to also receive the wrapped phase map `φ`,
 the fringe orders `k` and the residuals `r` from decoding.
 - `SSB` denotes **Single Sideband Demodulation** [[17]](#17-takeda) and is deployed
 if <code>K &equiv; H &equiv; N &equiv; 1</code>, i.e. <code>T &equiv; 1</code>
 and the [coordinate system](#coordinate-system) is eighter `'image'` or `'Cartesian'`.
 
 ### __Quality Metrics__
+`UMR` denotes the unambiguous measurement range.
+The coding is only unique in the interval `[0, UMR)`; after that it repeats itself.
+The `UMR` is derived from `l` and `v`:
+- If <code>l &isin; &#8469;</code>, <code>UMR = lcm(l<sub>i</sub>)</code> with `lcm` being the least common multiple.
+- Else, if <code>v &isin; &#8469;</code>,
+  <code>UMR = `L`/ gcd(v<sub>i</sub>)</code> with `gcd` being the greatest common divisor.
+- Else, if <code>l &and; v &isin; &#8474;</code>, `lcm` resp. `gdc` are extended to rational numbers.
+- Else, if <code>l &and; v &isin; &#8477; \ &#8474;</code>, `l` and `v` are approximated by rational numbers
+  with a fixed length of decimal digits.
+
 `eta` denotes the coding efficiency `L / UMR`. It makes no sense to choose `UMR` much larger than `L`,
 because then a significant part of the coding range is not used.
 
 `u` denotes the minimum possible uncertainty of the measurement in pixels.
 It is based on the phase noise model from [[7]](#7),
 propagated through [generalized temporal phase unwrapping](#temporal-phase-unwrapping--tpu-) and converted from phase to pixel units.
 It is influenced by the fringe parameters
 - `M`: number of [averaged](#coloring-and-averaging) intensity samples
 - `N`: number of phase shifts
 - `l`: wavelengths of the fringes
 - `B`: measured amplitude
 
 and the measurement hardware-specific noise sources [[8]](#8), [[9]](#9)
-- `dark`: dark noise of the used camera
 - `shot`: photon noise of light itself
 - `quant`: quantization noise of the light source or camera
+- `dark`: dark noise of the used camera
 
-The maximum possible dynamic range of the measurement is `DR = L / u`.
-It describes how many points can be discriminated on the interval `[0, L)`.
+The maximum possible dynamic range of the measurement is `DR = UMR / u`.
+It describes how many points can be discriminated on the interval `[0, UMR)`.
 It remains constant if `L` and hence `l` are scaled (the scaling factor cancels out).
 
 ## Methods
 - `load(fname)`\
   Load a parameter set from the file `fname` to a `Fringes` instance.
-  Supported file formats are `.json`, `.yaml` and `.asdf`.
+  Supported file formats are `*.json`, `*.yaml` and `*.asdf`.
 - `save(fname)`\
   Save the parameter set of the current `Fringes` instance to the file `fname`.
   If `fname` is not provided, the default is `params.yaml` within the package's directory 'fringes'.
 - `reset()`\
   Reset the parameter set of the current `Fringes` instance to the default values.
 - `auto(T)`\
   Automatically set the [optimal parameters](#optimal-coding-strategy) based on the argument `T` (number of frames).
@@ -358,15 +357,15 @@
   If either the argument `verbose` or the attribute with the same name is `True`,
   additional infomation is computed and retuned: phase maps `φ`, residuals `r` and fringe orders `k`.\
   If the argument `denoise` is `True`, the unwrapped phase map is smoothened by a bilateral filter
   which is edge-preserving.\
   If the argument `despike` is `True`, single pixel outliers in the unwrapped phase map
   are replaced by their local neighborhood using a median filter.
 - `remap(registration, modulation)`\
-  Mapping decoded registered coordinates `ξ` (having sub-pixel accuracy)
+  Mapping decoded, registered coordinates `ξ` (having sub-pixel accuracy)
   from camera grid to (integer) positions on the pattern/screen grid
   with weights from modulation `B`.
   The default for `modulation` is `None`, in which case all weights are assumed to equal one.
   The method yields a grid representing the screen (light source)
   with the pixel values being a relative measure
   of how much a screen (light source) pixel contributed
   to the exposure of the camera sensor.
@@ -385,15 +384,15 @@
   `T` is number of frames, `Y` is height, `X` is width, and `C` is number of color channels.
   Ensures that the array becomes 4-dimensional and that the size of the last dimension,
   i.e. the number of color channels <code>C &isin; {1; 3; 4}</code>. To do this, leading dimensions may be flattened.
 - `curvature(registration)`\
   Returns a curvature map. 
 - `height(curvature)`\
   Local height map by local integration via an inverse laplace filter [[19]](#19).\
-  Think of it as a relief, where height is only relative to the local neighborhood.`
+  Think of it as a relief, where height is only relative to the local neighborhood.
 
 ## __Optimal Coding Strategy__
 As makes sense intuitively, more sets `K` as well as more shifts `N` per set reduce the uncertainty `u` after decoding.
 A minimum of 3 shifts is needed to solve for the 3 unknowns brightness `A`, modulation `B` and coordinates `ξ`.
 Any additional 2 shifts compensate for one harmonic of the recorded fringe pattern.
 Therefore, higher accuracy can be achieved using more shifts `N`, but the time required to capture them 
 sets a practical upper limit to the feasible number of shifts.
@@ -402,14 +401,16 @@
 but the resolution of the camera and the display must resolve the fringe pattern spatially.
 Hence, the used hardware imposes a lower bound for the wavelength (or upper bound for the number of periods).
    
 Also, small wavelengths might result in a smaller unambiguous measurement range `UMR`.
 If two or more sets `K` are used and their wavelengths `l` resp. number of periods `v` are relative primes,
 the unmbiguous measurement range can be increased many times.
 As a consequence, one can use much smaller wavelenghts `l` (larger number of periods `v`).
+
+
 However, it must be assured that the unambiguous measurment range is always equal or larger than both,
 the width `X` and the height `Y`.
 Else, [temporal phase unwrapping](#temporal-phase-unwrapping--tpu-) would yield wrong results and thus instead
 [spatial phase unwrapping](#spatial-phase-unwrapping--spu-) is used.
 Be aware that in the latter case only a relative phase map is obtained,
 which lacks the information of where exactly the camera sight rays were looking at during acquisition.
 
@@ -448,28 +449,34 @@
   During the first execution, an initial compilation is executed. 
   This can take several tens of seconds up to single digit minutes, depending on your CPU.
   However, for any subsequent execution, the compiled code is cached and the code of the function runs much faster, 
   approaching the speeds of code written in C.
 
 
 - __My decoded coordinates show lots of noise__
-
-  Try using more, sets `K` and/or shifts `N` and adjust the used wavelengths `l` resp. number of periods `v`.\
-  Also, make sure the exposure of your camera is adjusted so that the fringe patterns show up with maximum contrast.\
-  Try to avoid under- and overexposure during acquisition.
-
-
-- #### My decoded coordinates show systematic offsets
-  First, ensure that the correct frame was captured while acquiring the fringe pattern sequence.
-  If the timings are not set correctly, the sequence may be a frame off.\
-  Secondly, this might occur if either the camera or the display used have a gamma value very different from 1.
-  Typical screens have a gamma value of 2.2;   therefore compensate by setting the inverse value
-  <code>gamma<sup>-1</sup> = 1 / 2.2 &approx; 0.45</code> to the `gamma` attribute of the `Fringes` instance.
-  Alternatively, change the gamma value of the light source or camera directly.
-  You might also use more shifts `N` to compensate for the dominant harmonics of the gamma-nonlinearities.
+  - Make sure the exposure of your camera is adjusted so that the fringe patterns show up with maximum contrast.
+    Try to avoid under- and overexposure during acquisition.
+  - Try using more, sets `K` and/or shifts `N`.
+  - Adjust the used wavelengths `l` resp. number of periods `v` to ensure the unamboguous measurement range
+    is larger than the pattern length, i.e. <code>UMR &ge; L</code>.
+  - If the decoded modulation is much lower than the decoded brightness,
+    try to use larger wavelengths `l` resp. smaller number of periods `v`.\
+    If the decoded modulation remains low even with very large wavelengths (less than five periods per screen length),
+    and you are conducting a deflectometric mesurement, the surface under test is probably too rough.
+    Since deflectometry is for specular and glossy surfsces only, it isn't suited for scattering ones.
+    You should consider a different measurement technique, e.g. fringe projection.
+
+- __My decoded coordinates show systematic offsets__
+  - First, ensure that the correct frame was captured while acquiring the fringe pattern sequence.
+    If the timings are not set correctly, the sequence may be a frame off.
+  - Secondly, this might occur if either the camera or the display used have a gamma value very different from 1.
+    Typical screens have a gamma value of 2.2;   therefore compensate by setting the inverse value
+    <code>gamma<sup>-1</sup> = 1 / 2.2 &approx; 0.45</code> to the `gamma` attribute of the `Fringes` instance.
+    Alternatively, change the gamma value of the light source or camera directly.
+    You might also use more shifts `N` to compensate for the dominant harmonics of the gamma-nonlinearities.
 
 ## References
 
 #### [11] [Burke 2002]
 [J. Burke, T. Bothe, W. Osten, and C. Hess,
 “Reverse engineering by fringe projection,”
 in Interferometry XI: Applications (W. Osten, ed.), vol. 4778, pp. 312–324, SPIE,
@@ -528,8 +535,8 @@
 
 ## License
 Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License
 
 ## Project Status
 This package is in an early stage and under active development,
 so features and functionally will be added in the future.
-Feature requests are warmly welcomed!
+Feature requests are warmly welcomed!
```

### Comparing `fringes-0.1.5/setup.py` & `fringes-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 ['asdf>=2.14.3,<3.0.0',
  'numba>=0.56.4,<0.57.0',
  'opencv-contrib-python>=4.7.0,<5.0.0',
  'pyyaml>=6.0,<7.0',
  'scikit-image>=0.19.3,<0.20.0',
  'scipy>=1.10.0,<2.0.0',
  'si-prefix>=1.2.2,<2.0.0',
- 'sympy>=1.11.1,<2.0.0']
+ 'sympy>=1.11.1,<2.0.0',
+ 'toml>=0.10.2,<0.11.0']
 
 setup_kwargs = {
     'name': 'fringes',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Phase shifting algorithms for encoding and decoding sinusoidal fringe patterns.',
-    'long_description': '# Fringes\n\nAuthor: Christian Kludt\n\n[//]: # (![Parameter Interdependencies]&#40;docs/spirals.png&#41;)\n\n## Description\nThis package provides the handy `Fringes` class which handles all the required parameters\nfor configuring fringe pattern sequences\nand provides methods for fringe analysis.\n<!---\nlink to  paper, please cite\n--->\n\n### Features\n<!---\n- Generalized Temporal Phase Unwrappting (GTPU)[[14](#14-kludt-2024)]\n--->\n- Generalized Temporal Phase Unwrappting (GTPU)\n- Uncertainty Propagation\n- Optimal Coding Strategy\n- Deinterlacing\n- Multiplexing\n- Filtering Phase Maps\n- Remapping\n\n### Background\nMany applications, such as fringe projection [[11]](#11-burke-2002) or deflectometry [[1]](#1-burke-2022),\nrequire the ability to encode positional data.\nTo do this, fringe patterns are used to encode the position on the screen / projector (in pixel coordinates)\nat which the camera pixels were looking at during acquisition.\n\n--- FIGURE coding ---\n\n```\nI = A + B * cos(2πvξ/L - 2πft - φ₀)\n  = A + B * cos(kx - wt - φ₀)\n  = A + B * cos(Φ)\n```\n\n- **Encoding**\n  - **Spatial Modulation**\\\nThe x- resp. y-coordinate `ξ` of the screen/projector is normalized into the range `[0, 1)`\nby dividing through the maximum coordinate `L`\nand used to modulate the luminance in a sinusoidal fringe pattern `I`\nwith offset `A`, amplitude `B` and spatial frequency `v`.\n  - **Temporal Modulation**\\\nThe pattern is then shifted `N` times with an equidistant phase shift of `2πf/N` radian each.\nAn additional phase offset `φ₀` may be set, e.g. to let the fringe patterns start with a gray value of zero.\n- **Decoding**\n  - **Temporal Demodulation**\\\nFrom these shifts, the phase map `φ` is determined [[13]](#13-burke-2012). Due to the trigonometric functions used,\nthe global phase `Φ` is wrapped into the interval <code>[0, 2 &pi;]</code> with `v` periods:\n<code>φ &equiv; Φ mod 2&pi;</code>.\n  - **Spatial Demodulation / Phase Unwrapping**\\\nIf only one set with spatial frequency <code>v &le; 1</code> is used,\nno unwrapping is required because one period covers the complete coding range.\nHence, the coordinates `ξ` are computed directly by scaling: <code>ξ = φ / (2&pi;) * L / v</code>.\nThis constitutes the registration, which is a mapping in the same pixel grid as the camera sensor\nand contains the information where each camera pixel, i.e. each camera sightray, was looking at\nduring the fringe pattern acquisition.\nNote that in contrast to binary coding schemes, e.g. Gray code,\nthe coordinates are obtained with sub-pixel precision.\n    - **Temporal Phase Unwrapping (TPU)**\\\nIf multiple sets with different spatial frequencies `v` are used\nand the [unmbiguous measurement range](#quality-metrics) is larger than the coding range <code>UMR &ge; L</code>,\nthe ambiguity of the phase map is resolved by\ngeneralized multi-frequency temporal phase unwrapping (GTPU) [[14]](#14-kludt-2024).\n    - **Spatial Phase Unwrapping (SPU)**\\\nHowever, if only one set with `v > 1` is used, or multiple sets but  `UMR < L`, the ambiguous phase `φ`\nis unwrapped analyzing the neighbouring phase values [[15]](#15-herráez-2002) [[16]](#16-lei-2015).\nThis only yields a relative phase map, therefore absolute positions are unknown.\n\n## Contents\n- [Installation](#installation)\n- [Usage](#usage)\n- [Graphical User Interface](#graphical-user-interface)\n- [Attributes](#attributes)\n- [Methods](#methods)\n- [Optimal Coding Strategy](#optimal-coding-strategy)\n- [Troubleshooting](#troubleshooting)\n- [License](#license)\n- [Project Status](#project-status)\n\n## Installation\nYou can install `fringes` directly from [PyPi](https://pypi.org/) via `pip`:\n\n```\npip install fringes\n```\n\n## Usage\nYou instantiate and deploy the `Fringes` class:\n\n```python\nimport fringes as frng\n\nf = frng.Fringes()      # instanciate class\n```\n\nFor creating the fringe pattern sequence `I`, use the method `encode()`.\nIt will return a [NumPy array](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) \nin [videoshape](#video-shape) (frames, width, height, color channels).\n\n```python\nI = f.encode()          # encode fringe patterns\n```\n\nFor analyzing (recorded) fringe patterns, use the method `decode()`.\nIt will return a [namedtuple](https://docs.python.org/3/library/collections.html#collections.namedtuple), \ncontaining the Numpy arrays brightness `A`, modulation `B` and the coordinates `ξ`,\nall in [videoshape](#video-shape).\n\n```python\nA, B, xi = f.decode(I)  # decode fringe patterns\n```\n\nAll parameters are accesible by the respective attributes of the `Fringes` class.\n\n```python\nf.X = 1920              # set width of the fringe patterns\nf.Y = 1080              # set height of the fringe patterns\nf.K = 2                 # set number of sets\nf.N = 4                 # set number of shifts\nf.v = [9, 10]           # set spatial frequencies\nf.T                     # get the number of frames\n```\n\nA glossary of them is obtained by the class attribute `doc`.\n\n```python\nfrng.Fringes.doc        # get glossary\n```\n\nYou can change the [logging level](https://docs.python.org/3/library/logging.html#levels) of a `Fringes` instance.\nChanging it to `\'DEBUG\'` gives you verbose feedback on which parameters are changed\nand how long functions take to execute.\n\n```python\nf.logger.setLevel("DEBUG")\n```\n<!---\n## Graphical User Interface\nDo you need a GUI? `Fringes` has a sister project that is called `Fringes GUI`:\nhttps://pypi.org/project/fringes-gui/\n--->\n## Attributes\nAll parameters are parsed when setting, so usually several input formats are accepted, e.g.\n`bool`, `int`, `float`, `str` for scalars and additionally `list`, `tuple`, `ndarray` for arrays.\n\nNote that parameters might have circular dependencies which are resolved automatically,\nhence dependent parameters might change as well. \nThe attributes in rectangular boxes are readonly, i.e. they are inferred from the others.\nOnly the ones in white boxes will never influence others.\n\n![Parameter Interdependencies](docs/interdependencies.svg)\\\nParameter and their Interdependencies.\n\n### __Video Shape__\nStandardized `shape` `(T, Y, X, C)` of fringe pattern sequence, with\n- `T`: number of frames\n- `Y`: height\n- `X`: width\n- `C`: number of color channels\n\n`T` depends on the paremeters `H`, `D`, `K`, `N` and the [multiplexing](#multiplexing) methods:\\\nIf all `N` are identical, then `T = H * D * K * N` with `N` as a scalar,\nelse <code>T = H * &sum; N<sub>i</sub></code> with `N` as an array.\\\nIf a [multiplexing](#multiplexing) methods is activated, `T` reduces further.\n\nThe length `L` is the maximum of `X` and `Y`.\n\n`C` depends on the [coloring](#coloring-and-averaging) and [multiplexing](#multiplexing) methods.\n\n`size` is the product of `shape`.\n\n### __Coordinate System__\nThe following coordinate systems can be used by setting `grid` to:\n- `\'image\'`: The top left corner pixel of the grid is the origin (0, 0)\nand positive directions are right- resp. downwards.\n- `\'Cartesian\'`: The center of grid is the origin (0, 0) and positive directions are right- resp. upwards.\n- `\'polar\'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.\n- `\'log-polar\'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.\n\n`D` denotes the number of directions to be encoded.\nIf <code>D &equiv; 1</code>, the parameter `axis` is used to define along which axis of the coordinate system\n(index 0 or 1) the fringes are shifted.\n\n`angle` can be used to tilt the coordinate system. The origin stays the same.\n\n### __Set__\nEach set consists of the following parameters:\n- `N`: number of shifts\n- `l`: wavelength [px]\n- `v`: spatial frequency, i.e. number of periods (per screen length `L`)\n- `f`: temporal frequency, i.e. number of periods to shift over\n\nEach is an array with shape (number of directions `D`, number of sets `K`).\\\nFor example, if <code>N.shape &equiv; (2, 3)</code>, it means that we encode `D = 2` directions with `K = 3` sets each.\n\nChanging `D` or `K` directly, changes the shape of all set parameters.\nWhen setting a set parameter with a new shape (`D\'`, `K\'`),\n`D` and `K` are updated as well as the shape of the other set parameters.\n\nPer direction at least one set with <code>N &ge; 3</code> is necessary\nto solve for the three unknowns brightness `A`, modulation `B` and coordinates `ξ`.\n\n`l` and `v` are related by `l = L / v`.\nWhen `L` changes, `v` is kept constant and only `l` is changed.\n\nUsually `f = 1` and is essentially only changed if [frequency division multiplexing](#multiplexing) `FDM` is activated.\n\n`reverse` is a boolean which reverses the direction of the shifts (by multiplying `f` with `-1`).\n\n`o` denotes the phase offset `φ₀` which can be used to\ne.g. let the fringe patterns start (at the origin) with a gray value of zero.\n\n`UMR` denotes the unambiguous measurement range.\nThe coding is only unique in the interval `[0, UMR)`; after that it repeats itself.\nThe `UMR` is derived from `l` and `v`:\n- If <code>l &isin; &#8469;</code>, <code>UMR = lcm(l<sub>i</sub>)</code> with `lcm` being the least common multiple.\n- Else, if <code>v &isin; &#8469;</code>,\n  <code>UMR = `L`/ gcd(v<sub>i</sub>)</code> with `gcd` being the greatest common divisor.\n- Else, if <code>l &and; v &isin; &#8474;</code>, `lcm` resp. `gdc` are extended to rational numbers.\n- Else, if <code>l &and; v &isin; &#8477; \\ &#8474;</code>, `l` and `v` are approximated by rational numbers\n  with a fixed length of decimal digits.\n\n### __Coloring and Averaging__\nThe fringe pattern sequence `I` can be colorized by setting the hue `h` to any RGB color tuple\nin the interval `[0, 255]`. However, black `(0, 0, 0)` is not allowed. `h` must be in shape `(H, 3)`:\\\n`H` is the number of hues and can be set directly; 3 is the length of the RGB color tuple.\\\nThe hues `h` can also be set by assigning any combination of the following characters as a string:\n- `\'r\'`: red\n- `\'g\'`: green\n- `\'b\'`: blue\n- `\'c\'`: cyan\n- `\'m\'`: magenta\n- `\'y\'`: yellow\n- `\'w\'`: white\n\n`C` is the number of color channels required for either the set of hues `h`\nor [wavelength division multiplexing](#multiplexing).\nFor example, if all hues are monochromatic, i.e. the RGB values are identical for each hue, `C` equals 1, else 3.\n\nRepeating hues will be fused by averaging them before decoding.\\\n`M` is the number of averaged intensity samples and can be set directly.\n\n### __Multiplexing__\nThe following multiplexing methods can be activated by setting them to `True`:\n- `SDM`: Spatial Division Multiplexing [[2]](#2)\\\n  This results in crossed fringe patterns. The amplitude `B` is halved.\\\n  It can only be activated if we have two directions <code>D &equiv; 2</code>.\\\n  The number of frames `T` is reduced by a factor of 2.\n- `WDM`: Wavelength Divison Multiplexing [[3]](#3)\\\n  All shifts `N` must equal 3. Then, the shifts are multiplexed into the color channel,\n  resulting in an RGB fringe pattern.\\\n  The number of frames `T` is reduced by a factor of 3.\n- `FDM`: Frequency Division Multiplexing [[4]](#4), [[5]](#5)\\\n  Here, the directions `D` and the sets `K` are multiplexed.\n  Hence, the amplitude `B` is reduced by a factor of `D * K`.\\\n  It can only be activated if <code>D &or; K > 1</code> i.e. `D * K > 1`.\\\n  This results in crossed fringe patterns if <code>D &equiv; 2</code>.\\\n  Each set per direction receives an individual temporal frequency `f`,\n  which is used in [temporal demodulation](#temporal-demodulation) to distinguish the individual sets.\\\n  A minimal number of shifts <code>N<sub>min</sub> &ge; &LeftCeiling;</sub> 2 * f<sub>max</sub> + 1 &RightCeiling;</code>\n  is required to satisfy the sampling theorem and `N` is updated automatically if necessary.\\\n  If one wants a static pattern, i.e. one that remains congruent when shifted, set `static` to `True`.\n\n`SDM` and `WDM` can be used together [[6]](#6) (reducing `T` by a factor of 2 * 3 = 6), `FDM` with neighter.\n\nBy default, the aforementioned multiplexing methods are deactivated,\nso we then only have `TDM`: Time Divison Multiplexing.\n\n### __Data Type__\n`dtype` denotes the data type of the fringe pattern sequence `I`.\\\nPossible values are:\n- `\'bool\'`\n- `\'uint8\'` (the default)\n- `\'uint16\'`\n- `\'float32\'`\n- `\'float64\'`\n\nThe total number of bytes `nbytes` consumed by the fringe pattern sequence\nas well as its maximum gray value `Imax` are derived directly from it:\\\n`Imax = 1` for `float` and `bool`,\nand <code>Imax = 2<sup>Q</sup> - 1</code> for `unsigned integers` with `Q` bits.\n\n`Imax` in turn limits the offset `A` and the amplitude `B`.\nThe fringe visibility (also called fringe contrast) is `V = A / B` with <code>V &isin; [0, 1]</code>.\n\nThe quantization step size `q` is also derived from `dtype`:\n`q = 1` for `bool` and `Q`-bit `unsigned integers`, \nand for `float` its corresponding [resolution](https://numpy.org/doc/stable/reference/generated/numpy.finfo.html).\n\nThe standard deviation of the quantization noise  is <code>QN = q / &radic; 12</code>.\n\n### Unwrapping\n- `PU` denotes the phase unwrapping method and is eihter `\'none\'`, `\'temporal\'`, `\'spatial\'` or `\'SSB\'`.\nSee [spatial demodulation](#spatial-demodulation--phase-unwrapping--pu-) for more details.\n- `mode` denotes the mode used for [temporal phase unwrapping](#temporal-phase-unwrapping--tpu-).\n  Choose either `\'fast\'` (the default) or `\'precise\'`.\n- `Vmin` denotes the minimal fringe visibility (fringe contrast) required for the measurement to be valid\nand is in the interval `[0, 1]`. During decoding, pixels with less are discarded, which can speed up the computation.\n- `verbose` can be set to `True` to also receive the wrapped phase map `φ`,\nthe fringe orders `k` and the residuals `r` from decoding.\n- `SSB` denotes **Single Sideband Demodulation** [[17]](#17-takeda) and is deployed\nif <code>K &equiv; H &equiv; N &equiv; 1</code>, i.e. <code>T &equiv; 1</code>\nand the [coordinate system](#coordinate-system) is eighter `\'image\'` or `\'Cartesian\'`.\n\n### __Quality Metrics__\n`eta` denotes the coding efficiency `L / UMR`. It makes no sense to choose `UMR` much larger than `L`,\nbecause then a significant part of the coding range is not used.\n\n`u` denotes the minimum possible uncertainty of the measurement in pixels.\nIt is based on the phase noise model from [[7]](#7),\npropagated through [generalized temporal phase unwrapping](#temporal-phase-unwrapping--tpu-) and converted from phase to pixel units.\nIt is influenced by the fringe parameters\n- `M`: number of [averaged](#coloring-and-averaging) intensity samples\n- `N`: number of phase shifts\n- `l`: wavelengths of the fringes\n- `B`: measured amplitude\n\nand the measurement hardware-specific noise sources [[8]](#8), [[9]](#9)\n- `dark`: dark noise of the used camera\n- `shot`: photon noise of light itself\n- `quant`: quantization noise of the light source or camera\n\nThe maximum possible dynamic range of the measurement is `DR = L / u`.\nIt describes how many points can be discriminated on the interval `[0, L)`.\nIt remains constant if `L` and hence `l` are scaled (the scaling factor cancels out).\n\n## Methods\n- `load(fname)`\\\n  Load a parameter set from the file `fname` to a `Fringes` instance.\n  Supported file formats are `.json`, `.yaml` and `.asdf`.\n- `save(fname)`\\\n  Save the parameter set of the current `Fringes` instance to the file `fname`.\n  If `fname` is not provided, the default is `params.yaml` within the package\'s directory \'fringes\'.\n- `reset()`\\\n  Reset the parameter set of the current `Fringes` instance to the default values.\n- `auto(T)`\\\n  Automatically set the [optimal parameters](#optimal-coding-strategy) based on the argument `T` (number of frames).\n  This also takes into account the minimum resolvable wavelength `lmin` and the length of the fringe patterns `L`.\n- `setMTF(B)`\\\n  Compute the normalized modulation transfer function at spatial frequencies `v`\n  and use the result to set the optimal `lmin`.\n  `B` is the modulation from decoding. For more details, see [Optimal Coding Strategy](#optimal-coding-strategy).\n- `coordinates()`\\\n  Generate the coordinate matrices of the defined [coordinate system](#coordinate-system).\n- `encode(frames)`\\\n  [Encode](#encoding) the fringe pattern sequence `I`.\\\n  The frames <code>I<sub>t</sub></code> can be encoded indiviually\n  by passing the frame indices `frames`, either as an `integer` or a `tuple`.\n  The default is `None` in which case all frames are encoded.\\\n  To receive the frames iteratively (i.e. in a lazy manner), simply iterate over the `Fringes` instance.\n- `decode(I, verbose)`\\\n  [Decode](#decoding) the fringe pattern sequence `I`.\\\n  If either the argument `verbose` or the attribute with the same name is `True`,\n  additional infomation is computed and retuned: phase maps `φ`, residuals `r` and fringe orders `k`.\\\n  If the argument `denoise` is `True`, the unwrapped phase map is smoothened by a bilateral filter\n  which is edge-preserving.\\\n  If the argument `despike` is `True`, single pixel outliers in the unwrapped phase map\n  are replaced by their local neighborhood using a median filter.\n- `remap(registration, modulation)`\\\n  Mapping decoded registered coordinates `ξ` (having sub-pixel accuracy)\n  from camera grid to (integer) positions on the pattern/screen grid\n  with weights from modulation `B`.\n  The default for `modulation` is `None`, in which case all weights are assumed to equal one.\n  The method yields a grid representing the screen (light source)\n  with the pixel values being a relative measure\n  of how much a screen (light source) pixel contributed\n  to the exposure of the camera sensor.\n- `deinterlace(I)`\\\n  Deinterlace a fringe pattern sequence `I` acquired with a line scan camera\n  while each frame has been displayed and captured\n  while the object has been moved by one pixel.\n\nThe next methods are class-methods:\n- `unwrap(phi)`\\\n  [Unwrap](#spatial-phase-unwrapping--spu-) the phase map `phi` i.e. `φ` spacially.\n\nThe next methods are package-methods:\n- `vshape(I)`\\\n  Transforms video data of arbitrary shape and dimensionality into the standardized shape `(T, Y, X, C)`, where\n  `T` is number of frames, `Y` is height, `X` is width, and `C` is number of color channels.\n  Ensures that the array becomes 4-dimensional and that the size of the last dimension,\n  i.e. the number of color channels <code>C &isin; {1; 3; 4}</code>. To do this, leading dimensions may be flattened.\n- `curvature(registration)`\\\n  Returns a curvature map. \n- `height(curvature)`\\\n  Local height map by local integration via an inverse laplace filter [[19]](#19).\\\n  Think of it as a relief, where height is only relative to the local neighborhood.`\n\n## __Optimal Coding Strategy__\nAs makes sense intuitively, more sets `K` as well as more shifts `N` per set reduce the uncertainty `u` after decoding.\nA minimum of 3 shifts is needed to solve for the 3 unknowns brightness `A`, modulation `B` and coordinates `ξ`.\nAny additional 2 shifts compensate for one harmonic of the recorded fringe pattern.\nTherefore, higher accuracy can be achieved using more shifts `N`, but the time required to capture them \nsets a practical upper limit to the feasible number of shifts.\n\nGenerally, shorter wavelengths `l` (or equivalently more periods `v`) reduce the uncertainty `u`,\nbut the resolution of the camera and the display must resolve the fringe pattern spatially.\nHence, the used hardware imposes a lower bound for the wavelength (or upper bound for the number of periods).\n   \nAlso, small wavelengths might result in a smaller unambiguous measurement range `UMR`.\nIf two or more sets `K` are used and their wavelengths `l` resp. number of periods `v` are relative primes,\nthe unmbiguous measurement range can be increased many times.\nAs a consequence, one can use much smaller wavelenghts `l` (larger number of periods `v`).\nHowever, it must be assured that the unambiguous measurment range is always equal or larger than both,\nthe width `X` and the height `Y`.\nElse, [temporal phase unwrapping](#temporal-phase-unwrapping--tpu-) would yield wrong results and thus instead\n[spatial phase unwrapping](#spatial-phase-unwrapping--spu-) is used.\nBe aware that in the latter case only a relative phase map is obtained,\nwhich lacks the information of where exactly the camera sight rays were looking at during acquisition.\n\nTo simplify finding and setting the optimal parameters, the following methods can be used:\n- `setMTF()`: The optimal `vmax` is determined automativally [[18]](#18-bothe-2008)\nby measuring the **modulation transfer function** `MTF`.\\\n  Therefore, a sequence of exponentially increasing `v` is acquired:\n    1. Set `v` to `\'exponential\'`.\n    2. Encode, acquire and decode the fringe pattern sequence.\n    3. Call the function `setMTF(B)` with the argument `B` from decoding.\n- `v` can be set to `\'auto\'`. This automatically determines the optimal integer set of `v`\n  based on the maximal resolvable spatial frequency `vmax`.\n-  Equivalently, `l` can also be set to `\'auto\'`. This will automatically determine the optimal integer set of `l`\n  based on the minimal resolvable wavelength `lmin = L / vmax`.\n- `T` can be set directly, based on the desired acquisition time.\n  The optimal `K`, `N` and the [multiplexing](#multiplexing) methods will be determined automatically.\n\nAlternatively, simply use the function `auto()`\nto automatically set the optimal `v`, `T` and [multiplexing](#multiplexing) methods.\n\n## Troubleshooting\n<!---\n- __`poetry install` does not work__\n  \n  First, ensure that poetry is installed correctly as descibed onthe [Poetry Website](https://python-poetry.org/docs/).\\\n  Secondly, ensure the correct python version is installed on your system, as specified in the file `pyproject.toml`!\\\n  Thirdly, this can be caused by a proxy which `pip` does not handle correctly.\n  Manually setting the proxy in the Windows settings or even adding a system variable \n`https_proxy = http://YOUR_PROXY:PORT` can resolve this.\n--->\n\n- __Decoding takes a long time__\n  \n  This is probably related to the just-in-time compiler [Numba](https://numba.pydata.org/) \n  used for this computationally expensive function:\n  During the first execution, an initial compilation is executed. \n  This can take several tens of seconds up to single digit minutes, depending on your CPU.\n  However, for any subsequent execution, the compiled code is cached and the code of the function runs much faster, \n  approaching the speeds of code written in C.\n\n\n- __My decoded coordinates show lots of noise__\n\n  Try using more, sets `K` and/or shifts `N` and adjust the used wavelengths `l` resp. number of periods `v`.\\\n  Also, make sure the exposure of your camera is adjusted so that the fringe patterns show up with maximum contrast.\\\n  Try to avoid under- and overexposure during acquisition.\n\n\n- #### My decoded coordinates show systematic offsets\n  First, ensure that the correct frame was captured while acquiring the fringe pattern sequence.\n  If the timings are not set correctly, the sequence may be a frame off.\\\n  Secondly, this might occur if either the camera or the display used have a gamma value very different from 1.\n  Typical screens have a gamma value of 2.2;   therefore compensate by setting the inverse value\n  <code>gamma<sup>-1</sup> = 1 / 2.2 &approx; 0.45</code> to the `gamma` attribute of the `Fringes` instance.\n  Alternatively, change the gamma value of the light source or camera directly.\n  You might also use more shifts `N` to compensate for the dominant harmonics of the gamma-nonlinearities.\n\n## References\n\n#### [11] [Burke 2002]\n[J. Burke, T. Bothe, W. Osten, and C. Hess,\n“Reverse engineering by fringe projection,”\nin Interferometry XI: Applications (W. Osten, ed.), vol. 4778, pp. 312–324, SPIE,\n2002.](https://doi.org/10.1117/12.473547)\n\n#### [1] [Burke 2022] \n[J. Burke, A. Pak, S. Höfer, M. Ziebarth, M. Roschani, J. Beyerer,\n"Deflectometry for specular surfaces: an overview",\narXiv:2204.11592v1 [physics.optics],\n2022.](https://arxiv.org/abs/2204.11592)\n\n#### [2] [Park2008]?\n\n#### [3] [Huang 1999]\n\n#### [4] [Liu 2014] [Liu2010] [Park2008]?\n\n#### [5] [Kludt 2018]\n\n#### [6] [Trumper 2016]\n\n#### [7] [Surrel 1997]\n\n#### [8] [EMVA1288]\n\n#### [9] [Bothe2008]\n\n#### [10] [Fischer]\n\n#### [13] [Burke 2012]\n[J. Burke,\n"Phase Decoding and Reconstruction",\nvol. Optical Methods for Solid Mechanics: A Full-Field Approach, ch. 3, pp. 83–141. Wiley, Weinheim,\n2012.](https://www.wiley.com/en-us/Optical+Methods+for+Solid+Mechanics%3A+A+Full+Field+Approach-p-9783527411115)\n\n#### [14] [Kludt 2024]\n\n#### [15] [Herráez 2002]\n[Miguel Arevallilo Herráaez, David R. Burton, Michael J. Lalor, and Munther A. Gdeisat.\nFast two-dimensional phase-unwrapping algorithm based on sorting by reliability following a noncontinuous path.\nAppl. Opt., 41(35):7437-7444,\nDec 2002.](https://opg.optica.org/ao/abstract.cfm?uri=ao-41-35-7437)\n\n#### [16] [Lei 2015]\n[Hai Lei, Xin yu Chang, Fei Wang, Xiao-Tang Hu, and Xiao-Dong Hu.\nA novel algorithm based on histogram processing of reliability for two-dimensional phase unwrapping.\nOptik - International Journal for Light and Electron Optics, 126(18):1640 - 1644,\n2015.](https://www.sciencedirect.com/science/article/abs/pii/S0030402615003228?via%3Dihub)\n\n#### [17] [Takeda]\n\n#### [18] [Bothe 2008]\n\n#### [19]\nInverse Laplace Filter\n\n## License\nCreative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License\n\n## Project Status\nThis package is in an early stage and under active development,\nso features and functionally will be added in the future.\nFeature requests are warmly welcomed!',
+    'long_description': '# Fringes\nAuthor: Christian Kludt\n\n[//]: # (![Parameter Interdependencies]&#40;docs/spirals.png&#41;)\n<img src="docs/du-bist-ein-wildschwein.gif">\n\n## Description\nThis package provides the handy `Fringes` class which handles all the required parameters\nfor configuring fringe pattern sequences\nand provides methods for fringe analysis.\n<!---\nlink to  paper, please cite\n--->\n\n### Features\n\n- Generalized Temporal Phase Unwrappting (GTPU)\n- Uncertainty Propagation\n- Optimal Coding Strategy\n- Deinterlacing\n- Multiplexing\n- Filtering Phase Maps\n- Remapping\n\n### Background\nMany applications, such as fringe projection [[11]](#11-burke-2002) or deflectometry [[1]](#1-burke-2022),\nrequire the ability to encode positional data.\nTo do this, fringe patterns are used to encode the position on the screen / projector (in pixel coordinates)\nat which the camera pixels were looking at during acquisition.\n\n--- FIGURE coding ---\n\n```\nI = A + B * cos(2πvξ/L - 2πft - φ₀)\n  = A + B * cos(kx - wt - φ₀)\n  = A + B * cos(Φ)\n```\n\n- **Encoding**\n  - **Spatial Modulation**\\\nThe x- resp. y-coordinate `ξ` of the screen/projector is normalized into the range `[0, 1)`\nby dividing through the maximum coordinate `L`\nand used to modulate the luminance in a sinusoidal fringe pattern `I`\nwith offset `A`, amplitude `B` and spatial frequency `v`.\n  - **Temporal Modulation**\\\nThe pattern is then shifted `N` times with an equidistant phase shift of `2πf/N` radian each.\nAn additional phase offset `φ₀` may be set, e.g. to let the fringe patterns start with a gray value of zero.\n- **Decoding**\n  - **Temporal Demodulation**\\\nFrom these shifts, the phase map `φ` is determined [[13]](#13-burke-2012). Due to the trigonometric functions used,\nthe global phase `Φ` is wrapped into the interval <code>[0, 2 &pi;]</code> with `v` periods:\n<code>φ &equiv; Φ mod 2&pi;</code>.\n  - **Spatial Demodulation / Phase Unwrapping**\\\nIf only one set with spatial frequency <code>v &le; 1</code> is used,\nno unwrapping is required because one period covers the complete coding range.\nHence, the coordinates `ξ` are computed directly by scaling: <code>ξ = φ / (2&pi;) * L / v</code>.\nThis constitutes the registration, which is a mapping in the same pixel grid as the camera sensor\nand contains the information where each camera pixel, i.e. each camera sightray, was looking at\nduring the fringe pattern acquisition.\nNote that in contrast to binary coding schemes, e.g. Gray code,\nthe coordinates are obtained with sub-pixel precision.\n    - **Temporal Phase Unwrapping (TPU)**\\\nIf multiple sets with different spatial frequencies `v` are used\nand the [unmbiguous measurement range](#quality-metrics) is larger than the coding range <code>UMR &ge; L</code>,\nthe ambiguity of the phase map is resolved by\ngeneralized multi-frequency temporal phase unwrapping (GTPU) [[14]](#14-kludt-2024).\n    - **Spatial Phase Unwrapping (SPU)**\\\nHowever, if only one set with `v > 1` is used, or multiple sets but  `UMR < L`, the ambiguous phase `φ`\nis unwrapped analyzing the neighbouring phase values [[15]](#15-herráez-2002) [[16]](#16-lei-2015).\nThis only yields a relative phase map, therefore absolute positions are unknown.\n\n## Contents\n- [Installation](#installation)\n- [Usage](#usage)\n- [Graphical User Interface](#graphical-user-interface)\n- [Attributes](#attributes)\n- [Methods](#methods)\n- [Optimal Coding Strategy](#optimal-coding-strategy)\n- [Troubleshooting](#troubleshooting)\n- [License](#license)\n- [Project Status](#project-status)\n\n## Installation\nYou can install `fringes` directly from [PyPi](https://pypi.org/) via `pip`:\n\n```\npip install fringes\n```\n\n## Usage\nYou instantiate and deploy the `Fringes` class:\n\n```python\nimport fringes as frng\n\nf = frng.Fringes()      # instanciate class\n```\n\nFor creating the fringe pattern sequence `I`, use the method `encode()`.\nIt will return a [NumPy array](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) \nin [videoshape](#video-shape) (frames, width, height, color channels).\n\n```python\nI = f.encode()          # encode fringe patterns\n```\n\nFor analyzing (recorded) fringe patterns, use the method `decode()`.\nIt will return a [namedtuple](https://docs.python.org/3/library/collections.html#collections.namedtuple), \ncontaining the Numpy arrays brightness `A`, modulation `B` and the coordinates `ξ`,\nall in [videoshape](#video-shape).\n\n```python\nA, B, xi = f.decode(I)  # decode fringe patterns\n```\n\nAll parameters are accesible by the respective attributes of the `Fringes` class.\n\n```python\nf.X = 1920              # set width of the fringe patterns\nf.Y = 1080              # set height of the fringe patterns\nf.K = 2                 # set number of sets\nf.N = 4                 # set number of shifts\nf.v = [9, 10]           # set spatial frequencies\nf.T                     # get the number of frames\n```\n\nA glossary of them is obtained by the class attribute `doc`.\n\n```python\nfrng.Fringes.doc        # get glossary\n```\n\nYou can change the [logging level](https://docs.python.org/3/library/logging.html#levels) of a `Fringes` instance.\nChanging it to `\'DEBUG\'` gives you verbose feedback on which parameters are changed\nand how long functions take to execute.\n\n```python\nf.logger.setLevel("DEBUG")\n```\n\n## Graphical User Interface\nDo you need a GUI? `Fringes` has a sister project that is called `Fringes-GUI`: https://pypi.org/project/fringes-gui/\n\n## Attributes\nAll parameters are parsed when setting, so usually several input formats are accepted, e.g.\n`bool`, `int`, `float`, `str` for scalars and additionally `list`, `tuple`, `ndarray` for arrays.\n\nNote that parameters might have circular dependencies which are resolved automatically,\nhence dependent parameters might change as well.\n\n![Parameter Interdependencies](docs/interdependencies.svg)\\\nParameter and their Interdependencies.\n\n### __Video Shape__\nStandardized `shape` `(T, Y, X, C)` of fringe pattern sequence, with\n- `T`: number of frames\n- `Y`: height\n- `X`: width\n- `C`: number of color channels\n\n`T` depends on the paremeters `H`, `D`, `K`, `N` and the [multiplexing](#multiplexing) methods:\\\nIf all `N` are identical, then `T = H * D * K * N` with `N` as a scalar,\nelse <code>T = H * &sum; N<sub>i</sub></code> with `N` as an array.\\\nIf a [multiplexing](#multiplexing) method is activated, `T` reduces further.\n\n`C` depends on the [coloring](#coloring-and-averaging) and [multiplexing](#multiplexing) methods.\n\nThe length `L` is the maximum of `X` and `Y` and denotes the length in [px] to be ancoded.\\\nIt can be extended by the factor `alpha`.\n\n`size` is the product of `shape`.\n\n### __Coordinate System__\nThe following coordinate systems can be used by setting `grid` to:\n- `\'image\'`: The top left corner pixel of the grid is the origin (0, 0)\nand positive directions are right- resp. downwards.\n- `\'Cartesian\'`: The center of grid is the origin (0, 0) and positive directions are right- resp. upwards.\n- `\'polar\'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.\n- `\'log-polar\'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.\n\n`D` denotes the number of directions to be encoded.\nIf <code>D &equiv; 1</code>, the parameter `axis` is used to define along which axis of the coordinate system\n(index 0 or 1) the fringes are shifted.\n\n`angle` can be used to tilt the coordinate system. The origin stays the same.\n\n### __Set__\nEach set consists of the following parameters:\n- `N`: number of shifts\n- `l`: wavelength [px]\n- `v`: spatial frequency, i.e. number of periods (per screen length `L`)\n- `f`: temporal frequency, i.e. number of periods to shift over\n\nEach is an array with shape (number of directions `D`, number of sets `K`).\\\nFor example, if <code>N.shape &equiv; (2, 3)</code>, it means that we encode `D = 2` directions with `K = 3` sets each.\n\nChanging `D` or `K` directly, changes the shape of all set parameters.\nWhen setting a set parameter with a new shape (`D\'`, `K\'`),\n`D` and `K` are updated as well as the shape of the other set parameters.\n\nPer direction at least one set with <code>N &ge; 3</code> is necessary\nto solve for the three unknowns brightness `A`, modulation `B` and coordinates `ξ`.\n\n`l` and `v` are related by `l = L / v`.\nWhen `L` changes, `v` is kept constant and only `l` is changed.\n\nUsually `f = 1` and is essentially only changed if [frequency division multiplexing](#multiplexing) `FDM` is activated.\n\n`reverse` is a boolean which reverses the direction of the shifts (by multiplying `f` with `-1`).\n\n`o` denotes the phase offset `φ₀` which can be used to\ne.g. let the fringe patterns start (at the origin) with a gray value of zero.\n\n### __Coloring and Averaging__\nThe fringe pattern sequence `I` can be colorized by setting the hue `h` to any RGB color tuple\nin the interval `[0, 255]`. However, black `(0, 0, 0)` is not allowed. `h` must be in shape `(H, 3)`:\\\n`H` is the number of hues and can be set directly; 3 is the length of the RGB color tuple.\\\nThe hues `h` can also be set by assigning any combination of the following characters as a string:\n- `\'r\'`: red\n- `\'g\'`: green\n- `\'b\'`: blue\n- `\'c\'`: cyan\n- `\'m\'`: magenta\n- `\'y\'`: yellow\n- `\'w\'`: white\n\n`C` is the number of color channels required for either the set of hues `h`\nor [wavelength division multiplexing](#multiplexing).\nFor example, if all hues are monochromatic, i.e. the RGB values are identical for each hue, `C` equals 1, else 3.\n\nRepeating hues will be fused by averaging them before decoding.\\\n`M` is the number of averaged intensity samples and can be set directly.\n\n### __Multiplexing__\nThe following multiplexing methods can be activated by setting them to `True`:\n- `SDM`: Spatial Division Multiplexing [[2]](#2)\\\n  This results in crossed fringe patterns. The amplitude `B` is halved.\\\n  It can only be activated if we have two directions <code>D &equiv; 2</code>.\\\n  The number of frames `T` is reduced by a factor of 2.\n- `WDM`: Wavelength Divison Multiplexing [[3]](#3)\\\n  All shifts `N` must equal 3. Then, the shifts are multiplexed into the color channel,\n  resulting in an RGB fringe pattern.\\\n  The number of frames `T` is reduced by a factor of 3.\n- `FDM`: Frequency Division Multiplexing [[4]](#4), [[5]](#5)\\\n  Here, the directions `D` and the sets `K` are multiplexed.\n  Hence, the amplitude `B` is reduced by a factor of `D * K`.\\\n  It can only be activated if <code>D &or; K > 1</code> i.e. `D * K > 1`.\\\n  This results in crossed fringe patterns if <code>D &equiv; 2</code>.\\\n  Each set per direction receives an individual temporal frequency `f`,\n  which is used in [temporal demodulation](#temporal-demodulation) to distinguish the individual sets.\\\n  A minimal number of shifts <code>N<sub>min</sub> &ge; &LeftCeiling;</sub> 2 * f<sub>max</sub> + 1 &RightCeiling;</code>\n  is required to satisfy the sampling theorem and `N` is updated automatically if necessary.\\\n  If one wants a static pattern, i.e. one that remains congruent when shifted, set `static` to `True`.\n\n`SDM` and `WDM` can be used together [[6]](#6) (reducing `T` by a factor of 2 * 3 = 6), `FDM` with neighter.\n\nBy default, the aforementioned multiplexing methods are deactivated,\nso we then only have `TDM`: Time Divison Multiplexing.\n\n### __Values__\n`dtype` denotes the data type of the fringe pattern sequence `I`.\\\nPossible values are:\n- `\'bool\'`\n- `\'uint8\'` (the default)\n- `\'uint16\'`\n- `\'float32\'`\n- `\'float64\'`\n\nThe total number of bytes `nbytes` consumed by the fringe pattern sequence\nas well as its maximum gray value `Imax` are derived directly from it:\\\n`Imax = 1` for `float` and `bool`,\nand <code>Imax = 2<sup>Q</sup> - 1</code> for `unsigned integers` with `Q` bits.\n\n`Imax` in turn limits the offset `A` and the amplitude `B`.\nThe fringe visibility (also called fringe contrast) is `V = A / B` with <code>V &isin; [0, 1]</code>.\n\nThe quantization step size `q` is also derived from `dtype`:\n`q = 1` for `bool` and `Q`-bit `unsigned integers`, \nand for `float` its corresponding [resolution](https://numpy.org/doc/stable/reference/generated/numpy.finfo.html).\n\nThe standard deviation of the quantization noise  is <code>quant = q / &radic; 12</code>.\n\n`gamma` denotes the gamma correction factor and can be used to compensate for nonlinearities\nof the display response curve.\n\n### Unwrapping\n- `PU` denotes the phase unwrapping method and is eihter `\'none\'`, `\'temporal\'`, `\'spatial\'` or `\'SSB\'`.\nSee [spatial demodulation](#spatial-demodulation--phase-unwrapping--pu-) for more details.\n- `mode` denotes the mode used for [temporal phase unwrapping](#temporal-phase-unwrapping--tpu-).\n  Choose either `\'fast\'` (the default) or `\'precise\'`.\n- `Vmin` denotes the minimal fringe visibility (fringe contrast) required for the measurement to be valid\nand is in the interval `[0, 1]`. During decoding, pixels with less are discarded, which can speed up the computation.\n- `verbose` can be set to `True` to also receive the wrapped phase map `φ`,\nthe fringe orders `k` and the residuals `r` from decoding.\n- `SSB` denotes **Single Sideband Demodulation** [[17]](#17-takeda) and is deployed\nif <code>K &equiv; H &equiv; N &equiv; 1</code>, i.e. <code>T &equiv; 1</code>\nand the [coordinate system](#coordinate-system) is eighter `\'image\'` or `\'Cartesian\'`.\n\n### __Quality Metrics__\n`UMR` denotes the unambiguous measurement range.\nThe coding is only unique in the interval `[0, UMR)`; after that it repeats itself.\nThe `UMR` is derived from `l` and `v`:\n- If <code>l &isin; &#8469;</code>, <code>UMR = lcm(l<sub>i</sub>)</code> with `lcm` being the least common multiple.\n- Else, if <code>v &isin; &#8469;</code>,\n  <code>UMR = `L`/ gcd(v<sub>i</sub>)</code> with `gcd` being the greatest common divisor.\n- Else, if <code>l &and; v &isin; &#8474;</code>, `lcm` resp. `gdc` are extended to rational numbers.\n- Else, if <code>l &and; v &isin; &#8477; \\ &#8474;</code>, `l` and `v` are approximated by rational numbers\n  with a fixed length of decimal digits.\n\n`eta` denotes the coding efficiency `L / UMR`. It makes no sense to choose `UMR` much larger than `L`,\nbecause then a significant part of the coding range is not used.\n\n`u` denotes the minimum possible uncertainty of the measurement in pixels.\nIt is based on the phase noise model from [[7]](#7),\npropagated through [generalized temporal phase unwrapping](#temporal-phase-unwrapping--tpu-) and converted from phase to pixel units.\nIt is influenced by the fringe parameters\n- `M`: number of [averaged](#coloring-and-averaging) intensity samples\n- `N`: number of phase shifts\n- `l`: wavelengths of the fringes\n- `B`: measured amplitude\n\nand the measurement hardware-specific noise sources [[8]](#8), [[9]](#9)\n- `shot`: photon noise of light itself\n- `quant`: quantization noise of the light source or camera\n- `dark`: dark noise of the used camera\n\nThe maximum possible dynamic range of the measurement is `DR = UMR / u`.\nIt describes how many points can be discriminated on the interval `[0, UMR)`.\nIt remains constant if `L` and hence `l` are scaled (the scaling factor cancels out).\n\n## Methods\n- `load(fname)`\\\n  Load a parameter set from the file `fname` to a `Fringes` instance.\n  Supported file formats are `*.json`, `*.yaml` and `*.asdf`.\n- `save(fname)`\\\n  Save the parameter set of the current `Fringes` instance to the file `fname`.\n  If `fname` is not provided, the default is `params.yaml` within the package\'s directory \'fringes\'.\n- `reset()`\\\n  Reset the parameter set of the current `Fringes` instance to the default values.\n- `auto(T)`\\\n  Automatically set the [optimal parameters](#optimal-coding-strategy) based on the argument `T` (number of frames).\n  This also takes into account the minimum resolvable wavelength `lmin` and the length of the fringe patterns `L`.\n- `setMTF(B)`\\\n  Compute the normalized modulation transfer function at spatial frequencies `v`\n  and use the result to set the optimal `lmin`.\n  `B` is the modulation from decoding. For more details, see [Optimal Coding Strategy](#optimal-coding-strategy).\n- `coordinates()`\\\n  Generate the coordinate matrices of the defined [coordinate system](#coordinate-system).\n- `encode(frames)`\\\n  [Encode](#encoding) the fringe pattern sequence `I`.\\\n  The frames <code>I<sub>t</sub></code> can be encoded indiviually\n  by passing the frame indices `frames`, either as an `integer` or a `tuple`.\n  The default is `None` in which case all frames are encoded.\\\n  To receive the frames iteratively (i.e. in a lazy manner), simply iterate over the `Fringes` instance.\n- `decode(I, verbose)`\\\n  [Decode](#decoding) the fringe pattern sequence `I`.\\\n  If either the argument `verbose` or the attribute with the same name is `True`,\n  additional infomation is computed and retuned: phase maps `φ`, residuals `r` and fringe orders `k`.\\\n  If the argument `denoise` is `True`, the unwrapped phase map is smoothened by a bilateral filter\n  which is edge-preserving.\\\n  If the argument `despike` is `True`, single pixel outliers in the unwrapped phase map\n  are replaced by their local neighborhood using a median filter.\n- `remap(registration, modulation)`\\\n  Mapping decoded, registered coordinates `ξ` (having sub-pixel accuracy)\n  from camera grid to (integer) positions on the pattern/screen grid\n  with weights from modulation `B`.\n  The default for `modulation` is `None`, in which case all weights are assumed to equal one.\n  The method yields a grid representing the screen (light source)\n  with the pixel values being a relative measure\n  of how much a screen (light source) pixel contributed\n  to the exposure of the camera sensor.\n- `deinterlace(I)`\\\n  Deinterlace a fringe pattern sequence `I` acquired with a line scan camera\n  while each frame has been displayed and captured\n  while the object has been moved by one pixel.\n\nThe next methods are class-methods:\n- `unwrap(phi)`\\\n  [Unwrap](#spatial-phase-unwrapping--spu-) the phase map `phi` i.e. `φ` spacially.\n\nThe next methods are package-methods:\n- `vshape(I)`\\\n  Transforms video data of arbitrary shape and dimensionality into the standardized shape `(T, Y, X, C)`, where\n  `T` is number of frames, `Y` is height, `X` is width, and `C` is number of color channels.\n  Ensures that the array becomes 4-dimensional and that the size of the last dimension,\n  i.e. the number of color channels <code>C &isin; {1; 3; 4}</code>. To do this, leading dimensions may be flattened.\n- `curvature(registration)`\\\n  Returns a curvature map. \n- `height(curvature)`\\\n  Local height map by local integration via an inverse laplace filter [[19]](#19).\\\n  Think of it as a relief, where height is only relative to the local neighborhood.\n\n## __Optimal Coding Strategy__\nAs makes sense intuitively, more sets `K` as well as more shifts `N` per set reduce the uncertainty `u` after decoding.\nA minimum of 3 shifts is needed to solve for the 3 unknowns brightness `A`, modulation `B` and coordinates `ξ`.\nAny additional 2 shifts compensate for one harmonic of the recorded fringe pattern.\nTherefore, higher accuracy can be achieved using more shifts `N`, but the time required to capture them \nsets a practical upper limit to the feasible number of shifts.\n\nGenerally, shorter wavelengths `l` (or equivalently more periods `v`) reduce the uncertainty `u`,\nbut the resolution of the camera and the display must resolve the fringe pattern spatially.\nHence, the used hardware imposes a lower bound for the wavelength (or upper bound for the number of periods).\n   \nAlso, small wavelengths might result in a smaller unambiguous measurement range `UMR`.\nIf two or more sets `K` are used and their wavelengths `l` resp. number of periods `v` are relative primes,\nthe unmbiguous measurement range can be increased many times.\nAs a consequence, one can use much smaller wavelenghts `l` (larger number of periods `v`).\n\n\nHowever, it must be assured that the unambiguous measurment range is always equal or larger than both,\nthe width `X` and the height `Y`.\nElse, [temporal phase unwrapping](#temporal-phase-unwrapping--tpu-) would yield wrong results and thus instead\n[spatial phase unwrapping](#spatial-phase-unwrapping--spu-) is used.\nBe aware that in the latter case only a relative phase map is obtained,\nwhich lacks the information of where exactly the camera sight rays were looking at during acquisition.\n\nTo simplify finding and setting the optimal parameters, the following methods can be used:\n- `setMTF()`: The optimal `vmax` is determined automativally [[18]](#18-bothe-2008)\nby measuring the **modulation transfer function** `MTF`.\\\n  Therefore, a sequence of exponentially increasing `v` is acquired:\n    1. Set `v` to `\'exponential\'`.\n    2. Encode, acquire and decode the fringe pattern sequence.\n    3. Call the function `setMTF(B)` with the argument `B` from decoding.\n- `v` can be set to `\'auto\'`. This automatically determines the optimal integer set of `v`\n  based on the maximal resolvable spatial frequency `vmax`.\n-  Equivalently, `l` can also be set to `\'auto\'`. This will automatically determine the optimal integer set of `l`\n  based on the minimal resolvable wavelength `lmin = L / vmax`.\n- `T` can be set directly, based on the desired acquisition time.\n  The optimal `K`, `N` and the [multiplexing](#multiplexing) methods will be determined automatically.\n\nAlternatively, simply use the function `auto()`\nto automatically set the optimal `v`, `T` and [multiplexing](#multiplexing) methods.\n\n## Troubleshooting\n<!---\n- __`poetry install` does not work__\n  \n  First, ensure that poetry is installed correctly as descibed onthe [Poetry Website](https://python-poetry.org/docs/).\\\n  Secondly, ensure the correct python version is installed on your system, as specified in the file `pyproject.toml`!\\\n  Thirdly, this can be caused by a proxy which `pip` does not handle correctly.\n  Manually setting the proxy in the Windows settings or even adding a system variable \n`https_proxy = http://YOUR_PROXY:PORT` can resolve this.\n--->\n\n- __Decoding takes a long time__\n  \n  This is probably related to the just-in-time compiler [Numba](https://numba.pydata.org/) \n  used for this computationally expensive function:\n  During the first execution, an initial compilation is executed. \n  This can take several tens of seconds up to single digit minutes, depending on your CPU.\n  However, for any subsequent execution, the compiled code is cached and the code of the function runs much faster, \n  approaching the speeds of code written in C.\n\n\n- __My decoded coordinates show lots of noise__\n  - Make sure the exposure of your camera is adjusted so that the fringe patterns show up with maximum contrast.\n    Try to avoid under- and overexposure during acquisition.\n  - Try using more, sets `K` and/or shifts `N`.\n  - Adjust the used wavelengths `l` resp. number of periods `v` to ensure the unamboguous measurement range\n    is larger than the pattern length, i.e. <code>UMR &ge; L</code>.\n  - If the decoded modulation is much lower than the decoded brightness,\n    try to use larger wavelengths `l` resp. smaller number of periods `v`.\\\n    If the decoded modulation remains low even with very large wavelengths (less than five periods per screen length),\n    and you are conducting a deflectometric mesurement, the surface under test is probably too rough.\n    Since deflectometry is for specular and glossy surfsces only, it isn\'t suited for scattering ones.\n    You should consider a different measurement technique, e.g. fringe projection.\n\n- __My decoded coordinates show systematic offsets__\n  - First, ensure that the correct frame was captured while acquiring the fringe pattern sequence.\n    If the timings are not set correctly, the sequence may be a frame off.\n  - Secondly, this might occur if either the camera or the display used have a gamma value very different from 1.\n    Typical screens have a gamma value of 2.2;   therefore compensate by setting the inverse value\n    <code>gamma<sup>-1</sup> = 1 / 2.2 &approx; 0.45</code> to the `gamma` attribute of the `Fringes` instance.\n    Alternatively, change the gamma value of the light source or camera directly.\n    You might also use more shifts `N` to compensate for the dominant harmonics of the gamma-nonlinearities.\n\n## References\n\n#### [11] [Burke 2002]\n[J. Burke, T. Bothe, W. Osten, and C. Hess,\n“Reverse engineering by fringe projection,”\nin Interferometry XI: Applications (W. Osten, ed.), vol. 4778, pp. 312–324, SPIE,\n2002.](https://doi.org/10.1117/12.473547)\n\n#### [1] [Burke 2022] \n[J. Burke, A. Pak, S. Höfer, M. Ziebarth, M. Roschani, J. Beyerer,\n"Deflectometry for specular surfaces: an overview",\narXiv:2204.11592v1 [physics.optics],\n2022.](https://arxiv.org/abs/2204.11592)\n\n#### [2] [Park2008]?\n\n#### [3] [Huang 1999]\n\n#### [4] [Liu 2014] [Liu2010] [Park2008]?\n\n#### [5] [Kludt 2018]\n\n#### [6] [Trumper 2016]\n\n#### [7] [Surrel 1997]\n\n#### [8] [EMVA1288]\n\n#### [9] [Bothe2008]\n\n#### [10] [Fischer]\n\n#### [13] [Burke 2012]\n[J. Burke,\n"Phase Decoding and Reconstruction",\nvol. Optical Methods for Solid Mechanics: A Full-Field Approach, ch. 3, pp. 83–141. Wiley, Weinheim,\n2012.](https://www.wiley.com/en-us/Optical+Methods+for+Solid+Mechanics%3A+A+Full+Field+Approach-p-9783527411115)\n\n#### [14] [Kludt 2024]\n\n#### [15] [Herráez 2002]\n[Miguel Arevallilo Herráaez, David R. Burton, Michael J. Lalor, and Munther A. Gdeisat.\nFast two-dimensional phase-unwrapping algorithm based on sorting by reliability following a noncontinuous path.\nAppl. Opt., 41(35):7437-7444,\nDec 2002.](https://opg.optica.org/ao/abstract.cfm?uri=ao-41-35-7437)\n\n#### [16] [Lei 2015]\n[Hai Lei, Xin yu Chang, Fei Wang, Xiao-Tang Hu, and Xiao-Dong Hu.\nA novel algorithm based on histogram processing of reliability for two-dimensional phase unwrapping.\nOptik - International Journal for Light and Electron Optics, 126(18):1640 - 1644,\n2015.](https://www.sciencedirect.com/science/article/abs/pii/S0030402615003228?via%3Dihub)\n\n#### [17] [Takeda]\n\n#### [18] [Bothe 2008]\n\n#### [19]\nInverse Laplace Filter\n\n## License\nCreative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License\n\n## Project Status\nThis package is in an early stage and under active development,\nso features and functionally will be added in the future.\nFeature requests are warmly welcomed!\n',
     'author': 'Christian Kludt',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/comimag/fringes',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fringes-0.1.5/PKG-INFO` & `fringes-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fringes
-Version: 0.1.5
+Version: 0.1.6
 Summary: Phase shifting algorithms for encoding and decoding sinusoidal fringe patterns.
 Home-page: https://github.com/comimag/fringes
 License: CC-BY-NC-SA-4.0
 Keywords: phase shifting,fringe analysis,fringe projection,deflectometry,computational imaging
 Author: Christian Kludt
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
@@ -14,35 +14,34 @@
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: opencv-contrib-python (>=4.7.0,<5.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Requires-Dist: si-prefix (>=1.2.2,<2.0.0)
 Requires-Dist: sympy (>=1.11.1,<2.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://github.com/comimag/fringes
 Description-Content-Type: text/markdown
 
 # Fringes
-
 Author: Christian Kludt
 
 [//]: # (![Parameter Interdependencies]&#40;docs/spirals.png&#41;)
+<img src="docs/du-bist-ein-wildschwein.gif">
 
 ## Description
 This package provides the handy `Fringes` class which handles all the required parameters
 for configuring fringe pattern sequences
 and provides methods for fringe analysis.
 <!---
 link to  paper, please cite
 --->
 
 ### Features
-<!---
-- Generalized Temporal Phase Unwrappting (GTPU)[[14](#14-kludt-2024)]
---->
+
 - Generalized Temporal Phase Unwrappting (GTPU)
 - Uncertainty Propagation
 - Optimal Coding Strategy
 - Deinterlacing
 - Multiplexing
 - Filtering Phase Maps
 - Remapping
@@ -158,47 +157,45 @@
 You can change the [logging level](https://docs.python.org/3/library/logging.html#levels) of a `Fringes` instance.
 Changing it to `'DEBUG'` gives you verbose feedback on which parameters are changed
 and how long functions take to execute.
 
 ```python
 f.logger.setLevel("DEBUG")
 ```
-<!---
+
 ## Graphical User Interface
-Do you need a GUI? `Fringes` has a sister project that is called `Fringes GUI`:
-https://pypi.org/project/fringes-gui/
---->
+Do you need a GUI? `Fringes` has a sister project that is called `Fringes-GUI`: https://pypi.org/project/fringes-gui/
+
 ## Attributes
 All parameters are parsed when setting, so usually several input formats are accepted, e.g.
 `bool`, `int`, `float`, `str` for scalars and additionally `list`, `tuple`, `ndarray` for arrays.
 
 Note that parameters might have circular dependencies which are resolved automatically,
-hence dependent parameters might change as well. 
-The attributes in rectangular boxes are readonly, i.e. they are inferred from the others.
-Only the ones in white boxes will never influence others.
+hence dependent parameters might change as well.
 
 ![Parameter Interdependencies](docs/interdependencies.svg)\
 Parameter and their Interdependencies.
 
 ### __Video Shape__
 Standardized `shape` `(T, Y, X, C)` of fringe pattern sequence, with
 - `T`: number of frames
 - `Y`: height
 - `X`: width
 - `C`: number of color channels
 
 `T` depends on the paremeters `H`, `D`, `K`, `N` and the [multiplexing](#multiplexing) methods:\
 If all `N` are identical, then `T = H * D * K * N` with `N` as a scalar,
 else <code>T = H * &sum; N<sub>i</sub></code> with `N` as an array.\
-If a [multiplexing](#multiplexing) methods is activated, `T` reduces further.
-
-The length `L` is the maximum of `X` and `Y`.
+If a [multiplexing](#multiplexing) method is activated, `T` reduces further.
 
 `C` depends on the [coloring](#coloring-and-averaging) and [multiplexing](#multiplexing) methods.
 
+The length `L` is the maximum of `X` and `Y` and denotes the length in [px] to be ancoded.\
+It can be extended by the factor `alpha`.
+
 `size` is the product of `shape`.
 
 ### __Coordinate System__
 The following coordinate systems can be used by setting `grid` to:
 - `'image'`: The top left corner pixel of the grid is the origin (0, 0)
 and positive directions are right- resp. downwards.
 - `'Cartesian'`: The center of grid is the origin (0, 0) and positive directions are right- resp. upwards.
@@ -234,24 +231,14 @@
 Usually `f = 1` and is essentially only changed if [frequency division multiplexing](#multiplexing) `FDM` is activated.
 
 `reverse` is a boolean which reverses the direction of the shifts (by multiplying `f` with `-1`).
 
 `o` denotes the phase offset `φ₀` which can be used to
 e.g. let the fringe patterns start (at the origin) with a gray value of zero.
 
-`UMR` denotes the unambiguous measurement range.
-The coding is only unique in the interval `[0, UMR)`; after that it repeats itself.
-The `UMR` is derived from `l` and `v`:
-- If <code>l &isin; &#8469;</code>, <code>UMR = lcm(l<sub>i</sub>)</code> with `lcm` being the least common multiple.
-- Else, if <code>v &isin; &#8469;</code>,
-  <code>UMR = `L`/ gcd(v<sub>i</sub>)</code> with `gcd` being the greatest common divisor.
-- Else, if <code>l &and; v &isin; &#8474;</code>, `lcm` resp. `gdc` are extended to rational numbers.
-- Else, if <code>l &and; v &isin; &#8477; \ &#8474;</code>, `l` and `v` are approximated by rational numbers
-  with a fixed length of decimal digits.
-
 ### __Coloring and Averaging__
 The fringe pattern sequence `I` can be colorized by setting the hue `h` to any RGB color tuple
 in the interval `[0, 255]`. However, black `(0, 0, 0)` is not allowed. `h` must be in shape `(H, 3)`:\
 `H` is the number of hues and can be set directly; 3 is the length of the RGB color tuple.\
 The hues `h` can also be set by assigning any combination of the following characters as a string:
 - `'r'`: red
 - `'g'`: green
@@ -290,15 +277,15 @@
   If one wants a static pattern, i.e. one that remains congruent when shifted, set `static` to `True`.
 
 `SDM` and `WDM` can be used together [[6]](#6) (reducing `T` by a factor of 2 * 3 = 6), `FDM` with neighter.
 
 By default, the aforementioned multiplexing methods are deactivated,
 so we then only have `TDM`: Time Divison Multiplexing.
 
-### __Data Type__
+### __Values__
 `dtype` denotes the data type of the fringe pattern sequence `I`.\
 Possible values are:
 - `'bool'`
 - `'uint8'` (the default)
 - `'uint16'`
 - `'float32'`
 - `'float64'`
@@ -311,15 +298,18 @@
 `Imax` in turn limits the offset `A` and the amplitude `B`.
 The fringe visibility (also called fringe contrast) is `V = A / B` with <code>V &isin; [0, 1]</code>.
 
 The quantization step size `q` is also derived from `dtype`:
 `q = 1` for `bool` and `Q`-bit `unsigned integers`, 
 and for `float` its corresponding [resolution](https://numpy.org/doc/stable/reference/generated/numpy.finfo.html).
 
-The standard deviation of the quantization noise  is <code>QN = q / &radic; 12</code>.
+The standard deviation of the quantization noise  is <code>quant = q / &radic; 12</code>.
+
+`gamma` denotes the gamma correction factor and can be used to compensate for nonlinearities
+of the display response curve.
 
 ### Unwrapping
 - `PU` denotes the phase unwrapping method and is eihter `'none'`, `'temporal'`, `'spatial'` or `'SSB'`.
 See [spatial demodulation](#spatial-demodulation--phase-unwrapping--pu-) for more details.
 - `mode` denotes the mode used for [temporal phase unwrapping](#temporal-phase-unwrapping--tpu-).
   Choose either `'fast'` (the default) or `'precise'`.
 - `Vmin` denotes the minimal fringe visibility (fringe contrast) required for the measurement to be valid
@@ -327,39 +317,49 @@
 - `verbose` can be set to `True` to also receive the wrapped phase map `φ`,
 the fringe orders `k` and the residuals `r` from decoding.
 - `SSB` denotes **Single Sideband Demodulation** [[17]](#17-takeda) and is deployed
 if <code>K &equiv; H &equiv; N &equiv; 1</code>, i.e. <code>T &equiv; 1</code>
 and the [coordinate system](#coordinate-system) is eighter `'image'` or `'Cartesian'`.
 
 ### __Quality Metrics__
+`UMR` denotes the unambiguous measurement range.
+The coding is only unique in the interval `[0, UMR)`; after that it repeats itself.
+The `UMR` is derived from `l` and `v`:
+- If <code>l &isin; &#8469;</code>, <code>UMR = lcm(l<sub>i</sub>)</code> with `lcm` being the least common multiple.
+- Else, if <code>v &isin; &#8469;</code>,
+  <code>UMR = `L`/ gcd(v<sub>i</sub>)</code> with `gcd` being the greatest common divisor.
+- Else, if <code>l &and; v &isin; &#8474;</code>, `lcm` resp. `gdc` are extended to rational numbers.
+- Else, if <code>l &and; v &isin; &#8477; \ &#8474;</code>, `l` and `v` are approximated by rational numbers
+  with a fixed length of decimal digits.
+
 `eta` denotes the coding efficiency `L / UMR`. It makes no sense to choose `UMR` much larger than `L`,
 because then a significant part of the coding range is not used.
 
 `u` denotes the minimum possible uncertainty of the measurement in pixels.
 It is based on the phase noise model from [[7]](#7),
 propagated through [generalized temporal phase unwrapping](#temporal-phase-unwrapping--tpu-) and converted from phase to pixel units.
 It is influenced by the fringe parameters
 - `M`: number of [averaged](#coloring-and-averaging) intensity samples
 - `N`: number of phase shifts
 - `l`: wavelengths of the fringes
 - `B`: measured amplitude
 
 and the measurement hardware-specific noise sources [[8]](#8), [[9]](#9)
-- `dark`: dark noise of the used camera
 - `shot`: photon noise of light itself
 - `quant`: quantization noise of the light source or camera
+- `dark`: dark noise of the used camera
 
-The maximum possible dynamic range of the measurement is `DR = L / u`.
-It describes how many points can be discriminated on the interval `[0, L)`.
+The maximum possible dynamic range of the measurement is `DR = UMR / u`.
+It describes how many points can be discriminated on the interval `[0, UMR)`.
 It remains constant if `L` and hence `l` are scaled (the scaling factor cancels out).
 
 ## Methods
 - `load(fname)`\
   Load a parameter set from the file `fname` to a `Fringes` instance.
-  Supported file formats are `.json`, `.yaml` and `.asdf`.
+  Supported file formats are `*.json`, `*.yaml` and `*.asdf`.
 - `save(fname)`\
   Save the parameter set of the current `Fringes` instance to the file `fname`.
   If `fname` is not provided, the default is `params.yaml` within the package's directory 'fringes'.
 - `reset()`\
   Reset the parameter set of the current `Fringes` instance to the default values.
 - `auto(T)`\
   Automatically set the [optimal parameters](#optimal-coding-strategy) based on the argument `T` (number of frames).
@@ -381,15 +381,15 @@
   If either the argument `verbose` or the attribute with the same name is `True`,
   additional infomation is computed and retuned: phase maps `φ`, residuals `r` and fringe orders `k`.\
   If the argument `denoise` is `True`, the unwrapped phase map is smoothened by a bilateral filter
   which is edge-preserving.\
   If the argument `despike` is `True`, single pixel outliers in the unwrapped phase map
   are replaced by their local neighborhood using a median filter.
 - `remap(registration, modulation)`\
-  Mapping decoded registered coordinates `ξ` (having sub-pixel accuracy)
+  Mapping decoded, registered coordinates `ξ` (having sub-pixel accuracy)
   from camera grid to (integer) positions on the pattern/screen grid
   with weights from modulation `B`.
   The default for `modulation` is `None`, in which case all weights are assumed to equal one.
   The method yields a grid representing the screen (light source)
   with the pixel values being a relative measure
   of how much a screen (light source) pixel contributed
   to the exposure of the camera sensor.
@@ -408,15 +408,15 @@
   `T` is number of frames, `Y` is height, `X` is width, and `C` is number of color channels.
   Ensures that the array becomes 4-dimensional and that the size of the last dimension,
   i.e. the number of color channels <code>C &isin; {1; 3; 4}</code>. To do this, leading dimensions may be flattened.
 - `curvature(registration)`\
   Returns a curvature map. 
 - `height(curvature)`\
   Local height map by local integration via an inverse laplace filter [[19]](#19).\
-  Think of it as a relief, where height is only relative to the local neighborhood.`
+  Think of it as a relief, where height is only relative to the local neighborhood.
 
 ## __Optimal Coding Strategy__
 As makes sense intuitively, more sets `K` as well as more shifts `N` per set reduce the uncertainty `u` after decoding.
 A minimum of 3 shifts is needed to solve for the 3 unknowns brightness `A`, modulation `B` and coordinates `ξ`.
 Any additional 2 shifts compensate for one harmonic of the recorded fringe pattern.
 Therefore, higher accuracy can be achieved using more shifts `N`, but the time required to capture them 
 sets a practical upper limit to the feasible number of shifts.
@@ -425,14 +425,16 @@
 but the resolution of the camera and the display must resolve the fringe pattern spatially.
 Hence, the used hardware imposes a lower bound for the wavelength (or upper bound for the number of periods).
    
 Also, small wavelengths might result in a smaller unambiguous measurement range `UMR`.
 If two or more sets `K` are used and their wavelengths `l` resp. number of periods `v` are relative primes,
 the unmbiguous measurement range can be increased many times.
 As a consequence, one can use much smaller wavelenghts `l` (larger number of periods `v`).
+
+
 However, it must be assured that the unambiguous measurment range is always equal or larger than both,
 the width `X` and the height `Y`.
 Else, [temporal phase unwrapping](#temporal-phase-unwrapping--tpu-) would yield wrong results and thus instead
 [spatial phase unwrapping](#spatial-phase-unwrapping--spu-) is used.
 Be aware that in the latter case only a relative phase map is obtained,
 which lacks the information of where exactly the camera sight rays were looking at during acquisition.
 
@@ -471,28 +473,34 @@
   During the first execution, an initial compilation is executed. 
   This can take several tens of seconds up to single digit minutes, depending on your CPU.
   However, for any subsequent execution, the compiled code is cached and the code of the function runs much faster, 
   approaching the speeds of code written in C.
 
 
 - __My decoded coordinates show lots of noise__
-
-  Try using more, sets `K` and/or shifts `N` and adjust the used wavelengths `l` resp. number of periods `v`.\
-  Also, make sure the exposure of your camera is adjusted so that the fringe patterns show up with maximum contrast.\
-  Try to avoid under- and overexposure during acquisition.
-
-
-- #### My decoded coordinates show systematic offsets
-  First, ensure that the correct frame was captured while acquiring the fringe pattern sequence.
-  If the timings are not set correctly, the sequence may be a frame off.\
-  Secondly, this might occur if either the camera or the display used have a gamma value very different from 1.
-  Typical screens have a gamma value of 2.2;   therefore compensate by setting the inverse value
-  <code>gamma<sup>-1</sup> = 1 / 2.2 &approx; 0.45</code> to the `gamma` attribute of the `Fringes` instance.
-  Alternatively, change the gamma value of the light source or camera directly.
-  You might also use more shifts `N` to compensate for the dominant harmonics of the gamma-nonlinearities.
+  - Make sure the exposure of your camera is adjusted so that the fringe patterns show up with maximum contrast.
+    Try to avoid under- and overexposure during acquisition.
+  - Try using more, sets `K` and/or shifts `N`.
+  - Adjust the used wavelengths `l` resp. number of periods `v` to ensure the unamboguous measurement range
+    is larger than the pattern length, i.e. <code>UMR &ge; L</code>.
+  - If the decoded modulation is much lower than the decoded brightness,
+    try to use larger wavelengths `l` resp. smaller number of periods `v`.\
+    If the decoded modulation remains low even with very large wavelengths (less than five periods per screen length),
+    and you are conducting a deflectometric mesurement, the surface under test is probably too rough.
+    Since deflectometry is for specular and glossy surfsces only, it isn't suited for scattering ones.
+    You should consider a different measurement technique, e.g. fringe projection.
+
+- __My decoded coordinates show systematic offsets__
+  - First, ensure that the correct frame was captured while acquiring the fringe pattern sequence.
+    If the timings are not set correctly, the sequence may be a frame off.
+  - Secondly, this might occur if either the camera or the display used have a gamma value very different from 1.
+    Typical screens have a gamma value of 2.2;   therefore compensate by setting the inverse value
+    <code>gamma<sup>-1</sup> = 1 / 2.2 &approx; 0.45</code> to the `gamma` attribute of the `Fringes` instance.
+    Alternatively, change the gamma value of the light source or camera directly.
+    You might also use more shifts `N` to compensate for the dominant harmonics of the gamma-nonlinearities.
 
 ## References
 
 #### [11] [Burke 2002]
 [J. Burke, T. Bothe, W. Osten, and C. Hess,
 “Reverse engineering by fringe projection,”
 in Interferometry XI: Applications (W. Osten, ed.), vol. 4778, pp. 312–324, SPIE,
@@ -552,7 +560,8 @@
 ## License
 Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License
 
 ## Project Status
 This package is in an early stage and under active development,
 so features and functionally will be added in the future.
 Feature requests are warmly welcomed!
+
```

