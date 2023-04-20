# Comparing `tmp/yopass_api-0.0.7.tar.gz` & `tmp/yopass_api-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yopass_api-0.0.7.tar", max compression
+gzip compressed data, was "yopass_api-0.0.8.tar", max compression
```

## Comparing `yopass_api-0.0.7.tar` & `yopass_api-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1096 2023-04-17 04:26:33.237964 yopass_api-0.0.7/LICENSE
--rw-r--r--   0        0        0     1039 2023-04-18 16:34:03.673135 yopass_api-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1082 2023-04-17 20:24:20.186363 yopass_api-0.0.7/README.md
--rw-r--r--   0        0        0       27 2023-04-17 04:26:33.238965 yopass_api-0.0.7/yopass_api/__init__.py
--rw-r--r--   0        0        0     5212 2023-04-18 15:44:20.479273 yopass_api-0.0.7/yopass_api/yopass_api.py
--rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 yopass_api-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-04-17 04:26:33.237964 yopass_api-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1108 2023-04-20 19:14:41.757350 yopass_api-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1082 2023-04-20 19:04:46.910682 yopass_api-0.0.8/README.md
+-rw-r--r--   0        0        0       27 2023-04-20 18:54:35.342791 yopass_api-0.0.8/yopass_api/__init__.py
+-rw-r--r--   0        0        0     5212 2023-04-18 15:44:20.479273 yopass_api-0.0.8/yopass_api/yopass_api.py
+-rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 yopass_api-0.0.8/PKG-INFO
```

### Comparing `yopass_api-0.0.7/LICENSE` & `yopass_api-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yopass_api-0.0.7/pyproject.toml` & `yopass_api-0.0.8/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yopass-api"
-version = "0.0.7"
+version = "0.0.8"
 description = "This module will allow you to use Python and Yopass in automation projects"
 license = "MIT"
 authors = ["Sergey Ilyashevich <silyashevich@gmail.com>"]
 maintainers = ["Sergey Ilyashevich <silyashevich@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/silyashevich/yopass_api"
 repository = "https://github.com/silyashevich/yopass_api"
@@ -25,12 +25,15 @@
 pytest = "^7.3.1"
 black = "^23.3.0"
 mypy = "^1.2.0"
 coverage = "^7.2.3"
 pytest-cov = "^4.0.0"
 
 [[tool.mypy.overrides]]
-module = "pgpy"
+module = ["pgpy", "requests"]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 filterwarnings = "ignore::DeprecationWarning:"
+
+[tool.mypy-requests]
+ignore_missing_imports = true
```

### Comparing `yopass_api-0.0.7/README.md` & `yopass_api-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `yopass_api-0.0.7/yopass_api/yopass_api.py` & `yopass_api-0.0.8/yopass_api/yopass_api.py`

 * *Files identical despite different names*

### Comparing `yopass_api-0.0.7/PKG-INFO` & `yopass_api-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yopass-api
-Version: 0.0.7
+Version: 0.0.8
 Summary: This module will allow you to use Python and Yopass in automation projects
 Home-page: https://github.com/silyashevich/yopass_api
 License: MIT
 Keywords: api,cryptography,yopass
 Author: Sergey Ilyashevich
 Author-email: silyashevich@gmail.com
 Maintainer: Sergey Ilyashevich
```

