# Comparing `tmp/yroom-0.0.2.tar.gz` & `tmp/yroom-0.0.3.tar.gz`

## Comparing `yroom-0.0.2.tar` & `yroom-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      315 1970-01-01 00:00:00.000000 yroom-0.0.2/Cargo.toml
--rw-r--r--   0     1001      123     2772 2023-03-29 20:52:17.000000 yroom-0.0.2/.github/workflows/release.yml
--rw-r--r--   0     1001      123     1169 2023-03-29 20:52:17.000000 yroom-0.0.2/.github/workflows/test.yml
--rw-r--r--   0     1001      123       40 2023-03-29 20:52:17.000000 yroom-0.0.2/.gitignore
--rw-r--r--   0     1001      123     1083 2023-03-29 20:52:17.000000 yroom-0.0.2/LICENSE
--rw-r--r--   0     1001      123      141 2023-03-29 20:52:17.000000 yroom-0.0.2/README.md
--rw-r--r--   0     1001      123       10 2023-03-29 20:54:02.000000 yroom-0.0.2/dist/yroom-0.0.2.tar.gz
--rw-r--r--   0     1001      123      736 2023-03-29 20:52:17.000000 yroom-0.0.2/pyproject.toml
--rw-r--r--   0     1001      123      272 2023-03-29 20:52:17.000000 yroom-0.0.2/src/lib.rs
--rw-r--r--   0     1001      123     9162 2023-03-29 20:52:17.000000 yroom-0.0.2/src/roomsync.rs
--rw-r--r--   0     1001      123     2392 2023-03-29 20:52:17.000000 yroom-0.0.2/tests/test_yroom.py
--rw-r--r--   0     1001      123     2105 2023-03-29 20:52:17.000000 yroom-0.0.2/yroom.pyi
--rw-r--r--   0     1001      123    13697 2023-03-29 20:52:17.000000 yroom-0.0.2/Cargo.lock
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 yroom-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      315 1970-01-01 00:00:00.000000 yroom-0.0.3/Cargo.toml
+-rw-r--r--   0     1001      123     2772 2023-04-20 13:59:19.000000 yroom-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0     1001      123     1169 2023-04-20 13:59:19.000000 yroom-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0     1001      123       40 2023-04-20 13:59:19.000000 yroom-0.0.3/.gitignore
+-rw-r--r--   0     1001      123     1083 2023-04-20 13:59:19.000000 yroom-0.0.3/LICENSE
+-rw-r--r--   0     1001      123      141 2023-04-20 13:59:19.000000 yroom-0.0.3/README.md
+-rw-r--r--   0     1001      123       10 2023-04-20 14:00:04.000000 yroom-0.0.3/dist/yroom-0.0.3.tar.gz
+-rw-r--r--   0     1001      123      736 2023-04-20 13:59:19.000000 yroom-0.0.3/pyproject.toml
+-rw-r--r--   0     1001      123      272 2023-04-20 13:59:19.000000 yroom-0.0.3/src/lib.rs
+-rw-r--r--   0     1001      123    12399 2023-04-20 13:59:19.000000 yroom-0.0.3/src/roomsync.rs
+-rw-r--r--   0     1001      123     2392 2023-04-20 13:59:19.000000 yroom-0.0.3/tests/test_yroom.py
+-rw-r--r--   0     1001      123     3421 2023-04-20 13:59:19.000000 yroom-0.0.3/yroom.pyi
+-rw-r--r--   0     1001      123    13697 2023-04-20 13:59:19.000000 yroom-0.0.3/Cargo.lock
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 yroom-0.0.3/PKG-INFO
```

### Comparing `yroom-0.0.2/.github/workflows/release.yml` & `yroom-0.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `yroom-0.0.2/.github/workflows/test.yml` & `yroom-0.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `yroom-0.0.2/LICENSE` & `yroom-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yroom-0.0.2/pyproject.toml` & `yroom-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "yroom"
-version = "0.0.2"
+version = "0.0.3"
 requires-python = ">=3.7"
 description = "Yjs sync and awareness protocol handler for a non-editing client (e.g. server)"
 authors = [
     { name = "Stefan Wehrmeyer", email = "mail@stefanwehrmeyer.com" }
 ]
 classifiers = [
     "Programming Language :: Rust",
```

### Comparing `yroom-0.0.2/tests/test_yroom.py` & `yroom-0.0.3/tests/test_yroom.py`

 * *Files identical despite different names*

### Comparing `yroom-0.0.2/yroom.pyi` & `yroom-0.0.3/yroom.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import Dict, List, Optional
 
 class YRoomMessage:
     """
     Container that holds two members: `payload` and `broadcast_payload`.
     `payload` is a message that should be sent to the connection that sent the message.
     `broadcast_payload` is a message that should be sent to all connections in the room.
     Either or both of the members can be of zero length and then must not be sent.
@@ -50,7 +50,37 @@
         """
         Remove the room, dropping the document, awareness and connection mapping.
         """
     def list_rooms(self) -> List[str]:
         """
         Return list all room names that are available.
         """
+    def get_map(self, room: str, name: str) -> Optional[str]:
+        """
+        Return the named map from the doc of that room as a JSON string or
+        None if map or room does not exist.
+        """
+    def get_array(self, room: str, name: str) -> Optional[str]:
+        """
+        Return the named array from the doc of that room as a JSON string or
+        None if array or room does not exist.
+        """
+    def get_text(self, room: str, name: str) -> Optional[str]:
+        """
+        Return the named text from the doc of that room or
+        None if text or room does not exist.
+        """
+    def get_xml_element(self, room: str, name: str) -> Optional[str]:
+        """
+        Return the named xml element from the doc of that room as serialized string or
+        None if xml element or room does not exist.
+        """
+    def get_xml_text(self, room: str, name: str) -> Optional[str]:
+        """
+        Return the named xml text from the doc of that room as serialized string or
+        None if xml text or room does not exist.
+        """
+    def get_xml_fragment(self, room: str, name: str) -> Optional[str]:
+        """
+        Return the named xml fragment from the doc of that room as serialized string or
+        None if xml fragment or room does not exist.
+        """
```

### Comparing `yroom-0.0.2/Cargo.lock` & `yroom-0.0.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,15 @@
  "lib0",
  "thiserror",
  "yrs",
 ]
 
 [[package]]
 name = "yroom"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
  "lib0",
  "log",
  "pyo3",
  "pyo3-log",
  "y-sync",
  "yrs",
```

### Comparing `yroom-0.0.2/PKG-INFO` & `yroom-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yroom
-Version: 0.0.2
+Version: 0.0.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pytest; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
 Summary: Yjs sync and awareness protocol handler for a non-editing client (e.g. server)
```

