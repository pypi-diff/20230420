# Comparing `tmp/ripplegw-0.0.1.tar.gz` & `tmp/ripplegw-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ripplegw-0.0.1.tar", last modified: Fri Feb 10 17:22:20 2023, max compression
+gzip compressed data, was "ripplegw-0.0.2.tar", last modified: Thu Apr 20 15:10:44 2023, max compression
```

## Comparing `ripplegw-0.0.1.tar` & `ripplegw-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-02-10 17:22:20.110734 ripplegw-0.0.1/
--rw-r--r--   0 thomasedwards   (501) staff       (20)     1088 2022-10-12 22:06:55.000000 ripplegw-0.0.1/LICENSE
--rw-r--r--   0 thomasedwards   (501) staff       (20)     2804 2023-02-10 17:22:20.110852 ripplegw-0.0.1/PKG-INFO
--rw-r--r--   0 thomasedwards   (501) staff       (20)     2241 2022-10-12 22:06:55.000000 ripplegw-0.0.1/README.md
--rw-r--r--   0 thomasedwards   (501) staff       (20)      104 2022-10-12 22:06:55.000000 ripplegw-0.0.1/pyproject.toml
--rw-r--r--   0 thomasedwards   (501) staff       (20)      725 2023-02-10 17:22:20.111336 ripplegw-0.0.1/setup.cfg
--rw-r--r--   0 thomasedwards   (501) staff       (20)       38 2022-10-12 22:06:55.000000 ripplegw-0.0.1/setup.py
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-02-10 17:22:20.102622 ripplegw-0.0.1/src/
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-02-10 17:22:20.103909 ripplegw-0.0.1/src/ripple/
--rw-r--r--   0 thomasedwards   (501) staff       (20)     9886 2023-01-26 20:48:01.000000 ripplegw-0.0.1/src/ripple/__init__.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)      483 2023-01-06 18:06:40.000000 ripplegw-0.0.1/src/ripple/constants.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)     4002 2022-10-12 22:06:55.000000 ripplegw-0.0.1/src/ripple/noise.py
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-02-10 17:22:20.108421 ripplegw-0.0.1/src/ripple/noise_resources/
--rw-r--r--   0 thomasedwards   (501) staff       (20)    48230 2022-10-12 22:06:55.000000 ripplegw-0.0.1/src/ripple/noise_resources/O2_ASD.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)  1117811 2022-10-12 22:06:55.000000 ripplegw-0.0.1/src/ripple/noise_resources/O3a_Livingston_ASD.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)        0 2022-10-12 22:06:55.000000 ripplegw-0.0.1/src/ripple/noise_resources/__init__.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    56415 2022-10-12 22:06:55.000000 ripplegw-0.0.1/src/ripple/noise_resources/aLIGO.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)    10070 2022-10-12 22:06:55.000000 ripplegw-0.0.1/src/ripple/noise_resources/aLIGOZeroDetHighPower.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)    87114 2022-10-12 22:06:55.000000 ripplegw-0.0.1/src/ripple/noise_resources/ce.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)    87132 2022-10-12 22:06:55.000000 ripplegw-0.0.1/src/ripple/noise_resources/et.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)      201 2022-10-12 22:06:55.000000 ripplegw-0.0.1/src/ripple/typing.py
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-02-10 17:22:20.109747 ripplegw-0.0.1/src/ripple/waveforms/
--rw-r--r--   0 thomasedwards   (501) staff       (20)    19782 2023-02-02 14:53:55.000000 ripplegw-0.0.1/src/ripple/waveforms/IMRPhenomD.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    53661 2023-01-31 13:59:58.000000 ripplegw-0.0.1/src/ripple/waveforms/IMRPhenomD_QNMdata.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    15783 2023-01-06 19:15:14.000000 ripplegw-0.0.1/src/ripple/waveforms/IMRPhenomD_utils.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    12586 2023-02-10 17:15:40.000000 ripplegw-0.0.1/src/ripple/waveforms/IMRPhenomXAS.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)        0 2022-10-12 22:06:55.000000 ripplegw-0.0.1/src/ripple/waveforms/__init__.py
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-02-10 17:22:20.110432 ripplegw-0.0.1/src/ripplegw.egg-info/
--rw-r--r--   0 thomasedwards   (501) staff       (20)     2804 2023-02-10 17:22:19.000000 ripplegw-0.0.1/src/ripplegw.egg-info/PKG-INFO
--rw-r--r--   0 thomasedwards   (501) staff       (20)      816 2023-02-10 17:22:20.000000 ripplegw-0.0.1/src/ripplegw.egg-info/SOURCES.txt
--rw-r--r--   0 thomasedwards   (501) staff       (20)        1 2023-02-10 17:22:19.000000 ripplegw-0.0.1/src/ripplegw.egg-info/dependency_links.txt
--rw-r--r--   0 thomasedwards   (501) staff       (20)       17 2023-02-10 17:22:19.000000 ripplegw-0.0.1/src/ripplegw.egg-info/requires.txt
--rw-r--r--   0 thomasedwards   (501) staff       (20)        7 2023-02-10 17:22:19.000000 ripplegw-0.0.1/src/ripplegw.egg-info/top_level.txt
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-02-10 17:22:20.110570 ripplegw-0.0.1/test/
--rw-r--r--   0 thomasedwards   (501) staff       (20)    21003 2023-01-30 21:58:17.000000 ripplegw-0.0.1/test/test_imrphenomd.py
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-04-20 15:10:44.892833 ripplegw-0.0.2/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     1088 2022-10-12 22:06:55.000000 ripplegw-0.0.2/LICENSE
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     2735 2023-04-20 15:10:44.892911 ripplegw-0.0.2/PKG-INFO
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     2208 2023-04-20 15:08:56.000000 ripplegw-0.0.2/README.md
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      104 2022-10-12 22:06:55.000000 ripplegw-0.0.2/pyproject.toml
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      726 2023-04-20 15:10:44.893286 ripplegw-0.0.2/setup.cfg
+-rw-r--r--   0 thomasedwards   (501) staff       (20)       38 2022-10-12 22:06:55.000000 ripplegw-0.0.2/setup.py
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-04-20 15:10:44.885270 ripplegw-0.0.2/src/
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-04-20 15:10:44.886652 ripplegw-0.0.2/src/ripple/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     9886 2023-01-26 20:48:01.000000 ripplegw-0.0.2/src/ripple/__init__.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      483 2023-01-06 18:06:40.000000 ripplegw-0.0.2/src/ripple/constants.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     4002 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise.py
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-04-20 15:10:44.890385 ripplegw-0.0.2/src/ripple/noise_resources/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    48230 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise_resources/O2_ASD.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)  1117811 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise_resources/O3a_Livingston_ASD.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)        0 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise_resources/__init__.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    56415 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise_resources/aLIGO.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    10070 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise_resources/aLIGOZeroDetHighPower.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    87114 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise_resources/ce.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    87132 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise_resources/et.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      201 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/typing.py
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-04-20 15:10:44.891828 ripplegw-0.0.2/src/ripple/waveforms/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    19476 2023-04-20 15:01:50.000000 ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomD.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    53661 2023-01-31 13:59:58.000000 ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomD_QNMdata.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    15783 2023-01-06 19:15:14.000000 ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomD_utils.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    44771 2023-04-20 15:01:50.000000 ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomXAS.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    39958 2023-04-20 15:01:50.000000 ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomX_utils.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)        0 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/waveforms/__init__.py
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-04-20 15:10:44.892448 ripplegw-0.0.2/src/ripplegw.egg-info/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     2735 2023-04-20 15:10:44.000000 ripplegw-0.0.2/src/ripplegw.egg-info/PKG-INFO
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      881 2023-04-20 15:10:44.000000 ripplegw-0.0.2/src/ripplegw.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasedwards   (501) staff       (20)        1 2023-04-20 15:10:44.000000 ripplegw-0.0.2/src/ripplegw.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasedwards   (501) staff       (20)       17 2023-04-20 15:10:44.000000 ripplegw-0.0.2/src/ripplegw.egg-info/requires.txt
+-rw-r--r--   0 thomasedwards   (501) staff       (20)        7 2023-04-20 15:10:44.000000 ripplegw-0.0.2/src/ripplegw.egg-info/top_level.txt
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-04-20 15:10:44.892714 ripplegw-0.0.2/test/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    26166 2023-04-20 15:01:50.000000 ripplegw-0.0.2/test/test_IMRPhenomX.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    21003 2023-01-30 21:58:17.000000 ripplegw-0.0.2/test/test_imrphenomd.py
```

### Comparing `ripplegw-0.0.1/LICENSE` & `ripplegw-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.1/PKG-INFO` & `ripplegw-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 Metadata-Version: 2.1
 Name: ripplegw
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small jax package for differentiable and fast gravitational wave data analysis.
 Home-page: https://ripple.readthedocs.io/en/latest/
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/tedwards2412/ripple
 Keywords: gravitational waves,jax
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Ripple
+# Ripple :ocean:
 
 A small `jax` package for differentiable and fast gravitational wave data analysis.
 
 # Getting Started
 
 ### Installation
 
-Ripple is still in its development stage and therefore has not been made available installable directly through pip yet. Instead,
-one can install using 
+Both waveforms have been tested extensively and match lalsuite implementations to machine precision across all the parameter space. 
+
+Ripple can be installed using 
 
 ```
-git clone git@github.com:tedwards2412/ripple.git
-cd ripple
-pip3 install .
+pip3 install ripplegw
 ```
 
+### Supported waveforms
+
+- IMRPhenomXAS (aligned spin)
+- IMRPhenomD (aligned spin)
+
 ### Generating a waveform and its derivative
 
-Generating a waveform is increadibly easy. Below is an example of calling the PhenomD waveform model
+Generating a waveform is increadibly easy. Below is an example of calling the PhenomXAS waveform model
 to get the h_+ and h_x polarizations of the waveform model
 
 We start with some basic imports:
 
 ```python
-from math import pi
 import jax.numpy as jnp
 
-from ripple.waveforms import IMRPhenomD
-import matplotlib.pyplot as plt
+from ripple.waveforms import IMRPhenomXAS
 from ripple import ms_to_Mc_eta
 ```
 
 And now we can just set the parameters and call the waveform!
 
 ```python
 # Get a frequency domain waveform
@@ -57,41 +57,39 @@
 m2_msun = 19.0
 chi1 = 0.5 # Dimensionless spin
 chi2 = -0.5
 tc = 0.0 # Time of coalescence in seconds
 phic = 0.0 # Time of coalescence
 dist_mpc = 440 # Distance to source in Mpc
 inclination = 0.0 # Inclination Angle
-polarization_angle = 0.2 # Polarization angle
 
 # The PhenomD waveform model is parameterized with the chirp mass and symmetric mass ratio
 Mc, eta = ms_to_Mc_eta(jnp.array([m1_msun, m2_msun]))
 
 # These are the parametrs that go into the waveform generator
 # Note that JAX does not give index errors, so if you pass in the
 # the wrong array it will behave strangely
-theta_ripple = jnp.array([Mc, eta, chi1, chi2, dist_mpc, tc, phic, inclination, polarization_angle])
+theta_ripple = jnp.array([Mc, eta, chi1, chi2, dist_mpc, tc, phic, inclination])
 
 # Now we need to generate the frequency grid
 f_l = 24
 f_u = 512
 del_f = 0.01
 fs = jnp.arange(f_l, f_u, del_f)
+f_ref = f_l
 
 # And finally lets generate the waveform!
-hp_ripple, hc_ripple = IMRPhenomD.gen_IMRPhenomD_polar(fs, theta_ripple)
+hp_ripple, hc_ripple = IMRPhenomXAS.gen_IMRPhenomXAS_polar(fs, theta_ripple, f_ref)
 
 # Note that we have not internally jitted the functions since this would
-# introduce an annoying overhead each time the use evaluated the function with a different length frequency array
-# We therefore recommend that the user jit the function themselves to accelerate evaluations. For example
+# introduce an annoying overhead each time the user evaluated the function with a different length frequency array
+# We therefore recommend that the user jit the function themselves to accelerate evaluations. For example:
 
 import jax
 
 @jax.jit
 def waveform(theta):
-    return IMRPhenomD.gen_IMRPhenomD_polar(fs, theta)
+    return IMRPhenomXAS.gen_IMRPhenomXAS_polar(fs, theta)
 ```
 
 
 
-
-
```

### Comparing `ripplegw-0.0.1/README.md` & `ripplegw-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-# Ripple
+# Ripple :ocean:
 
 A small `jax` package for differentiable and fast gravitational wave data analysis.
 
 # Getting Started
 
 ### Installation
 
-Ripple is still in its development stage and therefore has not been made available installable directly through pip yet. Instead,
-one can install using 
+Both waveforms have been tested extensively and match lalsuite implementations to machine precision across all the parameter space. 
+
+Ripple can be installed using 
 
 ```
-git clone git@github.com:tedwards2412/ripple.git
-cd ripple
-pip3 install .
+pip3 install ripplegw
 ```
 
+### Supported waveforms
+
+- IMRPhenomXAS (aligned spin)
+- IMRPhenomD (aligned spin)
+
 ### Generating a waveform and its derivative
 
-Generating a waveform is increadibly easy. Below is an example of calling the PhenomD waveform model
+Generating a waveform is increadibly easy. Below is an example of calling the PhenomXAS waveform model
 to get the h_+ and h_x polarizations of the waveform model
 
 We start with some basic imports:
 
 ```python
-from math import pi
 import jax.numpy as jnp
 
-from ripple.waveforms import IMRPhenomD
-import matplotlib.pyplot as plt
+from ripple.waveforms import IMRPhenomXAS
 from ripple import ms_to_Mc_eta
 ```
 
 And now we can just set the parameters and call the waveform!
 
 ```python
 # Get a frequency domain waveform
@@ -41,39 +43,39 @@
 m2_msun = 19.0
 chi1 = 0.5 # Dimensionless spin
 chi2 = -0.5
 tc = 0.0 # Time of coalescence in seconds
 phic = 0.0 # Time of coalescence
 dist_mpc = 440 # Distance to source in Mpc
 inclination = 0.0 # Inclination Angle
-polarization_angle = 0.2 # Polarization angle
 
 # The PhenomD waveform model is parameterized with the chirp mass and symmetric mass ratio
 Mc, eta = ms_to_Mc_eta(jnp.array([m1_msun, m2_msun]))
 
 # These are the parametrs that go into the waveform generator
 # Note that JAX does not give index errors, so if you pass in the
 # the wrong array it will behave strangely
-theta_ripple = jnp.array([Mc, eta, chi1, chi2, dist_mpc, tc, phic, inclination, polarization_angle])
+theta_ripple = jnp.array([Mc, eta, chi1, chi2, dist_mpc, tc, phic, inclination])
 
 # Now we need to generate the frequency grid
 f_l = 24
 f_u = 512
 del_f = 0.01
 fs = jnp.arange(f_l, f_u, del_f)
+f_ref = f_l
 
 # And finally lets generate the waveform!
-hp_ripple, hc_ripple = IMRPhenomD.gen_IMRPhenomD_polar(fs, theta_ripple)
+hp_ripple, hc_ripple = IMRPhenomXAS.gen_IMRPhenomXAS_polar(fs, theta_ripple, f_ref)
 
 # Note that we have not internally jitted the functions since this would
-# introduce an annoying overhead each time the use evaluated the function with a different length frequency array
-# We therefore recommend that the user jit the function themselves to accelerate evaluations. For example
+# introduce an annoying overhead each time the user evaluated the function with a different length frequency array
+# We therefore recommend that the user jit the function themselves to accelerate evaluations. For example:
 
 import jax
 
 @jax.jit
 def waveform(theta):
-    return IMRPhenomD.gen_IMRPhenomD_polar(fs, theta)
+    return IMRPhenomXAS.gen_IMRPhenomXAS_polar(fs, theta)
 ```
```

### Comparing `ripplegw-0.0.1/setup.cfg` & `ripplegw-0.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ripplegw
-version = 0.0.1
+version = 0.0.2
 description = A small jax package for differentiable and fast gravitational wave data analysis.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = gravitational waves, jax
 url = https://ripple.readthedocs.io/en/latest/
 project_urls = 
 	Bug Tracker = https://github.com/tedwards2412/ripple
@@ -13,15 +13,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.10
 install_requires = 
 	jax
 	jaxlib
 	numpy
 
 [options.package_data]
 * = *.dat
```

### Comparing `ripplegw-0.0.1/src/ripple/__init__.py` & `ripplegw-0.0.2/src/ripple/__init__.py`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.1/src/ripple/noise.py` & `ripplegw-0.0.2/src/ripple/noise.py`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.1/src/ripple/noise_resources/O2_ASD.dat` & `ripplegw-0.0.2/src/ripple/noise_resources/O2_ASD.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.1/src/ripple/noise_resources/O3a_Livingston_ASD.dat` & `ripplegw-0.0.2/src/ripple/noise_resources/O3a_Livingston_ASD.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.1/src/ripple/noise_resources/aLIGO.dat` & `ripplegw-0.0.2/src/ripple/noise_resources/aLIGO.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.1/src/ripple/noise_resources/aLIGOZeroDetHighPower.dat` & `ripplegw-0.0.2/src/ripple/noise_resources/aLIGOZeroDetHighPower.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.1/src/ripple/noise_resources/ce.dat` & `ripplegw-0.0.2/src/ripple/noise_resources/ce.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.1/src/ripple/noise_resources/et.dat` & `ripplegw-0.0.2/src/ripple/noise_resources/et.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.1/src/ripple/waveforms/IMRPhenomD.py` & `ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomD.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """
     # First lets calculate some of the vairables that will be used below
     # Mass variables
     m1, m2, chi1, chi2 = theta
     m1_s = m1 * gt
     m2_s = m2 * gt
     M_s = m1_s + m2_s
-    eta = m1_s * m2_s / (M_s ** 2.0)
+    eta = m1_s * m2_s / (M_s**2.0)
 
     # First lets construct the phase in the inspiral (region I)
     m1M = m1_s / M_s
     m2M = m2_s / M_s
 
     phi0 = 1.0
     phi1 = 0.0
@@ -47,33 +47,28 @@
         + ((-720.0 / 9.6 * m1M * m1M) + (1.0 / 9.6 * m1M * m1M)) * chi1 * chi1
         + ((-720.0 / 9.6 * m2M * m2M) + (1.0 / 9.6 * m2M * m2M)) * chi2 * chi2
         + ((240.0 / 9.6 * m1M * m1M) + (-7.0 / 9.6 * m1M * m1M)) * chi1 * chi1
         + ((240.0 / 9.6 * m2M * m2M) + (-7.0 / 9.6 * m2M * m2M)) * chi2 * chi2
     )
     phi5 = 5.0 / 9.0 * (772.9 / 8.4 - 13.0 * eta) * PI
     phi5 += (
-        (
-            -m1M
-            * (
-                1391.5 / 8.4
-                - m1M * (1.0 - m1M) * 10.0 / 3.0
-                + m1M * (1276.0 / 8.1 + m1M * (1.0 - m1M) * 170.0 / 9.0)
-            )
+        -m1M
+        * (
+            1391.5 / 8.4
+            - m1M * (1.0 - m1M) * 10.0 / 3.0
+            + m1M * (1276.0 / 8.1 + m1M * (1.0 - m1M) * 170.0 / 9.0)
         )
-        * chi1
-        + (
-            -m2M
-            * (
-                1391.5 / 8.4
-                - m2M * (1.0 - m2M) * 10.0 / 3.0
-                + m2M * (1276.0 / 8.1 + m2M * (1.0 - m2M) * 170.0 / 9.0)
-            )
+    ) * chi1 + (
+        -m2M
+        * (
+            1391.5 / 8.4
+            - m2M * (1.0 - m2M) * 10.0 / 3.0
+            + m2M * (1276.0 / 8.1 + m2M * (1.0 - m2M) * 170.0 / 9.0)
         )
-        * chi2
-    )
+    ) * chi2
     phi5_log = (5.0 / 3.0) * (772.9 / 8.4 - 13.0 * eta) * PI
     phi5_log += 3.0 * (
         (
             -m1M
             * (
                 1391.5 / 8.4
                 - m1M * (1.0 - m1M) * 10.0 / 3.0
@@ -108,45 +103,40 @@
     ) * chi2
     phi6_log = -684.8 / 2.1
 
     phi7 = PI * (
         770.96675 / 2.54016 + 378.515 / 1.512 * eta - 740.45 / 7.56 * eta * eta
     )
     phi7 += (
-        (
-            m1M
+        m1M
+        * (
+            -17097.8035 / 4.8384
+            + eta * 28764.25 / 6.72
+            + eta * eta * 47.35 / 1.44
+            + m1M
             * (
-                -17097.8035 / 4.8384
-                + eta * 28764.25 / 6.72
-                + eta * eta * 47.35 / 1.44
-                + m1M
-                * (
-                    -7189.233785 / 1.524096
-                    + eta * 458.555 / 3.024
-                    - eta * eta * 534.5 / 7.2
-                )
+                -7189.233785 / 1.524096
+                + eta * 458.555 / 3.024
+                - eta * eta * 534.5 / 7.2
             )
         )
-        * chi1
-        + (
-            m2M
+    ) * chi1 + (
+        m2M
+        * (
+            -17097.8035 / 4.8384
+            + eta * 28764.25 / 6.72
+            + eta * eta * 47.35 / 1.44
+            + m2M
             * (
-                -17097.8035 / 4.8384
-                + eta * 28764.25 / 6.72
-                + eta * eta * 47.35 / 1.44
-                + m2M
-                * (
-                    -7189.233785 / 1.524096
-                    + eta * 458.555 / 3.024
-                    - eta * eta * 534.5 / 7.2
-                )
+                -7189.233785 / 1.524096
+                + eta * 458.555 / 3.024
+                - eta * eta * 534.5 / 7.2
             )
         )
-        * chi2
-    )
+    ) * chi2
 
     # Add frequency dependence here
     v = (PI * fM_s) ** (1.0 / 3.0)
 
     phi_TF2 = (
         (phi5 - PI / 4.0)
         + phi0 * ((PI * fM_s) ** -(5.0 / 3.0))
@@ -162,50 +152,50 @@
 
     phi_Ins = (
         phi_TF2
         + (
             coeffs[7] * fM_s
             + (3.0 / 4.0) * coeffs[8] * (fM_s ** (4.0 / 3.0))
             + (3.0 / 5.0) * coeffs[9] * (fM_s ** (5.0 / 3.0))
-            + (1.0 / 2.0) * coeffs[10] * (fM_s ** 2.0)
+            + (1.0 / 2.0) * coeffs[10] * (fM_s**2.0)
         )
         / eta
     )
     return phi_Ins
 
 
 def get_IIa_raw_phase(fM_s: Array, theta: Array, coeffs: Array) -> Array:
     m1, m2, _, _ = theta
     m1_s = m1 * gt
     m2_s = m2 * gt
     M_s = m1_s + m2_s
-    eta = m1_s * m2_s / (M_s ** 2.0)
+    eta = m1_s * m2_s / (M_s**2.0)
 
     phi_IIa_raw = (
         coeffs[11] * fM_s
         + coeffs[12] * jnp.log(fM_s)
-        - coeffs[13] * (fM_s ** -3.0) / 3.0
+        - coeffs[13] * (fM_s**-3.0) / 3.0
     ) / eta
 
     return phi_IIa_raw
 
 
 def get_IIb_raw_phase(fM_s: Array, theta: Array, coeffs: Array, f_RD, f_damp) -> Array:
     m1, m2, _, _ = theta
     m1_s = m1 * gt
     m2_s = m2 * gt
     M_s = m1_s + m2_s
-    eta = m1_s * m2_s / (M_s ** 2.0)
+    eta = m1_s * m2_s / (M_s**2.0)
 
     f_RDM_s = f_RD * M_s
     f_dampM_s = f_damp * M_s
 
     phi_IIb_raw = (
         coeffs[14] * fM_s
-        - coeffs[15] * (fM_s ** -1.0)
+        - coeffs[15] * (fM_s**-1.0)
         + 4.0 * coeffs[16] * (fM_s ** (3.0 / 4.0)) / 3.0
         + coeffs[17] * jnp.arctan((fM_s - coeffs[18] * f_RDM_s) / f_dampM_s)
     ) / eta
 
     return phi_IIb_raw
 
 
@@ -219,15 +209,15 @@
 def get_inspiral_Amp(fM_s: Array, theta: Array, coeffs: Array) -> Array:
     # Below is taken from https://git.ligo.org/lscsoft/lalsuite/-/blob/master/lalsimulation/lib/LALSimIMRPhenomD_internals.c
     # Lines 302 --> 351
     m1, m2, chi1, chi2 = theta
     m1_s = m1 * gt
     m2_s = m2 * gt
     M_s = m1_s + m2_s
-    eta = m1_s * m2_s / (M_s ** 2.0)
+    eta = m1_s * m2_s / (M_s**2.0)
     eta2 = eta * eta
     eta3 = eta * eta2
 
     Seta = jnp.sqrt(1.0 - 4.0 * eta)
     SetaPlus1 = 1.0 + Seta
 
     # Spin variables
@@ -280,15 +270,15 @@
             )
             + 42840.0 * (-1.0 + 4.0 * eta) * PI
         )
     ) / 32256.0
 
     A6 = (
         -(
-            (PI ** 2.0)
+            (PI**2.0)
             * (
                 -336.0
                 * (
                     -3248849057.0
                     + 2943675504.0 * chi12
                     - 3339284256.0 * chi1 * chi2
                     + 2943675504.0 * chi22
@@ -308,15 +298,15 @@
                 * (
                     -545384828789.0
                     - 176491177632.0 * chi1 * chi2
                     + 202603761360.0 * chi22
                     + 77616.0 * chi12 * (2610335.0 + 995766.0 * Seta)
                     - 77287373856.0 * chi22 * Seta
                     + 5841690624.0 * (chi1 + chi2) * PI
-                    + 21384760320.0 * (PI ** 2.0)
+                    + 21384760320.0 * (PI**2.0)
                 )
             )
         )
         / 6.0085960704e10
     )
     A7 = coeffs[0]
     A8 = coeffs[1]
@@ -325,19 +315,19 @@
     Amp_Ins = (
         A0
         # A1 is missed since its zero
         + A2 * (fM_s ** (2.0 / 3.0))
         + A3 * fM_s
         + A4 * (fM_s ** (4.0 / 3.0))
         + A5 * (fM_s ** (5.0 / 3.0))
-        + A6 * (fM_s ** 2.0)
+        + A6 * (fM_s**2.0)
         # Now we add the coefficient terms
         + A7 * (fM_s ** (7.0 / 3.0))
         + A8 * (fM_s ** (8.0 / 3.0))
-        + A9 * (fM_s ** 3.0)
+        + A9 * (fM_s**3.0)
     )
 
     return Amp_Ins
 
 
 def get_IIa_Amp(
     fM_s: Array, theta: Array, coeffs: Array, f1, f3, f_RD, f_damp
@@ -361,17 +351,17 @@
     delta2 = get_delta2(f1 * M_s, f2 * M_s, f3 * M_s, v1, coeffs[3], v3, d1, d3)
     delta3 = get_delta3(f1 * M_s, f2 * M_s, f3 * M_s, v1, coeffs[3], v3, d1, d3)
     delta4 = get_delta4(f1 * M_s, f2 * M_s, f3 * M_s, v1, coeffs[3], v3, d1, d3)
 
     Amp_IIa = (
         delta0
         + delta1 * fM_s
-        + delta2 * (fM_s ** 2.0)
-        + delta3 * (fM_s ** 3.0)
-        + delta4 * (fM_s ** 4.0)
+        + delta2 * (fM_s**2.0)
+        + delta3 * (fM_s**3.0)
+        + delta4 * (fM_s**4.0)
     )
 
     return Amp_IIa
 
 
 def get_IIb_Amp(fM_s: Array, theta: Array, coeffs: Array, f_RD, f_damp) -> Array:
     m1, m2, _, _ = theta
@@ -487,15 +477,15 @@
 
     # First lets calculate some of the vairables that will be used below
     # Mass variables
     m1, m2, _, _ = theta
     m1_s = m1 * gt
     m2_s = m2 * gt
     M_s = m1_s + m2_s
-    eta = m1_s * m2_s / (M_s ** 2.0)
+    eta = m1_s * m2_s / (M_s**2.0)
 
     # _, _, f3, f4, f_RD, f_damp = get_transition_frequencies(theta, coeffs[5], coeffs[6])
     _, _, f3, f4, f_RD, f_damp = transition_frequencies
 
     # First we get the inspiral amplitude
     Amp_Ins = get_inspiral_Amp(f * M_s, theta, coeffs)
 
@@ -520,15 +510,15 @@
     # Prefactor
     Amp0 = get_Amp0(f * M_s, eta) * (
         2.0 * jnp.sqrt(5.0 / (64.0 * PI))
     )  # This second factor is from lalsuite
 
     # Need to add in an overall scaling of M_s^2 to make the units correct
     dist_s = (D * m_per_Mpc) / C
-    return Amp0 * Amp * (M_s ** 2.0) / dist_s
+    return Amp0 * Amp * (M_s**2.0) / dist_s
 
 
 # @jax.jit
 def _gen_IMRPhenomD(
     f: Array,
     theta_intrinsic: Array,
     theta_extrinsic: Array,
@@ -572,15 +562,15 @@
     Mchirp: Chirp mass of the system [solar masses]
     eta: Symmetric mass ratio [between 0.0 and 0.25]
     chi1: Dimensionless aligned spin of the primary object [between -1 and 1]
     chi2: Dimensionless aligned spin of the secondary object [between -1 and 1]
     D: Luminosity distance to source [Mpc]
     tc: Time of coalesence. This only appears as an overall linear in f contribution to the phase
     phic: Phase of coalesence
-    
+
     f_ref: Reference frequency for the waveform
 
     Returns:
     --------
       h0 (array): Strain
     """
     # Lets make this easier by starting in Mchirp and eta space
@@ -615,11 +605,10 @@
       hp (array): Strain of the plus polarization
       hc (array): Strain of the cross polarization
     """
     iota = params[7]
     h0 = gen_IMRPhenomD(f, params, f_ref)
 
     hp = h0 * (1 / 2 * (1 + jnp.cos(iota) ** 2))
-    # hc = h0 * jnp.cos(iota)
     hc = -1j * h0 * jnp.cos(iota)
 
     return hp, hc
```

### Comparing `ripplegw-0.0.1/src/ripple/waveforms/IMRPhenomD_QNMdata.py` & `ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomD_QNMdata.py`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.1/src/ripple/waveforms/IMRPhenomD_utils.py` & `ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomD_utils.py`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.1/src/ripplegw.egg-info/PKG-INFO` & `ripplegw-0.0.2/src/ripplegw.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 Metadata-Version: 2.1
 Name: ripplegw
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small jax package for differentiable and fast gravitational wave data analysis.
 Home-page: https://ripple.readthedocs.io/en/latest/
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/tedwards2412/ripple
 Keywords: gravitational waves,jax
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Ripple
+# Ripple :ocean:
 
 A small `jax` package for differentiable and fast gravitational wave data analysis.
 
 # Getting Started
 
 ### Installation
 
-Ripple is still in its development stage and therefore has not been made available installable directly through pip yet. Instead,
-one can install using 
+Both waveforms have been tested extensively and match lalsuite implementations to machine precision across all the parameter space. 
+
+Ripple can be installed using 
 
 ```
-git clone git@github.com:tedwards2412/ripple.git
-cd ripple
-pip3 install .
+pip3 install ripplegw
 ```
 
+### Supported waveforms
+
+- IMRPhenomXAS (aligned spin)
+- IMRPhenomD (aligned spin)
+
 ### Generating a waveform and its derivative
 
-Generating a waveform is increadibly easy. Below is an example of calling the PhenomD waveform model
+Generating a waveform is increadibly easy. Below is an example of calling the PhenomXAS waveform model
 to get the h_+ and h_x polarizations of the waveform model
 
 We start with some basic imports:
 
 ```python
-from math import pi
 import jax.numpy as jnp
 
-from ripple.waveforms import IMRPhenomD
-import matplotlib.pyplot as plt
+from ripple.waveforms import IMRPhenomXAS
 from ripple import ms_to_Mc_eta
 ```
 
 And now we can just set the parameters and call the waveform!
 
 ```python
 # Get a frequency domain waveform
@@ -57,41 +57,39 @@
 m2_msun = 19.0
 chi1 = 0.5 # Dimensionless spin
 chi2 = -0.5
 tc = 0.0 # Time of coalescence in seconds
 phic = 0.0 # Time of coalescence
 dist_mpc = 440 # Distance to source in Mpc
 inclination = 0.0 # Inclination Angle
-polarization_angle = 0.2 # Polarization angle
 
 # The PhenomD waveform model is parameterized with the chirp mass and symmetric mass ratio
 Mc, eta = ms_to_Mc_eta(jnp.array([m1_msun, m2_msun]))
 
 # These are the parametrs that go into the waveform generator
 # Note that JAX does not give index errors, so if you pass in the
 # the wrong array it will behave strangely
-theta_ripple = jnp.array([Mc, eta, chi1, chi2, dist_mpc, tc, phic, inclination, polarization_angle])
+theta_ripple = jnp.array([Mc, eta, chi1, chi2, dist_mpc, tc, phic, inclination])
 
 # Now we need to generate the frequency grid
 f_l = 24
 f_u = 512
 del_f = 0.01
 fs = jnp.arange(f_l, f_u, del_f)
+f_ref = f_l
 
 # And finally lets generate the waveform!
-hp_ripple, hc_ripple = IMRPhenomD.gen_IMRPhenomD_polar(fs, theta_ripple)
+hp_ripple, hc_ripple = IMRPhenomXAS.gen_IMRPhenomXAS_polar(fs, theta_ripple, f_ref)
 
 # Note that we have not internally jitted the functions since this would
-# introduce an annoying overhead each time the use evaluated the function with a different length frequency array
-# We therefore recommend that the user jit the function themselves to accelerate evaluations. For example
+# introduce an annoying overhead each time the user evaluated the function with a different length frequency array
+# We therefore recommend that the user jit the function themselves to accelerate evaluations. For example:
 
 import jax
 
 @jax.jit
 def waveform(theta):
-    return IMRPhenomD.gen_IMRPhenomD_polar(fs, theta)
+    return IMRPhenomXAS.gen_IMRPhenomXAS_polar(fs, theta)
 ```
 
 
 
-
-
```

### Comparing `ripplegw-0.0.1/src/ripplegw.egg-info/SOURCES.txt` & `ripplegw-0.0.2/src/ripplegw.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 src/ripple/noise_resources/aLIGOZeroDetHighPower.dat
 src/ripple/noise_resources/ce.dat
 src/ripple/noise_resources/et.dat
 src/ripple/waveforms/IMRPhenomD.py
 src/ripple/waveforms/IMRPhenomD_QNMdata.py
 src/ripple/waveforms/IMRPhenomD_utils.py
 src/ripple/waveforms/IMRPhenomXAS.py
+src/ripple/waveforms/IMRPhenomX_utils.py
 src/ripple/waveforms/__init__.py
 src/ripplegw.egg-info/PKG-INFO
 src/ripplegw.egg-info/SOURCES.txt
 src/ripplegw.egg-info/dependency_links.txt
 src/ripplegw.egg-info/requires.txt
 src/ripplegw.egg-info/top_level.txt
+test/test_IMRPhenomX.py
 test/test_imrphenomd.py
```

### Comparing `ripplegw-0.0.1/test/test_imrphenomd.py` & `ripplegw-0.0.2/test/test_imrphenomd.py`

 * *Files identical despite different names*

