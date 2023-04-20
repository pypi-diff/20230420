# Comparing `tmp/plix_kws-0.1015.tar.gz` & `tmp/plix_kws-0.1016.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plix_kws-0.1015.tar", last modified: Thu Apr 20 12:13:33 2023, max compression
+gzip compressed data, was "plix_kws-0.1016.tar", last modified: Thu Apr 20 12:23:23 2023, max compression
```

## Comparing `plix_kws-0.1015.tar` & `plix_kws-0.1016.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 12:13:33.517427 plix_kws-0.1015/
--rw-rw-rw-   0        0        0    11558 2023-04-20 10:09:41.000000 plix_kws-0.1015/LICENSE
--rw-rw-rw-   0        0        0     3907 2023-04-20 12:13:33.517427 plix_kws-0.1015/PKG-INFO
--rw-rw-rw-   0        0        0     3405 2023-04-20 11:51:09.000000 plix_kws-0.1015/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 12:13:33.517427 plix_kws-0.1015/plix_kws.egg-info/
--rw-rw-rw-   0        0        0     3907 2023-04-20 12:13:33.000000 plix_kws-0.1015/plix_kws.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-04-20 12:13:33.000000 plix_kws-0.1015/plix_kws.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 12:13:33.000000 plix_kws-0.1015/plix_kws.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-20 12:13:33.000000 plix_kws-0.1015/plix_kws.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 12:13:33.000000 plix_kws-0.1015/plix_kws.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 12:13:33.517427 plix_kws-0.1015/setup.cfg
--rw-rw-rw-   0        0        0      899 2023-04-20 12:12:57.000000 plix_kws-0.1015/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:23:23.407747 plix_kws-0.1016/
+-rw-rw-rw-   0        0        0    11558 2023-04-20 10:09:41.000000 plix_kws-0.1016/LICENSE
+-rw-rw-rw-   0        0        0     3907 2023-04-20 12:23:23.407747 plix_kws-0.1016/PKG-INFO
+-rw-rw-rw-   0        0        0     3405 2023-04-20 11:51:09.000000 plix_kws-0.1016/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 12:23:23.407747 plix_kws-0.1016/plix_kws.egg-info/
+-rw-rw-rw-   0        0        0     3907 2023-04-20 12:23:23.000000 plix_kws-0.1016/plix_kws.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-04-20 12:23:23.000000 plix_kws-0.1016/plix_kws.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 12:23:23.000000 plix_kws-0.1016/plix_kws.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-20 12:23:23.000000 plix_kws-0.1016/plix_kws.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 12:23:23.000000 plix_kws-0.1016/plix_kws.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 12:23:23.407747 plix_kws-0.1016/setup.cfg
+-rw-rw-rw-   0        0        0      899 2023-04-20 12:23:11.000000 plix_kws-0.1016/setup.py
```

### Comparing `plix_kws-0.1015/LICENSE` & `plix_kws-0.1016/LICENSE`

 * *Files identical despite different names*

### Comparing `plix_kws-0.1015/PKG-INFO` & `plix_kws-0.1016/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plix_kws
-Version: 0.1015
+Version: 0.1016
 Summary: Plug-and-Play Multilingual Few-shot Spoken Words Recognition
 Home-page: https://github.com/plix-kws/plix-kws
 Download-URL: https://pypi.org/project/plix_kws/
 Author: Aaqib Saeed
 Author-email: plix-kws@proton.me
 License: Apache-2.0 license
 Keywords: Keyword Spotting,Few-shot Learning,Deep Neural Network,Audio,Speech
```

### Comparing `plix_kws-0.1015/README.md` & `plix_kws-0.1016/README.md`

 * *Files identical despite different names*

### Comparing `plix_kws-0.1015/plix_kws.egg-info/PKG-INFO` & `plix_kws-0.1016/plix_kws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plix-kws
-Version: 0.1015
+Version: 0.1016
 Summary: Plug-and-Play Multilingual Few-shot Spoken Words Recognition
 Home-page: https://github.com/plix-kws/plix-kws
 Download-URL: https://pypi.org/project/plix_kws/
 Author: Aaqib Saeed
 Author-email: plix-kws@proton.me
 License: Apache-2.0 license
 Keywords: Keyword Spotting,Few-shot Learning,Deep Neural Network,Audio,Speech
```

### Comparing `plix_kws-0.1015/setup.py` & `plix_kws-0.1016/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name="plix_kws",
-    version="0.1015",
+    version="0.1016",
     description="Plug-and-Play Multilingual Few-shot Spoken Words Recognition",
     long_description_content_type="text/markdown",
     long_description=README,
     license="Apache-2.0 license",
     packages=find_packages(),
     author="Aaqib Saeed",
     author_email="plix-kws@proton.me",
```

