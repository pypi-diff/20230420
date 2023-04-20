# Comparing `tmp/sag-py-fastapi-request-id-0.1.0.tar.gz` & `tmp/sag-py-fastapi-request-id-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-fastapi-request-id-0.1.0.tar", last modified: Mon Apr  3 07:53:45 2023, max compression
+gzip compressed data, was "sag-py-fastapi-request-id-0.1.1.tar", last modified: Thu Apr 20 09:03:23 2023, max compression
```

## Comparing `sag-py-fastapi-request-id-0.1.0.tar` & `sag-py-fastapi-request-id-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:45.769250 sag-py-fastapi-request-id-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-03 07:53:36.000000 sag-py-fastapi-request-id-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-03 07:53:45.769250 sag-py-fastapi-request-id-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-03 07:53:36.000000 sag-py-fastapi-request-id-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-03 07:53:36.000000 sag-py-fastapi-request-id-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:45.769250 sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-03 07:53:36.000000 sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-03 07:53:36.000000 sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:36.000000 sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-03 07:53:36.000000 sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id/request_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-03 07:53:36.000000 sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id/request_context_logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-03 07:53:36.000000 sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id/request_context_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:45.769250 sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-03 07:53:45.000000 sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-03 07:53:45.000000 sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 07:53:45.000000 sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-03 07:53:45.000000 sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-03 07:53:45.000000 sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-03 07:53:45.773250 sag-py-fastapi-request-id-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-03 07:53:36.000000 sag-py-fastapi-request-id-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:45.769250 sag-py-fastapi-request-id-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-03 07:53:36.000000 sag-py-fastapi-request-id-0.1.0/tests/test_request_context_logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-03 07:53:36.000000 sag-py-fastapi-request-id-0.1.0/tests/test_request_context_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:03:23.660398 sag-py-fastapi-request-id-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 09:02:58.000000 sag-py-fastapi-request-id-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-20 09:03:23.660398 sag-py-fastapi-request-id-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-20 09:02:58.000000 sag-py-fastapi-request-id-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 09:02:58.000000 sag-py-fastapi-request-id-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:03:23.660398 sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-20 09:02:58.000000 sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 09:02:58.000000 sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:02:58.000000 sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-20 09:02:58.000000 sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id/request_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-20 09:02:58.000000 sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id/request_context_logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-20 09:02:58.000000 sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id/request_context_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:03:23.660398 sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-20 09:03:23.000000 sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-20 09:03:23.000000 sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:03:23.000000 sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 09:03:23.000000 sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 09:03:23.000000 sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 09:03:23.660398 sag-py-fastapi-request-id-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-20 09:02:58.000000 sag-py-fastapi-request-id-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:03:23.660398 sag-py-fastapi-request-id-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-20 09:02:58.000000 sag-py-fastapi-request-id-0.1.1/tests/test_request_context_logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-20 09:02:58.000000 sag-py-fastapi-request-id-0.1.1/tests/test_request_context_middleware.py
```

### Comparing `sag-py-fastapi-request-id-0.1.0/LICENSE.txt` & `sag-py-fastapi-request-id-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-request-id-0.1.0/PKG-INFO` & `sag-py-fastapi-request-id-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-fastapi-request-id
-Version: 0.1.0
+Version: 0.1.1
 Summary: Adds an unique identifiert to fastapi requests
 Home-page: https://github.com/SamhammerAG/sag_py_fastapi_request_id
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_fastapi_request_id
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_fastapi_request_id/issues
@@ -38,15 +38,15 @@
 * Provides a middleware to generate a random request id for every request
 * Contains a logging filter that adds the request id as field to every log entry
 
 ## How to use
 
 ### Installation
 
-pip install sag_py_fastapi_request_id
+pip install sag-py-fastapi-request-id
 
 ### Add the middleware
 
 Add this middleware so that the request ids are generated:
 ```python
 from sag_py_fastapi_request_id.request_context_middleware import RequestContextMiddleware
 from fastapi import FastAPI
@@ -80,12 +80,32 @@
 console_handler = logging.StreamHandler(sys.stdout)
 console_handler.addFilter(RequestContextLoggingFilter())
 
 ```
 
 The filter adds the field request_id if it has a value in the context.
 
-## How to publish
+## How to start developing
+
+### With vscode
+
+Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
 
+### With pycharm
+
+* Install latest pycharm
+* Install pycharm plugin BlackConnect
+* Install pycharm plugin Mypy
+* Configure the python interpreter/venv
+* pip install requirements-dev.txt
+* pip install black[d]
+* Ctl+Alt+S => Check Tools => BlackConnect => Trigger when saving changed files
+* Ctl+Alt+S => Check Tools => BlackConnect => Trigger on code reformat
+* Ctl+Alt+S => Click Tools => BlackConnect => "Load from pyproject.yaml" (ensure line length is 120)
+* Ctl+Alt+S => Click Tools => BlackConnect => Configure path to the blackd.exe at the "local instance" config (e.g. C:\Python310\Scripts\blackd.exe)
+* Ctl+Alt+S => Click Tools => Actions on save => Reformat code
+* Restart pycharm
+
+## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
```

### Comparing `sag-py-fastapi-request-id-0.1.0/README.md` & `sag-py-fastapi-request-id-0.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 * Provides a middleware to generate a random request id for every request
 * Contains a logging filter that adds the request id as field to every log entry
 
 ## How to use
 
 ### Installation
 
-pip install sag_py_fastapi_request_id
+pip install sag-py-fastapi-request-id
 
 ### Add the middleware
 
 Add this middleware so that the request ids are generated:
 ```python
 from sag_py_fastapi_request_id.request_context_middleware import RequestContextMiddleware
 from fastapi import FastAPI
@@ -57,12 +57,32 @@
 console_handler = logging.StreamHandler(sys.stdout)
 console_handler.addFilter(RequestContextLoggingFilter())
 
 ```
 
 The filter adds the field request_id if it has a value in the context.
 
-## How to publish
+## How to start developing
+
+### With vscode
+
+Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
 
+### With pycharm
+
+* Install latest pycharm
+* Install pycharm plugin BlackConnect
+* Install pycharm plugin Mypy
+* Configure the python interpreter/venv
+* pip install requirements-dev.txt
+* pip install black[d]
+* Ctl+Alt+S => Check Tools => BlackConnect => Trigger when saving changed files
+* Ctl+Alt+S => Check Tools => BlackConnect => Trigger on code reformat
+* Ctl+Alt+S => Click Tools => BlackConnect => "Load from pyproject.yaml" (ensure line length is 120)
+* Ctl+Alt+S => Click Tools => BlackConnect => Configure path to the blackd.exe at the "local instance" config (e.g. C:\Python310\Scripts\blackd.exe)
+* Ctl+Alt+S => Click Tools => Actions on save => Reformat code
+* Restart pycharm
+
+## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
```

### Comparing `sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id/request_context_middleware.py` & `sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id/request_context_middleware.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id.egg-info/PKG-INFO` & `sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-fastapi-request-id
-Version: 0.1.0
+Version: 0.1.1
 Summary: Adds an unique identifiert to fastapi requests
 Home-page: https://github.com/SamhammerAG/sag_py_fastapi_request_id
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_fastapi_request_id
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_fastapi_request_id/issues
@@ -38,15 +38,15 @@
 * Provides a middleware to generate a random request id for every request
 * Contains a logging filter that adds the request id as field to every log entry
 
 ## How to use
 
 ### Installation
 
-pip install sag_py_fastapi_request_id
+pip install sag-py-fastapi-request-id
 
 ### Add the middleware
 
 Add this middleware so that the request ids are generated:
 ```python
 from sag_py_fastapi_request_id.request_context_middleware import RequestContextMiddleware
 from fastapi import FastAPI
@@ -80,12 +80,32 @@
 console_handler = logging.StreamHandler(sys.stdout)
 console_handler.addFilter(RequestContextLoggingFilter())
 
 ```
 
 The filter adds the field request_id if it has a value in the context.
 
-## How to publish
+## How to start developing
+
+### With vscode
+
+Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
 
+### With pycharm
+
+* Install latest pycharm
+* Install pycharm plugin BlackConnect
+* Install pycharm plugin Mypy
+* Configure the python interpreter/venv
+* pip install requirements-dev.txt
+* pip install black[d]
+* Ctl+Alt+S => Check Tools => BlackConnect => Trigger when saving changed files
+* Ctl+Alt+S => Check Tools => BlackConnect => Trigger on code reformat
+* Ctl+Alt+S => Click Tools => BlackConnect => "Load from pyproject.yaml" (ensure line length is 120)
+* Ctl+Alt+S => Click Tools => BlackConnect => Configure path to the blackd.exe at the "local instance" config (e.g. C:\Python310\Scripts\blackd.exe)
+* Ctl+Alt+S => Click Tools => Actions on save => Reformat code
+* Restart pycharm
+
+## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
```

### Comparing `sag-py-fastapi-request-id-0.1.0/sag_py_fastapi_request_id.egg-info/SOURCES.txt` & `sag-py-fastapi-request-id-0.1.1/sag_py_fastapi_request_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-request-id-0.1.0/setup.py` & `sag-py-fastapi-request-id-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 with open("requirements.txt", "r") as fin:
     REQS = fin.read().splitlines()
 
+with open("requirements-dev.txt", "r") as fin:
+    REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
+
 setuptools.setup(
     name="sag-py-fastapi-request-id",
-    version="0.1.0",
+    version="0.1.1",
     description="Adds an unique identifiert to fastapi requests",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_fastapi_request_id",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
@@ -25,14 +28,14 @@
         "Topic :: Software Development",
     ],
     keywords="auth, fastapi, keycloak",
     packages=setuptools.find_packages(exclude=["tests"]),
     package_data={"sag_py_fastapi_request_id": ["py.typed"]},
     python_requires=">=3.8",
     install_requires=REQS,
-    extras_require={"dev": ["pytest"]},
+    extras_require={"dev": REQS_DEV},
     project_urls={
         "Documentation": "https://github.com/SamhammerAG/sag_py_fastapi_request_id",
         "Bug Reports": "https://github.com/SamhammerAG/sag_py_fastapi_request_id/issues",
         "Source": "https://github.com/SamhammerAG/sag_py_fastapi_request_id",
     },
 )
```

### Comparing `sag-py-fastapi-request-id-0.1.0/tests/test_request_context_logging_filter.py` & `sag-py-fastapi-request-id-0.1.1/tests/test_request_context_logging_filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from logging import INFO, LogRecord
 from typing import cast
 
 import pytest
 
-from sag_py_fastapi_request_id import RequestContextLoggingFilter, RequestIdLogRecord, request_context
+from sag_py_fastapi_request_id import request_context
+from sag_py_fastapi_request_id.models import RequestIdLogRecord
+from sag_py_fastapi_request_id.request_context_logging_filter import RequestContextLoggingFilter
 
 
 @pytest.fixture()
 def log_record() -> LogRecord:
     return LogRecord(name="", level=INFO, pathname="", lineno=0, msg="Hello, world!", args=(), exc_info=None)
```

### Comparing `sag-py-fastapi-request-id-0.1.0/tests/test_request_context_middleware.py` & `sag-py-fastapi-request-id-0.1.1/tests/test_request_context_middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from starlette.applications import Starlette
 from starlette.types import Scope
 
-from sag_py_fastapi_request_id import RequestContextMiddleware, request_context
+from sag_py_fastapi_request_id import request_context
+from sag_py_fastapi_request_id.request_context_middleware import RequestContextMiddleware
 
 
 def test_call_no_request_id_for_lifespan() -> None:
     # Arrange
     app = Starlette()
     middleware = RequestContextMiddleware(app)
     scope: Scope = {"type": "lifespan"}
```

