# Comparing `tmp/oidc-client-0.1.2.tar.gz` & `tmp/oidc_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc-client-0.1.2.tar", max compression
+gzip compressed data, was "oidc_client-0.1.3.tar", max compression
```

## Comparing `oidc-client-0.1.2.tar` & `oidc_client-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1085 2022-09-13 23:42:27.771376 oidc-client-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     1069 2022-09-13 23:42:27.771376 oidc-client-0.1.2/README.md
--rw-r--r--   0        0        0      487 2022-09-13 23:42:27.772376 oidc-client-0.1.2/oidc_client/__init__.py
--rw-r--r--   0        0        0       30 2022-09-13 23:42:27.772376 oidc-client-0.1.2/oidc_client/__main__.py
--rw-r--r--   0        0        0     4815 2022-09-13 23:42:27.772376 oidc-client-0.1.2/oidc_client/cli.py
--rw-r--r--   0        0        0     3548 2022-09-13 23:42:27.772376 oidc-client-0.1.2/oidc_client/config.py
--rw-r--r--   0        0        0      925 2022-09-13 23:42:27.772376 oidc-client-0.1.2/oidc_client/discovery.py
--rw-r--r--   0        0        0      488 2022-09-13 23:42:27.772376 oidc-client-0.1.2/oidc_client/error.py
--rw-r--r--   0        0        0      215 2022-09-13 23:42:27.772376 oidc-client-0.1.2/oidc_client/index.html
--rw-r--r--   0        0        0     1791 2022-09-13 23:42:27.772376 oidc-client-0.1.2/oidc_client/lib.py
--rw-r--r--   0        0        0     1123 2022-09-13 23:42:27.772376 oidc-client-0.1.2/oidc_client/localhost.crt
--rw-r--r--   0        0        0     1704 2022-09-13 23:42:27.772376 oidc-client-0.1.2/oidc_client/localhost.key
--rw-r--r--   0        0        0     7512 2022-09-13 23:42:27.772376 oidc-client-0.1.2/oidc_client/oauth.py
--rw-r--r--   0        0        0      807 2022-09-13 23:42:27.772376 oidc-client-0.1.2/oidc_client/pkce.py
--rw-r--r--   0        0        0      523 2022-09-13 23:42:27.772376 oidc-client-0.1.2/oidc_client/tls.py
--rw-r--r--   0        0        0     1250 2022-09-13 23:42:27.773376 oidc-client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 oidc-client-0.1.2/setup.py
--rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 oidc-client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-20 11:14:26.451110 oidc_client-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     1069 2023-04-20 11:14:26.451110 oidc_client-0.1.3/README.md
+-rw-r--r--   0        0        0      541 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/__main__.py
+-rw-r--r--   0        0        0     4815 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/cli.py
+-rw-r--r--   0        0        0     3540 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/config.py
+-rw-r--r--   0        0        0      925 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/discovery.py
+-rw-r--r--   0        0        0      488 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/error.py
+-rw-r--r--   0        0        0      215 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/index.html
+-rw-r--r--   0        0        0     1791 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/lib.py
+-rw-r--r--   0        0        0     1123 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/localhost.crt
+-rw-r--r--   0        0        0     1704 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/localhost.key
+-rw-r--r--   0        0        0     7603 2023-04-20 11:14:26.452111 oidc_client-0.1.3/oidc_client/oauth.py
+-rw-r--r--   0        0        0      807 2023-04-20 11:14:26.452111 oidc_client-0.1.3/oidc_client/pkce.py
+-rw-r--r--   0        0        0      556 2023-04-20 11:14:26.452111 oidc_client-0.1.3/oidc_client/tls.py
+-rw-r--r--   0        0        0     1320 2023-04-20 11:14:26.452111 oidc_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 oidc_client-0.1.3/PKG-INFO
```

### Comparing `oidc-client-0.1.2/LICENSE.md` & `oidc_client-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oidc-client-0.1.2/README.md` & `oidc_client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `oidc-client-0.1.2/oidc_client/cli.py` & `oidc_client-0.1.3/oidc_client/cli.py`

 * *Files identical despite different names*

### Comparing `oidc-client-0.1.2/oidc_client/config.py` & `oidc_client-0.1.3/oidc_client/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from urllib.parse import urlparse
 
 from .error import ProviderConfigError
 
 # FIXME: type-check when we drop support for Python 3.10
 try:
-    import tomllib  # type: ignore
+    import tomllib
 except ImportError:
     import toml as tomllib  # type: ignore
 
 DEFAULT_CONFIG_FILE = "pyproject.toml"
 
 DEFAULT_OIDC_SCOPE = "openid profile email"
 DEFAULT_REDIRECT_URI = "http://127.0.0.1:39303/oauth2/callback"
@@ -67,15 +67,15 @@
     profile_name: str | None = None,
     overrides: argparse.Namespace | None = None,
 ) -> ClientProfile:
     """Read an (optionally named) OIDC client profile from a config file."""
     data = {}
     try:
         with open(path) as config_file:
-            data = tomllib.load(config_file)["tool"]["oidc"]
+            data = tomllib.loads(config_file.read())["tool"]["oidc"]
             if profile_name:
                 data = data[profile_name]
     except FileNotFoundError:
         pass
 
     overrides = overrides or argparse.Namespace()
```

### Comparing `oidc-client-0.1.2/oidc_client/discovery.py` & `oidc_client-0.1.3/oidc_client/discovery.py`

 * *Files identical despite different names*

### Comparing `oidc-client-0.1.2/oidc_client/lib.py` & `oidc_client-0.1.3/oidc_client/lib.py`

 * *Files identical despite different names*

### Comparing `oidc-client-0.1.2/oidc_client/localhost.crt` & `oidc_client-0.1.3/oidc_client/localhost.crt`

 * *Files identical despite different names*

### Comparing `oidc-client-0.1.2/oidc_client/localhost.key` & `oidc_client-0.1.3/oidc_client/localhost.key`

 * *Files identical despite different names*

### Comparing `oidc-client-0.1.2/oidc_client/oauth.py` & `oidc_client-0.1.3/oidc_client/oauth.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 
 import base64
 import json
 import random
 import string
 import webbrowser
 from dataclasses import dataclass, fields
-from enum import Enum
 from http import HTTPStatus
 from http.server import BaseHTTPRequestHandler, HTTPServer
-from importlib import resources
+from importlib.resources import files
 from typing import cast
 from urllib.error import HTTPError
 from urllib.parse import parse_qs, urlencode, urlparse
 from urllib.request import Request, urlopen
 
 from .error import AuthorizationError, RedirectionError
 from .pkce import PKCESecret
 from .tls import setup_tls
 
+try:
+    from enum import StrEnum
+except ImportError:
+    from strenum import StrEnum  # type: ignore
+
 
 class AuthorizationCodeHandler(BaseHTTPRequestHandler):
     """OAuth 2.1 authorization code flow (with PKCE) HTTP handler."""
 
     def __init__(
         self, request: bytes, client_address: tuple[str, int], server: RedirectionServer
     ):
@@ -73,15 +77,15 @@
             return
 
         self.send_response(HTTPStatus.OK)
         self.send_header("Connection", "close")
         self.send_header("Content-type", "text/html;utf-8")
         self.end_headers()
 
-        self.wfile.write(resources.read_binary(__package__, "index.html"))
+        self.wfile.write(files(__package__).joinpath("index.html").read_bytes())
 
 
 class RedirectionServer(HTTPServer):
     """OAuth 2.1 authorization code flow (with PKCE) HTTP server."""
 
     def __init__(
         self,
@@ -156,15 +160,15 @@
             raise AuthorizationError(  # pragma: no cover
                 "no authorization code, unknown error."
             )
 
     return httpd.code
 
 
-class GrantType(str, Enum):
+class GrantType(StrEnum):
     """OAuth 2.1 authorization grant types."""
 
     AUTHORIZATION_CODE = "authorization_code"
     CLIENT_CREDENTIALS = "client_credentials"
 
 
 @dataclass(frozen=True)
```

### Comparing `oidc-client-0.1.2/oidc_client/pkce.py` & `oidc_client-0.1.3/oidc_client/pkce.py`

 * *Files identical despite different names*

### Comparing `oidc-client-0.1.2/pyproject.toml` & `oidc_client-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oidc-client"
-version = "0.1.2"
+version = "0.1.3"
 description = "A pure-Python OpenID Connect client"
 readme = "README.md"
 keywords = ["openid", "oidc", "oauth", "oauth2"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Topic :: Internet :: WWW/HTTP",
@@ -16,14 +16,15 @@
 
 [tool.poetry.scripts]
 oidc = "oidc_client.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 toml = { version = "^0.10.2", allow-prereleases = true, python = "<3.11" }
+StrEnum = { version = "^0.4.10", allow-prereleases = true, python = "<3.11" }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 flake8 = "^5.0.4"
 mypy = "^0.971"
 isort = "^5.10.1"
 black = "^22.6.0"
@@ -48,9 +49,9 @@
 [[tool.mypy.overrides]]
 module = "tests.*"
 ignore_errors = true
 
 
 # Example OIDC application
 [tool.oidc]
-issuer = "https://gitlab.com"
-client_id = "9ed8f309fe97b34d16afff0520a291f28e93a8991cfefeadc56203b2a79414c5"
+issuer = "https://dev-p2fx5mb1m0jeec4k.us.auth0.com/"
+client_id = "rBbLsINtTdZuUSXBCWZ8PNWjK5Z9fEmR"
```

### Comparing `oidc-client-0.1.2/PKG-INFO` & `oidc_client-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: oidc-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pure-Python OpenID Connect client
 Home-page: https://gitlab.com/lzinsou/oidc-client
 Keywords: openid,oidc,oauth,oauth2
 Author: Loris Zinsou
 Author-email: lzinsou@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Dist: toml (>=0.10.2,<0.11.0); python_version < "3.11"
+Requires-Dist: StrEnum (>=0.4.10,<0.5.0) ; python_version < "3.11"
+Requires-Dist: toml (>=0.10.2,<0.11.0) ; python_version < "3.11"
 Project-URL: Repository, https://gitlab.com/lzinsou/oidc-client
 Description-Content-Type: text/markdown
 
 OIDC Client
 ===========
 
 A pure-Python OpenID Connect client supporting OAuth 2.1 authorization flows, built for Python 3.10+ with minimal dependencies.
```

