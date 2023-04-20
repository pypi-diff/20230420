# Comparing `tmp/widgets-lib-2.7.1.tar.gz` & `tmp/widgets-lib-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widgets-lib-2.7.1.tar", last modified: Wed Apr 19 18:06:03 2023, max compression
+gzip compressed data, was "widgets-lib-2.7.2.tar", last modified: Thu Apr 20 16:30:29 2023, max compression
```

## Comparing `widgets-lib-2.7.1.tar` & `widgets-lib-2.7.2.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:06:03.768848 widgets-lib-2.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-19 18:06:03.768848 widgets-lib-2.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:06:03.768848 widgets-lib-2.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:06:03.748848 widgets-lib-2.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:06:03.752848 widgets-lib-2.7.1/src/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:06:03.760848 widgets-lib-2.7.1/src/widgets/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/base/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/base/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/base/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:06:03.760848 widgets-lib-2.7.1/src/widgets/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:06:03.760848 widgets-lib-2.7.1/src/widgets/st_base/
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/st_base/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/st_base/value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:06:03.760848 widgets-lib-2.7.1/src/widgets/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:06:03.760848 widgets-lib-2.7.1/src/widgets/streamlit/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/duplicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/expander.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:06:03.760848 widgets-lib-2.7.1/src/widgets/streamlit/resource/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/files/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/files/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/files/download_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:06:03.764848 widgets-lib-2.7.1/src/widgets/streamlit/resource/values/
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/values/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/values/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/values/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/values/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/values/selectstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/values/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/values/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/resource/values/textarea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:06:03.764848 widgets-lib-2.7.1/src/widgets/streamlit/widget/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/streamlit/widget/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:06:03.764848 widgets-lib-2.7.1/src/widgets/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/templates/source.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/templates/streamlit_single.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/src/widgets/templates/streamlit_single.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:06:03.764848 widgets-lib-2.7.1/src/widgets_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-19 18:06:03.000000 widgets-lib-2.7.1/src/widgets_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-19 18:06:03.000000 widgets-lib-2.7.1/src/widgets_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:06:03.000000 widgets-lib-2.7.1/src/widgets_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 18:06:03.000000 widgets-lib-2.7.1/src/widgets_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 18:06:03.000000 widgets-lib-2.7.1/src/widgets_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 18:06:03.000000 widgets-lib-2.7.1/src/widgets_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:06:03.764848 widgets-lib-2.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/tests/test_duplicator.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/tests/test_source_parents.py
--rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-04-19 18:05:18.000000 widgets-lib-2.7.1/tests/test_streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.842292 widgets-lib-2.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-20 16:30:29.842292 widgets-lib-2.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:30:29.842292 widgets-lib-2.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.834292 widgets-lib-2.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.834292 widgets-lib-2.7.2/src/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.834292 widgets-lib-2.7.2/src/widgets/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/base/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/base/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/base/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.834292 widgets-lib-2.7.2/src/widgets/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.834292 widgets-lib-2.7.2/src/widgets/st_base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/st_base/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/st_base/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.834292 widgets-lib-2.7.2/src/widgets/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.838292 widgets-lib-2.7.2/src/widgets/streamlit/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/duplicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/expander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.838292 widgets-lib-2.7.2/src/widgets/streamlit/resource/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/files/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/files/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/files/download_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.838292 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/selectstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/textarea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.838292 widgets-lib-2.7.2/src/widgets/streamlit/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/widget/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.838292 widgets-lib-2.7.2/src/widgets/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/templates/source.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/templates/streamlit_single.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/templates/streamlit_single.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/templates/streamlit_single_ga.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.838292 widgets-lib-2.7.2/src/widgets_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-20 16:30:29.000000 widgets-lib-2.7.2/src/widgets_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-20 16:30:29.000000 widgets-lib-2.7.2/src/widgets_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:30:29.000000 widgets-lib-2.7.2/src/widgets_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 16:30:29.000000 widgets-lib-2.7.2/src/widgets_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 16:30:29.000000 widgets-lib-2.7.2/src/widgets_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 16:30:29.000000 widgets-lib-2.7.2/src/widgets_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.842292 widgets-lib-2.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/tests/test_duplicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/tests/test_source_parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/tests/test_streamlit.py
```

### Comparing `widgets-lib-2.7.1/LICENSE` & `widgets-lib-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/PKG-INFO` & `widgets-lib-2.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgets-lib
-Version: 2.7.1
+Version: 2.7.2
 Summary: Merging code and data in webpages
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `widgets-lib-2.7.1/README.md` & `widgets-lib-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/pyproject.toml` & `widgets-lib-2.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/base/exceptions.py` & `widgets-lib-2.7.2/src/widgets/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/base/helpers.py` & `widgets-lib-2.7.2/src/widgets/base/helpers.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/base/io.py` & `widgets-lib-2.7.2/src/widgets/base/io.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/base/resource.py` & `widgets-lib-2.7.2/src/widgets/base/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -320,16 +320,25 @@
         Recursively traverse child elements to gather the source code for all
         Resource-based classes which are defined in the main scope.
         """
 
         # If this element was not defined in the widgets module
         if not self.__class__.__module__.startswith('widget'):
 
+            # If this element has already been added
+            if self._name() in gathered_source:
+
+                # Insert the source at the end of the dict
+                # so that it is bumped to the top of the source code
+                src = gathered_source[self._name()]
+                del gathered_source[self._name()]
+                gathered_source[self._name()] = src
+
             # If this element has not been added
-            if self._name() not in gathered_source:
+            else:
 
                 # Add it
                 gathered_source[self._name()] = self.source_self()
 
             # Recursively add the parent element
             p = self._parent_class()()
             gathered_source = p._recursive_source(
```

### Comparing `widgets-lib-2.7.1/src/widgets/base/widget.py` & `widgets-lib-2.7.2/src/widgets/base/widget.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/cli/main.py` & `widgets-lib-2.7.2/src/widgets/cli/main.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/st_base/resource.py` & `widgets-lib-2.7.2/src/widgets/st_base/resource.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/st_base/value.py` & `widgets-lib-2.7.2/src/widgets/st_base/value.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/__init__.py` & `widgets-lib-2.7.2/src/widgets/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/columns.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/columns.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/duplicator.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/duplicator.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/expander.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/expander.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/files/base.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/files/base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/files/dataframe.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/files/dataframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,8 +86,8 @@
 
         if isinstance(val, str):
             return f'"{val}"'
         elif isinstance(val, pd.DataFrame):
             return encode_dataframe_string(val)
 
         else:
-            return val
+            return super()._source_val(val)
```

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/files/download_dataframe.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/files/download_dataframe.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/markdown.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/markdown.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/selector.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/selector.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/values/checkbox.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/checkbox.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/values/float.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/float.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/values/integer.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/integer.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/values/multiselect.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/multiselect.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/values/selectstring.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/selectstring.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/values/slider.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/slider.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/values/string.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/string.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/resource/values/textarea.py` & `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/textarea.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/src/widgets/streamlit/widget/base.py` & `widgets-lib-2.7.2/src/widgets/streamlit/widget/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,36 +25,41 @@
 
     # "auto" or "expanded" or "collapsed"
     initial_sidebar_state = "auto"
 
     # "centered" or "wide"
     layout = "centered"
 
+    # Optional GA tag
+    ga_tag = None
+
     title = ""
     subtitle = ""
 
     def __init__(
         self,
         requirements: Union[List[str], None] = None,
         pyodide_requirements: Union[List[str], None] = None,
         imports: Union[List[str], None] = None,
         extra_imports: Union[List[str], None] = None,
         initial_sidebar_state: Union[str, None] = None,
         layout: Union[str, None] = None,
+        ga_tag: Union[str, None] = None,
         title: Union[str, None] = None,
         subtitle: Union[str, None] = None,
         **kwargs
     ):
         super().__init__(
             requirements=self.__class__.requirements,
             pyodide_requirements=self.__class__.pyodide_requirements,
             imports=self.__class__.imports,
             extra_imports=self.__class__.extra_imports,
             initial_sidebar_state=self.__class__.initial_sidebar_state,
             layout=self.__class__.layout,
+            ga_tag=self.__class__.ga_tag,
             title=self.__class__.title,
             subtitle=self.__class__.subtitle,
             **kwargs
         )
 
     def prep(self) -> None:
         """
@@ -97,16 +102,15 @@
             from streamlit.web.cli import _main_run
             _main_run(script.name, args, flag_options=flag_options)
 
     def clone_button(
             self,
             sidebar=True,
             as_html=True,
-            as_script=True,
-            footer="Widget (github.com/FredHutch/widgets)"
+            as_script=True
     ):
         """
         Render a button which gives the user the option to download a
         cloned copy of this widget.
         Importantly, the code is only generated once the button is
         initially pressed, which should make it more performant than
         download_html_button and download_script_buton, which have to
@@ -128,16 +132,15 @@
 
             if as_html:
                 button_container.download_button(
                     "Download HTML",
                     self._render_html(
                         title=self._name(),
                         layout=self.layout,
-                        initial_sidebar_state=self.initial_sidebar_state,
-                        footer=footer
+                        initial_sidebar_state=self.initial_sidebar_state
                     ),
                     file_name=f"{self._name()}.html",
                     mime="text/html",
                     help="Download this widget as a webpage (HTML)",
                     use_container_width=True,
                     on_click=self._set_session_state,
                     args=('_ready_to_clone', False)
@@ -165,16 +168,15 @@
 
     def _set_session_state(self, kw, val):
         """Utility to set a value in the session state."""
         st.session_state[kw] = val
 
     def download_html_button(
         self,
-        sidebar=True,
-        footer="Widget (github.com/FredHutch/widgets)"
+        sidebar=True
     ):
         """
         Render a button which allows the user to download the widget as HTML.
         """
 
         col1, col2, col3 = self._get_ui_element(
             sidebar=sidebar,
@@ -182,16 +184,15 @@
         ).columns(3)
 
         col2.download_button(
             "Download HTML",
             self._render_html(
                 title=self._name(),
                 layout=self.layout,
-                initial_sidebar_state=self.initial_sidebar_state,
-                footer=footer
+                initial_sidebar_state=self.initial_sidebar_state
             ),
             file_name=f"{self._name()}.html",
             mime="text/html",
             help="Download this widget as a webpage (HTML)",
             use_container_width=True
         )
 
@@ -252,29 +253,27 @@
         fp.seek(0)
 
         # Return the file object
         return fp
 
     def to_html(
         self,
-        fp: Union[Path, None] = None,
-        footer="Widget (github.com/FredHutch/widgets)"
+        fp: Union[Path, None] = None
     ) -> Union[None, str]:
         """
         Create an HTML file which will load this widget using the stlite
         library, based on pyodide.
         If no path is provided, return a string representation.
         """
 
         # Create the HTML as a string
         html = self._render_html(
             title=self._name(),
             layout=self.layout,
-            initial_sidebar_state=self.initial_sidebar_state,
-            footer=footer
+            initial_sidebar_state=self.initial_sidebar_state
         )
 
         # Write it out to a file (if provided), or return the string
         return self._to_file(html, fp)
 
     def to_script(self, fp: Union[Path, None] = None) -> Union[None, str]:
         """
@@ -294,41 +293,51 @@
         return "\n".join(["\n".join(self.imports), "\n".join(self.extra_imports)]) # noqa
 
     def _render_html(
         self,
         title="Widget",
         layout="centered",
         initial_sidebar_state="auto",
-        footer="Widget (github.com/FredHutch/widgets)",
-        stlite_ver="0.29.15",
+        stlite_ver="0.31.0",
     ):
         """Render the widget as HTML"""
 
         # Pin the version of all requirements
         requirements = [
             self._pin_module_version(module)
             for module in self.requirements
         ] + [
             f"widgets-lib=={widgets.__version__}"
         ]
 
-        # Render the template for this HTML
-        html = render_template(
-            "streamlit_single.html.j2",
+        # Set up the contents of the HTML
+        kwargs = dict(
             title=title,
             layout=layout,
             initial_sidebar_state=initial_sidebar_state,
             stlite_ver=stlite_ver,
-            footer=footer,
             requirements=requirements,
             imports=self._imports(),
             widget_source=self.source_all().replace("\\", "\\\\"),
             widget_name=self._name()
         )
 
+        # Select the template based on whether a ga_tag exists
+        if self.ga_tag is None:
+            template = "streamlit_single.html.j2"
+        else:
+            template = "streamlit_single_ga.html.j2"
+            kwargs['ga_tag'] = self.ga_tag
+
+        # Render the template for this HTML
+        html = render_template(
+            template,
+            **kwargs
+        )
+
         return html
 
     def _pin_module_version(self, module):
         """
         Pin a module version, if possible.
         Do not pin a version for any packages which are
         listed in self.pyodide_requirements.
```

### Comparing `widgets-lib-2.7.1/src/widgets_lib.egg-info/PKG-INFO` & `widgets-lib-2.7.2/src/widgets_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgets-lib
-Version: 2.7.1
+Version: 2.7.2
 Summary: Merging code and data in webpages
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `widgets-lib-2.7.1/src/widgets_lib.egg-info/SOURCES.txt` & `widgets-lib-2.7.2/src/widgets_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 src/widgets/streamlit/resource/values/string.py
 src/widgets/streamlit/resource/values/textarea.py
 src/widgets/streamlit/widget/__init__.py
 src/widgets/streamlit/widget/base.py
 src/widgets/templates/source.py.j2
 src/widgets/templates/streamlit_single.html.j2
 src/widgets/templates/streamlit_single.py.j2
+src/widgets/templates/streamlit_single_ga.html.j2
 src/widgets_lib.egg-info/PKG-INFO
 src/widgets_lib.egg-info/SOURCES.txt
 src/widgets_lib.egg-info/dependency_links.txt
 src/widgets_lib.egg-info/entry_points.txt
 src/widgets_lib.egg-info/requires.txt
 src/widgets_lib.egg-info/top_level.txt
 tests/test_base.py
```

### Comparing `widgets-lib-2.7.1/tests/test_base.py` & `widgets-lib-2.7.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/tests/test_cli.py` & `widgets-lib-2.7.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/tests/test_duplicator.py` & `widgets-lib-2.7.2/tests/test_duplicator.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/tests/test_helpers.py` & `widgets-lib-2.7.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/tests/test_io.py` & `widgets-lib-2.7.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/tests/test_source_parents.py` & `widgets-lib-2.7.2/tests/test_source_parents.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.1/tests/test_streamlit.py` & `widgets-lib-2.7.2/tests/test_streamlit.py`

 * *Files identical despite different names*

