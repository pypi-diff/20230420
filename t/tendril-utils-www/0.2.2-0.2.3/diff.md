# Comparing `tmp/tendril-utils-www-0.2.2.tar.gz` & `tmp/tendril-utils-www-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tendril-utils-www-0.2.2.tar", last modified: Fri Aug  2 00:41:40 2019, max compression
+gzip compressed data, was "tendril-utils-www-0.2.3.tar", last modified: Thu Apr 20 18:35:17 2023, max compression
```

## Comparing `tendril-utils-www-0.2.2.tar` & `tendril-utils-www-0.2.3.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2019-07-31 19:40:20.000000 tendril-utils-www-0.2.2/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3950 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/setup.cfg
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2223 2019-08-01 17:38:31.000000 tendril-utils-www-0.2.2/README.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2019-07-30 10:56:54.000000 tendril-utils-www-0.2.2/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      829 2019-08-01 09:31:09.000000 tendril-utils-www-0.2.2/tox.ini
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2121 2019-08-01 16:27:45.000000 tendril-utils-www-0.2.2/.gitignore
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/src/tendril/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/src/tendril/utils/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/src/tendril/utils/www/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5089 2019-08-01 14:03:24.000000 tendril-utils-www-0.2.2/src/tendril/utils/www/req.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1490 2019-08-01 14:03:24.000000 tendril-utils-www-0.2.2/src/tendril/utils/www/status.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3008 2019-08-01 16:42:41.000000 tendril-utils-www-0.2.2/src/tendril/utils/www/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3868 2019-08-01 14:03:24.000000 tendril-utils-www-0.2.2/src/tendril/utils/www/redirectcache.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7841 2019-08-01 16:44:05.000000 tendril-utils-www-0.2.2/src/tendril/utils/www/caching.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7607 2019-08-01 16:43:26.000000 tendril-utils-www-0.2.2/src/tendril/utils/www/bare.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3401 2019-08-01 14:03:24.000000 tendril-utils-www-0.2.2/src/tendril/utils/www/helpers.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9328 2019-08-01 16:44:22.000000 tendril-utils-www-0.2.2/src/tendril/utils/www/soap.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      851 2018-09-11 23:59:44.000000 tendril-utils-www-0.2.2/src/tendril/utils/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      851 2018-09-11 23:59:44.000000 tendril-utils-www-0.2.2/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2019-04-01 11:34:55.000000 tendril-utils-www-0.2.2/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1478 2019-04-08 10:43:38.000000 tendril-utils-www-0.2.2/src/tendril/config/www.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/src/tendril_utils_www.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3950 2019-08-02 00:41:39.000000 tendril-utils-www-0.2.2/src/tendril_utils_www.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      636 2019-08-02 00:41:39.000000 tendril-utils-www-0.2.2/src/tendril_utils_www.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2019-08-02 00:41:39.000000 tendril-utils-www-0.2.2/src/tendril_utils_www.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2019-08-02 00:41:39.000000 tendril-utils-www-0.2.2/src/tendril_utils_www.egg-info/top_level.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1371 2019-08-02 00:41:39.000000 tendril-utils-www-0.2.2/src/tendril_utils_www.egg-info/SOURCES.txt
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3425 2019-08-02 00:39:54.000000 tendril-utils-www-0.2.2/setup.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2019-08-01 09:20:25.000000 tendril-utils-www-0.2.2/MANIFEST.in
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2019-08-01 09:38:25.000000 tendril-utils-www-0.2.2/docs/conf.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       97 2019-08-01 13:47:42.000000 tendril-utils-www-0.2.2/docs/api/tendril.utils.www.soap.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      106 2019-08-01 13:49:05.000000 tendril-utils-www-0.2.2/docs/api/tendril.utils.www.redirectcache.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       93 2019-08-01 09:36:09.000000 tendril-utils-www-0.2.2/docs/api/tendril.config.www.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      100 2019-08-01 13:48:17.000000 tendril-utils-www-0.2.2/docs/api/tendril.utils.www.helpers.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       99 2019-08-01 13:49:23.000000 tendril-utils-www-0.2.2/docs/api/tendril.utils.www.status.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      100 2019-08-01 13:48:39.000000 tendril-utils-www-0.2.2/docs/api/tendril.utils.www.caching.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       97 2019-08-01 13:47:16.000000 tendril-utils-www-0.2.2/docs/api/tendril.utils.www.bare.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      577 2019-08-01 16:14:58.000000 tendril-utils-www-0.2.2/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       96 2019-08-01 13:47:38.000000 tendril-utils-www-0.2.2/docs/api/tendril.utils.www.req.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2015-08-23 17:49:15.000000 tendril-utils-www-0.2.2/docs/_static/logo_packed.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2019-07-31 07:34:28.000000 tendril-utils-www-0.2.2/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2019-07-31 06:52:53.000000 tendril-utils-www-0.2.2/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2015-08-23 17:49:15.000000 tendril-utils-www-0.2.2/docs/_static/logo.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2019-07-30 10:54:54.000000 tendril-utils-www-0.2.2/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2019-07-30 11:12:55.000000 tendril-utils-www-0.2.2/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2019-07-30 11:12:55.000000 tendril-utils-www-0.2.2/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1088 2019-08-01 09:32:21.000000 tendril-utils-www-0.2.2/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2019-07-30 10:54:54.000000 tendril-utils-www-0.2.2/docs/Makefile
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1723 2019-08-02 00:40:19.000000 tendril-utils-www-0.2.2/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-08-02 00:41:40.000000 tendril-utils-www-0.2.2/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1106 2019-08-01 14:24:03.000000 tendril-utils-www-0.2.2/tests/test_helpers.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1721 2019-08-01 16:19:53.000000 tendril-utils-www-0.2.2/tests/test_bare.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2019-07-30 10:55:00.000000 tendril-utils-www-0.2.2/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2245 2019-08-01 14:33:04.000000 tendril-utils-www-0.2.2/tests/test_redirectcache.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2019-07-30 10:55:00.000000 tendril-utils-www-0.2.2/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2018-09-11 23:59:44.000000 tendril-utils-www-0.2.2/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2019-07-30 10:47:23.000000 tendril-utils-www-0.2.2/CHANGELOG.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:35:17.099210 tendril-utils-www-0.2.3/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2121 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3518 2023-04-20 18:35:17.103210 tendril-utils-www-0.2.3/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2223 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:35:17.063211 tendril-utils-www-0.2.3/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:35:17.071210 tendril-utils-www-0.2.3/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:35:17.071210 tendril-utils-www-0.2.3/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:35:17.079210 tendril-utils-www-0.2.3/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      577 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       93 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/api/tendril.config.www.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       97 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/api/tendril.utils.www.bare.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      100 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/api/tendril.utils.www.caching.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      100 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/api/tendril.utils.www.helpers.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      106 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/api/tendril.utils.www.redirectcache.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       96 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/api/tendril.utils.www.req.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       97 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/api/tendril.utils.www.soap.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       99 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/api/tendril.utils.www.status.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1088 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1723 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:35:17.079210 tendril-utils-www-0.2.3/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-20 18:35:17.103210 tendril-utils-www-0.2.3/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3431 2023-04-20 11:35:41.000000 tendril-utils-www-0.2.3/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:35:17.043211 tendril-utils-www-0.2.3/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:35:17.079210 tendril-utils-www-0.2.3/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:50:25.000000 tendril-utils-www-0.2.3/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:35:17.083210 tendril-utils-www-0.2.3/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1790 2023-04-20 17:08:41.000000 tendril-utils-www-0.2.3/src/tendril/config/www.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:35:17.083210 tendril-utils-www-0.2.3/src/tendril/utils/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:50:32.000000 tendril-utils-www-0.2.3/src/tendril/utils/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:35:17.091210 tendril-utils-www-0.2.3/src/tendril/utils/www/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3079 2023-04-20 11:35:41.000000 tendril-utils-www-0.2.3/src/tendril/utils/www/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7607 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/src/tendril/utils/www/bare.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7694 2023-04-20 11:45:06.000000 tendril-utils-www-0.2.3/src/tendril/utils/www/caching.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3401 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/src/tendril/utils/www/helpers.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3061 2023-04-20 17:11:07.000000 tendril-utils-www-0.2.3/src/tendril/utils/www/hx.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3868 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/src/tendril/utils/www/redirectcache.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5089 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/src/tendril/utils/www/req.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9328 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/src/tendril/utils/www/soap.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      303 2023-04-20 16:44:31.000000 tendril-utils-www-0.2.3/src/tendril/utils/www/ssl.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1490 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/src/tendril/utils/www/status.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:35:17.095210 tendril-utils-www-0.2.3/src/tendril_utils_www.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3518 2023-04-20 18:35:16.000000 tendril-utils-www-0.2.3/src/tendril_utils_www.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1428 2023-04-20 18:35:16.000000 tendril-utils-www-0.2.3/src/tendril_utils_www.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-20 18:35:16.000000 tendril-utils-www-0.2.3/src/tendril_utils_www.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      639 2023-04-20 18:35:16.000000 tendril-utils-www-0.2.3/src/tendril_utils_www.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-20 18:35:16.000000 tendril-utils-www-0.2.3/src/tendril_utils_www.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:35:17.099210 tendril-utils-www-0.2.3/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1721 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/tests/test_bare.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1106 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/tests/test_helpers.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2245 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/tests/test_redirectcache.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      829 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.3/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tendril-utils-www-0.2.2/.readthedocs.yml` & `tendril-utils-www-0.2.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/PKG-INFO` & `tendril-utils-www-0.2.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,72 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-utils-www
-Version: 0.2.2
+Version: 0.2.3
 Summary: Internet utilities for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-www
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
-Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-www
-Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-www/issues
 Project-URL: Documentation, https://tendril-utils-www.readthedocs.io/en/latest
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-utils-www.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-utils-www
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-utils-www.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-utils-www
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-utils-www.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-utils-www
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-utils-www.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-utils-www
-        
-        .. image:: https://img.shields.io/codacy/grade/c72090d9e83648d8b7c1c52e3d502da6?logo=codacy
-            :target: https://www.codacy.com/app/chintal/tendril-utils-www
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-utils-www.svg
-            :target: https://requires.io/github/tendril-framework/tendril-utils-www/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-utils-www.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
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
-        `ReadTheDocs <https://tendril-utils-www.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-utils-www>`_. Please use 
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-utils-www`` is Chintalagiri Shashank. The 
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-utils-www`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
-        
+Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-www/issues
+Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-www
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -78,9 +23,64 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
-Provides-Extra: dev
 Provides-Extra: publish
+Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-utils-www.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-utils-www
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-utils-www.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-utils-www
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-utils-www.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-utils-www
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-utils-www.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-utils-www
+
+.. image:: https://img.shields.io/codacy/grade/c72090d9e83648d8b7c1c52e3d502da6?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-utils-www
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-utils-www.svg
+    :target: https://requires.io/github/tendril-framework/tendril-utils-www/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-utils-www.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
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
+`ReadTheDocs <https://tendril-utils-www.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-utils-www>`_. Please use 
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-utils-www`` is Chintalagiri Shashank. The 
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-utils-www`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
+
```

### Comparing `tendril-utils-www-0.2.2/README.rst` & `tendril-utils-www-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/.travis.yml` & `tendril-utils-www-0.2.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/tox.ini` & `tendril-utils-www-0.2.3/tox.ini`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/.gitignore` & `tendril-utils-www-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/src/tendril/utils/www/req.py` & `tendril-utils-www-0.2.3/src/tendril/utils/www/req.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/src/tendril/utils/www/status.py` & `tendril-utils-www-0.2.3/src/tendril/utils/www/status.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/src/tendril/utils/www/__init__.py` & `tendril-utils-www-0.2.3/src/tendril/utils/www/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,18 +80,21 @@
     is the major bottleneck and seems to cause a major
     performance hit.
 
 """
 
 from .helpers import strencode  # noqa
 
-# Bare urllib based access
+# Bare urllib based client
 from .bare import urlopen           # noqa
 from .bare import cached_fetcher    # noqa
 from .bare import get_soup          # noqa
 
-# Requests based access
+# Requests based client
 from .req import get_session        # noqa
 from .req import get_soup_requests  # noqa
 
-# suds based SOAP access
+# suds based SOAP client
 from .soap import get_soap_client   # noqa
+
+# httpx based async client
+from .hx import async_client        # noqa
```

### Comparing `tendril-utils-www-0.2.2/src/tendril/utils/www/redirectcache.py` & `tendril-utils-www-0.2.3/src/tendril/utils/www/redirectcache.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/src/tendril/utils/www/caching.py` & `tendril-utils-www-0.2.3/src/tendril/utils/www/caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 
 import os
 import time
 import codecs
 import tempfile
 
-from fs.opener import fsopendir
-from fs.utils import copyfile
+from fs import open_fs
+from fs.copy import copy_file
 from fs.osfs import OSFS
 from tendril.utils.fsutils import temp_fs
 from tendril.config import INSTANCE_CACHE
 
 from .status import is_connected
 
 from tendril.utils import log
@@ -59,15 +59,15 @@
         If the cache's :func:`_accessor` function is called with the
         ``getcpath`` attribute set to True, only the path to a (valid) file
         in the cache filesystem is returned, and opening and reading
         the file is left to the caller. This hook is provided to help deal
         with file encoding on a somewhat case-by-case basis, until the
         overall encoding problems can be ironed out.
         """
-        self.cache_fs = fsopendir(cache_dir, create_dir=True)
+        self.cache_fs = open_fs(cache_dir, create=True)
 
     def _get_filepath(self, *args, **kwargs):
         """
         Given the parameters necessary to obtain the resource in normal
         circumstances, return a hash which is usable as the filename for
         the resource in the cache.
 
@@ -176,35 +176,33 @@
                         filecontent = f.read()
                         return self._deserialize(filecontent)
             else:
                 return self.cache_fs.getsyspath(filepath)
 
         logger.debug("Cache MISS")
         data = self._get_fresh_content(*args, **kwargs)
+
+        sdata = self._serialize(data)
+        fd, temppath = tempfile.mkstemp()
+        fp = os.fdopen(fd, 'wb')
+        fp.write(sdata)
+        fp.close()
+        logger.debug("Creating new cache entry")
+        # This can be pretty expensive if the move is across a real
+        # filesystem boundary. We should instead use a temporary file
+        # in the cache_fs itself
         try:
-            sdata = self._serialize(data)
-            fd, temppath = tempfile.mkstemp()
-            fp = os.fdopen(fd, 'wb')
-            fp.write(sdata)
-            fp.close()
-            logger.debug("Creating new cache entry")
-            # This can be pretty expensive if the move is across a real
-            # filesystem boundary. We should instead use a temporary file
-            # in the cache_fs itself
-            try:
-                copyfile(temp_fs, temp_fs.unsyspath(temppath),
-                         self.cache_fs, filepath)
-                if isinstance(self.cache_fs, OSFS):
-                    # TODO Refine permissions
-                    os.chmod(self.cache_fs.getsyspath(filepath), 0o666)
-            except (KeyboardInterrupt, SystemExit):
-                raise
-            except:  # noqa
-                logger.warning("Unable to write cache file "
-                               "{0}".format(filepath))
-        except:  # noqa
+            copy_file(temp_fs, temp_fs.unsyspath(temppath),
+                      self.cache_fs, filepath)
+            if isinstance(self.cache_fs, OSFS):
+                # TODO Refine permissions
+                os.chmod(self.cache_fs.getsyspath(filepath), 0o666)
+        except (KeyboardInterrupt, SystemExit):
             raise
+        except:  # noqa
+            logger.warning("Unable to write cache file "
+                           "{0}".format(filepath))
 
         if getcpath is False:
             return data
         else:
             return self.cache_fs.getsyspath(filepath)
```

### Comparing `tendril-utils-www-0.2.2/src/tendril/utils/www/bare.py` & `tendril-utils-www-0.2.3/src/tendril/utils/www/bare.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/src/tendril/utils/www/helpers.py` & `tendril-utils-www-0.2.3/src/tendril/utils/www/helpers.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/src/tendril/utils/www/soap.py` & `tendril-utils-www-0.2.3/src/tendril/utils/www/soap.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/src/tendril/utils/__init__.py` & `tendril-utils-www-0.2.3/src/tendril/config/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
-# Copyright (C) 2018 Chintalagiri Shashank
+# Copyright (C) 2019 Chintalagiri Shashank
 #
 # This file is part of tendril.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -16,7 +16,15 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
+
+from tendril.utils.config import ConfigManager
+_manager = ConfigManager(prefix='tendril.config',
+                         legacy='tendril.config.legacy',
+                         excluded=['tendril.config.legacy'])
+
+import sys
+sys.modules[__name__] = _manager
```

### Comparing `tendril-utils-www-0.2.2/src/tendril/__init__.py` & `tendril-utils-www-0.2.3/tests/test_helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
-# Copyright (C) 2018 Chintalagiri Shashank
+# Copyright (C) 2015 Chintalagiri Shashank
 #
 # This file is part of tendril.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -14,9 +14,23 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from pkgutil import extend_path
-__path__ = extend_path(__path__, __name__)
+"""
+Docstring for test_utils_www
+"""
+
+from tendril.utils.www import helpers
+
+
+def test_www_strencode():
+    pairs = [
+        (u'Test String', b'Test String'),
+        (u'', b''),
+        (u'\u00b5ACD', b'uACD'),
+        (u'\u00b11323', b'+/-1323'),
+    ]
+    for inp, outp in pairs:
+        assert helpers.strencode(inp) == outp
```

### Comparing `tendril-utils-www-0.2.2/src/tendril/config/www.py` & `tendril-utils-www-0.2.3/src/tendril/config/www.py`

 * *Files 26% similar despite different names*

```diff
@@ -47,13 +47,25 @@
         'NETWORK_PROXY_PASS',
         "None",
         "The password to authenticate with the proxy server."
     ),
 ]
 
 
+config_elements_ssl = [
+    ConfigOption(
+        'CA_BUNDLE',
+        "None",
+        "Path to a custom CA certificate bundle to use. This is "
+        "presently only used by the httpx backend"
+    ),
+]
+
+
 def load(manager):
     logger.debug("Loading {0}".format(__name__))
     manager.load_elements(config_elements_network_caching,
                           doc="Network Caching Behavior Configuration")
     manager.load_elements(config_elements_proxy,
                           doc="Network Proxy Configuration")
+    manager.load_elements(config_elements_ssl,
+                          doc="SSL Client Configuration")
```

### Comparing `tendril-utils-www-0.2.2/src/tendril_utils_www.egg-info/PKG-INFO` & `tendril-utils-www-0.2.3/src/tendril_utils_www.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,72 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-utils-www
-Version: 0.2.2
+Version: 0.2.3
 Summary: Internet utilities for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-www
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
-Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-www
-Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-www/issues
 Project-URL: Documentation, https://tendril-utils-www.readthedocs.io/en/latest
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-utils-www.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-utils-www
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-utils-www.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-utils-www
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-utils-www.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-utils-www
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-utils-www.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-utils-www
-        
-        .. image:: https://img.shields.io/codacy/grade/c72090d9e83648d8b7c1c52e3d502da6?logo=codacy
-            :target: https://www.codacy.com/app/chintal/tendril-utils-www
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-utils-www.svg
-            :target: https://requires.io/github/tendril-framework/tendril-utils-www/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-utils-www.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
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
-        `ReadTheDocs <https://tendril-utils-www.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-utils-www>`_. Please use 
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-utils-www`` is Chintalagiri Shashank. The 
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-utils-www`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
-        
+Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-www/issues
+Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-www
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -78,9 +23,64 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
-Provides-Extra: dev
 Provides-Extra: publish
+Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-utils-www.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-utils-www
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-utils-www.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-utils-www
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-utils-www.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-utils-www
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-utils-www.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-utils-www
+
+.. image:: https://img.shields.io/codacy/grade/c72090d9e83648d8b7c1c52e3d502da6?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-utils-www
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-utils-www.svg
+    :target: https://requires.io/github/tendril-framework/tendril-utils-www/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-utils-www.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
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
+`ReadTheDocs <https://tendril-utils-www.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-utils-www>`_. Please use 
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-utils-www`` is Chintalagiri Shashank. The 
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-utils-www`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
+
```

### Comparing `tendril-utils-www-0.2.2/src/tendril_utils_www.egg-info/requires.txt` & `tendril-utils-www-0.2.3/src/tendril_utils_www.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 tendril-utils-fsutils
 tendril-config>=0.1.6
 six
 lxml
 beautifulsoup4
 cachecontrol[filecache]
 requests
+httpx
 bs4
-suds
-fs==0.5.4
+fs
+suds-py3
 wheel
 
 [build]
 setuptools_scm
 sphinx
 sphinx-argparse
 alabaster
```

### Comparing `tendril-utils-www-0.2.2/src/tendril_utils_www.egg-info/SOURCES.txt` & `tendril-utils-www-0.2.3/src/tendril_utils_www.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,19 @@
 src/tendril/config/__init__.py
 src/tendril/config/www.py
 src/tendril/utils/__init__.py
 src/tendril/utils/www/__init__.py
 src/tendril/utils/www/bare.py
 src/tendril/utils/www/caching.py
 src/tendril/utils/www/helpers.py
+src/tendril/utils/www/hx.py
 src/tendril/utils/www/redirectcache.py
 src/tendril/utils/www/req.py
 src/tendril/utils/www/soap.py
+src/tendril/utils/www/ssl.py
 src/tendril/utils/www/status.py
 src/tendril_utils_www.egg-info/PKG-INFO
 src/tendril_utils_www.egg-info/SOURCES.txt
 src/tendril_utils_www.egg-info/dependency_links.txt
 src/tendril_utils_www.egg-info/requires.txt
 src/tendril_utils_www.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `tendril-utils-www-0.2.2/setup.py` & `tendril-utils-www-0.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,17 +40,18 @@
     'tendril-utils-fsutils',
     'tendril-config>=0.1.6',
     'six',
     'lxml',
     'beautifulsoup4',
     'cachecontrol[filecache]',
     'requests',
+    'httpx',
     'bs4',
+    'fs',
     suds,
-    'fs==0.5.4',
 ]
 
 install_requires = core_dependencies + ['wheel']
 
 setup_requires = ['setuptools_scm']
 
 doc_requires = setup_requires + ['sphinx', 'sphinx-argparse', 'alabaster']
```

### Comparing `tendril-utils-www-0.2.2/docs/conf.py` & `tendril-utils-www-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/docs/api/index.rst` & `tendril-utils-www-0.2.3/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/docs/_static/logo_packed.png` & `tendril-utils-www-0.2.3/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/docs/_static/custom.css` & `tendril-utils-www-0.2.3/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/docs/_static/favicon.ico` & `tendril-utils-www-0.2.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/docs/_static/logo.png` & `tendril-utils-www-0.2.3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/docs/_templates/about.html` & `tendril-utils-www-0.2.3/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/docs/index.rst` & `tendril-utils-www-0.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/docs/Makefile` & `tendril-utils-www-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/docs/installation.rst` & `tendril-utils-www-0.2.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/tests/test_bare.py` & `tendril-utils-www-0.2.3/tests/test_bare.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/tests/test_redirectcache.py` & `tendril-utils-www-0.2.3/tests/test_redirectcache.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/tests/coveralls.py` & `tendril-utils-www-0.2.3/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.2/LICENSE` & `tendril-utils-www-0.2.3/LICENSE`

 * *Files identical despite different names*

