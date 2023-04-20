# Comparing `tmp/sag-py-fastapi-health-0.1.0.tar.gz` & `tmp/sag-py-fastapi-health-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-fastapi-health-0.1.0.tar", last modified: Tue Apr 11 07:51:31 2023, max compression
+gzip compressed data, was "sag-py-fastapi-health-0.1.1.tar", last modified: Thu Apr 20 08:46:10 2023, max compression
```

## Comparing `sag-py-fastapi-health-0.1.0.tar` & `sag-py-fastapi-health-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:51:31.390364 sag-py-fastapi-health-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-11 07:51:31.390364 sag-py-fastapi-health-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:51:31.386364 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:51:31.386364 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/checks/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/checks/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:51:31.386364 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-11 07:51:31.000000 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-11 07:51:31.000000 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:51:31.000000 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 07:51:31.000000 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 07:51:31.000000 sag-py-fastapi-health-0.1.0/sag_py_fastapi_health.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 07:51:31.390364 sag-py-fastapi-health-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:51:31.390364 sag-py-fastapi-health-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/tests/test_checks_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/tests/test_checks_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/tests/test_json_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/tests/test_prtg_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-11 07:51:15.000000 sag-py-fastapi-health-0.1.0/tests/test_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:46:10.128703 sag-py-fastapi-health-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-20 08:46:10.128703 sag-py-fastapi-health-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:46:10.128703 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:46:10.128703 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/checks/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/checks/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:46:10.128703 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-20 08:46:10.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-20 08:46:10.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 08:46:10.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 08:46:10.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 08:46:10.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 08:46:10.128703 sag-py-fastapi-health-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:46:10.128703 sag-py-fastapi-health-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/tests/test_checks_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/tests/test_checks_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/tests/test_json_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/tests/test_prtg_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/tests/test_router.py
```

### Comparing `sag-py-fastapi-health-0.1.0/LICENSE.txt` & `sag-py-fastapi-health-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.0/PKG-INFO` & `sag-py-fastapi-health-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: sag-py-fastapi-health
-Version: 0.1.0
-Summary: A library for fastapi health checks
-Home-page: https://github.com/SamhammerAG/sag_py_fastapi_health
-Author: Samhammer AG
-Author-email: support@samhammer.de
-License: MIT
-Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_fastapi_health
-Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_fastapi_health/issues
-Project-URL: Source, https://github.com/SamhammerAG/sag_py_fastapi_health
-Keywords: fastapi,health
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
 # sag_py_fastapi_health
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities][snyk-image]][snyk-url]
 
 Add health check endpoints to fastapi (similar to the ones dotnet core has)
 
@@ -88,14 +65,40 @@
             status="Healthy" if is_healthy else "Unhealthy",
             description=description,
         )
 ```
 The description contains something like "Directory ... was accessable" or "Service is running" if everything is ok.
 If there was an error, you can add the error message/exception message there.
 
+## How to configure in prtg
+
+use the sensor "HTTP data advanced" (https://www.paessler.com/manuals/prtg/http_data_advanced_sensor) and configure to your prtg health endpoint (like in the example above ([URL_TO_YOUR_SERVICE]/health/health-prtg)
+
+
+## How to start developing
+
+### With vscode
+
+Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
+
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
 ## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
 
 [codeclimate-image]:https://api.codeclimate.com/v1/badges/518206f10db22dbeb984/maintainability
 [codeclimate-url]:https://codeclimate.com/github/SamhammerAG/sag_py_fastapi_health/maintainability
```

### Comparing `sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/checks/http.py` & `sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/checks/http.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,36 +7,30 @@
 try:
     from aiohttp import BasicAuth, ClientResponseError, ClientSession, ClientTimeout, TCPConnector
 except ImportError as exc:
     raise ImportError("Using this module requires the aiohttp library.") from exc
 
 
 class HttpCheck(Check):
-    _url: str
-    _username: Optional[str]
-    _password: Optional[str]
-    _verify_ssl: bool
-    _timeout: float
-    _name: str
 
     def __init__(
         self,
         url: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         verify_ssl: bool = True,
         timeout: float = 60.0,
         name: str = "HTTP",
     ) -> None:
-        self._url = url
-        self._username = username
-        self._password = password
-        self._verify_ssl = verify_ssl
-        self._timeout = timeout
-        self._name = name
+        self._url: str = url
+        self._username: Optional[str] = username
+        self._password: Optional[str] = password
+        self._verify_ssl: bool = verify_ssl
+        self._timeout: float = timeout
+        self._name: str = name
 
     async def __call__(self) -> CheckResult:
         try:
             async with ClientSession(
                 connector=TCPConnector(verify_ssl=self._verify_ssl, enable_cleanup_closed=True),
                 auth=BasicAuth(self._username, self._password or "") if self._username else None,
                 timeout=ClientTimeout(self._timeout),
```

### Comparing `sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/checks/storage.py` & `sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/checks/storage.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/formatter.py` & `sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/formatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import Type, List
+from typing import List, Type
+
 from fastapi import Response
 from fastapi import status as http_status
 from fastapi.encoders import jsonable_encoder
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel, Field
 
-from sag_py_fastapi_health.models import HealthResponseFormatter, HealthcheckReport, Response
+from sag_py_fastapi_health.models import HealthcheckReport, HealthResponseFormatter
 
 
 class DefaultResponseFormatter(HealthResponseFormatter):
     def get_response_type(self) -> Type[BaseModel]:
         return HealthcheckReport
 
     def format(self, report: HealthcheckReport) -> Response:
```

### Comparing `sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/models.py` & `sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/models.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from abc import ABC, abstractmethod
 from typing import Iterable, List, Literal, NamedTuple, Optional, Type
-from fastapi import Response
 
+from fastapi import Response
 from pydantic import BaseModel
 
 
 class CheckResult(BaseModel):
     name: str
     status: Literal["Healthy", "Unhealthy", "Degraded"]
     duration: float = 0
```

### Comparing `sag-py-fastapi-health-0.1.0/sag_py_fastapi_health/router.py` & `sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/router.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import datetime
-from typing import Any, Coroutine, List, Literal
+from typing import Any, Coroutine, List, Literal, cast
 
 from fastapi import APIRouter, Response
 
 from sag_py_fastapi_health.models import Check, CheckResult, HealthcheckReport, Probe
 
 
 class HealthcheckRouter(APIRouter):
@@ -23,15 +23,15 @@
             response_model=probe.response_formatter.get_response_type(),
             summary=probe.endpoint_summary,
             include_in_schema=probe.include_in_schema,
         )
 
     async def _handle_request(self, probe: Probe) -> Response:
         tasks: List[Coroutine[Any, Any, CheckResult]] = [self._run_check(check) for check in probe.checks]
-        results: List[CheckResult] = await asyncio.gather(*tasks)
+        results: List[CheckResult] = cast(List[CheckResult], await asyncio.gather(*tasks))
 
         total_duration: float = sum(result.duration for result in results)
         status: Literal["Unhealthy", "Degraded", "Healthy"] = self._get_total_status(results)
         report = HealthcheckReport(status=status, entries=results, total_duration=total_duration)
 
         return probe.response_formatter.format(report)
```

### Comparing `sag-py-fastapi-health-0.1.0/sag_py_fastapi_health.egg-info/SOURCES.txt` & `sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.0/setup.py` & `sag-py-fastapi-health-0.1.1/setup.py`

 * *Files 6% similar despite different names*

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
     name="sag-py-fastapi-health",
-    version="0.1.0",
+    version="0.1.1",
     description="A library for fastapi health checks",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_fastapi_health",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
@@ -25,14 +28,14 @@
         "Topic :: Software Development",
     ],
     keywords="fastapi, health",
     packages=setuptools.find_packages(exclude=["tests"]),
     package_data={"sag_py_fastapi_health": ["py.typed"]},
     python_requires=">=3.8",
     install_requires=REQS,
-    extras_require={"dev": ["pytest"]},
+    extras_require={"dev": REQS_DEV},
     project_urls={
         "Documentation": "https://github.com/SamhammerAG/sag_py_fastapi_health",
         "Bug Reports": "https://github.com/SamhammerAG/sag_py_fastapi_health/issues",
         "Source": "https://github.com/SamhammerAG/sag_py_fastapi_health",
     },
 )
```

### Comparing `sag-py-fastapi-health-0.1.0/tests/test_checks_http.py` & `sag-py-fastapi-health-0.1.1/tests/test_checks_http.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         continue100=None,
         timer=TimerNoop(),
         traces=[],
         loop=mock.Mock(),
         session=mock.Mock(),
     )
     response.status = 200
-    monkeypatch.setattr("aiohttp.ClientSession.get", lambda self, url: response)  # type: ignore
+    monkeypatch.setattr("aiohttp.ClientSession.get", lambda self, url: response)
 
     # Act
     check: CheckResult = await HttpCheck("http://localhost/test", name="myHttpCheck")()
 
     # Assert
     assert check.name == "myHttpCheck"
     assert check.status == "Healthy"
@@ -45,15 +45,15 @@
         continue100=None,
         timer=TimerNoop(),
         traces=[],
         loop=mock.Mock(),
         session=mock.Mock(),
     )
     response.status = 204
-    monkeypatch.setattr("aiohttp.ClientSession.get", lambda self, url: response)  # type: ignore
+    monkeypatch.setattr("aiohttp.ClientSession.get", lambda self, url: response)
 
     # Act
     check: CheckResult = await HttpCheck("http://localhost/test", name="myHttpCheck")()
 
     # Assert
     assert check.name == "myHttpCheck"
     assert check.status == "Healthy"
@@ -71,15 +71,15 @@
         continue100=None,
         timer=TimerNoop(),
         traces=[],
         loop=mock.Mock(),
         session=mock.Mock(),
     )
     response.status = 500
-    monkeypatch.setattr("aiohttp.ClientSession.get", lambda self, url: response)  # type: ignore
+    monkeypatch.setattr("aiohttp.ClientSession.get", lambda self, url: response)
 
     # Act
     check: CheckResult = await HttpCheck("http://localhost/test", name="myHttpCheck")()
 
     # Assert
     assert check.name == "myHttpCheck"
     assert check.status == "Unhealthy"
```

### Comparing `sag-py-fastapi-health-0.1.0/tests/test_checks_storage.py` & `sag-py-fastapi-health-0.1.1/tests/test_checks_storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,29 +25,29 @@
     assert check.status == "Unhealthy"
     assert check.description == "Empty path"
 
 
 @pytest.mark.asyncio
 async def test__StorageExistsCheck__path_exists(monkeypatch: pytest.MonkeyPatch) -> None:
     # Arrange
-    monkeypatch.setattr("os.path.isdir", lambda path: True)  # type: ignore
+    monkeypatch.setattr("os.path.isdir", lambda path: True)
 
     # Act
     check: CheckResult = await StorageExistsCheck("/existing/path", "myStorageCheck", True)()
 
     # Assert
     assert check.name == "myStorageCheck"
     assert check.status == "Healthy"
     assert check.description == "Path exists"
 
 
 @pytest.mark.asyncio
 async def test__StorageExistsCheck__path_not_exists(monkeypatch: pytest.MonkeyPatch) -> None:
     # Arrange
-    monkeypatch.setattr("os.path.isdir", lambda path: False)  # type: ignore
+    monkeypatch.setattr("os.path.isdir", lambda path: False)
 
     # Act
     check: CheckResult = await StorageExistsCheck("/existing/path", "myStorageCheck", True)()
 
     # Assert
     assert check.name == "myStorageCheck"
     assert check.status == "Unhealthy"
@@ -75,29 +75,29 @@
     assert check.status == "Unhealthy"
     assert check.description == "Empty path"
 
 
 @pytest.mark.asyncio
 async def test__StorageReadableCheck__path_exists(monkeypatch: pytest.MonkeyPatch) -> None:
     # Arrange
-    monkeypatch.setattr("os.access", lambda path, mode: True)  # type: ignore
+    monkeypatch.setattr("os.access", lambda path, mode: True)
 
     # Act
     check: CheckResult = await StorageReadableCheck("/existing/path", "myStorageCheck", True)()
 
     # Assert
     assert check.name == "myStorageCheck"
     assert check.status == "Healthy"
     assert check.description == "Path readable"
 
 
 @pytest.mark.asyncio
 async def test__StorageReadableCheck__path_not_exists(monkeypatch: pytest.MonkeyPatch) -> None:
     # Arrange
-    monkeypatch.setattr("os.access", lambda path, mode: False)  # type: ignore
+    monkeypatch.setattr("os.access", lambda path, mode: False)
 
     # Act
     check: CheckResult = await StorageReadableCheck("/existing/path", "myStorageCheck", True)()
 
     # Assert
     assert check.name == "myStorageCheck"
     assert check.status == "Unhealthy"
@@ -125,29 +125,29 @@
     assert check.status == "Unhealthy"
     assert check.description == "Empty path"
 
 
 @pytest.mark.asyncio
 async def test__StorageWritableCheck__path_exists(monkeypatch: pytest.MonkeyPatch) -> None:
     # Arrange
-    monkeypatch.setattr("os.access", lambda path, mode: True)  # type: ignore
+    monkeypatch.setattr("os.access", lambda path, mode: True)
 
     # Act
     check: CheckResult = await StorageWritableCheck("/existing/path", "myStorageCheck", True)()
 
     # Assert
     assert check.name == "myStorageCheck"
     assert check.status == "Healthy"
     assert check.description == "Path writable"
 
 
 @pytest.mark.asyncio
 async def test__StorageWritableCheck__path_not_exists(monkeypatch: pytest.MonkeyPatch) -> None:
     # Arrange
-    monkeypatch.setattr("os.access", lambda path, mode: False)  # type: ignore
+    monkeypatch.setattr("os.access", lambda path, mode: False)
 
     # Act
     check: CheckResult = await StorageWritableCheck("/existing/path", "myStorageCheck", True)()
 
     # Assert
     assert check.name == "myStorageCheck"
     assert check.status == "Unhealthy"
```

### Comparing `sag-py-fastapi-health-0.1.0/tests/test_json_formatter.py` & `sag-py-fastapi-health-0.1.1/tests/test_json_formatter.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,37 +17,39 @@
 
 def test__json_response_formatter__healthy() -> None:
     # Arrange
     check_results: List[CheckResult] = [
         CheckResult(name="checkOne", status="Healthy", duration=50, description="Check ok"),
         CheckResult(name="checkTwo", status="Healthy", duration=50, description="Check ok"),
     ]
-    health_chekck_report = HealthcheckReport(status="Healthy", total_duration=100, entries=check_results)
+    health_check_report = HealthcheckReport(status="Healthy", total_duration=100, entries=check_results)
 
     # Act
-    actual: Response = DefaultResponseFormatter().format(health_chekck_report)
+    actual: Response = DefaultResponseFormatter().format(health_check_report)
 
     # Assert
     assert actual.status_code == 200
     assert (
-        actual.body
-        == b'{"status":"Healthy","total_duration":100.0,"entries":[{"name":"checkOne","status":"Healthy","duration":50.0,"description":"Check ok"},{"name":"checkTwo","status":"Healthy","duration":50.0,"description":"Check ok"}]}'
+        actual.body == b'{"status":"Healthy","total_duration":100.0,'
+        b'"entries":[{"name":"checkOne","status":"Healthy","duration":50.0,"description":"Check ok"},'
+        b'{"name":"checkTwo","status":"Healthy","duration":50.0,"description":"Check ok"}]}'
     )
 
 
 def test__json_response_formatter__unhealthy() -> None:
     # Arrange
     check_results: List[CheckResult] = [
         CheckResult(name="checkOne", status="Unhealthy", duration=50, description="Something failed"),
         CheckResult(name="checkTwo", status="Healthy", duration=50, description="Check ok"),
     ]
-    health_chekck_report = HealthcheckReport(status="Unhealthy", total_duration=100, entries=check_results)
+    health_check_report = HealthcheckReport(status="Unhealthy", total_duration=100, entries=check_results)
 
     # Act
-    actual: Response = DefaultResponseFormatter().format(health_chekck_report)
+    actual: Response = DefaultResponseFormatter().format(health_check_report)
 
     # Assert
     assert actual.status_code == 503
     assert (
-        actual.body
-        == b'{"status":"Unhealthy","total_duration":100.0,"entries":[{"name":"checkOne","status":"Unhealthy","duration":50.0,"description":"Something failed"},{"name":"checkTwo","status":"Healthy","duration":50.0,"description":"Check ok"}]}'
+        actual.body == b'{"status":"Unhealthy","total_duration":100.0,'
+        b'"entries":[{"name":"checkOne","status":"Unhealthy","duration":50.0,"description":"Something failed"},'
+        b'{"name":"checkTwo","status":"Healthy","duration":50.0,"description":"Check ok"}]}'
     )
```

### Comparing `sag-py-fastapi-health-0.1.0/tests/test_prtg_formatter.py` & `sag-py-fastapi-health-0.1.1/tests/test_prtg_formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,37 +17,40 @@
 
 def test__prtg_response_formatter__healthy() -> None:
     # Arrange
     check_results: List[CheckResult] = [
         CheckResult(name="checkOne", status="Healthy", duration=50, description="Check ok"),
         CheckResult(name="checkTwo", status="Healthy", duration=50, description="Check ok"),
     ]
-    health_chekck_report = HealthcheckReport(status="Healthy", total_duration=100, entries=check_results)
+    health_check_report = HealthcheckReport(status="Healthy", total_duration=100, entries=check_results)
 
     # Act
-    actual: Response = PrtgResponseFormatter().format(health_chekck_report)
+    actual: Response = PrtgResponseFormatter().format(health_check_report)
 
     # Assert
     assert actual.status_code == 200
     assert (
-        actual.body
-        == b'{"prtg":{"error":0,"text":"","result":[{"value":100.0,"channel":"TotalDuration","float":true,"unit":"TimeResponse"},{"value":50.0,"channel":"checkOne.Duration","float":true,"unit":"TimeResponse"},{"value":50.0,"channel":"checkTwo.Duration","float":true,"unit":"TimeResponse"}]}}'
+        actual.body == b'{"prtg":{"error":0,"text":"","result":[{"value":100.0,"channel":"TotalDuration","float":true,'
+        b'"unit":"TimeResponse"},{"value":50.0,"channel":"checkOne.Duration","float":true,"unit":"TimeResponse"},'
+        b'{"value":50.0,"channel":"checkTwo.Duration","float":true,"unit":"TimeResponse"}]}}'
     )
 
 
 def test__prtg_response_formatter__unhealthy() -> None:
     # Arrange
     check_results: List[CheckResult] = [
         CheckResult(name="checkOne", status="Unhealthy", duration=50, description="Something failed"),
         CheckResult(name="checkTwo", status="Healthy", duration=50, description="Check ok"),
     ]
-    health_chekck_report = HealthcheckReport(status="Unhealthy", total_duration=100, entries=check_results)
+    health_check_report = HealthcheckReport(status="Unhealthy", total_duration=100, entries=check_results)
 
     # Act
-    actual: Response = PrtgResponseFormatter().format(health_chekck_report)
+    actual: Response = PrtgResponseFormatter().format(health_check_report)
 
     # Assert
     assert actual.status_code == 200
     assert (
         actual.body
-        == b'{"prtg":{"error":1,"text":"checkOne: Something failed","result":[{"value":100.0,"channel":"TotalDuration","float":true,"unit":"TimeResponse"},{"value":50.0,"channel":"checkOne.Duration","float":true,"unit":"TimeResponse"},{"value":50.0,"channel":"checkTwo.Duration","float":true,"unit":"TimeResponse"}]}}'
+        == b'{"prtg":{"error":1,"text":"checkOne: Something failed","result":[{"value":100.0,"channel":"TotalDuration"'
+        b',"float":true,"unit":"TimeResponse"},{"value":50.0,"channel":"checkOne.Duration","float":true,'
+        b'"unit":"TimeResponse"},{"value":50.0,"channel":"checkTwo.Duration","float":true,"unit":"TimeResponse"}]}}'
     )
```

### Comparing `sag-py-fastapi-health-0.1.0/tests/test_router.py` & `sag-py-fastapi-health-0.1.1/tests/test_router.py`

 * *Files identical despite different names*

