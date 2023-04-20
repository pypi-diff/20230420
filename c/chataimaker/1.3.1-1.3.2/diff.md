# Comparing `tmp/chataimaker-1.3.1.tar.gz` & `tmp/chataimaker-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chataimaker-1.3.1.tar", last modified: Thu Apr 20 20:01:10 2023, max compression
+gzip compressed data, was "chataimaker-1.3.2.tar", last modified: Thu Apr 20 20:04:53 2023, max compression
```

## Comparing `chataimaker-1.3.1.tar` & `chataimaker-1.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 20:01:10.766021 chataimaker-1.3.1/
--rw-rw-rw-   0        0        0      293 2023-04-20 20:00:54.000000 chataimaker-1.3.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1055 2023-04-20 18:26:40.000000 chataimaker-1.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-20 18:28:44.000000 chataimaker-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      863 2023-04-20 20:01:10.756020 chataimaker-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       71 2023-04-20 19:04:00.000000 chataimaker-1.3.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 20:01:10.628984 chataimaker-1.3.1/chataimaker/
--rw-rw-rw-   0        0        0     2478 2023-04-20 20:00:21.000000 chataimaker-1.3.1/chataimaker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:01:10.745015 chataimaker-1.3.1/chataimaker.egg-info/
--rw-rw-rw-   0        0        0      863 2023-04-20 20:01:09.000000 chataimaker-1.3.1/chataimaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-04-20 20:01:10.000000 chataimaker-1.3.1/chataimaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 20:01:09.000000 chataimaker-1.3.1/chataimaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-20 20:01:09.000000 chataimaker-1.3.1/chataimaker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-20 20:01:09.000000 chataimaker-1.3.1/chataimaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 20:01:10.767020 chataimaker-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-04-20 20:00:34.000000 chataimaker-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:04:53.698150 chataimaker-1.3.2/
+-rw-rw-rw-   0        0        0      329 2023-04-20 20:04:44.000000 chataimaker-1.3.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1055 2023-04-20 18:26:40.000000 chataimaker-1.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-20 18:28:44.000000 chataimaker-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      899 2023-04-20 20:04:53.681145 chataimaker-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       71 2023-04-20 19:04:00.000000 chataimaker-1.3.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 20:04:53.556114 chataimaker-1.3.2/chataimaker/
+-rw-rw-rw-   0        0        0     2478 2023-04-20 20:00:21.000000 chataimaker-1.3.2/chataimaker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:04:53.673144 chataimaker-1.3.2/chataimaker.egg-info/
+-rw-rw-rw-   0        0        0      899 2023-04-20 20:04:52.000000 chataimaker-1.3.2/chataimaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-04-20 20:04:52.000000 chataimaker-1.3.2/chataimaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 20:04:52.000000 chataimaker-1.3.2/chataimaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-20 20:04:52.000000 chataimaker-1.3.2/chataimaker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 20:04:52.000000 chataimaker-1.3.2/chataimaker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 20:04:53.699150 chataimaker-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-04-20 20:04:34.000000 chataimaker-1.3.2/setup.py
```

### Comparing `chataimaker-1.3.1/LICENSE.txt` & `chataimaker-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chataimaker-1.3.1/PKG-INFO` & `chataimaker-1.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chataimaker
-Version: 1.3.1
+Version: 1.3.2
 Summary: Package, that can help make you AI chat bot
 Home-page: 
 Author: Boynfriend
 Author-email: justbnf@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -28,7 +28,10 @@
 - chataimaker.pchat(query) function (prints answer to the query)
 
 v1.3:
 - Fixed Bug With Module
 
 v1.3.1:
 - Fixed Bug With Module
+
+v1.3.2:
+- Fixed Bug With Module
```

### Comparing `chataimaker-1.3.1/chataimaker/__init__.py` & `chataimaker-1.3.2/chataimaker/__init__.py`

 * *Files identical despite different names*

### Comparing `chataimaker-1.3.1/chataimaker.egg-info/PKG-INFO` & `chataimaker-1.3.2/chataimaker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chataimaker
-Version: 1.3.1
+Version: 1.3.2
 Summary: Package, that can help make you AI chat bot
 Home-page: 
 Author: Boynfriend
 Author-email: justbnf@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -28,7 +28,10 @@
 - chataimaker.pchat(query) function (prints answer to the query)
 
 v1.3:
 - Fixed Bug With Module
 
 v1.3.1:
 - Fixed Bug With Module
+
+v1.3.2:
+- Fixed Bug With Module
```

### Comparing `chataimaker-1.3.1/setup.py` & `chataimaker-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3"
 ]
 
 setup(
     name = "chataimaker",
-    version = "1.3.1",
+    version = "1.3.2",
     description = "Package, that can help make you AI chat bot",
     long_description = open("README.txt").read() + '\n\n\n' + open("CHANGELOG.txt").read(),
     url="",
     author="Boynfriend",
     author_email="justbnf@gmail.com",
     license="MIT",
     classifiers=classifiers,
```

