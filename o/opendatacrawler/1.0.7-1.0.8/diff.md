# Comparing `tmp/opendatacrawler-1.0.7.tar.gz` & `tmp/opendatacrawler-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendatacrawler-1.0.7.tar", last modified: Thu Apr 20 15:21:08 2023, max compression
+gzip compressed data, was "opendatacrawler-1.0.8.tar", last modified: Thu Apr 20 15:31:34 2023, max compression
```

## Comparing `opendatacrawler-1.0.7.tar` & `opendatacrawler-1.0.8.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:21:08.569641 opendatacrawler-1.0.7/
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1070 2023-02-03 16:41:45.000000 opendatacrawler-1.0.7/LICENSE
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:21:08.568738 opendatacrawler-1.0.7/PKG-INFO
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7205 2023-03-08 15:49:21.000000 opendatacrawler-1.0.7/README.md
-drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:21:08.526176 opendatacrawler-1.0.7/opendatacrawler/
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4613 2023-04-20 15:15:12.000000 opendatacrawler-1.0.7/opendatacrawler/CkanCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3928 2023-04-20 15:19:24.000000 opendatacrawler-1.0.7/opendatacrawler/INECrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4644 2023-04-20 15:19:53.000000 opendatacrawler-1.0.7/opendatacrawler/OpenDataSoftCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1935 2023-04-20 15:14:34.000000 opendatacrawler-1.0.7/opendatacrawler/SocrataCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3164 2023-04-20 15:20:49.000000 opendatacrawler-1.0.7/opendatacrawler/ZenodoCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       95 2023-04-20 15:17:05.000000 opendatacrawler-1.0.7/opendatacrawler/__init__.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9194 2023-04-20 15:13:21.000000 opendatacrawler-1.0.7/opendatacrawler/__main__.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     6214 2023-04-20 15:18:49.000000 opendatacrawler-1.0.7/opendatacrawler/datosgobescrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3101 2023-04-20 15:18:33.000000 opendatacrawler-1.0.7/opendatacrawler/eurostatcrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9669 2023-04-20 15:16:58.000000 opendatacrawler-1.0.7/opendatacrawler/odcrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1938 2023-03-16 09:49:44.000000 opendatacrawler-1.0.7/opendatacrawler/opendatacrawlerInterface.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      881 2023-02-03 16:41:45.000000 opendatacrawler-1.0.7/opendatacrawler/setup_logger.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     5119 2023-04-20 15:11:35.000000 opendatacrawler-1.0.7/opendatacrawler/utils.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     2480 2023-04-20 15:14:50.000000 opendatacrawler-1.0.7/opendatacrawler/worldbankcrawler.py
-drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:21:08.567195 opendatacrawler-1.0.7/opendatacrawler.egg-info/
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:21:08.000000 opendatacrawler-1.0.7/opendatacrawler.egg-info/PKG-INFO
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      723 2023-04-20 15:21:08.000000 opendatacrawler-1.0.7/opendatacrawler.egg-info/SOURCES.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)        1 2023-04-20 15:21:08.000000 opendatacrawler-1.0.7/opendatacrawler.egg-info/dependency_links.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       58 2023-04-20 15:21:08.000000 opendatacrawler-1.0.7/opendatacrawler.egg-info/entry_points.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       12 2023-04-20 15:21:08.000000 opendatacrawler-1.0.7/opendatacrawler.egg-info/requires.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       16 2023-04-20 15:21:08.000000 opendatacrawler-1.0.7/opendatacrawler.egg-info/top_level.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       38 2023-04-20 15:21:08.569714 opendatacrawler-1.0.7/setup.cfg
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      988 2023-04-20 15:21:04.000000 opendatacrawler-1.0.7/setup.py
+drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:31:34.167551 opendatacrawler-1.0.8/
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1070 2023-02-03 16:41:45.000000 opendatacrawler-1.0.8/LICENSE
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:31:34.166943 opendatacrawler-1.0.8/PKG-INFO
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7205 2023-03-08 15:49:21.000000 opendatacrawler-1.0.8/README.md
+drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:31:34.144004 opendatacrawler-1.0.8/opendatacrawler/
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4613 2023-04-20 15:15:12.000000 opendatacrawler-1.0.8/opendatacrawler/CkanCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3928 2023-04-20 15:19:24.000000 opendatacrawler-1.0.8/opendatacrawler/INECrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4644 2023-04-20 15:19:53.000000 opendatacrawler-1.0.8/opendatacrawler/OpenDataSoftCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1935 2023-04-20 15:14:34.000000 opendatacrawler-1.0.8/opendatacrawler/SocrataCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3164 2023-04-20 15:20:49.000000 opendatacrawler-1.0.8/opendatacrawler/ZenodoCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       95 2023-04-20 15:17:05.000000 opendatacrawler-1.0.8/opendatacrawler/__init__.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9194 2023-04-20 15:13:21.000000 opendatacrawler-1.0.8/opendatacrawler/__main__.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     6214 2023-04-20 15:18:49.000000 opendatacrawler-1.0.8/opendatacrawler/datosgobescrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3101 2023-04-20 15:18:33.000000 opendatacrawler-1.0.8/opendatacrawler/eurostatcrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      818 2023-02-03 16:41:45.000000 opendatacrawler-1.0.8/opendatacrawler/intro.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9669 2023-04-20 15:16:58.000000 opendatacrawler-1.0.8/opendatacrawler/odcrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1938 2023-03-16 09:49:44.000000 opendatacrawler-1.0.8/opendatacrawler/opendatacrawlerInterface.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      881 2023-02-03 16:41:45.000000 opendatacrawler-1.0.8/opendatacrawler/setup_logger.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     5119 2023-04-20 15:11:35.000000 opendatacrawler-1.0.8/opendatacrawler/utils.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     2480 2023-04-20 15:14:50.000000 opendatacrawler-1.0.8/opendatacrawler/worldbankcrawler.py
+drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:31:34.165810 opendatacrawler-1.0.8/opendatacrawler.egg-info/
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:31:33.000000 opendatacrawler-1.0.8/opendatacrawler.egg-info/PKG-INFO
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      749 2023-04-20 15:31:34.000000 opendatacrawler-1.0.8/opendatacrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)        1 2023-04-20 15:31:33.000000 opendatacrawler-1.0.8/opendatacrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       58 2023-04-20 15:31:33.000000 opendatacrawler-1.0.8/opendatacrawler.egg-info/entry_points.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       12 2023-04-20 15:31:33.000000 opendatacrawler-1.0.8/opendatacrawler.egg-info/requires.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       16 2023-04-20 15:31:33.000000 opendatacrawler-1.0.8/opendatacrawler.egg-info/top_level.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       38 2023-04-20 15:31:34.167631 opendatacrawler-1.0.8/setup.cfg
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1041 2023-04-20 15:31:30.000000 opendatacrawler-1.0.8/setup.py
```

### Comparing `opendatacrawler-1.0.7/LICENSE` & `opendatacrawler-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/PKG-INFO` & `opendatacrawler-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendatacrawler
-Version: 1.0.7
+Version: 1.0.8
 Summary: Crawler for open data portals
 Home-page: https://github.com/aberenguerpas/OpenDataCrawler/
 Author: Alberto Berenguer Pastor
 Author-email: alberto.berenguer@ua.es
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.7 Summary: Crawler for
+Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.8 Summary: Crawler for
 open data portals Home-page: https://github.com/aberenguerpas/OpenDataCrawler/
 Author: Alberto Berenguer Pastor Author-email: alberto.berenguer@ua.es License:
 MIT Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
 [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
```

### Comparing `opendatacrawler-1.0.7/README.md` & `opendatacrawler-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/opendatacrawler/CkanCrawler.py` & `opendatacrawler-1.0.8/opendatacrawler/CkanCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/opendatacrawler/INECrawler.py` & `opendatacrawler-1.0.8/opendatacrawler/INECrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/opendatacrawler/OpenDataSoftCrawler.py` & `opendatacrawler-1.0.8/opendatacrawler/OpenDataSoftCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/opendatacrawler/SocrataCrawler.py` & `opendatacrawler-1.0.8/opendatacrawler/SocrataCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/opendatacrawler/ZenodoCrawler.py` & `opendatacrawler-1.0.8/opendatacrawler/ZenodoCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/opendatacrawler/__main__.py` & `opendatacrawler-1.0.8/opendatacrawler/__main__.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/opendatacrawler/datosgobescrawler.py` & `opendatacrawler-1.0.8/opendatacrawler/datosgobescrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/opendatacrawler/eurostatcrawler.py` & `opendatacrawler-1.0.8/opendatacrawler/eurostatcrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/opendatacrawler/odcrawler.py` & `opendatacrawler-1.0.8/opendatacrawler/odcrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/opendatacrawler/opendatacrawlerInterface.py` & `opendatacrawler-1.0.8/opendatacrawler/opendatacrawlerInterface.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/opendatacrawler/setup_logger.py` & `opendatacrawler-1.0.8/opendatacrawler/setup_logger.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/opendatacrawler/utils.py` & `opendatacrawler-1.0.8/opendatacrawler/utils.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/opendatacrawler/worldbankcrawler.py` & `opendatacrawler-1.0.8/opendatacrawler/worldbankcrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.7/opendatacrawler.egg-info/PKG-INFO` & `opendatacrawler-1.0.8/opendatacrawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendatacrawler
-Version: 1.0.7
+Version: 1.0.8
 Summary: Crawler for open data portals
 Home-page: https://github.com/aberenguerpas/OpenDataCrawler/
 Author: Alberto Berenguer Pastor
 Author-email: alberto.berenguer@ua.es
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.7 Summary: Crawler for
+Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.8 Summary: Crawler for
 open data portals Home-page: https://github.com/aberenguerpas/OpenDataCrawler/
 Author: Alberto Berenguer Pastor Author-email: alberto.berenguer@ua.es License:
 MIT Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
 [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
```

### Comparing `opendatacrawler-1.0.7/opendatacrawler.egg-info/SOURCES.txt` & `opendatacrawler-1.0.8/opendatacrawler.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 opendatacrawler/OpenDataSoftCrawler.py
 opendatacrawler/SocrataCrawler.py
 opendatacrawler/ZenodoCrawler.py
 opendatacrawler/__init__.py
 opendatacrawler/__main__.py
 opendatacrawler/datosgobescrawler.py
 opendatacrawler/eurostatcrawler.py
+opendatacrawler/intro.txt
 opendatacrawler/odcrawler.py
 opendatacrawler/opendatacrawlerInterface.py
 opendatacrawler/setup_logger.py
 opendatacrawler/utils.py
 opendatacrawler/worldbankcrawler.py
 opendatacrawler.egg-info/PKG-INFO
 opendatacrawler.egg-info/SOURCES.txt
```

### Comparing `opendatacrawler-1.0.7/setup.py` & `opendatacrawler-1.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="opendatacrawler",
-    version="1.0.7",
+    version="1.0.8",
     description="Crawler for open data portals",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/aberenguerpas/OpenDataCrawler/",
     author="Alberto Berenguer Pastor",
     author_email="alberto.berenguer@ua.es",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
     ],
     packages=find_packages(),
     include_package_data=True,
+    package_data={'opendatacrawler': ['intro.txt']},
     install_requires=["tqdm","sodapy"],
     entry_points={
         "console_scripts": [
             "crawler=opendatacrawler.__main__:main",
         ]
     },
 )
```

