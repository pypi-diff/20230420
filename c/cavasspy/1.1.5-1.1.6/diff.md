# Comparing `tmp/cavasspy-1.1.5.tar.gz` & `tmp/cavasspy-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cavasspy-1.1.5.tar", last modified: Thu Apr 20 08:05:28 2023, max compression
+gzip compressed data, was "cavasspy-1.1.6.tar", last modified: Thu Apr 20 08:08:02 2023, max compression
```

## Comparing `cavasspy-1.1.5.tar` & `cavasspy-1.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-04-20 08:05:28.415721 cavasspy-1.1.5/
--rw-r--r--   0 daijian    (501) staff       (20)    35149 2022-01-18 06:32:18.000000 cavasspy-1.1.5/LICENSE
--rw-r--r--   0 daijian    (501) staff       (20)      837 2023-04-20 08:05:28.415256 cavasspy-1.1.5/PKG-INFO
--rw-r--r--   0 daijian    (501) staff       (20)      438 2022-08-03 14:11:17.000000 cavasspy-1.1.5/README.md
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-04-20 08:05:28.410635 cavasspy-1.1.5/cavasspy/
--rw-r--r--   0 daijian    (501) staff       (20)        0 2022-08-03 11:45:14.000000 cavasspy-1.1.5/cavasspy/__init__.py
--rw-r--r--   0 daijian    (501) staff       (20)      971 2023-04-20 07:56:18.000000 cavasspy-1.1.5/cavasspy/converter.py
--rw-r--r--   0 daijian    (501) staff       (20)      837 2023-04-20 01:40:19.000000 cavasspy-1.1.5/cavasspy/match.py
--rw-r--r--   0 daijian    (501) staff       (20)     6161 2023-04-20 07:50:32.000000 cavasspy-1.1.5/cavasspy/op.py
--rw-r--r--   0 daijian    (501) staff       (20)      552 2022-09-01 11:35:28.000000 cavasspy-1.1.5/cavasspy/window_transform.py
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-04-20 08:05:28.413279 cavasspy-1.1.5/cavasspy.egg-info/
--rw-r--r--   0 daijian    (501) staff       (20)      837 2023-04-20 08:05:27.000000 cavasspy-1.1.5/cavasspy.egg-info/PKG-INFO
--rw-r--r--   0 daijian    (501) staff       (20)      290 2023-04-20 08:05:28.000000 cavasspy-1.1.5/cavasspy.egg-info/SOURCES.txt
--rw-r--r--   0 daijian    (501) staff       (20)        1 2023-04-20 08:05:27.000000 cavasspy-1.1.5/cavasspy.egg-info/dependency_links.txt
--rw-r--r--   0 daijian    (501) staff       (20)       16 2023-04-20 08:05:27.000000 cavasspy-1.1.5/cavasspy.egg-info/requires.txt
--rw-r--r--   0 daijian    (501) staff       (20)        9 2023-04-20 08:05:27.000000 cavasspy-1.1.5/cavasspy.egg-info/top_level.txt
--rw-r--r--   0 daijian    (501) staff       (20)       38 2023-04-20 08:05:28.415890 cavasspy-1.1.5/setup.cfg
--rw-r--r--   0 daijian    (501) staff       (20)      672 2023-04-20 08:05:24.000000 cavasspy-1.1.5/setup.py
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-04-20 08:08:02.876333 cavasspy-1.1.6/
+-rw-r--r--   0 daijian    (501) staff       (20)    35149 2022-01-18 06:32:18.000000 cavasspy-1.1.6/LICENSE
+-rw-r--r--   0 daijian    (501) staff       (20)      837 2023-04-20 08:08:02.875958 cavasspy-1.1.6/PKG-INFO
+-rw-r--r--   0 daijian    (501) staff       (20)      438 2022-08-03 14:11:17.000000 cavasspy-1.1.6/README.md
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-04-20 08:08:02.873519 cavasspy-1.1.6/cavasspy/
+-rw-r--r--   0 daijian    (501) staff       (20)        0 2022-08-03 11:45:14.000000 cavasspy-1.1.6/cavasspy/__init__.py
+-rw-r--r--   0 daijian    (501) staff       (20)      979 2023-04-20 08:07:22.000000 cavasspy-1.1.6/cavasspy/converter.py
+-rw-r--r--   0 daijian    (501) staff       (20)      837 2023-04-20 01:40:19.000000 cavasspy-1.1.6/cavasspy/match.py
+-rw-r--r--   0 daijian    (501) staff       (20)     6161 2023-04-20 07:50:32.000000 cavasspy-1.1.6/cavasspy/op.py
+-rw-r--r--   0 daijian    (501) staff       (20)      552 2022-09-01 11:35:28.000000 cavasspy-1.1.6/cavasspy/window_transform.py
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-04-20 08:08:02.875363 cavasspy-1.1.6/cavasspy.egg-info/
+-rw-r--r--   0 daijian    (501) staff       (20)      837 2023-04-20 08:08:02.000000 cavasspy-1.1.6/cavasspy.egg-info/PKG-INFO
+-rw-r--r--   0 daijian    (501) staff       (20)      290 2023-04-20 08:08:02.000000 cavasspy-1.1.6/cavasspy.egg-info/SOURCES.txt
+-rw-r--r--   0 daijian    (501) staff       (20)        1 2023-04-20 08:08:02.000000 cavasspy-1.1.6/cavasspy.egg-info/dependency_links.txt
+-rw-r--r--   0 daijian    (501) staff       (20)       16 2023-04-20 08:08:02.000000 cavasspy-1.1.6/cavasspy.egg-info/requires.txt
+-rw-r--r--   0 daijian    (501) staff       (20)        9 2023-04-20 08:08:02.000000 cavasspy-1.1.6/cavasspy.egg-info/top_level.txt
+-rw-r--r--   0 daijian    (501) staff       (20)       38 2023-04-20 08:08:02.876451 cavasspy-1.1.6/setup.cfg
+-rw-r--r--   0 daijian    (501) staff       (20)      672 2023-04-20 08:07:59.000000 cavasspy-1.1.6/setup.py
```

### Comparing `cavasspy-1.1.5/LICENSE` & `cavasspy-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cavasspy-1.1.5/PKG-INFO` & `cavasspy-1.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cavasspy
-Version: 1.1.5
+Version: 1.1.6
 Summary: CAVASS python APIs.
 Author: Dai Jian
 Author-email: daijian@stumail.ysu.edu.cn
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
```

### Comparing `cavasspy-1.1.5/cavasspy/match.py` & `cavasspy-1.1.6/cavasspy/match.py`

 * *Files identical despite different names*

### Comparing `cavasspy-1.1.5/cavasspy/op.py` & `cavasspy-1.1.6/cavasspy/op.py`

 * *Files identical despite different names*

### Comparing `cavasspy-1.1.5/cavasspy/window_transform.py` & `cavasspy-1.1.6/cavasspy/window_transform.py`

 * *Files identical despite different names*

### Comparing `cavasspy-1.1.5/cavasspy.egg-info/PKG-INFO` & `cavasspy-1.1.6/cavasspy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cavasspy
-Version: 1.1.5
+Version: 1.1.6
 Summary: CAVASS python APIs.
 Author: Dai Jian
 Author-email: daijian@stumail.ysu.edu.cn
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
```

### Comparing `cavasspy-1.1.5/setup.py` & `cavasspy-1.1.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='cavasspy',
-    version='1.1.5',
+    version='1.1.6',
     author='Dai Jian',
     author_email='daijian@stumail.ysu.edu.cn',
     description='CAVASS python APIs.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
```

