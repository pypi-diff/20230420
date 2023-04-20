# Comparing `tmp/dxlib-0.1.0.tar.gz` & `tmp/dxlib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxlib-0.1.0.tar", last modified: Thu Apr 20 13:33:49 2023, max compression
+gzip compressed data, was "dxlib-0.1.1.tar", last modified: Thu Apr 20 14:52:20 2023, max compression
```

## Comparing `dxlib-0.1.0.tar` & `dxlib-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-20 13:41:15.835040 dxlib-0.1.0/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-04-20 13:41:15.830031 dxlib-0.1.0/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      526 2023-04-20 12:53:37.000000 dxlib-0.1.0/README.md
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-20 13:41:15.658419 dxlib-0.1.0/dxlib/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       57 2023-04-20 12:46:06.000000 dxlib-0.1.0/dxlib/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      307 2023-04-20 12:56:26.000000 dxlib-0.1.0/dxlib/finite_differences.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-20 13:41:15.798431 dxlib-0.1.0/dxlib.egg-info/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-04-20 13:41:15.000000 dxlib-0.1.0/dxlib.egg-info/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      208 2023-04-20 13:41:15.000000 dxlib-0.1.0/dxlib.egg-info/SOURCES.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-04-20 13:41:15.000000 dxlib-0.1.0/dxlib.egg-info/dependency_links.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       17 2023-04-20 13:41:15.000000 dxlib-0.1.0/dxlib.egg-info/requires.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-04-20 13:41:15.000000 dxlib-0.1.0/dxlib.egg-info/top_level.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-04-20 13:41:15.835040 dxlib-0.1.0/setup.cfg
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1400 2023-04-20 13:41:13.000000 dxlib-0.1.0/setup.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-20 14:53:44.377639 dxlib-0.1.1/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-04-20 14:53:44.377639 dxlib-0.1.1/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      526 2023-04-20 14:34:27.000000 dxlib-0.1.1/README.md
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-20 14:53:44.205763 dxlib-0.1.1/dxlib/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      102 2023-04-20 14:41:28.000000 dxlib-0.1.1/dxlib/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      404 2023-04-20 14:41:16.000000 dxlib-0.1.1/dxlib/euler_method.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      274 2023-04-20 14:39:35.000000 dxlib-0.1.1/dxlib/finite_differences.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-20 14:53:44.346383 dxlib-0.1.1/dxlib.egg-info/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-04-20 14:53:43.000000 dxlib-0.1.1/dxlib.egg-info/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      230 2023-04-20 14:53:44.000000 dxlib-0.1.1/dxlib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-04-20 14:53:43.000000 dxlib-0.1.1/dxlib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       17 2023-04-20 14:53:43.000000 dxlib-0.1.1/dxlib.egg-info/requires.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-04-20 14:53:43.000000 dxlib-0.1.1/dxlib.egg-info/top_level.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-04-20 14:53:44.377639 dxlib-0.1.1/setup.cfg
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1400 2023-04-20 14:52:57.000000 dxlib-0.1.1/setup.py
```

### Comparing `dxlib-0.1.0/PKG-INFO` & `dxlib-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.1.0/README.md` & `dxlib-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dxlib-0.1.0/dxlib.egg-info/PKG-INFO` & `dxlib-0.1.1/dxlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.1.0/setup.py` & `dxlib-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to self.setup() does all the work
 setup(
     name="dxlib",
-    version="0.1.0",
+    version="0.1.1",
     description="Quantitative Methods for Finance",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/delphos-quant/dxlib",
     author="Rafael Zimmer",
     author_email="rzimmerde@gmail.com",
     license="MIT",
```

