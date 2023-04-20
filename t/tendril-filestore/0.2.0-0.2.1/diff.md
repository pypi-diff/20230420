# Comparing `tmp/tendril-filestore-0.2.0.tar.gz` & `tmp/tendril-filestore-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-filestore-0.2.0.tar", last modified: Thu Apr 20 18:31:02 2023, max compression
+gzip compressed data, was "tendril-filestore-0.2.1.tar", last modified: Thu Apr 20 19:35:54 2023, max compression
```

## Comparing `tendril-filestore-0.2.0.tar` & `tendril-filestore-0.2.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.612235 tendril-filestore-0.2.0/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2023-04-20 18:31:02.612235 tendril-filestore-0.2.0/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.560236 tendril-filestore-0.2.0/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.572236 tendril-filestore-0.2.0/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.572236 tendril-filestore-0.2.0/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.572236 tendril-filestore-0.2.0/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      943 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.576236 tendril-filestore-0.2.0/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-20 18:31:02.616235 tendril-filestore-0.2.0/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3281 2022-12-15 16:44:04.000000 tendril-filestore-0.2.0/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.536237 tendril-filestore-0.2.0/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.576236 tendril-filestore-0.2.0/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.576236 tendril-filestore-0.2.0/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.2.0/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.580236 tendril-filestore-0.2.0/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.2.0/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5603 2023-04-19 18:02:43.000000 tendril-filestore-0.2.0/src/tendril/apiserver/routers/filestore.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.584236 tendril-filestore-0.2.0/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:36:13.000000 tendril-filestore-0.2.0/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.584236 tendril-filestore-0.2.0/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 21:03:32.000000 tendril-filestore-0.2.0/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      264 2023-03-27 15:39:22.000000 tendril-filestore-0.2.0/src/tendril/authz/scopes/filestore.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.588236 tendril-filestore-0.2.0/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-19 12:09:04.000000 tendril-filestore-0.2.0/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.588236 tendril-filestore-0.2.0/src/tendril/common/filestore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-19 11:58:32.000000 tendril-filestore-0.2.0/src/tendril/common/filestore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1646 2023-04-19 17:38:08.000000 tendril-filestore-0.2.0/src/tendril/common/filestore/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.592236 tendril-filestore-0.2.0/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3744 2023-04-20 12:32:50.000000 tendril-filestore-0.2.0/src/tendril/config/filestore.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3458 2023-04-20 12:32:52.000000 tendril-filestore-0.2.0/src/tendril/config/filestore_core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.600236 tendril-filestore-0.2.0/src/tendril/filestore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 21:59:13.000000 tendril-filestore-0.2.0/src/tendril/filestore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6759 2023-04-19 17:30:32.000000 tendril-filestore-0.2.0/src/tendril/filestore/actual.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1467 2023-04-11 16:08:16.000000 tendril-filestore-0.2.0/src/tendril/filestore/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2977 2023-04-20 15:56:35.000000 tendril-filestore-0.2.0/src/tendril/filestore/buckets.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.604236 tendril-filestore-0.2.0/src/tendril/filestore/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 17:57:19.000000 tendril-filestore-0.2.0/src/tendril/filestore/db/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6250 2023-04-19 17:30:49.000000 tendril-filestore-0.2.0/src/tendril/filestore/db/controller.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1426 2023-04-11 18:49:23.000000 tendril-filestore-0.2.0/src/tendril/filestore/db/model.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1266 2023-04-20 18:21:53.000000 tendril-filestore-0.2.0/src/tendril/filestore/remote.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.608235 tendril-filestore-0.2.0/src/tendril_filestore.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2023-04-20 18:31:01.000000 tendril-filestore-0.2.0/src/tendril_filestore.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1362 2023-04-20 18:31:02.000000 tendril-filestore-0.2.0/src/tendril_filestore.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-20 18:31:01.000000 tendril-filestore-0.2.0/src/tendril_filestore.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      585 2023-04-20 18:31:01.000000 tendril-filestore-0.2.0/src/tendril_filestore.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-20 18:31:01.000000 tendril-filestore-0.2.0/src/tendril_filestore.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.612235 tendril-filestore-0.2.0/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.293819 tendril-filestore-0.2.1/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2023-04-20 19:35:54.297819 tendril-filestore-0.2.1/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.257819 tendril-filestore-0.2.1/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.265819 tendril-filestore-0.2.1/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.265819 tendril-filestore-0.2.1/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.269819 tendril-filestore-0.2.1/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      943 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.269819 tendril-filestore-0.2.1/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-20 19:35:54.297819 tendril-filestore-0.2.1/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3306 2023-04-20 19:33:00.000000 tendril-filestore-0.2.1/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.241819 tendril-filestore-0.2.1/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.269819 tendril-filestore-0.2.1/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.269819 tendril-filestore-0.2.1/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.2.1/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.273819 tendril-filestore-0.2.1/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.2.1/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5603 2023-04-19 18:02:43.000000 tendril-filestore-0.2.1/src/tendril/apiserver/routers/filestore.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.273819 tendril-filestore-0.2.1/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:36:13.000000 tendril-filestore-0.2.1/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.277819 tendril-filestore-0.2.1/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 21:03:32.000000 tendril-filestore-0.2.1/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      264 2023-03-27 15:39:22.000000 tendril-filestore-0.2.1/src/tendril/authz/scopes/filestore.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.277819 tendril-filestore-0.2.1/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-19 12:09:04.000000 tendril-filestore-0.2.1/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.277819 tendril-filestore-0.2.1/src/tendril/common/filestore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-19 11:58:32.000000 tendril-filestore-0.2.1/src/tendril/common/filestore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1646 2023-04-19 17:38:08.000000 tendril-filestore-0.2.1/src/tendril/common/filestore/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.281819 tendril-filestore-0.2.1/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3744 2023-04-20 12:32:50.000000 tendril-filestore-0.2.1/src/tendril/config/filestore.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3458 2023-04-20 12:32:52.000000 tendril-filestore-0.2.1/src/tendril/config/filestore_core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.285819 tendril-filestore-0.2.1/src/tendril/filestore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 21:59:13.000000 tendril-filestore-0.2.1/src/tendril/filestore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6759 2023-04-19 17:30:32.000000 tendril-filestore-0.2.1/src/tendril/filestore/actual.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1467 2023-04-11 16:08:16.000000 tendril-filestore-0.2.1/src/tendril/filestore/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2977 2023-04-20 15:56:35.000000 tendril-filestore-0.2.1/src/tendril/filestore/buckets.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.289819 tendril-filestore-0.2.1/src/tendril/filestore/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 17:57:19.000000 tendril-filestore-0.2.1/src/tendril/filestore/db/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6250 2023-04-19 17:30:49.000000 tendril-filestore-0.2.1/src/tendril/filestore/db/controller.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1426 2023-04-11 18:49:23.000000 tendril-filestore-0.2.1/src/tendril/filestore/db/model.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1252 2023-04-20 18:52:21.000000 tendril-filestore-0.2.1/src/tendril/filestore/remote.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.293819 tendril-filestore-0.2.1/src/tendril_filestore.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2023-04-20 19:35:53.000000 tendril-filestore-0.2.1/src/tendril_filestore.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1362 2023-04-20 19:35:53.000000 tendril-filestore-0.2.1/src/tendril_filestore.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-20 19:35:53.000000 tendril-filestore-0.2.1/src/tendril_filestore.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      603 2023-04-20 19:35:53.000000 tendril-filestore-0.2.1/src/tendril_filestore.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-20 19:35:53.000000 tendril-filestore-0.2.1/src/tendril_filestore.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 19:35:54.293819 tendril-filestore-0.2.1/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-08 18:25:43.000000 tendril-filestore-0.2.1/tox.ini
```

### Comparing `tendril-filestore-0.2.0/.gitignore` & `tendril-filestore-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/.readthedocs.yml` & `tendril-filestore-0.2.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/.travis.yml` & `tendril-filestore-0.2.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/LICENSE` & `tendril-filestore-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/PKG-INFO` & `tendril-filestore-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-filestore
-Version: 0.2.0
+Version: 0.2.1
 Summary: File Storage and Management Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-filestore
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-filestore.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-filestore/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-filestore
```

### Comparing `tendril-filestore-0.2.0/README.rst` & `tendril-filestore-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/docs/Makefile` & `tendril-filestore-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/docs/_static/custom.css` & `tendril-filestore-0.2.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/docs/_static/favicon.ico` & `tendril-filestore-0.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/docs/_static/logo.png` & `tendril-filestore-0.2.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/docs/_static/logo_packed.png` & `tendril-filestore-0.2.1/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/docs/_templates/about.html` & `tendril-filestore-0.2.1/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/docs/conf.py` & `tendril-filestore-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/docs/index.rst` & `tendril-filestore-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/docs/installation.rst` & `tendril-filestore-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/setup.py` & `tendril-filestore-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 core_dependencies = [
     'fs',
     'tendril-artefacts',
     'tendril-auth',
     'tendril-config',
     'tendril-utils-fsutils',
     'tendril-utils-db',
+    'tendril-utils-www',
 ]
 
 install_requires = core_dependencies + ['wheel']
 
 setup_requires = ['setuptools_scm']
 
 doc_requires = setup_requires + ['sphinx', 'sphinx-argparse', 'alabaster']
```

### Comparing `tendril-filestore-0.2.0/src/tendril/apiserver/routers/filestore.py` & `tendril-filestore-0.2.1/src/tendril/apiserver/routers/filestore.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/src/tendril/common/filestore/formats.py` & `tendril-filestore-0.2.1/src/tendril/common/filestore/formats.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/src/tendril/config/__init__.py` & `tendril-filestore-0.2.1/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/src/tendril/config/filestore.py` & `tendril-filestore-0.2.1/src/tendril/config/filestore.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/src/tendril/config/filestore_core.py` & `tendril-filestore-0.2.1/src/tendril/config/filestore_core.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/src/tendril/filestore/actual.py` & `tendril-filestore-0.2.1/src/tendril/filestore/actual.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/src/tendril/filestore/base.py` & `tendril-filestore-0.2.1/src/tendril/filestore/base.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/src/tendril/filestore/buckets.py` & `tendril-filestore-0.2.1/src/tendril/filestore/buckets.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/src/tendril/filestore/db/controller.py` & `tendril-filestore-0.2.1/src/tendril/filestore/db/controller.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/src/tendril/filestore/db/model.py` & `tendril-filestore-0.2.1/src/tendril/filestore/db/model.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/src/tendril/filestore/remote.py` & `tendril-filestore-0.2.1/src/tendril/filestore/remote.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     FILESTORE_REMOTE_AUDIENCE,
     FILESTORE_REMOTE_CLIENT_ID,
     FILESTORE_REMOTE_CLIENT_SECRET
 )
 
 
 async def get_remote_bucket_list(remote_uri):
-    async with async_client(base_url=remote_uri, auth=_authenticator, verify=False) as client:
+    async with async_client(base_url=remote_uri, auth=_authenticator) as client:
         response = await client.get('/v1/filestore/buckets')
         return response.json()["available_buckets"]
 
 
 class FilestoreBucketRemote(FilestoreBucketBase):
     async def upload(self, file, user, overwrite=False):
         pass
```

### Comparing `tendril-filestore-0.2.0/src/tendril_filestore.egg-info/PKG-INFO` & `tendril-filestore-0.2.1/src/tendril_filestore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-filestore
-Version: 0.2.0
+Version: 0.2.1
 Summary: File Storage and Management Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-filestore
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-filestore.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-filestore/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-filestore
```

### Comparing `tendril-filestore-0.2.0/src/tendril_filestore.egg-info/SOURCES.txt` & `tendril-filestore-0.2.1/src/tendril_filestore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/src/tendril_filestore.egg-info/requires.txt` & `tendril-filestore-0.2.1/src/tendril_filestore.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 fs
 tendril-artefacts
 tendril-auth
 tendril-config
 tendril-utils-fsutils
 tendril-utils-db
+tendril-utils-www
 wheel
 
 [build]
 setuptools_scm
 sphinx
 sphinx-argparse
 alabaster
```

### Comparing `tendril-filestore-0.2.0/tests/coveralls.py` & `tendril-filestore-0.2.1/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.2.0/tox.ini` & `tendril-filestore-0.2.1/tox.ini`

 * *Files identical despite different names*

