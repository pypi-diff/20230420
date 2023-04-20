# Comparing `tmp/spiralflow-0.0.1.tar.gz` & `tmp/spiralflow-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiralflow-0.0.1.tar", last modified: Thu Apr 20 04:19:33 2023, max compression
+gzip compressed data, was "spiralflow-0.0.2.tar", last modified: Thu Apr 20 04:20:49 2023, max compression
```

## Comparing `spiralflow-0.0.1.tar` & `spiralflow-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 04:19:33.438963 spiralflow-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-04-09 17:15:16.000000 spiralflow-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    12765 2023-04-20 04:19:33.433976 spiralflow-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    12239 2023-04-20 04:15:29.000000 spiralflow-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 04:19:33.438963 spiralflow-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-04-20 04:13:52.000000 spiralflow-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 04:19:33.420952 spiralflow-0.0.1/spiralflow/
--rw-rw-rw-   0        0        0       22 2023-04-19 15:05:48.000000 spiralflow-0.0.1/spiralflow/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-04-14 04:47:37.000000 spiralflow-0.0.1/spiralflow/chat_history.py
--rw-rw-rw-   0        0        0     1330 2023-04-14 04:47:37.000000 spiralflow-0.0.1/spiralflow/chat_llm.py
--rw-rw-rw-   0        0        0    52297 2023-04-19 15:05:49.000000 spiralflow-0.0.1/spiralflow/flow.py
--rw-rw-rw-   0        0        0     7781 2023-04-19 15:05:48.000000 spiralflow-0.0.1/spiralflow/memory.py
--rw-rw-rw-   0        0        0    16849 2023-04-19 15:05:24.000000 spiralflow-0.0.1/spiralflow/message.py
--rw-rw-rw-   0        0        0     2266 2023-04-14 15:31:34.000000 spiralflow-0.0.1/spiralflow/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-20 04:19:33.432979 spiralflow-0.0.1/spiralflow.egg-info/
--rw-rw-rw-   0        0        0    12765 2023-04-20 04:19:33.000000 spiralflow-0.0.1/spiralflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-04-20 04:19:33.000000 spiralflow-0.0.1/spiralflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 04:19:33.000000 spiralflow-0.0.1/spiralflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-20 04:19:33.000000 spiralflow-0.0.1/spiralflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 04:19:33.000000 spiralflow-0.0.1/spiralflow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 04:20:49.827964 spiralflow-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-04-09 17:15:16.000000 spiralflow-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    12765 2023-04-20 04:20:49.823975 spiralflow-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12239 2023-04-20 04:15:29.000000 spiralflow-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 04:20:49.827964 spiralflow-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-04-20 04:20:43.000000 spiralflow-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 04:20:49.810801 spiralflow-0.0.2/spiralflow/
+-rw-rw-rw-   0        0        0       22 2023-04-20 04:20:31.000000 spiralflow-0.0.2/spiralflow/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-04-14 04:47:37.000000 spiralflow-0.0.2/spiralflow/chat_history.py
+-rw-rw-rw-   0        0        0     1330 2023-04-14 04:47:37.000000 spiralflow-0.0.2/spiralflow/chat_llm.py
+-rw-rw-rw-   0        0        0    52297 2023-04-19 15:05:49.000000 spiralflow-0.0.2/spiralflow/flow.py
+-rw-rw-rw-   0        0        0     7781 2023-04-19 15:05:48.000000 spiralflow-0.0.2/spiralflow/memory.py
+-rw-rw-rw-   0        0        0    16849 2023-04-19 15:05:24.000000 spiralflow-0.0.2/spiralflow/message.py
+-rw-rw-rw-   0        0        0     2266 2023-04-14 15:31:34.000000 spiralflow-0.0.2/spiralflow/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-20 04:20:49.821813 spiralflow-0.0.2/spiralflow.egg-info/
+-rw-rw-rw-   0        0        0    12765 2023-04-20 04:20:49.000000 spiralflow-0.0.2/spiralflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-04-20 04:20:49.000000 spiralflow-0.0.2/spiralflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 04:20:49.000000 spiralflow-0.0.2/spiralflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-20 04:20:49.000000 spiralflow-0.0.2/spiralflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 04:20:49.000000 spiralflow-0.0.2/spiralflow.egg-info/top_level.txt
```

### Comparing `spiralflow-0.0.1/LICENSE` & `spiralflow-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.1/PKG-INFO` & `spiralflow-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiralflow
-Version: 0.0.1
+Version: 0.0.2
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/Spiralflow
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spiralflow-0.0.1/README.md` & `spiralflow-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.1/setup.py` & `spiralflow-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spiralflow",
-    version="0.0.1",
+    version="0.0.2",
     author="Travis Hammond",
     description="A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tiger767/Spiralflow",
     packages=setuptools.find_packages(),
     install_requires=[
```

### Comparing `spiralflow-0.0.1/spiralflow/chat_history.py` & `spiralflow-0.0.2/spiralflow/chat_history.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.1/spiralflow/chat_llm.py` & `spiralflow-0.0.2/spiralflow/chat_llm.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.1/spiralflow/flow.py` & `spiralflow-0.0.2/spiralflow/flow.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.1/spiralflow/memory.py` & `spiralflow-0.0.2/spiralflow/memory.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.1/spiralflow/message.py` & `spiralflow-0.0.2/spiralflow/message.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.1/spiralflow/tools.py` & `spiralflow-0.0.2/spiralflow/tools.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.1/spiralflow.egg-info/PKG-INFO` & `spiralflow-0.0.2/spiralflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiralflow
-Version: 0.0.1
+Version: 0.0.2
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/Spiralflow
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

