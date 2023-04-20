# Comparing `tmp/gwosc-0.7.0.tar.gz` & `tmp/gwosc-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwosc-0.7.0.tar", last modified: Mon Apr 10 14:32:53 2023, max compression
+gzip compressed data, was "gwosc-0.7.1.tar", last modified: Thu Apr 20 11:17:38 2023, max compression
```

## Comparing `gwosc-0.7.0.tar` & `gwosc-0.7.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.995620 gwosc-0.7.0/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1054 2022-10-21 10:12:50.000000 gwosc-0.7.0/.appveyor.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      407 2022-10-21 10:12:50.000000 gwosc-0.7.0/.flake8
--rw-r--r--   0 duncan    (1000) duncan    (1000)      474 2022-05-16 13:55:13.000000 gwosc-0.7.0/.gitignore
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.945620 gwosc-0.7.0/.gitlab/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.965620 gwosc-0.7.0/.gitlab/ci/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1105 2023-03-21 17:33:53.000000 gwosc-0.7.0/.gitlab/ci/analysis.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3605 2023-04-10 14:14:53.000000 gwosc-0.7.0/.gitlab/ci/debian.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      624 2022-10-21 10:12:50.000000 gwosc-0.7.0/.gitlab/ci/dist.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      729 2022-10-21 10:12:50.000000 gwosc-0.7.0/.gitlab/ci/docs.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1525 2023-04-10 13:21:39.000000 gwosc-0.7.0/.gitlab/ci/python.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3272 2022-10-21 10:12:50.000000 gwosc-0.7.0/.gitlab/ci/rhel.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1458 2022-10-21 10:12:50.000000 gwosc-0.7.0/.gitlab/ci/test.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      445 2022-10-21 10:12:50.000000 gwosc-0.7.0/.gitlab-ci.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)       44 2020-07-27 09:48:35.000000 gwosc-0.7.0/.pep8speaks.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1081 2020-07-27 09:48:35.000000 gwosc-0.7.0/LICENSE
--rw-r--r--   0 duncan    (1000) duncan    (1000)      112 2022-05-16 13:55:13.000000 gwosc-0.7.0/MANIFEST.in
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5931 2023-04-10 14:32:52.995620 gwosc-0.7.0/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4580 2022-10-21 10:12:50.000000 gwosc-0.7.0/README.md
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4899 2023-01-09 14:57:56.000000 gwosc-0.7.0/RELEASE.md
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.975620 gwosc-0.7.0/debian/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2929 2023-04-10 14:14:53.000000 gwosc-0.7.0/debian/changelog
--rw-r--r--   0 duncan    (1000) duncan    (1000)        2 2020-07-27 09:48:35.000000 gwosc-0.7.0/debian/compat
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1040 2022-10-21 10:12:50.000000 gwosc-0.7.0/debian/control
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1299 2020-07-27 09:48:35.000000 gwosc-0.7.0/debian/copyright
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)      284 2022-10-21 10:12:50.000000 gwosc-0.7.0/debian/rules
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.975620 gwosc-0.7.0/debian/source/
--rw-r--r--   0 duncan    (1000) duncan    (1000)       12 2020-07-27 09:48:35.000000 gwosc-0.7.0/debian/source/format
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.975620 gwosc-0.7.0/docs/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      605 2022-05-16 13:55:13.000000 gwosc-0.7.0/docs/Makefile
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.975620 gwosc-0.7.0/docs/_static/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      463 2020-07-27 09:48:35.000000 gwosc-0.7.0/docs/_static/gwosc.css
--rw-r--r--   0 duncan    (1000) duncan    (1000)      169 2021-10-13 10:04:46.000000 gwosc-0.7.0/docs/api.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3786 2022-05-16 13:55:13.000000 gwosc-0.7.0/docs/conf.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      238 2020-07-27 09:48:35.000000 gwosc-0.7.0/docs/datasets.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      533 2020-07-27 09:48:35.000000 gwosc-0.7.0/docs/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      211 2020-07-27 09:48:35.000000 gwosc-0.7.0/docs/locate.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      209 2020-07-27 09:48:35.000000 gwosc-0.7.0/docs/timeline.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.985620 gwosc-0.7.0/gwosc/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      371 2022-05-16 13:55:13.000000 gwosc-0.7.0/gwosc/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      160 2023-04-10 14:32:52.000000 gwosc-0.7.0/gwosc/_version.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    12698 2023-04-10 13:21:39.000000 gwosc-0.7.0/gwosc/api.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    16728 2023-03-21 17:33:53.000000 gwosc-0.7.0/gwosc/datasets.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7611 2023-01-09 14:57:42.000000 gwosc-0.7.0/gwosc/locate.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.995620 gwosc-0.7.0/gwosc/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      188 2022-05-16 13:55:13.000000 gwosc-0.7.0/gwosc/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1408 2022-05-16 13:55:13.000000 gwosc-0.7.0/gwosc/tests/conftest.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6498 2023-04-10 13:21:39.000000 gwosc-0.7.0/gwosc/tests/test_api.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7364 2023-03-21 17:33:53.000000 gwosc-0.7.0/gwosc/tests/test_datasets.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2403 2022-10-21 10:12:50.000000 gwosc-0.7.0/gwosc/tests/test_locate.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1361 2023-01-09 14:57:53.000000 gwosc-0.7.0/gwosc/tests/test_timeline.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1646 2022-05-16 13:55:13.000000 gwosc-0.7.0/gwosc/tests/test_urls.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1371 2022-05-16 13:55:13.000000 gwosc-0.7.0/gwosc/tests/test_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2429 2023-01-09 14:57:53.000000 gwosc-0.7.0/gwosc/timeline.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5236 2022-05-16 13:55:13.000000 gwosc-0.7.0/gwosc/urls.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2600 2022-05-16 13:55:13.000000 gwosc-0.7.0/gwosc/utils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-10 14:32:52.985620 gwosc-0.7.0/gwosc.egg-info/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5931 2023-04-10 14:32:52.000000 gwosc-0.7.0/gwosc.egg-info/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1022 2023-04-10 14:32:52.000000 gwosc-0.7.0/gwosc.egg-info/SOURCES.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-04-10 14:32:52.000000 gwosc-0.7.0/gwosc.egg-info/dependency_links.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      171 2023-04-10 14:32:52.000000 gwosc-0.7.0/gwosc.egg-info/requires.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        6 2023-04-10 14:32:52.000000 gwosc-0.7.0/gwosc.egg-info/top_level.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3837 2023-04-10 14:14:53.000000 gwosc-0.7.0/gwosc.spec
--rw-r--r--   0 duncan    (1000) duncan    (1000)      626 2022-10-21 10:12:50.000000 gwosc-0.7.0/pyproject.toml
--rw-r--r--   0 duncan    (1000) duncan    (1000)       61 2020-07-27 09:48:35.000000 gwosc-0.7.0/readthedocs.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1508 2023-04-10 14:32:52.995620 gwosc-0.7.0/setup.cfg
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)      192 2022-05-16 13:55:13.000000 gwosc-0.7.0/setup.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:17:38.379882 gwosc-0.7.1/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1054 2022-10-21 10:12:50.000000 gwosc-0.7.1/.appveyor.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      407 2022-10-21 10:12:50.000000 gwosc-0.7.1/.flake8
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      474 2022-05-16 13:55:13.000000 gwosc-0.7.1/.gitignore
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:17:38.109882 gwosc-0.7.1/.gitlab/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:17:38.359882 gwosc-0.7.1/.gitlab/ci/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1105 2023-03-21 17:33:53.000000 gwosc-0.7.1/.gitlab/ci/analysis.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3605 2023-04-10 14:14:53.000000 gwosc-0.7.1/.gitlab/ci/debian.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      624 2022-10-21 10:12:50.000000 gwosc-0.7.1/.gitlab/ci/dist.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      729 2022-10-21 10:12:50.000000 gwosc-0.7.1/.gitlab/ci/docs.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1525 2023-04-10 13:21:39.000000 gwosc-0.7.1/.gitlab/ci/python.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3272 2022-10-21 10:12:50.000000 gwosc-0.7.1/.gitlab/ci/rhel.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1458 2022-10-21 10:12:50.000000 gwosc-0.7.1/.gitlab/ci/test.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      445 2022-10-21 10:12:50.000000 gwosc-0.7.1/.gitlab-ci.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       44 2020-07-27 09:48:35.000000 gwosc-0.7.1/.pep8speaks.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1081 2020-07-27 09:48:35.000000 gwosc-0.7.1/LICENSE
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      112 2022-05-16 13:55:13.000000 gwosc-0.7.1/MANIFEST.in
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5796 2023-04-20 11:17:38.379882 gwosc-0.7.1/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4445 2023-04-20 11:16:38.000000 gwosc-0.7.1/README.md
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4899 2023-01-09 14:57:56.000000 gwosc-0.7.1/RELEASE.md
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:17:38.359882 gwosc-0.7.1/debian/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3068 2023-04-20 11:16:38.000000 gwosc-0.7.1/debian/changelog
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        2 2020-07-27 09:48:35.000000 gwosc-0.7.1/debian/compat
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1031 2023-04-20 11:16:38.000000 gwosc-0.7.1/debian/control
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1299 2020-07-27 09:48:35.000000 gwosc-0.7.1/debian/copyright
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)      284 2022-10-21 10:12:50.000000 gwosc-0.7.1/debian/rules
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:17:38.359882 gwosc-0.7.1/debian/source/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       12 2020-07-27 09:48:35.000000 gwosc-0.7.1/debian/source/format
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:17:38.369882 gwosc-0.7.1/docs/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      605 2022-05-16 13:55:13.000000 gwosc-0.7.1/docs/Makefile
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:17:38.369882 gwosc-0.7.1/docs/_static/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      463 2020-07-27 09:48:35.000000 gwosc-0.7.1/docs/_static/gwosc.css
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      169 2021-10-13 10:04:46.000000 gwosc-0.7.1/docs/api.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3786 2022-05-16 13:55:13.000000 gwosc-0.7.1/docs/conf.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      238 2020-07-27 09:48:35.000000 gwosc-0.7.1/docs/datasets.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      524 2023-04-20 11:16:38.000000 gwosc-0.7.1/docs/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      211 2020-07-27 09:48:35.000000 gwosc-0.7.1/docs/locate.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      209 2020-07-27 09:48:35.000000 gwosc-0.7.1/docs/timeline.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:17:38.369882 gwosc-0.7.1/gwosc/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      371 2022-05-16 13:55:13.000000 gwosc-0.7.1/gwosc/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      160 2023-04-20 11:17:37.000000 gwosc-0.7.1/gwosc/_version.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12740 2023-04-20 11:16:38.000000 gwosc-0.7.1/gwosc/api.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    16637 2023-04-20 11:16:38.000000 gwosc-0.7.1/gwosc/datasets.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7494 2023-04-20 11:16:38.000000 gwosc-0.7.1/gwosc/locate.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:17:38.379882 gwosc-0.7.1/gwosc/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      188 2022-05-16 13:55:13.000000 gwosc-0.7.1/gwosc/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1408 2022-05-16 13:55:13.000000 gwosc-0.7.1/gwosc/tests/conftest.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6472 2023-04-20 11:16:38.000000 gwosc-0.7.1/gwosc/tests/test_api.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7364 2023-03-21 17:33:53.000000 gwosc-0.7.1/gwosc/tests/test_datasets.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2403 2022-10-21 10:12:50.000000 gwosc-0.7.1/gwosc/tests/test_locate.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1361 2023-01-09 14:57:53.000000 gwosc-0.7.1/gwosc/tests/test_timeline.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1646 2022-05-16 13:55:13.000000 gwosc-0.7.1/gwosc/tests/test_urls.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1371 2022-05-16 13:55:13.000000 gwosc-0.7.1/gwosc/tests/test_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2420 2023-04-20 11:16:38.000000 gwosc-0.7.1/gwosc/timeline.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5236 2022-05-16 13:55:13.000000 gwosc-0.7.1/gwosc/urls.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2600 2022-05-16 13:55:13.000000 gwosc-0.7.1/gwosc/utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-20 11:17:38.379882 gwosc-0.7.1/gwosc.egg-info/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5796 2023-04-20 11:17:37.000000 gwosc-0.7.1/gwosc.egg-info/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1022 2023-04-20 11:17:38.000000 gwosc-0.7.1/gwosc.egg-info/SOURCES.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-04-20 11:17:37.000000 gwosc-0.7.1/gwosc.egg-info/dependency_links.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      171 2023-04-20 11:17:37.000000 gwosc-0.7.1/gwosc.egg-info/requires.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        6 2023-04-20 11:17:37.000000 gwosc-0.7.1/gwosc.egg-info/top_level.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3907 2023-04-20 11:16:38.000000 gwosc-0.7.1/gwosc.spec
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      626 2022-10-21 10:12:50.000000 gwosc-0.7.1/pyproject.toml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       61 2020-07-27 09:48:35.000000 gwosc-0.7.1/readthedocs.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1508 2023-04-20 11:17:38.379882 gwosc-0.7.1/setup.cfg
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)      192 2022-05-16 13:55:13.000000 gwosc-0.7.1/setup.py
```

### Comparing `gwosc-0.7.0/.appveyor.yml` & `gwosc-0.7.1/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/.gitlab/ci/analysis.yml` & `gwosc-0.7.1/.gitlab/ci/analysis.yml`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/.gitlab/ci/debian.yml` & `gwosc-0.7.1/.gitlab/ci/debian.yml`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/.gitlab/ci/dist.yml` & `gwosc-0.7.1/.gitlab/ci/dist.yml`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/.gitlab/ci/docs.yml` & `gwosc-0.7.1/.gitlab/ci/docs.yml`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/.gitlab/ci/python.yml` & `gwosc-0.7.1/.gitlab/ci/python.yml`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/.gitlab/ci/rhel.yml` & `gwosc-0.7.1/.gitlab/ci/rhel.yml`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/.gitlab/ci/test.yml` & `gwosc-0.7.1/.gitlab/ci/test.yml`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/LICENSE` & `gwosc-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/PKG-INFO` & `gwosc-0.7.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwosc
-Version: 0.7.0
+Version: 0.7.1
 Summary: A python interface to the GW Open Science data archive
 Home-page: https://git.ligo.org/gwosc/client/
 Download-URL: https://pypi.org/project/gwosc/
 Author: Duncan Macleod
 Author-email: duncan.macleod@ligo.org
 License: MIT
 Project-URL: Bug Tracker, https://git.ligo.org/gwosc/client/-/issues
@@ -31,15 +31,15 @@
 Provides-Extra: docs
 Provides-Extra: lint
 License-File: LICENSE
 
 # `gwosc` client API
 
 The `gwosc` package provides an interface to querying the open data
-releases hosted on <https://gw-openscience.org> from the GEO, LIGO,
+releases hosted on <https://gwosc.org> from the GEO, LIGO,
 and Virgo gravitational-wave observatories.
 
 ## Release status
 
 [![PyPI version](https://badge.fury.io/py/gwosc.svg)](http://badge.fury.io/py/gwosc)
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/gwosc.svg)](https://anaconda.org/conda-forge/gwosc/)  
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1196306.svg)](https://doi.org/10.5281/zenodo.1196306)
@@ -97,33 +97,33 @@
 ## Locating data URLs by event name
 
 You can search for remote data URLS based on the event name:
 
 ```python
 >>> from gwosc.locate import get_event_urls
 >>> get_event_urls('GW150914')
-['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126257415-4096.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126257415-4096.hdf5']
+['https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126257415-4096.hdf5', 'https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126257415-4096.hdf5']
 ```
 
 You can down-select the URLs using keyword arguments:
 
 ```python
 >>> get_event_urls('GW150914', detector='L1', duration=32)
-['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5']
+['https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5']
 ```
 
 ## Locating data URLs by GPS interval
 
 You can search for remote data URLs based on the GPS time interval as
 follows:
 
 ```python
 >>> from gwosc.locate import get_urls
 >>> get_urls('L1', 968650000, 968660000)
-['https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968646656-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968650752-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968654848-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968658944-4096.hdf5']
+['https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968646656-4096.hdf5', 'https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968650752-4096.hdf5', 'https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968654848-4096.hdf5', 'https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968658944-4096.hdf5']
 ```
 
 This arguments for this function are as follows
 
 -   `detector` : the prefix of the relevant gravitational-wave
     interferometer, either `'H1'` for LIGO-Hanford, or `'L1'` for LIGO
     Livingston,
@@ -149,10 +149,10 @@
 [(1126073529, 1126114861), (1126121462, 1126123267), (1126123553, 1126126832), (1126139205, 1126139266), (1126149058, 1126151217)]
 ```
 
 The output is a `list` of `(start, end)` 2-tuples which each represent a
 semi-open time interval.
 
 For documentation on what flags are available, for example for the O1
-science run, see [the O1 data release page](https://gw-openscience.org/O1/)
+science run, see [the O1 data release page](https://gwosc.org/O1/)
 (*Data Quality*).
```

### Comparing `gwosc-0.7.0/README.md` & `gwosc-0.7.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # `gwosc` client API
 
 The `gwosc` package provides an interface to querying the open data
-releases hosted on <https://gw-openscience.org> from the GEO, LIGO,
+releases hosted on <https://gwosc.org> from the GEO, LIGO,
 and Virgo gravitational-wave observatories.
 
 ## Release status
 
 [![PyPI version](https://badge.fury.io/py/gwosc.svg)](http://badge.fury.io/py/gwosc)
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/gwosc.svg)](https://anaconda.org/conda-forge/gwosc/)  
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1196306.svg)](https://doi.org/10.5281/zenodo.1196306)
@@ -63,33 +63,33 @@
 ## Locating data URLs by event name
 
 You can search for remote data URLS based on the event name:
 
 ```python
 >>> from gwosc.locate import get_event_urls
 >>> get_event_urls('GW150914')
-['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126257415-4096.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126257415-4096.hdf5']
+['https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126257415-4096.hdf5', 'https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126257415-4096.hdf5']
 ```
 
 You can down-select the URLs using keyword arguments:
 
 ```python
 >>> get_event_urls('GW150914', detector='L1', duration=32)
-['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5']
+['https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5']
 ```
 
 ## Locating data URLs by GPS interval
 
 You can search for remote data URLs based on the GPS time interval as
 follows:
 
 ```python
 >>> from gwosc.locate import get_urls
 >>> get_urls('L1', 968650000, 968660000)
-['https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968646656-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968650752-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968654848-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968658944-4096.hdf5']
+['https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968646656-4096.hdf5', 'https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968650752-4096.hdf5', 'https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968654848-4096.hdf5', 'https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968658944-4096.hdf5']
 ```
 
 This arguments for this function are as follows
 
 -   `detector` : the prefix of the relevant gravitational-wave
     interferometer, either `'H1'` for LIGO-Hanford, or `'L1'` for LIGO
     Livingston,
@@ -115,10 +115,10 @@
 [(1126073529, 1126114861), (1126121462, 1126123267), (1126123553, 1126126832), (1126139205, 1126139266), (1126149058, 1126151217)]
 ```
 
 The output is a `list` of `(start, end)` 2-tuples which each represent a
 semi-open time interval.
 
 For documentation on what flags are available, for example for the O1
-science run, see [the O1 data release page](https://gw-openscience.org/O1/)
+science run, see [the O1 data release page](https://gwosc.org/O1/)
 (*Data Quality*).
```

### Comparing `gwosc-0.7.0/RELEASE.md` & `gwosc-0.7.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/debian/changelog` & `gwosc-0.7.1/debian/changelog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+gwosc (0.7.1-1) unstable; urgency=low
+
+  * update to 0.7.1
+
+ -- Duncan Macleod <duncan.macleod@ligo.org>  Thu, 20 Apr 2023 10:30:00 +0100
+
 gwosc (0.7.0-1) unstable; urgency=low
 
   * update to 0.7.0
 
  -- Duncan Macleod <duncan.macleod@ligo.org>  Mon, 10 Apr 2023 14:23:00 +0100
 
 gwosc (0.6.1-1) unstable; urgency=low
```

### Comparing `gwosc-0.7.0/debian/control` & `gwosc-0.7.1/debian/control`

 * *Files 3% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 Architecture: all
 Depends:
   ${misc:Depends},
   ${python3:Depends},
   python3-requests,
 Description: Python interface to the Gravitational-Wave Open Science Center data archive
  The `gwosc` package provides an interface to querying the open data
- releases hosted on <https://gw-openscience.org> from the GEO, LIGO,
+ releases hosted on <https://gwosc.org> from the GEO, LIGO,
  and Virgo gravitational-wave observatories.
```

### Comparing `gwosc-0.7.0/debian/copyright` & `gwosc-0.7.1/debian/copyright`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/docs/Makefile` & `gwosc-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/docs/conf.py` & `gwosc-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/docs/index.rst` & `gwosc-0.7.1/docs/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 =======
  GWOSC
 =======
 
 A python interface to the
-`Gravitational-Wave Open Science Center <https://gw-openscience.org>`_ archive.
+`Gravitational-Wave Open Science Center <https://gwosc.org>`_ archive.
 
 Installation
 ------------
 
 ``gwosc`` can be installed via `pip <https://pip.pypa.io>`_:
 
 .. code-block:: shell
```

### Comparing `gwosc-0.7.0/gwosc/api.py` & `gwosc-0.7.1/gwosc/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 that handle direct requests to the GWOSC host.
 """
 
 import logging
 import os
 import re
 from urllib.parse import urlencode
+from . import __version__
 
 import requests
 
 logger = logging.getLogger("gwosc.api")
 _loghandler = logging.StreamHandler()
 _loghandler.setFormatter(
     logging.Formatter(logging.BASIC_FORMAT),
 )
 logger.addHandler(_loghandler)
 logger.setLevel(int(os.getenv("GWOSC_LOG_LEVEL", logging.NOTSET)))
 
 _MAX_GPS = 99999999999
 
 #: The default GWOSC host URL
-DEFAULT_URL = "https://www.gw-openscience.org"
+DEFAULT_URL = "https://gwosc.org"
 
 #: Cache of downloaded blobs
 JSON_CACHE = {}
 
 _ALLOWED_OPS = set((">=", "=>", "<=", "=<"))
 
 # -- JSON handling ------------------------------------------------------------
@@ -57,15 +58,16 @@
     json.loads
         for details of the JSON parsing
     """
     try:
         return JSON_CACHE[url]
     except KeyError:
         logger.debug("fetching {}".format(url))
-        resp = requests.get(url, **kwargs)
+        client_headers = {"User-Agent": f"python-gwosc/{__version__}"}
+        resp = requests.get(url, headers=client_headers, **kwargs)
         resp.raise_for_status()
         return JSON_CACHE.setdefault(
             url,
             resp.json(),
         )
 
 
@@ -84,15 +86,15 @@
         the GPS start of the desired interval
 
     gpsend : `int`
         the GPS end of the desired interval
 
     host : `str`, optional
         the URL of the GWOSC host to query, defaults to
-        https://www.gw-openscience.org
+        https://gwosc.org
 
     Returns
     -------
     data : `dict` or `list`
         the JSON data retrieved from GWOSC and returned by `json.loads`
     """
     return fetch_json(_dataset_url(gpsstart, gpsend, host=host))
@@ -120,15 +122,15 @@
         the GPS start of the desired interval
 
     gpsend : `int`
         the GPS end of the desired interval
 
     host : `str`, optional
         the URL of the GWOSC host to query, defaults to
-        https://www.gw-openscience.org
+        https://gwosc.org
 
     Returns
     -------
     data : `dict` or `list`
         the JSON data retrieved from GWOSC and returned by `json.loads`
     """
     return fetch_json(_run_url(run, detector, gpsstart, gpsend, host=host))
@@ -176,15 +178,15 @@
     Parameters
     ----------
     catalog : `str`
         the name of the event catalog, e.g. `GWTC-1-confident`
 
     host : `str`, optional
         the URL of the GWOSC host to query, defaults to
-        https://www.gw-openscience.org
+        https://gwosc.org
 
     Returns
     -------
     data : `dict` or `list`
         the JSON data retrieved from GWOSC and returnend by
         :meth:`requests.Response.json`
     """
@@ -203,15 +205,15 @@
 
 def fetch_allevents_json(full=False, host=DEFAULT_URL):
     """"Returns the JSON metadata for the allevents API
 
     Parameters
     ----------
     host : `str`, optional
-        the URL of the GWOSC host to query, defaults to gw-openscience.org
+        the URL of the GWOSC host to query, defaults to https://gwosc.org
 
     Returns
     -------
     data : `dict` or `list`
         the JSON data retrieved from GWOSC and returned by
         :meth:`requests.Response.json`
     """
@@ -376,15 +378,15 @@
     ----------
     select : `list-like`
         a list of range constrains for the events.
         All ranges should have inclusive ends (<= and >= operators).
 
     host : `str`, optional
         the URL of the GWOSC host to query, defaults to
-        https://www.gw-openscience.org
+        https://gwosc.org
 
     Returns
     -------
     data : `dict` or `list`
         the JSON data retrieved from GWOSC and returnend by
         :meth:`requests.Response.json`
 
@@ -437,15 +439,15 @@
         name of catalogue that hosts this event
 
     version : `int`, `None`, optional
         restrict query to a given data-release version
 
     host : `str`, optional
         the URL of the GWOSC host to query, defaults to
-        https://www.gw-openscience.org
+        https://gwosc.org
 
     Returns
     -------
     data : `dict` or `list`
         the JSON data retrieved from GWOSC and returned by `json.loads`
     """
     return fetch_json(
```

### Comparing `gwosc-0.7.0/gwosc/datasets.py` & `gwosc-0.7.1/gwosc/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         not used to filter catalogs
 
     match : `str`, optional
         regular expression string against which to match datasets
 
     host : `str`, optional
         the URL of the GWOSC host to query, defaults to
-        https://www.gw-openscience.org
+        https://gwosc.org
 
     Returns
     -------
     datasets : `list` of `str`
         the names of all matched datasets, possibly empty
 
     Examples
@@ -319,15 +319,15 @@
 
     version : `int`, `None`, optional
         the version of the data release to use,
         defaults to the highest available version
 
     host : `str`, optional
         the URL of the GWOSC host to query, defaults to
-        https://www.gw-openscience.org
+        https://gwosc.org
 
     Returns
     -------
     gps : `float`
         the GPS time of this event
 
     Examples
@@ -369,15 +369,15 @@
 
     version : `int`, `None`, optional
         the version of the data release to use,
         defaults to the highest available version
 
     host : `str`, optional
         the URL of the GWOSC host to query, defaults to
-        https://www.gw-openscience.org
+        https://gwosc.org
 
     Returns
     -------
     start, end : `int`
         the GPS ``[start, end)`` interval covered by this run dataset
 
     Examples
@@ -413,15 +413,15 @@
     Parameters
     ----------
     gps : `float`
         The GPS time to locate
 
     host : `str`, optional
         the URL of the GWOSC host to query, defaults to
-        https://www.gw-openscience.org
+        https://gwosc.org
 
     tol : `float`, optional
         the search window (in seconds), default: ``1``
 
     Returns
     -------
     event : `str`
@@ -454,15 +454,15 @@
     Parameters
     ----------
     event : `str`
         the name of the event to query
 
     host : `str`, optional
         the URL of the GWOSC host to query, defaults to
-        https://www.gw-openscience.org
+        https://gwosc.org
 
     version : `int`, `None`, optional
         the version of the data release to use,
         defaults to the highest available version
 
     Returns
     -------
@@ -494,15 +494,15 @@
     Parameters
     ----------
     run : `str`
         the name of the run dataset to query
 
     host : `str`, optional
         the URL of the GWOSC host to query, defaults to
-        https://www.gw-openscience.org
+        https://gwosc.org
 
     Returns
     -------
     start, end : `int`
         the GPS ``[start, end)`` interval covered by this run dataset
 
     Examples
@@ -529,15 +529,15 @@
     Parameters
     ----------
     gps : `float`
         The GPS time to locate
 
     host : `str`, optional
         the URL of the GWOSC host to query, defaults to
-        https://www.gw-openscience.org
+        https://gwosc.org
 
     Returns
     -------
     run : `str`
         the name of the matched observing run
 
     Raises
```

### Comparing `gwosc-0.7.0/gwosc/locate.py` & `gwosc-0.7.1/gwosc/locate.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 `gwosc.locate` provides functions to determine the file URLs containing
 data for a specific dataset.
 
 You can search for remote data URLS based on the event name:
 
 >>> from gwosc.locate import get_event_urls
 >>> get_event_urls('GW150914')
-['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126259447-32.hdf5',
- 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126257415-4096.hdf5',
- 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5',
- 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126257415-4096.hdf5']
+['https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126259447-32.hdf5',
+ 'https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126257415-4096.hdf5',
+ 'https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5',
+ 'https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126257415-4096.hdf5']
 
 You can down-select the URLs using keyword arguments:
 
 >>> get_event_urls('GW150914', detector='L1', duration=32)
-['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5']
+['https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5']
 
 You can search for remote data URLs based on the GPS time interval as
 follows:
 
 >>> from gwosc.locate import get_urls
 >>> get_urls('L1', 968650000, 968660000)
-['https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968646656-4096.hdf5',
- 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968650752-4096.hdf5',
- 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968654848-4096.hdf5',
- 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968658944-4096.hdf5']
+['https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968646656-4096.hdf5',
+ 'https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968650752-4096.hdf5',
+ 'https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968654848-4096.hdf5',
+ 'https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968658944-4096.hdf5']
 
 By default, this method will return the paths to HDF5 files for the 4 kHz
 sample-rate data, these can be specified as keyword arguments.
 For full information, see :func:`get_urls`.
 """  # noqa: E501
 
 from . import (
```

### Comparing `gwosc-0.7.0/gwosc/tests/conftest.py` & `gwosc-0.7.1/gwosc/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/gwosc/tests/test_api.py` & `gwosc-0.7.1/gwosc/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,26 @@
     for urld in urllist:
         for key in keys:
             assert key in urld
 
 
 @pytest.mark.remote
 def test_fetch_json():
-    url = 'https://www.gw-openscience.org/archive/1126257414/1126261510/json/'
+    url = 'https://gwosc.org/archive/1126257414/1126261510/json/'
     out = api.fetch_json(url)
     assert isinstance(out, dict)
     assert len(out['events']) == 3
     assert sorted(out['events']['GW150914-v1']['detectors']) == ['H1', 'L1']
     assert {'O1', 'O1_16KHZ', 'history'}.issubset(set(out['runs']))
 
 
 @pytest.mark.remote
 def test_fetch_json_error():
     # check errors (use legit URL that isn't JSON)
-    url = 'https://www.gw-openscience.org/archive/1126257414/1126261510/'
+    url = 'https://gwosc.org/archive/1126257414/1126261510/'
     with pytest.raises((RequestException, ValueError)):
         api.fetch_json(url)
 
 
 def test_fetch_json_local(requests_mock):
     url = 'http://anything'
     requests_mock.get(
```

### Comparing `gwosc-0.7.0/gwosc/tests/test_datasets.py` & `gwosc-0.7.1/gwosc/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/gwosc/tests/test_locate.py` & `gwosc-0.7.1/gwosc/tests/test_locate.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/gwosc/tests/test_timeline.py` & `gwosc-0.7.1/gwosc/tests/test_timeline.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/gwosc/tests/test_urls.py` & `gwosc-0.7.1/gwosc/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/gwosc/tests/test_utils.py` & `gwosc-0.7.1/gwosc/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/gwosc/timeline.py` & `gwosc-0.7.1/gwosc/timeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [(1126073529, 1126114861), (1126121462, 1126123267), (1126123553, 1126126832), (1126139205, 1126139266), (1126149058, 1126151217)]
 
 The output is a `list` of ``[start, end)`` 2-tuples which each
 represent a semi-open time interval.
 
 For documentation on what flags are available, for example for the O1
 science run, see `the O1 data release
-page <https://gw-openscience.org/O1/>`__ (*Data Quality*).
+page <https://gwosc.org/O1/>`__ (*Data Quality*).
 """  # noqa: E501
 
 from operator import itemgetter
 
 from . import (api, datasets)
```

### Comparing `gwosc-0.7.0/gwosc/urls.py` & `gwosc-0.7.1/gwosc/urls.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/gwosc/utils.py` & `gwosc-0.7.1/gwosc/utils.py`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/gwosc.egg-info/PKG-INFO` & `gwosc-0.7.1/gwosc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwosc
-Version: 0.7.0
+Version: 0.7.1
 Summary: A python interface to the GW Open Science data archive
 Home-page: https://git.ligo.org/gwosc/client/
 Download-URL: https://pypi.org/project/gwosc/
 Author: Duncan Macleod
 Author-email: duncan.macleod@ligo.org
 License: MIT
 Project-URL: Bug Tracker, https://git.ligo.org/gwosc/client/-/issues
@@ -31,15 +31,15 @@
 Provides-Extra: docs
 Provides-Extra: lint
 License-File: LICENSE
 
 # `gwosc` client API
 
 The `gwosc` package provides an interface to querying the open data
-releases hosted on <https://gw-openscience.org> from the GEO, LIGO,
+releases hosted on <https://gwosc.org> from the GEO, LIGO,
 and Virgo gravitational-wave observatories.
 
 ## Release status
 
 [![PyPI version](https://badge.fury.io/py/gwosc.svg)](http://badge.fury.io/py/gwosc)
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/gwosc.svg)](https://anaconda.org/conda-forge/gwosc/)  
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1196306.svg)](https://doi.org/10.5281/zenodo.1196306)
@@ -97,33 +97,33 @@
 ## Locating data URLs by event name
 
 You can search for remote data URLS based on the event name:
 
 ```python
 >>> from gwosc.locate import get_event_urls
 >>> get_event_urls('GW150914')
-['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126257415-4096.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126257415-4096.hdf5']
+['https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/H-H1_GWOSC_4KHZ_R1-1126257415-4096.hdf5', 'https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5', 'https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126257415-4096.hdf5']
 ```
 
 You can down-select the URLs using keyword arguments:
 
 ```python
 >>> get_event_urls('GW150914', detector='L1', duration=32)
-['https://www.gw-openscience.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5']
+['https://gwosc.org/eventapi/json/GWTC-1-confident/GW150914/v3/L-L1_GWOSC_4KHZ_R1-1126259447-32.hdf5']
 ```
 
 ## Locating data URLs by GPS interval
 
 You can search for remote data URLs based on the GPS time interval as
 follows:
 
 ```python
 >>> from gwosc.locate import get_urls
 >>> get_urls('L1', 968650000, 968660000)
-['https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968646656-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968650752-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968654848-4096.hdf5', 'https://www.gw-openscience.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968658944-4096.hdf5']
+['https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968646656-4096.hdf5', 'https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968650752-4096.hdf5', 'https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968654848-4096.hdf5', 'https://gwosc.org/archive/data/S6/967835648/L-L1_LOSC_4_V1-968658944-4096.hdf5']
 ```
 
 This arguments for this function are as follows
 
 -   `detector` : the prefix of the relevant gravitational-wave
     interferometer, either `'H1'` for LIGO-Hanford, or `'L1'` for LIGO
     Livingston,
@@ -149,10 +149,10 @@
 [(1126073529, 1126114861), (1126121462, 1126123267), (1126123553, 1126126832), (1126139205, 1126139266), (1126149058, 1126151217)]
 ```
 
 The output is a `list` of `(start, end)` 2-tuples which each represent a
 semi-open time interval.
 
 For documentation on what flags are available, for example for the O1
-science run, see [the O1 data release page](https://gw-openscience.org/O1/)
+science run, see [the O1 data release page](https://gwosc.org/O1/)
 (*Data Quality*).
```

### Comparing `gwosc-0.7.0/gwosc.egg-info/SOURCES.txt` & `gwosc-0.7.1/gwosc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/gwosc.spec` & `gwosc-0.7.1/gwosc.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 %define name    gwosc
-%define version 0.7.0
+%define version 0.7.1
 %define release 1
 
 Name:      %{name}
 Version:   %{version}
 Release:   %{release}%{?dist}
 Summary:   A python interface to the Gravitational-Wave Open Science Center data archive
 
@@ -34,26 +34,26 @@
 %if 0%{?rhel} == 0 || 0%{?rhel} >= 8
 BuildRequires: python%{python3_pkgversion}-pytest
 BuildRequires: python%{python3_pkgversion}-requests-mock >= 1.5.0
 %endif
 
 %description
 The `gwosc` package provides an interface to querying the open data
-releases hosted on <https://gw-openscience.org> from the GEO, LIGO,
+releases hosted on <https://gwosc.org> from the GEO, LIGO,
 and Virgo gravitational-wave observatories.
 
 # -- python-3X-gwosc
 
 %package -n python%{python3_pkgversion}-%{name}
 Summary:  %{summary}
 Requires: python%{python3_pkgversion}-requests >= 1.0.0
 %{?python_provide:%python_provide python%{python3_pkgversion}-%{name}}
 %description -n python%{python3_pkgversion}-%{name}
 The `gwosc` package provides an interface to querying the open data
-releases hosted on <https://gw-openscience.org> from the GEO, LIGO,
+releases hosted on <https://gwosc.org> from the GEO, LIGO,
 and Virgo gravitational-wave observatories.
 
 # -- build steps
 
 %prep
 %autosetup -n %{name}-%{version}
 
@@ -75,14 +75,17 @@
 %license LICENSE
 %doc README.md
 %{python3_sitelib}/*
 
 # -- changelog
 
 %changelog
+* Thu Apr 20 2023 Duncan Macleod <duncan.macleod@ligo.org> - 0.7.1-1
+- update to 0.7.1
+
 * Mon Apr 10 2023 Duncan Macleod <duncan.macleod@ligo.org> - 0.7.0-1
 - update to 0.7.0
 
 * Thu Aug 12 2021 Duncan Macleod <duncan.macleod@ligo.org> - 0.6.1-1
 - update to 0.6.1
 
 * Mon Aug 09 2021 Duncan Macleod <duncan.macleod@ligo.org> - 0.6.0-1
```

### Comparing `gwosc-0.7.0/pyproject.toml` & `gwosc-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gwosc-0.7.0/setup.cfg` & `gwosc-0.7.1/setup.cfg`

 * *Files identical despite different names*

