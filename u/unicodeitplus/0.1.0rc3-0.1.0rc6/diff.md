# Comparing `tmp/unicodeitplus-0.1.0rc3.tar.gz` & `tmp/unicodeitplus-0.1.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicodeitplus-0.1.0rc3.tar", last modified: Thu Apr 20 10:12:35 2023, max compression
+gzip compressed data, was "unicodeitplus-0.1.0rc6.tar", last modified: Thu Apr 20 10:35:18 2023, max compression
```

## Comparing `unicodeitplus-0.1.0rc3.tar` & `unicodeitplus-0.1.0rc6.tar`

### file list

```diff
@@ -1,47 +1,31 @@
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2023-04-20 10:12:35.486782 unicodeitplus-0.1.0rc3/
--rw-r--r--   0 hdembinski   (501) staff       (20)     3586 2023-04-20 07:45:29.952960 unicodeitplus-0.1.0rc3/CONTRIBUTING.rst
--rw-r--r--   0 hdembinski   (501) staff       (20)       89 2023-04-15 14:45:18.124248 unicodeitplus-0.1.0rc3/HISTORY.rst
--rw-r--r--   0 hdembinski   (501) staff       (20)     1792 2023-04-20 10:12:35.368814 unicodeitplus-0.1.0rc3/LICENSE
--rw-r--r--   0 hdembinski   (501) staff       (20)     1135 2023-04-20 07:45:29.953562 unicodeitplus-0.1.0rc3/Makefile
--rw-r--r--   0 hdembinski   (501) staff       (20)     4598 2023-04-20 10:12:35.487093 unicodeitplus-0.1.0rc3/PKG-INFO
--rw-r--r--   0 hdembinski   (501) staff       (20)     3901 2023-04-20 09:54:52.610002 unicodeitplus-0.1.0rc3/README.rst
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2023-04-20 10:12:35.470274 unicodeitplus-0.1.0rc3/docs/
--rw-r--r--   0 hdembinski   (501) staff       (20)      614 2023-04-20 07:45:29.953053 unicodeitplus-0.1.0rc3/docs/Makefile
--rwxr-xr-x   0 hdembinski   (501) staff       (20)     3441 2023-04-20 07:45:30.516384 unicodeitplus-0.1.0rc3/docs/conf.py
--rw-r--r--   0 hdembinski   (501) staff       (20)       33 2023-04-15 14:45:18.150401 unicodeitplus-0.1.0rc3/docs/contributing.rst
--rw-r--r--   0 hdembinski   (501) staff       (20)       28 2023-04-15 14:45:18.161248 unicodeitplus-0.1.0rc3/docs/history.rst
--rw-r--r--   0 hdembinski   (501) staff       (20)      283 2023-04-20 07:45:29.953099 unicodeitplus-0.1.0rc3/docs/index.rst
--rw-r--r--   0 hdembinski   (501) staff       (20)       27 2023-04-15 14:45:18.168847 unicodeitplus-0.1.0rc3/docs/readme.rst
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2023-04-20 10:12:35.471855 unicodeitplus-0.1.0rc3/extern/
--rw-r--r--   0 hdembinski   (501) staff       (20)    19035 2023-04-20 08:01:21.072676 unicodeitplus-0.1.0rc3/extern/LICENSE.LPPL
--rw-r--r--   0 hdembinski   (501) staff       (20)   216332 2023-04-09 10:55:07.062953 unicodeitplus-0.1.0rc3/extern/unimathsymbols.txt
--rw-r--r--   0 hdembinski   (501) staff       (20)     1537 2023-04-20 07:59:59.840576 unicodeitplus-0.1.0rc3/pyproject.toml
--rw-r--r--   0 hdembinski   (501) staff       (20)      943 2023-04-20 07:05:56.499193 unicodeitplus-0.1.0rc3/setup.py
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2023-04-20 10:12:35.462402 unicodeitplus-0.1.0rc3/src/
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2023-04-20 10:12:35.476242 unicodeitplus-0.1.0rc3/src/unicodeitplus/
--rw-r--r--   0 hdembinski   (501) staff       (20)      765 2023-04-20 09:20:16.023956 unicodeitplus-0.1.0rc3/src/unicodeitplus/__init__.py
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2023-04-20 10:12:35.484652 unicodeitplus-0.1.0rc3/src/unicodeitplus/__pycache__/
--rw-r--r--   0 hdembinski   (501) staff       (20)     1078 2023-04-20 09:20:16.738071 unicodeitplus-0.1.0rc3/src/unicodeitplus/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 hdembinski   (501) staff       (20)     3481 2023-04-20 10:00:35.118194 unicodeitplus-0.1.0rc3/src/unicodeitplus/__pycache__/_make_data.cpython-310.pyc
--rw-r--r--   0 hdembinski   (501) staff       (20)   190032 2023-04-20 10:00:35.890132 unicodeitplus-0.1.0rc3/src/unicodeitplus/__pycache__/data.cpython-310.pyc
--rw-r--r--   0 hdembinski   (501) staff       (20)      716 2023-04-20 08:10:42.357071 unicodeitplus-0.1.0rc3/src/unicodeitplus/__pycache__/parser.cpython-310.pyc
--rw-r--r--   0 hdembinski   (501) staff       (20)     2558 2023-04-20 09:04:20.366215 unicodeitplus-0.1.0rc3/src/unicodeitplus/__pycache__/transform.cpython-310.pyc
--rw-r--r--   0 hdembinski   (501) staff       (20)     4505 2023-04-20 10:00:34.183664 unicodeitplus-0.1.0rc3/src/unicodeitplus/_make_data.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      411 2023-04-20 08:18:22.141620 unicodeitplus-0.1.0rc3/src/unicodeitplus/cli.py
--rw-r--r--   0 hdembinski   (501) staff       (20)    69374 2023-04-20 10:11:50.229415 unicodeitplus-0.1.0rc3/src/unicodeitplus/data.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      540 2023-04-20 08:10:41.737201 unicodeitplus-0.1.0rc3/src/unicodeitplus/parser.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     3711 2023-04-20 09:04:19.617237 unicodeitplus-0.1.0rc3/src/unicodeitplus/transform.py
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2023-04-20 10:12:35.480735 unicodeitplus-0.1.0rc3/src/unicodeitplus.egg-info/
--rw-r--r--   0 hdembinski   (501) staff       (20)     4598 2023-04-20 10:12:35.412974 unicodeitplus-0.1.0rc3/src/unicodeitplus.egg-info/PKG-INFO
--rw-r--r--   0 hdembinski   (501) staff       (20)     1154 2023-04-20 10:12:35.455931 unicodeitplus-0.1.0rc3/src/unicodeitplus.egg-info/SOURCES.txt
--rw-r--r--   0 hdembinski   (501) staff       (20)        1 2023-04-20 10:12:35.413455 unicodeitplus-0.1.0rc3/src/unicodeitplus.egg-info/dependency_links.txt
--rw-r--r--   0 hdembinski   (501) staff       (20)       57 2023-04-20 10:12:35.413968 unicodeitplus-0.1.0rc3/src/unicodeitplus.egg-info/entry_points.txt
--rw-r--r--   0 hdembinski   (501) staff       (20)        1 2023-04-20 10:02:51.521879 unicodeitplus-0.1.0rc3/src/unicodeitplus.egg-info/not-zip-safe
--rw-r--r--   0 hdembinski   (501) staff       (20)       20 2023-04-20 10:12:35.414287 unicodeitplus-0.1.0rc3/src/unicodeitplus.egg-info/requires.txt
--rw-r--r--   0 hdembinski   (501) staff       (20)       14 2023-04-20 10:12:35.414671 unicodeitplus-0.1.0rc3/src/unicodeitplus.egg-info/top_level.txt
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2023-04-20 10:12:35.485295 unicodeitplus-0.1.0rc3/tests/
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2023-04-20 10:12:35.485998 unicodeitplus-0.1.0rc3/tests/__pycache__/
--rw-r--r--   0 hdembinski   (501) staff       (20)     2829 2023-04-20 09:20:59.247153 unicodeitplus-0.1.0rc3/tests/__pycache__/test_latex.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0 hdembinski   (501) staff       (20)     1967 2023-04-20 09:20:58.471792 unicodeitplus-0.1.0rc3/tests/test_latex.py
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2023-04-20 10:12:35.486647 unicodeitplus-0.1.0rc3/tools/
--rw-r--r--   0 hdembinski   (501) staff       (20)      744 2023-04-20 09:35:02.751250 unicodeitplus-0.1.0rc3/tools/generate_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:18.092018 unicodeitplus-0.1.0rc6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-20 10:35:03.107915 unicodeitplus-0.1.0rc6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 10:35:03.107915 unicodeitplus-0.1.0rc6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-20 10:35:18.052017 unicodeitplus-0.1.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-20 10:35:03.107915 unicodeitplus-0.1.0rc6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-20 10:35:18.092018 unicodeitplus-0.1.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-20 10:35:03.107915 unicodeitplus-0.1.0rc6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:18.092018 unicodeitplus-0.1.0rc6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-20 10:35:03.107915 unicodeitplus-0.1.0rc6/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3441 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:18.092018 unicodeitplus-0.1.0rc6/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)    19035 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/extern/LICENSE.LPPL
+-rw-r--r--   0 runner    (1001) docker     (123)   216332 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/extern/unimathsymbols.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:18.088018 unicodeitplus-0.1.0rc6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:18.092018 unicodeitplus-0.1.0rc6/src/unicodeitplus/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/src/unicodeitplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/src/unicodeitplus/_make_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/src/unicodeitplus/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69374 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/src/unicodeitplus/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/src/unicodeitplus/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/src/unicodeitplus/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:18.092018 unicodeitplus-0.1.0rc6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/tests/test_latex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:18.092018 unicodeitplus-0.1.0rc6/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-20 10:35:03.111914 unicodeitplus-0.1.0rc6/tools/generate_examples.py
```

### Comparing `unicodeitplus-0.1.0rc3/CONTRIBUTING.rst` & `unicodeitplus-0.1.0rc6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/LICENSE` & `unicodeitplus-0.1.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/Makefile` & `unicodeitplus-0.1.0rc6/Makefile`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/PKG-INFO` & `unicodeitplus-0.1.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodeitplus
-Version: 0.1.0rc3
+Version: 0.1.0rc6
 Summary: Converts simple LaTeX to an unicode approximation
 Maintainer: Hans Dembinski
 Maintainer-email: hans.dembinski@gmail.com
 License: BSD 3-Clause License
 Project-URL: repository, https://github.com/HDembinski/unicodeitplus
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `unicodeitplus-0.1.0rc3/README.rst` & `unicodeitplus-0.1.0rc6/README.rst`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/docs/Makefile` & `unicodeitplus-0.1.0rc6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/docs/conf.py` & `unicodeitplus-0.1.0rc6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/extern/LICENSE.LPPL` & `unicodeitplus-0.1.0rc6/extern/LICENSE.LPPL`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/extern/unimathsymbols.txt` & `unicodeitplus-0.1.0rc6/extern/unimathsymbols.txt`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/pyproject.toml` & `unicodeitplus-0.1.0rc6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-q -ra --ff"
 testpaths = ["tests"]
 xfail_strict = true
 filterwarnings = [
     "error::DeprecationWarning",
-    "error::numpy.VisibleDeprecationWarning",
 ]
 
 [tool.coverage.run]
 relative_files = true
 source = ["unicodeitplus"]
 
 [tool.coverage.report]
```

### Comparing `unicodeitplus-0.1.0rc3/setup.py` & `unicodeitplus-0.1.0rc6/setup.py`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/src/unicodeitplus/__init__.py` & `unicodeitplus-0.1.0rc6/src/unicodeitplus/__init__.py`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/src/unicodeitplus/_make_data.py` & `unicodeitplus-0.1.0rc6/src/unicodeitplus/_make_data.py`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/src/unicodeitplus/data.py` & `unicodeitplus-0.1.0rc6/src/unicodeitplus/data.py`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/src/unicodeitplus/parser.py` & `unicodeitplus-0.1.0rc6/src/unicodeitplus/parser.py`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/src/unicodeitplus/transform.py` & `unicodeitplus-0.1.0rc6/src/unicodeitplus/transform.py`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/tests/test_latex.py` & `unicodeitplus-0.1.0rc6/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `unicodeitplus-0.1.0rc3/tools/generate_examples.py` & `unicodeitplus-0.1.0rc6/tools/generate_examples.py`

 * *Files identical despite different names*

