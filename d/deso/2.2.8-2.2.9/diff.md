# Comparing `tmp/deso-2.2.8.tar.gz` & `tmp/deso-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deso-2.2.8.tar", last modified: Sat Apr  8 09:21:16 2023, max compression
+gzip compressed data, was "deso-2.2.9.tar", last modified: Thu Apr 20 15:12:46 2023, max compression
```

## Comparing `deso-2.2.8.tar` & `deso-2.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 09:21:16.917606 deso-2.2.8/
--rw-rw-rw-   0        0        0     1085 2022-07-14 19:21:22.000000 deso-2.2.8/LICENSE
--rw-rw-rw-   0        0        0    20346 2023-04-08 09:21:16.916606 deso-2.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    19062 2023-01-11 16:08:21.000000 deso-2.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 09:21:16.879597 deso-2.2.8/deso/
--rw-rw-rw-   0        0        0     2262 2022-07-14 19:21:22.000000 deso-2.2.8/deso/Derived.py
--rw-rw-rw-   0        0        0     2838 2023-01-11 16:02:29.000000 deso-2.2.8/deso/Identity.py
--rw-rw-rw-   0        0        0     1032 2022-07-14 19:21:22.000000 deso-2.2.8/deso/Media.py
--rw-rw-rw-   0        0        0     1745 2022-07-14 19:21:22.000000 deso-2.2.8/deso/Metadata.py
--rw-rw-rw-   0        0        0     5883 2023-03-08 15:36:10.000000 deso-2.2.8/deso/Posts.py
--rw-rw-rw-   0        0        0     3759 2023-03-03 15:59:26.000000 deso-2.2.8/deso/Sign.py
--rw-rw-rw-   0        0        0    28489 2023-04-08 09:19:16.000000 deso-2.2.8/deso/Social.py
--rw-rw-rw-   0        0        0    15734 2022-07-14 19:21:22.000000 deso-2.2.8/deso/Trade.py
--rw-rw-rw-   0        0        0     7817 2022-12-09 09:21:26.000000 deso-2.2.8/deso/User.py
--rw-rw-rw-   0        0        0      256 2022-07-14 19:21:22.000000 deso-2.2.8/deso/__init__.py
--rw-rw-rw-   0        0        0     1634 2022-07-14 19:21:22.000000 deso-2.2.8/deso/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-08 09:21:16.914607 deso-2.2.8/deso.egg-info/
--rw-rw-rw-   0        0        0    20346 2023-04-08 09:21:15.000000 deso-2.2.8/deso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-04-08 09:21:16.000000 deso-2.2.8/deso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 09:21:15.000000 deso-2.2.8/deso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-08 09:21:16.000000 deso-2.2.8/deso.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-08 09:21:16.000000 deso-2.2.8/deso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 09:21:16.918606 deso-2.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1413 2023-04-08 09:19:46.000000 deso-2.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 15:12:46.579748 deso-2.2.9/
+-rw-rw-rw-   0        0        0     1085 2022-10-22 06:55:06.000000 deso-2.2.9/LICENSE
+-rw-rw-rw-   0        0        0    20360 2023-04-20 15:12:46.578495 deso-2.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    19062 2023-02-08 08:09:20.000000 deso-2.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 15:12:46.554368 deso-2.2.9/deso/
+-rw-rw-rw-   0        0        0     2262 2022-10-22 06:55:06.000000 deso-2.2.9/deso/Derived.py
+-rw-rw-rw-   0        0        0     2838 2023-02-08 08:09:20.000000 deso-2.2.9/deso/Identity.py
+-rw-rw-rw-   0        0        0     1032 2022-10-22 06:55:06.000000 deso-2.2.9/deso/Media.py
+-rw-rw-rw-   0        0        0     1745 2022-10-22 06:55:06.000000 deso-2.2.9/deso/Metadata.py
+-rw-rw-rw-   0        0        0     5422 2023-04-20 15:06:54.000000 deso-2.2.9/deso/Posts.py
+-rw-rw-rw-   0        0        0     3759 2023-04-16 19:32:16.000000 deso-2.2.9/deso/Sign.py
+-rw-rw-rw-   0        0        0    28489 2023-04-16 19:32:16.000000 deso-2.2.9/deso/Social.py
+-rw-rw-rw-   0        0        0    15734 2022-10-22 06:55:06.000000 deso-2.2.9/deso/Trade.py
+-rw-rw-rw-   0        0        0     7817 2023-02-08 08:09:20.000000 deso-2.2.9/deso/User.py
+-rw-rw-rw-   0        0        0      256 2022-10-22 06:55:06.000000 deso-2.2.9/deso/__init__.py
+-rw-rw-rw-   0        0        0     1634 2022-10-22 06:55:06.000000 deso-2.2.9/deso/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-20 15:12:46.575496 deso-2.2.9/deso.egg-info/
+-rw-rw-rw-   0        0        0    20360 2023-04-20 15:12:46.000000 deso-2.2.9/deso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-04-20 15:12:46.000000 deso-2.2.9/deso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 15:12:46.000000 deso-2.2.9/deso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-20 15:12:46.000000 deso-2.2.9/deso.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-20 15:12:46.000000 deso-2.2.9/deso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 15:12:46.580755 deso-2.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1425 2023-04-20 15:12:35.000000 deso-2.2.9/setup.py
```

### Comparing `deso-2.2.8/LICENSE` & `deso-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `deso-2.2.8/PKG-INFO` & `deso-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: deso
-Version: 2.2.8
+Version: 2.2.9
 Summary: A python module for deso
-Author: ItsAditya (https://diamondapp.com/u/ItsAditya)
+Author: ItsAditya (https://itsaditya.xyz)
 Author-email: <chaudharyaditya0005@gmail.com>
-Keywords: deso,python,bitclout,social media,crypto,blockchain,decentralisation
+Keywords: deso,python,bitclout,social media,crypto,blockchain,decentralisation,decentralized social media
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `deso-2.2.8/README.md` & `deso-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `deso-2.2.8/deso/Derived.py` & `deso-2.2.9/deso/Derived.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.8/deso/Identity.py` & `deso-2.2.9/deso/Identity.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.8/deso/Media.py` & `deso-2.2.9/deso/Media.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.8/deso/Metadata.py` & `deso-2.2.9/deso/Metadata.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.8/deso/Sign.py` & `deso-2.2.9/deso/Sign.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.8/deso/Social.py` & `deso-2.2.9/deso/Social.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.8/deso/Trade.py` & `deso-2.2.9/deso/Trade.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.8/deso/User.py` & `deso-2.2.9/deso/User.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.8/deso/utils.py` & `deso-2.2.9/deso/utils.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.8/deso.egg-info/PKG-INFO` & `deso-2.2.9/deso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: deso
-Version: 2.2.8
+Version: 2.2.9
 Summary: A python module for deso
-Author: ItsAditya (https://diamondapp.com/u/ItsAditya)
+Author: ItsAditya (https://itsaditya.xyz)
 Author-email: <chaudharyaditya0005@gmail.com>
-Keywords: deso,python,bitclout,social media,crypto,blockchain,decentralisation
+Keywords: deso,python,bitclout,social media,crypto,blockchain,decentralisation,decentralized social media
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `deso-2.2.8/setup.py` & `deso-2.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,36 +3,37 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "2.2.8"
+VERSION = "2.2.9"
 DESCRIPTION = "A python module for DeSo"
 LONG_DESCRIPTION = "DesoPy is a python module that enables devs to interact with DeSo Blockchain using node.deso.org node by default. Includes all functions to read from or write to DeSo Blockchain"
 # Setting up
 setup(
     name="deso",
     version=VERSION,
-    author="ItsAditya (https://diamondapp.com/u/ItsAditya)",
+    author="ItsAditya (https://itsaditya.xyz)",
     author_email="<chaudharyaditya0005@gmail.com>",
     description="A python module for deso",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=["PyJWT", "ecdsa", "arweave-python-client", "base58"],
+    install_requires=["PyJWT", "ecdsa", "base58", "hdwallet"],
     keywords=[
         "deso",
         "python",
         "bitclout",
         "social media",
         "crypto",
         "blockchain",
         "decentralisation",
+        "decentralized social media"
     ],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

