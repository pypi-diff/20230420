# Comparing `tmp/pynight-0.2.0.1.tar.gz` & `tmp/pynight-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynight-0.2.0.1.tar", max compression
+gzip compressed data, was "pynight-0.2.1.tar", max compression
```

## Comparing `pynight-0.2.0.1.tar` & `pynight-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,23 @@
--rw-r--r--   0        0        0      246 2021-09-30 14:42:07.367092 pynight-0.2.0.1/pynight/__init__.py
--rw-r--r--   0        0        0      481 2022-06-10 16:56:54.292098 pynight-0.2.0.1/pynight/common_async.py
--rw-r--r--   0        0        0     1767 2022-06-19 08:20:42.336704 pynight-0.2.0.1/pynight/common_combinatorics.py
--rw-r--r--   0        0        0      169 2022-06-10 16:56:54.297271 pynight-0.2.0.1/pynight/common_debugging.py
--rw-r--r--   0        0        0      597 2022-06-17 12:19:42.438177 pynight-0.2.0.1/pynight/common_executing.py
--rw-r--r--   0        0        0      556 2022-06-10 16:56:54.321171 pynight-0.2.0.1/pynight/common_external.py
--rw-r--r--   0        0        0     2056 2022-06-10 16:56:54.366134 pynight-0.2.0.1/pynight/common_fastapi.py
--rw-r--r--   0        0        0      372 2022-06-10 16:56:54.317398 pynight-0.2.0.1/pynight/common_files.py
--rw-r--r--   0        0        0     1035 2022-09-04 19:41:51.789224 pynight-0.2.0.1/pynight/common_iterable.py
--rw-r--r--   0        0        0     1156 2022-06-10 16:56:54.368937 pynight-0.2.0.1/pynight/common_jax.py
--rw-r--r--   0        0        0      778 2022-06-10 16:56:54.344745 pynight-0.2.0.1/pynight/common_networking.py
--rw-r--r--   0        0        0     1104 2022-06-16 06:38:07.110095 pynight-0.2.0.1/pynight/common_random.py
--rw-r--r--   0        0        0     1360 2022-06-10 16:56:54.382906 pynight-0.2.0.1/pynight/common_redirections.py
--rw-r--r--   0        0        0      128 2022-06-10 16:56:54.366837 pynight-0.2.0.1/pynight/common_telegram.py
--rw-r--r--   0        0        0      537 2021-09-29 06:43:02.753727 pynight-0.2.0.1/pynight/common_uvicorn.py
--rw-r--r--   0        0        0      412 2022-09-04 19:41:59.652814 pynight-0.2.0.1/pyproject.toml
--rw-r--r--   0        0        0      678 2022-09-04 19:42:31.515011 pynight-0.2.0.1/setup.py
--rw-r--r--   0        0        0      621 2022-09-04 19:42:31.515372 pynight-0.2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      246 2021-09-30 14:42:07.367092 pynight-0.2.1/pynight/__init__.py
+-rw-r--r--   0        0        0      481 2022-06-10 16:56:54.292098 pynight-0.2.1/pynight/common_async.py
+-rw-r--r--   0        0        0       85 2023-03-25 14:54:28.702518 pynight-0.2.1/pynight/common_bells.py
+-rw-r--r--   0        0        0     1767 2022-06-19 08:20:42.336704 pynight-0.2.1/pynight/common_combinatorics.py
+-rw-r--r--   0        0        0      169 2022-06-10 16:56:54.297271 pynight-0.2.1/pynight/common_debugging.py
+-rw-r--r--   0        0        0      597 2022-06-17 12:19:42.438177 pynight-0.2.1/pynight/common_executing.py
+-rw-r--r--   0        0        0      556 2022-06-10 16:56:54.321171 pynight-0.2.1/pynight/common_external.py
+-rw-r--r--   0        0        0     2056 2022-06-10 16:56:54.366134 pynight-0.2.1/pynight/common_fastapi.py
+-rw-r--r--   0        0        0      555 2022-10-15 21:37:59.926924 pynight-0.2.1/pynight/common_files.py
+-rw-r--r--   0        0        0     1292 2023-03-28 22:05:55.799557 pynight-0.2.1/pynight/common_ipython.py
+-rw-r--r--   0        0        0     1035 2022-09-04 19:41:51.789224 pynight-0.2.1/pynight/common_iterable.py
+-rw-r--r--   0        0        0     1156 2022-06-10 16:56:54.368937 pynight-0.2.1/pynight/common_jax.py
+-rw-r--r--   0        0        0      778 2022-06-10 16:56:54.344745 pynight-0.2.1/pynight/common_networking.py
+-rw-r--r--   0        0        0     2793 2023-03-27 07:45:00.887719 pynight-0.2.1/pynight/common_openai.py
+-rw-r--r--   0        0        0     1104 2022-06-16 06:38:07.110095 pynight-0.2.1/pynight/common_random.py
+-rw-r--r--   0        0        0     1526 2023-03-28 21:34:54.966246 pynight-0.2.1/pynight/common_redirections.py
+-rw-r--r--   0        0        0      456 2023-03-20 12:49:53.873746 pynight-0.2.1/pynight/common_spacy.py
+-rw-r--r--   0        0        0      128 2022-06-10 16:56:54.366837 pynight-0.2.1/pynight/common_telegram.py
+-rw-r--r--   0        0        0     1539 2023-04-14 05:58:50.130668 pynight-0.2.1/pynight/common_torch.py
+-rw-r--r--   0        0        0      537 2021-09-29 06:43:02.753727 pynight-0.2.1/pynight/common_uvicorn.py
+-rw-r--r--   0        0        0      467 2023-04-20 10:26:10.785874 pynight-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 pynight-0.2.1/setup.py
+-rw-r--r--   0        0        0      791 1970-01-01 00:00:00.000000 pynight-0.2.1/PKG-INFO
```

### Comparing `pynight-0.2.0.1/pynight/common_combinatorics.py` & `pynight-0.2.1/pynight/common_combinatorics.py`

 * *Files identical despite different names*

### Comparing `pynight-0.2.0.1/pynight/common_executing.py` & `pynight-0.2.1/pynight/common_executing.py`

 * *Files identical despite different names*

### Comparing `pynight-0.2.0.1/pynight/common_external.py` & `pynight-0.2.1/pynight/common_external.py`

 * *Files identical despite different names*

### Comparing `pynight-0.2.0.1/pynight/common_fastapi.py` & `pynight-0.2.1/pynight/common_fastapi.py`

 * *Files identical despite different names*

### Comparing `pynight-0.2.0.1/pynight/common_iterable.py` & `pynight-0.2.1/pynight/common_iterable.py`

 * *Files identical despite different names*

### Comparing `pynight-0.2.0.1/pynight/common_jax.py` & `pynight-0.2.1/pynight/common_jax.py`

 * *Files identical despite different names*

### Comparing `pynight-0.2.0.1/pynight/common_networking.py` & `pynight-0.2.1/pynight/common_networking.py`

 * *Files identical despite different names*

### Comparing `pynight-0.2.0.1/pynight/common_random.py` & `pynight-0.2.1/pynight/common_random.py`

 * *Files identical despite different names*

### Comparing `pynight-0.2.0.1/pynight/common_uvicorn.py` & `pynight-0.2.1/pynight/common_uvicorn.py`

 * *Files identical despite different names*

### Comparing `pynight-0.2.0.1/setup.py` & `pynight-0.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,26 +4,31 @@
 packages = \
 ['pynight']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['brish>=0.3.3,<0.4.0', 'dnspython>=2.1.0,<3.0.0', 'executing>=0.8.3,<0.9.0']
+['brish>=0.3.3,<0.4.0',
+ 'dnspython>=2.1.0,<3.0.0',
+ 'executing>=1.2.0,<2.0.0',
+ 'openai>=0.27.2,<0.28.0',
+ 'pyperclip>=1.8.2,<2.0.0',
+ 'spacy>=3.5.1,<4.0.0']
 
 setup_kwargs = {
     'name': 'pynight',
-    'version': '0.2.0.1',
+    'version': '0.2.1',
     'description': 'My Python utility library.',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'NightMachinary',
     'author_email': 'rudiwillalwaysloveyou@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `pynight-0.2.0.1/PKG-INFO` & `pynight-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: pynight
-Version: 0.2.0.1
+Version: 0.2.1
 Summary: My Python utility library.
 License: MIT
 Author: NightMachinary
 Author-email: rudiwillalwaysloveyou@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: brish (>=0.3.3,<0.4.0)
 Requires-Dist: dnspython (>=2.1.0,<3.0.0)
-Requires-Dist: executing (>=0.8.3,<0.9.0)
+Requires-Dist: executing (>=1.2.0,<2.0.0)
+Requires-Dist: openai (>=0.27.2,<0.28.0)
+Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
+Requires-Dist: spacy (>=3.5.1,<4.0.0)
```

