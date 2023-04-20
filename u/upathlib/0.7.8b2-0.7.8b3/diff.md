# Comparing `tmp/upathlib-0.7.8b2.tar.gz` & `tmp/upathlib-0.7.8b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upathlib-0.7.8b2.tar", last modified: Mon Apr 17 17:57:17 2023, max compression
+gzip compressed data, was "upathlib-0.7.8b3.tar", last modified: Thu Apr 20 04:32:59 2023, max compression
```

## Comparing `upathlib-0.7.8b2.tar` & `upathlib-0.7.8b3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.7.8b2/LICENSE
--rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.7.8b2/README.rst
--rw-r--r--   0        0        0     1726 2023-04-15 03:57:22.660027 upathlib-0.7.8b2/pyproject.toml
--rw-r--r--   0        0        0     2305 2023-04-17 16:03:28.650934 upathlib-0.7.8b2/src/upathlib/__init__.py
--rw-r--r--   0        0        0     4438 2023-04-10 08:06:32.336660 upathlib-0.7.8b2/src/upathlib/_blob.py
--rw-r--r--   0        0        0    10985 2023-04-17 17:55:09.132671 upathlib-0.7.8b2/src/upathlib/_local.py
--rw-r--r--   0        0        0     7935 2023-04-17 17:40:01.495217 upathlib-0.7.8b2/src/upathlib/_tests.py
--rw-r--r--   0        0        0    34468 2023-04-17 17:41:36.641457 upathlib-0.7.8b2/src/upathlib/_upath.py
--rw-r--r--   0        0        0    12562 2023-04-10 08:06:32.346660 upathlib-0.7.8b2/src/upathlib/azure.py
--rw-r--r--   0        0        0    25832 2023-04-17 16:30:10.725430 upathlib-0.7.8b2/src/upathlib/gcs.py
--rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.7.8b2/src/upathlib/py.typed
--rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.7.8b2/src/upathlib/serializer.py
--rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 upathlib-0.7.8b2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.7.8b3/LICENSE
+-rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.7.8b3/README.rst
+-rw-r--r--   0        0        0     1726 2023-04-15 03:57:22.660027 upathlib-0.7.8b3/pyproject.toml
+-rw-r--r--   0        0        0     2320 2023-04-20 04:26:10.814627 upathlib-0.7.8b3/src/upathlib/__init__.py
+-rw-r--r--   0        0        0     4694 2023-04-20 04:26:10.454625 upathlib-0.7.8b3/src/upathlib/_blob.py
+-rw-r--r--   0        0        0    10997 2023-04-18 03:08:39.636189 upathlib-0.7.8b3/src/upathlib/_local.py
+-rw-r--r--   0        0        0     7935 2023-04-17 17:40:01.495217 upathlib-0.7.8b3/src/upathlib/_tests.py
+-rw-r--r--   0        0        0    34468 2023-04-17 17:41:36.641457 upathlib-0.7.8b3/src/upathlib/_upath.py
+-rw-r--r--   0        0        0    12562 2023-04-10 08:06:32.346660 upathlib-0.7.8b3/src/upathlib/azure.py
+-rw-r--r--   0        0        0    26061 2023-04-20 04:26:10.804627 upathlib-0.7.8b3/src/upathlib/gcs.py
+-rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.7.8b3/src/upathlib/py.typed
+-rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.7.8b3/src/upathlib/serializer.py
+-rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 upathlib-0.7.8b3/PKG-INFO
```

### Comparing `upathlib-0.7.8b2/LICENSE` & `upathlib-0.7.8b3/LICENSE`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.8b2/README.rst` & `upathlib-0.7.8b3/README.rst`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.8b2/pyproject.toml` & `upathlib-0.7.8b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.8b2/src/upathlib/__init__.py` & `upathlib-0.7.8b3/src/upathlib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 
 One use case is the package `biglist <https://biglist.readthedocs.io/en/latest/>`__,
 where the class `Biglist <https://biglist.readthedocs.io/en/latest/#biglist.Biglist>`__ takes a Upath object to indicate its location of storage.
 It does not care whether the storage is local or in a cloud blob store---it
 simply uses the common API to operate the storage.
 """
 
-__version__ = "0.7.8b2"
+__version__ = "0.7.8b3"
 
 from pathlib import Path
 from typing import Union
 
 from ._blob import BlobUpath
-from ._local import LocalUpath
+from ._local import LocalPathType, LocalUpath
 from ._upath import FileInfo, LockAcquireError, LockReleaseError, Upath
 
 try:
     from .gcs import GcsBlobUpath
 except ImportError:
     pass
 try:
```

### Comparing `upathlib-0.7.8b2/src/upathlib/_blob.py` & `upathlib-0.7.8b3/src/upathlib/_blob.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,49 +84,70 @@
             if "/" in tail:
                 tail = tail[: tail.find("/")]
             if tail not in subdirs:
                 yield self / tail
                 subdirs.add(tail)
 
     def download_dir(
-        self, target: LocalPathType, *, overwrite: bool = False, quiet: bool = False
+        self,
+        target: LocalPathType,
+        *,
+        overwrite: bool = False,
+        quiet: bool = False,
+        **kwargs,
     ) -> int:
         """
         A specialization of :meth:`~upathlib.Upath.copy_dir` where the target location
         is on the local disk.
         """
         target = _resolve_local_path(target)
 
         if not quiet:
             print(f"Downloading from {self!r} into {target!r}", file=sys.stderr)
         return self._copy_dir(
-            self, target, "download_file", overwrite=overwrite, quiet=quiet
+            self,
+            target,
+            "download_file",
+            overwrite=overwrite,
+            quiet=quiet,
+            **kwargs,
         )
 
     def download_file(self, target: LocalPathType, *, overwrite=False) -> None:
         """
         A specialization of :meth:`~upathlib.Upath.copy_file` where the target location
         is on the local disk.
 
         Subclass is expected to override with a more efficient implementation.
         """
         self.copy_file(target, overwrite=overwrite)
 
     def upload_dir(
-        self, source: LocalPathType, *, overwrite: bool = False, quiet: bool = False
+        self,
+        source: LocalPathType,
+        *,
+        overwrite: bool = False,
+        quiet: bool = False,
+        **kwargs,
     ) -> int:
         """
         A specialization of :meth:`~upathlib.Upath.copy_dir` for :class:`~upathlib.LocalUpath`
         where the target location is in a cloud blob store.
         """
         source = _resolve_local_path(source)
         if not quiet:
             print(f"Importing from {source!r} into {self!r}", file=sys.stderr)
         return self._copy_dir(
-            source, self, "upload_file", overwrite=overwrite, quiet=quiet, reversed=True
+            source,
+            self,
+            "upload_file",
+            overwrite=overwrite,
+            quiet=quiet,
+            reversed=True,
+            **kwargs,
         )
 
     def upload_file(self, source: LocalPathType, *, overwrite=False) -> None:
         """
         A specialization of :meth:`~upathlib.Upath.copy_file` for :class:`~upathlib.LocalUpath`
         where the target location is in a cloud blob store.
```

### Comparing `upathlib-0.7.8b2/src/upathlib/_local.py` & `upathlib-0.7.8b3/src/upathlib/_local.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,16 +304,16 @@
 
     @contextlib.contextmanager
     def lock(self, *, timeout=None):
         """
         This uses the package `filelock <https://github.com/tox-dev/py-filelock>`_ to implement
         a file lock for inter-process communication.
 
-        At the end, this file is not deleted. If it is purely a dummy file to implement locking
-        for other things, user may want to delete this file after use.
+        ..note.. At the end, this file is not deleted. If it is purely a dummy file to implement locking
+          for other things, user may want to delete this file after use.
         """
         if timeout is None:
             timeout = 60
         lock = self._lock
         if lock is None:
             lock = filelock.FileLock(str(self))  # this object manages re-entry itself
             self._lock = lock
@@ -331,8 +331,9 @@
             yield
         finally:
             try:
                 lock.release()  # in a re-entry situation, this may not actually "release" the lock
             except Exception as e:
                 raise LockReleaseError(f"failed to release lock on file {self}") from e
 
+
 LocalPathType = Union[str, pathlib.Path, LocalUpath]
```

### Comparing `upathlib-0.7.8b2/src/upathlib/_tests.py` & `upathlib-0.7.8b3/src/upathlib/_tests.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.8b2/src/upathlib/_upath.py` & `upathlib-0.7.8b3/src/upathlib/_upath.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.8b2/src/upathlib/azure.py` & `upathlib-0.7.8b3/src/upathlib/azure.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.8b2/src/upathlib/gcs.py` & `upathlib-0.7.8b3/src/upathlib/gcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,29 @@
 # `google.cloud` is repo python-cloud-core.
 from google.cloud.storage.retry import (
     DEFAULT_RETRY,
     DEFAULT_RETRY_IF_GENERATION_SPECIFIED,
     ConditionalRetryPolicy,
     is_generation_specified,
 )
-
-# The default timeout in `DEFAULT_RETRY` is 120 seconds.
 from mpservice.util import MAX_THREADS, get_shared_thread_pool
 from typing_extensions import Self
 
 from ._blob import BlobUpath, LocalPathType, _resolve_local_path
 from ._upath import FileInfo, LockAcquireError, LockReleaseError, Upath
 
+# To see retry info, uncomment the following. The printout is typically not overwhelming.
+# logging.getLogger('google.api_core.retry').setLevel(logging.DEBUG)
+
+
 logger = logging.getLogger(__name__)
 
 # When downloading large files, there may be INFO logs from `google.resumable_media._helpers` about "No MD5 checksum was returned...".
 # You may want to suppress that log by setting its level to WARNING.
 
-
 # 67108864 = 256 * 1024 * 256 = 64 MB
 MEGABYTES32 = 33554432
 MEGABYTES64 = 67108864
 LARGE_FILE_SIZE = MEGABYTES64
 
 # DEFAULT_RETRY has default timeout 120 seconds.
 
@@ -82,14 +83,17 @@
         not credentials.token
         or (credentials.expiry - datetime.utcnow()).total_seconds() < valid_for_seconds
     ):
         credentials.refresh(google.auth.transport.requests.Request())
         # One check shows that this token expires in one hour.
         renewed = True
 
+    if renewed:
+        logger.debug("Google credentials refreshed")
+
     return project_id, credentials, renewed
 
 
 class GcsBlobUpath(BlobUpath):
     """
     GcsBlobUpath implements the :class:`~upathlib.Upath` API for
     Google Cloud Storage.
@@ -420,38 +424,38 @@
             for tt in tasks[it:]:
                 if not tt.done():
                     tt.cancel()
                     # This may not succeed, but there isn't a good way to
                     # guarantee cancellation here.
             raise
 
-    def _read_into_buffer(self, file_obj, *, request_timeout=120):
-        file_info = self.file_info(request_timeout=request_timeout)
+    def _read_into_buffer(self, file_obj, *, concurrent=True):
+        file_info = self.file_info()
         if not file_info:
             raise FileNotFoundError(self)
         file_size = file_info.size  # bytes
-        if file_size <= LARGE_FILE_SIZE:
+        if file_size <= LARGE_FILE_SIZE or not concurrent:
             try:
                 self._blob().download_to_file(
                     file_obj, client=self._client(), raw_download=True
                 )
                 # "checksum mismatch" errors were encountered when downloading Parquet files.
                 # `raw_download=True` seems to prevent that error.
                 return
             except exceptions.NotFound:
                 raise FileNotFoundError(self)
         else:
             self._multipart_download(file_size, file_obj)
 
-    def read_bytes(self) -> bytes:
+    def read_bytes(self, **kwargs) -> bytes:
         """
         Return the content of the current blob as bytes.
         """
         buffer = BytesIO()
-        self._read_into_buffer(buffer)
+        self._read_into_buffer(buffer, **kwargs)
         return buffer.getvalue()
 
     # Google imposes rate limiting on create/update/delete requests.
     # According to Google doc, https://cloud.google.com/storage/quotas,
     #   There is a limit on writes to the same object name. This limit is once per second.
 
     def _copy_file(self, target: Upath, *, overwrite=False) -> None:
@@ -468,15 +472,17 @@
             except exceptions.NotFound:
                 raise FileNotFoundError(self)
             except exceptions.PreconditionFailed:
                 raise FileExistsError(target)
         else:
             super()._copy_file(target, overwrite=overwrite)
 
-    def download_file(self, target: LocalPathType, *, overwrite=False) -> None:
+    def download_file(
+        self, target: LocalPathType, *, overwrite=False, concurrent=True
+    ) -> None:
         """
         Download the content of the current blob to ``target``.
         """
         target = _resolve_local_path(target)
         if target.is_file():
             if not overwrite:
                 raise FileExistsError(target)
@@ -485,15 +491,15 @@
             raise IsADirectoryError(target)
 
         os.makedirs(str(target.parent), exist_ok=True)
         try:
             with open(target, "wb") as file_obj:
                 # If `target` is an existing directory,
                 # will raise `IsADirectoryError`.
-                self._read_into_buffer(file_obj)
+                self._read_into_buffer(file_obj, concurrent=concurrent)
             updated = self._blob().updated
             if updated is not None:
                 mtime = updated.timestamp()
                 os.utime(target, (mtime, mtime))
         except resumable_media.DataCorruption:
             target.remove_file()
             raise
```

### Comparing `upathlib-0.7.8b2/src/upathlib/serializer.py` & `upathlib-0.7.8b3/src/upathlib/serializer.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.8b2/PKG-INFO` & `upathlib-0.7.8b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upathlib
-Version: 0.7.8b2
+Version: 0.7.8b3
 Summary: The package *upathlib*
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

