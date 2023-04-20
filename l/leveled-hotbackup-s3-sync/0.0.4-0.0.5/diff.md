# Comparing `tmp/leveled_hotbackup_s3_sync-0.0.4-py3-none-any.whl.zip` & `tmp/leveled_hotbackup_s3_sync-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,22 @@
-Zip file size: 12009 bytes, number of entries: 11
+Zip file size: 9303665 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      273 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/__init__.py
 -rw-r--r--  2.0 unx      273 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/__main__.py
--rw-r--r--  2.0 unx     4219 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/app.py
+-rw-r--r--  2.0 unx     4283 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/app.py
+-rwxr-xr-x  2.0 unx    29628 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/erlang.py
 -rw-r--r--  2.0 unx     1029 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/hints.py
--rw-r--r--  2.0 unx     2223 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/journal.py
--rw-r--r--  2.0 unx     2221 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/manifest.py
--rw-r--r--  2.0 unx     3801 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3419 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1011 b- defN 16-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.4.dist-info/RECORD
-11 files, 29914 bytes uncompressed, 10269 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx     2306 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/journal.py
+-rw-r--r--  2.0 unx     2375 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/manifest.py
+-rw-r--r--  2.0 unx     6888 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/tests/app_test.py
+-rw-r--r--  2.0 unx     8800 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/tests/data/MANIFESTS
+-rw-r--r--  2.0 unx  9324237 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/tests/data/testdata.tgz
+-rwxr-xr-x  2.0 unx    26324 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/tests/erlang_test.py
+-rw-r--r--  2.0 unx     3250 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/tests/hints_test.py
+-rw-r--r--  2.0 unx     6419 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/tests/journal_test.py
+-rw-r--r--  2.0 unx    10195 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/tests/manifest_test.py
+-rw-r--r--  2.0 unx    43377 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/tests/utils_test.py
+-rw-r--r--  2.0 unx     3927 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3420 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1935 b- defN 16-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.5.dist-info/RECORD
+20 files, 9490384 bytes uncompressed, 9300433 bytes compressed:  2.0%
```

## zipnote {}

```diff
@@ -3,32 +3,59 @@
 
 Filename: leveled_hotbackup_s3_sync/__main__.py
 Comment: 
 
 Filename: leveled_hotbackup_s3_sync/app.py
 Comment: 
 
+Filename: leveled_hotbackup_s3_sync/erlang.py
+Comment: 
+
 Filename: leveled_hotbackup_s3_sync/hints.py
 Comment: 
 
 Filename: leveled_hotbackup_s3_sync/journal.py
 Comment: 
 
 Filename: leveled_hotbackup_s3_sync/manifest.py
 Comment: 
 
+Filename: leveled_hotbackup_s3_sync/tests/app_test.py
+Comment: 
+
+Filename: leveled_hotbackup_s3_sync/tests/data/MANIFESTS
+Comment: 
+
+Filename: leveled_hotbackup_s3_sync/tests/data/testdata.tgz
+Comment: 
+
+Filename: leveled_hotbackup_s3_sync/tests/erlang_test.py
+Comment: 
+
+Filename: leveled_hotbackup_s3_sync/tests/hints_test.py
+Comment: 
+
+Filename: leveled_hotbackup_s3_sync/tests/journal_test.py
+Comment: 
+
+Filename: leveled_hotbackup_s3_sync/tests/manifest_test.py
+Comment: 
+
+Filename: leveled_hotbackup_s3_sync/tests/utils_test.py
+Comment: 
+
 Filename: leveled_hotbackup_s3_sync/utils.py
 Comment: 
 
-Filename: leveled_hotbackup_s3_sync-0.0.4.dist-info/LICENSE
+Filename: leveled_hotbackup_s3_sync-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: leveled_hotbackup_s3_sync-0.0.4.dist-info/METADATA
+Filename: leveled_hotbackup_s3_sync-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: leveled_hotbackup_s3_sync-0.0.4.dist-info/WHEEL
+Filename: leveled_hotbackup_s3_sync-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: leveled_hotbackup_s3_sync-0.0.4.dist-info/RECORD
+Filename: leveled_hotbackup_s3_sync-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## leveled_hotbackup_s3_sync/app.py

```diff
@@ -1,10 +1,11 @@
 import argparse
 import os
 import os.path
+from typing import Union
 from urllib.parse import urlparse
 
 from leveled_hotbackup_s3_sync.journal import (
     maybe_download_journal,
     maybe_upload_journal,
     update_journal_filename,
 )
@@ -16,15 +17,15 @@
     save_local_manifest,
     upload_manifests,
     upload_new_manifest,
 )
 from leveled_hotbackup_s3_sync.utils import swap_path
 
 
-def backup(source: str, destination: str, create_hints_files: bool, endpoint: str) -> None:
+def backup(source: str, destination: str, create_hints_files: bool, endpoint: Union[str, None]) -> None:
     s3_manifests = []
     partitions = os.listdir(source)
     for partition in partitions:
         manifest_filename = os.path.join(source, partition, "journal/journal_manifest/0.man")
         print(f"Starting to process {manifest_filename}")
         manifest = read_manifest(manifest_filename)
 
@@ -34,29 +35,29 @@
             new_manifest.append(update_journal_filename(journal, source, destination))
 
         s3_path = upload_new_manifest(new_manifest, partition, destination, endpoint)
         s3_manifests.append(s3_path)
     upload_manifests(s3_manifests, destination, endpoint)
 
 
-def restore(source: str, version: str, destination: str, endpoint: str) -> None:
+def restore(source: str, version: str, destination: str, endpoint: Union[str, None]) -> None:
     manifests_list = get_manifests(source, version, endpoint)
     for manifest_path_version in manifests_list:
         print(f"Starting to process {manifest_path_version[0]}")
         manifest = read_s3_manifest(manifest_path_version[0], manifest_path_version[1], endpoint)
 
         new_manifest = []
         for journal in manifest:
             maybe_download_journal(journal, source, destination, endpoint)
             new_manifest.append(update_journal_filename(journal, source, destination))
         manifest_filename = swap_path(manifest_path_version[0], source, destination)
         save_local_manifest(new_manifest, manifest_filename)
 
 
-def list_versions(destination: str, endpoint: str) -> None:
+def list_versions(destination: str, endpoint: Union[str, None]) -> None:
     manifest_versions = get_manifests_versions(destination, endpoint)
     for manifest in manifest_versions:
         print(manifest["LastModified"], manifest["VersionId"])
 
 
 def check_s3_url(url: str) -> str:
     parsed_url = urlparse(url)
```

## leveled_hotbackup_s3_sync/journal.py

```diff
@@ -1,10 +1,12 @@
+from typing import Union
+
 import cdblib
-import erlang
 
+from leveled_hotbackup_s3_sync import erlang
 from leveled_hotbackup_s3_sync.hints import create_hints_file
 from leveled_hotbackup_s3_sync.utils import (
     download_file_from_s3,
     ensure_parent_dir_exists,
     local_path_exists,
     s3_path_exists,
     swap_path,
@@ -14,15 +16,15 @@
 
 def list_keys(filename: str) -> list:
     with cdblib.Reader.from_file_path(filename) as reader:
         return [erlang.binary_to_term(x) for x in reader.keys()]
 
 
 def maybe_upload_journal(
-    journal: tuple, source: str, destination: str, create_hints_files: bool, endpoint: str
+    journal: tuple, source: str, destination: str, create_hints_files: bool, endpoint: Union[str, None]
 ) -> None:
     journal_filename = f"{journal[1].decode('utf-8')}.cdb"
     journal_s3_path = swap_path(journal_filename, source, destination)
 
     if s3_path_exists(journal_s3_path, endpoint):
         print(f"{journal_s3_path} already exists")
     else:
@@ -36,15 +38,15 @@
             print(f"Uploading {hints_filename} to {hints_s3_path}")
             upload_file_to_s3(hints_filename, hints_s3_path, endpoint)
 
         print(f"Uploading {journal_filename} to {journal_s3_path}")
         upload_file_to_s3(journal_filename, journal_s3_path, endpoint)
 
 
-def maybe_download_journal(journal: tuple, source: str, destination: str, endpoint: str) -> None:
+def maybe_download_journal(journal: tuple, source: str, destination: str, endpoint: Union[str, None]) -> None:
     journal_filename = f"{journal[1].decode('utf-8')}.cdb"
     journal_local_path = swap_path(journal_filename, source, destination)
 
     if local_path_exists(journal_local_path):
         print(f"{journal_local_path} already exists")
     else:
         print(f"Downloading {journal_filename} to {journal_local_path}")
```

## leveled_hotbackup_s3_sync/manifest.py

```diff
@@ -1,60 +1,60 @@
 import os.path
+from typing import Union
 
-import erlang
-
+from leveled_hotbackup_s3_sync import erlang
 from leveled_hotbackup_s3_sync.utils import (
     download_bytes_from_s3,
     ensure_parent_dir_exists,
     list_s3_object_versions,
     upload_bytes_to_s3,
 )
 
 
 def read_manifest(filename: str) -> list:
     with open(filename, "rb") as file_handle:
         manifest = erlang.binary_to_term(file_handle.read())
     return manifest
 
 
-def read_s3_manifest(s3_path: str, version: str, endpoint: str) -> list:
+def read_s3_manifest(s3_path: str, version: str, endpoint: Union[str, None]) -> list:
     manifest_data = download_bytes_from_s3(s3_path, endpoint, version=version)
     manifest = erlang.binary_to_term(manifest_data)
     return manifest
 
 
 def save_local_manifest(new_manifest: list, filename: str) -> None:
     ensure_parent_dir_exists(filename)
-    manifest = erlang.term_to_binary(new_manifest)
+    manifest = erlang.term_to_binary(new_manifest, compressed=True)
     print(f"Saving new manifest to {filename}")
     with open(filename, "wb") as file_handle:
         file_handle.write(manifest)
 
 
-def upload_new_manifest(new_manifest: list, partition: str, destination: str, endpoint: str) -> str:
-    manifest = erlang.term_to_binary(new_manifest)
+def upload_new_manifest(new_manifest: list, partition: str, destination: str, endpoint: Union[str, None]) -> str:
+    manifest = erlang.term_to_binary(new_manifest, compressed=True)
     s3_path = os.path.join(destination, partition, "journal/journal_manifest/0.man")
     print(f"Uploading new manifest to {s3_path}")
     version_id = upload_bytes_to_s3(manifest, s3_path, endpoint)
     return f"{s3_path}#{version_id}"
 
 
-def upload_manifests(s3_manifests: list, destination: str, endpoint: str) -> None:
+def upload_manifests(s3_manifests: list, destination: str, endpoint: Union[str, None]) -> None:
     manifests_data = "\n".join(s3_manifests).encode("utf-8")
     s3_path = get_manifests_path(destination)
     print(f"Uploading manifest list to {s3_path}")
     upload_bytes_to_s3(manifests_data, s3_path, endpoint)
 
 
-def get_manifests_versions(destination: str, endpoint: str) -> list:
+def get_manifests_versions(destination: str, endpoint: Union[str, None]) -> list:
     s3_path = get_manifests_path(destination)
     return list_s3_object_versions(s3_path, endpoint)
 
 
-def get_manifests(source: str, version: str, endpoint: str) -> list:
+def get_manifests(source: str, version: str, endpoint: Union[str, None]) -> list:
     s3_path = get_manifests_path(source)
     manifests_data = download_bytes_from_s3(s3_path, endpoint, version=version)
     manifests = []
     for line in manifests_data.decode("utf-8").split("\n"):
         linedata = line.split("#")
         manifests.append((linedata[0], linedata[1]))
     return manifests
```

## leveled_hotbackup_s3_sync/utils.py

```diff
@@ -1,17 +1,18 @@
 import hashlib
 import os
 import os.path
 from typing import Tuple, Union
 from urllib.parse import urlparse
 
 import boto3
-import erlang
 from botocore.errorfactory import ClientError
 
+from leveled_hotbackup_s3_sync import erlang
+
 MAX_SHA_INT = 1461501637330902918203684832716283019655932542975
 
 
 def parse_s3_url(path: str) -> Tuple[str, str]:
     parsed_url = urlparse(path)
     if parsed_url.scheme != "s3":
         raise ValueError
@@ -20,53 +21,53 @@
     return bucket, key
 
 
 def swap_path(filename: str, source: str, destination: str) -> str:
     return os.path.join(destination, os.path.relpath(filename, source))
 
 
-def s3_path_exists(s3_path: str, endpoint: str) -> bool:
+def s3_path_exists(s3_path: str, endpoint: Union[str, None]) -> bool:
     s3_client = boto3.client("s3", endpoint_url=endpoint)
     bucket, key = parse_s3_url(s3_path)
     try:
         s3_client.head_object(Bucket=bucket, Key=key)
     except ClientError as err:
         if err.response["Error"]["Code"] == "404":
             return False
         raise err
     return True
 
 
-def upload_file_to_s3(source: str, destination: str, endpoint: str) -> None:
+def upload_file_to_s3(source: str, destination: str, endpoint: Union[str, None]) -> None:
     s3_client = boto3.client("s3", endpoint_url=endpoint)
     bucket, key = parse_s3_url(destination)
     s3_client.upload_file(source, bucket, key)
 
 
-def upload_bytes_to_s3(data: bytes, destination: str, endpoint: str) -> str:
+def upload_bytes_to_s3(data: bytes, destination: str, endpoint: Union[str, None]) -> str:
     s3_client = boto3.client("s3", endpoint_url=endpoint)
     bucket, key = parse_s3_url(destination)
     response = s3_client.put_object(Body=data, Bucket=bucket, Key=key)
     return response["VersionId"]
 
 
-def list_s3_object_versions(s3_path: str, endpoint: str) -> list:
+def list_s3_object_versions(s3_path: str, endpoint: Union[str, None]) -> list:
     s3_client = boto3.client("s3", endpoint_url=endpoint)
     bucket, key = parse_s3_url(s3_path)
     response = s3_client.list_object_versions(Bucket=bucket, Prefix=key)
     return response["Versions"]
 
 
-def download_file_from_s3(s3_path: str, local_path: str, endpoint: str) -> None:
+def download_file_from_s3(s3_path: str, local_path: str, endpoint: Union[str, None]) -> None:
     s3_client = boto3.client("s3", endpoint_url=endpoint)
     bucket, key = parse_s3_url(s3_path)
     s3_client.download_file(bucket, key, local_path)
 
 
-def download_bytes_from_s3(s3_path: str, endpoint: str, version: Union[str, None] = None) -> bytes:
+def download_bytes_from_s3(s3_path: str, endpoint: Union[str, None], version: Union[str, None] = None) -> bytes:
     s3_client = boto3.client("s3", endpoint_url=endpoint)
     bucket, key = parse_s3_url(s3_path)
     if version:
         response = s3_client.get_object(Bucket=bucket, Key=key, VersionId=version)
     else:
         response = s3_client.get_object(Bucket=bucket, Key=key)
     return response["Body"].read()
@@ -93,15 +94,15 @@
 def hash_bucket_key(bucket: bytes, bkey: bytes, buckettype: Union[bytes, None] = None) -> int:
     if buckettype:
         bucket_key = (
             (erlang.OtpErlangBinary(buckettype, bits=8), erlang.OtpErlangBinary(bucket, bits=8)),
             erlang.OtpErlangBinary(bkey, bits=8),
         )
     else:
-        bucket_key = (erlang.OtpErlangBinary(bucket, bits=8), erlang.OtpErlangBinary(bkey, bits=8))
+        bucket_key = (erlang.OtpErlangBinary(bucket, bits=8), erlang.OtpErlangBinary(bkey, bits=8))  # type: ignore
     hashed_bucket_key = hashlib.sha1(erlang.term_to_binary(bucket_key)).digest()
     return int.from_bytes(hashed_bucket_key, byteorder="big")
 
 
 def find_primary_partition(ring_size: int, bucket: bytes, bkey: bytes, buckettype: Union[bytes, None] = None) -> int:
     key_index = hash_bucket_key(bucket, bkey, buckettype)
     ring = riak_ring_indexes(ring_size)
```

## Comparing `leveled_hotbackup_s3_sync-0.0.4.dist-info/LICENSE` & `leveled_hotbackup_s3_sync-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `leveled_hotbackup_s3_sync-0.0.4.dist-info/METADATA` & `leveled_hotbackup_s3_sync-0.0.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: leveled-hotbackup-s3-sync
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool to syncrhonise LevelEd hotbackup files to Amazon S3
 Home-page: https://github.com/yorkshire-steve/leveled-hotbackup-s3-sync
 License: Apache-2.0
 Keywords: riak,leveled,backup,s3
 Author: yorkshire-steve
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.114,<2.0.0)
-Requires-Dist: erlang-py (>=2.0.5,<3.0.0)
+Requires-Dist: frozendict (>=2.3.7,<3.0.0)
 Requires-Dist: pure-cdb (>=4.0.0,<5.0.0)
 Project-URL: Repository, https://github.com/yorkshire-steve/leveled-hotbackup-s3-sync
 Description-Content-Type: text/markdown
 
 # leveled-hotbackup-s3-sync
 A Python 3.8 tool which can backup and restore leveled hotbackups with Amazon S3
```

