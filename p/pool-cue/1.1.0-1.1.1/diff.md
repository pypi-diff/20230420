# Comparing `tmp/pool_cue-1.1.0.tar.gz` & `tmp/pool_cue-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pool_cue-1.1.0.tar", max compression
+gzip compressed data, was "pool_cue-1.1.1.tar", max compression
```

## Comparing `pool_cue-1.1.0.tar` & `pool_cue-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1065 2023-04-20 07:47:24.577156 pool_cue-1.1.0/LICENSE
--rw-r--r--   0        0        0     1417 2023-04-20 07:47:24.577156 pool_cue-1.1.0/README.md
--rw-r--r--   0        0        0      309 2023-04-20 07:47:24.577156 pool_cue-1.1.0/pool_cue/__init__.py
--rw-r--r--   0        0        0      938 2023-04-20 07:47:24.577156 pool_cue-1.1.0/pool_cue/config.py
--rw-r--r--   0        0        0     1053 2023-04-20 07:47:24.577156 pool_cue-1.1.0/pool_cue/context.py
--rw-r--r--   0        0        0      158 2023-04-20 07:47:24.577156 pool_cue-1.1.0/pool_cue/exceptions.py
--rw-r--r--   0        0        0     5709 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pool_cue/jobs.py
--rw-r--r--   0        0        0     3451 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pool_cue/queue.py
--rw-r--r--   0        0        0      426 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pool_cue/serializers.py
--rw-r--r--   0        0        0     2247 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pool_cue/threading.py
--rw-r--r--   0        0        0      968 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pool_cue/typing.py
--rw-r--r--   0        0        0      984 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pool_cue/utils.py
--rw-r--r--   0        0        0     3967 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pool_cue/worker.py
--rw-r--r--   0        0        0      666 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 pool_cue-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-20 10:20:06.895622 pool_cue-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1417 2023-04-20 10:20:06.895622 pool_cue-1.1.1/README.md
+-rw-r--r--   0        0        0      309 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/__init__.py
+-rw-r--r--   0        0        0      938 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/config.py
+-rw-r--r--   0        0        0     1053 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/context.py
+-rw-r--r--   0        0        0      158 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/exceptions.py
+-rw-r--r--   0        0        0     5709 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/jobs.py
+-rw-r--r--   0        0        0     3451 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/queue.py
+-rw-r--r--   0        0        0      426 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/serializers.py
+-rw-r--r--   0        0        0     2247 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/threading.py
+-rw-r--r--   0        0        0      968 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/typing.py
+-rw-r--r--   0        0        0     1075 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/utils.py
+-rw-r--r--   0        0        0     3967 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/worker.py
+-rw-r--r--   0        0        0      666 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 pool_cue-1.1.1/PKG-INFO
```

### Comparing `pool_cue-1.1.0/LICENSE` & `pool_cue-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pool_cue-1.1.0/README.md` & `pool_cue-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pool_cue-1.1.0/pool_cue/config.py` & `pool_cue-1.1.1/pool_cue/config.py`

 * *Files identical despite different names*

### Comparing `pool_cue-1.1.0/pool_cue/context.py` & `pool_cue-1.1.1/pool_cue/context.py`

 * *Files identical despite different names*

### Comparing `pool_cue-1.1.0/pool_cue/jobs.py` & `pool_cue-1.1.1/pool_cue/jobs.py`

 * *Files identical despite different names*

### Comparing `pool_cue-1.1.0/pool_cue/queue.py` & `pool_cue-1.1.1/pool_cue/queue.py`

 * *Files identical despite different names*

### Comparing `pool_cue-1.1.0/pool_cue/threading.py` & `pool_cue-1.1.1/pool_cue/threading.py`

 * *Files identical despite different names*

### Comparing `pool_cue-1.1.0/pool_cue/typing.py` & `pool_cue-1.1.1/pool_cue/typing.py`

 * *Files identical despite different names*

### Comparing `pool_cue-1.1.0/pool_cue/utils.py` & `pool_cue-1.1.1/pool_cue/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,9 +22,11 @@
 
 
 def generate_job_id(_func: str, _children: list[str] | None = None, **kwargs) -> str:
     """
     Generate a 'unique' job identifier from the given arguments.
     """
     suffix: str = "_parent_job" if _children else "_job"
-    _hash: str = f"_{abs(hash(frozenset(kwargs.items())))}" if kwargs else ""
-    return _func + suffix + _hash
+    keyword_arguments_hash: str = (
+        f"_{abs(hash(frozenset((str(key), str(value)) for key, value in kwargs.items())))}" if kwargs else ""
+    )
+    return _func + suffix + keyword_arguments_hash
```

### Comparing `pool_cue-1.1.0/pool_cue/worker.py` & `pool_cue-1.1.1/pool_cue/worker.py`

 * *Files identical despite different names*

### Comparing `pool_cue-1.1.0/pyproject.toml` & `pool_cue-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pool-cue"
-version = "1.1.0"
+version = "1.1.1"
 description = "Tools for working with arq job queues"
 authors = ["skarre-r <skarre-r@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/skarre-r/pool-cue"
 packages = [
     { include = "pool_cue" }
 ]
```

### Comparing `pool_cue-1.1.0/PKG-INFO` & `pool_cue-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pool-cue
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tools for working with arq job queues
 Home-page: https://github.com/skarre-r/pool-cue
 Author: skarre-r
 Author-email: skarre-r@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

