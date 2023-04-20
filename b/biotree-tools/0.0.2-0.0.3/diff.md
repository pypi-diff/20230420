# Comparing `tmp/biotree_tools-0.0.2.tar.gz` & `tmp/biotree_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotree_tools-0.0.2.tar", last modified: Thu Apr 20 16:38:26 2023, max compression
+gzip compressed data, was "biotree_tools-0.0.3.tar", last modified: Thu Apr 20 20:27:26 2023, max compression
```

## Comparing `biotree_tools-0.0.2.tar` & `biotree_tools-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-20 16:38:26.408993 biotree_tools-0.0.2/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-03-29 13:25:29.000000 biotree_tools-0.0.2/LICENSE
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      582 2023-04-20 16:38:26.408993 biotree_tools-0.0.2/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       96 2023-03-29 13:25:29.000000 biotree_tools-0.0.2/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 biotree_tools-0.0.2/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      850 2023-04-20 16:38:26.408993 biotree_tools-0.0.2/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 biotree_tools-0.0.2/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-20 16:38:26.408993 biotree_tools-0.0.2/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-20 16:38:26.408993 biotree_tools-0.0.2/src/biotree_tools/
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)   341968 2023-03-29 13:48:02.000000 biotree_tools-0.0.2/src/biotree_tools/MMlib3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      141 2023-04-20 16:25:52.000000 biotree_tools-0.0.2/src/biotree_tools/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-04-20 16:38:18.000000 biotree_tools-0.0.2/src/biotree_tools/_version.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    24390 2023-04-20 16:23:51.000000 biotree_tools-0.0.2/src/biotree_tools/alignment_tools.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    19769 2023-04-20 16:22:01.000000 biotree_tools-0.0.2/src/biotree_tools/phylo_context.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    43207 2023-04-20 16:16:56.000000 biotree_tools-0.0.2/src/biotree_tools/show_tree.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    71529 2023-04-20 16:36:57.000000 biotree_tools-0.0.2/src/biotree_tools/tree_classes.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     7835 2023-04-20 16:14:04.000000 biotree_tools-0.0.2/src/biotree_tools/tree_tools.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-20 16:38:26.408993 biotree_tools-0.0.2/src/biotree_tools.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      582 2023-04-20 16:38:26.000000 biotree_tools-0.0.2/src/biotree_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      512 2023-04-20 16:38:26.000000 biotree_tools-0.0.2/src/biotree_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-04-20 16:38:26.000000 biotree_tools-0.0.2/src/biotree_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       63 2023-04-20 16:38:26.000000 biotree_tools-0.0.2/src/biotree_tools.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       14 2023-04-20 16:38:26.000000 biotree_tools-0.0.2/src/biotree_tools.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-20 20:27:26.897431 biotree_tools-0.0.3/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-03-29 13:25:29.000000 biotree_tools-0.0.3/LICENSE
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1128 2023-04-20 20:27:26.897431 biotree_tools-0.0.3/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      641 2023-04-20 20:13:16.000000 biotree_tools-0.0.3/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 biotree_tools-0.0.3/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      843 2023-04-20 20:27:26.901431 biotree_tools-0.0.3/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 biotree_tools-0.0.3/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-20 20:27:26.897431 biotree_tools-0.0.3/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-20 20:27:26.897431 biotree_tools-0.0.3/src/biotree_tools/
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)   341968 2023-03-29 13:48:02.000000 biotree_tools-0.0.3/src/biotree_tools/MMlib3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      141 2023-04-20 16:25:52.000000 biotree_tools-0.0.3/src/biotree_tools/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-04-20 20:27:07.000000 biotree_tools-0.0.3/src/biotree_tools/_version.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    24390 2023-04-20 16:23:51.000000 biotree_tools-0.0.3/src/biotree_tools/alignment_tools.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    19769 2023-04-20 16:22:01.000000 biotree_tools-0.0.3/src/biotree_tools/phylo_context.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    43207 2023-04-20 16:16:56.000000 biotree_tools-0.0.3/src/biotree_tools/show_tree.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    71529 2023-04-20 16:36:57.000000 biotree_tools-0.0.3/src/biotree_tools/tree_classes.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     7835 2023-04-20 16:14:04.000000 biotree_tools-0.0.3/src/biotree_tools/tree_tools.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-20 20:27:26.897431 biotree_tools-0.0.3/src/biotree_tools.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1128 2023-04-20 20:27:26.000000 biotree_tools-0.0.3/src/biotree_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      512 2023-04-20 20:27:26.000000 biotree_tools-0.0.3/src/biotree_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-04-20 20:27:26.000000 biotree_tools-0.0.3/src/biotree_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       57 2023-04-20 20:27:26.000000 biotree_tools-0.0.3/src/biotree_tools.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       14 2023-04-20 20:27:26.000000 biotree_tools-0.0.3/src/biotree_tools.egg-info/top_level.txt
```

### Comparing `biotree_tools-0.0.2/LICENSE` & `biotree_tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.2/setup.cfg` & `biotree_tools-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	biopython >=1.46
+	biopython
 	easyterm  >=1.0.0
 	ncbi_db
 	ete3 == 3.1.1
 	brewer2mpl
 
 [options.packages.find]
 where = src
```

### Comparing `biotree_tools-0.0.2/src/biotree_tools/MMlib3.py` & `biotree_tools-0.0.3/src/biotree_tools/MMlib3.py`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.2/src/biotree_tools/alignment_tools.py` & `biotree_tools-0.0.3/src/biotree_tools/alignment_tools.py`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.2/src/biotree_tools/phylo_context.py` & `biotree_tools-0.0.3/src/biotree_tools/phylo_context.py`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.2/src/biotree_tools/show_tree.py` & `biotree_tools-0.0.3/src/biotree_tools/show_tree.py`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.2/src/biotree_tools/tree_classes.py` & `biotree_tools-0.0.3/src/biotree_tools/tree_classes.py`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.2/src/biotree_tools/tree_tools.py` & `biotree_tools-0.0.3/src/biotree_tools/tree_tools.py`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.2/src/biotree_tools.egg-info/SOURCES.txt` & `biotree_tools-0.0.3/src/biotree_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

