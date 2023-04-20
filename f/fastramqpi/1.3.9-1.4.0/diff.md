# Comparing `tmp/fastramqpi-1.3.9.tar.gz` & `tmp/fastramqpi-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastramqpi-1.3.9.tar", max compression
+gzip compressed data, was "fastramqpi-1.4.0.tar", max compression
```

## Comparing `fastramqpi-1.3.9.tar` & `fastramqpi-1.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0        0        0        0 2023-03-08 12:47:24.103878 fastramqpi-1.3.9/LICENSES/
--rw-r--r--   0        0        0    15177 2023-03-08 12:47:24.104878 fastramqpi-1.3.9/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     2932 2023-03-08 12:47:24.104878 fastramqpi-1.3.9/README.md
--rw-r--r--   0        0        0       85 2023-03-08 12:47:24.104878 fastramqpi-1.3.9/fastramqpi/__init__.py
--rw-r--r--   0        0        0     2208 2023-03-08 12:47:24.104878 fastramqpi-1.3.9/fastramqpi/config.py
--rw-r--r--   0        0        0     1144 2023-03-08 12:47:24.104878 fastramqpi-1.3.9/fastramqpi/context.py
--rw-r--r--   0        0        0     7194 2023-03-08 12:47:24.104878 fastramqpi-1.3.9/fastramqpi/fastapi.py
--rw-r--r--   0        0        0     1573 2023-03-08 12:47:24.105878 fastramqpi-1.3.9/fastramqpi/healthcheck.py
--rw-r--r--   0        0        0     3899 2023-03-08 12:47:24.105878 fastramqpi-1.3.9/fastramqpi/main.py
--rw-r--r--   0        0        0        0 2023-03-08 12:47:24.151884 fastramqpi-1.3.9/fastramqpi/py.typed
--rw-r--r--   0        0        0     1377 2023-03-08 12:47:40.872265 fastramqpi-1.3.9/pyproject.toml
--rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 fastramqpi-1.3.9/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-04-20 11:30:25.500164 fastramqpi-1.4.0/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-04-20 11:30:25.500164 fastramqpi-1.4.0/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     2932 2023-04-20 11:30:25.500164 fastramqpi-1.4.0/README.md
+-rw-r--r--   0        0        0       85 2023-04-20 11:30:25.500164 fastramqpi-1.4.0/fastramqpi/__init__.py
+-rw-r--r--   0        0        0     2206 2023-04-20 11:30:25.501164 fastramqpi-1.4.0/fastramqpi/config.py
+-rw-r--r--   0        0        0     1144 2023-04-20 11:30:25.501164 fastramqpi-1.4.0/fastramqpi/context.py
+-rw-r--r--   0        0        0     7100 2023-04-20 11:30:25.501164 fastramqpi-1.4.0/fastramqpi/fastapi.py
+-rw-r--r--   0        0        0     1577 2023-04-20 11:30:25.501164 fastramqpi-1.4.0/fastramqpi/healthcheck.py
+-rw-r--r--   0        0        0     3930 2023-04-20 11:30:25.501164 fastramqpi-1.4.0/fastramqpi/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 11:30:25.552171 fastramqpi-1.4.0/fastramqpi/py.typed
+-rw-r--r--   0        0        0     1390 2023-04-20 11:30:38.503015 fastramqpi-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 fastramqpi-1.4.0/PKG-INFO
```

### Comparing `fastramqpi-1.3.9/LICENSES/MPL-2.0.txt` & `fastramqpi-1.4.0/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.3.9/README.md` & `fastramqpi-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.3.9/fastramqpi/config.py` & `fastramqpi-1.4.0/fastramqpi/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # SPDX-FileCopyrightText: 2021 Magenta ApS <https://magenta.dk>
 # SPDX-License-Identifier: MPL-2.0
 """Settings handling."""
 from pydantic import AnyHttpUrl
 from pydantic import BaseSettings
 from pydantic import Field
 from pydantic import parse_obj_as
+from pydantic import PositiveInt
 from pydantic import SecretStr
-from ramqp.config import ConnectionSettings
+from ramqp.config import AMQPConnectionSettings
 
 
 # pylint: disable=too-few-public-methods
 class FastAPIIntegrationSystemSettings(BaseSettings):
     """Settings for the FastAPIIntegrationSystem framework."""
 
     class Config:
@@ -37,14 +38,16 @@
 
         frozen = True
 
     mo_url: AnyHttpUrl = Field(
         parse_obj_as(AnyHttpUrl, "http://mo-service:5000"),
         description="Base URL for OS2mo.",
     )
+    mo_graphql_version: PositiveInt = 3
+
     client_id: str = Field(..., description="Client ID for OIDC client.")
     client_secret: SecretStr = Field(..., description="Client Secret for OIDC client.")
     auth_server: AnyHttpUrl = Field(
         parse_obj_as(AnyHttpUrl, "http://keycloak-service:8080/auth"),
         description="Base URL for OIDC server (Keycloak).",
     )
     auth_realm: str = Field("mo", description="Realm to authenticate against")
@@ -57,10 +60,8 @@
 
     class Config:
         """Settings are frozen."""
 
         frozen = True
         env_nested_delimiter = "__"
 
-    amqp: ConnectionSettings = Field(
-        ConnectionSettings(), description="AMQP connection settings"
-    )
+    amqp: AMQPConnectionSettings
```

### Comparing `fastramqpi-1.3.9/fastramqpi/context.py` & `fastramqpi-1.4.0/fastramqpi/context.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.3.9/fastramqpi/fastapi.py` & `fastramqpi-1.4.0/fastramqpi/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 #
 # SPDX-License-Identifier: MPL-2.0
 """FastAPI Framework."""
 import logging
 from contextlib import asynccontextmanager
 from contextlib import AsyncExitStack
-from functools import partial
 from typing import Any
 from typing import AsyncContextManager
-from typing import AsyncGenerator
+from typing import AsyncIterator
 
 import structlog
 from fastapi import APIRouter
 from fastapi import FastAPI
 from fastapi import Request
 from fastapi import Response
 from prometheus_client import Info
@@ -20,15 +19,14 @@
 from starlette.status import HTTP_204_NO_CONTENT
 from starlette.status import HTTP_503_SERVICE_UNAVAILABLE
 
 from .config import FastAPIIntegrationSystemSettings
 from .context import Context
 from .context import HealthcheckFunction
 
-
 logger = structlog.get_logger()
 fastapi_router = APIRouter()
 build_information = Info("build_information", "Build information")
 
 
 def update_build_information(version: str, build_hash: str) -> None:
     """Update build information.
@@ -104,24 +102,24 @@
     if not all_ready:
         response.status_code = HTTP_503_SERVICE_UNAVAILABLE
 
     return response
 
 
 @asynccontextmanager
-async def _lifespan(_1: FastAPI, context: Context) -> AsyncGenerator[None, None]:
+async def _lifespan(app: FastAPI) -> AsyncIterator[None]:
     """ASGI lifespan context handler.
 
     Runs all the configured lifespan managers according to their priority.
 
     Returns:
         None
     """
     async with AsyncExitStack() as stack:
-        lifespan_managers = context["lifespan_managers"]
+        lifespan_managers = app.state.context["lifespan_managers"]
         for _, priority_set in sorted(lifespan_managers.items()):
             for lifespan_manager in priority_set:
                 await stack.enter_async_context(lifespan_manager)
         # Yield to keep lifespan managers open until the ASGI application is shutdown.
         yield
 
 
@@ -161,18 +159,18 @@
                 "url": "https://www.magenta.dk/",
                 "email": "info@magenta.dk>",
             },
             license_info={
                 "name": "MPL-2.0",
                 "url": "https://www.mozilla.org/en-US/MPL/2.0/",
             },
+            lifespan=_lifespan,
         )
         app.include_router(fastapi_router)
         app.state.context = self._context
-        app.router.lifespan_context = partial(_lifespan, context=self._context)
         # Expose Metrics
         if self.settings.enable_metrics:
             # Update metrics info
             update_build_information(
                 version=self.settings.commit_tag, build_hash=self.settings.commit_sha
             )
```

### Comparing `fastramqpi-1.3.9/fastramqpi/healthcheck.py` & `fastramqpi-1.4.0/fastramqpi/healthcheck.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,14 +49,14 @@
 
     Returns:
         Whether the client is healthy or not.
     """
     model_client = context["model_client"]
 
     try:
-        response = await model_client.async_httpx_client("/service/o/")
+        response = await model_client.async_httpx_client.get("/service/o/")
         result = response.json()
         if one(result)["uuid"]:
             return True
     except Exception:  # pylint: disable=broad-except
         logger.exception("Exception occured during GraphQL healthcheck")
     return False
```

### Comparing `fastramqpi-1.3.9/fastramqpi/main.py` & `fastramqpi-1.4.0/fastramqpi/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         client_id=settings.client_id,
         client_secret=settings.client_secret.get_secret_value(),
         auth_realm=settings.auth_realm,
         auth_server=settings.auth_server,
     )
 
     gql_client = GraphQLClient(
-        url=settings.mo_url + "/graphql",
+        url=f"{settings.mo_url}/graphql/v{settings.mo_graphql_version}",
         execute_timeout=settings.graphql_timeout,
         httpx_client_kwargs={"timeout": settings.graphql_timeout},
         **client_kwargs,
     )
     model_client = ModelClient(
         base_url=settings.mo_url,
         **client_kwargs,
```

### Comparing `fastramqpi-1.3.9/pyproject.toml` & `fastramqpi-1.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
 [tool.poetry]
 name = "FastRAMQPI"
-version = "1.3.9"
+version = "1.4.0"
 description = "Rammearkitektur AMQP framework (FastAPI + RAMQP)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/FastRAMQPI"
 keywords = ["os2mo", "amqp"]
 packages = [ { include = "fastramqpi" } ]
 include = ["fastramqpi/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 structlog = "^22.3.0"
-ramqp = "^6.6.2"
-pydantic = "^1.10.2"
-raclients = "^3.0.3"
+ramqp = "^8.2.0"
+pydantic = "^1.10.5"
+raclients = "^3.0.5"
 gql = "^3.4.0"
-more-itertools = "^9.0.0"
-ra-utils = "^1.7.1"
-prometheus-fastapi-instrumentator = "^5.9.1"
-fastapi = "^0.88.0"
+more-itertools = "^9.1.0"
+ra-utils = "^1.12.2"
+prometheus-fastapi-instrumentator = ">=5.9.1,<7.0.0"
+fastapi = ">=0.93, <1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pre-commit = "^2.19.0"
-requests = "^2.28.0"
+requests = "^2.5.1"
 asgi-lifespan = "^1.0.1"
 pytest-asyncio = "^0.19.0"
 pytest-split = "^0.8.0"
 pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `fastramqpi-1.3.9/PKG-INFO` & `fastramqpi-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fastramqpi
-Version: 1.3.9
+Version: 1.4.0
 Summary: Rammearkitektur AMQP framework (FastAPI + RAMQP)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (>=0.88.0,<0.89.0)
+Requires-Dist: fastapi (>=0.93,<1.0)
 Requires-Dist: gql (>=3.4.0,<4.0.0)
-Requires-Dist: more-itertools (>=9.0.0,<10.0.0)
-Requires-Dist: prometheus-fastapi-instrumentator (>=5.9.1,<6.0.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
-Requires-Dist: ra-utils (>=1.7.1,<2.0.0)
-Requires-Dist: raclients (>=3.0.3,<4.0.0)
-Requires-Dist: ramqp (>=6.6.2,<7.0.0)
+Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
+Requires-Dist: prometheus-fastapi-instrumentator (>=5.9.1,<7.0.0)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: ra-utils (>=1.12.2,<2.0.0)
+Requires-Dist: raclients (>=3.0.5,<4.0.0)
+Requires-Dist: ramqp (>=8.2.0,<9.0.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
 Project-URL: Repository, https://git.magenta.dk/rammearkitektur/FastRAMQPI
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: 2021 Magenta ApS <https://magenta.dk>
 SPDX-License-Identifier: MPL-2.0
```

