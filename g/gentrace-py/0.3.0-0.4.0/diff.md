# Comparing `tmp/gentrace_py-0.3.0.tar.gz` & `tmp/gentrace_py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentrace_py-0.3.0.tar", max compression
+gzip compressed data, was "gentrace_py-0.4.0.tar", max compression
```

## Comparing `gentrace_py-0.3.0.tar` & `gentrace_py-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0      899 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/__init__.py
--rw-r--r--   0        0        0    59420 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/api_client.py
--rw-r--r--   0        0        0      215 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/apis/__init__.py
--rw-r--r--   0        0        0      325 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/apis/paths/__init__.py
--rw-r--r--   0        0        0      105 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/apis/paths/pipeline_run.py
--rw-r--r--   0        0        0      459 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/apis/tag_to_api.py
--rw-r--r--   0        0        0      335 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/apis/tags/__init__.py
--rw-r--r--   0        0        0      485 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/apis/tags/ingestion_api.py
--rw-r--r--   0        0        0    15476 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/configuration.py
--rw-r--r--   0        0        0     4444 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/exceptions.py
--rw-r--r--   0        0        0      342 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/model/__init__.py
--rw-r--r--   0        0        0     5629 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/model/feedback_request.py
--rw-r--r--   0        0        0     5308 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/model/feedback_request.pyi
--rw-r--r--   0        0        0     2144 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/model/feedback_response.py
--rw-r--r--   0        0        0     2121 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/model/feedback_response.pyi
--rw-r--r--   0        0        0    32769 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/model/pipeline_run_request.py
--rw-r--r--   0        0        0    32179 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/model/pipeline_run_request.pyi
--rw-r--r--   0        0        0     2779 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/model/pipeline_run_response.py
--rw-r--r--   0        0        0     2739 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/model/pipeline_run_response.pyi
--rw-r--r--   0        0        0      640 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/models/__init__.py
--rw-r--r--   0        0        0      318 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/paths/__init__.py
--rw-r--r--   0        0        0      299 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/paths/pipeline_run/__init__.py
--rw-r--r--   0        0        0    12578 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/paths/pipeline_run/post.py
--rw-r--r--   0        0        0    12355 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/paths/pipeline_run/post.pyi
--rw-r--r--   0        0        0      153 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/providers/__init__.py
--rw-r--r--   0        0        0      182 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/providers/llms/__init__.py
--rw-r--r--   0        0        0    12220 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/providers/llms/openai.py
--rw-r--r--   0        0        0     2963 2023-04-16 14:36:37.448516 gentrace_py-0.3.0/gentrace/providers/pipeline.py
--rw-r--r--   0        0        0     6016 2023-04-16 14:36:37.452516 gentrace_py-0.3.0/gentrace/providers/pipeline_run.py
--rw-r--r--   0        0        0      531 2023-04-16 14:36:37.452516 gentrace_py-0.3.0/gentrace/providers/step_run.py
--rw-r--r--   0        0        0      690 2023-04-16 14:36:37.452516 gentrace_py-0.3.0/gentrace/providers/utils.py
--rw-r--r--   0        0        0      219 2023-04-16 14:36:37.452516 gentrace_py-0.3.0/gentrace/providers/vectorstores/__init__.py
--rw-r--r--   0        0        0    10432 2023-04-16 14:36:37.452516 gentrace_py-0.3.0/gentrace/providers/vectorstores/pinecone.py
--rw-r--r--   0        0        0    10398 2023-04-16 14:36:37.452516 gentrace_py-0.3.0/gentrace/rest.py
--rw-r--r--   0        0        0   103185 2023-04-16 14:36:37.452516 gentrace_py-0.3.0/gentrace/schemas.py
--rw-r--r--   0        0        0     1298 2023-04-16 14:36:37.452516 gentrace_py-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      980 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/__init__.py
+-rw-r--r--   0        0        0    59420 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/api_client.py
+-rw-r--r--   0        0        0      215 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/apis/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/apis/paths/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/apis/paths/pipeline_run.py
+-rw-r--r--   0        0        0      459 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/apis/tag_to_api.py
+-rw-r--r--   0        0        0      335 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/apis/tags/__init__.py
+-rw-r--r--   0        0        0      485 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/apis/tags/ingestion_api.py
+-rw-r--r--   0        0        0    15476 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/configuration.py
+-rw-r--r--   0        0        0     4444 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/exceptions.py
+-rw-r--r--   0        0        0      342 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/__init__.py
+-rw-r--r--   0        0        0     5209 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/feedback_request.py
+-rw-r--r--   0        0        0     4998 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/feedback_request.pyi
+-rw-r--r--   0        0        0     2144 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/feedback_response.py
+-rw-r--r--   0        0        0     2121 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/feedback_response.pyi
+-rw-r--r--   0        0        0    33338 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/pipeline_run_request.py
+-rw-r--r--   0        0        0    32730 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/pipeline_run_request.pyi
+-rw-r--r--   0        0        0     2779 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/pipeline_run_response.py
+-rw-r--r--   0        0        0     2739 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/model/pipeline_run_response.pyi
+-rw-r--r--   0        0        0      640 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/models/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/paths/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/paths/pipeline_run/__init__.py
+-rw-r--r--   0        0        0    12578 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/paths/pipeline_run/post.py
+-rw-r--r--   0        0        0    12355 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/paths/pipeline_run/post.pyi
+-rw-r--r--   0        0        0      202 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/__init__.py
+-rw-r--r--   0        0        0     3352 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/getters.py
+-rw-r--r--   0        0        0      182 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/llms/__init__.py
+-rw-r--r--   0        0        0    22046 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/llms/openai.py
+-rw-r--r--   0        0        0     3042 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/pipeline.py
+-rw-r--r--   0        0        0     6252 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/pipeline_run.py
+-rw-r--r--   0        0        0      531 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/step_run.py
+-rw-r--r--   0        0        0      695 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/utils.py
+-rw-r--r--   0        0        0      219 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/vectorstores/__init__.py
+-rw-r--r--   0        0        0    10432 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/providers/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    10398 2023-04-19 22:15:13.684094 gentrace_py-0.4.0/gentrace/rest.py
+-rw-r--r--   0        0        0   103185 2023-04-19 22:15:13.688094 gentrace_py-0.4.0/gentrace/schemas.py
+-rw-r--r--   0        0        0     1298 2023-04-19 22:15:13.688094 gentrace_py-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.4.0/PKG-INFO
```

### Comparing `gentrace_py-0.3.0/gentrace/__init__.py` & `gentrace_py-0.4.0/gentrace/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.6
     Generated by: https://openapi-generator.tech
 """
 
 __version__ = "1.0.0"
 
 # import ApiClient
 from gentrace.api_client import ApiClient
@@ -24,10 +24,15 @@
 from gentrace.exceptions import ApiAttributeError
 from gentrace.exceptions import ApiTypeError
 from gentrace.exceptions import ApiValueError
 from gentrace.exceptions import ApiKeyError
 from gentrace.exceptions import ApiException
 
 from gentrace.providers.pipeline import Pipeline
-from gentrace.providers.pipeline_run import PipelineRun
+from gentrace.providers.pipeline_run import PipelineRun, flush
 from gentrace.providers.step_run import StepRun
 from gentrace.providers.utils import to_date_string
+
+from gentrace.providers.getters import providers
+
+api_key = ""
+host = ""
```

### Comparing `gentrace_py-0.3.0/gentrace/api_client.py` & `gentrace_py-0.4.0/gentrace/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.6
     Generated by: https://openapi-generator.tech
 """
 
 import atexit
 import email
 import enum
 import io
```

### Comparing `gentrace_py-0.3.0/gentrace/configuration.py` & `gentrace_py-0.4.0/gentrace/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.6
     Generated by: https://openapi-generator.tech
 """
 
 import copy
 import logging
 import multiprocessing
 import sys
@@ -370,15 +370,15 @@
 
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
-            "Version of the API: 0.4.1\n"
+            "Version of the API: 0.4.6\n"
             "SDK Package Version: 1.0.0".format(env=sys.platform, pyversion=sys.version)
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `gentrace_py-0.3.0/gentrace/exceptions.py` & `gentrace_py-0.4.0/gentrace/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.6
     Generated by: https://openapi-generator.tech
 """
 import dataclasses
 import typing
 
 from urllib3._collections import HTTPHeaderDict
```

### Comparing `gentrace_py-0.3.0/gentrace/model/feedback_request.py` & `gentrace_py-0.4.0/gentrace/model/feedback_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.6
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
@@ -28,41 +28,27 @@
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     class MetaOapg:
         required = {
+            "score",
             "pipelineRunId",
-            "rating",
             "recordedTime",
         }
 
         class properties:
             pipelineRunId = schemas.UUIDSchema
 
-            class rating(schemas.EnumBase, schemas.StrSchema):
+            class score(schemas.Float32Schema):
                 class MetaOapg:
-                    enum_value_to_name = {
-                        "positive": "POSITIVE",
-                        "negative": "NEGATIVE",
-                        "neutral": "NEUTRAL",
-                    }
-
-                @schemas.classproperty
-                def POSITIVE(cls):
-                    return cls("positive")
-
-                @schemas.classproperty
-                def NEGATIVE(cls):
-                    return cls("negative")
-
-                @schemas.classproperty
-                def NEUTRAL(cls):
-                    return cls("neutral")
+                    format = "float"
+                    inclusive_maximum = 1
+                    inclusive_minimum = 0
 
             recordedTime = schemas.DateTimeSchema
 
             class details(
                 schemas.StrBase, schemas.NoneBase, schemas.Schema, schemas.NoneStrMixin
             ):
                 def __new__(
@@ -77,35 +63,35 @@
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
 
             __annotations__ = {
                 "pipelineRunId": pipelineRunId,
-                "rating": rating,
+                "score": score,
                 "recordedTime": recordedTime,
                 "details": details,
             }
 
         additional_properties = schemas.NotAnyTypeSchema
 
+    score: MetaOapg.properties.score
     pipelineRunId: MetaOapg.properties.pipelineRunId
-    rating: MetaOapg.properties.rating
     recordedTime: MetaOapg.properties.recordedTime
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["pipelineRunId"]
-    ) -> MetaOapg.properties.pipelineRunId:
+        self, name: typing_extensions.Literal["score"]
+    ) -> MetaOapg.properties.score:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["rating"]
-    ) -> MetaOapg.properties.rating:
+        self, name: typing_extensions.Literal["pipelineRunId"]
+    ) -> MetaOapg.properties.pipelineRunId:
         ...
 
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["recordedTime"]
     ) -> MetaOapg.properties.recordedTime:
         ...
@@ -115,33 +101,33 @@
         self, name: typing_extensions.Literal["details"]
     ) -> MetaOapg.properties.details:
         ...
 
     def __getitem__(
         self,
         name: typing.Union[
+            typing_extensions.Literal["score"],
             typing_extensions.Literal["pipelineRunId"],
-            typing_extensions.Literal["rating"],
             typing_extensions.Literal["recordedTime"],
             typing_extensions.Literal["details"],
         ],
     ):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["pipelineRunId"]
-    ) -> MetaOapg.properties.pipelineRunId:
+        self, name: typing_extensions.Literal["score"]
+    ) -> MetaOapg.properties.score:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["rating"]
-    ) -> MetaOapg.properties.rating:
+        self, name: typing_extensions.Literal["pipelineRunId"]
+    ) -> MetaOapg.properties.pipelineRunId:
         ...
 
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["recordedTime"]
     ) -> MetaOapg.properties.recordedTime:
         ...
@@ -151,49 +137,51 @@
         self, name: typing_extensions.Literal["details"]
     ) -> typing.Union[MetaOapg.properties.details, schemas.Unset]:
         ...
 
     def get_item_oapg(
         self,
         name: typing.Union[
+            typing_extensions.Literal["score"],
             typing_extensions.Literal["pipelineRunId"],
-            typing_extensions.Literal["rating"],
             typing_extensions.Literal["recordedTime"],
             typing_extensions.Literal["details"],
         ],
     ):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *_args: typing.Union[
             dict,
             frozendict.frozendict,
         ],
+        score: typing.Union[
+            MetaOapg.properties.score,
+            decimal.Decimal,
+            int,
+            float,
+        ],
         pipelineRunId: typing.Union[
             MetaOapg.properties.pipelineRunId,
             str,
             uuid.UUID,
         ],
-        rating: typing.Union[
-            MetaOapg.properties.rating,
-            str,
-        ],
         recordedTime: typing.Union[
             MetaOapg.properties.recordedTime,
             str,
             datetime,
         ],
         details: typing.Union[
             MetaOapg.properties.details, None, str, schemas.Unset
         ] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
     ) -> "FeedbackRequest":
         return super().__new__(
             cls,
             *_args,
+            score=score,
             pipelineRunId=pipelineRunId,
-            rating=rating,
             recordedTime=recordedTime,
             details=details,
             _configuration=_configuration,
         )
```

### Comparing `gentrace_py-0.3.0/gentrace/model/feedback_request.pyi` & `gentrace_py-0.4.0/gentrace/model/feedback_request.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.6
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
@@ -27,32 +27,24 @@
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     class MetaOapg:
         required = {
+            "score",
             "pipelineRunId",
-            "rating",
             "recordedTime",
         }
 
         class properties:
             pipelineRunId = schemas.UUIDSchema
 
-            class rating(schemas.EnumBase, schemas.StrSchema):
-                @schemas.classproperty
-                def POSITIVE(cls):
-                    return cls("positive")
-                @schemas.classproperty
-                def NEGATIVE(cls):
-                    return cls("negative")
-                @schemas.classproperty
-                def NEUTRAL(cls):
-                    return cls("neutral")
+            class score(schemas.Float32Schema):
+                pass
             recordedTime = schemas.DateTimeSchema
 
             class details(
                 schemas.StrBase, schemas.NoneBase, schemas.Schema, schemas.NoneStrMixin
             ):
                 def __new__(
                     cls,
@@ -65,103 +57,105 @@
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
             __annotations__ = {
                 "pipelineRunId": pipelineRunId,
-                "rating": rating,
+                "score": score,
                 "recordedTime": recordedTime,
                 "details": details,
             }
         additional_properties = schemas.NotAnyTypeSchema
+    score: MetaOapg.properties.score
     pipelineRunId: MetaOapg.properties.pipelineRunId
-    rating: MetaOapg.properties.rating
     recordedTime: MetaOapg.properties.recordedTime
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["pipelineRunId"]
-    ) -> MetaOapg.properties.pipelineRunId: ...
+        self, name: typing_extensions.Literal["score"]
+    ) -> MetaOapg.properties.score: ...
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["rating"]
-    ) -> MetaOapg.properties.rating: ...
+        self, name: typing_extensions.Literal["pipelineRunId"]
+    ) -> MetaOapg.properties.pipelineRunId: ...
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["recordedTime"]
     ) -> MetaOapg.properties.recordedTime: ...
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["details"]
     ) -> MetaOapg.properties.details: ...
     def __getitem__(
         self,
         name: typing.Union[
+            typing_extensions.Literal["score"],
             typing_extensions.Literal["pipelineRunId"],
-            typing_extensions.Literal["rating"],
             typing_extensions.Literal["recordedTime"],
             typing_extensions.Literal["details"],
         ],
     ):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["pipelineRunId"]
-    ) -> MetaOapg.properties.pipelineRunId: ...
+        self, name: typing_extensions.Literal["score"]
+    ) -> MetaOapg.properties.score: ...
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["rating"]
-    ) -> MetaOapg.properties.rating: ...
+        self, name: typing_extensions.Literal["pipelineRunId"]
+    ) -> MetaOapg.properties.pipelineRunId: ...
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["recordedTime"]
     ) -> MetaOapg.properties.recordedTime: ...
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["details"]
     ) -> typing.Union[MetaOapg.properties.details, schemas.Unset]: ...
     def get_item_oapg(
         self,
         name: typing.Union[
+            typing_extensions.Literal["score"],
             typing_extensions.Literal["pipelineRunId"],
-            typing_extensions.Literal["rating"],
             typing_extensions.Literal["recordedTime"],
             typing_extensions.Literal["details"],
         ],
     ):
         return super().get_item_oapg(name)
     def __new__(
         cls,
         *_args: typing.Union[
             dict,
             frozendict.frozendict,
         ],
+        score: typing.Union[
+            MetaOapg.properties.score,
+            decimal.Decimal,
+            int,
+            float,
+        ],
         pipelineRunId: typing.Union[
             MetaOapg.properties.pipelineRunId,
             str,
             uuid.UUID,
         ],
-        rating: typing.Union[
-            MetaOapg.properties.rating,
-            str,
-        ],
         recordedTime: typing.Union[
             MetaOapg.properties.recordedTime,
             str,
             datetime,
         ],
         details: typing.Union[
             MetaOapg.properties.details, None, str, schemas.Unset
         ] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
     ) -> "FeedbackRequest":
         return super().__new__(
             cls,
             *_args,
+            score=score,
             pipelineRunId=pipelineRunId,
-            rating=rating,
             recordedTime=recordedTime,
             details=details,
             _configuration=_configuration,
         )
```

### Comparing `gentrace_py-0.3.0/gentrace/model/feedback_response.py` & `gentrace_py-0.4.0/gentrace/model/feedback_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.6
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
```

### Comparing `gentrace_py-0.3.0/gentrace/model/feedback_response.pyi` & `gentrace_py-0.4.0/gentrace/model/feedback_response.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.6
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
```

### Comparing `gentrace_py-0.3.0/gentrace/model/pipeline_run_request.py` & `gentrace_py-0.4.0/gentrace/model/pipeline_run_request.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.6
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
@@ -18,29 +18,30 @@
 from datetime import date, datetime  # noqa: F401
 
 import frozendict  # noqa: F401
 import typing_extensions  # noqa: F401
 
 from gentrace import schemas  # noqa: F401
 
-
 class PipelineRunRequest(schemas.DictSchema):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     class MetaOapg:
         required = {
             "stepRuns",
             "name",
+            "id",
         }
 
         class properties:
+            id = schemas.UUIDSchema
             name = schemas.StrSchema
 
             class stepRuns(schemas.ListSchema):
                 class MetaOapg:
                     class items(schemas.DictSchema):
                         class MetaOapg:
                             class properties:
@@ -51,26 +52,23 @@
                                             invocation = schemas.StrSchema
 
                                             class modelParams(schemas.DictSchema):
                                                 class MetaOapg:
                                                     additional_properties = (
                                                         schemas.AnyTypeSchema
                                                     )
-
                                                 def __getitem__(
                                                     self, name: typing.Union[str,]
                                                 ) -> MetaOapg.additional_properties:
                                                     # dict_instance[name] accessor
                                                     return super().__getitem__(name)
-
                                                 def get_item_oapg(
                                                     self, name: typing.Union[str,]
                                                 ) -> MetaOapg.additional_properties:
                                                     return super().get_item_oapg(name)
-
                                                 def __new__(
                                                     cls,
                                                     *_args: typing.Union[
                                                         dict,
                                                         frozendict.frozendict,
                                                     ],
                                                     _configuration: typing.Optional[
@@ -104,26 +102,23 @@
                                                     )
 
                                             class inputs(schemas.DictSchema):
                                                 class MetaOapg:
                                                     additional_properties = (
                                                         schemas.AnyTypeSchema
                                                     )
-
                                                 def __getitem__(
                                                     self, name: typing.Union[str,]
                                                 ) -> MetaOapg.additional_properties:
                                                     # dict_instance[name] accessor
                                                     return super().__getitem__(name)
-
                                                 def get_item_oapg(
                                                     self, name: typing.Union[str,]
                                                 ) -> MetaOapg.additional_properties:
                                                     return super().get_item_oapg(name)
-
                                                 def __new__(
                                                     cls,
                                                     *_args: typing.Union[
                                                         dict,
                                                         frozendict.frozendict,
                                                     ],
                                                     _configuration: typing.Optional[
@@ -157,26 +152,23 @@
                                                     )
 
                                             class outputs(schemas.DictSchema):
                                                 class MetaOapg:
                                                     additional_properties = (
                                                         schemas.AnyTypeSchema
                                                     )
-
                                                 def __getitem__(
                                                     self, name: typing.Union[str,]
                                                 ) -> MetaOapg.additional_properties:
                                                     # dict_instance[name] accessor
                                                     return super().__getitem__(name)
-
                                                 def get_item_oapg(
                                                     self, name: typing.Union[str,]
                                                 ) -> MetaOapg.additional_properties:
                                                     return super().get_item_oapg(name)
-
                                                 def __new__(
                                                     cls,
                                                     *_args: typing.Union[
                                                         dict,
                                                         frozendict.frozendict,
                                                     ],
                                                     _configuration: typing.Optional[
@@ -204,61 +196,47 @@
                                                 ) -> "outputs":
                                                     return super().__new__(
                                                         cls,
                                                         *_args,
                                                         _configuration=_configuration,
                                                         **kwargs,
                                                     )
-
                                             __annotations__ = {
                                                 "name": name,
                                                 "invocation": invocation,
                                                 "modelParams": modelParams,
                                                 "inputs": inputs,
                                                 "outputs": outputs,
                                             }
-
                                     @typing.overload
                                     def __getitem__(
                                         self, name: typing_extensions.Literal["name"]
-                                    ) -> MetaOapg.properties.name:
-                                        ...
-
+                                    ) -> MetaOapg.properties.name: ...
                                     @typing.overload
                                     def __getitem__(
                                         self,
                                         name: typing_extensions.Literal["invocation"],
-                                    ) -> MetaOapg.properties.invocation:
-                                        ...
-
+                                    ) -> MetaOapg.properties.invocation: ...
                                     @typing.overload
                                     def __getitem__(
                                         self,
                                         name: typing_extensions.Literal["modelParams"],
-                                    ) -> MetaOapg.properties.modelParams:
-                                        ...
-
+                                    ) -> MetaOapg.properties.modelParams: ...
                                     @typing.overload
                                     def __getitem__(
                                         self, name: typing_extensions.Literal["inputs"]
-                                    ) -> MetaOapg.properties.inputs:
-                                        ...
-
+                                    ) -> MetaOapg.properties.inputs: ...
                                     @typing.overload
                                     def __getitem__(
                                         self, name: typing_extensions.Literal["outputs"]
-                                    ) -> MetaOapg.properties.outputs:
-                                        ...
-
+                                    ) -> MetaOapg.properties.outputs: ...
                                     @typing.overload
                                     def __getitem__(
                                         self, name: str
-                                    ) -> schemas.UnsetAnyTypeSchema:
-                                        ...
-
+                                    ) -> schemas.UnsetAnyTypeSchema: ...
                                     def __getitem__(
                                         self,
                                         name: typing.Union[
                                             typing_extensions.Literal[
                                                 "name",
                                                 "invocation",
                                                 "modelParams",
@@ -266,80 +244,66 @@
                                                 "outputs",
                                             ],
                                             str,
                                         ],
                                     ):
                                         # dict_instance[name] accessor
                                         return super().__getitem__(name)
-
                                     @typing.overload
                                     def get_item_oapg(
                                         self, name: typing_extensions.Literal["name"]
                                     ) -> typing.Union[
                                         MetaOapg.properties.name, schemas.Unset
-                                    ]:
-                                        ...
-
+                                    ]: ...
                                     @typing.overload
                                     def get_item_oapg(
                                         self,
                                         name: typing_extensions.Literal["invocation"],
                                     ) -> typing.Union[
                                         MetaOapg.properties.invocation, schemas.Unset
-                                    ]:
-                                        ...
-
+                                    ]: ...
                                     @typing.overload
                                     def get_item_oapg(
                                         self,
                                         name: typing_extensions.Literal["modelParams"],
                                     ) -> typing.Union[
                                         MetaOapg.properties.modelParams, schemas.Unset
-                                    ]:
-                                        ...
-
+                                    ]: ...
                                     @typing.overload
                                     def get_item_oapg(
                                         self, name: typing_extensions.Literal["inputs"]
                                     ) -> typing.Union[
                                         MetaOapg.properties.inputs, schemas.Unset
-                                    ]:
-                                        ...
-
+                                    ]: ...
                                     @typing.overload
                                     def get_item_oapg(
                                         self, name: typing_extensions.Literal["outputs"]
                                     ) -> typing.Union[
                                         MetaOapg.properties.outputs, schemas.Unset
-                                    ]:
-                                        ...
-
+                                    ]: ...
                                     @typing.overload
                                     def get_item_oapg(
                                         self, name: str
                                     ) -> typing.Union[
                                         schemas.UnsetAnyTypeSchema, schemas.Unset
-                                    ]:
-                                        ...
-
+                                    ]: ...
                                     def get_item_oapg(
                                         self,
                                         name: typing.Union[
                                             typing_extensions.Literal[
                                                 "name",
                                                 "invocation",
                                                 "modelParams",
                                                 "inputs",
                                                 "outputs",
                                             ],
                                             str,
                                         ],
                                     ):
                                         return super().get_item_oapg(name)
-
                                     def __new__(
                                         cls,
                                         *_args: typing.Union[
                                             dict,
                                             frozendict.frozendict,
                                         ],
                                         name: typing.Union[
@@ -395,114 +359,100 @@
                                             invocation=invocation,
                                             modelParams=modelParams,
                                             inputs=inputs,
                                             outputs=outputs,
                                             _configuration=_configuration,
                                             **kwargs,
                                         )
-
                                 elapsedTime = schemas.IntSchema
                                 startTime = schemas.DateTimeSchema
                                 endTime = schemas.DateTimeSchema
                                 __annotations__ = {
                                     "provider": provider,
                                     "elapsedTime": elapsedTime,
                                     "startTime": startTime,
                                     "endTime": endTime,
                                 }
-
                         @typing.overload
                         def __getitem__(
                             self, name: typing_extensions.Literal["provider"]
-                        ) -> MetaOapg.properties.provider:
-                            ...
-
+                        ) -> MetaOapg.properties.provider: ...
                         @typing.overload
                         def __getitem__(
                             self, name: typing_extensions.Literal["elapsedTime"]
-                        ) -> MetaOapg.properties.elapsedTime:
-                            ...
-
+                        ) -> MetaOapg.properties.elapsedTime: ...
                         @typing.overload
                         def __getitem__(
                             self, name: typing_extensions.Literal["startTime"]
-                        ) -> MetaOapg.properties.startTime:
-                            ...
-
+                        ) -> MetaOapg.properties.startTime: ...
                         @typing.overload
                         def __getitem__(
                             self, name: typing_extensions.Literal["endTime"]
-                        ) -> MetaOapg.properties.endTime:
-                            ...
-
+                        ) -> MetaOapg.properties.endTime: ...
                         @typing.overload
-                        def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
-                            ...
-
+                        def __getitem__(
+                            self, name: str
+                        ) -> schemas.UnsetAnyTypeSchema: ...
                         def __getitem__(
                             self,
                             name: typing.Union[
                                 typing_extensions.Literal[
                                     "provider",
                                     "elapsedTime",
                                     "startTime",
                                     "endTime",
                                 ],
                                 str,
                             ],
                         ):
                             # dict_instance[name] accessor
                             return super().__getitem__(name)
-
                         @typing.overload
                         def get_item_oapg(
                             self, name: typing_extensions.Literal["provider"]
-                        ) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]:
-                            ...
-
+                        ) -> typing.Union[
+                            MetaOapg.properties.provider, schemas.Unset
+                        ]: ...
                         @typing.overload
                         def get_item_oapg(
                             self, name: typing_extensions.Literal["elapsedTime"]
                         ) -> typing.Union[
                             MetaOapg.properties.elapsedTime, schemas.Unset
-                        ]:
-                            ...
-
+                        ]: ...
                         @typing.overload
                         def get_item_oapg(
                             self, name: typing_extensions.Literal["startTime"]
-                        ) -> typing.Union[MetaOapg.properties.startTime, schemas.Unset]:
-                            ...
-
+                        ) -> typing.Union[
+                            MetaOapg.properties.startTime, schemas.Unset
+                        ]: ...
                         @typing.overload
                         def get_item_oapg(
                             self, name: typing_extensions.Literal["endTime"]
-                        ) -> typing.Union[MetaOapg.properties.endTime, schemas.Unset]:
-                            ...
-
+                        ) -> typing.Union[
+                            MetaOapg.properties.endTime, schemas.Unset
+                        ]: ...
                         @typing.overload
                         def get_item_oapg(
                             self, name: str
-                        ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
-                            ...
-
+                        ) -> typing.Union[
+                            schemas.UnsetAnyTypeSchema, schemas.Unset
+                        ]: ...
                         def get_item_oapg(
                             self,
                             name: typing.Union[
                                 typing_extensions.Literal[
                                     "provider",
                                     "elapsedTime",
                                     "startTime",
                                     "endTime",
                                 ],
                                 str,
                             ],
                         ):
                             return super().get_item_oapg(name)
-
                         def __new__(
                             cls,
                             *_args: typing.Union[
                                 dict,
                                 frozendict.frozendict,
                             ],
                             provider: typing.Union[
@@ -555,15 +505,14 @@
                                 provider=provider,
                                 elapsedTime=elapsedTime,
                                 startTime=startTime,
                                 endTime=endTime,
                                 _configuration=_configuration,
                                 **kwargs,
                             )
-
                 def __new__(
                     cls,
                     _arg: typing.Union[
                         typing.Tuple[
                             typing.Union[
                                 MetaOapg.items,
                                 dict,
@@ -581,85 +530,80 @@
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> "stepRuns":
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
-
                 def __getitem__(self, i: int) -> MetaOapg.items:
                     return super().__getitem__(i)
-
             __annotations__ = {
+                "id": id,
                 "name": name,
                 "stepRuns": stepRuns,
             }
-
     stepRuns: MetaOapg.properties.stepRuns
     name: MetaOapg.properties.name
+    id: MetaOapg.properties.id
 
     @typing.overload
     def __getitem__(
+        self, name: typing_extensions.Literal["id"]
+    ) -> MetaOapg.properties.id: ...
+    @typing.overload
+    def __getitem__(
         self, name: typing_extensions.Literal["name"]
-    ) -> MetaOapg.properties.name:
-        ...
-
+    ) -> MetaOapg.properties.name: ...
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["stepRuns"]
-    ) -> MetaOapg.properties.stepRuns:
-        ...
-
+    ) -> MetaOapg.properties.stepRuns: ...
     @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
-        ...
-
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     def __getitem__(
         self,
         name: typing.Union[
             typing_extensions.Literal[
+                "id",
                 "name",
                 "stepRuns",
             ],
             str,
         ],
     ):
         # dict_instance[name] accessor
         return super().__getitem__(name)
-
+    @typing.overload
+    def get_item_oapg(
+        self, name: typing_extensions.Literal["id"]
+    ) -> MetaOapg.properties.id: ...
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["name"]
-    ) -> MetaOapg.properties.name:
-        ...
-
+    ) -> MetaOapg.properties.name: ...
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["stepRuns"]
-    ) -> MetaOapg.properties.stepRuns:
-        ...
-
+    ) -> MetaOapg.properties.stepRuns: ...
     @typing.overload
     def get_item_oapg(
         self, name: str
-    ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
-        ...
-
+    ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     def get_item_oapg(
         self,
         name: typing.Union[
             typing_extensions.Literal[
+                "id",
                 "name",
                 "stepRuns",
             ],
             str,
         ],
     ):
         return super().get_item_oapg(name)
-
     def __new__(
         cls,
         *_args: typing.Union[
             dict,
             frozendict.frozendict,
         ],
         stepRuns: typing.Union[
@@ -667,14 +611,19 @@
             list,
             tuple,
         ],
         name: typing.Union[
             MetaOapg.properties.name,
             str,
         ],
+        id: typing.Union[
+            MetaOapg.properties.id,
+            str,
+            uuid.UUID,
+        ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[
             schemas.AnyTypeSchema,
             dict,
             frozendict.frozendict,
             str,
             date,
@@ -690,10 +639,11 @@
         ],
     ) -> "PipelineRunRequest":
         return super().__new__(
             cls,
             *_args,
             stepRuns=stepRuns,
             name=name,
+            id=id,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `gentrace_py-0.3.0/gentrace/model/pipeline_run_request.pyi` & `gentrace_py-0.4.0/gentrace/model/pipeline_run_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.6
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
@@ -18,28 +18,31 @@
 from datetime import date, datetime  # noqa: F401
 
 import frozendict  # noqa: F401
 import typing_extensions  # noqa: F401
 
 from gentrace import schemas  # noqa: F401
 
+
 class PipelineRunRequest(schemas.DictSchema):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     class MetaOapg:
         required = {
             "stepRuns",
             "name",
+            "id",
         }
 
         class properties:
+            id = schemas.UUIDSchema
             name = schemas.StrSchema
 
             class stepRuns(schemas.ListSchema):
                 class MetaOapg:
                     class items(schemas.DictSchema):
                         class MetaOapg:
                             class properties:
@@ -50,23 +53,26 @@
                                             invocation = schemas.StrSchema
 
                                             class modelParams(schemas.DictSchema):
                                                 class MetaOapg:
                                                     additional_properties = (
                                                         schemas.AnyTypeSchema
                                                     )
+
                                                 def __getitem__(
                                                     self, name: typing.Union[str,]
                                                 ) -> MetaOapg.additional_properties:
                                                     # dict_instance[name] accessor
                                                     return super().__getitem__(name)
+
                                                 def get_item_oapg(
                                                     self, name: typing.Union[str,]
                                                 ) -> MetaOapg.additional_properties:
                                                     return super().get_item_oapg(name)
+
                                                 def __new__(
                                                     cls,
                                                     *_args: typing.Union[
                                                         dict,
                                                         frozendict.frozendict,
                                                     ],
                                                     _configuration: typing.Optional[
@@ -100,23 +106,26 @@
                                                     )
 
                                             class inputs(schemas.DictSchema):
                                                 class MetaOapg:
                                                     additional_properties = (
                                                         schemas.AnyTypeSchema
                                                     )
+
                                                 def __getitem__(
                                                     self, name: typing.Union[str,]
                                                 ) -> MetaOapg.additional_properties:
                                                     # dict_instance[name] accessor
                                                     return super().__getitem__(name)
+
                                                 def get_item_oapg(
                                                     self, name: typing.Union[str,]
                                                 ) -> MetaOapg.additional_properties:
                                                     return super().get_item_oapg(name)
+
                                                 def __new__(
                                                     cls,
                                                     *_args: typing.Union[
                                                         dict,
                                                         frozendict.frozendict,
                                                     ],
                                                     _configuration: typing.Optional[
@@ -150,23 +159,26 @@
                                                     )
 
                                             class outputs(schemas.DictSchema):
                                                 class MetaOapg:
                                                     additional_properties = (
                                                         schemas.AnyTypeSchema
                                                     )
+
                                                 def __getitem__(
                                                     self, name: typing.Union[str,]
                                                 ) -> MetaOapg.additional_properties:
                                                     # dict_instance[name] accessor
                                                     return super().__getitem__(name)
+
                                                 def get_item_oapg(
                                                     self, name: typing.Union[str,]
                                                 ) -> MetaOapg.additional_properties:
                                                     return super().get_item_oapg(name)
+
                                                 def __new__(
                                                     cls,
                                                     *_args: typing.Union[
                                                         dict,
                                                         frozendict.frozendict,
                                                     ],
                                                     _configuration: typing.Optional[
@@ -194,47 +206,61 @@
                                                 ) -> "outputs":
                                                     return super().__new__(
                                                         cls,
                                                         *_args,
                                                         _configuration=_configuration,
                                                         **kwargs,
                                                     )
+
                                             __annotations__ = {
                                                 "name": name,
                                                 "invocation": invocation,
                                                 "modelParams": modelParams,
                                                 "inputs": inputs,
                                                 "outputs": outputs,
                                             }
+
                                     @typing.overload
                                     def __getitem__(
                                         self, name: typing_extensions.Literal["name"]
-                                    ) -> MetaOapg.properties.name: ...
+                                    ) -> MetaOapg.properties.name:
+                                        ...
+
                                     @typing.overload
                                     def __getitem__(
                                         self,
                                         name: typing_extensions.Literal["invocation"],
-                                    ) -> MetaOapg.properties.invocation: ...
+                                    ) -> MetaOapg.properties.invocation:
+                                        ...
+
                                     @typing.overload
                                     def __getitem__(
                                         self,
                                         name: typing_extensions.Literal["modelParams"],
-                                    ) -> MetaOapg.properties.modelParams: ...
+                                    ) -> MetaOapg.properties.modelParams:
+                                        ...
+
                                     @typing.overload
                                     def __getitem__(
                                         self, name: typing_extensions.Literal["inputs"]
-                                    ) -> MetaOapg.properties.inputs: ...
+                                    ) -> MetaOapg.properties.inputs:
+                                        ...
+
                                     @typing.overload
                                     def __getitem__(
                                         self, name: typing_extensions.Literal["outputs"]
-                                    ) -> MetaOapg.properties.outputs: ...
+                                    ) -> MetaOapg.properties.outputs:
+                                        ...
+
                                     @typing.overload
                                     def __getitem__(
                                         self, name: str
-                                    ) -> schemas.UnsetAnyTypeSchema: ...
+                                    ) -> schemas.UnsetAnyTypeSchema:
+                                        ...
+
                                     def __getitem__(
                                         self,
                                         name: typing.Union[
                                             typing_extensions.Literal[
                                                 "name",
                                                 "invocation",
                                                 "modelParams",
@@ -242,66 +268,80 @@
                                                 "outputs",
                                             ],
                                             str,
                                         ],
                                     ):
                                         # dict_instance[name] accessor
                                         return super().__getitem__(name)
+
                                     @typing.overload
                                     def get_item_oapg(
                                         self, name: typing_extensions.Literal["name"]
                                     ) -> typing.Union[
                                         MetaOapg.properties.name, schemas.Unset
-                                    ]: ...
+                                    ]:
+                                        ...
+
                                     @typing.overload
                                     def get_item_oapg(
                                         self,
                                         name: typing_extensions.Literal["invocation"],
                                     ) -> typing.Union[
                                         MetaOapg.properties.invocation, schemas.Unset
-                                    ]: ...
+                                    ]:
+                                        ...
+
                                     @typing.overload
                                     def get_item_oapg(
                                         self,
                                         name: typing_extensions.Literal["modelParams"],
                                     ) -> typing.Union[
                                         MetaOapg.properties.modelParams, schemas.Unset
-                                    ]: ...
+                                    ]:
+                                        ...
+
                                     @typing.overload
                                     def get_item_oapg(
                                         self, name: typing_extensions.Literal["inputs"]
                                     ) -> typing.Union[
                                         MetaOapg.properties.inputs, schemas.Unset
-                                    ]: ...
+                                    ]:
+                                        ...
+
                                     @typing.overload
                                     def get_item_oapg(
                                         self, name: typing_extensions.Literal["outputs"]
                                     ) -> typing.Union[
                                         MetaOapg.properties.outputs, schemas.Unset
-                                    ]: ...
+                                    ]:
+                                        ...
+
                                     @typing.overload
                                     def get_item_oapg(
                                         self, name: str
                                     ) -> typing.Union[
                                         schemas.UnsetAnyTypeSchema, schemas.Unset
-                                    ]: ...
+                                    ]:
+                                        ...
+
                                     def get_item_oapg(
                                         self,
                                         name: typing.Union[
                                             typing_extensions.Literal[
                                                 "name",
                                                 "invocation",
                                                 "modelParams",
                                                 "inputs",
                                                 "outputs",
                                             ],
                                             str,
                                         ],
                                     ):
                                         return super().get_item_oapg(name)
+
                                     def __new__(
                                         cls,
                                         *_args: typing.Union[
                                             dict,
                                             frozendict.frozendict,
                                         ],
                                         name: typing.Union[
@@ -357,100 +397,114 @@
                                             invocation=invocation,
                                             modelParams=modelParams,
                                             inputs=inputs,
                                             outputs=outputs,
                                             _configuration=_configuration,
                                             **kwargs,
                                         )
+
                                 elapsedTime = schemas.IntSchema
                                 startTime = schemas.DateTimeSchema
                                 endTime = schemas.DateTimeSchema
                                 __annotations__ = {
                                     "provider": provider,
                                     "elapsedTime": elapsedTime,
                                     "startTime": startTime,
                                     "endTime": endTime,
                                 }
+
                         @typing.overload
                         def __getitem__(
                             self, name: typing_extensions.Literal["provider"]
-                        ) -> MetaOapg.properties.provider: ...
+                        ) -> MetaOapg.properties.provider:
+                            ...
+
                         @typing.overload
                         def __getitem__(
                             self, name: typing_extensions.Literal["elapsedTime"]
-                        ) -> MetaOapg.properties.elapsedTime: ...
+                        ) -> MetaOapg.properties.elapsedTime:
+                            ...
+
                         @typing.overload
                         def __getitem__(
                             self, name: typing_extensions.Literal["startTime"]
-                        ) -> MetaOapg.properties.startTime: ...
+                        ) -> MetaOapg.properties.startTime:
+                            ...
+
                         @typing.overload
                         def __getitem__(
                             self, name: typing_extensions.Literal["endTime"]
-                        ) -> MetaOapg.properties.endTime: ...
+                        ) -> MetaOapg.properties.endTime:
+                            ...
+
                         @typing.overload
-                        def __getitem__(
-                            self, name: str
-                        ) -> schemas.UnsetAnyTypeSchema: ...
+                        def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
+                            ...
+
                         def __getitem__(
                             self,
                             name: typing.Union[
                                 typing_extensions.Literal[
                                     "provider",
                                     "elapsedTime",
                                     "startTime",
                                     "endTime",
                                 ],
                                 str,
                             ],
                         ):
                             # dict_instance[name] accessor
                             return super().__getitem__(name)
+
                         @typing.overload
                         def get_item_oapg(
                             self, name: typing_extensions.Literal["provider"]
-                        ) -> typing.Union[
-                            MetaOapg.properties.provider, schemas.Unset
-                        ]: ...
+                        ) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]:
+                            ...
+
                         @typing.overload
                         def get_item_oapg(
                             self, name: typing_extensions.Literal["elapsedTime"]
                         ) -> typing.Union[
                             MetaOapg.properties.elapsedTime, schemas.Unset
-                        ]: ...
+                        ]:
+                            ...
+
                         @typing.overload
                         def get_item_oapg(
                             self, name: typing_extensions.Literal["startTime"]
-                        ) -> typing.Union[
-                            MetaOapg.properties.startTime, schemas.Unset
-                        ]: ...
+                        ) -> typing.Union[MetaOapg.properties.startTime, schemas.Unset]:
+                            ...
+
                         @typing.overload
                         def get_item_oapg(
                             self, name: typing_extensions.Literal["endTime"]
-                        ) -> typing.Union[
-                            MetaOapg.properties.endTime, schemas.Unset
-                        ]: ...
+                        ) -> typing.Union[MetaOapg.properties.endTime, schemas.Unset]:
+                            ...
+
                         @typing.overload
                         def get_item_oapg(
                             self, name: str
-                        ) -> typing.Union[
-                            schemas.UnsetAnyTypeSchema, schemas.Unset
-                        ]: ...
+                        ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
+                            ...
+
                         def get_item_oapg(
                             self,
                             name: typing.Union[
                                 typing_extensions.Literal[
                                     "provider",
                                     "elapsedTime",
                                     "startTime",
                                     "endTime",
                                 ],
                                 str,
                             ],
                         ):
                             return super().get_item_oapg(name)
+
                         def __new__(
                             cls,
                             *_args: typing.Union[
                                 dict,
                                 frozendict.frozendict,
                             ],
                             provider: typing.Union[
@@ -503,14 +557,15 @@
                                 provider=provider,
                                 elapsedTime=elapsedTime,
                                 startTime=startTime,
                                 endTime=endTime,
                                 _configuration=_configuration,
                                 **kwargs,
                             )
+
                 def __new__(
                     cls,
                     _arg: typing.Union[
                         typing.Tuple[
                             typing.Union[
                                 MetaOapg.items,
                                 dict,
@@ -528,68 +583,101 @@
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> "stepRuns":
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
+
                 def __getitem__(self, i: int) -> MetaOapg.items:
                     return super().__getitem__(i)
+
             __annotations__ = {
+                "id": id,
                 "name": name,
                 "stepRuns": stepRuns,
             }
+
     stepRuns: MetaOapg.properties.stepRuns
     name: MetaOapg.properties.name
+    id: MetaOapg.properties.id
+
+    @typing.overload
+    def __getitem__(
+        self, name: typing_extensions.Literal["id"]
+    ) -> MetaOapg.properties.id:
+        ...
 
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["name"]
-    ) -> MetaOapg.properties.name: ...
+    ) -> MetaOapg.properties.name:
+        ...
+
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["stepRuns"]
-    ) -> MetaOapg.properties.stepRuns: ...
+    ) -> MetaOapg.properties.stepRuns:
+        ...
+
     @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
+        ...
+
     def __getitem__(
         self,
         name: typing.Union[
             typing_extensions.Literal[
+                "id",
                 "name",
                 "stepRuns",
             ],
             str,
         ],
     ):
         # dict_instance[name] accessor
         return super().__getitem__(name)
+
+    @typing.overload
+    def get_item_oapg(
+        self, name: typing_extensions.Literal["id"]
+    ) -> MetaOapg.properties.id:
+        ...
+
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["name"]
-    ) -> MetaOapg.properties.name: ...
+    ) -> MetaOapg.properties.name:
+        ...
+
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["stepRuns"]
-    ) -> MetaOapg.properties.stepRuns: ...
+    ) -> MetaOapg.properties.stepRuns:
+        ...
+
     @typing.overload
     def get_item_oapg(
         self, name: str
-    ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
+        ...
+
     def get_item_oapg(
         self,
         name: typing.Union[
             typing_extensions.Literal[
+                "id",
                 "name",
                 "stepRuns",
             ],
             str,
         ],
     ):
         return super().get_item_oapg(name)
+
     def __new__(
         cls,
         *_args: typing.Union[
             dict,
             frozendict.frozendict,
         ],
         stepRuns: typing.Union[
@@ -597,14 +685,19 @@
             list,
             tuple,
         ],
         name: typing.Union[
             MetaOapg.properties.name,
             str,
         ],
+        id: typing.Union[
+            MetaOapg.properties.id,
+            str,
+            uuid.UUID,
+        ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[
             schemas.AnyTypeSchema,
             dict,
             frozendict.frozendict,
             str,
             date,
@@ -620,10 +713,11 @@
         ],
     ) -> "PipelineRunRequest":
         return super().__new__(
             cls,
             *_args,
             stepRuns=stepRuns,
             name=name,
+            id=id,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `gentrace_py-0.3.0/gentrace/model/pipeline_run_response.py` & `gentrace_py-0.4.0/gentrace/model/pipeline_run_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.6
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
```

### Comparing `gentrace_py-0.3.0/gentrace/model/pipeline_run_response.pyi` & `gentrace_py-0.4.0/gentrace/model/pipeline_run_response.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.6
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
```

### Comparing `gentrace_py-0.3.0/gentrace/models/__init__.py` & `gentrace_py-0.4.0/gentrace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.3.0/gentrace/paths/pipeline_run/post.py` & `gentrace_py-0.4.0/gentrace/paths/pipeline_run/post.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.3.0/gentrace/paths/pipeline_run/post.pyi` & `gentrace_py-0.4.0/gentrace/paths/pipeline_run/post.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.3.0/gentrace/providers/pipeline.py` & `gentrace_py-0.4.0/gentrace/providers/pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import inspect
 from typing import Any, Optional
 
-from gentrace.providers.pipeline_run import PipelineRun
-
 
 class Pipeline:
     def __init__(
         self,
         id: str,
         api_key: str,
         host: Optional[str] = None,
@@ -73,16 +71,20 @@
                 )
 
         if self.openai_config:
             try:
                 from gentrace.providers.llms.openai import OpenAIPipelineHandler
 
                 OpenAIPipelineHandler.setup(self.openai_config)
-                openai_handler = OpenAIPipelineHandler(pipeline=self)
+                openai_handler = OpenAIPipelineHandler(
+                    self.config, self.openai_config, pipeline=self
+                )
                 self.pipeline_handlers["openai"] = openai_handler
             except ImportError:
                 raise ImportError(
                     "Please install OpenAI as a dependency with, e.g. `pip install openai`"
                 )
 
     def start(self):
+        from gentrace.providers.pipeline_run import PipelineRun
+
         return PipelineRun(pipeline=self)
```

### Comparing `gentrace_py-0.3.0/gentrace/providers/pipeline_run.py` & `gentrace_py-0.4.0/gentrace/providers/pipeline_run.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,69 @@
+import asyncio
+import concurrent
 import copy
-import json
-from typing import Dict, List, Type, Union, cast
+import inspect
+import threading
+import uuid
+from typing import Dict, List, cast
 
 from gentrace.api_client import ApiClient
 from gentrace.apis.tags.ingestion_api import IngestionApi
 from gentrace.configuration import Configuration
-from gentrace.providers.llms.openai import OpenAIPipelineHandler
+from gentrace.providers.pipeline import Pipeline
 from gentrace.providers.step_run import StepRun
-from gentrace.providers.utils import pipeline_run_post_async
+from gentrace.providers.utils import pipeline_run_post_background
+
+_pipeline_run_loop = None
+_pipeline_tasks = []
+
+
+# https://stackoverflow.com/a/63110035/1057411
+def fire_and_forget(coro):
+    global _pipeline_run_loop, _pipeline_tasks
+    if _pipeline_run_loop is None:
+        _pipeline_run_loop = asyncio.new_event_loop()
+        threading.Thread(target=_pipeline_run_loop.run_forever, daemon=True).start()
+    if inspect.iscoroutine(coro):
+        task = asyncio.run_coroutine_threadsafe(coro, _pipeline_run_loop)
+        _pipeline_tasks.append(task)
+
+
+def flush():
+    global _pipeline_tasks
+    if _pipeline_tasks:
+        # Wait for all tasks to complete
+        concurrent.futures.wait(_pipeline_tasks)
+        _pipeline_tasks.clear()
 
 
 class PipelineRun:
     def __init__(self, pipeline):
-        self.pipeline = pipeline
+        self.pipeline: Pipeline = pipeline
         self.step_runs: List[StepRun] = []
 
     def get_pipeline(self):
         return self.pipeline
 
     def get_openai(self):
         if "openai" in self.pipeline.pipeline_handlers:
             handler = self.pipeline.pipeline_handlers.get("openai")
             cloned_handler = copy.deepcopy(handler)
-            import openai
-
-            from .llms.openai import (
-                intercept_chat_completion,
-                intercept_chat_completion_async,
-                intercept_completion,
-                intercept_completion_async,
-                intercept_embedding,
-                intercept_embedding_async,
-            )
-
-            for name, cls in vars(openai.api_resources).items():
-                if isinstance(cls, type):
-                    # Create new class that inherits from the original class, don't directly monkey patch
-                    # the original class
-                    new_class = type(name, (cls,), {})
-                    if name == "Completion":
-                        new_class.create = intercept_completion(new_class.create)
-                        new_class.acreate = intercept_completion_async(
-                            new_class.acreate
-                        )
-                    elif name == "ChatCompletion":
-                        new_class.create = intercept_chat_completion(new_class.create)
-                        new_class.acreate = intercept_chat_completion_async(
-                            new_class.acreate
-                        )
-                    elif name == "Embedding":
-                        new_class.create = intercept_embedding(new_class.create)
-                        new_class.acreate = intercept_embedding_async(new_class.acreate)
 
-                    new_class.pipeline_run = self
+            from .llms.openai import annotate_pipeline_handler
 
-                    setattr(cloned_handler, name, new_class)
+            annotated_handler = annotate_pipeline_handler(
+                cloned_handler, self.pipeline.openai_config, self
+            )
 
-            cloned_handler.set_pipeline_run(self)
+            import openai
 
             # TODO: Could not find an easy way to create a union type with openai and
             # OpenAIPipelineHandler, so we just use openai.
-            typed_cloned_handler = cast(openai, cloned_handler)
+            typed_cloned_handler = cast(openai, annotated_handler)
 
             return typed_cloned_handler
         else:
             raise ValueError(
                 "Did not find OpenAI handler. Did you call setup() on the pipeline?"
             )
 
@@ -102,28 +101,35 @@
                 "elapsedTime": step_run.elapsed_time,
                 "startTime": step_run.start_time,
                 "endTime": step_run.end_time,
             }
             for step_run in self.step_runs
         ]
 
+        pipeline_run_id = str(uuid.uuid4())
+
         try:
-            pipeline_post_response = await pipeline_run_post_async(
-                ingestion_api, {"name": self.pipeline.id, "stepRuns": step_runs_data}
+            pipeline_post_response = await pipeline_run_post_background(
+                ingestion_api,
+                {
+                    "id": pipeline_run_id,
+                    "name": self.pipeline.id,
+                    "stepRuns": step_runs_data,
+                },
             )
             return {
                 "pipelineRunId": pipeline_post_response.body.get_item_oapg(
                     "pipelineRunId"
                 )
             }
         except Exception as e:
             print(f"Error submitting to Gentrace: {e}")
             return {"pipelineRunId": None}
 
-    def submit(self) -> Dict:
+    def submit(self, wait_for_server=False) -> Dict:
         configuration = Configuration(host=self.pipeline.config.get("host"))
         configuration.access_token = self.pipeline.config.get("api_key")
         api_client = ApiClient(configuration=configuration)
         ingestion_api = IngestionApi(api_client=api_client)
 
         step_runs_data = [
             {
@@ -137,20 +143,41 @@
                 "elapsedTime": step_run.elapsed_time,
                 "startTime": step_run.start_time,
                 "endTime": step_run.end_time,
             }
             for step_run in self.step_runs
         ]
 
-        try:
-            pipeline_post_response = ingestion_api.pipeline_run_post(
-                {"name": self.pipeline.id, "stepRuns": step_runs_data}
-            )
-            return {
-                "pipelineRunId": pipeline_post_response.body.get_item_oapg(
-                    "pipelineRunId"
+        pipeline_run_id = str(uuid.uuid4())
+
+        if not wait_for_server:
+            fire_and_forget(
+                pipeline_run_post_background(
+                    ingestion_api,
+                    {
+                        "id": pipeline_run_id,
+                        "name": self.pipeline.id,
+                        "stepRuns": step_runs_data,
+                    },
                 )
-            }
+            )
 
-        except Exception as e:
-            print(f"Error submitting to Gentrace: {e}")
-            return {"pipelineRunId": None}
+            return {"pipelineRunId": pipeline_run_id}
+
+        if wait_for_server:
+            try:
+                pipeline_post_response = ingestion_api.pipeline_run_post(
+                    {
+                        "id": pipeline_run_id,
+                        "name": self.pipeline.id,
+                        "stepRuns": step_runs_data,
+                    }
+                )
+                return {
+                    "pipelineRunId": pipeline_post_response.body.get_item_oapg(
+                        "pipelineRunId"
+                    )
+                }
+
+            except Exception as e:
+                print(f"Error submitting to Gentrace: {e}")
+                return {"pipelineRunId": None}
```

### Comparing `gentrace_py-0.3.0/gentrace/providers/step_run.py` & `gentrace_py-0.4.0/gentrace/providers/step_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.3.0/gentrace/providers/utils.py` & `gentrace_py-0.4.0/gentrace/providers/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def to_date_string(time_value):
     return (
         datetime.fromtimestamp(time_value).strftime("%Y-%m-%dT%H:%M:%S.%fZ")[:-4] + "Z"
     )
 
 
-async def pipeline_run_post_async(
+async def pipeline_run_post_background(
     api_instance: IngestionApi, pipeline_run_data: PipelineRunRequest
 ):
     with ThreadPoolExecutor() as executor:
         result = await asyncio.get_event_loop().run_in_executor(
             executor, api_instance.pipeline_run_post, pipeline_run_data
         )
     return result
```

### Comparing `gentrace_py-0.3.0/gentrace/providers/vectorstores/pinecone.py` & `gentrace_py-0.4.0/gentrace/providers/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.3.0/gentrace/rest.py` & `gentrace_py-0.4.0/gentrace/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.6
     Generated by: https://openapi-generator.tech
 """
 
 import logging
 import ssl
 import typing
 from urllib.parse import urlencode
```

### Comparing `gentrace_py-0.3.0/gentrace/schemas.py` & `gentrace_py-0.4.0/gentrace/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.6
     Generated by: https://openapi-generator.tech
 """
 
 import decimal
 import functools
 import io
 import re
```

### Comparing `gentrace_py-0.3.0/pyproject.toml` & `gentrace_py-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Python SDK for the Gentrace API"
 license = "MIT"
 name = "gentrace-py"
 packages = [
   {include = "gentrace"},
 ]
 repository = "https://github.com/gentrace/gentrace-python"
-version = "0.3.0"
+version = "0.4.0"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 frozendict = "^2.3.7"
 pydantic = ">=1.10.2"
 pystache = "^0.6.0"
 python = ">=3.8.1,<4.0"
```

### Comparing `gentrace_py-0.3.0/PKG-INFO` & `gentrace_py-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentrace-py
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python SDK for the Gentrace API
 Home-page: https://github.com/gentrace/gentrace-python
 License: MIT
 Author: Gentrace
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

