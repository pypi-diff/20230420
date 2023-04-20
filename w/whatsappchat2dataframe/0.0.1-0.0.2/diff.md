# Comparing `tmp/whatsappchat2dataframe-0.0.1.tar.gz` & `tmp/whatsappchat2dataframe-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsappchat2dataframe-0.0.1.tar", last modified: Thu Apr 20 19:12:49 2023, max compression
+gzip compressed data, was "whatsappchat2dataframe-0.0.2.tar", last modified: Thu Apr 20 19:29:56 2023, max compression
```

## Comparing `whatsappchat2dataframe-0.0.1.tar` & `whatsappchat2dataframe-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 19:12:49.953174 whatsappchat2dataframe-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-04-20 19:12:16.000000 whatsappchat2dataframe-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      844 2023-04-20 19:12:49.952188 whatsappchat2dataframe-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-20 12:30:20.000000 whatsappchat2dataframe-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 19:12:49.953174 whatsappchat2dataframe-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1078 2023-04-20 12:56:53.000000 whatsappchat2dataframe-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 19:12:49.932175 whatsappchat2dataframe-0.0.1/whatsappchat2dataframe/
--rw-rw-rw-   0        0        0       59 2023-04-20 12:54:20.000000 whatsappchat2dataframe-0.0.1/whatsappchat2dataframe/__init__.py
--rw-rw-rw-   0        0        0     1552 2023-04-20 12:54:48.000000 whatsappchat2dataframe-0.0.1/whatsappchat2dataframe/chat2dataframe.py
-drwxrwxrwx   0        0        0        0 2023-04-20 19:12:49.951173 whatsappchat2dataframe-0.0.1/whatsappchat2dataframe.egg-info/
--rw-rw-rw-   0        0        0      844 2023-04-20 19:12:49.000000 whatsappchat2dataframe-0.0.1/whatsappchat2dataframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-04-20 19:12:49.000000 whatsappchat2dataframe-0.0.1/whatsappchat2dataframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 19:12:49.000000 whatsappchat2dataframe-0.0.1/whatsappchat2dataframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-20 19:12:49.000000 whatsappchat2dataframe-0.0.1/whatsappchat2dataframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-04-20 19:12:49.000000 whatsappchat2dataframe-0.0.1/whatsappchat2dataframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 19:29:56.455076 whatsappchat2dataframe-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-04-20 19:12:16.000000 whatsappchat2dataframe-0.0.2/LICENCE
+-rw-rw-rw-   0        0        0      844 2023-04-20 19:29:56.454063 whatsappchat2dataframe-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-20 12:30:20.000000 whatsappchat2dataframe-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 19:29:56.455076 whatsappchat2dataframe-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-04-20 19:29:42.000000 whatsappchat2dataframe-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:29:56.442872 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe/
+-rw-rw-rw-   0        0        0       59 2023-04-20 12:54:20.000000 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe/__init__.py
+-rw-rw-rw-   0        0        0     1552 2023-04-20 12:54:48.000000 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe/chat2dataframe.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:29:56.453549 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe.egg-info/
+-rw-rw-rw-   0        0        0      844 2023-04-20 19:29:56.000000 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-04-20 19:29:56.000000 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 19:29:56.000000 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-20 19:29:56.000000 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-20 19:29:56.000000 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe.egg-info/top_level.txt
```

### Comparing `whatsappchat2dataframe-0.0.1/LICENCE` & `whatsappchat2dataframe-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `whatsappchat2dataframe-0.0.1/PKG-INFO` & `whatsappchat2dataframe-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsappchat2dataframe
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converting a Whatsapp chat into a pandas DataFrame
 Author: Kiran Busch
 Author-email: <kiranbusch@t-online.de>
 Keywords: python,whatsapp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `whatsappchat2dataframe-0.0.1/setup.py` & `whatsappchat2dataframe-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Converting a Whatsapp chat into a pandas DataFrame'
 LONG_DESCRIPTION = 'A package that allows...'
 
 # Setting up
 setup(
     name="whatsappchat2dataframe",
     version=VERSION,
     author="Kiran Busch",
     author_email="<kiranbusch@t-online.de>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['tqdm', 're', 'pandas'],
+    install_requires=['tqdm', 'regex', 'pandas'],
     keywords=['python', 'whatsapp'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `whatsappchat2dataframe-0.0.1/whatsappchat2dataframe/chat2dataframe.py` & `whatsappchat2dataframe-0.0.2/whatsappchat2dataframe/chat2dataframe.py`

 * *Files identical despite different names*

### Comparing `whatsappchat2dataframe-0.0.1/whatsappchat2dataframe.egg-info/PKG-INFO` & `whatsappchat2dataframe-0.0.2/whatsappchat2dataframe.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsappchat2dataframe
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converting a Whatsapp chat into a pandas DataFrame
 Author: Kiran Busch
 Author-email: <kiranbusch@t-online.de>
 Keywords: python,whatsapp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

