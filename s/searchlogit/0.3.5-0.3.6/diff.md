# Comparing `tmp/searchlogit-0.3.5.tar.gz` & `tmp/searchlogit-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchlogit-0.3.5.tar", last modified: Mon Apr 10 02:52:45 2023, max compression
+gzip compressed data, was "searchlogit-0.3.6.tar", last modified: Thu Apr 20 06:13:38 2023, max compression
```

## Comparing `searchlogit-0.3.5.tar` & `searchlogit-0.3.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:52:45.610794 searchlogit-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 02:52:34.000000 searchlogit-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-10 02:52:45.610794 searchlogit-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-10 02:52:34.000000 searchlogit-0.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:52:45.606793 searchlogit-0.3.5/searchlogit/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/_choice_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/boxcox_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    50431 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/latent_class_mixed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/latent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/mixed_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14368 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/multinomial_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)   169496 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:52:45.606793 searchlogit-0.3.5/searchlogit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-10 02:52:45.000000 searchlogit-0.3.5/searchlogit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-10 02:52:45.000000 searchlogit-0.3.5/searchlogit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:52:45.000000 searchlogit-0.3.5/searchlogit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:52:45.000000 searchlogit-0.3.5/searchlogit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 02:52:45.000000 searchlogit-0.3.5/searchlogit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 02:52:45.000000 searchlogit-0.3.5/searchlogit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 02:52:45.610794 searchlogit-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-10 02:52:34.000000 searchlogit-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:52:45.610794 searchlogit-0.3.5/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-04-10 02:52:34.000000 searchlogit-0.3.5/tests/test__choice_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-10 02:52:34.000000 searchlogit-0.3.5/tests/test__device.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-10 02:52:34.000000 searchlogit-0.3.5/tests/test_latent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-10 02:52:34.000000 searchlogit-0.3.5/tests/test_mixed_logit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-04-10 02:52:34.000000 searchlogit-0.3.5/tests/test_multinomial_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:52:34.000000 searchlogit-0.3.5/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:38.650545 searchlogit-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 06:13:28.000000 searchlogit-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-20 06:13:38.650545 searchlogit-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-20 06:13:28.000000 searchlogit-0.3.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:38.650545 searchlogit-0.3.6/searchlogit/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/_choice_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/boxcox_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50811 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/latent_class_mixed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/latent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/mixed_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14368 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/multinomial_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169496 2023-04-20 06:13:29.000000 searchlogit-0.3.6/searchlogit/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:38.650545 searchlogit-0.3.6/searchlogit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-20 06:13:38.000000 searchlogit-0.3.6/searchlogit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-20 06:13:38.000000 searchlogit-0.3.6/searchlogit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:13:38.000000 searchlogit-0.3.6/searchlogit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:13:38.000000 searchlogit-0.3.6/searchlogit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 06:13:38.000000 searchlogit-0.3.6/searchlogit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-20 06:13:38.000000 searchlogit-0.3.6/searchlogit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 06:13:38.650545 searchlogit-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-20 06:13:29.000000 searchlogit-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:38.650545 searchlogit-0.3.6/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-04-20 06:13:29.000000 searchlogit-0.3.6/tests/test__choice_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-20 06:13:29.000000 searchlogit-0.3.6/tests/test__device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-20 06:13:29.000000 searchlogit-0.3.6/tests/test_latent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-20 06:13:29.000000 searchlogit-0.3.6/tests/test_mixed_logit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-04-20 06:13:29.000000 searchlogit-0.3.6/tests/test_multinomial_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:13:29.000000 searchlogit-0.3.6/tests/test_search.py
```

### Comparing `searchlogit-0.3.5/LICENSE` & `searchlogit-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.5/PKG-INFO` & `searchlogit-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlogit
-Version: 0.3.5
+Version: 0.3.6
 Summary: Extensions for a Python package for                               GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/RyanJafefKelly/searchlogit
 Author: Ryan Kelly, Prithvi Beeramoole and Alexander Paz
 Author-email: ryan@kiiii.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `searchlogit-0.3.5/README.rst` & `searchlogit-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.5/searchlogit/_choice_model.py` & `searchlogit-0.3.6/searchlogit/_choice_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.5/searchlogit/_device.py` & `searchlogit-0.3.6/searchlogit/_device.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.5/searchlogit/boxcox_functions.py` & `searchlogit-0.3.6/searchlogit/boxcox_functions.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.5/searchlogit/latent_class_mixed_model.py` & `searchlogit-0.3.6/searchlogit/latent_class_mixed_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Implements Latent Class Mixed Model."""
 
 import itertools
 import logging
+import time
 
 import numpy as np
 from scipy.optimize import minimize
 
 from ._device import device as dev
 from .mixed_logit import MixedLogit
 
@@ -29,14 +30,15 @@
     ----------
     El Zarwi, F. (2017). lccm, a Python package for estimating latent
     class choice models using the Expectation Maximization (EM)
     algorithm to maximize the likelihood function.
     """
     def __init__(self):
         self.save_fitted_params = False  # speed-up computation
+        self.start_time = time.time()
         super(LatentClassMixedModel, self).__init__()
 
     def fit(self, X, y, varnames=None, alts=None, isvars=None, num_classes=2,
             class_params_spec=None, member_params_spec=None,
             transvars=None,
             transformation=None, ids=None, weights=None, avail=None,
             avail_latent=None,  # TODO?: separate param needed?
@@ -848,14 +850,15 @@
         self.trans_pos = [ii for ii, var in enumerate(self.varnames) if var in self.transvars]
 
         log_lik_old = 0
 
         self._make_short_df(X)
 
         max_iter = 2000
+        max_time = 3600  # seconds in an hour
         iter_num = 0
         class_betas_sd = [np.repeat(.99, len(betas))
                           for betas in class_betas]
         class_thetas_sd = np.repeat(.01, class_thetas.size)
 
         class_idxs = []
         class_fxidxs = []
@@ -883,14 +886,20 @@
             class_rvtransidx = [rvtransidx for ii, rvtransidx in enumerate(global_rvtransidx)
                                  if ii in X_class_idx]
             # class_rvtransidx = np.repeat(False, len(X_class_idx))
             class_rvidxs.append(class_rv_idx)
             class_rvtransidxs.append(class_rvtransidx)
 
         while not converged and iter_num < max_iter:
+            curr_time = time.time()
+            time_elapsed = curr_time - self.start_time
+            if time_elapsed > max_time:
+                logger.info('Time limit reached. Stopping EM algorithm.')
+                raise Exception("Time limit reached. Stopping EM algorithm.")
+
             # Expectation step
             self.ind_pred_prob_classes = []
             self.choice_pred_prob_classes = []
             # reset Kf, Kr in case weird isvars/intercept issues
             self.Kf = sum(class_fxidxs[0])
             self.Kr = sum(class_rvidxs[0])
             self.fxidx = class_fxidxs[0]
```

### Comparing `searchlogit-0.3.5/searchlogit/latent_class_model.py` & `searchlogit-0.3.6/searchlogit/latent_class_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Implements Latent Class Model."""
 
 import logging
 
 import numpy as np
+import time
 from scipy.optimize import minimize
 
 from .multinomial_logit import MultinomialLogit
 
 # define the computation boundary values not to be exceeded
 min_exp_val = -700
 max_exp_val = 700
@@ -16,14 +17,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class LatentClassModel(MultinomialLogit):
     """Class for estimation of Latent Class Models."""
     def __init__(self):
+        self.start_time = time.time()
         super(LatentClassModel, self).__init__()
 
     def fit(self, X, y, varnames=None, alts=None, isvars=None, num_classes=2,
             class_params_spec=None, member_params_spec=None,
             ids=None, weights=None, avail=None,
             avail_latent=None,
             transvars=None,
@@ -584,14 +586,15 @@
         # Remove intercept columns
         if self.fit_intercept:
             short_df = short_df[:, (self.J-2):]
             short_df[:, 0] = 1
         self.short_df = short_df
 
         max_iter = 2000
+        max_time = 3600  # one hour in second
         iter_num = 0
         class_betas_sd = [np.repeat(.99, len(betas))
                           for betas in class_betas]
         class_thetas_sd = np.repeat(.01, class_thetas.size)
         class_idxs = []
         class_fxidxs = []
         class_fxtransidxs = []
@@ -605,14 +608,19 @@
                             if ii in X_class_idx]
 
             class_fxtransidx = [not fxidx for fxidx in class_fx_idx]
             class_fxidxs.append(class_fx_idx)
             class_fxtransidxs.append(class_fxtransidx)
 
         while not converged and iter_num < max_iter:
+            curr_time = time.time()
+            time_elapsed = curr_time - self.start_time
+            if time_elapsed > max_time:
+                logger.info('Time limit reached. Stopping EM algorithm.')
+                raise Exception("Time limit reached. Stopping EM algorithm.")
             # Expectation step
             self.ind_pred_prob_classes = []
             self.choice_pred_prob_classes = []
             X_class0_idx = self._get_class_X_idx(0)
             # Set fxidx for base class when calling multinomial loglik
             self.fxidx = class_fxidxs[0]
             self.fxtransidx = class_fxtransidxs[0]
@@ -796,15 +804,15 @@
         for i in range(self.num_classes):
             pred_prob_tmp += p_class[i] * self.pred_prob_all[i*self.J:(i*self.J)+self.J]
         self.pred_prob = pred_prob_tmp
         return optimisation_result
 
     def validation_loglik(self, validation_X, validation_Y, avail=None,
                           avail_latent=None, weights=None, betas=None,
-                          anels=None):
+                          panels=None):
         """Compute the log-likelihood on the validation set."""
         validation_X, _ = self._setup_design_matrix(validation_X)
         N = validation_X.shape[0]
         validation_Y = validation_Y.reshape(N, -1)
 
         if panels is not None:
             ind_N = len(np.unique(panels))
```

### Comparing `searchlogit-0.3.5/searchlogit/mixed_logit.py` & `searchlogit-0.3.6/searchlogit/mixed_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.5/searchlogit/multinomial_logit.py` & `searchlogit-0.3.6/searchlogit/multinomial_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.5/searchlogit/search.py` & `searchlogit-0.3.6/searchlogit/search.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.5/searchlogit.egg-info/PKG-INFO` & `searchlogit-0.3.6/searchlogit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlogit
-Version: 0.3.5
+Version: 0.3.6
 Summary: Extensions for a Python package for                               GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/RyanJafefKelly/searchlogit
 Author: Ryan Kelly, Prithvi Beeramoole and Alexander Paz
 Author-email: ryan@kiiii.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `searchlogit-0.3.5/searchlogit.egg-info/SOURCES.txt` & `searchlogit-0.3.6/searchlogit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.5/setup.py` & `searchlogit-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import setuptools
 
 with codecs.open("README.rst", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='searchlogit',
-                 version='0.3.5',
+                 version='0.3.6',
                  description='Extensions for a Python package for \
                               GPU-accelerated estimation of mixed logit models.',
                  long_description=long_description,
                  long_description_content_type="text/x-rst",
                  url='https://github.com/RyanJafefKelly/searchlogit',
                  author='Ryan Kelly, Prithvi Beeramoole and Alexander Paz',
                  author_email='ryan@kiiii.com',
```

### Comparing `searchlogit-0.3.5/tests/test__choice_model.py` & `searchlogit-0.3.6/tests/test__choice_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.5/tests/test__device.py` & `searchlogit-0.3.6/tests/test__device.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.5/tests/test_latent_class_model.py` & `searchlogit-0.3.6/tests/test_latent_class_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.5/tests/test_mixed_logit.py` & `searchlogit-0.3.6/tests/test_mixed_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.5/tests/test_multinomial_logit.py` & `searchlogit-0.3.6/tests/test_multinomial_logit.py`

 * *Files identical despite different names*

