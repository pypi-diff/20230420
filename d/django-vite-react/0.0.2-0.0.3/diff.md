# Comparing `tmp/django-vite-react-0.0.2.tar.gz` & `tmp/django-vite-react-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vite-react-0.0.2.tar", last modified: Fri Apr 14 06:37:20 2023, max compression
+gzip compressed data, was "django-vite-react-0.0.3.tar", last modified: Thu Apr 20 09:58:17 2023, max compression
```

## Comparing `django-vite-react-0.0.2.tar` & `django-vite-react-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/
--rw-r--r--   0 chen      (1000) chen      (1000)     1063 2022-05-11 08:46:06.000000 django-vite-react-0.0.2/LICENSE
--rw-r--r--   0 chen      (1000) chen      (1000)      141 2023-04-14 06:09:06.000000 django-vite-react-0.0.2/MANIFEST.in
--rw-r--r--   0 chen      (1000) chen      (1000)     3176 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/PKG-INFO
--rw-r--r--   0 chen      (1000) chen      (1000)     2291 2023-04-14 06:25:21.000000 django-vite-react-0.0.2/README.rst
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/django_vite_react.egg-info/
--rw-r--r--   0 chen      (1000) chen      (1000)     3176 2023-04-14 06:37:20.000000 django-vite-react-0.0.2/django_vite_react.egg-info/PKG-INFO
--rw-r--r--   0 chen      (1000) chen      (1000)      520 2023-04-14 06:37:20.000000 django-vite-react-0.0.2/django_vite_react.egg-info/SOURCES.txt
--rw-r--r--   0 chen      (1000) chen      (1000)        1 2023-04-14 06:37:20.000000 django-vite-react-0.0.2/django_vite_react.egg-info/dependency_links.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       12 2023-04-14 06:37:20.000000 django-vite-react-0.0.2/django_vite_react.egg-info/requires.txt
--rw-r--r--   0 chen      (1000) chen      (1000)        6 2023-04-14 06:37:20.000000 django-vite-react-0.0.2/django_vite_react.egg-info/top_level.txt
--rw-r--r--   0 chen      (1000) chen      (1000)      108 2023-04-14 06:04:51.000000 django-vite-react-0.0.2/pyproject.toml
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/react/
--rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/__init__.py
--rw-r--r--   0 chen      (1000) chen      (1000)       63 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/admin.py
--rw-r--r--   0 chen      (1000) chen      (1000)      142 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/apps.py
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/react/components/
--rw-r--r--   0 chen      (1000) chen      (1000)      280 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/components/app.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)      370 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/generic.py
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/react/migrations/
--rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/migrations/__init__.py
--rw-r--r--   0 chen      (1000) chen      (1000)      442 2022-05-12 03:05:04.000000 django-vite-react-0.0.2/react/mixins.py
--rw-r--r--   0 chen      (1000) chen      (1000)       57 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/models.py
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:37:20.759502 django-vite-react-0.0.2/react/templates/
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/react/templates/react/
--rw-r--r--   0 chen      (1000) chen      (1000)      288 2022-05-12 03:04:03.000000 django-vite-react-0.0.2/react/templates/react/react.html
--rw-r--r--   0 chen      (1000) chen      (1000)      182 2022-05-12 03:04:09.000000 django-vite-react-0.0.2/react/templates/react/react_props.html
--rw-r--r--   0 chen      (1000) chen      (1000)       60 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/tests.py
--rw-r--r--   0 chen      (1000) chen      (1000)       63 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/views.py
--rw-r--r--   0 chen      (1000) chen      (1000)      895 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/setup.cfg
--rw-r--r--   0 chen      (1000) chen      (1000)       38 2023-04-14 06:07:50.000000 django-vite-react-0.0.2/setup.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-20 09:58:17.905575 django-vite-react-0.0.3/
+-rw-r--r--   0 chen      (1000) chen      (1000)     1063 2022-05-11 08:46:06.000000 django-vite-react-0.0.3/LICENSE
+-rw-r--r--   0 chen      (1000) chen      (1000)      180 2023-04-20 09:57:35.000000 django-vite-react-0.0.3/MANIFEST.in
+-rw-r--r--   0 chen      (1000) chen      (1000)     4062 2023-04-20 09:58:17.905575 django-vite-react-0.0.3/PKG-INFO
+-rw-r--r--   0 chen      (1000) chen      (1000)     3177 2023-04-14 06:37:58.000000 django-vite-react-0.0.3/README.rst
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-20 09:58:17.902242 django-vite-react-0.0.3/django_vite_react.egg-info/
+-rw-r--r--   0 chen      (1000) chen      (1000)     4062 2023-04-20 09:58:17.000000 django-vite-react-0.0.3/django_vite_react.egg-info/PKG-INFO
+-rw-r--r--   0 chen      (1000) chen      (1000)      611 2023-04-20 09:58:17.000000 django-vite-react-0.0.3/django_vite_react.egg-info/SOURCES.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)        1 2023-04-20 09:58:17.000000 django-vite-react-0.0.3/django_vite_react.egg-info/dependency_links.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       12 2023-04-20 09:58:17.000000 django-vite-react-0.0.3/django_vite_react.egg-info/requires.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)        6 2023-04-20 09:58:17.000000 django-vite-react-0.0.3/django_vite_react.egg-info/top_level.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)      108 2023-04-14 06:04:51.000000 django-vite-react-0.0.3/pyproject.toml
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-20 09:58:17.902242 django-vite-react-0.0.3/react/
+-rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-11 08:44:48.000000 django-vite-react-0.0.3/react/__init__.py
+-rw-r--r--   0 chen      (1000) chen      (1000)       63 2022-05-11 08:44:48.000000 django-vite-react-0.0.3/react/admin.py
+-rw-r--r--   0 chen      (1000) chen      (1000)      142 2022-05-11 08:44:48.000000 django-vite-react-0.0.3/react/apps.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-20 09:58:17.902242 django-vite-react-0.0.3/react/components/
+-rw-r--r--   0 chen      (1000) chen      (1000)      280 2022-05-11 08:44:48.000000 django-vite-react-0.0.3/react/components/app.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)      370 2022-05-11 08:44:48.000000 django-vite-react-0.0.3/react/generic.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-20 09:58:17.905575 django-vite-react-0.0.3/react/migrations/
+-rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-11 08:44:48.000000 django-vite-react-0.0.3/react/migrations/__init__.py
+-rw-r--r--   0 chen      (1000) chen      (1000)      442 2022-05-12 03:05:04.000000 django-vite-react-0.0.3/react/mixins.py
+-rw-r--r--   0 chen      (1000) chen      (1000)       57 2022-05-11 08:44:48.000000 django-vite-react-0.0.3/react/models.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-20 09:58:17.898908 django-vite-react-0.0.3/react/templates/
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-20 09:58:17.905575 django-vite-react-0.0.3/react/templates/react/
+-rw-r--r--   0 chen      (1000) chen      (1000)      288 2022-05-12 03:04:03.000000 django-vite-react-0.0.3/react/templates/react/react.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      182 2022-05-12 03:04:09.000000 django-vite-react-0.0.3/react/templates/react/react_props.html
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-20 09:58:17.905575 django-vite-react-0.0.3/react/templatetags/
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-20 09:58:17.905575 django-vite-react-0.0.3/react/templatetags/__pycache__/
+-rw-r--r--   0 chen      (1000) chen      (1000)     1824 2023-04-14 06:46:03.000000 django-vite-react-0.0.3/react/templatetags/__pycache__/react_tags.cpython-310.pyc
+-rw-r--r--   0 chen      (1000) chen      (1000)     1643 2023-04-14 06:30:52.000000 django-vite-react-0.0.3/react/templatetags/react_tags.py
+-rw-r--r--   0 chen      (1000) chen      (1000)       60 2022-05-11 08:44:48.000000 django-vite-react-0.0.3/react/tests.py
+-rw-r--r--   0 chen      (1000) chen      (1000)       63 2022-05-11 08:44:48.000000 django-vite-react-0.0.3/react/views.py
+-rw-r--r--   0 chen      (1000) chen      (1000)      895 2023-04-20 09:58:17.905575 django-vite-react-0.0.3/setup.cfg
+-rw-r--r--   0 chen      (1000) chen      (1000)       38 2023-04-14 06:07:50.000000 django-vite-react-0.0.3/setup.py
```

### Comparing `django-vite-react-0.0.2/LICENSE` & `django-vite-react-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-vite-react-0.0.2/django_vite_react.egg-info/SOURCES.txt` & `django-vite-react-0.0.3/django_vite_react.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -16,8 +16,10 @@
 react/mixins.py
 react/models.py
 react/tests.py
 react/views.py
 react/components/app.jsx
 react/migrations/__init__.py
 react/templates/react/react.html
-react/templates/react/react_props.html
+react/templates/react/react_props.html
+react/templatetags/react_tags.py
+react/templatetags/__pycache__/react_tags.cpython-310.pyc
```

### Comparing `django-vite-react-0.0.2/setup.cfg` & `django-vite-react-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-vite-react
-version = 0.0.2
+version = 0.0.3
 description = An easy way to Write React Component with Django.
 long_description = file: README.rst
 url = https://github.com/ChanMo/django-react/
 author = ChanMo
 author_email = chan.mo@outlook.com
 license = MIT
 classifiers =
```

