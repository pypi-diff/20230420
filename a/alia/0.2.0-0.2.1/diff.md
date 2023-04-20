# Comparing `tmp/alia-0.2.0.tar.gz` & `tmp/alia-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alia-0.2.0.tar", last modified: Wed Apr 19 20:15:41 2023, max compression
+gzip compressed data, was "alia-0.2.1.tar", last modified: Thu Apr 20 19:42:17 2023, max compression
```

## Comparing `alia-0.2.0.tar` & `alia-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-19 20:15:41.703047 alia-0.2.0/
--rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.2.0/LICENSE
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-19 20:15:41.702651 alia-0.2.0/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 19:00:09.000000 alia-0.2.0/README.md
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-19 20:15:41.700223 alia-0.2.0/alia/
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.2.0/alia/__init__.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    17437 2023-04-19 20:09:36.000000 alia-0.2.0/alia/colors.py
--rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.2.0/alia/df_tools.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    27520 2023-04-19 20:13:35.000000 alia-0.2.0/alia/tools.py
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-19 20:15:41.702275 alia-0.2.0/alia.egg-info/
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-19 20:15:41.000000 alia-0.2.0/alia.egg-info/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-04-19 20:15:41.000000 alia-0.2.0/alia.egg-info/SOURCES.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-04-19 20:15:41.000000 alia-0.2.0/alia.egg-info/dependency_links.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       81 2023-04-19 20:15:41.000000 alia-0.2.0/alia.egg-info/requires.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-04-19 20:15:41.000000 alia-0.2.0/alia.egg-info/top_level.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-04-19 20:15:41.703170 alia-0.2.0/setup.cfg
--rw-r--r--   0 aliavictor   (502) staff       (20)      902 2023-04-19 20:12:22.000000 alia-0.2.0/setup.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-20 19:42:17.218699 alia-0.2.1/
+-rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.2.1/LICENSE
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-20 19:42:17.218332 alia-0.2.1/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 19:00:09.000000 alia-0.2.1/README.md
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-20 19:42:17.214609 alia-0.2.1/alia/
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.2.1/alia/__init__.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    17437 2023-04-19 20:09:36.000000 alia-0.2.1/alia/colors.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.2.1/alia/df_tools.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    27520 2023-04-19 20:13:35.000000 alia-0.2.1/alia/tools.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-20 19:42:17.217693 alia-0.2.1/alia.egg-info/
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-20 19:42:17.000000 alia-0.2.1/alia.egg-info/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-04-20 19:42:17.000000 alia-0.2.1/alia.egg-info/SOURCES.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-04-20 19:42:17.000000 alia-0.2.1/alia.egg-info/dependency_links.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       94 2023-04-20 19:42:17.000000 alia-0.2.1/alia.egg-info/requires.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-04-20 19:42:17.000000 alia-0.2.1/alia.egg-info/top_level.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-04-20 19:42:17.218804 alia-0.2.1/setup.cfg
+-rw-r--r--   0 aliavictor   (502) staff       (20)      926 2023-04-20 19:40:04.000000 alia-0.2.1/setup.py
```

### Comparing `alia-0.2.0/LICENSE` & `alia-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alia-0.2.0/PKG-INFO` & `alia-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.2.0/alia/colors.py` & `alia-0.2.1/alia/colors.py`

 * *Files identical despite different names*

### Comparing `alia-0.2.0/alia/df_tools.py` & `alia-0.2.1/alia/df_tools.py`

 * *Files identical despite different names*

### Comparing `alia-0.2.0/alia/tools.py` & `alia-0.2.1/alia/tools.py`

 * *Files identical despite different names*

### Comparing `alia-0.2.0/alia.egg-info/PKG-INFO` & `alia-0.2.1/alia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.2.0/setup.py` & `alia-0.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="alia",
-    version="0.2.0",
+    version="0.2.1",
     description="A collection of random helper tools to make life easier",
     author="Alia",
     author_email="alia.jo.victor@gmail.com",
     url="https://github.com/aliavictor/alia",
     packages=find_packages(),
     install_requires=[
         # i.e. 'numpy>=1.18.0'
@@ -14,15 +14,16 @@
         "pandas",
         "requests",
         "python-dotenv",
         "sty",
         "pyperclip",
         "python-dateutil",
         "ipython",
-        "fernet"
+        "fernet",
+        "cryptography"
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

