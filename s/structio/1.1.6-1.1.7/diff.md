# Comparing `tmp/structio-1.1.6.tar.gz` & `tmp/structio-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structio-1.1.6.tar", last modified: Mon Apr 17 14:27:28 2023, max compression
+gzip compressed data, was "structio-1.1.7.tar", last modified: Thu Apr 20 00:24:59 2023, max compression
```

## Comparing `structio-1.1.6.tar` & `structio-1.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:27:28.688793 structio-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-04-17 14:27:28.688793 structio-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-04-17 14:27:11.000000 structio-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-17 14:27:11.000000 structio-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:27:28.688793 structio-1.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:27:28.688793 structio-1.1.6/structio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-04-17 14:27:28.000000 structio-1.1.6/structio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 14:27:28.000000 structio-1.1.6/structio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:27:28.000000 structio-1.1.6/structio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 14:27:28.000000 structio-1.1.6/structio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-04-17 14:27:11.000000 structio-1.1.6/structio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:24:59.772009 structio-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-04-20 00:24:59.772009 structio-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-04-20 00:24:41.000000 structio-1.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-20 00:24:41.000000 structio-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 00:24:59.772009 structio-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:24:59.772009 structio-1.1.7/structio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-04-20 00:24:59.000000 structio-1.1.7/structio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-20 00:24:59.000000 structio-1.1.7/structio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:24:59.000000 structio-1.1.7/structio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 00:24:59.000000 structio-1.1.7/structio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-04-20 00:24:41.000000 structio-1.1.7/structio.py
```

### Comparing `structio-1.1.6/PKG-INFO` & `structio-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.1.6
+Version: 1.1.7
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
```

### Comparing `structio-1.1.6/README.md` & `structio-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `structio-1.1.6/structio.egg-info/PKG-INFO` & `structio-1.1.7/structio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.1.6
+Version: 1.1.7
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
```

### Comparing `structio-1.1.6/structio.py` & `structio-1.1.7/structio.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,32 +13,39 @@
     def _get_endian(self, endian):
         if endian is None:
             return self.endian
         else:
             return endian
             
     def unpack_bool(self, b):
-        if len(b) == 1:
-            return b != b'\x00'
-        else:
-            raise ValueError('expected bytes object of length 1')
+        if isinstance(b, int):
+            return b != 0
             
+        else:
+            if len(b) == 1:
+                return b != b'\x00'
+            else:
+                raise ValueError('expected bytes object of length 1')
+                
     def pack_bool(self, boolean):
         if boolean:
             return b'\x01'
         else:
             return b'\x00'
             
     def unpack_bits(self, b):
-        if len(b) == 1:
-            number = self.unpack_int(b) 
-            return [number >> i & 1 for i in range(8)]
+        if isinstance(b, int):
+            number = b
+        elif len(b) == 1:
+            number = self.unpack_int(b)
         else:
             raise ValueError('expected bytes object of length 1')
             
+        return [number >> i & 1 for i in range(8)]
+        
     def pack_bits(self, bits):
         return self.pack_int(sum(bits[i] << i for i in range(8)), 1)
         
     def unpack_int(self, b, endian=None, signed=False):
         return int.from_bytes(b, self._get_endian(endian), signed=signed)
         
     def pack_int(self, number, numbytes, endian=None, signed=False):
```

