# Comparing `tmp/django-classy-settings-3.0.1.tar.gz` & `tmp/django_classy_settings-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-classy-settings-3.0.1.tar", max compression
+gzip compressed data, was "django_classy_settings-3.0.2.tar", max compression
```

## Comparing `django-classy-settings-3.0.1.tar` & `django_classy_settings-3.0.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1297 2015-06-16 05:39:35.220270 django-classy-settings-3.0.1/LICENSE
--rw-r--r--   0        0        0     1016 2022-09-14 22:32:13.875404 django-classy-settings-3.0.1/README.md
--rw-r--r--   0        0        0     5291 2022-09-14 22:34:11.052838 django-classy-settings-3.0.1/cbs/__init__.py
--rw-r--r--   0        0        0     1100 2022-09-14 22:33:35.589875 django-classy-settings-3.0.1/cbs/cast.py
--rw-r--r--   0        0        0     1729 2022-09-08 12:15:04.645999 django-classy-settings-3.0.1/cbs/urls.py
--rw-r--r--   0        0        0     1292 2022-09-14 22:41:26.937823 django-classy-settings-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     1743 2022-09-14 22:42:15.742594 django-classy-settings-3.0.1/setup.py
--rw-r--r--   0        0        0     2074 2022-09-14 22:42:15.743002 django-classy-settings-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1297 2015-06-16 05:39:35.220270 django_classy_settings-3.0.2/LICENSE
+-rw-r--r--   0        0        0     1016 2022-09-14 22:49:58.676866 django_classy_settings-3.0.2/README.md
+-rw-r--r--   0        0        0     5365 2023-03-27 02:16:25.229451 django_classy_settings-3.0.2/cbs/__init__.py
+-rw-r--r--   0        0        0     1102 2023-03-09 01:09:41.869659 django_classy_settings-3.0.2/cbs/cast.py
+-rw-r--r--   0        0        0     1729 2022-09-08 12:15:04.645999 django_classy_settings-3.0.2/cbs/urls.py
+-rw-r--r--   0        0        0     1292 2023-04-19 23:46:11.250970 django_classy_settings-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 django_classy_settings-3.0.2/PKG-INFO
```

### Comparing `django-classy-settings-3.0.1/LICENSE` & `django_classy_settings-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-classy-settings-3.0.1/README.md` & `django_classy_settings-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-classy-settings-3.0.1/cbs/__init__.py` & `django_classy_settings-3.0.2/cbs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,17 @@
 
         if self.cast and isinstance(value, str):
             value = self.cast(value)
 
         obj.__dict__[self.key] = value
         return value
 
+    def __call__(self):
+        return self.__get__(self)
+
     def __class_getitem__(cls, key):
         """Helper to allow creating env sub-classes with PREFIX pre-set."""
         return type(f"{cls.__name__}__{key}", (cls,), {"PREFIX": key})
 
     @classmethod
     def bool(cls, *args, **kwargs):
         """Helper for bool-cast settings.
@@ -188,15 +191,15 @@
 
         :return: function suitable for module-level ``__dir__``
         """
         from inspect import getmodule
 
         pkg = getmodule(cls)
 
-        keys = [x for x in vars(pkg).keys() if x.isupper()] + [
-            x for x in dir(cls) if x.isupper()
-        ]
-
-        def __dir__(keys=keys):
-            return keys
+        def __dir__(pkg=pkg):
+            return [
+                x for x in vars(pkg).keys() if x.isupper()
+            ] + [
+                x for x in dir(cls) if x.isupper()
+            ]
 
         return __dir__
```

### Comparing `django-classy-settings-3.0.1/cbs/cast.py` & `django_classy_settings-3.0.2/cbs/cast.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,21 @@
     if value in ("n", "no", "off", "f", "false", "0"):
         return False
     raise ValueError("Unrecognised value for bool: %r" % value)
 
 
 def as_list(value: str) -> list:
     """
-    Smart cast value to list by splittng the input on ",".
+    Smart cast value to list by splitting the input on ",".
     """
     if isinstance(value, list):
         return value
     return [x.strip() for x in value.split(",") if x.strip()]
 
 
 def as_tuple(value: str) -> tuple:
     """
-    Smart cast value to tuple by splittng the input on ",".
+    Smart cast value to tuple by splitting the input on ",".
     """
     if isinstance(value, tuple):
         return value
     return tuple(as_list(value))
```

### Comparing `django-classy-settings-3.0.1/cbs/urls.py` & `django_classy_settings-3.0.2/cbs/urls.py`

 * *Files identical despite different names*

### Comparing `django-classy-settings-3.0.1/pyproject.toml` & `django_classy_settings-3.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-classy-settings"
-version = "3.0.1"
+version = "3.0.2"
 description = "Simple class-based settings for Django"
 license = "BSD-2-Clause"
 authors = ["Curtis Maloney <curtis@tinbrain.net>"]
 readme = "README.md"
 homepage = "https://django-classy-settings.readthedocs.io/en/latest/"
 repository = "https://github.com/funkybob/django-classy-settings"
 documentation = "https://django-classy-settings.readthedocs.io/en/latest/"
```

### Comparing `django-classy-settings-3.0.1/PKG-INFO` & `django_classy_settings-3.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: django-classy-settings
-Version: 3.0.1
+Version: 3.0.2
 Summary: Simple class-based settings for Django
 Home-page: https://django-classy-settings.readthedocs.io/en/latest/
 License: BSD-2-Clause
 Author: Curtis Maloney
 Author-email: curtis@tinbrain.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: Django
 Project-URL: Documentation, https://django-classy-settings.readthedocs.io/en/latest/
```

