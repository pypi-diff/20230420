# Comparing `tmp/django_perm_trans-0.1.0.tar.gz` & `tmp/django_perm_trans-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_perm_trans-0.1.0.tar", max compression
+gzip compressed data, was "django_perm_trans-0.1.1.tar", max compression
```

## Comparing `django_perm_trans-0.1.0.tar` & `django_perm_trans-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2023-04-20 03:14:17.127773 django_perm_trans-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     1435 2023-04-20 03:18:20.674510 django_perm_trans-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-20 02:17:58.536417 django_perm_trans-0.1.0/django_perm_trans/__init__.py
--rw-r--r--   0        0        0       63 2023-04-19 00:54:30.063019 django_perm_trans-0.1.0/django_perm_trans/admin.py
--rw-r--r--   0        0        0      431 2023-04-20 02:28:36.909186 django_perm_trans-0.1.0/django_perm_trans/apps.py
--rw-r--r--   0        0        0      380 2023-04-20 01:35:55.667662 django_perm_trans-0.1.0/django_perm_trans/exceptions.py
--rw-r--r--   0        0        0     1890 2023-04-20 02:27:59.783352 django_perm_trans-0.1.0/django_perm_trans/functions.py
--rw-r--r--   0        0        0        0 2023-04-19 00:54:30.070358 django_perm_trans-0.1.0/django_perm_trans/migrations/__init__.py
--rw-r--r--   0        0        0       57 2023-04-19 00:54:30.067475 django_perm_trans-0.1.0/django_perm_trans/models.py
--rw-r--r--   0        0        0       60 2023-04-19 00:54:30.068818 django_perm_trans-0.1.0/django_perm_trans/tests.py
--rw-r--r--   0        0        0      491 2023-04-19 23:25:16.885924 django_perm_trans-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2067 1970-01-01 00:00:00.000000 django_perm_trans-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-20 03:14:17.127773 django_perm_trans-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     1435 2023-04-20 03:18:20.674510 django_perm_trans-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 02:17:58.536417 django_perm_trans-0.1.1/django_perm_trans/__init__.py
+-rw-r--r--   0        0        0       63 2023-04-19 00:54:30.063019 django_perm_trans-0.1.1/django_perm_trans/admin.py
+-rw-r--r--   0        0        0      431 2023-04-20 02:28:36.909186 django_perm_trans-0.1.1/django_perm_trans/apps.py
+-rw-r--r--   0        0        0      380 2023-04-20 01:35:55.667662 django_perm_trans-0.1.1/django_perm_trans/exceptions.py
+-rw-r--r--   0        0        0     1882 2023-04-20 03:48:31.406510 django_perm_trans-0.1.1/django_perm_trans/functions.py
+-rw-r--r--   0        0        0        0 2023-04-19 00:54:30.070358 django_perm_trans-0.1.1/django_perm_trans/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2023-04-19 00:54:30.067475 django_perm_trans-0.1.1/django_perm_trans/models.py
+-rw-r--r--   0        0        0       60 2023-04-19 00:54:30.068818 django_perm_trans-0.1.1/django_perm_trans/tests.py
+-rw-r--r--   0        0        0      491 2023-04-20 03:51:06.306100 django_perm_trans-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2067 1970-01-01 00:00:00.000000 django_perm_trans-0.1.1/PKG-INFO
```

### Comparing `django_perm_trans-0.1.0/LICENSE.md` & `django_perm_trans-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_perm_trans-0.1.0/README.md` & `django_perm_trans-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_perm_trans-0.1.0/django_perm_trans/functions.py` & `django_perm_trans-0.1.1/django_perm_trans/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 
 def str_override(perm):
     """Override __str__ method of Permission model
     """
     perm_words = []
 
-    if not DPT_REMOVE_APP:
+    if DPT_REMOVE_APP:
         perm_words.append(perm.content_type.app_label)
 
-    if not DPT_REMOVE_MODEL:
+    if DPT_REMOVE_MODEL:
         perm_words.append(perm.content_type.name)
 
     perm_words.append(perm.name)
 
     if DPT_CAPITALIZE_WORDS:
         perm_words = [word.capitalize() for word in perm_words]
```

### Comparing `django_perm_trans-0.1.0/PKG-INFO` & `django_perm_trans-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-perm-trans
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple way to translate the permissions of your Django project.
 License: MIT
 Author: Silas Vasconcelos
 Author-email: silasvasconcelos@hotmail.com.br
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

