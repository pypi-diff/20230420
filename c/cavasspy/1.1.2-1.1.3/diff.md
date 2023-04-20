# Comparing `tmp/cavasspy-1.1.2.tar.gz` & `tmp/cavasspy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cavasspy-1.1.2.tar", last modified: Fri Mar 31 05:47:34 2023, max compression
+gzip compressed data, was "cavasspy-1.1.3.tar", last modified: Thu Apr 20 01:20:17 2023, max compression
```

## Comparing `cavasspy-1.1.2.tar` & `cavasspy-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-03-31 05:47:34.219557 cavasspy-1.1.2/
--rw-r--r--   0 daijian    (501) staff       (20)    35149 2022-01-18 06:32:18.000000 cavasspy-1.1.2/LICENSE
--rw-r--r--   0 daijian    (501) staff       (20)      837 2023-03-31 05:47:34.218676 cavasspy-1.1.2/PKG-INFO
--rw-r--r--   0 daijian    (501) staff       (20)      438 2022-08-03 14:11:17.000000 cavasspy-1.1.2/README.md
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-03-31 05:47:34.211837 cavasspy-1.1.2/cavasspy/
--rw-r--r--   0 daijian    (501) staff       (20)        0 2022-08-03 11:45:14.000000 cavasspy-1.1.2/cavasspy/__init__.py
--rw-r--r--   0 daijian    (501) staff       (20)     6277 2023-03-31 05:46:29.000000 cavasspy-1.1.2/cavasspy/op.py
--rw-r--r--   0 daijian    (501) staff       (20)      552 2022-09-01 11:35:28.000000 cavasspy-1.1.2/cavasspy/window_transform.py
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-03-31 05:47:34.217922 cavasspy-1.1.2/cavasspy.egg-info/
--rw-r--r--   0 daijian    (501) staff       (20)      837 2023-03-31 05:47:33.000000 cavasspy-1.1.2/cavasspy.egg-info/PKG-INFO
--rw-r--r--   0 daijian    (501) staff       (20)      250 2023-03-31 05:47:33.000000 cavasspy-1.1.2/cavasspy.egg-info/SOURCES.txt
--rw-r--r--   0 daijian    (501) staff       (20)        1 2023-03-31 05:47:33.000000 cavasspy-1.1.2/cavasspy.egg-info/dependency_links.txt
--rw-r--r--   0 daijian    (501) staff       (20)       16 2023-03-31 05:47:33.000000 cavasspy-1.1.2/cavasspy.egg-info/requires.txt
--rw-r--r--   0 daijian    (501) staff       (20)        9 2023-03-31 05:47:33.000000 cavasspy-1.1.2/cavasspy.egg-info/top_level.txt
--rw-r--r--   0 daijian    (501) staff       (20)       38 2023-03-31 05:47:34.220250 cavasspy-1.1.2/setup.cfg
--rw-r--r--   0 daijian    (501) staff       (20)      672 2023-03-31 05:44:19.000000 cavasspy-1.1.2/setup.py
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-04-20 01:20:17.504094 cavasspy-1.1.3/
+-rw-r--r--   0 daijian    (501) staff       (20)    35149 2022-01-18 06:32:18.000000 cavasspy-1.1.3/LICENSE
+-rw-r--r--   0 daijian    (501) staff       (20)      837 2023-04-20 01:20:17.503729 cavasspy-1.1.3/PKG-INFO
+-rw-r--r--   0 daijian    (501) staff       (20)      438 2022-08-03 14:11:17.000000 cavasspy-1.1.3/README.md
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-04-20 01:20:17.499260 cavasspy-1.1.3/cavasspy/
+-rw-r--r--   0 daijian    (501) staff       (20)        0 2022-08-03 11:45:14.000000 cavasspy-1.1.3/cavasspy/__init__.py
+-rw-r--r--   0 daijian    (501) staff       (20)      566 2023-04-18 07:47:10.000000 cavasspy-1.1.3/cavasspy/match.py
+-rw-r--r--   0 daijian    (501) staff       (20)     6278 2023-04-18 02:40:03.000000 cavasspy-1.1.3/cavasspy/op.py
+-rw-r--r--   0 daijian    (501) staff       (20)      552 2022-09-01 11:35:28.000000 cavasspy-1.1.3/cavasspy/window_transform.py
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-04-20 01:20:17.503216 cavasspy-1.1.3/cavasspy.egg-info/
+-rw-r--r--   0 daijian    (501) staff       (20)      837 2023-04-20 01:20:16.000000 cavasspy-1.1.3/cavasspy.egg-info/PKG-INFO
+-rw-r--r--   0 daijian    (501) staff       (20)      268 2023-04-20 01:20:17.000000 cavasspy-1.1.3/cavasspy.egg-info/SOURCES.txt
+-rw-r--r--   0 daijian    (501) staff       (20)        1 2023-04-20 01:20:16.000000 cavasspy-1.1.3/cavasspy.egg-info/dependency_links.txt
+-rw-r--r--   0 daijian    (501) staff       (20)       16 2023-04-20 01:20:16.000000 cavasspy-1.1.3/cavasspy.egg-info/requires.txt
+-rw-r--r--   0 daijian    (501) staff       (20)        9 2023-04-20 01:20:16.000000 cavasspy-1.1.3/cavasspy.egg-info/top_level.txt
+-rw-r--r--   0 daijian    (501) staff       (20)       38 2023-04-20 01:20:17.504258 cavasspy-1.1.3/setup.cfg
+-rw-r--r--   0 daijian    (501) staff       (20)      672 2023-04-20 01:19:52.000000 cavasspy-1.1.3/setup.py
```

### Comparing `cavasspy-1.1.2/LICENSE` & `cavasspy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cavasspy-1.1.2/PKG-INFO` & `cavasspy-1.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cavasspy
-Version: 1.1.2
+Version: 1.1.3
 Summary: CAVASS python APIs.
 Author: Dai Jian
 Author-email: daijian@stumail.ysu.edu.cn
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
```

### Comparing `cavasspy-1.1.2/cavasspy/op.py` & `cavasspy-1.1.3/cavasspy/op.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 # CAVASS build path, default in installation is ~/cavass-build
 if os.path.exists(os.path.expanduser('~/cavass-build')):
     CAVASS_PROFILE_PATH = os.path.expanduser('~/cavass-build')
 else:
     CAVASS_PROFILE_PATH = None
 
+
 class CAVASSPyError(Exception):
     ...
 
 
 def env():
     if CAVASS_PROFILE_PATH is not None:
         PATH = f'{os.environ["PATH"]}:{os.path.expanduser(CAVASS_PROFILE_PATH)}'
```

### Comparing `cavasspy-1.1.2/cavasspy/window_transform.py` & `cavasspy-1.1.3/cavasspy/window_transform.py`

 * *Files identical despite different names*

### Comparing `cavasspy-1.1.2/cavasspy.egg-info/PKG-INFO` & `cavasspy-1.1.3/cavasspy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cavasspy
-Version: 1.1.2
+Version: 1.1.3
 Summary: CAVASS python APIs.
 Author: Dai Jian
 Author-email: daijian@stumail.ysu.edu.cn
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
```

### Comparing `cavasspy-1.1.2/setup.py` & `cavasspy-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='cavasspy',
-    version='1.1.2',
+    version='1.1.3',
     author='Dai Jian',
     author_email='daijian@stumail.ysu.edu.cn',
     description='CAVASS python APIs.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
```

