# Comparing `tmp/pysurfline-0.0.3.tar.gz` & `tmp/pysurfline-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysurfline-0.0.3.tar", last modified: Thu Feb  9 00:31:03 2023, max compression
+gzip compressed data, was "pysurfline-0.0.4.tar", last modified: Thu Apr 20 11:09:35 2023, max compression
```

## Comparing `pysurfline-0.0.3.tar` & `pysurfline-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 00:31:03.783114 pysurfline-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-09 00:30:52.000000 pysurfline-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-02-09 00:31:03.779114 pysurfline-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-02-09 00:30:52.000000 pysurfline-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 00:31:03.779114 pysurfline-0.0.3/pysurfline/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-09 00:30:52.000000 pysurfline-0.0.3/pysurfline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-02-09 00:30:52.000000 pysurfline-0.0.3/pysurfline/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-02-09 00:30:52.000000 pysurfline-0.0.3/pysurfline/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-02-09 00:30:52.000000 pysurfline-0.0.3/pysurfline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 00:31:03.779114 pysurfline-0.0.3/pysurfline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-02-09 00:31:03.000000 pysurfline-0.0.3/pysurfline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-09 00:31:03.000000 pysurfline-0.0.3/pysurfline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 00:31:03.000000 pysurfline-0.0.3/pysurfline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-09 00:31:03.000000 pysurfline-0.0.3/pysurfline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-09 00:31:03.000000 pysurfline-0.0.3/pysurfline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 00:31:03.783114 pysurfline-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-02-09 00:30:52.000000 pysurfline-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 00:31:03.779114 pysurfline-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-02-09 00:30:52.000000 pysurfline-0.0.3/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:09:35.923449 pysurfline-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 11:09:22.000000 pysurfline-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-20 11:09:35.923449 pysurfline-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-20 11:09:22.000000 pysurfline-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:09:35.923449 pysurfline-0.0.4/pysurfline/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-20 11:09:22.000000 pysurfline-0.0.4/pysurfline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-20 11:09:22.000000 pysurfline-0.0.4/pysurfline/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-20 11:09:22.000000 pysurfline-0.0.4/pysurfline/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-20 11:09:22.000000 pysurfline-0.0.4/pysurfline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:09:35.923449 pysurfline-0.0.4/pysurfline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-20 11:09:35.000000 pysurfline-0.0.4/pysurfline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 11:09:35.000000 pysurfline-0.0.4/pysurfline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:09:35.000000 pysurfline-0.0.4/pysurfline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 11:09:35.000000 pysurfline-0.0.4/pysurfline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 11:09:35.000000 pysurfline-0.0.4/pysurfline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 11:09:35.923449 pysurfline-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-20 11:09:22.000000 pysurfline-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:09:35.923449 pysurfline-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-20 11:09:22.000000 pysurfline-0.0.4/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 11:09:22.000000 pysurfline-0.0.4/tests/test_utils.py
```

### Comparing `pysurfline-0.0.3/LICENSE` & `pysurfline-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysurfline-0.0.3/PKG-INFO` & `pysurfline-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysurfline
-Version: 0.0.3
+Version: 0.0.4
 Summary: python client to Surfline API
 Home-page: https://github.com/giocaizzi/pysurfline
 Author: giocaizzi
 Author-email: giocaizzi@gmail.com
 License: MIT
 Project-URL: Documentation, https://giocaizzi.github.io/pysurfline/
 Project-URL: Bug Reports, https://github.com/giocaizzi/pysurfline/issues
```

### Comparing `pysurfline-0.0.3/README.md` & `pysurfline-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pysurfline-0.0.3/pysurfline/core.py` & `pysurfline-0.0.4/pysurfline/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,18 +129,19 @@
         baseurl (str) : URL built by :obj:`pysurfline.URLBuilder` object.
         response (:obj:`requests.response`): A :obj:`request.response` object.
         type (str): type of forecast to get ( :obj:`wave`, :obj:`wind`,
             :obj:`tides`, :obj:`weather`)
         params (dict): dictonary for request of forecast parameters
     """
 
+    baseurl = "https://services.surfline.com/kbyg/spots/forecasts/"
+
     def __init__(self, type: str, params: dict):
         self.type = type
         self.params = params
-        self.baseurl = "https://services.surfline.com/kbyg/spots/forecasts/"
         self.response = requests.get(self.baseurl + self.type, params=params)
         self.url = self.response.url
 
     def __repr__(self):
         return f"ForecastGetter(Type:{self.type}, Status:{self.response.status_code})"
 
     def __str__(self):
```

### Comparing `pysurfline-0.0.3/pysurfline/reports.py` & `pysurfline-0.0.4/pysurfline/reports.py`

 * *Files identical despite different names*

### Comparing `pysurfline-0.0.3/pysurfline.egg-info/PKG-INFO` & `pysurfline-0.0.4/pysurfline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysurfline
-Version: 0.0.3
+Version: 0.0.4
 Summary: python client to Surfline API
 Home-page: https://github.com/giocaizzi/pysurfline
 Author: giocaizzi
 Author-email: giocaizzi@gmail.com
 License: MIT
 Project-URL: Documentation, https://giocaizzi.github.io/pysurfline/
 Project-URL: Bug Reports, https://github.com/giocaizzi/pysurfline/issues
```

### Comparing `pysurfline-0.0.3/setup.py` & `pysurfline-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pysurfline",
-    version="0.0.3",
+    version="0.0.4",
     description="python client to Surfline API",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/giocaizzi/pysurfline",
     author="giocaizzi",
     author_email="giocaizzi@gmail.com",
     license="MIT",
```

