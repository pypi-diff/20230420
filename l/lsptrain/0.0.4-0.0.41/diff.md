# Comparing `tmp/lsptrain-0.0.4.tar.gz` & `tmp/lsptrain-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.4.tar", last modified: Thu Apr 20 15:15:29 2023, max compression
+gzip compressed data, was "lsptrain-0.0.41.tar", last modified: Thu Apr 20 15:17:15 2023, max compression
```

## Comparing `lsptrain-0.0.4.tar` & `lsptrain-0.0.41.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 15:15:29.672726 lsptrain-0.0.4/
--rw-rw-rw-   0        0        0      419 2023-04-20 15:15:29.671726 lsptrain-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-20 13:29:30.000000 lsptrain-0.0.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-20 15:15:29.659726 lsptrain-0.0.4/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.4/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 15:15:29.669726 lsptrain-0.0.4/lsptrain/nlp_classfication/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:11:48.000000 lsptrain-0.0.4/lsptrain/nlp_classfication/__init__.py
--rw-rw-rw-   0        0        0     8524 2023-04-20 14:56:41.000000 lsptrain-0.0.4/lsptrain/nlp_classfication/model.py
-drwxrwxrwx   0        0        0        0 2023-04-20 15:15:29.667726 lsptrain-0.0.4/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      419 2023-04-20 15:15:29.000000 lsptrain-0.0.4/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-04-20 15:15:29.000000 lsptrain-0.0.4/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 15:15:29.000000 lsptrain-0.0.4/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-20 15:15:29.000000 lsptrain-0.0.4/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 15:15:29.000000 lsptrain-0.0.4/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 15:15:29.672726 lsptrain-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      732 2023-04-20 15:15:13.000000 lsptrain-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 15:17:15.009638 lsptrain-0.0.41/
+-rw-rw-rw-   0        0        0      434 2023-04-20 15:17:15.008638 lsptrain-0.0.41/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-04-20 15:16:58.000000 lsptrain-0.0.41/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-20 15:17:14.995638 lsptrain-0.0.41/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.41/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 15:17:15.006638 lsptrain-0.0.41/lsptrain/nlp_classfication/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:11:48.000000 lsptrain-0.0.41/lsptrain/nlp_classfication/__init__.py
+-rw-rw-rw-   0        0        0     8524 2023-04-20 14:56:41.000000 lsptrain-0.0.41/lsptrain/nlp_classfication/model.py
+drwxrwxrwx   0        0        0        0 2023-04-20 15:17:15.002638 lsptrain-0.0.41/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-04-20 15:17:14.000000 lsptrain-0.0.41/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-04-20 15:17:14.000000 lsptrain-0.0.41/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 15:17:14.000000 lsptrain-0.0.41/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-20 15:17:14.000000 lsptrain-0.0.41/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 15:17:14.000000 lsptrain-0.0.41/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 15:17:15.009638 lsptrain-0.0.41/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-04-20 15:16:29.000000 lsptrain-0.0.41/setup.py
```

### Comparing `lsptrain-0.0.4/lsptrain/nlp_classfication/model.py` & `lsptrain-0.0.41/lsptrain/nlp_classfication/model.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.4/setup.py` & `lsptrain-0.0.41/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.4',
+      version='0.0.41',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
-      url='http://www.gitee.com/ykallan',
+      url='https://www.gitee.com/ykallan/lsptrain',
       install_requires=['torch>=1.10',
                         'transformers>=4.20.1',
                         'scikit-learn>=1.1.0',
                         'tqdm'],
       python_requires='>=3.7',
       license='BSD License',
       packages=find_packages(),
```

