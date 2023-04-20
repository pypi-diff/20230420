# Comparing `tmp/trailwatch-0.2.0.tar.gz` & `tmp/trailwatch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trailwatch-0.2.0.tar", max compression
+gzip compressed data, was "trailwatch-0.3.0.tar", max compression
```

## Comparing `trailwatch-0.2.0.tar` & `trailwatch-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-04-18 23:24:19.015464 trailwatch-0.2.0/LICENSE
--rw-r--r--   0        0        0     2988 2023-04-18 23:24:19.015464 trailwatch-0.2.0/README.md
--rw-r--r--   0        0        0     2026 2023-04-18 23:24:19.015464 trailwatch-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2811 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/__init__.py
--rw-r--r--   0        0        0     6071 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/config.py
--rw-r--r--   0        0        0        0 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/connectors/__init__.py
--rw-r--r--   0        0        0       85 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/connectors/aws/__init__.py
--rw-r--r--   0        0        0     4103 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/connectors/aws/api.py
--rw-r--r--   0        0        0     3453 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/connectors/aws/connector.py
--rw-r--r--   0        0        0      809 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/connectors/aws/handler.py
--rw-r--r--   0        0        0      930 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/connectors/base.py
--rw-r--r--   0        0        0     3030 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/context.py
--rw-r--r--   0        0        0      414 2023-04-18 23:24:19.015464 trailwatch-0.2.0/src/trailwatch/exceptions.py
--rw-r--r--   0        0        0     3714 1970-01-01 00:00:00.000000 trailwatch-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-20 01:52:59.126414 trailwatch-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7527 2023-04-20 01:52:59.130415 trailwatch-0.3.0/README.md
+-rw-r--r--   0        0        0     2026 2023-04-20 01:52:59.130415 trailwatch-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3195 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/__init__.py
+-rw-r--r--   0        0        0     6071 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/config.py
+-rw-r--r--   0        0        0        0 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/aws/__init__.py
+-rw-r--r--   0        0        0     8308 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/aws/api.py
+-rw-r--r--   0        0        0     3898 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/aws/connector.py
+-rw-r--r--   0        0        0      809 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/aws/handler.py
+-rw-r--r--   0        0        0     1081 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/base.py
+-rw-r--r--   0        0        0      306 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/salesforce/__init__.py
+-rw-r--r--   0        0        0     6116 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/connectors/salesforce/connector.py
+-rw-r--r--   0        0        0     7103 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/context.py
+-rw-r--r--   0        0        0      414 2023-04-20 01:52:59.130415 trailwatch-0.3.0/src/trailwatch/exceptions.py
+-rw-r--r--   0        0        0     8253 1970-01-01 00:00:00.000000 trailwatch-0.3.0/PKG-INFO
```

### Comparing `trailwatch-0.2.0/LICENSE` & `trailwatch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trailwatch-0.2.0/pyproject.toml` & `trailwatch-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trailwatch"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python SDK for TrailWatch by Kicksaw"
 license = "Apache-2.0"
 authors = ["George Bocharov <george@kicksaw.com>"]
 readme = "README.md"
 homepage = "https://www.kicksaw.com/"
 repository = "https://github.com/Kicksaw-Consulting/trailwatch-python-sdk"
 packages = [
```

### Comparing `trailwatch-0.2.0/src/trailwatch/__init__.py` & `trailwatch-0.3.0/src/trailwatch/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 __all__ = [
     "configure",
     "TrailwatchContext",
     "watch",
 ]
 
 import functools
-import signal
-
-from .config import DEFAULT, Default, configure
-from .context import TrailwatchContext
-from .exceptions import ExecutionTimeoutError
+import inspect
 
+from typing import Callable, TypeVar
 
-def throw_timeout_on_alarm(signum, frame):
-    raise ExecutionTimeoutError
+from typing_extensions import Concatenate, ParamSpec
 
+from .config import DEFAULT, Default, configure
+from .context import TrailwatchContext
 
-signal.signal(signal.SIGALRM, throw_timeout_on_alarm)
+_P = ParamSpec("_P")
+_T = TypeVar("_T")
 
 
-# TODO - add support for uploading files (use locals() to get execution context)
+# TODO - add support for uploading files (inspect for argument)
 def watch(
     job: str | None = None,
     job_description: str | None = None,
     loggers: list[str] | Default | None = DEFAULT,
     execution_ttl: int | Default | None = DEFAULT,
     log_ttl: int | Default | None = DEFAULT,
     error_ttl: int | Default | None = DEFAULT,
@@ -57,32 +56,41 @@
     timeout : int, optional
         Timeout in seconds. If the callable takes longer than this to execute,
         an execution timeout error is raised and execution is marked as timed out.
         By default, no timeout is set.
 
     """
 
-    def wrapper(func):
+    def wrapper(
+        func: Callable[Concatenate[TrailwatchContext, _P], _T]
+    ) -> Callable[_P, _T]:
+        if inspect.iscoroutinefunction(func):
+            raise NotImplementedError("Coroutine functions are not supported")
+
         decorator_kwargs = {
             "job": job or func.__name__,
             "job_description": job_description or func.__doc__,
             "loggers": loggers,
             "execution_ttl": execution_ttl,
             "log_ttl": log_ttl,
             "error_ttl": error_ttl,
+            "timeout": timeout,
         }
         if decorator_kwargs["job_description"] is None:
             raise ValueError(
                 "Job description must either be provided explicitly or "
                 "via the docstring of the decorated function"
             )
 
         @functools.wraps(func)
         def inner(*args, **kwargs):
-            if timeout is not None:
-                signal.alarm(timeout)
-            with TrailwatchContext(**decorator_kwargs):
+            with TrailwatchContext(**decorator_kwargs) as tw_context:
+                if "trailwatch_execution_context" in [
+                    *inspect.getfullargspec(func).args,
+                    *inspect.getfullargspec(func).kwonlyargs,
+                ]:
+                    kwargs["trailwatch_execution_context"] = tw_context
                 return func(*args, **kwargs)
 
         return inner
 
     return wrapper
```

### Comparing `trailwatch-0.2.0/src/trailwatch/config.py` & `trailwatch-0.3.0/src/trailwatch/config.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.2.0/src/trailwatch/connectors/aws/connector.py` & `trailwatch-0.3.0/src/trailwatch/connectors/aws/connector.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import logging
 import traceback
 
 from types import TracebackType
-from typing import TYPE_CHECKING, Type
+from typing import TYPE_CHECKING, BinaryIO, Type
 
 from requests import Session
 
 from trailwatch.connectors.base import Connector, ConnectorFactory
 
 from .api import TrailwatchApi
 from .handler import AwsHandler
@@ -21,14 +21,20 @@
 class AwsConnector(Connector):
     def __init__(self, config: "TrailwatchConfig", url: str, api_key: str) -> None:
         self.config = config
         self.api = TrailwatchApi(Session(), url, api_key)
         self.execution_id: str | None = None
         self.handler: AwsHandler | None = None
 
+    @property
+    def execution_url(self) -> str | None:
+        if self.execution_id is None:
+            return None
+        return "/".join([self.api.url, self.execution_id])
+
     def start_execution(self) -> None:
         # Create entries in TrailWatch database
         self.api.upsert_project(
             self.config.project,
             self.config.project_description,
         )
         self.api.upsert_environment(self.config.environment)
@@ -82,14 +88,22 @@
                         value=exc_value,
                         tb=exc_traceback,
                     )
                 ),
                 ttl=self.config.error_ttl,
             )
 
+    def send_fileobj(self, name: str, file: BinaryIO) -> None:
+        if self.execution_id is not None:
+            self.api.upload_file(
+                execution_id=self.execution_id,
+                name=name,
+                file=file,
+            )
+
 
 class AwsConnectorFactory(ConnectorFactory):
     def __init__(self, url: str, api_key: str) -> None:
         """
         Initialize TrailWatch AWS connector factory.
 
         Parameters
```

### Comparing `trailwatch-0.2.0/src/trailwatch/connectors/aws/handler.py` & `trailwatch-0.3.0/src/trailwatch/connectors/aws/handler.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.2.0/src/trailwatch/connectors/base.py` & `trailwatch-0.3.0/src/trailwatch/connectors/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 
 from abc import ABC, abstractmethod
 from types import TracebackType
-from typing import TYPE_CHECKING, Type
+from typing import TYPE_CHECKING, BinaryIO, Type
 
 if TYPE_CHECKING:
     from trailwatch.config import TrailwatchConfig
 
 
 class Connector(ABC):
     @abstractmethod
@@ -23,12 +23,16 @@
         timestamp: datetime.datetime,
         exc_type: Type[Exception],
         exc_value: Exception,
         exc_traceback: TracebackType,
     ):
         """Add exception to execution record (or do nothing)."""
 
+    @abstractmethod
+    def send_fileobj(self, name: str, file: BinaryIO) -> None:
+        """Send a file to TrailWatch (or do nothing)."""
+
 
 class ConnectorFactory(ABC):
     @abstractmethod
     def __call__(self, config: "TrailwatchConfig") -> Connector:
         """Create connector instance."""
```

