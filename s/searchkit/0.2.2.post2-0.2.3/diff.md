# Comparing `tmp/searchkit-0.2.2.post2.tar.gz` & `tmp/searchkit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.2.2.post2.tar", last modified: Tue Apr 18 16:15:14 2023, max compression
+gzip compressed data, was "searchkit-0.2.3.tar", last modified: Thu Apr 20 14:49:42 2023, max compression
```

## Comparing `searchkit-0.2.2.post2.tar` & `searchkit-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-18 16:15:14.192248 searchkit-0.2.2.post2/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.2.post2/LICENSE
--rw-rw-r--   0 user1     (1000) user1     (1000)     3111 2023-04-18 16:15:14.192248 searchkit-0.2.2.post2/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     2897 2023-04-12 11:04:01.000000 searchkit-0.2.2.post2/README.md
--rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-04-17 12:11:23.000000 searchkit-0.2.2.post2/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-18 16:15:14.192248 searchkit-0.2.2.post2/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-04-18 13:47:52.000000 searchkit-0.2.2.post2/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    22833 2023-04-11 08:53:59.000000 searchkit-0.2.2.post2/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.2.post2/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    44374 2023-04-18 16:13:04.000000 searchkit-0.2.2.post2/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4743 2023-04-13 20:08:39.000000 searchkit-0.2.2.post2/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-18 16:15:14.192248 searchkit-0.2.2.post2/searchkit.egg-info/
--rw-rw-r--   0 user1     (1000) user1     (1000)     3111 2023-04-18 16:15:14.000000 searchkit-0.2.2.post2/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-04-18 16:15:14.000000 searchkit-0.2.2.post2/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-04-18 16:15:14.000000 searchkit-0.2.2.post2/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-04-18 16:15:14.000000 searchkit-0.2.2.post2/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-04-18 16:15:14.000000 searchkit-0.2.2.post2/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-04-18 16:15:14.192248 searchkit-0.2.2.post2/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.2.post2/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-20 14:49:42.931016 searchkit-0.2.3/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.3/LICENSE
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3105 2023-04-20 14:49:42.931016 searchkit-0.2.3/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2897 2023-04-12 11:04:01.000000 searchkit-0.2.3/README.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-04-17 12:11:23.000000 searchkit-0.2.3/pyproject.toml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-20 14:49:42.931016 searchkit-0.2.3/searchkit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-04-18 13:47:52.000000 searchkit-0.2.3/searchkit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    22833 2023-04-11 08:53:59.000000 searchkit-0.2.3/searchkit/constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.3/searchkit/log.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    44374 2023-04-18 16:13:04.000000 searchkit-0.2.3/searchkit/search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4743 2023-04-13 20:08:39.000000 searchkit-0.2.3/searchkit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-20 14:49:42.931016 searchkit-0.2.3/searchkit.egg-info/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3105 2023-04-20 14:49:42.000000 searchkit-0.2.3/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-04-20 14:49:42.000000 searchkit-0.2.3/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-04-20 14:49:42.000000 searchkit-0.2.3/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-04-20 14:49:42.000000 searchkit-0.2.3/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-04-20 14:49:42.000000 searchkit-0.2.3/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-04-20 14:49:42.931016 searchkit-0.2.3/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.3/setup.py
```

### Comparing `searchkit-0.2.2.post2/LICENSE` & `searchkit-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.2.post2/PKG-INFO` & `searchkit-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.2.post2
+Version: 0.2.3
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

### Comparing `searchkit-0.2.2.post2/README.md` & `searchkit-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.2.post2/pyproject.toml` & `searchkit-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.2.post2/searchkit/constraints.py` & `searchkit-0.2.3/searchkit/constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.2.post2/searchkit/search.py` & `searchkit-0.2.3/searchkit/search.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.2.post2/searchkit/utils.py` & `searchkit-0.2.3/searchkit/utils.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.2.post2/searchkit.egg-info/PKG-INFO` & `searchkit-0.2.3/searchkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.2.post2
+Version: 0.2.3
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

