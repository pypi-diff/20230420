# Comparing `tmp/django-cookie-monster-0.1.8.tar.gz` & `tmp/django-cookie-monster-0.1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cookie-monster-0.1.8.tar", last modified: Thu Feb  2 12:34:00 2023, max compression
+gzip compressed data, was "django-cookie-monster-0.1.8.1.tar", last modified: Thu Apr 20 19:03:21 2023, max compression
```

## Comparing `django-cookie-monster-0.1.8.tar` & `django-cookie-monster-0.1.8.1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 tanjawyder   (501) staff       (20)        0 2023-02-02 12:34:00.499399 django-cookie-monster-0.1.8/
--rw-r--r--   0 tanjawyder   (501) staff       (20)      152 2023-02-02 09:00:25.000000 django-cookie-monster-0.1.8/AUTHORS.rst
--rw-r--r--   0 tanjawyder   (501) staff       (20)     3339 2023-02-02 09:00:25.000000 django-cookie-monster-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 tanjawyder   (501) staff       (20)      816 2023-02-02 12:28:35.000000 django-cookie-monster-0.1.8/HISTORY.rst
--rw-r--r--   0 tanjawyder   (501) staff       (20)     1509 2023-02-02 09:00:25.000000 django-cookie-monster-0.1.8/LICENSE
--rw-r--r--   0 tanjawyder   (501) staff       (20)      182 2023-02-02 09:00:25.000000 django-cookie-monster-0.1.8/MANIFEST.in
--rw-r--r--   0 tanjawyder   (501) staff       (20)     6440 2023-02-02 12:34:00.499536 django-cookie-monster-0.1.8/PKG-INFO
--rw-r--r--   0 tanjawyder   (501) staff       (20)     4703 2023-02-02 09:00:25.000000 django-cookie-monster-0.1.8/README.md
-drwxr-xr-x   0 tanjawyder   (501) staff       (20)        0 2023-02-02 12:34:00.494480 django-cookie-monster-0.1.8/cookie_monster/
--rw-r--r--   0 tanjawyder   (501) staff       (20)       22 2023-02-02 12:28:35.000000 django-cookie-monster-0.1.8/cookie_monster/__init__.py
--rw-r--r--   0 tanjawyder   (501) staff       (20)      122 2023-02-02 09:00:25.000000 django-cookie-monster-0.1.8/cookie_monster/apps.py
--rw-r--r--   0 tanjawyder   (501) staff       (20)     2370 2023-02-02 12:28:35.000000 django-cookie-monster-0.1.8/cookie_monster/settings.py
-drwxr-xr-x   0 tanjawyder   (501) staff       (20)        0 2023-02-02 12:34:00.489196 django-cookie-monster-0.1.8/cookie_monster/static/
-drwxr-xr-x   0 tanjawyder   (501) staff       (20)        0 2023-02-02 12:34:00.489485 django-cookie-monster-0.1.8/cookie_monster/static/cookie_monster/
-drwxr-xr-x   0 tanjawyder   (501) staff       (20)        0 2023-02-02 12:34:00.494813 django-cookie-monster-0.1.8/cookie_monster/static/cookie_monster/css/
--rw-r--r--   0 tanjawyder   (501) staff       (20)     1920 2023-02-02 09:00:25.000000 django-cookie-monster-0.1.8/cookie_monster/static/cookie_monster/css/minimal.css
-drwxr-xr-x   0 tanjawyder   (501) staff       (20)        0 2023-02-02 12:34:00.495574 django-cookie-monster-0.1.8/cookie_monster/static/cookie_monster/js/
--rw-r--r--   0 tanjawyder   (501) staff       (20)    48527 2023-02-02 09:00:25.000000 django-cookie-monster-0.1.8/cookie_monster/static/cookie_monster/js/cookie-monster.esm.js
--rw-r--r--   0 tanjawyder   (501) staff       (20)    48746 2023-02-02 09:00:25.000000 django-cookie-monster-0.1.8/cookie_monster/static/cookie_monster/js/cookie-monster.umd.js
-drwxr-xr-x   0 tanjawyder   (501) staff       (20)        0 2023-02-02 12:34:00.489787 django-cookie-monster-0.1.8/cookie_monster/templates/
-drwxr-xr-x   0 tanjawyder   (501) staff       (20)        0 2023-02-02 12:34:00.496101 django-cookie-monster-0.1.8/cookie_monster/templates/cookie_monster/
--rw-r--r--   0 tanjawyder   (501) staff       (20)     3413 2023-02-02 09:00:25.000000 django-cookie-monster-0.1.8/cookie_monster/templates/cookie_monster/base.html
-drwxr-xr-x   0 tanjawyder   (501) staff       (20)        0 2023-02-02 12:34:00.496724 django-cookie-monster-0.1.8/cookie_monster/templatetags/
--rw-r--r--   0 tanjawyder   (501) staff       (20)        0 2023-02-02 09:00:25.000000 django-cookie-monster-0.1.8/cookie_monster/templatetags/__init__.py
--rw-r--r--   0 tanjawyder   (501) staff       (20)      634 2023-02-02 09:00:25.000000 django-cookie-monster-0.1.8/cookie_monster/templatetags/cookie_monster.py
--rw-r--r--   0 tanjawyder   (501) staff       (20)      239 2023-02-02 09:00:25.000000 django-cookie-monster-0.1.8/cookie_monster/urls.py
--rw-r--r--   0 tanjawyder   (501) staff       (20)      540 2023-02-02 12:28:35.000000 django-cookie-monster-0.1.8/cookie_monster/utils.py
-drwxr-xr-x   0 tanjawyder   (501) staff       (20)        0 2023-02-02 12:34:00.499086 django-cookie-monster-0.1.8/django_cookie_monster.egg-info/
--rw-r--r--   0 tanjawyder   (501) staff       (20)     6440 2023-02-02 12:34:00.000000 django-cookie-monster-0.1.8/django_cookie_monster.egg-info/PKG-INFO
--rw-r--r--   0 tanjawyder   (501) staff       (20)      750 2023-02-02 12:34:00.000000 django-cookie-monster-0.1.8/django_cookie_monster.egg-info/SOURCES.txt
--rw-r--r--   0 tanjawyder   (501) staff       (20)        1 2023-02-02 12:34:00.000000 django-cookie-monster-0.1.8/django_cookie_monster.egg-info/dependency_links.txt
--rw-r--r--   0 tanjawyder   (501) staff       (20)        1 2023-02-02 09:03:37.000000 django-cookie-monster-0.1.8/django_cookie_monster.egg-info/not-zip-safe
--rw-r--r--   0 tanjawyder   (501) staff       (20)       15 2023-02-02 12:34:00.000000 django-cookie-monster-0.1.8/django_cookie_monster.egg-info/top_level.txt
--rw-r--r--   0 tanjawyder   (501) staff       (20)      329 2023-02-02 12:34:00.500146 django-cookie-monster-0.1.8/setup.cfg
--rwxr-xr-x   0 tanjawyder   (501) staff       (20)     2396 2023-02-02 09:00:25.000000 django-cookie-monster-0.1.8/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.416188 django-cookie-monster-0.1.8.1/
+-rw-r--r--   0 phil       (501) staff       (20)      152 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/AUTHORS.rst
+-rw-r--r--   0 phil       (501) staff       (20)     3339 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/CONTRIBUTING.rst
+-rw-r--r--   0 phil       (501) staff       (20)      903 2023-04-20 19:01:58.000000 django-cookie-monster-0.1.8.1/HISTORY.rst
+-rw-r--r--   0 phil       (501) staff       (20)     1509 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      187 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)     6529 2023-04-20 19:03:21.416287 django-cookie-monster-0.1.8.1/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     4703 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.411466 django-cookie-monster-0.1.8.1/cookie_monster/
+-rw-r--r--   0 phil       (501) staff       (20)       24 2023-04-20 19:01:53.000000 django-cookie-monster-0.1.8.1/cookie_monster/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)      122 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/apps.py
+-rw-r--r--   0 phil       (501) staff       (20)     2370 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/settings.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.405073 django-cookie-monster-0.1.8.1/cookie_monster/static/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.405218 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.411802 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/css/
+-rw-r--r--   0 phil       (501) staff       (20)     1920 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/css/minimal.css
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.414087 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/
+-rw-r--r--   0 phil       (501) staff       (20)    48527 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/cookie-monster.esm.js
+-rw-r--r--   0 phil       (501) staff       (20)   288273 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/cookie-monster.esm.js.map
+-rw-r--r--   0 phil       (501) staff       (20)    48746 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/cookie-monster.umd.js
+-rw-r--r--   0 phil       (501) staff       (20)   288321 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/cookie-monster.umd.js.map
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.405362 django-cookie-monster-0.1.8.1/cookie_monster/templates/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.414941 django-cookie-monster-0.1.8.1/cookie_monster/templates/cookie_monster/
+-rw-r--r--   0 phil       (501) staff       (20)     3413 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/templates/cookie_monster/base.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.415261 django-cookie-monster-0.1.8.1/cookie_monster/templatetags/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/templatetags/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)      634 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/templatetags/cookie_monster.py
+-rw-r--r--   0 phil       (501) staff       (20)      239 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/urls.py
+-rw-r--r--   0 phil       (501) staff       (20)      540 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/cookie_monster/utils.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-20 19:03:21.416043 django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)     6529 2023-04-20 19:03:21.000000 django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      882 2023-04-20 19:03:21.000000 django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-20 19:03:21.000000 django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-20 19:03:21.000000 django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/not-zip-safe
+-rw-r--r--   0 phil       (501) staff       (20)       15 2023-04-20 19:03:21.000000 django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)      329 2023-04-20 19:03:21.416665 django-cookie-monster-0.1.8.1/setup.cfg
+-rwxr-xr-x   0 phil       (501) staff       (20)     2396 2023-04-20 19:00:17.000000 django-cookie-monster-0.1.8.1/setup.py
```

### Comparing `django-cookie-monster-0.1.8/CONTRIBUTING.rst` & `django-cookie-monster-0.1.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8/HISTORY.rst` & `django-cookie-monster-0.1.8.1/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 .. :changelog:
 
 History
 -------
+0.1.8.1 (2023-04-20)
+++++++++++++++++++
+
+* Include *.map files in source distribution
+
 
 0.1.8 (2023-02-02)
 ++++++++++++++++++
 
 * Add Django 4 compatibility
 
 0.1.7 (2022-10-11)
```

### Comparing `django-cookie-monster-0.1.8/LICENSE` & `django-cookie-monster-0.1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8/PKG-INFO` & `django-cookie-monster-0.1.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cookie-monster
-Version: 0.1.8
+Version: 0.1.8.1
 Summary: Your project description goes here
 Home-page: https://github.com/victoriameyer/django-cookie-monster
 Author: dreipol GmbH
 Author-email: dev@dreipol.ch
 License: BSD
 Keywords: django-cookie-monster
 Platform: UNKNOWN
@@ -206,14 +206,19 @@
 
 
 
 
 
 History
 -------
+0.1.8.1 (2023-04-20)
+++++++++++++++++++
+
+* Include *.map files in source distribution
+
 
 0.1.8 (2023-02-02)
 ++++++++++++++++++
 
 * Add Django 4 compatibility
 
 0.1.7 (2022-10-11)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: django-cookie-monster Version: 0.1.8 Summary: Your
-project description goes here Home-page: https://github.com/victoriameyer/
+Metadata-Version: 2.1 Name: django-cookie-monster Version: 0.1.8.1 Summary:
+Your project description goes here Home-page: https://github.com/victoriameyer/
 django-cookie-monster Author: dreipol GmbH Author-email: dev@dreipol.ch
 License: BSD Keywords: django-cookie-monster Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0 Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: BSD License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
@@ -47,18 +47,19 @@
 'Purpose', ], 'groups': [ { 'title': 'Necessary', 'required': True, 'cookies':
 [ { 'id': 'application', 'rows': [ 'Language', 'example.com', 'site language',
 ], }, ], }, { 'title': 'Marketing', 'required': False, 'cookies': [ { 'id':
 'GTM', 'rows': [ 'Google Tag Manager', 'Google.com', 'tracking cookie', ], },
 ], }, ], }, } ``` # Contribute ## Installation To install the frontend you will
 need to run: ```sh npm i ``` ## Building frontend The frontend can be built
 via: ```sh npm run build ``` ## Unit test You can unit test the frontend code
-with: ```sh npm test ``` History ------- 0.1.8 (2023-02-02) ++++++++++++++++++
-* Add Django 4 compatibility 0.1.7 (2022-10-11) ++++++++++++++++++ * Add
-samesite configuration option 0.1.6 (2022-01-31) ++++++++++++++++++ * Simplify
-banner text to prevent fails DEPRECATION WARNING: * The setting variable
-`policy_link` was removed due to errors. Please handle any text/link
-combinations yourself. 0.1.5 (2021-02-15) ++++++++++++++++++ * Add plain html
-support for the groups labels 0.1.4 (2020-05-13) ++++++++++++++++++ * Improve
-backward compatibility of browsers 0.1.3 (2020-05-13) ++++++++++++++++++ * Fix
-translation issue in banner text 0.1.2 (2020-04-09) ++++++++++++++++++ * Bugfix
-0.1.1 (2020-04-08) ++++++++++++++++++ * Bugfix 0.1.0 (2019-10-16)
-++++++++++++++++++ * First release on PyPI.
+with: ```sh npm test ``` History ------- 0.1.8.1 (2023-04-20)
+++++++++++++++++++ * Include *.map files in source distribution 0.1.8 (2023-02-
+02) ++++++++++++++++++ * Add Django 4 compatibility 0.1.7 (2022-10-11)
+++++++++++++++++++ * Add samesite configuration option 0.1.6 (2022-01-31)
+++++++++++++++++++ * Simplify banner text to prevent fails DEPRECATION WARNING:
+* The setting variable `policy_link` was removed due to errors. Please handle
+any text/link combinations yourself. 0.1.5 (2021-02-15) ++++++++++++++++++ *
+Add plain html support for the groups labels 0.1.4 (2020-05-13)
+++++++++++++++++++ * Improve backward compatibility of browsers 0.1.3 (2020-05-
+13) ++++++++++++++++++ * Fix translation issue in banner text 0.1.2 (2020-04-
+09) ++++++++++++++++++ * Bugfix 0.1.1 (2020-04-08) ++++++++++++++++++ * Bugfix
+0.1.0 (2019-10-16) ++++++++++++++++++ * First release on PyPI.
```

### Comparing `django-cookie-monster-0.1.8/README.md` & `django-cookie-monster-0.1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8/cookie_monster/settings.py` & `django-cookie-monster-0.1.8.1/cookie_monster/settings.py`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8/cookie_monster/static/cookie_monster/css/minimal.css` & `django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/css/minimal.css`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8/cookie_monster/static/cookie_monster/js/cookie-monster.esm.js` & `django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/cookie-monster.esm.js`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8/cookie_monster/static/cookie_monster/js/cookie-monster.umd.js` & `django-cookie-monster-0.1.8.1/cookie_monster/static/cookie_monster/js/cookie-monster.umd.js`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8/cookie_monster/templates/cookie_monster/base.html` & `django-cookie-monster-0.1.8.1/cookie_monster/templates/cookie_monster/base.html`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8/cookie_monster/templatetags/cookie_monster.py` & `django-cookie-monster-0.1.8.1/cookie_monster/templatetags/cookie_monster.py`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8/cookie_monster/utils.py` & `django-cookie-monster-0.1.8.1/cookie_monster/utils.py`

 * *Files identical despite different names*

### Comparing `django-cookie-monster-0.1.8/django_cookie_monster.egg-info/PKG-INFO` & `django-cookie-monster-0.1.8.1/django_cookie_monster.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cookie-monster
-Version: 0.1.8
+Version: 0.1.8.1
 Summary: Your project description goes here
 Home-page: https://github.com/victoriameyer/django-cookie-monster
 Author: dreipol GmbH
 Author-email: dev@dreipol.ch
 License: BSD
 Keywords: django-cookie-monster
 Platform: UNKNOWN
@@ -206,14 +206,19 @@
 
 
 
 
 
 History
 -------
+0.1.8.1 (2023-04-20)
+++++++++++++++++++
+
+* Include *.map files in source distribution
+
 
 0.1.8 (2023-02-02)
 ++++++++++++++++++
 
 * Add Django 4 compatibility
 
 0.1.7 (2022-10-11)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: django-cookie-monster Version: 0.1.8 Summary: Your
-project description goes here Home-page: https://github.com/victoriameyer/
+Metadata-Version: 2.1 Name: django-cookie-monster Version: 0.1.8.1 Summary:
+Your project description goes here Home-page: https://github.com/victoriameyer/
 django-cookie-monster Author: dreipol GmbH Author-email: dev@dreipol.ch
 License: BSD Keywords: django-cookie-monster Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0 Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: BSD License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
@@ -47,18 +47,19 @@
 'Purpose', ], 'groups': [ { 'title': 'Necessary', 'required': True, 'cookies':
 [ { 'id': 'application', 'rows': [ 'Language', 'example.com', 'site language',
 ], }, ], }, { 'title': 'Marketing', 'required': False, 'cookies': [ { 'id':
 'GTM', 'rows': [ 'Google Tag Manager', 'Google.com', 'tracking cookie', ], },
 ], }, ], }, } ``` # Contribute ## Installation To install the frontend you will
 need to run: ```sh npm i ``` ## Building frontend The frontend can be built
 via: ```sh npm run build ``` ## Unit test You can unit test the frontend code
-with: ```sh npm test ``` History ------- 0.1.8 (2023-02-02) ++++++++++++++++++
-* Add Django 4 compatibility 0.1.7 (2022-10-11) ++++++++++++++++++ * Add
-samesite configuration option 0.1.6 (2022-01-31) ++++++++++++++++++ * Simplify
-banner text to prevent fails DEPRECATION WARNING: * The setting variable
-`policy_link` was removed due to errors. Please handle any text/link
-combinations yourself. 0.1.5 (2021-02-15) ++++++++++++++++++ * Add plain html
-support for the groups labels 0.1.4 (2020-05-13) ++++++++++++++++++ * Improve
-backward compatibility of browsers 0.1.3 (2020-05-13) ++++++++++++++++++ * Fix
-translation issue in banner text 0.1.2 (2020-04-09) ++++++++++++++++++ * Bugfix
-0.1.1 (2020-04-08) ++++++++++++++++++ * Bugfix 0.1.0 (2019-10-16)
-++++++++++++++++++ * First release on PyPI.
+with: ```sh npm test ``` History ------- 0.1.8.1 (2023-04-20)
+++++++++++++++++++ * Include *.map files in source distribution 0.1.8 (2023-02-
+02) ++++++++++++++++++ * Add Django 4 compatibility 0.1.7 (2022-10-11)
+++++++++++++++++++ * Add samesite configuration option 0.1.6 (2022-01-31)
+++++++++++++++++++ * Simplify banner text to prevent fails DEPRECATION WARNING:
+* The setting variable `policy_link` was removed due to errors. Please handle
+any text/link combinations yourself. 0.1.5 (2021-02-15) ++++++++++++++++++ *
+Add plain html support for the groups labels 0.1.4 (2020-05-13)
+++++++++++++++++++ * Improve backward compatibility of browsers 0.1.3 (2020-05-
+13) ++++++++++++++++++ * Fix translation issue in banner text 0.1.2 (2020-04-
+09) ++++++++++++++++++ * Bugfix 0.1.1 (2020-04-08) ++++++++++++++++++ * Bugfix
+0.1.0 (2019-10-16) ++++++++++++++++++ * First release on PyPI.
```

### Comparing `django-cookie-monster-0.1.8/setup.py` & `django-cookie-monster-0.1.8.1/setup.py`

 * *Files identical despite different names*

