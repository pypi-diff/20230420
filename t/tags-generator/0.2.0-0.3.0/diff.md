# Comparing `tmp/tags-generator-0.2.0.tar.gz` & `tmp/tags-generator-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tags-generator-0.2.0.tar", last modified: Thu Apr 20 02:33:03 2023, max compression
+gzip compressed data, was "tags-generator-0.3.0.tar", last modified: Thu Apr 20 02:40:46 2023, max compression
```

## Comparing `tags-generator-0.2.0.tar` & `tags-generator-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 nigohiroki   (501) staff       (20)        0 2023-04-20 02:33:03.868125 tags-generator-0.2.0/
--rw-r--r--   0 nigohiroki   (501) staff       (20)      257 2023-04-20 00:59:35.000000 tags-generator-0.2.0/LICENSE
--rw-r--r--   0 nigohiroki   (501) staff       (20)     1219 2023-04-20 02:33:03.868016 tags-generator-0.2.0/PKG-INFO
--rw-r--r--   0 nigohiroki   (501) staff       (20)      495 2023-04-20 02:08:18.000000 tags-generator-0.2.0/README.md
--rw-r--r--   0 nigohiroki   (501) staff       (20)       38 2023-04-20 02:33:03.868170 tags-generator-0.2.0/setup.cfg
--rw-r--r--   0 nigohiroki   (501) staff       (20)      884 2023-04-20 02:31:46.000000 tags-generator-0.2.0/setup.py
-drwxr-xr-x   0 nigohiroki   (501) staff       (20)        0 2023-04-20 02:33:03.867835 tags-generator-0.2.0/tags_generator.egg-info/
--rw-r--r--   0 nigohiroki   (501) staff       (20)     1219 2023-04-20 02:33:03.000000 tags-generator-0.2.0/tags_generator.egg-info/PKG-INFO
--rw-r--r--   0 nigohiroki   (501) staff       (20)      215 2023-04-20 02:33:03.000000 tags-generator-0.2.0/tags_generator.egg-info/SOURCES.txt
--rw-r--r--   0 nigohiroki   (501) staff       (20)        1 2023-04-20 02:33:03.000000 tags-generator-0.2.0/tags_generator.egg-info/dependency_links.txt
--rw-r--r--   0 nigohiroki   (501) staff       (20)        7 2023-04-20 02:33:03.000000 tags-generator-0.2.0/tags_generator.egg-info/requires.txt
--rw-r--r--   0 nigohiroki   (501) staff       (20)        1 2023-04-20 02:33:03.000000 tags-generator-0.2.0/tags_generator.egg-info/top_level.txt
+drwxr-xr-x   0 nigohiroki   (501) staff       (20)        0 2023-04-20 02:40:46.417584 tags-generator-0.3.0/
+-rw-r--r--   0 nigohiroki   (501) staff       (20)      257 2023-04-20 00:59:35.000000 tags-generator-0.3.0/LICENSE
+-rw-r--r--   0 nigohiroki   (501) staff       (20)     1219 2023-04-20 02:40:46.417476 tags-generator-0.3.0/PKG-INFO
+-rw-r--r--   0 nigohiroki   (501) staff       (20)      495 2023-04-20 02:08:18.000000 tags-generator-0.3.0/README.md
+-rw-r--r--   0 nigohiroki   (501) staff       (20)       38 2023-04-20 02:40:46.417692 tags-generator-0.3.0/setup.cfg
+-rw-r--r--   0 nigohiroki   (501) staff       (20)      884 2023-04-20 02:40:11.000000 tags-generator-0.3.0/setup.py
+drwxr-xr-x   0 nigohiroki   (501) staff       (20)        0 2023-04-20 02:40:46.416528 tags-generator-0.3.0/tags_generator/
+-rw-r--r--   0 nigohiroki   (501) staff       (20)       42 2023-04-20 01:54:25.000000 tags-generator-0.3.0/tags_generator/__init__.py
+-rw-r--r--   0 nigohiroki   (501) staff       (20)      684 2023-04-20 02:29:14.000000 tags-generator-0.3.0/tags_generator/tags_generator.py
+drwxr-xr-x   0 nigohiroki   (501) staff       (20)        0 2023-04-20 02:40:46.417299 tags-generator-0.3.0/tags_generator.egg-info/
+-rw-r--r--   0 nigohiroki   (501) staff       (20)     1219 2023-04-20 02:40:46.000000 tags-generator-0.3.0/tags_generator.egg-info/PKG-INFO
+-rw-r--r--   0 nigohiroki   (501) staff       (20)      275 2023-04-20 02:40:46.000000 tags-generator-0.3.0/tags_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 nigohiroki   (501) staff       (20)        1 2023-04-20 02:40:46.000000 tags-generator-0.3.0/tags_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 nigohiroki   (501) staff       (20)        7 2023-04-20 02:40:46.000000 tags-generator-0.3.0/tags_generator.egg-info/requires.txt
+-rw-r--r--   0 nigohiroki   (501) staff       (20)       15 2023-04-20 02:40:46.000000 tags-generator-0.3.0/tags_generator.egg-info/top_level.txt
```

### Comparing `tags-generator-0.2.0/PKG-INFO` & `tags-generator-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tags-generator
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library to generate tags list from a text using OpenAI
 Home-page: https://github.com/nigohiroki/tags-generator
 Author: nigohiroki
 Author-email: nigohiroki@teit-inc.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tags-generator-0.2.0/setup.py` & `tags-generator-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tags-generator',
-    version='0.2.0',
+    version='0.3.0',
     author='nigohiroki',
     author_email='nigohiroki@teit-inc.com',
     description='A library to generate tags list from a text using OpenAI',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/nigohiroki/tags-generator',
     packages=find_packages(),
```

### Comparing `tags-generator-0.2.0/tags_generator.egg-info/PKG-INFO` & `tags-generator-0.3.0/tags_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tags-generator
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library to generate tags list from a text using OpenAI
 Home-page: https://github.com/nigohiroki/tags-generator
 Author: nigohiroki
 Author-email: nigohiroki@teit-inc.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

