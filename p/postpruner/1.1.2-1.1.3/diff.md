# Comparing `tmp/postpruner-1.1.2.tar.gz` & `tmp/postpruner-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postpruner-1.1.2.tar", last modified: Wed Apr 19 23:44:23 2023, max compression
+gzip compressed data, was "postpruner-1.1.3.tar", last modified: Thu Apr 20 06:58:58 2023, max compression
```

## Comparing `postpruner-1.1.2.tar` & `postpruner-1.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.764683 postpruner-1.1.2/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       54 2023-04-19 23:44:23.764683 postpruner-1.1.2/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3648 2023-04-19 22:11:32.000000 postpruner-1.1.2/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.756683 postpruner-1.1.2/postpruner/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:14:28.000000 postpruner-1.1.2/postpruner/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1684 2023-04-19 23:43:36.000000 postpruner-1.1.2/postpruner/__main__.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.760683 postpruner-1.1.2/postpruner/dataset/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.2/postpruner/dataset/__init__.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.760683 postpruner-1.1.2/postpruner/dataset/evaluate/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.2/postpruner/dataset/evaluate/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1023 2023-04-19 23:29:53.000000 postpruner-1.1.2/postpruner/dataset/evaluate/glue.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1232 2023-04-19 23:31:54.000000 postpruner-1.1.2/postpruner/dataset/evaluate/nlp.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2094 2023-04-19 23:29:53.000000 postpruner-1.1.2/postpruner/dataset/evaluate/squad.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3804 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/dataset/glue.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    22749 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/dataset/squad.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.760683 postpruner-1.1.2/postpruner/efficiency/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.2/postpruner/efficiency/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1565 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/efficiency/latency.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1633 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/efficiency/mac.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5007 2023-04-19 23:29:53.000000 postpruner-1.1.2/postpruner/generate_lut.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6889 2023-04-19 23:44:10.000000 postpruner-1.1.2/postpruner/postpruner.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.760683 postpruner-1.1.2/postpruner/prune/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.2/postpruner/prune/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1095 2023-04-19 23:29:53.000000 postpruner-1.1.2/postpruner/prune/fisher.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1303 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/prune/rearrange.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7610 2023-04-19 23:29:53.000000 postpruner-1.1.2/postpruner/prune/rescale.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7421 2023-04-19 23:29:53.000000 postpruner-1.1.2/postpruner/prune/search.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.760683 postpruner-1.1.2/postpruner/utils/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.2/postpruner/utils/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3307 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/utils/arch.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      689 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/utils/linalg.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      439 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/utils/meter.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      180 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/utils/schedule.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      807 2023-04-19 22:11:32.000000 postpruner-1.1.2/postpruner/utils/timer.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:44:23.756683 postpruner-1.1.2/postpruner.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       54 2023-04-19 23:44:23.000000 postpruner-1.1.2/postpruner.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      955 2023-04-19 23:44:23.000000 postpruner-1.1.2/postpruner.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-19 23:44:23.000000 postpruner-1.1.2/postpruner.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-19 23:44:23.000000 postpruner-1.1.2/postpruner.egg-info/entry_points.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-19 23:44:23.000000 postpruner-1.1.2/postpruner.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-04-19 23:44:23.000000 postpruner-1.1.2/postpruner.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-19 23:44:23.764683 postpruner-1.1.2/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      409 2023-04-19 23:44:22.000000 postpruner-1.1.2/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 06:58:58.691128 postpruner-1.1.3/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       54 2023-04-20 06:58:58.691128 postpruner-1.1.3/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3648 2023-04-19 22:11:32.000000 postpruner-1.1.3/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 06:58:58.687127 postpruner-1.1.3/postpruner/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       28 2023-04-20 06:52:52.000000 postpruner-1.1.3/postpruner/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1684 2023-04-19 23:43:36.000000 postpruner-1.1.3/postpruner/__main__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 06:58:58.687127 postpruner-1.1.3/postpruner/dataset/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.3/postpruner/dataset/__init__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 06:58:58.687127 postpruner-1.1.3/postpruner/dataset/evaluate/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.3/postpruner/dataset/evaluate/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1023 2023-04-19 23:29:53.000000 postpruner-1.1.3/postpruner/dataset/evaluate/glue.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1232 2023-04-19 23:31:54.000000 postpruner-1.1.3/postpruner/dataset/evaluate/nlp.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2094 2023-04-19 23:29:53.000000 postpruner-1.1.3/postpruner/dataset/evaluate/squad.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3804 2023-04-19 22:11:32.000000 postpruner-1.1.3/postpruner/dataset/glue.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    22749 2023-04-19 22:11:32.000000 postpruner-1.1.3/postpruner/dataset/squad.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 06:58:58.687127 postpruner-1.1.3/postpruner/efficiency/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.3/postpruner/efficiency/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1565 2023-04-19 22:11:32.000000 postpruner-1.1.3/postpruner/efficiency/latency.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1633 2023-04-19 22:11:32.000000 postpruner-1.1.3/postpruner/efficiency/mac.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5007 2023-04-19 23:29:53.000000 postpruner-1.1.3/postpruner/generate_lut.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6889 2023-04-19 23:44:10.000000 postpruner-1.1.3/postpruner/postpruner.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 06:58:58.691128 postpruner-1.1.3/postpruner/prune/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.3/postpruner/prune/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1095 2023-04-19 23:29:53.000000 postpruner-1.1.3/postpruner/prune/fisher.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1303 2023-04-19 22:11:32.000000 postpruner-1.1.3/postpruner/prune/rearrange.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7610 2023-04-19 23:29:53.000000 postpruner-1.1.3/postpruner/prune/rescale.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7421 2023-04-19 23:29:53.000000 postpruner-1.1.3/postpruner/prune/search.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 06:58:58.691128 postpruner-1.1.3/postpruner/utils/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-1.1.3/postpruner/utils/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3307 2023-04-19 22:11:32.000000 postpruner-1.1.3/postpruner/utils/arch.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      689 2023-04-19 22:11:32.000000 postpruner-1.1.3/postpruner/utils/linalg.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      439 2023-04-19 22:11:32.000000 postpruner-1.1.3/postpruner/utils/meter.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      180 2023-04-19 22:11:32.000000 postpruner-1.1.3/postpruner/utils/schedule.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      807 2023-04-19 22:11:32.000000 postpruner-1.1.3/postpruner/utils/timer.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 06:58:58.687127 postpruner-1.1.3/postpruner.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       54 2023-04-20 06:58:58.000000 postpruner-1.1.3/postpruner.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      955 2023-04-20 06:58:58.000000 postpruner-1.1.3/postpruner.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-20 06:58:58.000000 postpruner-1.1.3/postpruner.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-20 06:58:58.000000 postpruner-1.1.3/postpruner.egg-info/entry_points.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-20 06:58:58.000000 postpruner-1.1.3/postpruner.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-04-20 06:58:58.000000 postpruner-1.1.3/postpruner.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-20 06:58:58.691128 postpruner-1.1.3/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      409 2023-04-20 06:58:53.000000 postpruner-1.1.3/setup.py
```

### Comparing `postpruner-1.1.2/README.md` & `postpruner-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/__main__.py` & `postpruner-1.1.3/postpruner/__main__.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/dataset/evaluate/glue.py` & `postpruner-1.1.3/postpruner/dataset/evaluate/glue.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/dataset/evaluate/nlp.py` & `postpruner-1.1.3/postpruner/dataset/evaluate/nlp.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/dataset/evaluate/squad.py` & `postpruner-1.1.3/postpruner/dataset/evaluate/squad.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/dataset/glue.py` & `postpruner-1.1.3/postpruner/dataset/glue.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/dataset/squad.py` & `postpruner-1.1.3/postpruner/dataset/squad.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/efficiency/latency.py` & `postpruner-1.1.3/postpruner/efficiency/latency.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/efficiency/mac.py` & `postpruner-1.1.3/postpruner/efficiency/mac.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/generate_lut.py` & `postpruner-1.1.3/postpruner/generate_lut.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/postpruner.py` & `postpruner-1.1.3/postpruner/postpruner.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/prune/fisher.py` & `postpruner-1.1.3/postpruner/prune/fisher.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/prune/rearrange.py` & `postpruner-1.1.3/postpruner/prune/rearrange.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/prune/rescale.py` & `postpruner-1.1.3/postpruner/prune/rescale.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/prune/search.py` & `postpruner-1.1.3/postpruner/prune/search.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/utils/arch.py` & `postpruner-1.1.3/postpruner/utils/arch.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/utils/linalg.py` & `postpruner-1.1.3/postpruner/utils/linalg.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner/utils/timer.py` & `postpruner-1.1.3/postpruner/utils/timer.py`

 * *Files identical despite different names*

### Comparing `postpruner-1.1.2/postpruner.egg-info/SOURCES.txt` & `postpruner-1.1.3/postpruner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

