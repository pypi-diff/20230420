# Comparing `tmp/mitreattack-python-2.0.7.tar.gz` & `tmp/mitreattack-python-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitreattack-python-2.0.7.tar", last modified: Tue Apr 18 21:11:19 2023, max compression
+gzip compressed data, was "mitreattack-python-2.0.8.tar", last modified: Thu Apr 20 16:55:52 2023, max compression
```

## Comparing `mitreattack-python-2.0.7.tar` & `mitreattack-python-2.0.8.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.979008 mitreattack-python-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-18 21:11:19.979008 mitreattack-python-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.967008 mitreattack-python-2.0.7/mitreattack/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.967008 mitreattack-python-2.0.7/mitreattack/attackToExcel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/attackToExcel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/attackToExcel/attackToExcel.py
--rw-r--r--   0 runner    (1001) docker     (123)    43100 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/attackToExcel/stixToDf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.967008 mitreattack-python-2.0.7/mitreattack/collections/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/collections/collection_to_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/collections/index_to_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/collections/stix_to_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.967008 mitreattack-python-2.0.7/mitreattack/diffStix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/diffStix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    87227 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/diffStix/changelog_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/download_stix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.967008 mitreattack-python-2.0.7/mitreattack/navlayers/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.971008 mitreattack-python-2.0.7/mitreattack/navlayers/core/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/layerobj.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/legenditem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/objlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/technique.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.971008 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/excel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.975008 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   358460 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/fonts/monospace.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/fonts/sans-serif.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    85240 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/fonts/serif.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    17843 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/matrix_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/svg_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    19848 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/svg_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/to_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18266 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/to_svg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.975008 mitreattack-python-2.0.7/mitreattack/navlayers/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/generators/gen_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/generators/overview_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/generators/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/generators/usage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/layerExporter_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/layerGenerator_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.975008 mitreattack-python-2.0.7/mitreattack/navlayers/manipulators/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/manipulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/manipulators/layerops.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/release_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.975008 mitreattack-python-2.0.7/mitreattack/stix20/
--rw-r--r--   0 runner    (1001) docker     (123)    61287 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/stix20/MitreAttackData.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/stix20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/stix20/custom_attack_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.975008 mitreattack-python-2.0.7/mitreattack_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-18 21:11:19.000000 mitreattack-python-2.0.7/mitreattack_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-18 21:11:19.000000 mitreattack-python-2.0.7/mitreattack_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:11:19.000000 mitreattack-python-2.0.7/mitreattack_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-18 21:11:19.000000 mitreattack-python-2.0.7/mitreattack_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-18 21:11:19.000000 mitreattack-python-2.0.7/mitreattack_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 21:11:19.000000 mitreattack-python-2.0.7/mitreattack_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:11:19.979008 mitreattack-python-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.979008 mitreattack-python-2.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/tests/test_mass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/tests/test_to_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.664911 mitreattack-python-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-20 16:55:52.664911 mitreattack-python-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.652911 mitreattack-python-2.0.8/mitreattack/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.652911 mitreattack-python-2.0.8/mitreattack/attackToExcel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/attackToExcel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/attackToExcel/attackToExcel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43100 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/attackToExcel/stixToDf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.652911 mitreattack-python-2.0.8/mitreattack/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/collections/collection_to_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/collections/index_to_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/collections/stix_to_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.652911 mitreattack-python-2.0.8/mitreattack/diffStix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/diffStix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88547 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/diffStix/changelog_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/download_stix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.652911 mitreattack-python-2.0.8/mitreattack/navlayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.656911 mitreattack-python-2.0.8/mitreattack/navlayers/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/layerobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/legenditem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/objlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/technique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/core/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.656911 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/excel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.656911 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   358460 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/fonts/monospace.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/fonts/sans-serif.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    85240 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/fonts/serif.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    17843 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/matrix_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/svg_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19848 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/svg_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/to_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18266 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/exporters/to_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.656911 mitreattack-python-2.0.8/mitreattack/navlayers/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/generators/gen_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/generators/overview_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/generators/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/generators/usage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/layerExporter_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/layerGenerator_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.656911 mitreattack-python-2.0.8/mitreattack/navlayers/manipulators/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/manipulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/navlayers/manipulators/layerops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/release_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.656911 mitreattack-python-2.0.8/mitreattack/stix20/
+-rw-r--r--   0 runner    (1001) docker     (123)    61287 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/stix20/MitreAttackData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/stix20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/mitreattack/stix20/custom_attack_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.656911 mitreattack-python-2.0.8/mitreattack_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-20 16:55:52.000000 mitreattack-python-2.0.8/mitreattack_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-20 16:55:52.000000 mitreattack-python-2.0.8/mitreattack_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:55:52.000000 mitreattack-python-2.0.8/mitreattack_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-20 16:55:52.000000 mitreattack-python-2.0.8/mitreattack_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 16:55:52.000000 mitreattack-python-2.0.8/mitreattack_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-20 16:55:52.000000 mitreattack-python-2.0.8/mitreattack_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:55:52.664911 mitreattack-python-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:55:52.664911 mitreattack-python-2.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/tests/test_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-20 16:38:53.000000 mitreattack-python-2.0.8/tests/test_to_excel.py
```

### Comparing `mitreattack-python-2.0.7/LICENSE.txt` & `mitreattack-python-2.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/NOTICE.txt` & `mitreattack-python-2.0.8/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/PKG-INFO` & `mitreattack-python-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitreattack-python
-Version: 2.0.7
+Version: 2.0.8
 Summary: MITRE ATT&CK python library
 Home-page: https://github.com/mitre-attack/mitreattack-python/
 Author: MITRE ATT&CK, MITRE Corporation
 Author-email: attack@mitre.org
 Maintainer: Jared Ondricek
 Maintainer-email: jondricek@mitre.org
 License: Apache 2.0
```

### Comparing `mitreattack-python-2.0.7/README.md` & `mitreattack-python-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/attackToExcel/attackToExcel.py` & `mitreattack-python-2.0.8/mitreattack/attackToExcel/attackToExcel.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/attackToExcel/stixToDf.py` & `mitreattack-python-2.0.8/mitreattack/attackToExcel/stixToDf.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/collections/collection_to_index.py` & `mitreattack-python-2.0.8/mitreattack/collections/collection_to_index.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/collections/index_to_markdown.py` & `mitreattack-python-2.0.8/mitreattack/collections/index_to_markdown.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/collections/stix_to_collection.py` & `mitreattack-python-2.0.8/mitreattack/collections/stix_to_collection.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/diffStix/changelog_helper.py` & `mitreattack-python-2.0.8/mitreattack/diffStix/changelog_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """A helper script to generate changelogs between different versions of ATT&CK."""
 
 import argparse
 import datetime
 import difflib
 import json
-import math
 import os
 import re
 import sys
 import textwrap
+from dataclasses import dataclass
 from pathlib import Path
 from typing import Dict, List, Optional
 
 import markdown
 import requests
 import stix2
 from dateutil import parser as dateparser
@@ -31,14 +31,38 @@
     os.path.join("output", f"{this_month}_Updates_Enterprise.json"),
     os.path.join("output", f"{this_month}_Updates_Mobile.json"),
     os.path.join("output", f"{this_month}_Updates_ICS.json"),
     os.path.join("output", f"{this_month}_Updates_Pre.json"),
 ]
 
 
+@dataclass
+class AttackObjectVersion:
+    """An ATT&CK object version."""
+
+    major: int
+    minor: int
+
+    def __repr__(self):
+        return f"{self.major}.{self.minor}"
+
+
+# TODO: Implement a custom decoder as well. Possible solution at this link
+# https://alexisgomes19.medium.com/custom-json-encoder-with-python-f52c91b48cd2
+class AttackChangesEncoder(json.JSONEncoder):
+    """Custom JSON encoder for changes made to ATT&CK between releases."""
+
+    def default(self, obj):
+        """Handle custom object types so they can be serialized to JSON."""
+        if isinstance(obj, AttackObjectVersion):
+            return str(obj)
+
+        return json.JSONEncoder.default(self, obj)
+
+
 class DiffStix(object):
     """Utilities for detecting and summarizing differences between two versions of the ATT&CK content."""
 
     def __init__(
         self,
         domains: List[str] = ["enterprise-attack", "mobile-attack", "ics-attack"],
         layers: List[str] = None,
@@ -295,15 +319,15 @@
                     new_stix_obj = new_attack_objects[stix_id]
                     attack_id = get_attack_id(new_stix_obj)
 
                     # Add contributions from additions
                     self.update_contributors(old_object=None, new_object=new_stix_obj)
 
                     # verify version is 1.0
-                    x_mitre_version = new_stix_obj.get("x_mitre_version")
+                    x_mitre_version = get_attack_object_version(stix_obj=new_stix_obj)
                     if not version_increment_is_valid(None, x_mitre_version, "additions"):
                         logger.warning(
                             f"{stix_id} - Unexpected new version. Expected 1.0, but is {x_mitre_version}. [{attack_id}] {new_stix_obj['name']}"
                         )
 
                 #################
                 # Deleted objects
@@ -1107,28 +1131,28 @@
     color = gray
 
     object_version = get_attack_object_version(stix_obj=stix_object)
     version_display = f"(v{object_version})"
 
     if section in ["additions", "deprecations", "revocations"]:
         # only display current version
-        if not version_increment_is_valid(old_version=None, new_version=str(object_version), section=section):
+        if not version_increment_is_valid(old_version=None, new_version=object_version, section=section):
             color = red
 
     elif section == "deletions":
         color = red
 
     # nothing needs to be added to this statement - it just needs to skip the 'else' clause
     elif section == "patches":
         pass
 
     else:
         # the "previous_version" key was added in the load_data() function
         old_version = stix_object.get("previous_version")
-        if not version_increment_is_valid(old_version=old_version, new_version=str(object_version), section=section):
+        if not version_increment_is_valid(old_version=old_version, new_version=object_version, section=section):
             color = red
         version_display = f"(v{old_version}&#8594;v{object_version})"
 
     return f'<small style="color:{color}">{version_display}</small>'
 
 
 def cleanup_values(groupings: List[dict]) -> List[dict]:
@@ -1151,87 +1175,87 @@
 
         for child in sorted(grouping["children"], key=lambda child: child["name"]):
             new_values.append(child)
 
     return new_values
 
 
-def version_increment_is_valid(old_version: str, new_version: str, section: str) -> bool:
+def version_increment_is_valid(old_version: AttackObjectVersion, new_version: AttackObjectVersion, section: str) -> bool:
     """Validate version increment between old and new STIX objects.
 
     Valid increments include the following:
 
         * Major version increases: e.g. 1.2 → 2.0
         * Minor version increases: e.g. 1.2 → 1.3
         * New version for new objects must be 1.0
         * Any value when section is "revocations" or "deprecations"
 
     Parameters
     ----------
-    old_version : str
+    old_version : AttackObjectVersion
         Old version of an ATT&CK STIX Domain Object (SDO).
-    new_version : str
+    new_version : AttackObjectVersion
         New version of an ATT&CK STIX Domain Object (SDO).
     section : str
         Section change type, e.g major_version_change, revocations, etc.
 
     Returns
     -------
     bool
         Returns True when a valid version increment is found
     """
     if section in ["revocations", "deprecations"]:
         return True
     if section == "additions":
-        if new_version != "1.0":
+        if new_version != AttackObjectVersion(major=1, minor=0):
             return False
         return True
     if not (old_version and new_version):
         return False
 
-    old_version = float(old_version)
-    new_version = float(new_version)
     major_change = is_major_version_change(old_version=old_version, new_version=new_version)
     minor_change = is_minor_version_change(old_version=old_version, new_version=new_version)
 
     if major_change or minor_change:
         return True
     return False
 
 
-def is_major_version_change(old_version: float, new_version: float) -> bool:
+def is_major_version_change(old_version: AttackObjectVersion, new_version: AttackObjectVersion) -> bool:
     """Determine if the new version is a major change."""
-    next_major = float(math.floor(old_version + 1))
-    if next_major == new_version:
+    next_major_num = old_version.major + 1
+    next_major_version = AttackObjectVersion(major=next_major_num, minor=0)
+    if new_version == next_major_version:
         return True
     return False
 
 
-def is_minor_version_change(old_version: float, new_version: float) -> bool:
+def is_minor_version_change(old_version: AttackObjectVersion, new_version: AttackObjectVersion) -> bool:
     """Determine if the new version is a minor change."""
-    diff = round(new_version - old_version, 1)
-    if diff == 0.1:
+    next_minor_num = old_version.minor + 1
+    next_minor_version = AttackObjectVersion(major=old_version.major, minor=next_minor_num)
+    if new_version == next_minor_version:
         return True
     return False
 
 
-def is_other_version_change(old_version: float, new_version: float) -> bool:
+def is_other_version_change(old_version: AttackObjectVersion, new_version: AttackObjectVersion) -> bool:
     """Determine if the new version is an unexpected change."""
-    next_major = float(math.floor(old_version + 1))
-    diff = round(new_version - old_version, 1)
-
-    # went up by more than 0.1, but not next major version
-    if (diff > 0.1) and (new_version != next_major):
-        return True
-    # version number went down
-    elif diff < 0:
-        return True
-
     # either stayed the same or was a normal version change
-    return False
+    if is_major_version_change(old_version=old_version, new_version=new_version):
+        return False
+    elif is_minor_version_change(old_version=old_version, new_version=new_version):
+        return False
+    elif ((old_version.major == new_version.major) and (old_version.minor == new_version.minor)):
+        return False
+
+    # Possible scenarios
+    # * went up by more than 0.1, but not next major version
+    # * version number went down
+    return True
 
 
 def is_patch_change(old_stix_obj: dict, new_stix_obj: dict) -> bool:
     """Determine if ATT&CK Object changes are considered a patch change.
 
     Parameters
     ----------
@@ -1363,30 +1387,34 @@
             "mitre-mobile-attack",
             "mitre-ics-attack",
         ]:
             attack_id = attack_source["external_id"]
     return attack_id
 
 
-def get_attack_object_version(stix_obj: dict) -> Optional[float]:
+def get_attack_object_version(stix_obj: dict) -> AttackObjectVersion:
     """Get the object's ATT&CK version.
 
     Parameters
     ----------
     stix_obj : dict
         An ATT&CK STIX Domain Object (SDO).
 
     Returns
     -------
-    Optional[float]
-        The object version of the ATT&CK object. Defaults to 0.0
+    AttackObjectVersion
+        The object version of the ATT&CK object.
     """
     # ICS objects didn't have x_mitre_version until v11.0, so pretend they were version 0.0
-    version = stix_obj.get("x_mitre_version", 0)
-    return float(version)
+    version = stix_obj.get("x_mitre_version", "0.0")
+    major, minor = version.split(".")
+    major = int(major)
+    minor = int(minor)
+    object_version = AttackObjectVersion(major=major, minor=minor)
+    return object_version
 
 
 def markdown_to_html(outfile: str, content: str, diffStix: DiffStix):
     """Convert the markdown string passed in to HTML and store in index.html of indicated output file path.
 
     Parameters
     ----------
@@ -1964,15 +1992,15 @@
         layers_dict_to_files(outfiles=layers, layers=layers_dict)
 
     if json_file:
         changes_dict = diffStix.get_changes_dict()
 
         logger.info("Writing JSON updates to file")
         Path(json_file).parent.mkdir(parents=True, exist_ok=True)
-        json.dump(changes_dict, open(json_file, "w"), indent=4)
+        json.dump(changes_dict, open(json_file, "w"), cls=AttackChangesEncoder, indent=4)
 
     return md_string
 
 
 def main():
     """Entrypoint for running this file as a script or as a Python console command."""
     args = get_parsed_args()
```

### Comparing `mitreattack-python-2.0.7/mitreattack/download_stix.py` & `mitreattack-python-2.0.8/mitreattack/download_stix.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/core/exceptions.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/core/filter.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/core/filter.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/core/gradient.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/core/gradient.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/core/helpers.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/core/helpers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/core/layer.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/core/layer.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/core/layerobj.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/core/layerobj.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/core/layout.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/core/layout.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/core/legenditem.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/core/legenditem.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/core/metadata.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/core/metadata.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/core/objlink.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/core/objlink.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/core/technique.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/core/technique.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/core/versions.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/core/versions.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/excel_templates.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/excel_templates.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/fonts/monospace.ttf` & `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/fonts/monospace.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/fonts/sans-serif.ttf` & `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/fonts/sans-serif.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/fonts/serif.ttf` & `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/fonts/serif.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/matrix_gen.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/matrix_gen.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/svg_objects.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/svg_objects.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/svg_templates.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/svg_templates.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/to_excel.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/to_excel.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/to_svg.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/exporters/to_svg.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/generators/gen_helpers.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/generators/gen_helpers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/generators/overview_generator.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/generators/overview_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/generators/sum_generator.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/generators/sum_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/generators/usage_generator.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/generators/usage_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/layerExporter_cli.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/layerExporter_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/layerGenerator_cli.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/layerGenerator_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/navlayers/manipulators/layerops.py` & `mitreattack-python-2.0.8/mitreattack/navlayers/manipulators/layerops.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/release_info.py` & `mitreattack-python-2.0.8/mitreattack/release_info.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/stix20/MitreAttackData.py` & `mitreattack-python-2.0.8/mitreattack/stix20/MitreAttackData.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack/stix20/custom_attack_objects.py` & `mitreattack-python-2.0.8/mitreattack/stix20/custom_attack_objects.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack_python.egg-info/PKG-INFO` & `mitreattack-python-2.0.8/mitreattack_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitreattack-python
-Version: 2.0.7
+Version: 2.0.8
 Summary: MITRE ATT&CK python library
 Home-page: https://github.com/mitre-attack/mitreattack-python/
 Author: MITRE ATT&CK, MITRE Corporation
 Author-email: attack@mitre.org
 Maintainer: Jared Ondricek
 Maintainer-email: jondricek@mitre.org
 License: Apache 2.0
```

### Comparing `mitreattack-python-2.0.7/mitreattack_python.egg-info/SOURCES.txt` & `mitreattack-python-2.0.8/mitreattack_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/mitreattack_python.egg-info/entry_points.txt` & `mitreattack-python-2.0.8/mitreattack_python.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/setup.py` & `mitreattack-python-2.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mitreattack-python",
-    version="2.0.7",
+    version="2.0.8",
     author="MITRE ATT&CK, MITRE Corporation",
     author_email="attack@mitre.org",
     description="MITRE ATT&CK python library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     maintainer="Jared Ondricek",
     maintainer_email="jondricek@mitre.org",
```

### Comparing `mitreattack-python-2.0.7/tests/test_cli.py` & `mitreattack-python-2.0.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/tests/test_collections.py` & `mitreattack-python-2.0.8/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/tests/test_layers.py` & `mitreattack-python-2.0.8/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/tests/test_mass.py` & `mitreattack-python-2.0.8/tests/test_mass.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.7/tests/test_to_excel.py` & `mitreattack-python-2.0.8/tests/test_to_excel.py`

 * *Files identical despite different names*

