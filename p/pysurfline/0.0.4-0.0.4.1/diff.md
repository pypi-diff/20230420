# Comparing `tmp/pysurfline-0.0.4.tar.gz` & `tmp/pysurfline-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysurfline-0.0.4.tar", last modified: Thu Apr 20 11:09:35 2023, max compression
+gzip compressed data, was "pysurfline-0.0.4.1.tar", last modified: Thu Apr 20 11:41:18 2023, max compression
```

## Comparing `pysurfline-0.0.4.tar` & `pysurfline-0.0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:09:35.923449 pysurfline-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 11:09:22.000000 pysurfline-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-20 11:09:35.923449 pysurfline-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-20 11:09:22.000000 pysurfline-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:09:35.923449 pysurfline-0.0.4/pysurfline/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-20 11:09:22.000000 pysurfline-0.0.4/pysurfline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-20 11:09:22.000000 pysurfline-0.0.4/pysurfline/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-20 11:09:22.000000 pysurfline-0.0.4/pysurfline/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-20 11:09:22.000000 pysurfline-0.0.4/pysurfline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:09:35.923449 pysurfline-0.0.4/pysurfline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-20 11:09:35.000000 pysurfline-0.0.4/pysurfline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 11:09:35.000000 pysurfline-0.0.4/pysurfline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:09:35.000000 pysurfline-0.0.4/pysurfline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 11:09:35.000000 pysurfline-0.0.4/pysurfline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 11:09:35.000000 pysurfline-0.0.4/pysurfline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 11:09:35.923449 pysurfline-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-20 11:09:22.000000 pysurfline-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:09:35.923449 pysurfline-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-20 11:09:22.000000 pysurfline-0.0.4/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 11:09:22.000000 pysurfline-0.0.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:18.679029 pysurfline-0.0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 11:41:03.000000 pysurfline-0.0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-20 11:41:18.679029 pysurfline-0.0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-20 11:41:03.000000 pysurfline-0.0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:18.675028 pysurfline-0.0.4.1/pysurfline/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-20 11:41:03.000000 pysurfline-0.0.4.1/pysurfline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-20 11:41:03.000000 pysurfline-0.0.4.1/pysurfline/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-20 11:41:03.000000 pysurfline-0.0.4.1/pysurfline/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-20 11:41:03.000000 pysurfline-0.0.4.1/pysurfline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:18.675028 pysurfline-0.0.4.1/pysurfline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-20 11:41:18.000000 pysurfline-0.0.4.1/pysurfline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 11:41:18.000000 pysurfline-0.0.4.1/pysurfline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:41:18.000000 pysurfline-0.0.4.1/pysurfline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 11:41:18.000000 pysurfline-0.0.4.1/pysurfline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 11:41:18.000000 pysurfline-0.0.4.1/pysurfline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 11:41:18.679029 pysurfline-0.0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-20 11:41:03.000000 pysurfline-0.0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:18.679029 pysurfline-0.0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-20 11:41:03.000000 pysurfline-0.0.4.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 11:41:03.000000 pysurfline-0.0.4.1/tests/test_utils.py
```

### Comparing `pysurfline-0.0.4/LICENSE` & `pysurfline-0.0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysurfline-0.0.4/PKG-INFO` & `pysurfline-0.0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pysurfline
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: python client to Surfline API
 Home-page: https://github.com/giocaizzi/pysurfline
 Author: giocaizzi
 Author-email: giocaizzi@gmail.com
 License: MIT
 Project-URL: Documentation, https://giocaizzi.github.io/pysurfline/
 Project-URL: Bug Reports, https://github.com/giocaizzi/pysurfline/issues
 Project-URL: Source, https://github.com/giocaizzi/pysurfline
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 # pysurfline
```

### Comparing `pysurfline-0.0.4/README.md` & `pysurfline-0.0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pysurfline-0.0.4/pysurfline/core.py` & `pysurfline-0.0.4.1/pysurfline/core.py`

 * *Files identical despite different names*

### Comparing `pysurfline-0.0.4/pysurfline/reports.py` & `pysurfline-0.0.4.1/pysurfline/reports.py`

 * *Files identical despite different names*

### Comparing `pysurfline-0.0.4/pysurfline/utils.py` & `pysurfline-0.0.4.1/pysurfline/utils.py`

 * *Files identical despite different names*

### Comparing `pysurfline-0.0.4/pysurfline.egg-info/PKG-INFO` & `pysurfline-0.0.4.1/pysurfline.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pysurfline
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: python client to Surfline API
 Home-page: https://github.com/giocaizzi/pysurfline
 Author: giocaizzi
 Author-email: giocaizzi@gmail.com
 License: MIT
 Project-URL: Documentation, https://giocaizzi.github.io/pysurfline/
 Project-URL: Bug Reports, https://github.com/giocaizzi/pysurfline/issues
 Project-URL: Source, https://github.com/giocaizzi/pysurfline
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 # pysurfline
```

### Comparing `pysurfline-0.0.4/setup.py` & `pysurfline-0.0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pysurfline",
-    version="0.0.4",
+    version="0.0.4.1",
     description="python client to Surfline API",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/giocaizzi/pysurfline",
     author="giocaizzi",
     author_email="giocaizzi@gmail.com",
     license="MIT",
@@ -30,14 +30,16 @@
     },
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+
     ],
     project_urls={
         "Documentation": "https://giocaizzi.github.io/pysurfline/",
         "Bug Reports": "https://github.com/giocaizzi/pysurfline/issues",
         "Source": "https://github.com/giocaizzi/pysurfline",
     },
 )
```

### Comparing `pysurfline-0.0.4/tests/test_core.py` & `pysurfline-0.0.4.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pysurfline-0.0.4/tests/test_utils.py` & `pysurfline-0.0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

