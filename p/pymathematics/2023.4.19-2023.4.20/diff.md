# Comparing `tmp/pymathematics-2023.4.19.tar.gz` & `tmp/pymathematics-2023.4.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.19.tar", last modified: Wed Apr 19 10:26:51 2023, max compression
+gzip compressed data, was "pymathematics-2023.4.20.tar", last modified: Thu Apr 20 13:13:23 2023, max compression
```

## Comparing `pymathematics-2023.4.19.tar` & `pymathematics-2023.4.20.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-19 10:26:51.024355 pymathematics-2023.4.19/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.19/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-19 10:26:50.997290 pymathematics-2023.4.19/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       27 2023-04-18 17:29:05.000000 pymathematics-2023.4.19/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-19 10:26:50.463290 pymathematics-2023.4.19/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    14568 2023-04-19 09:30:51.000000 pymathematics-2023.4.19/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-18 17:28:53.000000 pymathematics-2023.4.19/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-19 10:26:50.797290 pymathematics-2023.4.19/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-19 10:26:47.000000 pymathematics-2023.4.19/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-19 10:26:47.000000 pymathematics-2023.4.19/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-19 10:26:47.000000 pymathematics-2023.4.19/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-19 10:26:47.000000 pymathematics-2023.4.19/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-19 10:26:51.027291 pymathematics-2023.4.19/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      689 2023-04-18 17:29:00.000000 pymathematics-2023.4.19/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-20 13:13:22.946279 pymathematics-2023.4.20/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.20/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-20 13:13:22.899279 pymathematics-2023.4.20/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      118 2023-04-20 13:03:45.000000 pymathematics-2023.4.20/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-20 13:13:22.562279 pymathematics-2023.4.20/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    15030 2023-04-20 13:00:09.000000 pymathematics-2023.4.20/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-20 13:02:21.000000 pymathematics-2023.4.20/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-20 13:13:22.809277 pymathematics-2023.4.20/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-20 13:13:19.000000 pymathematics-2023.4.20/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-20 13:13:19.000000 pymathematics-2023.4.20/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-20 13:13:19.000000 pymathematics-2023.4.20/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-20 13:13:19.000000 pymathematics-2023.4.20/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-20 13:13:22.950282 pymathematics-2023.4.20/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      689 2023-04-20 13:02:30.000000 pymathematics-2023.4.20/setup.py
```

### Comparing `pymathematics-2023.4.19/LICENSE` & `pymathematics-2023.4.20/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.19/pymathematics/__init__.py` & `pymathematics-2023.4.20/pymathematics/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from .info import (
-    author,version,homepage
-)
-
-author = author
-version = version
-homepage = homepage
+# from .info import (
+#     author,version,homepage
+# )
+
+# author = author
+# version = version
+# homepage = homepage
 
 class constants:
     pi = 3.1415926535897932384626433832795
     e = 2.7182818284590452353602874713527
 
 class vector:
     def cross_product(vector1:list,vector2:list) -> int|float:
@@ -147,16 +147,19 @@
         x2 = f"{-coefficients[1]} - {sqrt(absolute(D))}i"
         return [x1,x2]
     x1 = -coefficients[1]+sqrt(D)
     x2 = -coefficients[1]-sqrt(D)
     return [x1,x2]
 
 def log(number:int|float) -> float:
+    """
+    `log(number) to the base 10`
+    """
     if number <= 0:
-        return "invalid input!"
+        raise ValueError("domain error")
     else:
         n = 0
         while number >= 10:
             number /= 10
             n += 1
         if number == 1:
             return n
@@ -172,16 +175,29 @@
                     left = mid
                 else:
                     right = mid
             return n+left
 
 
 def ln(number:int|float) -> int|float:
+    """
+    `log(number) to the base e`
+    """
+    if number <= 0:
+        raise ValueError("domain error")
     return 2.303*log(number)
 
+def logn(number:int|float,base:int|float = constants.e) -> int|float:
+    """
+    `log(number) to the base n(user defined)`
+    """
+    if number <= 0 or base <= 0 or base == 1:
+        raise ValueError("domain error")
+    return 2.303*log(number)/(2.303*log(base))
+
 def summation(array:list) -> list:
     sigma = 0
     for x in array:
         sigma += x
     return sigma
 
 def product(array:list) -> list:
```

### Comparing `pymathematics-2023.4.19/setup.py` & `pymathematics-2023.4.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.4.19",
+    version = "2023.4.20",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```

