# Comparing `tmp/datacheck-0.2.1.tar.gz` & `tmp/datacheck-0.3.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datacheck-0.2.1.tar", last modified: Mon Jul 24 03:03:35 2017, max compression
+gzip compressed data, was "datacheck-0.3.0rc0.tar", last modified: Thu Apr 20 19:13:58 2023, max compression
```

## Comparing `datacheck-0.2.1.tar` & `datacheck-0.3.0rc0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-07-24 03:03:35.000000 datacheck-0.2.1/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-07-24 03:03:35.000000 datacheck-0.2.1/datacheck/
--rw-r--r--   0 travis    (1000) travis    (1000)      365 2017-07-24 03:03:14.000000 datacheck-0.2.1/datacheck/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1197 2017-07-24 03:03:14.000000 datacheck-0.2.1/datacheck/compat.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4116 2017-07-24 03:03:14.000000 datacheck-0.2.1/datacheck/core.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2417 2017-07-24 03:03:14.000000 datacheck-0.2.1/datacheck/exceptions.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1022 2017-07-24 03:03:14.000000 datacheck-0.2.1/datacheck/path.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-07-24 03:03:35.000000 datacheck-0.2.1/datacheck.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)      567 2017-07-24 03:03:35.000000 datacheck-0.2.1/datacheck.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      274 2017-07-24 03:03:35.000000 datacheck-0.2.1/datacheck.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-07-24 03:03:35.000000 datacheck-0.2.1/datacheck.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       25 2017-07-24 03:03:35.000000 datacheck-0.2.1/datacheck.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       10 2017-07-24 03:03:35.000000 datacheck-0.2.1/datacheck.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)     1990 2017-07-24 03:03:14.000000 datacheck-0.2.1/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)      567 2017-07-24 03:03:35.000000 datacheck-0.2.1/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)       38 2017-07-24 03:03:35.000000 datacheck-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:13:58.482067 datacheck-0.3.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 19:13:58.482067 datacheck-0.3.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:13:58.482067 datacheck-0.3.0rc0/datacheck/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/datacheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/datacheck/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/datacheck/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/datacheck/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/datacheck/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:13:58.482067 datacheck-0.3.0rc0/datacheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 19:13:58.000000 datacheck-0.3.0rc0/datacheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-20 19:13:58.000000 datacheck-0.3.0rc0/datacheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:13:58.000000 datacheck-0.3.0rc0/datacheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 19:13:58.000000 datacheck-0.3.0rc0/datacheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 19:13:58.000000 datacheck-0.3.0rc0/datacheck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:13:58.482067 datacheck-0.3.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `datacheck-0.2.1/datacheck/compat.py` & `datacheck-0.3.0rc0/datacheck/compat.py`

 * *Files identical despite different names*

### Comparing `datacheck-0.2.1/datacheck/core.py` & `datacheck-0.3.0rc0/datacheck/core.py`

 * *Files identical despite different names*

### Comparing `datacheck-0.2.1/datacheck/exceptions.py` & `datacheck-0.3.0rc0/datacheck/exceptions.py`

 * *Files identical despite different names*

### Comparing `datacheck-0.2.1/datacheck/path.py` & `datacheck-0.3.0rc0/datacheck/path.py`

 * *Files identical despite different names*

### Comparing `datacheck-0.2.1/setup.py` & `datacheck-0.3.0rc0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,40 +32,40 @@
     def initialize_options(self):
         TestCommand.initialize_options(self)
         self.tox_args = '-r'
 
 
 setup(
     name='datacheck',
-    version='0.2.1',
+    version='0.3.0-rc0',
     packages=['datacheck'],
     url='https://github.com/csdev/datacheck',
     license='MIT',
     author='Christopher Sang',
     description='data validation library',
     long_description='data validation library',
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Topic :: Utilities',
     ],
 
     install_requires=[
-        'future >= 0.14.3, < 0.17',
+        'future >= 0.14.3',
     ],
 
     # tox is responsible for setting up the test runner and its dependencies
     # (e.g., code coverage tools) -- see the tox.ini file
     tests_require=[
-        'tox >= 1.9, < 3',
+        'tox >= 4, < 5',
     ],
 
     cmdclass={
         'test': Tox,
         'clean_test': ToxWithRecreate,
     },
 )
```

