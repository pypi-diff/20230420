# Comparing `tmp/asyncsleepiq-1.3.2.tar.gz` & `tmp/asyncsleepiq-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncsleepiq-1.3.2.tar", last modified: Wed Apr 19 21:54:18 2023, max compression
+gzip compressed data, was "asyncsleepiq-1.3.3.tar", last modified: Thu Apr 20 18:36:15 2023, max compression
```

## Comparing `asyncsleepiq-1.3.2.tar` & `asyncsleepiq-1.3.3.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:54:18.834859 asyncsleepiq-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-19 21:54:01.000000 asyncsleepiq-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-19 21:54:18.830859 asyncsleepiq-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-19 21:54:01.000000 asyncsleepiq-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:54:18.830859 asyncsleepiq-1.3.2/asyncsleepiq/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-19 21:54:10.000000 asyncsleepiq-1.3.2/asyncsleepiq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-19 21:54:01.000000 asyncsleepiq-1.3.2/asyncsleepiq/actuator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-19 21:54:01.000000 asyncsleepiq-1.3.2/asyncsleepiq/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-19 21:54:01.000000 asyncsleepiq-1.3.2/asyncsleepiq/asyncsleepiq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-19 21:54:01.000000 asyncsleepiq-1.3.2/asyncsleepiq/bed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-19 21:54:01.000000 asyncsleepiq-1.3.2/asyncsleepiq/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-19 21:54:01.000000 asyncsleepiq-1.3.2/asyncsleepiq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-19 21:54:01.000000 asyncsleepiq-1.3.2/asyncsleepiq/foundation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-19 21:54:01.000000 asyncsleepiq-1.3.2/asyncsleepiq/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-19 21:54:01.000000 asyncsleepiq-1.3.2/asyncsleepiq/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:54:01.000000 asyncsleepiq-1.3.2/asyncsleepiq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-19 21:54:01.000000 asyncsleepiq-1.3.2/asyncsleepiq/sleeper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:54:18.830859 asyncsleepiq-1.3.2/asyncsleepiq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-19 21:54:18.000000 asyncsleepiq-1.3.2/asyncsleepiq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-19 21:54:18.000000 asyncsleepiq-1.3.2/asyncsleepiq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:54:18.000000 asyncsleepiq-1.3.2/asyncsleepiq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-19 21:54:18.000000 asyncsleepiq-1.3.2/asyncsleepiq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 21:54:18.000000 asyncsleepiq-1.3.2/asyncsleepiq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 21:54:18.834859 asyncsleepiq-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-19 21:54:10.000000 asyncsleepiq-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:15.463537 asyncsleepiq-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-20 18:36:15.463537 asyncsleepiq-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:15.463537 asyncsleepiq-1.3.3/asyncsleepiq/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-20 18:36:08.000000 asyncsleepiq-1.3.3/asyncsleepiq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/actuator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/asyncsleepiq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/bed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/foundation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:15.463537 asyncsleepiq-1.3.3/asyncsleepiq/fuzion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/fuzion/actuator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/fuzion/bed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/fuzion/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/fuzion/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/fuzion/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/fuzion/sleeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/sleeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:15.463537 asyncsleepiq-1.3.3/asyncsleepiq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-20 18:36:15.000000 asyncsleepiq-1.3.3/asyncsleepiq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-20 18:36:15.000000 asyncsleepiq-1.3.3/asyncsleepiq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:36:15.000000 asyncsleepiq-1.3.3/asyncsleepiq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-20 18:36:15.000000 asyncsleepiq-1.3.3/asyncsleepiq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 18:36:15.000000 asyncsleepiq-1.3.3/asyncsleepiq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 18:36:15.463537 asyncsleepiq-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-20 18:36:08.000000 asyncsleepiq-1.3.3/setup.py
```

### Comparing `asyncsleepiq-1.3.2/LICENSE` & `asyncsleepiq-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.2/PKG-INFO` & `asyncsleepiq-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncsleepiq
-Version: 1.3.2
+Version: 1.3.3
 Summary: ASync SleepIQ API
 Home-page: http://github.com/kbickar/asyncsleepiq
 Author: Keilin Bickar
 Author-email: trumpetgod@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `asyncsleepiq-1.3.2/README.md` & `asyncsleepiq-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.2/asyncsleepiq/actuator.py` & `asyncsleepiq-1.3.3/asyncsleepiq/actuator.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.2/asyncsleepiq/api.py` & `asyncsleepiq-1.3.3/asyncsleepiq/api.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.2/asyncsleepiq/asyncsleepiq.py` & `asyncsleepiq-1.3.3/asyncsleepiq/asyncsleepiq.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.2/asyncsleepiq/bed.py` & `asyncsleepiq-1.3.3/asyncsleepiq/bed.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.2/asyncsleepiq/consts.py` & `asyncsleepiq-1.3.3/asyncsleepiq/consts.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.2/asyncsleepiq/foundation.py` & `asyncsleepiq-1.3.3/asyncsleepiq/foundation.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.2/asyncsleepiq/light.py` & `asyncsleepiq-1.3.3/asyncsleepiq/light.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.2/asyncsleepiq/preset.py` & `asyncsleepiq-1.3.3/asyncsleepiq/preset.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.2/asyncsleepiq/sleeper.py` & `asyncsleepiq-1.3.3/asyncsleepiq/sleeper.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.2/asyncsleepiq.egg-info/PKG-INFO` & `asyncsleepiq-1.3.3/asyncsleepiq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncsleepiq
-Version: 1.3.2
+Version: 1.3.3
 Summary: ASync SleepIQ API
 Home-page: http://github.com/kbickar/asyncsleepiq
 Author: Keilin Bickar
 Author-email: trumpetgod@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `asyncsleepiq-1.3.2/setup.py` & `asyncsleepiq-1.3.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
 setup(
     name="asyncsleepiq",
-    packages=["asyncsleepiq"],
+    packages=["asyncsleepiq", "asyncsleepiq.fuzion"],
     package_data={"asyncsleepiq": ["py.typed"]},
-    version="1.3.2",
+    version="1.3.3",
     description="ASync SleepIQ API",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="http://github.com/kbickar/asyncsleepiq",
     author="Keilin Bickar",
     author_email="trumpetgod@gmail.com",
     license="MIT",
```

