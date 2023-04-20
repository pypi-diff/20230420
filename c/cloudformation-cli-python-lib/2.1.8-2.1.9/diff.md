# Comparing `tmp/cloudformation-cli-python-lib-2.1.8.tar.gz` & `tmp/cloudformation-cli-python-lib-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudformation-cli-python-lib-2.1.8.tar", last modified: Tue Aug 24 19:50:22 2021, max compression
+gzip compressed data, was "cloudformation-cli-python-lib-2.1.9.tar", last modified: Thu Feb 10 22:25:42 2022, max compression
```

## Comparing `cloudformation-cli-python-lib-2.1.8.tar` & `cloudformation-cli-python-lib-2.1.9.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 omkhegde (1559287979) staff       (20)        0 2021-08-24 19:50:22.597960 cloudformation-cli-python-lib-2.1.8/
--rw-r--r--   0 omkhegde (1559287979) staff       (20)      139 2020-12-10 23:45:14.000000 cloudformation-cli-python-lib-2.1.8/MANIFEST.in
--rw-r--r--   0 omkhegde (1559287979) staff       (20)      985 2021-08-24 19:50:22.597715 cloudformation-cli-python-lib-2.1.8/PKG-INFO
-drwxr-xr-x   0 omkhegde (1559287979) staff       (20)        0 2021-08-24 19:50:22.595591 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/
--rw-r--r--   0 omkhegde (1559287979) staff       (20)      323 2021-03-30 21:08:42.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/__init__.py
--rw-r--r--   0 omkhegde (1559287979) staff       (20)      735 2021-08-24 19:22:31.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/boto3_proxy.py
--rw-r--r--   0 omkhegde (1559287979) staff       (20)     1676 2021-06-24 22:30:40.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/exceptions.py
--rw-r--r--   0 omkhegde (1559287979) staff       (20)     1774 2020-12-10 23:45:14.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/identifier_utils.py
--rw-r--r--   0 omkhegde (1559287979) staff       (20)     4248 2021-06-24 22:30:40.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/interface.py
--rw-r--r--   0 omkhegde (1559287979) staff       (20)     3856 2021-08-24 19:22:31.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/log_delivery.py
--rw-r--r--   0 omkhegde (1559287979) staff       (20)     6440 2020-12-10 23:45:14.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/metrics.py
--rw-r--r--   0 omkhegde (1559287979) staff       (20)        0 2020-12-10 23:45:14.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/py.typed
--rw-r--r--   0 omkhegde (1559287979) staff       (20)     5433 2020-12-10 23:45:14.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/recast.py
--rw-r--r--   0 omkhegde (1559287979) staff       (20)     9308 2021-08-24 19:22:31.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/resource.py
--rw-r--r--   0 omkhegde (1559287979) staff       (20)     6620 2021-08-24 19:22:31.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/utils.py
-drwxr-xr-x   0 omkhegde (1559287979) staff       (20)        0 2021-08-24 19:50:22.597366 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib.egg-info/
--rw-r--r--   0 omkhegde (1559287979) staff       (20)      985 2021-08-24 19:50:22.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib.egg-info/PKG-INFO
--rw-r--r--   0 omkhegde (1559287979) staff       (20)      814 2021-08-24 19:50:22.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib.egg-info/SOURCES.txt
--rw-r--r--   0 omkhegde (1559287979) staff       (20)        1 2021-08-24 19:50:22.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib.egg-info/dependency_links.txt
--rw-r--r--   0 omkhegde (1559287979) staff       (20)       54 2021-08-24 19:50:22.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib.egg-info/requires.txt
--rw-r--r--   0 omkhegde (1559287979) staff       (20)       30 2021-08-24 19:50:22.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib.egg-info/top_level.txt
--rw-r--r--   0 omkhegde (1559287979) staff       (20)        1 2021-08-24 19:50:22.000000 cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib.egg-info/zip-safe
--rw-r--r--   0 omkhegde (1559287979) staff       (20)       38 2021-08-24 19:50:22.598048 cloudformation-cli-python-lib-2.1.8/setup.cfg
--rw-r--r--   0 omkhegde (1559287979) staff       (20)     1263 2021-08-24 19:23:40.000000 cloudformation-cli-python-lib-2.1.8/setup.py
+drwxr-xr-x   0 omkhegde (1559287979) staff       (20)        0 2022-02-10 22:25:42.354282 cloudformation-cli-python-lib-2.1.9/
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)    10142 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/LICENSE
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)      139 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/MANIFEST.in
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)      996 2022-02-10 22:25:42.354037 cloudformation-cli-python-lib-2.1.9/PKG-INFO
+drwxr-xr-x   0 omkhegde (1559287979) staff       (20)        0 2022-02-10 22:25:42.351935 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)      469 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/__init__.py
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)      735 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/boto3_proxy.py
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)     3603 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/cipher.py
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)     2009 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/exceptions.py
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)    11833 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/hook.py
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)     1774 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/identifier_utils.py
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)     6261 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/interface.py
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)     5456 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/log_delivery.py
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)    10038 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/metrics.py
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)        0 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/py.typed
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)     5426 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/recast.py
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)     9372 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/resource.py
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)    10415 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/utils.py
+drwxr-xr-x   0 omkhegde (1559287979) staff       (20)        0 2022-02-10 22:25:42.353712 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib.egg-info/
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)      996 2022-02-10 22:25:42.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib.egg-info/PKG-INFO
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)      900 2022-02-10 22:25:42.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)        1 2022-02-10 22:25:42.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)       80 2022-02-10 22:25:42.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib.egg-info/requires.txt
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)       30 2022-02-10 22:25:42.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib.egg-info/top_level.txt
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)        1 2022-02-10 22:25:42.000000 cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib.egg-info/zip-safe
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)       38 2022-02-10 22:25:42.354365 cloudformation-cli-python-lib-2.1.9/setup.cfg
+-rw-r--r--   0 omkhegde (1559287979) staff       (20)     1323 2022-02-10 22:18:45.000000 cloudformation-cli-python-lib-2.1.9/setup.py
```

### Comparing `cloudformation-cli-python-lib-2.1.8/PKG-INFO` & `cloudformation-cli-python-lib-2.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: cloudformation-cli-python-lib
-Version: 2.1.8
+Version: 2.1.9
 Summary: Support library to enable Python-based CloudFormation resource types
 Home-page: https://github.com/aws-cloudformation/aws-cloudformation-rpdk-python-plugin/
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
-Description: UNKNOWN
 Keywords: Amazon Web Services AWS CloudFormation
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/boto3_proxy.py` & `cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/boto3_proxy.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/exceptions.py` & `cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,7 +78,23 @@
 
 class InvalidTypeConfiguration(_HandlerError):
     def __init__(self, type_name: str, message: str):
         super().__init__(
             f"Invalid TypeConfiguration provided for type {type_name}."
             f" Reason: {message}"
         )
+
+
+class HandlerInternalFailure(_HandlerError):
+    pass
+
+
+class NonCompliant(_HandlerError):
+    def __init__(self, type_name: str, message: str):
+        super().__init__(
+            f"Hook of type '{type_name}' returned a Non-Complaint status."
+            f" Reason: {message}"
+        )
+
+
+class Unknown(_HandlerError):
+    pass
```

### Comparing `cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/identifier_utils.py` & `cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/identifier_utils.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/interface.py` & `cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/interface.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,14 +19,20 @@
     CREATE = auto()
     READ = auto()
     UPDATE = auto()
     DELETE = auto()
     LIST = auto()
 
 
+class HookInvocationPoint(str, _AutoName):
+    CREATE_PRE_PROVISION = auto()
+    UPDATE_PRE_PROVISION = auto()
+    DELETE_PRE_PROVISION = auto()
+
+
 class StandardUnit(str, _AutoName):
     Count = auto()
     Milliseconds = auto()
 
 
 class MetricTypes(str, _AutoName):
     HandlerException = auto()
@@ -37,14 +43,21 @@
 class OperationStatus(str, _AutoName):
     PENDING = auto()
     IN_PROGRESS = auto()
     SUCCESS = auto()
     FAILED = auto()
 
 
+class HookStatus(str, _AutoName):
+    PENDING = auto()
+    IN_PROGRESS = auto()
+    SUCCESS = auto()
+    FAILED = auto()
+
+
 class HandlerErrorCode(str, _AutoName):
     NotUpdatable = auto()
     InvalidRequest = auto()
     AccessDenied = auto()
     InvalidCredentials = auto()
     AlreadyExists = auto()
     NotFound = auto()
@@ -53,14 +66,17 @@
     ServiceLimitExceeded = auto()
     NotStabilized = auto()
     GeneralServiceException = auto()
     ServiceInternalError = auto()
     NetworkFailure = auto()
     InternalFailure = auto()
     InvalidTypeConfiguration = auto()
+    HandlerInternalFailure = auto()
+    NonCompliant = auto()
+    Unknown = auto()
 
 
 class BaseModel:
     def _serialize(self) -> Mapping[str, Any]:
         return {
             k: self._serialize_item(v)
             for k, v in self.__dict__.items()
@@ -87,14 +103,15 @@
 # pylint: disable=too-many-instance-attributes
 @dataclass
 class ProgressEvent:
     # pylint: disable=invalid-name
     status: OperationStatus
     errorCode: Optional[HandlerErrorCode] = None
     message: str = ""
+    result: Optional[str] = None
     callbackContext: Optional[MutableMapping[str, Any]] = None
     callbackDelaySeconds: int = 0
     resourceModel: Optional[BaseModel] = None
     resourceModels: Optional[List[BaseModel]] = None
     nextToken: Optional[str] = None
 
     def _serialize(self) -> MutableMapping[str, Any]:
@@ -117,17 +134,25 @@
             ]
         if self.errorCode:
             ser["errorCode"] = self.errorCode.name
         return ser
 
     @classmethod
     def failed(
-        cls: Type["ProgressEvent"], error_code: HandlerErrorCode, message: str = ""
+        cls: Type["ProgressEvent"],
+        error_code: HandlerErrorCode,
+        message: str = "",
+        result: Optional[str] = None,
     ) -> "ProgressEvent":
-        return cls(status=OperationStatus.FAILED, errorCode=error_code, message=message)
+        return cls(
+            status=OperationStatus.FAILED,
+            errorCode=error_code,
+            message=message,
+            result=result,
+        )
 
 
 @dataclass
 class BaseResourceHandlerRequest:
     # pylint: disable=invalid-name
     clientRequestToken: str
     desiredResourceState: Optional[BaseModel]
@@ -139,7 +164,57 @@
     awsAccountId: Optional[str]
     logicalResourceIdentifier: Optional[str]
     typeConfiguration: Optional[BaseModel]
     nextToken: Optional[str]
     region: Optional[str]
     awsPartition: Optional[str]
     stackId: Optional[str]
+
+
+@dataclass
+class HookProgressEvent:
+    hookStatus: HookStatus
+    errorCode: Optional[HandlerErrorCode] = None
+    message: str = ""
+    callbackContext: Optional[MutableMapping[str, Any]] = None
+    callbackDelaySeconds: int = 0
+    result: Optional[str] = None
+    clientRequestToken: Optional[str] = None
+
+    def _serialize(self) -> MutableMapping[str, Any]:
+        # to match Java serialization, which drops `null` values, and the
+        # contract tests currently expect this also
+        ser = {k: v for k, v in self.__dict__.items() if v is not None}
+
+        # mutate to what's expected in the response
+
+        ser["hookStatus"] = ser.pop("hookStatus").name
+
+        if self.errorCode:
+            ser["errorCode"] = self.errorCode.name
+        return ser
+
+    @classmethod
+    def failed(
+        cls: Type["HookProgressEvent"], error_code: HandlerErrorCode, message: str = ""
+    ) -> "HookProgressEvent":
+        return cls(hookStatus=HookStatus.FAILED, errorCode=error_code, message=message)
+
+
+@dataclass
+class HookContext:
+    awsAccountId: Optional[str]
+    stackId: Optional[str]
+    hookTypeName: Optional[str]
+    hookTypeVersion: Optional[str]
+    invocationPoint: Optional[HookInvocationPoint]
+    targetName: Optional[str]
+    targetType: Optional[str]
+    targetLogicalId: Optional[str]
+    targetModel: Optional[Mapping[str, Any]]
+    changeSetId: Optional[str] = None
+
+
+@dataclass
+class BaseHookHandlerRequest:
+    clientRequestToken: str
+    hookContext: HookContext
```

### Comparing `cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/log_delivery.py` & `cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/log_delivery.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import time
+import uuid
 from typing import Any, Optional
 
 from .boto3_proxy import SessionProxy
-from .utils import HandlerRequest
+from .utils import HandlerRequest, HookInvocationRequest
 
 
 class ProviderFilter(logging.Filter):
     def __init__(self, provider: str):
         super().__init__()
         self.provider = provider
 
@@ -97,7 +98,42 @@
         try:
             self._put_log_event(record)
         except self.client.exceptions.ResourceNotFoundException as e:
             if "log group does not exist" in str(e):
                 self._create_log_group()
             self._create_log_stream()
             self._put_log_event(record)
+
+
+class HookProviderLogHandler(ProviderLogHandler):
+    @classmethod
+    def _get_existing_logger(cls) -> Optional["HookProviderLogHandler"]:
+        for handler in logging.getLogger().handlers:
+            if isinstance(handler, cls):
+                return handler
+        return None
+
+    @classmethod
+    def setup(  # type: ignore
+        cls, request: HookInvocationRequest, provider_sess: Optional[SessionProxy]
+    ) -> None:
+        log_group = request.requestData.providerLogGroupName
+        if request.stackId and request.requestData.targetLogicalId:
+            stream_name = f"{request.stackId}/{request.requestData.targetLogicalId}"
+        else:
+            stream_name = f"{request.awsAccountId}-{uuid.uuid4()}"
+
+        log_handler = cls._get_existing_logger()
+        if provider_sess and log_group and request.hookTypeName:
+            if log_handler:
+                # This is a re-used lambda container, log handler is already setup, so
+                # we just refresh the client with new creds
+                log_handler.client = provider_sess.client("logs")
+                return
+            # filter provider messages from platform
+            provider = request.hookTypeName.replace("::", "_").lower()
+            logging.getLogger().handlers[0].addFilter(ProviderFilter(provider))
+            log_handler = cls(
+                group=log_group, stream=stream_name, session=provider_sess
+            )
+            # add log handler to root, so that provider gets plugin logs too
+            logging.getLogger().addHandler(log_handler)
```

### Comparing `cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/metrics.py` & `cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/metrics.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import logging
-from typing import Any, List, Mapping, Optional
+from typing import Any, List, Mapping, Optional, Union
 
 from botocore.exceptions import ClientError  # type: ignore
 
 from .boto3_proxy import SessionProxy
-from .interface import Action, MetricTypes, StandardUnit
+from .interface import Action, HookInvocationPoint, MetricTypes, StandardUnit
 
 LOG = logging.getLogger(__name__)
 
 METRIC_NAMESPACE_ROOT = "AWS/CloudFormation"
 
 
 def format_dimensions(dimensions: Mapping[str, str]) -> List[Mapping[str, str]]:
@@ -130,14 +130,99 @@
 
     @staticmethod
     def _make_namespace(resource_type: str) -> str:
         suffix = resource_type.replace("::", "/")
         return f"{METRIC_NAMESPACE_ROOT}/{suffix}"
 
 
+class HookMetricsPublisher(MetricsPublisher):
+    def __init__(self, session: SessionProxy, hook_type: str, account_id: str) -> None:
+        super().__init__(session, hook_type)
+        self._hook_type = hook_type
+        self._account_id = account_id
+        self._namespace = self._make_hook_namespace(hook_type, account_id)
+
+    # pylint: disable=arguments-differ
+    def publish_exception_metric(  # type: ignore
+        self,
+        timestamp: datetime.datetime,
+        invocation_point: HookInvocationPoint,
+        error: Any,
+    ) -> None:
+        dimensions: Mapping[str, str] = {
+            "DimensionKeyInvocationPointType": invocation_point.name,
+            "DimensionKeyExceptionType": str(type(error)),
+            "DimensionKeyHookType": self._hook_type,
+        }
+        self.publish_metric(
+            metric_name=MetricTypes.HandlerException,
+            dimensions=dimensions,
+            unit=StandardUnit.Count,
+            value=1.0,
+            timestamp=timestamp,
+        )
+
+    # pylint: disable=arguments-differ
+    def publish_invocation_metric(  # type: ignore
+        self, timestamp: datetime.datetime, invocation_point: HookInvocationPoint
+    ) -> None:
+        dimensions = {
+            "DimensionKeyInvocationPointType": invocation_point.name,
+            "DimensionKeyHookType": self._hook_type,
+        }
+        self.publish_metric(
+            metric_name=MetricTypes.HandlerInvocationCount,
+            dimensions=dimensions,
+            unit=StandardUnit.Count,
+            value=1.0,
+            timestamp=timestamp,
+        )
+
+    # pylint: disable=arguments-differ
+    def publish_duration_metric(  # type: ignore
+        self,
+        timestamp: datetime.datetime,
+        invocation_point: HookInvocationPoint,
+        milliseconds: float,
+    ) -> None:
+        dimensions = {
+            "DimensionKeyInvocationPointType": invocation_point.name,
+            "DimensionKeyHookType": self._hook_type,
+        }
+
+        self.publish_metric(
+            metric_name=MetricTypes.HandlerInvocationDuration,
+            dimensions=dimensions,
+            unit=StandardUnit.Milliseconds,
+            value=milliseconds,
+            timestamp=timestamp,
+        )
+
+    def publish_log_delivery_exception_metric(
+        self, timestamp: datetime.datetime, error: Any
+    ) -> None:
+        dimensions = {
+            "DimensionKeyInvocationPointType": "ProviderLogDelivery",
+            "DimensionKeyExceptionType": str(type(error)),
+            "DimensionKeyHookType": self._hook_type,
+        }
+        self.publish_metric(
+            metric_name=MetricTypes.HandlerException,
+            dimensions=dimensions,
+            unit=StandardUnit.Count,
+            value=1.0,
+            timestamp=timestamp,
+        )
+
+    @staticmethod
+    def _make_hook_namespace(hook_type: str, account_id: str) -> str:
+        suffix = hook_type.replace("::", "/")
+        return f"{METRIC_NAMESPACE_ROOT}/{account_id}/{suffix}"
+
+
 class MetricsPublisherProxy:
     """A proxy for publishing metrics to multiple publishers. \
     Iterates over available publishers and publishes.
 
     Functions:
     ----------
     add_metrics_publisher: Adds a metrics publisher to the list of publishers
@@ -160,30 +245,49 @@
     def add_metrics_publisher(
         self, session: Optional[SessionProxy], type_name: Optional[str]
     ) -> None:
         if session and type_name:
             publisher = MetricsPublisher(session, type_name)
             self._publishers.append(publisher)
 
+    def add_hook_metrics_publisher(
+        self,
+        session: Optional[SessionProxy],
+        type_name: Optional[str],
+        account_id: Optional[str],
+    ) -> None:
+        if session and type_name and account_id:
+            publisher = HookMetricsPublisher(session, type_name, account_id)
+            self._publishers.append(publisher)
+
     def publish_exception_metric(
-        self, timestamp: datetime.datetime, action: Action, error: Any
+        self,
+        timestamp: datetime.datetime,
+        action: Union[Action, HookInvocationPoint],
+        error: Any,
     ) -> None:
         for publisher in self._publishers:
-            publisher.publish_exception_metric(timestamp, action, error)
+            publisher.publish_exception_metric(timestamp, action, error)  # type: ignore
 
     def publish_invocation_metric(
-        self, timestamp: datetime.datetime, action: Action
+        self, timestamp: datetime.datetime, action: Union[Action, HookInvocationPoint]
     ) -> None:
         for publisher in self._publishers:
-            publisher.publish_invocation_metric(timestamp, action)
+            publisher.publish_invocation_metric(timestamp, action)  # type: ignore
 
+    # pylint: disable=line-too-long
     def publish_duration_metric(
-        self, timestamp: datetime.datetime, action: Action, milliseconds: float
+        self,
+        timestamp: datetime.datetime,
+        action: Union[Action, HookInvocationPoint],
+        milliseconds: float,
     ) -> None:
+        # fmt off
         for publisher in self._publishers:
-            publisher.publish_duration_metric(timestamp, action, milliseconds)
+            publisher.publish_duration_metric(timestamp, action, milliseconds)  # type: ignore
+        # fmt on
 
     def publish_log_delivery_exception_metric(
         self, timestamp: datetime.datetime, error: Any
     ) -> None:
         for publisher in self._publishers:
             publisher.publish_log_delivery_exception_metric(timestamp, error)
```

### Comparing `cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/recast.py` & `cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/recast.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import typing
 from typing import Any, Dict, List, Mapping, Set
 
 from .exceptions import InvalidRequest
 
 PRIMITIVES = (str, bool, int, float)
 
@@ -10,15 +11,15 @@
 # the types in the type hints
 def recast_object(
     cls: Any, json_data: Mapping[str, Any], classes: Dict[str, Any]
 ) -> None:
     if not isinstance(json_data, dict):
         raise InvalidRequest(f"Can only parse dict items, not {type(json_data)}")
     # if type is Any, we leave it as is
-    if cls == typing.Any:
+    if cls is typing.Any:
         return
     for k, v in json_data.items():
         if isinstance(v, dict):
             child_cls = _field_to_type(cls.__dataclass_fields__[k].type, k, classes)
             recast_object(child_cls, v, classes)
         elif isinstance(v, list):
             json_data[k] = _recast_lists(cls, k, v, classes)
@@ -31,15 +32,15 @@
             json_data[k] = _recast_primitive(dest_type, k, v)
         else:
             raise InvalidRequest(f"Unsupported type: {type(v)} for {k}")
 
 
 def _recast_lists(cls: Any, k: str, v: List[Any], classes: Dict[str, Any]) -> List[Any]:
     # Leave as is if type is Any
-    if cls == typing.Any:
+    if cls is typing.Any:
         return v
     if "__dataclass_fields__" not in dir(cls):
         pass
     elif k in cls.__dataclass_fields__:
         cls = _field_to_type(cls.__dataclass_fields__[k].type, k, classes)
     return [cast_sequence_item(cls, k, item, classes) for item in v]
 
@@ -60,15 +61,15 @@
     if isinstance(item, dict):
         recast_object(cls, item, classes)
         return item
     raise InvalidRequest(f"Unsupported type: {type(item)} for {k}")
 
 
 def _recast_primitive(cls: Any, k: str, v: Any) -> Any:
-    if cls == typing.Any:
+    if cls is typing.Any:
         # If the type is Any, we cannot guess what the original type was, so we leave
         # it as a string
         return v
     if cls == bool and isinstance(v, str):
         if v.lower() == "true":
             return True
         if v.lower() == "false":
@@ -122,10 +123,10 @@
 
 
 # pylint: disable=protected-access,no-member
 def get_forward_ref_type() -> Any:
     # ignoring mypy on the import as it catches (_)ForwardRef as invalid, use for
     # introspection is valid:
     # https://docs.python.org/3/library/typing.html#typing.ForwardRef
-    if "ForwardRef" in dir(typing):
-        return typing.ForwardRef  # type: ignore
-    return typing._ForwardRef  # type: ignore
+    if sys.version_info < (3, 7):
+        return typing._ForwardRef  # type: ignore
+    return typing.ForwardRef
```

### Comparing `cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib/resource.py` & `cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,10 +223,13 @@
         except Exception as e:  # pylint: disable=broad-except
             print_or_log("Exception caught {0}".format(e))
             progress = ProgressEvent.failed(HandlerErrorCode.InternalFailure)
         except BaseException as e:  # pylint: disable=broad-except
             print_or_log("Base exception caught (this is usually bad) {0}".format(e))
             progress = ProgressEvent.failed(HandlerErrorCode.InternalFailure)
 
+        if progress.result:
+            progress.result = None
+
         # use the raw event_data as a last-ditch attempt to call back if the
         # request is invalid
         return progress._serialize()  # pylint: disable=protected-access
```

### Comparing `cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib.egg-info/PKG-INFO` & `cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: cloudformation-cli-python-lib
-Version: 2.1.8
+Version: 2.1.9
 Summary: Support library to enable Python-based CloudFormation resource types
 Home-page: https://github.com/aws-cloudformation/aws-cloudformation-rpdk-python-plugin/
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
-Description: UNKNOWN
 Keywords: Amazon Web Services AWS CloudFormation
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `cloudformation-cli-python-lib-2.1.8/cloudformation_cli_python_lib.egg-info/SOURCES.txt` & `cloudformation-cli-python-lib-2.1.9/cloudformation_cli_python_lib.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+LICENSE
 MANIFEST.in
 setup.py
 ../LICENSE
 cloudformation_cli_python_lib/__init__.py
 cloudformation_cli_python_lib/boto3_proxy.py
+cloudformation_cli_python_lib/cipher.py
 cloudformation_cli_python_lib/exceptions.py
+cloudformation_cli_python_lib/hook.py
 cloudformation_cli_python_lib/identifier_utils.py
 cloudformation_cli_python_lib/interface.py
 cloudformation_cli_python_lib/log_delivery.py
 cloudformation_cli_python_lib/metrics.py
 cloudformation_cli_python_lib/py.typed
 cloudformation_cli_python_lib/recast.py
 cloudformation_cli_python_lib/resource.py
```

### Comparing `cloudformation-cli-python-lib-2.1.8/setup.py` & `cloudformation-cli-python-lib-2.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """Support library to enable Python-based CloudFormation resource types"""
 from setuptools import setup
 
 setup(
     name="cloudformation-cli-python-lib",
-    version="2.1.8",
+    version="2.1.9",
     description=__doc__,
     author="Amazon Web Services",
     author_email="aws-cloudformation-developers@amazon.com",
     url="https://github.com/aws-cloudformation/aws-cloudformation-rpdk-python-plugin/",
     packages=["cloudformation_cli_python_lib"],
     # package_data -> use MANIFEST.in instead
     include_package_data=True,
     zip_safe=True,
     python_requires=">=3.6",
-    install_requires=["boto3>=1.10.20", 'dataclasses;python_version<"3.7"'],
+    install_requires=[
+        "boto3>=1.10.20",
+        "aws-encryption-sdk==2.0.0",
+        'dataclasses;python_version<"3.7"',
+    ],
     license="Apache License 2.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Topic :: Software Development :: Build Tools",
```

