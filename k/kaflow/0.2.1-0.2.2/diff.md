# Comparing `tmp/kaflow-0.2.1.tar.gz` & `tmp/kaflow-0.2.2.tar.gz`

## Comparing `kaflow-0.2.1.tar` & `kaflow-0.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kaflow-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 kaflow-0.2.1/Makefile
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kaflow-0.2.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 kaflow-0.2.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/__init__.py
--rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/_consumer.py
--rw-r--r--   0        0        0    22216 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/applications.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/dependencies.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/exceptions.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/logger.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/message.py
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/py.typed
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/serializers.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/testclient.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/_utils/__init__.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/_utils/asyncio.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/_utils/inspect.py
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/_utils/overrides.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/asyncapi/__init__.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/asyncapi/_builder.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/asyncapi/docs.py
--rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 kaflow-0.2.1/kaflow/asyncapi/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kaflow-0.2.1/tests/key_value.proto
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 kaflow-0.2.1/tests/key_value_pb2.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 kaflow-0.2.1/tests/key_value_pb2.pyi
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 kaflow-0.2.1/tests/test_application.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 kaflow-0.2.1/tests/test_serializers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.1/tests/_utils/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 kaflow-0.2.1/tests/_utils/test_asyncio.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 kaflow-0.2.1/tests/_utils/test_inspect.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 kaflow-0.2.1/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 kaflow-0.2.1/LICENSE
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 kaflow-0.2.1/README.md
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 kaflow-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 kaflow-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kaflow-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 kaflow-0.2.2/Makefile
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kaflow-0.2.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 kaflow-0.2.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/__init__.py
+-rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/_consumer.py
+-rw-r--r--   0        0        0    22216 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/applications.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/dependencies.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/exceptions.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/logger.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/message.py
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/py.typed
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/serializers.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/testclient.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/_utils/__init__.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/_utils/asyncio.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/_utils/inspect.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/_utils/overrides.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/asyncapi/__init__.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/asyncapi/_builder.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/asyncapi/docs.py
+-rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 kaflow-0.2.2/kaflow/asyncapi/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kaflow-0.2.2/tests/key_value.proto
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 kaflow-0.2.2/tests/key_value_pb2.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 kaflow-0.2.2/tests/key_value_pb2.pyi
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 kaflow-0.2.2/tests/test_application.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 kaflow-0.2.2/tests/test_serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.2.2/tests/_utils/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 kaflow-0.2.2/tests/_utils/test_asyncio.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 kaflow-0.2.2/tests/_utils/test_inspect.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 kaflow-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 kaflow-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 kaflow-0.2.2/README.md
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 kaflow-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 kaflow-0.2.2/PKG-INFO
```

### Comparing `kaflow-0.2.1/.github/workflows/release.yaml` & `kaflow-0.2.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/.github/workflows/test.yaml` & `kaflow-0.2.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/kaflow/__init__.py` & `kaflow-0.2.2/kaflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,8 @@
     __all__.append("Avro")
 
 if has_protobuf:
     from kaflow.serializers import Protobuf  # noqa: F401
 
     __all__.append("Protobuf")
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

### Comparing `kaflow-0.2.1/kaflow/_consumer.py` & `kaflow-0.2.2/kaflow/_consumer.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/kaflow/applications.py` & `kaflow-0.2.2/kaflow/applications.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/kaflow/message.py` & `kaflow-0.2.2/kaflow/message.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/kaflow/parameters.py` & `kaflow-0.2.2/kaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/kaflow/serializers.py` & `kaflow-0.2.2/kaflow/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             return bytes_io.getvalue()
 
         def deserialize(self, data: bytes) -> Any:
             bytes_io = io.BytesIO(data)
             if self.seek_offset is not None:
                 bytes_io.seek(self.seek_offset)
             if self.avro_schema:
-                return fastavro.schemaless_reader(io.BytesIO(data), self.avro_schema)
+                return fastavro.schemaless_reader(bytes_io, self.avro_schema)
             return list(fastavro.reader(bytes_io))[0]
 
         @staticmethod
         def extra_annotations_keys() -> list[str]:
             return ["avro_schema"]
 
     Avro = Annotated[T, AvroSerializer, MESSAGE_SERIALIZER_FLAG]
```

### Comparing `kaflow-0.2.1/kaflow/testclient.py` & `kaflow-0.2.2/kaflow/testclient.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/kaflow/_utils/asyncio.py` & `kaflow-0.2.2/kaflow/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/kaflow/_utils/inspect.py` & `kaflow-0.2.2/kaflow/_utils/inspect.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/kaflow/_utils/overrides.py` & `kaflow-0.2.2/kaflow/_utils/overrides.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/kaflow/asyncapi/_builder.py` & `kaflow-0.2.2/kaflow/asyncapi/_builder.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/kaflow/asyncapi/docs.py` & `kaflow-0.2.2/kaflow/asyncapi/docs.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/kaflow/asyncapi/models.py` & `kaflow-0.2.2/kaflow/asyncapi/models.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/tests/key_value_pb2.py` & `kaflow-0.2.2/tests/key_value_pb2.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/tests/test_serializers.py` & `kaflow-0.2.2/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/tests/_utils/test_inspect.py` & `kaflow-0.2.2/tests/_utils/test_inspect.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/.gitignore` & `kaflow-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/LICENSE` & `kaflow-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/README.md` & `kaflow-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/pyproject.toml` & `kaflow-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kaflow-0.2.1/PKG-INFO` & `kaflow-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaflow
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Stream processing backed by Apache Kafka.
 Project-URL: Documentation, https://github.com/gabrielmbmb/kaflow#readme
 Project-URL: Issues, https://github.com/gabrielmbmb/kaflow/issues
 Project-URL: Source, https://github.com/gabrielmbmb/kaflow
 Author-email: Gabriel Martin Blazquez <gmartinbdev@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

