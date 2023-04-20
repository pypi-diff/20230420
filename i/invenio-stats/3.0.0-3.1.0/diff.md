# Comparing `tmp/invenio-stats-3.0.0.tar.gz` & `tmp/invenio-stats-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-stats-3.0.0.tar", last modified: Wed Mar  1 16:27:28 2023, max compression
+gzip compressed data, was "dist/invenio-stats-3.1.0.tar", last modified: Thu Apr 20 09:29:41 2023, max compression
```

## Comparing `invenio-stats-3.0.0.tar` & `invenio-stats-3.1.0.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      642 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      737 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2282 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3715 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      348 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7437 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      619 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10247 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1446 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/examplesapp.rst
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6995 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)     4418 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/examples/
--rwxr-xr-x   0 runner    (1001) docker     (122)      284 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/examples/app-setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      109 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/examples/app-teardown.sh
--rw-r--r--   0 runner    (1001) docker     (122)     4533 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/examples/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/
--rw-r--r--   0 runner    (1001) docker     (122)    14422 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15944 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (122)     5070 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_file_download/
--rw-r--r--   0 runner    (1001) docker     (122)      317 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_file_download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v1/
--rw-r--r--   0 runner    (1001) docker     (122)      321 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v1/aggr-file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v2/
--rw-r--r--   0 runner    (1001) docker     (122)      321 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v2/aggr-file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_file_download/v7/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_file_download/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_file_download/v7/aggr-file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_record_view/
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_record_view/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v1/
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v1/aggr-record-view-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v2/
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v2/aggr-record-view-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_record_view/v7/
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_record_view/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_record_view/v7/aggr-record-view-v1.json
--rw-r--r--   0 runner    (1001) docker     (122)     3652 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/event_builders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/file_download/
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/file_download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/file_download/os-v1/
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/file_download/os-v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/file_download/os-v1/file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/file_download/os-v2/
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/file_download/os-v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/file_download/os-v2/file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/file_download/v7/
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/file_download/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/file_download/v7/file-download-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/record_view/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/record_view/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/record_view/os-v1/
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/record_view/os-v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/record_view/os-v1/record-view-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/record_view/os-v2/
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/record_view/os-v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/record_view/os-v2/record-view-v1.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats/contrib/record_view/v7/
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/record_view/v7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/contrib/record_view/v7/record-view-v1.json
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     5130 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     7882 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/processors.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)    12927 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/queries.py
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/queues.py
--rw-r--r--   0 runner    (1001) docker     (122)     2502 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/receivers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     3463 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3400 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/invenio_stats/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-03-01 16:27:27.000000 invenio-stats-3.0.0/invenio_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/invenio_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-01 16:27:27.000000 invenio-stats-3.0.0/invenio_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      483 2023-03-01 16:27:27.000000 invenio-stats-3.0.0/invenio_stats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-01 16:27:27.000000 invenio-stats-3.0.0/invenio_stats.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      563 2023-03-01 16:27:27.000000 invenio-stats-3.0.0/invenio_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-03-01 16:27:27.000000 invenio-stats-3.0.0/invenio_stats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      745 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      862 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      357 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    17722 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 16:27:28.000000 invenio-stats-3.0.0/tests/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/tests/contrib/test_event_builders.py
--rw-r--r--   0 runner    (1001) docker     (122)      848 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    10006 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/tests/test_aggregations.py
--rw-r--r--   0 runner    (1001) docker     (122)     9261 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/tests/test_invenio_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2998 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/tests/test_prefixing.py
--rw-r--r--   0 runner    (1001) docker     (122)    13802 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/tests/test_processors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2088 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (122)     2813 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/tests/test_receivers.py
--rw-r--r--   0 runner    (1001) docker     (122)      939 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-03-01 16:27:19.000000 invenio-stats-3.0.0/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      642 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      737 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2282 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3715 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5108 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7437 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10247 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1446 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/examplesapp.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6995 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)     4418 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      284 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/examples/app-setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      109 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/examples/app-teardown.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     4533 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/examples/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/
+-rw-r--r--   0 runner    (1001) docker     (122)    14422 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15918 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5070 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_file_download/
+-rw-r--r--   0 runner    (1001) docker     (122)      317 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_file_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      321 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v1/aggr-file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      321 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v2/aggr-file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_file_download/v7/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_file_download/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_file_download/v7/aggr-file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_record_view/
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_record_view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v1/aggr-record-view-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v2/aggr-record-view-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_record_view/v7/
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_record_view/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_record_view/v7/aggr-record-view-v1.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3652 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/event_builders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/file_download/
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/file_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/file_download/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/file_download/os-v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/file_download/os-v1/file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/file_download/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/file_download/os-v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/file_download/os-v2/file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/file_download/v7/
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/file_download/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/file_download/v7/file-download-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/record_view/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/record_view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/record_view/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/record_view/os-v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/record_view/os-v1/record-view-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/record_view/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/record_view/os-v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/record_view/os-v2/record-view-v1.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats/contrib/record_view/v7/
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/record_view/v7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/contrib/record_view/v7/record-view-v1.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7882 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/processors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12927 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/queues.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2502 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3409 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/invenio_stats/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5108 2023-04-20 09:29:40.000000 invenio-stats-3.1.0/invenio_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/invenio_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 09:29:40.000000 invenio-stats-3.1.0/invenio_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      483 2023-04-20 09:29:40.000000 invenio-stats-3.1.0/invenio_stats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 09:29:40.000000 invenio-stats-3.1.0/invenio_stats.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-04-20 09:29:40.000000 invenio-stats-3.1.0/invenio_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-20 09:29:40.000000 invenio-stats-3.1.0/invenio_stats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      745 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      862 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      357 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    17722 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:29:41.000000 invenio-stats-3.1.0/tests/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/tests/contrib/test_event_builders.py
+-rw-r--r--   0 runner    (1001) docker     (122)      848 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10006 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/tests/test_aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9261 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/tests/test_invenio_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2998 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/tests/test_prefixing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13802 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/tests/test_processors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2088 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2813 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/tests/test_receivers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      939 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-04-20 09:29:27.000000 invenio-stats-3.1.0/tests/test_views.py
```

### Comparing `invenio-stats-3.0.0/.editorconfig` & `invenio-stats-3.1.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/.github/workflows/pypi-publish.yml` & `invenio-stats-3.1.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/.github/workflows/tests.yml` & `invenio-stats-3.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/.tx/config` & `invenio-stats-3.1.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/CHANGES.rst` & `invenio-stats-3.1.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,19 @@
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 
 Changes
 =======
 
+Version 3.1.0 (release 2023-04-20)
+-------------------------------------
+
+- add extension method for building and caching queries
+
 Version 3.0.0 (release 2023-03-01)
 -------------------------------------
 
 - Upgrade to ``invenio-search`` 2.x
 - Drop support for Elasticsearch 2, 5, and 6
 - Add support for OpenSearch 1 and 2
 - Drop support for Python 2.7 and 3.6
```

### Comparing `invenio-stats-3.0.0/CONTRIBUTING.rst` & `invenio-stats-3.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/LICENSE` & `invenio-stats-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/MANIFEST.in` & `invenio-stats-3.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/PKG-INFO` & `invenio-stats-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-stats
-Version: 3.0.0
+Version: 3.1.0
 Summary: "Invenio module for collecting statistics."
 Home-page: https://github.com/inveniosoftware/invenio-stats
 Author: CERN
 Author-email: info@invenio-software.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -54,14 +54,19 @@
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         
         Changes
         =======
         
+        Version 3.1.0 (release 2023-04-20)
+        -------------------------------------
+        
+        - add extension method for building and caching queries
+        
         Version 3.0.0 (release 2023-03-01)
         -------------------------------------
         
         - Upgrade to ``invenio-search`` 2.x
         - Drop support for Elasticsearch 2, 5, and 6
         - Add support for OpenSearch 1 and 2
         - Drop support for Python 2.7 and 3.6
```

### Comparing `invenio-stats-3.0.0/README.rst` & `invenio-stats-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/docs/Makefile` & `invenio-stats-3.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/docs/api.rst` & `invenio-stats-3.1.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/docs/conf.py` & `invenio-stats-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/docs/configuration.rst` & `invenio-stats-3.1.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/docs/index.rst` & `invenio-stats-3.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/docs/make.bat` & `invenio-stats-3.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/docs/overview.rst` & `invenio-stats-3.1.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/examples/app.py` & `invenio-stats-3.1.0/examples/app.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/__init__.py` & `invenio-stats-3.1.0/invenio_stats/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,14 +436,14 @@
 Invenio-Stats provides some default statistics which can be found in
 :py:mod:`invenio_stats.contrib.event_builders`.
 """
 
 from .ext import InvenioStats
 from .proxies import current_stats
 
-__version__ = "3.0.0"
+__version__ = "3.1.0"
 
 __all__ = (
     "__version__",
     "current_stats",
     "InvenioStats",
 )
```

### Comparing `invenio-stats-3.0.0/invenio_stats/aggregations.py` & `invenio-stats-3.1.0/invenio_stats/aggregations.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Aggregation classes."""
 
 import math
 from collections import OrderedDict
-from copy import deepcopy
 from datetime import datetime
 from functools import wraps
 
 from dateutil import parser
 from dateutil.relativedelta import relativedelta
 from invenio_search import current_search_client
 from invenio_search.engine import dsl, search
```

### Comparing `invenio-stats-3.0.0/invenio_stats/cli.py` & `invenio-stats-3.1.0/invenio_stats/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/config.py` & `invenio-stats-3.1.0/invenio_stats/config.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v1/aggr-file-download-v1.json` & `invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v1/aggr-file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v2/aggr-file-download-v1.json` & `invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_file_download/os-v2/aggr-file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_file_download/v7/aggr-file-download-v1.json` & `invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_file_download/v7/aggr-file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v1/aggr-record-view-v1.json` & `invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v1/aggr-record-view-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v2/aggr-record-view-v1.json` & `invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_record_view/os-v2/aggr-record-view-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/contrib/aggregations/aggr_record_view/v7/aggr-record-view-v1.json` & `invenio-stats-3.1.0/invenio_stats/contrib/aggregations/aggr_record_view/v7/aggr-record-view-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/contrib/config.py` & `invenio-stats-3.1.0/invenio_stats/contrib/config.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/contrib/event_builders.py` & `invenio-stats-3.1.0/invenio_stats/contrib/event_builders.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/contrib/file_download/os-v1/file-download-v1.json` & `invenio-stats-3.1.0/invenio_stats/contrib/file_download/os-v1/file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/contrib/file_download/os-v2/file-download-v1.json` & `invenio-stats-3.1.0/invenio_stats/contrib/file_download/os-v2/file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/contrib/file_download/v7/file-download-v1.json` & `invenio-stats-3.1.0/invenio_stats/contrib/file_download/v7/file-download-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/contrib/record_view/os-v1/record-view-v1.json` & `invenio-stats-3.1.0/invenio_stats/contrib/record_view/os-v1/record-view-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/contrib/record_view/os-v2/record-view-v1.json` & `invenio-stats-3.1.0/invenio_stats/contrib/record_view/os-v2/record-view-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/contrib/record_view/v7/record-view-v1.json` & `invenio-stats-3.1.0/invenio_stats/contrib/record_view/v7/record-view-v1.json`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/errors.py` & `invenio-stats-3.1.0/invenio_stats/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/ext.py` & `invenio-stats-3.1.0/invenio_stats/ext.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,36 +28,50 @@
 class _InvenioStatsState(object):
     """State object for Invenio stats."""
 
     def __init__(self, app):
         self.app = app
         self.exchange = app.config["STATS_MQ_EXCHANGE"]
         self._event_emitters = {}
+        self._query_objects = {}
 
     @property
     def events_config(self):
         return self.app.config["STATS_EVENTS"]
 
     @property
     def aggregations_config(self):
         return self.app.config["STATS_AGGREGATIONS"]
 
     @property
     def queries_config(self):
         return self.app.config["STATS_QUERIES"]
 
     def get_event_emitter(self, event_name):
-        """Get the event emitter for the given event name."""
+        """Get the (cached) event emitter for the given event name."""
         if event_name not in self._event_emitters:
             self._event_emitters[event_name] = build_event_emitter(
                 event_name, self.events_config
             )
 
         return self._event_emitters[event_name]
 
+    def get_query(self, query_name):
+        """Get the (cached) query object for the given name.
+
+        Note: Because this method potentially shares references to the same query
+        objects multiple times, their internal states should not be modified after
+        construction.
+        """
+        if query_name not in self._query_objects:
+            query = self.queries[query_name]
+            self._query_objects[query_name] = query.cls(name=query.name, **query.params)
+
+        return self._query_objects[query_name]
+
     @cached_property
     def events(self):
         """Configured events."""
         result = {}
         for name, event in self.events_config.items():
             event = obj_or_import_string(event)
             if callable(event):
```

### Comparing `invenio-stats-3.0.0/invenio_stats/processors.py` & `invenio-stats-3.1.0/invenio_stats/processors.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/queries.py` & `invenio-stats-3.1.0/invenio_stats/queries.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/receivers.py` & `invenio-stats-3.1.0/invenio_stats/receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/tasks.py` & `invenio-stats-3.1.0/invenio_stats/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/templates.py` & `invenio-stats-3.1.0/invenio_stats/templates.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats/utils.py` & `invenio-stats-3.1.0/invenio_stats/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 
 """Utilities for Invenio-Stats."""
 
 import os
 from base64 import b64encode
 from math import ceil
 
-from flask import current_app, request, session
+from flask import request, session
 from flask_login import current_user
 from geolite2 import geolite2
 from invenio_cache import current_cache
 from invenio_search.engine import dsl
-from werkzeug.utils import import_string
 
 
 def get_anonymization_salt(ts):
     """Get the anonymization salt based on the event timestamp's day."""
     salt_key = "stats:salt:{}".format(ts.date().isoformat())
     salt = current_cache.get(salt_key)
     if not salt:
```

### Comparing `invenio-stats-3.0.0/invenio_stats/views.py` & `invenio-stats-3.1.0/invenio_stats/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                     '{ STATISTIC_NAME: { "stat": STAT_TYPE, '
                     '"params": STAT_PARAMS }}'
                 )
 
             stat = config["stat"]
             params = config.get("params", {})
             try:
-                query_cfg = current_stats.queries[stat]
+                query = current_stats.get_query(stat)
             except KeyError:
                 raise UnknownQueryError(stat)
 
             permission = current_stats.permission_factory(stat, params)
             if permission is not None and not permission.can():
                 message = (
                     "You do not have a permission to query the "
@@ -82,15 +82,14 @@
 
                 if current_user.is_authenticated:
                     abort(403, message)
 
                 abort(401, message)
 
             try:
-                query = query_cfg.cls(name=query_name, **query_cfg.params)
                 result[query_name] = query.run(**params)
 
             except ValueError as e:
                 raise InvalidRequestInputError(e.args[0])
             except search.exceptions.NotFoundError:
                 # In case there is no index or value for the metric we return 0
                 result[query_name] = dict.fromkeys(query.metric_fields.keys(), 0)
```

### Comparing `invenio-stats-3.0.0/invenio_stats.egg-info/PKG-INFO` & `invenio-stats-3.1.0/invenio_stats.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-stats
-Version: 3.0.0
+Version: 3.1.0
 Summary: "Invenio module for collecting statistics."
 Home-page: https://github.com/inveniosoftware/invenio-stats
 Author: CERN
 Author-email: info@invenio-software.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -54,14 +54,19 @@
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         
         Changes
         =======
         
+        Version 3.1.0 (release 2023-04-20)
+        -------------------------------------
+        
+        - add extension method for building and caching queries
+        
         Version 3.0.0 (release 2023-03-01)
         -------------------------------------
         
         - Upgrade to ``invenio-search`` 2.x
         - Drop support for Elasticsearch 2, 5, and 6
         - Add support for OpenSearch 1 and 2
         - Drop support for Python 2.7 and 3.6
```

### Comparing `invenio-stats-3.0.0/invenio_stats.egg-info/SOURCES.txt` & `invenio-stats-3.1.0/invenio_stats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/invenio_stats.egg-info/requires.txt` & `invenio-stats-3.1.0/invenio_stats.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/requirements-devel.txt` & `invenio-stats-3.1.0/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/run-tests.sh` & `invenio-stats-3.1.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/setup.cfg` & `invenio-stats-3.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/tests/conftest.py` & `invenio-stats-3.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/tests/contrib/test_event_builders.py` & `invenio-stats-3.1.0/tests/contrib/test_event_builders.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/tests/helpers.py` & `invenio-stats-3.1.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/tests/test_aggregations.py` & `invenio-stats-3.1.0/tests/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/tests/test_cli.py` & `invenio-stats-3.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/tests/test_events.py` & `invenio-stats-3.1.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/tests/test_invenio_stats.py` & `invenio-stats-3.1.0/tests/test_invenio_stats.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio Stats extension tests."""
 
 from flask import Flask
 
 from invenio_stats import InvenioStats
+from invenio_stats.proxies import current_stats
 
 
 def test_version():
     """Test version import."""
     from invenio_stats import __version__
 
     assert __version__
@@ -28,7 +29,15 @@
     assert "invenio-stats" in app.extensions
 
     app = Flask("testapp")
     ext = InvenioStats()
     assert "invenio-stats" not in app.extensions
     ext.init_app(app)
     assert "invenio-stats" in app.extensions
+
+
+def test_extension_get_query_cache(app, queries_config):
+    """Test if the query object cache works properly."""
+    query1 = current_stats.get_query("test-query")
+    query2 = current_stats.get_query("test-query")
+
+    assert query1 is query2
```

### Comparing `invenio-stats-3.0.0/tests/test_prefixing.py` & `invenio-stats-3.1.0/tests/test_prefixing.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/tests/test_processors.py` & `invenio-stats-3.1.0/tests/test_processors.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/tests/test_queries.py` & `invenio-stats-3.1.0/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/tests/test_receivers.py` & `invenio-stats-3.1.0/tests/test_receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/tests/test_tasks.py` & `invenio-stats-3.1.0/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/tests/test_utils.py` & `invenio-stats-3.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-stats-3.0.0/tests/test_views.py` & `invenio-stats-3.1.0/tests/test_views.py`

 * *Files identical despite different names*

