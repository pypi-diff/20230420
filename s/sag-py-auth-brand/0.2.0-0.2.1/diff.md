# Comparing `tmp/sag-py-auth-brand-0.2.0.tar.gz` & `tmp/sag-py-auth-brand-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-auth-brand-0.2.0.tar", last modified: Thu Apr  6 11:14:33 2023, max compression
+gzip compressed data, was "sag-py-auth-brand-0.2.1.tar", last modified: Thu Apr 20 08:23:33 2023, max compression
```

## Comparing `sag-py-auth-brand-0.2.0.tar` & `sag-py-auth-brand-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:14:33.598403 sag-py-auth-brand-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-06 11:14:33.598403 sag-py-auth-brand-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:14:33.598403 sag-py-auth-brand-0.2.0/sag_py_auth_brand/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/sag_py_auth_brand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/sag_py_auth_brand/brand_jwt_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/sag_py_auth_brand/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/sag_py_auth_brand/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/sag_py_auth_brand/request_brand_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/sag_py_auth_brand/request_brand_logging_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:14:33.598403 sag-py-auth-brand-0.2.0/sag_py_auth_brand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-06 11:14:33.000000 sag-py-auth-brand-0.2.0/sag_py_auth_brand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-06 11:14:33.000000 sag-py-auth-brand-0.2.0/sag_py_auth_brand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 11:14:33.000000 sag-py-auth-brand-0.2.0/sag_py_auth_brand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-06 11:14:33.000000 sag-py-auth-brand-0.2.0/sag_py_auth_brand.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-06 11:14:33.000000 sag-py-auth-brand-0.2.0/sag_py_auth_brand.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-06 11:14:33.602403 sag-py-auth-brand-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:14:33.598403 sag-py-auth-brand-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/tests/test_brand_jwt_auth__call.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/tests/test_brand_jwt_auth__init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/tests/test_brand_jwt_auth__verify_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/tests/test_brand_jwt_auth__verify_brand_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/tests/test_request_brand_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-06 11:14:18.000000 sag-py-auth-brand-0.2.0/tests/test_request_brand_logging_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:23:33.818901 sag-py-auth-brand-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-04-20 08:23:33.818901 sag-py-auth-brand-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:23:33.818901 sag-py-auth-brand-0.2.1/sag_py_auth_brand/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand/brand_jwt_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand/request_brand_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand/request_brand_logging_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:23:33.818901 sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-04-20 08:23:33.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-20 08:23:33.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 08:23:33.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 08:23:33.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 08:23:33.000000 sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 08:23:33.822901 sag-py-auth-brand-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:23:33.818901 sag-py-auth-brand-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/tests/test_brand_jwt_auth__call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/tests/test_brand_jwt_auth__init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/tests/test_brand_jwt_auth__verify_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/tests/test_brand_jwt_auth__verify_brand_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/tests/test_request_brand_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-20 08:23:23.000000 sag-py-auth-brand-0.2.1/tests/test_request_brand_logging_filter.py
```

### Comparing `sag-py-auth-brand-0.2.0/LICENSE.txt` & `sag-py-auth-brand-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-auth-brand-0.2.0/sag_py_auth_brand.egg-info/SOURCES.txt` & `sag-py-auth-brand-0.2.1/sag_py_auth_brand.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 sag_py_auth_brand/__init__.py
 sag_py_auth_brand/brand_jwt_auth.py
+sag_py_auth_brand/constants.py
 sag_py_auth_brand/models.py
-sag_py_auth_brand/py.typed
 sag_py_auth_brand/request_brand_context.py
 sag_py_auth_brand/request_brand_logging_filter.py
 sag_py_auth_brand.egg-info/PKG-INFO
 sag_py_auth_brand.egg-info/SOURCES.txt
 sag_py_auth_brand.egg-info/dependency_links.txt
 sag_py_auth_brand.egg-info/requires.txt
 sag_py_auth_brand.egg-info/top_level.txt
```

### Comparing `sag-py-auth-brand-0.2.0/setup.py` & `sag-py-auth-brand-0.2.1/setup.py`

 * *Files 9% similar despite different names*

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
     name="sag-py-auth-brand",
-    version="0.2.0",
+    version="0.2.1",
     description="Keycloak brand/instance authentication for python projects",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_auth_brand",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
@@ -22,15 +25,15 @@
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development",
     ],
     keywords="auth, fastapi, keycloak",
     packages=setuptools.find_packages(exclude=["tests"]),
-    package_data={"sag_py_auth_brand": ["py.typed"]},
+    package_data={"sag_py_auth_brand": REQS_DEV},
     python_requires=">=3.8",
     install_requires=REQS,
     extras_require={"dev": ["pytest"]},
     project_urls={
         "Documentation": "https://github.com/SamhammerAG/sag_py_auth_brand",
         "Bug Reports": "https://github.com/SamhammerAG/sag_py_auth_brand/issues",
         "Source": "https://github.com/SamhammerAG/sag_py_auth_brand",
```

### Comparing `sag-py-auth-brand-0.2.0/tests/test_brand_jwt_auth__call.py` & `sag-py-auth-brand-0.2.1/tests/test_brand_jwt_auth__call.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,44 @@
 from typing import Literal, Tuple
 
 import pytest
 from fastapi import Request
-from pytest import MonkeyPatch
 from sag_py_auth.models import Token
 from starlette.datastructures import Headers
 
 from sag_py_auth_brand.brand_jwt_auth import BrandJwtAuth
-from sag_py_auth_brand.models import BrandAuthConfig
-from tests.helpers import get_token
+from tests.helpers import build_sample_jwt_auth, get_token
 
 pytest_plugins: Tuple[Literal["pytest_asyncio"]] = ("pytest_asyncio",)
 
 
-async def jwt_auth_call_mock(self: BrandJwtAuth, request: Request) -> Token:
+async def mock_jwt_auth_call(_: BrandJwtAuth, __: Request) -> Token:
     return get_token(None, None)
 
 
-def _verify_brand_mock(self: BrandJwtAuth, token: Token, brand: str) -> None:
+def mock_verify_brand(_: BrandJwtAuth, token: Token, request_brand: str) -> None:
     if token:
         token.token_dict["_verify_brand"] = "True"
-
-
-was_brand_set_to_context = False
-
-
-def set_brand_to_context_mock(brand_to_set: str) -> None:
-    global was_brand_set_to_context
-    was_brand_set_to_context = True
+        token.token_dict["_brand"] = request_brand
 
 
 @pytest.mark.asyncio
-async def test__call__correctly_processes_request(monkeypatch: MonkeyPatch) -> None:
+async def test__call__correctly_processes_request(monkeypatch: pytest.MonkeyPatch) -> None:
     # Arrange
-    auth_config = BrandAuthConfig(
-        "https://authserver.com/auth/realms/projectName", "audienceOne", "myInstance", "myStage"
-    )
-
-    monkeypatch.setattr("sag_py_auth.JwtAuth.__call__", jwt_auth_call_mock)
-    monkeypatch.setattr("sag_py_auth_brand.brand_jwt_auth.BrandJwtAuth._verify_brand", _verify_brand_mock)
-    monkeypatch.setattr("sag_py_auth_brand.brand_jwt_auth.set_brand_to_context", set_brand_to_context_mock)
+    jwt: BrandJwtAuth = build_sample_jwt_auth(None)
 
-    jwt = BrandJwtAuth(auth_config, None)
+    monkeypatch.setattr("sag_py_auth.JwtAuth.__call__", mock_jwt_auth_call)
+    monkeypatch.setattr("sag_py_auth_brand.brand_jwt_auth.BrandJwtAuth._verify_brand", mock_verify_brand)
 
     request: Request = Request(scope={"type": "http"})
     request._headers = Headers({"Authorization": "Bearer validToken"})
 
     # Act
-    actual: Token = await jwt.__call__(request)
+    actual: Token = await jwt.__call__(request, "mybrand")
 
     # Assert - Verify that all steps have been executed
+    # Comment: the calls of the mocked function are verified via variables,
+    # alternatively one could use unittest.mock and assertions like assert_called on the functions.
     assert actual.get_field_value("typ") == "Bearer"
     assert actual.get_field_value("azp") == "public-project-swagger"
     assert actual.get_field_value("_verify_brand") == "True"
-    assert was_brand_set_to_context
+    assert actual.get_field_value("_brand") == "mybrand"
```

### Comparing `sag-py-auth-brand-0.2.0/tests/test_brand_jwt_auth__init.py` & `sag-py-auth-brand-0.2.1/tests/test_brand_jwt_auth__init.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 from typing import List
 
 from sag_py_auth.models import TokenRole
 
 from sag_py_auth_brand.brand_jwt_auth import BrandJwtAuth
 from sag_py_auth_brand.models import BrandAuthConfig
+from tests.helpers import build_sample_auth_config
 
 
-def test__jwt_auth__init__with_multiple_roles() -> None:
+def _verify_token_role(jwt: BrandJwtAuth, item_no: int, client: str, role: str) -> None:
+    instance: TokenRole = jwt.required_roles[item_no]
+    assert instance.client == client
+    assert instance.role == role
+
+
+def test__jwt_auth__init__with_endpoint_role() -> None:
     # Arrange
-    auth_config = BrandAuthConfig(
-        "https://authserver.com/auth/realms/projectName", "audienceOne", "myInstance", "myStage"
-    )
-    required_roles: List[str] = ["roleOne", "roleTwo"]
+    auth_config: BrandAuthConfig = build_sample_auth_config()
+    required_endpoint_roles: List[str] = ["myEndpoint"]
 
     # Act
-    jwt = BrandJwtAuth(auth_config, required_roles)
+    jwt = BrandJwtAuth(auth_config, required_endpoint_roles)
 
     # Assert
     assert len(jwt.required_realm_roles) == 1
     assert "myStage" in jwt.required_realm_roles
 
-    assert len(jwt.required_roles) == 3
+    assert len(jwt.required_roles) == 2
     _verify_token_role(jwt, 0, "role-instance", "myInstance")
-    _verify_token_role(jwt, 1, "role-endpoint", "roleOne")
-    _verify_token_role(jwt, 2, "role-endpoint", "roleTwo")
+    _verify_token_role(jwt, 1, "role-endpoint", "myEndpoint")
 
 
-def test__jwt_auth__init__without_roles() -> None:
+def test__jwt_auth__init__without_endpoint_role() -> None:
     # Arrange
-    auth_config = BrandAuthConfig(
-        "https://authserver.com/auth/realms/projectName", "audienceOne", "myInstance", "myStage"
-    )
+    auth_config: BrandAuthConfig = build_sample_auth_config()
 
     # Act
     jwt = BrandJwtAuth(auth_config, None)
 
     # Assert
     assert len(jwt.required_realm_roles) == 1
     assert "myStage" in jwt.required_realm_roles
 
     assert len(jwt.required_roles) == 1
     _verify_token_role(jwt, 0, "role-instance", "myInstance")
-
-
-def _verify_token_role(jwt: BrandJwtAuth, item_no: int, client: str, role: str) -> None:
-    instance: TokenRole = jwt.required_roles[item_no]
-    assert instance.client == client
-    assert instance.role == role
```

### Comparing `sag-py-auth-brand-0.2.0/tests/test_request_brand_logging_filter.py` & `sag-py-auth-brand-0.2.1/tests/test_request_brand_logging_filter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,78 @@
 from logging import LogRecord
 from typing import cast
 
 from sag_py_auth_brand.models import BrandLogRecord
-from sag_py_auth_brand.request_brand_context import set_brand as set_brand_to_context
-from sag_py_auth_brand.request_brand_context import set_brand_alias as set_brand_alias_to_context
+from sag_py_auth_brand.request_brand_context import set_request_brand as set_request_brand_to_context
+from sag_py_auth_brand.request_brand_context import set_request_brand_alias as set_request_brand_alias_to_context
 from sag_py_auth_brand.request_brand_logging_filter import RequestBrandLoggingFilter
 
 
 def test__get_field_value__with_brand() -> None:
     # Arrange
     logging_filter = RequestBrandLoggingFilter()
     log_entry = LogRecord("LogRecord", 0, "path.py", 100, "A test message", None, None)
 
-    set_brand_to_context("myBrand")
-    set_brand_alias_to_context(None)
+    set_request_brand_to_context("myBrand")
+    set_request_brand_alias_to_context(None)
 
     # Act
     logging_filter.filter(log_entry)
 
     # Assert
     assert log_entry.msg == "A test message"
     assert cast(BrandLogRecord, log_entry).request_brand == "myBrand"
+    assert cast(BrandLogRecord, log_entry).brand == "myBrand"
 
 
 def test__get_field_value__with_brand_alias() -> None:
     # Arrange
     logging_filter = RequestBrandLoggingFilter()
     log_entry = LogRecord("LogRecord", 0, "path.py", 100, "A test message", None, None)
 
-    set_brand_to_context(None)
-    set_brand_alias_to_context("myBrandAlias")
+    set_request_brand_to_context(None)
+    set_request_brand_alias_to_context("myBrandAlias")
 
     # Act
     logging_filter.filter(log_entry)
 
     # Assert
     assert log_entry.msg == "A test message"
-    assert cast(BrandLogRecord, log_entry).request_brand == "myBrandAlias"
+    assert not hasattr(log_entry, "request_brand")
+    assert cast(BrandLogRecord, log_entry).request_brand_alias == "myBrandAlias"
+    assert cast(BrandLogRecord, log_entry).brand == "myBrandAlias"
 
 
 def test__get_field_value__without_data() -> None:
     # Arrange
     logging_filter = RequestBrandLoggingFilter()
     log_entry = LogRecord("LogRecord", 0, "path.py", 100, "A test message", None, None)
 
-    set_brand_to_context(None)
-    set_brand_alias_to_context(None)
+    set_request_brand_to_context(None)
+    set_request_brand_alias_to_context(None)
 
     # Act
     logging_filter.filter(log_entry)
 
     # Assert
     assert log_entry.msg == "A test message"
     assert not hasattr(log_entry, "request_brand")
+    assert not hasattr(log_entry, "request_brand_alias")
+    assert not hasattr(log_entry, "brand")
+
+
+def test__get_field_value__with_both() -> None:
+    # Arrange
+    logging_filter = RequestBrandLoggingFilter()
+    log_entry = LogRecord("LogRecord", 0, "path.py", 100, "A test message", None, None)
+
+    set_request_brand_to_context("myBrand")
+    set_request_brand_alias_to_context("myBrandAlias")
+
+    # Act
+    logging_filter.filter(log_entry)
+
+    # Assert
+    assert log_entry.msg == "A test message"
+    assert cast(BrandLogRecord, log_entry).request_brand == "myBrand"
+    assert cast(BrandLogRecord, log_entry).request_brand_alias == "myBrandAlias"
+    assert cast(BrandLogRecord, log_entry).brand == "myBrandAlias"
```

