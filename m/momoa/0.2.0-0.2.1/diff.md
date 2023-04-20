# Comparing `tmp/momoa-0.2.0.tar.gz` & `tmp/momoa-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momoa-0.2.0.tar", last modified: Thu Feb 16 11:10:07 2023, max compression
+gzip compressed data, was "momoa-0.2.1.tar", last modified: Thu Apr 20 15:03:06 2023, max compression
```

## Comparing `momoa-0.2.0.tar` & `momoa-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1244 2023-02-16 11:10:00.576187 momoa-0.2.0/README.md
--rw-r--r--   0        0        0     3125 2023-02-16 11:10:00.576187 momoa-0.2.0/momoa/__init__.py
--rw-r--r--   0        0        0      294 2023-02-16 11:10:00.576187 momoa-0.2.0/momoa/exceptions.py
--rw-r--r--   0        0        0     1987 2023-02-16 11:10:00.576187 momoa-0.2.0/momoa/format.py
--rw-r--r--   0        0        0     4055 2023-02-16 11:10:00.576187 momoa-0.2.0/momoa/model.py
--rw-r--r--   0        0        0        0 2023-02-16 11:10:00.576187 momoa-0.2.0/momoa/py.typed
--rw-r--r--   0        0        0     2354 2023-02-16 11:10:00.576187 momoa-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-16 11:10:00.576187 momoa-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      339 2023-02-16 11:10:00.576187 momoa-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0      606 2023-02-16 11:10:00.576187 momoa-0.2.0/tests/test_data/action_description.json
--rw-r--r--   0        0        0      169 2023-02-16 11:10:00.576187 momoa-0.2.0/tests/test_data/action_input_schema.json
--rw-r--r--   0        0        0      180 2023-02-16 11:10:00.576187 momoa-0.2.0/tests/test_data/action_output_schema.json
--rw-r--r--   0        0        0     1410 2023-02-16 11:10:00.576187 momoa-0.2.0/tests/test_data/schema.json
--rw-r--r--   0        0        0      304 2023-02-16 11:10:00.576187 momoa-0.2.0/tests/test_data/valid.json
--rw-r--r--   0        0        0     4167 2023-02-16 11:10:00.576187 momoa-0.2.0/tests/test_deserialization.py
--rw-r--r--   0        0        0     1847 2023-02-16 11:10:00.576187 momoa-0.2.0/tests/test_format.py
--rw-r--r--   0        0        0     3476 2023-02-16 11:10:00.576187 momoa-0.2.0/tests/test_model.py
--rw-r--r--   0        0        0     1653 2023-02-16 11:10:00.576187 momoa-0.2.0/tests/test_schema.py
--rw-r--r--   0        0        0     3687 2023-02-16 11:10:00.576187 momoa-0.2.0/tests/test_serialization.py
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 momoa-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1244 2023-04-20 15:02:55.984472 momoa-0.2.1/README.md
+-rw-r--r--   0        0        0     3125 2023-04-20 15:02:55.984472 momoa-0.2.1/momoa/__init__.py
+-rw-r--r--   0        0        0      294 2023-04-20 15:02:55.984472 momoa-0.2.1/momoa/exceptions.py
+-rw-r--r--   0        0        0     1977 2023-04-20 15:02:55.984472 momoa-0.2.1/momoa/format.py
+-rw-r--r--   0        0        0     4278 2023-04-20 15:02:55.984472 momoa-0.2.1/momoa/model.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:02:55.984472 momoa-0.2.1/momoa/py.typed
+-rw-r--r--   0        0        0     2605 2023-04-20 15:02:55.984472 momoa-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      339 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0      606 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_data/action_description.json
+-rw-r--r--   0        0        0      169 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_data/action_input_schema.json
+-rw-r--r--   0        0        0      180 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_data/action_output_schema.json
+-rw-r--r--   0        0        0     1410 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_data/schema.json
+-rw-r--r--   0        0        0      304 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_data/valid.json
+-rw-r--r--   0        0        0     4167 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_deserialization.py
+-rw-r--r--   0        0        0     2240 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_format.py
+-rw-r--r--   0        0        0     3476 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_model.py
+-rw-r--r--   0        0        0     1653 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_schema.py
+-rw-r--r--   0        0        0     3687 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_serialization.py
+-rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 momoa-0.2.1/PKG-INFO
```

### Comparing `momoa-0.2.0/README.md` & `momoa-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `momoa-0.2.0/momoa/__init__.py` & `momoa-0.2.1/momoa/__init__.py`

 * *Files identical despite different names*

### Comparing `momoa-0.2.0/momoa/format.py` & `momoa-0.2.1/momoa/format.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 """Helper utilities for formatting serialized data."""
 from datetime import date, datetime
 from ipaddress import ip_address
-from typing import Any, cast
+from typing import Any, Callable, cast, Mapping
+from uuid import UUID
 
 from dateutil.parser import isoparse
 
+FormatMapping = Mapping[str, Callable]
+
 
 def _format_date_time(value: datetime) -> str:
     """
     Helper function for formatting date-time values.
 
     If all the sub-day units are set to `00`, the value is formatted as a date.
     """
     if not any((value.hour, value.minute, value.second, value.microsecond)):
         value = cast(datetime, date(value.year, value.month, value.day))
     return value.isoformat()
 
 
-def _passthrough(value: Any) -> Any:
-    """Simple callable that returns the value intact."""
-    return value
-
-
 class StringFormat:
     """
     Helper utility for converting values of string fields with format.
 
     JSON Schema `string` type supports the `format` keyword, which can be used to
     convert its value to and from a native Python type. This class supports custom
     implementation of that conversion.
     """
 
-    _to_mapping = {"date-time": _format_date_time}
-    _from_mapping = {
+    _to_mapping: FormatMapping = {"date-time": _format_date_time}
+    _from_mapping: FormatMapping = {
         "date-time": isoparse,
         "ipv4": ip_address,
         "ipv6": ip_address,
+        "uuid": UUID,
     }
 
     def __init__(self, fmt):
         self.format = fmt
 
     def to_(self, value: Any) -> str:
         """
         Converts a value of a Python native type to a formatted JSON string.
 
-        Attributes:
+        Args:
             value: Any Python type, to be converted if supported.
 
         Returns:
             A formatted string.
         """
-        return self._to_mapping.get(self.format, _passthrough)(value)
+        return self._to_mapping.get(self.format, str)(value)
 
     def from_(self, value: str) -> Any:
         """
         Converts a formatted JSON string to a native Python type.
 
-        Attributes:
+        Args:
             value: A formatted string, to be converted if supported.
 
         Returns:
             A native Python type if conversion is supported, or the original
             string value if not.
         """
-        return self._from_mapping.get(self.format, _passthrough)(value)
+        return self._from_mapping.get(self.format, str)(value)
```

### Comparing `momoa-0.2.0/momoa/model.py` & `momoa-0.2.1/momoa/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,35 +15,36 @@
 UNDEFINED = NotPassed()
 
 
 class Model:
     """Base model class."""
 
     _schema_class: meta.ObjectMeta
+    _formatter: Type[StringFormat]
 
     def __init__(self, **data):
         try:
             self._instance = self._schema_class(
                 {key: self._format(key, value) for key, value in data.items()}
             )
         except ValidationError as ex:
             raise DataValidationError(f"{type(self).__name__} validation error: {ex}") from ex
 
     def _format(self, field: str, value: Any) -> str:
         """Converts Python native values to JSONSchema string equivalents on the fly."""
         element = self._get_field_element(field)
         if isinstance(element, String) and not isinstance(value, str):
-            value = StringFormat(element.format).to_(value)
+            value = self._formatter(element.format).to_(value)
         return value
 
     def _unformat(self, field: str, value: str) -> Any:
         """Converts JSONSchema formatted string values to Python native on the fly."""
         element = self._get_field_element(field)
         if isinstance(element, String) and value:
-            value = StringFormat(element.format).from_(value)
+            value = self._formatter(element.format).from_(value)
         else:
             value = element(value)
         return value
 
     def __getattr__(self, item: str) -> Any:
         if item in self._schema_class.properties:  # type: ignore
             return self._unformat(item, getattr(self._instance, item))
@@ -75,26 +76,32 @@
             raise DataValidationError(f"Invalid field '{field}'") from ex
 
     def serialize(self):
         """Validates data and serializes it into JSON-ready format."""
         return _serialize_schema_value(self._instance)
 
     @staticmethod  # pragma: no mutate
-    def make_model(schema_class: meta.ObjectMeta) -> Type[Model]:
+    def make_model(schema_class: meta.ObjectMeta, string_formatter=StringFormat) -> Type[Model]:
         """
         Constructs a Model subclass based on the class derived from JSONSchema.
 
-        Attributes:
+        Args:
             schema_class: Class derived from the JSONSchema.
+            string_formatter: Class used to format strings.
 
         Returns:
             Subclass of the Model class.
         """
         name = pascalcase(schema_class.__name__) + "Model"
-        return cast(Type[Model], type(name, (Model,), {"_schema_class": schema_class}))
+        return cast(
+            Type[Model],
+            type(
+                name, (Model,), {"_schema_class": schema_class, "_formatter": string_formatter}
+            ),
+        )
 
 
 ModelFactory = Callable[[meta.ObjectMeta], Type[Model]]  # pragma: no mutate
 
 
 def _serialize_schema_value(value: Any) -> Any:
     """Helper function to recursively serialize schema values."""
```

### Comparing `momoa-0.2.0/pyproject.toml` & `momoa-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "momoa"
-version = "0.2.0"
+version = "0.2.1"
 description = "A library for definition, validation and serialisation of Python objects based on JSONSchema specifications."
 readme = "README.md"
 authors = [
     { name = "Berislav Lopac", email = "berislav@lopac.net" },
 ]
 requires-python = ">=3.8,<4.0"
 dependencies = [
@@ -112,16 +112,41 @@
 
 [tool.pydocstyle]
 add-ignore = "D105, D107, D212, D401"
 convention = "google"
 match-dir = "(?!tests).*"
 
 [tool.ruff]
+select = [
+    "E",
+    "F",
+    "W",
+    "D",
+    "PL",
+    "ERA",
+    "N",
+]
+ignore = [
+    "D105",
+    "D107",
+    "D203",
+    "D212",
+    "D401",
+    "D406",
+    "D407",
+]
 line-length = 96
 target-version = "py38"
 format = "grouped"
 
+[tool.ruff.per-file-ignores]
+"tests/*" = [
+    "D",
+    "N",
+    "PLR",
+]
+
 [build-system]
 requires = [
     "pdm-pep517>=1.0.0",
 ]
 build-backend = "pdm.pep517.api"
```

### Comparing `momoa-0.2.0/tests/test_data/action_description.json` & `momoa-0.2.1/tests/test_data/action_description.json`

 * *Files identical despite different names*

### Comparing `momoa-0.2.0/tests/test_data/schema.json` & `momoa-0.2.1/tests/test_data/schema.json`

 * *Files identical despite different names*

### Comparing `momoa-0.2.0/tests/test_deserialization.py` & `momoa-0.2.1/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `momoa-0.2.0/tests/test_format.py` & `momoa-0.2.1/tests/test_format.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import datetime, timezone
 from ipaddress import IPv4Address, IPv6Address
+from uuid import UUID
 
 import pytest
 
 from momoa.format import StringFormat
 
 
 @pytest.mark.parametrize(
@@ -20,18 +21,24 @@
             "date-time",
             "2002-05-22T11:45:00Z",
             datetime(2002, 5, 22, 11, 45, tzinfo=timezone.utc),
             id="datetime with timezone",
         ),
         pytest.param("ipv4", "192.168.0.1", IPv4Address("192.168.0.1"), id="IPv4"),
         pytest.param("ipv6", "2001:db8::1000", IPv6Address("2001:db8::1000"), id="IPv6"),
+        pytest.param(
+            "uuid",
+            "4cbf6ab8-1785-4264-a011-ee655edbe4f5",
+            UUID("4cbf6ab8-1785-4264-a011-ee655edbe4f5"),
+            id="UUID",
+        ),
         pytest.param("unknown", "blabla", "blabla", id="unknown format"),
     ),
 )
-def test_strings_are_deserializsed_to_correct_value(format_name, value, deserialized):
+def test_strings_are_deserialised_to_correct_value(format_name, value, deserialized):
     fmt = StringFormat(format_name)
     assert fmt.from_(value) == deserialized
 
 
 @pytest.mark.parametrize(
     "format_name, serialized, value",
     (
@@ -45,12 +52,18 @@
         pytest.param(
             "date-time",
             "2002-05-22T11:45:00+00:00",
             datetime(2002, 5, 22, 11, 45, tzinfo=timezone.utc),
             id="datetime with timezone",
         ),
         pytest.param("unknown", "blabla", "blabla", id="unknown format"),
+        pytest.param(
+            "uuid",
+            "4cbf6ab8-1785-4264-a011-ee655edbe4f5",
+            UUID("4cbf6ab8-1785-4264-a011-ee655edbe4f5"),
+            id="UUID",
+        ),
     ),
 )
 def test_values_are_serialized_to_correct_format(format_name, serialized, value):
     fmt = StringFormat(format_name)
     assert fmt.to_(value) == serialized
```

### Comparing `momoa-0.2.0/tests/test_model.py` & `momoa-0.2.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `momoa-0.2.0/tests/test_schema.py` & `momoa-0.2.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `momoa-0.2.0/tests/test_serialization.py` & `momoa-0.2.1/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `momoa-0.2.0/PKG-INFO` & `momoa-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momoa
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library for definition, validation and serialisation of Python objects based on JSONSchema specifications.
 License: MIT
 Author-email: Berislav Lopac <berislav@lopac.net>
 Requires-Python: >=3.8,<4.0
 Project-URL: homepage, https://momoa.readthedocs.io
 Project-URL: repository, https://github.com/berislavlopac/momoa
 Description-Content-Type: text/markdown
```

