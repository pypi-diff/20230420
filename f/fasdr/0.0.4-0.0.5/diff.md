# Comparing `tmp/fasdr-0.0.4.tar.gz` & `tmp/fasdr-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasdr-0.0.4.tar", last modified: Wed Apr 19 20:36:02 2023, max compression
+gzip compressed data, was "fasdr-0.0.5.tar", last modified: Thu Apr 20 00:13:00 2023, max compression
```

## Comparing `fasdr-0.0.4.tar` & `fasdr-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:36:02.066323 fasdr-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-19 20:36:02.066323 fasdr-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-19 20:35:48.000000 fasdr-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:36:02.066323 fasdr-0.0.4/fasdr/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-19 20:35:48.000000 fasdr-0.0.4/fasdr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-19 20:35:48.000000 fasdr-0.0.4/fasdr/fasdr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:36:02.066323 fasdr-0.0.4/fasdr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-19 20:36:02.000000 fasdr-0.0.4/fasdr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 20:36:02.000000 fasdr-0.0.4/fasdr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:36:02.000000 fasdr-0.0.4/fasdr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 20:36:02.000000 fasdr-0.0.4/fasdr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 20:36:02.000000 fasdr-0.0.4/fasdr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:36:02.066323 fasdr-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-19 20:35:48.000000 fasdr-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:36:02.066323 fasdr-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-19 20:35:48.000000 fasdr-0.0.4/tests/test_fasdr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:00.006703 fasdr-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-20 00:13:00.006703 fasdr-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-20 00:12:43.000000 fasdr-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:00.006703 fasdr-0.0.5/fasdr/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-20 00:12:43.000000 fasdr-0.0.5/fasdr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-20 00:12:43.000000 fasdr-0.0.5/fasdr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-20 00:12:43.000000 fasdr-0.0.5/fasdr/fasdr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:00.006703 fasdr-0.0.5/fasdr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-20 00:12:59.000000 fasdr-0.0.5/fasdr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 00:13:00.000000 fasdr-0.0.5/fasdr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:12:59.000000 fasdr-0.0.5/fasdr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 00:12:59.000000 fasdr-0.0.5/fasdr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 00:12:59.000000 fasdr-0.0.5/fasdr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 00:12:59.000000 fasdr-0.0.5/fasdr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 00:13:00.006703 fasdr-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-20 00:12:43.000000 fasdr-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:00.006703 fasdr-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-20 00:12:43.000000 fasdr-0.0.5/tests/test_fasdr.py
```

### Comparing `fasdr-0.0.4/PKG-INFO` & `fasdr-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasdr
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple dense retrieval using SciPy, spaCy, and Sentence-Transformers
 Home-page: https://github.com/dmarx/fast-and-simple-dense-retrieval/
 Author: David Marx
 Author-email: david.marx84@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fasdr-0.0.4/README.md` & `fasdr-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fasdr-0.0.4/fasdr/fasdr.py` & `fasdr-0.0.5/fasdr/fasdr.py`

 * *Files identical despite different names*

### Comparing `fasdr-0.0.4/fasdr.egg-info/PKG-INFO` & `fasdr-0.0.5/fasdr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasdr
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple dense retrieval using SciPy, spaCy, and Sentence-Transformers
 Home-page: https://github.com/dmarx/fast-and-simple-dense-retrieval/
 Author: David Marx
 Author-email: david.marx84@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fasdr-0.0.4/setup.py` & `fasdr-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from setuptools import setup
 
 setup(
     name='fasdr',
-    version='0.0.4',
+    version='0.0.5',
     author='David Marx',
     author_email='david.marx84@gmail.com',
     description='Simple dense retrieval using SciPy, spaCy, and Sentence-Transformers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dmarx/fast-and-simple-dense-retrieval/',
     packages=['fasdr'],
     install_requires=[
         'numpy',
         'spacy',
         'sentence_transformers',
         'scipy',
         'spacy-sentence-bert',
+        'rich',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
+    entry_points={
+        'console_scripts': [
+            'fasdr=fasdr.cli:main',
+        ],
+    },
 )
```

### Comparing `fasdr-0.0.4/tests/test_fasdr.py` & `fasdr-0.0.5/tests/test_fasdr.py`

 * *Files identical despite different names*

