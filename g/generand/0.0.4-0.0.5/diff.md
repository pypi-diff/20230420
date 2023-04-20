# Comparing `tmp/generand-0.0.4.tar.gz` & `tmp/generand-0.0.5.tar.gz`

## Comparing `generand-0.0.4.tar` & `generand-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 generand-0.0.4/Python.gitignore
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 generand-0.0.4/Tests.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 generand-0.0.4/.vscode/launch.json
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 generand-0.0.4/src/generand/Bernoulli.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 generand-0.0.4/src/generand/Binomial.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 generand-0.0.4/src/generand/Exponential.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 generand-0.0.4/src/generand/Poisson.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 generand-0.0.4/src/generand/Triangular.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 generand-0.0.4/src/generand/Uniform.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 generand-0.0.4/src/generand/Weibull.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 generand-0.0.4/src/generand/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 generand-0.0.4/LICENSE
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 generand-0.0.4/README.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 generand-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 generand-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 generand-0.0.5/Python.gitignore
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 generand-0.0.5/Tests.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 generand-0.0.5/.vscode/launch.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/__init__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/bernoulli.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/binomial.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/exponential.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/poisson.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/triangular.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/uniform.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/weibull.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 generand-0.0.5/LICENSE
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 generand-0.0.5/README.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 generand-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 generand-0.0.5/PKG-INFO
```

### Comparing `generand-0.0.4/Python.gitignore` & `generand-0.0.5/Python.gitignore`

 * *Files identical despite different names*

### Comparing `generand-0.0.4/Tests.py` & `generand-0.0.5/Tests.py`

 * *Files identical despite different names*

### Comparing `generand-0.0.4/src/generand/Poisson.py` & `generand-0.0.5/src/generand/poisson.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import Uniform
+from .uniform import Uniform
 import time
 import math
+class Poisson:
 
-    
-# def generate(self, alpha= 1 , count= 1):
-#     """Generates pseudo poisson random numbers using A-R method"""
-#     poisson = []
-#     for i in range(count):
-#         x = -1
-#         p = 1
-#         while p >= math.exp(-alpha):
-#             u = Uniform().generate()
-#             x+=1
-#             p = u[0]*p
-#         poisson.append(x)
-#     return poisson
+    """Generates pseudo poisson random numbers using A-R method"""
+    # def generate(self, alpha= 1 , count= 1):
+    #     poisson = []
+    #     for i in range(count):
+    #         x = -1
+    #         p = 1
+    #         while p >= math.exp(-alpha):
+    #             u = Uniform(time.perf_counter_ns()).generate()
+    #             x+=1
+    #             p = u[0]*p
+    #         poisson.append(x)
+    #     return poisson
 
-def generate(alpha= 1 , count= 1):
-    poissons = []
-    for _ in range(count):
-        
-        x = 0
-        p = 1
-        i= 0
-        u = Uniform.generate(time.perf_counter_ns(), 10*alpha)
-        while p >= math.exp(-alpha):
+    def generate(self, alpha= 1 , count= 1):
+        poisson = []
+        for _ in range(count):
             
-            x+=1
-            p = u[i]*p
-            i+=1
-        poissons.append(x)
-    return poissons
+            x = 0
+            p = 1
+            i= 0
+            u = Uniform(time.perf_counter_ns()).generate(5*alpha)
+            while p >= math.exp(-alpha):
+                
+                x+=1
+                p = u[i]*p
+                i+=1
+            poisson.append(x)
+        return poisson
```

### Comparing `generand-0.0.4/LICENSE` & `generand-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `generand-0.0.4/pyproject.toml` & `generand-0.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "generand"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="rajat maheshwari", email="rajt.maheshwari30@gmail.com" },
 ]
 description = "A package to generate random numbers from various distributions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `generand-0.0.4/PKG-INFO` & `generand-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generand
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to generate random numbers from various distributions
 Project-URL: Homepage, https://github.com/pypa/generand
 Project-URL: Bug Tracker, https://github.com/pypa/generand/issues
 Author-email: rajat maheshwari <rajt.maheshwari30@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

