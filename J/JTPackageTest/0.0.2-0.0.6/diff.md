# Comparing `tmp/JTPackageTest-0.0.2.tar.gz` & `tmp/JTPackageTest-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JTPackageTest-0.0.2.tar", last modified: Thu Apr 20 17:41:53 2023, max compression
+gzip compressed data, was "JTPackageTest-0.0.6.tar", last modified: Thu Apr 20 17:25:05 2023, max compression
```

## Comparing `JTPackageTest-0.0.2.tar` & `JTPackageTest-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 17:41:53.023254 JTPackageTest-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-04-20 17:41:52.967715 JTPackageTest-0.0.2/JTPackageTest.egg-info/
--rw-rw-rw-   0        0        0      565 2023-04-20 17:41:52.000000 JTPackageTest-0.0.2/JTPackageTest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-20 17:41:52.000000 JTPackageTest-0.0.2/JTPackageTest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 17:41:52.000000 JTPackageTest-0.0.2/JTPackageTest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-20 17:41:52.000000 JTPackageTest-0.0.2/JTPackageTest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-20 17:41:52.000000 JTPackageTest-0.0.2/JTPackageTest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      565 2023-04-20 17:41:53.022255 JTPackageTest-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-20 17:41:52.975708 JTPackageTest-0.0.2/TestPackage/
--rw-rw-rw-   0        0        0        0 2023-04-20 17:41:31.000000 JTPackageTest-0.0.2/TestPackage/__init__.py
--rw-rw-rw-   0        0        0       43 2023-04-20 17:41:33.000000 JTPackageTest-0.0.2/TestPackage/test.py
--rw-rw-rw-   0        0        0       42 2023-04-20 17:41:53.023254 JTPackageTest-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1107 2023-04-20 17:41:39.000000 JTPackageTest-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:25:05.348272 JTPackageTest-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-04-20 17:25:05.338272 JTPackageTest-0.0.6/JTPackageTest.egg-info/
+-rw-rw-rw-   0        0        0      565 2023-04-20 17:25:05.000000 JTPackageTest-0.0.6/JTPackageTest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-20 17:25:05.000000 JTPackageTest-0.0.6/JTPackageTest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 17:25:05.000000 JTPackageTest-0.0.6/JTPackageTest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-20 17:25:05.000000 JTPackageTest-0.0.6/JTPackageTest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 17:25:05.000000 JTPackageTest-0.0.6/JTPackageTest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      565 2023-04-20 17:25:05.347273 JTPackageTest-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-20 17:25:05.343291 JTPackageTest-0.0.6/TestPackage/
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:08:02.000000 JTPackageTest-0.0.6/TestPackage/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:07:39.000000 JTPackageTest-0.0.6/TestPackage/test.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 17:25:05.348272 JTPackageTest-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1107 2023-04-20 17:24:05.000000 JTPackageTest-0.0.6/setup.py
```

### Comparing `JTPackageTest-0.0.2/JTPackageTest.egg-info/PKG-INFO` & `JTPackageTest-0.0.6/JTPackageTest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JTPackageTest
-Version: 0.0.2
+Version: 0.0.6
 Summary: Testing module functionality and package creation
 Author: Joshua Taylor
 Author-email: joshua.taylor@integer-tech.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `JTPackageTest-0.0.2/PKG-INFO` & `JTPackageTest-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JTPackageTest
-Version: 0.0.2
+Version: 0.0.6
 Summary: Testing module functionality and package creation
 Author: Joshua Taylor
 Author-email: joshua.taylor@integer-tech.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `JTPackageTest-0.0.2/setup.py` & `JTPackageTest-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'Testing module functionality and package creation'
 LONG_DESCRIPTION = 'Testing module functionality and package creation'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="JTPackageTest",
```

