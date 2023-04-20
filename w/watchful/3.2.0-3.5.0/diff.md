# Comparing `tmp/watchful-3.2.0.tar.gz` & `tmp/watchful-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchful-3.2.0.tar", last modified: Thu Apr 20 08:53:55 2023, max compression
+gzip compressed data, was "watchful-3.5.0.tar", last modified: Thu Apr  6 12:17:55 2023, max compression
```

## Comparing `watchful-3.2.0.tar` & `watchful-3.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:53:55.551729 watchful-3.2.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-04-20 08:49:57.000000 watchful-3.2.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      261 2023-04-20 08:49:57.000000 watchful-3.2.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2650 2023-04-20 08:53:55.551729 watchful-3.2.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6405 2023-04-20 08:49:57.000000 watchful-3.2.0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2064 2023-04-20 08:49:57.000000 watchful-3.2.0/README_PYPI.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1554 2023-04-20 08:49:57.000000 watchful-3.2.0/README_PY_ENV.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:53:55.547729 watchful-3.2.0/examples/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   325333 2023-04-20 08:49:57.000000 watchful-3.2.0/examples/api_intro.ipynb
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1892 2023-04-20 08:49:57.000000 watchful-3.2.0/examples/requirements_api_intro.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      998 2023-04-20 08:49:57.000000 watchful-3.2.0/pylama.ini
--rw-r--r--   0 circleci  (3434) circleci  (3434)      375 2023-04-20 08:49:57.000000 watchful-3.2.0/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      983 2023-04-20 08:53:55.555729 watchful-3.2.0/setup.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:53:55.543729 watchful-3.2.0/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:53:55.551729 watchful-3.2.0/src/watchful/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2023-04-20 08:49:57.000000 watchful-3.2.0/src/watchful/VERSION
--rw-r--r--   0 circleci  (3434) circleci  (3434)      575 2023-04-20 08:49:57.000000 watchful-3.2.0/src/watchful/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39611 2023-04-20 08:49:57.000000 watchful-3.2.0/src/watchful/attributes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    49386 2023-04-20 08:49:57.000000 watchful-3.2.0/src/watchful/client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15767 2023-04-20 08:49:57.000000 watchful-3.2.0/src/watchful/enrich.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6356 2023-04-20 08:49:57.000000 watchful-3.2.0/src/watchful/enricher.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:53:55.551729 watchful-3.2.0/src/watchful.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2650 2023-04-20 08:53:55.000000 watchful-3.2.0/src/watchful.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-04-20 08:53:55.000000 watchful-3.2.0/src/watchful.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-20 08:53:55.000000 watchful-3.2.0/src/watchful.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2023-04-20 08:53:55.000000 watchful-3.2.0/src/watchful.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-04-20 08:53:55.000000 watchful-3.2.0/src/watchful.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:53:55.551729 watchful-3.2.0/tests/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      388 2023-04-20 08:49:57.000000 watchful-3.2.0/tests/test_0000_import_sdk.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2691 2023-04-20 08:49:57.000000 watchful-3.2.0/tests/test_0001_sdk_version_and_default_conn.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      772 2023-04-20 08:49:57.000000 watchful-3.2.0/tests/test_0002_encoding.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-04-06 12:14:03.000000 watchful-3.5.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      261 2023-04-06 12:14:03.000000 watchful-3.5.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2650 2023-04-06 12:17:55.945730 watchful-3.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6405 2023-04-06 12:14:03.000000 watchful-3.5.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2064 2023-04-06 12:14:03.000000 watchful-3.5.0/README_PYPI.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1554 2023-04-06 12:14:03.000000 watchful-3.5.0/README_PY_ENV.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/examples/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   325333 2023-04-06 12:14:03.000000 watchful-3.5.0/examples/api_intro.ipynb
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1900 2023-04-06 12:14:03.000000 watchful-3.5.0/examples/requirements_api_intro.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      998 2023-04-06 12:14:03.000000 watchful-3.5.0/pylama.ini
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      375 2023-04-06 12:14:03.000000 watchful-3.5.0/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      983 2023-04-06 12:17:55.949730 watchful-3.5.0/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.941730 watchful-3.5.0/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/src/watchful/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/VERSION
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      575 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39332 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/attributes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    48367 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15767 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/enrich.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6356 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/enricher.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/src/watchful.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2650 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/tests/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      388 2023-04-06 12:14:03.000000 watchful-3.5.0/tests/test_0000_import_sdk.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2691 2023-04-06 12:14:03.000000 watchful-3.5.0/tests/test_0001_sdk_version_and_default_conn.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      772 2023-04-06 12:14:03.000000 watchful-3.5.0/tests/test_0002_encoding.py
```

### Comparing `watchful-3.2.0/LICENSE` & `watchful-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `watchful-3.2.0/PKG-INFO` & `watchful-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchful
-Version: 3.2.0
+Version: 3.5.0
 Summary: Watchful API for Interacting with Watchful Environment
 Home-page: https://github.com/Watchfulio/watchful-py
 Author: Watchful, Inc.
 Author-email: engineering@watchful.io
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/Watchfulio/watchful-py/issues
 Keywords: watchful
```

### Comparing `watchful-3.2.0/README.md` & `watchful-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `watchful-3.2.0/README_PYPI.md` & `watchful-3.5.0/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `watchful-3.2.0/README_PY_ENV.md` & `watchful-3.5.0/README_PY_ENV.md`

 * *Files identical despite different names*

### Comparing `watchful-3.2.0/examples/api_intro.ipynb` & `watchful-3.5.0/examples/api_intro.ipynb`

 * *Files identical despite different names*

### Comparing `watchful-3.2.0/examples/requirements_api_intro.txt` & `watchful-3.5.0/examples/requirements_api_intro.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 asttokens==2.2.1
 backcall==0.2.0
 beautifulsoup4==4.11.1
 blis==0.7.9
 bpemb==0.3.4
 catalogue==2.0.8
 certifi==2022.12.7
-charset-normalizer==3.1.0
+charset-normalizer==2.1.1
 click==8.1.3
 cloudpickle==2.2.0
 confection==0.0.3
 conllu==4.5.2
 contourpy==1.0.6
 cycler==0.11.0
 cymem==2.0.7
 decorator==4.4.2
 Deprecated==1.2.13
 entrypoints==0.4
 executing==1.2.0
 filelock==3.8.0
-flair==0.12.2
+flair==0.11.3
 fonttools==4.38.0
 ftfy==6.1.1
 future==0.18.3
 gdown==4.5.3
-gensim==4.3.1
-huggingface-hub==0.13.4
+gensim==4.3.0
+huggingface-hub==0.13.3
 hyperopt==0.2.7
 idna==3.4
 importlib-metadata==6.1.0
 ipykernel==5.3.4
 ipython==8.10.0
 ipython-genutils==0.2.0
 Janome==0.4.2
@@ -80,17 +80,17 @@
 scikit-learn==1.1.3
 scipy==1.9.3
 segtok==1.5.11
 sentencepiece==0.1.97
 setuptools==67.5.1
 six==1.16.0
 smart-open==6.3.0
-soupsieve==2.4
+soupsieve==2.3.2.post1
 spacy==3.4.3
-spacy-legacy==3.0.12
+spacy-legacy==3.0.10
 spacy-loggers==1.0.3
 spacytextblob==4.0.0
 sqlitedict==2.1.0
 srsly==2.4.6
 stack-data==0.6.2
 tabulate==0.9.0
 textblob==0.15.3
@@ -104,11 +104,11 @@
 transformers==4.26.1
 typer==0.7.0
 typing_extensions==4.4.0
 urllib3==1.26.13
 wasabi==0.10.1
 watchful==1.2.0
 wcwidth==0.2.5
-wheel==0.40.0
+wheel==0.38.1
 Wikipedia-API==0.5.4
 wrapt==1.14.1
 zipp==3.15.0
```

### Comparing `watchful-3.2.0/pylama.ini` & `watchful-3.5.0/pylama.ini`

 * *Files identical despite different names*

### Comparing `watchful-3.2.0/setup.cfg` & `watchful-3.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `watchful-3.2.0/src/watchful/__init__.py` & `watchful-3.5.0/src/watchful/__init__.py`

 * *Files identical despite different names*

### Comparing `watchful-3.2.0/src/watchful/attributes.py` & `watchful-3.5.0/src/watchful/attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 ################################################################################
 
 
 import csv
 import io
 import json
+import numbers
 import os
 import pprint
 import re
 from heapq import merge
 from multiprocessing import Pool
 from typing import Callable, Dict, List, Optional, Tuple
 import psutil
@@ -267,25 +268,22 @@
             # Gather and create new mappings at the same time. Duh :)
             for attr, vals in attr_vals.items():
                 if attr not in attrs:
                     attrs[attr] = len(attrs) + 1
                     values[attr] = {}
                     new_attrs.append(attr)
                 for val in vals:
-                    if isinstance(val, (int, float, bool)):
+                    if isinstance(val, numbers.Number):
                         val = str(val)
-                    elif val is None:
-                        pass
-                    elif val == "" or not isinstance(val, str):
-                        raise ValueError(
-                            "Attribute value needs to be either a non-empty "
-                            f"string, int, float, bool or None; got {val} "
-                            "instead."
+                    elif val and not isinstance(val, str):
+                        raise Exception(
+                            "Attribute value must be a string, "
+                            "None or a number. Was: " + val
                         )
-                    if val and val not in values[attr]:
+                    if val and not val in values[attr]:
                         values[attr][val] = len(values[attr]) + 1
                         if attr not in new_values:
                             new_values[attr] = []
                         new_values[attr].append(val)
 
             # Create the vector for the current cell.
             span_val = []
@@ -295,20 +293,15 @@
                 assert len(span) == len(
                     vals
                 ), "Must be the same amount of spans as attribute values."
                 # Not base64 the attributes to save space since there aren't
                 # that many of them.
                 span_val.append(attrs[attr])
                 span_val.append(
-                    base64str(
-                        [
-                            0 if val is None else values[attr][str(val)]
-                            for val in vals
-                        ]
-                    )
+                    base64str([values[attr][val] if val else 0 for val in vals])
                 )
 
             cell.append(base64str(contig_spans(span)))
             cell.append(span_val)
 
         # Output the lines (attributes, values and the cell value itself).
         if new_attrs:
@@ -1175,13 +1168,13 @@
     summary = client._assert_success(summary)
     dataset_id = client.get_dataset_id(summary)
     datasets_dir = client.get_datasets_dir(summary, is_local)
 
     if in_file != "":
         # Check that ``in_file`` exists.
         if not os.path.isfile(in_file):
-            raise FileNotFoundError(f"File {in_file} does not exist.")
+            raise Exception(f"File {in_file} does not exist.")
         dataset_filepath = in_file
     else:
         dataset_filepath = client.get_dataset_filepath(summary, is_local)
 
     return dataset_id, datasets_dir, dataset_filepath
```

### Comparing `watchful-3.2.0/src/watchful/client.py` & `watchful-3.5.0/src/watchful/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         sock.settimeout(timeout_sec)
         res = sock.connect_ex((HOST, port))
         if res == 0:
             return None
         time.sleep(0.001)
 
-    raise TimeoutError("Timed out waiting for Watchful to start")
+    raise Exception("Timed out waiting for Watchful to start")
 
 
 def spawn_cmd(cmd: str, env: str = None) -> int:
     """
     This function spawns a command and returns the PID of the spawned process.
 
     :param cmd: The command.
@@ -129,15 +129,15 @@
         if pred(summary):
             return summary
         if prev_summary == summary:
             end = time.time_ns() + (unchanged_timeout * 1_000_000_000)
         prev_summary = summary
         time.sleep(0.03)  # 30ms sleep for ~30 requests per second
 
-    raise requests.exceptions.Timeout(
+    raise Exception(
         "Timed out awaiting summary. Summary went stale for "
         + str(unchanged_timeout)
         + " seconds"
     )
 
 
 def _assert_success(summary: Dict) -> Optional[Dict]:
@@ -152,15 +152,15 @@
     :rtype: Dict, optional
     """
 
     if "error_msg" in summary and summary["error_msg"]:
         verb_str = ""
         if "error_verb" in summary and summary["error_verb"]:
             verb_str = f' ({summary["error_verb"]})'
-        raise ValueError(f'Summary error{verb_str}: {summary["error_msg"]}')
+        raise Exception(f'Summary error{verb_str}: {summary["error_msg"]}')
 
     return summary
 
 
 # as used by register_summary_string_hook
 API_SUMMARY_HOOK_CALLBACK = None
 
@@ -427,15 +427,15 @@
     :return: The project id.
     :rtype: str
     """
 
     if "project_id" in summary:
         return summary["project_id"]
 
-    raise WatchfulAppInstanceError("No project is currently active.")
+    raise Exception("No project is currently active.")
 
 
 def get_dataset_id(summary: Dict) -> str:
     """
     This function gets the active dataset id from ``summary``. For correctness,
     we use the ``summary`` that has been success asserted via
     ``_assert_success``.
@@ -447,19 +447,19 @@
     :rtype: str
     """
 
     if "datasets" in summary:
         # ``dataset_ids`` should either be empty or contain one dataset id.
         dataset_ids = summary["datasets"]
         if len(dataset_ids) == 0:
-            raise WatchfulAppInstanceError("No dataset is currently opened.")
+            raise Exception("No dataset is currently opened.")
         dataset_id = dataset_ids[0]
         return dataset_id
 
-    raise WatchfulAppInstanceError("`datasets` is currently not available.")
+    raise Exception("`datasets` is currently not available.")
 
 
 def get_watchful_home(summary: Dict, is_local: bool = True) -> str:
     """
     This function gets Watchful home from ``summary``. For correctness, we use
     the summary that has been success asserted via ``_assert_success``. If
     Watchful home is not available and the Watchful application is local, we
@@ -478,17 +478,15 @@
     if "watchful_home" in summary:
         return summary["watchful_home"]
     if is_local:
         user_home = os.path.expanduser("~")
         watchful_home = os.path.join(user_home, "watchful")
         return watchful_home
 
-    raise WatchfulAppInstanceError(
-        "`watchful_home` is currently not available."
-    )
+    raise Exception("`watchful_home` is currently not available.")
 
 
 def get_datasets_dir(summary: Dict, is_local: bool = True) -> str:
     """
     This function infers the datasets directory from ``summary``. For
     correctness, we use the summary that has been success asserted via
     ``_assert_success``.
@@ -530,22 +528,22 @@
 
     datasets_dir = get_datasets_dir(summary, is_local)
     dataset_id = get_dataset_id(summary)
     dataset_ref_path = os.path.join(datasets_dir, "refs", dataset_id)
 
     # Check that ``dataset_ref_path`` exists.
     if not os.path.isfile(dataset_ref_path):
-        raise FileNotFoundError(f"File {dataset_ref_path} does not exist.")
+        raise Exception(f"File {dataset_ref_path} does not exist.")
     with open(dataset_ref_path, encoding="utf-8") as f:
         dataset_ref = f.readline()
     dataset_filepath = os.path.join(datasets_dir, "raw", dataset_ref)
 
     # Check that ``dataset_filepath`` exists.
     if not os.path.isfile(dataset_filepath):
-        raise FileNotFoundError(f"File {dataset_filepath} does not exist.")
+        raise Exception(f"File {dataset_filepath} does not exist.")
 
     return dataset_filepath
 
 
 # def poll():
 #     pass
 
@@ -1096,15 +1094,15 @@
         stream = export_stream().raw
         stream.auto_close = False
         reader = csv.reader(
             io.TextIOWrapper(stream, encoding="utf-8", newline="")
         )
         header = next(reader)
         if header[:n_cols] != fields:
-            raise ValueError(
+            raise Exception(
                 f"Dataset's column names {header} did not match the expected "
                 f"column names {fields}."
             )
         writer.writerow(fields)
         for row in reader:
             writer.writerow(row[:n_cols])
 
@@ -1193,20 +1191,20 @@
         accuracy, or not.
     :type is_fast: bool, optional
     :return: `True` if the detected encoding is utf-8 and has a confidence of
         the given threshold or more, otherwise `False`.
     :rtype: bool
     """
     if csv_bytes is None and filepath is None:
-        raise ValueError(
+        raise Exception(
             "Both filepath and csv_bytes are not specified. "
             "One of them needs to be specified."
         )
     if csv_bytes and filepath:
-        raise ValueError(
+        raise Exception(
             "Both filepath and csv_bytes are specified. "
             "Only one of them needs to be specified."
         )
 
     if is_fast:
         import cchardet as chardet
     else:
@@ -1215,15 +1213,15 @@
     if csv_bytes:
         res = chardet.detect(csv_bytes)
     else:
         if os.path.isfile(filepath):
             with open(filepath, "rb") as f:
                 res = chardet.detect(f.read())
         else:
-            raise FileNotFoundError(
+            raise Exception(
                 f"There is no file at the given file path {filepath}!"
             )
 
     # Because cChardet likes to be specific with encoding,
     # ASCII will be specified if the valid UTF-8 characters
     # fit within that subset.
     valid_encodings = ["utf-8", "ascii"]
@@ -1299,15 +1297,15 @@
         )
         dataset_id = _read_response(response)["id"]
 
         api("dataset_add", id=dataset_id, columns=columns)
 
         return dataset_id
 
-    raise Warning(
+    raise Exception(
         "Dataset is not loaded as the encoding of the csv dataset is not "
         "detected to be utf-8 and dataset loading is not forced."
     )
 
 
 def label_single(row: List[str]) -> List[str]:
     """
@@ -1600,35 +1598,7 @@
     :param token: The user's auth token, defaults to None.
     :type token: str, optional
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
     return hub_api("whoami", token)
-
-
-class WatchfulAppInstanceError(Exception):
-    """
-    This class specifies the exception raised for errors relating to the
-    watchful app instance.
-    """
-
-    base_error_message = (
-        "This is a watchful app instance related error and could be resolved "
-        "by for example, creating a project, and/or opening a project, and/or "
-        "and/or adding a dataset to it."
-    )
-
-    def __init__(self, error_message=""):
-        """
-        This function concatenates the base error message with the specific
-        error message.
-
-        :param error_message: The specific error message, defaults to "".
-        :type error_message: str, optional
-        """
-        self.error_message = (
-            " ".join([error_message, self.base_error_message])
-            if error_message
-            else self.base_error_message
-        )
-        super().__init__(self.error_message)
```

### Comparing `watchful-3.2.0/src/watchful/enrich.py` & `watchful-3.5.0/src/watchful/enrich.py`

 * *Files identical despite different names*

### Comparing `watchful-3.2.0/src/watchful/enricher.py` & `watchful-3.5.0/src/watchful/enricher.py`

 * *Files identical despite different names*

### Comparing `watchful-3.2.0/src/watchful.egg-info/PKG-INFO` & `watchful-3.5.0/src/watchful.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchful
-Version: 3.2.0
+Version: 3.5.0
 Summary: Watchful API for Interacting with Watchful Environment
 Home-page: https://github.com/Watchfulio/watchful-py
 Author: Watchful, Inc.
 Author-email: engineering@watchful.io
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/Watchfulio/watchful-py/issues
 Keywords: watchful
```

### Comparing `watchful-3.2.0/src/watchful.egg-info/SOURCES.txt` & `watchful-3.5.0/src/watchful.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `watchful-3.2.0/tests/test_0001_sdk_version_and_default_conn.py` & `watchful-3.5.0/tests/test_0001_sdk_version_and_default_conn.py`

 * *Files identical despite different names*

### Comparing `watchful-3.2.0/tests/test_0002_encoding.py` & `watchful-3.5.0/tests/test_0002_encoding.py`

 * *Files identical despite different names*

