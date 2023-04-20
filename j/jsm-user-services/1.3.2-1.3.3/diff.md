# Comparing `tmp/jsm_user_services-1.3.2.tar.gz` & `tmp/jsm_user_services-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jsm_user_services-1.3.2.tar", last modified: Mon Mar 13 13:10:33 2023, max compression
+gzip compressed data, was "jsm_user_services-1.3.3.tar", max compression
```

## Comparing `jsm_user_services-1.3.2.tar` & `jsm_user_services-1.3.3.tar`

### file list

```diff
@@ -1,68 +1,31 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/
--rw-r--r--   0 vsts      (1001) docker     (122)    13144 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    10233 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/jsm_user_services/
--rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/apps.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/jsm_user_services/decorators/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/decorators/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3779 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/decorators/lgpd.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5934 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/decorators/lgpd_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/jsm_user_services/drf_tools/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/drf_tools/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2474 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/drf_tools/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14146 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/drf_tools/permissions.py
--rw-r--r--   0 vsts      (1001) docker     (122)      692 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/exception.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/jsm_user_services/flask/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/flask/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3445 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/flask/middleware.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3149 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/middleware.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/jsm_user_services/services/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/services/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4233 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/services/everest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2000 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/services/google.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4548 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/services/user.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1778 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/settings.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/jsm_user_services/support/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/support/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1006 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/support/auth_jwt.py
--rw-r--r--   0 vsts      (1001) docker     (122)      865 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/support/email_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2305 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/support/http_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)      287 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/support/import_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)      405 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/support/local_threading_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)      268 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/support/logging_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/support/request_id.py
--rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/support/settings_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)      197 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/jsm_user_services/support/string_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/jsm_user_services.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    13144 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/jsm_user_services.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1815 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/jsm_user_services.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/jsm_user_services.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/jsm_user_services.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       24 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/jsm_user_services.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      299 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     1365 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/tests/decorators/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/decorators/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15173 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/decorators/test_lgpd.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2664 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/decorators/test_lgpd_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-13 13:10:33.000000 jsm_user_services-1.3.2/tests/flask/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/flask/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1063 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/flask/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1201 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/flask/test_middleware.py
--rw-r--r--   0 vsts      (1001) docker     (122)      572 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/settings.py
--rw-r--r--   0 vsts      (1001) docker     (122)    25884 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/test_drf_tools.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6518 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/test_email_validations.py
--rw-r--r--   0 vsts      (1001) docker     (122)      914 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/test_http_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)      425 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/test_import_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)      981 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/test_local_threading_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1046 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/test_logging_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6042 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/test_middleware.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2265 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/test_request_id.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1376 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/test_service_google.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11899 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/test_service_user.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1832 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/test_settings.py
--rw-r--r--   0 vsts      (1001) docker     (122)      467 2023-03-13 13:09:01.000000 jsm_user_services-1.3.2/tests/test_string_split_utils.py
+-rw-r--r--   0        0        0     1070 2023-04-20 13:29:37.852234 jsm_user_services-1.3.3/LICENSE
+-rw-r--r--   0        0        0    10306 2023-04-20 13:29:37.852234 jsm_user_services-1.3.3/README.md
+-rw-r--r--   0        0        0       54 2023-04-20 13:29:37.852234 jsm_user_services-1.3.3/jsm_user_services/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-20 13:29:37.852234 jsm_user_services-1.3.3/jsm_user_services/apps.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:29:37.852234 jsm_user_services-1.3.3/jsm_user_services/decorators/__init__.py
+-rw-r--r--   0        0        0     3795 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/decorators/lgpd.py
+-rw-r--r--   0        0        0     5933 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/decorators/lgpd_utils.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/drf_tools/__init__.py
+-rw-r--r--   0        0        0     2475 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/drf_tools/helpers.py
+-rw-r--r--   0        0        0    14221 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/drf_tools/permissions.py
+-rw-r--r--   0        0        0      692 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/exception.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/flask/__init__.py
+-rw-r--r--   0        0        0     3462 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/flask/middleware.py
+-rw-r--r--   0        0        0     3167 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/middleware.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/services/__init__.py
+-rw-r--r--   0        0        0     4258 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/services/everest.py
+-rw-r--r--   0        0        0     1996 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/services/google.py
+-rw-r--r--   0        0        0     4657 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/services/user.py
+-rw-r--r--   0        0        0     1840 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/settings.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/__init__.py
+-rw-r--r--   0        0        0     1007 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/auth_jwt.py
+-rw-r--r--   0        0        0      866 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/email_utils.py
+-rw-r--r--   0        0        0     2333 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/http_utils.py
+-rw-r--r--   0        0        0      304 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/import_utils.py
+-rw-r--r--   0        0        0      419 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/local_threading_utils.py
+-rw-r--r--   0        0        0      268 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/logging_utils.py
+-rw-r--r--   0        0        0     1971 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/request_id.py
+-rw-r--r--   0        0        0      618 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/settings_utils.py
+-rw-r--r--   0        0        0      237 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/string_utils.py
+-rw-r--r--   0        0        0     1572 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0    11435 1970-01-01 00:00:00.000000 jsm_user_services-1.3.3/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jsm_user_services-1.3.2/PKG-INFO` & `jsm_user_services-1.3.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,282 +1,264 @@
-Metadata-Version: 2.1
-Name: jsm_user_services
-Version: 1.3.2
-Summary: Middleware to intercept JWT auth token and more utils functions
-Home-page: https://github.com/juntossomosmais/jsm-user-service
-Author: Juntos Somos Mais
-Author-email: labs@juntossomosmais.com.br
-License: MIT
-Description: # JSM User JWT Service
-        
-        Middleware to intercept JWT auth token and more utils functions
-        
-        ## Local development
-        
-        ### Running tests
-        
-        `docker-compose up integration-tests`
-        
-        ## Install - For Django users
-        
-        `pip install jsm-user-services[drf]`
-        
-        Add `jsm_user_services` to your `INSTALLED_APPS`:
-        
-        ```python
-        INSTALLED_APPS = [
-            "django.contrib.admin",
-            "django.contrib.auth",
-            "django.contrib.contenttypes",
-            "django.contrib.sessions",
-            "django.contrib.messages",
-            "django.contrib.staticfiles",
-            "jsm_user_services",
-            "app_test",
-        ]
-        ```
-        
-        Add the Middleware:
-        
-        ```python
-        MIDDLEWARE = [
-            ...
-            "jsm_user_services.middleware.JsmJwtService",
-        ]
-        
-        # Dev url
-        USER_API_HOST = "http://ishtar-gate.dev.juntossomosmaisi.com.br/api/v1"
-        USER_API_TOKEN = "user_api_token"
-        ```
-        
-        ## Install - For Flask users
-        
-        `pip install jsm-user-services[flask]`
-        
-        Add the middleware in your Flask app:
-        
-        ```python
-        from flask import Flask
-        from jsm_user_services.flask import middleware
-        
-        app = Flask(__name__)
-        
-        middleware.JsmJwtService(app)
-        app.config.update(
-            USER_API_HOST="http://ishtar-gate.dev.juntossomosmaisi.com.br/api/v1", USER_API_TOKEN="user_api_token"
-        )
-        ```
-        
-        **DISCLAIMER**
-        - Currently, only the middleware is implemented for Flask apps
-        
-        ## Use
-        
-        ```python
-        from jsm_user_services.services.user import current_jwt_token
-        from jsm_user_services.services.user import get_jsm_token
-        from jsm_user_services.services.user import get_jsm_user_data_from_jwt
-        from jsm_user_services.services.user import get_ltm_token
-        from jsm_user_services.services.user import get_user_email_from_jwt
-        from jsm_user_services.services.user import get_user_id_from_jwt
-        from jsm_user_services.services.user import get_user_data_from_server
-        from jsm_user_services.services.user import get_user_data_from_cpf
-        from jsm_user_services.services.user import get_cpf_from_jwt
-        
-        current_jwt_token()
-        """
-        Response example:
-        "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNTY1ODc4MjI4LCJqdGkiOiJiZDFmMzBiMGEzMTc0MmRmYjk3MTBiMzEzMTY0M2E2ZiIsInl1bnRpYW5kdSI6IjhyR0NjVHZGTE9VemR2LWRhTFk4SzdHZTF2MmVyQS01TWJOVkZ4TFBwTUNDTmRwTjQ2bDlJMHZFNG9aTmNNanRfZTh5SWJkTlczN0tKRUhWdzM3dmJjOEdLZmlfd0ZmZDJTRDlIYUJuNk80SVVabWVNUjlROVRqVTd0WFI1WDZPeFoyRDRiNXNHSWlKWGQwcGtPcXptOFpFSUl2Y2xtLUNuMjVJMklKNGJ2M2RaeTVtQUhqUnhaTmNMM2RyX1NkX1FGTFpVMWthNmtfQ0FFTkZxOE9CR1RoelNlRmtxeDFfTFBDLXE1dUVCUE9FSmpVdlF0bXhHTF8zUHNiZ0twLXFaazRfQUJ1enY1Zmk5XzFSaHJ5ZzZVWWF6WFRYNkVxcTdDdUJTUlBRMWFqM0FpU1VadGFmNjZjSTZJSThHMkxKYmd3bHhSZ19aRzY1QlpielJ3QnRvUTllUkNxY2FSRG56ZXhKVEhKMUJ0X2N6Z0J5NGxhRnFmbUZFYWZ6b3RNa0ZrZ2lLT1BNRnhMaFdaZlBEYVB0UFA0UjJjeXJEWWxaMkxNdGhrY09lZmVxMTNLa0doT0FRV2FQUHpEbzBNekRXa0VmbEVFUlpRTHo2NkItSE1TaDE1cHNBR09hUS1YcV85SWNLY05paUUzTVBfSWFpU3ZwbVQteGx2VXFiZFR5NDJkMUhhUWh6RmdPaHFoZ2F1cHoxejN0Z0VIWnNwaFdidmdBMlZQaVIyeUUzTnBLMEhPekkwMTk4NnhJRjFiRmlCOGdLMHhCQnBqRjd2bmcxU0N1OEl0TTJGRjNRQUV3czltakgyTXBMZEp5T0ViWmRGT2FLb29SeEZlY3hzRkhaV19LeEsweFdsRVBBZ2loV1NNWmNwRnpZTExiZGlLVDYtamtNckVXZ1NuRk9xajZPeWJxT05NdzRqdVZ3YTV2TTlmcVkzY0EyVlZsOU12dWlieWZRdWV1c3pJa2RaYlMyLW9YZ0oxYmZETERjckp4YWtjVXZMUE0wdmtlZjllZSIsImpzbV9pZGVudGl0eSI6ImV5SmhiR2NpT2lKSVV6STFOaUlzSW5SNWNDSTZJa3BYVkNKOS5leUpsYldGcGJDSTZJakV5TXpRMVFHeHZlV0ZzZEhsS1UwMHVZMjl0SWl3aWRXNXBjWFZsWDI1aGJXVWlPaUpoYzJRaUxDSjNaV0p6YVhSbElqb2lRMnhwWlc1MFFYQndiR2xqWVhScGIyNGlMQ0oxYVdRaU9pSTROVEEzTVdSa1pTMWlOVFk0TFRReFlXWXRZVFUzT1MwelpqUXlZekZrWmpBNU9UZ2lMQ0p6Wld4c1pYSnpJam9pTVdVellqZ3pNV1l0T1RWa01DMDBNV0UzTFdJelpURXRNV1psTURObVlXVXlNRFEySWl3aWNtOXNaU0k2SWtOMWMzUnZiV1Z5SWl3aVkyNXdhbk1pT2lJMk9DNDFPVGN1TWpnd0x6QXdNREV0TURraUxDSnVZbVlpT2pFMU5qRTFOVGd5T0Rjc0ltVjRjQ0k2TVRVMk1qRTJNekE0Tnl3aWFXRjBJam94TlRZeE5UVTRNamczTENKcGMzTWlPaUowWm5BNkx5OXBaR1Z1ZEdsMGVTNXFjMjB2WVhWMGFHOXlhWFI1SWl3aVlYVmtJam9pWW1Nd05URmtaVE10WVdWaFlTMDBZV001TFRobVltWXRNRFZoT0RabE1EZ3pabU5tSW4wLlBVQnRFbGE5ajJHSFFqNEk2TmxpVHV3cjZ4d1M4czZ2UkNWRGp6dy1QeEEifQ.oZvlK-XOBrgN9xZrChHHRdQ0rLMFTPp9jjuGvGM1U78"
-        """
-        
-        get_jsm_token()
-        """
-        Response example:
-        "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6IjY0NzIyMzM4NjEyQGxveWFsdHlKU00uY29tIiwidW5pcXVlX25hbWUiOiJUZXN0IFVzZXIiLCJ3ZWJzaXRlIjoiQ2xpZW50QXBwbGljYXRpb24iLCJ1aWQiOiI4NzM1YmY4ZC01NDc5LTQ0NDgtODNjZi04OTk5N2Q3ZGY2MDgiLCJzZWxsZXJzIjoiMWUzYjgzMWYtOTVkMC00MWE3LWIzZTEtMWZlMDNmYWUyMDQ2Iiwicm9sZSI6IkN1c3RvbWVyIiwiY25wanMiOiI2OC41OTcuMjgwLzAwMDEtMDkiLCJuYmYiOjE1NjE1NTg2MzUsImV4cCI6MTU2MjE2MzQzNSwiaWF0IjoxNTYxNTU4NjM1LCJpc3MiOiJ0ZnA6Ly9pZGVudGl0eS5qc20vYXV0aG9yaXR5IiwiYXVkIjoiYmMwNTFkZTMtYWVhYS00YWM5LThmYmYtMDVhODZlMDgzZmNmIn0.4dT-6_PmJEbWGw5Q1F18mJBQcXcVmNugQwiLxp6e4Ew"
-        """
-        get_ltm_token()
-        """
-        Response example:
-        "b51yreTQ3_4l2Z7zGsEb7UCosv-xulOtzkfflxsxTwrbOYva7loVGhxHmD6Qv5P0x5enm3LuykiAOGvf9fjDkr7qUETk5_OPONonkw1roSwHBpCCjS_IiGWdk2t2mpR4o-SFKMPfKyATzQQkBi886wMJ5g8Sg7GJNaQBHimbHDoWsvSF4zZhMin3IkD-3aVruS3IpBM6-72f4mabCB2kbtRQfTfjU5BvMYYKQzEp79_AWHbUm34gpgh5OJEt9VynHVb0Wzj-_M5sNl8uzEEQ0kixlWyueha2e5gZPHPA2TiSb0dt4WdBUqSL9BPXpsCB9TBtyRkU6JeH-DXo05Px02joOUh_MrjqhbXxYtJXWTkX4E6krHI1kS2r75DFU3dUTfQtELrvn1lQxpNCG_FAX0gB5B_XMWiX2Pn6hWE-QO9uglJgnkllxwhBBiwC1K57ony1tgpZLPY7kapAQveGmJAgWAkFXKtR2s4DK9Bkz_Xz-dUdZRONlBIH6yP4QotiE58QT0DFEluRMXhQX6huPSKuVnyaGLRrbFxdocUPuVgLTigg4rk9zgXX-GmOdHD5sxvC-cd8OWep0r7Pn5URwIdkWFjY_vly8dQDb3Cx2TXx2lXQeXBlj4XwQNlrAJTBGdmnL-Nu6Sk3oyh1_r-u53JyaF4frbt8Q6ZZsNAeZtRNLvM3l1JJ591XpApteouRRFakC6Iu8ED3IRmuzYvCgajDIDede7vtpsBvEp4yxl0"
-        """
-        
-        get_jsm_user_data_from_jwt()
-        """
-        Response example:
+# JSM User JWT Service
+
+Middleware to intercept JWT auth token and more utils functions
+
+## Local development
+
+### Running tests
+
+`docker-compose up integration-tests`
+
+### Running lint and code formatter
+
+`docker-compose up lint-formatter`
+
+## Install - For Django users
+
+`pip install jsm-user-services[drf]`
+
+Add `jsm_user_services` to your `INSTALLED_APPS`:
+
+```python
+INSTALLED_APPS = [
+    "django.contrib.admin",
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.sessions",
+    "django.contrib.messages",
+    "django.contrib.staticfiles",
+    "jsm_user_services",
+    "app_test",
+]
+```
+
+Add the Middleware:
+
+```python
+MIDDLEWARE = [
+    ...
+    "jsm_user_services.middleware.JsmJwtService",
+]
+
+# Dev url
+USER_API_HOST = "http://ishtar-gate.dev.juntossomosmaisi.com.br/api/v1"
+USER_API_TOKEN = "user_api_token"
+```
+
+## Install - For Flask users
+
+`pip install jsm-user-services[flask]`
+
+Add the middleware in your Flask app:
+
+```python
+from flask import Flask
+from jsm_user_services.flask import middleware
+
+app = Flask(__name__)
+
+middleware.JsmJwtService(app)
+app.config.update(
+    USER_API_HOST="http://ishtar-gate.dev.juntossomosmaisi.com.br/api/v1", USER_API_TOKEN="user_api_token"
+)
+```
+
+**DISCLAIMER**
+- Currently, only the middleware is implemented for Flask apps
+
+## Use
+
+```python
+from jsm_user_services.services.user import current_jwt_token
+from jsm_user_services.services.user import get_jsm_token
+from jsm_user_services.services.user import get_jsm_user_data_from_jwt
+from jsm_user_services.services.user import get_ltm_token
+from jsm_user_services.services.user import get_user_email_from_jwt
+from jsm_user_services.services.user import get_user_id_from_jwt
+from jsm_user_services.services.user import get_user_data_from_server
+from jsm_user_services.services.user import get_user_data_from_cpf
+from jsm_user_services.services.user import get_cpf_from_jwt
+
+current_jwt_token()
+"""
+Response example:
+"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNTY1ODc4MjI4LCJqdGkiOiJiZDFmMzBiMGEzMTc0MmRmYjk3MTBiMzEzMTY0M2E2ZiIsInl1bnRpYW5kdSI6IjhyR0NjVHZGTE9VemR2LWRhTFk4SzdHZTF2MmVyQS01TWJOVkZ4TFBwTUNDTmRwTjQ2bDlJMHZFNG9aTmNNanRfZTh5SWJkTlczN0tKRUhWdzM3dmJjOEdLZmlfd0ZmZDJTRDlIYUJuNk80SVVabWVNUjlROVRqVTd0WFI1WDZPeFoyRDRiNXNHSWlKWGQwcGtPcXptOFpFSUl2Y2xtLUNuMjVJMklKNGJ2M2RaeTVtQUhqUnhaTmNMM2RyX1NkX1FGTFpVMWthNmtfQ0FFTkZxOE9CR1RoelNlRmtxeDFfTFBDLXE1dUVCUE9FSmpVdlF0bXhHTF8zUHNiZ0twLXFaazRfQUJ1enY1Zmk5XzFSaHJ5ZzZVWWF6WFRYNkVxcTdDdUJTUlBRMWFqM0FpU1VadGFmNjZjSTZJSThHMkxKYmd3bHhSZ19aRzY1QlpielJ3QnRvUTllUkNxY2FSRG56ZXhKVEhKMUJ0X2N6Z0J5NGxhRnFmbUZFYWZ6b3RNa0ZrZ2lLT1BNRnhMaFdaZlBEYVB0UFA0UjJjeXJEWWxaMkxNdGhrY09lZmVxMTNLa0doT0FRV2FQUHpEbzBNekRXa0VmbEVFUlpRTHo2NkItSE1TaDE1cHNBR09hUS1YcV85SWNLY05paUUzTVBfSWFpU3ZwbVQteGx2VXFiZFR5NDJkMUhhUWh6RmdPaHFoZ2F1cHoxejN0Z0VIWnNwaFdidmdBMlZQaVIyeUUzTnBLMEhPekkwMTk4NnhJRjFiRmlCOGdLMHhCQnBqRjd2bmcxU0N1OEl0TTJGRjNRQUV3czltakgyTXBMZEp5T0ViWmRGT2FLb29SeEZlY3hzRkhaV19LeEsweFdsRVBBZ2loV1NNWmNwRnpZTExiZGlLVDYtamtNckVXZ1NuRk9xajZPeWJxT05NdzRqdVZ3YTV2TTlmcVkzY0EyVlZsOU12dWlieWZRdWV1c3pJa2RaYlMyLW9YZ0oxYmZETERjckp4YWtjVXZMUE0wdmtlZjllZSIsImpzbV9pZGVudGl0eSI6ImV5SmhiR2NpT2lKSVV6STFOaUlzSW5SNWNDSTZJa3BYVkNKOS5leUpsYldGcGJDSTZJakV5TXpRMVFHeHZlV0ZzZEhsS1UwMHVZMjl0SWl3aWRXNXBjWFZsWDI1aGJXVWlPaUpoYzJRaUxDSjNaV0p6YVhSbElqb2lRMnhwWlc1MFFYQndiR2xqWVhScGIyNGlMQ0oxYVdRaU9pSTROVEEzTVdSa1pTMWlOVFk0TFRReFlXWXRZVFUzT1MwelpqUXlZekZrWmpBNU9UZ2lMQ0p6Wld4c1pYSnpJam9pTVdVellqZ3pNV1l0T1RWa01DMDBNV0UzTFdJelpURXRNV1psTURObVlXVXlNRFEySWl3aWNtOXNaU0k2SWtOMWMzUnZiV1Z5SWl3aVkyNXdhbk1pT2lJMk9DNDFPVGN1TWpnd0x6QXdNREV0TURraUxDSnVZbVlpT2pFMU5qRTFOVGd5T0Rjc0ltVjRjQ0k2TVRVMk1qRTJNekE0Tnl3aWFXRjBJam94TlRZeE5UVTRNamczTENKcGMzTWlPaUowWm5BNkx5OXBaR1Z1ZEdsMGVTNXFjMjB2WVhWMGFHOXlhWFI1SWl3aVlYVmtJam9pWW1Nd05URmtaVE10WVdWaFlTMDBZV001TFRobVltWXRNRFZoT0RabE1EZ3pabU5tSW4wLlBVQnRFbGE5ajJHSFFqNEk2TmxpVHV3cjZ4d1M4czZ2UkNWRGp6dy1QeEEifQ.oZvlK-XOBrgN9xZrChHHRdQ0rLMFTPp9jjuGvGM1U78"
+"""
+
+get_jsm_token()
+"""
+Response example:
+"eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6IjY0NzIyMzM4NjEyQGxveWFsdHlKU00uY29tIiwidW5pcXVlX25hbWUiOiJUZXN0IFVzZXIiLCJ3ZWJzaXRlIjoiQ2xpZW50QXBwbGljYXRpb24iLCJ1aWQiOiI4NzM1YmY4ZC01NDc5LTQ0NDgtODNjZi04OTk5N2Q3ZGY2MDgiLCJzZWxsZXJzIjoiMWUzYjgzMWYtOTVkMC00MWE3LWIzZTEtMWZlMDNmYWUyMDQ2Iiwicm9sZSI6IkN1c3RvbWVyIiwiY25wanMiOiI2OC41OTcuMjgwLzAwMDEtMDkiLCJuYmYiOjE1NjE1NTg2MzUsImV4cCI6MTU2MjE2MzQzNSwiaWF0IjoxNTYxNTU4NjM1LCJpc3MiOiJ0ZnA6Ly9pZGVudGl0eS5qc20vYXV0aG9yaXR5IiwiYXVkIjoiYmMwNTFkZTMtYWVhYS00YWM5LThmYmYtMDVhODZlMDgzZmNmIn0.4dT-6_PmJEbWGw5Q1F18mJBQcXcVmNugQwiLxp6e4Ew"
+"""
+get_ltm_token()
+"""
+Response example:
+"b51yreTQ3_4l2Z7zGsEb7UCosv-xulOtzkfflxsxTwrbOYva7loVGhxHmD6Qv5P0x5enm3LuykiAOGvf9fjDkr7qUETk5_OPONonkw1roSwHBpCCjS_IiGWdk2t2mpR4o-SFKMPfKyATzQQkBi886wMJ5g8Sg7GJNaQBHimbHDoWsvSF4zZhMin3IkD-3aVruS3IpBM6-72f4mabCB2kbtRQfTfjU5BvMYYKQzEp79_AWHbUm34gpgh5OJEt9VynHVb0Wzj-_M5sNl8uzEEQ0kixlWyueha2e5gZPHPA2TiSb0dt4WdBUqSL9BPXpsCB9TBtyRkU6JeH-DXo05Px02joOUh_MrjqhbXxYtJXWTkX4E6krHI1kS2r75DFU3dUTfQtELrvn1lQxpNCG_FAX0gB5B_XMWiX2Pn6hWE-QO9uglJgnkllxwhBBiwC1K57ony1tgpZLPY7kapAQveGmJAgWAkFXKtR2s4DK9Bkz_Xz-dUdZRONlBIH6yP4QotiE58QT0DFEluRMXhQX6huPSKuVnyaGLRrbFxdocUPuVgLTigg4rk9zgXX-GmOdHD5sxvC-cd8OWep0r7Pn5URwIdkWFjY_vly8dQDb3Cx2TXx2lXQeXBlj4XwQNlrAJTBGdmnL-Nu6Sk3oyh1_r-u53JyaF4frbt8Q6ZZsNAeZtRNLvM3l1JJ591XpApteouRRFakC6Iu8ED3IRmuzYvCgajDIDede7vtpsBvEp4yxl0"
+"""
+
+get_jsm_user_data_from_jwt()
+"""
+Response example:
+{
+  "email": "64722338612@loyaltyJSM.com",
+  "unique_name": "Test User",
+  "website": "ClientApplication",
+  "uid": "8735bf8d-5479-4448-83cf-89997d7df608",
+  "sellers": "1e3b831f-95d0-41a7-b3e1-1fe03fae2046",
+  "role": "Customer",
+  "cnpjs": "68.597.280/0001-09",
+  "nbf": 1561558635,
+  "exp": 1562163435,
+  "iat": 1561558635,
+  "iss": "tfp://identity.jsm/authority",
+  "aud": "bc051de3-aeaa-4ac9-8fbf-05a86e083fcf"
+}
+"""
+
+get_user_email_from_jwt()
+"""
+Response example:
+"64722338612@loyaltyJSM.com"
+"""
+
+get_user_id_from_jwt()
+"""
+Response example:
+"85071dde-b568-41af-a579-3f42c1df0998"
+"""
+
+get_user_data_from_server()
+"""
+Response example:
+{
+    "id": "85071dde-b568-41af-a579-3f42c1df0998",
+    "username": "44444444444",
+    "cpf": "44444444444",
+    "occupation": "owner",
+    "name": "ca1bd09f-b109-435f-b6d5-206d28a3e5e2",
+    "birthday": "1990-06-15",
+    "phones": [{"number": "5511111111111", "type": "MOBILE"}],
+    "emails": [{"email": "fernando@gmail.com", "type": "PERSONAL"}],
+    "roles": ["Proprietário"],
+    "gender": "male",
+    "allow_contact": True,
+    "mediums": ["SMS", "Push"],
+    "rules_agreement": True,
+    "addresses": [
         {
-          "email": "64722338612@loyaltyJSM.com",
-          "unique_name": "Test User",
-          "website": "ClientApplication",
-          "uid": "8735bf8d-5479-4448-83cf-89997d7df608",
-          "sellers": "1e3b831f-95d0-41a7-b3e1-1fe03fae2046",
-          "role": "Customer",
-          "cnpjs": "68.597.280/0001-09",
-          "nbf": 1561558635,
-          "exp": 1562163435,
-          "iat": 1561558635,
-          "iss": "tfp://identity.jsm/authority",
-          "aud": "bc051de3-aeaa-4ac9-8fbf-05a86e083fcf"
+            "postal_code": "06763180",
+            "street": "Rua Adolfino Arruda Castanho",
+            "number": "200",
+            "complement": "Ap 133",
+            "district": "Jardim Bom Tempo",
+            "city": "Taboao da Serra",
+            "state": "SP",
+            "country": "Brazil",
+            "type": "HOME",
         }
-        """
-        
-        get_user_email_from_jwt()
-        """
-        Response example:
-        "64722338612@loyaltyJSM.com"
-        """
-        
-        get_user_id_from_jwt()
-        """
-        Response example:
-        "85071dde-b568-41af-a579-3f42c1df0998"
-        """
-        
-        get_user_data_from_server()
-        """
-        Response example:
+    ]
+}
+"""
+
+get_user_data_from_cpf(cpf)
+"""
+Response example:
+{
+    "count": 1,
+    "next": null,
+    "previous": null,
+    "results": [
         {
-            "id": "85071dde-b568-41af-a579-3f42c1df0998",
-            "username": "44444444444",
-            "cpf": "44444444444",
-            "occupation": "owner",
-            "name": "ca1bd09f-b109-435f-b6d5-206d28a3e5e2",
-            "birthday": "1990-06-15",
-            "phones": [{"number": "5511111111111", "type": "MOBILE"}],
-            "emails": [{"email": "fernando@gmail.com", "type": "PERSONAL"}],
-            "roles": ["Proprietário"],
-            "gender": "male",
-            "allow_contact": True,
-            "mediums": ["SMS", "Push"],
-            "rules_agreement": True,
-            "addresses": [
-                {
-                    "postal_code": "06763180",
-                    "street": "Rua Adolfino Arruda Castanho",
-                    "number": "200",
-                    "complement": "Ap 133",
-                    "district": "Jardim Bom Tempo",
-                    "city": "Taboao da Serra",
-                    "state": "SP",
-                    "country": "Brazil",
-                    "type": "HOME",
-                }
-            ]
-        }
-        """
-        
-        get_user_data_from_cpf(cpf)
-        """
-        Response example:
-        {
-            "count": 1,
-            "next": null,
-            "previous": null,
-            "results": [
-                {
-                    "id": "888707ab-9866-42a3-a67e-23a937cb3e7f",
-                    "created_at": "2019-10-18T20:06:44.552669Z",
-                    "updated_at": "2019-10-23T14:08:05.737326Z",
-                    "user_id_ref": "5cfd56c1-1bc1-4175-9fa9-00449ec448b8",
-                    "metadata": {
-                        "id": "5cfd56c1-1bc1-4175-9fa9-00449ec448b8",
-                        "cpf": "42879321964",
-                        "name": "Fernanda Gabrielly Duarte",
-                        "roles": [
-                            "manager"
-                        ],
-                        "emails": [
-                            {
-                                "type": "personal",
-                                "email": "fernandagabriellyduarte@ymail.com"
-                            }
-                        ],
-                        "gender": "female",
-                        "phones": [
-                            {
-                                "type": "mobile",
-                                "number": "5519991901717"
-                            }
-                        ],
-                        "status": "active",
-                        "mediums": [
-                            "sms"
-                        ],
-                        "birthday": "1982-06-04",
-                        "username": "42879321964",
-                        "addresses": [
-                            {
-                                "city": "Cascavel",
-                                "type": "main",
-                                "state": "PR",
-                                "number": "217",
-                                "street": "Rua Riachuelo",
-                                "country": "Brazil",
-                                "district": "Centro",
-                                "postal_code": "85812110"
-                            },
-                            {
-                                "city": "Cascavel",
-                                "type": "shipping",
-                                "state": "PR",
-                                "number": "217",
-                                "street": "Rua Riachuelo",
-                                "country": "Brazil",
-                                "district": "Centro",
-                                "postal_code": "85812110"
-                            }
-                        ],
-                        "occupation": "c85583ef-b602-4fea-b202-6fc5c58d8189",
-                        "allow_contact": true,
-                        "blocked_reason": null,
-                        "favorite_medium": "sms",
-                        "registered_date": "2019-10-18T20:06:31.705758+00:00",
-                        "rules_agreement": true,
-                        "rules_agreement_date": "2019-10-18T20:06:31.708640+00:00"
+            "id": "888707ab-9866-42a3-a67e-23a937cb3e7f",
+            "created_at": "2019-10-18T20:06:44.552669Z",
+            "updated_at": "2019-10-23T14:08:05.737326Z",
+            "user_id_ref": "5cfd56c1-1bc1-4175-9fa9-00449ec448b8",
+            "metadata": {
+                "id": "5cfd56c1-1bc1-4175-9fa9-00449ec448b8",
+                "cpf": "42879321964",
+                "name": "Fernanda Gabrielly Duarte",
+                "roles": [
+                    "manager"
+                ],
+                "emails": [
+                    {
+                        "type": "personal",
+                        "email": "fernandagabriellyduarte@ymail.com"
+                    }
+                ],
+                "gender": "female",
+                "phones": [
+                    {
+                        "type": "mobile",
+                        "number": "5519991901717"
+                    }
+                ],
+                "status": "active",
+                "mediums": [
+                    "sms"
+                ],
+                "birthday": "1982-06-04",
+                "username": "42879321964",
+                "addresses": [
+                    {
+                        "city": "Cascavel",
+                        "type": "main",
+                        "state": "PR",
+                        "number": "217",
+                        "street": "Rua Riachuelo",
+                        "country": "Brazil",
+                        "district": "Centro",
+                        "postal_code": "85812110"
                     },
-                    "emails": "fernandagabriellyduarte@ymail.com",
-                    "phones": "5519991901717"
-                }
-            ]
+                    {
+                        "city": "Cascavel",
+                        "type": "shipping",
+                        "state": "PR",
+                        "number": "217",
+                        "street": "Rua Riachuelo",
+                        "country": "Brazil",
+                        "district": "Centro",
+                        "postal_code": "85812110"
+                    }
+                ],
+                "occupation": "c85583ef-b602-4fea-b202-6fc5c58d8189",
+                "allow_contact": true,
+                "blocked_reason": null,
+                "favorite_medium": "sms",
+                "registered_date": "2019-10-18T20:06:31.705758+00:00",
+                "rules_agreement": true,
+                "rules_agreement_date": "2019-10-18T20:06:31.708640+00:00"
+            },
+            "emails": "fernandagabriellyduarte@ymail.com",
+            "phones": "5519991901717"
         }
-        """
-        
-        get_cpf_from_jwt()
-        """
-        Response example:
-        "09345699823"
-        """
-        
-        get_user_ip()
-        """
-        Response example:
-        "192.168.0.1" or None
-        """
-        
-        ```
-        
-        ## Versioning
-        This lib follows the [pypi version format](https://www.python.org/dev/peps/pep-0440/) with the convention of using 
-        _major_._minor_._patch_ version.
-        
-        ### When to bump a patch version?
-        Bump the patch version if you are doing a quick fix, nothing that changes the library functionality.
-        
-        ### When to bump the minor version?
-        Bump the minor version if you are adding new functionality without breaking backwards compatibility. For example, 
-        adding support to new events.
-        
-        ### When to bump the major version?
-        Bump the major version if you are breaking backwards compatibility by adding new functionality or refactoring.
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Framework :: Django :: 2.1
-Classifier: Environment :: Web Environment
-Classifier: Natural Language :: Portuguese (Brazilian)
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: drf
-Provides-Extra: flask
+    ]
+}
+"""
+
+get_cpf_from_jwt()
+"""
+Response example:
+"09345699823"
+"""
+
+get_user_ip()
+"""
+Response example:
+"192.168.0.1" or None
+"""
+
+```
+
+## Versioning
+This lib follows the [pypi version format](https://www.python.org/dev/peps/pep-0440/) with the convention of using 
+_major_._minor_._patch_ version.
+
+### When to bump a patch version?
+Bump the patch version if you are doing a quick fix, nothing that changes the library functionality.
+
+### When to bump the minor version?
+Bump the minor version if you are adding new functionality without breaking backwards compatibility. For example, 
+adding support to new events.
+
+### When to bump the major version?
+Bump the major version if you are breaking backwards compatibility by adding new functionality or refactoring.
```

### Comparing `jsm_user_services-1.3.2/README.md` & `jsm_user_services-1.3.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,51 @@
+Metadata-Version: 2.1
+Name: jsm-user-services
+Version: 1.3.3
+Summary: Middleware to intercept JWT auth token and more utils functions
+License: MIT
+Author: Juntos Somos Mais
+Author-email: labs@juntossomosmais.com.br
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.1
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Portuguese (Brazilian)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Provides-Extra: drf
+Provides-Extra: flask
+Requires-Dist: PyJWT (==2.1.0)
+Requires-Dist: requests
+Description-Content-Type: text/markdown
+
 # JSM User JWT Service
 
 Middleware to intercept JWT auth token and more utils functions
 
 ## Local development
 
 ### Running tests
 
 `docker-compose up integration-tests`
 
+### Running lint and code formatter
+
+`docker-compose up lint-formatter`
+
 ## Install - For Django users
 
 `pip install jsm-user-services[drf]`
 
 Add `jsm_user_services` to your `INSTALLED_APPS`:
 
 ```python
@@ -253,8 +287,8 @@
 Bump the patch version if you are doing a quick fix, nothing that changes the library functionality.
 
 ### When to bump the minor version?
 Bump the minor version if you are adding new functionality without breaking backwards compatibility. For example, 
 adding support to new events.
 
 ### When to bump the major version?
-Bump the major version if you are breaking backwards compatibility by adding new functionality or refactoring.
+Bump the major version if you are breaking backwards compatibility by adding new functionality or refactoring.
```

### Comparing `jsm_user_services-1.3.2/jsm_user_services/decorators/lgpd.py` & `jsm_user_services-1.3.3/jsm_user_services/decorators/lgpd.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         if not isinstance(to_be_anonymized, dict):
             raise DecoratorWrongUsage("Please, pass a dict as param.")
 
         for key, value in to_be_anonymized.items():
             if not isinstance(key, str):
                 raise DecoratorWrongUsage("The keys must be a str, got key %s of type %s", key, type(key))
-            if not isinstance(value, Callable) or not hasattr(AnonymizeLogic, value.__name__):
+            if not isinstance(value, Callable) or not hasattr(AnonymizeLogic, value.__name__):  # type: ignore
                 raise DecoratorWrongUsage("The values must be a AnonymizeLogic, got value %s", value)
 
         def main_logic(*args, **kwargs):
             """
             Method that will be executed only when the method with decorator is called. Given a field to be
             anonymized (key) and the logic that it should use (value), it anonymizes the dict to be in agreement with
             LGPD.
```

### Comparing `jsm_user_services-1.3.2/jsm_user_services/decorators/lgpd_utils.py` & `jsm_user_services-1.3.3/jsm_user_services/decorators/lgpd_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,14 @@
 
     path_to_traverse = path.split(traverse_dict_pattern)
 
     # by doing this, all changes made on "current_key" will go to "original_data" as well
     current_key = original_data
 
     while len(path_to_traverse) > 0:
-
         if isinstance(current_key, list):
             # iterating on each item to deal with them recursively
             for item in current_key:
                 traverse_within_dict_overriding_data(
                     traverse_dict_pattern.join(path_to_traverse),
                     item,
                     anonymize_logic,
```

### Comparing `jsm_user_services-1.3.2/jsm_user_services/drf_tools/helpers.py` & `jsm_user_services-1.3.3/jsm_user_services/drf_tools/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+
 from typing import Type
 from typing import Union
 
 from rest_framework.exceptions import APIException
 
 
 class AllowClassBehaviorAsFunction:
```

### Comparing `jsm_user_services-1.3.2/jsm_user_services/drf_tools/permissions.py` & `jsm_user_services-1.3.3/jsm_user_services/drf_tools/permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """
 Module with useful user permissions classes meant to be used with Django Rest Framework.
 """
 
 import logging
+
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
 
 import requests
+
 from django.conf import settings
+from rest_framework import permissions
+from rest_framework.exceptions import APIException
+from rest_framework.request import Request
+
 from jsm_user_services.drf_tools.helpers import AllowClassBehaviorAsFunction
 from jsm_user_services.drf_tools.helpers import is_exception_related_to_api_exception
 from jsm_user_services.exception import IncorrectTypePermissionConfiguration
 from jsm_user_services.services.google import perform_recaptcha_validation
 from jsm_user_services.services.user import get_user_data_from_server
-from rest_framework import permissions
-from rest_framework.exceptions import APIException
-from rest_framework.request import Request
 
 logger = logging.getLogger(__name__)
 
 
 class JSMUserBasePermission(permissions.BasePermission):
     """
     Base class for JSM user permissions. Implements methods for validating requests against
@@ -251,22 +254,22 @@
 
         g_recaptcha_response = self._retrieve_g_recaptcha_response(request)
         use_received_exception = is_exception_related_to_api_exception(self.exception_in_case_of_failed_verification)
 
         # preventing an unnecessary request to Google, since key is not defined
         if not g_recaptcha_response:
             if use_received_exception:
-                raise self.exception_in_case_of_failed_verification
+                raise self.exception_in_case_of_failed_verification  # type: ignore
             return False
 
         google_response: bool = perform_recaptcha_validation(g_recaptcha_response)
 
         if not google_response and use_received_exception:
             # raising an APIException that will return the customized response
-            raise self.exception_in_case_of_failed_verification
+            raise self.exception_in_case_of_failed_verification  # type: ignore
 
         return google_response
 
     @classmethod
     def _retrieve_g_recaptcha_response(cls, request: Request) -> Optional[str]:
         """
         Lookup on the request's body and header in order to retrieve the recaptcha key.
@@ -277,14 +280,15 @@
 
         expected_keys = ["g_recaptcha_response", "g-recaptcha-response"]
 
         for key in expected_keys:
             key_value = request.data.get(key) or request.headers.get(key)
             if key_value:
                 return key_value
+        return None
 
 
 class IsUserAllowedToPermission(JSMUserBasePermission, AllowClassBehaviorAsFunction):
     """
     A permission class which checks if user is authorized to execute an action based on 'not_allowed_to' parameter.
     Implements methods for validating requests against the user micro service and an utility method that asserts
     the user has the appropriate permission for to do, or not to do, a determined action.
@@ -297,18 +301,18 @@
                 )
             ]
 
         In this example, the custom exception should be implemented into your own project.
     """
 
     def __init__(
-            self,
-            not_allowed_to: List[str],
-            full_match: bool = False,
-            exception_in_case_of_failed: Optional[Union[APIException, Type[APIException]]] = None,
+        self,
+        not_allowed_to: List[str],
+        full_match: bool = False,
+        exception_in_case_of_failed: Optional[Union[APIException, Type[APIException]]] = None,
     ):
         """
         Sets the default value for "exception_in_case_of_failed_verification" property. It will be used to return
         a custom response, in case of this permission fails. This exception must inherit APIException,
         from rest_framework.exceptions, otherwise it will be ignored.
 
         Full match property indicates that user data must contains all the 'not_allowed_to' defined parameters.
@@ -325,15 +329,15 @@
             )
             raise IncorrectTypePermissionConfiguration(f"Expected type 'List[str]', got {type(not_allowed_to)} instead")
 
         self.not_allowed_to = not_allowed_to
 
     @classmethod
     def _verify_if_user_should_be_allowed(
-            cls, request: Request, not_allowed_actions: List[str], full_match: bool
+        cls, request: Request, not_allowed_actions: List[str], full_match: bool
     ) -> bool:
         """
         Validates 'not_allowed_to' user parameter against the 'not_allowed_actions' permission class parameter.
         """
 
         append_user_data_to_request = cls.APPEND_USER_DATA
         user_data = cls._validate_request_against_user_service(
@@ -358,14 +362,16 @@
         """
 
         use_received_exception: bool = is_exception_related_to_api_exception(
             self.exception_in_case_of_failed_verification
         )
 
         is_allowed: bool = self._verify_if_user_should_be_allowed(
-            request, not_allowed_actions=self.not_allowed_to, full_match=self.full_match,
+            request,
+            not_allowed_actions=self.not_allowed_to,
+            full_match=self.full_match,
         )
 
         if use_received_exception and not is_allowed:
-            raise self.exception_in_case_of_failed_verification
+            raise self.exception_in_case_of_failed_verification  # type: ignore
 
         return is_allowed
```

### Comparing `jsm_user_services-1.3.2/jsm_user_services/exception.py` & `jsm_user_services-1.3.3/jsm_user_services/exception.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.2/jsm_user_services/flask/middleware.py` & `jsm_user_services-1.3.3/jsm_user_services/flask/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+
 from importlib import import_module
 from typing import Optional
 
 from flask import Flask
 from flask import request
 
 from jsm_user_services.support.auth_jwt import get_bearer_authorization_token
@@ -72,15 +73,17 @@
         return get_bearer_authorization_token(authorization_value)
 
     @staticmethod
     def _get_user_ip_from_request() -> Optional[str]:
         """
         Retrieve the user ip that made this request from Flask request object
 
-        When running a service behind Akamai or other CDN solutions, it is expected that this header might contain a string with multiple IPs (comma separated values). In this case, the user's public IP that originated the request is considered to be the first one of this list.
+        When running a service behind Akamai or other CDN solutions, it is expected that this header might contain a
+        string with multiple IPs (comma separated values).
+        In this case, the user's public IP that originated the request is considered to be the first one of this list.
         For reference: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Forwarded-For
         """
         return get_first_value_from_comma_separated_string(request.headers.get(ip_address_meta_key))
 
     @staticmethod
     def _get_user_session_id_from_request() -> Optional[str]:
         bearer_token = JsmJwtService._get_jwt_token_from_request()
```

### Comparing `jsm_user_services-1.3.2/jsm_user_services/middleware.py` & `jsm_user_services-1.3.3/jsm_user_services/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 import os
+
 from typing import Optional
 
 from django.http import HttpRequest
+
 from jsm_user_services.services.user import get_session_id_from_bearer_token
 from jsm_user_services.support.auth_jwt import get_bearer_authorization_token
 from jsm_user_services.support.http_utils import convert_header_to_meta_key
 from jsm_user_services.support.local_threading_utils import add_to_local_threading
 from jsm_user_services.support.local_threading_utils import remove_from_local_threading
 from jsm_user_services.support.string_utils import get_first_value_from_comma_separated_string
 
@@ -43,15 +45,17 @@
         return get_bearer_authorization_token(authorization_value)
 
     @staticmethod
     def _get_user_ip_from_request(request: HttpRequest) -> Optional[str]:
         """
         Retrieve the user ip that made this request from Django HttpRequest object
 
-        When running a service behind Akamai or other CDN solutions, it is expected that this header might contain a string with multiple IPs (comma separated values). In this case, the user's public IP that originated the request is considered to be the first one of this list.
+        When running a service behind Akamai or other CDN solutions, it is expected that this header might contain
+        a string with multiple IPs (comma separated values).
+        In this case, the user's public IP that originated the request is considered to be the first one of this list.
         For reference: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Forwarded-For
         """
         first_attempt_value = request.META.get(header_with_client_ip_address)
         if first_attempt_value:
             return first_attempt_value.strip()
 
         second_attempt_value = request.META.get(header_with_list_of_addresses)
```

### Comparing `jsm_user_services-1.3.2/jsm_user_services/services/everest.py` & `jsm_user_services-1.3.3/jsm_user_services/services/everest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from requests import Response
 from typing_extensions import TypedDict
@@ -13,15 +14,15 @@
 from jsm_user_services.support.http_utils import get_response_body
 from jsm_user_services.support.http_utils import request
 from jsm_user_services.support.settings_utils import get_from_settings_or_raise_missing_config
 
 logger = logging.getLogger(__name__)
 
 
-DEFAULT_VALIDATORS_FUNCTION = [validate_format_email]
+DEFAULT_VALIDATORS_FUNCTION: List[Callable] = [validate_format_email]
 
 
 class ValidationResult(TypedDict):
     is_valid: bool
     external_api_validation: bool
 
 
@@ -31,15 +32,15 @@
     functions_to_validate_email: Optional[List[Callable]] = None,
 ) -> ValidationResult:
     """
     Parameters:
         `email (str)`: the e-mail that will be validated
         `use_callback_function_validator (bool)`: indicates if some validators must be considered if the `status_code`
         is different from 200 (success)
-        `functions_to_validate_email (List[Callable])`: a list of validators that will be considered if the `status_code`
+        `functions_to_validate_email (List[Callable])`: list of validators that will be considered if the `status_code`
         is different from 200 (success) and the `use_callback_function_validator` is `False`
 
     Returns:
         A dict containing two values:
         - `is_valid (bool)`: indicates if the email string is valid
         - `external_api_validation (bool)`: indicates if the email validation was made by Everest or locally
 
@@ -68,16 +69,16 @@
     )
     EVEREST_LIST_INVALIDS_STATUS_RESPONSES = get_from_settings_or_raise_missing_config(
         "EVEREST_LIST_INVALIDS_STATUS_RESPONSES", "invalid"
     )
     invalid_status_list = EVEREST_LIST_INVALIDS_STATUS_RESPONSES.split(",")
     try:
         email_validation_response: Dict = get_email_validation(email)
-        results: Dict = email_validation_response.get("results") or {}
-        status: str = results.get("status")
+        results: dict = email_validation_response.get("results") or {}
+        status: Optional[str] = results.get("status")
         is_valid: bool = status not in invalid_status_list and status is not None
         return ValidationResult(is_valid=is_valid, external_api_validation=True)
     except Exception as err:
         logger.warning(f"Everest API Response Failed: {err}")
         if use_callback_function_validator:
             return ValidationResult(
                 is_valid=perform_callback_function_validators(
```

### Comparing `jsm_user_services-1.3.2/jsm_user_services/services/google.py` & `jsm_user_services-1.3.3/jsm_user_services/services/google.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     if user_ip:
         data["remoteip"] = user_ip
 
     logger.debug("Performing request to Google to check if recaptcha is valid")
 
     with request() as r:
         resp = r.post(google_recaptcha_url, data=data, headers=headers)
-    
+
     result_json = resp.json()
 
     logger.info(f"Status code: {resp.status_code}; min_score_threshold: {min_score_threshold}, body: {result_json}")
 
     if resp.status_code != 200:
         logger.info(f"GoogleRecaptcha response {g_recaptcha_response} status: {resp.status_code} failed: {result_json}")
         return False
```

### Comparing `jsm_user_services-1.3.2/jsm_user_services/services/user.py` & `jsm_user_services-1.3.3/jsm_user_services/services/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import hashlib
+
 from importlib import import_module
 from typing import List
 from typing import Optional
 
 from jsm_user_services.support.auth_jwt import get_decoded_jwt_token
 from jsm_user_services.support.http_utils import get_response_body
 from jsm_user_services.support.http_utils import request
 from jsm_user_services.support.local_threading_utils import get_from_local_threading
 from jsm_user_services.support.request_id import current_request_id
+from jsm_user_services.support.request_id import request_id_header_name
 
 
 def jwt_has_required_roles(jwt_required_roles: List[str], assert_all=True) -> bool:
     """
     Asserts that the jwt token has all the required roles.
     """
     jsm_token_data = get_jsm_user_data_from_jwt()
@@ -83,72 +85,68 @@
     if user_data:
         return user_data.get("fid", None)
 
     return None
 
 
 def get_user_data_from_server() -> dict:
-
     current_token = current_jwt_token()
-    headers = {"REQUEST-ID": current_request_id()}
+    headers = {request_id_header_name: current_request_id()}
     settings = import_module("jsm_user_services.settings")
     user_url = settings.USER_API_HOST
 
     if current_token:
         headers["Authorization"] = f"Bearer {current_jwt_token()}"
 
     with request() as r:
         response = r.get(f"{user_url}/users/me/", headers=headers)
         return get_response_body(response)
 
 
 def get_user_data_from_cpf(cpf: str) -> dict:
-
     current_token = current_jwt_token()
-    headers = {"REQUEST-ID": current_request_id()}
+    headers = {request_id_header_name: current_request_id()}
     settings = import_module("jsm_user_services.settings")
     user_url = settings.USER_API_HOST
 
     if current_token:
         headers["Authorization"] = f"Bearer {current_jwt_token()}"
 
     with request() as r:
         response = r.get(f"{user_url}/users/search?cpf={cpf}", headers=headers)
         return get_response_body(response)
 
 
 def get_user_data_from_id(user_id: str) -> dict:
-
     current_token = current_jwt_token()
-    headers = {"REQUEST-ID": current_request_id()}
+    headers = {request_id_header_name: current_request_id()}
     settings = import_module("jsm_user_services.settings")
     user_url = settings.USER_API_HOST
 
     if current_token:
         headers["Authorization"] = f"Bearer {current_jwt_token()}"
 
     with request() as r:
         response = r.get(f"{user_url}/users/{user_id}/", headers=headers)
 
         return get_response_body(response)
 
 
 def get_cpf_from_jwt() -> Optional[str]:
-
     email = get_user_email_from_jwt()
 
     return email.split("@")[0] if email else None
 
 
 def is_retail_user(user_id: str) -> bool:
     settings = import_module("jsm_user_services.settings")
     user_api_token = settings.USER_API_TOKEN
     user_url = settings.USER_API_HOST
 
-    headers = {"REQUEST-ID": current_request_id(), "Authorization": f"Token {user_api_token}"}
+    headers = {request_id_header_name: current_request_id(), "Authorization": f"Token {user_api_token}"}
 
     with request() as r:
         response = r.get(f"{user_url}/users/search/?user_id_ref={user_id}&is_retail_user=True", headers=headers)
         response_content = get_response_body(response)
     return response_content["count"] == 1
```

### Comparing `jsm_user_services-1.3.2/jsm_user_services/settings.py` & `jsm_user_services-1.3.3/jsm_user_services/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,7 +36,8 @@
 GOOGLE_RECAPTCHA_URL = get_setting_from_app("GOOGLE_RECAPTCHA_URL")
 GOOGLE_RECAPTCHA_SECRET_KEY = get_setting_from_app("GOOGLE_RECAPTCHA_SECRET_KEY")
 GOOGLE_RECAPTCHA_SCORE_THRESHOLD = get_setting_from_app("GOOGLE_RECAPTCHA_SCORE_THRESHOLD")
 GOOGLE_RECAPTCHA_BYPASS_IP_HEADER_NAME = get_setting_from_app("GOOGLE_RECAPTCHA_BYPASS_IP_HEADER_NAME")
 EVEREST_API_KEY = get_setting_from_app("EVEREST_API_KEY")
 EVEREST_API_HOST = get_setting_from_app("EVEREST_API_HOST")
 EVEREST_LIST_INVALIDS_STATUS_RESPONSES = get_setting_from_app("EVEREST_LIST_INVALIDS_STATUS_RESPONSES")
+REQUEST_ID_CONFIG = get_setting_from_app("REQUEST_ID_CONFIG")
```

### Comparing `jsm_user_services-1.3.2/jsm_user_services/support/auth_jwt.py` & `jsm_user_services-1.3.3/jsm_user_services/support/auth_jwt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+
 from typing import Optional
 
 import jwt
 
 
 def get_decoded_jwt_token(jwt_token: str) -> dict:
     """
```

### Comparing `jsm_user_services-1.3.2/jsm_user_services/support/email_utils.py` & `jsm_user_services-1.3.3/jsm_user_services/support/email_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import re
+
 from typing import Callable
 from typing import List
 
 
 def validate_format_email(email: str) -> bool:
     """
     Check if the given string has a valid format e-mail
     """
-    regex = r'\b^[A-Za-z0-9](([_\.\-]?[a-zA-Z0-9\_]+)*)@([A-Za-z0-9]+)(([\.\-]?[a-zA-Z0-9]+)*)\.([A-Za-z]{2,})$\b'
+    regex = r"\b^[A-Za-z0-9](([_\.\-]?[a-zA-Z0-9\_]+)*)@([A-Za-z0-9]+)(([\.\-]?[a-zA-Z0-9]+)*)\.([A-Za-z]{2,})$\b"
     return bool(re.match(regex, email))
 
 
 def perform_callback_function_validators(functions_to_validate_email: List[Callable], email: str) -> bool:
     """
     Returns if the e-mail is valid by `functions_to_validate_email`
         Parameters:
```

### Comparing `jsm_user_services-1.3.2/jsm_user_services/support/http_utils.py` & `jsm_user_services-1.3.3/jsm_user_services/support/http_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 HTTP utils module
 """
 import functools
 import logging
+
 from contextlib import contextmanager
 from importlib import import_module
 from typing import Any
 from typing import Generator
 from typing import Optional
 
 from requests import Response
@@ -35,15 +36,15 @@
     session = Session()
     session.hooks.update(response=[_log_response, _check_for_errors])
     max_retries = Retry(total=total, backoff_factor=backoff_factor, **kwargs)
     adapter = HTTPAdapter(max_retries=max_retries)
     session.mount("https://", adapter)
     session.mount("http://", adapter)
 
-    session.request = functools.partial(session.request, timeout=JSM_USER_SERVICE_HTTP_TIMEOUT)
+    session.request = functools.partial(session.request, timeout=JSM_USER_SERVICE_HTTP_TIMEOUT)  # type: ignore
     try:
         yield session
     finally:
         session.close()
 
 
 def get_response_body(response: Response) -> Any:
@@ -53,18 +54,18 @@
     try:
         response_body = response.json()
     except ValueError:
         response_body = response.text
     return response_body
 
 
-def convert_header_to_meta_key(header: Optional[str]) -> str:
+def convert_header_to_meta_key(header: Optional[str]) -> Optional[str]:
     """
     Django Http Request has a dictionary called META with the request headers.
-    But it replace the header name following the rules:
+    But it replaces the header name following the rules:
       - all characters to uppercase
       - replacing any hyphens with underscores
       - adding an HTTP_ prefix to the name.
     So, for example, a header called X-Bender would be mapped to the META key HTTP_X_BENDER.
     """
     if header is None:
         return None
```

### Comparing `jsm_user_services-1.3.2/jsm_user_services/support/settings_utils.py` & `jsm_user_services-1.3.3/jsm_user_services/support/settings_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.2/setup.py` & `jsm_user_services-1.3.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,73 @@
-import os
+[tool.poetry]
+name = "jsm-user-services"
+version = "1.3.3"
+description = "Middleware to intercept JWT auth token and more utils functions"
+authors = ["Juntos Somos Mais <labs@juntossomosmais.com.br>"]
+license = "MIT"
+readme = "README.md"
+packages = [{include = "jsm_user_services"}]
+classifiers=[
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3.7",
+    "Framework :: Django :: 2.1",
+    "Environment :: Web Environment",
+    "Natural Language :: Portuguese (Brazilian)",
+    "Development Status :: 4 - Beta",
+    "Framework :: Django",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
 
-from setuptools import find_packages
-from setuptools import setup
+[tool.poetry.dependencies]
+python = "^3.7"
+PyJWT = "2.1.0"
+requests = "*"
 
-with open(os.path.join(os.path.dirname(__file__), "README.md")) as readme:
-    README = readme.read()
+[tool.poetry.extras]
+flask = ["flask", "flask-log-request-id"]
+drf = ["djangorestframework", "request-id-django-log"]
 
-os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
-
-setup(
-    name="jsm_user_services",
-    version="1.3.2",
-    description="Middleware to intercept JWT auth token and more utils functions",
-    long_description=README,
-    long_description_content_type="text/markdown",
-    include_package_data=True,
-    author="Juntos Somos Mais",
-    author_email="labs@juntossomosmais.com.br",
-    license="MIT",
-    url="https://github.com/juntossomosmais/jsm-user-service",
-    packages=find_packages(),
-    install_requires=["PyJWT==2.1.0", "requests"],
-    extras_require={
-        "drf": ["djangorestframework", "request-id-django-log"],
-        "flask": ["flask", "flask-log-request-id"],
-    },
-    classifiers=[
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
-        "Framework :: Django :: 2.1",
-        "Environment :: Web Environment",
-        "Natural Language :: Portuguese (Brazilian)",
-        "Development Status :: 4 - Beta",
-        "Framework :: Django",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-)
+[tool.poetry.group.dev.dependencies]
+django = "*"
+PyJWT = "*"
+pluggy = "*"
+request-id-django-log = "*"
+djangorestframework = "*"
+flask = "*"
+flask-log-request-id = "*"
+
+pytest_django = "*"
+requests-mock = "*"
+pytest = "*"
+pytest-cov = "*"
+pytest-mock = "*"
+httpretty = "*"
+pre-commit = "v2.21.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 120
+py36 = true
+include = '\.pyi?$'
+exclude = '''
+/(
+    \.eggs
+  | \.git
+  | \.hg
+  | \.mypy_cache
+  | \.tox
+  | \.venv
+  | _build
+  | buck-out
+  | build
+  | dist
+
+  # The following are specific to Black, you probably don't want those.
+  | blib2to3
+  | tests/data
+)/
+'''
```

### Comparing `jsm_user_services-1.3.2/tests/test_request_id.py` & `jsm_user_services-1.3.3/jsm_user_services/support/request_id.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,47 @@
-import pytest
-from flask_log_request_id.ctx_fetcher import MultiContextRequestIdFetcher
-from pytest_mock import MockFixture
-from request_id_django_log import local_threading
+from importlib import import_module
+from typing import Callable
 
 from jsm_user_services.exception import RequestIDModuleNotFound
-from jsm_user_services.support.request_id import get_current_request_id_callable
-from jsm_user_services.support.request_id import import_module_otherwise_none
+from jsm_user_services.support.import_utils import import_module_otherwise_none
 
 
-@pytest.fixture
-def no_flask_request_id_module(mocker: MockFixture):
-    def mock_only_if_flask_log_request_id_module(module_to_import: str):
-        if module_to_import == "flask_log_request_id":
-            return None
-        return import_module_otherwise_none(module_to_import)
-
-    mocker.patch(
-        "jsm_user_services.support.request_id.import_module_otherwise_none",
-        side_effect=mock_only_if_flask_log_request_id_module,
+def get_request_id_header_name() -> str:
+    """
+    Helper function to get request_id header name to included in request to another application
+    REQUEST_ID_CONFIG dict configuration exists in the projects with similarity structure below
+    REQUEST_ID_CONFIG = {
+        "REQUEST_ID_HEADER": "HTTP_X_REQUEST_ID",
+        "GENERATE_REQUEST_ID_IF_NOT_FOUND": True,
+        "RESPONSE_HEADER_REQUEST_ID": "HTTP_X_REQUEST_ID",
+    }
+    """
+    settings = import_module("jsm_user_services.settings")
+    default_request_id_header_name = getattr(settings, "REQUEST_ID_HEADER_NAME", "HTTP_X_REQUEST_ID")
+    default_request_id_config = {
+        "GENERATE_REQUEST_ID_IF_NOT_FOUND": True,
+        "REQUEST_ID_HEADER": default_request_id_header_name,
+        "RESPONSE_HEADER_REQUEST_ID": default_request_id_header_name,
+    }
+    request_id_config = getattr(settings, "REQUEST_ID_CONFIG", default_request_id_config)
+    if request_id_config and type(request_id_config) == dict and request_id_config.get("REQUEST_ID_HEADER"):
+        return request_id_config.get("REQUEST_ID_HEADER", default_request_id_header_name)
+    return default_request_id_header_name
+
+
+def get_current_request_id_callable() -> Callable:
+    django_request_id_module, flask_request_id_module = (
+        import_module_otherwise_none("request_id_django_log.request_id"),
+        import_module_otherwise_none("flask_log_request_id"),
     )
 
+    if django_request_id_module is not None:
+        return django_request_id_module.current_request_id
 
-@pytest.fixture
-def no_django_request_id_module(mocker: MockFixture):
-    def mock_only_if_django_request_id_module(module_to_import: str):
-        if module_to_import == "request_id_django_log.request_id":
-            return None
-        return import_module_otherwise_none(module_to_import)
-
-    mocker.patch(
-        "jsm_user_services.support.request_id.import_module_otherwise_none",
-        side_effect=mock_only_if_django_request_id_module,
-    )
-
-
-@pytest.fixture
-def no_request_id_module_found(mocker: MockFixture):
-    mocker.patch("jsm_user_services.support.request_id.import_module_otherwise_none", return_value=None)
-
-
-def test_should_successfully_retrieve_current_request_id_for_django_app(no_flask_request_id_module: None):
-    local_threading.request_id, current_request_id = ("django", get_current_request_id_callable())
-
-    django_request_id = current_request_id()
-
-    assert django_request_id == local_threading.request_id
-
-    del local_threading.request_id
-
-
-def test_should_succesfully_retrieve_current_request_id_for_flask_app(no_django_request_id_module: None):
-    current_request_id = get_current_request_id_callable()
+    if flask_request_id_module is not None:
+        return flask_request_id_module.current_request_id
 
-    assert isinstance(current_request_id, MultiContextRequestIdFetcher)
+    raise RequestIDModuleNotFound
 
 
-def test_should_raise_exception_when_request_id_module_is_not_found(no_request_id_module_found: None):
-    with pytest.raises(RequestIDModuleNotFound):
-        get_current_request_id_callable()
+current_request_id = get_current_request_id_callable()
+request_id_header_name = get_request_id_header_name()
```

