# Comparing `tmp/cpmax_toolbox-0.3.4.tar.gz` & `tmp/cpmax_toolbox-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpmax_toolbox-0.3.4.tar", max compression
+gzip compressed data, was "cpmax_toolbox-0.3.5.tar", max compression
```

## Comparing `cpmax_toolbox-0.3.4.tar` & `cpmax_toolbox-0.3.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       38 2023-02-01 12:56:05.830314 cpmax_toolbox-0.3.4/cpmax_toolbox/__init__.py
--rw-r--r--   0        0        0     6420 2023-03-14 14:14:10.753141 cpmax_toolbox-0.3.4/cpmax_toolbox/analyzing.py
--rw-r--r--   0        0        0     9981 2023-03-14 13:57:32.685343 cpmax_toolbox-0.3.4/cpmax_toolbox/file_repair.py
--rw-r--r--   0        0        0    13047 2023-02-28 12:35:49.809546 cpmax_toolbox-0.3.4/cpmax_toolbox/vib_measurement.py
--rw-r--r--   0        0        0      531 2023-03-21 07:59:26.625630 cpmax_toolbox-0.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-01 08:47:07.339719 cpmax_toolbox-0.3.4/README.md
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 cpmax_toolbox-0.3.4/setup.py
--rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 cpmax_toolbox-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-02-01 12:56:05.830314 cpmax_toolbox-0.3.5/cpmax_toolbox/__init__.py
+-rw-r--r--   0        0        0     6451 2023-03-23 22:03:22.851073 cpmax_toolbox-0.3.5/cpmax_toolbox/analyzing.py
+-rw-r--r--   0        0        0     9981 2023-03-14 13:57:32.685343 cpmax_toolbox-0.3.5/cpmax_toolbox/file_repair.py
+-rw-r--r--   0        0        0    13047 2023-02-28 12:35:49.809546 cpmax_toolbox-0.3.5/cpmax_toolbox/vib_measurement.py
+-rw-r--r--   0        0        0      531 2023-04-20 12:16:17.114416 cpmax_toolbox-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-01 08:47:07.339719 cpmax_toolbox-0.3.5/README.md
+-rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 cpmax_toolbox-0.3.5/setup.py
+-rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 cpmax_toolbox-0.3.5/PKG-INFO
```

### Comparing `cpmax_toolbox-0.3.4/cpmax_toolbox/analyzing.py` & `cpmax_toolbox-0.3.5/cpmax_toolbox/analyzing.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,7 +175,9 @@
         fig.savefig(
             output_pdf,  # type:ignore - suppress pylint warning message (Path -> str not compatible)
             bbox_inches="tight",
             dpi=600,
         )
     else:
         plt.show()
+
+# create a function prototype
```

### Comparing `cpmax_toolbox-0.3.4/cpmax_toolbox/file_repair.py` & `cpmax_toolbox-0.3.5/cpmax_toolbox/file_repair.py`

 * *Files identical despite different names*

### Comparing `cpmax_toolbox-0.3.4/cpmax_toolbox/vib_measurement.py` & `cpmax_toolbox-0.3.5/cpmax_toolbox/vib_measurement.py`

 * *Files identical despite different names*

### Comparing `cpmax_toolbox-0.3.4/pyproject.toml` & `cpmax_toolbox-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpmax-toolbox"
-version = "0.3.4"
+version = "0.3.5"
 description = ""
 authors = ["JRoseCPMax <j.rose@cpmax.com>"]
 readme = "README.md"
 packages = [{include = "cpmax_toolbox"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `cpmax_toolbox-0.3.4/setup.py` & `cpmax_toolbox-0.3.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'pytz>=2022.7.1,<2023.0.0',
  'requests>=2.28.2,<3.0.0',
  'rich>=13.3.1,<14.0.0',
  'scipy>=1.10.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'cpmax-toolbox',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': '',
     'long_description': '',
     'author': 'JRoseCPMax',
     'author_email': 'j.rose@cpmax.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cpmax_toolbox-0.3.4/PKG-INFO` & `cpmax_toolbox-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpmax-toolbox
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 Author: JRoseCPMax
 Author-email: j.rose@cpmax.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

