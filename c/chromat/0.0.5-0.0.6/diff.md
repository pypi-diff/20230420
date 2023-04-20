# Comparing `tmp/chromat-0.0.5.tar.gz` & `tmp/chromat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromat-0.0.5.tar", max compression
+gzip compressed data, was "chromat-0.0.6.tar", max compression
```

## Comparing `chromat-0.0.5.tar` & `chromat-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0       60 2023-04-14 16:30:12.300399 chromat-0.0.5/chromat/__init__.py
--rw-r--r--   0        0        0     2405 2023-04-16 01:32:09.534293 chromat-0.0.5/chromat/console.py
--rw-r--r--   0        0        0      146 2023-04-13 19:57:48.808921 chromat-0.0.5/chromat/palettes.py
--rw-r--r--   0        0        0    10612 2023-04-16 21:59:38.809938 chromat-0.0.5/chromat/swatches.py
--rw-r--r--   0        0        0     3004 2023-04-16 01:29:19.967497 chromat-0.0.5/chromat/utils.py
--rw-r--r--   0        0        0     1239 2023-04-16 22:00:54.627267 chromat-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       93 2023-04-03 02:42:30.536779 chromat-0.0.5/README.md
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 chromat-0.0.5/setup.py
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 chromat-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      305 2023-04-18 23:53:29.579167 chromat-0.0.6/chromat/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-18 23:54:23.722579 chromat-0.0.6/chromat/palette/__init__.py
+-rw-r--r--   0        0        0      357 2023-04-18 23:51:06.245326 chromat-0.0.6/chromat/palette/palettes.py
+-rw-r--r--   0        0        0      161 2023-04-18 23:43:53.684606 chromat-0.0.6/chromat/swatch/__init__.py
+-rw-r--r--   0        0        0     3237 2023-04-18 23:38:19.613861 chromat-0.0.6/chromat/swatch/props.py
+-rw-r--r--   0        0        0     5903 2023-04-18 23:58:02.442868 chromat-0.0.6/chromat/swatch/swatches.py
+-rw-r--r--   0        0        0      321 2023-04-18 23:41:26.111699 chromat-0.0.6/chromat/utility/__init__.py
+-rw-r--r--   0        0        0     1435 2023-04-18 23:45:11.192797 chromat-0.0.6/chromat/utility/colors.py
+-rw-r--r--   0        0        0      606 2023-04-18 23:57:36.596032 chromat-0.0.6/chromat/utility/console.py
+-rw-r--r--   0        0        0     1375 2023-04-20 04:22:25.092035 chromat-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-04-18 06:50:24.406547 chromat-0.0.6/README.md
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 chromat-0.0.6/setup.py
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 chromat-0.0.6/PKG-INFO
```

### Comparing `chromat-0.0.5/pyproject.toml` & `chromat-0.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chromat"
-version = "0.0.5"
+version = "0.0.6"
 description = "color palettes! under heavy construction!"
 license = "GPL-3.0-or-later"
 authors = ["hex benjamin <hex@hexbenjam.in>"]
 readme = "README.md"
 repository = "https://github.com/hexbenjamin/chromat"
 keywords = ["color", "palette"]
 classifiers = [
@@ -18,32 +18,34 @@
     "Topic :: Artistic Software",
     "Topic :: Utilities",
 ]
 packages = [
     { include = "chromat" },
 ]
 exclude = [
-    "backup/*",
-    "img/*",
-    "tests/*",
-    "__pycache__/*",
+    "*/__pycache__/*",
     "*.dist-info/*",
     "*.egg-info/*",
     "*.pyc",
-    ".flake8",
     ".gitignore",
-    "testing.py",
+    ".replit",
+    "replit.nix",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10.0,<3.11"
+numpy = "^1.22.2"
+replit = "^3.2.4"
+Flask = "^2.2.0"
+urllib3 = "^1.26.12"
 rich = "^13.3.4"
 
+[tool.poetry.dev-dependencies]
+debugpy = "^1.6.2"
+replit-python-lsp-server = {extras = ["yapf", "rope", "pyflakes"], version = "^1.5.9"}
+
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
-flake8 = "^6.0.0"
-mypy = "^1.1.1"
-pytest = "^7.2.2"
 
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `chromat-0.0.5/setup.py` & `chromat-0.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['chromat']
+['chromat', 'chromat.palette', 'chromat.swatch', 'chromat.utility']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['rich>=13.3.4,<14.0.0']
+['Flask>=2.2.0,<3.0.0',
+ 'numpy>=1.22.2,<2.0.0',
+ 'replit>=3.2.4,<4.0.0',
+ 'rich>=13.3.4,<14.0.0',
+ 'urllib3>=1.26.12,<2.0.0']
 
 setup_kwargs = {
     'name': 'chromat',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'color palettes! under heavy construction!',
     'long_description': '\ufeff# chromat: algorithmic color palettes\ncoming soon!\n\nhttps://github.com/hexbenjamin/chromat',
     'author': 'hex benjamin',
     'author_email': 'hex@hexbenjam.in',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/hexbenjamin/chromat',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.10.0,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `chromat-0.0.5/PKG-INFO` & `chromat-0.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: chromat
-Version: 0.0.5
+Version: 0.0.6
 Summary: color palettes! under heavy construction!
 Home-page: https://github.com/hexbenjamin/chromat
 License: GPL-3.0-or-later
 Keywords: color,palette
 Author: hex benjamin
 Author-email: hex@hexbenjam.in
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10.0,<3.11
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Utilities
+Requires-Dist: Flask (>=2.2.0,<3.0.0)
+Requires-Dist: numpy (>=1.22.2,<2.0.0)
+Requires-Dist: replit (>=3.2.4,<4.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
 Project-URL: Repository, https://github.com/hexbenjamin/chromat
 Description-Content-Type: text/markdown
 
 ﻿# chromat: algorithmic color palettes
 coming soon!
 
 https://github.com/hexbenjamin/chromat
```

