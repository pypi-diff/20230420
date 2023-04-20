# Comparing `tmp/gitberg-0.8.2.tar.gz` & `tmp/gitberg-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitberg-0.8.2.tar", last modified: Thu Dec  8 03:34:21 2022, max compression
+gzip compressed data, was "gitberg-0.8.3.tar", last modified: Thu Apr 20 17:16:11 2023, max compression
```

## Comparing `gitberg-0.8.2.tar` & `gitberg-0.8.3.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.974943 gitberg-0.8.2/
--rw-r--r--   0 eric       (501) staff       (20)      413 2016-03-08 17:03:43.000000 gitberg-0.8.2/CONTRIBUTING.rst
--rw-r--r--   0 eric       (501) staff       (20)     6298 2022-12-08 03:31:08.000000 gitberg-0.8.2/HISTORY.rst
--rw-r--r--   0 eric       (501) staff       (20)    35065 2016-02-05 20:21:16.000000 gitberg-0.8.2/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      126 2016-03-12 19:39:51.000000 gitberg-0.8.2/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)    35647 2022-12-08 03:34:21.975098 gitberg-0.8.2/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     2463 2022-09-26 22:28:56.000000 gitberg-0.8.2/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.924224 gitberg-0.8.2/bin/
--rwxr-xr-x   0 eric       (501) staff       (20)     5744 2022-09-26 22:28:56.000000 gitberg-0.8.2/bin/gitberg
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.925113 gitberg-0.8.2/gitberg.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)    35647 2022-12-08 03:34:21.000000 gitberg-0.8.2/gitberg.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     6739 2022-12-08 03:34:21.000000 gitberg-0.8.2/gitberg.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2022-12-08 03:34:21.000000 gitberg-0.8.2/gitberg.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)      294 2022-12-08 03:34:21.000000 gitberg-0.8.2/gitberg.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       10 2022-12-08 03:34:21.000000 gitberg-0.8.2/gitberg.egg-info/top_level.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.931171 gitberg-0.8.2/gitenberg/
--rw-r--r--   0 eric       (501) staff       (20)    10244 2022-11-15 16:34:52.000000 gitberg-0.8.2/gitenberg/.DS_Store
--rw-r--r--   0 eric       (501) staff       (20)      418 2022-12-08 03:30:49.000000 gitberg-0.8.2/gitenberg/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      717 2019-08-16 13:25:41.000000 gitberg-0.8.2/gitenberg/__init__.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.937707 gitberg-0.8.2/gitenberg/__pycache__/
--rw-r--r--   0 eric       (501) staff       (20)      591 2020-01-02 18:44:43.000000 gitberg-0.8.2/gitenberg/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)      599 2022-09-03 19:19:32.000000 gitberg-0.8.2/gitenberg/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2496 2022-09-03 19:19:34.000000 gitberg-0.8.2/gitenberg/__pycache__/actions.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     9466 2020-01-02 18:44:43.000000 gitberg-0.8.2/gitenberg/__pycache__/book.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     9620 2022-09-03 19:19:32.000000 gitberg-0.8.2/gitenberg/__pycache__/book.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2510 2020-01-02 18:44:44.000000 gitberg-0.8.2/gitenberg/__pycache__/clone.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2545 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/__pycache__/clone.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3446 2020-01-02 18:44:44.000000 gitberg-0.8.2/gitenberg/__pycache__/config.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3565 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2388 2020-01-02 18:44:44.000000 gitberg-0.8.2/gitenberg/__pycache__/dialog.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2651 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/__pycache__/dialog.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1127 2020-01-02 18:44:44.000000 gitberg-0.8.2/gitenberg/__pycache__/fetch.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1153 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/__pycache__/fetch.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1704 2022-09-03 19:19:34.000000 gitberg-0.8.2/gitenberg/__pycache__/library.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3812 2020-01-02 18:44:44.000000 gitberg-0.8.2/gitenberg/__pycache__/local_repo.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3812 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/__pycache__/local_repo.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2393 2020-01-02 18:44:44.000000 gitberg-0.8.2/gitenberg/__pycache__/make.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2449 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/__pycache__/make.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)      260 2020-01-02 18:44:44.000000 gitberg-0.8.2/gitenberg/__pycache__/parameters.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)      268 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/__pycache__/parameters.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2202 2020-01-02 18:44:44.000000 gitberg-0.8.2/gitenberg/__pycache__/pg_wikipedia.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2339 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/__pycache__/pg_wikipedia.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     5456 2020-01-02 18:44:44.000000 gitberg-0.8.2/gitenberg/__pycache__/push.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     4585 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/__pycache__/push.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3550 2022-09-03 19:19:34.000000 gitberg-0.8.2/gitenberg/__pycache__/workflow.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2608 2018-10-23 16:38:04.000000 gitberg-0.8.2/gitenberg/actions.py
--rw-r--r--   0 eric       (501) staff       (20)     3374 2018-10-23 16:40:03.000000 gitberg-0.8.2/gitenberg/actions.pyc
--rw-r--r--   0 eric       (501) staff       (20)    12687 2022-09-26 22:28:56.000000 gitberg-0.8.2/gitenberg/book.py
--rw-r--r--   0 eric       (501) staff       (20)    12013 2020-01-06 13:39:38.000000 gitberg-0.8.2/gitenberg/book.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2205 2018-09-15 18:38:44.000000 gitberg-0.8.2/gitenberg/clone.py
--rw-r--r--   0 eric       (501) staff       (20)     3139 2018-09-15 18:38:50.000000 gitberg-0.8.2/gitenberg/clone.pyc
--rwxr-xr-x   0 eric       (501) staff       (20)     3328 2022-09-26 22:28:56.000000 gitberg-0.8.2/gitenberg/config.py
--rw-r--r--   0 eric       (501) staff       (20)     4413 2020-01-06 13:39:38.000000 gitberg-0.8.2/gitenberg/config.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.953831 gitberg-0.8.2/gitenberg/data/
--rw-r--r--   0 eric       (501) staff       (20)     6148 2018-10-03 17:58:06.000000 gitberg-0.8.2/gitenberg/data/.DS_Store
--rw-r--r--   0 eric       (501) staff       (20)  3818651 2022-11-16 14:55:01.000000 gitberg-0.8.2/gitenberg/data/GITenberg_repo_list.tsv
--rw-r--r--   0 eric       (501) staff       (20)  1815872 2017-03-29 18:11:05.000000 gitberg-0.8.2/gitenberg/data/gutenberg_descriptions.json
--rw-r--r--   0 eric       (501) staff       (20)    57617 2022-09-26 22:31:30.000000 gitberg-0.8.2/gitenberg/data/missing.tsv
--rw-r--r--   0 eric       (501) staff       (20)       17 2020-01-18 01:02:06.000000 gitberg-0.8.2/gitenberg/data/removed.txt
--rw-r--r--   0 eric       (501) staff       (20)     2265 2020-03-24 17:09:28.000000 gitberg-0.8.2/gitenberg/dialog.py
--rw-r--r--   0 eric       (501) staff       (20)     2963 2018-05-14 18:18:37.000000 gitberg-0.8.2/gitenberg/dialog.pyc
--rw-r--r--   0 eric       (501) staff       (20)      681 2018-10-03 19:32:10.000000 gitberg-0.8.2/gitenberg/fetch.py
--rw-r--r--   0 eric       (501) staff       (20)     1365 2018-10-03 21:25:03.000000 gitberg-0.8.2/gitenberg/fetch.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.954432 gitberg-0.8.2/gitenberg/gitenberg/
--rw-r--r--   0 eric       (501) staff       (20)      243 2017-03-29 18:13:43.000000 gitberg-0.8.2/gitenberg/gitenberg/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      373 2017-11-09 21:09:26.000000 gitberg-0.8.2/gitenberg/gitenberg/__init__.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1197 2019-01-01 22:05:08.000000 gitberg-0.8.2/gitenberg/library.py
--rw-r--r--   0 eric       (501) staff       (20)     2062 2019-01-01 23:27:51.000000 gitberg-0.8.2/gitenberg/library.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3093 2020-01-02 22:45:38.000000 gitberg-0.8.2/gitenberg/local_repo.py
--rw-r--r--   0 eric       (501) staff       (20)     4380 2020-01-02 22:46:15.000000 gitberg-0.8.2/gitenberg/local_repo.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2243 2018-10-20 18:41:52.000000 gitberg-0.8.2/gitenberg/make.py
--rw-r--r--   0 eric       (501) staff       (20)     2966 2018-10-20 18:42:53.000000 gitberg-0.8.2/gitenberg/make.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.958825 gitberg-0.8.2/gitenberg/metadata/
--rw-r--r--   0 eric       (501) staff       (20)     6148 2017-03-15 21:43:48.000000 gitberg-0.8.2/gitenberg/metadata/.DS_Store
--rwxr-xr-x   0 eric       (501) staff       (20)        0 2020-01-17 23:13:49.000000 gitberg-0.8.2/gitenberg/metadata/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      150 2020-01-02 22:46:16.000000 gitberg-0.8.2/gitenberg/metadata/__init__.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.959961 gitberg-0.8.2/gitenberg/metadata/__pycache__/
--rw-r--r--   0 eric       (501) staff       (20)      154 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/metadata/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     9544 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/metadata/__pycache__/licenses.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3813 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/metadata/__pycache__/marc.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     7888 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/metadata/__pycache__/pandata.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     8948 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/metadata/__pycache__/pg_rdf.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1284 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/metadata/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1450 2022-09-26 22:28:56.000000 gitberg-0.8.2/gitenberg/metadata/fileinfo.py
--rw-r--r--   0 eric       (501) staff       (20)     1752 2020-01-02 22:46:16.000000 gitberg-0.8.2/gitenberg/metadata/fileinfo.pyc
--rw-r--r--   0 eric       (501) staff       (20)     9254 2016-03-08 17:03:43.000000 gitberg-0.8.2/gitenberg/metadata/licenses.py
--rw-r--r--   0 eric       (501) staff       (20)    11538 2016-03-09 21:30:05.000000 gitberg-0.8.2/gitenberg/metadata/licenses.pyc
--rw-r--r--   0 eric       (501) staff       (20)     7973 2020-01-17 23:13:49.000000 gitberg-0.8.2/gitenberg/metadata/marc.py
--rw-r--r--   0 eric       (501) staff       (20)     5057 2020-01-02 22:46:16.000000 gitberg-0.8.2/gitenberg/metadata/marc.pyc
--rw-r--r--   0 eric       (501) staff       (20)     8408 2022-09-26 22:28:56.000000 gitberg-0.8.2/gitenberg/metadata/pandata.py
--rw-r--r--   0 eric       (501) staff       (20)    10101 2020-01-02 22:46:16.000000 gitberg-0.8.2/gitenberg/metadata/pandata.pyc
--rw-r--r--   0 eric       (501) staff       (20)       29 2016-03-08 17:03:43.000000 gitberg-0.8.2/gitenberg/metadata/parameters.py
--rw-r--r--   0 eric       (501) staff       (20)      119 2016-03-09 21:30:05.000000 gitberg-0.8.2/gitenberg/metadata/parameters.pyc
--rw-r--r--   0 eric       (501) staff       (20)    11560 2022-09-26 22:28:56.000000 gitberg-0.8.2/gitenberg/metadata/pg_rdf.py
--rw-r--r--   0 eric       (501) staff       (20)    11832 2020-01-02 22:46:16.000000 gitberg-0.8.2/gitenberg/metadata/pg_rdf.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1019 2016-03-08 17:03:43.000000 gitberg-0.8.2/gitenberg/metadata/utils.py
--rw-r--r--   0 eric       (501) staff       (20)     1703 2016-03-09 21:30:05.000000 gitberg-0.8.2/gitenberg/metadata/utils.pyc
--rw-r--r--   0 eric       (501) staff       (20)      114 2018-03-06 20:16:12.000000 gitberg-0.8.2/gitenberg/parameters.py
--rw-r--r--   0 eric       (501) staff       (20)      291 2018-03-06 20:26:11.000000 gitberg-0.8.2/gitenberg/parameters.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2003 2020-01-17 23:13:49.000000 gitberg-0.8.2/gitenberg/pg_wikipedia.py
--rw-r--r--   0 eric       (501) staff       (20)     2926 2020-01-02 22:46:15.000000 gitberg-0.8.2/gitenberg/pg_wikipedia.pyc
--rw-r--r--   0 eric       (501) staff       (20)     4658 2022-12-01 17:24:51.000000 gitberg-0.8.2/gitenberg/push.py
--rw-r--r--   0 eric       (501) staff       (20)     6839 2019-01-01 21:04:42.000000 gitberg-0.8.2/gitenberg/push.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.960845 gitberg-0.8.2/gitenberg/templates/
--rw-r--r--   0 eric       (501) staff       (20)     6148 2018-08-30 21:11:21.000000 gitberg-0.8.2/gitenberg/templates/.DS_Store
--rw-r--r--   0 eric       (501) staff       (20)      413 2017-03-29 18:14:25.000000 gitberg-0.8.2/gitenberg/templates/CONTRIBUTING.rst
--rw-r--r--   0 eric       (501) staff       (20)    17504 2017-03-29 18:14:30.000000 gitberg-0.8.2/gitenberg/templates/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)     1986 2018-10-20 00:56:40.000000 gitberg-0.8.2/gitenberg/templates/README.rst.j2
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.964771 gitberg-0.8.2/gitenberg/tests/
--rw-r--r--   0 eric       (501) staff       (20)     6148 2020-01-02 21:11:31.000000 gitberg-0.8.2/gitenberg/tests/.DS_Store
--rw-r--r--   0 eric       (501) staff       (20)        0 2016-02-05 20:21:16.000000 gitberg-0.8.2/gitenberg/tests/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      147 2016-03-02 17:13:57.000000 gitberg-0.8.2/gitenberg/tests/__init__.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1324 2018-10-24 05:11:21.000000 gitberg-0.8.2/gitenberg/tests/test_book.py
--rw-r--r--   0 eric       (501) staff       (20)     2450 2018-10-24 05:11:32.000000 gitberg-0.8.2/gitenberg/tests/test_book.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1733 2018-09-05 14:03:00.000000 gitberg-0.8.2/gitenberg/tests/test_config.py
--rw-r--r--   0 eric       (501) staff       (20)     2394 2018-09-05 14:05:51.000000 gitberg-0.8.2/gitenberg/tests/test_config.pyc
--rwxr-xr-x   0 eric       (501) staff       (20)      985 2018-03-06 20:16:12.000000 gitberg-0.8.2/gitenberg/tests/test_cover.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.965095 gitberg-0.8.2/gitenberg/tests/test_data/
--rw-r--r--   0 eric       (501) staff       (20)     6148 2020-01-02 21:21:15.000000 gitberg-0.8.2/gitenberg/tests/test_data/.DS_Store
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.965657 gitberg-0.8.2/gitenberg/tests/test_data/1234/
--rw-r--r--   0 eric       (501) staff       (20)   154730 2018-03-06 20:16:12.000000 gitberg-0.8.2/gitenberg/tests/test_data/1234/1234.txt
--rw-r--r--   0 eric       (501) staff       (20)    10564 2016-02-05 20:21:16.000000 gitberg-0.8.2/gitenberg/tests/test_data/1234/pg1234.rdf
--rw-r--r--   0 eric       (501) staff       (20)      176 2018-03-06 20:16:12.000000 gitberg-0.8.2/gitenberg/tests/test_data/config.yaml
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.965910 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/
--rw-r--r--   0 eric       (501) staff       (20)     6148 2018-09-24 20:45:43.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/.DS_Store
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.966078 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.966646 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/
--rw-r--r--   0 eric       (501) staff       (20)       23 2017-03-03 19:26:13.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/HEAD
--rw-r--r--   0 eric       (501) staff       (20)      137 2017-03-03 19:26:13.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/config
--rw-r--r--   0 eric       (501) staff       (20)       73 2017-03-03 19:26:13.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/description
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.968260 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/
--rwxr-xr-x   0 eric       (501) staff       (20)      478 2017-03-03 19:26:13.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 eric       (501) staff       (20)      896 2017-03-03 19:26:13.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 eric       (501) staff       (20)      189 2017-03-03 19:26:13.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/post-update.sample
--rwxr-xr-x   0 eric       (501) staff       (20)      424 2017-03-03 19:26:13.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     1642 2017-03-03 19:26:13.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     1348 2017-03-03 19:26:13.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-push.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     4951 2017-03-03 19:26:13.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-rebase.sample
--rw-r--r--   0 eric       (501) staff       (20)      544 2017-03-03 19:26:13.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     1239 2017-03-03 19:26:13.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     3610 2017-03-03 19:26:13.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/update.sample
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.968411 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/info/
--rw-r--r--   0 eric       (501) staff       (20)      240 2017-03-03 19:26:13.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/info/exclude
--rw-r--r--   0 eric       (501) staff       (20)     9545 2016-08-13 21:57:29.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/pg1234.rdf
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.968570 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.969159 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/
--rw-r--r--   0 eric       (501) staff       (20)       23 2017-03-15 17:13:08.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/HEAD
--rw-r--r--   0 eric       (501) staff       (20)      137 2017-03-15 17:13:08.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/config
--rw-r--r--   0 eric       (501) staff       (20)       73 2017-03-15 17:13:08.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/description
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.970752 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/
--rwxr-xr-x   0 eric       (501) staff       (20)      478 2017-03-15 17:13:08.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 eric       (501) staff       (20)      896 2017-03-15 17:13:08.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 eric       (501) staff       (20)      189 2017-03-15 17:13:08.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/post-update.sample
--rwxr-xr-x   0 eric       (501) staff       (20)      424 2017-03-15 17:13:08.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     1642 2017-03-15 17:13:08.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     1348 2017-03-15 17:13:08.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-push.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     4951 2017-03-15 17:13:08.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-rebase.sample
--rw-r--r--   0 eric       (501) staff       (20)      544 2017-03-15 17:13:08.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     1239 2017-03-15 17:13:08.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     3610 2017-03-15 17:13:08.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/update.sample
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.970905 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/info/
--rw-r--r--   0 eric       (501) staff       (20)      240 2017-03-15 17:13:08.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/info/exclude
--rw-r--r--   0 eric       (501) staff       (20)    11002 2018-09-24 20:32:21.000000 gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/pg7.rdf
--rw-r--r--   0 eric       (501) staff       (20)      910 2018-08-23 14:55:00.000000 gitberg-0.8.2/gitenberg/tests/test_fetch.py
--rw-r--r--   0 eric       (501) staff       (20)     1449 2018-08-23 15:14:49.000000 gitberg-0.8.2/gitenberg/tests/test_fetch.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2078 2020-01-17 23:13:49.000000 gitberg-0.8.2/gitenberg/tests/test_local_repo.py
--rw-r--r--   0 eric       (501) staff       (20)     3406 2020-01-02 22:46:16.000000 gitberg-0.8.2/gitenberg/tests/test_local_repo.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1463 2018-09-05 14:03:10.000000 gitberg-0.8.2/gitenberg/tests/test_make.py
--rw-r--r--   0 eric       (501) staff       (20)     2369 2018-09-05 14:05:51.000000 gitberg-0.8.2/gitenberg/tests/test_make.pyc
--rw-r--r--   0 eric       (501) staff       (20)     4614 2020-01-17 23:13:49.000000 gitberg-0.8.2/gitenberg/tests/test_metadata.py
--rw-r--r--   0 eric       (501) staff       (20)     6713 2020-01-02 22:46:16.000000 gitberg-0.8.2/gitenberg/tests/test_metadata.pyc
--rw-r--r--   0 eric       (501) staff       (20)      947 2018-03-06 20:16:12.000000 gitberg-0.8.2/gitenberg/tests/test_old_metadata.py
--rw-r--r--   0 eric       (501) staff       (20)     1645 2018-03-08 16:32:09.000000 gitberg-0.8.2/gitenberg/tests/test_old_metadata.pyc
--rw-r--r--   0 eric       (501) staff       (20)      839 2018-09-26 20:43:13.000000 gitberg-0.8.2/gitenberg/tests/test_push.py
--rw-r--r--   0 eric       (501) staff       (20)     1675 2018-09-26 20:43:45.000000 gitberg-0.8.2/gitenberg/tests/test_push.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.972661 gitberg-0.8.2/gitenberg/util/
--rw-r--r--   0 eric       (501) staff       (20)        0 2016-02-05 20:21:16.000000 gitberg-0.8.2/gitenberg/util/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      146 2016-02-05 21:55:38.000000 gitberg-0.8.2/gitenberg/util/__init__.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-12-08 03:34:21.974551 gitberg-0.8.2/gitenberg/util/__pycache__/
--rw-r--r--   0 eric       (501) staff       (20)      142 2020-01-02 18:44:44.000000 gitberg-0.8.2/gitenberg/util/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)      150 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/util/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     5787 2020-01-02 18:44:44.000000 gitberg-0.8.2/gitenberg/util/__pycache__/catalog.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     5970 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/util/__pycache__/catalog.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)      722 2020-01-02 18:44:44.000000 gitberg-0.8.2/gitenberg/util/__pycache__/filetypes.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)      668 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/util/__pycache__/filetypes.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)      674 2022-09-03 19:19:34.000000 gitberg-0.8.2/gitenberg/util/__pycache__/pg.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)    18365 2020-01-02 18:44:44.000000 gitberg-0.8.2/gitenberg/util/__pycache__/tenprintcover.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)    18375 2022-09-03 19:19:33.000000 gitberg-0.8.2/gitenberg/util/__pycache__/tenprintcover.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     6252 2022-09-26 22:27:52.000000 gitberg-0.8.2/gitenberg/util/catalog.py
--rw-r--r--   0 eric       (501) staff       (20)     7415 2020-01-06 13:39:38.000000 gitberg-0.8.2/gitenberg/util/catalog.pyc
--rw-r--r--   0 eric       (501) staff       (20)      653 2019-01-02 17:21:37.000000 gitberg-0.8.2/gitenberg/util/filetypes.py
--rw-r--r--   0 eric       (501) staff       (20)      986 2019-01-02 17:25:13.000000 gitberg-0.8.2/gitenberg/util/filetypes.pyc
--rw-r--r--   0 eric       (501) staff       (20)      710 2018-10-01 21:31:41.000000 gitberg-0.8.2/gitenberg/util/pg.py
--rw-r--r--   0 eric       (501) staff       (20)      826 2018-10-01 21:31:49.000000 gitberg-0.8.2/gitenberg/util/pg.pyc
--rwxr-xr-x   0 eric       (501) staff       (20)    27391 2018-08-23 14:57:32.000000 gitberg-0.8.2/gitenberg/util/tenprintcover.py
--rw-r--r--   0 eric       (501) staff       (20)    22658 2018-08-23 15:14:49.000000 gitberg-0.8.2/gitenberg/util/tenprintcover.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3988 2022-09-26 22:28:56.000000 gitberg-0.8.2/gitenberg/workflow.py
--rw-r--r--   0 eric       (501) staff       (20)     4453 2019-01-02 00:03:57.000000 gitberg-0.8.2/gitenberg/workflow.pyc
--rw-r--r--   0 eric       (501) staff       (20)      523 2020-11-25 17:33:55.000000 gitberg-0.8.2/requirements.pip
--rw-r--r--   0 eric       (501) staff       (20)       67 2022-12-08 03:34:21.975461 gitberg-0.8.2/setup.cfg
--rwxr-xr-x   0 eric       (501) staff       (20)     2010 2022-12-01 17:10:57.000000 gitberg-0.8.2/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.591438 gitberg-0.8.3/
+-rw-r--r--   0 eric       (501) staff       (20)      413 2016-03-08 17:03:43.000000 gitberg-0.8.3/CONTRIBUTING.rst
+-rw-r--r--   0 eric       (501) staff       (20)     6422 2023-04-20 17:13:11.000000 gitberg-0.8.3/HISTORY.rst
+-rw-r--r--   0 eric       (501) staff       (20)    35065 2016-02-05 20:21:16.000000 gitberg-0.8.3/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      126 2016-03-12 19:39:51.000000 gitberg-0.8.3/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)    35647 2023-04-20 17:16:11.591550 gitberg-0.8.3/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     2463 2022-09-26 22:28:56.000000 gitberg-0.8.3/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.546415 gitberg-0.8.3/bin/
+-rwxr-xr-x   0 eric       (501) staff       (20)     5744 2022-09-26 22:28:56.000000 gitberg-0.8.3/bin/gitberg
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.547324 gitberg-0.8.3/gitberg.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)    35647 2023-04-20 17:16:11.000000 gitberg-0.8.3/gitberg.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     6739 2023-04-20 17:16:11.000000 gitberg-0.8.3/gitberg.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-04-20 17:16:11.000000 gitberg-0.8.3/gitberg.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)      294 2023-04-20 17:16:11.000000 gitberg-0.8.3/gitberg.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       10 2023-04-20 17:16:11.000000 gitberg-0.8.3/gitberg.egg-info/top_level.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.553444 gitberg-0.8.3/gitenberg/
+-rw-r--r--   0 eric       (501) staff       (20)    10244 2023-04-20 16:15:38.000000 gitberg-0.8.3/gitenberg/.DS_Store
+-rw-r--r--   0 eric       (501) staff       (20)      418 2023-04-20 16:10:13.000000 gitberg-0.8.3/gitenberg/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      717 2019-08-16 13:25:41.000000 gitberg-0.8.3/gitenberg/__init__.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.558570 gitberg-0.8.3/gitenberg/__pycache__/
+-rw-r--r--   0 eric       (501) staff       (20)      591 2020-01-02 18:44:43.000000 gitberg-0.8.3/gitenberg/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      599 2022-09-03 19:19:32.000000 gitberg-0.8.3/gitenberg/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2496 2022-09-03 19:19:34.000000 gitberg-0.8.3/gitenberg/__pycache__/actions.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     9466 2020-01-02 18:44:43.000000 gitberg-0.8.3/gitenberg/__pycache__/book.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     9620 2022-09-03 19:19:32.000000 gitberg-0.8.3/gitenberg/__pycache__/book.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2510 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/clone.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2545 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/clone.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3446 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/config.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3565 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2388 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/dialog.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2651 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/dialog.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1127 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/fetch.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1153 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/fetch.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1704 2022-09-03 19:19:34.000000 gitberg-0.8.3/gitenberg/__pycache__/library.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3812 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/local_repo.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3812 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/local_repo.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2393 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/make.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2449 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/make.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      260 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/parameters.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      268 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/parameters.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2202 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/pg_wikipedia.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2339 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/pg_wikipedia.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     5456 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/push.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     4585 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/push.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3550 2022-09-03 19:19:34.000000 gitberg-0.8.3/gitenberg/__pycache__/workflow.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2608 2018-10-23 16:38:04.000000 gitberg-0.8.3/gitenberg/actions.py
+-rw-r--r--   0 eric       (501) staff       (20)     3374 2018-10-23 16:40:03.000000 gitberg-0.8.3/gitenberg/actions.pyc
+-rw-r--r--   0 eric       (501) staff       (20)    12687 2022-09-26 22:28:56.000000 gitberg-0.8.3/gitenberg/book.py
+-rw-r--r--   0 eric       (501) staff       (20)    12013 2020-01-06 13:39:38.000000 gitberg-0.8.3/gitenberg/book.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2205 2018-09-15 18:38:44.000000 gitberg-0.8.3/gitenberg/clone.py
+-rw-r--r--   0 eric       (501) staff       (20)     3139 2018-09-15 18:38:50.000000 gitberg-0.8.3/gitenberg/clone.pyc
+-rwxr-xr-x   0 eric       (501) staff       (20)     3328 2022-09-26 22:28:56.000000 gitberg-0.8.3/gitenberg/config.py
+-rw-r--r--   0 eric       (501) staff       (20)     4413 2020-01-06 13:39:38.000000 gitberg-0.8.3/gitenberg/config.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.568389 gitberg-0.8.3/gitenberg/data/
+-rw-r--r--   0 eric       (501) staff       (20)     6148 2018-10-03 17:58:06.000000 gitberg-0.8.3/gitenberg/data/.DS_Store
+-rw-r--r--   0 eric       (501) staff       (20)  3876689 2023-04-20 15:58:58.000000 gitberg-0.8.3/gitenberg/data/GITenberg_repo_list.tsv
+-rw-r--r--   0 eric       (501) staff       (20)  1815872 2017-03-29 18:11:05.000000 gitberg-0.8.3/gitenberg/data/gutenberg_descriptions.json
+-rw-r--r--   0 eric       (501) staff       (20)    57617 2022-09-26 22:31:30.000000 gitberg-0.8.3/gitenberg/data/missing.tsv
+-rw-r--r--   0 eric       (501) staff       (20)       17 2020-01-18 01:02:06.000000 gitberg-0.8.3/gitenberg/data/removed.txt
+-rw-r--r--   0 eric       (501) staff       (20)     2265 2020-03-24 17:09:28.000000 gitberg-0.8.3/gitenberg/dialog.py
+-rw-r--r--   0 eric       (501) staff       (20)     2963 2018-05-14 18:18:37.000000 gitberg-0.8.3/gitenberg/dialog.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      681 2018-10-03 19:32:10.000000 gitberg-0.8.3/gitenberg/fetch.py
+-rw-r--r--   0 eric       (501) staff       (20)     1365 2018-10-03 21:25:03.000000 gitberg-0.8.3/gitenberg/fetch.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.568939 gitberg-0.8.3/gitenberg/gitenberg/
+-rw-r--r--   0 eric       (501) staff       (20)      243 2017-03-29 18:13:43.000000 gitberg-0.8.3/gitenberg/gitenberg/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      373 2017-11-09 21:09:26.000000 gitberg-0.8.3/gitenberg/gitenberg/__init__.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1197 2019-01-01 22:05:08.000000 gitberg-0.8.3/gitenberg/library.py
+-rw-r--r--   0 eric       (501) staff       (20)     2062 2019-01-01 23:27:51.000000 gitberg-0.8.3/gitenberg/library.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3093 2020-01-02 22:45:38.000000 gitberg-0.8.3/gitenberg/local_repo.py
+-rw-r--r--   0 eric       (501) staff       (20)     4380 2020-01-02 22:46:15.000000 gitberg-0.8.3/gitenberg/local_repo.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2243 2018-10-20 18:41:52.000000 gitberg-0.8.3/gitenberg/make.py
+-rw-r--r--   0 eric       (501) staff       (20)     2966 2018-10-20 18:42:53.000000 gitberg-0.8.3/gitenberg/make.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.572473 gitberg-0.8.3/gitenberg/metadata/
+-rw-r--r--   0 eric       (501) staff       (20)     6148 2017-03-15 21:43:48.000000 gitberg-0.8.3/gitenberg/metadata/.DS_Store
+-rwxr-xr-x   0 eric       (501) staff       (20)        0 2020-01-17 23:13:49.000000 gitberg-0.8.3/gitenberg/metadata/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      150 2020-01-02 22:46:16.000000 gitberg-0.8.3/gitenberg/metadata/__init__.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.573590 gitberg-0.8.3/gitenberg/metadata/__pycache__/
+-rw-r--r--   0 eric       (501) staff       (20)      154 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/metadata/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     9544 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/metadata/__pycache__/licenses.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3813 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/metadata/__pycache__/marc.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     7888 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/metadata/__pycache__/pandata.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     8948 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/metadata/__pycache__/pg_rdf.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1284 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/metadata/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1458 2023-04-20 16:26:42.000000 gitberg-0.8.3/gitenberg/metadata/fileinfo.py
+-rw-r--r--   0 eric       (501) staff       (20)     1752 2020-01-02 22:46:16.000000 gitberg-0.8.3/gitenberg/metadata/fileinfo.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     9254 2016-03-08 17:03:43.000000 gitberg-0.8.3/gitenberg/metadata/licenses.py
+-rw-r--r--   0 eric       (501) staff       (20)    11538 2016-03-09 21:30:05.000000 gitberg-0.8.3/gitenberg/metadata/licenses.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     7973 2020-01-17 23:13:49.000000 gitberg-0.8.3/gitenberg/metadata/marc.py
+-rw-r--r--   0 eric       (501) staff       (20)     5057 2020-01-02 22:46:16.000000 gitberg-0.8.3/gitenberg/metadata/marc.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     8408 2022-09-26 22:28:56.000000 gitberg-0.8.3/gitenberg/metadata/pandata.py
+-rw-r--r--   0 eric       (501) staff       (20)    10101 2020-01-02 22:46:16.000000 gitberg-0.8.3/gitenberg/metadata/pandata.pyc
+-rw-r--r--   0 eric       (501) staff       (20)       29 2016-03-08 17:03:43.000000 gitberg-0.8.3/gitenberg/metadata/parameters.py
+-rw-r--r--   0 eric       (501) staff       (20)      119 2016-03-09 21:30:05.000000 gitberg-0.8.3/gitenberg/metadata/parameters.pyc
+-rw-r--r--   0 eric       (501) staff       (20)    11568 2023-04-20 16:29:26.000000 gitberg-0.8.3/gitenberg/metadata/pg_rdf.py
+-rw-r--r--   0 eric       (501) staff       (20)    11832 2020-01-02 22:46:16.000000 gitberg-0.8.3/gitenberg/metadata/pg_rdf.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1019 2016-03-08 17:03:43.000000 gitberg-0.8.3/gitenberg/metadata/utils.py
+-rw-r--r--   0 eric       (501) staff       (20)     1703 2016-03-09 21:30:05.000000 gitberg-0.8.3/gitenberg/metadata/utils.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      114 2018-03-06 20:16:12.000000 gitberg-0.8.3/gitenberg/parameters.py
+-rw-r--r--   0 eric       (501) staff       (20)      291 2018-03-06 20:26:11.000000 gitberg-0.8.3/gitenberg/parameters.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2003 2020-01-17 23:13:49.000000 gitberg-0.8.3/gitenberg/pg_wikipedia.py
+-rw-r--r--   0 eric       (501) staff       (20)     2926 2020-01-02 22:46:15.000000 gitberg-0.8.3/gitenberg/pg_wikipedia.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     4658 2022-12-01 17:24:51.000000 gitberg-0.8.3/gitenberg/push.py
+-rw-r--r--   0 eric       (501) staff       (20)     6839 2019-01-01 21:04:42.000000 gitberg-0.8.3/gitenberg/push.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.575813 gitberg-0.8.3/gitenberg/templates/
+-rw-r--r--   0 eric       (501) staff       (20)     6148 2018-08-30 21:11:21.000000 gitberg-0.8.3/gitenberg/templates/.DS_Store
+-rw-r--r--   0 eric       (501) staff       (20)      413 2017-03-29 18:14:25.000000 gitberg-0.8.3/gitenberg/templates/CONTRIBUTING.rst
+-rw-r--r--   0 eric       (501) staff       (20)    17504 2017-03-29 18:14:30.000000 gitberg-0.8.3/gitenberg/templates/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)     1986 2018-10-20 00:56:40.000000 gitberg-0.8.3/gitenberg/templates/README.rst.j2
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.580579 gitberg-0.8.3/gitenberg/tests/
+-rw-r--r--   0 eric       (501) staff       (20)     6148 2023-04-20 16:14:35.000000 gitberg-0.8.3/gitenberg/tests/.DS_Store
+-rw-r--r--   0 eric       (501) staff       (20)        0 2016-02-05 20:21:16.000000 gitberg-0.8.3/gitenberg/tests/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      147 2016-03-02 17:13:57.000000 gitberg-0.8.3/gitenberg/tests/__init__.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1324 2018-10-24 05:11:21.000000 gitberg-0.8.3/gitenberg/tests/test_book.py
+-rw-r--r--   0 eric       (501) staff       (20)     2450 2018-10-24 05:11:32.000000 gitberg-0.8.3/gitenberg/tests/test_book.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1733 2018-09-05 14:03:00.000000 gitberg-0.8.3/gitenberg/tests/test_config.py
+-rw-r--r--   0 eric       (501) staff       (20)     2394 2018-09-05 14:05:51.000000 gitberg-0.8.3/gitenberg/tests/test_config.pyc
+-rwxr-xr-x   0 eric       (501) staff       (20)      985 2018-03-06 20:16:12.000000 gitberg-0.8.3/gitenberg/tests/test_cover.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.581014 gitberg-0.8.3/gitenberg/tests/test_data/
+-rw-r--r--   0 eric       (501) staff       (20)     6148 2020-01-02 21:21:15.000000 gitberg-0.8.3/gitenberg/tests/test_data/.DS_Store
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.581887 gitberg-0.8.3/gitenberg/tests/test_data/1234/
+-rw-r--r--   0 eric       (501) staff       (20)   154730 2018-03-06 20:16:12.000000 gitberg-0.8.3/gitenberg/tests/test_data/1234/1234.txt
+-rw-r--r--   0 eric       (501) staff       (20)    10564 2016-02-05 20:21:16.000000 gitberg-0.8.3/gitenberg/tests/test_data/1234/pg1234.rdf
+-rw-r--r--   0 eric       (501) staff       (20)      176 2018-03-06 20:16:12.000000 gitberg-0.8.3/gitenberg/tests/test_data/config.yaml
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.582150 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/
+-rw-r--r--   0 eric       (501) staff       (20)     6148 2018-09-24 20:45:43.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/.DS_Store
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.582315 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.582911 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/
+-rw-r--r--   0 eric       (501) staff       (20)       23 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/HEAD
+-rw-r--r--   0 eric       (501) staff       (20)      137 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/config
+-rw-r--r--   0 eric       (501) staff       (20)       73 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/description
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.584596 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/
+-rwxr-xr-x   0 eric       (501) staff       (20)      478 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)      896 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)      189 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/post-update.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)      424 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     1642 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     1348 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     4951 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-rebase.sample
+-rw-r--r--   0 eric       (501) staff       (20)      544 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     1239 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     3610 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/update.sample
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.584798 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/info/
+-rw-r--r--   0 eric       (501) staff       (20)      240 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/info/exclude
+-rw-r--r--   0 eric       (501) staff       (20)     9545 2016-08-13 21:57:29.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/pg1234.rdf
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.584977 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.585459 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/
+-rw-r--r--   0 eric       (501) staff       (20)       23 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/HEAD
+-rw-r--r--   0 eric       (501) staff       (20)      137 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/config
+-rw-r--r--   0 eric       (501) staff       (20)       73 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/description
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.587186 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/
+-rwxr-xr-x   0 eric       (501) staff       (20)      478 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)      896 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)      189 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/post-update.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)      424 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     1642 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     1348 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     4951 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-rebase.sample
+-rw-r--r--   0 eric       (501) staff       (20)      544 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     1239 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     3610 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/update.sample
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.587366 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/info/
+-rw-r--r--   0 eric       (501) staff       (20)      240 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/info/exclude
+-rw-r--r--   0 eric       (501) staff       (20)    11002 2018-09-24 20:32:21.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/pg7.rdf
+-rw-r--r--   0 eric       (501) staff       (20)      910 2018-08-23 14:55:00.000000 gitberg-0.8.3/gitenberg/tests/test_fetch.py
+-rw-r--r--   0 eric       (501) staff       (20)     1449 2018-08-23 15:14:49.000000 gitberg-0.8.3/gitenberg/tests/test_fetch.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2078 2020-01-17 23:13:49.000000 gitberg-0.8.3/gitenberg/tests/test_local_repo.py
+-rw-r--r--   0 eric       (501) staff       (20)     3406 2020-01-02 22:46:16.000000 gitberg-0.8.3/gitenberg/tests/test_local_repo.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1463 2018-09-05 14:03:10.000000 gitberg-0.8.3/gitenberg/tests/test_make.py
+-rw-r--r--   0 eric       (501) staff       (20)     2369 2018-09-05 14:05:51.000000 gitberg-0.8.3/gitenberg/tests/test_make.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     4614 2020-01-17 23:13:49.000000 gitberg-0.8.3/gitenberg/tests/test_metadata.py
+-rw-r--r--   0 eric       (501) staff       (20)     6713 2020-01-02 22:46:16.000000 gitberg-0.8.3/gitenberg/tests/test_metadata.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      947 2018-03-06 20:16:12.000000 gitberg-0.8.3/gitenberg/tests/test_old_metadata.py
+-rw-r--r--   0 eric       (501) staff       (20)     1645 2018-03-08 16:32:09.000000 gitberg-0.8.3/gitenberg/tests/test_old_metadata.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      839 2018-09-26 20:43:13.000000 gitberg-0.8.3/gitenberg/tests/test_push.py
+-rw-r--r--   0 eric       (501) staff       (20)     1675 2018-09-26 20:43:45.000000 gitberg-0.8.3/gitenberg/tests/test_push.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.589097 gitberg-0.8.3/gitenberg/util/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2016-02-05 20:21:16.000000 gitberg-0.8.3/gitenberg/util/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      146 2016-02-05 21:55:38.000000 gitberg-0.8.3/gitenberg/util/__init__.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.591032 gitberg-0.8.3/gitenberg/util/__pycache__/
+-rw-r--r--   0 eric       (501) staff       (20)      142 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/util/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      150 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/util/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     5787 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/util/__pycache__/catalog.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     5970 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/util/__pycache__/catalog.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      722 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/util/__pycache__/filetypes.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      668 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/util/__pycache__/filetypes.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      674 2022-09-03 19:19:34.000000 gitberg-0.8.3/gitenberg/util/__pycache__/pg.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)    18365 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/util/__pycache__/tenprintcover.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)    18375 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/util/__pycache__/tenprintcover.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     6252 2023-02-17 22:50:16.000000 gitberg-0.8.3/gitenberg/util/catalog.py
+-rw-r--r--   0 eric       (501) staff       (20)     7415 2020-01-06 13:39:38.000000 gitberg-0.8.3/gitenberg/util/catalog.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      653 2019-01-02 17:21:37.000000 gitberg-0.8.3/gitenberg/util/filetypes.py
+-rw-r--r--   0 eric       (501) staff       (20)      986 2019-01-02 17:25:13.000000 gitberg-0.8.3/gitenberg/util/filetypes.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      710 2018-10-01 21:31:41.000000 gitberg-0.8.3/gitenberg/util/pg.py
+-rw-r--r--   0 eric       (501) staff       (20)      826 2018-10-01 21:31:49.000000 gitberg-0.8.3/gitenberg/util/pg.pyc
+-rwxr-xr-x   0 eric       (501) staff       (20)    27391 2018-08-23 14:57:32.000000 gitberg-0.8.3/gitenberg/util/tenprintcover.py
+-rw-r--r--   0 eric       (501) staff       (20)    22658 2018-08-23 15:14:49.000000 gitberg-0.8.3/gitenberg/util/tenprintcover.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3988 2022-09-26 22:28:56.000000 gitberg-0.8.3/gitenberg/workflow.py
+-rw-r--r--   0 eric       (501) staff       (20)     4453 2019-01-02 00:03:57.000000 gitberg-0.8.3/gitenberg/workflow.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      523 2020-11-25 17:33:55.000000 gitberg-0.8.3/requirements.pip
+-rw-r--r--   0 eric       (501) staff       (20)       67 2023-04-20 17:16:11.591892 gitberg-0.8.3/setup.cfg
+-rwxr-xr-x   0 eric       (501) staff       (20)     2010 2022-12-01 17:10:57.000000 gitberg-0.8.3/setup.py
```

### Comparing `gitberg-0.8.2/HISTORY.rst` & `gitberg-0.8.3/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 .. :changelog:
 
 History
 -------
+0.8.3 (2023-04-20)
+==================
+* fix opening rdf files and reading mod date
+* update repo lists
+  * add 69347-70401
+
 0.8.2 (2022-12-07)
 ==================
 * fixed long authorname issue
 * update repo lists
   * add 69024-69346
 * update some dependencies
```

### Comparing `gitberg-0.8.2/LICENSE` & `gitberg-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/PKG-INFO` & `gitberg-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitberg
-Version: 0.8.2
+Version: 0.8.3
 Summary: A library and command for interacting with the GITenberg books project
 Home-page: https://github.com/gitenberg-dev/gitberg
 Author: Seth Woodworth
 Author-email: seth@sethish.com
 License: GPLv3
 Keywords: books ebooks gitenberg gutenberg epub metadata
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gitberg-0.8.2/README.md` & `gitberg-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/bin/gitberg` & `gitberg-0.8.3/bin/gitberg`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitberg.egg-info/PKG-INFO` & `gitberg-0.8.3/gitberg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitberg
-Version: 0.8.2
+Version: 0.8.3
 Summary: A library and command for interacting with the GITenberg books project
 Home-page: https://github.com/gitenberg-dev/gitberg
 Author: Seth Woodworth
 Author-email: seth@sethish.com
 License: GPLv3
 Keywords: books ebooks gitenberg gutenberg epub metadata
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gitberg-0.8.2/gitberg.egg-info/SOURCES.txt` & `gitberg-0.8.3/gitberg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/.DS_Store` & `gitberg-0.8.3/gitenberg/.DS_Store`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 2000 0000 0800  ....Bud1.. .....
 00000010: 0000 2000 0000 100c 0000 0000 0000 0000  .. .............
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0002 0000 0000 0000 0011  ................
 00000050: 0000 0001 0000 1000 6473 636c 626f 6f6c  ........dsclbool
-00000060: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -252,15 +252,15 @@
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 0011 0000 0004  ................
 00001010: 0064 0061 0074 0061 6473 636c 626f 6f6c  .d.a.t.adsclbool
-00001020: 0100 0000 0400 6400 6100 7400 6166 6473  ......d.a.t.afds
+00001020: 0000 0000 0400 6400 6100 7400 6166 6473  ......d.a.t.afds
 00001030: 6362 6f6f 6c01 0000 0004 0064 0061 0074  cbool......d.a.t
 00001040: 0061 6c67 3153 636f 6d70 0000 0000 0000  .alg1Scomp......
 00001050: 0000 0000 0004 0064 0061 0074 0061 6d6f  .......d.a.t.amo
 00001060: 4444 6475 7463 0000 d304 e6f7 0000 0000  DDdutc..........
 00001070: 0004 0064 0061 0074 0061 6d6f 6444 6475  ...d.a.t.amodDdu
 00001080: 7463 0000 d304 e6f7 0000 0000 0004 0064  tc.............d
 00001090: 0061 0074 0061 7068 3153 636f 6d70 0000  .a.t.aph1Scomp..
@@ -283,15 +283,15 @@
 000011a0: 7750 6174 6862 6172 0810 8409 0809 5f10  wPathbar......_.
 000011b0: 187b 7b31 3036 2c20 3233 357d 2c20 7b37  .{{106, 235}, {7
 000011c0: 3730 2c20 3433 367d 7d08 0908 081d 2b4a  70, 436}}.....+J
 000011d0: 5662 7986 93ab b7c3 c4c6 c7c8 c9e4 e5e6  Vby.............
 000011e0: 0000 0000 0000 0101 0000 0000 0000 0014  ................
 000011f0: 0000 0000 0000 0000 0000 0000 0000 00e7  ................
 00001200: 0000 0008 006d 0065 0074 0061 0064 0061  .....m.e.t.a.d.a
-00001210: 0074 0061 6473 636c 626f 6f6c 0000 0000  .t.adsclbool....
+00001210: 0074 0061 6473 636c 626f 6f6c 0100 0000  .t.adsclbool....
 00001220: 0800 6d00 6500 7400 6100 6400 6100 7400  ..m.e.t.a.d.a.t.
 00001230: 6176 5372 6e6c 6f6e 6700 0000 0100 0000  avSrnlong.......
 00001240: 0900 7400 6500 6d00 7000 6c00 6100 7400  ..t.e.m.p.l.a.t.
 00001250: 6500 7364 7363 6c62 6f6f 6c00 0000 0005  e.sdsclbool.....
 00001260: 0074 0065 0073 0074 0073 6277 7370 626c  .t.e.s.t.sbwspbl
 00001270: 6f62 0000 00f8 6270 6c69 7374 3030 d901  ob....bplist00..
 00001280: 0203 0405 0607 0809 0a0b 0a0b 0a0b 1011  ................
@@ -306,15 +306,15 @@
 00001310: 7369 6269 6c69 7479 0809 0809 0809 5f10  sibility......_.
 00001320: 177b 7b36 332c 2032 3737 7d2c 207b 3936  .{{63, 277}, {96
 00001330: 392c 2034 3531 7d7d 1084 0808 1b29 3541  9, 451}}.....)5A
 00001340: 4d59 707d 8aa2 a3a4 a5a6 a7a8 c2c4 0000  MYp}............
 00001350: 0000 0000 0101 0000 0000 0000 0013 0000  ................
 00001360: 0000 0000 0000 0000 0000 0000 00c5 0000  ................
 00001370: 0005 0074 0065 0073 0074 0073 6473 636c  ...t.e.s.t.sdscl
-00001380: 626f 6f6c 0000 0000 0500 7400 6500 7300  bool......t.e.s.
+00001380: 626f 6f6c 0100 0000 0500 7400 6500 7300  bool......t.e.s.
 00001390: 7400 736c 7376 5062 6c6f 6200 0002 6f62  t.slsvPblob...ob
 000013a0: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
 000013b0: 0909 0b0c 4415 4546 5f10 1075 7365 5265  ....D.EF_..useRe
 000013c0: 6c61 7469 7665 4461 7465 735f 100f 7368  lativeDates_..sh
 000013d0: 6f77 4963 6f6e 5072 6576 6965 775f 1011  owIconPreview_..
 000013e0: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
 000013f0: 7357 636f 6c75 6d6e 7358 7465 7874 5369  sWcolumnsXtextSi
```

### Comparing `gitberg-0.8.2/gitenberg/__init__.pyc` & `gitberg-0.8.3/gitenberg/__init__.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/__init__.cpython-36.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/__init__.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/__init__.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/actions.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/actions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/book.cpython-36.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/book.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/book.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/book.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/clone.cpython-36.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/clone.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/clone.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/clone.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/config.cpython-36.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/config.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/config.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/dialog.cpython-36.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/dialog.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/dialog.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/fetch.cpython-36.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/fetch.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/fetch.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/fetch.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/library.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/library.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/local_repo.cpython-36.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/local_repo.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/local_repo.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/local_repo.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/make.cpython-36.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/make.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/make.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/make.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/pg_wikipedia.cpython-36.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/pg_wikipedia.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/pg_wikipedia.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/pg_wikipedia.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/push.cpython-36.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/push.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/push.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/push.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/__pycache__/workflow.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/__pycache__/workflow.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/actions.py` & `gitberg-0.8.3/gitenberg/actions.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/actions.pyc` & `gitberg-0.8.3/gitenberg/actions.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/book.py` & `gitberg-0.8.3/gitenberg/book.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/book.pyc` & `gitberg-0.8.3/gitenberg/book.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/clone.py` & `gitberg-0.8.3/gitenberg/clone.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/clone.pyc` & `gitberg-0.8.3/gitenberg/clone.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/config.py` & `gitberg-0.8.3/gitenberg/config.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/config.pyc` & `gitberg-0.8.3/gitenberg/config.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/data/.DS_Store` & `gitberg-0.8.3/gitenberg/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/data/GITenberg_repo_list.tsv` & `gitberg-0.8.3/gitenberg/data/GITenberg_repo_list.tsv`

 * *Files 1% similar despite different names*

```diff
@@ -68826,7 +68826,1062 @@
 69340	Sard-Harker-A-novel_69340
 69341	Bonanza-A-story-of-the-Gold-Trail_69341
 69342	Troubled-Waters_69342
 69343	Neves-de-antanho_69343
 69344	Poine-a-study-in-ancient-Greek-blood-vengeance_69344
 69345	The-mother-s-book_69345
 69346	Dishes-made-without-meat_69346
+69347	Drakula-angol-regeny_69347
+69348	Considerations-on-the-present-peace-as-far-as-it-is-relative-to-the-colonies-and-the-African-__69348
+69349	A-story-of-the-sawdust-The-pathetic-history-of-Old-Props-darling_69349
+69350	The-vanishers_69350
+69351	Lectures-on-the-constitution-and-laws-of-England-With-a-commentary-on-Magna-Charta-and-illust__69351
+69352	The-X-Bar-X-boys-on-Whirlpool-River_69352
+69353	A-flor-secca-romance_69353
+69354	Three-gringos-in-Venezuela-and-Central-America_69354
+69355	Footing-it-in-Franconia_69355
+69356	The-X-Bar-X-boys-on-the-ranch_69356
+69357	Forgotten-world_69357
+69358	Siren-satellite_69358
+69359	Landesverein-Sachsischer-Heimatschutz-Mitteilungen-Band-XI-Heft-10-12-Monatsschrift-fur-Heima__69359
+69360	The-steeple-jack-s-instructor_69360
+69361	Dr-Vermont-s-fantasy-and-other-stories_69361
+69362	Mendel-s-principles-of-heredity-A-defence_69362
+69363	Mutiny-of-the-Bounty-and-story-of-Pitcairn-Island-1790-1894_69363
+69364	A-little-girl-s-cookery-book_69364
+69365	Zephyrs_69365
+69366	In-de-koffie-Oorspronkelijke-Indische-Roman_69366
+69367	An-apology-for-abolitionists-addressed-by-the-anti-slavery-society-of-Meriden-Conn-to-their-f__69367
+69368	The-motion-picture-comrades-aboard-a-submarine-or-Searching-for-treasure-under-the-sea_69368
+69369	Deep-channel_69369
+69370	Leaves-from-our-Tuscan-kitchen-or-How-to-cook-vegetables_69370
+69371	The-Elizabethan-Stage-Vol-4_69371
+69372	Narrative-of-Henry-Watson-a-fugitive-slave_69372
+69373	The-ragged-edge-A-tale-of-ward-life-politics_69373
+69374	On-the-relation-which-ought-to-subsist-between-the-strength-of-an-electric-current-and-the-di__69374
+69375	The-automobile-owner-s-guide_69375
+69376	Anti-slavery-catechism_69376
+69377	Tarinoita_69377
+69378	Negro-workaday-songs_69378
+69379	Prince-Ragnal-and-other-holiday-verses_69379
+69380	Zord-ido-1-kotet-Regeny-harom-reszben_69380
+69381	Zord-ido-2-kotet-Regeny-harom-reszben_69381
+69382	Quaker-idyls_69382
+69383	In-Old-Madras_69383
+69384	Omwandelingen-door-een-gedeelte-van-Spanje-De-Aarde-en-haar-volken-1868_69384
+69385	Nick-Carter-Stories-No-124-January-23-1915-The-girl-kidnaper-or-Nick-Carter-s-up-to-date-clew_69385
+69386	Origin-of-modern-calculating-machines_69386
+69387	The-southern-literary-messenger-Vol-II-No-7-June-1836_69387
+69388	The-official-chaperon_69388
+69389	The-Arctic-regions-and-the-northern-whale-fishery_69389
+69390	Aristocracy-in-America-from-the-sketch-book-of-a-German-nobleman-vol-1_69390
+69391	Utazas-a-Holdba-kilenczvenhet-ora-es-husz-percz-alatt_69391
+69392	Eminent-doctors-Their-lives-and-their-work-Vol-2-of-2_69392
+69393	Spacemen-lost_69393
+69394	The-dream-A-novel_69394
+69395	The-quilt-of-happiness-Creeping-Jenny-and-other-New-England-stories_69395
+69396	Sint-Nikolaas-en-zijn-knecht_69396
+69397	Tales-of-the-supernatural-Six-romantic-stories_69397
+69398	Don-Sturdy-in-the-tombs-of-gold-or-The-old-Egyptian-s-great-secret_69398
+69399	The-old-town_69399
+69400	Gay-life-in-Paris-how-life-is-enjoyed-by-the-people-of-that-great-metropolis_69400
+69401	Mr-and-Mrs-Santa-Claus-Musical-Christmas-play-in-four-scenes_69401
+69402	Twice-round-the-clock-or-The-hours-of-the-day-and-night-in-London_69402
+69403	Ornithological-biography-Vol-3-of-5-An-account-of-the-habits-of-the-birds-of-the-United-State__69403
+69404	You-can-t-win_69404
+69405	Bolo-the-cave-boy_69405
+69406	Eminent-doctors-Their-lives-and-their-work-Vol-1-of-2_69406
+69407	Outposts-of-Asia_69407
+69408	The-shoemaker-A-powerful-picture-of-nature-adapted-from-Hal-Reids-famous-drama-of-the-same-na__69408
+69409	Straight-America-a-call-to-national-service_69409
+69410	Christina-Alberta-s-father_69410
+69411	Historia-del-levantamiento-guerra-y-revolucion-de-Espana-3-de-5_69411
+69412	Mountains-and-molehills-or-Recollections-of-a-burnt-journal_69412
+69413	Pamela-Pounce-A-tale-of-tempestuous-petticoats_69413
+69414	To-arms-for-liberty-A-pageant-of-the-war-for-schools-and-societies_69414
+69415	The-spirit-of-76-Some-recollections-of-the-artist-and-the-painting_69415
+69416	Christmas-stories_69416
+69417	Grotesque-architecture-or-rural-amusement-consisting-of-plans-elevations-and-sections-for-hut__69417
+69418	Impressions-of-Ukiyo-ye-the-school-of-the-Japanese-colour-print-artists_69418
+69419	American-Indian-love-lyrics-and-other-verse-From-the-songs-of-the-North-American-Indians_69419
+69420	The-adventures-of-Rob-Roy_69420
+69421	The-humour-of-Germany_69421
+69422	Le-gaie-farandole_69422
+69423	O-retrato-de-Venus-e-estudos-de-historia-litteraria_69423
+69424	Lord-Lister-No-0377-De-Heuvel-van-den-Dooden-Man_69424
+69425	Paradisi-in-sole-paradisus-terrestris-or-A-garden-of-all-sorts-of-pleasant-flowers-which-our-__69425
+69426	History-of-a-literary-radical-and-other-essays_69426
+69427	Stonepastures_69427
+69428	The-Wellfields-A-novel-Vol-1-of-3_69428
+69429	Perch-of-the-Devil_69429
+69430	Madame-Margot-A-grotesque-legend-of-old-Charleston_69430
+69431	Thomas-D-Arcy-McGee_69431
+69432	David-Thompson-the-explorer_69432
+69433	Smugglers-Island-and-the-devil-fires-of-San-Moros_69433
+69434	Herder-s-conception-of-das-Volk_69434
+69435	Rhoda-of-the-Underground_69435
+69436	Granadan-ruusu-Romaani_69436
+69437	Prodige-du-coeur_69437
+69438	Tedious-brief-tales-of-Granta-and-Gramarye_69438
+69439	Physiological-economy-in-nutrition-with-special-reference-to-the-minimal-proteid-requirement-__69439
+69440	Letters-to-a-daughter_69440
+69441	Narrative-of-a-five-years-expedition-against-the-Revolted-Negroes-of-Surinam-in-Guiana-on-the__69441
+69442	Medical-symbolism-in-connection-with-historical-studies-in-the-arts-of-healing-and-hygiene_69442
+69443	The-kiss-to-the-leper_69443
+69444	Present-status-and-prospects-of-the-Peace-Movement_69444
+69445	Universal-peacefrom-a-womans-standpoint_69445
+69446	The-Massarenes_69446
+69447	The-regiments-of-the-British-Army-chronologically-arranged_69447
+69448	The-disciplinary-circuit_69448
+69449	The-island-of-anarchy-A-fragment-of-history-in-the-20th-century_69449
+69450	An-episode-in-the-doings-of-the-dualized_69450
+69451	Behind-the-scenes-in-a-restaurant-A-study-of-1017-women-restaurant-employees_69451
+69452	Shells-and-pebbles-A-story-for-children_69452
+69453	Welcome-to-the-ransomed-or-Duties-of-the-colored-inhabitants-of-the-District-of-Columbia_69453
+69454	A-defence-of-modern-spiritualism_69454
+69455	Lord-Lister-No-0378-De-Aanslag-op-de-Londensche-Beurs_69455
+69456	Islandische-Marchen-und-Volkssagen_69456
+69457	Stories-from-the-olden-time-Teacher-s-text-book-course-IV-part-I_69457
+69458	Uncle-Wiggily-and-Mother-Goose-Complete-in-two-parts-fifty-two-storiesone-for-each-week-of-th__69458
+69459	Noticias-de-Portugal_69459
+69460	Rulers-of-kings-A-novel_69460
+69461	Rondah-or-thirty-three-years-in-a-star_69461
+69462	Komediak-A-magyar-tarsadalom-regenye_69462
+69463	The-Rover-Boys-winning-a-fortune-or-Strenuous-days-ashore-and-afloat_69463
+69464	Light-from-the-spirit-world-The-pilgrimage-of-Thomas-Paine-and-others-to-the-seventh-circle-i__69464
+69465	The-manless-worlds_69465
+69466	A-few-days-in-Athens-being-the-translation-of-a-Greek-manuscript-discovered-in-Herculaneum_69466
+69467	A-laugh-a-day-keeps-the-doctor-away_69467
+69468	Shakespeare-s-treatment-of-love-and-marriage-and-other-essays_69468
+69469	Baume-und-Straucher_69469
+69470	Am-Teich-und-Flu0xdfufer_69470
+69471	Onnen-maille-Romaani_69471
+69472	Aus-dem-Leben-unserer-Vogel_69472
+69473	The-life-of-Cardinal-Mezzofanti-With-an-introductory-memoir-of-eminent-linguists-ancient-and-__69473
+69474	A-Modern-Trio-in-an-Old-Town_69474
+69475	The-Chinese-theater_69475
+69476	Account-of-an-expedition-to-the-interior-of-New-Holland_69476
+69477	Joe-Strong-the-boy-wizard-or-The-mysteries-of-magic-exposed_69477
+69478	The-girls-of-Rivercliff-School-Beth-Baldwin-s-resolve_69478
+69479	The-garden-as-a-picture_69479
+69480	The-truth-about-socialism_69480
+69481	Austria-Hungary_69481
+69482	The-cats-Arabian-nights-or-King-Grimalkum_69482
+69483	The-amulet_69483
+69484	Bonnie-Joann-and-other-poems_69484
+69485	Letters-on-the-equality-of-the-sexes-and-the-condition-of-woman_69485
+69486	Through-Bolshevik-Russia_69486
+69487	The-complete-servant-Being-a-practical-guide-to-the-peculiar-duties-and-business-of-all-descr__69487
+69488	Practical-forging-and-art-smithing_69488
+69489	The-Wellfields-A-novel-Vol-3-of-3_69489
+69490	The-Wood-King-or-Daniel-Boone-s-last-trail-Beadle-s-Pocket-Novels-No-108_69490
+69491	The-Ohio-Naturalist-Vol-1-No-8-June-1901_69491
+69492	Memorials-of-old-Cheshire_69492
+69493	Lessons-in-chalk-modeling-The-new-method-of-map-drawing_69493
+69494	The-professor-s-experiment-Vol-1-of-3-A-novel_69494
+69495	The-professor-s-experiment-Vol-2-of-3-A-novel_69495
+69496	The-professor-s-experiment-Vol-3-of-3-A-novel_69496
+69497	Records-by-Admiral-of-the-Fleet-Lord-Fisher_69497
+69498	The-Wellfields-A-novel-Vol-2-of-3_69498
+69499	Anne-Hyde-Duchess-of-York_69499
+69500	The-Queen-s-cadet-and-other-tales_69500
+69501	At-the-fall-of-Montreal-or-A-soldier-boy-s-final-victory_69501
+69502	Hans-Holbein-the-Younger-Volume-2-of-2_69502
+69503	Looking-toward-sunset_69503
+69504	The-northern-whale-fishery_69504
+69505	They-wouldn-t-dare_69505
+69506	The-irritated-people_69506
+69507	Color-mixing-guide-for-artists-painters-decorators-printing-pressmen-show-card-writers-sign-p__69507
+69508	Sculptured-tombs-of-Hellas_69508
+69509	Frank-Allen-and-his-motor-boat-or-Racing-to-save-a-life_69509
+69510	Goa-and-the-Blue-Mountains-or-Six-months-of-sick-leave_69510
+69511	Ben-Hardy-s-flying-machine-or-Making-a-record-for-himself_69511
+69512	The-calculus-of-logic_69512
+69513	The-Aneroid-Barometer-Its-Instruction-and-Use_69513
+69514	The-best-man_69514
+69515	In-the-tiger-s-lair_69515
+69516	Piety_69516
+69517	The-ocean-wireless-boys-of-the-iceberg-patrol_69517
+69518	Vanhoja-muistoja_69518
+69519	New-system-of-domestic-cookery-formed-upon-principles-of-economy-and-adapted-to-the-use-of-pr__69519
+69520	Capillaria_69520
+69521	Surprise-house_69521
+69522	Elektrotechnisches-Experimentierbuch-Eine-Anleitung-zur-Ausfuhrung-elektrotechnischer-Experim__69522
+69523	Das-Friedensfest_69523
+69524	Pflanzenleben-in-Feld-und-Garten_69524
+69525	Das-Weihnachtslied-Eine-Erzahlung-fur-junge-Madchen_69525
+69526	Arizona-ghost-trails-From-the-handbook-to-Arizona_69526
+69527	War-against-Germany-Europe-and-adjacent-areas-pictorial-record_69527
+69528	Nuts-to-crack-Multum-in-parvo-library-v-2-no-20-August-1895-A-galaxy-of-puzzles-riddles-conun__69528
+69529	The-Aborigines-of-Australia_69529
+69530	The-humour-of-Spain_69530
+69531	Advice-to-young-men-and-boys-A-series-of-addresses-delivered-by-B-B-Comegys-to-the-pupils-of-__69531
+69532	What-luck-A-study-in-opposites_69532
+69533	Impressionist-painting-its-genesis-and-development_69533
+69534	The-doctor-c-vol-II-of-7_69534
+69535	Planet-explorer_69535
+69536	La-Terre-de-Feu-d-apres-le-Dr-Otto-Nordenskjold_69536
+69537	The-holy-war-Made-in-Germany_69537
+69538	Riches-have-wings-or-A-tale-for-the-rich-and-poor_69538
+69539	Alide-an-episode-of-Goethe-s-life_69539
+69540	Nasr-Eddine-et-son-epouse_69540
+69541	Memoires-de-Mme-la-Comtesse-de-Genlis_69541
+69542	Marie-Antoinette_69542
+69543	Around-the-world-in-eighty-minutes-Photographic-reproductions-of-the-most-magnificent-edifice__69543
+69544	The-exploits-of-Captain-O-Hagan_69544
+69545	Oliver-October_69545
+69546	Together_69546
+69547	Never-the-twain-shall-meet_69547
+69548	Landesverein-Sachsischer-Heimatschutz-Mitteilungen-Band-XII-Heft-1-3_69548
+69549	The-painted-room_69549
+69550	Mercia-the-astronomer-royal-A-romance_69550
+69551	The-natural-and-artificial-disintegration-of-the-elements-An-address-by-Professor-Sir-Ernest-__69551
+69552	El-libro-de-las-tierras-virgenes_69552
+69553	Feudal-tyrants-volume-I-of-4-The-Counts-of-Carlsheim-and-Sargans_69553
+69554	The-boy-explorers-in-darkest-New-Guinea_69554
+69555	Cactus-and-pine-Songs-of-the-Southwest_69555
+69556	Golden-rules-of-medical-evidence-Golden-Rules-Series-No-XVI_69556
+69557	A-definition-of-social-work-A-thesis-in-sociology_69557
+69558	Congo-life-and-folklore_69558
+69559	Crito-Een-dialoog-van-Plato_69559
+69560	Leisure-hours-among-the-gems_69560
+69561	Mes-Prisons_69561
+69562	Gas-and-flame-in-modern-warfare_69562
+69563	Everyday-birds-Elementary-studies_69563
+69564	The-long-way-back_69564
+69565	The-admiral-s-walk_69565
+69566	Egyptian-Book-of-the-dead_69566
+69567	Maan-tasalta-Vaatimattomia-tarinoita_69567
+69568	Brelan-des-dames_69568
+69569	The-wooing-of-Leola_69569
+69570	Friends-and-cousins_69570
+69571	Euterpe-Or-the-future-of-art_69571
+69572	Fundamental-ideas-and-problems-of-the-theory-of-relativity_69572
+69573	The-light-An-educational-pageant_69573
+69574	Excavations-at-the-LoDaisKa-Site-in-the-Denver-Colorado-area_69574
+69575	Wanderschuhe-und-andere-Erzahlungen_69575
+69576	Mathias-Sandorf-De-Middellandsche-Zee_69576
+69577	The-zoology-of-the-voyage-of-HMS-Beagle-vol-2-of-5-Under-the-command-of-Captain-Fitzroy-RN-du__69577
+69578	El-equipaje-del-rey-Jose_69578
+69579	Adventures-of-the-Comte-de-la-Muette-during-the-Reign-of-Terror_69579
+69580	Colonial-facts-and-fictions-Humorous-sketches_69580
+69581	Sacred-and-Legendary-Art-Volume-I-of-2-Containing-legends-of-the-angels-and-archangels-the-ev__69581
+69582	The-Life-and-Times-of-the-Rev-John-Wesley-Volume-I-of-3-Founder-of-the-Methodists_69582
+69583	Mon-voyage-aventureux-en-Russie-communiste_69583
+69584	Gray-lensman_69584
+69585	Napoleon-and-his-court_69585
+69586	Om-The-secret-of-Ahbor-Valley_69586
+69587	The-quenchless-light_69587
+69588	The-romance-of-the-Canadian-Pacific-Railway_69588
+69589	To-morrow-and-to-morrow-A-novel_69589
+69590	Salt-and-the-salt-industry_69590
+69591	The-conquest-of-the-great-Northwest-Volume-I-of-2-being-the-story-of-the-Adventurers-of-Engla__69591
+69592	The-popular-superstitions-and-festive-amusements-of-the-Highlanders-of-Scotland_69592
+69593	The-history-of-the-Jews-From-the-war-with-Rome-to-the-present-time_69593
+69594	San-Salvador_69594
+69595	The-life-of-John-Metcalf-commonly-called-Blind-Jack-of-Knaresborough-with-anecdotes-of-his-ex__69595
+69596	Instruccam-sobre-a-cultura-das-amoreiras-criacao-dos-bichos-da-seda-dirigida-a-conservacao-au__69596
+69597	Quand-la-Terre-trembla_69597
+69598	Buddenbrookit-II-Eraan-suvun-rappeutumistarina_69598
+69599	Dorothea-Beale-Principal-of-the-Cheltenham-Ladies-College-1858-1906_69599
+69600	A-Christmas-greeting_69600
+69601	The-escape-of-Alice-A-Christmas-fantasy_69601
+69602	The-Riddle-Club-through-the-holidays-The-club-and-its-doings-how-the-riddles-were-solved-and-__69602
+69603	Bisayan-grammar-and-notes-on-Bisayan-rhetoric-and-poetics-and-Filipino-dialectology_69603
+69604	Die-heimtuckischen-Champignons-und-andere-Geschichten_69604
+69605	Fantasques-Petits-poemes-de-propos-divers_69605
+69606	Weird-Tales-Volume-1-Number-2-April-1923-The-unique-magazine_69606
+69607	Weird-Tales-Volume-1-Number-3-May-1923-The-unique-magazine_69607
+69608	Weird-Tales-Volume-1-Number-4-June-1923-The-unique-magazine_69608
+69609	Martin-of-Old-London_69609
+69610	Robin_69610
+69611	The-Tower-Rooms_69611
+69612	The-Sea-Scouts-of-the-Kestrel-The-story-of-a-cruise-of-adventure-pluck-in-a-small-yacht-on-th__69612
+69613	Storm_69613
+69614	Have-you-an-educated-heart_69614
+69615	King-Arthur-in-history-and-legend_69615
+69616	A-teacher-s-gift_69616
+69617	Pierre-Curie_69617
+69618	Sentiments_69618
+69619	Character-of-Renaissance-Architecture_69619
+69620	Library-of-the-best-American-literature-Containing-the-lives-of-our-authors-in-story-form-the__69620
+69621	Les-causeries-du-docteur_69621
+69622	The-place-of-magic-in-the-intellectual-history-of-Europe-studies-in-history-economics-and-pub__69622
+69623	Feudal-tyrants-volume-2-of-4-The-counts-of-Carlsheim-and-Sargans_69623
+69624	Feudal-tyrants-volume-3-of-4-The-counts-of-Carlsheim-and-Sargans_69624
+69625	Feudal-tyrants-volume-4-of-4-The-counts-of-Carlsheim-and-Sargans_69625
+69626	Ce-qu-il-faut-lire-dans-sa-vie_69626
+69627	Thoughts-Selected-from-the-writings-of-favorite-authors_69627
+69628	The-Princess-Casamassima-Volume-1-of-2_69628
+69629	The-Princess-Casamassima-Volume-2-of-2_69629
+69630	The-Treatment-of-Armenians-in-the-Ottoman-Empire-Documents-Presented-to-Viscount-Grey-of-Fall__69630
+69631	0x152uvres-de-Voltaire-Tome-XX-Siecle-de-Louis-XIVTome-II_69631
+69632	The-cynic-s-breviary-Maxims-and-anecdotes-from-Nicolas-de-Chamfort_69632
+69633	Jungle-night-Atlantic-readings-number-3_69633
+69634	Lord-Lister-No-0381-De-Misdaad-in-Sutherland-Avenue_69634
+69635	Recent-research-on-radioactivity_69635
+69636	Salome-Shepard-Reformer_69636
+69637	On-a-lark-to-the-planets-a-sequel-to-the-wonderful-electric-elephant_69637
+69638	Nineteen-hundred-A-forecast-and-a-story_69638
+69639	The-Heathery-vol-1_69639
+69640	Woodburn-Grange-vol-1-of-3-A-story-of-English-country-life_69640
+69641	Schneider-Von-Groot-s-Christmas-dream_69641
+69642	Woodburn-Grange-vol-2-of-3-A-story-of-English-country-life_69642
+69643	Woodburn-Grange-vol-3-of-3-A-story-of-English-country-life_69643
+69644	Nazareth-a-morality-in-one-act_69644
+69645	Turckse-slavernie_69645
+69646	Armenia-a-martyr-nation-A-historical-sketch-of-the-Armenian-people-from-traditional-times-to-__69646
+69647	Indian-tales-of-the-great-ones-among-men-women-and-bird-people_69647
+69648	Roger-Williams_69648
+69649	The-Ranch-Girls-and-the-silver-arrow_69649
+69650	Among-Congo-cannibals_69650
+69651	Where-England-sets-her-feet-a-romance_69651
+69652	The-timeless-tomorrow_69652
+69653	Lord-Lister-No-0382-De-agent-van-Lenin_69653
+69654	The-Rambler-Club-s-ball-nine_69654
+69655	Gay-Lawless_69655
+69656	Greek-primer-colloquial-and-constructive_69656
+69657	Itinerarium-Curiosum-Centuria-I-or-An-account-of-the-antiquities-and-remarkable-curiosities-i__69657
+69658	Quarantine_69658
+69659	Space-Can_69659
+69660	Historia-del-levantamiento-guerra-y-revolucion-de-Espana-4-de-5_69660
+69661	Lord-Lister-No-0017-De-gestrafte-Don-Juan_69661
+69662	Watching-on-the-Rhine_69662
+69663	Yhteiskunnan-hylkaama-Langenneen-naisen-paivakirja_69663
+69664	The-law-of-the-road-or-wrongs-and-rights-of-a-traveller_69664
+69665	The-knowledge-machine_69665
+69666	Regulations_69666
+69667	The-giftie-gien_69667
+69668	The-education-of-Uncle-Paul_69668
+69669	Messalina-of-the-suburbs_69669
+69670	A-voice-from-Waterloo-A-history-of-the-battle-fought-on-the-18th-June-1815_69670
+69671	Greener-than-spruce_69671
+69672	The-summers-readers-Manual-first-lessons-in-reading_69672
+69673	Karl-Heinrich_69673
+69674	Wilde-v-Whistler-Being-an-Acrimonious-Correspondence-on-Art-Between-Oscar-Wilde-and-James-A-M__69674
+69675	Allworth-Abbey_69675
+69676	The-Italian-Alp-bee_69676
+69677	The-man-in-the-street-Papers-on-American-topics_69677
+69678	Memoirs-of-a-millionaire_69678
+69679	Wessagusset-and-Weymouth_69679
+69680	Lord-Lister-No-0018-Het-geheim-van-de-verminkte-kinderen_69680
+69681	The-southern-war-poetry-of-the-Civil-War_69681
+69682	Tom-Swift-circling-the-globe-or-The-daring-cruise-of-the-Air-Monarch_69682
+69683	Men-without-women_69683
+69684	Red-blight_69684
+69685	Just-sweethearts-A-Christmas-love-story_69685
+69686	The-hand-book-of-the-Law-of-Legacies-Tyas-legal-hand-books_69686
+69687	Referent_69687
+69688	Softie_69688
+69689	A-Pal-utcai-fiuk-Regeny-kis-diakok-szamara_69689
+69690	Look-out-for-paint-A-farce-comedy-in-three-acts_69690
+69691	The-West-Riding-Territorials-in-the-Great-War_69691
+69692	Frederick-Douglass_69692
+69693	Life-of-Beethoven-Biographies-of-musicians_69693
+69694	The-Devil-of-East-Lupton-Vermont_69694
+69695	Suudelma-rakkaimmalle_69695
+69696	The-Star-of-India_69696
+69697	Suuri-arvoitus_69697
+69698	The-war-against-Japan-Pictorial-record_69698
+69699	Supplement-to-the-catalogue-of-seals-and-whales-in-the-British-Museum_69699
+69700	The-case-book-of-Sherlock-Holmes_69700
+69701	Antennae_69701
+69702	A-backwoods-princess_69702
+69703	The-master-mind-of-Mars_69703
+69704	The-case-of-Oscar-Slater_69704
+69705	Gardening-for-women_69705
+69706	Proceedings-fourth-National-Conservation-Congress-Indianapolis-October-1-4-1912_69706
+69707	Princess-Sukey-The-story-of-a-pigeon-and-her-human-friends_69707
+69708	The-square-pegs_69708
+69709	Date-line_69709
+69710	The-neutral-merchant_69710
+69711	The-star-dreamer-A-romance_69711
+69712	When-Africa-awakes-The-inside-story-of-the-stirrings-and-strivings-of-the-new-Negro-in-the-We__69712
+69713	Reverse-English_69713
+69714	The-discarded-daughter-Or-the-children-of-the-isle_69714
+69715	The-scarlet-car-the-Princess-Aline_69715
+69716	Life-and-labor-in-the-spirit-world-Being-a-description-of-localities-employments-surroundings__69716
+69717	That-Eurasian_69717
+69718	Tall-tales-of-Cape-Cod_69718
+69719	Galactic-heritage_69719
+69720	Moll-Davis_69720
+69721	The-Flame-Gatherers_69721
+69722	The-shape-of-things_69722
+69723	An-embroidery-book_69723
+69724	At-the-gateways-of-the-day_69724
+69725	Elementary-woodworking_69725
+69726	Lord-Lister-No-0019-De-erfenis-van-Eaglestone_69726
+69727	The-land-of-gold-or-Three-years-in-California_69727
+69728	Authors-at-home-Personal-and-biographical-sketches-of-well-known-American-writers_69728
+69729	Transuranic_69729
+69730	Death-comes-for-the-archbishop_69730
+69731	The-cosmic-jackpot_69731
+69732	The-Review-Vol-1-No-7-July-1911_69732
+69733	Memory_69733
+69734	Lysistrata-or-woman-s-future-and-future-woman_69734
+69735	New-Nick-Carter-weekly-no-197-The-little-glass-vial-or-A-beautiful-blackmailer-brought-to-bay_69735
+69736	Young-Grandison-Vol-2-of-2-A-series-of-letters-from-young-persons-to-their-friends-Translated__69736
+69737	Papa-s-own-girl-A-novel_69737
+69738	A-ven-gazember_69738
+69739	Swiss-Fairy-Tales_69739
+69740	The-Review-Vol-1-No-8-August-1911_69740
+69741	The-house-of-five-gables_69741
+69742	I-like-you-too_69742
+69743	Feuilles-persanes_69743
+69744	A-rablolovag-Szinjatek-harom-felvonasban_69744
+69745	The-Grip-cartoons-vols-I-II-May-1873-to-May-1874_69745
+69746	The-book-of-friendly-giants_69746
+69747	The-gold-rock-of-the-Chippewa_69747
+69748	Lord-Lister-0461-De-moord-op-John-Cormick_69748
+69749	On-to-Pekin-Or-Old-Glory-in-China_69749
+69750	Under-the-periscope_69750
+69751	The-inequality-of-human-races_69751
+69752	A-Year-of-prophesying_69752
+69753	Gulliverin-retket_69753
+69754	Pieni-Runon-seppa_69754
+69755	Women-for-votes_69755
+69756	The-child-s-curiosity-book-embellished-with-cuts_69756
+69757	Dawn-in-darkest-Africa_69757
+69758	Folly-Corner_69758
+69759	The-North-West-Passage-by-land-Being-the-narrative-of-an-expedition-from-the-Atlantic-to-the-__69759
+69760	Brothers-and-sisters_69760
+69761	The-sinking-of-the-Titanic-and-other-poems_69761
+69762	Hellflower_69762
+69763	Kwasa-the-cliff-dweller_69763
+69764	Novum-organon-renovatum_69764
+69765	The-Minoans_69765
+69766	The-training-of-teachers-in-the-United-States-of-America_69766
+69767	All-About-Miniature-Plants-and-Gardens-Indoors-and-Out_69767
+69768	The-bridge-of-San-Luis-Rey_69768
+69769	The-boys-book-of-Indian-battles-and-adventures-with-anecdotes-about-them_69769
+69770	L-Ete-a-l-ombre_69770
+69771	Rabok_69771
+69772	A-Christmas-snowflake-a-rhyme-for-children_69772
+69773	The-long-patrol_69773
+69774	Nature-s-invitation-Notes-of-a-bird-gazer-North-and-South_69774
+69775	Pen-portraits-of-literary-women-Volume-I-of-2-By-themselves-and-others_69775
+69776	Four-little-Blossoms-through-the-holidays_69776
+69777	The-rat-trap_69777
+69778	The-sleeper-is-a-rebel_69778
+69779	Something-about-Eve-A-comedy-of-fig-leaves_69779
+69780	Mrs-Hallams-companion-And-the-spring-farm-and-other-tales_69780
+69781	Frederick-Warne-Co-s-list-of-juvenile-literature-prize-books-and-gift-books-for-young-people_69781
+69782	A-southern-cross-fairy-tale_69782
+69783	A-synopsis-of-the-palms-of-Puerto-Rico_69783
+69784	Shadows-and-sunbeams-Being-a-second-series-of-Fern-leaves-from-Fannys-portfolio_69784
+69785	West-Lawn-and-The-rector-of-St-Marks_69785
+69786	Dreams-and-delights_69786
+69787	The-splendour-of-Asia-The-story-and-teaching-of-the-Buddha_69787
+69788	The-Avenger_69788
+69789	The-fellowship-of-the-Frog_69789
+69790	The-three-Just-Men_69790
+69791	The-testing-of-Janice-Day_69791
+69792	Aatelispesa_69792
+69793	Caught-napping_69793
+69794	De-Pontoise-a-Stamboul-Le-grain-de-plomb-dans-les-ruines-les-0x153ufs-de-Paques-le-jardin-de-__69794
+69795	Der-Moskauer-Proze0xdf-gegen-die-Sozialrevolutionare-1922-Revolution-und-Konterrevolution-Au0__69795
+69796	The-seven-temporary-moons_69796
+69797	Wera-Njedin-Erzahlungen-und-Skizzen_69797
+69798	Smoky-The-cow-horse_69798
+69799	Comedias-tomo-2-de-3-Las-Avispas-la-Paz-las-Aves-Lisistrata_69799
+69800	Christmas-stories_69800
+69801	The-dread-Apache-That-early-day-scourge-of-the-Southwest_69801
+69802	L-Anglais-mangeur-d-opium-Traduit-de-l-Anglais-et-augmente-par-Alfred-de-Musset-avec-une-noti__69802
+69803	AustraliaFortune-land_69803
+69804	Muzsika-Elbeszelesek_69804
+69805	The-Little-Review-April-1916-Vol-3-No-2_69805
+69806	The-Circe-of-the-deserts_69806
+69807	The-mystery-of-Easter-island-the-story-of-an-expedition_69807
+69808	Numa-Roumestan_69808
+69809	For-whose-sake-a-sequel-to-why-did-he-wed-her_69809
+69810	The-Pronunciation-of-Greek_69810
+69811	Ismerosok-Feljegyzesek-kronikak_69811
+69812	Practical-vegetarian-cookery_69812
+69813	Go-she-must_69813
+69814	Campaign-and-battle-of-Lynchburg-Va_69814
+69815	Jane-Austen-s-sailor-brothers-Being-the-adventures-of-Sir-Francis-Austen-GCB-Admiral-of-the-F__69815
+69816	The-works-of-Richard-Hurd-volume-7-of-8_69816
+69817	A-kiss-for-Cinderella-A-comedy_69817
+69818	An-essay-towards-a-natural-history-of-serpents_69818
+69819	No-101_69819
+69820	ClimateIncorporated_69820
+69821	Consulate_69821
+69822	Oskuld-och-arsenik-Analyser_69822
+69823	Public-health-and-insurance-American-addresses_69823
+69824	The-works-of-Richard-Hurd-volume-8-of-8_69824
+69825	An-apology-for-idlers-and-other-essays_69825
+69826	Monarchs-of-minstrelsy-from-Daddy-Rice-to-date_69826
+69827	A-manual-on-the-origin-and-development-of-Washington_69827
+69828	The-bride-s-fate-The-sequel-to-The-changed-brides_69828
+69829	Kuningatar-Dragan-rakkausseikkailut-ja-Kuningas-Aleksanterin-onneton-kohtalo-Historiallinen-r__69829
+69830	My-experiments-with-volcanoes_69830
+69831	A-history-of-the-mathematical-theories-of-attraction-and-the-figure-of-the-earth-from-the-tim__69831
+69832	A-history-of-the-mathematical-theories-of-attraction-and-the-figure-of-the-earth-from-the-tim__69832
+69833	Ahead-of-his-time_69833
+69834	Seven-years-in-Vienna-August-1907-August-1914-a-record-of-intrigue_69834
+69835	The-Negro-and-the-nation_69835
+69836	Down-the-Mackenzie-and-up-the-Yukon-in-1906_69836
+69837	An-index-finger_69837
+69838	Captain-Chap-or-The-Rolling-Stones_69838
+69839	The-Piccinino-Volume-1-of-2_69839
+69840	The-Piccinino-Volume-2-of-2-The-last-of-Aldinis_69840
+69841	The-boy-s-book-of-trades-and-the-tools-used-in-them_69841
+69842	Aegle-and-the-elf-a-fantasy_69842
+69843	Gloriana-or-the-revolution-of-1900_69843
+69844	A-history-of-Italian-painting_69844
+69845	The-club-of-masks_69845
+69846	Encaustic-Or-Count-Caylus-s-method-of-painting-in-the-manner-of-the-ancients-To-which-is-adde__69846
+69847	Travels-through-Central-Africa-to-Timbuctoo-and-across-the-Great-Desert-to-Morocco-performed-__69847
+69848	La-police-secrete-prussienne_69848
+69849	Mr-Arnold-A-romance-of-the-Revolution_69849
+69850	Maantiede-ja-loytoretket-3-Uusin-aika-17-vuosisadan-alusta-nykyaikaan-alkupuoli_69850
+69851	The-medieval-Inquisition-A-study-in-religious-persecution_69851
+69852	Westminster-Abbey-The-last-days-of-the-monastery-as-shown-by-the-life-and-times-of-Abbot-John__69852
+69853	Andor-Regeny_69853
+69854	The-Christmas-Makers-Club_69854
+69855	Letters-sentences-and-maxims_69855
+69856	Orpheus-or-The-music-of-the-future_69856
+69857	Pride-and-Passion-Robert-Burns-1759-1796_69857
+69858	Motherly-talks-with-young-housekeepers-embracing-eighty-seven-brief-articles-on-topics-of-hom__69858
+69859	Table-traits-with-something-on-them_69859
+69860	Medee-tragedie_69860
+69861	Pimeyden-valta-eli-Kun-kynsi-on-kiinni-niin-on-koko-lintu-hukassa-5-naytoksinen-naytelma_69861
+69862	Days-and-hours-in-a-garden_69862
+69863	L-inquiete-adolescence_69863
+69864	Schulmadelgeschichten-fur-Madchen-von-7-12-Jahren_69864
+69865	North-by-night_69865
+69866	Dark-of-the-Moon_69866
+69867	The-Southern-Literary-Messenger-Vol-II-No-8-July-1836_69867
+69868	The-barber-s-chair-and-The-hedgehog-letters_69868
+69869	Harriet-Beecher-Stowe-a-biography-for-girls_69869
+69870	Rose-Mather-A-tale_69870
+69871	Bradford-s-history-of-the-Plymouth-settlement-1608-1650-Rendered-into-modern-English-by-Harol__69871
+69872	Le-monde-de-la-mer_69872
+69873	Cuentos-ilustrados_69873
+69874	Gout-with-a-section-on-ocular-disease-in-the-gouty_69874
+69875	The-windfairies-and-other-tales_69875
+69876	The-ideal-cookery-book-A-reliable-guide-for-home-cooking-containing-249-useful-and-dainty-rec__69876
+69877	The-fire-in-the-flint_69877
+69878	Mappa-de-Portugal-antigo-e-moderno-tomo-1-of-3-Parte-I-II_69878
+69879	Newer-ideals-of-peace_69879
+69880	The-valley-of-Arcana_69880
+69881	Preservation-of-forests-as-a-measure-of-public-safety-Address-before-the-17th-National-Irriga__69881
+69882	Adventures-in-indigence-and-other-essays_69882
+69883	Aamutuuli-Runoja_69883
+69884	Uittomiehia-ja-kullankaivajia_69884
+69885	The-extraordinary-confessions-of-Diana-Please_69885
+69886	Famous-pets-of-famous-people_69886
+69887	Considerations-politiques-sur-les-coups-d-estat_69887
+69888	The-instinct-of-workmanship-and-the-state-of-industrial-arts_69888
+69889	Anecdotes-and-memoirs-of-William-Boen-a-coloured-man-who-lived-and-died-near-Mount-Holly-New-__69889
+69890	The-golden-bridle_69890
+69891	Les-liaisons-dangereuses-volume-1-of-2-or-letters-collected-in-a-private-society-and-publishe__69891
+69892	Zetetic-astronomy-Earth-not-a-globe-An-experimental-inquiry-into-the-true-figure-of-the-earth__69892
+69893	Deutsche-und-Franzosische-Orgelbaukunst-und-Orgelkunst_69893
+69894	Allerhand-Sprachdummheiten-Kleine-deutsche-Grammatik-des-Zweifelhaften-des-Falschen-und-des-H__69894
+69895	The-farm-and-the-woodlot_69895
+69896	The-book-of-the-child-An-attempt-to-set-down-what-is-in-the-mind-of-children_69896
+69897	Women-artists-in-all-ages-and-countries_69897
+69898	Cronica-di-Matteo-Villani-vol-I-A-miglior-lezione-ridotta-coll-aiuto-de-testi-a-penna_69898
+69899	Cronica-di-Matteo-Villani-vol-II-A-miglior-lezione-ridotta-coll-aiuto-de-testi-a-penna_69899
+69900	Cronica-di-Matteo-Villani-vol-III-A-miglior-lezione-ridotta-coll-aiuto-de-testi-a-penna_69900
+69901	Cronica-di-Matteo-Villani-vol-IV-A-miglior-lezione-ridotta-coll-aiuto-de-testi-a-penna_69901
+69902	Cronica-di-Matteo-Villani-vol-V-A-miglior-lezione-ridotta-coll-aiuto-de-testi-a-penna_69902
+69903	Deutsche-Nordseekuste-Friesische-Inseln-und-Helgoland_69903
+69904	Animal-intelligence-Experimental-studies_69904
+69905	Sparlakanslaxor_69905
+69906	Through-lands-that-were-dark_69906
+69907	A-Viking-s-love-and-other-tales-of-the-North_69907
+69908	The-Review-Vol-1-No-11-November-1911_69908
+69909	Cork-Being-the-story-of-the-origin-of-cork-the-processes-employed-in-its-manufacture-its-vari__69909
+69910	The-cranberry_69910
+69911	War-against-Germany-and-Italy-Mediterranean-and-adjacent-areas-pictorial-record_69911
+69912	The-Popish-Plot-A-study-in-the-history-of-the-reign-of-Charles-II_69912
+69913	Les-liaisons-dangereuses-volume-2-of-2-or-letters-collected-in-a-private-society-and-publishe__69913
+69914	An-elementary-treatise-on-electricity_69914
+69915	Reflexions-pour-les-fermiers-generaux-des-messageries_69915
+69916	The-last-space-ship_69916
+69917	La-legende-doree-traduite-du-latin-d-apres-les-plus-anciens-manuscrits-avec-une-introduction-__69917
+69918	Souvenirs-de-la-Cour-d-Assises_69918
+69919	The-foxholes-of-Mars_69919
+69920	Holly-The-Romance-of-a-Southern-Girl_69920
+69921	Schizophrenic_69921
+69922	Dairying-exemplified-or-The-business-of-cheese-making-the-second-edition-corrected-and-improv__69922
+69923	Fuzzy-Wuzz-a-little-brown-bear-of-the-Sierras_69923
+69924	A-list-of-books-published-by-Chatto-Windus_69924
+69925	The-new-northland_69925
+69926	Papa-knows-best_69926
+69927	Case-of-Filaria-loa_69927
+69928	My-fight-for-Irish-freedom_69928
+69929	The-cowboy-and-the-lady-and-her-pa-b-A-story-of-a-fish-out-of-water_69929
+69930	The-unconscious-b-The-fundamentals-of-human-personality-normal-and-abnormal_69930
+69931	Fuzzy-head_69931
+69932	A-horse-on-me_69932
+69933	Kuninkaitten-kuningas_69933
+69934	Early-British-Trackways-Moats-Mounds-Camps-and-Sites_69934
+69935	The-Safety-First-Club_69935
+69936	Les-miens_69936
+69937	Shakespeare-s-Roman-Plays-and-Their-Background_69937
+69938	Told-in-the-twilight_69938
+69939	Essays-in-medical-sociology-Volume-I-of-2_69939
+69940	The-ionian-cycle_69940
+69941	Tarua-ja-totta-elamastani-I-b-Kirjat-I-V_69941
+69942	Tarua-ja-totta-elamastani-II-b-Kirjat-VI-X_69942
+69943	The-training-of-an-infantry-company_69943
+69944	Jud-Su0xdf_69944
+69945	Tahiti-the-island-paradise_69945
+69946	The-wolf-trail_69946
+69947	Flowering-plants-of-South-Africa-vol-4_69947
+69948	Diccionario-Espanol-Bisaya-b-Segunda-edicion_69948
+69949	Turkische-Marchen_69949
+69950	Reminiscences-of-the-Cleveland-Light-Artillery_69950
+69951	Divinas-palabras-b-Tragicomedia-de-aldea_69951
+69952	Leonard-Lindsay-b-or-the-story-of-a-buccaneer_69952
+69953	Life-and-writings-of-Amelia-Bloomer_69953
+69954	The-Cameron-pride-b-or-purified-by-suffering_69954
+69955	Was-it-a-ghost-The-murders-in-Bussey-s-wood-b-An-extraordinary-narrative_69955
+69956	Daily-stories-of-Pennsylvania-b-prepared-for-publication-in-the-leading-daily-newspapers-of-t__69956
+69957	Finding-Youth-b-A-human-experience_69957
+69958	The-factory_69958
+69959	Your-vote-and-how-to-use-it_69959
+69960	Abendfalter-b-Geschichten-der-Sehnsucht_69960
+69961	The-story-of-my-house_69961
+69962	The-virgin-of-the-sun-b-A-play-in-five-acts_69962
+69963	Isaac-Watts-his-life-and-writings-his-homes-and-friends_69963
+69964	History-of-the-war-in-the-Peninsula-and-in-the-south-of-France-from-the-year-1807-to-the-year__69964
+69965	Horrors-of-vaccination-exposed-and-illustrated-b-Petition-to-the-President-to-abolish-compuls__69965
+69966	The-Yale-Literary-Magazine-Vol-LXXXIX-No-1-1923_69966
+69967	Kyla-ja-kaupunki-b-Laatukuvia_69967
+69968	Frank-Allen-at-Gold-Fork-b-Locating-the-Lost-Claim_69968
+69969	The-golden-whales-of-California-and-other-rhymes-in-the-American-language_69969
+69970	The-English-Husbandman-The-Second-Booke-b-Contayning-the-Ordering-of-the-Kitchin-Garden-and-t__69970
+69971	The-Swiss-Republic_69971
+69972	The-changed-brides_69972
+69973	Ingleside-b-or-Without-Christ-and-With-Him_69973
+69974	Star-Book-No-189-Fashion-Parade-knit-and-crochet-for-him-and-her_69974
+69975	Linotype-mechanism_69975
+69976	All-about-Little-Boy-Blue_69976
+69977	Onkel-Tom-s-Hutte-b-oder-die-Geschichte-eines-christlichen-Sklaven_69977
+69978	Types-of-prehistoric-Southwestern-architecture_69978
+69979	Star-Book-No-225-Aunt-Lydia-s-Rug-Yarn-Collection_69979
+69980	Yanks-b-AEF-verse-originally-published-in-The-Stars-and-Stripes-the-official-newspaper-of-the__69980
+69981	Storia-degli-Italiani-vol-8-di-15_69981
+69982	La-cocarde-rouge_69982
+69983	An-original-theory-or-new-hypothesis-of-the-Universe_69983
+69984	The-mystery-of-Central-Park_69984
+69985	Ilex-cassine-the-Aboriginal-North-American-tea-b-Its-history-distribution-and-use-among-the-N__69985
+69986	The-highland-bagpipe-b-its-history-literature-and-music-with-some-account-of-the-traditions-s__69986
+69987	Star-book-no-234-mood-fashions_69987
+69988	The-house-on-the-cliff_69988
+69989	Handicraft-for-boys_69989
+69990	A-month-in-Switzerland_69990
+69991	Stock-and-stalks-b-A-book-for-the-dairy-farmer_69991
+69992	The-botanist-s-repository-for-new-and-rare-plants-vols-1-2_69992
+69993	Ireland-s-disease_69993
+69994	The-triumphs-of-perseverance-and-enterprise_69994
+69995	Report-on-the-lands-of-the-arid-region-of-the-United-States-with-a-more-detailed-account-of-t__69995
+69996	The-dawn-in-Russia_69996
+69997	La-vita-che-ti-diedi_69997
+69998	Essays-in-medical-sociology-Volume-2-of-2_69998
+69999	Jigsaw_69999
+70000	Wakeman-s-handbook-of-Irish-antiquities-b-Third-Edition_70000
+70001	Metamorphosis_70001
+70002	The-eternal-savage_70002
+70003	Flight-Eighteen_70003
+70004	Raggety-b-His-life-and-adventures_70004
+70005	If-at-first_70005
+70006	The-hermit-thrush_70006
+70007	Omistani-ja-omilleni_70007
+70008	Unnatural-death_70008
+70009	The-plurality-of-the-human-race_70009
+70010	The-shadow-between-them-b-or-A-blighted-name_70010
+70011	Travels-through-Central-Africa-to-Timbuctoo-and-across-the-Great-Desert-to-Morocco-performed-__70011
+70012	Moon-dust_70012
+70013	Acoustics-of-auditoriums-b-University-of-Illinois-Bulletin-Vol-XI-March-16-1914-No-29_70013
+70014	How-to-paint-permanent-pictures_70014
+70015	The-Trans-Galactic-Twins_70015
+70016	A-new-Robinson-Crusoe_70016
+70017	Uncle-Wiggily-on-roller-skates-b-Or-What-happened-when-the-skillery-skallery-alligator-gave-c__70017
+70018	Some-architectural-problems-of-to-day_70018
+70019	The-female-impersonators-b-A-sequel-to-the-autobiography-of-an-androgyne-and-an-account-of-so__70019
+70020	La-spada-di-fuoco_70020
+70021	Edna-Browning-b-or-the-Leighton-homestead-A-novel_70021
+70022	Deck-and-port-b-or-incidents-of-a-cruise-in-the-United-States-frigate-Congress-to-California-__70022
+70023	The-reigning-belle-b-A-society-novel_70023
+70024	The-old-man-s-guide-to-health-and-longer-life-b-With-rules-for-diet-exercise-and-physic-for-p__70024
+70025	Gora-I-b-Romaani_70025
+70026	A-world-of-green-hills-b-Observations-of-nature-and-human-nature-in-the-Blue-Ridge_70026
+70027	Az-orias-es-egyeb-elbeszelesek_70027
+70028	A-Catalogue-of-Remarkable-Books-published-by-Mr-George-Redway-1887_70028
+70029	Biography-and-bibliography-of-Jesse-Walter-Fewkes_70029
+70030	Off-the-Bluebush-b-Verses-for-Australians-West-and-East_70030
+70031	The-Women-of-the-Mayflower-and-Women-of-Plymouth-Colony_70031
+70032	Zanzibar-City-Island-and-Coast-Vol-2-of-2_70032
+70033	The-history-of-magic-b-including-a-clear-and-precise-exposition-of-its-procedure-its-rites-an__70033
+70034	The-stainless-steel-rat_70034
+70035	Syria-the-land-of-Lebanon_70035
+70036	Governor-William-Bradford-s-letter-book_70036
+70037	The-fog_70037
+70038	Freak-trees-of-the-State-of-New-York_70038
+70039	First-harvests-an-episode-in-the-life-of-Mrs-Levison-Gower-b-A-satire-without-a-moral_70039
+70040	Practical-recitations-b-Selections-for-literary-exercises-appropriate-for-reception-days-holi__70040
+70041	The-small-bachelor_70041
+70042	Des-paquebots-transatlantiques-b-BrestLe-HavreCherbourgMarseilleParisNantesBordeaux_70042
+70043	Pimean-kammion-kuningas-ja-muita-draamoja_70043
+70044	Der-Schandfleck-b-Eine-Dorfgeschichte_70044
+70045	Coloured-engravings-of-heaths-vol-2_70045
+70046	A-guide-to-Plymouth-and-its-history_70046
+70047	The-peaceful-atom_70047
+70048	The-great-Skene-mystery_70048
+70049	Egyptian-decorative-art-b-A-course-of-lectures-delivered-at-the-Royal-Institution_70049
+70050	Racehorses-in-Australia_70050
+70051	Gambler-s-dollar_70051
+70052	Ancient-calendars-and-constellations_70052
+70053	Capelli-biondi_70053
+70054	Nummer-Elf-b-Oorspronkelijke-roman_70054
+70055	Satan-s-Invisible-World-Discovered-b-or-a-choice-collection-of-modern-relations-proving-evide__70055
+70056	Historical-record-of-the-71st-Regiment-Highland-Light-Infantry-b-from-its-formation-in-1777-u__70056
+70057	Koti-ja-maailma_70057
+70058	Origenes-de-la-novela-Tomo-I_70058
+70059	Hidden-blood_70059
+70060	Paul-Bunyan_70060
+70061	En-avion-vers-le-pole-nord_70061
+70062	Coloured-engravings-of-heaths-vol-3_70062
+70063	Lord-Lister-No-0115-Een-Sinterklaas-verrassing_70063
+70064	Estudios-americanos-primera-serie_70064
+70065	La-fleche-noire_70065
+70066	Twenty-years-a-fakir_70066
+70067	Cheese-and-its-economical-uses-in-the-diet_70067
+70068	Good-housing-that-pays-b-A-study-of-the-aims-and-the-accomplishment-of-the-Octavia-Hill-Assoc__70068
+70069	A-little-child_70069
+70070	Prose-remains-of-Arthur-Hugh-Clough-with-a-selection-from-his-letters-and-a-memoir_70070
+70071	Ames-inconnues-b-Notes-intimes-d-un-seminariste_70071
+70072	Coloured-engravings-of-heaths-vol-4_70072
+70073	Caprice_70073
+70074	Invisible-helpers_70074
+70075	Palm-trees-of-the-Amazon-and-their-uses_70075
+70076	The-Tusayan-ritual-b-A-study-on-the-influence-of-environment-on-aboriginal-cults_70076
+70077	Beyond-the-sunset_70077
+70078	The-heathery-or-A-monograph-of-the-genus-Erica-vol-2_70078
+70079	Architecture-b-nineteenth-and-twentieth-centuries_70079
+70080	Buzzards-know_70080
+70081	La-fleur-d-or_70081
+70082	The-heathery-or-A-monograph-of-the-genus-Erica-vol-3_70082
+70083	The-tower-treasure_70083
+70084	Une-annee-au-desert-b-Scenes-et-recits-du-Far-West-americain_70084
+70085	The-heathery-or-A-monograph-of-the-genus-Erica-vol-4_70085
+70086	Sketch-of-the-Reformation-in-England_70086
+70087	Winona-b-A-tale-of-Negro-life-in-the-South-and-Southwest_70087
+70088	Le-cycle-du-printemps_70088
+70089	Drifted-ashore-b-or-a-child-without-a-name_70089
+70090	The-little-elves-seeking-the-beautiful-world-b-A-book-for-children_70090
+70091	Six-metaphysical-meditations-b-Wherein-it-is-proved-that-there-is-a-God-and-that-mans-mind-is__70091
+70092	The-treatise-of-Lorenzo-Valla-on-the-Donation-of-Constantine_70092
+70093	The-heathery-or-A-monograph-of-the-genus-Erica-vol-5_70093
+70094	Itineraires_70094
+70095	Le-Negre-du-Narcisse_70095
+70096	The-heathery-or-A-monograph-of-the-genus-Erica-vol-6_70096
+70097	A-new-note-in-the-Christmas-Carol_70097
+70098	Handbook-of-Old-Burial-Hill-Plymouth-Massachusetts-b-its-history-its-famous-dead-and-its-quai__70098
+70099	Petition-and-memorial-of-David-Quinn-asking-for-the-re-establishment-of-Negro-slavery-in-the-__70099
+70100	The-turner-s-companion-b-containing-instructions-in-concentric-elliptic-and-eccentric-turning__70100
+70101	Apache-devil_70101
+70102	Adam-Eve-et-Brid-oison_70102
+70103	Chantemerle-b-A-romance-of-the-Vendean-War_70103
+70104	The-doctor-c-vol-3-of-7_70104
+70105	Gilead-Balm-knight-errant-b-His-adventures-in-search-of-the-truth_70105
+70106	Dymer_70106
+70107	The-free-press-b-portrait-of-a-monopoly_70107
+70108	The-Y-M-C-A-boys-of-Cliffwood-b-or-The-struggle-for-the-Holwell-Prize_70108
+70109	Historic-Jamaica_70109
+70110	A-West-Pointer-with-the-Boers-b-personal-narrative-of-Colonel-J-Y-F-Blake-commander-of-the-Ir__70110
+70111	New-England-s-rarities-discovered-b-In-birds-beasts-fishes-serpents-and-plants-of-that-countr__70111
+70112	Naisen-mahti_70112
+70113	Thirty-years-in-Madagascar_70113
+70114	The-Big-Four_70114
+70115	The-Creator-and-what-we-may-know-of-the-method-of-creation_70115
+70116	The-Safety-First-Club-fights-fire_70116
+70117	Mon-corps-et-moi_70117
+70118	In-Cupid-s-court_70118
+70119	Concerning-the-bi-literal-cypher-of-Francis-Bacon-discovered-in-his-works_70119
+70120	The-Blackguard_70120
+70121	A-capital-federal-impressoes-de-um-sertanejo_70121
+70122	The-conquest-of-the-great-Northwest-Volume-2-of-2-b-Being-the-story-of-the-adventurers-of-Eng__70122
+70123	A-Yankee-in-Canada-with-Anti-slavery-and-reform-papers_70123
+70124	The-war-chief_70124
+70125	Mexican-letters-written-during-the-progress-of-the-late-war-between-the-United-States-and-Mex__70125
+70126	Nene_70126
+70127	Federico-Lennois-b-romanzo_70127
+70128	Max-Havelaar-b-or-the-coffee-auctions-of-the-Dutch-trading-company_70128
+70129	General-Washington-s-spies-on-Long-Island-and-in-New-York_70129
+70130	To-Panama-and-back-b-The-record-of-an-experience_70130
+70131	How-he-won-her-b-A-sequel-to-Fair-play_70131
+70132	Mezzotints-in-modern-music-b-Brahms-Tschaikowsky-Chopin-Richard-Strauss-Liszt-and-Wagner_70132
+70133	The-suppression-of-tuberculosis-b-Together-with-observations-concerning-phthisiogenesis-in-ma__70133
+70134	The-curse-of-gold_70134
+70135	The-lost-oases_70135
+70136	Islam_70136
+70137	Little-Mother-Goose_70137
+70138	Wanderings-of-a-beauty-b-A-tale-of-the-real-and-the-ideal_70138
+70139	A-bitter-reckoning-b-or-Violet-Arleigh_70139
+70140	The-early-English-cotton-industry_70140
+70141	Pikku-Pietari_70141
+70142	The-story-of-Santa-Klaus-b-Told-for-children-of-all-ages-from-six-to-sixty_70142
+70143	Frank-Allen-at-Old-Moose-Lake-b-or-The-trail-in-the-snow_70143
+70144	Mes-cahiers-rouges-au-temps-de-la-Commune_70144
+70145	The-marrying-monster_70145
+70146	The-perverse-Erse_70146
+70147	The-psychology-of-the-poet-Shelley_70147
+70148	Time-for-survival_70148
+70149	Under-England-s-flag-b-from-1804-1809-the-memoirs-diary-and-correspondence-of-Charles-Boothy-__70149
+70150	An-A-B-C-of-every-day-people-b-Good-bad-indifferent_70150
+70151	Myra-b-the-child-of-adoption-A-romance-of-real-life_70151
+70152	The-Hungry-Tiger-of-Oz_70152
+70153	Historia-del-levantamiento-guerra-y-revolucion-de-Espana-5-de-5_70153
+70154	Murderer-s-chain_70154
+70155	Sibling_70155
+70156	The-house-of-the-wizard_70156
+70157	The-Vinegar-Saint_70157
+70158	Beast-of-prey_70158
+70159	The-little-Barefoot-b-A-tale_70159
+70160	Bombs-awry_70160
+70161	Isolee_70161
+70162	L-ange-du-bizarre_70162
+70163	Millbank-b-or-Roger-Irving-s-ward-A-novel_70163
+70164	The-best-vegetarian-dishes-I-know_70164
+70165	Elizabeth-Hooton-b-First-Quaker-woman-preacher-1600-1672_70165
+70166	The-Katcina-altars-in-Hopi-worship_70166
+70167	The-horrors-of-the-Negro-slavery-existing-in-our-West-Indian-Islands-irrefragably-demonstrate__70167
+70168	Up-the-ladder-b-or-striving-and-thriving_70168
+70169	Harness-making_70169
+70170	Three-years-in-field-hospitals-of-the-Army-of-the-Potomac_70170
+70171	North-Africa-and-the-desert-b-Scenes-and-moods_70171
+70172	Catherine-s-coquetries-b-A-tale-of-French-country-life_70172
+70173	Arbiter_70173
+70174	Madam-Constantia-b-The-romance-of-a-prisoner-of-war-in-the-revolution-South-Carolina_70174
+70175	The-secret-of-Father-Brown_70175
+70176	The-history-of-steam-navigation_70176
+70177	Gora-II_70177
+70178	Ri-Ra-Rutsch-b-Alte-und-neue-Kinderreime_70178
+70179	English-spelling-and-spelling-reform_70179
+70180	Twenty-years-around-the-world_70180
+70181	Fors-Clavigera-Volume-6-of-8-b-Letters-to-the-workmen-and-labourers-of-Great-Britain_70181
+70182	Tom-Swift-and-his-flying-boat-b-Or-The-castaways-of-the-giant-iceberg_70182
+70183	The-dreamers_70183
+70184	Daughter_70184
+70185	Chateau-d-Or-b-Norah-and-Kitty-Craig_70185
+70186	Dans-l-ombre-chaude-de-l-Islam_70186
+70187	240-000-miles-straight-up_70187
+70188	Advertising-by-motion-pictures_70188
+70189	The-sensitive-plant_70189
+70190	The-Yale-literary-magazine-Vol-LXXXIX-No-3-December-1923_70190
+70191	Glen-s-Creek_70191
+70192	Where-the-forest-murmurs-b-Nature-essays_70192
+70193	With-Washington-in-the-west-b-A-soldier-boy-s-battles-in-the-wilderness_70193
+70194	Motor-car-principles-the-gasoline-automobile_70194
+70195	Pirates-of-Venus_70195
+70196	Evil-eye-in-the-Western-Highlands_70196
+70197	Captain-Kodak-b-A-camera-story-third-edition_70197
+70198	Seven-Xmas-Eves-b-Being-the-romance-of-a-social-evolution_70198
+70199	Tanar-of-Pellucidar_70199
+70200	Pen-portraits-of-literary-women-Volume-II-of-2-b-By-themselves-and-others_70200
+70201	Chasseurs-de-nomades_70201
+70202	Le-parfum-de-la-Dame-Noire-b-Physiologie-humoristique-de-l-amour-Africain_70202
+70203	The-story-of-chamber-music_70203
+70204	Confederate-wizards-of-the-saddle_70204
+70205	Designs-for-Crazy-Daisy-Winder-b-Crochet-Time-Cut-in-Half_70205
+70206	The-carriages-at-Shelburne-Museum-b-Museum-pamphlet-series-no-1_70206
+70207	The-man-with-the-iron-mask_70207
+70208	La-vendetta-di-Zoe-b-Aristocrazia-I_70208
+70209	Bird-in-Hand_70209
+70210	A-Select-Glossary-of-English-words-used-formerly-in-senses-different-from-their-present_70210
+70211	At-Hotel-On-de-Blink-b-An-Entertainment-in-Two-Parts_70211
+70212	The-agile-Algolian_70212
+70213	Yashka-b-My-life-as-peasant-exile-and-soldier_70213
+70214	Peeps-at-many-lands-Wales_70214
+70215	The-belly-of-Gor-Jeetl_70215
+70216	Booby-prize_70216
+70217	Bruggil-s-bride_70217
+70218	The-gadget-had-a-ghost_70218
+70219	Historia-natural-y-moral-de-las-Indias-vol-1-of-2_70219
+70220	Mary-Derwent-b-a-tale-of-Wyoming-and-Mohawk-Valleys-in-1778_70220
+70221	Through-Timbuctu-and-across-the-great-Sahara-b-an-account-of-an-adventurous-journey-of-explor__70221
+70222	Meet-Mr-Mulliner_70222
+70223	Two-Colored-Women-with-the-American-Expeditionary-Forces_70223
+70224	The-chariot-of-the-sun_70224
+70225	The-Fortunate-Calamity_70225
+70226	Carpentry_70226
+70227	The-Mobius-trail_70227
+70228	Book-No-173-old-and-new-favorites-crochet-designs-b-Nation-wide-favorites-repeated-by-request__70228
+70229	Indian-types-of-beauty_70229
+70230	The-ghost-planet_70230
+70231	Everyday-experiences_70231
+70232	Aristocracy-in-America-vol-II-of-2-b-from-the-sketch-book-of-a-German-nobleman_70232
+70233	The-duplicate-death_70233
+70234	Hugh-Worthington-b-A-novel_70234
+70235	The-expendables_70235
+70236	The-secret-of-the-old-mill_70236
+70237	The-unlit-lamp-b-A-study-in-inter-actions_70237
+70238	Valittuja-kertomuksia_70238
+70239	Whistle-stop-in-space_70239
+70240	Fruits-of-the-agathon_70240
+70241	La-meilleure-part_70241
+70242	Prize-ship_70242
+70243	Labour-policyfalse-and-true-b-A-study-in-economic-history-and-industrial-economics_70243
+70244	Studies-of-contemporary-American-composers-Deems-Taylor_70244
+70245	Chambers-s-journal-of-popular-literature-science-and-art-fifth-series-no-119-vol-III-April-4-__70245
+70246	Wir-ritten-fur-Deutsch-Ostafrika_70246
+70247	Second-landing_70247
+70248	Nur-wer-die-Sehnsucht-kennt-_70248
+70249	Uncle-Jo-s-Old-Coat_70249
+70250	The-moon-that-vanished_70250
+70251	Yesterday-s-doors_70251
+70252	Threads-gathered-up-b-A-sequel-to-Virgie-s-Inheritance_70252
+70253	James-Sherman-Kimball-b-A-Sketch_70253
+70254	Bedouins_70254
+70255	Fancy-free_70255
+70256	Virginia-b-Vapaista-metsista-tarina_70256
+70257	Mr-Zytztz-goes-to-Mars_70257
+70258	The-last-age-of-the-church_70258
+70259	Season-s-best-dishes-b-for-2-or-4-or-6_70259
+70260	0x152uvres-completes-de-Gustave-Flaubert-tome-8_70260
+70261	Tannhauser-b-A-Story-of-all-time_70261
+70262	The-tithe_70262
+70263	Daughter-of-the-sky-b-The-story-of-Amelia-Earhart_70263
+70264	Women-as-army-surgeons-b-Being-the-history-of-the-Women-s-Hospital-Corps-in-Paris-Wimereux-an__70264
+70265	The-pot-of-basil_70265
+70266	Lyrical-tales_70266
+70267	The-condition-of-England_70267
+70268	Du-Diable-a-Dieu-b-Histoire-d-une-conversion_70268
+70269	A-Hoosier-holiday_70269
+70270	In-Exitu-Israel-Volume-2-of-2-b-An-Historic-Novel_70270
+70271	When-we-were-very-young_70271
+70272	The-theory-of-relativity-and-its-influence-on-scientific-thought_70272
+70273	The-Boy-who-Brought-Christmas_70273
+70274	Inger-Johanne-s-Lively-Doings_70274
+70275	Mrs-Gurney-s-apology-b-In-justification-of-Mrs-s-friendship_70275
+70276	Pottery-decoration-under-the-glaze_70276
+70277	Med-service_70277
+70278	Chambers-s-Journal-of-Popular-Literature-Science-and-Art-fifth-series-no-120-vol-III-April-17__70278
+70279	Bertha-Weisser-s-Wish-b-A-Christmas-Story_70279
+70280	The-Story-of-the-Congo-Free-State-b-Racial-Political-and-Economic-Aspects-of-the-Belgian-Syst__70280
+70281	St-Domingo-its-revolution-and-its-hero-Toussaint-Louverture_70281
+70282	Ella-a-little-schoolgirl-of-the-sixties-b-A-book-for-children-and-for-grown-ups-who-remember_70282
+70283	Is-it-I-A-book-for-every-man_70283
+70284	Dream-Tapestries_70284
+70285	The-Snow-Man-b-A-metrical-play-in-one-act_70285
+70286	From-flag-to-flag-b-A-woman-s-adventures-and-experiences-in-the-South-during-the-War-in-Mexic__70286
+70287	Algeria-from-within_70287
+70288	Conjure-Wife_70288
+70289	Corduroy_70289
+70290	The-adventures-of-Hatim-Tai-a-romance_70290
+70291	X-mas-Sketches-from-the-Dartmouth-Literary-Monthly_70291
+70292	Least-Said-Soonest-Mended_70292
+70293	The-old-South-b-A-monograph_70293
+70294	The-first-church-s-Christmas-barrel_70294
+70295	Uncle-Wiggily-s-Airship-b-Bedtime-Stories_70295
+70296	Kapellendorf-b-Roman_70296
+70297	Merihaukka_70297
+70298	The-deformities-of-the-fingers-and-toes_70298
+70299	L-impudente_70299
+70300	Legendary-romantic-tales-of-Indian-history_70300
+70301	My-leper-friends-b-An-account-of-personal-work-among-lepers-and-of-their-daily-life-in-India_70301
+70302	Education-and-the-good-life_70302
+70303	Valkoisella-kivella_70303
+70304	The-Inquisition-b-a-political-and-military-study-of-its-establishment_70304
+70305	Torwood-s-trust-Vol-1-of-3-b-A-novel_70305
+70306	Torwood-s-trust-Vol-2-of-3-b-A-novel_70306
+70307	Torwood-s-trust-Vol-3-of-3-b-A-novel_70307
+70308	On-the-mechanism-of-the-physiological-action-of-the-cathartics_70308
+70309	Songs-of-the-Slav-b-Translations-from-the-Czecho-Slovak_70309
+70310	The-starmen_70310
+70311	Uusia-maailmoita-vanhojen-sijaan_70311
+70312	Histoire-de-ma-jeunesse_70312
+70313	American-nights-entertainment_70313
+70314	English-monasteries-b-From-Saxon-days-to-their-dissolution_70314
+70315	The-old-lady-shows-her-medals_70315
+70316	Thamyris-b-or-Is-there-a-future-for-poetry_70316
+70317	Landesverein-Sachsischer-Heimatschutz-Mitteilungen-Band-XII-Heft-4-6-b-Monatsschrift-fur-Heim__70317
+70318	Indian-Nature-Myths_70318
+70319	Les-Sources_70319
+70320	The-Navy-of-the-American-revolution-b-Its-administration-its-policy-and-its-achievements_70320
+70321	The-Riddle-Club-at-Sunrise-Beach-b-How-they-toured-to-the-shore-what-happened-on-the-sand-and__70321
+70322	Amor-y-llanto_70322
+70323	Exploration-of-Air-b-Out-of-the-world-north-of-Nigeria_70323
+70324	The-lonely-plough_70324
+70325	Mary-Christmas_70325
+70326	The-art-of-preserving-health-A-poem_70326
+70327	Panouille_70327
+70328	Bobby-and-Betty-with-the-workers_70328
+70329	Arctic-exploration_70329
+70330	The-essentials-of-bandaging_70330
+70331	Educational-laws-of-Virginia-b-The-personal-narrative-of-Mrs-Margaret-Douglass-a-southern-wom__70331
+70332	The-declaration-and-confession-of-Robert-Watt-b-Written-subscribed-delivered-by-himself-the-e__70332
+70333	Dress-and-care-of-the-feet-b-showing-their-natural-shape-and-construction-their-usual-distort__70333
+70334	The-moat-house-b-or-Sir-Jasper-s-favourite-niece_70334
+70335	La-peste-di-Milano-del-1630_70335
+70336	Herinneringen-van-Dr-Aletta-H-Jacobs_70336
+70337	Lord-Lister-No-0356-Het-verdrag-met-de-Oekraine_70337
+70338	Paper-paper-making-b-ancient-and-modern_70338
+70339	Furniture-upholstery-for-schools_70339
+70340	Images-exotiques-et-francaises_70340
+70341	Moo-cow-tales_70341
+70342	Trials-of-war-criminals-before-the-Nuernberg-military-tribunals-under-control-council-law-no-__70342
+70343	A-scheme-there-was_70343
+70344	Odds-and-ends_70344
+70345	A-constitutional-league-of-peace-in-the-stone-age-of-America-b-The-league-of-the-Iroquois-and__70345
+70346	The-Alosaka-cult-of-the-Hopi-Indians_70346
+70347	Momentum_70347
+70348	Imitation-of-death_70348
+70349	When-the-squadron-dropped-anchor_70349
+70350	Dr-B-Mure-s-materia-medica-b-or-provings-of-the-principal-animal-and-vegetable-poisons-of-the__70350
+70351	Tante-Million_70351
+70352	Sir-Christopher-Wren-b-Scientist-scholar-and-architect_70352
+70353	Zwanzig-Jahre-an-Indischen-Furstenhofen-b-Indisches-und-Allzu-Indisches_70353
+70354	Notes-de-route-b-MarocAlgerieTunisie_70354
+70355	Rupertsweiler-Leut_70355
+70356	Heroes-of-science-b-Botanists-zoologists-and-geologists_70356
+70357	The-Jumano-Indians_70357
+70358	Bunny-Brown-and-his-sister-Sue-and-their-trick-dog_70358
+70359	The-history-of-the-damnable-life-and-deserved-death-of-Doctor-John-Faustus-1592-together-with__70359
+70360	A-Cathcart-or-a-Riggs_70360
+70361	The-terror_70361
+70362	Kaunis-ystava_70362
+70363	Les-amours-de-Faustine-b-Poesies-latines-traduites-pour-la-premiere-fois-et-publiees-avec-une__70363
+70364	And-there-was-light_70364
+70365	Chambers-s-Journal-of-Popular-Literature-Science-and-Art-fifth-series-no-121-vol-III-April-24__70365
+70366	Antiquities-of-the-Mesa-Verde-National-Park-b-Spruce-tree-House_70366
+70367	Accounting-theory-and-practice-Volume-1-of-3-b-a-textbook-for-colleges-and-schools-of-busines__70367
+70368	Washington-cover-up_70368
+70369	Monsieur-Barbe-Bleue-et-Madame_70369
+70370	Lord-Lister-No-0020-De-bloeddorstige_70370
+70371	Colas-Breugnon_70371
+70372	Chambers-s-journal-of-popular-literature-science-and-art-fifth-series-no-122-vol-III-May-1-18__70372
+70373	Our-Arctic-province-b-Alaska-and-the-Seal-Islands_70373
+70374	The-Burlington-magazine-b-for-connoisseurs-vol-IIJune-to-August_70374
+70375	Discoveries-in-Egypt-Ethiopia-and-the-peninsula-of-Sinai-in-the-years-1842-1845-during-the-mi__70375
+70376	Il-segreto-di-Matteo-Arpione-b-Aristocrazia-II_70376
+70377	Fifty-years-in-Wall-Street_70377
+70378	Twelve-months-in-Madagascar_70378
+70379	Oil-b-A-novel_70379
+70380	The-Land-Water-edition-of-Raemaekers-cartoons-volume-1_70380
+70381	The-Abbey-of-St-Albans-from-1300-to-the-dissolution-of-the-monasteries-b-The-Stanhope-essay-1__70381
+70382	The-music-of-the-spheres-b-A-nature-lover-s-astronomy_70382
+70383	Combat-lessons-no-1-rank-and-file-in-combat-b-What-they-are-doing-how-they-do-it_70383
+70384	Arthur-b-A-tragedy_70384
+70385	South-Australia-and-Western-Australia_70385
+70386	Chambers-s-Journal-of-Popular-Literature-Science-and-Art-fifth-series-no-123-vol-III-May-8-18__70386
+70387	Parking-unlimited_70387
+70388	Remember-the-4th_70388
+70389	Two-worlds-for-one_70389
+70390	The-monster-hunters_70390
+70391	Martians-keep-out_70391
+70392	Nobody-saw-the-ship_70392
+70393	Prejudices_70393
+70394	Travels-in-the-Upper-Egyptian-deserts_70394
+70395	De-zwervers-op-de-grenzen-b-Naar-de-achtste-Fransche-uitgave_70395
+70396	Chroniques-de-J-Froissart-tome-1013_70396
+70397	How-to-swim-b-A-practical-manual-of-swimming-by-a-practical-swimmer-and-a-guide-to-the-novice__70397
+70398	A-bibliography-of-the-writings-of-D-H-Lawrence_70398
+70399	The-clammer_70399
+70400	The-cheerful-blackguard_70400
+70401	By-paths-in-Hebraic-bookland_70401
```

### Comparing `gitberg-0.8.2/gitenberg/data/gutenberg_descriptions.json` & `gitberg-0.8.3/gitenberg/data/gutenberg_descriptions.json`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/data/missing.tsv` & `gitberg-0.8.3/gitenberg/data/missing.tsv`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/dialog.py` & `gitberg-0.8.3/gitenberg/dialog.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/dialog.pyc` & `gitberg-0.8.3/gitenberg/dialog.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/fetch.py` & `gitberg-0.8.3/gitenberg/fetch.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/fetch.pyc` & `gitberg-0.8.3/gitenberg/fetch.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/library.py` & `gitberg-0.8.3/gitenberg/library.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/library.pyc` & `gitberg-0.8.3/gitenberg/library.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/local_repo.py` & `gitberg-0.8.3/gitenberg/local_repo.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/local_repo.pyc` & `gitberg-0.8.3/gitenberg/local_repo.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/make.py` & `gitberg-0.8.3/gitenberg/make.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/make.pyc` & `gitberg-0.8.3/gitenberg/make.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/.DS_Store` & `gitberg-0.8.3/gitenberg/metadata/.DS_Store`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/__pycache__/licenses.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/metadata/__pycache__/licenses.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/__pycache__/marc.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/metadata/__pycache__/marc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/__pycache__/pandata.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/metadata/__pycache__/pandata.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/__pycache__/pg_rdf.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/metadata/__pycache__/pg_rdf.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/__pycache__/utils.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/metadata/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/fileinfo.py` & `gitberg-0.8.3/gitenberg/metadata/fileinfo.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from rdflib.plugins.serializers import jsonld as serializer
 from .pg_rdf import unblank_node, context
 
 # get the modified data for the htm file from PG RDF
 def htm_modified(file_path):
     g=rdflib.Graph()
     try:
-        g.load(file_path)
+        g.parse(source=file_path)
     except IOError:
         return None
 
     ld = serializer.from_rdf(g, context_data=context, base=None,
             use_native_types=False, use_rdf_type=False,
             auto_compact=False, startnode=None, index=False)
```

### Comparing `gitberg-0.8.2/gitenberg/metadata/fileinfo.pyc` & `gitberg-0.8.3/gitenberg/metadata/fileinfo.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/licenses.py` & `gitberg-0.8.3/gitenberg/metadata/licenses.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/licenses.pyc` & `gitberg-0.8.3/gitenberg/metadata/licenses.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/marc.py` & `gitberg-0.8.3/gitenberg/metadata/marc.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/marc.pyc` & `gitberg-0.8.3/gitenberg/metadata/marc.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/pandata.py` & `gitberg-0.8.3/gitenberg/metadata/pandata.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/pandata.pyc` & `gitberg-0.8.3/gitenberg/metadata/pandata.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/pg_rdf.py` & `gitberg-0.8.3/gitenberg/metadata/pg_rdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,15 @@
     return top2
     
 #print(json.dumps(pg_rdf_to_yaml('/Users/eric/Downloads/cache/epub/19218/pg19218.rdf'),indent=2, separators=(',', ': '), sort_keys=True))
 
 def htm_modified(file_path):
     g = rdflib.Graph()
     try:
-        g.load(file_path)
+        g.parse(source=file_path)
     except IOError:
         return None
 
     ld = serializer.from_rdf(g, context_data=context, base=None,
             use_native_types=False, use_rdf_type=False,
             auto_compact=False, startnode=None, index=False)
```

### Comparing `gitberg-0.8.2/gitenberg/metadata/pg_rdf.pyc` & `gitberg-0.8.3/gitenberg/metadata/pg_rdf.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/utils.py` & `gitberg-0.8.3/gitenberg/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/metadata/utils.pyc` & `gitberg-0.8.3/gitenberg/metadata/utils.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/pg_wikipedia.py` & `gitberg-0.8.3/gitenberg/pg_wikipedia.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/pg_wikipedia.pyc` & `gitberg-0.8.3/gitenberg/pg_wikipedia.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/push.py` & `gitberg-0.8.3/gitenberg/push.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/push.pyc` & `gitberg-0.8.3/gitenberg/push.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/templates/.DS_Store` & `gitberg-0.8.3/gitenberg/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/templates/LICENSE` & `gitberg-0.8.3/gitenberg/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/templates/README.rst.j2` & `gitberg-0.8.3/gitenberg/templates/README.rst.j2`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/.DS_Store` & `gitberg-0.8.3/gitenberg/tests/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0002 0000 0000 0000 0001  ................
 00000050: 0000 0001 0000 1000 005f 0064 0061 0074  ........._.d.a.t
 00000060: 0061 6473 0000 0000 0000 0000 0000 0000  .ads............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0001 0000 0009  ................
 00000090: 0074 0065 0073 0074 005f 0064 0061 0074  .t.e.s.t._.d.a.t
-000000a0: 0061 6473 636c 626f 6f6c 0100 0000 0000  .adsclbool......
+000000a0: 0061 6473 636c 626f 6f6c 0000 0000 0000  .adsclbool......
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `gitberg-0.8.2/gitenberg/tests/test_book.py` & `gitberg-0.8.3/gitenberg/tests/test_book.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_book.pyc` & `gitberg-0.8.3/gitenberg/tests/test_book.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_config.py` & `gitberg-0.8.3/gitenberg/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_config.pyc` & `gitberg-0.8.3/gitenberg/tests/test_config.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_cover.py` & `gitberg-0.8.3/gitenberg/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/.DS_Store` & `gitberg-0.8.3/gitenberg/tests/test_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/1234/1234.txt` & `gitberg-0.8.3/gitenberg/tests/test_data/1234/1234.txt`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/1234/pg1234.rdf` & `gitberg-0.8.3/gitenberg/tests/test_data/1234/pg1234.rdf`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/.DS_Store` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/.DS_Store`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/commit-msg.sample` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-commit.sample` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-push.sample` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-rebase.sample` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-receive.sample` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/prepare-commit-msg.sample` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/update.sample` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/1234/pg1234.rdf` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/pg1234.rdf`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/commit-msg.sample` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-commit.sample` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-push.sample` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-rebase.sample` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-receive.sample` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/prepare-commit-msg.sample` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/.git/hooks/update.sample` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_data/rdf_library/7/pg7.rdf` & `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/pg7.rdf`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_fetch.py` & `gitberg-0.8.3/gitenberg/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_fetch.pyc` & `gitberg-0.8.3/gitenberg/tests/test_fetch.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_local_repo.py` & `gitberg-0.8.3/gitenberg/tests/test_local_repo.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_local_repo.pyc` & `gitberg-0.8.3/gitenberg/tests/test_local_repo.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_make.py` & `gitberg-0.8.3/gitenberg/tests/test_make.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_make.pyc` & `gitberg-0.8.3/gitenberg/tests/test_make.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_metadata.py` & `gitberg-0.8.3/gitenberg/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_metadata.pyc` & `gitberg-0.8.3/gitenberg/tests/test_metadata.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_old_metadata.py` & `gitberg-0.8.3/gitenberg/tests/test_old_metadata.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_old_metadata.pyc` & `gitberg-0.8.3/gitenberg/tests/test_old_metadata.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_push.py` & `gitberg-0.8.3/gitenberg/tests/test_push.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/tests/test_push.pyc` & `gitberg-0.8.3/gitenberg/tests/test_push.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/__pycache__/catalog.cpython-36.pyc` & `gitberg-0.8.3/gitenberg/util/__pycache__/catalog.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/__pycache__/catalog.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/util/__pycache__/catalog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/__pycache__/filetypes.cpython-36.pyc` & `gitberg-0.8.3/gitenberg/util/__pycache__/filetypes.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/__pycache__/filetypes.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/util/__pycache__/filetypes.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/__pycache__/pg.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/util/__pycache__/pg.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/__pycache__/tenprintcover.cpython-36.pyc` & `gitberg-0.8.3/gitenberg/util/__pycache__/tenprintcover.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/__pycache__/tenprintcover.cpython-39.pyc` & `gitberg-0.8.3/gitenberg/util/__pycache__/tenprintcover.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/catalog.py` & `gitberg-0.8.3/gitenberg/util/catalog.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/catalog.pyc` & `gitberg-0.8.3/gitenberg/util/catalog.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/filetypes.py` & `gitberg-0.8.3/gitenberg/util/filetypes.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/filetypes.pyc` & `gitberg-0.8.3/gitenberg/util/filetypes.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/pg.py` & `gitberg-0.8.3/gitenberg/util/pg.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/pg.pyc` & `gitberg-0.8.3/gitenberg/util/pg.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/tenprintcover.py` & `gitberg-0.8.3/gitenberg/util/tenprintcover.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/util/tenprintcover.pyc` & `gitberg-0.8.3/gitenberg/util/tenprintcover.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/workflow.py` & `gitberg-0.8.3/gitenberg/workflow.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/gitenberg/workflow.pyc` & `gitberg-0.8.3/gitenberg/workflow.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/requirements.pip` & `gitberg-0.8.3/requirements.pip`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.2/setup.py` & `gitberg-0.8.3/setup.py`

 * *Files identical despite different names*

