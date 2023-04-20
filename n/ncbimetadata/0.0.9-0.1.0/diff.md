# Comparing `tmp/ncbimetadata-0.0.9.tar.gz` & `tmp/ncbimetadata-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncbimetadata-0.0.9.tar", last modified: Thu Apr 20 10:29:17 2023, max compression
+gzip compressed data, was "ncbimetadata-0.1.0.tar", last modified: Thu Apr 20 11:28:27 2023, max compression
```

## Comparing `ncbimetadata-0.0.9.tar` & `ncbimetadata-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:29:17.345615 ncbimetadata-0.0.9/
--rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.0.9/LICENSE
--rw-r--r--   0 taiyuan    (501) staff       (20)     3075 2023-04-20 10:29:17.345491 ncbimetadata-0.0.9/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.0.9/README.md
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:29:17.343789 ncbimetadata-0.0.9/bin/
--rw-r--r--   0 taiyuan    (501) staff       (20)      152 2023-04-20 08:50:52.000000 ncbimetadata-0.0.9/bin/ncbimetadata
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:29:17.344233 ncbimetadata-0.0.9/ncbimetadata/
--rw-r--r--   0 taiyuan    (501) staff       (20)    11112 2023-04-20 08:02:11.000000 ncbimetadata-0.0.9/ncbimetadata/__init__.py
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:29:17.345318 ncbimetadata-0.0.9/ncbimetadata.egg-info/
--rw-r--r--   0 taiyuan    (501) staff       (20)     3075 2023-04-20 10:29:17.000000 ncbimetadata-0.0.9/ncbimetadata.egg-info/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)      282 2023-04-20 10:29:17.000000 ncbimetadata-0.0.9/ncbimetadata.egg-info/SOURCES.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 10:29:17.000000 ncbimetadata-0.0.9/ncbimetadata.egg-info/dependency_links.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 10:27:53.000000 ncbimetadata-0.0.9/ncbimetadata.egg-info/not-zip-safe
--rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 10:29:17.000000 ncbimetadata-0.0.9/ncbimetadata.egg-info/requires.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 10:29:17.000000 ncbimetadata-0.0.9/ncbimetadata.egg-info/top_level.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 10:29:17.345656 ncbimetadata-0.0.9/setup.cfg
--rw-r--r--   0 taiyuan    (501) staff       (20)      910 2023-04-20 10:27:57.000000 ncbimetadata-0.0.9/setup.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 11:28:27.708372 ncbimetadata-0.1.0/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.1.0/LICENSE
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3061 2023-04-20 11:28:27.708253 ncbimetadata-0.1.0/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.1.0/README.md
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 11:28:27.706941 ncbimetadata-0.1.0/ncbimetadata/
+-rw-r--r--   0 taiyuan    (501) staff       (20)       81 2023-04-20 11:24:39.000000 ncbimetadata-0.1.0/ncbimetadata/__init__.py
+-rw-r--r--   0 taiyuan    (501) staff       (20)    10958 2023-04-20 11:26:15.000000 ncbimetadata-0.1.0/ncbimetadata/core.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 11:28:27.708070 ncbimetadata-0.1.0/ncbimetadata.egg-info/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3061 2023-04-20 11:28:27.000000 ncbimetadata-0.1.0/ncbimetadata.egg-info/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)      290 2023-04-20 11:28:27.000000 ncbimetadata-0.1.0/ncbimetadata.egg-info/SOURCES.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 11:28:27.000000 ncbimetadata-0.1.0/ncbimetadata.egg-info/dependency_links.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       51 2023-04-20 11:28:27.000000 ncbimetadata-0.1.0/ncbimetadata.egg-info/entry_points.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 11:28:27.000000 ncbimetadata-0.1.0/ncbimetadata.egg-info/requires.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 11:28:27.000000 ncbimetadata-0.1.0/ncbimetadata.egg-info/top_level.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 11:28:27.708438 ncbimetadata-0.1.0/setup.cfg
+-rw-r--r--   0 taiyuan    (501) staff       (20)      807 2023-04-20 11:28:05.000000 ncbimetadata-0.1.0/setup.py
```

### Comparing `ncbimetadata-0.0.9/LICENSE` & `ncbimetadata-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.9/PKG-INFO` & `ncbimetadata-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.0.9
+Version: 0.1.0
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
 Home-page: https://github.com/RyanYuanSun/ncbimetadata
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
@@ -22,16 +22,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Platform: Linux
-Platform: MacOS X
+Requires-Python: >3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ncbimetadata
 ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and converting to csv format.
 <hr>
```

### Comparing `ncbimetadata-0.0.9/README.md` & `ncbimetadata-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.9/ncbimetadata/__init__.py` & `ncbimetadata-0.1.0/ncbimetadata/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,56 +153,52 @@
     request_payload = '{"page_size":1000,"page_token":null,"returned_content":"COMPLETE","taxons":["' + str(taxon_id) + '"]}'
     try:
         result_page = requests.post("https://api.ncbi.nlm.nih.gov/datasets/v2alpha/genome/dataset_report", data=request_payload)
         return result_page.json()['total_count']
     except:
         return -1
 
-def main():
+def run():
     parser = argparse.ArgumentParser()
     parser.add_argument("-id", "--taxon_id", type=int, help="the taxon ID", required=True)
     parser.add_argument("-t", "--thread_num", type=int, help="number of threads", default=1)
 
     args = parser.parse_args()
     # print(args)
 
     taxon_id = args.taxon_id
     multi_proc_num = args.thread_num
 
     if multi_proc_num <= 0:
         raise ValueError("Bad argument: -t")
 
-    print("Checking taxon ID...", end="")
+    print("Collecting metadata...")
     total_links_count = check_taxon(taxon_id)
     if total_links_count <= 0:
         raise InvalidTaxonException("Bad taxon ID")
-    print("Done.")
 
-    print("Searching NCBI database...", end="")
     manager = multiprocessing.Manager()
     accession_list = manager.list()
     process_collect_links = multiprocessing.Process(target=collect_links, args=(taxon_id, accession_list))
     # process_watcher = multiprocessing.Process(target=watcher, args=(total_links_count, accession_list))
     process_collect_links.start()
     # process_watcher.start()
     process_collect_links.join()
     # process_watcher.join()
-    print("Found: " + str(total_links_count))
 
     job_pool = []
     i = 0
     while i < len(accession_list):
         if (i + multi_proc_num - 1) <= (len(accession_list) - 1):
             job_pool.append(accession_list[i:(i + multi_proc_num)])
             i += multi_proc_num
         else:
             job_pool.append(accession_list[i:])
             i += multi_proc_num
 
-    print("Collecting metadata...")
     data = manager.list()
     data_failed = manager.list()
     process_watcher = multiprocessing.Process(target=watcher, args=(total_links_count, data, data_failed))
     process_collect_data = multiprocessing.Process(target=collect_data, args=(job_pool, data, data_failed))
     process_collect_data.start()
     process_watcher.start()
     process_collect_data.join()
@@ -256,8 +252,8 @@
 
     # output
     with open('result_taxonid_' + str(taxon_id) + '_time_' + str(time.time()) + '.csv', 'w+') as out:
         writer = csv.writer(out)
         writer.writerow(headers)
         for row in data_sorted:
             writer.writerow(row)
-    print('Results: ' + 'result_taxonid_' + str(taxon_id) + '_time_' + str(time.time()) + '.csv')
+    print('Filename: ' + 'result_taxonid_' + str(taxon_id) + '_time_' + str(time.time()) + '.csv')
```

### Comparing `ncbimetadata-0.0.9/ncbimetadata.egg-info/PKG-INFO` & `ncbimetadata-0.1.0/ncbimetadata.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.0.9
+Version: 0.1.0
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
 Home-page: https://github.com/RyanYuanSun/ncbimetadata
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
@@ -22,16 +22,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Platform: Linux
-Platform: MacOS X
+Requires-Python: >3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ncbimetadata
 ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and converting to csv format.
 <hr>
```

### Comparing `ncbimetadata-0.0.9/setup.py` & `ncbimetadata-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 from setuptools import setup
-import sys
-import os
 
 
 def readfile(filename):
     with open(filename, 'r+') as f:
         return f.read()
 
 
-if sys.platform == 'win32' or os.name == 'nt':
-    script = "bin/ncbimetadata.exe"
-else:
-    script = "bin/ncbimetadata"
-
-
 setup(
     name="ncbimetadata",
-    version="0.0.9",
+    version="0.1.0",
     description="ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!",
     long_description=readfile('README.md'),
     long_description_content_type='text/markdown',
     author="Ryan Alloriadonis",
     author_email="yuantai78@gmail.com",
     url="https://github.com/RyanYuanSun/ncbimetadata",
-    platforms=['Linux', 'MacOS X'],
     py_modules=['ncbimetadata'],
+    python_requires='>3',
     packages=['ncbimetadata'],
     license=readfile('LICENSE'),
-    scripts=[script],
     install_requires=[
           'requests',
       ],
-    zip_safe=False
+    entry_points={
+        'console_scripts': ['ncbimetadata=ncbimetadata:main']
+        },
 )
```

