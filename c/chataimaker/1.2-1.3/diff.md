# Comparing `tmp/chataimaker-1.2.tar.gz` & `tmp/chataimaker-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chataimaker-1.2.tar", last modified: Thu Apr 20 19:18:29 2023, max compression
+gzip compressed data, was "chataimaker-1.3.tar", last modified: Thu Apr 20 19:53:00 2023, max compression
```

## Comparing `chataimaker-1.2.tar` & `chataimaker-1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 19:18:29.140649 chataimaker-1.2/
--rw-rw-rw-   0        0        0      223 2023-04-20 19:18:17.000000 chataimaker-1.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1055 2023-04-20 18:26:40.000000 chataimaker-1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-20 18:28:44.000000 chataimaker-1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      791 2023-04-20 19:18:29.122644 chataimaker-1.2/PKG-INFO
--rw-rw-rw-   0        0        0       71 2023-04-20 19:04:00.000000 chataimaker-1.2/README.txt
--rw-rw-rw-   0        0        0     2477 2023-04-20 19:17:50.000000 chataimaker-1.2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 19:18:29.113642 chataimaker-1.2/chataimaker.egg-info/
--rw-rw-rw-   0        0        0      791 2023-04-20 19:18:28.000000 chataimaker-1.2/chataimaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-20 19:18:28.000000 chataimaker-1.2/chataimaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 19:18:28.000000 chataimaker-1.2/chataimaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-20 19:18:28.000000 chataimaker-1.2/chataimaker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 19:18:28.000000 chataimaker-1.2/chataimaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 19:18:29.141649 chataimaker-1.2/setup.cfg
--rw-rw-rw-   0        0        0      857 2023-04-20 19:17:55.000000 chataimaker-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:53:00.297713 chataimaker-1.3/
+-rw-rw-rw-   0        0        0      257 2023-04-20 19:52:45.000000 chataimaker-1.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1055 2023-04-20 18:26:40.000000 chataimaker-1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-20 18:28:44.000000 chataimaker-1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      825 2023-04-20 19:53:00.287710 chataimaker-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       71 2023-04-20 19:04:00.000000 chataimaker-1.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 19:53:00.196686 chataimaker-1.3/chataimaker/
+-rw-rw-rw-   0        0        0     2477 2023-04-20 19:17:50.000000 chataimaker-1.3/chataimaker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:53:00.278708 chataimaker-1.3/chataimaker.egg-info/
+-rw-rw-rw-   0        0        0      825 2023-04-20 19:52:59.000000 chataimaker-1.3/chataimaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-04-20 19:52:59.000000 chataimaker-1.3/chataimaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 19:52:59.000000 chataimaker-1.3/chataimaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-20 19:52:59.000000 chataimaker-1.3/chataimaker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 19:52:59.000000 chataimaker-1.3/chataimaker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 19:53:00.298713 chataimaker-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      857 2023-04-20 19:52:13.000000 chataimaker-1.3/setup.py
```

### Comparing `chataimaker-1.2/LICENSE.txt` & `chataimaker-1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chataimaker-1.2/PKG-INFO` & `chataimaker-1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chataimaker
-Version: 1.2
+Version: 1.3
 Summary: Package, that can help make you AI chat bot
 Home-page: 
 Author: Boynfriend
 Author-email: justbnf@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -22,7 +22,10 @@
 - chataimaker.chat(query) function (gives answer to any query)
 
 v1.1:
 - Bug fix with pickle module.
 
 v1.2:
 - chataimaker.pchat(query) function (prints answer to the query)
+
+v1.3:
+- Fixed Bug With Module
```

### Comparing `chataimaker-1.2/__init__.py` & `chataimaker-1.3/chataimaker/__init__.py`

 * *Files identical despite different names*

### Comparing `chataimaker-1.2/chataimaker.egg-info/PKG-INFO` & `chataimaker-1.3/chataimaker.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chataimaker
-Version: 1.2
+Version: 1.3
 Summary: Package, that can help make you AI chat bot
 Home-page: 
 Author: Boynfriend
 Author-email: justbnf@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -22,7 +22,10 @@
 - chataimaker.chat(query) function (gives answer to any query)
 
 v1.1:
 - Bug fix with pickle module.
 
 v1.2:
 - chataimaker.pchat(query) function (prints answer to the query)
+
+v1.3:
+- Fixed Bug With Module
```

### Comparing `chataimaker-1.2/setup.py` & `chataimaker-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3"
 ]
 
 setup(
     name = "chataimaker",
-    version = "1.2",
+    version = "1.3",
     description = "Package, that can help make you AI chat bot",
     long_description = open("README.txt").read() + '\n\n\n' + open("CHANGELOG.txt").read(),
     url="",
     author="Boynfriend",
     author_email="justbnf@gmail.com",
     license="MIT",
     classifiers=classifiers,
```

