# Comparing `tmp/Flask-Meter-1.0.1.tar.gz` & `tmp/Flask-Meter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Meter-1.0.1.tar", last modified: Mon Apr 10 14:29:54 2023, max compression
+gzip compressed data, was "Flask-Meter-1.0.2.tar", last modified: Thu Apr 20 16:37:49 2023, max compression
```

## Comparing `Flask-Meter-1.0.1.tar` & `Flask-Meter-1.0.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/
--rw-rw-r--   0 herman    (1000) herman    (1000)      156 2023-04-10 07:49:10.000000 Flask-Meter-1.0.1/AUTHORS.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     3267 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/CONTRIBUTING.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      372 2023-04-10 14:27:15.000000 Flask-Meter-1.0.1/HISTORY.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     1077 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/LICENSE
--rw-rw-r--   0 herman    (1000) herman    (1000)      264 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/MANIFEST.in
--rw-rw-r--   0 herman    (1000) herman    (1000)     3514 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/PKG-INFO
--rw-rw-r--   0 herman    (1000) herman    (1000)     2085 2023-04-10 14:24:39.000000 Flask-Meter-1.0.1/README.rst
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/docs/
--rw-rw-r--   0 herman    (1000) herman    (1000)     6782 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/docs/Makefile
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.980450 Flask-Meter-1.0.1/docs/_build/
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.980450 Flask-Meter-1.0.1/docs/_build/html/
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/docs/_build/html/_static/
--rw-rw-r--   0 herman    (1000) herman    (1000)      286 2023-04-10 12:45:48.000000 Flask-Meter-1.0.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-04-10 12:45:48.000000 Flask-Meter-1.0.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-04-10 12:45:48.000000 Flask-Meter-1.0.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 herman    (1000) herman    (1000)       28 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/docs/authors.rst
--rwxrwxr-x   0 herman    (1000) herman    (1000)     8585 2023-04-10 13:26:44.000000 Flask-Meter-1.0.1/docs/conf.py
--rw-rw-r--   0 herman    (1000) herman    (1000)       33 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/docs/contributing.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      479 2023-04-10 14:06:54.000000 Flask-Meter-1.0.1/docs/flask_meter.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)       28 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/docs/history.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      298 2023-04-10 11:47:36.000000 Flask-Meter-1.0.1/docs/index.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     1147 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/docs/installation.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     6469 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/docs/make.bat
--rw-rw-r--   0 herman    (1000) herman    (1000)       70 2023-04-10 14:06:54.000000 Flask-Meter-1.0.1/docs/modules.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)       27 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/docs/readme.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      420 2023-04-10 11:51:37.000000 Flask-Meter-1.0.1/docs/usage.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     1724 2023-04-10 14:06:24.000000 Flask-Meter-1.0.1/pyproject.toml
--rw-rw-r--   0 herman    (1000) herman    (1000)       69 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/setup.cfg
--rw-rw-r--   0 herman    (1000) herman    (1000)       38 2023-04-10 08:04:42.000000 Flask-Meter-1.0.1/setup.py
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.980450 Flask-Meter-1.0.1/src/
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/src/Flask_Meter.egg-info/
--rw-rw-r--   0 herman    (1000) herman    (1000)     3514 2023-04-10 14:29:54.000000 Flask-Meter-1.0.1/src/Flask_Meter.egg-info/PKG-INFO
--rw-rw-r--   0 herman    (1000) herman    (1000)      713 2023-04-10 14:29:54.000000 Flask-Meter-1.0.1/src/Flask_Meter.egg-info/SOURCES.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)        1 2023-04-10 14:29:54.000000 Flask-Meter-1.0.1/src/Flask_Meter.egg-info/dependency_links.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-04-10 14:29:54.000000 Flask-Meter-1.0.1/src/Flask_Meter.egg-info/requires.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-04-10 14:29:54.000000 Flask-Meter-1.0.1/src/Flask_Meter.egg-info/top_level.txt
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/src/flask_meter/
--rw-rw-r--   0 herman    (1000) herman    (1000)      109 2023-04-10 14:26:51.000000 Flask-Meter-1.0.1/src/flask_meter/__init__.py
--rw-rw-r--   0 herman    (1000) herman    (1000)     1446 2023-04-10 13:09:59.000000 Flask-Meter-1.0.1/src/flask_meter/flask_meter.py
--rw-rw-r--   0 herman    (1000) herman    (1000)      742 2023-04-10 07:53:30.000000 Flask-Meter-1.0.1/src/flask_meter/git.py
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/tests/
--rw-rw-r--   0 herman    (1000) herman    (1000)     2191 2023-04-10 13:12:53.000000 Flask-Meter-1.0.1/tests/test_flask_meter.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.056286 Flask-Meter-1.0.2/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      156 2023-04-10 07:49:10.000000 Flask-Meter-1.0.2/AUTHORS.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     3267 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/CONTRIBUTING.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      489 2023-04-20 15:36:44.000000 Flask-Meter-1.0.2/HISTORY.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1077 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/LICENSE
+-rw-rw-r--   0 herman    (1000) herman    (1000)      264 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/MANIFEST.in
+-rw-rw-r--   0 herman    (1000) herman    (1000)     3823 2023-04-20 16:37:49.056286 Flask-Meter-1.0.2/PKG-INFO
+-rw-rw-r--   0 herman    (1000) herman    (1000)     2394 2023-04-20 07:43:19.000000 Flask-Meter-1.0.2/README.rst
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.048286 Flask-Meter-1.0.2/docs/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     6782 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/docs/Makefile
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.032286 Flask-Meter-1.0.2/docs/_build/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.032286 Flask-Meter-1.0.2/docs/_build/html/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.052286 Flask-Meter-1.0.2/docs/_build/html/_static/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      286 2023-04-10 12:45:48.000000 Flask-Meter-1.0.2/docs/_build/html/_static/file.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-04-10 12:45:48.000000 Flask-Meter-1.0.2/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-04-10 12:45:48.000000 Flask-Meter-1.0.2/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       28 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/docs/authors.rst
+-rwxrwxr-x   0 herman    (1000) herman    (1000)     8585 2023-04-10 13:26:44.000000 Flask-Meter-1.0.2/docs/conf.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)       33 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/docs/contributing.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      479 2023-04-20 15:37:13.000000 Flask-Meter-1.0.2/docs/flask_meter.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)       28 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/docs/history.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      298 2023-04-10 11:47:36.000000 Flask-Meter-1.0.2/docs/index.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1147 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/docs/installation.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     6469 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/docs/make.bat
+-rw-rw-r--   0 herman    (1000) herman    (1000)       70 2023-04-20 15:37:13.000000 Flask-Meter-1.0.2/docs/modules.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)       27 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/docs/readme.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      420 2023-04-10 11:51:37.000000 Flask-Meter-1.0.2/docs/usage.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1724 2023-04-10 14:06:24.000000 Flask-Meter-1.0.2/pyproject.toml
+-rw-rw-r--   0 herman    (1000) herman    (1000)       69 2023-04-20 16:37:49.060286 Flask-Meter-1.0.2/setup.cfg
+-rw-rw-r--   0 herman    (1000) herman    (1000)       38 2023-04-10 08:04:42.000000 Flask-Meter-1.0.2/setup.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.036286 Flask-Meter-1.0.2/src/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.056286 Flask-Meter-1.0.2/src/Flask_Meter.egg-info/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     3823 2023-04-20 16:37:48.000000 Flask-Meter-1.0.2/src/Flask_Meter.egg-info/PKG-INFO
+-rw-rw-r--   0 herman    (1000) herman    (1000)      731 2023-04-20 16:37:49.000000 Flask-Meter-1.0.2/src/Flask_Meter.egg-info/SOURCES.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)        1 2023-04-20 16:37:48.000000 Flask-Meter-1.0.2/src/Flask_Meter.egg-info/dependency_links.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-04-20 16:37:48.000000 Flask-Meter-1.0.2/src/Flask_Meter.egg-info/requires.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-04-20 16:37:48.000000 Flask-Meter-1.0.2/src/Flask_Meter.egg-info/top_level.txt
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.056286 Flask-Meter-1.0.2/src/flask_meter/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      109 2023-04-20 15:35:50.000000 Flask-Meter-1.0.2/src/flask_meter/__init__.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)     2227 2023-04-20 15:34:23.000000 Flask-Meter-1.0.2/src/flask_meter/flask_meter.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1179 2023-04-20 15:34:42.000000 Flask-Meter-1.0.2/src/flask_meter/git.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.056286 Flask-Meter-1.0.2/tests/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     2608 2023-04-20 15:34:23.000000 Flask-Meter-1.0.2/tests/test_flask_meter.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)      449 2023-04-20 15:34:05.000000 Flask-Meter-1.0.2/tests/test_git.py
```

### Comparing `Flask-Meter-1.0.1/CONTRIBUTING.rst` & `Flask-Meter-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.1/LICENSE` & `Flask-Meter-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.1/PKG-INFO` & `Flask-Meter-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Meter
-Version: 1.0.1
+Version: 1.0.2
 Summary: Flask-Meter adds a healthcheck endpoint for Flask apps.
 Author-email: Herman Singh <kartstig@gmail.com>
 Maintainer-email: Herman Singh <kartstig@gmail.com>
 License: MIT License
 Project-URL: Donate, https://github.com/sponsors/Kartstig/dashboard
 Project-URL: Documentation, https://flask.palletsprojects.com/
 Project-URL: Source Code, https://github.com/Kartstig/flask-meter
@@ -29,45 +29,53 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===============================
 Flask-Meter
 ===============================
-Healthchecks for Flask
+
+        Healthchecks for Flask_ Apps
+
+.. _Flask: https://github.com/pallets/flask/
 
 .. image:: https://img.shields.io/pypi/v/Flask-Meter.svg
         :target: https://pypi.python.org/pypi/Flask-Meter
 
 .. image:: https://tc.spin-flip.com/app/rest/builds/buildType:id:FlaskMeter_TestPython310/statusIcon.svg
         :target: https://tc.spin-flip.com/project/FlaskMeter?mode=trends
 
 .. image:: https://readthedocs.org/projects/flask-meter/badge/?version=latest
         :target: https://flask-meter.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. image:: https://codecov.io/gh/Kartstig/flask-meter/branch/master/graph/badge.svg?token=NsmixA2iCH
         :target: https://codecov.io/gh/Kartstig/flask-meter
 
+.. image:: https://img.shields.io/pypi/dm/Flask-Meter
+        :alt: PyPI - Downloads
+
 Flask-Meter is an add-on to the Flask web framework. Flask-Meter adds a
 monitoring endpoint for consuming application metrics. It can be really simple
 to set up. Flask-Meter modifies the Flask application to provide an enpoint
 at `/_health` where you will get a JSON response of the system's uptime,
 current git revision.
 
 You can also add in extra checks by passing in a list of checks to the
 constructor.
 
 Installing
 ----------
 
-Install and update using `pip`:
+Install and update using `pip`\:
+
 .. code-block:: text
 
-    pip install -U Flask-Meter
+        pip install -U Flask-Meter
+
 
 Flask Configuration
 -------------------
 
 .. code-block:: python
 
   from Flask import Flask
@@ -95,14 +103,24 @@
 
 Features
 --------
 
 * Current Git Commit
 * Accepts custom functions
 
+
+Sponsorship
+-----------
+
+Put your logo here! `Become a sponsor`_ and support this project!
+
+.. _Become a sponsor: https://github.com/sponsors/Kartstig
+
+
+
 Credits
 ---------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `Flask-Meter-1.0.1/README.rst` & `Flask-Meter-1.0.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 ===============================
 Flask-Meter
 ===============================
-Healthchecks for Flask
+
+        Healthchecks for Flask_ Apps
+
+.. _Flask: https://github.com/pallets/flask/
 
 .. image:: https://img.shields.io/pypi/v/Flask-Meter.svg
         :target: https://pypi.python.org/pypi/Flask-Meter
 
 .. image:: https://tc.spin-flip.com/app/rest/builds/buildType:id:FlaskMeter_TestPython310/statusIcon.svg
         :target: https://tc.spin-flip.com/project/FlaskMeter?mode=trends
 
 .. image:: https://readthedocs.org/projects/flask-meter/badge/?version=latest
         :target: https://flask-meter.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. image:: https://codecov.io/gh/Kartstig/flask-meter/branch/master/graph/badge.svg?token=NsmixA2iCH
         :target: https://codecov.io/gh/Kartstig/flask-meter
 
+.. image:: https://img.shields.io/pypi/dm/Flask-Meter
+        :alt: PyPI - Downloads
+
 Flask-Meter is an add-on to the Flask web framework. Flask-Meter adds a
 monitoring endpoint for consuming application metrics. It can be really simple
 to set up. Flask-Meter modifies the Flask application to provide an enpoint
 at `/_health` where you will get a JSON response of the system's uptime,
 current git revision.
 
 You can also add in extra checks by passing in a list of checks to the
 constructor.
 
 Installing
 ----------
 
-Install and update using `pip`:
+Install and update using `pip`\:
+
 .. code-block:: text
 
-    pip install -U Flask-Meter
+        pip install -U Flask-Meter
+
 
 Flask Configuration
 -------------------
 
 .. code-block:: python
 
   from Flask import Flask
@@ -63,14 +71,24 @@
 
 Features
 --------
 
 * Current Git Commit
 * Accepts custom functions
 
+
+Sponsorship
+-----------
+
+Put your logo here! `Become a sponsor`_ and support this project!
+
+.. _Become a sponsor: https://github.com/sponsors/Kartstig
+
+
+
 Credits
 ---------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `Flask-Meter-1.0.1/docs/Makefile` & `Flask-Meter-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.1/docs/conf.py` & `Flask-Meter-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.1/docs/installation.rst` & `Flask-Meter-1.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.1/docs/make.bat` & `Flask-Meter-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.1/pyproject.toml` & `Flask-Meter-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.1/src/Flask_Meter.egg-info/PKG-INFO` & `Flask-Meter-1.0.2/src/Flask_Meter.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Meter
-Version: 1.0.1
+Version: 1.0.2
 Summary: Flask-Meter adds a healthcheck endpoint for Flask apps.
 Author-email: Herman Singh <kartstig@gmail.com>
 Maintainer-email: Herman Singh <kartstig@gmail.com>
 License: MIT License
 Project-URL: Donate, https://github.com/sponsors/Kartstig/dashboard
 Project-URL: Documentation, https://flask.palletsprojects.com/
 Project-URL: Source Code, https://github.com/Kartstig/flask-meter
@@ -29,45 +29,53 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===============================
 Flask-Meter
 ===============================
-Healthchecks for Flask
+
+        Healthchecks for Flask_ Apps
+
+.. _Flask: https://github.com/pallets/flask/
 
 .. image:: https://img.shields.io/pypi/v/Flask-Meter.svg
         :target: https://pypi.python.org/pypi/Flask-Meter
 
 .. image:: https://tc.spin-flip.com/app/rest/builds/buildType:id:FlaskMeter_TestPython310/statusIcon.svg
         :target: https://tc.spin-flip.com/project/FlaskMeter?mode=trends
 
 .. image:: https://readthedocs.org/projects/flask-meter/badge/?version=latest
         :target: https://flask-meter.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. image:: https://codecov.io/gh/Kartstig/flask-meter/branch/master/graph/badge.svg?token=NsmixA2iCH
         :target: https://codecov.io/gh/Kartstig/flask-meter
 
+.. image:: https://img.shields.io/pypi/dm/Flask-Meter
+        :alt: PyPI - Downloads
+
 Flask-Meter is an add-on to the Flask web framework. Flask-Meter adds a
 monitoring endpoint for consuming application metrics. It can be really simple
 to set up. Flask-Meter modifies the Flask application to provide an enpoint
 at `/_health` where you will get a JSON response of the system's uptime,
 current git revision.
 
 You can also add in extra checks by passing in a list of checks to the
 constructor.
 
 Installing
 ----------
 
-Install and update using `pip`:
+Install and update using `pip`\:
+
 .. code-block:: text
 
-    pip install -U Flask-Meter
+        pip install -U Flask-Meter
+
 
 Flask Configuration
 -------------------
 
 .. code-block:: python
 
   from Flask import Flask
@@ -95,14 +103,24 @@
 
 Features
 --------
 
 * Current Git Commit
 * Accepts custom functions
 
+
+Sponsorship
+-----------
+
+Put your logo here! `Become a sponsor`_ and support this project!
+
+.. _Become a sponsor: https://github.com/sponsors/Kartstig
+
+
+
 Credits
 ---------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `Flask-Meter-1.0.1/src/Flask_Meter.egg-info/SOURCES.txt` & `Flask-Meter-1.0.2/src/Flask_Meter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,8 +26,9 @@
 src/Flask_Meter.egg-info/SOURCES.txt
 src/Flask_Meter.egg-info/dependency_links.txt
 src/Flask_Meter.egg-info/requires.txt
 src/Flask_Meter.egg-info/top_level.txt
 src/flask_meter/__init__.py
 src/flask_meter/flask_meter.py
 src/flask_meter/git.py
-tests/test_flask_meter.py
+tests/test_flask_meter.py
+tests/test_git.py
```

### Comparing `Flask-Meter-1.0.1/src/flask_meter/git.py` & `Flask-Meter-1.0.2/src/flask_meter/git.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,39 @@
 import re
 import subprocess
+from typing import Union
+
+try:
+    from typing import Literal, TypedDict
+except ImportError:
+    from typing_extensions import Literal, TypedDict  # Python 3.7 support
+
+
+class GitReturn(TypedDict):
+    commit: Union[str, Literal["Unknown"]]
+    author: Union[str, Literal["Unknown"]]
+    date: Union[str, Literal["Unknown"]]
 
 
 GIT_CMD = "git log | head -4"
 RE_COMMIT = re.compile(r"commit[\W]+(\w+)", re.MULTILINE)
 RE_AUTHOR = re.compile(r"Author\:[\W]+(.*)", re.MULTILINE)
 RE_DATE = re.compile(r"Date\:[\W]+(.*)", re.MULTILINE)
 
 
-def git_stats():
+def git_stats() -> GitReturn:
     try:
         ret = subprocess.check_output([GIT_CMD], shell=True).decode("utf-8")
         commit = re.search(RE_COMMIT, ret)
         author = re.search(RE_AUTHOR, ret)
         date = re.search(RE_DATE, ret)
         return {
             "commit": commit.group(1) if commit else "Unknown",
             "author": author.group(1) if author else "Unknown",
             "date": date.group(1) if date else "Unknown",
         }
     except subprocess.CalledProcessError:
-        return {"Error"}
+        return {
+            "commit": "Unknown",
+            "author": "Unknown",
+            "date": "Unknown",
+        }
```

### Comparing `Flask-Meter-1.0.1/tests/test_flask_meter.py` & `Flask-Meter-1.0.2/tests/test_flask_meter.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,21 +72,37 @@
     fm.init_app(flask_app)
     client = fm.app.test_client()
     rv = client.get("/_health")
 
     assert rv.status_code == 404
 
 
-def test_extra(flask_app):
+def test_extra_ok(flask_app):
     def fake_function():
         """TestingFunc"""
         return True
 
     fm = FlaskMeter()
     fm.init_app(flask_app, extra_checks=[fake_function])
 
     client = fm.app.test_client()
     rv = client.get("/_health")
 
     assert rv.status_code == 200
     data = json.loads(rv.data.decode("utf-8"))
     assert data["TestingFunc"] == "OK"
+
+
+def test_extra_exception(flask_app):
+    def fake_function():
+        """FailFunc"""
+        raise Exception("This function raised an exception")
+
+    fm = FlaskMeter()
+    fm.init_app(flask_app, extra_checks=[fake_function])
+
+    client = fm.app.test_client()
+    rv = client.get("/_health")
+
+    assert rv.status_code == 200
+    data = json.loads(rv.data.decode("utf-8"))
+    assert data["FailFunc"] == "DOWN"
```

