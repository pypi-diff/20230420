# Comparing `tmp/jscc-0.1.0.tar.gz` & `tmp/jscc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jscc-0.1.0.tar", last modified: Fri Oct 28 20:15:58 2022, max compression
+gzip compressed data, was "jscc-0.1.1.tar", last modified: Wed Apr 19 22:54:10 2023, max compression
```

## Comparing `jscc-0.1.0.tar` & `jscc-0.1.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.338811 jscc-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-10-28 20:15:54.000000 jscc-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-10-28 20:15:54.000000 jscc-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-10-28 20:15:58.338811 jscc-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-10-28 20:15:54.000000 jscc-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.326811 jscc-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-10-28 20:15:54.000000 jscc-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.326811 jscc-0.1.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-28 20:15:54.000000 jscc-0.1.0/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-10-28 20:15:54.000000 jscc-0.1.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-28 20:15:54.000000 jscc-0.1.0/docs/api/schema.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.326811 jscc-0.1.0/docs/api/testing/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-10-28 20:15:54.000000 jscc-0.1.0/docs/api/testing/checks.rst
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-10-28 20:15:54.000000 jscc-0.1.0/docs/api/testing/filesystem.rst
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-28 20:15:54.000000 jscc-0.1.0/docs/api/testing/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-28 20:15:54.000000 jscc-0.1.0/docs/api/testing/util.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2850 2022-10-28 20:15:54.000000 jscc-0.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-10-28 20:15:54.000000 jscc-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-10-28 20:15:54.000000 jscc-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-28 20:15:54.000000 jscc-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.326811 jscc-0.1.0/jscc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:54.000000 jscc-0.1.0/jscc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-10-28 20:15:54.000000 jscc-0.1.0/jscc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3624 2022-10-28 20:15:54.000000 jscc-0.1.0/jscc/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.330811 jscc-0.1.0/jscc/testing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:54.000000 jscc-0.1.0/jscc/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31447 2022-10-28 20:15:54.000000 jscc-0.1.0/jscc/testing/checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-10-28 20:15:54.000000 jscc-0.1.0/jscc/testing/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-10-28 20:15:54.000000 jscc-0.1.0/jscc/testing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.326811 jscc-0.1.0/jscc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-10-28 20:15:58.000000 jscc-0.1.0/jscc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2389 2022-10-28 20:15:58.000000 jscc-0.1.0/jscc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 20:15:58.000000 jscc-0.1.0/jscc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-10-28 20:15:58.000000 jscc-0.1.0/jscc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-28 20:15:58.000000 jscc-0.1.0/jscc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-28 20:15:54.000000 jscc-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-28 20:15:58.338811 jscc-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-10-28 20:15:54.000000 jscc-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.330811 jscc-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.330811 jscc-0.1.0/tests/cassettes/
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/cassettes/test_http_get_error.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/cassettes/test_http_head_error.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.330811 jscc-0.1.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/codelist.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.330811 jscc-0.1.0/tests/fixtures/csv/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/csv/empty.csv
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/csv/valid.csv
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/data.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.334811 jscc-0.1.0/tests/fixtures/empty/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/empty/empty-array.json
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/empty/empty-object.json
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/empty/empty-string.json
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/empty/false.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.334811 jscc-0.1.0/tests/fixtures/empty/htmlcov/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/empty/htmlcov/empty.txt
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/empty/invalid.json
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/empty/null.json
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/empty/whitespace.json
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/empty/whitespace.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/empty/zero-float.json
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/empty/zero-int.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.334811 jscc-0.1.0/tests/fixtures/indent/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/indent/ascii.json
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/indent/compact.json
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/indent/indented.json
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/indent/invalid.json
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/indent/no-newline.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.334811 jscc-0.1.0/tests/fixtures/json/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/json/duplicate-key.json
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/json/invalid.json
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/json/valid.json
--rw-r--r--   0 runner    (1001) docker     (121)     4357 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/meta-schema.json
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/patch.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.338811 jscc-0.1.0/tests/fixtures/schema/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/array_items.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.338811 jscc-0.1.0/tests/fixtures/schema/build/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/build/ignore.json
--rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/codelist_enum.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 20:15:58.338811 jscc-0.1.0/tests/fixtures/schema/codelists/
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/codelists/+nonexistent.csv
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/codelists/extra.csv
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/codelists/failClosedArray.csv
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/codelists/failClosedString.csv
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/codelists/test.csv
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/deep_properties.json
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/items_type.json
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/letter_case.json
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/merge_properties.json
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/metadata_presence.json
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/null_type.json
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/object_id.json
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/ref.json
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/fixtures/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)    12294 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2546 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-28 20:15:54.000000 jscc-0.1.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.417623 jscc-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-19 22:54:01.000000 jscc-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-19 22:54:01.000000 jscc-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-19 22:54:10.417623 jscc-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-19 22:54:01.000000 jscc-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.405623 jscc-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/api/schema.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/docs/api/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/api/testing/checks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/api/testing/filesystem.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/api/testing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/api/testing/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/jscc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:01.000000 jscc-0.1.1/jscc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-19 22:54:01.000000 jscc-0.1.1/jscc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-04-19 22:54:01.000000 jscc-0.1.1/jscc/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/jscc/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:01.000000 jscc-0.1.1/jscc/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31444 2023-04-19 22:54:01.000000 jscc-0.1.1/jscc/testing/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-19 22:54:01.000000 jscc-0.1.1/jscc/testing/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-19 22:54:01.000000 jscc-0.1.1/jscc/testing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/jscc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-19 22:54:10.000000 jscc-0.1.1/jscc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-19 22:54:10.000000 jscc-0.1.1/jscc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 22:54:10.000000 jscc-0.1.1/jscc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-19 22:54:10.000000 jscc-0.1.1/jscc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 22:54:10.000000 jscc-0.1.1/jscc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-19 22:54:01.000000 jscc-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-19 22:54:10.417623 jscc-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/tests/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/cassettes/test_http_get_error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/cassettes/test_http_head_error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/codelist.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/tests/fixtures/csv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/csv/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/csv/valid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.413623 jscc-0.1.1/tests/fixtures/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/empty-array.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/empty-object.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/empty-string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/false.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.413623 jscc-0.1.1/tests/fixtures/empty/htmlcov/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/htmlcov/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/null.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/whitespace-string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/whitespace.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/zero-float.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/zero-int.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.413623 jscc-0.1.1/tests/fixtures/indent/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/indent/ascii.json
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/indent/compact.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/indent/indented.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/indent/invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/indent/no-newline.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.413623 jscc-0.1.1/tests/fixtures/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/json/duplicate-key.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/json/invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/json/valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/meta-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/patch.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.413623 jscc-0.1.1/tests/fixtures/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/array_items.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.413623 jscc-0.1.1/tests/fixtures/schema/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/build/ignore.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/codelist_enum.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.417623 jscc-0.1.1/tests/fixtures/schema/codelists/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/codelists/+nonexistent.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/codelists/extra.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/codelists/failClosedArray.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/codelists/failClosedString.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/codelists/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/deep_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/items_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/letter_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/merge_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/metadata_presence.json
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/null_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/object_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/ref.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/test_util.py
```

### Comparing `jscc-0.1.0/LICENSE` & `jscc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/PKG-INFO` & `jscc-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: jscc
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for data standards that use JSON Schema and CSV codelists
 Home-page: https://github.com/open-contracting/jscc
 Author: Open Contracting Partnership and Open Data Services Co-operative Limited
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `jscc-0.1.0/README.rst` & `jscc-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/docs/Makefile` & `jscc-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/docs/changelog.rst` & `jscc-0.1.1/docs/changelog.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 Changelog
 =========
 
+0.1.1 (2023-04-19)
+------------------
+
+Changed
+~~~~~~~
+
+-  Drop support for Python 3.6 (end-of-life 2021-12-23).
+
+Fixed
+~~~~~
+
+-  :meth:`jscc.testing.checks.get_empty_files` correctly returns JSON files that are whitespace only.
+
 0.1.0 (2022-10-28)
 ------------------
 
 Changed
 ~~~~~~~
 
 -  Update to `jsonref <https://jsonref.readthedocs.io/>`__ 1.0's API.
```

### Comparing `jscc-0.1.0/docs/conf.py` & `jscc-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/jscc/exceptions.py` & `jscc-0.1.1/jscc/exceptions.py`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/jscc/schema.py` & `jscc-0.1.1/jscc/schema.py`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/jscc/testing/checks.py` & `jscc-0.1.1/jscc/testing/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,30 +129,30 @@
         if tracked(path) and include(path, name) and name != '__init__.py':
             try:
                 with open(path) as f:
                     text = f.read()
             except UnicodeDecodeError:
                 continue  # the file is non-empty, and might be binary
 
-            if name.endswith('.json'):
+            if not text.strip():
+                yield path,
+            elif name.endswith('.json'):
                 try:
                     value = json.loads(text)
                     if not value and not isinstance(value, (bool, int, float)):
                         yield path,
                 except json.decoder.JSONDecodeError:
                     continue  # the file is non-empty
-            elif not text.strip():
-                yield path,
 
 
 def get_misindented_files(include=_true, **kwargs):
     """
     Yields the path (as a tuple) of any JSON file that isn't formatted for humans.
 
-    JSON files must be indented with two spaces, musn't escape non-ASCII characters (no ``\\uXXXX`` sequences), and
+    JSON files must be indented with two spaces, mustn't escape non-ASCII characters (no ``\\uXXXX`` sequences), and
     must have a newline at end of file.
 
     :param function include: a method that accepts a file path and file name, and returns whether to test the file
                              (default true)
 
     pytest example::
 
@@ -444,15 +444,15 @@
                     actual = set(data['items']['enum'])
 
                 # It'd be faster to cache the CSVs, but most extensions have only one closed codelist.
                 for _, csvname, _, _, rows in walk_csv_data():
                     # The codelist's CSV file must exist.
                     if csvname == data['codelist']:
                         if actual:
-                            expected = set([row['Code'] for row in rows])
+                            expected = {row['Code'] for row in rows}
                             if 'string' in types and 'null' in types:
                                 expected.add(None)
 
                             if actual != expected:
                                 added, removed = difference(actual, expected)
 
                                 errors += 1
@@ -616,15 +616,15 @@
     return _traverse(block)(*args)
 
 
 def validate_merge_properties(*args):
     """
     Warns and returns the number of errors relating to missing or extra merge properties.
 
-    The "omitWhenMerged" and "wholeListMerge" properties mustn't both be set, and musn't be set to ``false`` or
+    The "omitWhenMerged" and "wholeListMerge" properties mustn't both be set, and mustn't be set to ``false`` or
     ``null``. The "wholeListMerge" property must be set on non-nullable arrays of objects only.
 
     See https://standard.open-contracting.org/1.1/en/schema/merging/#whole-list-merge
 
     :returns: the number of errors
     :rtype: int
     """
```

### Comparing `jscc-0.1.0/jscc/testing/filesystem.py` & `jscc-0.1.1/jscc/testing/filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     for path, name in walk(**kwargs):
         if path.endswith('.csv'):
             with open(path, newline='') as f:
                 text = f.read()
                 reader = csv.DictReader(StringIO(text))
                 try:
                     fieldnames = reader.fieldnames
-                    rows = [row for row in reader]
+                    rows = list(reader)
                     yield (path, name, text, fieldnames, rows)
                 except csv.Error:
                     continue
 
 
 def tracked(path):
     """
```

### Comparing `jscc-0.1.0/jscc/testing/util.py` & `jscc-0.1.1/jscc/testing/util.py`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/jscc.egg-info/PKG-INFO` & `jscc-0.1.1/jscc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: jscc
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for data standards that use JSON Schema and CSV codelists
 Home-page: https://github.com/open-contracting/jscc
 Author: Open Contracting Partnership and Open Data Services Co-operative Limited
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `jscc-0.1.0/jscc.egg-info/SOURCES.txt` & `jscc-0.1.1/jscc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.py
+setup.cfg
 docs/Makefile
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
 docs/api/exceptions.rst
 docs/api/index.rst
@@ -44,14 +44,15 @@
 tests/fixtures/empty/__init__.py
 tests/fixtures/empty/empty-array.json
 tests/fixtures/empty/empty-object.json
 tests/fixtures/empty/empty-string.json
 tests/fixtures/empty/false.json
 tests/fixtures/empty/invalid.json
 tests/fixtures/empty/null.json
+tests/fixtures/empty/whitespace-string.json
 tests/fixtures/empty/whitespace.json
 tests/fixtures/empty/whitespace.txt
 tests/fixtures/empty/zero-float.json
 tests/fixtures/empty/zero-int.json
 tests/fixtures/empty/htmlcov/empty.txt
 tests/fixtures/indent/ascii.json
 tests/fixtures/indent/compact.json
```

### Comparing `jscc-0.1.0/tests/cassettes/test_http_get_error.yaml` & `jscc-0.1.1/tests/cassettes/test_http_get_error.yaml`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/tests/cassettes/test_http_head_error.yaml` & `jscc-0.1.1/tests/cassettes/test_http_head_error.yaml`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/tests/fixtures/meta-schema.json` & `jscc-0.1.1/tests/fixtures/meta-schema.json`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/tests/fixtures/schema/codelist_enum.json` & `jscc-0.1.1/tests/fixtures/schema/codelist_enum.json`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/tests/fixtures/schema/null_type.json` & `jscc-0.1.1/tests/fixtures/schema/null_type.json`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/tests/fixtures/schema/object_id.json` & `jscc-0.1.1/tests/fixtures/schema/object_id.json`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/tests/fixtures/schema.json` & `jscc-0.1.1/tests/fixtures/schema.json`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/tests/test_checks.py` & `jscc-0.1.1/tests/test_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
             assert len(result) == 1
 
         assert paths == {
             'empty-array.json',
             'empty-object.json',
             'empty-string.json',
             'null.json',
+            'whitespace.json',
             'whitespace.txt',
         }
 
 
 def test_get_misindented_files():
     directory = os.path.realpath(path('indent')) + os.sep
     with chdir(directory):
```

### Comparing `jscc-0.1.0/tests/test_schema.py` & `jscc-0.1.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `jscc-0.1.0/tests/test_util.py` & `jscc-0.1.1/tests/test_util.py`

 * *Files identical despite different names*

