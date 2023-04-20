# Comparing `tmp/quantum_serverless-0.0.6.tar.gz` & `tmp/quantum_serverless-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantum_serverless-0.0.6.tar", last modified: Tue Mar 21 23:24:25 2023, max compression
+gzip compressed data, was "quantum_serverless-0.0.7.tar", last modified: Thu Apr 20 15:16:54 2023, max compression
```

## Comparing `quantum_serverless-0.0.6.tar` & `quantum_serverless-0.0.7.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:25.973846 quantum_serverless-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-03-21 23:24:25.973846 quantum_serverless-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:25.969846 quantum_serverless-0.0.6/quantum_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:25.973846 quantum_serverless-0.0.6/quantum_serverless/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/core/program.py
--rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/core/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:25.973846 quantum_serverless-0.0.6/quantum_serverless/library/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/library/transpiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/quantum_serverless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:25.973846 quantum_serverless-0.0.6/quantum_serverless/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/serializers/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:25.973846 quantum_serverless-0.0.6/quantum_serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/quantum_serverless/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:25.969846 quantum_serverless-0.0.6/quantum_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-03-21 23:24:25.000000 quantum_serverless-0.0.6/quantum_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-03-21 23:24:25.000000 quantum_serverless-0.0.6/quantum_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 23:24:25.000000 quantum_serverless-0.0.6/quantum_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-21 23:24:25.000000 quantum_serverless-0.0.6/quantum_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-21 23:24:25.000000 quantum_serverless-0.0.6/quantum_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-21 23:24:25.973846 quantum_serverless-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:25.973846 quantum_serverless-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:25.973846 quantum_serverless-0.0.6/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/tests/core/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/tests/core/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/tests/core/test_program_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/tests/core/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:25.973846 quantum_serverless-0.0.6/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/tests/library/test_transpiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:25.973846 quantum_serverless-0.0.6/tests/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/tests/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/tests/serializers/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/tests/test_quantum_serverless.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-21 23:24:19.000000 quantum_serverless-0.0.6/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.131033 quantum_serverless-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-20 15:16:54.131033 quantum_serverless-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.119033 quantum_serverless-0.0.7/quantum_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.127033 quantum_serverless-0.0.7/quantum_serverless/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20595 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.127033 quantum_serverless-0.0.7/quantum_serverless/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/library/transpiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/quantum_serverless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.127033 quantum_serverless-0.0.7/quantum_serverless/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/serializers/program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/serializers/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.127033 quantum_serverless-0.0.7/quantum_serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/utils/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.123033 quantum_serverless-0.0.7/quantum_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-20 15:16:54.000000 quantum_serverless-0.0.7/quantum_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-20 15:16:54.000000 quantum_serverless-0.0.7/quantum_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:16:54.000000 quantum_serverless-0.0.7/quantum_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-20 15:16:54.000000 quantum_serverless-0.0.7/quantum_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 15:16:54.000000 quantum_serverless-0.0.7/quantum_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 15:16:54.131033 quantum_serverless-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.127033 quantum_serverless-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.131033 quantum_serverless-0.0.7/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/core/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/core/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/core/test_program_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/core/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.131033 quantum_serverless-0.0.7/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/library/test_transpiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.131033 quantum_serverless-0.0.7/tests/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/serializers/test_program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/serializers/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/test_quantum_serverless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/utils.py
```

### Comparing `quantum_serverless-0.0.6/PKG-INFO` & `quantum_serverless-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum_serverless
-Version: 0.0.6
+Version: 0.0.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.0.6/README.md` & `quantum_serverless-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.6/quantum_serverless/__init__.py` & `quantum_serverless-0.0.7/quantum_serverless/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 """Quantum serverless."""
 
 from importlib_metadata import version as metadata_version, PackageNotFoundError
 
 from .core import (
     Provider,
     run_qiskit_remote,
+    distribute_task,
     get,
     put,
     get_refs_by_status,
     KuberayProvider,
     GatewayProvider,
     save_result,
 )
 from .quantum_serverless import QuantumServerless
 from .core.program import Program
+from .serializers import get_arguments
 
 try:
     __version__ = metadata_version("quantum_serverless")
 except PackageNotFoundError:  # pragma: no cover
     # package is not installed
     pass
```

### Comparing `quantum_serverless-0.0.6/quantum_serverless/core/__init__.py` & `quantum_serverless-0.0.7/quantum_serverless/core/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 .. autosummary::
     :toctree: ../stubs/
 
     Provider
     ComputeResource
 
+    distribute_task
     run_qiskit_remote
     get
     put
     get_refs_by_status
 
 
 Events classes
@@ -52,11 +53,18 @@
     :toctree: ../stubs/
 
     StateHandler
     RedisStateHandler
 """
 
 from .provider import Provider, ComputeResource, KuberayProvider, GatewayProvider
-from .decorators import remote, get, put, run_qiskit_remote, get_refs_by_status
+from .decorators import (
+    remote,
+    get,
+    put,
+    run_qiskit_remote,
+    get_refs_by_status,
+    distribute_task,
+)
 from .events import RedisEventHandler, EventHandler, ExecutionMessage
 from .state import RedisStateHandler, StateHandler
 from .job import save_result
```

### Comparing `quantum_serverless-0.0.6/quantum_serverless/core/constants.py` & `quantum_serverless-0.0.7/quantum_serverless/core/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,13 +35,16 @@
 ENV_KEYCLOAK_REALM = "ENV_KEYCLOAK_REALM"
 ENV_KEYCLOAK_CLIENT_ID = "ENV_KEYCLOAK_CLIENT_ID"
 
 # request timeout
 REQUESTS_TIMEOUT: int = 30
 
 # gateway
-GATEWAY_PROVIDER_HOST = "GATEWAY_PROVIDER_HOST"
+ENV_GATEWAY_PROVIDER_HOST = "ENV_GATEWAY_PROVIDER_HOST"
+ENV_GATEWAY_PROVIDER_VERSION = "ENV_GATEWAY_PROVIDER_VERSION"
+GATEWAY_PROVIDER_VERSION_DEFAULT = "v1"
 
 # auth
 ENV_JOB_GATEWAY_TOKEN = "ENV_JOB_GATEWAY_TOKEN"
 ENV_JOB_GATEWAY_HOST = "ENV_JOB_GATEWAY_HOST"
 ENV_JOB_ID_GATEWAY = "ENV_JOB_ID_GATEWAY"
+ENV_JOB_ARGUMENTS = "ENV_JOB_ARGUMENTS"
```

### Comparing `quantum_serverless-0.0.6/quantum_serverless/core/decorators.py` & `quantum_serverless-0.0.7/quantum_serverless/core/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,17 +23,19 @@
 .. autosummary::
     :toctree: ../stubs/
 
     get
     put
     run_qiskit_remote
     get_refs_by_status
+    distribute_task
 """
 import functools
 import os
+import warnings
 from dataclasses import dataclass
 from typing import Optional, Dict, Any, Union, List, Callable, Sequence
 
 import ray
 from opentelemetry.trace.propagation.tracecontext import TraceContextTextMapPropagator
 from qiskit import QuantumCircuit
 from ray.runtime_env import RuntimeEnv
@@ -204,31 +206,53 @@
     return decorator
 
 
 def run_qiskit_remote(
     target: Optional[Union[Dict[str, Any], Target]] = None,
     state: Optional[StateHandler] = None,
 ):
+    """(Deprecated) Wraps local function as remote executable function.
+    New function will return reference object when called.
+
+    Args:
+        target: target object or dictionary for requirements for node resources
+        state: state handler
+
+    Returns:
+        object reference
+    """
+    warnings.warn(
+        "Decorator `run_qiskit_remote` is deprecated. "
+        "Please, consider using `distribute_task` instead.",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return distribute_task(target, state)
+
+
+def distribute_task(
+    target: Optional[Union[Dict[str, Any], Target]] = None,
+    state: Optional[StateHandler] = None,
+):
     """Wraps local function as remote executable function.
     New function will return reference object when called.
 
     Example:
         >>> import quantum_serverless as qs
         >>>
-        >>> @run_qiskit_remote()
+        >>> @distribute_task()
         >>> def awesome_function(seed: int):
         >>>     return 42
         >>>
         >>> reference = awesome_function()
         >>> function_result = qs.get(reference)
 
     Args:
         target: target object or dictionary for requirements for node resources
         state: state handler
-        events: events handler
 
     Returns:
         object reference
     """
     if target is None:
         target = Target(cpu=1)
```

### Comparing `quantum_serverless-0.0.6/quantum_serverless/core/events.py` & `quantum_serverless-0.0.7/quantum_serverless/core/events.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.6/quantum_serverless/core/job.py` & `quantum_serverless-0.0.7/quantum_serverless/core/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
 from quantum_serverless.core.constants import (
     OT_PROGRAM_NAME,
     REQUESTS_TIMEOUT,
     ENV_JOB_GATEWAY_TOKEN,
     ENV_JOB_GATEWAY_HOST,
     ENV_JOB_ID_GATEWAY,
+    ENV_GATEWAY_PROVIDER_VERSION,
+    GATEWAY_PROVIDER_VERSION_DEFAULT,
 )
 from quantum_serverless.core.program import Program
 from quantum_serverless.utils.json import is_jsonable
 
 RuntimeEnv = ray.runtime_env.RuntimeEnv
 
 
@@ -107,15 +109,18 @@
                     arg_list.append(f"--{key}='{json.dumps(value)}'")
                 else:
                     arg_list.append(f"--{key}={value}")
             arguments = " ".join(arg_list)
         entrypoint = f"python {program.entrypoint} {arguments}"
 
         # set program name so OT can use it as parent span name
-        env_vars = {**(program.env_vars or {}), **{OT_PROGRAM_NAME: program.title}}
+        env_vars = {
+            **(program.env_vars or {}),
+            **{OT_PROGRAM_NAME: program.title},
+        }
 
         job_id = self._job_client.submit_job(
             entrypoint=entrypoint,
             submission_id=f"qs_{uuid4()}",
             runtime_env={
                 "working_dir": program.working_dir,
                 "pip": program.dependencies,
@@ -124,29 +129,31 @@
         )
         return Job(job_id=job_id, job_client=self)
 
 
 class GatewayJobClient(BaseJobClient):
     """GatewayJobClient."""
 
-    def __init__(self, host: str, token: str):
+    def __init__(self, host: str, token: str, version: str):
         """Job client for Gateway service.
 
         Args:
             host: gateway host
+            version: gateway version
             token: authorization token
         """
         self.host = host
+        self.version = version
         self._token = token
 
     def status(self, job_id: str):
         default_status = "Unknown"
         status = default_status
         response = requests.get(
-            f"{self.host}/jobs/{job_id}/",
+            f"{self.host}/api/{self.version}/jobs/{job_id}/",
             headers={"Authorization": f"Bearer {self._token}"},
             timeout=REQUESTS_TIMEOUT,
         )
         if response.ok:
             status = json.loads(response.text).get("status", default_status)
         else:
             logging.warning(
@@ -156,30 +163,30 @@
 
     def stop(self, job_id: str):
         raise NotImplementedError
 
     def logs(self, job_id: str):
         result = None
         response = requests.get(
-            f"{self.host}/jobs/{job_id}/logs/",
+            f"{self.host}/api/{self.version}/jobs/{job_id}/logs/",
             headers={"Authorization": f"Bearer {self._token}"},
             timeout=REQUESTS_TIMEOUT,
         )
         if response.ok:
             result = json.loads(response.text).get("logs", None)
         else:
             logging.warning(
                 "Something went wrong during job result fetching. %s", response.text
             )
         return result
 
     def result(self, job_id: str):
         result = None
         response = requests.get(
-            f"{self.host}/jobs/{job_id}/",
+            f"{self.host}/api/{self.version}/jobs/{job_id}/",
             headers={"Authorization": f"Bearer {self._token}"},
             timeout=REQUESTS_TIMEOUT,
         )
         if response.ok:
             result = json.loads(response.text).get("result", None)
         else:
             logging.warning(
@@ -219,14 +226,19 @@
 
     def __repr__(self):
         return f"<Job | {self.job_id}>"
 
 
 def save_result(result: Dict[str, Any]):
     """Saves job results."""
+
+    version = os.environ.get(ENV_GATEWAY_PROVIDER_VERSION)
+    if version is None:
+        version = GATEWAY_PROVIDER_VERSION_DEFAULT
+
     token = os.environ.get(ENV_JOB_GATEWAY_TOKEN)
     if token is None:
         logging.warning(
             "Results will not be saves as "
             "there are no information about "
             "authorization token in environment."
         )
@@ -234,15 +246,15 @@
 
     if not is_jsonable(result):
         logging.warning("Object passed is not json serializable.")
         return False
 
     url = (
         f"{os.environ.get(ENV_JOB_GATEWAY_HOST)}/"
-        f"jobs/{os.environ.get(ENV_JOB_ID_GATEWAY)}/result/"
+        f"api/{version}/jobs/{os.environ.get(ENV_JOB_ID_GATEWAY)}/result/"
     )
     response = requests.post(
         url,
         json={"result": result},
         headers={"Authorization": f"Bearer {token}"},
         timeout=REQUESTS_TIMEOUT,
     )
```

### Comparing `quantum_serverless-0.0.6/quantum_serverless/core/program.py` & `quantum_serverless-0.0.7/quantum_serverless/core/program.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 """
 =================================================
 Provider (:mod:`quantum_serverless.core.program`)
 =================================================
 
 .. currentmodule:: quantum_serverless.core.program
 
-Quantum serverless nested program
-=================================
+Quantum serverless program
+==========================
 
 .. autosummary::
     :toctree: ../stubs/
 
     Program
 """
 import dataclasses
@@ -40,28 +40,29 @@
 
 from quantum_serverless.core.constants import (
     REPO_HOST_KEY,
     REPO_PORT_KEY,
 )
 
 from quantum_serverless.exception import QuantumServerlessException
+from quantum_serverless.serializers.program_serializers import QiskitObjectsEncoder
 from quantum_serverless.utils.json import is_jsonable
 
 
 @dataclass
 class Program:  # pylint: disable=too-many-instance-attributes
-    """Serverless programs.
+    """Serverless Program.
 
     Args:
         title: program name
         entrypoint: is a script that will be executed as a job
             ex: job.py
         arguments: arguments for entrypoint script
         env_vars: env vars
-        dependencies: list of python dependencies for program to execute
+        dependencies: list of python dependencies to execute a program
         working_dir: directory where entrypoint file is located
         description: description of a program
         version: version of a program
     """
 
     title: str
     entrypoint: str
@@ -76,28 +77,30 @@
     @classmethod
     def from_json(cls, data: Dict[str, Any]):
         """Reconstructs Program from dictionary."""
         field_names = set(f.name for f in dataclasses.fields(Program))
         return Program(**{k: v for k, v in data.items() if k in field_names})
 
     def __post_init__(self):
-        if self.arguments is not None and not is_jsonable(self.arguments):
+        if self.arguments is not None and not is_jsonable(
+            self.arguments, cls=QiskitObjectsEncoder
+        ):
             raise QuantumServerlessException(
                 "Arguments provided are not json serializable."
             )
 
 
 class ProgramStorage(ABC):
     """Base program backend to save and load programs from."""
 
     def save_program(self, program: Program) -> bool:
         """Save program in specified backend.
 
         Args:
-            program: program
+            program: program object
 
         Returns:
             success state
         """
         raise NotImplementedError
 
     def get_programs(self, **kwargs) -> List[str]:
@@ -108,15 +111,15 @@
 
         Returns:
             List of names of programs
         """
         raise NotImplementedError
 
     def get_program(self, title: str, **kwargs) -> Optional[Program]:
-        """Returns program by name of other query criteria.
+        """Returns program by name and other query criteria.
 
         Args:
             title: title of the program
             **kwargs: other args
 
         Returns:
             Program
@@ -142,15 +145,15 @@
             token: authentication token
             folder: path to directory where title files will be stored
         """
         self.folder = folder or os.path.dirname(os.path.abspath(__file__))
         self._host = host or os.environ.get(REPO_HOST_KEY, "http://localhost")
         self._port = port or os.environ.get(REPO_PORT_KEY, 80)
         self._token = token
-        self._base_url = f"{self._host}:{self._port}/v1/api/nested-programs/"
+        self._base_url = f"{self._host}:{self._port}/api/v1/programs/"
 
     def save_program(self, program: Program) -> bool:
         raise NotImplementedError("Not implemented yet.")
 
     def get_programs(self, **kwargs) -> List[str]:
         result = []
         response = requests.get(url=self._base_url, params=kwargs, timeout=10)
@@ -198,15 +201,15 @@
     Returns:
         workdir for program
     """
     program_folder_path = os.path.join(folder, program.title)
     artifact_file_name = "artifact"
     tarfile_path = os.path.join(program_folder_path, artifact_file_name)
 
-    # check if program already exist on the disc
+    # check if program path already exist on the disc
     if os.path.exists(program_folder_path):
         logging.warning("Program folder already exist. Will be overwritten.")
 
     # download file
     response = requests.get(url=artifact_url, stream=True, headers=headers, timeout=100)
     if not response.ok:
         raise QuantumServerlessException(
```

### Comparing `quantum_serverless-0.0.6/quantum_serverless/core/provider.py` & `quantum_serverless-0.0.7/quantum_serverless/core/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,28 @@
 import ray
 import requests
 from ray.dashboard.modules.job.sdk import JobSubmissionClient
 
 from quantum_serverless.core.constants import (
     RAY_IMAGE,
     REQUESTS_TIMEOUT,
-    GATEWAY_PROVIDER_HOST,
+    ENV_GATEWAY_PROVIDER_HOST,
+    ENV_GATEWAY_PROVIDER_VERSION,
+    GATEWAY_PROVIDER_VERSION_DEFAULT,
 )
 from quantum_serverless.core.job import (
     Job,
     RayJobClient,
     GatewayJobClient,
     BaseJobClient,
 )
 from quantum_serverless.core.program import Program
 from quantum_serverless.core.tracing import _trace_env_vars
 from quantum_serverless.exception import QuantumServerlessException
+from quantum_serverless.serializers.program_serializers import QiskitObjectsEncoder
 from quantum_serverless.utils import JsonSerializable
 
 TIMEOUT = 30
 
 
 @dataclass
 class ComputeResource:
@@ -247,28 +250,28 @@
                 "Job has not been found as no provider "
                 "with remote host has been configured. "
             )
             return None
         return Job(job_id=job_id, job_client=job_client)
 
     def run_program(self, program: Program) -> Job:
-        """Execute program as a async job.
+        """Execute a program as a async job.
 
         Example:
             >>> serverless = QuantumServerless()
-            >>> nested_program = Program(
+            >>> program = Program(
             >>>     "job.py",
             >>>     arguments={"arg1": "val1"},
             >>>     dependencies=["requests"]
             >>> )
-            >>> job = serverless.run_program(nested_program)
+            >>> job = serverless.run_program(program)
             >>> # <Job | ...>
 
         Args:
-            program: program object
+            program: Program object
 
         Returns:
             Job
         """
         job_client = self.job_client()
 
         if job_client is None:
@@ -471,42 +474,49 @@
 class GatewayProvider(Provider):
     """GatewayProvider."""
 
     def __init__(
         self,
         name: Optional[str] = None,
         host: Optional[str] = None,
+        version: Optional[str] = None,
         username: Optional[str] = None,
         password: Optional[str] = None,
         token: Optional[str] = None,
     ):
         """GatewayProvider.
 
         Args:
             name: name of provider
             host: host of gateway
+            version: version of gateway
             username: username
             password: password
             token: authorization token
         """
         name = name or "gateway-provider"
 
-        host = host or os.environ.get(GATEWAY_PROVIDER_HOST)
+        host = host or os.environ.get(ENV_GATEWAY_PROVIDER_HOST)
         if host is None:
             raise QuantumServerlessException("Please provide `host` of gateway.")
 
+        version = version or os.environ.get(ENV_GATEWAY_PROVIDER_VERSION)
+        if version is None:
+            version = GATEWAY_PROVIDER_VERSION_DEFAULT
+
         if token is None and (username is None or password is None):
             raise QuantumServerlessException(
                 "Authentication credentials must "
                 "be provided in form of `username` "
                 "and `password` or `token`."
             )
 
         super().__init__(name)
         self.host = host
+        self.version = version
         self._token = token
         if token is None:
             self._fetch_token(username, password)
 
     def get_compute_resources(self) -> List[ComputeResource]:
         raise NotImplementedError("GatewayProvider does not support resources api yet.")
 
@@ -514,46 +524,49 @@
         raise NotImplementedError("GatewayProvider does not support resources api yet.")
 
     def delete_compute_resource(self, resource) -> int:
         raise NotImplementedError("GatewayProvider does not support resources api yet.")
 
     def get_job_by_id(self, job_id: str) -> Optional[Job]:
         job = None
-        url = f"{self.host}/jobs/{job_id}/"
+        url = f"{self.host}/api/{self.version}/jobs/{job_id}/"
         response = requests.get(
             url,
             headers={"Authorization": f"Bearer {self._token}"},
             timeout=REQUESTS_TIMEOUT,
         )
         if response.ok:
             data = json.loads(response.text)
             job = Job(
                 job_id=data.get("id"),
-                job_client=GatewayJobClient(self.host, self._token),
+                job_client=GatewayJobClient(self.host, self._token, self.version),
             )
         else:
             logging.warning(response.text)
 
         return job
 
     def run_program(self, program: Program) -> Job:
-        url = f"{self.host}/programs/run_program/"
+        url = f"{self.host}/api/{self.version}/programs/run/"
         artifact_file_path = os.path.join(program.working_dir, "artifact.tar")
+
         with tarfile.open(artifact_file_path, "w") as tar:
             for filename in os.listdir(program.working_dir):
                 fpath = os.path.join(program.working_dir, filename)
                 tar.add(fpath, arcname=filename)
 
         with open(artifact_file_path, "rb") as file:
             response = requests.post(
                 url=url,
                 data={
                     "title": program.title,
                     "entrypoint": program.entrypoint,
-                    "arguments": json.dumps(program.arguments or {}),
+                    "arguments": json.dumps(
+                        program.arguments or {}, cls=QiskitObjectsEncoder
+                    ),
                     "dependencies": json.dumps(program.dependencies or []),
                 },
                 files={"artifact": file},
                 headers={"Authorization": f"Bearer {self._token}"},
                 timeout=REQUESTS_TIMEOUT,
             )
             if not response.ok:
@@ -563,29 +576,31 @@
 
             json_response = json.loads(response.text)
             job_id = json_response.get("id")
 
         if os.path.exists(artifact_file_path):
             os.remove(artifact_file_path)
 
-        return Job(job_id, job_client=GatewayJobClient(self.host, self._token))
+        return Job(
+            job_id, job_client=GatewayJobClient(self.host, self._token, self.version)
+        )
 
     def get_jobs(self, **kwargs) -> List[Job]:
         jobs = []
-        url = f"{self.host}/jobs/"
+        url = f"{self.host}/api/{self.version}/jobs/"
         response = requests.get(
             url,
             headers={"Authorization": f"Bearer {self._token}"},
             timeout=REQUESTS_TIMEOUT,
         )
         if response.ok:
             jobs = [
                 Job(
                     job_id=job.get("id"),
-                    job_client=GatewayJobClient(self.host, self._token),
+                    job_client=GatewayJobClient(self.host, self._token, self.version),
                 )
                 for job in json.loads(response.text).get("results", [])
             ]
         else:
             logging.warning(response.text)
 
         return jobs
```

### Comparing `quantum_serverless-0.0.6/quantum_serverless/core/state.py` & `quantum_serverless-0.0.7/quantum_serverless/core/state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.6/quantum_serverless/core/tracing.py` & `quantum_serverless-0.0.7/quantum_serverless/core/tracing.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.6/quantum_serverless/exception.py` & `quantum_serverless-0.0.7/quantum_serverless/exception.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.6/quantum_serverless/library/__init__.py` & `quantum_serverless-0.0.7/quantum_serverless/library/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.6/quantum_serverless/library/transpiler.py` & `quantum_serverless-0.0.7/quantum_serverless/library/transpiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 """
 from typing import List, Union
 
 from qiskit import QuantumCircuit, transpile
 from qiskit.providers import Backend
 
 from quantum_serverless.exception import QuantumServerlessException
-from quantum_serverless import run_qiskit_remote, get, put
+from quantum_serverless import distribute_task, get, put
 
-transpile_ray = run_qiskit_remote()(transpile)
+transpile_ray = distribute_task()(transpile)
 
 
-@run_qiskit_remote()
+@distribute_task()
 def remote_transpile(
     circuits: List[Union[QuantumCircuit, List[QuantumCircuit]]], backends: List[Backend]
 ) -> List[List[QuantumCircuit]]:
     """Remote transpile."""
     transpile_circuits_tasks = [
         transpile_ray(circuits=circuits, backend=backend)
         for circuits, backend in zip(circuits, backends)
```

### Comparing `quantum_serverless-0.0.6/quantum_serverless/quantum_serverless.py` & `quantum_serverless-0.0.7/quantum_serverless/quantum_serverless.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,28 +82,28 @@
 
     @property
     def job_client(self):
         """Job client for given provider."""
         return self._selected_provider.job_client()
 
     def run_program(self, program: Program) -> Optional[Job]:
-        """Execute program as a async job
+        """Execute a program as a async job
 
         Example:
             >>> serverless = QuantumServerless()
-            >>> nested_program = Program(
+            >>> program = Program(
             >>>     "job.py",
             >>>     arguments={"arg1": "val1"},
             >>>     dependencies=["requests"]
             >>> )
-            >>> job = serverless.run_program(nested_program)
+            >>> job = serverless.run_program(program)
             >>> # <Job | ...>
 
         Args:
-            program: program object
+            program: Program object
 
         Returns:
             Job
         """
         return self._selected_provider.run_program(program)
 
     def get_job_by_id(self, job_id: str) -> Optional[Job]:
```

### Comparing `quantum_serverless-0.0.6/quantum_serverless/serializers/__init__.py` & `quantum_serverless-0.0.7/quantum_serverless/serializers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,33 +7,36 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
-===============================================================
-Serializers (:mod:`quantum_serverless.serializers.serializers`)
-===============================================================
+===================================================
+Serializers (:mod:`quantum_serverless.serializers`)
+===================================================
 
-.. currentmodule:: quantum_serverless.serializers.serializers
+.. currentmodule:: quantum_serverless.serializers
 
 Quantum serverless serializers
 ==============================
 
 .. autosummary::
     :toctree: ../stubs/
 
     register_all_serializers
     circuit_serializer
     circuit_deserializer
     service_serializer
     service_deserializer
+    get_arguments
 """
 
 from .serializers import (
     register_all_serializers,
     circuit_serializer,
     circuit_deserializer,
     service_serializer,
     service_deserializer,
 )
+
+from .program_serializers import get_arguments
```

### Comparing `quantum_serverless-0.0.6/quantum_serverless/serializers/serializers.py` & `quantum_serverless-0.0.7/quantum_serverless/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.6/quantum_serverless/utils/__init__.py` & `quantum_serverless-0.0.7/quantum_serverless/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.6/quantum_serverless/utils/json.py` & `quantum_serverless-0.0.7/quantum_serverless/utils/json.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 .. autosummary::
     :toctree: ../stubs/
 
     JsonSerializable
 """
 import json
 from abc import ABC
+from json import JSONEncoder
+from typing import Optional, Type
 
 
 class JsonSerializable(ABC):
     """Classes that can be serialized as json."""
 
     @classmethod
     def from_dict(cls, dictionary: dict):
@@ -54,14 +56,14 @@
                 element = val.to_dict()  # type: ignore
             else:
                 element = val
             result[key] = element
         return result
 
 
-def is_jsonable(data):
+def is_jsonable(data, cls: Optional[Type[JSONEncoder]] = None):
     """Check if data can be serialized to json."""
     try:
-        json.dumps(data)
+        json.dumps(data, cls=cls)
         return True
     except (TypeError, OverflowError):
         return False
```

### Comparing `quantum_serverless-0.0.6/quantum_serverless.egg-info/PKG-INFO` & `quantum_serverless-0.0.7/quantum_serverless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum-serverless
-Version: 0.0.6
+Version: 0.0.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.0.6/quantum_serverless.egg-info/SOURCES.txt` & `quantum_serverless-0.0.7/quantum_serverless.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,24 @@
 quantum_serverless/core/program.py
 quantum_serverless/core/provider.py
 quantum_serverless/core/state.py
 quantum_serverless/core/tracing.py
 quantum_serverless/library/__init__.py
 quantum_serverless/library/transpiler.py
 quantum_serverless/serializers/__init__.py
+quantum_serverless/serializers/program_serializers.py
 quantum_serverless/serializers/serializers.py
 quantum_serverless/utils/__init__.py
 quantum_serverless/utils/json.py
 tests/__init__.py
 tests/test_quantum_serverless.py
 tests/utils.py
 tests/core/__init__.py
 tests/core/test_decorator.py
 tests/core/test_program.py
 tests/core/test_program_repository.py
 tests/core/test_state.py
 tests/library/__init__.py
 tests/library/test_transpiler.py
 tests/serializers/__init__.py
+tests/serializers/test_program_serializers.py
 tests/serializers/test_serializers.py
```

### Comparing `quantum_serverless-0.0.6/setup.py` & `quantum_serverless-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.6/tests/core/test_decorator.py` & `quantum_serverless-0.0.7/tests/core/test_decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from qiskit import QuantumCircuit
 from qiskit.circuit.random import random_circuit
 
 from quantum_serverless import QuantumServerless, get
 from quantum_serverless.core.decorators import (
     run_qiskit_remote,
+    distribute_task,
     Target,
     fetch_execution_meta,
 )
 from quantum_serverless.core.state import StateHandler
 
 
 class TestHandler(StateHandler):
@@ -61,14 +62,42 @@
             mid_result = get(
                 another_function(
                     [random_circuit(5, 2)], other_circuit=random_circuit(5, 2)
                 )
             )
             return mid_result
 
+        with self.assertWarns(Warning), serverless.context():
+            reference = ultimate_function(1)
+            result = get(reference)
+            self.assertEqual(result, 4)
+
+    def test_distribute_task(self):
+        """Test for run_qiskit_remote."""
+
+        serverless = QuantumServerless()
+
+        @distribute_task()
+        def another_function(
+            circuit: List[QuantumCircuit], other_circuit: QuantumCircuit
+        ):
+            """Another test function."""
+            return circuit[0].compose(other_circuit, range(5)).depth()
+
+        @distribute_task(target={"cpu": 1})
+        def ultimate_function(ultimate_argument: int):
+            """Test function."""
+            print("Printing function argument:", ultimate_argument)
+            mid_result = get(
+                another_function(
+                    [random_circuit(5, 2)], other_circuit=random_circuit(5, 2)
+                )
+            )
+            return mid_result
+
         with serverless.context():
             reference = ultimate_function(1)
             result = get(reference)
             self.assertEqual(result, 4)
 
     def test_target(self):
         """Test for target."""
@@ -77,15 +106,15 @@
         self.assertEqual(target.pip, target_expected.pip)
 
     def test_remote_with_state_injection(self):
         """Tests remote with state injection."""
         serverless = QuantumServerless()
         state_handler = TestHandler()
 
-        @run_qiskit_remote(target={"cpu": 1}, state=state_handler)
+        @distribute_task(target={"cpu": 1}, state=state_handler)
         def ultimate_function_with_state(state: StateHandler, ultimate_argument: int):
             """Test function."""
             state.set("some_key", {"result": ultimate_argument})
             return state.get("some_key")
 
         with serverless.context():
             reference = (
```

### Comparing `quantum_serverless-0.0.6/tests/core/test_program.py` & `quantum_serverless-0.0.7/tests/core/test_program.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """Tests jobs."""
 import os
 from unittest import TestCase
 
-import numpy as np
 from ray.dashboard.modules.job.common import JobStatus
 from testcontainers.compose import DockerCompose
 
 from quantum_serverless import QuantumServerless, Provider
 from quantum_serverless.core import ComputeResource
 from quantum_serverless.core.job import Job
 from quantum_serverless.core.program import Program
-from quantum_serverless.exception import QuantumServerlessException
 from tests.utils import wait_for_job_client, wait_for_job_completion
 
 resources_path = os.path.join(
     os.path.dirname(os.path.abspath(__file__)), "../resources"
 )
 
 
@@ -26,24 +24,17 @@
         program = Program(
             title="awesome_program",
             entrypoint="awesome.py",
             arguments={"one": 1, "json": {"one": 1, "two": 2}},
         )
         self.assertIsInstance(program, Program)
 
-        with self.assertRaises(QuantumServerlessException):
-            Program(
-                title="awesome_program",
-                entrypoint="awesome.py",
-                arguments={"one": 1, "json": {"one": np.array([1]), "two": 2}},
-            )
-
 
 def test_program():
-    """Integration test for programs."""
+    """Integration test for program."""
 
     with DockerCompose(
         resources_path, compose_file_name="test-compose.yml", pull=True
     ) as compose:
         host = compose.get_service_host("testrayhead", 8265)
         port = compose.get_service_port("testrayhead", 8265)
```

### Comparing `quantum_serverless-0.0.6/tests/core/test_program_repository.py` & `quantum_serverless-0.0.7/tests/core/test_program_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Test program repository."""
 import json
 import os.path
 import shutil
 from pathlib import Path
 from unittest import TestCase, mock
 
-from quantum_serverless.core.program import ProgramRepository, Program
+from quantum_serverless.core.program import (
+    ProgramRepository,
+    Program,
+)
 
 responses = {
-    "http://localhost:80/v1/api/nested-programs/": {
+    "http://localhost:80/api/v1/programs/": {
         "count": 2,
         "results": [
             {
                 "id": "be7e5406-d111-4768-9a93-7cedf4d46608",
                 "created": "2023-02-15T14:38:41.120934Z",
                 "updated": "2023-02-15T14:38:41.120975Z",
                 "title": "hello_world",
@@ -120,15 +123,15 @@
 
     def tearDown(self) -> None:
         if os.path.exists(self.programs_folder):
             shutil.rmtree(self.programs_folder)
 
     @mock.patch("requests.get", side_effect=mocked_requests_get)
     def test_repository_get_programs(self, mock_get):
-        """Tests program repository."""
+        """Tests programs repository."""
 
         repository = ProgramRepository(host="http://localhost")
         programs = repository.get_programs()
         self.assertEqual(programs, ["hello_world", "Test"])
         self.assertEqual(len(mock_get.call_args_list), 1)
 
     @mock.patch("requests.get", side_effect=mocked_requests_get)
```

### Comparing `quantum_serverless-0.0.6/tests/core/test_state.py` & `quantum_serverless-0.0.7/tests/core/test_state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.6/tests/library/test_transpiler.py` & `quantum_serverless-0.0.7/tests/library/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.6/tests/serializers/test_serializers.py` & `quantum_serverless-0.0.7/tests/serializers/test_serializers.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 class TestSerializers(TestCase):
     """TestSerializers."""
 
     def test_quantum_circuit_serializers(self):
         """Tests quantum service serialization."""
         serverless = QuantumServerless()
-        with serverless:
+        with serverless.context():
             register_serializer(
                 QuantumCircuit,
                 serializer=circuit_serializer,
                 deserializer=circuit_deserializer,
             )
 
             res = get(circuit_function(random_circuit(3, 2)))
```

### Comparing `quantum_serverless-0.0.6/tests/test_quantum_serverless.py` & `quantum_serverless-0.0.7/tests/test_quantum_serverless.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 class TestQuantumServerless(TestCase):
     """Tests for QuantumServerless."""
 
     def test_qs_class(self):
         """Tests template class."""
         serverless = QuantumServerless()
 
-        with serverless:
+        with serverless.context():
             self.assertTrue(ray.is_initialized())
 
         self.assertFalse(ray.is_initialized())
 
     def test_for_at_least_one_cluster_and_one_provider(self):
         """Test for at least one compute_resource."""
         serverless = QuantumServerless()
```

### Comparing `quantum_serverless-0.0.6/tests/utils.py` & `quantum_serverless-0.0.7/tests/utils.py`

 * *Files identical despite different names*

