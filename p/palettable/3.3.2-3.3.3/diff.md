# Comparing `tmp/palettable-3.3.2.tar.gz` & `tmp/palettable-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palettable-3.3.2.tar", last modified: Sun Apr 16 20:31:10 2023, max compression
+gzip compressed data, was "palettable-3.3.3.tar", last modified: Wed Apr 19 23:12:43 2023, max compression
```

## Comparing `palettable-3.3.2.tar` & `palettable-3.3.3.tar`

### file list

```diff
@@ -1,71 +1,78 @@
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.729449 palettable-3.3.2/
--rw-r--r--   0 jiffyclub   (501) staff       (20)       59 2018-05-14 14:49:57.000000 palettable-3.3.2/MANIFEST.in
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1941 2023-04-16 20:31:10.729606 palettable-3.3.2/PKG-INFO
--rw-r--r--   0 jiffyclub   (501) staff       (20)      985 2015-07-11 16:45:18.000000 palettable-3.3.2/README.rst
--rw-r--r--   0 jiffyclub   (501) staff       (20)    10476 2014-09-11 18:21:02.000000 palettable-3.3.2/ez_setup.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1065 2019-07-11 23:03:53.000000 palettable-3.3.2/license.txt
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.687970 palettable-3.3.2/palettable/
--rw-r--r--   0 jiffyclub   (501) staff       (20)      481 2023-04-16 20:30:46.000000 palettable-3.3.2/palettable/__init__.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.694967 palettable-3.3.2/palettable/cartocolors/
--rw-r--r--   0 jiffyclub   (501) staff       (20)       89 2017-09-02 05:18:58.000000 palettable-3.3.2/palettable/cartocolors/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      932 2017-09-02 05:18:58.000000 palettable-3.3.2/palettable/cartocolors/cartocolorspalette.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     6104 2017-09-02 05:18:58.000000 palettable-3.3.2/palettable/cartocolors/colormaps.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1049 2017-09-02 05:18:58.000000 palettable-3.3.2/palettable/cartocolors/diverging.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1276 2017-09-02 05:18:58.000000 palettable-3.3.2/palettable/cartocolors/qualitative.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1410 2019-09-07 23:30:52.000000 palettable-3.3.2/palettable/cartocolors/sequential.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.701268 palettable-3.3.2/palettable/cmocean/
--rw-r--r--   0 jiffyclub   (501) staff       (20)       76 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/cmocean/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      884 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/cmocean/cmoceanpalette.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)   101253 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/cmocean/colormaps.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      817 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/cmocean/diverging.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1130 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/cmocean/sequential.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.706827 palettable-3.3.2/palettable/colorbrewer/
--rw-r--r--   0 jiffyclub   (501) staff       (20)      116 2015-03-04 06:18:35.000000 palettable-3.3.2/palettable/colorbrewer/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     6309 2023-04-06 03:47:14.000000 palettable-3.3.2/palettable/colorbrewer/colorbrewer.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)    99495 2023-04-06 03:47:14.000000 palettable-3.3.2/palettable/colorbrewer/colorbrewer_all_schemes.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.709638 palettable-3.3.2/palettable/colorbrewer/data/
--rw-r--r--   0 jiffyclub   (501) staff       (20)    37224 2015-03-04 06:18:35.000000 palettable-3.3.2/palettable/colorbrewer/data/colorbrewer_all_schemes.csv
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1712 2015-03-04 06:18:35.000000 palettable-3.3.2/palettable/colorbrewer/data/colorbrewer_licence.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)      135 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/colorbrewer/diverging.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      137 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/colorbrewer/qualitative.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      136 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/colorbrewer/sequential.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.711512 palettable-3.3.2/palettable/cubehelix/
--rw-r--r--   0 jiffyclub   (501) staff       (20)      153 2015-05-01 04:35:16.000000 palettable-3.3.2/palettable/cubehelix/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)    13383 2015-05-01 04:35:16.000000 palettable-3.3.2/palettable/cubehelix/cubehelix.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.715813 palettable-3.3.2/palettable/lightbartlein/
--rw-r--r--   0 jiffyclub   (501) staff       (20)       76 2019-07-11 22:44:07.000000 palettable-3.3.2/palettable/lightbartlein/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     4398 2019-07-11 22:44:07.000000 palettable-3.3.2/palettable/lightbartlein/colordata.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     2181 2019-07-11 22:44:07.000000 palettable-3.3.2/palettable/lightbartlein/diverging.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      998 2019-07-11 22:44:07.000000 palettable-3.3.2/palettable/lightbartlein/lightbartlein.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1194 2019-07-11 22:44:07.000000 palettable-3.3.2/palettable/lightbartlein/sequential.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.718069 palettable-3.3.2/palettable/matplotlib/
--rw-r--r--   0 jiffyclub   (501) staff       (20)      207 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/matplotlib/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)    33280 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/matplotlib/colormaps.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1548 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/matplotlib/matplotlib.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.720223 palettable-3.3.2/palettable/mycarta/
--rw-r--r--   0 jiffyclub   (501) staff       (20)      204 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/mycarta/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)    15123 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/mycarta/colordata.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1491 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/mycarta/mycarta.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     7200 2017-09-02 05:18:58.000000 palettable-3.3.2/palettable/palette.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.724099 palettable-3.3.2/palettable/scientific/
--rw-r--r--   0 jiffyclub   (501) staff       (20)       76 2019-09-07 23:30:52.000000 palettable-3.3.2/palettable/scientific/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)   122443 2019-09-07 23:30:52.000000 palettable-3.3.2/palettable/scientific/colordata.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      799 2019-09-07 23:30:52.000000 palettable-3.3.2/palettable/scientific/diverging.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      888 2019-09-07 23:30:52.000000 palettable-3.3.2/palettable/scientific/scientific.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      907 2019-09-07 23:30:52.000000 palettable-3.3.2/palettable/scientific/sequential.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.725412 palettable-3.3.2/palettable/tableau/
--rw-r--r--   0 jiffyclub   (501) staff       (20)      140 2015-03-04 06:18:35.000000 palettable-3.3.2/palettable/tableau/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     5921 2015-03-04 06:18:35.000000 palettable-3.3.2/palettable/tableau/tableau.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     7124 2017-09-02 05:18:58.000000 palettable-3.3.2/palettable/utils.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.726869 palettable-3.3.2/palettable/wesanderson/
--rw-r--r--   0 jiffyclub   (501) staff       (20)      156 2017-02-20 23:03:00.000000 palettable-3.3.2/palettable/wesanderson/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)    12587 2019-09-07 18:37:56.000000 palettable-3.3.2/palettable/wesanderson/wesanderson.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.689971 palettable-3.3.2/palettable.egg-info/
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1941 2023-04-16 20:31:10.000000 palettable-3.3.2/palettable.egg-info/PKG-INFO
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1792 2023-04-16 20:31:10.000000 palettable-3.3.2/palettable.egg-info/SOURCES.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)        1 2023-04-16 20:31:10.000000 palettable-3.3.2/palettable.egg-info/dependency_links.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)       11 2023-04-16 20:31:10.000000 palettable-3.3.2/palettable.egg-info/top_level.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)       67 2023-04-16 20:31:10.730142 palettable-3.3.2/setup.cfg
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1256 2023-04-16 20:30:40.000000 palettable-3.3.2/setup.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-16 20:31:10.728820 palettable-3.3.2/test/
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1154 2017-09-02 05:18:58.000000 palettable-3.3.2/test/test_installed.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.350567 palettable-3.3.3/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       39 2023-04-17 00:20:22.000000 palettable-3.3.3/MANIFEST.in
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     3268 2023-04-19 23:12:43.351044 palettable-3.3.3/PKG-INFO
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1183 2023-04-16 23:15:50.000000 palettable-3.3.3/README.rst
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.266315 palettable-3.3.3/docs/
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.274837 palettable-3.3.3/docs/_python/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       29 2015-03-04 06:18:35.000000 palettable-3.3.3/docs/_python/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      125 2015-03-04 06:18:35.000000 palettable-3.3.3/docs/_python/filters.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     3536 2019-09-07 23:30:52.000000 palettable-3.3.3/docs/gendocs.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1065 2019-07-11 23:03:53.000000 palettable-3.3.3/license.txt
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.281336 palettable-3.3.3/palettable/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      491 2023-04-19 23:12:15.000000 palettable-3.3.3/palettable/__init__.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.313153 palettable-3.3.3/palettable/cartocolors/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       89 2017-09-02 05:18:58.000000 palettable-3.3.3/palettable/cartocolors/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      932 2017-09-02 05:18:58.000000 palettable-3.3.3/palettable/cartocolors/cartocolorspalette.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     6104 2017-09-02 05:18:58.000000 palettable-3.3.3/palettable/cartocolors/colormaps.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1049 2017-09-02 05:18:58.000000 palettable-3.3.3/palettable/cartocolors/diverging.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1276 2017-09-02 05:18:58.000000 palettable-3.3.3/palettable/cartocolors/qualitative.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1410 2019-09-07 23:30:52.000000 palettable-3.3.3/palettable/cartocolors/sequential.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.318109 palettable-3.3.3/palettable/cmocean/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       76 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/cmocean/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      884 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/cmocean/cmoceanpalette.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)   101253 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/cmocean/colormaps.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      817 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/cmocean/diverging.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1130 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/cmocean/sequential.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.324146 palettable-3.3.3/palettable/colorbrewer/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      116 2015-03-04 06:18:35.000000 palettable-3.3.3/palettable/colorbrewer/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     6309 2023-04-06 03:47:14.000000 palettable-3.3.3/palettable/colorbrewer/colorbrewer.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    99495 2023-04-06 03:47:14.000000 palettable-3.3.3/palettable/colorbrewer/colorbrewer_all_schemes.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.327321 palettable-3.3.3/palettable/colorbrewer/data/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    37224 2015-03-04 06:18:35.000000 palettable-3.3.3/palettable/colorbrewer/data/colorbrewer_all_schemes.csv
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1712 2015-03-04 06:18:35.000000 palettable-3.3.3/palettable/colorbrewer/data/colorbrewer_licence.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     2087 2023-04-06 03:47:14.000000 palettable-3.3.3/palettable/colorbrewer/data/colorbrewer_schemes_csv_to_py.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      135 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/colorbrewer/diverging.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      137 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/colorbrewer/qualitative.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      136 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/colorbrewer/sequential.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.328789 palettable-3.3.3/palettable/cubehelix/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      153 2015-05-01 04:35:16.000000 palettable-3.3.3/palettable/cubehelix/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    13383 2015-05-01 04:35:16.000000 palettable-3.3.3/palettable/cubehelix/cubehelix.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.332691 palettable-3.3.3/palettable/lightbartlein/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       76 2019-07-11 22:44:07.000000 palettable-3.3.3/palettable/lightbartlein/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     4398 2019-07-11 22:44:07.000000 palettable-3.3.3/palettable/lightbartlein/colordata.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     2181 2019-07-11 22:44:07.000000 palettable-3.3.3/palettable/lightbartlein/diverging.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      998 2019-07-11 22:44:07.000000 palettable-3.3.3/palettable/lightbartlein/lightbartlein.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1194 2019-07-11 22:44:07.000000 palettable-3.3.3/palettable/lightbartlein/sequential.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.337678 palettable-3.3.3/palettable/matplotlib/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      207 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/matplotlib/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    33280 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/matplotlib/colormaps.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1548 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/matplotlib/matplotlib.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.340092 palettable-3.3.3/palettable/mycarta/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      204 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/mycarta/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    15123 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/mycarta/colordata.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1491 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/mycarta/mycarta.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     7200 2017-09-02 05:18:58.000000 palettable-3.3.3/palettable/palette.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.345470 palettable-3.3.3/palettable/scientific/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       76 2019-09-07 23:30:52.000000 palettable-3.3.3/palettable/scientific/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)   122443 2019-09-07 23:30:52.000000 palettable-3.3.3/palettable/scientific/colordata.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      799 2019-09-07 23:30:52.000000 palettable-3.3.3/palettable/scientific/diverging.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      888 2019-09-07 23:30:52.000000 palettable-3.3.3/palettable/scientific/scientific.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      907 2019-09-07 23:30:52.000000 palettable-3.3.3/palettable/scientific/sequential.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.346773 palettable-3.3.3/palettable/tableau/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      140 2015-03-04 06:18:35.000000 palettable-3.3.3/palettable/tableau/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     5921 2015-03-04 06:18:35.000000 palettable-3.3.3/palettable/tableau/tableau.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     7124 2017-09-02 05:18:58.000000 palettable-3.3.3/palettable/utils.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.348268 palettable-3.3.3/palettable/wesanderson/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      156 2017-02-20 23:03:00.000000 palettable-3.3.3/palettable/wesanderson/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    12587 2019-09-07 18:37:56.000000 palettable-3.3.3/palettable/wesanderson/wesanderson.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.284681 palettable-3.3.3/palettable.egg-info/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     3268 2023-04-19 23:12:43.000000 palettable-3.3.3/palettable.egg-info/PKG-INFO
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1934 2023-04-19 23:12:43.000000 palettable-3.3.3/palettable.egg-info/SOURCES.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)        1 2023-04-19 23:12:43.000000 palettable-3.3.3/palettable.egg-info/dependency_links.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       45 2023-04-19 23:12:43.000000 palettable-3.3.3/palettable.egg-info/top_level.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1087 2023-04-17 00:20:22.000000 palettable-3.3.3/pyproject.toml
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.348937 palettable-3.3.3/scripts/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1169 2019-09-07 23:30:52.000000 palettable-3.3.3/scripts/scientific.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       67 2023-04-19 23:12:43.352254 palettable-3.3.3/setup.cfg
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-19 23:12:43.349658 palettable-3.3.3/test/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1154 2017-09-02 05:18:58.000000 palettable-3.3.3/test/test_installed.py
```

### Comparing `palettable-3.3.2/README.rst` & `palettable-3.3.3/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Palettable
 ==========
 
-.. image:: https://travis-ci.org/jiffyclub/palettable.png?branch=master
-   :alt: Travis-CI
-   :target: https://travis-ci.org/jiffyclub/palettable
+.. image:: https://github.com/jiffyclub/palettable/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/jiffyclub/palettable/actions/workflows/ci.yml
+   :alt: Build Status
 
-.. image:: https://coveralls.io/repos/jiffyclub/palettable/badge.png
-   :alt: Coveralls
+.. image:: https://coveralls.io/repos/jiffyclub/palettable/badge.svg
    :target: https://coveralls.io/r/jiffyclub/palettable
+   :alt: Coveralls
 
 .. image:: https://img.shields.io/pypi/v/palettable.svg
-   :alt: PyPI
    :target: https://pypi.python.org/pypi/palettable/
+   :alt: Latest Version
+
+.. image:: https://img.shields.io/pypi/pyversions/snakeviz.svg
+   :target: https://pypi.python.org/pypi/snakeviz/
+   :alt: Supported Python versions
 
-.. image::  https://img.shields.io/pypi/wheel/palettable.svg
+.. image:: https://img.shields.io/pypi/wheel/palettable.svg
     :target: https://pypi.python.org/pypi/palettable/
     :alt: Wheel Status
 
 Color Palettes for Python
 -------------------------
 
 Palettable (formerly brewer2mpl) is a library of color palettes for Python.
```

### Comparing `palettable-3.3.2/license.txt` & `palettable-3.3.3/license.txt`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/cartocolors/cartocolorspalette.py` & `palettable-3.3.3/palettable/cartocolors/cartocolorspalette.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/cartocolors/colormaps.py` & `palettable-3.3.3/palettable/cartocolors/colormaps.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/cartocolors/diverging.py` & `palettable-3.3.3/palettable/cartocolors/diverging.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/cartocolors/qualitative.py` & `palettable-3.3.3/palettable/cartocolors/qualitative.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/cartocolors/sequential.py` & `palettable-3.3.3/palettable/cartocolors/sequential.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/cmocean/cmoceanpalette.py` & `palettable-3.3.3/palettable/cmocean/cmoceanpalette.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/cmocean/colormaps.py` & `palettable-3.3.3/palettable/cmocean/colormaps.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/cmocean/diverging.py` & `palettable-3.3.3/palettable/cmocean/diverging.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/cmocean/sequential.py` & `palettable-3.3.3/palettable/cmocean/sequential.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/colorbrewer/colorbrewer.py` & `palettable-3.3.3/palettable/colorbrewer/colorbrewer.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/colorbrewer/colorbrewer_all_schemes.py` & `palettable-3.3.3/palettable/colorbrewer/colorbrewer_all_schemes.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/colorbrewer/data/colorbrewer_all_schemes.csv` & `palettable-3.3.3/palettable/colorbrewer/data/colorbrewer_all_schemes.csv`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/colorbrewer/data/colorbrewer_licence.txt` & `palettable-3.3.3/palettable/colorbrewer/data/colorbrewer_licence.txt`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/cubehelix/cubehelix.py` & `palettable-3.3.3/palettable/cubehelix/cubehelix.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/lightbartlein/colordata.py` & `palettable-3.3.3/palettable/lightbartlein/colordata.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/lightbartlein/diverging.py` & `palettable-3.3.3/palettable/lightbartlein/diverging.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/lightbartlein/lightbartlein.py` & `palettable-3.3.3/palettable/lightbartlein/lightbartlein.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/lightbartlein/sequential.py` & `palettable-3.3.3/palettable/lightbartlein/sequential.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/matplotlib/colormaps.py` & `palettable-3.3.3/palettable/matplotlib/colormaps.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/matplotlib/matplotlib.py` & `palettable-3.3.3/palettable/matplotlib/matplotlib.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/mycarta/colordata.py` & `palettable-3.3.3/palettable/mycarta/colordata.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/mycarta/mycarta.py` & `palettable-3.3.3/palettable/mycarta/mycarta.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/palette.py` & `palettable-3.3.3/palettable/palette.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/scientific/colordata.py` & `palettable-3.3.3/palettable/scientific/colordata.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/scientific/diverging.py` & `palettable-3.3.3/palettable/scientific/diverging.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/scientific/scientific.py` & `palettable-3.3.3/palettable/scientific/scientific.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/scientific/sequential.py` & `palettable-3.3.3/palettable/scientific/sequential.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/tableau/tableau.py` & `palettable-3.3.3/palettable/tableau/tableau.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/utils.py` & `palettable-3.3.3/palettable/utils.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable/wesanderson/wesanderson.py` & `palettable-3.3.3/palettable/wesanderson/wesanderson.py`

 * *Files identical despite different names*

### Comparing `palettable-3.3.2/palettable.egg-info/SOURCES.txt` & `palettable-3.3.3/palettable.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 MANIFEST.in
 README.rst
-ez_setup.py
 license.txt
+pyproject.toml
 setup.cfg
-setup.py
+docs/gendocs.py
+docs/_python/__init__.py
+docs/_python/filters.py
 palettable/__init__.py
 palettable/palette.py
 palettable/utils.py
 palettable.egg-info/PKG-INFO
 palettable.egg-info/SOURCES.txt
 palettable.egg-info/dependency_links.txt
 palettable.egg-info/top_level.txt
@@ -26,14 +28,15 @@
 palettable/colorbrewer/colorbrewer.py
 palettable/colorbrewer/colorbrewer_all_schemes.py
 palettable/colorbrewer/diverging.py
 palettable/colorbrewer/qualitative.py
 palettable/colorbrewer/sequential.py
 palettable/colorbrewer/data/colorbrewer_all_schemes.csv
 palettable/colorbrewer/data/colorbrewer_licence.txt
+palettable/colorbrewer/data/colorbrewer_schemes_csv_to_py.py
 palettable/cubehelix/__init__.py
 palettable/cubehelix/cubehelix.py
 palettable/lightbartlein/__init__.py
 palettable/lightbartlein/colordata.py
 palettable/lightbartlein/diverging.py
 palettable/lightbartlein/lightbartlein.py
 palettable/lightbartlein/sequential.py
@@ -48,8 +51,9 @@
 palettable/scientific/diverging.py
 palettable/scientific/scientific.py
 palettable/scientific/sequential.py
 palettable/tableau/__init__.py
 palettable/tableau/tableau.py
 palettable/wesanderson/__init__.py
 palettable/wesanderson/wesanderson.py
+scripts/scientific.py
 test/test_installed.py
```

### Comparing `palettable-3.3.2/test/test_installed.py` & `palettable-3.3.3/test/test_installed.py`

 * *Files identical despite different names*

