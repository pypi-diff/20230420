# Comparing `tmp/pyplotterlib-1.4.0.tar.gz` & `tmp/pyplotterlib-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplotterlib-1.4.0.tar", last modified: Wed Dec 28 19:24:27 2022, max compression
+gzip compressed data, was "pyplotterlib-1.5.0.tar", last modified: Thu Apr 20 09:31:28 2023, max compression
```

## Comparing `pyplotterlib-1.4.0.tar` & `pyplotterlib-1.5.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.853796 pyplotterlib-1.4.0/
--rw-rw-r--   0 richard   (1000) richard   (1000)     1066 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/LICENSE
--rw-rw-r--   0 richard   (1000) richard   (1000)     2054 2022-12-28 19:24:27.853796 pyplotterlib-1.4.0/PKG-INFO
--rw-rw-r--   0 richard   (1000) richard   (1000)      151 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/README.md
--rw-rw-r--   0 richard   (1000) richard   (1000)     1124 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/pyproject.toml
--rw-rw-r--   0 richard   (1000) richard   (1000)       38 2022-12-28 19:24:27.853796 pyplotterlib-1.4.0/setup.cfg
--rw-rw-r--   0 richard   (1000) richard   (1000)       50 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/setup.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.849796 pyplotterlib-1.4.0/src/
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.849796 pyplotterlib-1.4.0/src/pyplotterlib/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/__init__.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.849796 pyplotterlib-1.4.0/src/pyplotterlib/core/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/core/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      570 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/core/json_transform.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1088 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/core/plot_command.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    11890 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/core/plot_options.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     5558 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/core/plotters.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.849796 pyplotterlib-1.4.0/src/pyplotterlib/core/serialization/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/core/serialization/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      510 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/core/serialization/json_io.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      175 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/core/serialization/register.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2617 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/core/serialization/registration_funct.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.849796 pyplotterlib-1.4.0/src/pyplotterlib/core/serialization/unit_tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/core/serialization/unit_tests/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2222 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/core/serialization/unit_tests/utest_create_from_json.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.853796 pyplotterlib-1.4.0/src/pyplotterlib/core/unit_tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/core/unit_tests/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    17393 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/core/unit_tests/utest_plot_options.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     5031 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/core/unit_tests/utest_plotters.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.853796 pyplotterlib-1.4.0/src/pyplotterlib/reg_testing/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/reg_testing/__init__.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.853796 pyplotterlib-1.4.0/src/pyplotterlib/reg_testing/read_serialization_test/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/reg_testing/read_serialization_test/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1276 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/reg_testing/read_serialization_test/helpers.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      570 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/reg_testing/shared.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.853796 pyplotterlib-1.4.0/src/pyplotterlib/reg_testing/viz_diff/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/reg_testing/viz_diff/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1693 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/reg_testing/viz_diff/helpers.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.853796 pyplotterlib-1.4.0/src/pyplotterlib/standard/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    36353 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/plot_commands.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    26292 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/plot_options.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      911 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/plotters.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.853796 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    10864 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/bar_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    16170 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/box_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    15049 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/disc_heat_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     8449 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/histogram_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     5391 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/image_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4129 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/line_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    23966 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/rect_multi_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2686 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/shared.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     5300 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/shared_axis_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    18443 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/split_axis_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    23588 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/split_axis_plotter_creator.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.853796 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/unit_tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/unit_tests/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2079 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/private/unit_tests/utests_histogram_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1937 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/serialization.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.853796 pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/__init__.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.853796 pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1119 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_bar_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      888 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_histogram_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      951 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_image_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1269 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_line_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1049 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_rect_multi_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1093 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_shared_axis_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1289 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_creator.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1059 2022-12-28 19:24:07.000000 pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_plotter.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2022-12-28 19:24:27.849796 pyplotterlib-1.4.0/src/pyplotterlib.egg-info/
--rw-rw-r--   0 richard   (1000) richard   (1000)     2054 2022-12-28 19:24:27.000000 pyplotterlib-1.4.0/src/pyplotterlib.egg-info/PKG-INFO
--rw-rw-r--   0 richard   (1000) richard   (1000)     2945 2022-12-28 19:24:27.000000 pyplotterlib-1.4.0/src/pyplotterlib.egg-info/SOURCES.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)        1 2022-12-28 19:24:27.000000 pyplotterlib-1.4.0/src/pyplotterlib.egg-info/dependency_links.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)      110 2022-12-28 19:24:27.000000 pyplotterlib-1.4.0/src/pyplotterlib.egg-info/requires.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)       13 2022-12-28 19:24:27.000000 pyplotterlib-1.4.0/src/pyplotterlib.egg-info/top_level.txt
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1066 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/LICENSE
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2054 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/PKG-INFO
+-rw-rw-r--   0 richard   (1000) richard   (1000)      151 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/README.md
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1124 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/pyproject.toml
+-rw-rw-r--   0 richard   (1000) richard   (1000)       38 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/setup.cfg
+-rw-rw-r--   0 richard   (1000) richard   (1000)       50 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/setup.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.532442 pyplotterlib-1.5.0/src/
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/__init__.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/core/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      570 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/json_transform.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1088 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/plot_command.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    11890 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/plot_options.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     5558 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/plotters.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      510 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/json_io.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      175 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/register.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2617 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/registration_funct.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/unit_tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/unit_tests/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2222 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/unit_tests/utest_create_from_json.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/core/unit_tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/unit_tests/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    17393 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/unit_tests/utest_plot_options.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     5031 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/unit_tests/utest_plotters.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/__init__.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/read_serialization_test/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/read_serialization_test/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1276 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/read_serialization_test/helpers.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      570 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/shared.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/viz_diff/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/viz_diff/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1693 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/viz_diff/helpers.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/standard/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    37511 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/plot_commands.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    27328 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/plot_options.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      911 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/plotters.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    10931 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/bar_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    16170 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/box_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    15587 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/disc_heat_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     8516 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/histogram_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     4673 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/image_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     4129 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/line_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    23966 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/rect_multi_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2686 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/shared.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     5300 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/shared_axis_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    18443 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/split_axis_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    23588 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/split_axis_plotter_creator.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/unit_tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/unit_tests/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2079 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/unit_tests/utests_histogram_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1937 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/serialization.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/__init__.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1119 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_bar_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      888 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_histogram_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      951 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_image_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1269 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_line_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1049 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_rect_multi_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1093 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_shared_axis_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1289 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_creator.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1059 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_plotter.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib.egg-info/
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2054 2023-04-20 09:31:28.000000 pyplotterlib-1.5.0/src/pyplotterlib.egg-info/PKG-INFO
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2945 2023-04-20 09:31:28.000000 pyplotterlib-1.5.0/src/pyplotterlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)        1 2023-04-20 09:31:28.000000 pyplotterlib-1.5.0/src/pyplotterlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)      110 2023-04-20 09:31:28.000000 pyplotterlib-1.5.0/src/pyplotterlib.egg-info/requires.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)       13 2023-04-20 09:31:28.000000 pyplotterlib-1.5.0/src/pyplotterlib.egg-info/top_level.txt
```

### Comparing `pyplotterlib-1.4.0/LICENSE` & `pyplotterlib-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/PKG-INFO` & `pyplotterlib-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplotterlib
-Version: 1.4.0
+Version: 1.5.0
 Summary: A package used to create plots in python
 Author-email: Richard Fogarty <richard.m.fogarty@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 RFogarty1
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyplotterlib-1.4.0/pyproject.toml` & `pyplotterlib-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=60.9.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyplotterlib"
-version = "1.4.0"
+version = "1.5.0"
 description = "A package used to create plots in python"
 readme = "README.md"
 authors = [{ name = "Richard Fogarty", email = "richard.m.fogarty@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Framework :: Matplotlib",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/core/json_transform.py` & `pyplotterlib-1.5.0/src/pyplotterlib/core/json_transform.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/core/plot_command.py` & `pyplotterlib-1.5.0/src/pyplotterlib/core/plot_command.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/core/plot_options.py` & `pyplotterlib-1.5.0/src/pyplotterlib/core/plot_options.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/core/plotters.py` & `pyplotterlib-1.5.0/src/pyplotterlib/core/plotters.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/core/serialization/registration_funct.py` & `pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/registration_funct.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/core/serialization/unit_tests/utest_create_from_json.py` & `pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/unit_tests/utest_create_from_json.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/core/unit_tests/utest_plot_options.py` & `pyplotterlib-1.5.0/src/pyplotterlib/core/unit_tests/utest_plot_options.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/core/unit_tests/utest_plotters.py` & `pyplotterlib-1.5.0/src/pyplotterlib/core/unit_tests/utest_plotters.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/reg_testing/read_serialization_test/helpers.py` & `pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/read_serialization_test/helpers.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/reg_testing/shared.py` & `pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/shared.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/reg_testing/viz_diff/helpers.py` & `pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/viz_diff/helpers.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/plot_commands.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/plot_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,14 +338,29 @@
 			linePositions = [linePositions]
 		else:
 			pass
 
 		return linePositions
 
 
+@serializationReg.registerForSerialization()
+class SetAspectStr(plotCommCoreHelp.PlotCommand):
+
+	def __init__(self):
+		self._name = "set-aspect-str"
+		self._description = "Sets the aspect string for the axis"
+		self._optName = "aspectStr"
+
+	def execute(self, plotterInstance):
+		aspectStr = _getValueFromOptName(plotterInstance, self._optName)
+		if aspectStr is None:
+			return None
+		else:
+			_setScratchSpaceDictKey(plotterInstance, "plotKwargs", "aspect", aspectStr)
+
 
 @serializationReg.registerForSerialization()
 class SetAxisBorderInvisible(plotCommCoreHelp.PlotCommand):
 
 	def __init__(self):
 		self._name = "SetAxisBorderVisibility"
 		self._description = "Sets the border visibility for various axes (top/bottom/left/right)"
@@ -540,14 +555,36 @@
 
 		for color,barSet in zip(useColors,plottedBars):
 			_children = barSet.get_children()
 			for child in _children:
 				child.set_color(color)
 
 @serializationReg.registerForSerialization()
+class SetBarOpacities(plotCommCoreHelp.PlotCommand):
+
+	def __init__(self):
+		self._name = "set-opacities-for-bars"
+		self._description = "Sets the opacities for a series of bars"
+		self._optName = "barOpacities"
+
+	def execute(self, plotterInstance):
+		opacities = getattr(plotterInstance.opts, self._optName).value
+		plottedBars = plotterInstance._scratchSpace.get("barHandles", None)
+
+		if (plottedBars is None) or (opacities is None):
+			return None
+
+		useOpacities = it.cycle(opacities)
+		for opacity, barSet in zip(useOpacities, plottedBars):
+			_children = barSet.get_children()
+			for child in _children:
+				child.set_alpha(opacity)
+
+
+@serializationReg.registerForSerialization()
 class SetColorbarFontSizes(plotCommCoreHelp.PlotCommand):
 
 	def __init__(self):
 		self._name = "set-color-bar-fonts"
 		self._description = "Sets the font sizes on the color bar (if its present)"
 		self._dictKey = "cbar"
```

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/plot_options.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/plot_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 import types
 
 import numpy as np
 
 from ..core import plot_options as plotOptCore
 from ..core.serialization import register as serializationReg
 
+@serializationReg.registerForSerialization()
+class AspectString(plotOptCore.StringPlotOption):
+	""" String controlling how the image aspect works
+
+	equal: Pixels kept square; aspect ratio is maintained but axes may not fill the space
+	auto: Aspect ratio is altered such that the image fits the axes; may be useful when creating grids of images
+
+	"""
+	def __init__(self, name=None, value=None):
+		self.name = "aspectStr"
+		self.value = value
 
 @serializationReg.registerForSerialization()
 class AxisBorderMakeInvisible(plotOptCore.BoolNamespaceOption):
 	""" Namespace controlling visibility of axis borders. Access values with .value.top, .value.bottom, .value.left, .value.right.
 
 	Setting to True should hide that border, including any tick markers. This is useful for split axis plotters.
 
@@ -91,14 +102,25 @@
 
 	"""
 	def __init__(self, name=None, value=None):
 		self.name = "barColors"
 		self.value = value
 
 @serializationReg.registerForSerialization()
+class BarOpacities(plotOptCore.FloatIterPlotOption):
+	""" The opacities to use for each bar. Values should be between 0 (invisible) and 1 (fully opaque). Corresponds to the alpha keyword in matplotlib.
+
+	Note: The number of values doesnt have to match the number of data series, if you provide too few values, they should cycle. For example setting [0.5,1.0] may lead to plotted opacities of [0.5, 1.0, 0.5, 1.0, .... etc]
+
+	"""
+	def __init__(self, name=None, value=None):
+		self.name = "barOpacities" if name is None else name
+		self.value = value
+
+@serializationReg.registerForSerialization()
 class ColorBarFontSize(plotOptCore.IntPlotOption):
 	""" The font size to use for the colorbar
 	
 	"""
 	def __init__(self, name=None, value=None):
 		self.name = "colorBarFontSize"
 		self.value = value
```

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/plotters.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/plotters.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/private/bar_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/bar_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 	PlotOneDimDataAsBars(),
 	SetTickValsToGroupCentres(),
 	SetTickLabelsToGroupLabels(),
 	SetTickMinorValsOnOrOff(),
 	plotCmdStdHelp.GridLinesCreate(),
 	SetBarDataLabels(),
 	plotCmdStdHelp.SetBarColors(),
+	plotCmdStdHelp.SetBarOpacities(),
 	plotCmdStdHelp.SetXLabelStr(),
 	plotCmdStdHelp.SetYLabelStr(),
 	plotCmdStdHelp.SetTickLabelFontSize(),
 	plotCmdStdHelp.SetXLabelFractPos(),
 	plotCmdStdHelp.SetYLabelFractPos(),
 	plotCmdStdHelp.SetXLimit(),
 	plotCmdStdHelp.SetYLimit(),
@@ -78,14 +79,15 @@
 	outList = [
 	plotOptStdHelp.AxisBorderMakeInvisible(),
 	plotOptStdHelp.AxisColorX(),
 	plotOptStdHelp.AxisColorX_exclSpines(),
 	plotOptStdHelp.AxisColorY(),
 	plotOptStdHelp.AxisColorY_exclSpines(),
 	plotOptStdHelp.BarColors(),
+	plotOptStdHelp.BarOpacities(),
 	plotOptStdHelp.DataLabels(),
 	plotOptStdHelp.FontSizeDefault(),
 	plotOptStdHelp.GridLinesShow(value=False),
 	plotOptStdHelp.GridLinesShowX(),
 	plotOptStdHelp.GridLinesShowY(),
 	plotOptStdHelp.GridLinesStyle(),
 	plotOptStdHelp.GridLinesWidth(),
```

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/private/box_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/box_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/private/disc_heat_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/disc_heat_plotter.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 		self._options = plotOptCoreHelp.OptionsCollection(options=_optionsList)
 
 
 
 def _createCommandsList():
 	outList = [
 	plotCmdStdHelp.CreateFigureIfNoAxHandle(),
+	plotCmdStdHelp.SetAspectStr(),
 	plotCmdStdHelp.AddPlotterToOutput(),
 	plotCmdStdHelp.CopyNumpyArrayPlotDataToScratchSpace(),
 	RemoveUnwantedPlotData(),
 	plotCmdStdHelp.SetColormapInPlotKwargs(),
 	plotCmdStdHelp.SetColormapMaxValInPlotKwargs(),
 	plotCmdStdHelp.SetColormapMinValInPlotKwargs(),
 	AddDataToPlot(),
@@ -67,16 +68,18 @@
 	]
 	return outList
 
 def _createOptionsList():
 	outList = [
 	AnnotateVals(),
 	AnnotateValsFontSize(),
+	AnnotateValsRotation(),
 	AnnotateValsStrFmt(value="{:.2f}"),
 	AnnotateValsTextColor(),
+	plotOptStdHelp.AspectString(value="auto"),
 	plotOptStdHelp.ColorBarFontSize(),
 	plotOptStdHelp.ColorBarLabelFontSize(),
 	plotOptStdHelp.ColorBarTickLabelFontSize(),
 	plotOptStdHelp.ColorBarLabel(),
 	plotOptStdHelp.ColorBarLocation(),
 	plotOptStdHelp.ColorBarShow(),
 	plotOptStdHelp.ColorBarLabelRotation(),
@@ -94,14 +97,15 @@
 	GroupLabelsColsRotation(),
 	GroupLabelsRows(),
 	GroupLabelsRowsRotation(),
 	PlotDataDiscHeat(),
 	PlotDiag(value=True),
 	PlotLowerTri(value=True),
 	PlotUpperTri(value=True),
+	plotOptStdHelp.SetFigsizeOnCreation(),
 	plotOptStdHelp.TitleStr(),
 	plotOptStdHelp.XLabelStr(),
 	plotOptStdHelp.YLabelStr()
 	]
 	return outList
 
 
@@ -121,14 +125,23 @@
 	
 	"""
 	def __init__(self, name=None, value=None):
 		self.name = "annotateValsFontSize"
 		self.value = value
 
 @serializationReg.registerForSerialization()
+class AnnotateValsRotation(plotOptCoreHelp.FloatPlotOption):
+	""" The rotation of text annotations. Units are degrees
+
+	"""
+	def __init__(self, name=None, value=None):
+		self.name = "annotateValsRotation"
+		self.value = value
+
+@serializationReg.registerForSerialization()
 class AnnotateValsStrFmt(plotOptCoreHelp.StringPlotOption):
 	""" The string format to use when generating annotation values from data. E.g. "{:.2f}" means use two decimal places. We generate each annotation by applying AnnotateValsStrFmt.value.format(x) [where x is the plotted data value]
 	
 	"""
 	def __init__(self, name=None, value=None):
 		self.name = "annotateValsStrFmt"
 		self.value = value
@@ -252,26 +265,27 @@
 			return None
 		data = np.array(data)
 
 		#Add the text annotations
 		fmtStr = plotCmdStdHelp._getValueFromOptName(plotterInstance,"annotateValsStrFmt", retIfNone="{}")
 		nRows, nCols = data.shape
 		annotateColor = plotCmdStdHelp._getValueFromOptName(plotterInstance, "annotateValsTextColor")
+		annotateRotation = plotCmdStdHelp._getValueFromOptName(plotterInstance, "annotateValsRotation")
 
 		useFontSize = plotCmdStdHelp._getValueFromOptName(plotterInstance, "fontSizeDefault")
 		useFontSize = plotCmdStdHelp._getValueFromOptName(plotterInstance, "annotateValsFontSize", retIfNone=useFontSize)
 
 		colorArray = self._getColorArray(plotterInstance, data)
 
 		for rIdx in range(nRows):
 			for cIdx in range(nCols):
 				currVal = data[rIdx,cIdx]
 				if not np.isnan(currVal):
 					plt.gca().text(cIdx, rIdx, fmtStr.format(currVal),
-					               ha="center", va="center", color=colorArray[rIdx][cIdx], fontsize=useFontSize)
+					               ha="center", va="center", color=colorArray[rIdx][cIdx], fontsize=useFontSize, rotation=annotateRotation)
 
 
 	def _getColorArray(self, plotterInstance, inpData):
 		outArray = np.empty( inpData.shape, dtype= object )
 		nRows, nCols = inpData.shape
 		colors = self._getListOfColorsToUse(plotterInstance)
```

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/private/histogram_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/histogram_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 def _createCommandsList():
 	outList = [
 	plotCmdStdHelp.CreateFigureIfNoAxHandle(),
 	PlotHistoData(),
 	plotCmdStdHelp.SetBarDataLabels(),
 	plotCmdStdHelp.SetBarColors(),
+	plotCmdStdHelp.SetBarOpacities(),
 	plotCmdStdHelp.GridLinesCreate(),
 	plotCmdStdHelp.SetXLabelStr(),
 	plotCmdStdHelp.SetYLabelStr(),
 	plotCmdStdHelp.SetTickMarkerValues(),
 	plotCmdStdHelp.SetTickLabelValues(),
 	plotCmdStdHelp.SetTickLabelFontSize(),
 	plotCmdStdHelp.SetAxisTickAndLabelVisibilitiesEachSide(),
@@ -79,14 +80,15 @@
 	outList = [
 	plotOptStdHelp.AxisBorderMakeInvisible(),
 	plotOptStdHelp.AxisColorX(),
 	plotOptStdHelp.AxisColorX_exclSpines(),
 	plotOptStdHelp.AxisColorY(),
 	plotOptStdHelp.AxisColorY_exclSpines(),
 	plotOptStdHelp.BarColors(),
+	plotOptStdHelp.BarOpacities(),
 	plotOptStdHelp.DataLabels(),
 	plotOptStdHelp.FontSizeDefault(),
 	plotOptStdHelp.GridLinesShow(value=False),
 	plotOptStdHelp.GridLinesShowX(),
 	plotOptStdHelp.GridLinesShowY(),
 	plotOptStdHelp.GridLinesStyle(),
 	plotOptStdHelp.GridLinesWidth(),
```

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/private/image_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/image_plotter.py`

 * *Files 11% similar despite different names*

```diff
@@ -101,24 +101,16 @@
 	]
 
 	return outList
 
 
 #Options
 @serializationReg.registerForSerialization()
-class AspectString(plotOptCoreHelp.StringPlotOption):
-	""" String controlling how the image aspect works
-
-	equal: Pixels kept square; aspect ratio is maintained but axes may not fill the space
-	auto: Aspect ratio is altered such that the image fits the axes; may be useful when creating grids of images
-
-	"""
-	def __init__(self, name=None, value=None):
-		self.name = "aspectStr"
-		self.value = value
+class AspectString(plotOptStdHelp.AspectString):
+	pass
 
 @serializationReg.registerForSerialization()
 class ColormapStr(plotOptStdHelp.ColormapStr):
 	pass
 
 @serializationReg.registerForSerialization()
 class PlotDataImage(plotOptCoreHelp.NumpyArrayPlotOption):
@@ -154,26 +146,16 @@
 			plt.imshow(data, **plotterInstance._scratchSpace["plotKwargs"])
 
 @serializationReg.registerForSerialization()
 class AddColorBar(plotCmdStdHelp.AddColorBar):
 	pass
 
 @serializationReg.registerForSerialization()
-class SetAspectStr(plotCmdCoreHelp.PlotCommand):
-
-	def __init__(self):
-		self._name = "set-aspect-str"
-		self._description = "Sets the aspect string for the axis"
-		self._optName = "aspectStr"
+class SetAspectStr(plotCmdStdHelp.SetAspectStr):
+	pass
 
-	def execute(self, plotterInstance):
-		aspectStr = plotCmdStdHelp._getValueFromOptName(plotterInstance, self._optName)
-		if aspectStr is None:
-			return None
-		else:
-			plotterInstance._scratchSpace["plotKwargs"]["aspect"] = aspectStr
 
 @serializationReg.registerForSerialization()
 class SetColormap(plotCmdStdHelp.SetColormapInPlotKwargs):
 	pass
```

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/private/line_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/line_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/private/rect_multi_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/rect_multi_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/private/shared.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/shared.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/private/shared_axis_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/shared_axis_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/private/split_axis_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/split_axis_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/private/split_axis_plotter_creator.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/split_axis_plotter_creator.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/private/unit_tests/utests_histogram_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/unit_tests/utests_histogram_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/serialization.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/serialization.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_bar_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_bar_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_histogram_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_histogram_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_image_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_image_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_line_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_line_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_rect_multi_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_rect_multi_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_shared_axis_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_shared_axis_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_creator.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_creator.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_plotter.py` & `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib.egg-info/PKG-INFO` & `pyplotterlib-1.5.0/src/pyplotterlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplotterlib
-Version: 1.4.0
+Version: 1.5.0
 Summary: A package used to create plots in python
 Author-email: Richard Fogarty <richard.m.fogarty@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 RFogarty1
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyplotterlib-1.4.0/src/pyplotterlib.egg-info/SOURCES.txt` & `pyplotterlib-1.5.0/src/pyplotterlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

