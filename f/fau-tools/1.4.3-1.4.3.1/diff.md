# Comparing `tmp/fau_tools-1.4.3.tar.gz` & `tmp/fau_tools-1.4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fau_tools-1.4.3.tar", max compression
+gzip compressed data, was "fau_tools-1.4.3.1.tar", max compression
```

## Comparing `fau_tools-1.4.3.tar` & `fau_tools-1.4.3.1.tar`

### file list

```diff
@@ -1,21 +1,13 @@
--rw-r--r--   0        0        0     2680 2023-04-20 02:37:45.625671 fau_tools-1.4.3/README.md
--rw-r--r--   0        0        0     6148 2023-01-07 12:47:38.094251 fau_tools-1.4.3/fau_tools/.DS_Store
--rw-r--r--   0        0        0      179 2022-09-17 06:01:57.485247 fau_tools-1.4.3/fau_tools/__init__.py
--rw-r--r--   0        0        0       30 2022-11-07 07:34:00.261010 fau_tools-1.4.3/fau_tools/data_structure/__init__.py
--rw-r--r--   0        0        0      221 2022-11-07 08:03:32.272377 fau_tools-1.4.3/fau_tools/data_structure/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4683 2023-04-20 02:49:37.919630 fau_tools-1.4.3/fau_tools/data_structure/__pycache__/data_structure.cpython-310.pyc
--rw-r--r--   0        0        0     3420 2023-04-20 02:46:11.824418 fau_tools-1.4.3/fau_tools/data_structure/data_structure.py
--rw-r--r--   0        0        0      914 2023-04-20 02:46:11.824752 fau_tools-1.4.3/fau_tools/data_structure/data_structure.pyi
--rw-r--r--   0        0        0      678 2023-03-24 03:23:27.260855 fau_tools-1.4.3/fau_tools/pyproject.toml
--rw-r--r--   0        0        0       27 2022-09-17 05:48:40.673809 fau_tools-1.4.3/fau_tools/torch_tools/__init__.py
--rw-r--r--   0        0        0      215 2022-09-18 01:31:17.722972 fau_tools-1.4.3/fau_tools/torch_tools/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8154 2023-04-20 02:49:35.921881 fau_tools-1.4.3/fau_tools/torch_tools/__pycache__/torch_tools.cpython-310.pyc
--rw-r--r--   0        0        0    10050 2023-04-20 02:47:54.439467 fau_tools-1.4.3/fau_tools/torch_tools/torch_tools.py
--rw-r--r--   0        0        0     1440 2023-04-20 02:46:11.825456 fau_tools-1.4.3/fau_tools/torch_tools/torch_tools.pyi
--rw-r--r--   0        0        0       23 2022-09-17 05:58:01.298778 fau_tools-1.4.3/fau_tools/utility/__init__.py
--rw-r--r--   0        0        0      207 2022-09-18 01:31:17.726340 fau_tools-1.4.3/fau_tools/utility/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4470 2023-03-24 06:35:44.247630 fau_tools-1.4.3/fau_tools/utility/__pycache__/utility.cpython-310.pyc
--rw-r--r--   0        0        0     8727 2023-03-24 06:33:55.632551 fau_tools-1.4.3/fau_tools/utility/utility.py
--rw-r--r--   0        0        0      797 2023-03-24 02:36:31.555258 fau_tools-1.4.3/fau_tools/utility/utility.pyi
--rw-r--r--   0        0        0      468 2023-04-20 02:56:20.565005 fau_tools-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 fau_tools-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0      179 2022-09-17 06:01:57.485247 fau_tools-1.4.3.1/Fau_tools/__init__.py
+-rw-r--r--   0        0        0       30 2022-11-07 07:34:00.261010 fau_tools-1.4.3.1/Fau_tools/data_structure/__init__.py
+-rw-r--r--   0        0        0     3420 2023-04-20 02:46:11.824418 fau_tools-1.4.3.1/Fau_tools/data_structure/data_structure.py
+-rw-r--r--   0        0        0      914 2023-04-20 02:46:11.824752 fau_tools-1.4.3.1/Fau_tools/data_structure/data_structure.pyi
+-rw-r--r--   0        0        0       27 2022-09-17 05:48:40.673809 fau_tools-1.4.3.1/Fau_tools/torch_tools/__init__.py
+-rw-r--r--   0        0        0    10050 2023-04-20 02:47:54.439467 fau_tools-1.4.3.1/Fau_tools/torch_tools/torch_tools.py
+-rw-r--r--   0        0        0     1440 2023-04-20 02:46:11.825456 fau_tools-1.4.3.1/Fau_tools/torch_tools/torch_tools.pyi
+-rw-r--r--   0        0        0       23 2022-09-17 05:58:01.298778 fau_tools-1.4.3.1/Fau_tools/utility/__init__.py
+-rw-r--r--   0        0        0     8727 2023-03-24 06:33:55.632551 fau_tools-1.4.3.1/Fau_tools/utility/utility.py
+-rw-r--r--   0        0        0      797 2023-03-24 02:36:31.555258 fau_tools-1.4.3.1/Fau_tools/utility/utility.pyi
+-rw-r--r--   0        0        0     2680 2023-04-20 02:37:45.625671 fau_tools-1.4.3.1/README.md
+-rw-r--r--   0        0        0     1150 2023-04-20 07:15:06.555876 fau_tools-1.4.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3431 1970-01-01 00:00:00.000000 fau_tools-1.4.3.1/PKG-INFO
```

### Comparing `fau_tools-1.4.3/README.md` & `fau_tools-1.4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.3/fau_tools/data_structure/data_structure.py` & `fau_tools-1.4.3.1/Fau_tools/data_structure/data_structure.py`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.3/fau_tools/data_structure/data_structure.pyi` & `fau_tools-1.4.3.1/Fau_tools/data_structure/data_structure.pyi`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.3/fau_tools/torch_tools/torch_tools.py` & `fau_tools-1.4.3.1/Fau_tools/torch_tools/torch_tools.py`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.3/fau_tools/torch_tools/torch_tools.pyi` & `fau_tools-1.4.3.1/Fau_tools/torch_tools/torch_tools.pyi`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.3/fau_tools/utility/utility.py` & `fau_tools-1.4.3.1/Fau_tools/utility/utility.py`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.3/fau_tools/utility/utility.pyi` & `fau_tools-1.4.3.1/Fau_tools/utility/utility.pyi`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.3/PKG-INFO` & `fau_tools-1.4.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fau-tools
-Version: 1.4.3
+Version: 1.4.3.1
 Summary: A python module. The main function is for pytorch training.
 Home-page: https://github.com/Fau818/Fau_tools
 License: MIT
 Author: Fau
 Author-email: Fau818@qq.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
```

