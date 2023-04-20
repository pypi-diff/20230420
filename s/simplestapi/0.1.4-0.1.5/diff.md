# Comparing `tmp/simplestapi-0.1.4.tar.gz` & `tmp/simplestapi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplestapi-0.1.4.tar", max compression
+gzip compressed data, was "simplestapi-0.1.5.tar", max compression
```

## Comparing `simplestapi-0.1.4.tar` & `simplestapi-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1068 2022-08-27 08:54:16.177446 simplestapi-0.1.4/LICENSE
--rw-r--r--   0        0        0      987 2022-09-03 14:19:20.831207 simplestapi-0.1.4/README.md
--rw-r--r--   0        0        0     1165 2023-03-31 15:35:16.141522 simplestapi-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      776 2022-08-27 08:54:16.188446 simplestapi-0.1.4/simpleapi/README.md
--rw-r--r--   0        0        0      623 2023-03-30 19:42:08.112918 simplestapi-0.1.4/simpleapi/__init__.py
--rw-r--r--   0        0        0     1967 2022-09-03 14:13:27.360389 simplestapi-0.1.4/simpleapi/core.py
--rw-r--r--   0        0        0      441 2023-03-30 22:15:00.873620 simplestapi-0.1.4/simpleapi/custom_types.py
--rw-r--r--   0        0        0     7370 2023-03-31 14:09:10.473535 simplestapi-0.1.4/simpleapi/handler.py
--rw-r--r--   0        0        0     1088 2023-03-31 15:37:40.800563 simplestapi-0.1.4/simpleapi/request.py
--rw-r--r--   0        0        0     4470 2022-09-02 11:14:51.228631 simplestapi-0.1.4/simpleapi/response.py
--rw-r--r--   0        0        0       52 2022-08-27 08:56:26.016708 simplestapi-0.1.4/simpleapi/router.py
--rw-r--r--   0        0        0     2124 2022-08-27 08:56:26.017708 simplestapi-0.1.4/simpleapi/simpleapi.py
--rw-r--r--   0        0        0     3252 2023-03-31 15:41:55.108636 simplestapi-0.1.4/simpleapi/utils.py
--rw-r--r--   0        0        0     1764 1970-01-01 00:00:00.000000 simplestapi-0.1.4/setup.py
--rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 simplestapi-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-08-27 08:54:16.177446 simplestapi-0.1.5/LICENSE
+-rw-r--r--   0        0        0      987 2022-09-03 14:19:20.831207 simplestapi-0.1.5/README.md
+-rw-r--r--   0        0        0     1141 2023-04-19 23:51:09.437598 simplestapi-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      776 2022-08-27 08:54:16.188446 simplestapi-0.1.5/simpleapi/README.md
+-rw-r--r--   0        0        0      623 2023-04-19 23:53:00.151020 simplestapi-0.1.5/simpleapi/__init__.py
+-rw-r--r--   0        0        0     1967 2022-09-03 14:13:27.360389 simplestapi-0.1.5/simpleapi/core.py
+-rw-r--r--   0        0        0      441 2023-04-06 18:52:41.109297 simplestapi-0.1.5/simpleapi/custom_types.py
+-rw-r--r--   0        0        0     7632 2023-04-19 23:49:08.714550 simplestapi-0.1.5/simpleapi/handler.py
+-rw-r--r--   0        0        0     1088 2023-03-31 15:37:40.800563 simplestapi-0.1.5/simpleapi/request.py
+-rw-r--r--   0        0        0     4470 2022-09-02 11:14:51.228631 simplestapi-0.1.5/simpleapi/response.py
+-rw-r--r--   0        0        0       52 2022-08-27 08:56:26.016708 simplestapi-0.1.5/simpleapi/router.py
+-rw-r--r--   0        0        0     2124 2022-08-27 08:56:26.017708 simplestapi-0.1.5/simpleapi/simpleapi.py
+-rw-r--r--   0        0        0     3252 2023-03-31 15:41:55.108636 simplestapi-0.1.5/simpleapi/utils.py
+-rw-r--r--   0        0        0     1764 1970-01-01 00:00:00.000000 simplestapi-0.1.5/setup.py
+-rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 simplestapi-0.1.5/PKG-INFO
```

### Comparing `simplestapi-0.1.4/LICENSE` & `simplestapi-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simplestapi-0.1.4/README.md` & `simplestapi-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `simplestapi-0.1.4/pyproject.toml` & `simplestapi-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simplestapi"
-version = "0.1.4"
+version = "0.1.5"
 description = "SimpleAPI is a minimalistic, unopinionated web framework for Python, inspired by FastAPI & Flask"
 authors = ["Adham Salama <adham.salama@zohomail.com>"]
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -22,21 +22,21 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^1.9.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 requests = "^2.28.1"
-poethepoet = "^0.16.0"
 mypy = "^0.971"
 types-requests = "^2.28.8"
 gunicorn = "^20.1.0"
 mkdocs-material = "^8.4.1"
+yasta = "^0.1.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.poe.tasks]
+[yasta-tasks]
 typecheck = "mypy ."
-test.shell   = "gunicorn tests.app:app & pytest tests/test.py && kill -9 $(lsof -t -i:8000)"     
-fulltest.sequence = ["typecheck", "test"]
+test   = "gunicorn tests.app:app & pytest tests/test.py && kill -9 $(lsof -t -i:8000)"     
+fulltest = ["typecheck", "test"]
```

### Comparing `simplestapi-0.1.4/simpleapi/README.md` & `simplestapi-0.1.5/simpleapi/README.md`

 * *Files identical despite different names*

### Comparing `simplestapi-0.1.4/simpleapi/__init__.py` & `simplestapi-0.1.5/simpleapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.2"
+__version__ = "0.1.5"
 
 from .custom_types import RouteHandler, ViewFunction, Middleware, Query
 from .request import Request
 from .response import (
     ErrorResponse,
     JSONResponse,
     NotFoundErrorResponse,
```

### Comparing `simplestapi-0.1.4/simpleapi/core.py` & `simplestapi-0.1.5/simpleapi/core.py`

 * *Files identical despite different names*

### Comparing `simplestapi-0.1.4/simpleapi/handler.py` & `simplestapi-0.1.5/simpleapi/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,18 @@
 
             # Apply handlers middleware
             middleware_response = apply_middleware(request, handler["middleware"])
             if middleware_response:
                 return middleware_response
 
             handler_type_hints = get_type_hints(handler["handler"])
+            # Remove return type hint as we don't need it because it had caused
+            # a validation error for any handler function that had a return type hint
+            if "return" in handler_type_hints:
+                del handler_type_hints["return"]
             dependency_injection: dict[str, Any] = {}
             for k, v in handler_type_hints.items():
                 if v == Request:
                     dependency_injection[k] = request
                 elif k in request.body.keys():
                     if isinstance(request.body[k], v):
                         dependency_injection[k] = request.body[k]
```

### Comparing `simplestapi-0.1.4/simpleapi/request.py` & `simplestapi-0.1.5/simpleapi/request.py`

 * *Files identical despite different names*

### Comparing `simplestapi-0.1.4/simpleapi/response.py` & `simplestapi-0.1.5/simpleapi/response.py`

 * *Files identical despite different names*

### Comparing `simplestapi-0.1.4/simpleapi/simpleapi.py` & `simplestapi-0.1.5/simpleapi/simpleapi.py`

 * *Files identical despite different names*

### Comparing `simplestapi-0.1.4/simpleapi/utils.py` & `simplestapi-0.1.5/simpleapi/utils.py`

 * *Files identical despite different names*

### Comparing `simplestapi-0.1.4/setup.py` & `simplestapi-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.9.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'simplestapi',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'SimpleAPI is a minimalistic, unopinionated web framework for Python, inspired by FastAPI & Flask',
     'long_description': '# SimpleAPI\n\n![banner](https://i.imgur.com/Q3kFiKf.png)\nSimpleAPI is a minimalistic, unopinionated web framework for Python, inspired by FastAPI & Flask.\n\nSimpleAPI is a WSGI compliant framework.\n\nThis is a hobby project made for educational purposes because I want to try learning writing a web server framework.\n\nSo, this is obviously not meant for production environments.\n\nDevelopment of SimpleAPI is tracked at [this](https://github.com/users/adhamsalama/projects/1) GitHub project.\n\n## Installation\n\n`pip install simplestapi`\n\n## Usage\n\nAn example of using SimpleAPI:\n\nCopy the following code to a file called `app.py`\n\n```python\nfrom simpleapi import SimpleAPI\n\napp = SimpleAPI()\n\n@app.get("/hello")\ndef hello():\n    return "Hello, world!"\n```\n\nRun it with `gunicorn app:app`\n\nMore examples can be found in [tests](./tests)\n\n## Documentation\n\n[https://adhamsalama.github.io/simpleapi](https://adhamsalama.github.io/simpleapi)\n\n---\n\n![django_kofta](./docs/assets/django_kofta.png)\n',
     'author': 'Adham Salama',
     'author_email': 'adham.salama@zohomail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://adhamsalama.github.io/simpleapi',
```

### Comparing `simplestapi-0.1.4/PKG-INFO` & `simplestapi-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplestapi
-Version: 0.1.4
+Version: 0.1.5
 Summary: SimpleAPI is a minimalistic, unopinionated web framework for Python, inspired by FastAPI & Flask
 Home-page: https://adhamsalama.github.io/simpleapi
 License: MIT
 Author: Adham Salama
 Author-email: adham.salama@zohomail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

