# Comparing `tmp/foxglove-data-platform-0.4.0.tar.gz` & `tmp/foxglove-data-platform-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxglove-data-platform-0.4.0.tar", last modified: Tue Feb  7 14:24:11 2023, max compression
+gzip compressed data, was "foxglove-data-platform-0.5.0.tar", last modified: Wed Apr 19 23:07:27 2023, max compression
```

## Comparing `foxglove-data-platform-0.4.0.tar` & `foxglove-data-platform-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:24:11.083168 foxglove-data-platform-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-07 14:24:11.083168 foxglove-data-platform-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:24:11.079168 foxglove-data-platform-0.4.0/foxglove_data_platform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/foxglove_data_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19889 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/foxglove_data_platform/client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/foxglove_data_platform/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:24:11.079168 foxglove-data-platform-0.4.0/foxglove_data_platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-07 14:24:11.000000 foxglove-data-platform-0.4.0/foxglove_data_platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-07 14:24:11.000000 foxglove-data-platform-0.4.0/foxglove_data_platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 14:24:11.000000 foxglove-data-platform-0.4.0/foxglove_data_platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-07 14:24:11.000000 foxglove-data-platform-0.4.0/foxglove_data_platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-07 14:24:11.000000 foxglove-data-platform-0.4.0/foxglove_data_platform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-07 14:24:11.083168 foxglove-data-platform-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:24:11.079168 foxglove-data-platform-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/tests/api_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/tests/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/tests/string_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/tests/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/tests/test_json_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/tests/test_protobuf_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/tests/test_ros1_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-02-07 14:23:40.000000 foxglove-data-platform-0.4.0/tests/test_ros2_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:27.120818 foxglove-data-platform-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-19 23:07:27.120818 foxglove-data-platform-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:27.116818 foxglove-data-platform-0.5.0/foxglove_data_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/foxglove_data_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/foxglove_data_platform/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/foxglove_data_platform/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:27.116818 foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-19 23:07:27.000000 foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-19 23:07:27.000000 foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:07:27.000000 foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 23:07:27.000000 foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-19 23:07:27.000000 foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-19 23:07:27.120818 foxglove-data-platform-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:27.120818 foxglove-data-platform-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/api_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/string_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_json_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_protobuf_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_ros1_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_ros2_messages.py
```

### Comparing `foxglove-data-platform-0.4.0/LICENSE` & `foxglove-data-platform-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.4.0/PKG-INFO` & `foxglove-data-platform-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-data-platform
-Version: 0.4.0
+Version: 0.5.0
 Summary: Client library for Foxglove Data Platform.
 Home-page: https://github.com/foxglove/py-data-platform
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-data-platform-0.4.0/README.md` & `foxglove-data-platform-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.4.0/foxglove_data_platform/client.py` & `foxglove-data-platform-0.5.0/foxglove_data_platform/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,132 +154,107 @@
         self.__host = host
 
     def __url__(self, path: str):
         return f"https://{self.__host}{path}"
 
     def create_event(
         self,
+        *,
         device_id: str,
-        time: datetime.datetime,
-        duration: int,
+        start: datetime.datetime,
+        end: Optional[datetime.datetime],
         metadata: Optional[Dict[str, str]] = {},
     ):
         """
         Creates a new event.
 
         device_id: The unique of the device associated with this event.
-        time: The time at which the event occurred.
-        duration: The duration of the event. Zero for an instantaneous event.
+        start: The event start time.
+        end: The event end time. If not provided, an instantaneous event (with end == start)
+            is created.
         metadata: Optional metadata attached to the event.
         """
+        if end is None:
+            end = start
         response = requests.post(
-            self.__url__("/beta/device-events"),
+            self.__url__("/v1/events"),
             headers=self.__headers,
             json={
                 "deviceId": device_id,
-                "durationNanos": str(duration),
+                "start": start.astimezone().isoformat(),
+                "end": end.astimezone().isoformat(),
                 "metadata": metadata,
-                "timestamp": time.astimezone().isoformat(),
             },
         )
 
-        event = json_or_raise(response)
-        return {
-            "id": event["id"],
-            "device_id": event["deviceId"],
-            "timestamp_nanos": event["timestampNanos"],
-            "duration_nanos": event["durationNanos"],
-            "metadata": event["metadata"],
-            "created_at": arrow.get(event["createdAt"]).datetime,
-            "updated_at": arrow.get(event["updatedAt"]).datetime,
-        }
+        return _event_dict(json_or_raise(response))
 
     def delete_event(
         self,
+        *,
         event_id: str,
     ):
         """
         Deletes an event.
 
         event_id: The id of the event to delete.
         """
         response = requests.delete(
-            self.__url__(f"/beta/device-events/{event_id}"),
+            self.__url__(f"/v1/events/{event_id}"),
             headers=self.__headers,
         )
-        json_or_raise(response)
+        return json_or_raise(response)
 
     def get_events(
         self,
+        *,
         device_id: Optional[str] = None,
-        device_name: Optional[str] = None,
         sort_by: Optional[str] = None,
         sort_order: Optional[str] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         start: Optional[datetime.datetime] = None,
         end: Optional[datetime.datetime] = None,
-        key: Optional[str] = None,
-        value: Optional[str] = None,
+        query: Optional[str] = None,
     ):
         """
         Retrieves events.
 
         device_id: Id of the device associated with the events.
-        device_name: Name of the device associated with events.
-            Either device_id or device_name is required.
         sort_by: Optionally sort records by this field name (e.g. "device_id").
         sort_order: Optionally specify the sort order, either "asc" or "desc".
         limit: Optionally limit the number of records returned.
         offset: Optionally offset the results by this many records.
         start: Optionally exclude records before this time.
         end: Optionally exclude records after this time.
-        key: Optionally only return records having this key = this value.
-        value: Optionally only return records having this key = this value.
+        query: optional query string to filter events by metadata.
+            See https://foxglove.dev/docs/api#tag/Events/paths/~1events/get for a syntax definition
+            of `query`.
         """
-        if not device_id and not device_name:
-            raise FoxgloveException("One of device_id or device_name is required.")
-
         params = {
             "deviceId": device_id,
-            "deviceName": device_name,
             "sortBy": camelize(sort_by),
             "sortOrder": sort_order,
             "limit": limit,
             "offset": offset,
             "start": start.astimezone().isoformat() if start else None,
             "end": end.astimezone().isoformat() if end else None,
-            "key": key,
-            "value": value,
+            "query": query,
         }
         response = requests.get(
-            self.__url__("/beta/device-events"),
+            self.__url__("/v1/events"),
             headers=self.__headers,
             params={k: v for k, v in params.items() if v is not None},
         )
 
-        json = json_or_raise(response)
-
-        return [
-            {
-                "id": e["id"],
-                "device_id": e["deviceId"],
-                "duration": int(e["durationNanos"]),
-                "metadata": e["metadata"],
-                # datetime doesn't support nanoseconds so we have to divide by 1e9 first.
-                "timestamp": arrow.get(int(e["timestampNanos"]) / 1e9).datetime,
-                "timestamp_nanos": int(e["timestampNanos"]),
-                "created_at": arrow.get(e["createdAt"]).datetime,
-                "updated_at": arrow.get(e["updatedAt"]).datetime,
-            }
-            for e in json
-        ]
+        return [_event_dict(event) for event in json_or_raise(response)]
 
     def get_messages(
         self,
+        *,
         device_id: str,
         start: datetime.datetime,
         end: datetime.datetime,
         topics: List[str] = [],
     ):
         """
         Returns a list of tuples of (topic, raw mcap record, decoded message).
@@ -309,14 +284,15 @@
             output_messages.append(
                 (channel.topic, message, decoder.decode(schema, message))
             )
         return output_messages
 
     def download_data(
         self,
+        *,
         device_id: str,
         start: datetime.datetime,
         end: datetime.datetime,
         topics: List[str] = [],
         output_format: OutputFormat = OutputFormat.mcap0,
         callback: Optional[ProgressCallback] = None,
     ) -> bytes:
@@ -352,14 +328,15 @@
             data.write(chunk)
             if callback:
                 callback(progress=data.tell())
         return data.getvalue()
 
     def get_coverage(
         self,
+        *,
         start: datetime.datetime,
         end: datetime.datetime,
         device_id: Optional[str] = None,
         tolerance: Optional[int] = None,
     ):
         """
         List coverage ranges for data.
@@ -388,15 +365,15 @@
                 "device_id": c["deviceId"],
                 "start": arrow.get(c["start"]).datetime,
                 "end": arrow.get(c["end"]).datetime,
             }
             for c in json
         ]
 
-    def get_device(self, device_id: str):
+    def get_device(self, *, device_id: str):
         """
         Gets a single device by id.
 
         :param device_id: The id of the device to retrieve.
         """
         response = requests.get(
             self.__url__(f"/v1/devices/{device_id}"),
@@ -427,14 +404,15 @@
                 "name": d["name"],
             }
             for d in json
         ]
 
     def create_device(
         self,
+        *,
         name: str,
         serial_number: Optional[str] = None,
     ):
         """
         Creates a new device.
 
         name: The name of the devicee.
@@ -451,29 +429,29 @@
         device = json_or_raise(response)
 
         return {
             "id": device["id"],
             "name": device["name"],
         }
 
-    def delete_device(self, device_id: str):
+    def delete_device(self, *, device_id: str):
         """
         Deletes an existing device.
 
         Note: you must first delete all imports from the device; see `delete_import`.
 
         :param device_id: The id of the device.
         """
         response = requests.delete(
             self.__url__(f"/v1/devices/{device_id}"),
             headers=self.__headers,
         )
         json_or_raise(response)
 
-    def delete_import(self, device_id: str, import_id: str):
+    def delete_import(self, *, device_id: str, import_id: str):
         """
         Deletes an existing import.
 
         :param device_id: The id of the device associated with the import.
         :param import_id: The id of the import to delete.
         """
         response = requests.delete(
@@ -481,14 +459,15 @@
             params={"deviceId": device_id},
             headers=self.__headers,
         )
         json_or_raise(response)
 
     def get_imports(
         self,
+        *,
         device_id: Optional[str] = None,
         start: Optional[datetime.datetime] = None,
         end: Optional[datetime.datetime] = None,
         data_start: Optional[datetime.datetime] = None,
         data_end: Optional[datetime.datetime] = None,
         include_deleted: bool = False,
         filename: Optional[str] = None,
@@ -546,14 +525,15 @@
                 "total_output_size": i["totalOutputSize"],
             }
             for i in json
         ]
 
     def get_topics(
         self,
+        *,
         device_id: str,
         start: datetime.datetime,
         end: datetime.datetime,
     ):
         response = requests.get(
             self.__url__("/v1/data/topics"),
             headers=self.__headers,
@@ -576,14 +556,15 @@
                 "schema_name": t["schemaName"],
             }
             for t in json
         ]
 
     def upload_data(
         self,
+        *,
         device_id: str,
         filename: str,
         data: Union[bytes, IO[Any]],
         callback: Optional[SizeProgressCallback] = None,
     ):
         """
         Uploads data in bytes.
@@ -615,8 +596,20 @@
         return {
             "link": link,
             "text": upload_request.text,
             "code": upload_request.status_code,
         }
 
 
+def _event_dict(json_event):
+    return {
+        "id": json_event["id"],
+        "device_id": json_event["deviceId"],
+        "start": arrow.get(json_event["start"]).datetime,
+        "end": arrow.get(json_event["end"]).datetime,
+        "metadata": json_event["metadata"],
+        "created_at": arrow.get(json_event["createdAt"]).datetime,
+        "updated_at": arrow.get(json_event["updatedAt"]).datetime,
+    }
+
+
 __all__ = ["Client", "FoxgloveException", "OutputFormat"]
```

### Comparing `foxglove-data-platform-0.4.0/foxglove_data_platform.egg-info/PKG-INFO` & `foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-data-platform
-Version: 0.4.0
+Version: 0.5.0
 Summary: Client library for Foxglove Data Platform.
 Home-page: https://github.com/foxglove/py-data-platform
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-data-platform-0.4.0/foxglove_data_platform.egg-info/SOURCES.txt` & `foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.4.0/setup.cfg` & `foxglove-data-platform-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foxglove-data-platform
-version = 0.4.0
+version = 0.5.0
 description = Client library for Foxglove Data Platform.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/foxglove/py-data-platform
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `foxglove-data-platform-0.4.0/tests/generate.py` & `foxglove-data-platform-0.5.0/tests/generate.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.4.0/tests/string_message_pb2.py` & `foxglove-data-platform-0.5.0/tests/string_message_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.4.0/tests/test_client.py` & `foxglove-data-platform-0.5.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.4.0/tests/test_coverage.py` & `foxglove-data-platform-0.5.0/tests/test_coverage.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.4.0/tests/test_data.py` & `foxglove-data-platform-0.5.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.4.0/tests/test_devices.py` & `foxglove-data-platform-0.5.0/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.4.0/tests/test_imports.py` & `foxglove-data-platform-0.5.0/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.4.0/tests/test_protobuf_messages.py` & `foxglove-data-platform-0.5.0/tests/test_protobuf_messages.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.4.0/tests/test_ros1_messages.py` & `foxglove-data-platform-0.5.0/tests/test_ros1_messages.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.4.0/tests/test_ros2_messages.py` & `foxglove-data-platform-0.5.0/tests/test_ros2_messages.py`

 * *Files identical despite different names*

