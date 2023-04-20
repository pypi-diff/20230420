# Comparing `tmp/PDKMaster-0.9.0.tar.gz` & `tmp/PDKMaster-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDKMaster-0.9.0.tar", last modified: Wed Mar  8 16:09:58 2023, max compression
+gzip compressed data, was "PDKMaster-0.9.1.tar", last modified: Thu Apr 20 13:20:07 2023, max compression
```

## Comparing `PDKMaster-0.9.0.tar` & `PDKMaster-0.9.1.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.958865 PDKMaster-0.9.0/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.926865 PDKMaster-0.9.0/.ci/
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1069 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/.ci/check-dco.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      155 2022-01-13 16:15:17.000000 PDKMaster-0.9.0/.gitignore
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2183 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/.gitlab-ci.yml
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6586 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/Contributing.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      566 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/LICENSE.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.930865 PDKMaster-0.9.0/LICENSES/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2021-02-28 15:28:15.000000 PDKMaster-0.9.0/LICENSES/agpl-3.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11358 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/LICENSES/apache-2.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2021-02-28 15:28:15.000000 PDKMaster-0.9.0/LICENSES/cern_ohl_s_v2.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2021-02-28 15:28:15.000000 PDKMaster-0.9.0/LICENSES/gpl-2.0.txt
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.930865 PDKMaster-0.9.0/PDKMaster.egg-info/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9497 2023-03-08 16:09:58.000000 PDKMaster-0.9.0/PDKMaster.egg-info/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3842 2023-03-08 16:09:58.000000 PDKMaster-0.9.0/PDKMaster.egg-info/SOURCES.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-03-08 16:09:58.000000 PDKMaster-0.9.0/PDKMaster.egg-info/dependency_links.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-03-08 16:09:58.000000 PDKMaster-0.9.0/PDKMaster.egg-info/requires.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       15 2023-03-08 16:09:58.000000 PDKMaster-0.9.0/PDKMaster.egg-info/top_level.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9497 2023-03-08 16:09:58.958865 PDKMaster-0.9.0/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9029 2023-03-08 15:27:35.000000 PDKMaster-0.9.0/README.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.930865 PDKMaster-0.9.0/ReleaseNotes/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      442 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/ReleaseNotes/v0.1.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1234 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/ReleaseNotes/v0.2.0.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1471 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/ReleaseNotes/v0.3.0.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2547 2023-03-08 15:27:35.000000 PDKMaster-0.9.0/ReleaseNotes/v0.9.0.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.930865 PDKMaster-0.9.0/assura_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.0/assura_yaml/.keepme
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      595 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/checkskill.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       14 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/ci-requirements.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2022-06-14 17:01:59.000000 PDKMaster-0.9.0/dev-requirements.txt
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.930865 PDKMaster-0.9.0/display_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.0/display_yaml/.keepme
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.918865 PDKMaster-0.9.0/docs/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.934865 PDKMaster-0.9.0/docs/src/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6063 2023-03-08 15:27:35.000000 PDKMaster-0.9.0/docs/src/conf.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      456 2021-07-22 09:01:44.000000 PDKMaster-0.9.0/docs/src/index.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      141 2021-07-22 09:01:44.000000 PDKMaster-0.9.0/docs/src/pdkmaster._util.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      560 2021-07-22 09:01:44.000000 PDKMaster-0.9.0/docs/src/pdkmaster.design.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      443 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/docs/src/pdkmaster.dispatch.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      312 2022-01-13 16:15:17.000000 PDKMaster-0.9.0/docs/src/pdkmaster.io.coriolis.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2022-02-15 17:28:27.000000 PDKMaster-0.9.0/docs/src/pdkmaster.io.klayout.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      934 2021-07-22 09:01:44.000000 PDKMaster-0.9.0/docs/src/pdkmaster.io.parsing.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      318 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/docs/src/pdkmaster.io.pdkmaster.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      262 2022-01-13 16:15:17.000000 PDKMaster-0.9.0/docs/src/pdkmaster.io.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      449 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/docs/src/pdkmaster.io.spice.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      290 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/docs/src/pdkmaster.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1556 2022-01-13 16:15:17.000000 PDKMaster-0.9.0/docs/src/pdkmaster.technology.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3746 2023-02-22 14:34:15.000000 PDKMaster-0.9.0/dodo.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     4469 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/extract_rules.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    26261 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/files.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.934865 PDKMaster-0.9.0/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      709 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18133 2023-02-22 14:34:28.000000 PDKMaster-0.9.0/pdkmaster/_util.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.938865 PDKMaster-0.9.0/pdkmaster/design/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      237 2023-03-03 15:09:40.000000 PDKMaster-0.9.0/pdkmaster/design/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6045 2023-03-03 14:39:11.000000 PDKMaster-0.9.0/pdkmaster/design/cell.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10199 2023-03-03 14:39:11.000000 PDKMaster-0.9.0/pdkmaster/design/circuit.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8637 2023-03-07 09:14:53.000000 PDKMaster-0.9.0/pdkmaster/design/factory.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.938865 PDKMaster-0.9.0/pdkmaster/design/layout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      664 2023-03-03 15:09:40.000000 PDKMaster-0.9.0/pdkmaster/design/layout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    28469 2023-03-03 15:09:40.000000 PDKMaster-0.9.0/pdkmaster/design/layout/_circuitlayouter.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    48526 2023-03-03 15:09:40.000000 PDKMaster-0.9.0/pdkmaster/design/layout/_primitivelayouter.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3335 2023-03-03 15:09:40.000000 PDKMaster-0.9.0/pdkmaster/design/layout/factory_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    22622 2023-03-03 15:09:40.000000 PDKMaster-0.9.0/pdkmaster/design/layout/layout_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2887 2023-03-06 12:04:55.000000 PDKMaster-0.9.0/pdkmaster/design/library.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2600 2023-03-06 12:04:55.000000 PDKMaster-0.9.0/pdkmaster/design/routinggauge.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.938865 PDKMaster-0.9.0/pdkmaster/dispatch/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1375 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/dispatch/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1378 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/dispatch/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1956 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/dispatch/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7326 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/dispatch/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2803 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/dispatch/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3801 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/dispatch/shape.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.938865 PDKMaster-0.9.0/pdkmaster/io/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.942865 PDKMaster-0.9.0/pdkmaster/io/coriolis/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/coriolis/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    53537 2023-03-06 12:04:55.000000 PDKMaster-0.9.0/pdkmaster/io/coriolis/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.942865 PDKMaster-0.9.0/pdkmaster/io/klayout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      142 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/klayout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37893 2023-03-07 09:15:07.000000 PDKMaster-0.9.0/pdkmaster/io/klayout/export.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    23519 2023-03-03 14:39:11.000000 PDKMaster-0.9.0/pdkmaster/io/klayout/merge_.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.942865 PDKMaster-0.9.0/pdkmaster/io/notebook/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      121 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/notebook/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1253 2023-02-22 14:34:28.000000 PDKMaster-0.9.0/pdkmaster/io/notebook/plotter.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.942865 PDKMaster-0.9.0/pdkmaster/io/parsing/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      214 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/parsing/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18847 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/parsing/assura.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      422 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/parsing/display.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      822 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/parsing/layermap.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17548 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/parsing/skill_grammar.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24374 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/parsing/tf.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.942865 PDKMaster-0.9.0/pdkmaster/io/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18085 2023-03-03 15:09:40.000000 PDKMaster-0.9.0/pdkmaster/io/pdkmaster/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.946865 PDKMaster-0.9.0/pdkmaster/io/spice/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      165 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/spice/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    15809 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/spice/pyspice.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     5904 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/spice/spice_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      181 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/io/spice/typing.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.946865 PDKMaster-0.9.0/pdkmaster/technology/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      276 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/technology/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4032 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/technology/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    77846 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/technology/geometry.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17939 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/technology/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      627 2023-02-22 14:34:21.000000 PDKMaster-0.9.0/pdkmaster/technology/net.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.950865 PDKMaster-0.9.0/pdkmaster/technology/primitive/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      466 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/pdkmaster/technology/primitive/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9661 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/technology/primitive/_core.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1519 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/technology/primitive/_derived.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1176 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/technology/primitive/_param.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24763 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/technology/primitive/conductors.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    44189 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/technology/primitive/devices.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4573 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/technology/primitive/layers.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6752 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/technology/primitive/rules.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9109 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/technology/property_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2138 2023-02-22 14:34:21.000000 PDKMaster-0.9.0/pdkmaster/technology/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20002 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/technology/technology_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2059 2023-02-27 17:19:06.000000 PDKMaster-0.9.0/pdkmaster/technology/wafer_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2958 2023-02-22 14:36:30.000000 PDKMaster-0.9.0/pdkmaster/typing.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-03-08 16:09:58.958865 PDKMaster-0.9.0/setup.cfg
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1410 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/setup.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      863 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/skill.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1278 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/skill2yaml.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.950865 PDKMaster-0.9.0/test/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.950865 PDKMaster-0.9.0/test/unit/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7946 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/_util.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.954865 PDKMaster-0.9.0/test/unit/design/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/design/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3025 2023-03-03 15:09:40.000000 PDKMaster-0.9.0/test/unit/design/cell.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2470 2023-03-03 14:39:11.000000 PDKMaster-0.9.0/test/unit/design/circuit.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3664 2023-03-03 15:12:54.000000 PDKMaster-0.9.0/test/unit/design/factory.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37534 2023-03-03 14:39:11.000000 PDKMaster-0.9.0/test/unit/design/layout.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4584 2023-03-06 12:04:55.000000 PDKMaster-0.9.0/test/unit/design/library.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.954865 PDKMaster-0.9.0/test/unit/dispatch/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/dispatch/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1343 2023-02-22 14:34:21.000000 PDKMaster-0.9.0/test/unit/dispatch/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1397 2023-02-22 14:34:21.000000 PDKMaster-0.9.0/test/unit/dispatch/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1688 2023-02-22 17:29:56.000000 PDKMaster-0.9.0/test/unit/dispatch/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1531 2023-02-22 14:34:21.000000 PDKMaster-0.9.0/test/unit/dispatch/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3403 2023-02-22 17:29:40.000000 PDKMaster-0.9.0/test/unit/dispatch/shape.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    12967 2023-03-03 15:09:40.000000 PDKMaster-0.9.0/test/unit/dummy.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.954865 PDKMaster-0.9.0/test/unit/io/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/io/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.954865 PDKMaster-0.9.0/test/unit/io/klayout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/io/klayout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13480 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/io/klayout/export.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20839 2023-02-22 14:34:28.000000 PDKMaster-0.9.0/test/unit/io/klayout/merge.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.954865 PDKMaster-0.9.0/test/unit/io/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/io/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1863 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/io/pdkmaster/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.954865 PDKMaster-0.9.0/test/unit/io/spice/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/io/spice/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7947 2023-03-03 14:39:11.000000 PDKMaster-0.9.0/test/unit/io/spice/pyspice.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1317 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/io/spice/spice_.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.958865 PDKMaster-0.9.0/test/unit/technology/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/technology/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1313 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/technology/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    56025 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/technology/geometry.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6112 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/technology/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    53503 2023-02-22 14:34:21.000000 PDKMaster-0.9.0/test/unit/technology/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2775 2023-02-22 15:53:25.000000 PDKMaster-0.9.0/test/unit/technology/property.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2072 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/technology/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    12794 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/technology/technology.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1052 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/technology/wafer.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1278 2023-02-16 11:53:22.000000 PDKMaster-0.9.0/test/unit/typing.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      673 2020-03-11 19:28:52.000000 PDKMaster-0.9.0/test.tf
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:09:58.958865 PDKMaster-0.9.0/tf_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.0/tf_yaml/.keepme
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.581072 PDKMaster-0.9.1/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.549072 PDKMaster-0.9.1/.ci/
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1069 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/.ci/check-dco.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      155 2022-01-13 16:15:17.000000 PDKMaster-0.9.1/.gitignore
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2183 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/.gitlab-ci.yml
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6586 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/Contributing.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      566 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/LICENSE.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.549072 PDKMaster-0.9.1/LICENSES/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2021-02-28 15:28:15.000000 PDKMaster-0.9.1/LICENSES/agpl-3.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11358 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/LICENSES/apache-2.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2021-02-28 15:28:15.000000 PDKMaster-0.9.1/LICENSES/cern_ohl_s_v2.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2021-02-28 15:28:15.000000 PDKMaster-0.9.1/LICENSES/gpl-2.0.txt
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.553072 PDKMaster-0.9.1/PDKMaster.egg-info/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9572 2023-04-20 13:20:07.000000 PDKMaster-0.9.1/PDKMaster.egg-info/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3842 2023-04-20 13:20:07.000000 PDKMaster-0.9.1/PDKMaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-04-20 13:20:07.000000 PDKMaster-0.9.1/PDKMaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-04-20 13:20:07.000000 PDKMaster-0.9.1/PDKMaster.egg-info/requires.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       15 2023-04-20 13:20:07.000000 PDKMaster-0.9.1/PDKMaster.egg-info/top_level.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9572 2023-04-20 13:20:07.581072 PDKMaster-0.9.1/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9104 2023-04-20 12:59:58.000000 PDKMaster-0.9.1/README.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.553072 PDKMaster-0.9.1/ReleaseNotes/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      442 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/ReleaseNotes/v0.1.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1234 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/ReleaseNotes/v0.2.0.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1471 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/ReleaseNotes/v0.3.0.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2547 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/ReleaseNotes/v0.9.0.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.553072 PDKMaster-0.9.1/assura_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.1/assura_yaml/.keepme
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      595 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/checkskill.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       14 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/ci-requirements.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2022-06-14 17:01:59.000000 PDKMaster-0.9.1/dev-requirements.txt
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.553072 PDKMaster-0.9.1/display_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.1/display_yaml/.keepme
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.541072 PDKMaster-0.9.1/docs/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.557072 PDKMaster-0.9.1/docs/src/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6063 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/docs/src/conf.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      456 2021-07-22 09:01:44.000000 PDKMaster-0.9.1/docs/src/index.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      141 2021-07-22 09:01:44.000000 PDKMaster-0.9.1/docs/src/pdkmaster._util.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      560 2021-07-22 09:01:44.000000 PDKMaster-0.9.1/docs/src/pdkmaster.design.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      443 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/docs/src/pdkmaster.dispatch.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      312 2022-01-13 16:15:17.000000 PDKMaster-0.9.1/docs/src/pdkmaster.io.coriolis.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2022-02-15 17:28:27.000000 PDKMaster-0.9.1/docs/src/pdkmaster.io.klayout.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      934 2021-07-22 09:01:44.000000 PDKMaster-0.9.1/docs/src/pdkmaster.io.parsing.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      318 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/docs/src/pdkmaster.io.pdkmaster.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      262 2022-01-13 16:15:17.000000 PDKMaster-0.9.1/docs/src/pdkmaster.io.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      449 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/docs/src/pdkmaster.io.spice.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      290 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/docs/src/pdkmaster.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1556 2022-01-13 16:15:17.000000 PDKMaster-0.9.1/docs/src/pdkmaster.technology.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3746 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/dodo.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     4469 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/extract_rules.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    26261 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/files.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.557072 PDKMaster-0.9.1/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      709 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18133 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/_util.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.557072 PDKMaster-0.9.1/pdkmaster/design/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      237 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/design/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6045 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/design/cell.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10199 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/design/circuit.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8637 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/design/factory.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.561072 PDKMaster-0.9.1/pdkmaster/design/layout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      664 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/design/layout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    28468 2023-04-20 12:59:58.000000 PDKMaster-0.9.1/pdkmaster/design/layout/_circuitlayouter.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    48524 2023-04-20 12:59:58.000000 PDKMaster-0.9.1/pdkmaster/design/layout/_primitivelayouter.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3335 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/design/layout/factory_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    22622 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/design/layout/layout_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2887 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/design/library.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2600 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/design/routinggauge.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.561072 PDKMaster-0.9.1/pdkmaster/dispatch/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1375 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/dispatch/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1378 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/dispatch/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1956 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/dispatch/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7326 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/dispatch/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2803 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/dispatch/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3801 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/dispatch/shape.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.561072 PDKMaster-0.9.1/pdkmaster/io/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.561072 PDKMaster-0.9.1/pdkmaster/io/coriolis/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/coriolis/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    57052 2023-04-20 12:59:58.000000 PDKMaster-0.9.1/pdkmaster/io/coriolis/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.565072 PDKMaster-0.9.1/pdkmaster/io/klayout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      142 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/klayout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37892 2023-04-20 12:59:58.000000 PDKMaster-0.9.1/pdkmaster/io/klayout/export.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    23519 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/klayout/merge_.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.565072 PDKMaster-0.9.1/pdkmaster/io/notebook/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      121 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/notebook/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1253 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/notebook/plotter.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.565072 PDKMaster-0.9.1/pdkmaster/io/parsing/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      214 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/parsing/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18847 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/parsing/assura.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      422 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/parsing/display.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      822 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/parsing/layermap.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17548 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/parsing/skill_grammar.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24374 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/parsing/tf.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.565072 PDKMaster-0.9.1/pdkmaster/io/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18079 2023-04-20 12:59:58.000000 PDKMaster-0.9.1/pdkmaster/io/pdkmaster/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.565072 PDKMaster-0.9.1/pdkmaster/io/spice/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      165 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/spice/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    15809 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/spice/pyspice.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     5904 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/spice/spice_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      181 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/io/spice/typing.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.569072 PDKMaster-0.9.1/pdkmaster/technology/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      276 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4032 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    77846 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/geometry.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17939 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      627 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/net.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.573072 PDKMaster-0.9.1/pdkmaster/technology/primitive/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      466 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/primitive/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9661 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/primitive/_core.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1519 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/primitive/_derived.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1176 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/primitive/_param.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24763 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/primitive/conductors.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    44372 2023-04-20 12:59:58.000000 PDKMaster-0.9.1/pdkmaster/technology/primitive/devices.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4914 2023-04-20 12:59:58.000000 PDKMaster-0.9.1/pdkmaster/technology/primitive/layers.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6752 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/primitive/rules.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9109 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/property_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2138 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20002 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/technology_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2059 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/technology/wafer_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2958 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/pdkmaster/typing.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-04-20 13:20:07.581072 PDKMaster-0.9.1/setup.cfg
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1410 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/setup.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      863 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/skill.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1278 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/skill2yaml.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.573072 PDKMaster-0.9.1/test/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.573072 PDKMaster-0.9.1/test/unit/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7946 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/_util.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.573072 PDKMaster-0.9.1/test/unit/design/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/design/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3025 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/design/cell.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2470 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/design/circuit.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3664 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/design/factory.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37534 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/design/layout.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4584 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/design/library.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.577072 PDKMaster-0.9.1/test/unit/dispatch/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/dispatch/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1343 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/dispatch/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1397 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/dispatch/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1688 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/dispatch/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1531 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/dispatch/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3403 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/dispatch/shape.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    12960 2023-04-20 12:59:58.000000 PDKMaster-0.9.1/test/unit/dummy.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.577072 PDKMaster-0.9.1/test/unit/io/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/io/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.577072 PDKMaster-0.9.1/test/unit/io/klayout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/io/klayout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13480 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/io/klayout/export.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20839 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/io/klayout/merge.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.577072 PDKMaster-0.9.1/test/unit/io/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/io/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1862 2023-04-20 12:59:58.000000 PDKMaster-0.9.1/test/unit/io/pdkmaster/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.577072 PDKMaster-0.9.1/test/unit/io/spice/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/io/spice/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7947 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/io/spice/pyspice.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1317 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/io/spice/spice_.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.581072 PDKMaster-0.9.1/test/unit/technology/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/technology/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1313 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/technology/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    56025 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/technology/geometry.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6112 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/technology/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    53443 2023-04-20 12:59:58.000000 PDKMaster-0.9.1/test/unit/technology/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2775 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/technology/property.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2072 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/technology/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    12778 2023-04-20 12:59:58.000000 PDKMaster-0.9.1/test/unit/technology/technology.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1052 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/technology/wafer.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1278 2023-04-07 09:59:24.000000 PDKMaster-0.9.1/test/unit/typing.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      673 2020-03-11 19:28:52.000000 PDKMaster-0.9.1/test.tf
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-04-20 13:20:07.581072 PDKMaster-0.9.1/tf_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.1/tf_yaml/.keepme
```

### Comparing `PDKMaster-0.9.0/.ci/check-dco.py` & `PDKMaster-0.9.1/.ci/check-dco.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/.gitlab-ci.yml` & `PDKMaster-0.9.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/Contributing.md` & `PDKMaster-0.9.1/Contributing.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/LICENSE.md` & `PDKMaster-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/LICENSES/agpl-3.0.txt` & `PDKMaster-0.9.1/LICENSES/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/LICENSES/apache-2.0.txt` & `PDKMaster-0.9.1/LICENSES/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/LICENSES/cern_ohl_s_v2.txt` & `PDKMaster-0.9.1/LICENSES/cern_ohl_s_v2.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/LICENSES/gpl-2.0.txt` & `PDKMaster-0.9.1/LICENSES/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/PDKMaster.egg-info/PKG-INFO` & `PDKMaster-0.9.1/PDKMaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDKMaster
-Version: 0.9.0
+Version: 0.9.1
 Summary: ASIC PDK Manager and Design Framework
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/PDKMaster
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/PDKMaster/issues
 Requires-Python: >=3.6
@@ -14,14 +14,15 @@
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.1: fix coriolis export, primitive type values are not python types.
 * v0.9.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * v0.3.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.3.0/ReleaseNotes/v0.3.0.md)
 * v0.2.1: add klayout dependency
 * v0.2.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.2.0/ReleaseNotes/v0.2.0.md)
 * v0.1: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.2.0/ReleaseNotes/v0.1.md)
 
 # Overview
```

### Comparing `PDKMaster-0.9.0/PDKMaster.egg-info/SOURCES.txt` & `PDKMaster-0.9.1/PDKMaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/PKG-INFO` & `PDKMaster-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDKMaster
-Version: 0.9.0
+Version: 0.9.1
 Summary: ASIC PDK Manager and Design Framework
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/PDKMaster
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/PDKMaster/issues
 Requires-Python: >=3.6
@@ -14,14 +14,15 @@
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.1: fix coriolis export, primitive type values are not python types.
 * v0.9.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * v0.3.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.3.0/ReleaseNotes/v0.3.0.md)
 * v0.2.1: add klayout dependency
 * v0.2.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.2.0/ReleaseNotes/v0.2.0.md)
 * v0.1: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.2.0/ReleaseNotes/v0.1.md)
 
 # Overview
```

### Comparing `PDKMaster-0.9.0/README.md` & `PDKMaster-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.1: fix coriolis export, primitive type values are not python types.
 * v0.9.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * v0.3.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.3.0/ReleaseNotes/v0.3.0.md)
 * v0.2.1: add klayout dependency
 * v0.2.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.2.0/ReleaseNotes/v0.2.0.md)
 * v0.1: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.2.0/ReleaseNotes/v0.1.md)
 
 # Overview
```

### Comparing `PDKMaster-0.9.0/ReleaseNotes/v0.2.0.md` & `PDKMaster-0.9.1/ReleaseNotes/v0.2.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/ReleaseNotes/v0.3.0.md` & `PDKMaster-0.9.1/ReleaseNotes/v0.3.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/ReleaseNotes/v0.9.0.md` & `PDKMaster-0.9.1/ReleaseNotes/v0.9.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/checkskill.py` & `PDKMaster-0.9.1/checkskill.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/docs/src/conf.py` & `PDKMaster-0.9.1/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/docs/src/pdkmaster.design.rst` & `PDKMaster-0.9.1/docs/src/pdkmaster.design.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/docs/src/pdkmaster.io.parsing.rst` & `PDKMaster-0.9.1/docs/src/pdkmaster.io.parsing.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/docs/src/pdkmaster.technology.rst` & `PDKMaster-0.9.1/docs/src/pdkmaster.technology.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/dodo.py` & `PDKMaster-0.9.1/dodo.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/extract_rules.py` & `PDKMaster-0.9.1/extract_rules.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/files.py` & `PDKMaster-0.9.1/files.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/__init__.py` & `PDKMaster-0.9.1/pdkmaster/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/_util.py` & `PDKMaster-0.9.1/pdkmaster/_util.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/design/cell.py` & `PDKMaster-0.9.1/pdkmaster/design/cell.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/design/circuit.py` & `PDKMaster-0.9.1/pdkmaster/design/circuit.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/design/factory.py` & `PDKMaster-0.9.1/pdkmaster/design/factory.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/design/layout/__init__.py` & `PDKMaster-0.9.1/pdkmaster/design/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/design/layout/_circuitlayouter.py` & `PDKMaster-0.9.1/pdkmaster/design/layout/_circuitlayouter.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         if contact_right is not None:
             if len(contact_right.top) != 1:
                 raise NotImplementedError(
                     f"Multiple top layers for Via '{contact_right.name}'",
                 )
 
         impls = tuple(filter(
-            lambda impl: isinstance(impl, _prm.Implant) and impl.type_ != _prm.adjImplT,
+            lambda impl: isinstance(impl, _prm.Implant) and impl.type_ != _prm.adjImpl,
             mosfet.implant,
         ))
         if len(impls) != 1:
             raise NotImplementedError(
                 f"Multiple implant for MOSFET '{inst.prim.name}'",
             )
         self._implant = impls[0]
@@ -582,15 +582,15 @@
                     via_left = top_left + top_henc
                 else:
                     via_left = None
             if bottom_bottom is not None:
                 if top_bottom is not None:
                     via_bottom = max(bottom_bottom + bottom_venc, top_bottom + top_venc)
                 else:
-                    via_bottom = bottom_bottom + bottom_henc
+                    via_bottom = bottom_bottom + bottom_venc
             else:
                 if top_bottom is not None:
                     via_bottom = top_bottom + top_venc
                 else:
                     via_bottom = None
             if bottom_right is not None:
                 if top_right is not None:
```

### Comparing `PDKMaster-0.9.0/pdkmaster/design/layout/_primitivelayouter.py` & `PDKMaster-0.9.1/pdkmaster/design/layout/_primitivelayouter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1112,22 +1112,22 @@
             cath = prim.ports.cathode
         else:
             an = portnets["anode"]
             cath = portnets["cathode"]
 
         wirenet_args = {
             "implant": prim.implant,
-            "portnets": {"conn": an if prim.implant.type_ == _prm.pImplT else cath},
+            "portnets": {"conn": an if prim.implant.type_ == _prm.pImpl else cath},
         }
         if prim.min_implant_enclosure is not None:
             wirenet_args["implant_enclosure"] = prim.min_implant_enclosure
         if prim.well is not None:
             wirenet_args.update({
                 "well": prim.well,
-                "well_net": cath if prim.implant.type_ == _prm.pImplT else an,
+                "well_net": cath if prim.implant.type_ == _prm.pImpl else an,
             })
 
         layout = self.fab.new_layout()
         layout.add_primitive(prim=prim.wire, **wirenet_args, **diode_params)
         wireact_bounds = layout.bounds(mask=prim.wire.mask)
         act_width = wireact_bounds.right - wireact_bounds.left
         act_height = wireact_bounds.top - wireact_bounds.bottom
```

### Comparing `PDKMaster-0.9.0/pdkmaster/design/layout/factory_.py` & `PDKMaster-0.9.1/pdkmaster/design/layout/factory_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/design/layout/layout_.py` & `PDKMaster-0.9.1/pdkmaster/design/layout/layout_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/design/library.py` & `PDKMaster-0.9.1/pdkmaster/design/library.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/design/routinggauge.py` & `PDKMaster-0.9.1/pdkmaster/design/routinggauge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/dispatch/__init__.py` & `PDKMaster-0.9.1/pdkmaster/dispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/dispatch/edge.py` & `PDKMaster-0.9.1/pdkmaster/dispatch/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/dispatch/mask.py` & `PDKMaster-0.9.1/pdkmaster/dispatch/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/dispatch/primitive.py` & `PDKMaster-0.9.1/pdkmaster/dispatch/primitive.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/dispatch/rule.py` & `PDKMaster-0.9.1/pdkmaster/dispatch/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/dispatch/shape.py` & `PDKMaster-0.9.1/pdkmaster/dispatch/shape.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/io/coriolis/export.py` & `PDKMaster-0.9.1/pdkmaster/io/coriolis/export.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,44 @@
 """Generate coriolis setup file"""
 # SPDX-License-Identifier: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
 from textwrap import dedent, indent
 from itertools import product
-from typing import Set, Tuple, Optional, cast, overload
+from typing import Set, Tuple, Iterable, Optional, Callable, cast, overload
 
 from ... import dispatch as _dsp
 from ...typing  import GDSLayerSpecDict
 from ...technology import (
-    mask as _msk, primitive as _prm, geometry as _geo, technology_ as _tch,
+    mask as _msk, net as _net, primitive as _prm, geometry as _geo, technology_ as _tch,
 )
 from ...design import cell as _cell, routinggauge as _rg, library as _lbry
 from ...design.layout import layout_ as _laylay
 
-__all__ = ["FileExporter"]
+__all__ = ["CoriolisExportSpec", "FileExporter"]
+
+
+class CoriolisExportSpec:
+    """This class allows to specify
+
+    API Notes:
+        * No backwards guarantees are given for this class yet. Future changes
+          may break user code.
+    """
+    def __init__(self, *,
+        globalnets: Iterable[str]=(),
+        net_direction_cb: Optional[Callable[[str], str]]=None,
+    ) -> None:
+        self._globalnets = tuple(globalnets)
+        self._net_direction_cb = net_direction_cb
+
+    @property
+    def globalnets(self) -> Tuple[str]:
+        return self._globalnets
+    @property
+    def net_direction_cb(self) -> Optional[Callable[[str], str]]:
+        return self._net_direction_cb
 
 
 def _str_create_basic(name, mat, *,
     minsize=None, minspace=None, minarea=None, gds_layer=None, gds_datatype=None
 ):
     s = "createBL(\n"
     s += f"    tech, '{name}', BasicLayer.Material.{mat},\n"
@@ -108,15 +130,15 @@
         ))
 
     def Implant(self, prim: _prm.Implant):
         return _str_create_basic(
             prim.name,
             (
                 f"{prim.type_.value}Implant"
-                if prim.type_ in (_prm.nImplT, _prm.pImplT)
+                if prim.type_ in (_prm.nImpl, _prm.pImpl)
                 else "other"
             ),
             minsize=prim.min_width, minspace=prim.min_space,
             minarea=prim.min_area,
             **_args_gds_layer(prim, gds_layers=self.gds_layers),
         )
 
@@ -327,15 +349,15 @@
                 f"('minEnclosure', '{ind.name}', '{prim.wire.name}', {enc}, "
                 "Length|Asymmetric, ''),\n"
             )
         s = indent(s, prefix="# ")
         return s
 
     def MIMCapacitor(self, prim: _prm.Diode):
-        s = f"('minWidth', '{prim.name}', {prim.min_width}, Length, ''),\n"
+        s = f"# ('minWidth', '{prim.name}', {prim.min_width}, Length, ''),\n"
         s += "# TODO: MIMCapacitor rules\n"
 
         return s
 
     def Diode(self, prim: _prm.Diode):
         s = f"('minWidth', '{prim.name}', {prim.min_width}, Length, ''),\n"
         for i in range(len(prim.indicator)):
@@ -414,21 +436,29 @@
     def Bipolar(self, prim: _prm.Bipolar):
         return f"# Not implemented: Bipolar '{prim.name}'\n"
 
     def MinWidth(self, prim: _prm.MinWidth):
         return f"# ('minWidth', '{prim.prim.name}', '{prim.min_width}', Length, '')"
 
     def Spacing(self, prim: _prm.Spacing):
+        from ...technology.primitive._derived import _DerivedPrimitive
+        def comment_string(*, prim1: _prm.PrimitiveT, prim2: Optional[_prm.PrimitiveT]):
+            if isinstance(prim1, _DerivedPrimitive) or isinstance(prim2, _DerivedPrimitive):
+                return "# "
+            else:
+                return ""
         if prim.primitives2 is None:
             return "".join(
+                f"{comment_string(prim1=prim1, prim2=None)}"
                 f"('minSpacing', '{prim1.name}', {prim.min_space}, Length, ''),\n"
                 for prim1 in prim.primitives1
             )
         else:
             return "".join(
+                f"{comment_string(prim1=prim1, prim2=prim2)}"
                 f"('minSpacing', '{prim1.name}', '{prim2.name}', {prim.min_space}, "
                 "Length|Asymmetric, ''),\n"
                 for prim1, prim2 in product(prim.primitives1, prim.primitives2)
             )
 
     def Enclosure(self, prim: _prm.Enclosure):
         return (
@@ -437,16 +467,17 @@
         )
 
     def NoOverlap(self, prim: _prm.NoOverlap):
         return f"# ('noOverlap', '{prim.prim1.name}', '{prim.prim2.name}'),\n"
 
 
 class _LibraryGenerator:
-    def __init__(self, *, tech: _tch.Technology):
+    def __init__(self, *, tech: _tch.Technology, spec: Optional[CoriolisExportSpec]):
         self.tech = tech
+        self.spec = spec
         self.metals: Tuple[_prm.MetalWire, ...] = tuple(filter(
             lambda m: not isinstance(m, _prm.MIMTop),
             tech.primitives.__iter_type__(_prm.MetalWire),
         ))
         self.vias: Tuple[_prm.Via, ...] = tuple(tech.primitives.__iter_type__(_prm.Via))
         assert len(self.metals) == len(self.vias)
         self.pinmasks = pinmasks = {}
@@ -810,35 +841,71 @@
                 bnd = layout.boundary
                 assert bnd is not None, f"Cell boundary needed for {cell.name}"
 
                 pls = tuple(layout._sublayouts.__iter_type__(_laylay._MaskShapesSubLayout))
                 def get_netname(sl: _laylay._MaskShapesSubLayout):
                     return "*" if sl.net is None else sl.net.name
 
-                netnames = {get_netname(sl) for sl in pls}
+                net_names = sorted({get_netname(sl) for sl in pls})
 
                 s += (
                     "    cell.setAbutmentBox(Box(\n"
                     f"        u({bnd.left}), u({bnd.bottom}), u({bnd.right}), u({bnd.top}),\n"
                     "    ))\n"
                     "    nets = {\n"
                     + "\n".join(
-                        f"        '{net}': Net.create(cell, '{net}'),"
-                        for net in sorted(netnames)
+                        f"        '{net_name}': Net.create(cell, '{net_name}'),"
+                        for net_name in net_names
                     )
                     + "\n    }\n"
                 )
 
                 for sl in pls:
                     s += indent(
                         f"net = nets['{get_netname(sl)}']\n" +
                         "".join(self._s_shape(ms) for ms in sl.shapes),
                         prefix="    ",
                     )
 
+                spec = self.spec
+                if spec is not None:
+                    ckt = cell.circuit
+
+                    for net in ckt.ports:
+                        if net.name in spec.globalnets:
+                            s += f"    nets['{net.name}'].setGlobal(True)\n"
+                    cb = spec.net_direction_cb
+                    if cb is not None:
+                        for net in ckt.ports:
+                            net_name = net.name
+                            t = cb(net_name)
+                            if t == "supply":
+                                s += (
+                                    f"    nets['{net_name}'].setType(Net.Type.POWER)\n"
+                                    f"    nets['{net_name}'].setDirection(Net.Direction.IN)\n"
+                                )
+                            elif t == "ground":
+                                s += (
+                                    f"    nets['{net_name}'].setType(Net.Type.GROUND)\n"
+                                    f"    nets['{net_name}'].setDirection(Net.Direction.IN)\n"
+                                )
+                            elif t == "clock":
+                                s += (
+                                    f"    nets['{net_name}'].setType(Net.Type.CLOCK)\n"
+                                    f"    nets['{net_name}'].setDirection(Net.Direction.IN)\n"
+                                )
+                            elif t == "in":
+                                s += f"    nets['{net_name}'].setDirection(Net.Direction.IN)\n"
+                            elif t == "out":
+                                s += f"    nets['{net_name}'].setDirection(Net.Direction.OUT)\n"
+                            else:
+                                raise ValueError(
+                                    f"wrong net_direction_cb return value '{t}'"
+                                )
+                        
                 for sl in layout._sublayouts.__iter_type__(_laylay._InstanceSubLayout):
                     # Currently usage of af.getCell() may not work as intended when
                     # two libraries have a cell with the same name.
                     # TODO: support libraries with cells with same name properly
                     r = {
                         _geo.Rotation.R0: "ID",
                         _geo.Rotation.R90: "R1",
@@ -1176,25 +1243,25 @@
                 style.addDrawingStyle( group='Viewer', name='undef'         , color=toRGB('Violet'     ), border=0, pattern='2244118822441188' )
         """[1:])
 
         clrs = ("Blue", "Aqua", "LightPink", "Green", "Yellow", "Violet", "Red")
 
         s += "\n    # Active Layers.\n"
         for prim in self.tech.primitives.__iter_type__(_prm.Well):
-            rgb = "Tan" if prim.type_ == _prm.nImplT else "LightYellow"
+            rgb = "Tan" if prim.type_ == _prm.nImpl else "LightYellow"
             s += (
                 f"    style.addDrawingStyle(group='Active Layers', name='{prim.name}'"
                 f", color=toRGB('{rgb}'), pattern=toHexa('urgo.8'), border=1"
                 ", threshold=threshold)\n"
             )
         for prim in filter(
             lambda p: not isinstance(p, _prm.Well),
             self.tech.primitives.__iter_type__(_prm.Implant),
         ):
-            rgb = "LawnGreen" if prim.type_ == _prm.nImplT else "Yellow"
+            rgb = "LawnGreen" if prim.type_ == _prm.nImpl else "Yellow"
             s += (
                 f"    style.addDrawingStyle(group='Active Layers', name='{prim.name}'"
                 f", color=toRGB('{rgb}'), pattern=toHexa('antihash0.8'), border=1"
                 ", threshold=threshold)\n"
             )
         for prim in self.tech.primitives.__iter_type__(_prm.WaferWire):
             s += (
@@ -1295,17 +1362,31 @@
             Viewer.Graphics.setStyle( 'Alliance.Classic [black]' )
         """[1:]), prefix="    ")
 
         return s
 
 
 class FileExporter:
-    def __init__(self, *, tech: _tch.Technology, gds_layers: GDSLayerSpecDict):
-        self.tech = tech
-        self.gds_layers = gds_layers
+    def __init__(self, *,
+        tech: _tch.Technology, gds_layers: GDSLayerSpecDict,
+        spec: Optional[CoriolisExportSpec]=None
+    ):
+        self._tech = tech
+        self._gds_layers = gds_layers
+        self._spec = spec
+
+    @property
+    def tech(self) -> _tch.Technology:
+        return self._tech
+    @property
+    def gds_layers(self) -> GDSLayerSpecDict:
+        return self._gds_layers
+    @property
+    def spec(self) -> Optional[CoriolisExportSpec]:
+        return self._spec
 
     @overload
     def __call__(self,
         obj: None, *, routinggauge: None=None,
     ) -> str:
         ...
     @overload
@@ -1331,9 +1412,9 @@
         return s
 
     def _s_tech(self):
         gen = _TechnologyGenerator()
         return gen(tech=self.tech, gds_layers=self.gds_layers)
 
     def _s_lib(self, lib: _lbry.Library, *, routinggauge: Optional[_rg.RoutingGauge]):
-        gen = _LibraryGenerator(tech=self.tech)
+        gen = _LibraryGenerator(tech=self.tech, spec=self.spec)
         return gen(lib, routinggauge=routinggauge)
```

### Comparing `PDKMaster-0.9.0/pdkmaster/io/klayout/export.py` & `PDKMaster-0.9.1/pdkmaster/io/klayout/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,15 @@
 
     return s
 
 
 def _str_lvsdiode(tech: _tch.Technology, diode: _prm.Diode, spice_params: SpicePrimParamsT):
     s = f"# {diode.name}\n"
 
-    is_n = diode.implant.type_ == _prm.nImplT
+    is_n = diode.implant.type_ == _prm.nImpl
 
     s_diode = _mask_conv(diode.mask)
     s_conn = _mask_conv(diode.wire.conn_mask)
     s_well = _mask_conv(
         diode.well.mask if diode.well is not None
         else tech.substrate
     )
```

### Comparing `PDKMaster-0.9.0/pdkmaster/io/klayout/merge_.py` & `PDKMaster-0.9.1/pdkmaster/io/klayout/merge_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/io/notebook/plotter.py` & `PDKMaster-0.9.1/pdkmaster/io/notebook/plotter.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/io/parsing/assura.py` & `PDKMaster-0.9.1/pdkmaster/io/parsing/assura.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/io/parsing/layermap.py` & `PDKMaster-0.9.1/pdkmaster/io/parsing/layermap.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/io/parsing/skill_grammar.py` & `PDKMaster-0.9.1/pdkmaster/io/parsing/skill_grammar.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/io/parsing/tf.py` & `PDKMaster-0.9.1/pdkmaster/io/parsing/tf.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/io/pdkmaster/export.py` & `PDKMaster-0.9.1/pdkmaster/io/pdkmaster/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,17 +103,17 @@
         return s
 
     def _params_widthspacedesignmask(self, prim: _prm.WidthSpaceDesignMaskPrimitiveT):
         return self._params_widthspace(prim) + self._params_designmask(prim)
 
     def _params_Base(self, prim: _prm.Base):
         lookup = {
-            _prm.nBaseT: "nBaseT",
-            _prm.pBaseT: "pBaseT",
-            _prm.undopedBaseT: "undopedBaseT",
+            _prm.nBase: "nBase",
+            _prm.pBase: "pBase",
+            _prm.undopedBase: "undopedBase",
         }
         return f"type_={lookup[prim.type_]}"
 
     def _params_Marker(self, prim: _prm.Marker):
         return self._params_designmask(prim)
 
     def _params_Auxiliary(self, prim: _prm.Auxiliary):
```

### Comparing `PDKMaster-0.9.0/pdkmaster/io/spice/pyspice.py` & `PDKMaster-0.9.1/pdkmaster/io/spice/pyspice.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/io/spice/spice_.py` & `PDKMaster-0.9.1/pdkmaster/io/spice/spice_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/edge.py` & `PDKMaster-0.9.1/pdkmaster/technology/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/geometry.py` & `PDKMaster-0.9.1/pdkmaster/technology/geometry.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/mask.py` & `PDKMaster-0.9.1/pdkmaster/technology/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/net.py` & `PDKMaster-0.9.1/pdkmaster/technology/net.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/primitive/_core.py` & `PDKMaster-0.9.1/pdkmaster/technology/primitive/_core.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/primitive/_derived.py` & `PDKMaster-0.9.1/pdkmaster/technology/primitive/_derived.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/primitive/_param.py` & `PDKMaster-0.9.1/pdkmaster/technology/primitive/_param.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/primitive/conductors.py` & `PDKMaster-0.9.1/pdkmaster/technology/primitive/conductors.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/primitive/devices.py` & `PDKMaster-0.9.1/pdkmaster/technology/primitive/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,26 @@
 )
 
 from ._core import (
     _Primitive, _PrimitiveNet, _MaskPrimitive, _WidthSpacePrimitive,
 )
 from ._param import _PrimParam
 from ._derived import _Intersect
-from .layers import Marker, ExtraProcess, Insulator, Implant, adjImplT
+from .layers import Marker, ExtraProcess, Insulator, Implant, adjImpl
 from .conductors import Well,  WaferWire, GateWire, MetalWire, MIMTop, Via
 
 
 __all__ = [
     "DevicePrimitiveT", "DeviceParamT", "DeviceParamsT",
     "ResistorWireT", "ResistorIndicatorT", "Resistor",
     "DiodeIndicatorT", "Diode",
     "CapacitorT", "MIMCapacitor",
-    "MOSFETGate", "MOSFET", "Bipolar", "npnBipolarT", "pnpBipolarT",
+    "MOSFETGate", "MOSFET", "Bipolar", "BipolarTypeT", "npnBipolar", "pnpBipolar",
+    # Backwards compatibility
+    "npnBipolarT", "pnpBipolarT",
 ]
 
 
 class _DevicePrimitive(_Primitive):
     """This is a base class to indicate that the primitive is a device
     primitive. A device is a primitive that can be instantiated in a
     circuit and thus has a certain electrical characterics that typically
@@ -840,15 +842,15 @@
         min_contactgate_space: Optional[float]=None,
     ):
         super().__init__(name=name)
 
         implant = cast_MultiT(implant)
         type_ = None
         for impl in implant:
-            if impl.type_ != adjImplT:
+            if impl.type_ != adjImpl:
                 if type_ is None:
                     type_ = impl.type_
                 elif type_ != impl.type_:
                     raise ValueError(
                         "both n and p type implants for same MOSFET are not allowed"
                     )
         if type_ is None:
@@ -1048,15 +1050,15 @@
         are reserved for implemting more general layout generation.
     """
     class BipolarType(Enum):
         """The type of implant.
         Currently implemented types are: npn, pnp. The .value of the enum
         object is the string of the type; e.g. "npn", "pnp".
 
-        These types are also made available as `npnBipolarT` and `pnpBipolarT`
+        These types are also made available as `npnBipolar` and `pnpBipolar`
         in the primitive module.
         """
         npn = "npn"
         pnp = "pnp"
 
         def __hash__(self) -> int:
             return super().__hash__()
@@ -1086,9 +1088,13 @@
         return super()._generate_rules(tech=tech)
 
     @property
     def designmasks(self) -> Iterable[_msk.DesignMask]:
         yield from super().designmasks
         for indicator in self.indicator:
             yield from indicator.designmasks
-npnBipolarT = Bipolar.BipolarType.npn
-pnpBipolarT = Bipolar.BipolarType.pnp
+BipolarTypeT = Bipolar.BipolarType
+npnBipolar = Bipolar.BipolarType.npn
+pnpBipolar = Bipolar.BipolarType.pnp
+# Backwards compatibility
+npnBipolarT = npnBipolar
+pnpBipolarT = pnpBipolar
```

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/primitive/layers.py` & `PDKMaster-0.9.1/pdkmaster/technology/primitive/layers.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,42 +7,50 @@
 
 from ._core import (
     _MaskPrimitive, _DesignMaskPrimitive, _WidthSpaceDesignMaskPrimitive,
 )
 
 
 __all__ = [
-    "Base", "nBaseT", "pBaseT", "undopedBaseT",
+    "Base", "BaseTypeT", "nBase", "pBase", "undopedBase",
     "Marker", "Auxiliary", "ExtraProcess", "Insulator", 
-    "Implant", "nImplT", "pImplT", "adjImplT",
+    "Implant", "ImplantTypeT", "nImpl", "pImpl", "adjImpl",
+    # Backwards compatibility
+    "nBaseT", "pBaseT", "undopedBaseT",
+    "nImplT", "pImplT", "adjImplT",
 ]
 
 
 class Base(_MaskPrimitive):
     class BaseType(Enum):
         n = "n"
         p = "p"
         undoped = "undoped"
 
-    def __init__(self, *, type_: BaseType):
+    def __init__(self, *, type_: "BaseTypeT"):
         super().__init__(name="base", mask=_wfr.wafer)
 
         self._type = type_
 
     @property
     def type_(self) -> "Base.BaseType":
         return self._type
 
     def _generate_rules(self, *,
         tech: _tch.Technology, gen_mask: bool = True,
     ) -> Iterable[_rle.RuleT]:
         return super()._generate_rules(tech=tech, gen_mask=gen_mask)
-nBaseT = Base.BaseType.n
-pBaseT = Base.BaseType.p
-undopedBaseT = Base.BaseType.undoped
+BaseTypeT = Base.BaseType
+nBase = Base.BaseType.n
+pBase = Base.BaseType.p
+undopedBase = Base.BaseType.undoped
+# Backward compatibility
+nBaseT = nBase
+pBaseT = pBase
+undopedBaseT = undopedBase
 
 
 class Marker(_DesignMaskPrimitive):
     """The Marker primitive represents a layer used by other primitives for definition
     of these primitives; typically a recognition.
     It does not represent a processing layer and thus no physical mask is corresponding
     with this primitive.
@@ -110,15 +118,15 @@
             arguments
     """
     class ImplantType(Enum):
         """The type of implant.
         Currently implemented types are: n, p, adjust. The .value of the enum
         object is the string of the type; e.g. "n", "p", ...
 
-        These types are also made available as `nImplT`, `pImplT` and `adjImplT`
+        These types are also made available as `nImpl`, `pImpl` and `adjImpl`
         in the primitive module.
         """
         n = "n"
         p = "p"
         adjust = "adjust"
 
         def __hash__(self) -> int:
@@ -140,10 +148,15 @@
         tech: "_tch.Technology",
     ) -> Iterable[_rle.RuleT]:
         return super()._generate_rules(tech=tech)
 
     @property
     def type_(self) -> ImplantType:
         return self._type
-nImplT = Implant.ImplantType.n
-pImplT = Implant.ImplantType.p
-adjImplT = Implant.ImplantType.adjust
+ImplantTypeT = Implant.ImplantType
+nImpl = Implant.ImplantType.n
+pImpl = Implant.ImplantType.p
+adjImpl = Implant.ImplantType.adjust
+# Backwards compatibility
+nImplT = nImpl
+pImplT = pImpl
+adjImplT = adjImpl
```

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/primitive/rules.py` & `PDKMaster-0.9.1/pdkmaster/technology/primitive/rules.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/property_.py` & `PDKMaster-0.9.1/pdkmaster/technology/property_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/rule.py` & `PDKMaster-0.9.1/pdkmaster/technology/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/technology_.py` & `PDKMaster-0.9.1/pdkmaster/technology/technology_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/technology/wafer_.py` & `PDKMaster-0.9.1/pdkmaster/technology/wafer_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/pdkmaster/typing.py` & `PDKMaster-0.9.1/pdkmaster/typing.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/setup.py` & `PDKMaster-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/skill.py` & `PDKMaster-0.9.1/skill.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/skill2yaml.py` & `PDKMaster-0.9.1/skill2yaml.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/_util.py` & `PDKMaster-0.9.1/test/unit/_util.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/design/cell.py` & `PDKMaster-0.9.1/test/unit/design/cell.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/design/circuit.py` & `PDKMaster-0.9.1/test/unit/design/circuit.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/design/factory.py` & `PDKMaster-0.9.1/test/unit/design/factory.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/design/layout.py` & `PDKMaster-0.9.1/test/unit/design/layout.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/design/library.py` & `PDKMaster-0.9.1/test/unit/design/library.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/dispatch/edge.py` & `PDKMaster-0.9.1/test/unit/dispatch/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/dispatch/mask.py` & `PDKMaster-0.9.1/test/unit/dispatch/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/dispatch/primitive.py` & `PDKMaster-0.9.1/test/unit/dispatch/primitive.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/dispatch/rule.py` & `PDKMaster-0.9.1/test/unit/dispatch/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/dispatch/shape.py` & `PDKMaster-0.9.1/test/unit/dispatch/shape.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/dummy.py` & `PDKMaster-0.9.1/test/unit/dummy.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,37 +21,37 @@
         return "Empty"
     @property
     def grid(self) -> float:
         return 0.005
 
     def __init__(self):
         super().__init__(
-            primitives=_prm.Primitives(_prm.Base(type_=_prm.undopedBaseT)),
+            primitives=_prm.Primitives(_prm.Base(type_=_prm.undopedBase)),
         )
 empty_tech = EmptyTech()
 
 
 class DummyTech(_tch.Technology):
     @property
     def name(self) -> str:
         return "Dummy"
     @property
     def grid(self) -> float:
         return 0.005
     
     def __init__(self):
-        prims = _prm.Primitives(_prm.Base(type_=_prm.nBaseT))
+        prims = _prm.Primitives(_prm.Base(type_=_prm.nBase))
 
-        nwell = _prm.Well(type_=_prm.nImplT, name="nwell", min_width=1.5, min_space=1.5)
+        nwell = _prm.Well(type_=_prm.nImpl, name="nwell", min_width=1.5, min_space=1.5)
         deepwell = _prm.DeepWell(
             name="deepwell", min_width=3.0, min_space=3.0,
             well=nwell, min_well_overlap=0.8, min_well_enclosure=0.8,
         )
-        nplus = _prm.Implant(type_=_prm.nImplT, name="nplus", min_width=1.0, min_space=1.0)
-        pplus = _prm.Implant(type_=_prm.pImplT, name="pplus", min_width=1.0, min_space=1.0)
+        nplus = _prm.Implant(type_=_prm.nImpl, name="nplus", min_width=1.0, min_space=1.0)
+        pplus = _prm.Implant(type_=_prm.pImpl, name="pplus", min_width=1.0, min_space=1.0)
         hvox = _prm.Insulator(name="hvox", min_width=0.5, min_space=0.5)
         active = _prm.WaferWire(
             name="active", min_width=0.3, min_space=0.2,
             allow_in_substrate=True,
             implant=(nplus, pplus), min_implant_enclosure=_prp.Enclosure(0.2),
             implant_abut="none", allow_contactless_implant=False,
             well=nwell, min_well_enclosure=_prp.Enclosure(1.0),
@@ -172,17 +172,17 @@
             implant=nplus, min_gateimplant_enclosure=_prp.Enclosure((0.4, 0.6)),
             contact=contact, min_contactgate_space=0.75,
             min_sd_width=0.8,
         )
         prims += (mosgate, hvgate, esdgate, nmos, pmos, esd, hvnmos, hvpmos, esdnmos)
 
         bip = _prm.Marker(name="bip")
-        npn = _prm.Bipolar(name="npn", type_=_prm.npnBipolarT, indicator=bip)
+        npn = _prm.Bipolar(name="npn", type_=_prm.npnBipolar, indicator=bip)
         pnp = _prm.Bipolar(
-            name="pnp", type_=_prm.pnpBipolarT, indicator=bip,
+            name="pnp", type_=_prm.pnpBipolar, indicator=bip,
         )
         prims += (bip, npn, pnp)
 
         mimcap = _prm.MIMCapacitor(
             name="MIMCap", bottom=metal, top=mimtop, via=via,
             min_bottom_top_enclosure=_prp.Enclosure(0.2),
             min_bottomvia_top_space=0.25,
```

### Comparing `PDKMaster-0.9.0/test/unit/io/klayout/export.py` & `PDKMaster-0.9.1/test/unit/io/klayout/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/io/klayout/merge.py` & `PDKMaster-0.9.1/test/unit/io/klayout/merge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/io/pdkmaster/export.py` & `PDKMaster-0.9.1/test/unit/io/pdkmaster/export.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class ExportTest(unittest.TestCase):
     def test_primitivegenerator(self):
         # Some more test to cover code not covered by test_pdkmastergenerator()
         primgen = _PrimitiveGenerator()
 
         prim = _prm.Well(
-            type_=_prm.pImplT, name="pwell",
+            type_=_prm.pImpl, name="pwell",
             min_width=1.5, min_space=1.5, min_space_samenet=1.0,
         )
         primgen(prim)
 
         prim = _prm.MetalWire(
             name="M1", min_width=0.1, min_space=0.1, grid=0.010,
             min_density=0.20, max_density=0.80,
```

### Comparing `PDKMaster-0.9.0/test/unit/io/spice/pyspice.py` & `PDKMaster-0.9.1/test/unit/io/spice/pyspice.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/io/spice/spice_.py` & `PDKMaster-0.9.1/test/unit/io/spice/spice_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/technology/edge.py` & `PDKMaster-0.9.1/test/unit/technology/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/technology/geometry.py` & `PDKMaster-0.9.1/test/unit/technology/geometry.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/technology/mask.py` & `PDKMaster-0.9.1/test/unit/technology/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/technology/primitive.py` & `PDKMaster-0.9.1/test/unit/technology/primitive.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,32 +102,32 @@
         self.assertEqual(prim1, prim1bis)
         self.assertNotEqual(prim1, prim2)
 
         rules = tuple(prim1._generate_rules(tech=dummy_tech))
         self.assertIn(prim1.mask, rules)
 
     def test_implanttype(self):
-        self.assertEqual(_prm.nImplT, _prm.nImplT)
-        self.assertNotEqual(_prm.nImplT, _prm.pImplT)
+        self.assertEqual(_prm.nImpl, _prm.nImpl)
+        self.assertNotEqual(_prm.nImpl, _prm.pImpl)
 
-        self.assertEqual(hash(_prm.nImplT), hash(_prm.nImplT))
-        self.assertNotEqual(hash(_prm.nImplT), hash(_prm.pImplT))
+        self.assertEqual(hash(_prm.nImpl), hash(_prm.nImpl))
+        self.assertNotEqual(hash(_prm.nImpl), hash(_prm.pImpl))
 
         with self.assertWarns(UserWarning):
-            _prm.nImplT == "n"
+            _prm.nImpl == "n"
 
     def test_implant(self):
         prim1 = _prm.Implant(
-            name="prim1", min_width=1.0, min_space=1.0, type_=_prm.nImplT,
+            name="prim1", min_width=1.0, min_space=1.0, type_=_prm.nImpl,
         )
         prim1bis = _prm.Implant(
-            name="prim1", min_width=1.0, min_space=1.0, type_=_prm.nImplT,
+            name="prim1", min_width=1.0, min_space=1.0, type_=_prm.nImpl,
         )
         prim2 = _prm.Implant(
-            name="prim2", min_width=0.2, min_space=0.5, type_=_prm.pImplT,
+            name="prim2", min_width=0.2, min_space=0.5, type_=_prm.pImpl,
         )
 
         self.assertEqual(prim1, prim1bis)
         self.assertNotEqual(prim1, prim2)
 
         rules = tuple(prim1._generate_rules(tech=dummy_tech))
         self.assertIn(prim1.mask, rules)
@@ -151,62 +151,62 @@
 
     def test_well(self):
         with self.assertRaises(TypeError):
             _prm.Well(name="prim1", min_width=1.0, min_space=1.0)
         with self.assertRaises(ValueError):
             _prm.Well(
                 name="prim2", min_width=0.2, min_space=0.5, min_space_samenet=0.6,
-                type_=_prm.nImplT,
+                type_=_prm.nImpl,
             )
 
         prim1 = _prm.Well(
-            name="prim1", min_width=1.0, min_space=1.0, type_=_prm.nImplT,
+            name="prim1", min_width=1.0, min_space=1.0, type_=_prm.nImpl,
         )
         prim1bis = _prm.Well(
-            name="prim1", min_width=1.0, min_space=1.0, type_=_prm.nImplT,
+            name="prim1", min_width=1.0, min_space=1.0, type_=_prm.nImpl,
         )
         prim2 = _prm.Well(
             name="prim2", min_width=0.2, min_space=0.5, min_space_samenet=0.25,
-            type_=_prm.nImplT,
+            type_=_prm.nImpl,
         )
 
         self.assertEqual(prim1, prim1bis)
         self.assertNotEqual(prim1, prim2)
 
         rules = tuple(prim2._generate_rules(tech=dummy_tech))
         self.assertIn(prim2.mask, rules)
 
     def test_deepwell(self):
         with self.assertRaises(TypeError):
             _prm.DeepWell(name="prim1", min_width=1.0, min_space=1.0)
         with self.assertRaises(TypeError):
             _prm.DeepWell(
-                name="prim1", min_width=1.0, min_space=1.0, type_=_prm.pImplT,
+                name="prim1", min_width=1.0, min_space=1.0, type_=_prm.pImpl,
             )
 
         well1 = _prm.Well(
-            name="well1", min_width=1.0, min_space=1.0, type_=_prm.nImplT,
+            name="well1", min_width=1.0, min_space=1.0, type_=_prm.nImpl,
         )
         well2 = _prm.Well(
-            name="well2", min_width=1.0, min_space=1.0, type_=_prm.pImplT,
+            name="well2", min_width=1.0, min_space=1.0, type_=_prm.pImpl,
         )
 
         with self.assertRaises(ValueError):
             _prm.DeepWell(
                 name="typemismatch", min_width=1.0, min_space=1.0, well=well1,
-                type_=_prm.pImplT,
+                type_=_prm.pImpl,
                 min_well_overlap=1.5, min_well_enclosure=2.0,
             )
 
         prim1 = _prm.DeepWell(
-            name="prim1", min_width=1.0, min_space=1.0, well=well1, type_=_prm.nImplT,
+            name="prim1", min_width=1.0, min_space=1.0, well=well1, type_=_prm.nImpl,
             min_well_overlap=1.5, min_well_enclosure=2.0,
         )
         prim1bis = _prm.DeepWell(
-            name="prim1", min_width=1.0, min_space=1.0, well=well1, type_=_prm.nImplT,
+            name="prim1", min_width=1.0, min_space=1.0, well=well1, type_=_prm.nImpl,
             min_well_overlap=1.5, min_well_enclosure=2.0,
         )
         prim2 = _prm.DeepWell(
             name="prim2", min_width=0.2, min_space=0.5, well=well2,
             min_well_overlap=1.5, min_well_enclosure=2.0,
         )
 
@@ -214,25 +214,25 @@
         self.assertNotEqual(prim1, prim2)
 
         rules = tuple(prim2._generate_rules(tech=dummy_tech))
         self.assertIn(prim2.mask, rules)
 
     def test_waferwire(self):
         nimpl = _prm.Implant(
-            name="nimplant", min_width=1.0, min_space=1.0, type_=_prm.nImplT,
+            name="nimplant", min_width=1.0, min_space=1.0, type_=_prm.nImpl,
         )
         pimpl = _prm.Implant(
-            name="pimplant", min_width=1.0, min_space=1.0, type_=_prm.pImplT,
+            name="pimplant", min_width=1.0, min_space=1.0, type_=_prm.pImpl,
         )
         oxide = _prm.Insulator(name="oxide", min_width=1.0, min_space=1.0)
         well = _prm.Well(
-            name="well", min_width=1.0, min_space=1.0, type_=_prm.pImplT,
+            name="well", min_width=1.0, min_space=1.0, type_=_prm.pImpl,
         )
         well2 = _prm.Well(
-            name="well2", min_width=1.0, min_space=1.0, type_=_prm.nImplT,
+            name="well2", min_width=1.0, min_space=1.0, type_=_prm.nImpl,
         )
 
         with self.assertRaises(TypeError):
             _prm.WaferWire(name="prim1", min_width=1.0, min_space=1.0)
 
         with self.assertRaises(_prm.UnconnectedPrimitiveError):
             # Unconnected well
@@ -428,28 +428,28 @@
         rules = tuple(prim1._generate_rules(tech=dummy_tech))
         self.assertIn(prim1.mask, rules)
         rules = tuple(prim2._generate_rules(tech=dummy_tech))
         self.assertIn(prim2.mask, rules)
 
     def test_via(self):
         nimpl = _prm.Implant(
-            name="nimplant", min_width=0.5, min_space=0.5, type_=_prm.nImplT,
+            name="nimplant", min_width=0.5, min_space=0.5, type_=_prm.nImpl,
         )
         nimpl2 = _prm.Implant(
-            name="nimplant2", min_width=0.5, min_space=0.5, type_=_prm.nImplT,
+            name="nimplant2", min_width=0.5, min_space=0.5, type_=_prm.nImpl,
         )
         pimpl = _prm.Implant(
-            name="pimplant", min_width=0.5, min_space=0.5, type_=_prm.pImplT,
+            name="pimplant", min_width=0.5, min_space=0.5, type_=_prm.pImpl,
         )
         oxide = _prm.Insulator(name="oxide", min_width=1.0, min_space=1.0)
         well = _prm.Well(
-            name="well", min_width=1.0, min_space=1.0, type_=_prm.pImplT,
+            name="well", min_width=1.0, min_space=1.0, type_=_prm.pImpl,
         )
         well2 = _prm.Well(
-            name="well2", min_width=1.0, min_space=1.0, type_=_prm.nImplT,
+            name="well2", min_width=1.0, min_space=1.0, type_=_prm.nImpl,
         )
         active = _prm.WaferWire(
             name="aa", min_width=1.0, min_space=1.0,
             allow_in_substrate=True,
             implant=(nimpl, pimpl), min_implant_enclosure=_prp.Enclosure(0.05),
             implant_abut="all", allow_contactless_implant=False,
             well=well, min_well_enclosure=_prp.Enclosure(0.1),
@@ -510,15 +510,15 @@
                 return "MyTech"
             @property
             def grid(self):
                 return 0.005
 
             def __init__(self):
                 super().__init__(primitives=_prm.Primitives((
-                    _prm.Base(type_=_prm.pBaseT),
+                    _prm.Base(type_=_prm.pBase),
                     nimpl, pimpl, well, oxide, active, prim1, m1,
                 )))
         mytech = MyTech()
 
         rules = tuple(prim1._generate_rules(tech=mytech))
         self.assertIn(prim1.mask, rules)
 
@@ -569,24 +569,24 @@
         self.assertIn(prim1.mask, rules)
 
         # designmasks
         self.assertEqual(set(prim1.designmasks), {prim1.mask, m1.mask})
 
     def test_resistor(self):
         well = _prm.Well(
-            name="well", min_width=1.0, min_space=1.0, type_=_prm.pImplT,
+            name="well", min_width=1.0, min_space=1.0, type_=_prm.pImpl,
         )
         nimpl = _prm.Implant(
-            name="nimplant", min_width=0.5, min_space=0.5, type_=_prm.nImplT,
+            name="nimplant", min_width=0.5, min_space=0.5, type_=_prm.nImpl,
         )
         nimpl2 = _prm.Implant(
-            name="nimplant2", min_width=0.5, min_space=0.5, type_=_prm.nImplT,
+            name="nimplant2", min_width=0.5, min_space=0.5, type_=_prm.nImpl,
         )
         pimpl = _prm.Implant(
-            name="pimplant", min_width=0.5, min_space=0.5, type_=_prm.pImplT,
+            name="pimplant", min_width=0.5, min_space=0.5, type_=_prm.pImpl,
         )
         active = _prm.WaferWire(
             name="aa", min_width=1.0, min_space=1.0,
             allow_in_substrate=True,
             implant=(nimpl, pimpl), min_implant_enclosure=_prp.Enclosure(0.05),
             implant_abut="all", allow_contactless_implant=False,
             well=well, min_well_enclosure=_prp.Enclosure(0.1),
@@ -719,15 +719,15 @@
                 return "MyTech"
             @property
             def grid(self):
                 return 0.005
 
             def __init__(self):
                 super().__init__(primitives=_prm.Primitives((
-                    _prm.Base(type_=_prm.pBaseT),
+                    _prm.Base(type_=_prm.pBase),
                     well, nimpl, pimpl, active,
                     poly, polyres, prim1,
                     via, m1,
                 )))
         MyTech()
 
     def test_mimcapacitor(self): # Also include MIMTop
@@ -810,27 +810,27 @@
         rules = tuple(prim1._generate_rules(tech=dummy_tech))
         self.assertIn(prim1.mask, rules)
         rules = tuple(prim2._generate_rules(tech=dummy_tech))
         self.assertIn(prim2.mask, rules)
 
     def test_diode(self):
         nwell = _prm.Well(
-            name="nwell", min_width=1.0, min_space=1.0, type_=_prm.nImplT,
+            name="nwell", min_width=1.0, min_space=1.0, type_=_prm.nImpl,
         )
         pwell = _prm.Well(
-            name="pwell", min_width=1.0, min_space=1.0, type_=_prm.pImplT,
+            name="pwell", min_width=1.0, min_space=1.0, type_=_prm.pImpl,
         )
         nimpl = _prm.Implant(
-            name="nimplant", min_width=0.5, min_space=0.5, type_=_prm.nImplT,
+            name="nimplant", min_width=0.5, min_space=0.5, type_=_prm.nImpl,
         )
         nimpl2 = _prm.Implant(
-            name="nimplant2", min_width=0.5, min_space=0.5, type_=_prm.nImplT,
+            name="nimplant2", min_width=0.5, min_space=0.5, type_=_prm.nImpl,
         )
         pimpl = _prm.Implant(
-            name="pimplant", min_width=0.5, min_space=0.5, type_=_prm.pImplT,
+            name="pimplant", min_width=0.5, min_space=0.5, type_=_prm.pImpl,
         )
         active = _prm.WaferWire(
             name="aa", min_width=1.0, min_space=1.0,
             allow_in_substrate=True,
             implant=(nimpl, pimpl), min_implant_enclosure=_prp.Enclosure(0.05),
             implant_abut="all", allow_contactless_implant=False,
             well=pwell, min_well_enclosure=_prp.Enclosure(0.1),
@@ -934,30 +934,30 @@
         rules = tuple(prim1._generate_rules(tech=dummy_tech))
         self.assertIn(prim1.mask, rules)
         rules = tuple(prim2._generate_rules(tech=dummy_tech))
         self.assertIn(prim2.mask, rules)
 
     def test_mosfet(self): # also test MOSFETGate
         well = _prm.Well(
-            name="well", min_width=1.0, min_space=1.0, type_=_prm.pImplT,
+            name="well", min_width=1.0, min_space=1.0, type_=_prm.pImpl,
         )
         well2 = _prm.Well(
-            name="well2", min_width=1.0, min_space=1.0, type_=_prm.nImplT,
+            name="well2", min_width=1.0, min_space=1.0, type_=_prm.nImpl,
         )
         nimpl = _prm.Implant(
-            name="nimplant", min_width=1.0, min_space=1.0, type_=_prm.nImplT,
+            name="nimplant", min_width=1.0, min_space=1.0, type_=_prm.nImpl,
         )
         nimpl2 = _prm.Implant(
-            name="nimplant2", min_width=1.0, min_space=1.0, type_=_prm.nImplT,
+            name="nimplant2", min_width=1.0, min_space=1.0, type_=_prm.nImpl,
         )
         pimpl = _prm.Implant(
-            name="pimplant", min_width=1.0, min_space=1.0, type_=_prm.pImplT,
+            name="pimplant", min_width=1.0, min_space=1.0, type_=_prm.pImpl,
         )
         adjust = _prm.Implant(
-            name="nimplant", min_width=1.0, min_space=1.0, type_=_prm.adjImplT,
+            name="nimplant", min_width=1.0, min_space=1.0, type_=_prm.adjImpl,
         )
         oxide = _prm.Insulator(name="oxide", min_width=1.0, min_space=1.0)
         oxide2 = _prm.Insulator(name="oxide2", min_width=1.0, min_space=1.0)
         active = _prm.WaferWire(
             name="aa", min_width=1.0, min_space=1.0,
             allow_in_substrate=True,
             implant=(nimpl, pimpl, adjust), min_implant_enclosure=_prp.Enclosure(0.05),
@@ -1175,30 +1175,30 @@
         dummy_nmos = dummy_prims.nmos
         dummy_pmos = dummy_prims.pmos
         self.assertIn(dummy_mosgate.mask, dummy_mosgate.rules)
         self.assertNotIn(dummy_mosgate.mask, dummy_nmos.rules)
         self.assertNotIn(dummy_mosgate.mask, dummy_pmos.rules)
 
     def test_bipolartype(self):
-        self.assertEqual(_prm.npnBipolarT, _prm.npnBipolarT)
-        self.assertNotEqual(_prm.npnBipolarT, _prm.pnpBipolarT)
+        self.assertEqual(_prm.npnBipolar, _prm.npnBipolar)
+        self.assertNotEqual(_prm.npnBipolar, _prm.pnpBipolar)
 
-        self.assertEqual(hash(_prm.npnBipolarT), hash(_prm.npnBipolarT))
-        self.assertNotEqual(hash(_prm.npnBipolarT), hash(_prm.pnpBipolarT))
+        self.assertEqual(hash(_prm.npnBipolar), hash(_prm.npnBipolar))
+        self.assertNotEqual(hash(_prm.npnBipolar), hash(_prm.pnpBipolar))
 
         with self.assertWarns(UserWarning):
-            _prm.npnBipolarT == "npn"
+            _prm.npnBipolar == "npn"
 
     def test_bipolar(self):
         npn = _prm.Marker(name="npn")
         pnp = _prm.Marker(name="pnp")
 
-        prim1 = _prm.Bipolar(name="prim1", type_=_prm.npnBipolarT, indicator=npn)
-        prim1bis = _prm.Bipolar(name="prim1", type_=_prm.npnBipolarT, indicator=npn)
-        prim2 = _prm.Bipolar(name="prim2", type_=_prm.pnpBipolarT, indicator=pnp)
+        prim1 = _prm.Bipolar(name="prim1", type_=_prm.npnBipolar, indicator=npn)
+        prim1bis = _prm.Bipolar(name="prim1", type_=_prm.npnBipolar, indicator=npn)
+        prim2 = _prm.Bipolar(name="prim2", type_=_prm.pnpBipolar, indicator=pnp)
 
         self.assertEqual(prim1, prim1bis)
         self.assertNotEqual(prim1, prim2)
 
         tuple(prim1._generate_rules(tech=dummy_tech))
         tuple(prim2._generate_rules(tech=dummy_tech))
```

### Comparing `PDKMaster-0.9.0/test/unit/technology/property.py` & `PDKMaster-0.9.1/test/unit/technology/property.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/technology/rule.py` & `PDKMaster-0.9.1/test/unit/technology/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/technology/technology.py` & `PDKMaster-0.9.1/test/unit/technology/technology.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,45 +140,45 @@
                 return "MyTech"
             @property
             def grid(self) -> float:
                 return 2.5e-3
 
             def __init__(self):
                 super().__init__(primitives=_prm.Primitives(
-                    _prm.Base(type_=_prm.pBaseT),
+                    _prm.Base(type_=_prm.pBase),
                 ))
         mytech = MyTech()
         self.assertAlmostEqual(mytech.dbu, 1e-4, delta=_geo.epsilon)
 
         class MyTech(_tch.Technology):
             @property
             def name(self) -> str:
                 return "MyTech"
             @property
             def grid(self) -> float:
                 return 1.25e-3
 
             def __init__(self):
                 super().__init__(primitives=_prm.Primitives(
-                    _prm.Base(type_=_prm.pBaseT),
+                    _prm.Base(type_=_prm.pBase),
                 ))
         mytech = MyTech()
         self.assertAlmostEqual(mytech.dbu, 1e-5, delta=_geo.epsilon)
 
     def test_padopening(self):
         class MyTech(_tch.Technology):
             @property
             def name(self) -> str:
                 return "MyTech"
             @property
             def grid(self) -> float:
                 return 5e-3
 
             def __init__(self):
-                prims = _prm.Primitives(_prm.Base(type_=_prm.pBaseT))
+                prims = _prm.Primitives(_prm.Base(type_=_prm.pBase))
 
                 metal1 = _prm.MetalWire(name="metal1", min_width=1.0, min_space=1.0)
                 pad = _prm.PadOpening(
                     name="pad", min_width=20.0, min_space=3.0,
                     bottom=metal1, min_bottom_enclosure=2.0,
                 )
                 prims += (metal1, pad)
@@ -193,18 +193,18 @@
             def name(self) -> str:
                 return "MyTech"
             @property
             def grid(self) -> float:
                 return 2.5e-3
 
             def __init__(self):
-                prims = _prm.Primitives(_prm.Base(type_=_prm.pBaseT))
+                prims = _prm.Primitives(_prm.Base(type_=_prm.pBase))
 
                 prims += _prm.Well(
-                    name="well", min_width=5.0, min_space=3.0, type_=_prm.nImplT,
+                    name="well", min_width=5.0, min_space=3.0, type_=_prm.nImpl,
                 )
 
                 super().__init__(primitives=prims)
         with self.assertRaises(_prm.UnconnectedPrimitiveError):
             MyTech()
 
         class MyTech(_tch.Technology):
@@ -212,15 +212,15 @@
             def name(self) -> str:
                 return "MyTech"
             @property
             def grid(self) -> float:
                 return 5e-3
 
             def __init__(self):
-                prims = _prm.Primitives(_prm.Base(type_=_prm.pBaseT))
+                prims = _prm.Primitives(_prm.Base(type_=_prm.pBase))
 
                 metal1 = _prm.MetalWire(name="metal1", min_width=1.0, min_space=1.0)
                 prims += metal1
 
                 super().__init__(primitives=prims)
         with self.assertRaises(_prm.UnusedPrimitiveError):
             MyTech()
@@ -230,24 +230,24 @@
             def name(self) -> str:
                 return "MyTech"
             @property
             def grid(self) -> float:
                 return 5e-3
 
             def __init__(self):
-                prims = _prm.Primitives(_prm.Base(type_=_prm.pBaseT))
+                prims = _prm.Primitives(_prm.Base(type_=_prm.pBase))
 
                 nimpl = _prm.Implant(
-                    name="nimplant", min_width=1.2, min_space=1.2, type_=_prm.nImplT,
+                    name="nimplant", min_width=1.2, min_space=1.2, type_=_prm.nImpl,
                 )
                 pimpl = _prm.Implant(
-                    name="pimplant", min_width=1.2, min_space=1.2, type_=_prm.pImplT,
+                    name="pimplant", min_width=1.2, min_space=1.2, type_=_prm.pImpl,
                 )
                 nwell = _prm.Well(
-                    name="nwell", min_width=5.0, min_space=3.0, type_=_prm.nImplT,
+                    name="nwell", min_width=5.0, min_space=3.0, type_=_prm.nImpl,
                 )
                 prims += (nimpl, pimpl, nwell)
 
                 active = _prm.WaferWire(
                     name="active", min_width=0.8, min_space=0.8,
                     implant=(nimpl, pimpl), min_implant_enclosure=_prp.Enclosure(0.2),
                     implant_abut="all", allow_contactless_implant=False,
@@ -272,24 +272,24 @@
             def name(self) -> str:
                 return "MyTech"
             @property
             def grid(self) -> float:
                 return 5e-3
 
             def __init__(self):
-                prims = _prm.Primitives(_prm.Base(type_=_prm.pBaseT))
+                prims = _prm.Primitives(_prm.Base(type_=_prm.pBase))
 
                 nimpl = _prm.Implant(
-                    name="nimplant", min_width=1.2, min_space=1.2, type_=_prm.nImplT,
+                    name="nimplant", min_width=1.2, min_space=1.2, type_=_prm.nImpl,
                 )
                 pimpl = _prm.Implant(
-                    name="pimplant", min_width=1.2, min_space=1.2, type_=_prm.pImplT,
+                    name="pimplant", min_width=1.2, min_space=1.2, type_=_prm.pImpl,
                 )
                 nwell = _prm.Well(
-                    name="nwell", min_width=5.0, min_space=3.0, type_=_prm.nImplT,
+                    name="nwell", min_width=5.0, min_space=3.0, type_=_prm.nImpl,
                 )
                 prims += (nimpl, pimpl, nwell)
 
                 active = _prm.WaferWire(
                     name="active", min_width=0.8, min_space=0.8,
                     implant=(nimpl, pimpl), min_implant_enclosure=_prp.Enclosure(0.2),
                     implant_abut="all", allow_contactless_implant=False,
@@ -325,15 +325,15 @@
             def name(self) -> str:
                 return "MyTech"
             @property
             def grid(self) -> float:
                 return 5e-3
 
             def __init__(self):
-                prims = _prm.Primitives(_prm.Base(type_=_prm.pBaseT))
+                prims = _prm.Primitives(_prm.Base(type_=_prm.pBase))
 
                 metal1 = _prm.MetalWire(name="metal1", min_width=1.0, min_space=1.0)
                 metal2 = _prm.MetalWire(name="metal1", min_width=1.0, min_space=1.0)
                 via = _prm.Via(
                     name="via", width=0.8, min_space=0.8,
                     bottom=metal1, min_bottom_enclosure=_prp.Enclosure(0.2),
                     top=metal2, min_top_enclosure=_prp.Enclosure(0.2),
@@ -350,15 +350,15 @@
                 return "MyTech"
             @property
             def grid(self) -> float:
                 return 5e-3
 
             def __init__(self):
                 super().__init__(primitives=_prm.Primitives((
-                    _prm.Base(type_=_prm.pBaseT),
+                    _prm.Base(type_=_prm.pBase),
                     _prm.MIMTop(name="error", min_width=1.0, min_space=1.0),
                 )))
         with self.assertRaises(_prm.UnusedPrimitiveError):
             MyTech()
 
         class MyTech(_tch.Technology):
             @property
```

### Comparing `PDKMaster-0.9.0/test/unit/technology/wafer.py` & `PDKMaster-0.9.1/test/unit/technology/wafer.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test/unit/typing.py` & `PDKMaster-0.9.1/test/unit/typing.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.0/test.tf` & `PDKMaster-0.9.1/test.tf`

 * *Files identical despite different names*

