# Comparing `tmp/bfrac-0.0.52.tar.gz` & `tmp/bfrac-0.0.53.tar.gz`

## Comparing `bfrac-0.0.52.tar` & `bfrac-0.0.53.tar`

### file list

```diff
@@ -1,16 +1,21 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bfrac-0.0.52/example_config.ini
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bfrac-0.0.52/bfrac/__about__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bfrac-0.0.52/bfrac/__init__.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 bfrac-0.0.52/bfrac/app_config.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 bfrac-0.0.52/bfrac/match_info_object.py
--rw-r--r--   0        0        0     8079 2020-02-02 00:00:00.000000 bfrac-0.0.52/bfrac/query_context.py
--rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 bfrac-0.0.52/bfrac/riot_api_caller.py
--rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 bfrac-0.0.52/bfrac/riot_api_helper.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 bfrac-0.0.52/tests/context.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bfrac-0.0.52/tests/simple_test.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 bfrac-0.0.52/tests/tester.ipynb
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 bfrac-0.0.52/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 bfrac-0.0.52/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bfrac-0.0.52/README.md
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 bfrac-0.0.52/pyproject.toml
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 bfrac-0.0.52/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bfrac-0.0.53/example_config.ini
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bfrac-0.0.53/bfrac/__about__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bfrac-0.0.53/bfrac/__init__.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 bfrac-0.0.53/bfrac/app_config.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 bfrac-0.0.53/bfrac/match_info_object.py
+-rw-r--r--   0        0        0     8290 2020-02-02 00:00:00.000000 bfrac-0.0.53/bfrac/query_context.py
+-rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 bfrac-0.0.53/bfrac/riot_api_caller.py
+-rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 bfrac-0.0.53/bfrac/riot_api_helper.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bfrac-0.0.53/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 bfrac-0.0.53/docs/make.bat
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bfrac-0.0.53/docs/source/conf.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 bfrac-0.0.53/docs/source/index.rst
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bfrac-0.0.53/docs/source/usage.rst
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 bfrac-0.0.53/tests/context.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bfrac-0.0.53/tests/simple_test.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 bfrac-0.0.53/tests/tester.ipynb
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 bfrac-0.0.53/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 bfrac-0.0.53/LICENSE
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bfrac-0.0.53/README.md
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 bfrac-0.0.53/pyproject.toml
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 bfrac-0.0.53/PKG-INFO
```

### Comparing `bfrac-0.0.52/bfrac/app_config.py` & `bfrac-0.0.53/bfrac/app_config.py`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.52/bfrac/query_context.py` & `bfrac-0.0.53/bfrac/query_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,7 +177,11 @@
 
         Returns
         -------
             JSON like data structure containing match_info
         """
         match_info = RiotAPIHelper.get_match_info(self.riot_api_caller, self.region_continent, in_match_id)
         return match_info
+
+    def get_match_timeline(self, in_match_id: str) -> dict:
+        match_timeline = RiotAPIHelper.get_match_timeline(self.riot_api_caller, self.region_continent, in_match_id)
+        return match_timeline
```

### Comparing `bfrac-0.0.52/bfrac/riot_api_caller.py` & `bfrac-0.0.53/bfrac/riot_api_caller.py`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.52/bfrac/riot_api_helper.py` & `bfrac-0.0.53/bfrac/riot_api_helper.py`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.52/tests/tester.ipynb` & `bfrac-0.0.53/tests/tester.ipynb`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.52/.gitignore` & `bfrac-0.0.53/.gitignore`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.52/LICENSE` & `bfrac-0.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.52/pyproject.toml` & `bfrac-0.0.53/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.52/PKG-INFO` & `bfrac-0.0.53/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfrac
-Version: 0.0.52
+Version: 0.0.53
 Summary: Beginner Friendly Riot API Caller is a simple wrapper for RiotAPI with rate maintenance built in.
 Project-URL: Documentation, https://github.com/deamonpog/bfrac#readme
 Project-URL: Issues, https://github.com/deamonpog/bfrac/issues
 Project-URL: Source, https://github.com/deamonpog/bfrac
 Author-email: deamonpog <pog666@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -18,8 +18,26 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Beginner Friendly Riot API Caller (bfrac)
 
-This is a python wrapper for RiotAPI with rate maintenance built in.
+This is a python wrapper for RiotAPI with rate maintenance built in.
+
+-----
+
+**Table of Contents**
+
+- [Installation](#installation)
+- [License](#license)
+
+## Installation
+
+```console
+pip install bfrac
+```
+## License
+
+MIT License
+
+Copyright (c) 2023 Chathura Jayalath (deamonpog)
```

