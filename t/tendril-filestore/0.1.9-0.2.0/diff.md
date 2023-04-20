# Comparing `tmp/tendril-filestore-0.1.9.tar.gz` & `tmp/tendril-filestore-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-filestore-0.1.9.tar", last modified: Wed Dec 14 20:31:12 2022, max compression
+gzip compressed data, was "tendril-filestore-0.2.0.tar", last modified: Thu Apr 20 18:31:02 2023, max compression
```

## Comparing `tendril-filestore-0.1.9.tar` & `tendril-filestore-0.2.0.tar`

### file list

```diff
@@ -1,65 +1,70 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.217102 tendril-filestore-0.1.9/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3983 2022-12-14 20:31:12.217102 tendril-filestore-0.1.9/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.205102 tendril-filestore-0.1.9/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.209102 tendril-filestore-0.1.9/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.209102 tendril-filestore-0.1.9/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-07 18:38:54.000000 tendril-filestore-0.1.9/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.209102 tendril-filestore-0.1.9/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      943 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.213102 tendril-filestore-0.1.9/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2022-12-14 20:31:12.217102 tendril-filestore-0.1.9/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3281 2022-12-11 14:50:39.000000 tendril-filestore-0.1.9/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.201102 tendril-filestore-0.1.9/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.213102 tendril-filestore-0.1.9/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.213102 tendril-filestore-0.1.9/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-25 03:24:33.000000 tendril-filestore-0.1.9/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.213102 tendril-filestore-0.1.9/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-07 14:54:45.000000 tendril-filestore-0.1.9/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6908 2022-12-14 20:17:30.000000 tendril-filestore-0.1.9/src/tendril/apiserver/routers/filestore.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.213102 tendril-filestore-0.1.9/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-10 07:41:07.000000 tendril-filestore-0.1.9/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.213102 tendril-filestore-0.1.9/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      212 2022-12-10 07:41:07.000000 tendril-filestore-0.1.9/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      157 2022-12-10 07:41:07.000000 tendril-filestore-0.1.9/src/tendril/authz/scopes/filestore.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.213102 tendril-filestore-0.1.9/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-03-20 07:52:05.000000 tendril-filestore-0.1.9/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3304 2022-12-11 09:56:27.000000 tendril-filestore-0.1.9/src/tendril/config/filestore.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2578 2022-12-11 09:56:27.000000 tendril-filestore-0.1.9/src/tendril/config/filestore_core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.217102 tendril-filestore-0.1.9/src/tendril/filestore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 07:18:42.000000 tendril-filestore-0.1.9/src/tendril/filestore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5998 2022-12-14 18:06:40.000000 tendril-filestore-0.1.9/src/tendril/filestore/actual.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1389 2022-12-14 14:41:06.000000 tendril-filestore-0.1.9/src/tendril/filestore/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2839 2022-12-11 09:56:27.000000 tendril-filestore-0.1.9/src/tendril/filestore/buckets.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.217102 tendril-filestore-0.1.9/src/tendril/filestore/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 14:37:31.000000 tendril-filestore-0.1.9/src/tendril/filestore/db/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5289 2022-12-14 20:29:18.000000 tendril-filestore-0.1.9/src/tendril/filestore/db/controller.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1290 2022-12-11 09:56:27.000000 tendril-filestore-0.1.9/src/tendril/filestore/db/model.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      101 2022-12-11 09:56:27.000000 tendril-filestore-0.1.9/src/tendril/filestore/remote.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.217102 tendril-filestore-0.1.9/src/tendril_filestore.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3983 2022-12-14 20:31:12.000000 tendril-filestore-0.1.9/src/tendril_filestore.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1250 2022-12-14 20:31:12.000000 tendril-filestore-0.1.9/src/tendril_filestore.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2022-12-14 20:31:12.000000 tendril-filestore-0.1.9/src/tendril_filestore.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      585 2022-12-14 20:31:12.000000 tendril-filestore-0.1.9/src/tendril_filestore.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2022-12-14 20:31:12.000000 tendril-filestore-0.1.9/src/tendril_filestore.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.217102 tendril-filestore-0.1.9/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.612235 tendril-filestore-0.2.0/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2023-04-20 18:31:02.612235 tendril-filestore-0.2.0/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.560236 tendril-filestore-0.2.0/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.572236 tendril-filestore-0.2.0/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.572236 tendril-filestore-0.2.0/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.572236 tendril-filestore-0.2.0/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      943 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.576236 tendril-filestore-0.2.0/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-20 18:31:02.616235 tendril-filestore-0.2.0/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3281 2022-12-15 16:44:04.000000 tendril-filestore-0.2.0/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.536237 tendril-filestore-0.2.0/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.576236 tendril-filestore-0.2.0/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.576236 tendril-filestore-0.2.0/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.2.0/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.580236 tendril-filestore-0.2.0/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.2.0/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5603 2023-04-19 18:02:43.000000 tendril-filestore-0.2.0/src/tendril/apiserver/routers/filestore.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.584236 tendril-filestore-0.2.0/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:36:13.000000 tendril-filestore-0.2.0/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.584236 tendril-filestore-0.2.0/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 21:03:32.000000 tendril-filestore-0.2.0/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      264 2023-03-27 15:39:22.000000 tendril-filestore-0.2.0/src/tendril/authz/scopes/filestore.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.588236 tendril-filestore-0.2.0/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-19 12:09:04.000000 tendril-filestore-0.2.0/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.588236 tendril-filestore-0.2.0/src/tendril/common/filestore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-19 11:58:32.000000 tendril-filestore-0.2.0/src/tendril/common/filestore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1646 2023-04-19 17:38:08.000000 tendril-filestore-0.2.0/src/tendril/common/filestore/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.592236 tendril-filestore-0.2.0/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3744 2023-04-20 12:32:50.000000 tendril-filestore-0.2.0/src/tendril/config/filestore.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3458 2023-04-20 12:32:52.000000 tendril-filestore-0.2.0/src/tendril/config/filestore_core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.600236 tendril-filestore-0.2.0/src/tendril/filestore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 21:59:13.000000 tendril-filestore-0.2.0/src/tendril/filestore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6759 2023-04-19 17:30:32.000000 tendril-filestore-0.2.0/src/tendril/filestore/actual.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1467 2023-04-11 16:08:16.000000 tendril-filestore-0.2.0/src/tendril/filestore/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2977 2023-04-20 15:56:35.000000 tendril-filestore-0.2.0/src/tendril/filestore/buckets.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.604236 tendril-filestore-0.2.0/src/tendril/filestore/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 17:57:19.000000 tendril-filestore-0.2.0/src/tendril/filestore/db/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6250 2023-04-19 17:30:49.000000 tendril-filestore-0.2.0/src/tendril/filestore/db/controller.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1426 2023-04-11 18:49:23.000000 tendril-filestore-0.2.0/src/tendril/filestore/db/model.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1266 2023-04-20 18:21:53.000000 tendril-filestore-0.2.0/src/tendril/filestore/remote.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.608235 tendril-filestore-0.2.0/src/tendril_filestore.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2023-04-20 18:31:01.000000 tendril-filestore-0.2.0/src/tendril_filestore.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1362 2023-04-20 18:31:02.000000 tendril-filestore-0.2.0/src/tendril_filestore.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-20 18:31:01.000000 tendril-filestore-0.2.0/src/tendril_filestore.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      585 2023-04-20 18:31:01.000000 tendril-filestore-0.2.0/src/tendril_filestore.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-20 18:31:01.000000 tendril-filestore-0.2.0/src/tendril_filestore.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:31:02.612235 tendril-filestore-0.2.0/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-08 18:25:43.000000 tendril-filestore-0.2.0/tox.ini
```

### Comparing `tendril-filestore-0.1.9/.gitignore` & `tendril-filestore-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/.readthedocs.yml` & `tendril-filestore-0.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/.travis.yml` & `tendril-filestore-0.2.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/LICENSE` & `tendril-filestore-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/PKG-INFO` & `tendril-filestore-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-filestore
-Version: 0.1.9
+Version: 0.2.0
 Summary: File Storage and Management Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-filestore
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
 Project-URL: Documentation, https://tendril-filestore.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-filestore/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-filestore
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-filestore.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-filestore
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-filestore.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-filestore
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-filestore.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-filestore
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-filestore.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-filestore
-        
-        .. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
-            :target: https://www.codacy.com/app/chintal/tendril-filestore
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-filestore.svg
-            :target: https://requires.io/github/tendril-framework/tendril-filestore/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-filestore.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
-        
-        
-        
-        .. inclusion-marker-do-not-remove
-        
-        Introduction
-        ------------
-        
-        TODO Some brief introduction
-        
-        
-        Package Information
-        -------------------
-        
-        The latest version of the documentation, including installation, usage, and
-        API/developer notes can be found at
-        `ReadTheDocs <https://tendril-filestore.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-filestore>`_. Please use 
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-filestore`` is Chintalagiri Shashank. The 
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-filestore`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
-        
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -81,7 +25,63 @@
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
 Provides-Extra: publish
 Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-filestore.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-filestore
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-filestore.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-filestore
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-filestore.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-filestore
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-filestore.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-filestore
+
+.. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-filestore
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-filestore.svg
+    :target: https://requires.io/github/tendril-framework/tendril-filestore/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-filestore.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
+
+
+
+.. inclusion-marker-do-not-remove
+
+Introduction
+------------
+
+TODO Some brief introduction
+
+
+Package Information
+-------------------
+
+The latest version of the documentation, including installation, usage, and
+API/developer notes can be found at
+`ReadTheDocs <https://tendril-filestore.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-filestore>`_. Please use 
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-filestore`` is Chintalagiri Shashank. The 
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-filestore`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
+
```

### Comparing `tendril-filestore-0.1.9/README.rst` & `tendril-filestore-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/docs/Makefile` & `tendril-filestore-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/docs/_static/custom.css` & `tendril-filestore-0.2.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/docs/_static/favicon.ico` & `tendril-filestore-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/docs/_static/logo.png` & `tendril-filestore-0.2.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/docs/_static/logo_packed.png` & `tendril-filestore-0.2.0/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/docs/_templates/about.html` & `tendril-filestore-0.2.0/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/docs/conf.py` & `tendril-filestore-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/docs/index.rst` & `tendril-filestore-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/docs/installation.rst` & `tendril-filestore-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/setup.py` & `tendril-filestore-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/src/tendril/apiserver/routers/filestore.py` & `tendril-filestore-0.2.0/src/tendril/apiserver/routers/filestore.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,29 @@
 
 
-import json
-import datetime
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import Request
 from fastapi import File
 from fastapi import UploadFile
 from fastapi import HTTPException
-from fastapi import Body
 from fastapi_pagination import Page
 from fastapi_pagination import Params
-from fastapi_pagination import add_pagination
-
-from typing import Union
-from pydantic import Field
-from pydantic import validator
 
 from tendril.authn.users import auth_spec
 from tendril.authn.users import AuthUserModel
 from tendril.authn.users import authn_dependency
-from tendril.authn.users import UserStubTMixin
 
-from tendril.filestore.buckets import available_buckets
 from tendril.filestore.buckets import get_bucket
+from tendril.filestore.buckets import available_buckets
 from tendril.filestore.actual import FilestoreBucket
 
-from tendril.utils.pydantic import TendrilTBaseModel
+from tendril.common.filestore.formats import BucketName
+from tendril.common.filestore.formats import MoveRequest
+from tendril.common.filestore.formats import StoredFileTModel
 
 from tendril.config import FILESTORE_ENABLED
 
 
 filestore = APIRouter(prefix='/filestore',
                       tags=["File Management API"],
                       dependencies=[Depends(authn_dependency),
@@ -39,47 +32,14 @@
 
 filestore_management = APIRouter(prefix='/filestore',
                                  tags=["File Management Administration API"],
                                  dependencies=[Depends(authn_dependency),
                                                auth_spec(scopes=['file_management:admin'])])
 
 
-_available_buckets = available_buckets()
-
-
-class BucketName(str):
-    @classmethod
-    def _get_validators__(cls):
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, v):
-        if v not in _available_buckets:
-            raise ValueError(f"'{v}' is not in {_available_buckets}")
-        return cls(v)
-
-
-class StoredFile(str):
-    @classmethod
-    def _get_validators__(cls):
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, v):
-        if v not in _available_buckets:
-            raise ValueError(f"'{v}' is not in {_available_buckets}")
-        return cls(v)
-
-
-class MoveRequest(TendrilTBaseModel):
-    to_bucket: BucketName
-    filename: str
-    overwrite : bool = False
-
-
 @filestore.get("/buckets")
 async def get_available_buckets():
     return {'available_buckets': available_buckets()}
 
 
 @filestore.post("/{bucket}/upload")
 async def upload_file_to_bucket(
@@ -175,50 +135,32 @@
         raise HTTPException(
             status_code=403,
             detail=str(e)
         )
     return {'deleted': filename}
 
 
-class StoredFilePropsTModel(TendrilTBaseModel):
-    size: int = Field(..., example=714794)
-    created: Union[datetime.datetime, None]
-    modified: Union[datetime.datetime, None]
-
-
-class StoredFileHashTModel(TendrilTBaseModel):
-    sha256: str = Field(..., example='e4dd9b81d05aec0ce7f3a66b9efd15a13da5dae6e6672b84c7a75b3504c22d43')
-
-
-class StoredFileInfoTModel(TendrilTBaseModel):
-    ext: str = Field(..., example='.jpg')
-    hash: StoredFileHashTModel
-    props: StoredFilePropsTModel
-
-
-class StoredFileTModel(UserStubTMixin(out='owner'), TendrilTBaseModel):
-    filename: str = Field(..., example="some_filename.jpg")
-    fileinfo: StoredFileInfoTModel
-
-
 @filestore_management.post("/{bucket}/ls",
-                           response_model=Page[StoredFileTModel])
+                           response_model=Page[StoredFileTModel],
+                           response_model_exclude_none=True)
 async def list_files_in_bucket(
         request: Request,
         bucket: BucketName,
+        include_owner: bool = False,
         params: Params = Depends(),
         user: AuthUserModel = auth_spec()):
     try:
         bucket: FilestoreBucket = get_bucket(bucket)
     except KeyError:
         raise HTTPException(
             status_code=404,
             detail=f'{bucket} is not a recognized filestore bucket'
         )
-    return bucket.list_info(params)
+    return bucket.list_info(include_owner=include_owner,
+                            pagination_params=params)
 
 
 @filestore_management.post("/{bucket}/purge")
 async def purge_all_files_in_bucket(
         request: Request,
         bucket: BucketName,
         user: AuthUserModel = auth_spec()):
```

### Comparing `tendril-filestore-0.1.9/src/tendril/config/__init__.py` & `tendril-filestore-0.2.0/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/src/tendril/config/filestore.py` & `tendril-filestore-0.2.0/src/tendril/config/filestore.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,22 @@
             'FILESTORE_{}_ALLOW_OVERWRITE'.format(filestore_name),
             "False",
             "Whether the filestore API should allow overwwriting of files in this bucket. "
             "Users can still overwrite files owned by them, and Tendril internals can "
             "still overwrite files in this file store irrespective of this setting."
         ),
         ConfigOption(
+            'FILESTORE_{}_EXPOSE_URI'.format(filestore_name),
+            "None",
+            "URI at which the filestore content is exposed. Tendril filestore code will "
+            "simply construct URIs for individual files using string operations. The "
+            "URI may be public, private or entirely invalid depending on the bucket and "
+            "ingress configurations, outside of Tendril."
+        ),
+        ConfigOption(
             'FILESTORE_{}_ACTUAL'.format(filestore_name),
             "None",
             "Path to store this filestore bucket. If not provided, it will be placed within "
             "the default FILESTORE_ACTUAL path. This should either be a local file path or "
             "a pyfilesystems2 supported URI."
         ),
         FileStoreActualURI(
```

### Comparing `tendril-filestore-0.1.9/src/tendril/config/filestore_core.py` & `tendril-filestore-0.2.0/src/tendril/config/filestore_core.py`

 * *Files 26% similar despite different names*

```diff
@@ -47,19 +47,40 @@
         'FILESTORE_REMOTE_URI',
         "None",
         "Location of the actual filestore component, as a network URL. When set, this "
         "option will be used in components where FILESTORE_ENABLED is False to provide "
         "filestore functionality by proxying to the remote."
     ),
     ConfigOption(
+        'FILESTORE_REMOTE_AUDIENCE',
+        "None",
+        "API Audience to use when connecting to the actual filestore component. This is "
+        "presently not configured per-bucket and is intended for use only as an Auth0 M2M "
+        "application"
+    ),
+    ConfigOption(
+        'FILESTORE_REMOTE_CLIENT_ID',
+        "None",
+        "Auth0 Client ID to use when connecting to the actual filestore component. This is "
+        "presently not configured per-bucket and is intended for use only as an Auth0 M2M "
+        "application", masked=True
+    ),
+    ConfigOption(
+        'FILESTORE_REMOTE_CLIENT_SECRET',
+        "None",
+        "Auth0 Client Secret to use when connecting to the actual filestore component. This is "
+        "presently not configured per-bucket and is intended for use only as an Auth0 M2M "
+        "application", masked=True
+    ),
+    ConfigOption(
         'FILESTORE_ACTUAL',
         "os.path.join(INSTANCE_ROOT, 'filestore')",
         "Default path to create filestore folders at. This may "
         "be overridden by individual filestore bucket configurations."
     )
 ]
 
 
 def load(manager):
     logger.debug("Loading {0}".format(__name__))
     manager.load_elements(config_elements_filestore_core,
-                          doc="Tendril Filestore Core Configuration")
+                          doc="Filestore Core Configuration")
```

### Comparing `tendril-filestore-0.1.9/src/tendril/filestore/actual.py` & `tendril-filestore-0.2.0/src/tendril/filestore/actual.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 
 import hashlib
 import os
 
 from fs import open_fs
 from fs import move
+from sqlalchemy.exc import NoResultFound
 
 from tendril.authn.users import get_user_stub
 from tendril.filestore.base import FilestoreBucketBase
 from tendril.filestore.db.controller import register_bucket
 from tendril.filestore.db.controller import get_storedfile_owner
 from tendril.filestore.db.controller import register_stored_file
 from tendril.filestore.db.controller import change_file_bucket
@@ -52,24 +53,34 @@
         return self._id
 
     def _create_in_db(self):
         b = register_bucket(name=self.name)
         self._id = b.id
 
     @with_db
-    def _prep_for_upload(self, bucket, filename, user, overwrite=False, session=None):
+    def _prep_for_upload(self, bucket, filename, user, overwrite=False, auto_prune=True, session=None):
         if bucket.fs.exists(filename):
             if not overwrite:
                 raise FileExistsError(f'{filename} already exists in the {bucket.name} bucket. Delete it first.')
-            # TODO If file exists in fs but not in DB?
-            owner = get_storedfile_owner(filename, bucket.id, session=session)
-            if not bucket.allow_overwrite and owner.puid != user:
-                raise FileExistsError(f'{filename} already exists in the {bucket.name} bucket and owned by someone else.')
-            logger.warning(f"Overwriting file {filename} in bucket {bucket.name}.")
-            bucket.delete(filename, user, session=session)
+            try:
+                owner = get_storedfile_owner(filename, bucket.id, session=session)
+            except NoResultFound:
+                # file exists in fs but not in DB
+                if not auto_prune:
+                    raise FileExistsError(f"'{filename}' already exists in the '{bucket.name}' filesystem but "
+                                          f"not in the database. This needs to be manually resolved.")
+                logger.warning(f"'{filename}' exists in the '{bucket.name}' filesystem but "
+                               f"not in the database. Pruning. Possible Data Loss.")
+                bucket.fs.remove(filename)
+            else:
+                if not bucket.allow_overwrite and owner.puid != user:
+                    raise FileExistsError(f'{filename} already exists in the {bucket.name} bucket '
+                                          f'and owned by someone else.')
+                logger.warning(f"Overwriting file {filename} in bucket {bucket.name}.")
+                bucket.delete(filename, user, session=session)
 
     @with_db
     def upload(self, file, user, overwrite=False, session=None):
         filename = file.filename
         self._prep_for_upload(self, filename, user, overwrite)
 
         with self._fs.open(filename, 'wb') as target:
@@ -135,19 +146,22 @@
                                    exclude_files=self._exclude_filenames,
                                    exclude_dirs=self._exclude_directories):
             yield f.name
 
     def list(self, page=None):
         return list(self._list(page=page))
 
-    @with_db
-    def list_info(self, params, page=None, session=None):
+    def list_info(self, include_owner=False,
+                  pagination_params=None, page=None):
         items = self.list(page)
         return get_paginated_stored_files(
-            params, filenames=items, bucket=self.id, session=session)
+            pagination_params=pagination_params,
+            filenames=items, bucket=self.id,
+            include_owner=include_owner
+        )
 
     def purge(self, user):
         if not self._allow_delete:
             raise PermissionError(f"Deletion of files from bucket {self.name} "
                                   f"is not permitted")
         logger.warning(f"Purging all files from bucket {self.name}")
         for filename in self.list():
```

### Comparing `tendril-filestore-0.1.9/src/tendril/filestore/base.py` & `tendril-filestore-0.2.0/src/tendril/filestore/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 
 
 import os
 
 
 class FilestoreBucketBase(object):
-    def __init__(self, uri, name, accept_ext=None, allow_delete=False, allow_overwrite=False):
+    def __init__(self, uri, name, expose_uri=None,
+                 accept_ext=None, allow_delete=False, allow_overwrite=False):
         self._id = None
         self._uri = uri
         self._name = name
+        self._expose_uri = expose_uri or ''
         self._accept_ext = accept_ext or []
         self._allow_delete = allow_delete
         self._allow_overwrite = allow_overwrite
 
     @property
     def id(self):
         return self._id
```

### Comparing `tendril-filestore-0.1.9/src/tendril/filestore/buckets.py` & `tendril-filestore-0.2.0/src/tendril/filestore/buckets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 
+
+import asyncio
 from tendril import config
 from tendril.filestore.actual import FilestoreBucket
 from tendril.filestore.remote import FilestoreBucketRemote
+from tendril.filestore.remote import get_remote_bucket_list
 
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEFAULT)
 
 
 _available_buckets = {}
 
@@ -21,44 +24,44 @@
 def _bucket_config(bucket_name):
     bucket_name = bucket_name.upper()
     enabled = getattr(config, "FILESTORE_{}_ENABLED".format(bucket_name))
     accept_ext = getattr(config, "FILESTORE_{}_ACCEPT_EXT".format(bucket_name))
     allow_delete = getattr(config, "FILESTORE_{}_ALLOW_DELETE".format(bucket_name))
     allow_overwrite = getattr(config, "FILESTORE_{}_ALLOW_OVERWRITE".format(bucket_name))
     actual_uri = getattr(config, "FILESTORE_{}_ACTUAL_URI".format(bucket_name))
-    return enabled, accept_ext, allow_delete, allow_overwrite, actual_uri
+    expose_uri = getattr(config, "FILESTORE_{}_EXPOSE_URI".format(bucket_name))
+    return enabled, accept_ext, expose_uri, allow_delete, allow_overwrite, actual_uri
 
 
 def init_remote():
     if not config.FILESTORE_REMOTE_URI:
         logger.warning("Filestore is not enabled and a remote filestore "
                        "has not been configured. Filestore operations "
                        "should be executed via the appropriate API on "
                        "the filestore component. ")
     else:
         logger.info("Attempting to make a connection to the remote filestore.")
         uri = config.FILESTORE_REMOTE_URI
-        # Get remote filestore bucket list from FILESTORE_REMOTE_URI/filestore/buckets
-        remote_bucket_list = ['incoming', 'cdn', 'outgoing']
+        remote_bucket_list = asyncio.run(get_remote_bucket_list(uri))
         for bucket_name in config.FILESTORE_BUCKETS:
-            enabled, accept_ext, allow_delete, allow_overwrite, _ = _bucket_config(bucket_name)
+            enabled, accept_ext, expose_uri, allow_delete, allow_overwrite, _ = _bucket_config(bucket_name)
             if enabled and bucket_name in remote_bucket_list:
                 logger.info(f"Creating proxy to the remote filestore bucket {bucket_name} at {uri}.")
-                bucket = FilestoreBucketRemote(uri, bucket_name, accept_ext, allow_delete, allow_overwrite)
+                bucket = FilestoreBucketRemote(uri, bucket_name, expose_uri, accept_ext, allow_delete, allow_overwrite)
                 _available_buckets[bucket_name] = bucket
 
 
 def init_actual():
     for bucket_name in config.FILESTORE_BUCKETS:
-        enabled, accept_ext, allow_delete, allow_overwrite, actual_uri = _bucket_config(bucket_name)
+        enabled, accept_ext, expose_uri, allow_delete, allow_overwrite, actual_uri = _bucket_config(bucket_name)
         if not enabled:
             logger.debug("Bucket '{}' not enabled. Skipping.".format(bucket_name))
             continue
         logger.info("Creating filestore bucket '{}' at {}".format(bucket_name, actual_uri))
-        bucket = FilestoreBucket(actual_uri, bucket_name, accept_ext, allow_delete, allow_overwrite)
+        bucket = FilestoreBucket(actual_uri, bucket_name, expose_uri, accept_ext, allow_delete, allow_overwrite)
         _available_buckets[bucket_name] = bucket
 
 
 def init():
     if not config.FILESTORE_ENABLED:
         logger.info("Filestore actual not enabled on this component.")
         init_remote()
```

### Comparing `tendril-filestore-0.1.9/src/tendril/filestore/db/controller.py` & `tendril-filestore-0.2.0/src/tendril/filestore/db/controller.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 
 
+from functools import partial
+from sqlalchemy import select
 from fastapi_pagination.ext.sqlalchemy import paginate
 from sqlalchemy.orm.exc import NoResultFound
 
 from tendril.utils.db import with_db
 from tendril.authn.db.model import User
 from tendril.authn.db.controller import preprocess_user
 from tendril.artefacts.db.controller import get_artefact_owner
@@ -78,25 +80,50 @@
     if filenames:
         filters.append(StoredFileModel.filename.in_(filenames))
 
     q = session.query(StoredFileModel).filter(*filters)
     return q.all()
 
 
+def _stored_file_transformer(items, include_owner=False):
+    if not include_owner:
+        return [{'filename': x[0], 'fileinfo': x[1]}
+                for x in items]
+    return [
+        {'filename': x[0],
+         'fileinfo': x[1],
+         'puid': x[2]}
+        for x in items
+    ]
+
+
 @with_db
-def get_paginated_stored_files(params, bucket, filenames=None, session=None):
+def get_paginated_stored_files(bucket, pagination_params=None, filenames=None, include_owner=False, session=None):
     bucket_id = preprocess_bucket(bucket, session=None)
     filters = [StoredFileModel.bucket_id == bucket_id]
 
     if filenames:
         filters.append(StoredFileModel.filename.in_(filenames))
 
-    q = session.query(StoredFileModel.filename, StoredFileModel.fileinfo, User.puid).\
-        join(User).filter(*filters)
-    return paginate(q, params)
+    if include_owner:
+        stmt = select(StoredFileModel.filename, StoredFileModel.fileinfo, User.puid)\
+            .join(StoredFileModel.user)\
+            .filter(*filters)
+    else:
+        stmt = select(StoredFileModel.filename, StoredFileModel.fileinfo)\
+            .filter(*filters)
+
+    if pagination_params:
+        return paginate(query=stmt, conn=session, unique=False,
+                        params=pagination_params,
+                        transformer=partial(_stored_file_transformer,
+                                            include_owner=include_owner))
+    else:
+        return _stored_file_transformer(session.execute(stmt).all(),
+                                        include_owner=include_owner)
 
 
 @with_db
 def register_stored_file(filename, bucket, user, fileinfo=None, overwrite=True, session=None):
     if not config.FILESTORE_ENABLED:
         raise EnvironmentError("Filestore not enabled on this component. "
                                "Use the filestore API on the filestore component instead.")
@@ -157,8 +184,8 @@
 @with_db
 def delete_stored_file(filename, bucket, user, session=None):
     sf = get_stored_file(filename=filename, bucket=bucket, session=session)
 
     # TODO Create Log Entry and archive log?
 
     session.delete(sf)
-    return
+    return
```

### Comparing `tendril-filestore-0.1.9/src/tendril/filestore/db/model.py` & `tendril-filestore-0.2.0/src/tendril/filestore/db/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 
+from urllib.parse import urljoin
 from sqlalchemy import Column
 from sqlalchemy import String
 from sqlalchemy import Integer
 from sqlalchemy import ForeignKey
 from sqlalchemy import UniqueConstraint
 from sqlalchemy.orm import relationship
 from sqlalchemy_json import mutable_json_type
@@ -29,14 +30,18 @@
     id = Column(Integer, ForeignKey("Artefact.id"), primary_key=True)
     filename = Column(String(255), nullable=False)
     fileinfo = Column(mutable_json_type(dbtype=JSONB, nested=True))
     bucket_id = Column(Integer(),
                        ForeignKey('FilestoreBucket.id'), nullable=False)
     bucket = relationship("FilestoreBucketModel", back_populates="files")
 
+    @property
+    def expose_uri(self):
+        return urljoin(self.bucket.expose_uri, self.filename)
+
     __mapper_args__ = {
         "polymorphic_identity": _type_name,
     }
 
     __table_args__ = (
         UniqueConstraint('filename', 'bucket_id'),
     )
```

### Comparing `tendril-filestore-0.1.9/src/tendril_filestore.egg-info/PKG-INFO` & `tendril-filestore-0.2.0/src/tendril_filestore.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-filestore
-Version: 0.1.9
+Version: 0.2.0
 Summary: File Storage and Management Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-filestore
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
 Project-URL: Documentation, https://tendril-filestore.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-filestore/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-filestore
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-filestore.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-filestore
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-filestore.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-filestore
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-filestore.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-filestore
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-filestore.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-filestore
-        
-        .. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
-            :target: https://www.codacy.com/app/chintal/tendril-filestore
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-filestore.svg
-            :target: https://requires.io/github/tendril-framework/tendril-filestore/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-filestore.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
-        
-        
-        
-        .. inclusion-marker-do-not-remove
-        
-        Introduction
-        ------------
-        
-        TODO Some brief introduction
-        
-        
-        Package Information
-        -------------------
-        
-        The latest version of the documentation, including installation, usage, and
-        API/developer notes can be found at
-        `ReadTheDocs <https://tendril-filestore.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-filestore>`_. Please use 
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-filestore`` is Chintalagiri Shashank. The 
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-filestore`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
-        
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -81,7 +25,63 @@
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
 Provides-Extra: publish
 Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-filestore.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-filestore
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-filestore.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-filestore
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-filestore.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-filestore
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-filestore.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-filestore
+
+.. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-filestore
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-filestore.svg
+    :target: https://requires.io/github/tendril-framework/tendril-filestore/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-filestore.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
+
+
+
+.. inclusion-marker-do-not-remove
+
+Introduction
+------------
+
+TODO Some brief introduction
+
+
+Package Information
+-------------------
+
+The latest version of the documentation, including installation, usage, and
+API/developer notes can be found at
+`ReadTheDocs <https://tendril-filestore.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-filestore>`_. Please use 
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-filestore`` is Chintalagiri Shashank. The 
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-filestore`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
+
```

### Comparing `tendril-filestore-0.1.9/src/tendril_filestore.egg-info/SOURCES.txt` & `tendril-filestore-0.2.0/src/tendril_filestore.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 src/tendril/__init__.py
 src/tendril/apiserver/__init__.py
 src/tendril/apiserver/routers/__init__.py
 src/tendril/apiserver/routers/filestore.py
 src/tendril/authz/__init__.py
 src/tendril/authz/scopes/__init__.py
 src/tendril/authz/scopes/filestore.py
+src/tendril/common/__init__.py
+src/tendril/common/filestore/__init__.py
+src/tendril/common/filestore/formats.py
 src/tendril/config/__init__.py
 src/tendril/config/filestore.py
 src/tendril/config/filestore_core.py
 src/tendril/filestore/__init__.py
 src/tendril/filestore/actual.py
 src/tendril/filestore/base.py
 src/tendril/filestore/buckets.py
```

### Comparing `tendril-filestore-0.1.9/src/tendril_filestore.egg-info/requires.txt` & `tendril-filestore-0.2.0/src/tendril_filestore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/tests/coveralls.py` & `tendril-filestore-0.2.0/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.9/tox.ini` & `tendril-filestore-0.2.0/tox.ini`

 * *Files identical despite different names*

