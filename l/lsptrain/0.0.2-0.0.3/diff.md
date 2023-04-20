# Comparing `tmp/lsptrain-0.0.2.tar.gz` & `tmp/lsptrain-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.2.tar", last modified: Thu Apr 20 13:30:04 2023, max compression
+gzip compressed data, was "lsptrain-0.0.3.tar", last modified: Thu Apr 20 14:59:28 2023, max compression
```

## Comparing `lsptrain-0.0.2.tar` & `lsptrain-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 13:30:04.457477 lsptrain-0.0.2/
--rw-rw-rw-   0        0        0      419 2023-04-20 13:30:04.457477 lsptrain-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-20 13:29:30.000000 lsptrain-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-20 13:30:04.449478 lsptrain-0.0.2/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.2/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 13:30:04.455477 lsptrain-0.0.2/lsptrain/nlp_classfication/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:11:48.000000 lsptrain-0.0.2/lsptrain/nlp_classfication/__init__.py
--rw-rw-rw-   0        0        0      818 2023-04-20 13:29:11.000000 lsptrain-0.0.2/lsptrain/nlp_classfication/model.py
-drwxrwxrwx   0        0        0        0 2023-04-20 13:30:04.453478 lsptrain-0.0.2/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      419 2023-04-20 13:30:04.000000 lsptrain-0.0.2/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-04-20 13:30:04.000000 lsptrain-0.0.2/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 13:30:04.000000 lsptrain-0.0.2/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-20 13:30:04.000000 lsptrain-0.0.2/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 13:30:04.000000 lsptrain-0.0.2/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 13:30:04.458478 lsptrain-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      674 2023-04-20 13:30:03.000000 lsptrain-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:59:28.875635 lsptrain-0.0.3/
+-rw-rw-rw-   0        0        0      419 2023-04-20 14:59:28.874635 lsptrain-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-20 13:29:30.000000 lsptrain-0.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-20 14:59:28.862635 lsptrain-0.0.3/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.3/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:59:28.872635 lsptrain-0.0.3/lsptrain/nlp_classfication/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:11:48.000000 lsptrain-0.0.3/lsptrain/nlp_classfication/__init__.py
+-rw-rw-rw-   0        0        0     8524 2023-04-20 14:56:41.000000 lsptrain-0.0.3/lsptrain/nlp_classfication/model.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:59:28.869635 lsptrain-0.0.3/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-04-20 14:59:28.000000 lsptrain-0.0.3/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-04-20 14:59:28.000000 lsptrain-0.0.3/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 14:59:28.000000 lsptrain-0.0.3/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-20 14:59:28.000000 lsptrain-0.0.3/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 14:59:28.000000 lsptrain-0.0.3/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 14:59:28.875635 lsptrain-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      732 2023-04-20 14:59:10.000000 lsptrain-0.0.3/setup.py
```

### Comparing `lsptrain-0.0.2/setup.py` & `lsptrain-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.2',
+      version='0.0.3',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
       url='http://www.gitee.com/ykallan',
-      install_requires=['torch',
-                        'transformers',
-                        'argparse'],
+      install_requires=['torch>=1.10',
+                        'transformers>=4.20.1',
+                        'scikit-learn>=1.1.0',
+                        'tqdm'],
       python_requires='>=3.7',
       license='BSD License',
       packages=find_packages(),
       platforms=['all'],
       include_package_data=True
       )
```

