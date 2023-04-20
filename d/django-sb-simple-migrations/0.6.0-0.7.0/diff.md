# Comparing `tmp/django-sb-simple-migrations-0.6.0.tar.gz` & `tmp/django_sb_simple_migrations-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sb-simple-migrations-0.6.0.tar", max compression
+gzip compressed data, was "django_sb_simple_migrations-0.7.0.tar", max compression
```

## Comparing `django-sb-simple-migrations-0.6.0.tar` & `django_sb_simple_migrations-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0      846 2022-05-17 11:12:14.304277 django-sb-simple-migrations-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2021-06-18 19:38:07.567951 django-sb-simple-migrations-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     4102 2022-05-17 11:06:03.328175 django-sb-simple-migrations-0.6.0/README.md
--rw-r--r--   0        0        0       88 2021-07-25 03:05:43.869217 django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/__init__.py
--rw-r--r--   0        0        0        0 2021-06-05 15:40:46.675640 django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/admin.py
--rw-r--r--   0        0        0      229 2021-06-18 19:10:51.882041 django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/apps.py
--rw-r--r--   0        0        0     2228 2021-06-21 08:42:24.109394 django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/conf.py
--rw-r--r--   0        0        0        0 2021-06-05 15:39:06.367275 django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/management/__init__.py
--rw-r--r--   0        0        0        0 2021-06-05 15:39:06.383275 django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/management/commands/__init__.py
--rw-r--r--   0        0        0     1868 2021-06-05 16:33:42.478378 django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/management/commands/makemigrations.py
--rw-r--r--   0        0        0     1117 2021-06-05 16:02:46.026702 django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/management/commands/migrate.py
--rw-r--r--   0        0        0        0 2021-06-05 15:35:18.058243 django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/migrations/__init__.py
--rw-r--r--   0        0        0        0 2021-06-05 15:40:28.551577 django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/models.py
--rw-r--r--   0        0        0        0 2021-06-05 15:40:25.947568 django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/tests.py
--rw-r--r--   0        0        0       20 2022-05-17 11:12:14.308277 django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/version.py
--rw-r--r--   0        0        0        0 2021-06-05 15:40:23.291559 django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/views.py
--rw-r--r--   0        0        0     2185 2022-05-17 11:12:14.304277 django-sb-simple-migrations-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5064 2022-05-17 11:12:17.148059 django-sb-simple-migrations-0.6.0/setup.py
--rw-r--r--   0        0        0     5489 2022-05-17 11:12:17.148469 django-sb-simple-migrations-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-20 05:53:07.857550 django_sb_simple_migrations-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2022-12-12 01:48:28.326594 django_sb_simple_migrations-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     3191 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/README.md
+-rw-r--r--   0        0        0     2225 2023-04-20 05:53:07.853549 django_sb_simple_migrations-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/admin.py
+-rw-r--r--   0        0        0      229 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/apps.py
+-rw-r--r--   0        0        0     2190 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/conf.py
+-rw-r--r--   0        0        0        0 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/management/commands/__init__.py
+-rw-r--r--   0        0        0     1868 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/management/commands/makemigrations.py
+-rw-r--r--   0        0        0     1117 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/management/commands/migrate.py
+-rw-r--r--   0        0        0        0 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/models.py
+-rw-r--r--   0        0        0        0 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/tests.py
+-rw-r--r--   0        0        0       20 2023-04-20 05:53:07.861549 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/version.py
+-rw-r--r--   0        0        0        0 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/views.py
+-rw-r--r--   0        0        0     4762 1970-01-01 00:00:00.000000 django_sb_simple_migrations-0.7.0/PKG-INFO
```

### Comparing `django-sb-simple-migrations-0.6.0/CHANGELOG.md` & `django_sb_simple_migrations-0.7.0/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,23 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.7.0] - 2023-04-20
+
+- Drop support for python 3.8.0
+- Update dependencies
+- Update development tools configuration
+- Update repository structure
+- Update references from Github to GitLab
+- Update `README.md` and `CONTRIBUTING.md`
+
 ## [0.6.0] - 2022-05-17
 
 - Drop support for python 3.6
 - Drop support for python 3.7
 - Add support for python 3.10
 - Add support for Django 4
```

### Comparing `django-sb-simple-migrations-0.6.0/LICENSE.txt` & `django_sb_simple_migrations-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-sb-simple-migrations-0.6.0/README.md` & `django_sb_simple_migrations-0.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,46 @@
-![Community project](https://raw.githubusercontent.com/softbutterfly/django-sb-simple-migrations/master/resources/softbutterfly-open-source-community-project.png)
+Metadata-Version: 2.1
+Name: django-sb-simple-migrations
+Version: 0.7.0
+Summary: Django migrations without unnecesary change alert triggers.
+Home-page: https://gitlab.com/softbutterfly/open-source/django-sb-simple-migrations
+License: MIT
+Keywords: Softbutterfly,Django,Migrations
+Author: SoftButterfly Development Team
+Author-email: dev@softbutterfly.io
+Requires-Python: >=3.8,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: Django (<5.0.0)
+Project-URL: Bug Tracker, https://github.com/softbutterfly/django-sb-simple-migrations/issues
+Project-URL: Documentation, https://gitlab.com/softbutterfly/open-source/django-sb-simple-migrations/-/wikis
+Project-URL: Download, https://github.com/softbutterfly/django-sb-simple-migrations/archive/v0.7.0.tar.gz
+Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/django-sb-simple-migrations
+Description-Content-Type: text/markdown
+
+![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/django-sb-simple-migrations)
 ![PyPI - Package version](https://img.shields.io/pypi/v/django-sb-simple-migrations)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/django-sb-simple-migrations)
 ![PyPI - MIT License](https://img.shields.io/pypi/l/django-sb-simple-migrations)
 
-[![Build Status](https://www.travis-ci.org/softbutterfly/django-sb-simple-migrations.svg?branch=develop)](https://www.travis-ci.org/softbutterfly/django-sb-simple-migrations)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/9ed3b8725e094a648b38b96a3acdc1eb)](https://www.codacy.com/gh/softbutterfly/django-sb-simple-migrations/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=softbutterfly/django-sb-simple-migrations&amp;utm_campaign=Badge_Grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/9ed3b8725e094a648b38b96a3acdc1eb)](https://www.codacy.com/gh/softbutterfly/django-sb-simple-migrations/dashboard?utm_source=github.com&utm_medium=referral&utm_content=softbutterfly/django-sb-simple-migrations&utm_campaign=Badge_Coverage)
-[![codecov](https://codecov.io/gh/softbutterfly/django-sb-simple-migrations/branch/master/graph/badge.svg?token=pbqXUUOu1F)](https://codecov.io/gh/softbutterfly/django-sb-simple-migrations)
-[![Requirements Status](https://requires.io/github/softbutterfly/django-sb-simple-migrations/requirements.svg?branch=master)](https://requires.io/github/softbutterfly/django-sb-simple-migrations/requirements/?branch=master)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/cbdc556a2ca246d2b906dfc5e1195541)](https://app.codacy.com/gl/softbutterfly/django-sb-simple-migrations/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
 # Django Simple Migrations
 
 Django migrations without unnecesary change alert triggers.
 
 This project was originally taken from [Pretix source code](https://github.com/pretix/pretix/tree/master/src/pretix/base/management/commands) and battle testet across many projects on [SoftButterfly](https://softbutterfly.io).
 
@@ -51,21 +78,22 @@
   "django_sb_simple_migrations",
   # ...
 ]
 ```
 
 ## Docs
 
-- [Ejemplos](https://github.com/softbutterfly/django-sb-simple-migrations/wiki)
-- [Wiki](https://github.com/softbutterfly/django-sb-simple-migrations/wiki)
+- [Ejemplos](https://gitlab.com/softbutterfly/open-source/django-sb-simple-migrations/-/wikis)
+- [Wiki](https://gitlab.com/softbutterfly/open-source/django-sb-simple-migrations/-/wikis)
 
 ## Changelog
 
 All changes to versions of this library are listed in the [change history](CHANGELOG.md).
 
 ## Development
 
 Check out our [contribution guide](CONTRIBUTING.md).
 
 ## Contributors
 
-See the list of contributors [here](https://github.com/softbutterfly/django-sb-simple-migrations/graphs/contributors).
+See the list of contributors [here](https://gitlab.com/softbutterfly/open-source/django-sb-simple-migrations/-/graphs/develop).
+
```

### Comparing `django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/conf.py` & `django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,29 +53,27 @@
     }
     required_settings = []
 
     def __init__(self, base_settings):
         self.base_settings = base_settings
 
         for setting in self.required_settings:
-            prefixed_name = "%s_%s" % (self.prefix, setting)
+            prefixed_name = f"{self.prefix}_{setting}"
 
             if not hasattr(self.base_settings, prefixed_name):
                 raise ImproperlyConfigured(
-                    "The '%s' setting is required." % prefixed_name
+                    f"The '{prefixed_name}' setting is required."
                 )
 
     def __getattr__(self, name):
-        prefixed_name = "%s_%s" % (self.prefix, name)
+        prefixed_name = f"{self.prefix}_{name}"
 
         if hasattr(self.base_settings, prefixed_name):
             return getattr(self.base_settings, prefixed_name)
 
         if name in self.defaults:
             return self.defaults[name]
 
-        raise AttributeError(
-            "'AppSettings' object does not have a '%s' attribute" % name
-        )
+        raise AttributeError(f"'AppSettings' object does not have a '{name}' attribute")
 
 
 settings = AppSettings(django_settings)
```

### Comparing `django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/management/commands/makemigrations.py` & `django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/management/commands/makemigrations.py`

 * *Files identical despite different names*

### Comparing `django-sb-simple-migrations-0.6.0/django_sb_simple_migrations/management/commands/migrate.py` & `django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/management/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `django-sb-simple-migrations-0.6.0/pyproject.toml` & `django_sb_simple_migrations-0.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [tool.poetry]
 name = "django-sb-simple-migrations"
-version = "0.6.0"
+version = "0.7.0"
 description = "Django migrations without unnecesary change alert triggers."
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
-homepage = "https://github.com/softbutterfly/django-sb-simple-migrations"
-repository = "https://github.com/softbutterfly/django-sb-simple-migrations"
-documentation = "https://github.com/softbutterfly/django-sb-simple-migrations/wiki"
+homepage = "https://gitlab.com/softbutterfly/open-source/django-sb-simple-migrations"
+repository = "https://gitlab.com/softbutterfly/open-source/django-sb-simple-migrations"
+documentation = "https://gitlab.com/softbutterfly/open-source/django-sb-simple-migrations/-/wikis"
 keywords = ["Softbutterfly", "Django", "Migrations"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
+  "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
-  "Programming Language :: Python :: 3.6",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
-    { include = "django_sb_simple_migrations" }
+    { include = "django_sb_simple_migrations", from = "src" }
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://github.com/softbutterfly/django-sb-simple-migrations/archive/v0.6.0.tar.gz"
+"Download" = "https://github.com/softbutterfly/django-sb-simple-migrations/archive/v0.7.0.tar.gz"
 "Bug Tracker" = "https://github.com/softbutterfly/django-sb-simple-migrations/issues"
 
 
 [tool.poetry.dependencies]
 python = ">= 3.8, < 4.0.0"
 Django = "< 5.0.0"
 
@@ -81,9 +81,9 @@
   |dist
   |legacy
   |example
 )/
 '''
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

