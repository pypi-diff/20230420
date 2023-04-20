# Comparing `tmp/Kart-0.9.2.tar.gz` & `tmp/Kart-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kart-0.9.2.tar", last modified: Sat Jul 31 10:47:43 2021, max compression
+gzip compressed data, was "Kart-0.9.3.tar", last modified: Sat Jul 31 10:56:05 2021, max compression
```

## Comparing `Kart-0.9.2.tar` & `Kart-0.9.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2021-07-04 21:17:05.637057 Kart-0.9.2/LICENSE
--rw-r--r--   0        0        0      976 2021-07-04 21:17:05.637057 Kart-0.9.2/README.md
--rw-r--r--   0        0        0     5085 2021-07-31 10:23:16.154762 Kart-0.9.2/kart/__init__.py
--rw-r--r--   0        0        0     5606 2021-07-31 10:30:26.797540 Kart-0.9.2/kart/mappers.py
--rw-r--r--   0        0        0     3440 2021-07-30 20:08:39.424259 Kart-0.9.2/kart/markdown.py
--rw-r--r--   0        0        0     5182 2021-07-31 10:08:18.438364 Kart-0.9.2/kart/miners.py
--rw-r--r--   0        0        0     1096 2021-07-04 21:17:05.641057 Kart-0.9.2/kart/modifiers.py
--rw-r--r--   0        0        0     6690 2021-07-30 20:26:42.396568 Kart-0.9.2/kart/renderers.py
--rw-r--r--   0        0        0     2946 2021-07-31 10:22:39.498352 Kart-0.9.2/kart/utils.py
--rw-r--r--   0        0        0      459 2021-07-31 10:37:19.758018 Kart-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     1770 2021-07-31 10:47:43.072199 Kart-0.9.2/setup.py
--rw-r--r--   0        0        0     1773 2021-07-31 10:47:43.072454 Kart-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2021-07-04 21:17:05.637057 Kart-0.9.3/LICENSE
+-rw-r--r--   0        0        0      976 2021-07-04 21:17:05.637057 Kart-0.9.3/README.md
+-rw-r--r--   0        0        0     5085 2021-07-31 10:23:16.154762 Kart-0.9.3/kart/__init__.py
+-rw-r--r--   0        0        0     5606 2021-07-31 10:30:26.797540 Kart-0.9.3/kart/mappers.py
+-rw-r--r--   0        0        0     3440 2021-07-30 20:08:39.424259 Kart-0.9.3/kart/markdown.py
+-rw-r--r--   0        0        0     5182 2021-07-31 10:08:18.438364 Kart-0.9.3/kart/miners.py
+-rw-r--r--   0        0        0     1096 2021-07-04 21:17:05.641057 Kart-0.9.3/kart/modifiers.py
+-rw-r--r--   0        0        0     6690 2021-07-30 20:26:42.396568 Kart-0.9.3/kart/renderers.py
+-rw-r--r--   0        0        0     2946 2021-07-31 10:22:39.498352 Kart-0.9.3/kart/utils.py
+-rw-r--r--   0        0        0      486 2021-07-31 10:55:20.519140 Kart-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     1804 2021-07-31 10:56:05.904657 Kart-0.9.3/setup.py
+-rw-r--r--   0        0        0     1821 2021-07-31 10:56:05.904919 Kart-0.9.3/PKG-INFO
```

### Comparing `Kart-0.9.2/LICENSE` & `Kart-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Kart-0.9.2/README.md` & `Kart-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `Kart-0.9.2/kart/__init__.py` & `Kart-0.9.3/kart/__init__.py`

 * *Files identical despite different names*

### Comparing `Kart-0.9.2/kart/mappers.py` & `Kart-0.9.3/kart/mappers.py`

 * *Files identical despite different names*

### Comparing `Kart-0.9.2/kart/markdown.py` & `Kart-0.9.3/kart/markdown.py`

 * *Files identical despite different names*

### Comparing `Kart-0.9.2/kart/miners.py` & `Kart-0.9.3/kart/miners.py`

 * *Files identical despite different names*

### Comparing `Kart-0.9.2/kart/modifiers.py` & `Kart-0.9.3/kart/modifiers.py`

 * *Files identical despite different names*

### Comparing `Kart-0.9.2/kart/renderers.py` & `Kart-0.9.3/kart/renderers.py`

 * *Files identical despite different names*

### Comparing `Kart-0.9.2/kart/utils.py` & `Kart-0.9.3/kart/utils.py`

 * *Files identical despite different names*

### Comparing `Kart-0.9.2/setup.py` & `Kart-0.9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['jinja2>=2.11,<3.0',
  'mistune==2.0.0rc1',
  'pygments>=2.6.1,<3.0.0',
+ 'python-dateutil>=2.8.2,<3.0.0',
  'python-slugify>=4.0.1,<5.0.0',
  'pyyaml>=5.1,<6.0',
  'watchdog>=0.10.3,<0.11.0']
 
 setup_kwargs = {
     'name': 'kart',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'A very flexible static site generator written in python',
     'long_description': '# Kart\nA very flexible static site generator written in python\n\n# Getting started\nInstall Kart with pip\n```bash\n$ pip install Kart\n```\n\nBuild the basic structure\n```bash\n$ python -m kart init\n```\n\nIn this configuration Kart will only build a basic blog with a paginated blog index and paginated tags. If you want to customize the urls of the blog you will have to modify main.py with custom python code\n\n\nYou can then build and serve your site with this command\n```bash\n$ python3 main.py serve\n```\n\n# Disclaimer\nKart is not yet ready to use in a real-world scenario. It is still in development its api can change abruptly each minor version.\n\nI am currently writing the [documentation](https://giacomocaironi.gitlab.io/Kart) of kart but it is by no mean complete. If you want to look at some examples you can look the docs folder, where the documentation is held, and the source code of the [example site](https://gitlab.com/giacomocaironi/Kart/-/tree/master/kart_quickstart)\n',
     'author': 'Giacomo Caironi',
     'author_email': 'giacomo.caironi@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `Kart-0.9.2/PKG-INFO` & `Kart-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: kart
-Version: 0.9.2
+Version: 0.9.3
 Summary: A very flexible static site generator written in python
 License: MIT
 Author: Giacomo Caironi
 Author-email: giacomo.caironi@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: jinja2 (>=2.11,<3.0)
 Requires-Dist: mistune (==2.0.0rc1)
 Requires-Dist: pygments (>=2.6.1,<3.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-slugify (>=4.0.1,<5.0.0)
 Requires-Dist: pyyaml (>=5.1,<6.0)
 Requires-Dist: watchdog (>=0.10.3,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Kart
 A very flexible static site generator written in python
```

