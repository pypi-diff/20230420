# Comparing `tmp/recfast4py-0.2.7.tar.gz` & `tmp/recfast4py-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recfast4py-0.2.7.tar", last modified: Tue Apr 18 15:53:42 2023, max compression
+gzip compressed data, was "recfast4py-0.2.8.tar", last modified: Thu Apr 20 09:40:47 2023, max compression
```

## Comparing `recfast4py-0.2.7.tar` & `recfast4py-0.2.8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 15:53:42.849764 recfast4py-0.2.7/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      164 2017-09-08 11:49:33.000000 recfast4py-0.2.7/AUTHORS.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1569 2017-03-14 15:09:27.000000 recfast4py-0.2.7/CONTRIBUTING.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      314 2017-09-08 11:49:02.000000 recfast4py-0.2.7/HISTORY.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      514 2017-03-14 14:20:31.000000 recfast4py-0.2.7/LICENSE
--rw-r--r--   0 uweschmitt   (501) staff       (20)      246 2023-04-18 14:09:48.000000 recfast4py-0.2.7/MANIFEST.in
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1683 2023-04-18 14:57:39.000000 recfast4py-0.2.7/Makefile
--rw-r--r--   0 uweschmitt   (501) staff       (20)      893 2023-04-18 15:53:42.849594 recfast4py-0.2.7/PKG-INFO
--rw-r--r--   0 uweschmitt   (501) staff       (20)      101 2023-04-18 14:56:34.000000 recfast4py-0.2.7/README.rst
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 15:53:42.842499 recfast4py-0.2.7/docs/
--rw-r--r--   0 uweschmitt   (501) staff       (20)        9 2017-03-14 15:09:54.000000 recfast4py-0.2.7/docs/.gitignore
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6777 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/Makefile
--rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/authors.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      515 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/check_sphinx.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8562 2019-05-09 14:45:36.000000 recfast4py-0.2.7/docs/conf.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)       32 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/contributing.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/history.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      607 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/index.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      230 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/installation.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6466 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/make.bat
--rw-r--r--   0 uweschmitt   (501) staff       (20)       67 2017-03-28 12:31:43.000000 recfast4py-0.2.7/docs/modules.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      481 2017-03-28 12:31:43.000000 recfast4py-0.2.7/docs/recfast4py.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      395 2017-03-14 14:59:53.000000 recfast4py-0.2.7/docs/usage.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2013 2023-04-18 15:53:35.000000 recfast4py-0.2.7/pyproject.toml
--rw-r--r--   0 uweschmitt   (501) staff       (20)       38 2023-04-18 15:53:42.849803 recfast4py-0.2.7/setup.cfg
--rw-r--r--   0 uweschmitt   (501) staff       (20)      734 2023-04-18 15:46:42.000000 recfast4py-0.2.7/setup.py
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 15:53:42.838029 recfast4py-0.2.7/src/
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 15:53:42.848060 recfast4py-0.2.7/src/recfast4py/
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3175 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/DM_annihilation.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1036 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/DM_annihilation.Recfast.h
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)    42560 2021-04-16 07:26:49.000000 recfast4py-0.2.7/src/recfast4py/ODE_solver.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2955 2020-02-13 17:11:51.000000 recfast4py-0.2.7/src/recfast4py/ODE_solver.Recfast.h
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3902 2018-04-10 15:58:01.000000 recfast4py-0.2.7/src/recfast4py/Rec_corrs_CT.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1278 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/Rec_corrs_CT.Recfast.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)      181 2023-04-18 14:51:17.000000 recfast4py-0.2.7/src/recfast4py/__init__.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)   242951 2023-04-18 15:43:50.000000 recfast4py-0.2.7/src/recfast4py/_recfast.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)   243408 2023-04-18 15:53:42.000000 recfast4py-0.2.7/src/recfast4py/_recfast.cpp
--rw-r--r--   0 uweschmitt   (501) staff       (20)      789 2023-04-18 15:53:42.000000 recfast4py-0.2.7/src/recfast4py/_recfast.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1738 2023-04-18 14:44:23.000000 recfast4py-0.2.7/src/recfast4py/_recfast.pyx
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     6675 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/constants.Recfast.h
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2485 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/cosmology.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1974 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/cosmology.Recfast.h
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 15:53:42.848970 recfast4py-0.2.7/src/recfast4py/data/
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)    23196 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/data/DXe_Xe.CT2010.dat
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     8479 2021-04-16 07:26:49.000000 recfast4py-0.2.7/src/recfast4py/evalode.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1627 2017-03-14 14:18:01.000000 recfast4py-0.2.7/src/recfast4py/evalode.Recfast.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1056 2023-04-18 14:44:01.000000 recfast4py-0.2.7/src/recfast4py/recfast.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)      200 2023-04-18 14:51:44.000000 recfast4py-0.2.7/src/recfast4py/recfast4py.py
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)    15164 2020-02-13 17:11:51.000000 recfast4py-0.2.7/src/recfast4py/recombination.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2256 2019-05-09 11:00:46.000000 recfast4py-0.2.7/src/recfast4py/recombination.Recfast.h
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 15:53:42.848830 recfast4py-0.2.7/src/recfast4py.egg-info/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      893 2023-04-18 15:53:42.000000 recfast4py-0.2.7/src/recfast4py.egg-info/PKG-INFO
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1260 2023-04-18 15:53:42.000000 recfast4py-0.2.7/src/recfast4py.egg-info/SOURCES.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2023-04-18 15:53:42.000000 recfast4py-0.2.7/src/recfast4py.egg-info/dependency_links.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)      184 2023-04-18 15:53:42.000000 recfast4py-0.2.7/src/recfast4py.egg-info/requires.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)       11 2023-04-18 15:53:42.000000 recfast4py-0.2.7/src/recfast4py.egg-info/top_level.txt
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-18 15:53:42.849274 recfast4py-0.2.7/tests/
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1114 2023-04-18 14:51:35.000000 recfast4py-0.2.7/tests/test_recfast4py.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:40:47.538301 recfast4py-0.2.8/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      164 2017-09-08 11:49:33.000000 recfast4py-0.2.8/AUTHORS.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1569 2017-03-14 15:09:27.000000 recfast4py-0.2.8/CONTRIBUTING.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      314 2017-09-08 11:49:02.000000 recfast4py-0.2.8/HISTORY.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      514 2017-03-14 14:20:31.000000 recfast4py-0.2.8/LICENSE
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      246 2023-04-18 14:09:48.000000 recfast4py-0.2.8/MANIFEST.in
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1683 2023-04-18 14:57:39.000000 recfast4py-0.2.8/Makefile
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      893 2023-04-20 09:40:47.538140 recfast4py-0.2.8/PKG-INFO
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      101 2023-04-18 14:56:34.000000 recfast4py-0.2.8/README.rst
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:40:47.533554 recfast4py-0.2.8/docs/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        9 2017-03-14 15:09:54.000000 recfast4py-0.2.8/docs/.gitignore
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6777 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/Makefile
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/authors.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      515 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/check_sphinx.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8562 2019-05-09 14:45:36.000000 recfast4py-0.2.8/docs/conf.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       32 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/contributing.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/history.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      607 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/index.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      230 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/installation.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6466 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/make.bat
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       67 2017-03-28 12:31:43.000000 recfast4py-0.2.8/docs/modules.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      481 2017-03-28 12:31:43.000000 recfast4py-0.2.8/docs/recfast4py.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      395 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/usage.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2013 2023-04-20 09:40:37.000000 recfast4py-0.2.8/pyproject.toml
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       38 2023-04-20 09:40:47.538340 recfast4py-0.2.8/setup.cfg
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      723 2023-04-20 09:38:47.000000 recfast4py-0.2.8/setup.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:40:47.530301 recfast4py-0.2.8/src/
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:40:47.536917 recfast4py-0.2.8/src/recfast4py/
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3175 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/DM_annihilation.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1036 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/DM_annihilation.Recfast.h
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)    42560 2021-04-16 07:26:49.000000 recfast4py-0.2.8/src/recfast4py/ODE_solver.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2955 2020-02-13 17:11:51.000000 recfast4py-0.2.8/src/recfast4py/ODE_solver.Recfast.h
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3902 2018-04-10 15:58:01.000000 recfast4py-0.2.8/src/recfast4py/Rec_corrs_CT.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1278 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/Rec_corrs_CT.Recfast.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      181 2023-04-18 14:51:17.000000 recfast4py-0.2.8/src/recfast4py/__init__.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)   242951 2023-04-18 15:43:50.000000 recfast4py-0.2.8/src/recfast4py/_recfast.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)   243343 2023-04-20 09:34:20.000000 recfast4py-0.2.8/src/recfast4py/_recfast.cpp
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      789 2023-04-20 09:34:20.000000 recfast4py-0.2.8/src/recfast4py/_recfast.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1750 2023-04-20 09:37:08.000000 recfast4py-0.2.8/src/recfast4py/_recfast.pyx
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     6675 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/constants.Recfast.h
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2485 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/cosmology.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1974 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/cosmology.Recfast.h
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:40:47.537770 recfast4py-0.2.8/src/recfast4py/data/
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)    23196 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/data/DXe_Xe.CT2010.dat
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     8479 2021-04-16 07:26:49.000000 recfast4py-0.2.8/src/recfast4py/evalode.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1627 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/evalode.Recfast.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1056 2023-04-18 14:44:01.000000 recfast4py-0.2.8/src/recfast4py/recfast.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      200 2023-04-18 14:51:44.000000 recfast4py-0.2.8/src/recfast4py/recfast4py.py
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)    15164 2020-02-13 17:11:51.000000 recfast4py-0.2.8/src/recfast4py/recombination.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2256 2019-05-09 11:00:46.000000 recfast4py-0.2.8/src/recfast4py/recombination.Recfast.h
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:40:47.537622 recfast4py-0.2.8/src/recfast4py.egg-info/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      893 2023-04-20 09:40:47.000000 recfast4py-0.2.8/src/recfast4py.egg-info/PKG-INFO
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1260 2023-04-20 09:40:47.000000 recfast4py-0.2.8/src/recfast4py.egg-info/SOURCES.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2023-04-20 09:40:47.000000 recfast4py-0.2.8/src/recfast4py.egg-info/dependency_links.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      184 2023-04-20 09:40:47.000000 recfast4py-0.2.8/src/recfast4py.egg-info/requires.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       11 2023-04-20 09:40:47.000000 recfast4py-0.2.8/src/recfast4py.egg-info/top_level.txt
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:40:47.537935 recfast4py-0.2.8/tests/
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1114 2023-04-18 14:51:35.000000 recfast4py-0.2.8/tests/test_recfast4py.py
```

### Comparing `recfast4py-0.2.7/CONTRIBUTING.rst` & `recfast4py-0.2.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/LICENSE` & `recfast4py-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/Makefile` & `recfast4py-0.2.8/Makefile`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/PKG-INFO` & `recfast4py-0.2.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recfast4py
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python wrapper for recfast++
 Author-email: Uwe Schmitt <uwe.schmitt@id.ethz.ch>
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `recfast4py-0.2.7/docs/Makefile` & `recfast4py-0.2.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/docs/check_sphinx.py` & `recfast4py-0.2.8/docs/check_sphinx.py`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/docs/conf.py` & `recfast4py-0.2.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/docs/index.rst` & `recfast4py-0.2.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/docs/make.bat` & `recfast4py-0.2.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/pyproject.toml` & `recfast4py-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 40.6.0", "wheel", "numpy", "Cython"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "recfast4py"
-version = "0.2.7"
+version = "0.2.8"
 license = {text = "GPLv3"}
 description = "Python wrapper for recfast++"
 authors = [
     {name = "Uwe Schmitt", email = "uwe.schmitt@id.ethz.ch"},
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `recfast4py-0.2.7/src/recfast4py/DM_annihilation.Recfast.cpp` & `recfast4py-0.2.8/src/recfast4py/DM_annihilation.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/DM_annihilation.Recfast.h` & `recfast4py-0.2.8/src/recfast4py/DM_annihilation.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/ODE_solver.Recfast.cpp` & `recfast4py-0.2.8/src/recfast4py/ODE_solver.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/ODE_solver.Recfast.h` & `recfast4py-0.2.8/src/recfast4py/ODE_solver.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/Rec_corrs_CT.Recfast.cpp` & `recfast4py-0.2.8/src/recfast4py/Rec_corrs_CT.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/Rec_corrs_CT.Recfast.h` & `recfast4py-0.2.8/src/recfast4py/Rec_corrs_CT.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/_recfast.c` & `recfast4py-0.2.8/src/recfast4py/_recfast.c`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/_recfast.cpp` & `recfast4py-0.2.8/src/recfast4py/_recfast.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1004,29 +1004,29 @@
   "stringsource",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct__recombination;
 struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr;
 
-/* "recfast4py/_recfast.pyx":29
+/* "recfast4py/_recfast.pyx":30
  * 
  * 
  * def recombination(double Yp, double T0, double Om, double Ob, double OL, double Ok, double h100,             # <<<<<<<<<<<<<<
  *                   double Nnu, double F, double fDM, int flag, int npz, double zstart, double zend):
  * 
  */
 struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct__recombination {
   PyObject_HEAD
   int __pyx_v_npz;
   double *__pyx_v_results[5];
 };
 
 
-/* "recfast4py/_recfast.pyx":66
+/* "recfast4py/_recfast.pyx":67
  * 
  *     # arrays to lists
  *     result = tuple([results[i][j] for j in range(npz)] for i in range(5))             # <<<<<<<<<<<<<<
  * 
  *     free(results_array)
  */
 struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr {
@@ -1601,15 +1601,15 @@
 static PyObject *__pyx_tp_new_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_codeobj__4;
 /* Late includes */
 std::string installPath;
 
-/* "recfast4py/_recfast.pyx":29
+/* "recfast4py/_recfast.pyx":30
  * 
  * 
  * def recombination(double Yp, double T0, double Om, double Ob, double OL, double Ok, double h100,             # <<<<<<<<<<<<<<
  *                   double Nnu, double F, double fDM, int flag, int npz, double zstart, double zend):
  * 
  */
 
@@ -1680,91 +1680,91 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_Yp)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_T0)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 1); __PYX_ERR(0, 29, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 1); __PYX_ERR(0, 30, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_Om)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 2); __PYX_ERR(0, 29, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 2); __PYX_ERR(0, 30, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_Ob)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 3); __PYX_ERR(0, 29, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 3); __PYX_ERR(0, 30, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_OL)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 4); __PYX_ERR(0, 29, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 4); __PYX_ERR(0, 30, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_Ok)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 5); __PYX_ERR(0, 29, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 5); __PYX_ERR(0, 30, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_h100)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 6); __PYX_ERR(0, 29, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 6); __PYX_ERR(0, 30, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_Nnu)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 7); __PYX_ERR(0, 29, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 7); __PYX_ERR(0, 30, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (likely((values[8] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_F)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 8); __PYX_ERR(0, 29, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 8); __PYX_ERR(0, 30, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  9:
         if (likely((values[9] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fDM)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 9); __PYX_ERR(0, 29, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 9); __PYX_ERR(0, 30, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 10:
         if (likely((values[10] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flag)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 10); __PYX_ERR(0, 29, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 10); __PYX_ERR(0, 30, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 11:
         if (likely((values[11] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_npz)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 11); __PYX_ERR(0, 29, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 11); __PYX_ERR(0, 30, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 12:
         if (likely((values[12] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_zstart)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 12); __PYX_ERR(0, 29, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 12); __PYX_ERR(0, 30, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 13:
         if (likely((values[13] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_zend)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 13); __PYX_ERR(0, 29, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, 13); __PYX_ERR(0, 30, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "recombination") < 0)) __PYX_ERR(0, 29, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "recombination") < 0)) __PYX_ERR(0, 30, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 14) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -1776,46 +1776,46 @@
       values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
       values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
       values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
       values[11] = PyTuple_GET_ITEM(__pyx_args, 11);
       values[12] = PyTuple_GET_ITEM(__pyx_args, 12);
       values[13] = PyTuple_GET_ITEM(__pyx_args, 13);
     }
-    __pyx_v_Yp = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_Yp == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
-    __pyx_v_T0 = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_T0 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
-    __pyx_v_Om = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_Om == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
-    __pyx_v_Ob = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_Ob == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
-    __pyx_v_OL = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_OL == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
-    __pyx_v_Ok = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_Ok == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
-    __pyx_v_h100 = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_h100 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
-    __pyx_v_Nnu = __pyx_PyFloat_AsDouble(values[7]); if (unlikely((__pyx_v_Nnu == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
-    __pyx_v_F = __pyx_PyFloat_AsDouble(values[8]); if (unlikely((__pyx_v_F == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
-    __pyx_v_fDM = __pyx_PyFloat_AsDouble(values[9]); if (unlikely((__pyx_v_fDM == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
-    __pyx_v_flag = __Pyx_PyInt_As_int(values[10]); if (unlikely((__pyx_v_flag == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
-    __pyx_v_npz = __Pyx_PyInt_As_int(values[11]); if (unlikely((__pyx_v_npz == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
-    __pyx_v_zstart = __pyx_PyFloat_AsDouble(values[12]); if (unlikely((__pyx_v_zstart == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
-    __pyx_v_zend = __pyx_PyFloat_AsDouble(values[13]); if (unlikely((__pyx_v_zend == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+    __pyx_v_Yp = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_Yp == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+    __pyx_v_T0 = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_T0 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+    __pyx_v_Om = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_Om == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+    __pyx_v_Ob = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_Ob == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+    __pyx_v_OL = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_OL == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+    __pyx_v_Ok = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_Ok == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+    __pyx_v_h100 = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_h100 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+    __pyx_v_Nnu = __pyx_PyFloat_AsDouble(values[7]); if (unlikely((__pyx_v_Nnu == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L3_error)
+    __pyx_v_F = __pyx_PyFloat_AsDouble(values[8]); if (unlikely((__pyx_v_F == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L3_error)
+    __pyx_v_fDM = __pyx_PyFloat_AsDouble(values[9]); if (unlikely((__pyx_v_fDM == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L3_error)
+    __pyx_v_flag = __Pyx_PyInt_As_int(values[10]); if (unlikely((__pyx_v_flag == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L3_error)
+    __pyx_v_npz = __Pyx_PyInt_As_int(values[11]); if (unlikely((__pyx_v_npz == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L3_error)
+    __pyx_v_zstart = __pyx_PyFloat_AsDouble(values[12]); if (unlikely((__pyx_v_zstart == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L3_error)
+    __pyx_v_zend = __pyx_PyFloat_AsDouble(values[13]); if (unlikely((__pyx_v_zend == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 29, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("recombination", 1, 14, 14, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 30, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("recfast4py._recfast.recombination", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10recfast4py_8_recfast_recombination(__pyx_self, __pyx_v_Yp, __pyx_v_T0, __pyx_v_Om, __pyx_v_Ob, __pyx_v_OL, __pyx_v_Ok, __pyx_v_h100, __pyx_v_Nnu, __pyx_v_F, __pyx_v_fDM, __pyx_v_flag, __pyx_v_npz, __pyx_v_zstart, __pyx_v_zend);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_10recfast4py_8_recfast_13recombination_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "recfast4py/_recfast.pyx":66
+/* "recfast4py/_recfast.pyx":67
  * 
  *     # arrays to lists
  *     result = tuple([results[i][j] for j in range(npz)] for i in range(5))             # <<<<<<<<<<<<<<
  * 
  *     free(results_array)
  */
 
@@ -1827,23 +1827,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr *)__pyx_tp_new_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr(__pyx_ptype_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 66, __pyx_L1_error)
+    __PYX_ERR(0, 67, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct__recombination *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10recfast4py_8_recfast_13recombination_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_recombination_locals_genexpr, __pyx_n_s_recfast4py__recfast); if (unlikely(!gen)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10recfast4py_8_recfast_13recombination_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_recombination_locals_genexpr, __pyx_n_s_recfast4py__recfast); if (unlikely(!gen)) __PYX_ERR(0, 67, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -1874,40 +1874,40 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L8_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 66, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 67, __pyx_L1_error)
   for (__pyx_t_1 = 0; __pyx_t_1 < 5; __pyx_t_1+=1) {
     __pyx_cur_scope->__pyx_v_i = __pyx_t_1;
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = __pyx_cur_scope->__pyx_outer_scope->__pyx_v_npz;
     __pyx_t_4 = __pyx_t_3;
     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
       __pyx_cur_scope->__pyx_v_j = __pyx_t_5;
-      __pyx_t_6 = PyFloat_FromDouble(((__pyx_cur_scope->__pyx_outer_scope->__pyx_v_results[__pyx_cur_scope->__pyx_v_i])[__pyx_cur_scope->__pyx_v_j])); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 66, __pyx_L1_error)
+      __pyx_t_6 = PyFloat_FromDouble(((__pyx_cur_scope->__pyx_outer_scope->__pyx_v_results[__pyx_cur_scope->__pyx_v_i])[__pyx_cur_scope->__pyx_v_j])); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 67, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 66, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 67, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __Pyx_XGIVEREF(__pyx_r);
     __Pyx_RefNannyFinishContext();
     __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
     /* return from generator, yielding value */
     __pyx_generator->resume_label = 1;
     return __pyx_r;
     __pyx_L8_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 66, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 67, __pyx_L1_error)
   }
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -1921,15 +1921,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "recfast4py/_recfast.pyx":29
+/* "recfast4py/_recfast.pyx":30
  * 
  * 
  * def recombination(double Yp, double T0, double Om, double Ob, double OL, double Ok, double h100,             # <<<<<<<<<<<<<<
  *                   double Nnu, double F, double fDM, int flag, int npz, double zstart, double zend):
  * 
  */
 
@@ -1951,285 +1951,285 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("recombination", 0);
   __pyx_cur_scope = (struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct__recombination *)__pyx_tp_new_10recfast4py_8_recfast___pyx_scope_struct__recombination(__pyx_ptype_10recfast4py_8_recfast___pyx_scope_struct__recombination, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10recfast4py_8_recfast___pyx_scope_struct__recombination *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 29, __pyx_L1_error)
+    __PYX_ERR(0, 30, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_npz = __pyx_v_npz;
 
-  /* "recfast4py/_recfast.pyx":34
+  /* "recfast4py/_recfast.pyx":35
  *     cdef double[14] params
  * 
  *     params[0] = npz             # <<<<<<<<<<<<<<
  *     params[1] = zstart
  *     params[2] = zend
  */
   (__pyx_v_params[0]) = __pyx_cur_scope->__pyx_v_npz;
 
-  /* "recfast4py/_recfast.pyx":35
+  /* "recfast4py/_recfast.pyx":36
  * 
  *     params[0] = npz
  *     params[1] = zstart             # <<<<<<<<<<<<<<
  *     params[2] = zend
  *     params[3] = Yp
  */
   (__pyx_v_params[1]) = __pyx_v_zstart;
 
-  /* "recfast4py/_recfast.pyx":36
+  /* "recfast4py/_recfast.pyx":37
  *     params[0] = npz
  *     params[1] = zstart
  *     params[2] = zend             # <<<<<<<<<<<<<<
  *     params[3] = Yp
  *     params[4] = T0
  */
   (__pyx_v_params[2]) = __pyx_v_zend;
 
-  /* "recfast4py/_recfast.pyx":37
+  /* "recfast4py/_recfast.pyx":38
  *     params[1] = zstart
  *     params[2] = zend
  *     params[3] = Yp             # <<<<<<<<<<<<<<
  *     params[4] = T0
  *     params[5] = Om
  */
   (__pyx_v_params[3]) = __pyx_v_Yp;
 
-  /* "recfast4py/_recfast.pyx":38
+  /* "recfast4py/_recfast.pyx":39
  *     params[2] = zend
  *     params[3] = Yp
  *     params[4] = T0             # <<<<<<<<<<<<<<
  *     params[5] = Om
  *     params[6] = Ob
  */
   (__pyx_v_params[4]) = __pyx_v_T0;
 
-  /* "recfast4py/_recfast.pyx":39
+  /* "recfast4py/_recfast.pyx":40
  *     params[3] = Yp
  *     params[4] = T0
  *     params[5] = Om             # <<<<<<<<<<<<<<
  *     params[6] = Ob
  *     params[7] = OL
  */
   (__pyx_v_params[5]) = __pyx_v_Om;
 
-  /* "recfast4py/_recfast.pyx":40
+  /* "recfast4py/_recfast.pyx":41
  *     params[4] = T0
  *     params[5] = Om
  *     params[6] = Ob             # <<<<<<<<<<<<<<
  *     params[7] = OL
  *     params[8] = Ok
  */
   (__pyx_v_params[6]) = __pyx_v_Ob;
 
-  /* "recfast4py/_recfast.pyx":41
+  /* "recfast4py/_recfast.pyx":42
  *     params[5] = Om
  *     params[6] = Ob
  *     params[7] = OL             # <<<<<<<<<<<<<<
  *     params[8] = Ok
  *     params[9] = h100
  */
   (__pyx_v_params[7]) = __pyx_v_OL;
 
-  /* "recfast4py/_recfast.pyx":42
+  /* "recfast4py/_recfast.pyx":43
  *     params[6] = Ob
  *     params[7] = OL
  *     params[8] = Ok             # <<<<<<<<<<<<<<
  *     params[9] = h100
  *     params[10] = Nnu
  */
   (__pyx_v_params[8]) = __pyx_v_Ok;
 
-  /* "recfast4py/_recfast.pyx":43
+  /* "recfast4py/_recfast.pyx":44
  *     params[7] = OL
  *     params[8] = Ok
  *     params[9] = h100             # <<<<<<<<<<<<<<
  *     params[10] = Nnu
  *     params[11] = F
  */
   (__pyx_v_params[9]) = __pyx_v_h100;
 
-  /* "recfast4py/_recfast.pyx":44
+  /* "recfast4py/_recfast.pyx":45
  *     params[8] = Ok
  *     params[9] = h100
  *     params[10] = Nnu             # <<<<<<<<<<<<<<
  *     params[11] = F
  *     params[12] = fDM
  */
   (__pyx_v_params[10]) = __pyx_v_Nnu;
 
-  /* "recfast4py/_recfast.pyx":45
+  /* "recfast4py/_recfast.pyx":46
  *     params[9] = h100
  *     params[10] = Nnu
  *     params[11] = F             # <<<<<<<<<<<<<<
  *     params[12] = fDM
  *     params[13] = flag
  */
   (__pyx_v_params[11]) = __pyx_v_F;
 
-  /* "recfast4py/_recfast.pyx":46
+  /* "recfast4py/_recfast.pyx":47
  *     params[10] = Nnu
  *     params[11] = F
  *     params[12] = fDM             # <<<<<<<<<<<<<<
  *     params[13] = flag
  * 
  */
   (__pyx_v_params[12]) = __pyx_v_fDM;
 
-  /* "recfast4py/_recfast.pyx":47
+  /* "recfast4py/_recfast.pyx":48
  *     params[11] = F
  *     params[12] = fDM
  *     params[13] = flag             # <<<<<<<<<<<<<<
  * 
  *     cdef double * results[5]
  */
   (__pyx_v_params[13]) = __pyx_v_flag;
 
-  /* "recfast4py/_recfast.pyx":53
+  /* "recfast4py/_recfast.pyx":54
  *     cdef int i
  * 
  *     results_array = <double *>malloc(npz * 5 * sizeof(double))             # <<<<<<<<<<<<<<
  *     if results_array == NULL:
  *         raise MemoryError()
  */
   __pyx_v_results_array = ((double *)malloc(((__pyx_cur_scope->__pyx_v_npz * 5) * (sizeof(double)))));
 
-  /* "recfast4py/_recfast.pyx":54
+  /* "recfast4py/_recfast.pyx":55
  * 
  *     results_array = <double *>malloc(npz * 5 * sizeof(double))
  *     if results_array == NULL:             # <<<<<<<<<<<<<<
  *         raise MemoryError()
  * 
  */
   __pyx_t_1 = ((__pyx_v_results_array == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "recfast4py/_recfast.pyx":55
+    /* "recfast4py/_recfast.pyx":56
  *     results_array = <double *>malloc(npz * 5 * sizeof(double))
  *     if results_array == NULL:
  *         raise MemoryError()             # <<<<<<<<<<<<<<
  * 
  *     for i in range(5):
  */
-    PyErr_NoMemory(); __PYX_ERR(0, 55, __pyx_L1_error)
+    PyErr_NoMemory(); __PYX_ERR(0, 56, __pyx_L1_error)
 
-    /* "recfast4py/_recfast.pyx":54
+    /* "recfast4py/_recfast.pyx":55
  * 
  *     results_array = <double *>malloc(npz * 5 * sizeof(double))
  *     if results_array == NULL:             # <<<<<<<<<<<<<<
  *         raise MemoryError()
  * 
  */
   }
 
-  /* "recfast4py/_recfast.pyx":57
+  /* "recfast4py/_recfast.pyx":58
  *         raise MemoryError()
  * 
  *     for i in range(5):             # <<<<<<<<<<<<<<
  *         results[i] = results_array + i * npz
  * 
  */
   for (__pyx_t_2 = 0; __pyx_t_2 < 5; __pyx_t_2+=1) {
     __pyx_v_i = __pyx_t_2;
 
-    /* "recfast4py/_recfast.pyx":58
+    /* "recfast4py/_recfast.pyx":59
  * 
  *     for i in range(5):
  *         results[i] = results_array + i * npz             # <<<<<<<<<<<<<<
  * 
  *     cdef err_code = Xe_frac(params, results[0], results[1], results[2], results[3], results[4], 1, DEBUG)
  */
     (__pyx_cur_scope->__pyx_v_results[__pyx_v_i]) = (__pyx_v_results_array + (__pyx_v_i * __pyx_cur_scope->__pyx_v_npz));
   }
 
-  /* "recfast4py/_recfast.pyx":60
+  /* "recfast4py/_recfast.pyx":61
  *         results[i] = results_array + i * npz
  * 
  *     cdef err_code = Xe_frac(params, results[0], results[1], results[2], results[3], results[4], 1, DEBUG)             # <<<<<<<<<<<<<<
  * 
  *     if err_code:
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(Xe_frac(__pyx_v_params, (__pyx_cur_scope->__pyx_v_results[0]), (__pyx_cur_scope->__pyx_v_results[1]), (__pyx_cur_scope->__pyx_v_results[2]), (__pyx_cur_scope->__pyx_v_results[3]), (__pyx_cur_scope->__pyx_v_results[4]), 1, __pyx_v_10recfast4py_8_recfast_DEBUG)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(Xe_frac(__pyx_v_params, (__pyx_cur_scope->__pyx_v_results[0]), (__pyx_cur_scope->__pyx_v_results[1]), (__pyx_cur_scope->__pyx_v_results[2]), (__pyx_cur_scope->__pyx_v_results[3]), (__pyx_cur_scope->__pyx_v_results[4]), 1, __pyx_v_10recfast4py_8_recfast_DEBUG)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_err_code = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "recfast4py/_recfast.pyx":62
+  /* "recfast4py/_recfast.pyx":63
  *     cdef err_code = Xe_frac(params, results[0], results[1], results[2], results[3], results[4], 1, DEBUG)
  * 
  *     if err_code:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Xe_frac returned code %s" % err_code)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_err_code); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_err_code); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 63, __pyx_L1_error)
   if (unlikely(__pyx_t_1)) {
 
-    /* "recfast4py/_recfast.pyx":63
+    /* "recfast4py/_recfast.pyx":64
  * 
  *     if err_code:
  *         raise RuntimeError("Xe_frac returned code %s" % err_code)             # <<<<<<<<<<<<<<
  * 
  *     # arrays to lists
  */
-    __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Xe_frac_returned_code_s, __pyx_v_err_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Xe_frac_returned_code_s, __pyx_v_err_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 63, __pyx_L1_error)
+    __PYX_ERR(0, 64, __pyx_L1_error)
 
-    /* "recfast4py/_recfast.pyx":62
+    /* "recfast4py/_recfast.pyx":63
  *     cdef err_code = Xe_frac(params, results[0], results[1], results[2], results[3], results[4], 1, DEBUG)
  * 
  *     if err_code:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Xe_frac returned code %s" % err_code)
  * 
  */
   }
 
-  /* "recfast4py/_recfast.pyx":66
+  /* "recfast4py/_recfast.pyx":67
  * 
  *     # arrays to lists
  *     result = tuple([results[i][j] for j in range(npz)] for i in range(5))             # <<<<<<<<<<<<<<
  * 
  *     free(results_array)
  */
-  __pyx_t_4 = __pyx_pf_10recfast4py_8_recfast_13recombination_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_4 = __pyx_pf_10recfast4py_8_recfast_13recombination_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PySequence_Tuple(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PySequence_Tuple(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_result = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "recfast4py/_recfast.pyx":68
+  /* "recfast4py/_recfast.pyx":69
  *     result = tuple([results[i][j] for j in range(npz)] for i in range(5))
  * 
  *     free(results_array)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   free(__pyx_v_results_array);
 
-  /* "recfast4py/_recfast.pyx":70
+  /* "recfast4py/_recfast.pyx":71
  *     free(results_array)
  * 
  *     return result             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "recfast4py/_recfast.pyx":29
+  /* "recfast4py/_recfast.pyx":30
  * 
  * 
  * def recombination(double Yp, double T0, double Om, double Ob, double OL, double Ok, double h100,             # <<<<<<<<<<<<<<
  *                   double Nnu, double F, double fDM, int flag, int npz, double zstart, double zend):
  * 
  */
 
@@ -2616,48 +2616,48 @@
   {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
   {&__pyx_kp_s_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 0, 1, 0},
   {&__pyx_n_s_zend, __pyx_k_zend, sizeof(__pyx_k_zend), 0, 0, 1, 1},
   {&__pyx_n_s_zstart, __pyx_k_zstart, sizeof(__pyx_k_zstart), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 55, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 57, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 64, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "recfast4py/_recfast.pyx":26
- * cdef public string installPath = here
+  /* "recfast4py/_recfast.pyx":27
+ * installPath = here
  * 
  * cdef int DEBUG = (os.environ.get("DEBUG_RECFAST", "") != "")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_s_DEBUG_RECFAST, __pyx_n_s_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_s_DEBUG_RECFAST, __pyx_n_s_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "recfast4py/_recfast.pyx":29
+  /* "recfast4py/_recfast.pyx":30
  * 
  * 
  * def recombination(double Yp, double T0, double Om, double Ob, double OL, double Ok, double h100,             # <<<<<<<<<<<<<<
  *                   double Nnu, double F, double fDM, int flag, int npz, double zstart, double zend):
  * 
  */
-  __pyx_tuple__3 = PyTuple_Pack(22, __pyx_n_s_Yp, __pyx_n_s_T0, __pyx_n_s_Om, __pyx_n_s_Ob, __pyx_n_s_OL, __pyx_n_s_Ok, __pyx_n_s_h100, __pyx_n_s_Nnu, __pyx_n_s_F, __pyx_n_s_fDM, __pyx_n_s_flag, __pyx_n_s_npz, __pyx_n_s_zstart, __pyx_n_s_zend, __pyx_n_s_params, __pyx_n_s_results, __pyx_n_s_results_array, __pyx_n_s_i, __pyx_n_s_err_code, __pyx_n_s_result, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(22, __pyx_n_s_Yp, __pyx_n_s_T0, __pyx_n_s_Om, __pyx_n_s_Ob, __pyx_n_s_OL, __pyx_n_s_Ok, __pyx_n_s_h100, __pyx_n_s_Nnu, __pyx_n_s_F, __pyx_n_s_fDM, __pyx_n_s_flag, __pyx_n_s_npz, __pyx_n_s_zstart, __pyx_n_s_zend, __pyx_n_s_params, __pyx_n_s_results, __pyx_n_s_results_array, __pyx_n_s_i, __pyx_n_s_err_code, __pyx_n_s_result, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(14, 0, 22, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_recfast4py__recfast_pyx, __pyx_n_s_recombination, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(14, 0, 22, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_recfast4py__recfast_pyx, __pyx_n_s_recombination, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -2703,23 +2703,23 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_10recfast4py_8_recfast___pyx_scope_struct__recombination) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10recfast4py_8_recfast___pyx_scope_struct__recombination) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10recfast4py_8_recfast___pyx_scope_struct__recombination.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10recfast4py_8_recfast___pyx_scope_struct__recombination.tp_dictoffset && __pyx_type_10recfast4py_8_recfast___pyx_scope_struct__recombination.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10recfast4py_8_recfast___pyx_scope_struct__recombination.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10recfast4py_8_recfast___pyx_scope_struct__recombination = &__pyx_type_10recfast4py_8_recfast___pyx_scope_struct__recombination;
-  if (PyType_Ready(&__pyx_type_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr.tp_dictoffset && __pyx_type_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr = &__pyx_type_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr;
@@ -3051,15 +3051,15 @@
   if (__pyx_t_6) {
 
     /* "recfast4py/_recfast.pyx":22
  * if bytes is not str:
  *     # for python 3
  *     here = bytes(here, "utf-8")             # <<<<<<<<<<<<<<
  * 
- * cdef public string installPath = here
+ * cdef public string installPath
  */
     __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_here); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 22, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
@@ -3078,61 +3078,61 @@
  * 
  * if bytes is not str:             # <<<<<<<<<<<<<<
  *     # for python 3
  *     here = bytes(here, "utf-8")
  */
   }
 
-  /* "recfast4py/_recfast.pyx":24
- *     here = bytes(here, "utf-8")
+  /* "recfast4py/_recfast.pyx":25
  * 
- * cdef public string installPath = here             # <<<<<<<<<<<<<<
+ * cdef public string installPath
+ * installPath = here             # <<<<<<<<<<<<<<
  * 
  * cdef int DEBUG = (os.environ.get("DEBUG_RECFAST", "") != "")
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_here); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_here); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __pyx_convert_string_from_py_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_7 = __pyx_convert_string_from_py_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   installPath = __pyx_t_7;
 
-  /* "recfast4py/_recfast.pyx":26
- * cdef public string installPath = here
+  /* "recfast4py/_recfast.pyx":27
+ * installPath = here
  * 
  * cdef int DEBUG = (os.environ.get("DEBUG_RECFAST", "") != "")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_environ); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_environ); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_n_s_, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_n_s_, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_10recfast4py_8_recfast_DEBUG = __pyx_t_8;
 
-  /* "recfast4py/_recfast.pyx":29
+  /* "recfast4py/_recfast.pyx":30
  * 
  * 
  * def recombination(double Yp, double T0, double Om, double Ob, double OL, double Ok, double h100,             # <<<<<<<<<<<<<<
  *                   double Nnu, double F, double fDM, int flag, int npz, double zstart, double zend):
  * 
  */
-  __pyx_t_3 = PyCFunction_NewEx(&__pyx_mdef_10recfast4py_8_recfast_1recombination, NULL, __pyx_n_s_recfast4py__recfast); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_3 = PyCFunction_NewEx(&__pyx_mdef_10recfast4py_8_recfast_1recombination, NULL, __pyx_n_s_recfast4py__recfast); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_recombination, __pyx_t_3) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_recombination, __pyx_t_3) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "recfast4py/_recfast.pyx":1
  * from libc.stdlib cimport free, malloc             # <<<<<<<<<<<<<<
  * from libcpp.string cimport string
  * 
  */
```

### Comparing `recfast4py-0.2.7/src/recfast4py/_recfast.h` & `recfast4py-0.2.8/src/recfast4py/_recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/_recfast.pyx` & `recfast4py-0.2.8/src/recfast4py/_recfast.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 here = os.path.dirname(os.path.abspath(__file))
 
 if bytes is not str:
     # for python 3
     here = bytes(here, "utf-8")
 
-cdef public string installPath = here
+cdef public string installPath
+installPath = here
 
 cdef int DEBUG = (os.environ.get("DEBUG_RECFAST", "") != "")
 
 
 def recombination(double Yp, double T0, double Om, double Ob, double OL, double Ok, double h100,
                   double Nnu, double F, double fDM, int flag, int npz, double zstart, double zend):
```

### Comparing `recfast4py-0.2.7/src/recfast4py/constants.Recfast.h` & `recfast4py-0.2.8/src/recfast4py/constants.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/cosmology.Recfast.cpp` & `recfast4py-0.2.8/src/recfast4py/cosmology.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/cosmology.Recfast.h` & `recfast4py-0.2.8/src/recfast4py/cosmology.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/data/DXe_Xe.CT2010.dat` & `recfast4py-0.2.8/src/recfast4py/data/DXe_Xe.CT2010.dat`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/evalode.Recfast.cpp` & `recfast4py-0.2.8/src/recfast4py/evalode.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/evalode.Recfast.h` & `recfast4py-0.2.8/src/recfast4py/evalode.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/recfast.py` & `recfast4py-0.2.8/src/recfast4py/recfast.py`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/recombination.Recfast.cpp` & `recfast4py-0.2.8/src/recfast4py/recombination.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py/recombination.Recfast.h` & `recfast4py-0.2.8/src/recfast4py/recombination.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/src/recfast4py.egg-info/PKG-INFO` & `recfast4py-0.2.8/src/recfast4py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recfast4py
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python wrapper for recfast++
 Author-email: Uwe Schmitt <uwe.schmitt@id.ethz.ch>
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `recfast4py-0.2.7/src/recfast4py.egg-info/SOURCES.txt` & `recfast4py-0.2.8/src/recfast4py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.7/tests/test_recfast4py.py` & `recfast4py-0.2.8/tests/test_recfast4py.py`

 * *Files identical despite different names*

