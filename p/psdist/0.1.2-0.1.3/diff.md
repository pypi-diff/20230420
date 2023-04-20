# Comparing `tmp/psdist-0.1.2.tar.gz` & `tmp/psdist-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdist-0.1.2.tar", last modified: Mon Mar  6 16:33:39 2023, max compression
+gzip compressed data, was "psdist-0.1.3.tar", last modified: Thu Apr 20 17:37:57 2023, max compression
```

## Comparing `psdist-0.1.2.tar` & `psdist-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-03-06 16:33:39.187680 psdist-0.1.2/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1070 2022-11-29 16:42:20.000000 psdist-0.1.2/LICENSE
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1919 2023-03-06 16:33:39.187537 psdist-0.1.2/PKG-INFO
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1461 2023-01-20 00:19:35.000000 psdist-0.1.2/README.md
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-03-06 16:33:39.184685 psdist-0.1.2/psdist/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       95 2023-03-02 16:46:32.000000 psdist-0.1.2/psdist/__init__.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4925 2023-01-17 23:20:27.000000 psdist-0.1.2/psdist/ap.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    12559 2023-03-02 16:46:32.000000 psdist-0.1.2/psdist/cloud.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1247 2023-01-17 19:53:50.000000 psdist-0.1.2/psdist/data.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    17797 2023-01-18 14:35:27.000000 psdist-0.1.2/psdist/image.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1344 2023-03-02 16:46:32.000000 psdist-0.1.2/psdist/utils.py
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-03-06 16:33:39.187323 psdist-0.1.2/psdist/visualization/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      156 2023-03-02 16:46:32.000000 psdist-0.1.2/psdist/visualization/__init__.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    14884 2023-03-02 16:46:32.000000 psdist-0.1.2/psdist/visualization/cloud.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    32457 2023-03-02 16:46:32.000000 psdist-0.1.2/psdist/visualization/grid.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    22274 2023-03-02 16:46:32.000000 psdist-0.1.2/psdist/visualization/image.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4152 2023-03-02 16:46:32.000000 psdist-0.1.2/psdist/visualization/visualization.py
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-03-06 16:33:39.185602 psdist-0.1.2/psdist.egg-info/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1919 2023-03-06 16:33:39.000000 psdist-0.1.2/psdist.egg-info/PKG-INFO
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      436 2023-03-06 16:33:39.000000 psdist-0.1.2/psdist.egg-info/SOURCES.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        1 2023-03-06 16:33:39.000000 psdist-0.1.2/psdist.egg-info/dependency_links.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      110 2023-03-06 16:33:39.000000 psdist-0.1.2/psdist.egg-info/requires.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        7 2023-03-06 16:33:39.000000 psdist-0.1.2/psdist.egg-info/top_level.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      716 2023-03-06 16:30:50.000000 psdist-0.1.2/pyproject.toml
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       38 2023-03-06 16:33:39.187734 psdist-0.1.2/setup.cfg
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-04-20 17:37:57.390984 psdist-0.1.3/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1070 2022-11-29 16:42:20.000000 psdist-0.1.3/LICENSE
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1160 2023-04-20 17:37:57.390861 psdist-0.1.3/PKG-INFO
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      702 2023-03-07 19:34:27.000000 psdist-0.1.3/README.md
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-04-20 17:37:57.389092 psdist-0.1.3/psdist/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       95 2023-03-02 16:46:32.000000 psdist-0.1.3/psdist/__init__.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4925 2023-01-17 23:20:27.000000 psdist-0.1.3/psdist/ap.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    12559 2023-04-20 15:24:28.000000 psdist-0.1.3/psdist/cloud.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1247 2023-01-17 19:53:50.000000 psdist-0.1.3/psdist/data.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    17797 2023-04-19 23:33:18.000000 psdist-0.1.3/psdist/image.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1344 2023-03-02 16:46:32.000000 psdist-0.1.3/psdist/utils.py
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-04-20 17:37:57.390707 psdist-0.1.3/psdist/visualization/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      156 2023-03-02 16:46:32.000000 psdist-0.1.3/psdist/visualization/__init__.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    14884 2023-03-02 16:46:32.000000 psdist-0.1.3/psdist/visualization/cloud.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    36292 2023-04-20 17:16:20.000000 psdist-0.1.3/psdist/visualization/grid.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    22274 2023-03-02 16:46:32.000000 psdist-0.1.3/psdist/visualization/image.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4152 2023-03-02 16:46:32.000000 psdist-0.1.3/psdist/visualization/visualization.py
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-04-20 17:37:57.389774 psdist-0.1.3/psdist.egg-info/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1160 2023-04-20 17:37:57.000000 psdist-0.1.3/psdist.egg-info/PKG-INFO
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      436 2023-04-20 17:37:57.000000 psdist-0.1.3/psdist.egg-info/SOURCES.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        1 2023-04-20 17:37:57.000000 psdist-0.1.3/psdist.egg-info/dependency_links.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      110 2023-04-20 17:37:57.000000 psdist-0.1.3/psdist.egg-info/requires.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        7 2023-04-20 17:37:57.000000 psdist-0.1.3/psdist.egg-info/top_level.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      716 2023-04-20 17:36:13.000000 psdist-0.1.3/pyproject.toml
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       38 2023-04-20 17:37:57.391022 psdist-0.1.3/setup.cfg
```

### Comparing `psdist-0.1.2/LICENSE` & `psdist-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psdist-0.1.2/psdist/ap.py` & `psdist-0.1.3/psdist/ap.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.2/psdist/cloud.py` & `psdist-0.1.3/psdist/cloud.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.2/psdist/data.py` & `psdist-0.1.3/psdist/data.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.2/psdist/image.py` & `psdist-0.1.3/psdist/image.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.2/psdist/utils.py` & `psdist-0.1.3/psdist/utils.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.2/psdist/visualization/cloud.py` & `psdist-0.1.3/psdist/visualization/cloud.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.2/psdist/visualization/grid.py` & `psdist-0.1.3/psdist/visualization/grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,15 +131,16 @@
                 flipxy=bool(axis),
                 **marg_kws,
             )
         return _out
 
     def colorbar(self, mappable, **kws):
         """Add a colorbar."""
-        kws.setdefault(loc="r", pad=2.0)
+        kws.setdefault("loc", "r")
+        kws.setdefault("pad", 2.0)
         self.fig.colorbar(mappable, **kws)
 
 
 class CornerGrid:
     """Grid for corner plots.
 
     * https://seaborn.pydata.org/generated/seaborn.PairGrid.html
@@ -156,71 +157,92 @@
         The axes for diagonal (univariate) subplots. Can be empty.
     offdiag_axs : list[proplot.gridspec.SubplotGrid]
         The axes for off-diagonal (bivariate) subplots.
     diag_indices : list[int]
         The index of the dimension plotted on each diagonal subplot.
     offdiag_indices : list[2-tuple of int]
         Indices of the dimensions plotted on each off-diagonal subplot.
-
-    Parameters
-    ----------
-    n : int
-        The number of rows/columns.
-    diag : bool
-        Whether to include diagonal subplots (univariate plots). If False,
-        we have an (n - 1) x (n - 1) grid instead of an n x n grid.
-    diag_height_frac : float
-        This reduces the height of the diagonal plots relative to the ax
-        height.
-    limits : list[tuple], length n
-        The (min, max) for each dimension. (These can be set later.)
-    labels : list[str]
-        The label for each dimension. (These can be set later.)
-    **fig_kws
-        Key word arguments passed to `pplt.subplots()`.
     """
-
+    
     def __init__(
-        self, n=4, diag=True, diag_height_frac=0.65, limits=None, labels=None, **fig_kws
+        self, 
+        n=4, 
+        diag=True, 
+        diag_norm="max",
+        diag_scale=0.65,
+        diag_rspine=False,
+        limits=None, 
+        labels=None, 
+        corner=True,
+        **fig_kws
     ):
+        """
+        Parameters
+        ----------
+        n : int
+            The number of rows/columns.
+        diag : bool
+            Whether to include diagonal subplots (univariate plots). If False,
+            we have an (n - 1) x (n - 1) grid instead of an n x n grid.
+        diag_norm : {"max", "area"}
+            Normalize 1D histograms max value or the area under the curve.
+        diag_scale : float
+            Scale the 1D histograms by this value.
+        diag_rspine : bool
+            Whether to include right spine on diagonal subplots (if `corner`).
+        limits : list[tuple], length n
+            The (min, max) for each dimension. (These can be set later.)
+        labels : list[str]
+            The label for each dimension. (These can be set later.)
+        corner : bool
+            Whether to hide the upper-triangular subplots.
+        **fig_kws
+            Key word arguments passed to `pplt.subplots()`.
+        """
         # Create figure.
         self.new = True
         self.n = n
+        self.corner = corner
         self.diag = diag
-        self.diag_height_frac = diag_height_frac
-        self.start = int(self.diag)
+        self.diag_norm = diag_norm
+        self.diag_scale = diag_scale
+        self.diag_rspine = diag_rspine
         self.nrows = self.ncols = self.n
         if not self.diag:
             self.nrows = self.nrows - 1
             self.ncols = self.ncols - 1
         self.fig_kws = fig_kws
         self.fig_kws.setdefault("figwidth", 1.5 * self.nrows)
         self.fig_kws.setdefault("aligny", True)
         self.fig, self.axs = pplt.subplots(
             nrows=self.nrows,
             ncols=self.ncols,
-            sharex=1,
-            sharey=1,
             spanx=False,
             spany=False,
+            sharex=False,
+            sharey=False,
             **self.fig_kws,
         )
         # Collect diagonal/off-diagonal subplots and indices.
         self.diag_axs = []
         self.offdiag_axs = []
+        self.offdiag_axs_u = []
         self.diag_indices = []
         self.offdiag_indices = []
+        self.offdiag_indices_u = []
         if self.diag:
             for i in range(self.n):
                 self.diag_axs.append(self.axs[i, i])
                 self.diag_indices.append(i)
             for i in range(1, self.n):
                 for j in range(i):
                     self.offdiag_axs.append(self.axs[i, j])
+                    self.offdiag_axs_u.append(self.axs[j, i])
                     self.offdiag_indices.append((j, i))
+                    self.offdiag_indices_u.append((i, j))
         else:
             for i in range(self.n - 1):
                 for j in range(i + 1):
                     self.offdiag_axs.append(self.axs[i, j])
                     self.offdiag_indices.append((j, i + 1))
 
         # Set limits and labels.
@@ -228,51 +250,72 @@
         if limits is not None:
             self.set_limits(limits)
         self.labels = labels
         if labels is not None:
             self.set_labels(labels)
 
         # Formatting
+        if self.corner or not self.diag:
+            for i in range(self.nrows):
+                for j in range(self.ncols):
+                    if j > i:
+                        self.axs[i, j].axis("off")   
+        self.axs[:-1, :].format(xticklabels=[])
         for i in range(self.nrows):
             for j in range(self.ncols):
-                if j > i:
-                    self.axs[i, j].axis("off")
-        for i in range(self.nrows):
-            self.axs[:-1, i].format(xticklabels=[])
-            self.axs[i, 1:].format(yticklabels=[])
-        for ax in self.axs:
-            ax.format(xspineloc="bottom", yspineloc="left")
-        for ax in self.diag_axs:
-            ax.format(yspineloc="neither")
-        self.axs.format(
-            xtickminor=True, ytickminor=True, xlocator=("maxn", 3), ylocator=("maxn", 3)
-        )
-        self.set_limits(limits)
+                ax = self.axs[i, j]
+                if i != self.nrows - 1:
+                    ax.format(xticklabels=[])
+                if j != 0:
+                    if not (i == j and self.diag_rspine and self.corner and self.diag):                
+                        ax.format(yticklabels=[])
+        self.axs.format(xspineloc="bottom", yspineloc="left")
+        if self.corner:
+            if self.diag_rspine:
+                self.format_diag(yspineloc="right")
+            else:
+                self.format_diag(yspineloc="neither")
+        self.format_diag(ylim=(0.0, 1.0))
+        self.axs.format(xtickminor=True, ytickminor=True, xlocator=("maxn", 3), ylocator=("maxn", 3))
+            
+    def format_offdiag(self, **kws):
+        """Format off-diagonal subplots."""
+        for ax in [self.offdiag_axs + self.offdiag_axs_u]:
+            ax.format(**kws)
+            
+    def format_diag(self, **kws):
+        """Format diagonal subplots."""
         for ax in self.diag_axs:
-            ax.format(ylim=(0.0, 1.01))
+            ax.format(**kws)
+        if not self.corner:
+            for ax in self.diag_axs[1:]:
+                ax.format(yticklabels=[])
+        self._fake_diag_yticks()
 
     def get_labels(self):
-        """Return the n plot labels."""
+        """Return the dimension labels."""
         if self.diag:
             labels = [ax.get_xlabel() for ax in self.diag_axs]
         else:
             labels = [self.axs[-1, i].get_xlabel() for i in range(self.n - 1)]
             labels = labels + [self.axs[-1, 0].get_ylabel()]
         return labels
 
     def set_labels(self, labels):
-        """Set the n plot labels."""
+        """Set the dimension labels."""
         for ax, label in zip(self.axs[-1, :], labels):
             ax.format(xlabel=label)
-        for ax, label in zip(self.axs[self.start :, 0], labels[1:]):
+        for ax, label in zip(self.axs[int(self.diag):, 0], labels[1:]):
             ax.format(ylabel=label)
+        if self.diag and not self.corner:
+            self.axs[0, 0].format(ylabel=labels[0])
         self.labels = labels
 
     def get_limits(self):
-        """Return the n plot limits. (min, max)"""
+        """Return the plot limits."""
         if self.diag:
             limits = [ax.get_xlim() for ax in self.diag_axs]
         else:
             limits = [self.axs[-1, i].get_xlim() for i in range(self.n - 1)]
             limits = limits + [self.axs[-1, 0].get_ylim()]
         return limits
 
@@ -290,25 +333,62 @@
         if limits is not None:
             if expand:
                 limits = np.array(limits)
                 limits_old = np.array(self.get_limits())
                 mins = np.minimum(limits[:, 0], limits_old[:, 0])
                 maxs = np.maximum(limits[:, 1], limits_old[:, 1])
                 limits = list(zip(mins, maxs))
-            for i in range(self.axs.shape[1]):
+            for (i, j), ax in zip(self.offdiag_indices, self.offdiag_axs):
+                ax.format(ylim=limits[j])
+            for i in range(self.ncols):
                 self.axs[:, i].format(xlim=limits[i])
-            for i, lim in enumerate(limits[1:], start=self.start):
-                self.axs[i, : (i + 1 - self.start)].format(ylim=lim)
         self.limits = self.get_limits()
+        
+    def _fake_diag_yticks(self):
+        """The yticks on the (0, 0) subplot correspond to the other subplots in the row.
+        
+        Source: pandas.plotting.scatterplot_matrix.
+        """
+        if self.corner or not self.diag:
+            return
+        limits = self.limits
+        if limits is None:
+            limits = self.get_limits()
+            
+        lim1 = limits[0]
+        locs = self.axs[0, 0].xaxis.get_majorticklocs()
+        locs = locs[(lim1[0] <= locs) & (locs <= lim1[1])]
+        adj = (locs - lim1[0]) / (lim1[1] - lim1[0])
+
+        lim0 = self.axs[0, 0].get_ylim()
+        adj = adj * (lim0[1] - lim0[0]) + lim0[0]
+        self.axs[0, 0].yaxis.set_ticks(adj)
+
+        if np.all(locs == locs.astype(int)):
+            locs = locs.astype(int)
+        self.axs[0, 0].yaxis.set_ticklabels(locs)
+        
+    def plot_diag(self, x, y, axis=0, **kws):
+        """Plot data on diagonal subplot. The plot is assumed to represent
+        a probability density, so is normalized by area."""
+        if self.diag_norm == "max":
+            y = y / np.max(y)
+        elif self.diag_norm == "area":
+            dx = np.abs(np.diff(x)[0])
+            y = y / (np.sum(y) * dx)
+        y = y * self.diag_scale
+        return plot1d(x, y, ax=self.diag_axs[axis], **kws)
 
     def plot_image(
         self,
         f,
         coords=None,
         prof_edge_only=False,
+        lower=True,
+        upper=True,
         update_limits=True,
         diag_kws=None,
         **kws,
     ):
         """Plot an n-dimensional image.
 
         Parameters
@@ -316,14 +396,16 @@
         f : ndarray
             An n-dimensional image.
         coords : list[ndarray]
             Coordinates along each axis of the grid (if `data` is an image).
         prof_edge_only : bool
             If plotting profiles on top of images (on off-diagonal subplots), whether
             to plot x profiles only in bottom row and y profiles only in left column.
+        lower, upper, bool
+            Whether to plot on the lower or upper triangular subplots (or both).
         update_limits : bool
             Whether to extend the existing plot limits.
         diag_kws : dict
             Key word argument passed to `visualization.plot1d`.
         **kws
             Key word arguments pass to `visualization.image.plot2d`
         """
@@ -344,38 +426,46 @@
             limits = [(np.min(e), np.max(e)) for e in edges]
             self.set_limits(limits, expand=(not self.new))
         self.new = False
 
         # Univariate plots.
         for ax, axis in zip(self.diag_axs, self.diag_indices):
             profile = psdist.image.project(f, axis=axis)
-            profile = profile / np.max(profile)
-            profile = profile * self.diag_height_frac
-            plot1d(coords[axis], profile, ax=ax, **diag_kws)
+            self.plot_diag(coords[axis], profile, axis=axis, **diag_kws)
 
         # Bivariate plots.
         profx, profy = [kws.pop(key) for key in ("profx", "profy")]
-        for ax, axis in zip(self.offdiag_axs, self.offdiag_indices):
-            if prof_edge_only:
-                if profx:
-                    kws["profx"] = axis[1] == self.n - 1
-                if profy:
-                    kws["profy"] = axis[0] == 0
-            _f = psdist.image.project(f, axis=axis)
-            _f = _f / np.max(_f)
-            _coords = [coords[i] for i in axis]
-            vis_image.plot2d(_f, coords=_coords, ax=ax, **kws)
+        if lower:
+            for ax, axis in zip(self.offdiag_axs, self.offdiag_indices):
+                if prof_edge_only:
+                    if profx:
+                        kws["profx"] = axis[1] == self.n - 1
+                    if profy:
+                        kws["profy"] = axis[0] == 0
+                _f = psdist.image.project(f, axis=axis)
+                _f = _f / np.max(_f)
+                _coords = [coords[k] for k in axis]
+                vis_image.plot2d(_f, coords=_coords, ax=ax, **kws)
+        if not self.corner and upper:
+            for ax, axis in zip(self.offdiag_axs_u, self.offdiag_indices_u):
+                _f = psdist.image.project(f, axis=axis)
+                _f = _f / np.max(_f)
+                _coords = [coords[k] for k in axis]
+                vis_image.plot2d(_f, coords=_coords, ax=ax, **kws)
+        self._fake_diag_yticks()
             
     def plot_cloud(
         self,
         X,
         limits=None,
         bins="auto",
         autolim_kws=None,
         prof_edge_only=False,
+        lower=True,
+        upper=True,
         update_limits=True,
         diag_kws=None,
         **kws,
     ):
         """Plot an n-dimensional point cloud.
 
         Parameters
@@ -388,14 +478,16 @@
             The number of bins along each dimension (if plot type requires histogram
             computation). If int or 'auto', applies to all dimensions. Currently
             the histogram is computed with limits based on the data min/max, not
             the plot limits.
         prof_edge_only : bool
             If plotting profiles on top of images (on off-diagonal subplots), whether
             to plot x profiles only in bottom row and y profiles only in left column.
+        lower, upper, bool
+            Whether to plot on the lower or upper triangular subplots (or both).
         update_limits : bool
             Whether to extend the existing plot limits.
         diag_kws : dict
             Key word argument passed to `visualization.plot1d`.
         **kws
             Key word arguments pass to `visualization.cloud.plot2d`
         """
@@ -414,45 +506,50 @@
                 autolim_kws = dict()
             autolim_kws.setdefault("pad", 0.1)
             limits = vis_cloud.auto_limits(X, **autolim_kws)
         if update_limits:
             self.set_limits(limits, expand=(not self.new))
         limits = self.get_limits()
         self.new = False
-
+        
         if not psdist.utils.array_like(bins):
             bins = n * [bins]
 
         # Univariate plots. Remember histogram bins and use them for 2D histograms.
         edges = []
-        for ax, axis in zip(self.diag_axs, self.diag_indices):
+        for axis in range(self.n):
             if psdist.utils.array_like(bins[axis]):
                 _edges = bins[axis]
             else:
                 _edges = np.histogram_bin_edges(X[:, axis], bins[axis], limits[axis])
             edges.append(_edges)
-            
-            heights, _ = np.histogram(X[:, axis], _edges)
-            heights = heights / np.max(heights)
-            heights = heights * self.diag_height_frac
-            centers = psdist.utils.centers_from_edges(_edges)
-            plot1d(centers, heights, ax=ax, **diag_kws)
+            if self.diag:
+                heights, _ = np.histogram(X[:, axis], _edges)
+                centers = psdist.utils.centers_from_edges(_edges)
+                self.plot_diag(centers, heights, axis=axis, **diag_kws)
 
         # Bivariate plots:
         profx, profy = [kws.pop(key) for key in ("profx", "profy")]
-        for ax, axis in zip(self.offdiag_axs, self.offdiag_indices):
-            if prof_edge_only:
-                if profx:
-                    kws["profx"] = axis[1] == self.n - 1
-                if profy:
-                    kws["profy"] = axis[0] == 0
-            if kws["kind"] in ["hist", "contour", "contourf"]:
-                kws["bins"] = [edges[axis[0]], edges[axis[1]]]
-            vis_cloud.plot2d(X[:, axis], ax=ax, **kws)
-            
+        if lower:
+            for ax, axis in zip(self.offdiag_axs, self.offdiag_indices):
+                if prof_edge_only:
+                    if profx:
+                        kws["profx"] = axis[1] == self.n - 1
+                    if profy:
+                        kws["profy"] = axis[0] == 0
+                if kws["kind"] in ["hist", "contour", "contourf"]:
+                    kws["bins"] = [edges[axis[0]], edges[axis[1]]]
+                vis_cloud.plot2d(X[:, axis], ax=ax, **kws)
+        if upper and not self.corner:
+            for ax, axis in zip(self.offdiag_axs_u, self.offdiag_indices_u):
+                if kws["kind"] in ["hist", "contour", "contourf"]:
+                    kws["bins"] = [edges[axis[0]], edges[axis[1]]]
+                vis_cloud.plot2d(X[:, axis], ax=ax, **kws)
+        self._fake_diag_yticks()
+
 
 class SliceGrid:
     """Grid for slice matrix plots (https://arxiv.org/abs/2301.04178).
 
     This plot is used to visualize four dimensions of a distribution f(x1, x2, x3, x4).
 
     The main panel is an nrows x ncols grid that shows f(x1, x2 | x3, x4) -- the
```

### Comparing `psdist-0.1.2/psdist/visualization/image.py` & `psdist-0.1.3/psdist/visualization/image.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.2/psdist/visualization/visualization.py` & `psdist-0.1.3/psdist/visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.2/pyproject.toml` & `psdist-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psdist"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Austin Hoover", email="ahoover1218@gmail.com" },
 ]
 description = "Analysis/visualization of phase space distributions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

