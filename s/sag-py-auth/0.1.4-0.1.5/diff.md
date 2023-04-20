# Comparing `tmp/sag-py-auth-0.1.4.tar.gz` & `tmp/sag-py-auth-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-auth-0.1.4.tar", last modified: Thu Apr  6 11:01:54 2023, max compression
+gzip compressed data, was "sag-py-auth-0.1.5.tar", last modified: Thu Apr 20 07:46:02 2023, max compression
```

## Comparing `sag-py-auth-0.1.4.tar` & `sag-py-auth-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:01:54.324050 sag-py-auth-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-06 11:01:54.324050 sag-py-auth-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:01:54.320050 sag-py-auth-0.1.4/sag_py_auth/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/sag_py_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/sag_py_auth/auth_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/sag_py_auth/jwt_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/sag_py_auth/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/sag_py_auth/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/sag_py_auth/token_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/sag_py_auth/token_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/sag_py_auth/user_name_logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/sag_py_auth/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:01:54.324050 sag-py-auth-0.1.4/sag_py_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-06 11:01:54.000000 sag-py-auth-0.1.4/sag_py_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-06 11:01:54.000000 sag-py-auth-0.1.4/sag_py_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 11:01:54.000000 sag-py-auth-0.1.4/sag_py_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-06 11:01:54.000000 sag-py-auth-0.1.4/sag_py_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-06 11:01:54.000000 sag-py-auth-0.1.4/sag_py_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-06 11:01:54.324050 sag-py-auth-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:01:54.324050 sag-py-auth-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/tests/test_auth_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/tests/test_jwt_auth__call.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/tests/test_jwt_auth__init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/tests/test_jwt_auth__realm_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/tests/test_jwt_auth__roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/tests/test_jwt_auth__verify_and_decode_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/tests/test_token_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/tests/test_user_name_logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-06 11:01:45.000000 sag-py-auth-0.1.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:46:02.491515 sag-py-auth-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-20 07:46:02.491515 sag-py-auth-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:46:02.487515 sag-py-auth-0.1.5/sag_py_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/sag_py_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/sag_py_auth/auth_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/sag_py_auth/jwt_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/sag_py_auth/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/sag_py_auth/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/sag_py_auth/token_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/sag_py_auth/token_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/sag_py_auth/user_name_logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/sag_py_auth/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:46:02.491515 sag-py-auth-0.1.5/sag_py_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-20 07:46:02.000000 sag-py-auth-0.1.5/sag_py_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-20 07:46:02.000000 sag-py-auth-0.1.5/sag_py_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:46:02.000000 sag-py-auth-0.1.5/sag_py_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-20 07:46:02.000000 sag-py-auth-0.1.5/sag_py_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-20 07:46:02.000000 sag-py-auth-0.1.5/sag_py_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 07:46:02.491515 sag-py-auth-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:46:02.491515 sag-py-auth-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/tests/test_auth_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/tests/test_jwt_auth__call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/tests/test_jwt_auth__init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/tests/test_jwt_auth__realm_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/tests/test_jwt_auth__roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/tests/test_jwt_auth__verify_and_decode_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/tests/test_token_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/tests/test_user_name_logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-20 07:45:52.000000 sag-py-auth-0.1.5/tests/test_utils.py
```

### Comparing `sag-py-auth-0.1.4/LICENSE.txt` & `sag-py-auth-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-auth-0.1.4/PKG-INFO` & `sag-py-auth-0.1.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: sag-py-auth
-Version: 0.1.4
-Summary: Keycloak authentication for python projects
-Home-page: https://github.com/SamhammerAG/sag_py_auth
-Author: Samhammer AG
-Author-email: support@samhammer.de
-License: MIT
-Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_auth
-Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_auth/issues
-Project-URL: Source, https://github.com/SamhammerAG/sag_py_auth
-Keywords: auth,fastapi,keycloak
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
 # sag_py_auth
 
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities](https://snyk.io/test/github/SamhammerAG/sag_py_auth/badge.svg)](https://snyk.io/test/github/SamhammerAG/sag_py_auth)
 
 [coveralls-image]:https://coveralls.io/repos/github/SamhammerAG/sag_py_auth/badge.svg?branch=master
@@ -137,12 +114,32 @@
     }
 }
 ```
 
 * realm_access contains the realm roles
 * resource_access contains the token roles for one or multiple clients
 
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

### Comparing `sag-py-auth-0.1.4/sag_py_auth/jwt_auth.py` & `sag-py-auth-0.1.5/sag_py_auth/jwt_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         token: Token = self._verify_and_decode_token(token_string)
 
         self._verify_roles(token)
         self._verify_realm_roles(token)
         auth_context_set_token(token)
         return token
 
-    def _verify_and_decode_token(self, token_string: str) -> Token:  # type: ignore
+    def _verify_and_decode_token(self, token_string: str) -> Token:
         try:
             token_dict: TokenDict = verify_and_decode_token(self.auth_config, token_string)
             return Token(token_dict)
         except Exception:
             logger.warning("Invalid auth token", exc_info=True)
             self._raise_auth_error(HTTP_401_UNAUTHORIZED, "Invalid token.")
```

### Comparing `sag-py-auth-0.1.4/sag_py_auth/models.py` & `sag-py-auth-0.1.5/sag_py_auth/models.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-0.1.4/sag_py_auth/token_decoder.py` & `sag-py-auth-0.1.5/sag_py_auth/token_decoder.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-0.1.4/sag_py_auth/user_name_logging_filter.py` & `sag-py-auth-0.1.5/sag_py_auth/user_name_logging_filter.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-0.1.4/sag_py_auth.egg-info/PKG-INFO` & `sag-py-auth-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-auth
-Version: 0.1.4
+Version: 0.1.5
 Summary: Keycloak authentication for python projects
 Home-page: https://github.com/SamhammerAG/sag_py_auth
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_auth
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_auth/issues
@@ -137,12 +137,32 @@
     }
 }
 ```
 
 * realm_access contains the realm roles
 * resource_access contains the token roles for one or multiple clients
 
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

### Comparing `sag-py-auth-0.1.4/sag_py_auth.egg-info/SOURCES.txt` & `sag-py-auth-0.1.5/sag_py_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-auth-0.1.4/setup.py` & `sag-py-auth-0.1.5/setup.py`

 * *Files 10% similar despite different names*

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
     name="sag-py-auth",
-    version="0.1.4",
+    version="0.1.5",
     description="Keycloak authentication for python projects",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_auth",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
@@ -25,14 +28,14 @@
         "Topic :: Software Development",
     ],
     keywords="auth, fastapi, keycloak",
     packages=setuptools.find_packages(exclude=["tests"]),
     package_data={"sag_py_auth": ["py.typed"]},
     python_requires=">=3.8",
     install_requires=REQS,
-    extras_require={"dev": ["pytest"]},
+    extras_require={"dev": REQS_DEV},
     project_urls={
         "Documentation": "https://github.com/SamhammerAG/sag_py_auth",
         "Bug Reports": "https://github.com/SamhammerAG/sag_py_auth/issues",
         "Source": "https://github.com/SamhammerAG/sag_py_auth",
     },
 )
```

### Comparing `sag-py-auth-0.1.4/tests/test_auth_context.py` & `sag-py-auth-0.1.5/tests/test_auth_context.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-0.1.4/tests/test_jwt_auth__call.py` & `sag-py-auth-0.1.5/tests/test_jwt_auth__call.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-0.1.4/tests/test_jwt_auth__init.py` & `sag-py-auth-0.1.5/tests/test_jwt_auth__init.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-0.1.4/tests/test_jwt_auth__realm_roles.py` & `sag-py-auth-0.1.5/tests/test_jwt_auth__realm_roles.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-0.1.4/tests/test_jwt_auth__roles.py` & `sag-py-auth-0.1.5/tests/test_jwt_auth__roles.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-0.1.4/tests/test_jwt_auth__verify_and_decode_token.py` & `sag-py-auth-0.1.5/tests/test_jwt_auth__verify_and_decode_token.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-0.1.4/tests/test_models.py` & `sag-py-auth-0.1.5/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-0.1.4/tests/test_token_decoder.py` & `sag-py-auth-0.1.5/tests/test_token_decoder.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-0.1.4/tests/test_user_name_logging_filter.py` & `sag-py-auth-0.1.5/tests/test_user_name_logging_filter.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-0.1.4/tests/test_utils.py` & `sag-py-auth-0.1.5/tests/test_utils.py`

 * *Files identical despite different names*

