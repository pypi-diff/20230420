# Comparing `tmp/cwsearch_utils-0.1.7-py3-none-any.whl.zip` & `tmp/cwsearch_utils-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5635 bytes, number of entries: 8
+Zip file size: 5632 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 04:52 cwsearch_utils/__init__.py
--rw-rw-r--  2.0 unx     7900 b- defN 23-Apr-19 17:53 cwsearch_utils/aggregate.py
+-rw-rw-r--  2.0 unx     7836 b- defN 23-Apr-20 04:42 cwsearch_utils/aggregate.py
 -rw-rw-r--  2.0 unx      210 b- defN 23-Apr-19 17:07 cwsearch_utils/infinstor_dbutils.py
 -rw-rw-r--  2.0 unx     4780 b- defN 23-Apr-18 00:21 cwsearch_utils/infinstor_lock.py
--rw-rw-r--  2.0 unx      570 b- defN 23-Apr-19 17:54 cwsearch_utils-0.1.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 17:54 cwsearch_utils-0.1.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-19 17:54 cwsearch_utils-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      669 b- defN 23-Apr-19 17:54 cwsearch_utils-0.1.7.dist-info/RECORD
-8 files, 14236 bytes uncompressed, 4453 bytes compressed:  68.7%
+-rw-rw-r--  2.0 unx      570 b- defN 23-Apr-20 04:43 cwsearch_utils-0.1.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 04:43 cwsearch_utils-0.1.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-20 04:43 cwsearch_utils-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      669 b- defN 23-Apr-20 04:43 cwsearch_utils-0.1.8.dist-info/RECORD
+8 files, 14172 bytes uncompressed, 4450 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: cwsearch_utils/infinstor_dbutils.py
 Comment: 
 
 Filename: cwsearch_utils/infinstor_lock.py
 Comment: 
 
-Filename: cwsearch_utils-0.1.7.dist-info/METADATA
+Filename: cwsearch_utils-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: cwsearch_utils-0.1.7.dist-info/WHEEL
+Filename: cwsearch_utils-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: cwsearch_utils-0.1.7.dist-info/top_level.txt
+Filename: cwsearch_utils-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: cwsearch_utils-0.1.7.dist-info/RECORD
+Filename: cwsearch_utils-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cwsearch_utils/aggregate.py

```diff
@@ -14,21 +14,14 @@
         if nm in ner_entities:
             full = ner_entities[nm] + dct[nm]
         else:
             full = dct[nm]
         full.sort(reverse=True, key=my_sort_fnx)
         ner_entities[nm] = full[:100]
 
-def update_cache(infinstor_time_spec, tfile, s3client, bucket, prefix):
-    object_name = f"{prefix}/index/{infinstor_time_spec}/names.json"
-    try:
-        response = s3client.upload_file(tfile, bucket, object_name)
-    except Exception as ex:
-        print(f"Caught {ex} while uploading names entry for timespec {infinstor_time_spec}. Objectname={object_name}")
-
 def my_filelisting_sort_fnx(a):
     return a[2]
 
 def get_files_list_one_group(s3client, bucket, prefix, olg, resources, rv):
     print(f"get_files_list_one_group: Entered. group={olg}")
     if olg:
         prefix = prefix + olg
@@ -154,16 +147,20 @@
         print(f'Caught {ex} while list_objects_v2 of {bucket} prefix {prefix} time {infinstor_time_spec}', flush=True)
 
     print(f"Reverse Chronological Order Files:")
     for fl in files:
         print(f"{fl[2]} : sz={fl[1]} : {fl[0]}", flush=True)
 
     # next, read each file and fill ner_entities
+    if tag:
+        tfname = f"names-{tag}.db"
+    else:
+        tfname = "names.db"
     tdir = tempfile.mkdtemp()
-    tfile = os.path.join(tdir, "names.db")
+    tfile = os.path.join(tdir, tfname)
     con = sqlite3.connect(tfile)
     infinstor_dbutils.create_table(con)
 
     ner_entities = {}
     total_sz = 0
     for one_entry in files:
         print(f"Processing file {one_entry[0]} last_modified {one_entry[2]}")
@@ -180,9 +177,14 @@
             print(f"Stopping after working for {delta.total_seconds()} seconds")
             break
         else:
             print(f"Continuing after working for {delta.total_seconds()} seconds")
     con.close()
 
     # finally, write ner_entites to s3
-    update_cache(infinstor_time_spec, tfile, s3client, bucket, prefix)
+    object_name = f"{prefix}/index/{infinstor_time_spec}/{tfname}"
+    try:
+        response = s3client.upload_file(tfile, bucket, object_name)
+    except Exception as ex:
+        print(f"Caught {ex} while uploading names entry for timespec {infinstor_time_spec}. Objectname={object_name}")
+
     return ner_entities
```

## Comparing `cwsearch_utils-0.1.7.dist-info/METADATA` & `cwsearch_utils-0.1.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwsearch-utils
-Version: 0.1.7
+Version: 0.1.8
 Summary: InfinStor InfinLogs CloudWatch Search Utilities
 Home-page: https://infinstor.com/
 Author: InfinStor, Inc.
 Author-email: support@infinstor.com
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

