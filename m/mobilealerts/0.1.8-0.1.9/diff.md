# Comparing `tmp/mobilealerts-0.1.8.tar.gz` & `tmp/mobilealerts-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobilealerts-0.1.8.tar", max compression
+gzip compressed data, was "mobilealerts-0.1.9.tar", max compression
```

## Comparing `mobilealerts-0.1.8.tar` & `mobilealerts-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1095 2021-11-10 18:03:27.161936 mobilealerts-0.1.8/LICENSE
--rw-r--r--   0        0        0      347 2022-09-21 19:16:08.233493 mobilealerts-0.1.8/mobilealerts/__init__.py
--rw-r--r--   0        0        0    27874 2022-12-27 06:58:41.297861 mobilealerts-0.1.8/mobilealerts/gateway.py
--rw-r--r--   0        0        0     5585 2022-09-24 11:14:54.756849 mobilealerts-0.1.8/mobilealerts/proxy.py
--rw-r--r--   0        0        0    29815 2022-12-27 06:36:43.009499 mobilealerts-0.1.8/mobilealerts/sensor.py
--rw-r--r--   0        0        0     3428 2022-12-27 06:55:47.884594 mobilealerts-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2368 2022-11-30 06:29:13.474437 mobilealerts-0.1.8/README.md
--rw-r--r--   0        0        0     3173 2022-12-27 07:14:09.421232 mobilealerts-0.1.8/setup.py
--rw-r--r--   0        0        0     3340 2022-12-27 07:14:09.422229 mobilealerts-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1095 2021-11-10 18:03:27.161936 mobilealerts-0.1.9/LICENSE
+-rw-r--r--   0        0        0      347 2022-09-21 19:16:08.233493 mobilealerts-0.1.9/mobilealerts/__init__.py
+-rw-r--r--   0        0        0    28111 2023-03-07 14:18:42.272475 mobilealerts-0.1.9/mobilealerts/gateway.py
+-rw-r--r--   0        0        0     5581 2023-03-07 14:17:03.591770 mobilealerts-0.1.9/mobilealerts/proxy.py
+-rw-r--r--   0        0        0    29815 2022-12-27 06:36:43.009499 mobilealerts-0.1.9/mobilealerts/sensor.py
+-rw-r--r--   0        0        0     3426 2023-03-07 14:17:03.599748 mobilealerts-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2368 2022-11-30 06:29:13.474437 mobilealerts-0.1.9/README.md
+-rw-r--r--   0        0        0     3590 1970-01-01 00:00:00.000000 mobilealerts-0.1.9/PKG-INFO
```

### Comparing `mobilealerts-0.1.8/LICENSE` & `mobilealerts-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mobilealerts-0.1.8/mobilealerts/gateway.py` & `mobilealerts-0.1.9/mobilealerts/gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,14 +542,19 @@
             try:
                 proxy_to_use: Optional[str] = None
                 if self.orig_use_proxy:
                     proxy_to_use = ("http://%s:%s") % (
                         self.orig_proxy,
                         self.orig_proxy_port,
                     )
+                    _LOGGER.debug(
+                        "Sending data to cloud: %s via proxy: %s", url, proxy_to_use
+                    )
+                else:
+                    _LOGGER.debug("Sending data to cloud: %s", url)
                 async with aiohttp.ClientSession() as session:
                     async with session.put(
                         str(url), proxy=proxy_to_use, headers=headers, data=content
                     ) as response:
                         response_content = await response.content.read()
                         _LOGGER.debug(
                             "Cloud response status: %s content: %s",
```

### Comparing `mobilealerts-0.1.8/mobilealerts/proxy.py` & `mobilealerts-0.1.9/mobilealerts/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                         content = await request.content.read(
                             int(request.headers["Content-Length"])
                         )
                         await gateway.handle_update(
                             identify[2], content, request.remote
                         )
                         await gateway.resend_data_to_cloud(
-                            request.rel_url, headers, content
+                            request.url, headers, content
                         )
                     else:
                         _LOGGER.error(
                             "Invalid HTTP_IDENTIFY header in gateway's PUT request"
                         )
                 else:
                     _LOGGER.error("No HTTP_IDENTIFY header in gateway's PUT request")
```

### Comparing `mobilealerts-0.1.8/mobilealerts/sensor.py` & `mobilealerts-0.1.9/mobilealerts/sensor.py`

 * *Files identical despite different names*

### Comparing `mobilealerts-0.1.8/pyproject.toml` & `mobilealerts-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 #name = "python-mobilealerts"
 name = "mobilealerts"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python classes for MobileAlerts gateway and sensors"
 readme = "README.md"
 authors = ["PlusPlus-ua <alexplas@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/PlusPlus-ua/python-mobilealerts"
 homepage = "https://github.com/PlusPlus-ua/python-mobilealerts"
 
@@ -31,26 +31,26 @@
 ]
 
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 aiohttp = "^3.8"
-importlib_metadata = {version = ">=4.5,<6.0", python = "<3.8"}
+importlib_metadata = {version = ">=4.5,<7.0", python = "<3.8"}
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.4"
 black = {version = "^22.12", allow-prereleases = true}
 darglint = "^1.8.0"
-isort = {extras = ["colors"], version = "^5.11.4"}
-mypy = "^0.991"
-mypy-extensions = "^0.4.3"
+isort = {extras = ["colors"], version = "^5.11.5"}
+mypy = "^1.0"
+mypy-extensions = "^1.0.0"
 pre-commit = "^2.21.0"
 pydocstyle = "^6.1.1"
 pylint = "^2.13.9"
-pytest = "^7.2.0"
+pytest = "^7.2.2"
 pyupgrade = "^3.3.1"
 safety = "^2.3.5"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py37"]
 line-length = 88
```

### Comparing `mobilealerts-0.1.8/README.md` & `mobilealerts-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mobilealerts-0.1.8/PKG-INFO` & `mobilealerts-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: mobilealerts
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python classes for MobileAlerts gateway and sensors
 Home-page: https://github.com/PlusPlus-ua/python-mobilealerts
 License: MIT
 Author: PlusPlus-ua
 Author-email: alexplas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.8,<4.0)
-Requires-Dist: importlib_metadata (>=4.5,<6.0); python_version < "3.8"
+Requires-Dist: importlib_metadata (>=4.5,<7.0) ; python_version < "3.8"
 Project-URL: Repository, https://github.com/PlusPlus-ua/python-mobilealerts
 Description-Content-Type: text/markdown
 
 # python-mobilealerts
 
 [![build](https://github.com/PlusPlus-ua/python-mobilealerts/actions/workflows/build.yml/badge.svg)](https://github.com/PlusPlus-ua/python-mobilealerts/actions/workflows/build.yml) [![Python Version](https://img.shields.io/pypi/pyversions/mobilealerts.svg)](https://pypi.org/project/mobilealerts/) [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/PlusPlus-ua/python-mobilealerts/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit) [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/PlusPlus-ua/python-mobilealerts/blob/master/.pre-commit-config.yaml) [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/PlusPlus-ua/python-mobilealerts/releases) [![License](https://img.shields.io/github/license/PlusPlus-ua/python-mobilealerts)](https://github.com/PlusPlus-ua/python-mobilealerts/blob/master/LICENSE)
```

