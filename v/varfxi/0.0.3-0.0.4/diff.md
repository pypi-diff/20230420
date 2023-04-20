# Comparing `tmp/varfxi-0.0.3.tar.gz` & `tmp/varfxi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varfxi-0.0.3.tar", max compression
+gzip compressed data, was "varfxi-0.0.4.tar", max compression
```

## Comparing `varfxi-0.0.3.tar` & `varfxi-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-03-14 06:10:54.473765 varfxi-0.0.3/LICENSE
--rw-r--r--   0        0        0     2131 2023-03-14 06:48:41.529526 varfxi-0.0.3/README.md
--rw-r--r--   0        0        0     1168 2023-04-19 09:56:52.340421 varfxi-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    99792 2023-04-19 09:53:31.728969 varfxi-0.0.3/varfxi/.ipynb_checkpoints/distGARCH-checkpoint.py
--rw-r--r--   0        0        0       23 2023-03-14 06:10:55.421776 varfxi-0.0.3/varfxi/__init__.py
--rw-r--r--   0        0        0    99792 2023-04-19 09:53:31.728969 varfxi-0.0.3/varfxi/distGARCH.py
--rw-r--r--   0        0        0    21321 2023-03-14 06:10:55.421776 varfxi-0.0.3/varfxi/joyplot2.py
--rw-r--r--   0        0        0    34634 2023-03-14 06:10:55.421776 varfxi-0.0.3/varfxi/quantileproj.py
--rw-r--r--   0        0        0     3142 1970-01-01 00:00:00.000000 varfxi-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-14 06:10:54.473765 varfxi-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2131 2023-03-14 06:48:41.529526 varfxi-0.0.4/README.md
+-rw-r--r--   0        0        0     1168 2023-04-20 09:26:00.959958 varfxi-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    99794 2023-04-20 08:55:24.716915 varfxi-0.0.4/varfxi/.ipynb_checkpoints/distGARCH-checkpoint.py
+-rw-r--r--   0        0        0    21321 2023-04-20 08:53:48.077186 varfxi-0.0.4/varfxi/.ipynb_checkpoints/joyplot2-checkpoint.py
+-rw-r--r--   0        0        0    34634 2023-04-20 08:53:48.077186 varfxi-0.0.4/varfxi/.ipynb_checkpoints/quantileproj-checkpoint.py
+-rw-r--r--   0        0        0       23 2023-03-14 06:10:55.421776 varfxi-0.0.4/varfxi/__init__.py
+-rw-r--r--   0        0        0    99794 2023-04-20 08:55:24.716915 varfxi-0.0.4/varfxi/distGARCH.py
+-rw-r--r--   0        0        0    21321 2023-03-14 06:10:55.421776 varfxi-0.0.4/varfxi/joyplot2.py
+-rw-r--r--   0        0        0    34634 2023-03-14 06:10:55.421776 varfxi-0.0.4/varfxi/quantileproj.py
+-rw-r--r--   0        0        0     3142 1970-01-01 00:00:00.000000 varfxi-0.0.4/PKG-INFO
```

### Comparing `varfxi-0.0.3/LICENSE` & `varfxi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `varfxi-0.0.3/README.md` & `varfxi-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `varfxi-0.0.3/pyproject.toml` & `varfxi-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "varfxi"
-version = "0.0.3"
+version = "0.0.4"
 description = "Volatility based estimation for FX interventions"
 authors = ["romainlafarguette <romain.lafarguette@gmail.com>", "amineraboun <amineraboun@gmail.com>"]
 repository ="https://github.com/romainlafarguette/varfxi"
 homepage  ="https://github.com/romainlafarguette/varfxi"
 
 readme = "README.md"
 keywords = ["var", "garch"]
```

### Comparing `varfxi-0.0.3/varfxi/.ipynb_checkpoints/distGARCH-checkpoint.py` & `varfxi-0.0.4/varfxi/.ipynb_checkpoints/distGARCH-checkpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1523,19 +1523,19 @@
             ], axis=1, keys=['params', 'pvalues'])
             
             if i>=1:
                 prev_param = iter_params[f"iteration_{i-1}"].params
                 new_params = iter_params[f"iteration_{i}"].params
                 pct_param_shift = ((new_params-prev_param)/prev_param).abs().max()
                 if pct_param_shift < convergence_rate:
-                    converge=True
+                    converged=True
                     break;
                 else:
                     continue
-        if converge:
+        if converged:
             print('Converged !')
         else:
             print('Max iteration reached without convergion !')
 
         params_df = pd.concat(iter_params.values(), keys = iter_params.keys(), axis=1)
         
         self.final_model = DistGARCH(
```

### Comparing `varfxi-0.0.3/varfxi/distGARCH.py` & `varfxi-0.0.4/varfxi/distGARCH.py`

 * *Files 0% similar despite different names*

```diff
@@ -1523,19 +1523,19 @@
             ], axis=1, keys=['params', 'pvalues'])
             
             if i>=1:
                 prev_param = iter_params[f"iteration_{i-1}"].params
                 new_params = iter_params[f"iteration_{i}"].params
                 pct_param_shift = ((new_params-prev_param)/prev_param).abs().max()
                 if pct_param_shift < convergence_rate:
-                    converge=True
+                    converged=True
                     break;
                 else:
                     continue
-        if converge:
+        if converged:
             print('Converged !')
         else:
             print('Max iteration reached without convergion !')
 
         params_df = pd.concat(iter_params.values(), keys = iter_params.keys(), axis=1)
         
         self.final_model = DistGARCH(
```

### Comparing `varfxi-0.0.3/varfxi/joyplot2.py` & `varfxi-0.0.4/varfxi/.ipynb_checkpoints/joyplot2-checkpoint.py`

 * *Files identical despite different names*

### Comparing `varfxi-0.0.3/varfxi/quantileproj.py` & `varfxi-0.0.4/varfxi/.ipynb_checkpoints/quantileproj-checkpoint.py`

 * *Files identical despite different names*

### Comparing `varfxi-0.0.3/PKG-INFO` & `varfxi-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varfxi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Volatility based estimation for FX interventions
 Home-page: https://github.com/romainlafarguette/varfxi
 Keywords: var,garch
 Author: romainlafarguette
 Author-email: romain.lafarguette@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
```

