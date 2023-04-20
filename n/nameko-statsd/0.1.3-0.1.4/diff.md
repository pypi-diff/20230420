# Comparing `tmp/nameko-statsd-0.1.3.tar.gz` & `tmp/nameko-statsd-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nameko-statsd-0.1.3.tar", last modified: Wed Oct  2 16:50:57 2019, max compression
+gzip compressed data, was "/Users/tomviner/dev/cvf/nameko-statsd/dist/tmpyvj6nvqo/nameko-statsd-0.1.4.tar", last modified: Thu Apr 20 14:00:03 2023, max compression
```

## Comparing `nameko-statsd-0.1.3.tar` & `nameko-statsd-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tomviner   (501) staff       (20)        0 2019-10-02 16:50:57.000000 nameko-statsd-0.1.3/
--rw-r--r--   0 tomviner   (501) staff       (20)     1446 2019-10-02 16:50:35.000000 nameko-statsd-0.1.3/CHANGELOG.md
--rw-r--r--   0 tomviner   (501) staff       (20)      140 2019-09-30 10:03:03.000000 nameko-statsd-0.1.3/CONTRIBUTORS.txt
--rw-r--r--   0 tomviner   (501) staff       (20)     1077 2019-09-25 15:08:17.000000 nameko-statsd-0.1.3/LICENSE
--rw-r--r--   0 tomviner   (501) staff       (20)      189 2019-09-25 15:08:17.000000 nameko-statsd-0.1.3/MANIFEST.in
--rw-r--r--   0 tomviner   (501) staff       (20)     1004 2019-10-02 16:50:57.000000 nameko-statsd-0.1.3/PKG-INFO
--rw-r--r--   0 tomviner   (501) staff       (20)     5345 2019-09-25 15:08:17.000000 nameko-statsd-0.1.3/README.rst
-drwxr-xr-x   0 tomviner   (501) staff       (20)        0 2019-10-02 16:50:57.000000 nameko-statsd-0.1.3/nameko_statsd/
--rw-r--r--   0 tomviner   (501) staff       (20)       90 2019-09-25 15:08:17.000000 nameko-statsd-0.1.3/nameko_statsd/__init__.py
--rw-r--r--   0 tomviner   (501) staff       (20)      659 2019-09-25 15:08:17.000000 nameko-statsd-0.1.3/nameko_statsd/bases.py
--rw-r--r--   0 tomviner   (501) staff       (20)     4662 2019-10-02 16:50:35.000000 nameko-statsd-0.1.3/nameko_statsd/statsd_dep.py
-drwxr-xr-x   0 tomviner   (501) staff       (20)        0 2019-10-02 16:50:57.000000 nameko-statsd-0.1.3/nameko_statsd.egg-info/
--rw-r--r--   0 tomviner   (501) staff       (20)     1004 2019-10-02 16:50:55.000000 nameko-statsd-0.1.3/nameko_statsd.egg-info/PKG-INFO
--rw-r--r--   0 tomviner   (501) staff       (20)      476 2019-10-02 16:50:56.000000 nameko-statsd-0.1.3/nameko_statsd.egg-info/SOURCES.txt
--rw-r--r--   0 tomviner   (501) staff       (20)        1 2019-10-02 16:50:55.000000 nameko-statsd-0.1.3/nameko_statsd.egg-info/dependency_links.txt
--rw-r--r--   0 tomviner   (501) staff       (20)      160 2019-10-02 16:50:55.000000 nameko-statsd-0.1.3/nameko_statsd.egg-info/requires.txt
--rw-r--r--   0 tomviner   (501) staff       (20)       14 2019-10-02 16:50:55.000000 nameko-statsd-0.1.3/nameko_statsd.egg-info/top_level.txt
--rw-r--r--   0 tomviner   (501) staff       (20)        1 2019-09-25 15:11:43.000000 nameko-statsd-0.1.3/nameko_statsd.egg-info/zip-safe
-drwxr-xr-x   0 tomviner   (501) staff       (20)        0 2019-10-02 16:50:57.000000 nameko-statsd-0.1.3/requirements/
--rw-r--r--   0 tomviner   (501) staff       (20)       88 2019-09-30 13:17:40.000000 nameko-statsd-0.1.3/requirements/base.txt
--rw-r--r--   0 tomviner   (501) staff       (20)       60 2019-09-30 10:03:03.000000 nameko-statsd-0.1.3/requirements/dev.txt
--rw-r--r--   0 tomviner   (501) staff       (20)       38 2019-10-02 16:50:57.000000 nameko-statsd-0.1.3/setup.cfg
--rw-r--r--   0 tomviner   (501) staff       (20)     1372 2019-10-02 16:50:35.000000 nameko-statsd-0.1.3/setup.py
-drwxr-xr-x   0 tomviner   (501) staff       (20)        0 2019-10-02 16:50:57.000000 nameko-statsd-0.1.3/test/
--rw-r--r--   0 tomviner   (501) staff       (20)      699 2019-09-25 15:08:17.000000 nameko-statsd-0.1.3/test/test_bases.py
--rw-r--r--   0 tomviner   (501) staff       (20)     7089 2019-09-30 10:03:03.000000 nameko-statsd-0.1.3/test/test_lazy_client.py
--rw-r--r--   0 tomviner   (501) staff       (20)     8365 2019-10-02 16:50:35.000000 nameko-statsd-0.1.3/test/test_nameko_statsd.py
+drwxr-xr-x   0 tomviner   (503) staff       (20)        0 2023-04-20 14:00:03.000000 nameko-statsd-0.1.4/
+-rw-r--r--   0 tomviner   (503) staff       (20)      990 2023-04-20 14:00:03.000000 nameko-statsd-0.1.4/PKG-INFO
+-rw-r--r--   0 tomviner   (503) staff       (20)     1077 2022-04-04 22:40:52.000000 nameko-statsd-0.1.4/LICENSE
+drwxr-xr-x   0 tomviner   (503) staff       (20)        0 2023-04-20 14:00:03.000000 nameko-statsd-0.1.4/test/
+-rw-r--r--   0 tomviner   (503) staff       (20)     8365 2023-04-18 16:24:38.000000 nameko-statsd-0.1.4/test/test_nameko_statsd.py
+-rw-r--r--   0 tomviner   (503) staff       (20)      699 2022-04-04 22:40:52.000000 nameko-statsd-0.1.4/test/test_bases.py
+-rw-r--r--   0 tomviner   (503) staff       (20)     7089 2023-04-18 16:24:42.000000 nameko-statsd-0.1.4/test/test_lazy_client.py
+-rw-r--r--   0 tomviner   (503) staff       (20)     1558 2023-04-19 15:27:49.000000 nameko-statsd-0.1.4/CHANGELOG.md
+drwxr-xr-x   0 tomviner   (503) staff       (20)        0 2023-04-20 14:00:03.000000 nameko-statsd-0.1.4/nameko_statsd/
+-rw-r--r--   0 tomviner   (503) staff       (20)       90 2022-04-04 22:40:52.000000 nameko-statsd-0.1.4/nameko_statsd/__init__.py
+-rw-r--r--   0 tomviner   (503) staff       (20)     4662 2022-04-04 22:40:52.000000 nameko-statsd-0.1.4/nameko_statsd/statsd_dep.py
+-rw-r--r--   0 tomviner   (503) staff       (20)      659 2022-04-04 22:40:52.000000 nameko-statsd-0.1.4/nameko_statsd/bases.py
+-rw-r--r--   0 tomviner   (503) staff       (20)      189 2022-04-04 22:40:52.000000 nameko-statsd-0.1.4/MANIFEST.in
+drwxr-xr-x   0 tomviner   (503) staff       (20)        0 2023-04-20 14:00:03.000000 nameko-statsd-0.1.4/requirements/
+-rw-r--r--   0 tomviner   (503) staff       (20)       76 2023-04-19 14:49:59.000000 nameko-statsd-0.1.4/requirements/dev.txt
+-rw-r--r--   0 tomviner   (503) staff       (20)       51 2023-04-18 15:28:48.000000 nameko-statsd-0.1.4/requirements/base.txt
+drwxr-xr-x   0 tomviner   (503) staff       (20)        0 2023-04-20 14:00:03.000000 nameko-statsd-0.1.4/nameko_statsd.egg-info/
+-rw-r--r--   0 tomviner   (503) staff       (20)      990 2023-04-20 14:00:03.000000 nameko-statsd-0.1.4/nameko_statsd.egg-info/PKG-INFO
+-rw-r--r--   0 tomviner   (503) staff       (20)        1 2023-04-18 15:19:57.000000 nameko-statsd-0.1.4/nameko_statsd.egg-info/zip-safe
+-rw-r--r--   0 tomviner   (503) staff       (20)      476 2023-04-20 14:00:03.000000 nameko-statsd-0.1.4/nameko_statsd.egg-info/SOURCES.txt
+-rw-r--r--   0 tomviner   (503) staff       (20)      134 2023-04-20 14:00:03.000000 nameko-statsd-0.1.4/nameko_statsd.egg-info/requires.txt
+-rw-r--r--   0 tomviner   (503) staff       (20)       14 2023-04-20 14:00:03.000000 nameko-statsd-0.1.4/nameko_statsd.egg-info/top_level.txt
+-rw-r--r--   0 tomviner   (503) staff       (20)        1 2023-04-20 14:00:03.000000 nameko-statsd-0.1.4/nameko_statsd.egg-info/dependency_links.txt
+-rw-r--r--   0 tomviner   (503) staff       (20)     1354 2023-04-18 15:42:17.000000 nameko-statsd-0.1.4/setup.py
+-rw-r--r--   0 tomviner   (503) staff       (20)       38 2023-04-20 14:00:03.000000 nameko-statsd-0.1.4/setup.cfg
+-rw-r--r--   0 tomviner   (503) staff       (20)     5354 2023-04-20 13:45:12.000000 nameko-statsd-0.1.4/README.rst
+-rw-r--r--   0 tomviner   (503) staff       (20)      140 2022-04-04 22:40:52.000000 nameko-statsd-0.1.4/CONTRIBUTORS.txt
```

### Comparing `nameko-statsd-0.1.3/CHANGELOG.md` & `nameko-statsd-0.1.4/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 Here you can see the full list of changes between
 nameko-statsd versions, where semantic versioning is used:
 *major.minor.patch*.
 
 Backwards-compatible changes increment the minor version number only.
 
 
+Version 0.1.4
+-------------
+* Drop support for Python < 3.6. Add tests for new Python and Nameko 2.x versions.
+
 Version 0.1.3
 -------------
 * Prevent timer decorator and tests using worker_factory from failing
 
 Version 0.1.2
 -------------
 * Only install enum backport when needed
```

### Comparing `nameko-statsd-0.1.3/LICENSE` & `nameko-statsd-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nameko-statsd-0.1.3/PKG-INFO` & `nameko-statsd-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: nameko-statsd
-Version: 0.1.3
+Version: 0.1.4
 Summary: StatsD dependency for nameko services.
 Home-page: https://github.com/sohonetlabs/nameko-statsd
 Author: Sohonet product team
 Author-email: fabrizio.romano@sohonet.com
 License: MIT License
-Description: StatsD dependency for nameko services.
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
+License-File: LICENSE
+
+StatsD dependency for nameko services.
+
```

### Comparing `nameko-statsd-0.1.3/README.rst` & `nameko-statsd-0.1.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 dependencies to your service as you fancy, and no client will be created
 unless it is actually used.
 
 
 Nameko support
 --------------
 
-The following Nameko versions are supported: ``2.11``, ``2.12``.
+The following Nameko versions are supported: ``2.12``, ``2.13``, ``2.14``
 
 
 Deprecation of the ``ServiceBase`` base class and ``name`` argument
 -------------------------------------------------------------------
 
 In previous versions of ``nameko-statsd``, the ``timer`` decorator could only
 be used if the service class inherited from  ``nameko_statsd.ServiceBase`` or
```

### Comparing `nameko-statsd-0.1.3/nameko_statsd/bases.py` & `nameko-statsd-0.1.4/nameko_statsd/bases.py`

 * *Files identical despite different names*

### Comparing `nameko-statsd-0.1.3/nameko_statsd/statsd_dep.py` & `nameko-statsd-0.1.4/nameko_statsd/statsd_dep.py`

 * *Files identical despite different names*

### Comparing `nameko-statsd-0.1.3/nameko_statsd.egg-info/PKG-INFO` & `nameko-statsd-0.1.4/nameko_statsd.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: nameko-statsd
-Version: 0.1.3
+Version: 0.1.4
 Summary: StatsD dependency for nameko services.
 Home-page: https://github.com/sohonetlabs/nameko-statsd
 Author: Sohonet product team
 Author-email: fabrizio.romano@sohonet.com
 License: MIT License
-Description: StatsD dependency for nameko services.
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
+License-File: LICENSE
+
+StatsD dependency for nameko services.
+
```

### Comparing `nameko-statsd-0.1.3/setup.py` & `nameko-statsd-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 
 
 description = 'StatsD dependency for nameko services.'
 
 
 setup(
     name='nameko-statsd',
-    version='0.1.3',
+    version='0.1.4',
     description=description,
     long_description=description,
     long_description_content_type='text/x-rst',
     author='Sohonet product team',
     author_email='fabrizio.romano@sohonet.com',
     url='https://github.com/sohonetlabs/nameko-statsd',
     packages=['nameko_statsd'],
+    python_requires='>=3.6',
     install_requires=reqs('requirements/base.txt'),
     extras_require={
         'dev': reqs('requirements/dev.txt'),
     },
     zip_safe=True,
     license='MIT License',
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Topic :: Internet",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ]
 )
```

### Comparing `nameko-statsd-0.1.3/test/test_bases.py` & `nameko-statsd-0.1.4/test/test_bases.py`

 * *Files identical despite different names*

### Comparing `nameko-statsd-0.1.3/test/test_lazy_client.py` & `nameko-statsd-0.1.4/test/test_lazy_client.py`

 * *Files identical despite different names*

### Comparing `nameko-statsd-0.1.3/test/test_nameko_statsd.py` & `nameko-statsd-0.1.4/test/test_nameko_statsd.py`

 * *Files identical despite different names*

