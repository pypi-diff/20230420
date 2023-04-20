# Comparing `tmp/autofaker-1.0.12.tar.gz` & `tmp/autofaker-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofaker-1.0.12.tar", last modified: Mon Nov 14 18:49:25 2022, max compression
+gzip compressed data, was "autofaker-1.0.14.tar", last modified: Thu Apr 20 10:34:49 2023, max compression
```

## Comparing `autofaker-1.0.12.tar` & `autofaker-1.0.14.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:49:25.984762 autofaker-1.0.12/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-11-14 18:49:14.000000 autofaker-1.0.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-14 18:49:14.000000 autofaker-1.0.12/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13912 2022-11-14 18:49:25.984762 autofaker-1.0.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11288 2022-11-14 18:49:14.000000 autofaker-1.0.12/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-14 18:49:14.000000 autofaker-1.0.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 18:49:25.984762 autofaker-1.0.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-11-14 18:49:16.000000 autofaker-1.0.12/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:49:25.980762 autofaker-1.0.12/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:49:25.980762 autofaker-1.0.12/src/autofaker/
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-11-14 18:49:14.000000 autofaker-1.0.12/src/autofaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-11-14 18:49:14.000000 autofaker-1.0.12/src/autofaker/attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-11-14 18:49:14.000000 autofaker-1.0.12/src/autofaker/autodata.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-11-14 18:49:14.000000 autofaker-1.0.12/src/autofaker/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-11-14 18:49:14.000000 autofaker-1.0.12/src/autofaker/builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-11-14 18:49:14.000000 autofaker-1.0.12/src/autofaker/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-11-14 18:49:14.000000 autofaker-1.0.12/src/autofaker/dates.py
--rw-r--r--   0 runner    (1001) docker     (121)     4964 2022-11-14 18:49:14.000000 autofaker-1.0.12/src/autofaker/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-11-14 18:49:14.000000 autofaker-1.0.12/src/autofaker/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-11-14 18:49:14.000000 autofaker-1.0.12/src/autofaker/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-11-14 18:49:14.000000 autofaker-1.0.12/src/autofaker/fakes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4872 2022-11-14 18:49:14.000000 autofaker-1.0.12/src/autofaker/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:49:25.984762 autofaker-1.0.12/src/autofaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13912 2022-11-14 18:49:25.000000 autofaker-1.0.12/src/autofaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2274 2022-11-14 18:49:25.000000 autofaker-1.0.12/src/autofaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 18:49:25.000000 autofaker-1.0.12/src/autofaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-14 18:49:25.000000 autofaker-1.0.12/src/autofaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-14 18:49:25.000000 autofaker-1.0.12/src/autofaker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:49:25.984762 autofaker-1.0.12/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:49:25.984762 autofaker-1.0.12/tests/pytests/
--rw-r--r--   0 runner    (1001) docker     (121)     7156 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/pytests/test_decorator_anonymous_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/pytests/test_decorator_anonymous_data_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2557 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/pytests/test_decorator_anonymous_data_classes_nested.py
--rw-r--r--   0 runner    (1001) docker     (121)     2522 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/pytests/test_decorator_anonymous_dataframe_pandas.py
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/pytests/test_decorator_anonymous_enum_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3138 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/pytests/test_decorator_anonymous_nested_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2549 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/pytests/test_decorator_anonymous_simple_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_anonymous_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)     5927 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_anonymous_complex_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3073 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_anonymous_data_class_with_fakes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3941 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_anonymous_data_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3281 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_anonymous_data_classes_with_fakes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5507 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_anonymous_dataframe_pandas.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_anonymous_dataframe_with_fakes.py
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_anonymous_dates.py
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_anonymous_enum_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3560 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_anonymous_lists.py
--rw-r--r--   0 runner    (1001) docker     (121)     2105 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_anonymous_nested_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3021 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_anonymous_nested_classes_with_lists.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_anonymous_simple_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     7483 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_anonymous_sut.py
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_many_anonymous_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_many_anonymous_dates.py
--rw-r--r--   0 runner    (1001) docker     (121)     2407 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_many_anonymous_nested_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3477 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_many_anonymous_nested_classes_with_lists.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_create_many_anonymous_simple_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3405 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/test_decorator_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:49:25.984762 autofaker-1.0.12/tests/unittests/
--rw-r--r--   0 runner    (1001) docker     (121)     8712 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/unittests/test_decorator_anonymous_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/unittests/test_decorator_anonymous_data_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3086 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/unittests/test_decorator_anonymous_data_classes_nested.py
--rw-r--r--   0 runner    (1001) docker     (121)     2876 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/unittests/test_decorator_anonymous_dataframe_pandas.py
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/unittests/test_decorator_anonymous_enum_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3669 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/unittests/test_decorator_anonymous_nested_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-11-14 18:49:14.000000 autofaker-1.0.12/tests/unittests/test_decorator_anonymous_simple_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:34:49.104710 autofaker-1.0.14/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-20 10:34:20.000000 autofaker-1.0.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-20 10:34:20.000000 autofaker-1.0.14/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-04-20 10:34:49.104710 autofaker-1.0.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-20 10:34:20.000000 autofaker-1.0.14/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 10:34:20.000000 autofaker-1.0.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:34:49.104710 autofaker-1.0.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-20 10:34:33.000000 autofaker-1.0.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:34:49.096710 autofaker-1.0.14/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:34:49.096710 autofaker-1.0.14/src/autofaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/autodata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:34:49.100710 autofaker-1.0.14/src/autofaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-04-20 10:34:48.000000 autofaker-1.0.14/src/autofaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-20 10:34:49.000000 autofaker-1.0.14/src/autofaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:34:48.000000 autofaker-1.0.14/src/autofaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 10:34:48.000000 autofaker-1.0.14/src/autofaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 10:34:48.000000 autofaker-1.0.14/src/autofaker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:34:49.104710 autofaker-1.0.14/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:34:49.104710 autofaker-1.0.14/tests/pytests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/pytests/test_decorator_anonymous_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/pytests/test_decorator_anonymous_data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/pytests/test_decorator_anonymous_data_classes_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/pytests/test_decorator_anonymous_dataframe_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/pytests/test_decorator_anonymous_enum_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/pytests/test_decorator_anonymous_nested_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/pytests/test_decorator_anonymous_simple_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_complex_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_data_class_with_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_data_classes_with_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_dataframe_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_dataframe_with_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_enum_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_nested_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_nested_classes_with_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_simple_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_sut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_many_anonymous_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_many_anonymous_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_many_anonymous_nested_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_many_anonymous_nested_classes_with_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_many_anonymous_simple_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_decorator_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:34:49.104710 autofaker-1.0.14/tests/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/unittests/test_decorator_anonymous_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/unittests/test_decorator_anonymous_data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/unittests/test_decorator_anonymous_data_classes_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/unittests/test_decorator_anonymous_dataframe_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/unittests/test_decorator_anonymous_enum_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/unittests/test_decorator_anonymous_nested_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/unittests/test_decorator_anonymous_simple_classes.py
```

### Comparing `autofaker-1.0.12/LICENSE` & `autofaker-1.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/PKG-INFO` & `autofaker-1.0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofaker
-Version: 1.0.12
+Version: 1.0.14
 Summary: Python library designed to minimize the setup/arrange phase of your unit tests
 Home-page: https://github.com/christianhelle/autofaker
 Author: Christian Helle
 Author-email: christian.helle@outlook.com
 License: MIT License
 Description: AutoFaker is a Python library designed to minimize the setup/arrange phase of your unit tests by removing the need to manually 
         write code to create anonymous variables as part of a test cases setup/arrange phase.
```

### Comparing `autofaker-1.0.12/README.md` & `autofaker-1.0.14/README.md`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/setup.py` & `autofaker-1.0.14/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('docs/pypi.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='autofaker',
-    version='1.0.12',
+    version='1.0.14',
     url='https://github.com/christianhelle/autofaker',
     license='MIT License',
     license_files=["LICENSE"],
     author='Christian Helle',
     author_email='christian.helle@outlook.com',
     description='Python library designed to minimize the setup/arrange phase of your unit tests',
     long_description=long_description,
```

### Comparing `autofaker-1.0.12/src/autofaker/attributes.py` & `autofaker-1.0.14/src/autofaker/attributes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/src/autofaker/autodata.py` & `autofaker-1.0.14/src/autofaker/autodata.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/src/autofaker/builtins.py` & `autofaker-1.0.14/src/autofaker/builtins.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/src/autofaker/dataframe.py` & `autofaker-1.0.14/src/autofaker/dataframe.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/src/autofaker/dates.py` & `autofaker-1.0.14/src/autofaker/dates.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/src/autofaker/decorators.py` & `autofaker-1.0.14/src/autofaker/decorators.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/src/autofaker/factory.py` & `autofaker-1.0.14/src/autofaker/factory.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/src/autofaker/fakes.py` & `autofaker-1.0.14/src/autofaker/fakes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/src/autofaker/generator.py` & `autofaker-1.0.14/src/autofaker/generator.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/src/autofaker.egg-info/PKG-INFO` & `autofaker-1.0.14/src/autofaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofaker
-Version: 1.0.12
+Version: 1.0.14
 Summary: Python library designed to minimize the setup/arrange phase of your unit tests
 Home-page: https://github.com/christianhelle/autofaker
 Author: Christian Helle
 Author-email: christian.helle@outlook.com
 License: MIT License
 Description: AutoFaker is a Python library designed to minimize the setup/arrange phase of your unit tests by removing the need to manually 
         write code to create anonymous variables as part of a test cases setup/arrange phase.
```

### Comparing `autofaker-1.0.12/src/autofaker.egg-info/SOURCES.txt` & `autofaker-1.0.14/src/autofaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/pytests/test_decorator_anonymous_builtins.py` & `autofaker-1.0.14/tests/pytests/test_decorator_anonymous_builtins.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/pytests/test_decorator_anonymous_data_classes.py` & `autofaker-1.0.14/tests/pytests/test_decorator_anonymous_data_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/pytests/test_decorator_anonymous_data_classes_nested.py` & `autofaker-1.0.14/tests/pytests/test_decorator_anonymous_data_classes_nested.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/pytests/test_decorator_anonymous_dataframe_pandas.py` & `autofaker-1.0.14/tests/pytests/test_decorator_anonymous_dataframe_pandas.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/pytests/test_decorator_anonymous_nested_classes.py` & `autofaker-1.0.14/tests/pytests/test_decorator_anonymous_nested_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/pytests/test_decorator_anonymous_simple_classes.py` & `autofaker-1.0.14/tests/pytests/test_decorator_anonymous_simple_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_anonymous_builtins.py` & `autofaker-1.0.14/tests/test_create_anonymous_builtins.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_anonymous_complex_classes.py` & `autofaker-1.0.14/tests/test_create_anonymous_complex_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_anonymous_data_class_with_fakes.py` & `autofaker-1.0.14/tests/test_create_anonymous_data_class_with_fakes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_anonymous_data_classes.py` & `autofaker-1.0.14/tests/test_create_anonymous_data_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_anonymous_data_classes_with_fakes.py` & `autofaker-1.0.14/tests/test_create_anonymous_data_classes_with_fakes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_anonymous_dataframe_pandas.py` & `autofaker-1.0.14/tests/test_create_anonymous_dataframe_pandas.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_anonymous_dataframe_with_fakes.py` & `autofaker-1.0.14/tests/test_create_anonymous_dataframe_with_fakes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_anonymous_dates.py` & `autofaker-1.0.14/tests/test_create_anonymous_dates.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_anonymous_lists.py` & `autofaker-1.0.14/tests/test_create_anonymous_lists.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_anonymous_nested_classes.py` & `autofaker-1.0.14/tests/test_create_anonymous_nested_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_anonymous_nested_classes_with_lists.py` & `autofaker-1.0.14/tests/test_create_anonymous_nested_classes_with_lists.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_anonymous_simple_classes.py` & `autofaker-1.0.14/tests/test_create_anonymous_simple_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_anonymous_sut.py` & `autofaker-1.0.14/tests/test_create_anonymous_sut.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_many_anonymous_builtins.py` & `autofaker-1.0.14/tests/test_create_many_anonymous_builtins.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_many_anonymous_dates.py` & `autofaker-1.0.14/tests/test_create_many_anonymous_dates.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_many_anonymous_nested_classes.py` & `autofaker-1.0.14/tests/test_create_many_anonymous_nested_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_many_anonymous_nested_classes_with_lists.py` & `autofaker-1.0.14/tests/test_create_many_anonymous_nested_classes_with_lists.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_create_many_anonymous_simple_classes.py` & `autofaker-1.0.14/tests/test_create_many_anonymous_simple_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/test_decorator_exceptions.py` & `autofaker-1.0.14/tests/test_decorator_exceptions.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/unittests/test_decorator_anonymous_builtins.py` & `autofaker-1.0.14/tests/unittests/test_decorator_anonymous_builtins.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/unittests/test_decorator_anonymous_data_classes.py` & `autofaker-1.0.14/tests/unittests/test_decorator_anonymous_data_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/unittests/test_decorator_anonymous_data_classes_nested.py` & `autofaker-1.0.14/tests/unittests/test_decorator_anonymous_data_classes_nested.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/unittests/test_decorator_anonymous_dataframe_pandas.py` & `autofaker-1.0.14/tests/unittests/test_decorator_anonymous_dataframe_pandas.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/unittests/test_decorator_anonymous_nested_classes.py` & `autofaker-1.0.14/tests/unittests/test_decorator_anonymous_nested_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.12/tests/unittests/test_decorator_anonymous_simple_classes.py` & `autofaker-1.0.14/tests/unittests/test_decorator_anonymous_simple_classes.py`

 * *Files identical despite different names*

