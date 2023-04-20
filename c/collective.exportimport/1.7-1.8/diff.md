# Comparing `tmp/collective.exportimport-1.7.tar.gz` & `tmp/collective.exportimport-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.exportimport-1.7.tar", last modified: Fri Jan 20 15:52:44 2023, max compression
+gzip compressed data, was "collective.exportimport-1.8.tar", last modified: Thu Apr 20 14:48:16 2023, max compression
```

## Comparing `collective.exportimport-1.7.tar` & `collective.exportimport-1.8.tar`

### file list

```diff
@@ -1,76 +1,79 @@
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.807968 collective.exportimport-1.7/
--rw-r--r--   0 pbauer     (501) staff       (20)     8390 2023-01-20 15:52:44.000000 collective.exportimport-1.7/CHANGES.rst
--rw-r--r--   0 pbauer     (501) staff       (20)      152 2023-01-20 15:52:44.000000 collective.exportimport-1.7/CONTRIBUTORS.rst
--rw-r--r--   0 pbauer     (501) staff       (20)      552 2023-01-20 15:52:44.000000 collective.exportimport-1.7/DEVELOP.rst
--rw-r--r--   0 pbauer     (501) staff       (20)    18092 2023-01-20 15:52:44.000000 collective.exportimport-1.7/LICENSE.GPL
--rw-r--r--   0 pbauer     (501) staff       (20)      666 2023-01-20 15:52:44.000000 collective.exportimport-1.7/LICENSE.rst
--rw-r--r--   0 pbauer     (501) staff       (20)      110 2023-01-20 15:52:44.000000 collective.exportimport-1.7/MANIFEST.in
--rw-r--r--   0 pbauer     (501) staff       (20)    82625 2023-01-20 15:52:44.808117 collective.exportimport-1.7/PKG-INFO
--rw-r--r--   0 pbauer     (501) staff       (20)    72380 2023-01-20 15:52:44.000000 collective.exportimport-1.7/README.rst
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.802243 collective.exportimport-1.7/docs/
--rw-r--r--   0 pbauer     (501) staff       (20)     7993 2023-01-20 15:52:44.000000 collective.exportimport-1.7/docs/conf.py
--rw-r--r--   0 pbauer     (501) staff       (20)   147262 2023-01-20 15:52:44.000000 collective.exportimport-1.7/docs/export.png
--rw-r--r--   0 pbauer     (501) staff       (20)   110637 2023-01-20 15:52:44.000000 collective.exportimport-1.7/docs/import.png
--rw-r--r--   0 pbauer     (501) staff       (20)       92 2023-01-20 15:52:44.000000 collective.exportimport-1.7/docs/index.rst
--rw-r--r--   0 pbauer     (501) staff       (20)     5663 2023-01-20 15:52:44.000000 collective.exportimport-1.7/docs/starzel.png
--rw-r--r--   0 pbauer     (501) staff       (20)      164 2023-01-20 15:52:44.000000 collective.exportimport-1.7/requirements.txt
--rw-r--r--   0 pbauer     (501) staff       (20)      547 2023-01-20 15:52:44.808560 collective.exportimport-1.7/setup.cfg
--rw-r--r--   0 pbauer     (501) staff       (20)     3297 2023-01-20 15:52:44.000000 collective.exportimport-1.7/setup.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.799682 collective.exportimport-1.7/src/
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.802370 collective.exportimport-1.7/src/collective/
--rw-r--r--   0 pbauer     (501) staff       (20)       80 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/__init__.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.805043 collective.exportimport-1.7/src/collective/exportimport/
--rw-r--r--   0 pbauer     (501) staff       (20)      140 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/__init__.py
--rw-r--r--   0 pbauer     (501) staff       (20)      666 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/config.py
--rw-r--r--   0 pbauer     (501) staff       (20)     7665 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/configure.zcml
--rw-r--r--   0 pbauer     (501) staff       (20)     1353 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/deserializer.py
--rw-r--r--   0 pbauer     (501) staff       (20)    20078 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/export_content.py
--rw-r--r--   0 pbauer     (501) staff       (20)    27711 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/export_other.py
--rw-r--r--   0 pbauer     (501) staff       (20)    18282 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/fix_html.py
--rw-r--r--   0 pbauer     (501) staff       (20)    38274 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/import_content.py
--rw-r--r--   0 pbauer     (501) staff       (20)    30511 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/import_other.py
--rw-r--r--   0 pbauer     (501) staff       (20)      653 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/interfaces.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.805531 collective.exportimport-1.7/src/collective/exportimport/locales/
--rw-r--r--   0 pbauer     (501) staff       (20)      611 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/locales/README.rst
--rw-r--r--   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/locales/__init__.py
--rw-r--r--   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/locales/collective.exportimport.pot
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.799930 collective.exportimport-1.7/src/collective/exportimport/locales/en/
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.805636 collective.exportimport-1.7/src/collective/exportimport/locales/en/LC_MESSAGES/
--rw-r--r--   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/locales/en/LC_MESSAGES/collective.exportimport.po
--rw-r--r--   0 pbauer     (501) staff       (20)     1762 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/locales/update.py
--rwxr-xr-x   0 pbauer     (501) staff       (20)      506 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/locales/update.sh
--rw-r--r--   0 pbauer     (501) staff       (20)      260 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/permissions.zcml
--rw-r--r--   0 pbauer     (501) staff       (20)    19088 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/serializer.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.806996 collective.exportimport-1.7/src/collective/exportimport/templates/
--rw-r--r--   0 pbauer     (501) staff       (20)     7557 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/templates/export_content.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     2112 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/templates/export_other.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     4523 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/templates/import_content.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     1919 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/templates/import_defaultpages.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     3366 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/templates/import_discussion.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     2065 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/templates/import_localroles.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     3935 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/templates/import_members.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     1701 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/templates/import_ordering.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     3176 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/templates/import_portlets.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     1717 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/templates/import_redirects.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     1928 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/templates/import_relations.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     1760 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/templates/import_translations.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     3376 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/templates/links.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     1273 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/testing.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.807855 collective.exportimport-1.7/src/collective/exportimport/tests/
--rw-r--r--   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/tests/__init__.py
--rw-r--r--   0 pbauer     (501) staff       (20)     8561 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/tests/file.pdf
--rw-r--r--   0 pbauer     (501) staff       (20)     3397 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/tests/test_drop_and_include.py
--rw-r--r--   0 pbauer     (501) staff       (20)    29510 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/tests/test_export.py
--rw-r--r--   0 pbauer     (501) staff       (20)    11871 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/tests/test_fix_html.py
--rw-r--r--   0 pbauer     (501) staff       (20)    55414 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/tests/test_import.py
--rw-r--r--   0 pbauer     (501) staff       (20)      902 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective/exportimport/tests/test_setup.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-01-20 15:52:44.803470 collective.exportimport-1.7/src/collective.exportimport.egg-info/
--rw-r--r--   0 pbauer     (501) staff       (20)    82625 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective.exportimport.egg-info/PKG-INFO
--rw-r--r--   0 pbauer     (501) staff       (20)     2619 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective.exportimport.egg-info/SOURCES.txt
--rw-r--r--   0 pbauer     (501) staff       (20)        1 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective.exportimport.egg-info/dependency_links.txt
--rw-r--r--   0 pbauer     (501) staff       (20)      128 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective.exportimport.egg-info/entry_points.txt
--rw-r--r--   0 pbauer     (501) staff       (20)       11 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective.exportimport.egg-info/namespace_packages.txt
--rw-r--r--   0 pbauer     (501) staff       (20)        1 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective.exportimport.egg-info/not-zip-safe
--rw-r--r--   0 pbauer     (501) staff       (20)      156 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective.exportimport.egg-info/requires.txt
--rw-r--r--   0 pbauer     (501) staff       (20)       11 2023-01-20 15:52:44.000000 collective.exportimport-1.7/src/collective.exportimport.egg-info/top_level.txt
--rw-r--r--   0 pbauer     (501) staff       (20)      987 2023-01-20 15:52:44.000000 collective.exportimport-1.7/tox.ini
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.434996 collective.exportimport-1.8/
+-rw-r--r--   0 pbauer     (501) staff       (20)     9514 2023-04-20 14:48:16.000000 collective.exportimport-1.8/CHANGES.rst
+-rw-r--r--   0 pbauer     (501) staff       (20)      210 2023-04-20 14:48:16.000000 collective.exportimport-1.8/CONTRIBUTORS.rst
+-rw-r--r--   0 pbauer     (501) staff       (20)      552 2023-04-20 14:48:16.000000 collective.exportimport-1.8/DEVELOP.rst
+-rw-r--r--   0 pbauer     (501) staff       (20)    18092 2023-04-20 14:48:16.000000 collective.exportimport-1.8/LICENSE.GPL
+-rw-r--r--   0 pbauer     (501) staff       (20)      666 2023-04-20 14:48:16.000000 collective.exportimport-1.8/LICENSE.rst
+-rw-r--r--   0 pbauer     (501) staff       (20)      110 2023-04-20 14:48:16.000000 collective.exportimport-1.8/MANIFEST.in
+-rw-r--r--   0 pbauer     (501) staff       (20)    93315 2023-04-20 14:48:16.435107 collective.exportimport-1.8/PKG-INFO
+-rw-r--r--   0 pbauer     (501) staff       (20)    81888 2023-04-20 14:48:16.000000 collective.exportimport-1.8/README.rst
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.428356 collective.exportimport-1.8/docs/
+-rw-r--r--   0 pbauer     (501) staff       (20)     7993 2023-04-20 14:48:16.000000 collective.exportimport-1.8/docs/conf.py
+-rw-r--r--   0 pbauer     (501) staff       (20)   147262 2023-04-20 14:48:16.000000 collective.exportimport-1.8/docs/export.png
+-rw-r--r--   0 pbauer     (501) staff       (20)   110637 2023-04-20 14:48:16.000000 collective.exportimport-1.8/docs/import.png
+-rw-r--r--   0 pbauer     (501) staff       (20)       92 2023-04-20 14:48:16.000000 collective.exportimport-1.8/docs/index.rst
+-rw-r--r--   0 pbauer     (501) staff       (20)     5663 2023-04-20 14:48:16.000000 collective.exportimport-1.8/docs/starzel.png
+-rw-r--r--   0 pbauer     (501) staff       (20)      222 2023-04-20 14:48:16.000000 collective.exportimport-1.8/requirements.txt
+-rw-r--r--   0 pbauer     (501) staff       (20)      547 2023-04-20 14:48:16.435459 collective.exportimport-1.8/setup.cfg
+-rw-r--r--   0 pbauer     (501) staff       (20)     3297 2023-04-20 14:48:16.000000 collective.exportimport-1.8/setup.py
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.426006 collective.exportimport-1.8/src/
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.428462 collective.exportimport-1.8/src/collective/
+-rw-r--r--   0 pbauer     (501) staff       (20)       80 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/__init__.py
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.431513 collective.exportimport-1.8/src/collective/exportimport/
+-rw-r--r--   0 pbauer     (501) staff       (20)      140 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/__init__.py
+-rw-r--r--   0 pbauer     (501) staff       (20)      666 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/config.py
+-rw-r--r--   0 pbauer     (501) staff       (20)     7665 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/configure.zcml
+-rw-r--r--   0 pbauer     (501) staff       (20)     1353 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/deserializer.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    20141 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/export_content.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    28015 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/export_other.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    19308 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/fix_html.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    39323 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/import_content.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    30663 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/import_other.py
+-rw-r--r--   0 pbauer     (501) staff       (20)      653 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/interfaces.py
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.432092 collective.exportimport-1.8/src/collective/exportimport/locales/
+-rw-r--r--   0 pbauer     (501) staff       (20)      639 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/locales/README.rst
+-rw-r--r--   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/locales/__init__.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    12849 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/locales/collective.exportimport.pot
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.426236 collective.exportimport-1.8/src/collective/exportimport/locales/en/
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.432252 collective.exportimport-1.8/src/collective/exportimport/locales/en/LC_MESSAGES/
+-rw-r--r--   0 pbauer     (501) staff       (20)    12723 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/locales/en/LC_MESSAGES/collective.exportimport.po
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.426337 collective.exportimport-1.8/src/collective/exportimport/locales/es/
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.432395 collective.exportimport-1.8/src/collective/exportimport/locales/es/LC_MESSAGES/
+-rw-r--r--   0 pbauer     (501) staff       (20)    17399 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/locales/es/LC_MESSAGES/collective.exportimport.po
+-rw-r--r--   0 pbauer     (501) staff       (20)     1762 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/locales/update.py
+-rwxr-xr-x   0 pbauer     (501) staff       (20)      506 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/locales/update.sh
+-rw-r--r--   0 pbauer     (501) staff       (20)      260 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/permissions.zcml
+-rw-r--r--   0 pbauer     (501) staff       (20)    23410 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/serializer.py
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.434028 collective.exportimport-1.8/src/collective/exportimport/templates/
+-rw-r--r--   0 pbauer     (501) staff       (20)     7850 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/export_content.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     2163 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/export_other.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     4745 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_content.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     2043 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_defaultpages.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     3490 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_discussion.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     2189 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_localroles.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     4059 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_members.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     1825 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_ordering.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     3300 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_portlets.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     1877 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_redirects.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     2052 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_relations.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     1884 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_translations.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     4035 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/links.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     1273 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/testing.py
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.434898 collective.exportimport-1.8/src/collective/exportimport/tests/
+-rw-r--r--   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/tests/__init__.py
+-rw-r--r--   0 pbauer     (501) staff       (20)     8561 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/tests/file.pdf
+-rw-r--r--   0 pbauer     (501) staff       (20)     3397 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/tests/test_drop_and_include.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    29510 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/tests/test_export.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    11863 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/tests/test_fix_html.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    55401 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/tests/test_import.py
+-rw-r--r--   0 pbauer     (501) staff       (20)      902 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/tests/test_setup.py
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.429450 collective.exportimport-1.8/src/collective.exportimport.egg-info/
+-rw-r--r--   0 pbauer     (501) staff       (20)    93315 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/PKG-INFO
+-rw-r--r--   0 pbauer     (501) staff       (20)     2697 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/SOURCES.txt
+-rw-r--r--   0 pbauer     (501) staff       (20)        1 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/dependency_links.txt
+-rw-r--r--   0 pbauer     (501) staff       (20)      128 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/entry_points.txt
+-rw-r--r--   0 pbauer     (501) staff       (20)       11 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/namespace_packages.txt
+-rw-r--r--   0 pbauer     (501) staff       (20)        1 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/not-zip-safe
+-rw-r--r--   0 pbauer     (501) staff       (20)      156 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/requires.txt
+-rw-r--r--   0 pbauer     (501) staff       (20)       11 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/top_level.txt
+-rw-r--r--   0 pbauer     (501) staff       (20)      987 2023-04-20 14:48:16.000000 collective.exportimport-1.8/tox.ini
```

### Comparing `collective.exportimport-1.7/CHANGES.rst` & `collective.exportimport-1.8/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,56 @@
 Changelog
 =========
 
 
+1.8 (2023-04-20)
+----------------
+
+- Import: run set_uuid method before we call custom hooks, so the hooks have access to
+  the item UUID. Fix #185.
+  [fredvd]
+
+- Add Spanish translation.
+  [macagua]
+
+- Add i18n support.
+  [macagua]
+
+- Fix html: improve mapping from scale to picture variant.  [maurits]
+
+- Allow overriding the fallback variant in img_variant_fixer.
+  Use 'medium' by default.
+  [maurits]
+
+- Let fix_html view work on the current context.  [maurits]
+
+- Fix the way we get a blob path. (#180)
+  [ale-rt]
+
+- Create documents as containers for items without parent when documents are folderish.
+  [JeffersonBledsoe]
+
+- Add support for passing any iterator as data-source to the import.
+  [pbauer]
+
+- Add example for importing collective.jsonify data to documentation.
+  [pbauer]
+
+- Better serialization of Topics:
+  - Use newer criteria added in Plone 5
+  - Add fallback for some criteria
+  - Export sort_on and sort_reversed
+  - Export customView as tabular_view
+  [pbauer]
+  
+- Always import discussions independent if discussion support is enabled or not
+  on a particular content object (#182)
+  [ajung]
+
+
 1.7 (2023-01-20)
 ----------------
 
 - Filter out 'Discussion Item' in content type export list. Comments have their own export and
   import views. A normal content type export for comments will raise a KeyError when trying to find
   the parent. (#112)
   [fredvd]
```

### Comparing `collective.exportimport-1.7/DEVELOP.rst` & `collective.exportimport-1.8/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/LICENSE.GPL` & `collective.exportimport-1.8/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/LICENSE.rst` & `collective.exportimport-1.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/PKG-INFO` & `collective.exportimport-1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.exportimport
-Version: 1.7
+Version: 1.8
 Summary: An add-on for Plone to Export and import content, members, relations, translations and localroles.
 Home-page: https://github.com/collective/collective.exportimport
 Author: Philip Bauer (for starzel.de)
 Author-email: info@starzel.de
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.exportimport
 Project-URL: Source, https://github.com/collective/collective.exportimport
@@ -60,15 +60,15 @@
 
 Export and import content, members, relations, translations, localroles and much more.
 
 Export and import all kinds of data from and to Plone sites using a intermediate json-format.
 The main use-case is migrations since it enables you to for example migrate from Plone 4 with Archetypes and Python 2 to Plone 6 with Dexterity and Python 3 in one step.
 Most features use `plone.restapi` to serialize and deserialize data.
 
-See also the training on migrating with exportimport: https://training.plone.org/migrations/exportimport.html
+See also the training on migrating with ``exportimport``: https://training.plone.org/migrations/exportimport.html
 
 .. contents:: Contents
     :local:
 
 Features
 ========
 
@@ -129,26 +129,26 @@
 Migrations
 ----------
 
 When a in-place-migration is not required you can choose this addon to migrate the most important parts of your site to json and then import it into a new Plone instance of your targeted version:
 
 * Export content from a Plone site (it supports Plone 4 and 5, Archetypes and Dexterity, Python 2 and 3).
 * Import the exported content into a new site (Plone 5.2+, Dexterity, Python 3)
-* Export and import relations, users and groups with their roles, translations, local roles, ordering, dedault-pages, comments, portlets and redirects.
+* Export and import relations, users and groups with their roles, translations, local roles, ordering, default-pages, comments, portlets and redirects.
 
 How to migrate additional features like Annotations or Marker Interfaces is discussed in the FAQ section.
 
 Other
 -----
 
 You can use this addon to
 
 * Archive your content as json
 * Export data to prepare a migration to another system
-* Combine content from mutiple plone-sites into one.
+* Combine content from multiple plone-sites into one.
 * Import a plone-site as a subsite into another.
 * Import content from other systems as long as it fits the required format.
 * Update or replace existing data
 * ...
 
 Details
 =======
@@ -189,16 +189,16 @@
 Exporting Archetypes content and importing that as Dexterity content works fine but due to changes in field-names some settings would get lost.
 For example the setting to exclude content from the navigation was renamed from ``excludeFromNav`` to ``exclude_from_nav``.
 
 To fix this you can check the checkbox "Modify exported data for migrations".
 This will modify the data during export:
 
 * Drop unused data (e.g. `next_item` and `components`)
-* Remove all relationfields
-* Change some fieldnames that changed between AT and DX
+* Remove all relation fields
+* Change some field names that changed between Archetypes and Dexterity
 
   * ``excludeFromNav`` → ``exclude_from_nav``
   * ``allowDiscussion`` → ``allow_discussion``
   * ``subject`` → ``subjects``
   * ``expirationDate`` → ``expires``
   * ``effectiveDate`` → ``effective``
   * ``creation_date`` → ``created``
@@ -207,16 +207,16 @@
   * ``endDate`` → ``end``
   * ``openEnd`` → ``open_end``
   * ``wholeDay`` → ``whole_day``
   * ``contactEmail`` → ``contact_email``
   * ``contactName`` → ``contact_name``
   * ``contactPhone`` → ``contact_phone``
 
-* Update view names on Folders and Collection thet changed since Plone 4.
-* Export ATTopic and their criteria to Collections with querystrings.
+* Update view names on Folders and Collection that changed since Plone 4.
+* Export ``ATTopic`` and their criteria to Collections with querystrings.
 * Update Collection-criteria.
 * Links and images in Richtext-Fields of content and portlets have changes since Plone 4.
   the view ``/@@fix_html`` allows you to fix these.
 
 
 Control creating imported content
 ---------------------------------
@@ -224,16 +224,16 @@
 You can choose between four options how to deal with content that already exists:
 
   * Skip: Don't import at all
   * Replace: Delete item and create new
   * Update: Reuse and only overwrite imported data
   * Ignore: Create with a new id
 
-Imported content is initially created with ``invokeFactory`` using portal_type and id of the exported item before deserialing the rest of the data.
-You can set additional values by specifying a dict ``factory_kwargs`` that will be passed to the facory.
+Imported content is initially created with ``invokeFactory`` using portal_type and id of the exported item before deserializing the rest of the data.
+You can set additional values by specifying a dict ``factory_kwargs`` that will be passed to the factory.
 Like this you can set values on the imported object that are expected to be there by subscribers to IObjectAddedEvent.
 
 
 Export versioned content
 ------------------------
 
 Exporting versions of Archetypes content will not work because of a bug in plone.restapi (https://github.com/plone/plone.restapi/issues/1335).
@@ -591,15 +591,15 @@
 
 .. code-block:: python
 
     def global_dict_hook(self, item):
         item["creators"] = [i for i in item.get("creators", []) if i]
         return item
 
-This example migrates a PloneHelpCenter to a simple folder/document structure during import.
+This example migrates a ``PloneHelpCenter`` to a simple folder/document structure during import.
 There are a couple more types to handle (as folder or document) but you get the idea, don't you?
 
 .. code-block:: python
 
     def dict_hook_helpcenter(self, item):
         item["@type"] = "Folder"
         item["layout"] = "listing_view"
@@ -867,15 +867,15 @@
 That can happen when options in a field are generated from content in the site.
 In these cases you cannot be sure that all options already exist in the portal while importing the content.
 
 It may also happen, when you have validators that rely on content or configuration that does not exist on import.
 
 .. note::
 
-    For relationfields this is not necessary since relations are imported after content anyway!
+    For relation fields this is not necessary since relations are imported after content anyway!
 
 There are two ways to handle these issues:
 
 * Use a simple setter bypassing the validation used by the restapi
 * Defer the import until all other imports were run
 
 
@@ -1312,15 +1312,15 @@
             results["registry"] = json_compatible(registry)
             return results
 
 
 **Import:**
 
 The import installs the addons and load the settings in the registry.
-Since Plone 5 portal_properties is no longer used.
+Since Plone 5 ``portal_properties`` is no longer used.
 
 .. code-block:: python
 
     from logging import getLogger
     from plone import api
     from plone.registry.interfaces import IRegistry
     from Products.CMFPlone.utils import get_installer
@@ -1483,15 +1483,15 @@
                     "Number of columns does not match for all rows. Some data were skipped in "
                     "data adapter %s/%s",
                     "/".join(obj.getPhysicalPath()),
                     data_adapter_name,
                 )
         return actions
 
-Import exported PloneFormGen data into Easyform:
+Import exported ``PloneFormGen`` data into ``Easyform``:
 
 .. code-block:: python
 
     def obj_hook_easyform(self, obj, item):
         if not item.get("exportimport._inputStorage"):
             return
         from collective.easyform.actions import SavedDataBTree
@@ -1897,22 +1897,288 @@
                 link.decompose()
             elif not link.get("href") and link.text:
                 # drop links without a href but keep the text
                 link.unwrap()
         return soup.decode()
 
 
+Migrate very old Plone Versions with data created by collective.jsonify
+-----------------------------------------------------------------------
+
+Versions older than Plone 4 do not support ``plone.restapi`` which is required to serialize the content used by ``collective.exportimport``.
+
+To migrate Plone 1, 2 and 3 to Plone 6 you can use ``collective.jsonify`` for the export and ``collective.exportimport`` for the import.
+
+Export
+******
+
+Use https://github.com/collective/collective.jsonify to export content.
+
+You include the methods of ``collective.jsonify`` using `External Methods`.
+See https://github.com/collective/collective.jsonify/blob/master/docs/install.rst for more info.
+
+To work better with ``collective.exportimport`` you could extend the exported data using the feature ``additional_wrappers``.
+Add info on the parent of an item to make it easier for ``collective.exportimport`` to import the data.
+
+Here is a full example for `json_methods.py` which should be in `BUILDOUT_ROOT/parts/instance/Extensions/`
+
+.. code-block:: python
+
+    def extend_item(obj, item):
+        """Extend to work better well with collective.exportimport"""
+        from Acquisition import aq_parent
+        parent = aq_parent(obj)
+        item["parent"] = {
+            "@id": parent.absolute_url(),
+            "@type": getattr(parent, "portal_type", None),
+        }
+        if getattr(parent.aq_base, "UID", None) is not None:
+            item["parent"]["UID"] = parent.UID()
+
+        return item
+
+
+Here is a full example for ``json_methods.py`` which should be in ``<BUILDOUT_ROOT>/parts/instance/Extensions/``
+
+.. code-block:: python
+
+    from collective.jsonify.export import export_content as export_content_orig
+    from collective.jsonify.export import get_item
+
+    EXPORTED_TYPES = [
+        "Folder",
+        "Document",
+        "News Item",
+        "Event",
+        "Link",
+        "Topic",
+        "File",
+        "Image",
+        "RichTopic",
+    ]
+
+    EXTRA_SKIP_PATHS = [
+        "/Plone/archiv/",
+        "/Plone/do-not-import/",
+    ]
+
+    # Path from which to continue the export.
+    # The export walks the whole site respecting the order.
+    # It will ignore everything untill this path is reached.
+    PREVIOUS = ""
+
+    def export_content(self):
+        return export_content_orig(
+            self,
+            basedir="/var/lib/zope/json",
+            skip_callback=skip_item,
+            extra_skip_classname=[],
+            extra_skip_id=[],
+            extra_skip_paths=EXTRA_SKIP_PATHS,
+            batch_start=0,
+            batch_size=10000,
+            batch_previous_path=PREVIOUS or None,
+        )
+
+    def skip_item(item):
+        """Return True if the item should be skipped"""
+        portal_type = getattr(item, "portal_type", None)
+        if portal_type not in EXPORTED_TYPES:
+            return True
+
+    def extend_item(obj, item):
+        """Extend to work better well with collective.exportimport"""
+        from Acquisition import aq_parent
+        parent = aq_parent(obj)
+        item["parent"] = {
+            "@id": parent.absolute_url(),
+            "@type": getattr(parent, "portal_type", None),
+        }
+        if getattr(parent.aq_base, "UID", None) is not None:
+            item["parent"]["UID"] = parent.UID()
+
+        return item
+
+To use these create three "External Method" in the ZMI root at the Zope root to use that:
+
+* id: "export_content", module name: "json_methods", function name: "export_content"
+* id: "get_item", module name: "json_methods", function name: "get_item"
+* id: "extend_item", module name: "json_methods", function name: "extend_item"
+
+Then you can pass the extender to the export using a query-string: http://localhost:8080/Plone/export_content?additional_wrappers=extend_item
+
+
+Import
+******
+
+Two issues need to be dealt with to allow ``collective.exportimport`` to import the data generated by ``collective.jsonify``.
+
+#. The data is in directories instead of in one large json-file.
+#. The json is not in the expected format.
+
+Starting with version 1.8 you can pass an iterator to the import.
+
+You need to create a directory-walker that sorts the json-files the right way.
+By default it would import them in the order `1.json`, `10.json`, `100.json`, `101.json` and so on.
+
+.. code-block:: python
+
+    from pathlib import Path
+
+    def filesystem_walker(path=None):
+        root = Path(path)
+        assert(root.is_dir())
+        folders = sorted([i for i in root.iterdir() if i.is_dir() and i.name.isdecimal()], key=lambda i: int(i.name))
+        for folder in folders:
+            json_files = sorted([i for i in folder.glob("*.json") if i.stem.isdecimal()], key=lambda i: int(i.stem))
+            for json_file in json_files:
+                logger.debug("Importing %s", json_file)
+                item = json.loads(json_file.read_text())
+                item["json_file"] = str(json_file)
+                item = prepare_data(item)
+                if item:
+                    yield item
+
+The walker takes the path to be the root with one or more directories holding the json-files.
+The sorting of the files is done using the number in the filename.
+
+The method ``prepare_data`` modifies the data before passing it to the import.
+A very similar task is done by ``collective.exportimport`` during export.
+
+.. code-block:: python
+
+    def prepare_data(item):
+        """modify jsonify data to work with c.exportimport"""
+
+        # Drop relationfields or defer the import
+        item.pop("relatedItems", None)
+
+        mapping = {
+            # jsonify => exportimport
+            "_uid": "UID",
+            "_type": "@type",
+            "_path": "@id",
+            "_layout": "layout",
+            # AT fieldnames => DX fieldnames
+            "excludeFromNav": "exclude_from_nav",
+            "allowDiscussion": "allow_discussion",
+            "subject": "subjects",
+            "expirationDate": "expires",
+            "effectiveDate": "effective",
+            "creation_date": "created",
+            "modification_date": "modified",
+            "startDate": "start",
+            "endDate": "end",
+            "openEnd": "open_end",
+            "eventUrl": "event_url",
+            "wholeDay": "whole_day",
+            "contactEmail": "contact_email",
+            "contactName": "contact_name",
+            "contactPhone": "contact_phone",
+            "imageCaption": "image_caption",
+        }
+        for old, new in mapping.items():
+            item = migrate_field(item, old, new)
+
+        if item.get("constrainTypesMode", None) == 1:
+            item = migrate_field(item, "constrainTypesMode", "constrain_types_mode")
+        else:
+            item.pop("locallyAllowedTypes", None)
+            item.pop("immediatelyAddableTypes", None)
+            item.pop("constrainTypesMode", None)
+
+        if "id" not in item:
+            item["id"] = item["_id"]
+        return item
+
+
+    def migrate_field(item, old, new):
+        if item.get(old, _marker) is not _marker:
+            item[new] = item.pop(old)
+        return item
+
+You can pass the generator ``filesystem_walker`` to the import:
+
+.. code-block:: python
+
+    class ImportAll(BrowserView):
+
+        def __call__(self):
+            # ...
+            cfg = getConfiguration()
+            directory = Path(cfg.clienthome) / "import"
+
+            # import content
+            view = api.content.get_view("import_content", portal, request)
+            request.form["form.submitted"] = True
+            request.form["commit"] = 1000
+            view(iterator=filesystem_walker(directory / "mydata"))
+
+            # import default-pages
+            import_deferred = api.content.get_view("import_deferred", portal, request)
+            import_deferred()
+
+
+    class ImportDeferred(BrowserView):
+
+        def __call__(self):
+            self.title = "Import Deferred Settings (default pages)"
+            if not self.request.form.get("form.submitted", False):
+                return self.index()
+
+            for brain in api.content.find(portal_type="Folder"):
+                obj = brain.getObject()
+                annotations = IAnnotations(obj)
+                if DEFERRED_KEY not in annotations:
+                    continue
+
+                default = annotations[DEFERRED_KEY].pop("_defaultpage", None)
+                if default and default in obj:
+                    logger.info("Setting %s as default page for %s", default, obj.absolute_url())
+                    obj.setDefaultPage(default)
+                if not annotations[DEFERRED_KEY]:
+                    annotations.pop(DEFERRED_KEY)
+            api.portal.show_message("Done", self.request)
+            return self.index()
+
+``collective.jsonify`` puts the info on relations, translations and default-pages in the export-file.
+You can use the approach to defer imports to deal with that data after all items were imported.
+The example ``ImportDeferred`` above uses that approach to set the default pages.
+
+This ``global_obj_hook`` below stores that data in a annotation:
+
+.. code-block:: python
+
+    def global_obj_hook(self, obj, item):
+        # Store deferred data in an annotation.
+        keys = ["_defaultpage"]
+        data = {}
+        for key in keys:
+            if value := item.get(key, None):
+                data[key] = value
+        if data:
+            annotations = IAnnotations(obj)
+            annotations[DEFERRED_KEY] = data
+
+
 Written by
 ==========
 
 .. image:: ./docs/starzel.png
     :target: https://www.starzel.de
     :alt: Starzel.de
 
 
+Translations
+============
+
+This product has been translated into
+
+- Spanish
+
 
 Installation
 ============
 
 Install collective.exportimport by adding it to your buildout::
 
     [buildout]
@@ -1921,22 +2187,22 @@
 
     eggs =
         collective.exportimport
 
 
 and then running ``bin/buildout``
 
-You don't need to activate the add-on in the Site Setup Add-ons control panel to be able to use the forms @@export_content and @@import_content in your site.
+You don't need to activate the add-on in the Site Setup Add-ons control panel to be able to use the forms ``@@export_content`` and ``@@import_content`` in your site.
 
 You do need to add it to your buildout configuration and run buildout to make these features available at all. See https://docs.plone.org/manage/installing/installing_addons.html for details.
 
 Installing in Plone 4
 ---------------------
 
-collective.exportimport depends on plone.restapi . For Plone 4, you need to pin plone.restapi to 7.x . When installing plone.restapi version 7.x.x in Plone 4 you may need to add the following version pins to your buildout::
+``collective.exportimport`` depends on ``plone.restapi``. For Plone 4, you need to pin ``plone.restapi`` to 7.x . When installing ``plone.restapi`` version 7.x.x in Plone 4 you may need to add the following version pins to your buildout::
 
     [versions]
     PyJWT = 1.7.1
 
     six = 1.11.0
     attrs = 21.2.0
     plone.rest = 1.6.2
@@ -1965,16 +2231,15 @@
 
     importlib-metadata = 2.1.3
     zipp = 1.2.0
     configparser = 4.0.2
     contextlib2 = 0.6.0.post1
 
 
-These versions are taken from the plone.restapi 7.x README: https://pypi.org/project/plone.restapi/7.8.1/
-
+These versions are taken from the ``plone.restapi`` 7.x README: https://pypi.org/project/plone.restapi/7.8.1/
 
 
 Contribute
 ==========
 
 - Issue Tracker: https://github.com/collective/collective.exportimport/issues
 - Source Code: https://github.com/collective/collective.exportimport
@@ -1997,18 +2262,66 @@
 
 - Philip Bauer, bauer@starzel.de
 
 - Maurits van Rees, m.van.rees@zestsoftware.nl
 
 - Fred van Dijk, f.van.dijk@zestsoftware.nl
 
+- Leonardo J. Caballero G., leonardocaballero@gmail.com
+
+
 Changelog
 =========
 
 
+1.8 (2023-04-20)
+----------------
+
+- Import: run set_uuid method before we call custom hooks, so the hooks have access to
+  the item UUID. Fix #185.
+  [fredvd]
+
+- Add Spanish translation.
+  [macagua]
+
+- Add i18n support.
+  [macagua]
+
+- Fix html: improve mapping from scale to picture variant.  [maurits]
+
+- Allow overriding the fallback variant in img_variant_fixer.
+  Use 'medium' by default.
+  [maurits]
+
+- Let fix_html view work on the current context.  [maurits]
+
+- Fix the way we get a blob path. (#180)
+  [ale-rt]
+
+- Create documents as containers for items without parent when documents are folderish.
+  [JeffersonBledsoe]
+
+- Add support for passing any iterator as data-source to the import.
+  [pbauer]
+
+- Add example for importing collective.jsonify data to documentation.
+  [pbauer]
+
+- Better serialization of Topics:
+  - Use newer criteria added in Plone 5
+  - Add fallback for some criteria
+  - Export sort_on and sort_reversed
+  - Export customView as tabular_view
+  [pbauer]
+  
+- Always import discussions independent if discussion support is enabled or not
+  on a particular content object (#182)
+  [ajung]
+
+
 1.7 (2023-01-20)
 ----------------
 
 - Filter out 'Discussion Item' in content type export list. Comments have their own export and
   import views. A normal content type export for comments will raise a KeyError when trying to find
   the parent. (#112)
   [fredvd]
```

### Comparing `collective.exportimport-1.7/README.rst` & `collective.exportimport-1.8/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 Export and import content, members, relations, translations, localroles and much more.
 
 Export and import all kinds of data from and to Plone sites using a intermediate json-format.
 The main use-case is migrations since it enables you to for example migrate from Plone 4 with Archetypes and Python 2 to Plone 6 with Dexterity and Python 3 in one step.
 Most features use `plone.restapi` to serialize and deserialize data.
 
-See also the training on migrating with exportimport: https://training.plone.org/migrations/exportimport.html
+See also the training on migrating with ``exportimport``: https://training.plone.org/migrations/exportimport.html
 
 .. contents:: Contents
     :local:
 
 Features
 ========
 
@@ -92,26 +92,26 @@
 Migrations
 ----------
 
 When a in-place-migration is not required you can choose this addon to migrate the most important parts of your site to json and then import it into a new Plone instance of your targeted version:
 
 * Export content from a Plone site (it supports Plone 4 and 5, Archetypes and Dexterity, Python 2 and 3).
 * Import the exported content into a new site (Plone 5.2+, Dexterity, Python 3)
-* Export and import relations, users and groups with their roles, translations, local roles, ordering, dedault-pages, comments, portlets and redirects.
+* Export and import relations, users and groups with their roles, translations, local roles, ordering, default-pages, comments, portlets and redirects.
 
 How to migrate additional features like Annotations or Marker Interfaces is discussed in the FAQ section.
 
 Other
 -----
 
 You can use this addon to
 
 * Archive your content as json
 * Export data to prepare a migration to another system
-* Combine content from mutiple plone-sites into one.
+* Combine content from multiple plone-sites into one.
 * Import a plone-site as a subsite into another.
 * Import content from other systems as long as it fits the required format.
 * Update or replace existing data
 * ...
 
 Details
 =======
@@ -152,16 +152,16 @@
 Exporting Archetypes content and importing that as Dexterity content works fine but due to changes in field-names some settings would get lost.
 For example the setting to exclude content from the navigation was renamed from ``excludeFromNav`` to ``exclude_from_nav``.
 
 To fix this you can check the checkbox "Modify exported data for migrations".
 This will modify the data during export:
 
 * Drop unused data (e.g. `next_item` and `components`)
-* Remove all relationfields
-* Change some fieldnames that changed between AT and DX
+* Remove all relation fields
+* Change some field names that changed between Archetypes and Dexterity
 
   * ``excludeFromNav`` → ``exclude_from_nav``
   * ``allowDiscussion`` → ``allow_discussion``
   * ``subject`` → ``subjects``
   * ``expirationDate`` → ``expires``
   * ``effectiveDate`` → ``effective``
   * ``creation_date`` → ``created``
@@ -170,16 +170,16 @@
   * ``endDate`` → ``end``
   * ``openEnd`` → ``open_end``
   * ``wholeDay`` → ``whole_day``
   * ``contactEmail`` → ``contact_email``
   * ``contactName`` → ``contact_name``
   * ``contactPhone`` → ``contact_phone``
 
-* Update view names on Folders and Collection thet changed since Plone 4.
-* Export ATTopic and their criteria to Collections with querystrings.
+* Update view names on Folders and Collection that changed since Plone 4.
+* Export ``ATTopic`` and their criteria to Collections with querystrings.
 * Update Collection-criteria.
 * Links and images in Richtext-Fields of content and portlets have changes since Plone 4.
   the view ``/@@fix_html`` allows you to fix these.
 
 
 Control creating imported content
 ---------------------------------
@@ -187,16 +187,16 @@
 You can choose between four options how to deal with content that already exists:
 
   * Skip: Don't import at all
   * Replace: Delete item and create new
   * Update: Reuse and only overwrite imported data
   * Ignore: Create with a new id
 
-Imported content is initially created with ``invokeFactory`` using portal_type and id of the exported item before deserialing the rest of the data.
-You can set additional values by specifying a dict ``factory_kwargs`` that will be passed to the facory.
+Imported content is initially created with ``invokeFactory`` using portal_type and id of the exported item before deserializing the rest of the data.
+You can set additional values by specifying a dict ``factory_kwargs`` that will be passed to the factory.
 Like this you can set values on the imported object that are expected to be there by subscribers to IObjectAddedEvent.
 
 
 Export versioned content
 ------------------------
 
 Exporting versions of Archetypes content will not work because of a bug in plone.restapi (https://github.com/plone/plone.restapi/issues/1335).
@@ -554,15 +554,15 @@
 
 .. code-block:: python
 
     def global_dict_hook(self, item):
         item["creators"] = [i for i in item.get("creators", []) if i]
         return item
 
-This example migrates a PloneHelpCenter to a simple folder/document structure during import.
+This example migrates a ``PloneHelpCenter`` to a simple folder/document structure during import.
 There are a couple more types to handle (as folder or document) but you get the idea, don't you?
 
 .. code-block:: python
 
     def dict_hook_helpcenter(self, item):
         item["@type"] = "Folder"
         item["layout"] = "listing_view"
@@ -830,15 +830,15 @@
 That can happen when options in a field are generated from content in the site.
 In these cases you cannot be sure that all options already exist in the portal while importing the content.
 
 It may also happen, when you have validators that rely on content or configuration that does not exist on import.
 
 .. note::
 
-    For relationfields this is not necessary since relations are imported after content anyway!
+    For relation fields this is not necessary since relations are imported after content anyway!
 
 There are two ways to handle these issues:
 
 * Use a simple setter bypassing the validation used by the restapi
 * Defer the import until all other imports were run
 
 
@@ -1275,15 +1275,15 @@
             results["registry"] = json_compatible(registry)
             return results
 
 
 **Import:**
 
 The import installs the addons and load the settings in the registry.
-Since Plone 5 portal_properties is no longer used.
+Since Plone 5 ``portal_properties`` is no longer used.
 
 .. code-block:: python
 
     from logging import getLogger
     from plone import api
     from plone.registry.interfaces import IRegistry
     from Products.CMFPlone.utils import get_installer
@@ -1446,15 +1446,15 @@
                     "Number of columns does not match for all rows. Some data were skipped in "
                     "data adapter %s/%s",
                     "/".join(obj.getPhysicalPath()),
                     data_adapter_name,
                 )
         return actions
 
-Import exported PloneFormGen data into Easyform:
+Import exported ``PloneFormGen`` data into ``Easyform``:
 
 .. code-block:: python
 
     def obj_hook_easyform(self, obj, item):
         if not item.get("exportimport._inputStorage"):
             return
         from collective.easyform.actions import SavedDataBTree
@@ -1860,22 +1860,288 @@
                 link.decompose()
             elif not link.get("href") and link.text:
                 # drop links without a href but keep the text
                 link.unwrap()
         return soup.decode()
 
 
+Migrate very old Plone Versions with data created by collective.jsonify
+-----------------------------------------------------------------------
+
+Versions older than Plone 4 do not support ``plone.restapi`` which is required to serialize the content used by ``collective.exportimport``.
+
+To migrate Plone 1, 2 and 3 to Plone 6 you can use ``collective.jsonify`` for the export and ``collective.exportimport`` for the import.
+
+Export
+******
+
+Use https://github.com/collective/collective.jsonify to export content.
+
+You include the methods of ``collective.jsonify`` using `External Methods`.
+See https://github.com/collective/collective.jsonify/blob/master/docs/install.rst for more info.
+
+To work better with ``collective.exportimport`` you could extend the exported data using the feature ``additional_wrappers``.
+Add info on the parent of an item to make it easier for ``collective.exportimport`` to import the data.
+
+Here is a full example for `json_methods.py` which should be in `BUILDOUT_ROOT/parts/instance/Extensions/`
+
+.. code-block:: python
+
+    def extend_item(obj, item):
+        """Extend to work better well with collective.exportimport"""
+        from Acquisition import aq_parent
+        parent = aq_parent(obj)
+        item["parent"] = {
+            "@id": parent.absolute_url(),
+            "@type": getattr(parent, "portal_type", None),
+        }
+        if getattr(parent.aq_base, "UID", None) is not None:
+            item["parent"]["UID"] = parent.UID()
+
+        return item
+
+
+Here is a full example for ``json_methods.py`` which should be in ``<BUILDOUT_ROOT>/parts/instance/Extensions/``
+
+.. code-block:: python
+
+    from collective.jsonify.export import export_content as export_content_orig
+    from collective.jsonify.export import get_item
+
+    EXPORTED_TYPES = [
+        "Folder",
+        "Document",
+        "News Item",
+        "Event",
+        "Link",
+        "Topic",
+        "File",
+        "Image",
+        "RichTopic",
+    ]
+
+    EXTRA_SKIP_PATHS = [
+        "/Plone/archiv/",
+        "/Plone/do-not-import/",
+    ]
+
+    # Path from which to continue the export.
+    # The export walks the whole site respecting the order.
+    # It will ignore everything untill this path is reached.
+    PREVIOUS = ""
+
+    def export_content(self):
+        return export_content_orig(
+            self,
+            basedir="/var/lib/zope/json",
+            skip_callback=skip_item,
+            extra_skip_classname=[],
+            extra_skip_id=[],
+            extra_skip_paths=EXTRA_SKIP_PATHS,
+            batch_start=0,
+            batch_size=10000,
+            batch_previous_path=PREVIOUS or None,
+        )
+
+    def skip_item(item):
+        """Return True if the item should be skipped"""
+        portal_type = getattr(item, "portal_type", None)
+        if portal_type not in EXPORTED_TYPES:
+            return True
+
+    def extend_item(obj, item):
+        """Extend to work better well with collective.exportimport"""
+        from Acquisition import aq_parent
+        parent = aq_parent(obj)
+        item["parent"] = {
+            "@id": parent.absolute_url(),
+            "@type": getattr(parent, "portal_type", None),
+        }
+        if getattr(parent.aq_base, "UID", None) is not None:
+            item["parent"]["UID"] = parent.UID()
+
+        return item
+
+To use these create three "External Method" in the ZMI root at the Zope root to use that:
+
+* id: "export_content", module name: "json_methods", function name: "export_content"
+* id: "get_item", module name: "json_methods", function name: "get_item"
+* id: "extend_item", module name: "json_methods", function name: "extend_item"
+
+Then you can pass the extender to the export using a query-string: http://localhost:8080/Plone/export_content?additional_wrappers=extend_item
+
+
+Import
+******
+
+Two issues need to be dealt with to allow ``collective.exportimport`` to import the data generated by ``collective.jsonify``.
+
+#. The data is in directories instead of in one large json-file.
+#. The json is not in the expected format.
+
+Starting with version 1.8 you can pass an iterator to the import.
+
+You need to create a directory-walker that sorts the json-files the right way.
+By default it would import them in the order `1.json`, `10.json`, `100.json`, `101.json` and so on.
+
+.. code-block:: python
+
+    from pathlib import Path
+
+    def filesystem_walker(path=None):
+        root = Path(path)
+        assert(root.is_dir())
+        folders = sorted([i for i in root.iterdir() if i.is_dir() and i.name.isdecimal()], key=lambda i: int(i.name))
+        for folder in folders:
+            json_files = sorted([i for i in folder.glob("*.json") if i.stem.isdecimal()], key=lambda i: int(i.stem))
+            for json_file in json_files:
+                logger.debug("Importing %s", json_file)
+                item = json.loads(json_file.read_text())
+                item["json_file"] = str(json_file)
+                item = prepare_data(item)
+                if item:
+                    yield item
+
+The walker takes the path to be the root with one or more directories holding the json-files.
+The sorting of the files is done using the number in the filename.
+
+The method ``prepare_data`` modifies the data before passing it to the import.
+A very similar task is done by ``collective.exportimport`` during export.
+
+.. code-block:: python
+
+    def prepare_data(item):
+        """modify jsonify data to work with c.exportimport"""
+
+        # Drop relationfields or defer the import
+        item.pop("relatedItems", None)
+
+        mapping = {
+            # jsonify => exportimport
+            "_uid": "UID",
+            "_type": "@type",
+            "_path": "@id",
+            "_layout": "layout",
+            # AT fieldnames => DX fieldnames
+            "excludeFromNav": "exclude_from_nav",
+            "allowDiscussion": "allow_discussion",
+            "subject": "subjects",
+            "expirationDate": "expires",
+            "effectiveDate": "effective",
+            "creation_date": "created",
+            "modification_date": "modified",
+            "startDate": "start",
+            "endDate": "end",
+            "openEnd": "open_end",
+            "eventUrl": "event_url",
+            "wholeDay": "whole_day",
+            "contactEmail": "contact_email",
+            "contactName": "contact_name",
+            "contactPhone": "contact_phone",
+            "imageCaption": "image_caption",
+        }
+        for old, new in mapping.items():
+            item = migrate_field(item, old, new)
+
+        if item.get("constrainTypesMode", None) == 1:
+            item = migrate_field(item, "constrainTypesMode", "constrain_types_mode")
+        else:
+            item.pop("locallyAllowedTypes", None)
+            item.pop("immediatelyAddableTypes", None)
+            item.pop("constrainTypesMode", None)
+
+        if "id" not in item:
+            item["id"] = item["_id"]
+        return item
+
+
+    def migrate_field(item, old, new):
+        if item.get(old, _marker) is not _marker:
+            item[new] = item.pop(old)
+        return item
+
+You can pass the generator ``filesystem_walker`` to the import:
+
+.. code-block:: python
+
+    class ImportAll(BrowserView):
+
+        def __call__(self):
+            # ...
+            cfg = getConfiguration()
+            directory = Path(cfg.clienthome) / "import"
+
+            # import content
+            view = api.content.get_view("import_content", portal, request)
+            request.form["form.submitted"] = True
+            request.form["commit"] = 1000
+            view(iterator=filesystem_walker(directory / "mydata"))
+
+            # import default-pages
+            import_deferred = api.content.get_view("import_deferred", portal, request)
+            import_deferred()
+
+
+    class ImportDeferred(BrowserView):
+
+        def __call__(self):
+            self.title = "Import Deferred Settings (default pages)"
+            if not self.request.form.get("form.submitted", False):
+                return self.index()
+
+            for brain in api.content.find(portal_type="Folder"):
+                obj = brain.getObject()
+                annotations = IAnnotations(obj)
+                if DEFERRED_KEY not in annotations:
+                    continue
+
+                default = annotations[DEFERRED_KEY].pop("_defaultpage", None)
+                if default and default in obj:
+                    logger.info("Setting %s as default page for %s", default, obj.absolute_url())
+                    obj.setDefaultPage(default)
+                if not annotations[DEFERRED_KEY]:
+                    annotations.pop(DEFERRED_KEY)
+            api.portal.show_message("Done", self.request)
+            return self.index()
+
+``collective.jsonify`` puts the info on relations, translations and default-pages in the export-file.
+You can use the approach to defer imports to deal with that data after all items were imported.
+The example ``ImportDeferred`` above uses that approach to set the default pages.
+
+This ``global_obj_hook`` below stores that data in a annotation:
+
+.. code-block:: python
+
+    def global_obj_hook(self, obj, item):
+        # Store deferred data in an annotation.
+        keys = ["_defaultpage"]
+        data = {}
+        for key in keys:
+            if value := item.get(key, None):
+                data[key] = value
+        if data:
+            annotations = IAnnotations(obj)
+            annotations[DEFERRED_KEY] = data
+
+
 Written by
 ==========
 
 .. image:: ./docs/starzel.png
     :target: https://www.starzel.de
     :alt: Starzel.de
 
 
+Translations
+============
+
+This product has been translated into
+
+- Spanish
+
 
 Installation
 ============
 
 Install collective.exportimport by adding it to your buildout::
 
     [buildout]
@@ -1884,22 +2150,22 @@
 
     eggs =
         collective.exportimport
 
 
 and then running ``bin/buildout``
 
-You don't need to activate the add-on in the Site Setup Add-ons control panel to be able to use the forms @@export_content and @@import_content in your site.
+You don't need to activate the add-on in the Site Setup Add-ons control panel to be able to use the forms ``@@export_content`` and ``@@import_content`` in your site.
 
 You do need to add it to your buildout configuration and run buildout to make these features available at all. See https://docs.plone.org/manage/installing/installing_addons.html for details.
 
 Installing in Plone 4
 ---------------------
 
-collective.exportimport depends on plone.restapi . For Plone 4, you need to pin plone.restapi to 7.x . When installing plone.restapi version 7.x.x in Plone 4 you may need to add the following version pins to your buildout::
+``collective.exportimport`` depends on ``plone.restapi``. For Plone 4, you need to pin ``plone.restapi`` to 7.x . When installing ``plone.restapi`` version 7.x.x in Plone 4 you may need to add the following version pins to your buildout::
 
     [versions]
     PyJWT = 1.7.1
 
     six = 1.11.0
     attrs = 21.2.0
     plone.rest = 1.6.2
@@ -1928,16 +2194,15 @@
 
     importlib-metadata = 2.1.3
     zipp = 1.2.0
     configparser = 4.0.2
     contextlib2 = 0.6.0.post1
 
 
-These versions are taken from the plone.restapi 7.x README: https://pypi.org/project/plone.restapi/7.8.1/
-
+These versions are taken from the ``plone.restapi`` 7.x README: https://pypi.org/project/plone.restapi/7.8.1/
 
 
 Contribute
 ==========
 
 - Issue Tracker: https://github.com/collective/collective.exportimport/issues
 - Source Code: https://github.com/collective/collective.exportimport
```

### Comparing `collective.exportimport-1.7/docs/conf.py` & `collective.exportimport-1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/docs/export.png` & `collective.exportimport-1.8/docs/export.png`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/docs/import.png` & `collective.exportimport-1.8/docs/import.png`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/docs/starzel.png` & `collective.exportimport-1.8/docs/starzel.png`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/setup.cfg` & `collective.exportimport-1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/setup.py` & `collective.exportimport-1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 else:
     install_requires.append("plone.restapi")
     install_requires.append("beautifulsoup4")
 
 
 setup(
     name="collective.exportimport",
-    version="1.7",
+    version="1.8",
     description="An add-on for Plone to Export and import content, members, relations, translations and localroles.",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Web Environment",
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/config.py` & `collective.exportimport-1.8/src/collective/exportimport/config.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/src/collective/exportimport/configure.zcml` & `collective.exportimport-1.8/src/collective/exportimport/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/src/collective/exportimport/deserializer.py` & `collective.exportimport-1.8/src/collective/exportimport/deserializer.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/src/collective/exportimport/export_content.py` & `collective.exportimport-1.8/src/collective/exportimport/export_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 from Acquisition import aq_base
 from App.config import getConfiguration
+from collective.exportimport import _
 from collective.exportimport import config
 from collective.exportimport.interfaces import IBase64BlobsMarker
 from collective.exportimport.interfaces import IMigrationMarker
 from collective.exportimport.interfaces import IPathBlobsMarker
 from collective.exportimport.interfaces import IRawRichTextMarker
 from operator import itemgetter
 from plone import api
@@ -115,42 +116,42 @@
         if isinstance(self.portal_type, str):
             self.portal_type = [self.portal_type]
         self.migration = migration
         self.path = path or "/".join(self.context.getPhysicalPath())
 
         self.depth = int(depth)
         self.depth_options = (
-            ("-1", "unlimited"),
+            ("-1", _(u"unlimited")),
             ("0", "0"),
             ("1", "1"),
             ("2", "2"),
             ("3", "3"),
             ("4", "4"),
             ("5", "5"),
             ("6", "6"),
             ("7", "7"),
             ("8", "8"),
             ("9", "9"),
             ("10", "10"),
         )
         self.include_blobs = int(include_blobs)
         self.include_blobs_options = (
-            ("0", "as download urls"),
-            ("1", "as base-64 encoded strings"),
-            ("2", "as blob paths"),
+            ("0", _(u"as download urls")),
+            ("1", _(u"as base-64 encoded strings")),
+            ("2", _(u"as blob paths")),
         )
         self.include_revisions = include_revisions
 
         self.update()
 
         if not self.request.form.get("form.submitted", False):
             return self.template()
 
         if not self.portal_type:
-            api.portal.show_message(u"Select at least one type to export", self.request)
+            api.portal.show_message(_(u"Select at least one type to export"), self.request)
             return self.template()
 
         if self.include_blobs == 1:
             # Add marker-interface to request to use our custom serializers
             alsoProvides(self.request, IBase64BlobsMarker)
         elif self.include_blobs == 2:
             # Add marker interface to export blob paths
@@ -190,15 +191,15 @@
                     if number == 1:
                         f.write("[")
                     else:
                         f.write(",")
                     json.dump(datum, f, sort_keys=True, indent=4)
                 if number:
                     f.write("]")
-            msg = u"Exported {} items ({}) as {} to {}".format(
+            msg = _(u"Exported {} items ({}) as {} to {}").format(
                 number, ", ".join(self.portal_type), filename, filepath
             )
             logger.info(msg)
             api.portal.show_message(msg, self.request)
 
             if self.include_blobs == 1:
                 # remove marker interface
@@ -214,15 +215,15 @@
                     if number == 1:
                         f.write("[")
                     else:
                         f.write(",")
                     json.dump(datum, f, sort_keys=True, indent=4)
                 if number:
                     f.write("]")
-                msg = u"Exported {} {}".format(number, self.portal_type)
+                msg = _(u"Exported {} {}").format(number, self.portal_type)
                 logger.info(msg)
                 api.portal.show_message(msg, self.request)
                 response = self.request.response
                 response.setHeader("content-type", "application/json")
                 response.setHeader("content-length", f.tell())
                 response.setHeader(
                     "content-disposition",
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/export_other.py` & `collective.exportimport-1.8/src/collective/exportimport/export_other.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 from Acquisition import aq_base
 from App.config import getConfiguration
+from collective.exportimport import _
 from collective.exportimport import config
 from OFS.interfaces import IOrderedContainer
 from operator import itemgetter
 from plone import api
 from plone.app.discussion.interfaces import IConversation
 from plone.app.portlets.interfaces import IPortletTypeInterface
 from plone.app.redirector.interfaces import IRedirectionStorage
@@ -76,15 +77,15 @@
 
 class BaseExport(BrowserView):
     """Just DRY"""
 
     def download(self, data):
         filename = u"{}.json".format(self.__name__)
         if not data:
-            msg = u"No data to export for {}".format(self.__name__)
+            msg = _(u"No data to export for {}").format(self.__name__)
             logger.info(msg)
             api.portal.show_message(msg, self.request)
             return self.request.response.redirect(self.request["ACTUAL_URL"])
 
         if self.download_to_server:
             directory = config.CENTRAL_DIRECTORY
             if directory:
@@ -93,15 +94,15 @@
                     logger.info("Created central export/import directory %s", directory)
             else:
                 cfg = getConfiguration()
                 directory = cfg.clienthome
             filepath = os.path.join(directory, filename)
             with open(filepath, "w") as f:
                 json.dump(data, f, sort_keys=True, indent=4)
-            msg = u"Exported to {}".format(filepath)
+            msg = _(u"Exported to {}").format(filepath)
             logger.info(msg)
             api.portal.show_message(msg, self.request)
             return self.request.response.redirect(self.request["ACTUAL_URL"])
 
         else:
             data = json.dumps(data, sort_keys=True, indent=4)
             data = safe_bytes(data)
@@ -117,15 +118,15 @@
 
 class ExportRelations(BaseExport):
     """Export all relations"""
 
     def __call__(
         self, download_to_server=False, debug=False, include_linkintegrity=False
     ):
-        self.title = "Export relations"
+        self.title = _(u"Export relations")
         self.download_to_server = download_to_server
         if not self.request.form.get("form.submitted", False):
             return self.index()
         logger.info(u"Exporting relations...")
         data = self.get_all_references(debug, include_linkintegrity)
         logger.info(u"Exported %s relations", len(data))
         self.download(data)
@@ -225,15 +226,15 @@
 
     AUTO_GROUPS = ["AuthenticatedUsers"]
     AUTO_ROLES = ["Authenticated"]
 
     def __init__(self, context, request):
         super(ExportMembers, self).__init__(context, request)
         self.pms = api.portal.get_tool("portal_membership")
-        self.title = "Export members, groups and roles"
+        self.title = _(u"Export members, groups and roles")
         self.group_roles = {}
 
     def __call__(self, download_to_server=False):
         self.download_to_server = download_to_server
         if not self.request.form.get("form.submitted", False):
             return self.index()
 
@@ -323,15 +324,15 @@
 
 
 class ExportTranslations(BaseExport):
 
     DROP_PATH = []
 
     def __call__(self, download_to_server=False):
-        self.title = "Export translations"
+        self.title = _(u"Export translations")
         self.download_to_server = download_to_server
         if not self.request.form.get("form.submitted", False):
             return self.index()
 
         logger.info(u"Exporting translations...")
         data = self.all_translations()
         logger.info(u"Exported %s groups of translations", len(data))
@@ -405,15 +406,15 @@
         return results
 
 
 class ExportLocalRoles(BaseExport):
     """Export all local roles"""
 
     def __call__(self, download_to_server=False):
-        self.title = "Export local roles"
+        self.title = _(u"Export local roles")
         self.download_to_server = download_to_server
         if not self.request.form.get("form.submitted", False):
             return self.index()
 
         logger.info(u"Exporting local roles...")
         data = self.all_localroles()
         logger.info(u"Exported local roles for %s items", len(data))
@@ -462,15 +463,15 @@
         return item
 
 
 class ExportOrdering(BaseExport):
     """Export all local roles"""
 
     def __call__(self, download_to_server=False):
-        self.title = "Export ordering"
+        self.title = _(u"Export ordering")
         self.download_to_server = download_to_server
         if not self.request.form.get("form.submitted", False):
             return self.index()
 
         logger.info(u"Exporting positions in parent...")
         data = self.all_orders()
         logger.info(u"Exported %s positions in parent", len(data))
@@ -498,15 +499,15 @@
         return sorted(results, key=itemgetter("order"))
 
 
 class ExportDefaultPages(BaseExport):
     """Export all default_page settings."""
 
     def __call__(self, download_to_server=False):
-        self.title = "Export default pages"
+        self.title = _(u"Export default pages")
         self.download_to_server = download_to_server
         if not self.request.form.get("form.submitted", False):
             return self.index()
 
         logger.info(u"Exporting default pages...")
         data = self.all_default_pages()
         logger.info(u"Exported %s default pages", len(data))
@@ -577,15 +578,15 @@
                     "default_page": default_page,
                     "default_page_uuid": default_page_uid,
                 }
 
 
 class ExportDiscussion(BaseExport):
     def __call__(self, download_to_server=False):
-        self.title = "Export comments"
+        self.title = _(u"Export comments")
         self.download_to_server = download_to_server
         if not self.request.form.get("form.submitted", False):
             return self.index()
 
         logger.info(u"Exporting discussions...")
         data = self.all_discussions()
         logger.info(u"Exported %s discussions", len(data))
@@ -616,47 +617,54 @@
                 )
                 continue
         return results
 
 
 class ExportPortlets(BaseExport):
     def __call__(self, download_to_server=False):
-        self.title = "Export portlets"
+        self.title = _(u"Export portlets")
         self.download_to_server = download_to_server
         if not self.request.form.get("form.submitted", False):
             return self.index()
 
         logger.info(u"Exporting portlets...")
         data = self.all_portlets()
         logger.info(u"Exported info for %s items with portlets", len(data))
         self.download(data)
 
-    def all_portlets(context=None):
-        results = []
+    def all_portlets(self):
+        self.results = []
 
-        def get_portlets(obj, path):
-            uid = IUUID(obj, None)
-            if not uid:
-                return
-            portlets = export_local_portlets(obj)
-            blacklist = export_portlets_blacklist(obj)
-            obj_results = {}
-            if portlets:
-                obj_results["portlets"] = portlets
-            if blacklist:
-                obj_results["blacklist_status"] = blacklist
-            if obj_results:
-                obj_results["uuid"] = uid
-                results.append(obj_results)
+        portal = api.portal.get()
+        portal.ZopeFindAndApply(portal, search_sub=True, apply_func=self.get_portlets)
+        return self.results
+
+    def get_portlets(self,obj, path):
+        uid = IUUID(obj, None)
+        if not uid:
             return
+        portlets = export_local_portlets(obj)
+        blacklist = export_portlets_blacklist(obj)
+        portlets = self.local_portlets_hook(portlets)
+        blacklist = self.portlets_blacklist_hook(blacklist)
+        obj_results = {}
+        if portlets:
+            obj_results["portlets"] = portlets
+        if blacklist:
+            obj_results["blacklist_status"] = blacklist
+        if obj_results:
+            obj_results["uuid"] = uid
+            self.results.append(obj_results)
+        return
 
-        portal = api.portal.get()
-        portal.ZopeFindAndApply(portal, search_sub=True, apply_func=get_portlets)
-        return results
+    def local_portlets_hook(self, portlets):
+        return portlets
 
+    def portlets_blacklist_hook(self, blacklist):
+        return blacklist
 
 def export_local_portlets(obj):
     """Serialize portlets for one content object
     Code mostly taken from https://github.com/plone/plone.restapi/pull/669
     """
     portlets_schemata = {
         iface: name for name, iface in getUtilitiesFor(IPortletTypeInterface)
@@ -677,15 +685,15 @@
             if portlet_type is None:
                 continue
             assignment = assignment.__of__(mapping)
             settings = IPortletAssignmentSettings(assignment)
             if manager_name not in items:
                 items[manager_name] = []
             values = {}
-            for name in schema.names():
+            for name in schema.names(all=True):
                 value = getattr(assignment, name, None)
                 if RelationValue is not None and isinstance(value, RelationValue):
                     value = value.to_object.UID()
                 elif isinstance(value, RichTextValue):
                     value = {
                         "data": json_compatible(value.raw),
                         "content-type": json_compatible(value.mimeType),
@@ -751,15 +759,15 @@
         redirects[key] = value
 
     return redirects
 
 
 class ExportRedirects(BaseExport):
     def __call__(self, download_to_server=False):
-        self.title = "Export redirects"
+        self.title = _(u"Export redirects")
         self.download_to_server = download_to_server
         if not self.request.form.get("form.submitted", False):
             return self.index()
 
         logger.info(u"Exporting redirects...")
         data = export_plone_redirects()
         logger.info(u"Exported %s redirects", len(data))
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/fix_html.py` & `collective.exportimport-1.8/src/collective/exportimport/fix_html.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: UTF-8 -*-
 from Acquisition import aq_parent
 from bs4 import BeautifulSoup
+from collective.exportimport import _
 from collections import defaultdict
 from logging import getLogger
 from plone import api
 from plone.api.exc import InvalidParameterError
 from plone.app.portlets.interfaces import IPortletTypeInterface
 from plone.app.textfield import RichTextValue
 from plone.app.textfield.interfaces import IRichText
@@ -30,31 +31,32 @@
     "large": "large",
     "listing": "listing",
     "mini": "mini",
     "preview": "preview",
     "thumb": "thumb",
     "tile": "tile",
 }
+FALLBACK_VARIANT = "medium"
 
 
 class FixHTML(BrowserView):
     def __call__(self):
-        self.title = "Fix links to content and images in richtext"
+        self.title = _(u"Fix links to content and images in richtext")
         if not self.request.form.get("form.submitted", False):
             return self.index()
         commit = self.request.form.get("form.commit", True)
 
         msg = []
 
-        fix_count = fix_html_in_content_fields(commit=commit)
-        msg.append(u"Fixed HTML for {} fields in content items".format(fix_count))
+        fix_count = fix_html_in_content_fields(context=self.context, commit=commit)
+        msg.append(_(u"Fixed HTML for {} fields in content items").format(fix_count))
         logger.info(msg[-1])
 
-        fix_count = fix_html_in_portlets()
-        msg.append(u"Fixed HTML for {} portlets".format(fix_count))
+        fix_count = fix_html_in_portlets(context=self.context)
+        msg.append(_(u"Fixed HTML for {} portlets").format(fix_count))
         logger.info(msg[-1])
 
         # TODO: Fix html in tiles
         # tiles = fix_html_in_tiles()
         # msg = u"Fixed html for {} tiles".format(tiles)
 
         api.portal.show_message(u" ".join(m + u"." for m in msg), self.request)
@@ -157,20 +159,20 @@
                         path = path.split("/@@images/")[0]
                         scaled = True
 
             # get uuid from path
             if not uuid:
                 target = find_object(obj, path)
                 if not target:
-                    logger.debug(u"Cannot find target obj for {path}".format(path=path))
+                    logger.debug("Cannot find target obj for %s", path)
                     continue
                 uuid = IUUID(target, None)
 
             if not uuid:
-                logger.debug("Cannot find target obj for {link}".format(link=link))
+                logger.debug("Cannot find target obj for %s", link)
                 continue
 
             # construct new link
             if tag == "img":
                 if scaled:
                     new_href = "resolveuid/{uuid}/@@images/image/{scale}".format(
                         uuid=uuid, scale=scale
@@ -214,19 +216,15 @@
             links[n] = new_href
 
         content_link[attr] = ",".join(
             " ".join([link] + addendum) for link, addendum in zip(links, addenda)
         )
 
         if orig != content_link.decode():
-            logger.debug(
-                u"Changed {tag} {attr} from {orig} to {content_link}".format(
-                    tag=tag, attr=attr, orig=orig, content_link=content_link
-                )
-            )
+            logger.debug("Changed %s %s from %s to %s", tag, attr, orig, content_link)
 
 
 def find_object(base, path):
     """Find a link target based ob a absolute or relative path.
     When the target in the link is no content leave the link as is.
     It might be a link to a browser-view, form or script...
     """
@@ -314,14 +312,16 @@
             for fieldname, field in schema.namesAndDescriptions():
                 if IRichText.providedBy(field):
                     types_with_richtext_fields[portal_type].append(fieldname)
     query = {
         "portal_type": list(types_with_richtext_fields.keys()),
         "sort_on": "path",
     }
+    if context is not None:
+        query["path"] = "/".join(context.getPhysicalPath())
     brains = catalog(**query)
     total = len(brains)
     logger.info("There are %s content items in total, starting migration...", len(brains))
     fixed_fields = 0
     fixed_items = 0
     for index, brain in enumerate(brains, start=1):
         try:
@@ -410,53 +410,83 @@
                                     mimeType=text.mimeType,
                                     outputMimeType=text.outputMimeType,
                                     encoding=text.encoding,
                                 )
                                 fix_count_ref.append(True)
                                 setattr(assignment, fieldname, textvalue)
                                 logger.info(
-                                    "Fixed html for field {} of portlet at {}".format(
-                                        fieldname, obj.absolute_url()
-                                    )
+                                    "Fixed html for field %s of portlet at %s",
+                                    fieldname,
+                                    obj.absolute_url(),
                                 )
                         elif text and isinstance(text, str):
                             clean_text = html_fixer(text, obj)
                             if clean_text and clean_text != text:
                                 textvalue = RichTextValue(
                                     raw=clean_text,
                                     mimeType="text/html",
                                     outputMimeType="text/x-html-safe",
                                     encoding="utf-8",
                                 )
                                 fix_count_ref.append(True)
                                 setattr(assignment, fieldname, textvalue)
                                 logger.info(
-                                    "Fixed html for field {} of portlet {} at {}".format(
-                                        fieldname, str(assignment), obj.absolute_url()
-                                    )
+                                    "Fixed html for field %s of portlet %s at %s",
+                                    fieldname,
+                                    str(assignment),
+                                    obj.absolute_url(),
                                 )
 
-    portal = api.portal.get()
+    if context is None:
+        context = api.portal.get()
     fix_count = []
     f = lambda obj, path: get_portlets(obj, path, fix_count)
-    portal.ZopeFindAndApply(portal, search_sub=True, apply_func=f)
+    context.ZopeFindAndApply(context, search_sub=True, apply_func=f)
     return len(fix_count)
 
 
-def img_variant_fixer(text, obj=None):
+def _get_picture_variant_mapping():
+    """Get mapping from scale to picture variant.
+
+    In standard Plone 6.0 we get:
+
+        {'great': 'large',
+         'huge': 'large',
+         'large': 'large',
+         'larger': 'large',
+         'preview': 'small',
+         'teaser': 'medium'}
+    """
+    picture_variants = api.portal.get_registry_record("plone.picture_variants")
+    mapping = {}
+    for variant, value in picture_variants.items():
+        sourceset = value.get("sourceset")
+        if not sourceset:
+            continue
+        # sourceset is a list, although I expect it to only contain one dictionary.
+        # Sample:
+        # [{'additionalScales': ['large', 'great', 'huge'], 'scale': 'larger'}]
+        for source in sourceset:
+            default_scale = source.get("scale")
+            if default_scale:
+                mapping[default_scale] = variant
+            for scale in source.get("additionalScales", []):
+                if scale not in mapping:
+                    mapping[scale] = variant
+    return mapping
+
+
+def img_variant_fixer(text, obj=None, fallback_variant=None):
     """Set image-variants"""
     if not text:
         return text
 
-    picture_variants = api.portal.get_registry_record("plone.picture_variants")
-    scale_variant_mapping = {
-        k: v["sourceset"][0]["scale"] for k, v in picture_variants.items()
-    }
-    scale_variant_mapping["thumb"] = "mini"
-    fallback_variant = "preview"
+    scale_variant_mapping = _get_picture_variant_mapping()
+    if fallback_variant is None:
+        fallback_variant = FALLBACK_VARIANT
 
     soup = BeautifulSoup(text, "html.parser")
     for tag in soup.find_all("img"):
         if "data-val" not in tag.attrs:
             # maybe external image
             continue
         scale = tag["data-scale"]
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/import_content.py` & `collective.exportimport-1.8/src/collective/exportimport/import_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 from Acquisition import aq_base
+from collective.exportimport import _
 from collective.exportimport import config
 from collective.exportimport.interfaces import IMigrationMarker
 from datetime import datetime
 from DateTime import DateTime
 from datetime import timedelta
 from Persistence import PersistentMapping
 from plone import api
@@ -101,26 +102,33 @@
     # Example: ['/Plone/important/', '/Plone/standard/item']
     INCLUDE_PATHS = []
 
     # Default values for some fields
     # Example: {'which_price': 'normal'}
     DEFAULTS = {}
 
-    def __call__(self, jsonfile=None, return_json=False, limit=None, server_file=None):
+    def __call__(
+        self,
+        jsonfile=None,
+        return_json=False,
+        limit=None,
+        server_file=None,
+        iterator=None
+    ):
         request = self.request
         self.limit = limit
         self.commit = int(request["commit"]) if request.get("commit") else None
         self.import_to_current_folder = request.get("import_to_current_folder", False)
 
         self.handle_existing_content = int(request.get("handle_existing_content", 0))
         self.handle_existing_content_options = (
-            ("0", "Skip: Don't import at all"),
-            ("1", "Replace: Delete item and create new"),
-            ("2", "Update: Reuse and only overwrite imported data"),
-            ("3", "Ignore: Create with a new id"),
+            ("0", _("Skip: Don't import at all")),
+            ("1", _("Replace: Delete item and create new")),
+            ("2", _("Update: Reuse and only overwrite imported data")),
+            ("3", _("Ignore: Create with a new id")),
         )
         self.import_old_revisions = request.get("import_old_revisions", False)
 
         if not self.request.form.get("form.submitted", False):
             return self.template()
 
         # If we open a server file, we should close it at the end.
@@ -128,15 +136,15 @@
         status = "success"
         msg = ""
 
         if server_file and jsonfile:
             # This is an error.  But when you upload 10 GB AND select a server file,
             # it is a pity when you would have to upload again.
             api.portal.show_message(
-                u"json file was uploaded, so the selected server file was ignored.",
+                _(u"json file was uploaded, so the selected server file was ignored."),
                 request=self.request,
                 type="warn",
             )
             server_file = None
             status = "error"
         if server_file and not jsonfile:
             if server_file in self.server_files:
@@ -145,15 +153,15 @@
                     if os.path.exists(full_path):
                         logger.info("Using server file %s", full_path)
                         # Open the file in binary mode and use it as jsonfile.
                         jsonfile = open(full_path, "rb")
                         close_file = True
                         break
             else:
-                msg = "File '{}' not found on server.".format(server_file)
+                msg = _("File '{}' not found on server.").format(server_file)
                 api.portal.show_message(msg, request=self.request, type="warn")
                 server_file = None
                 status = "error"
         if jsonfile:
             self.portal = api.portal.get()
             try:
                 if isinstance(jsonfile, str):
@@ -164,25 +172,30 @@
                 else:
                     raise RuntimeError("Data is neither text, file nor upload.")
             except Exception as e:
                 logger.error(str(e))
                 status = "error"
                 msg = str(e)
                 api.portal.show_message(
-                    u"Exception during uplad: {}".format(e),
+                    _(u"Exception during upload: {}").format(e),
                     request=self.request,
                 )
             else:
                 self.start()
                 msg = self.do_import(data)
                 api.portal.show_message(msg, self.request)
 
         if close_file:
             jsonfile.close()
 
+        if not jsonfile and iterator:
+            self.start()
+            msg = self.do_import(iterator)
+            api.portal.show_message(msg, self.request)
+
         self.finish()
 
         if return_json:
             msg = {"state": status, "msg": msg}
             return json.dumps(msg)
         return self.template()
 
@@ -388,68 +401,88 @@
 
             if not self.update_existing:
                 # create without checking constrains and permissions
                 new = _createObjectByType(
                     item["@type"], container, item["id"], **factory_kwargs
                 )
 
-            new, item = self.global_obj_hook_before_deserializing(new, item)
-
-            # import using plone.restapi deserializers
-            deserializer = getMultiAdapter((new, self.request), IDeserializeFromJson)
             try:
-                new = deserializer(validate_all=False, data=item)
-            except Exception:
-                logger.warning("Cannot deserialize %s %s", item["@type"], item["@id"], exc_info=True)
+                new = self.handle_new_object(item, index, new)
+
+                added.append(new.absolute_url())
+
+                if self.commit and not len(added) % self.commit:
+                    self.commit_hook(added, index)
+            except Exception as e:
+                item_id = item['@id'].split('/')[-1]
+                container.manage_delObjects(item_id)
+                logger.warning(e)
+                logger.warning("Didn't add %s %s", item["@type"], item["@id"], exc_info=True)
                 continue
 
-            # Blobs can be exported as only a path in the blob storage.
-            # It seems difficult to dynamically use a different deserializer,
-            # based on whether or not there is a blob_path somewhere in the item.
-            # So handle this case with a separate method.
-            self.import_blob_paths(new, item)
-            self.import_constrains(new, item)
-
-            self.global_obj_hook(new, item)
-            self.custom_obj_hook(new, item)
-
-            uuid = self.set_uuid(item, new)
-
-            if uuid != item.get("UID"):
-                item["UID"] = uuid
-
-            # Try to set the original review_state
-            self.import_review_state(new, item)
-
-            # Import workflow_history last to drop entries created during import
-            self.import_workflow_history(new, item)
-
-            # Set modification and creation-date as a custom attribute as last step.
-            # These are reused and dropped in ResetModifiedAndCreatedDate
-            modified = item.get("modified", item.get("modification_date", None))
-            if modified:
-                modification_date = DateTime(dateutil.parser.parse(modified))
-                new.modification_date = modification_date
-                new.aq_base.modification_date_migrated = modification_date
-            created = item.get("created", item.get("creation_date", None))
-            if created:
-                creation_date = DateTime(dateutil.parser.parse(created))
-                new.creation_date = creation_date
-                new.aq_base.creation_date_migrated = creation_date
+        return added
+
+    def handle_new_object(self, item, index, new):
+
+        new, item = self.global_obj_hook_before_deserializing(new, item)
+
+        # import using plone.restapi deserializers
+        deserializer = getMultiAdapter((new, self.request), IDeserializeFromJson)
+        try:
+            new = deserializer(validate_all=False, data=item)
+        except Exception:
+            logger.warning("Cannot deserialize %s %s", item["@type"], item["@id"], exc_info=True)
+            raise
+
+        # Blobs can be exported as only a path in the blob storage.
+        # It seems difficult to dynamically use a different deserializer,
+        # based on whether or not there is a blob_path somewhere in the item.
+        # So handle this case with a separate method.
+        self.import_blob_paths(new, item)
+        self.import_constrains(new, item)
+
+        uuid = self.set_uuid(item, new)
+
+        if uuid != item.get("UID"):
+            # Happens only when we import content that doesn't have a UID
+            # for instance when importing from non Plone systems.
             logger.info(
-                "Created item #{}: {} {}".format(
-                    index, item["@type"], new.absolute_url()
-                )
+                "Created new UID for item %s with type %s.",
+                item["@id"],
+                item["@type"]
             )
-            added.append(new.absolute_url())
+            item["UID"] = uuid
 
-            if self.commit and not len(added) % self.commit:
-                self.commit_hook(added, index)
+        self.global_obj_hook(new, item)
+        self.custom_obj_hook(new, item)
 
-        return added
+        # Try to set the original review_state
+        self.import_review_state(new, item)
+
+        # Import workflow_history last to drop entries created during import
+        self.import_workflow_history(new, item)
+
+        # Set modification and creation-date as a custom attribute as last step.
+        # These are reused and dropped in ResetModifiedAndCreatedDate
+        modified = item.get("modified", item.get("modification_date", None))
+        if modified:
+            modification_date = DateTime(dateutil.parser.parse(modified))
+            new.modification_date = modification_date
+            new.aq_base.modification_date_migrated = modification_date
+        created = item.get("created", item.get("creation_date", None))
+        if created:
+            creation_date = DateTime(dateutil.parser.parse(created))
+            new.creation_date = creation_date
+            new.aq_base.creation_date_migrated = creation_date
+        logger.info(
+            "Created item #{}: {} {}".format(
+                index, item["@type"], new.absolute_url()
+            )
+        )
+        return new
 
     def import_versions(self, container, item):
         """Import one item with all its revisions..
         We only apply hooks for the current object not for each version.
         TODO: refactor into import_item to prevent duplicattion
         """
         portal_workflow = api.portal.get_tool("portal_workflow")
@@ -893,28 +926,27 @@
             or parent_url_parsed.netloc == "nohost"
         ):
             # For example localhost:8080, or nohost when running tests.
             # First element will then be a Plone Site id.
             # Get rid of it.
             parent_path = parent_path[1:]
 
+        # Handle folderish Documents provided by plone.volto
+        fti = getUtility(IDexterityFTI, name="Document")
+        parent_type = "Document" if fti.klass.endswith("FolderishDocument") else "Folder"
         # create original structure for imported content
         for element in parent_path:
             if element not in folder:
                 folder = api.content.create(
                     container=folder,
-                    type="Folder",
+                    type=parent_type,
                     id=element,
                     title=element,
                 )
-                logger.info(
-                    u"Created container {} to hold {}".format(
-                        folder.absolute_url(), item["@id"]
-                    )
-                )
+                logger.info(u"Created container %s to hold %s", folder.absolute_url(), item["@id"])
             else:
                 folder = folder[element]
 
         return folder
 
     def set_uuid(self, item, obj):
         uuid = item.get("UID")
@@ -941,24 +973,24 @@
 def fix_portal_type(portal_type):
     normalizer = getUtility(IIDNormalizer)
     return normalizer.normalize(portal_type).replace("-", "")
 
 
 class ResetModifiedAndCreatedDate(BrowserView):
     def __call__(self):
-        self.title = "Reset creation and modification date"
-        self.help_text = """<p>Creation- and modification-dates are changed during import.
-        This resets them to the original dates of the imported content.</p>"""
+        self.title = _(u"Reset creation and modification date")
+        self.help_text = _("<p>Creation- and modification-dates are changed during import." \
+                         "This resets them to the original dates of the imported content.</p>")
         if not self.request.form.get("form.submitted", False):
             return self.index()
 
         portal = api.portal.get()
 
         portal.ZopeFindAndApply(portal, search_sub=True, apply_func=reset_dates)
-        msg = "Finished resetting creation and modification dates."
+        msg = _(u"Finished resetting creation and modification dates.")
         logger.info(msg)
         api.portal.show_message(msg, self.request)
         return self.index()
 
 
 def reset_dates(obj, path):
     modified = getattr(obj.aq_base, "modification_date_migrated", None)
@@ -972,25 +1004,25 @@
         obj.creation_date = created
         del obj.creation_date_migrated
         obj.reindexObject(idxs=["created"])
 
 
 class FixCollectionQueries(BrowserView):
     def __call__(self):
-        self.title = "Fix collection queries"
-        self.help_text = """<p>This fixes invalid collection-criteria that were imported from Plone 4 or 5.</p>"""
+        self.title = _(u"Fix collection queries")
+        self.help_text = _(u"""<p>This fixes invalid collection-criteria that were imported from Plone 4 or 5.</p>""")
 
         if not HAS_COLLECTION_FIX:
             api.portal.show_message(
-                "plone.app.querystring.upgrades.fix_select_all_existing_collections is not available",
+                _(u"plone.app.querystring.upgrades.fix_select_all_existing_collections is not available"),
                 self.request,
             )
             return self.index()
 
         if not self.request.form.get("form.submitted", False):
             return self.index()
 
         portal = api.portal.get()
         fix_select_all_existing_collections(portal)
-        msg = "Finished fixing collection queries."
+        msg = _("Finished fixing collection queries.")
         api.portal.show_message(msg, self.request)
         return self.index()
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/import_other.py` & `collective.exportimport-1.8/src/collective/exportimport/import_other.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 from Acquisition import aq_base
 from BTrees.LLBTree import LLSet
+from collective.exportimport import _
 from collective.exportimport import config
 from datetime import datetime
 from OFS.interfaces import IOrderedContainer
 from operator import itemgetter
 from collective.exportimport.export_other import PORTAL_PLACEHOLDER
 from plone import api
 from plone.app.discussion.comment import Comment
@@ -83,15 +84,15 @@
                     else:
                         raise ("Data is neither text nor upload.")
                 except Exception as e:
                     logger.error(e)
                     status = "error"
                     msg = e
                     api.portal.show_message(
-                        u"Failure while uploading: {}".format(e),
+                        _(u"Failure while uploading: {}").format(e),
                         request=self.request,
                     )
                 else:
                     msg = self.do_import(data)
                     api.portal.show_message(msg, self.request)
 
             if return_json:
@@ -187,21 +188,21 @@
                     data = json.loads(jsonfile.read())
                 else:
                     raise ("Data is neither text nor upload.")
             except Exception as e:
                 status = "error"
                 logger.error(e)
                 api.portal.show_message(
-                    u"Failure while uploading: {}".format(e),
+                    _(u"Failure while uploading: {}").format(e),
                     request=self.request,
                 )
             else:
                 groups = self.import_groups(data["groups"])
                 members = self.import_members(data["members"])
-                msg = u"Imported {} groups and {} members".format(groups, members)
+                msg = _(u"Imported {} groups and {} members").format(groups, members)
                 api.portal.show_message(msg, self.request)
             if return_json:
                 msg = {"state": status, "msg": msg}
                 return json.dumps(msg)
 
         return self.index()
 
@@ -280,15 +281,15 @@
         "relatesTo": "relatedItems",
     }
 
     def __call__(self, jsonfile=None, return_json=False):
 
         if not HAS_RELAPI and not HAS_PLONE6:
             api.portal.show_message(
-                "You need either Plone 6 or collective.relationhelpers to import relations",
+                _("You need either Plone 6 or collective.relationhelpers to import relations"),
                 self.request,
             )
             return self.index()
 
         if jsonfile:
             self.portal = api.portal.get()
             status = "success"
@@ -299,15 +300,15 @@
                 elif isinstance(jsonfile, FileUpload):
                     data = json.loads(jsonfile.read())
                 else:
                     raise ("Data is neither text nor upload.")
             except Exception as e:
                 status = "error"
                 logger.error(e)
-                msg = u"Failure while uploading: {}".format(e)
+                msg = _(u"Failure while uploading: {}").format(e)
                 api.portal.show_message(msg, request=self.request)
             else:
                 msg = self.do_import(data)
                 api.portal.show_message(msg, self.request)
             if return_json:
                 msg = {"state": status, "msg": msg}
                 return json.dumps(msg)
@@ -379,20 +380,20 @@
                     data = json.loads(jsonfile.read())
                 else:
                     raise ("Data is neither text nor upload.")
             except Exception as e:
                 status = "error"
                 logger.error(e)
                 api.portal.show_message(
-                    u"Failure while uploading: {}".format(e),
+                    _(u"Failure while uploading: {}").format(e),
                     request=self.request,
                 )
             else:
                 localroles = self.import_localroles(data)
-                msg = u"Imported {} localroles".format(localroles)
+                msg = _(u"Imported {} localroles").format(localroles)
                 api.portal.show_message(msg, self.request)
             if return_json:
                 msg = {"state": status, "msg": msg}
                 return json.dumps(msg)
 
         return self.index()
 
@@ -400,14 +401,17 @@
         results = 0
         total = len(data)
         for index, item in enumerate(data, start=1):
             obj = api.content.get(UID=item["uuid"])
             if not obj:
                 if item["uuid"] == PORTAL_PLACEHOLDER:
                     obj = api.portal.get()
+                else:
+                    logger.info("Could not find object to set localroles on. UUID: {}".format(item["uuid"]))
+                    continue
             if item.get("localroles"):
                 localroles = item["localroles"]
                 for userid in localroles:
                     obj.manage_setLocalRoles(userid=userid, roles=localroles[userid])
                 logger.debug(
                     u"Set roles on {}: {}".format(obj.absolute_url(), localroles)
                 )
@@ -448,23 +452,23 @@
                     data = json.loads(jsonfile.read())
                 else:
                     raise ("Data is neither text nor upload.")
             except Exception as e:
                 status = "error"
                 logger.error(e)
                 api.portal.show_message(
-                    u"Failure while uploading: {}".format(e),
+                    _(u"Failure while uploading: {}").format(e),
                     request=self.request,
                 )
             else:
                 start = datetime.now()
                 orders = self.import_ordering(data)
                 end = datetime.now()
                 delta = end - start
-                msg = u"Imported {} orders in {} seconds".format(orders, delta.seconds)
+                msg = _(u"Imported {} orders in {} seconds").format(orders, delta.seconds)
                 logger.info(msg)
                 api.portal.show_message(msg, self.request)
             if return_json:
                 msg = {"state": status, "msg": msg}
                 return json.dumps(msg)
 
         return self.index()
@@ -509,15 +513,15 @@
                 logger.error(e)
                 api.portal.show_message(
                     u"Failure while uploading: {}".format(e),
                     request=self.request,
                 )
             else:
                 defaultpages = self.import_default_pages(data)
-                msg = u"Changed {} default pages".format(defaultpages)
+                msg = _(u"Changed {} default pages").format(defaultpages)
                 api.portal.show_message(msg, self.request)
             if return_json:
                 msg = {"state": status, "msg": msg}
                 return json.dumps(msg)
 
         return self.index()
 
@@ -577,35 +581,33 @@
                     data = json.loads(jsonfile.read())
                 else:
                     raise ("Data is neither text nor upload.")
             except Exception as e:
                 status = "error"
                 logger.error(e)
                 api.portal.show_message(
-                    u"Failure while uploading: {}".format(e),
+                    _(u"Failure while uploading: {}").format(e),
                     request=self.request,
                 )
             else:
                 results = self.import_data(data)
-                msg = u"Imported {} comments".format(results)
+                msg = _(u"Imported {} comments").format(results)
                 api.portal.show_message(msg, self.request)
             if return_json:
                 msg = {"state": status, "msg": msg}
                 return json.dumps(msg)
 
         return self.index()
 
     def import_data(self, data):
         results = 0
         for conversation_data in data:
             obj = api.content.get(UID=conversation_data["uuid"])
             if not obj:
                 continue
-            if not obj.restrictedTraverse("@@conversation_view").enabled():
-                continue
             added = 0
             conversation = IConversation(obj)
 
             for item in conversation_data["conversation"]["items"]:
 
                 if isinstance(item["text"], dict) and item["text"].get("data"):
                     item["text"] = item["text"]["data"]
@@ -674,20 +676,20 @@
                     data = json.loads(jsonfile.read())
                 else:
                     raise ("Data is neither text nor upload.")
             except Exception as e:
                 status = "error"
                 logger.error(e)
                 api.portal.show_message(
-                    u"Failure while uploading: {}".format(e),
+                    _(u"Failure while uploading: {}").format(e),
                     request=self.request,
                 )
             else:
                 portlets = self.import_portlets(data)
-                msg = u"Created {} portlets".format(portlets)
+                msg = _(u"Created {} portlets").format(portlets)
                 api.portal.show_message(msg, self.request)
             if return_json:
                 msg = {"state": status, "msg": msg}
                 return json.dumps(msg)
 
         return self.index()
 
@@ -746,15 +748,15 @@
             for property_name, value in assignment_data.items():
                 field = portlet_interface.get(property_name, None)
                 if field is None:
                     continue
                 field = field.bind(assignment)
                 # deserialize data (e.g. for RichText)
                 deserializer = queryMultiAdapter(
-                    (field, obj, request), IFieldDeserializer
+                    (field, assignment, request), IFieldDeserializer
                 )
                 if deserializer is not None:
                     try:
                         value = deserializer(value)
                     except Exception as e:
                         logger.info(
                             u"Could not import portlet data {} for field {} on {}: {}".format(
@@ -809,19 +811,19 @@
                     data = json.loads(jsonfile.read())
                 else:
                     raise ("Data is neither text nor upload.")
             except Exception as e:
                 status = "error"
                 logger.error(e)
                 api.portal.show_message(
-                    u"Failure while uploading: {}".format(e),
+                    _(u"Failure while uploading: {}").format(e),
                     request=self.request,
                 )
             else:
                 import_plone_redirects(data)
-                msg = u"Redirects imported"
+                msg = _(u"Redirects imported")
                 api.portal.show_message(msg, self.request)
             if return_json:
                 msg = {"state": status, "msg": msg}
                 return json.dumps(msg)
 
         return self.index()
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/interfaces.py` & `collective.exportimport-1.8/src/collective/exportimport/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/src/collective/exportimport/locales/update.py` & `collective.exportimport-1.8/src/collective/exportimport/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/src/collective/exportimport/serializer.py` & `collective.exportimport-1.8/src/collective/exportimport/serializer.py`

 * *Files 23% similar despite different names*

```diff
@@ -63,14 +63,23 @@
 IMAGE_SIZE_WARNING = 5000000
 
 logger = logging.getLogger(__name__)
 
 
 # Custom Serializers for Dexterity
 
+def get_blob_path(blob):
+    """Get the path of a ZODB.blob.Blob instance"""
+    connection = blob._p_jar
+    connection.setstate(blob)
+    db = blob._p_jar.db()
+    oid = blob._p_oid
+    tid = blob._p_serial
+    return connection._storage.fshelper.layout.getBlobFilePath(blob._p_oid, blob._p_serial)
+
 
 @adapter(INamedImageField, IDexterityContent, IBase64BlobsMarker)
 class ImageFieldSerializerWithBlobs(DefaultFieldSerializer):
     def __call__(self):
         try:
             image = self.field.get(self.context)
         except AttributeError:
@@ -312,18 +321,15 @@
                 "content-type": self.field.getContentType(self.context),
                 "data": base64.b64encode(data),
                 "encoding": "base64",
             }
             return json_compatible(result)
 
     def get_at_blob_path(obj):
-        oid = obj.getBlob()._p_oid
-        tid = obj._p_serial
-        db = obj._p_jar.db()
-        return db._storage.fshelper.layout.getBlobFilePath(oid, tid)
+        return get_blob_path(obj.getBlob())
 
     @adapter(IBlobImageField, IBaseObject, IPathBlobsMarker)
     @implementer(IFieldSerializer)
     class ATImageFieldSerializerWithBlobPaths(ATDefaultFieldSerializer):
         def __call__(self):
             file_obj = self.field.get(self.context)
             if not file_obj:
@@ -398,64 +404,154 @@
 
     @implementer(ISerializeToJson)
     @adapter(IATTopic, IMigrationMarker)
     class SerializeTopicToJson(SerializeToJson):
         """This uses the topic migration from p.a.contenttypes to turn Criteria into a Querystring."""
 
         def __call__(self, version=None, include_items=False):
-            topic_metadata = super(SerializeTopicToJson, self).__call__(version=version)
+            # 1. Get the default serialisation for AT content
+            item = super(SerializeTopicToJson, self).__call__(version=version)
 
-            # migrate criteria
-            formquery = []
+            # 2. Get querystring-registry
+            query = []
             reg = getUtility(IRegistry)
             reader = IQuerystringRegistryReader(reg)
-            self.registry = reader.parseRegistry()
+            registry = reader.parseRegistry()
+
+            # Inject new selection-operators that were added in Plone 5
+            selection = registry["plone"]["app"]["querystring"]["operation"]["selection"]
+            new_operators = ["all", "any", "none"]
+            for operator  in new_operators:
+                if operator not in selection:
+                    # just a dummy method to pass validation
+                    selection[operator] = {"operation": "collective.exportimport"}
+
+            # Inject any operator for some fields
+            any_operator = "plone.app.querystring.operation.selection.any"
+            fields_with_any_operator = ['Creator', 'Subject', 'portal_type', 'review_state']
+            for field in fields_with_any_operator:
+                operations = registry["plone"]["app"]["querystring"]["field"][field]["operations"]
+                if any_operator not in operations:
+                    registry["plone"]["app"]["querystring"]["field"][field]["operations"].append(any_operator)
+
+            # Inject all operator for Subject
+            all_operator= "plone.app.querystring.operation.selection.all"
+            fields_with_any_operator = ["Subject"]
+            for field in fields_with_any_operator:
+                operations = registry["plone"]["app"]["querystring"]["field"][field]["operations"]
+                if all_operator not in operations:
+                    registry["plone"]["app"]["querystring"]["field"][field]["operations"].append(all_operator)
 
+            # 3. Migrate criteria using the converters from p.a.contenttypes
             criteria = self.context.listCriteria()
             for criterion in criteria:
                 type_ = criterion.__class__.__name__
                 if type_ == "ATSortCriterion":
-                    # Sort order and direction are now stored in the Collection.
-                    self._collection_sort_reversed = criterion.getReversed()
-                    self._collection_sort_on = criterion.Field()
-                    logger.debug(
-                        "Sort on %r, reverse: %s.",
-                        self._collection_sort_on,
-                        self._collection_sort_reversed,
-                    )
+                    # Migrate sorting
+                    item["sort_reversed"] = criterion.getReversed()
+                    item["sort_on"] = criterion.Field()
                     continue
 
                 converter = CONVERTERS.get(type_)
                 if converter is None:
-                    msg = "Unsupported criterion {0}".format(type_)
+                    msg = u"Unsupported criterion {0}".format(type_)
                     logger.error(msg)
                     raise ValueError(msg)
+                before = len(query)
                 try:
-                    converter(formquery, criterion, self.registry)
-                except Exception as e:
-                    logger.info(e)
-
-            topic_metadata["query"] = json_compatible(formquery)
+                    converter(query, criterion, registry)
+                except Exception:
+                    logger.info(u"Error converting criterion %s", criterion.__dict__, exc_info=True)
+                    pass
+
+                # Try to manually convert when no criterion was added
+                # this happens with invalid criteria (e.g. path without a path)
+                if len(query) == before:
+                    fixed = self.fix_criteria(criterion)
+                    if fixed:
+                        query.append(fixed)
+                    else:
+                        logger.info(u"Check maybe broken collection %s", self.context.absolute_url())
+
+            # 4. So some manual fixes in the migrated query
+            indexes_to_fix = [
+                u"portal_type",
+                u"review_state",
+                u"Creator",
+                u"Subject",
+            ]
+            operator_mapping = {
+                # old -> new
+                u"plone.app.querystring.operation.selection.is":
+                    u"plone.app.querystring.operation.selection.any",
+                u"plone.app.querystring.operation.string.is":
+                    u"plone.app.querystring.operation.selection.any",
+            }
+            fixed_query = []
+            for crit in query:
+                if crit["o"].endswith("relativePath") and crit["v"] == "..":
+                    # relativePath no longer accepts ..
+                    crit["v"] = "..::1"
+                if crit["i"] in indexes_to_fix:
+                    for old_operator, new_operator in operator_mapping.items():
+                        if crit["o"] == old_operator:
+                            crit["o"] = new_operator
+                if crit["o"] == u"plone.app.querystring.operation.string.currentUser":
+                    crit["v"] = ""
+                fixed_query.append(crit)
+            query = fixed_query
 
-            # migrate batch size
+            # 5. Migrate batch size
             if self.context.itemCount:
-                topic_metadata["b_size"] = self.context.itemCount
+                item["item_count"] = self.context.itemCount
 
-            if hasattr(self, "_collection_sort_on"):
-                topic_metadata["sort_on"] = self._collection_sort_on
-                topic_metadata["sort_reversed"] = self._collection_sort_reversed
+            # 6. Migrate customView
+            if item.pop("customView", False):
+                item["layout"] = "tabular_view"
+
+            item["query"] = json_compatible(query)
+            return item
+
+        def fix_criteria(self, criterion):
+            """Try to fix some invalid criteria"""
+            FIXES = {
+                # real operators
+                "or": "plone.app.querystring.operation.selection.any",
+                # fake operators
+                "contains": "plone.app.querystring.operation.string.contains",
+                "any": "plone.app.querystring.operation.selection.any",
+            }
 
-            return topic_metadata
+            type_ = criterion.__class__.__name__
+            field = criterion.field
+            value = getattr(criterion, "value", None)
+            operator = getattr(criterion, "operator", None)
+
+            if type_ == "ATSimpleStringCriterion":
+                operator = "contains"
+            if type_ == "ATSelectionCriterion":
+                operator = "any"
+            if type_ == "ATListCriterion":
+                operator = "any"
+            if type_ in ["ATPathCriterion", "ATDateCriteria"] and not value:
+                return
+            if field == "commentators":
+                # no index
+                return
+
+            query = {
+                "i": field,
+                "o": FIXES.get(operator, operator),
+                "v": value,
+            }
+            return query
 
 
 def get_dx_blob_path(obj):
-    oid = obj._blob._p_oid
-    tid = obj._p_serial
-    db = obj._p_jar.db()
-    return db._storage.fshelper.layout.getBlobFilePath(oid, tid)
+    return get_blob_path(obj._blob)
 
 
 @adapter(INamedFileField, IDexterityContent, IPathBlobsMarker)
 @implementer(IFieldSerializer)
 class FileFieldSerializerWithBlobPaths(DefaultFieldSerializer):
     def __call__(self):
         namedfile = self.field.get(self.context)
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/templates/export_other.pt` & `collective.exportimport-1.8/src/collective/exportimport/templates/export_other.pt`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-      i18n:domain="plone.z3cform"
+      i18n:domain="collective.exportimport"
       metal:use-macro="context/main_template/macros/master">
 
 <div metal:fill-slot="main">
     <tal:main-macro metal:define-macro="main">
 
        <h1 class="documentFirstHeading" tal:content="python: view.title" i18n:translate="">
            Export other
        </h1>
 
         <form action="@@export_other" tal:attributes="action request/URL" method="post" enctype="multipart/form-data">
             <div class="field mb-3">
               <div class="form-check">
                 <input class="form-check-input" type="radio" name="download_to_server:int" value="0" id="download_local" checked="checked">
-                <label for="download_local" class="form-check-label"  i18n:translate="">
+                <label for="download_local" class="form-check-label" i18n:translate="">
                   Download to local machine
                 </label>
               </div>
               <div class="form-check">
                 <input class="form-check-input" type="radio" name="download_to_server:int" value="1" id="download_server">
                 <label for="download_server" class="form-check-label" i18n:translate="">
                   Save to file on server
                 </label>
               </div>
             </div>
 
             <div class="formControls" class="form-group">
                 <button class="btn btn-primary submit-widget button-field context"
-                        type="submit" name="form.submitted" value="Export" tal:content="python: view.title" i18n:translate="">Export
+                        type="submit" name="form.submitted" value="Export" tal:content="python: view.title" i18n:attributes="value" i18n:translate="">Export
                 </button>
             </div>
         </form>
 
         <div metal:use-macro="context/@@exportimport_links/links">
           Links to all exports and imports
         </div>
 
         <div tal:define="help_text python: getattr(view, 'help_text', None)"
              tal:condition="python: help_text">
-          <h3>Help</h3>
+          <h3 i18n:translate="">Help</h3>
           <div tal:replace="structure python: help_text"></div>
         </div>
 
     </tal:main-macro>
 </div>
 
 </html>
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/templates/import_content.pt` & `collective.exportimport-1.8/src/collective/exportimport/templates/import_content.pt`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-      i18n:domain="plone.z3cform"
+      i18n:domain="collective.exportimport"
       metal:use-macro="context/main_template/macros/master">
 
 <div metal:fill-slot="main">
     <tal:main-macro metal:define-macro="main">
 
-      <h1 class="documentFirstHeading">Import Content</h1>
+      <h1 class="documentFirstHeading" i18n:translate="">Import Content</h1>
 
-      <p class="documentDescription">Here you can upload a json-file.</p>
+      <p class="documentDescription" i18n:translate="">Here you can upload a json-file.</p>
 
         <form action="." tal:attributes="action request/URL" method="post" enctype="multipart/form-data">
             <div class="form-group">
                 <input type="file" name="jsonfile"/><br/>
             </div>
 
             <tal:block define="server_files view/server_files">
@@ -31,16 +31,16 @@
                   <option tal:repeat="filename server_files" tal:content="filename" tal:attributes="value filename">
                   </option>
                 </select>
               </div>
             </tal:block>
 
             <div class="field mb-3">
-              <label for="include_blobs">Handle existing content</label>
-              <span class="formHelp">
+              <label for="include_blobs" i18n:translate="">Handle existing content</label>
+              <span class="formHelp" i18n:translate="">
                   How should content be handled that exists with the same id/path?
               </span>
               <div class="widget">
                 <select name="handle_existing_content" class="">
                   <option value="0"
                           tal:repeat="current python:view.handle_existing_content_options"
                           tal:attributes="value python: current[0];
@@ -49,52 +49,52 @@
                         0
                   </option>
                 </select>
               </div>
             </div>
 
             <div class="field mb-3">
-              <label for="commit">Do a commit after each number of items</label>
+              <label for="commit" i18n:translate="">Do a commit after each number of items</label>
               <div class="widget">
                 <input type="text" size="5" name="commit" id="commit" value=""
                        tal:attributes="value python:view.commit">
               </div>
             </div>
 
             <div class="field">
               <label>
                 <input
                     type="checkbox"
                     name="import_to_current_folder:boolean"
                     id="import_to_current_folder"
                     tal:attributes="checked python:'checked' if view.import_to_current_folder else None"
                     />
-                Import all items into the current folder
+                <span i18n:translate="">Import all items into the current folder</span>
               </label>
             </div>
 
             <div class="field">
               <label>
                 <input
                     type="checkbox"
                     name="import_old_revisions:boolean"
                     id="import_old_revisions"
                     tal:attributes="checked python:'checked' if view.import_old_revisions else None"
                     />
-                Import all old revisions
-                <span class="formHelp">
+                <span i18n:translate="">Import all old revisions</span>
+                <span class="formHelp" i18n:translate="">
                   This will import the content-history (versioning) for each item that has revisions. Warning: This can significantly slow down the import!
                 </span>
               </label>
             </div>
 
             <div class="formControls" class="form-group">
                 <input type="hidden" name="form.submitted" value="1"/>
                 <button class="btn btn-primary submit-widget button-field context"
-                        type="submit" name="submit" value="Import">Import
+                        type="submit" name="submit" value="Import" i18n:attributes="value" i18n:translate="">Import
                 </button>
             </div>
 
         </form>
 
         <div metal:use-macro="context/@@exportimport_links/links">
           Links to all exports and imports
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/templates/import_defaultpages.pt` & `collective.exportimport-1.8/src/collective/exportimport/templates/import_defaultpages.pt`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-      i18n:domain="plone.z3cform"
+      i18n:domain="collective.exportimport"
       metal:use-macro="context/main_template/macros/master">
 
 <div metal:fill-slot="main">
     <tal:main-macro metal:define-macro="main">
 
-      <h1 class="documentFirstHeading">Import Default Pages</h1>
+      <h1 class="documentFirstHeading" i18n:translate="">Import Default Pages</h1>
 
-      <p class="documentDescription">Here you can upload a json-file.</p>
+      <p class="documentDescription" i18n:translate="">Here you can upload a json-file.</p>
 
         <form action="@@import_defaultpages" tal:attributes="action request/URL" method="post" enctype="multipart/form-data">
             <div class="form-group">
                 <input type="file" name="jsonfile"/><br/>
             </div>
             <div class="formControls" class="form-group">
                 <button class="btn btn-primary submit-widget button-field context"
-                        type="submit" name="form.submitted" value="Import">Import
+                        type="submit" name="form.submitted" value="Import" i18n:attributes="value" i18n:translate="">Import
                 </button>
             </div>
         </form>
 
         <div metal:use-macro="context/@@exportimport_links/links">
           Links to all exports and imports
         </div>
 
         <div>
-          <h3>Help</h3>
-          <p>Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
+          <h3 i18n:translate="">Help</h3>
+          <p i18n:translate="">Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
           <pre>
 [
     {
         "default_page_uuid": "a8e20cec90104700beae7f1cfbad76e6",
         "default_page": "some-page"
         "uuid": "af553734a2e94b2b8d37fab0ea44f633",
     },
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/templates/import_discussion.pt` & `collective.exportimport-1.8/src/collective/exportimport/templates/import_discussion.pt`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-      i18n:domain="plone.z3cform"
+      i18n:domain="collective.exportimport"
       metal:use-macro="context/main_template/macros/master">
 
 <div metal:fill-slot="main">
     <tal:main-macro metal:define-macro="main">
 
-      <h1 class="documentFirstHeading">Import Discussion</h1>
+      <h1 class="documentFirstHeading" i18n:translate="">Import Discussion</h1>
 
-      <p class="documentDescription">Here you can upload a json-file.</p>
+      <p class="documentDescription" i18n:translate="">Here you can upload a json-file.</p>
 
         <form action="@@import_discussion" tal:attributes="action request/URL" method="post" enctype="multipart/form-data">
             <div class="form-group">
                 <input type="file" name="jsonfile"/><br/>
             </div>
             <div class="formControls" class="form-group">
                 <button class="btn btn-primary submit-widget button-field context"
-                        type="submit" name="form.submitted" value="Import">Import
+                        type="submit" name="form.submitted" value="Import" i18n:attributes="value" i18n:translate="">Import
                 </button>
             </div>
         </form>
 
         <div metal:use-macro="context/@@exportimport_links/links">
           Links to all exports and imports
         </div>
 
         <div>
-          <h3>Help</h3>
-          <p>Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
+          <h3 i18n:translate="">Help</h3>
+          <p i18n:translate="">Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
           <pre>
 [
     {
         "conversation": {
             "items_total": 2,
             "items": [
                 {
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/templates/import_localroles.pt` & `collective.exportimport-1.8/src/collective/exportimport/templates/import_localroles.pt`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-      i18n:domain="plone.z3cform"
+      i18n:domain="collective.exportimport"
       metal:use-macro="context/main_template/macros/master">
 
 <div metal:fill-slot="main">
     <tal:main-macro metal:define-macro="main">
 
-      <h1 class="documentFirstHeading">Import Localroles</h1>
+      <h1 class="documentFirstHeading" i18n:translate="">Import Localroles</h1>
 
-      <p class="documentDescription">Here you can upload a json-file.</p>
+      <p class="documentDescription" i18n:translate="">Here you can upload a json-file.</p>
 
         <form action="@@import_localroles" tal:attributes="action request/URL" method="post" enctype="multipart/form-data">
             <div class="form-group">
                 <input type="file" name="jsonfile"/><br/>
             </div>
             <div class="formControls" class="form-group">
                 <button class="btn btn-primary submit-widget button-field context"
-                        type="submit" name="form.submitted" value="Import">Import
+                        type="submit" name="form.submitted" value="Import" i18n:attributes="value" i18n:translate="">Import
                 </button>
             </div>
         </form>
 
         <div metal:use-macro="context/@@exportimport_links/links">
           Links to all exports and imports
         </div>
 
         <div>
-          <h3>Help</h3>
-          <p>Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
+          <h3 i18n:translate="">Help</h3>
+          <p i18n:translate="">Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
           <pre>
 [
     {
         "uuid": "108b9ca15b3f4680b448203ed2f798d1",
         "localroles": {
             "admin": [
                 "Owner"
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/templates/import_members.pt` & `collective.exportimport-1.8/src/collective/exportimport/templates/import_members.pt`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-      i18n:domain="plone.z3cform"
+      i18n:domain="collective.exportimport"
       metal:use-macro="context/main_template/macros/master">
 
 <div metal:fill-slot="main">
     <tal:main-macro metal:define-macro="main">
 
-      <h1 class="documentFirstHeading">Import Members, Groups and their Roles</h1>
+      <h1 class="documentFirstHeading" i18n:translate="">Import Members, Groups and their Roles</h1>
 
-      <p class="documentDescription">Here you can upload a json-file.</p>
+      <p class="documentDescription" i18n:translate="">Here you can upload a json-file.</p>
 
         <form action="@@import_members" tal:attributes="action request/URL" method="post" enctype="multipart/form-data">
             <div class="form-group">
                 <input type="file" name="jsonfile"/><br/>
             </div>
             <div class="formControls" class="form-group">
                 <button class="btn btn-primary submit-widget button-field context"
-                        type="submit" name="form.submitted" value="Import">Import
+                        type="submit" name="form.submitted" value="Import" i18n:attributes="value" i18n:translate="">Import
                 </button>
             </div>
         </form>
 
         <div metal:use-macro="context/@@exportimport_links/links">
           Links to all exports and imports
         </div>
 
         <div>
-          <h3>Help</h3>
-          <p>Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
+          <h3 i18n:translate="">Help</h3>
+          <p i18n:translate="">Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
           <pre>
 {
     "groups": [
         {
             "description": "",
             "email": "",
             "groupid": "Reviewers",
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/templates/import_ordering.pt` & `collective.exportimport-1.8/src/collective/exportimport/templates/import_ordering.pt`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-      i18n:domain="plone.z3cform"
+      i18n:domain="collective.exportimport"
       metal:use-macro="context/main_template/macros/master">
 
 <div metal:fill-slot="main">
     <tal:main-macro metal:define-macro="main">
 
-      <h1 class="documentFirstHeading">Import Object Positions in Parent</h1>
+      <h1 class="documentFirstHeading" i18n:translate="">Import Object Positions in Parent</h1>
 
-      <p class="documentDescription">Here you can upload a json-file.</p>
+      <p class="documentDescription" i18n:translate="">Here you can upload a json-file.</p>
 
         <form action="@@import_ordering" tal:attributes="action request/URL" method="post" enctype="multipart/form-data">
             <div class="form-group">
                 <input type="file" name="jsonfile"/><br/>
             </div>
             <div class="formControls" class="form-group">
                 <button class="btn btn-primary submit-widget button-field context"
-                        type="submit" name="form.submitted" value="Import">Import
+                        type="submit" name="form.submitted" value="Import" i18n:attributes="value" i18n:translate="">Import
                 </button>
             </div>
         </form>
 
         <div metal:use-macro="context/@@exportimport_links/links">
           Links to all exports and imports
         </div>
 
         <div>
-          <h3>Help</h3>
-          <p>Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
+          <h3 i18n:translate="">Help</h3>
+          <p i18n:translate="">Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
           <pre>
 [
     {
         "uuid": "108b9ca15b3f4680b448203ed2f798d1",
         "order": 60
     },
     {
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/templates/import_portlets.pt` & `collective.exportimport-1.8/src/collective/exportimport/templates/import_portlets.pt`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-      i18n:domain="plone.z3cform"
+      i18n:domain="collective.exportimport"
       metal:use-macro="context/main_template/macros/master">
 
 <div metal:fill-slot="main">
     <tal:main-macro metal:define-macro="main">
 
-      <h1 class="documentFirstHeading">Import portlets</h1>
+      <h1 class="documentFirstHeading" i18n:translate="">Import portlets</h1>
 
-      <p class="documentDescription">Here you can upload a json-file.</p>
+      <p class="documentDescription" i18n:translate="">Here you can upload a json-file.</p>
 
         <form action="@@import_portlets" tal:attributes="action request/URL" method="post" enctype="multipart/form-data">
             <div class="form-group">
                 <input type="file" name="jsonfile"/><br/>
             </div>
             <div class="formControls" class="form-group">
                 <button class="btn btn-primary submit-widget button-field context"
-                        type="submit" name="form.submitted" value="Import">Import
+                        type="submit" name="form.submitted" value="Import" i18n:attributes="value" i18n:translate="">Import
                 </button>
             </div>
         </form>
 
         <div metal:use-macro="context/@@exportimport_links/links">
           Links to all exports and imports
         </div>
 
         <div>
-          <h3>Help</h3>
-          <p>Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
+          <h3 i18n:translate="">Help</h3>
+          <p i18n:translate="">Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
           <pre>
 [
     {
         "uuid": "6287ebd5464547dea8e3d5b845677912",
         "portlets": {
             "plone.leftcolumn": [
                 {
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/templates/import_redirects.pt` & `collective.exportimport-1.8/src/collective/exportimport/templates/import_redirects.pt`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-      i18n:domain="plone.z3cform"
+      i18n:domain="collective.exportimport"
       metal:use-macro="context/main_template/macros/master">
 
 <div metal:fill-slot="main">
     <tal:main-macro metal:define-macro="main">
 
-      <h1 class="documentFirstHeading">Import Redirects</h1>
+      <h1 class="documentFirstHeading" i18n:translate="">Import Redirects</h1>
 
-      <p class="documentDescription">Here you can upload a json-file.</p>
+      <p class="documentDescription" i18n:translate="">Here you can upload a json-file.</p>
 
         <form action="@@import_redirects" tal:attributes="action request/URL" method="post" enctype="multipart/form-data">
             <div class="form-group">
                 <input type="file" name="jsonfile"/><br/>
             </div>
             <div class="formControls" class="form-group">
                 <button class="btn btn-primary submit-widget button-field context"
-                        type="submit" name="form.submitted" value="Import">Import
+                        type="submit" name="form.submitted" value="Import" i18n:attributes="value" i18n:translate="">Import
                 </button>
             </div>
         </form>
 
         <div metal:use-macro="context/@@exportimport_links/links">
           Links to all exports and imports
         </div>
 
         <div>
-          <h3>Help</h3>
-          <p>Beware that this import would work only if you keep the same Plone site id and location in the site !</p>
-          <p>More code is needed if you have another use case.</p>
-          <p>Here is an example for the expected format. This is the format created by collective.exportimport when used for export.</p>
+          <h3 i18n:translate="">Help</h3>
+          <p i18n:translate="">Beware that this import would work only if you keep the same Plone site id and location in the site !</p>
+          <p i18n:translate="">More code is needed if you have another use case.</p>
+          <p i18n:translate="">Here is an example for the expected format. This is the format created by collective.exportimport when used for export.</p>
           <pre>
 {
     "/Plone/my-page": "/Plone/my-renamed-page",
     "/Plone/other-page": "/Plone/other-page-moved"
 }
           </pre>
         </div>
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/templates/import_relations.pt` & `collective.exportimport-1.8/src/collective/exportimport/templates/import_relations.pt`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-      i18n:domain="plone.z3cform"
+      i18n:domain="collective.exportimport"
       metal:use-macro="context/main_template/macros/master">
 
 <div metal:fill-slot="main">
     <tal:main-macro metal:define-macro="main">
 
-      <h1 class="documentFirstHeading">Import Relations</h1>
+      <h1 class="documentFirstHeading" i18n:translate="">Import Relations</h1>
 
-      <p class="documentDescription">Here you can upload a json-file.</p>
+      <p class="documentDescription" i18n:translate="">Here you can upload a json-file.</p>
 
         <form action="@@import_relations" tal:attributes="action request/URL" method="post" enctype="multipart/form-data">
             <div class="form-group">
                 <input type="file" name="jsonfile"/><br/>
             </div>
             <div class="formControls" class="form-group">
                 <button class="btn btn-primary submit-widget button-field context"
-                        type="submit" name="form.submitted" value="Import">Import
+                        type="submit" name="form.submitted" value="Import" i18n:attributes="value" i18n:translate="">Import
                 </button>
             </div>
         </form>
 
         <div metal:use-macro="context/@@exportimport_links/links">
           Links to all exports and imports
         </div>
 
         <div>
-          <h3>Help</h3>
-          <p>Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
+          <h3 i18n:translate="">Help</h3>
+          <p i18n:translate="">Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
           <pre>
 [
     {
         "to_uuid": "f83e9e7eff0b4d97a78b87b699f69eb5",
         "relationship": "relatedItems",
         "from_uuid": "6105de8ae2674b5e8433ed18fc305ab6"
     },
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/templates/import_translations.pt` & `collective.exportimport-1.8/src/collective/exportimport/templates/import_translations.pt`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-      i18n:domain="plone.z3cform"
+      i18n:domain="collective.exportimport"
       metal:use-macro="context/main_template/macros/master">
 
 <div metal:fill-slot="main">
     <tal:main-macro metal:define-macro="main">
 
-      <h1 class="documentFirstHeading">Import translations</h1>
+      <h1 class="documentFirstHeading" i18n:translate="">Import translations</h1>
 
-      <p class="documentDescription">Here you can upload a json-file.</p>
+      <p class="documentDescription" i18n:translate="">Here you can upload a json-file.</p>
 
         <form action="@@import_translations" tal:attributes="action request/URL" method="post" enctype="multipart/form-data">
             <div class="form-group">
                 <input type="file" name="jsonfile"/><br/>
             </div>
             <div class="formControls" class="form-group">
                 <button class="btn btn-primary submit-widget button-field context"
-                        type="submit" name="form.submitted" value="Import">Import
+                        type="submit" name="form.submitted" value="Import" i18n:attributes="value" i18n:translate="">Import
                 </button>
             </div>
         </form>
 
         <div metal:use-macro="context/@@exportimport_links/links">
           Links to all exports and imports
         </div>
 
         <div>
-          <h3>Help</h3>
-          <p>Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
+          <h3 i18n:translate="">Help</h3>
+          <p i18n:translate="">Here is a example for the expected format. This is the format created by collective.exportimport when used for export.</p>
           <pre>
 [
     {
         "fr": "8fadf82915554bed8e4ad832175d789a",
         "de": "2a938385be574886b37fd842ef5659b7",
         "en": "6e2fb9b53be94950bea89ba2059e22c1"
     },
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/testing.py` & `collective.exportimport-1.8/src/collective/exportimport/testing.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/src/collective/exportimport/tests/file.pdf` & `collective.exportimport-1.8/src/collective/exportimport/tests/file.pdf`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/src/collective/exportimport/tests/test_drop_and_include.py` & `collective.exportimport-1.8/src/collective/exportimport/tests/test_drop_and_include.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/src/collective/exportimport/tests/test_export.py` & `collective.exportimport-1.8/src/collective/exportimport/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/src/collective/exportimport/tests/test_fix_html.py` & `collective.exportimport-1.8/src/collective/exportimport/tests/test_fix_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,17 +193,17 @@
             # Plone 6 also sets img-variants
             fixed_html = """
 <p><a class="some-class" data-linktype="internal" data-val="{0}" href="resolveuid/{0}">Links to uuid</a></p>
 <p><a href="delete_confirmation">Link to view/form</a></p>
 <p><a data-linktype="internal" data-val="{1}" href="resolveuid/{1}">Link to content</a></p>
 <a href="edit?somequery=foo" target="_self" title="">Link to view with query string</a><br/>
 <a href="#target">Link to anchor</a>
-<img class="image-richtext image-inline picture-variant-preview" data-linktype="image" data-picturevariant="preview" data-scale="" data-val="{2}" src="resolveuid/{2}/@@images/image"/>
-<img class="image-richtext image-inline picture-variant-larger" data-linktype="image" data-picturevariant="larger" data-scale="large" data-val="{2}" src="resolveuid/{2}/@@images/image/large"/>
-<p><a href="image/image_preview"><img class="image-richtext image-inline picture-variant-preview" data-linktype="image" data-picturevariant="preview" data-scale="preview" data-val="{2}" src="resolveuid/{2}/@@images/image/preview"/></a></p>
+<img class="image-richtext image-inline picture-variant-medium" data-linktype="image" data-picturevariant="medium" data-scale="" data-val="{2}" src="resolveuid/{2}/@@images/image"/>
+<img class="image-richtext image-inline picture-variant-large" data-linktype="image" data-picturevariant="large" data-scale="large" data-val="{2}" src="resolveuid/{2}/@@images/image/large"/>
+<p><a href="image/image_preview"><img class="image-richtext image-inline picture-variant-small" data-linktype="image" data-picturevariant="small" data-scale="preview" data-val="{2}" src="resolveuid/{2}/@@images/image/preview"/></a></p>
 """.format(self.contact.UID(), self.team.UID(), self.image.UID())
 
         self.assertEqual(fixed_html, doc.text.raw)
 
     def test_fix_html_status_message(self):
         """Test that the status message displays the correct number of fields fixed."""
         self.create_demo_content()
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/tests/test_import.py` & `collective.exportimport-1.8/src/collective/exportimport/tests/test_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
         changed_raw_data = json.dumps(data)
 
         browser = self.open_page("@@import_content")
         upload = browser.getControl(name="jsonfile")
         upload.add_file(changed_raw_data.encode(), "application/json", "Document.json")
         browser.getControl(name="handle_existing_content").value = ["2"]  # update!
         browser.getForm(action="@@import_content").submit()
-        self.assertIn("Imported 1 items in 0 seconds", browser.contents)
+        self.assertIn("Imported 1 items", browser.contents)
 
         # new_doc now has a updated title
         new_doc = portal["doc1"]
         self.assertEqual(len(portal.contentIds()), 1)
         self.assertEqual(new_doc.Title(), "A different title")
         self.assertEqual(new_doc.portal_type, "Document")
         # The UID is still the same
```

### Comparing `collective.exportimport-1.7/src/collective/exportimport/tests/test_setup.py` & `collective.exportimport-1.8/src/collective/exportimport/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.7/src/collective.exportimport.egg-info/PKG-INFO` & `collective.exportimport-1.8/src/collective.exportimport.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.exportimport
-Version: 1.7
+Version: 1.8
 Summary: An add-on for Plone to Export and import content, members, relations, translations and localroles.
 Home-page: https://github.com/collective/collective.exportimport
 Author: Philip Bauer (for starzel.de)
 Author-email: info@starzel.de
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.exportimport
 Project-URL: Source, https://github.com/collective/collective.exportimport
@@ -60,15 +60,15 @@
 
 Export and import content, members, relations, translations, localroles and much more.
 
 Export and import all kinds of data from and to Plone sites using a intermediate json-format.
 The main use-case is migrations since it enables you to for example migrate from Plone 4 with Archetypes and Python 2 to Plone 6 with Dexterity and Python 3 in one step.
 Most features use `plone.restapi` to serialize and deserialize data.
 
-See also the training on migrating with exportimport: https://training.plone.org/migrations/exportimport.html
+See also the training on migrating with ``exportimport``: https://training.plone.org/migrations/exportimport.html
 
 .. contents:: Contents
     :local:
 
 Features
 ========
 
@@ -129,26 +129,26 @@
 Migrations
 ----------
 
 When a in-place-migration is not required you can choose this addon to migrate the most important parts of your site to json and then import it into a new Plone instance of your targeted version:
 
 * Export content from a Plone site (it supports Plone 4 and 5, Archetypes and Dexterity, Python 2 and 3).
 * Import the exported content into a new site (Plone 5.2+, Dexterity, Python 3)
-* Export and import relations, users and groups with their roles, translations, local roles, ordering, dedault-pages, comments, portlets and redirects.
+* Export and import relations, users and groups with their roles, translations, local roles, ordering, default-pages, comments, portlets and redirects.
 
 How to migrate additional features like Annotations or Marker Interfaces is discussed in the FAQ section.
 
 Other
 -----
 
 You can use this addon to
 
 * Archive your content as json
 * Export data to prepare a migration to another system
-* Combine content from mutiple plone-sites into one.
+* Combine content from multiple plone-sites into one.
 * Import a plone-site as a subsite into another.
 * Import content from other systems as long as it fits the required format.
 * Update or replace existing data
 * ...
 
 Details
 =======
@@ -189,16 +189,16 @@
 Exporting Archetypes content and importing that as Dexterity content works fine but due to changes in field-names some settings would get lost.
 For example the setting to exclude content from the navigation was renamed from ``excludeFromNav`` to ``exclude_from_nav``.
 
 To fix this you can check the checkbox "Modify exported data for migrations".
 This will modify the data during export:
 
 * Drop unused data (e.g. `next_item` and `components`)
-* Remove all relationfields
-* Change some fieldnames that changed between AT and DX
+* Remove all relation fields
+* Change some field names that changed between Archetypes and Dexterity
 
   * ``excludeFromNav`` → ``exclude_from_nav``
   * ``allowDiscussion`` → ``allow_discussion``
   * ``subject`` → ``subjects``
   * ``expirationDate`` → ``expires``
   * ``effectiveDate`` → ``effective``
   * ``creation_date`` → ``created``
@@ -207,16 +207,16 @@
   * ``endDate`` → ``end``
   * ``openEnd`` → ``open_end``
   * ``wholeDay`` → ``whole_day``
   * ``contactEmail`` → ``contact_email``
   * ``contactName`` → ``contact_name``
   * ``contactPhone`` → ``contact_phone``
 
-* Update view names on Folders and Collection thet changed since Plone 4.
-* Export ATTopic and their criteria to Collections with querystrings.
+* Update view names on Folders and Collection that changed since Plone 4.
+* Export ``ATTopic`` and their criteria to Collections with querystrings.
 * Update Collection-criteria.
 * Links and images in Richtext-Fields of content and portlets have changes since Plone 4.
   the view ``/@@fix_html`` allows you to fix these.
 
 
 Control creating imported content
 ---------------------------------
@@ -224,16 +224,16 @@
 You can choose between four options how to deal with content that already exists:
 
   * Skip: Don't import at all
   * Replace: Delete item and create new
   * Update: Reuse and only overwrite imported data
   * Ignore: Create with a new id
 
-Imported content is initially created with ``invokeFactory`` using portal_type and id of the exported item before deserialing the rest of the data.
-You can set additional values by specifying a dict ``factory_kwargs`` that will be passed to the facory.
+Imported content is initially created with ``invokeFactory`` using portal_type and id of the exported item before deserializing the rest of the data.
+You can set additional values by specifying a dict ``factory_kwargs`` that will be passed to the factory.
 Like this you can set values on the imported object that are expected to be there by subscribers to IObjectAddedEvent.
 
 
 Export versioned content
 ------------------------
 
 Exporting versions of Archetypes content will not work because of a bug in plone.restapi (https://github.com/plone/plone.restapi/issues/1335).
@@ -591,15 +591,15 @@
 
 .. code-block:: python
 
     def global_dict_hook(self, item):
         item["creators"] = [i for i in item.get("creators", []) if i]
         return item
 
-This example migrates a PloneHelpCenter to a simple folder/document structure during import.
+This example migrates a ``PloneHelpCenter`` to a simple folder/document structure during import.
 There are a couple more types to handle (as folder or document) but you get the idea, don't you?
 
 .. code-block:: python
 
     def dict_hook_helpcenter(self, item):
         item["@type"] = "Folder"
         item["layout"] = "listing_view"
@@ -867,15 +867,15 @@
 That can happen when options in a field are generated from content in the site.
 In these cases you cannot be sure that all options already exist in the portal while importing the content.
 
 It may also happen, when you have validators that rely on content or configuration that does not exist on import.
 
 .. note::
 
-    For relationfields this is not necessary since relations are imported after content anyway!
+    For relation fields this is not necessary since relations are imported after content anyway!
 
 There are two ways to handle these issues:
 
 * Use a simple setter bypassing the validation used by the restapi
 * Defer the import until all other imports were run
 
 
@@ -1312,15 +1312,15 @@
             results["registry"] = json_compatible(registry)
             return results
 
 
 **Import:**
 
 The import installs the addons and load the settings in the registry.
-Since Plone 5 portal_properties is no longer used.
+Since Plone 5 ``portal_properties`` is no longer used.
 
 .. code-block:: python
 
     from logging import getLogger
     from plone import api
     from plone.registry.interfaces import IRegistry
     from Products.CMFPlone.utils import get_installer
@@ -1483,15 +1483,15 @@
                     "Number of columns does not match for all rows. Some data were skipped in "
                     "data adapter %s/%s",
                     "/".join(obj.getPhysicalPath()),
                     data_adapter_name,
                 )
         return actions
 
-Import exported PloneFormGen data into Easyform:
+Import exported ``PloneFormGen`` data into ``Easyform``:
 
 .. code-block:: python
 
     def obj_hook_easyform(self, obj, item):
         if not item.get("exportimport._inputStorage"):
             return
         from collective.easyform.actions import SavedDataBTree
@@ -1897,22 +1897,288 @@
                 link.decompose()
             elif not link.get("href") and link.text:
                 # drop links without a href but keep the text
                 link.unwrap()
         return soup.decode()
 
 
+Migrate very old Plone Versions with data created by collective.jsonify
+-----------------------------------------------------------------------
+
+Versions older than Plone 4 do not support ``plone.restapi`` which is required to serialize the content used by ``collective.exportimport``.
+
+To migrate Plone 1, 2 and 3 to Plone 6 you can use ``collective.jsonify`` for the export and ``collective.exportimport`` for the import.
+
+Export
+******
+
+Use https://github.com/collective/collective.jsonify to export content.
+
+You include the methods of ``collective.jsonify`` using `External Methods`.
+See https://github.com/collective/collective.jsonify/blob/master/docs/install.rst for more info.
+
+To work better with ``collective.exportimport`` you could extend the exported data using the feature ``additional_wrappers``.
+Add info on the parent of an item to make it easier for ``collective.exportimport`` to import the data.
+
+Here is a full example for `json_methods.py` which should be in `BUILDOUT_ROOT/parts/instance/Extensions/`
+
+.. code-block:: python
+
+    def extend_item(obj, item):
+        """Extend to work better well with collective.exportimport"""
+        from Acquisition import aq_parent
+        parent = aq_parent(obj)
+        item["parent"] = {
+            "@id": parent.absolute_url(),
+            "@type": getattr(parent, "portal_type", None),
+        }
+        if getattr(parent.aq_base, "UID", None) is not None:
+            item["parent"]["UID"] = parent.UID()
+
+        return item
+
+
+Here is a full example for ``json_methods.py`` which should be in ``<BUILDOUT_ROOT>/parts/instance/Extensions/``
+
+.. code-block:: python
+
+    from collective.jsonify.export import export_content as export_content_orig
+    from collective.jsonify.export import get_item
+
+    EXPORTED_TYPES = [
+        "Folder",
+        "Document",
+        "News Item",
+        "Event",
+        "Link",
+        "Topic",
+        "File",
+        "Image",
+        "RichTopic",
+    ]
+
+    EXTRA_SKIP_PATHS = [
+        "/Plone/archiv/",
+        "/Plone/do-not-import/",
+    ]
+
+    # Path from which to continue the export.
+    # The export walks the whole site respecting the order.
+    # It will ignore everything untill this path is reached.
+    PREVIOUS = ""
+
+    def export_content(self):
+        return export_content_orig(
+            self,
+            basedir="/var/lib/zope/json",
+            skip_callback=skip_item,
+            extra_skip_classname=[],
+            extra_skip_id=[],
+            extra_skip_paths=EXTRA_SKIP_PATHS,
+            batch_start=0,
+            batch_size=10000,
+            batch_previous_path=PREVIOUS or None,
+        )
+
+    def skip_item(item):
+        """Return True if the item should be skipped"""
+        portal_type = getattr(item, "portal_type", None)
+        if portal_type not in EXPORTED_TYPES:
+            return True
+
+    def extend_item(obj, item):
+        """Extend to work better well with collective.exportimport"""
+        from Acquisition import aq_parent
+        parent = aq_parent(obj)
+        item["parent"] = {
+            "@id": parent.absolute_url(),
+            "@type": getattr(parent, "portal_type", None),
+        }
+        if getattr(parent.aq_base, "UID", None) is not None:
+            item["parent"]["UID"] = parent.UID()
+
+        return item
+
+To use these create three "External Method" in the ZMI root at the Zope root to use that:
+
+* id: "export_content", module name: "json_methods", function name: "export_content"
+* id: "get_item", module name: "json_methods", function name: "get_item"
+* id: "extend_item", module name: "json_methods", function name: "extend_item"
+
+Then you can pass the extender to the export using a query-string: http://localhost:8080/Plone/export_content?additional_wrappers=extend_item
+
+
+Import
+******
+
+Two issues need to be dealt with to allow ``collective.exportimport`` to import the data generated by ``collective.jsonify``.
+
+#. The data is in directories instead of in one large json-file.
+#. The json is not in the expected format.
+
+Starting with version 1.8 you can pass an iterator to the import.
+
+You need to create a directory-walker that sorts the json-files the right way.
+By default it would import them in the order `1.json`, `10.json`, `100.json`, `101.json` and so on.
+
+.. code-block:: python
+
+    from pathlib import Path
+
+    def filesystem_walker(path=None):
+        root = Path(path)
+        assert(root.is_dir())
+        folders = sorted([i for i in root.iterdir() if i.is_dir() and i.name.isdecimal()], key=lambda i: int(i.name))
+        for folder in folders:
+            json_files = sorted([i for i in folder.glob("*.json") if i.stem.isdecimal()], key=lambda i: int(i.stem))
+            for json_file in json_files:
+                logger.debug("Importing %s", json_file)
+                item = json.loads(json_file.read_text())
+                item["json_file"] = str(json_file)
+                item = prepare_data(item)
+                if item:
+                    yield item
+
+The walker takes the path to be the root with one or more directories holding the json-files.
+The sorting of the files is done using the number in the filename.
+
+The method ``prepare_data`` modifies the data before passing it to the import.
+A very similar task is done by ``collective.exportimport`` during export.
+
+.. code-block:: python
+
+    def prepare_data(item):
+        """modify jsonify data to work with c.exportimport"""
+
+        # Drop relationfields or defer the import
+        item.pop("relatedItems", None)
+
+        mapping = {
+            # jsonify => exportimport
+            "_uid": "UID",
+            "_type": "@type",
+            "_path": "@id",
+            "_layout": "layout",
+            # AT fieldnames => DX fieldnames
+            "excludeFromNav": "exclude_from_nav",
+            "allowDiscussion": "allow_discussion",
+            "subject": "subjects",
+            "expirationDate": "expires",
+            "effectiveDate": "effective",
+            "creation_date": "created",
+            "modification_date": "modified",
+            "startDate": "start",
+            "endDate": "end",
+            "openEnd": "open_end",
+            "eventUrl": "event_url",
+            "wholeDay": "whole_day",
+            "contactEmail": "contact_email",
+            "contactName": "contact_name",
+            "contactPhone": "contact_phone",
+            "imageCaption": "image_caption",
+        }
+        for old, new in mapping.items():
+            item = migrate_field(item, old, new)
+
+        if item.get("constrainTypesMode", None) == 1:
+            item = migrate_field(item, "constrainTypesMode", "constrain_types_mode")
+        else:
+            item.pop("locallyAllowedTypes", None)
+            item.pop("immediatelyAddableTypes", None)
+            item.pop("constrainTypesMode", None)
+
+        if "id" not in item:
+            item["id"] = item["_id"]
+        return item
+
+
+    def migrate_field(item, old, new):
+        if item.get(old, _marker) is not _marker:
+            item[new] = item.pop(old)
+        return item
+
+You can pass the generator ``filesystem_walker`` to the import:
+
+.. code-block:: python
+
+    class ImportAll(BrowserView):
+
+        def __call__(self):
+            # ...
+            cfg = getConfiguration()
+            directory = Path(cfg.clienthome) / "import"
+
+            # import content
+            view = api.content.get_view("import_content", portal, request)
+            request.form["form.submitted"] = True
+            request.form["commit"] = 1000
+            view(iterator=filesystem_walker(directory / "mydata"))
+
+            # import default-pages
+            import_deferred = api.content.get_view("import_deferred", portal, request)
+            import_deferred()
+
+
+    class ImportDeferred(BrowserView):
+
+        def __call__(self):
+            self.title = "Import Deferred Settings (default pages)"
+            if not self.request.form.get("form.submitted", False):
+                return self.index()
+
+            for brain in api.content.find(portal_type="Folder"):
+                obj = brain.getObject()
+                annotations = IAnnotations(obj)
+                if DEFERRED_KEY not in annotations:
+                    continue
+
+                default = annotations[DEFERRED_KEY].pop("_defaultpage", None)
+                if default and default in obj:
+                    logger.info("Setting %s as default page for %s", default, obj.absolute_url())
+                    obj.setDefaultPage(default)
+                if not annotations[DEFERRED_KEY]:
+                    annotations.pop(DEFERRED_KEY)
+            api.portal.show_message("Done", self.request)
+            return self.index()
+
+``collective.jsonify`` puts the info on relations, translations and default-pages in the export-file.
+You can use the approach to defer imports to deal with that data after all items were imported.
+The example ``ImportDeferred`` above uses that approach to set the default pages.
+
+This ``global_obj_hook`` below stores that data in a annotation:
+
+.. code-block:: python
+
+    def global_obj_hook(self, obj, item):
+        # Store deferred data in an annotation.
+        keys = ["_defaultpage"]
+        data = {}
+        for key in keys:
+            if value := item.get(key, None):
+                data[key] = value
+        if data:
+            annotations = IAnnotations(obj)
+            annotations[DEFERRED_KEY] = data
+
+
 Written by
 ==========
 
 .. image:: ./docs/starzel.png
     :target: https://www.starzel.de
     :alt: Starzel.de
 
 
+Translations
+============
+
+This product has been translated into
+
+- Spanish
+
 
 Installation
 ============
 
 Install collective.exportimport by adding it to your buildout::
 
     [buildout]
@@ -1921,22 +2187,22 @@
 
     eggs =
         collective.exportimport
 
 
 and then running ``bin/buildout``
 
-You don't need to activate the add-on in the Site Setup Add-ons control panel to be able to use the forms @@export_content and @@import_content in your site.
+You don't need to activate the add-on in the Site Setup Add-ons control panel to be able to use the forms ``@@export_content`` and ``@@import_content`` in your site.
 
 You do need to add it to your buildout configuration and run buildout to make these features available at all. See https://docs.plone.org/manage/installing/installing_addons.html for details.
 
 Installing in Plone 4
 ---------------------
 
-collective.exportimport depends on plone.restapi . For Plone 4, you need to pin plone.restapi to 7.x . When installing plone.restapi version 7.x.x in Plone 4 you may need to add the following version pins to your buildout::
+``collective.exportimport`` depends on ``plone.restapi``. For Plone 4, you need to pin ``plone.restapi`` to 7.x . When installing ``plone.restapi`` version 7.x.x in Plone 4 you may need to add the following version pins to your buildout::
 
     [versions]
     PyJWT = 1.7.1
 
     six = 1.11.0
     attrs = 21.2.0
     plone.rest = 1.6.2
@@ -1965,16 +2231,15 @@
 
     importlib-metadata = 2.1.3
     zipp = 1.2.0
     configparser = 4.0.2
     contextlib2 = 0.6.0.post1
 
 
-These versions are taken from the plone.restapi 7.x README: https://pypi.org/project/plone.restapi/7.8.1/
-
+These versions are taken from the ``plone.restapi`` 7.x README: https://pypi.org/project/plone.restapi/7.8.1/
 
 
 Contribute
 ==========
 
 - Issue Tracker: https://github.com/collective/collective.exportimport/issues
 - Source Code: https://github.com/collective/collective.exportimport
@@ -1997,18 +2262,66 @@
 
 - Philip Bauer, bauer@starzel.de
 
 - Maurits van Rees, m.van.rees@zestsoftware.nl
 
 - Fred van Dijk, f.van.dijk@zestsoftware.nl
 
+- Leonardo J. Caballero G., leonardocaballero@gmail.com
+
+
 Changelog
 =========
 
 
+1.8 (2023-04-20)
+----------------
+
+- Import: run set_uuid method before we call custom hooks, so the hooks have access to
+  the item UUID. Fix #185.
+  [fredvd]
+
+- Add Spanish translation.
+  [macagua]
+
+- Add i18n support.
+  [macagua]
+
+- Fix html: improve mapping from scale to picture variant.  [maurits]
+
+- Allow overriding the fallback variant in img_variant_fixer.
+  Use 'medium' by default.
+  [maurits]
+
+- Let fix_html view work on the current context.  [maurits]
+
+- Fix the way we get a blob path. (#180)
+  [ale-rt]
+
+- Create documents as containers for items without parent when documents are folderish.
+  [JeffersonBledsoe]
+
+- Add support for passing any iterator as data-source to the import.
+  [pbauer]
+
+- Add example for importing collective.jsonify data to documentation.
+  [pbauer]
+
+- Better serialization of Topics:
+  - Use newer criteria added in Plone 5
+  - Add fallback for some criteria
+  - Export sort_on and sort_reversed
+  - Export customView as tabular_view
+  [pbauer]
+  
+- Always import discussions independent if discussion support is enabled or not
+  on a particular content object (#182)
+  [ajung]
+
+
 1.7 (2023-01-20)
 ----------------
 
 - Filter out 'Discussion Item' in content type export list. Comments have their own export and
   import views. A normal content type export for comments will raise a KeyError when trying to find
   the parent. (#112)
   [fredvd]
```

### Comparing `collective.exportimport-1.7/src/collective.exportimport.egg-info/SOURCES.txt` & `collective.exportimport-1.8/src/collective.exportimport.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 src/collective/exportimport/testing.py
 src/collective/exportimport/locales/README.rst
 src/collective/exportimport/locales/__init__.py
 src/collective/exportimport/locales/collective.exportimport.pot
 src/collective/exportimport/locales/update.py
 src/collective/exportimport/locales/update.sh
 src/collective/exportimport/locales/en/LC_MESSAGES/collective.exportimport.po
+src/collective/exportimport/locales/es/LC_MESSAGES/collective.exportimport.po
 src/collective/exportimport/templates/export_content.pt
 src/collective/exportimport/templates/export_other.pt
 src/collective/exportimport/templates/import_content.pt
 src/collective/exportimport/templates/import_defaultpages.pt
 src/collective/exportimport/templates/import_discussion.pt
 src/collective/exportimport/templates/import_localroles.pt
 src/collective/exportimport/templates/import_members.pt
```

### Comparing `collective.exportimport-1.7/tox.ini` & `collective.exportimport-1.8/tox.ini`

 * *Files identical despite different names*

