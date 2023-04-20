# Comparing `tmp/conlp-0.0.2.tar.gz` & `tmp/conlp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conlp-0.0.2.tar", last modified: Wed Apr 19 02:01:43 2023, max compression
+gzip compressed data, was "conlp-0.0.3.tar", last modified: Thu Apr 20 18:46:50 2023, max compression
```

## Comparing `conlp-0.0.2.tar` & `conlp-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 02:01:43.892523 conlp-0.0.2/
--rw-rw-rw-   0        0        0    11824 2023-04-19 00:13:02.000000 conlp-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      403 2023-04-19 02:01:43.892523 conlp-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-19 00:11:59.000000 conlp-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 02:01:43.886523 conlp-0.0.2/conlp/
--rw-rw-rw-   0        0        0      115 2023-04-18 23:35:11.000000 conlp-0.0.2/conlp/__init__.py
--rw-rw-rw-   0        0        0    13706 2023-04-18 23:14:20.000000 conlp-0.0.2/conlp/download.py
--rw-rw-rw-   0        0        0     2553 2023-04-18 23:05:17.000000 conlp-0.0.2/conlp/preprocess.py
--rw-rw-rw-   0        0        0    26133 2023-04-18 23:47:32.000000 conlp-0.0.2/conlp/sentiment.py
-drwxrwxrwx   0        0        0        0 2023-04-19 02:01:43.892523 conlp-0.0.2/conlp.egg-info/
--rw-rw-rw-   0        0        0      403 2023-04-19 02:01:43.000000 conlp-0.0.2/conlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-19 02:01:43.000000 conlp-0.0.2/conlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 02:01:43.000000 conlp-0.0.2/conlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-19 02:01:43.000000 conlp-0.0.2/conlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 02:01:43.000000 conlp-0.0.2/conlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-19 02:01:43.893523 conlp-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      665 2023-04-19 02:00:46.000000 conlp-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 18:46:50.763656 conlp-0.0.3/
+-rw-rw-rw-   0        0        0    11824 2023-04-19 00:13:02.000000 conlp-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      403 2023-04-20 18:46:50.763656 conlp-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-19 00:11:59.000000 conlp-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 18:46:50.756668 conlp-0.0.3/conlp/
+-rw-rw-rw-   0        0        0      115 2023-04-18 23:35:11.000000 conlp-0.0.3/conlp/__init__.py
+-rw-rw-rw-   0        0        0    13706 2023-04-18 23:14:20.000000 conlp-0.0.3/conlp/download.py
+-rw-rw-rw-   0        0        0     2553 2023-04-18 23:05:17.000000 conlp-0.0.3/conlp/preprocess.py
+-rw-rw-rw-   0        0        0    26133 2023-04-18 23:47:32.000000 conlp-0.0.3/conlp/sentiment.py
+drwxrwxrwx   0        0        0        0 2023-04-20 18:46:50.762655 conlp-0.0.3/conlp.egg-info/
+-rw-rw-rw-   0        0        0      403 2023-04-20 18:46:50.000000 conlp-0.0.3/conlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-20 18:46:50.000000 conlp-0.0.3/conlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 18:46:50.000000 conlp-0.0.3/conlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-20 18:46:50.000000 conlp-0.0.3/conlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 18:46:50.000000 conlp-0.0.3/conlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-20 18:46:50.763656 conlp-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      648 2023-04-20 18:44:51.000000 conlp-0.0.3/setup.py
```

### Comparing `conlp-0.0.2/LICENSE.txt` & `conlp-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conlp-0.0.2/conlp/download.py` & `conlp-0.0.3/conlp/download.py`

 * *Files identical despite different names*

### Comparing `conlp-0.0.2/conlp/preprocess.py` & `conlp-0.0.3/conlp/preprocess.py`

 * *Files identical despite different names*

### Comparing `conlp-0.0.2/conlp/sentiment.py` & `conlp-0.0.3/conlp/sentiment.py`

 * *Files identical despite different names*

### Comparing `conlp-0.0.2/setup.py` & `conlp-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from distutils.core import setup 
 
 setup(
   name = 'conlp',
   packages = ['conlp'],
-  version = '0.0.2',
+  version = '0.0.3',
   license='Apache-2.0',
   description = 'TYPE YOUR DESCRIPTION HERE',   
   author = 'Nick S.H Oh',
   author_email = 'nick.sh.oh@socialscience.ai',    
   url = 'https://github.com/SOCIALSCIENCEai/coNLP',  
-  download_url = 'https://github.com/SOCIALSCIENCEai/coNLP/archive/refs/tags/0.0.2.tar.gz',
+  download_url = 'https://github.com/SOCIALSCIENCEai/coNLP/archive/refs/tags/0.0.3.tar.gz',
   keywords = ['NLP', 'SOCIAL SCIENCE'],   
   install_requires=[           
           'torch',
           'transformers',
           'transformers[sentencepiece]',
           'scipy',
           'numpy',
-          're',
           'tqdm'
       ]
 )
```

