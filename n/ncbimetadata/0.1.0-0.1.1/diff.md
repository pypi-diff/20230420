# Comparing `tmp/ncbimetadata-0.1.0.tar.gz` & `tmp/ncbimetadata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncbimetadata-0.1.0.tar", last modified: Thu Apr 20 11:28:27 2023, max compression
+gzip compressed data, was "ncbimetadata-0.1.1.tar", last modified: Thu Apr 20 15:28:17 2023, max compression
```

## Comparing `ncbimetadata-0.1.0.tar` & `ncbimetadata-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 11:28:27.708372 ncbimetadata-0.1.0/
--rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.1.0/LICENSE
--rw-r--r--   0 taiyuan    (501) staff       (20)     3061 2023-04-20 11:28:27.708253 ncbimetadata-0.1.0/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.1.0/README.md
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 11:28:27.706941 ncbimetadata-0.1.0/ncbimetadata/
--rw-r--r--   0 taiyuan    (501) staff       (20)       81 2023-04-20 11:24:39.000000 ncbimetadata-0.1.0/ncbimetadata/__init__.py
--rw-r--r--   0 taiyuan    (501) staff       (20)    10958 2023-04-20 11:26:15.000000 ncbimetadata-0.1.0/ncbimetadata/core.py
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 11:28:27.708070 ncbimetadata-0.1.0/ncbimetadata.egg-info/
--rw-r--r--   0 taiyuan    (501) staff       (20)     3061 2023-04-20 11:28:27.000000 ncbimetadata-0.1.0/ncbimetadata.egg-info/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)      290 2023-04-20 11:28:27.000000 ncbimetadata-0.1.0/ncbimetadata.egg-info/SOURCES.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 11:28:27.000000 ncbimetadata-0.1.0/ncbimetadata.egg-info/dependency_links.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       51 2023-04-20 11:28:27.000000 ncbimetadata-0.1.0/ncbimetadata.egg-info/entry_points.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 11:28:27.000000 ncbimetadata-0.1.0/ncbimetadata.egg-info/requires.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 11:28:27.000000 ncbimetadata-0.1.0/ncbimetadata.egg-info/top_level.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 11:28:27.708438 ncbimetadata-0.1.0/setup.cfg
--rw-r--r--   0 taiyuan    (501) staff       (20)      807 2023-04-20 11:28:05.000000 ncbimetadata-0.1.0/setup.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 15:28:17.592576 ncbimetadata-0.1.1/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.1.1/LICENSE
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3061 2023-04-20 15:28:17.592374 ncbimetadata-0.1.1/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.1.1/README.md
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 15:28:17.590797 ncbimetadata-0.1.1/ncbimetadata/
+-rw-r--r--   0 taiyuan    (501) staff       (20)       81 2023-04-20 11:24:39.000000 ncbimetadata-0.1.1/ncbimetadata/__init__.py
+-rw-r--r--   0 taiyuan    (501) staff       (20)    11000 2023-04-20 15:24:04.000000 ncbimetadata-0.1.1/ncbimetadata/core.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 15:28:17.592101 ncbimetadata-0.1.1/ncbimetadata.egg-info/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3061 2023-04-20 15:28:17.000000 ncbimetadata-0.1.1/ncbimetadata.egg-info/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)      290 2023-04-20 15:28:17.000000 ncbimetadata-0.1.1/ncbimetadata.egg-info/SOURCES.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 15:28:17.000000 ncbimetadata-0.1.1/ncbimetadata.egg-info/dependency_links.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       51 2023-04-20 15:28:17.000000 ncbimetadata-0.1.1/ncbimetadata.egg-info/entry_points.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 15:28:17.000000 ncbimetadata-0.1.1/ncbimetadata.egg-info/requires.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 15:28:17.000000 ncbimetadata-0.1.1/ncbimetadata.egg-info/top_level.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 15:28:17.592655 ncbimetadata-0.1.1/setup.cfg
+-rw-r--r--   0 taiyuan    (501) staff       (20)      807 2023-04-20 15:27:49.000000 ncbimetadata-0.1.1/setup.py
```

### Comparing `ncbimetadata-0.1.0/LICENSE` & `ncbimetadata-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.1.0/PKG-INFO` & `ncbimetadata-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.1.0
+Version: 0.1.1
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
 Home-page: https://github.com/RyanYuanSun/ncbimetadata
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
```

### Comparing `ncbimetadata-0.1.0/README.md` & `ncbimetadata-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.1.0/ncbimetadata/core.py` & `ncbimetadata-0.1.1/ncbimetadata/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,19 @@
     bogus_values = ['missing', 'n/a', 'not provided', 'not provided; submitted under MIGS 2.1', '', 'NA', '/', 'N/A',
                     'missed', 'not located', 'Not Applicable', 'Missing', 'unknown', 'Unknown', 'not collected',
                     'Not applicable', 'not applicable']
     detail_request_url = 'https://api.ncbi.nlm.nih.gov/datasets/v2alpha/genome/accession/' + accession + '/dataset_report?filters.assembly_version=all_assemblies&page_size=1000'
     try:
         result_detail = requests.get(url=detail_request_url)
     except:
-        data_failed.append(accession)
-        return
+        if accession not in data_failed:
+            data_failed.append(accession)
+            return
+        else:
+            return
 
     # RefSeq
     attributes.append(['RefSeq', result_detail.json()['reports'][0]['accession']])
 
     # Sample details
     biosample = result_detail.json()['reports'][0]['assembly_info']['biosample']
     if biosample['accession'] not in bogus_values:
@@ -92,17 +95,22 @@
     if 'gc_percent' in assembly_stats:
         attributes.append(['GC percent', assembly_stats['gc_percent']])
     if 'assembly_level' in assembly_info:
         attributes.append(['Assembly level', assembly_info['assembly_level']])
 
     try:
         data.append(attributes)
+        if accession in data_failed:
+            data_failed.remove(accession)
     except:
-        data_failed.append(accession)
-        return
+        if accession not in data_failed:
+            data_failed.append(accession)
+            return
+        else:
+            return
 
 
 def sub_process(job, data, data_failed):
     for accession in job:
         subProcess = multiprocessing.Process(target=worker, args=(accession, data, data_failed))
         subProcess.start()
 
@@ -137,14 +145,26 @@
         num = len(list) + len(list_2)
         i = round((num / total) * 100)
         progress_bar(num, total, i)
         if num == total:
             print()
             break
 
+def allocate_jobs(job_list, num_thread):
+    job_p = []
+    i = 0
+    while i < len(job_list):
+        if (i + num_thread - 1) <= (len(job_list) - 1):
+            job_p.append(job_list[i:(i + num_thread)])
+            i += num_thread
+        else:
+            job_p.append(job_list[i:])
+            i += num_thread
+    return job_p
+
 
 def progress_bar(done, total, i):
     # print("\r", end="")
     print("\r" + "▋" * (i // 4) + " {}% ".format(i) + "(" + str(done) + "/" + str(total) + ")", end="",
           flush=True)
     # sys.stdout.flush()
 
@@ -181,56 +201,40 @@
     process_collect_links = multiprocessing.Process(target=collect_links, args=(taxon_id, accession_list))
     # process_watcher = multiprocessing.Process(target=watcher, args=(total_links_count, accession_list))
     process_collect_links.start()
     # process_watcher.start()
     process_collect_links.join()
     # process_watcher.join()
 
-    job_pool = []
-    i = 0
-    while i < len(accession_list):
-        if (i + multi_proc_num - 1) <= (len(accession_list) - 1):
-            job_pool.append(accession_list[i:(i + multi_proc_num)])
-            i += multi_proc_num
-        else:
-            job_pool.append(accession_list[i:])
-            i += multi_proc_num
+    job_pool = allocate_jobs(accession_list, multi_proc_num)
 
     data = manager.list()
     data_failed = manager.list()
     process_watcher = multiprocessing.Process(target=watcher, args=(total_links_count, data, data_failed))
     process_collect_data = multiprocessing.Process(target=collect_data, args=(job_pool, data, data_failed))
     process_collect_data.start()
     process_watcher.start()
     process_collect_data.join()
     process_watcher.join()
 
     # retry
     while len(data_failed) > 0:
         retry = 1
         print("Number of failed requests:", len(data_failed))
+        print("Retying failed requests...")
 
         total_links_count_failed = len(data_failed)
-        job_pool = []
-        i = 0
-        while i < len(data_failed):
-            if (i + multi_proc_num - 1) <= (len(data_failed) - 1):
-                job_pool.append(data_failed[i:(i + multi_proc_num)])
-                i += multi_proc_num
-            else:
-                job_pool.append(data_failed[i:])
-                i += multi_proc_num
+        job_pool = allocate_jobs(data_failed, multi_proc_num)
 
-        data_failed = manager.list()
-        process_watcher = multiprocessing.Process(target=watcher, args=(total_links_count_failed, data_failed))
+        # process_watcher = multiprocessing.Process(target=watcher, args=(total_links_count_failed, data_failed))
         process_collect_data = multiprocessing.Process(target=collect_data, args=(job_pool, data, data_failed))
         process_collect_data.start()
-        process_watcher.start()
+        # process_watcher.start()
         process_collect_data.join()
-        process_watcher.join()
+        # process_watcher.join()
 
     # Sorting
     headers = []
     for item in data:
         for sub_item in item:
             if sub_item[0] not in headers:
                 headers.append(sub_item[0])
```

### Comparing `ncbimetadata-0.1.0/ncbimetadata.egg-info/PKG-INFO` & `ncbimetadata-0.1.1/ncbimetadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.1.0
+Version: 0.1.1
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
 Home-page: https://github.com/RyanYuanSun/ncbimetadata
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
```

### Comparing `ncbimetadata-0.1.0/setup.py` & `ncbimetadata-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readfile(filename):
     with open(filename, 'r+') as f:
         return f.read()
 
 
 setup(
     name="ncbimetadata",
-    version="0.1.0",
+    version="0.1.1",
     description="ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!",
     long_description=readfile('README.md'),
     long_description_content_type='text/markdown',
     author="Ryan Alloriadonis",
     author_email="yuantai78@gmail.com",
     url="https://github.com/RyanYuanSun/ncbimetadata",
     py_modules=['ncbimetadata'],
```

