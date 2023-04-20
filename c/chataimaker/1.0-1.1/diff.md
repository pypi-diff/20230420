# Comparing `tmp/chataimaker-1.0.tar.gz` & `tmp/chataimaker-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chataimaker-1.0.tar", last modified: Thu Apr 20 19:05:01 2023, max compression
+gzip compressed data, was "chataimaker-1.1.tar", last modified: Thu Apr 20 19:13:23 2023, max compression
```

## Comparing `chataimaker-1.0.tar` & `chataimaker-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 19:05:01.792853 chataimaker-1.0/
--rw-rw-rw-   0        0        0      108 2023-04-20 19:04:12.000000 chataimaker-1.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1055 2023-04-20 18:26:40.000000 chataimaker-1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-20 18:28:44.000000 chataimaker-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      676 2023-04-20 19:05:01.780849 chataimaker-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       71 2023-04-20 19:04:00.000000 chataimaker-1.0/README.txt
--rw-rw-rw-   0        0        0     2178 2023-04-20 18:14:15.000000 chataimaker-1.0/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 19:05:01.772848 chataimaker-1.0/chataimaker.egg-info/
--rw-rw-rw-   0        0        0      676 2023-04-20 19:05:01.000000 chataimaker-1.0/chataimaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-20 19:05:01.000000 chataimaker-1.0/chataimaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 19:05:01.000000 chataimaker-1.0/chataimaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-20 19:05:01.000000 chataimaker-1.0/chataimaker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 19:05:01.000000 chataimaker-1.0/chataimaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 19:05:01.792853 chataimaker-1.0/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-04-20 19:04:43.000000 chataimaker-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:13:23.659068 chataimaker-1.1/
+-rw-rw-rw-   0        0        0      108 2023-04-20 19:04:12.000000 chataimaker-1.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1055 2023-04-20 18:26:40.000000 chataimaker-1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-20 18:28:44.000000 chataimaker-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      676 2023-04-20 19:13:23.641060 chataimaker-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       71 2023-04-20 19:04:00.000000 chataimaker-1.1/README.txt
+-rw-rw-rw-   0        0        0     2178 2023-04-20 18:14:15.000000 chataimaker-1.1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:13:23.632058 chataimaker-1.1/chataimaker.egg-info/
+-rw-rw-rw-   0        0        0      676 2023-04-20 19:13:22.000000 chataimaker-1.1/chataimaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-04-20 19:13:23.000000 chataimaker-1.1/chataimaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 19:13:22.000000 chataimaker-1.1/chataimaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-20 19:13:22.000000 chataimaker-1.1/chataimaker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 19:13:22.000000 chataimaker-1.1/chataimaker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 19:13:23.661063 chataimaker-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      857 2023-04-20 19:13:09.000000 chataimaker-1.1/setup.py
```

### Comparing `chataimaker-1.0/LICENSE.txt` & `chataimaker-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chataimaker-1.0/PKG-INFO` & `chataimaker-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chataimaker
-Version: 1.0
+Version: 1.1
 Summary: Package, that can help make you AI chat bot
 Home-page: 
 Author: Boynfriend
 Author-email: justbnf@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `chataimaker-1.0/__init__.py` & `chataimaker-1.1/__init__.py`

 * *Files identical despite different names*

### Comparing `chataimaker-1.0/chataimaker.egg-info/PKG-INFO` & `chataimaker-1.1/chataimaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chataimaker
-Version: 1.0
+Version: 1.1
 Summary: Package, that can help make you AI chat bot
 Home-page: 
 Author: Boynfriend
 Author-email: justbnf@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `chataimaker-1.0/setup.py` & `chataimaker-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3"
 ]
 
 setup(
     name = "chataimaker",
-    version = "1.0",
+    version = "1.1",
     description = "Package, that can help make you AI chat bot",
     long_description = open("README.txt").read() + '\n\n\n' + open("CHANGELOG.txt").read(),
     url="",
     author="Boynfriend",
     author_email="justbnf@gmail.com",
     license="MIT",
     classifiers=classifiers,
     keywords='',
     packages=find_packages(),
-    install_requires=['nltk', 'numpy', 'tflearn', 'tensorflow', 'pickle']
+    install_requires=['nltk', 'numpy', 'tflearn', 'tensorflow']
 )
```

