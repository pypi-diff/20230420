# Comparing `tmp/python_ssdb-1.0.1.tar.gz` & `tmp/python_ssdb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ssdb-1.0.1.tar", max compression
+gzip compressed data, was "python_ssdb-1.0.3.tar", max compression
```

## Comparing `python_ssdb-1.0.1.tar` & `python_ssdb-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      179 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/README.md
--rw-r--r--   0        0        0     1129 2022-12-15 08:49:40.002401 python_ssdb-1.0.1/build_extension.py
--rw-r--r--   0        0        0      457 2022-12-15 10:00:44.317214 python_ssdb-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       49 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/__init__.py
--rw-r--r--   0        0        0       57 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/asyncio/__init__.py
--rw-r--r--   0        0        0     2528 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/asyncio/client.pyx
--rw-r--r--   0        0        0     7310 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/asyncio/connection.pyx
--rw-r--r--   0        0        0     2119 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/client.pyx
--rw-r--r--   0        0        0     1176 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/connection.pxd
--rw-r--r--   0        0        0     7088 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/connection.pyx
--rw-r--r--   0        0        0      158 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/core/__init__.pxd
--rw-r--r--   0        0        0       74 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/core/__init__.py
--rw-r--r--   0        0        0      454 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/core/encode.pyx
--rw-r--r--   0        0        0       63 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/core/interface.pxd
--rw-r--r--   0        0        0    24892 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/core/interface.pyx
--rw-r--r--   0        0        0      649 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/core/parser.pxd
--rw-r--r--   0        0        0     4292 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/core/parser.pyx
--rw-r--r--   0        0        0       74 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/core/response.pxd
--rw-r--r--   0        0        0     4017 2022-12-15 08:38:07.512638 python_ssdb-1.0.1/ssdb/core/response.pyx
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 python_ssdb-1.0.1/setup.py
--rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 python_ssdb-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-02-01 01:52:39.060341 python_ssdb-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1183 2023-02-01 01:52:39.060341 python_ssdb-1.0.3/README.md
+-rw-r--r--   0        0        0     2091 2023-02-01 06:39:45.304914 python_ssdb-1.0.3/build_extension.py
+-rw-r--r--   0        0        0     1179 2023-02-01 07:15:35.917927 python_ssdb-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-02-01 01:52:39.064340 python_ssdb-1.0.3/ssdb/__init__.py
+-rw-r--r--   0        0        0       57 2023-02-01 01:52:39.064340 python_ssdb-1.0.3/ssdb/asyncio/__init__.py
+-rw-r--r--   0        0        0     2598 2023-02-01 06:39:45.304914 python_ssdb-1.0.3/ssdb/asyncio/client.pyx
+-rw-r--r--   0        0        0     7311 2023-02-01 01:52:39.064340 python_ssdb-1.0.3/ssdb/asyncio/connection.pyx
+-rw-r--r--   0        0        0     2118 2023-02-01 01:56:44.714468 python_ssdb-1.0.3/ssdb/client.pyx
+-rw-r--r--   0        0        0     1176 2023-02-01 01:52:39.064340 python_ssdb-1.0.3/ssdb/connection.pxd
+-rw-r--r--   0        0        0     7088 2023-02-01 01:52:39.064340 python_ssdb-1.0.3/ssdb/connection.pyx
+-rw-r--r--   0        0        0      158 2023-02-01 01:52:39.064340 python_ssdb-1.0.3/ssdb/core/__init__.pxd
+-rw-r--r--   0        0        0       74 2023-02-01 01:52:39.064340 python_ssdb-1.0.3/ssdb/core/__init__.py
+-rw-r--r--   0        0        0      454 2023-02-01 01:52:39.064340 python_ssdb-1.0.3/ssdb/core/encode.pyx
+-rw-r--r--   0        0        0       63 2023-02-01 01:52:39.064340 python_ssdb-1.0.3/ssdb/core/interface.pxd
+-rw-r--r--   0        0        0    24891 2023-02-01 01:56:44.714468 python_ssdb-1.0.3/ssdb/core/interface.pyx
+-rw-r--r--   0        0        0      649 2023-02-01 01:52:39.064340 python_ssdb-1.0.3/ssdb/core/parser.pxd
+-rw-r--r--   0        0        0     4292 2023-02-01 01:52:39.064340 python_ssdb-1.0.3/ssdb/core/parser.pyx
+-rw-r--r--   0        0        0       74 2023-02-01 01:52:39.064340 python_ssdb-1.0.3/ssdb/core/response.pxd
+-rw-r--r--   0        0        0     4017 2023-02-01 01:52:39.064340 python_ssdb-1.0.3/ssdb/core/response.pyx
+-rw-r--r--   0        0        0     1816 1970-01-01 00:00:00.000000 python_ssdb-1.0.3/PKG-INFO
```

### Comparing `python_ssdb-1.0.1/ssdb/asyncio/client.pyx` & `python_ssdb-1.0.3/ssdb/asyncio/client.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # cython: language_level=3, boundscheck=False, wraparound=False, embedsignature=True
 
 import asyncio
 from typing import TypeVar
 
-from ssdb.core cimport wrap_response, SSDBInterface
-from ssdb.asyncio.connection import Connection, ConnectionPool
+from ssdb.core cimport SSDBInterface, wrap_response
 
+from ssdb.asyncio.connection import Connection, ConnectionPool
 
 T = TypeVar("T")
 
 
 class SSDB(SSDBInterface):
     def __init__(
         self,
@@ -30,20 +30,23 @@
             "socket_keepalive_options": socket_keepalive_options,
         }
         self.connection_pool = ConnectionPool(max_connections, **connection_kwargs)
         self.connection = None
         self.single_connection_client = single_connection_client
 
     def __del__(self) -> None:
-        loop = asyncio.get_event_loop()
-        coro = self.close()
-        if loop.is_running():
-            loop.create_task(coro)
-        else:
-            loop.run_until_complete(coro)
+        try:
+            loop = asyncio.get_event_loop()
+            coro = self.close()
+            if loop.is_running():
+                loop.create_task(coro)
+            else:
+                loop.run_until_complete(coro)
+        except:
+            pass
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}<{repr(self.connection_pool)}>"
 
     def __await__(self):
         return self.initialize().__await__()
```

### Comparing `python_ssdb-1.0.1/ssdb/asyncio/connection.pyx` & `python_ssdb-1.0.3/ssdb/asyncio/connection.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # cython: language_level=3, boundscheck=False, wraparound=False
 
+import asyncio
 import os
 import socket
-import asyncio
 import threading
-from typing import List
 from itertools import chain
+from typing import List
 
 from libc.stdint cimport INT32_MAX
 
 from ssdb.core cimport Reader
+
 from ssdb.core import encode_command
 
 
 class Connection:
     def __init__(
         self,
         str host="localhost",
```

### Comparing `python_ssdb-1.0.1/ssdb/client.pyx` & `python_ssdb-1.0.3/ssdb/client.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # cython: language_level=3, boundscheck=False, wraparound=False, embedsignature=True
 
 from typing import TypeVar
 
-from ssdb.core cimport wrap_response, SSDBInterface
 from ssdb.connection cimport Connection, ConnectionPool
-
+from ssdb.core cimport SSDBInterface, wrap_response
 
 T = TypeVar("T")
 
 
 cdef class SSDB(SSDBInterface):
     cdef Connection connection
     cdef ConnectionPool connection_pool
```

### Comparing `python_ssdb-1.0.1/ssdb/connection.pxd` & `python_ssdb-1.0.3/ssdb/connection.pxd`

 * *Files identical despite different names*

### Comparing `python_ssdb-1.0.1/ssdb/connection.pyx` & `python_ssdb-1.0.3/ssdb/connection.pyx`

 * *Files identical despite different names*

### Comparing `python_ssdb-1.0.1/ssdb/core/interface.pyx` & `python_ssdb-1.0.3/ssdb/core/interface.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # cython: language_level=3, boundscheck=False, wraparound=False, embedsignature=True
 
 from collections.abc import Mapping
-from typing import TypeVar, Awaitable, Optional, Union, List, Dict
-
+from typing import Awaitable, Dict, List, Optional, TypeVar, Union
 
 T = TypeVar("T")
 NameT = Union[bytes, str]
 KeyT = Union[bytes, str]
 ValueT = Union[bytes, str, int, float]
```

### Comparing `python_ssdb-1.0.1/ssdb/core/parser.pxd` & `python_ssdb-1.0.3/ssdb/core/parser.pxd`

 * *Files identical despite different names*

### Comparing `python_ssdb-1.0.1/ssdb/core/parser.pyx` & `python_ssdb-1.0.3/ssdb/core/parser.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # cython: boundscheck=False, wraparound=False
 
 cimport cython
 from libc.stdint cimport uint8_t
 from libc.stdlib cimport atoi, free, malloc, realloc
-from libc.string cimport memchr, memcpy, memset, memmove
+from libc.string cimport memchr, memcpy, memmove, memset
 
 DEF INITIAL_BUF_SIZE = 8192  # 8KiB
 DEF BUF_MAX_SIZE = 16 * 1024 * 1024  # 16MiB
 
 
 @cython.internal
 cdef class ParserException(Exception):
```

### Comparing `python_ssdb-1.0.1/ssdb/core/response.pyx` & `python_ssdb-1.0.3/ssdb/core/response.pyx`

 * *Files identical despite different names*

