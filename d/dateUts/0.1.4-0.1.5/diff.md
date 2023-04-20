# Comparing `tmp/dateUts-0.1.4.tar.gz` & `tmp/dateUts-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dateUts-0.1.4.tar", last modified: Thu Apr 20 19:57:57 2023, max compression
+gzip compressed data, was "dist\dateUts-0.1.5.tar", last modified: Thu Apr 20 20:15:56 2023, max compression
```

## Comparing `dateUts-0.1.4.tar` & `dateUts-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 19:57:57.994744 dateUts-0.1.4/
--rw-rw-rw-   0        0        0      583 2023-04-20 19:55:45.000000 dateUts-0.1.4/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 19:57:57.971745 dateUts-0.1.4/DateUts/
--rw-rw-rw-   0        0        0     4751 2023-04-20 19:55:03.000000 dateUts-0.1.4/DateUts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 19:57:57.990745 dateUts-0.1.4/DateUts.egg-info/
--rw-rw-rw-   0        0        0     6136 2023-04-20 19:57:57.000000 dateUts-0.1.4/DateUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-04-20 19:57:57.000000 dateUts-0.1.4/DateUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 19:57:57.000000 dateUts-0.1.4/DateUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-20 19:57:57.000000 dateUts-0.1.4/DateUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1058 2022-05-25 14:00:44.000000 dateUts-0.1.4/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2022-05-25 22:21:08.000000 dateUts-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6136 2023-04-20 19:57:57.993741 dateUts-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3159 2023-04-20 19:57:17.000000 dateUts-0.1.4/README.md
--rw-rw-rw-   0        0        0      122 2022-10-03 19:44:47.000000 dateUts-0.1.4/commands.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 19:57:57.994744 dateUts-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-04-20 19:57:55.000000 dateUts-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:15:56.494061 dateUts-0.1.5/
+-rw-rw-rw-   0        0        0      583 2023-04-20 19:55:45.000000 dateUts-0.1.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2022-05-25 14:00:44.000000 dateUts-0.1.5/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2022-05-25 22:21:08.000000 dateUts-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6136 2023-04-20 20:15:56.493061 dateUts-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3159 2023-04-20 19:57:17.000000 dateUts-0.1.5/README.md
+-rw-rw-rw-   0        0        0      122 2022-10-03 19:44:47.000000 dateUts-0.1.5/commands.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 20:15:56.481069 dateUts-0.1.5/dateUts/
+-rw-rw-rw-   0        0        0     4751 2023-04-20 19:55:03.000000 dateUts-0.1.5/dateUts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:15:56.491063 dateUts-0.1.5/dateUts.egg-info/
+-rw-rw-rw-   0        0        0     6136 2023-04-20 20:15:56.000000 dateUts-0.1.5/dateUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-04-20 20:15:56.000000 dateUts-0.1.5/dateUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 20:15:56.000000 dateUts-0.1.5/dateUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-20 20:15:56.000000 dateUts-0.1.5/dateUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 20:15:56.495061 dateUts-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-04-20 20:03:43.000000 dateUts-0.1.5/setup.py
```

### Comparing `dateUts-0.1.4/CHANGELOG.txt` & `dateUts-0.1.5/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.4/DateUts/__init__.py` & `dateUts-0.1.5/dateUts/__init__.py`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.4/DateUts.egg-info/PKG-INFO` & `dateUts-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dateUts
-Version: 0.1.4
+Version: 0.1.5
 Summary: Date package
 Home-page: UNKNOWN
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Description: # Sql Uts
         #
```

### Comparing `dateUts-0.1.4/LICENCE.txt` & `dateUts-0.1.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.4/PKG-INFO` & `dateUts-0.1.5/dateUts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dateUts
-Version: 0.1.4
+Version: 0.1.5
 Summary: Date package
 Home-page: UNKNOWN
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Description: # Sql Uts
         #
```

### Comparing `dateUts-0.1.4/README.md` & `dateUts-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.4/setup.py` & `dateUts-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='dateUts',
-  version='0.1.4',
+  version='0.1.5',
   description='Date package',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

