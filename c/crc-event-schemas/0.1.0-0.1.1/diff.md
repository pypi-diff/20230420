# Comparing `tmp/crc-event-schemas-0.1.0.tar.gz` & `tmp/crc-event-schemas-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc-event-schemas-0.1.0.tar", last modified: Wed Sep 28 13:49:51 2022, max compression
+gzip compressed data, was "crc-event-schemas-0.1.1.tar", last modified: Thu Apr 20 17:53:39 2023, max compression
```

## Comparing `crc-event-schemas-0.1.0.tar` & `crc-event-schemas-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,39 @@
-drwxr-xr-x   0 khowell  (22338) khowell  (22338)        0 2022-09-28 13:49:51.752035 crc-event-schemas-0.1.0/
--rw-r--r--   0 khowell  (22338) khowell  (22338)    11358 2022-09-28 13:48:29.000000 crc-event-schemas-0.1.0/LICENSE.txt
--rw-r--r--   0 khowell  (22338) khowell  (22338)      211 2022-09-28 13:49:51.752035 crc-event-schemas-0.1.0/PKG-INFO
--rw-r--r--   0 khowell  (22338) khowell  (22338)      105 2022-09-28 13:49:40.000000 crc-event-schemas-0.1.0/README.md
-drwxr-xr-x   0 khowell  (22338) khowell  (22338)        0 2022-09-28 13:49:51.751035 crc-event-schemas-0.1.0/crc_event_schemas.egg-info/
--rw-r--r--   0 khowell  (22338) khowell  (22338)      211 2022-09-28 13:49:51.000000 crc-event-schemas-0.1.0/crc_event_schemas.egg-info/PKG-INFO
--rw-r--r--   0 khowell  (22338) khowell  (22338)      537 2022-09-28 13:49:51.000000 crc-event-schemas-0.1.0/crc_event_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 khowell  (22338) khowell  (22338)        1 2022-09-28 13:49:51.000000 crc-event-schemas-0.1.0/crc_event_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 khowell  (22338) khowell  (22338)       14 2022-09-28 13:49:51.000000 crc-event-schemas-0.1.0/crc_event_schemas.egg-info/top_level.txt
-drwxr-xr-x   0 khowell  (22338) khowell  (22338)        0 2022-09-28 13:49:51.751035 crc-event-schemas-0.1.0/event_schemas/
--rw-r--r--   0 khowell  (22338) khowell  (22338)        0 2022-08-26 21:08:42.000000 crc-event-schemas-0.1.0/event_schemas/__init__.py
-drwxr-xr-x   0 khowell  (22338) khowell  (22338)        0 2022-09-28 13:49:51.751035 crc-event-schemas-0.1.0/event_schemas/apps/
--rw-r--r--   0 khowell  (22338) khowell  (22338)        0 2022-08-26 21:08:42.000000 crc-event-schemas-0.1.0/event_schemas/apps/__init__.py
-drwxr-xr-x   0 khowell  (22338) khowell  (22338)        0 2022-09-28 13:49:51.752035 crc-event-schemas-0.1.0/event_schemas/apps/advisor/
--rw-r--r--   0 khowell  (22338) khowell  (22338)        0 2022-08-26 21:08:42.000000 crc-event-schemas-0.1.0/event_schemas/apps/advisor/__init__.py
-drwxr-xr-x   0 khowell  (22338) khowell  (22338)        0 2022-09-28 13:49:51.752035 crc-event-schemas-0.1.0/event_schemas/apps/advisor/v1/
--rw-r--r--   0 khowell  (22338) khowell  (22338)        0 2022-08-26 21:08:42.000000 crc-event-schemas-0.1.0/event_schemas/apps/advisor/v1/__init__.py
--rw-r--r--   0 khowell  (22338) khowell  (22338)     6552 2022-08-26 21:08:42.000000 crc-event-schemas-0.1.0/event_schemas/apps/advisor/v1/advisor_recommendations.py
-drwxr-xr-x   0 khowell  (22338) khowell  (22338)        0 2022-09-28 13:49:51.752035 crc-event-schemas-0.1.0/event_schemas/core/
--rw-r--r--   0 khowell  (22338) khowell  (22338)        0 2022-08-26 21:08:42.000000 crc-event-schemas-0.1.0/event_schemas/core/__init__.py
-drwxr-xr-x   0 khowell  (22338) khowell  (22338)        0 2022-09-28 13:49:51.752035 crc-event-schemas-0.1.0/event_schemas/core/v1/
--rw-r--r--   0 khowell  (22338) khowell  (22338)        0 2022-08-26 21:08:42.000000 crc-event-schemas-0.1.0/event_schemas/core/v1/__init__.py
--rw-r--r--   0 khowell  (22338) khowell  (22338)     2803 2022-08-26 21:08:42.000000 crc-event-schemas-0.1.0/event_schemas/core/v1/error.py
--rw-r--r--   0 khowell  (22338) khowell  (22338)     4092 2022-08-26 21:08:42.000000 crc-event-schemas-0.1.0/event_schemas/core/v1/rhel_system.py
--rw-r--r--   0 khowell  (22338) khowell  (22338)       87 2022-09-28 13:41:30.000000 crc-event-schemas-0.1.0/pyproject.toml
--rw-r--r--   0 khowell  (22338) khowell  (22338)       38 2022-09-28 13:49:51.752035 crc-event-schemas-0.1.0/setup.cfg
--rw-r--r--   0 khowell  (22338) khowell  (22338)      269 2022-09-28 13:44:32.000000 crc-event-schemas-0.1.0/setup.py
+drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.687796 crc-event-schemas-0.1.1/
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)    11358 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/LICENSE.txt
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)      354 2023-04-20 17:53:39.687796 crc-event-schemas-0.1.1/PKG-INFO
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)      105 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/README.md
+drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.685796 crc-event-schemas-0.1.1/crc_event_schemas.egg-info/
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)      354 2023-04-20 17:53:39.000000 crc-event-schemas-0.1.1/crc_event_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)      888 2023-04-20 17:53:39.000000 crc-event-schemas-0.1.1/crc_event_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)        1 2023-04-20 17:53:39.000000 crc-event-schemas-0.1.1/crc_event_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)       14 2023-04-20 17:53:39.000000 crc-event-schemas-0.1.1/crc_event_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.685796 crc-event-schemas-0.1.1/event_schemas/
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/event_schemas/__init__.py
+drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.685796 crc-event-schemas-0.1.1/event_schemas/apps/
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/event_schemas/apps/__init__.py
+drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.685796 crc-event-schemas-0.1.1/event_schemas/apps/advisor/
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/event_schemas/apps/advisor/__init__.py
+drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.685796 crc-event-schemas-0.1.1/event_schemas/apps/advisor/v1/
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/event_schemas/apps/advisor/v1/__init__.py
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)     6908 2023-04-20 12:44:44.000000 crc-event-schemas-0.1.1/event_schemas/apps/advisor/v1/advisor_recommendations.py
+drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.685796 crc-event-schemas-0.1.1/event_schemas/apps/policies/
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 12:44:44.000000 crc-event-schemas-0.1.1/event_schemas/apps/policies/__init__.py
+drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.685796 crc-event-schemas-0.1.1/event_schemas/apps/policies/v1/
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 12:44:44.000000 crc-event-schemas-0.1.1/event_schemas/apps/policies/v1/__init__.py
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)     5652 2023-04-20 17:08:50.000000 crc-event-schemas-0.1.1/event_schemas/apps/policies/v1/policy_triggered.py
+drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.686796 crc-event-schemas-0.1.1/event_schemas/apps/repositories/
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:08:50.000000 crc-event-schemas-0.1.1/event_schemas/apps/repositories/__init__.py
+drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.686796 crc-event-schemas-0.1.1/event_schemas/apps/repositories/v1/
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:08:50.000000 crc-event-schemas-0.1.1/event_schemas/apps/repositories/v1/__init__.py
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)     7133 2023-04-20 17:08:50.000000 crc-event-schemas-0.1.1/event_schemas/apps/repositories/v1/repository_events.py
+drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.686796 crc-event-schemas-0.1.1/event_schemas/core/
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/event_schemas/core/__init__.py
+drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.686796 crc-event-schemas-0.1.1/event_schemas/core/v1/
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/event_schemas/core/v1/__init__.py
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)      125 2023-04-20 12:44:44.000000 crc-event-schemas-0.1.1/event_schemas/core/v1/common.py
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)     2687 2023-04-20 12:44:44.000000 crc-event-schemas-0.1.1/event_schemas/core/v1/error.py
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)     3829 2023-04-20 12:44:44.000000 crc-event-schemas-0.1.1/event_schemas/core/v1/notification.py
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)     4669 2023-04-20 12:44:44.000000 crc-event-schemas-0.1.1/event_schemas/core/v1/rhel_system.py
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)       87 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/pyproject.toml
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)       38 2023-04-20 17:53:39.687796 crc-event-schemas-0.1.1/setup.cfg
+-rw-r--r--   0 josejulio  (1000) josejulio  (1000)      364 2023-04-20 17:53:16.000000 crc-event-schemas-0.1.1/setup.py
```

### Comparing `crc-event-schemas-0.1.0/LICENSE.txt` & `crc-event-schemas-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crc-event-schemas-0.1.0/event_schemas/apps/advisor/v1/advisor_recommendations.py` & `crc-event-schemas-0.1.1/event_schemas/apps/advisor/v1/advisor_recommendations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-# This code parses date/times, so please
-#
-#     pip install python-dateutil
-#
-# To use this code, make sure you
-#
-#     import json
-#
-# and then, to convert JSON from a string, do
-#
-#     result = advisor_recommendations_from_dict(json.loads(json_string))
-
 from datetime import datetime
 from typing import Any, Optional, List, TypeVar, Callable, Type, cast
 import dateutil.parser
 
 
 T = TypeVar("T")
 
@@ -118,48 +106,59 @@
         result["namespace"] = from_str(self.namespace)
         result["value"] = from_str(self.value)
         return result
 
 
 class RHELSystem:
     """A RHEL system managed by console.redhat.com"""
+    """Timestamp of when the system did a check in. Must adhere to RFC 3339."""
+    check_in: Optional[datetime]
     display_name: Optional[str]
     host_url: Optional[str]
     hostname: Optional[str]
     inventory_id: str
     rhel_version: Optional[str]
     tags: Optional[List[RHELSystemTag]]
 
-    def __init__(self, display_name: Optional[str], host_url: Optional[str], hostname: Optional[str], inventory_id: str, rhel_version: Optional[str], tags: Optional[List[RHELSystemTag]]) -> None:
+    def __init__(self, check_in: Optional[datetime], display_name: Optional[str], host_url: Optional[str], hostname: Optional[str], inventory_id: str, rhel_version: Optional[str], tags: Optional[List[RHELSystemTag]]) -> None:
+        self.check_in = check_in
         self.display_name = display_name
         self.host_url = host_url
         self.hostname = hostname
         self.inventory_id = inventory_id
         self.rhel_version = rhel_version
         self.tags = tags
 
     @staticmethod
     def from_dict(obj: Any) -> 'RHELSystem':
         assert isinstance(obj, dict)
+        check_in = from_union([from_datetime, from_none], obj.get("check_in"))
         display_name = from_union([from_str, from_none], obj.get("display_name"))
         host_url = from_union([from_str, from_none], obj.get("host_url"))
         hostname = from_union([from_str, from_none], obj.get("hostname"))
         inventory_id = from_str(obj.get("inventory_id"))
         rhel_version = from_union([from_str, from_none], obj.get("rhel_version"))
         tags = from_union([lambda x: from_list(RHELSystemTag.from_dict, x), from_none], obj.get("tags"))
-        return RHELSystem(display_name, host_url, hostname, inventory_id, rhel_version, tags)
+        return RHELSystem(check_in, display_name, host_url, hostname, inventory_id, rhel_version, tags)
 
     def to_dict(self) -> dict:
         result: dict = {}
-        result["display_name"] = from_union([from_str, from_none], self.display_name)
-        result["host_url"] = from_union([from_str, from_none], self.host_url)
-        result["hostname"] = from_union([from_str, from_none], self.hostname)
+        if self.check_in is not None:
+            result["check_in"] = from_union([lambda x: x.isoformat(), from_none], self.check_in)
+        if self.display_name is not None:
+            result["display_name"] = from_union([from_str, from_none], self.display_name)
+        if self.host_url is not None:
+            result["host_url"] = from_union([from_str, from_none], self.host_url)
+        if self.hostname is not None:
+            result["hostname"] = from_union([from_str, from_none], self.hostname)
         result["inventory_id"] = from_str(self.inventory_id)
-        result["rhel_version"] = from_union([from_str, from_none], self.rhel_version)
-        result["tags"] = from_union([lambda x: from_list(lambda x: to_class(RHELSystemTag, x), x), from_none], self.tags)
+        if self.rhel_version is not None:
+            result["rhel_version"] = from_union([from_str, from_none], self.rhel_version)
+        if self.tags is not None:
+            result["tags"] = from_union([lambda x: from_list(lambda x: to_class(RHELSystemTag, x), x), from_none], self.tags)
         return result
 
 
 class AdvisorRecommendations:
     """Event data for Advisor Recommendations."""
     """Advisor recommendations for a system"""
     advisor_recommendations: List[AdvisorRecommendation]
```

### Comparing `crc-event-schemas-0.1.0/event_schemas/core/v1/error.py` & `crc-event-schemas-0.1.1/event_schemas/core/v1/error.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-# To use this code, make sure you
-#
-#     import json
-#
-# and then, to convert JSON from a string, do
-#
-#     result = error_from_dict(json.loads(json_string))
-
 from enum import Enum
 from typing import Optional, Any, TypeVar, Type, cast
 
 
 T = TypeVar("T")
 EnumT = TypeVar("EnumT", bound=Enum)
 
@@ -77,15 +69,16 @@
         return ErrorClass(code, message, severity, stack_trace)
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["code"] = from_str(self.code)
         result["message"] = from_str(self.message)
         result["severity"] = to_enum(Severity, self.severity)
-        result["stack_trace"] = from_union([from_str, from_none], self.stack_trace)
+        if self.stack_trace is not None:
+            result["stack_trace"] = from_union([from_str, from_none], self.stack_trace)
         return result
 
 
 class Error:
     """Event data for an application error."""
     error: ErrorClass
```

### Comparing `crc-event-schemas-0.1.0/event_schemas/core/v1/rhel_system.py` & `crc-event-schemas-0.1.1/event_schemas/core/v1/rhel_system.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-# To use this code, make sure you
-#
-#     import json
-#
-# and then, to convert JSON from a string, do
-#
-#     result = rhel_system_from_dict(json.loads(json_string))
-
 from typing import Any, Optional, List, TypeVar, Callable, Type, cast
+from datetime import datetime
+import dateutil.parser
 
 
 T = TypeVar("T")
 
 
 def from_str(x: Any) -> str:
     assert isinstance(x, str)
     return x
 
 
+def from_datetime(x: Any) -> datetime:
+    return dateutil.parser.parse(x)
+
+
 def from_none(x: Any) -> Any:
     assert x is None
     return x
 
 
 def from_union(fs, x):
     for f in fs:
@@ -65,48 +63,59 @@
         result["namespace"] = from_str(self.namespace)
         result["value"] = from_str(self.value)
         return result
 
 
 class SystemClass:
     """A RHEL system managed by console.redhat.com"""
+    """Timestamp of when the system did a check in. Must adhere to RFC 3339."""
+    check_in: Optional[datetime]
     display_name: Optional[str]
     host_url: Optional[str]
     hostname: Optional[str]
     inventory_id: str
     rhel_version: Optional[str]
     tags: Optional[List[RHELSystemTag]]
 
-    def __init__(self, display_name: Optional[str], host_url: Optional[str], hostname: Optional[str], inventory_id: str, rhel_version: Optional[str], tags: Optional[List[RHELSystemTag]]) -> None:
+    def __init__(self, check_in: Optional[datetime], display_name: Optional[str], host_url: Optional[str], hostname: Optional[str], inventory_id: str, rhel_version: Optional[str], tags: Optional[List[RHELSystemTag]]) -> None:
+        self.check_in = check_in
         self.display_name = display_name
         self.host_url = host_url
         self.hostname = hostname
         self.inventory_id = inventory_id
         self.rhel_version = rhel_version
         self.tags = tags
 
     @staticmethod
     def from_dict(obj: Any) -> 'SystemClass':
         assert isinstance(obj, dict)
+        check_in = from_union([from_datetime, from_none], obj.get("check_in"))
         display_name = from_union([from_str, from_none], obj.get("display_name"))
         host_url = from_union([from_str, from_none], obj.get("host_url"))
         hostname = from_union([from_str, from_none], obj.get("hostname"))
         inventory_id = from_str(obj.get("inventory_id"))
         rhel_version = from_union([from_str, from_none], obj.get("rhel_version"))
         tags = from_union([lambda x: from_list(RHELSystemTag.from_dict, x), from_none], obj.get("tags"))
-        return SystemClass(display_name, host_url, hostname, inventory_id, rhel_version, tags)
+        return SystemClass(check_in, display_name, host_url, hostname, inventory_id, rhel_version, tags)
 
     def to_dict(self) -> dict:
         result: dict = {}
-        result["display_name"] = from_union([from_str, from_none], self.display_name)
-        result["host_url"] = from_union([from_str, from_none], self.host_url)
-        result["hostname"] = from_union([from_str, from_none], self.hostname)
+        if self.check_in is not None:
+            result["check_in"] = from_union([lambda x: x.isoformat(), from_none], self.check_in)
+        if self.display_name is not None:
+            result["display_name"] = from_union([from_str, from_none], self.display_name)
+        if self.host_url is not None:
+            result["host_url"] = from_union([from_str, from_none], self.host_url)
+        if self.hostname is not None:
+            result["hostname"] = from_union([from_str, from_none], self.hostname)
         result["inventory_id"] = from_str(self.inventory_id)
-        result["rhel_version"] = from_union([from_str, from_none], self.rhel_version)
-        result["tags"] = from_union([lambda x: from_list(lambda x: to_class(RHELSystemTag, x), x), from_none], self.tags)
+        if self.rhel_version is not None:
+            result["rhel_version"] = from_union([from_str, from_none], self.rhel_version)
+        if self.tags is not None:
+            result["tags"] = from_union([lambda x: from_list(lambda x: to_class(RHELSystemTag, x), x), from_none], self.tags)
         return result
 
 
 class RHELSystem:
     """Event data for a RHEL system."""
     system: SystemClass
```

