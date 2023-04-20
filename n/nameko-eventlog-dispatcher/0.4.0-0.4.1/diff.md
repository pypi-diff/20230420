# Comparing `tmp/nameko-eventlog-dispatcher-0.4.0.tar.gz` & `tmp/nameko-eventlog-dispatcher-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nameko-eventlog-dispatcher-0.4.0.tar", last modified: Fri Mar 15 23:27:07 2019, max compression
+gzip compressed data, was "dist/nameko-eventlog-dispatcher-0.4.1.tar", last modified: Thu Mar 21 14:49:23 2019, max compression
```

## Comparing `nameko-eventlog-dispatcher-0.4.0.tar` & `nameko-eventlog-dispatcher-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 juliotrigo   (501) staff       (20)        0 2019-03-15 23:27:07.000000 nameko-eventlog-dispatcher-0.4.0/
--rw-r--r--   0 juliotrigo   (501) staff       (20)     1158 2019-03-15 17:55:53.000000 nameko-eventlog-dispatcher-0.4.0/CHANGELOG.rst
--rw-r--r--   0 juliotrigo   (501) staff       (20)      140 2019-01-25 13:48:41.000000 nameko-eventlog-dispatcher-0.4.0/CONTRIBUTORS.txt
--rw-r--r--   0 juliotrigo   (501) staff       (20)     1079 2019-02-18 23:36:17.000000 nameko-eventlog-dispatcher-0.4.0/LICENSE
--rw-r--r--   0 juliotrigo   (501) staff       (20)      131 2019-01-25 13:48:41.000000 nameko-eventlog-dispatcher-0.4.0/MANIFEST.in
-drwxr-xr-x   0 juliotrigo   (501) staff       (20)        0 2019-03-15 23:27:07.000000 nameko-eventlog-dispatcher-0.4.0/nameko_eventlog_dispatcher/
--rw-r--r--   0 juliotrigo   (501) staff       (20)       91 2019-01-25 13:48:41.000000 nameko-eventlog-dispatcher-0.4.0/nameko_eventlog_dispatcher/__init__.py
--rw-r--r--   0 juliotrigo   (501) staff       (20)     3310 2019-03-15 15:46:19.000000 nameko-eventlog-dispatcher-0.4.0/nameko_eventlog_dispatcher/eventlog_dispatcher.py
-drwxr-xr-x   0 juliotrigo   (501) staff       (20)        0 2019-03-15 23:27:07.000000 nameko-eventlog-dispatcher-0.4.0/nameko_eventlog_dispatcher.egg-info/
--rw-r--r--   0 juliotrigo   (501) staff       (20)        1 2019-03-15 23:27:06.000000 nameko-eventlog-dispatcher-0.4.0/nameko_eventlog_dispatcher.egg-info/dependency_links.txt
--rw-r--r--   0 juliotrigo   (501) staff       (20)     8151 2019-03-15 23:27:06.000000 nameko-eventlog-dispatcher-0.4.0/nameko_eventlog_dispatcher.egg-info/PKG-INFO
--rw-r--r--   0 juliotrigo   (501) staff       (20)       86 2019-03-15 23:27:06.000000 nameko-eventlog-dispatcher-0.4.0/nameko_eventlog_dispatcher.egg-info/requires.txt
--rw-r--r--   0 juliotrigo   (501) staff       (20)      453 2019-03-15 23:27:06.000000 nameko-eventlog-dispatcher-0.4.0/nameko_eventlog_dispatcher.egg-info/SOURCES.txt
--rw-r--r--   0 juliotrigo   (501) staff       (20)       27 2019-03-15 23:27:06.000000 nameko-eventlog-dispatcher-0.4.0/nameko_eventlog_dispatcher.egg-info/top_level.txt
--rw-r--r--   0 juliotrigo   (501) staff       (20)        1 2019-03-15 23:27:06.000000 nameko-eventlog-dispatcher-0.4.0/nameko_eventlog_dispatcher.egg-info/zip-safe
--rw-r--r--   0 juliotrigo   (501) staff       (20)     8151 2019-03-15 23:27:07.000000 nameko-eventlog-dispatcher-0.4.0/PKG-INFO
--rw-r--r--   0 juliotrigo   (501) staff       (20)     5696 2019-03-15 17:46:00.000000 nameko-eventlog-dispatcher-0.4.0/README.rst
--rw-r--r--   0 juliotrigo   (501) staff       (20)       38 2019-03-15 23:27:07.000000 nameko-eventlog-dispatcher-0.4.0/setup.cfg
--rw-r--r--   0 juliotrigo   (501) staff       (20)     1567 2019-03-15 17:46:00.000000 nameko-eventlog-dispatcher-0.4.0/setup.py
+drwxr-xr-x   0 juliotrigo   (501) staff       (20)        0 2019-03-21 14:49:23.000000 nameko-eventlog-dispatcher-0.4.1/
+-rw-r--r--   0 juliotrigo   (501) staff       (20)     1305 2019-03-21 14:37:11.000000 nameko-eventlog-dispatcher-0.4.1/CHANGELOG.rst
+-rw-r--r--   0 juliotrigo   (501) staff       (20)      140 2019-01-25 13:48:41.000000 nameko-eventlog-dispatcher-0.4.1/CONTRIBUTORS.txt
+-rw-r--r--   0 juliotrigo   (501) staff       (20)     1079 2019-02-18 23:36:17.000000 nameko-eventlog-dispatcher-0.4.1/LICENSE
+-rw-r--r--   0 juliotrigo   (501) staff       (20)      131 2019-01-25 13:48:41.000000 nameko-eventlog-dispatcher-0.4.1/MANIFEST.in
+drwxr-xr-x   0 juliotrigo   (501) staff       (20)        0 2019-03-21 14:49:23.000000 nameko-eventlog-dispatcher-0.4.1/nameko_eventlog_dispatcher/
+-rw-r--r--   0 juliotrigo   (501) staff       (20)       91 2019-01-25 13:48:41.000000 nameko-eventlog-dispatcher-0.4.1/nameko_eventlog_dispatcher/__init__.py
+-rw-r--r--   0 juliotrigo   (501) staff       (20)     3310 2019-03-19 22:58:28.000000 nameko-eventlog-dispatcher-0.4.1/nameko_eventlog_dispatcher/eventlog_dispatcher.py
+drwxr-xr-x   0 juliotrigo   (501) staff       (20)        0 2019-03-21 14:49:23.000000 nameko-eventlog-dispatcher-0.4.1/nameko_eventlog_dispatcher.egg-info/
+-rw-r--r--   0 juliotrigo   (501) staff       (20)        1 2019-03-21 14:49:23.000000 nameko-eventlog-dispatcher-0.4.1/nameko_eventlog_dispatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 juliotrigo   (501) staff       (20)     8363 2019-03-21 14:49:23.000000 nameko-eventlog-dispatcher-0.4.1/nameko_eventlog_dispatcher.egg-info/PKG-INFO
+-rw-r--r--   0 juliotrigo   (501) staff       (20)       80 2019-03-21 14:49:23.000000 nameko-eventlog-dispatcher-0.4.1/nameko_eventlog_dispatcher.egg-info/requires.txt
+-rw-r--r--   0 juliotrigo   (501) staff       (20)      453 2019-03-21 14:49:23.000000 nameko-eventlog-dispatcher-0.4.1/nameko_eventlog_dispatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 juliotrigo   (501) staff       (20)       27 2019-03-21 14:49:23.000000 nameko-eventlog-dispatcher-0.4.1/nameko_eventlog_dispatcher.egg-info/top_level.txt
+-rw-r--r--   0 juliotrigo   (501) staff       (20)        1 2019-03-21 14:49:23.000000 nameko-eventlog-dispatcher-0.4.1/nameko_eventlog_dispatcher.egg-info/zip-safe
+-rw-r--r--   0 juliotrigo   (501) staff       (20)     8363 2019-03-21 14:49:23.000000 nameko-eventlog-dispatcher-0.4.1/PKG-INFO
+-rw-r--r--   0 juliotrigo   (501) staff       (20)     5827 2019-03-21 14:37:11.000000 nameko-eventlog-dispatcher-0.4.1/README.rst
+-rw-r--r--   0 juliotrigo   (501) staff       (20)       38 2019-03-21 14:49:23.000000 nameko-eventlog-dispatcher-0.4.1/setup.cfg
+-rw-r--r--   0 juliotrigo   (501) staff       (20)     1561 2019-03-21 14:37:11.000000 nameko-eventlog-dispatcher-0.4.1/setup.py
```

### Comparing `nameko-eventlog-dispatcher-0.4.0/CHANGELOG.rst` & `nameko-eventlog-dispatcher-0.4.1/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -4,22 +4,31 @@
 Here you can see the full list of changes between
 nameko-eventlog-dispatcher versions, where semantic versioning is used:
 *major.minor.patch*.
 
 Backwards-compatible changes increment the minor version number only.
 
 
+0.4.1
+-----
+
+Released 2019-03-21
+
+* Add Nameko ``2.12`` support (#16)
+* Ensure that Tox can be run cleanly locally (#15)
+
+
 0.4.0
 -----
 
 Released 2019-03-15
 
 * Add support for Python 3.7 (#12)
-* Add support for older Nameko versions: 2.6, 2.7, 2.8, 2.9, 2.10, 2.11
-  (#13, #14)
+* Add support for older Nameko versions: ``2.6``, ``2.7``, ``2.8``,
+  ``2.9``, ``2.10``, ``2.11`` (#13, #14)
 
 
 0.3.0
 -----
 
 Released 2019-01-28
```

### Comparing `nameko-eventlog-dispatcher-0.4.0/LICENSE` & `nameko-eventlog-dispatcher-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nameko-eventlog-dispatcher-0.4.0/nameko_eventlog_dispatcher/eventlog_dispatcher.py` & `nameko-eventlog-dispatcher-0.4.1/nameko_eventlog_dispatcher/eventlog_dispatcher.py`

 * *Files identical despite different names*

### Comparing `nameko-eventlog-dispatcher-0.4.0/nameko_eventlog_dispatcher.egg-info/PKG-INFO` & `nameko-eventlog-dispatcher-0.4.1/nameko_eventlog_dispatcher.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: nameko-eventlog-dispatcher
-Version: 0.4.0
+Version: 0.4.1
 Summary: Nameko dependency provider that dispatches log data using Events (Pub-Sub).
 Home-page: https://github.com/sohonetlabs/nameko-eventlog-dispatcher
 Author: Julio Trigo
 Author-email: julio.trigo@sohonet.com
 License: MIT License
 Description: Nameko eventlog dispatcher
         ==========================
@@ -158,18 +158,20 @@
         
         .. code-block:: shell
         
             $ # Create/activate a virtual environment
             $ pip install tox
             $ tox
         
-        There are other Makefile targets to run tests:
+        There are other Makefile targets to run the tests, but extra
+        dependencies will have to be installed:
         
         .. code-block:: bash
         
+            $ pip install -U --editable ".[dev]"
             $ make test
             $ make coverage
         
         A different RabbitMQ URI can be provided overriding the following
         environment variables: ``RABBIT_CTL_URI`` and ``AMQP_URI``.
         
         Additional ``pytest`` parameters can be also provided using the ``ARGS``
@@ -182,15 +184,16 @@
         
         
         Nameko support
         --------------
         
         The following Nameko_ versions are supported:
         
-        - ``2.x`` series: 2.6, 2.7, 2.8, 2.9, 2.10, 2.11
+        - ``2.x`` series: ``2.6``, ``2.7``, ``2.8``, ``2.9``, ``2.10``, ``2.11``,
+          ``2.12``
         
         
         Changelog
         ---------
         
         Consult the `CHANGELOG <https://github.com/sohonetlabs/nameko-eventlog-dispatcher/blob/master/CHANGELOG.rst>`_
         document for fixes and enhancements of each version.
@@ -213,7 +216,9 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
```

### Comparing `nameko-eventlog-dispatcher-0.4.0/PKG-INFO` & `nameko-eventlog-dispatcher-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: nameko-eventlog-dispatcher
-Version: 0.4.0
+Version: 0.4.1
 Summary: Nameko dependency provider that dispatches log data using Events (Pub-Sub).
 Home-page: https://github.com/sohonetlabs/nameko-eventlog-dispatcher
 Author: Julio Trigo
 Author-email: julio.trigo@sohonet.com
 License: MIT License
 Description: Nameko eventlog dispatcher
         ==========================
@@ -158,18 +158,20 @@
         
         .. code-block:: shell
         
             $ # Create/activate a virtual environment
             $ pip install tox
             $ tox
         
-        There are other Makefile targets to run tests:
+        There are other Makefile targets to run the tests, but extra
+        dependencies will have to be installed:
         
         .. code-block:: bash
         
+            $ pip install -U --editable ".[dev]"
             $ make test
             $ make coverage
         
         A different RabbitMQ URI can be provided overriding the following
         environment variables: ``RABBIT_CTL_URI`` and ``AMQP_URI``.
         
         Additional ``pytest`` parameters can be also provided using the ``ARGS``
@@ -182,15 +184,16 @@
         
         
         Nameko support
         --------------
         
         The following Nameko_ versions are supported:
         
-        - ``2.x`` series: 2.6, 2.7, 2.8, 2.9, 2.10, 2.11
+        - ``2.x`` series: ``2.6``, ``2.7``, ``2.8``, ``2.9``, ``2.10``, ``2.11``,
+          ``2.12``
         
         
         Changelog
         ---------
         
         Consult the `CHANGELOG <https://github.com/sohonetlabs/nameko-eventlog-dispatcher/blob/master/CHANGELOG.rst>`_
         document for fixes and enhancements of each version.
@@ -213,7 +216,9 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
```

### Comparing `nameko-eventlog-dispatcher-0.4.0/README.rst` & `nameko-eventlog-dispatcher-0.4.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -150,18 +150,20 @@
 
 .. code-block:: shell
 
     $ # Create/activate a virtual environment
     $ pip install tox
     $ tox
 
-There are other Makefile targets to run tests:
+There are other Makefile targets to run the tests, but extra
+dependencies will have to be installed:
 
 .. code-block:: bash
 
+    $ pip install -U --editable ".[dev]"
     $ make test
     $ make coverage
 
 A different RabbitMQ URI can be provided overriding the following
 environment variables: ``RABBIT_CTL_URI`` and ``AMQP_URI``.
 
 Additional ``pytest`` parameters can be also provided using the ``ARGS``
@@ -174,15 +176,16 @@
 
 
 Nameko support
 --------------
 
 The following Nameko_ versions are supported:
 
-- ``2.x`` series: 2.6, 2.7, 2.8, 2.9, 2.10, 2.11
+- ``2.x`` series: ``2.6``, ``2.7``, ``2.8``, ``2.9``, ``2.10``, ``2.11``,
+  ``2.12``
 
 
 Changelog
 ---------
 
 Consult the `CHANGELOG <https://github.com/sohonetlabs/nameko-eventlog-dispatcher/blob/master/CHANGELOG.rst>`_
 document for fixes and enhancements of each version.
```

### Comparing `nameko-eventlog-dispatcher-0.4.0/setup.py` & `nameko-eventlog-dispatcher-0.4.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 file_path = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(file_path, 'README.rst'), 'r', 'utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='nameko-eventlog-dispatcher',
-    version='0.4.0',
+    version='0.4.1',
     description=(
         'Nameko dependency provider that dispatches log data using Events '
         '(Pub-Sub).'
     ),
     long_description=readme,
     long_description_content_type='text/x-rst',
     author='Julio Trigo',
     author_email='julio.trigo@sohonet.com',
     url='https://github.com/sohonetlabs/nameko-eventlog-dispatcher',
     packages=find_packages(exclude=['test', 'test.*']),
-    install_requires=['nameko>=2.6,<2.12'],
+    install_requires=['nameko>=2.6'],
     extras_require={
         'dev': [
             'pytest<=4.3.0',
             'flake8',
             'coverage',
             'restructuredtext-lint',
             'Pygments',
```

