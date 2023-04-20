# Comparing `tmp/recfast4py-0.2.8.tar.gz` & `tmp/recfast4py-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recfast4py-0.2.8.tar", last modified: Thu Apr 20 09:40:47 2023, max compression
+gzip compressed data, was "recfast4py-0.2.9.tar", last modified: Thu Apr 20 09:57:19 2023, max compression
```

## Comparing `recfast4py-0.2.8.tar` & `recfast4py-0.2.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:40:47.538301 recfast4py-0.2.8/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      164 2017-09-08 11:49:33.000000 recfast4py-0.2.8/AUTHORS.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1569 2017-03-14 15:09:27.000000 recfast4py-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      314 2017-09-08 11:49:02.000000 recfast4py-0.2.8/HISTORY.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      514 2017-03-14 14:20:31.000000 recfast4py-0.2.8/LICENSE
--rw-r--r--   0 uweschmitt   (501) staff       (20)      246 2023-04-18 14:09:48.000000 recfast4py-0.2.8/MANIFEST.in
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1683 2023-04-18 14:57:39.000000 recfast4py-0.2.8/Makefile
--rw-r--r--   0 uweschmitt   (501) staff       (20)      893 2023-04-20 09:40:47.538140 recfast4py-0.2.8/PKG-INFO
--rw-r--r--   0 uweschmitt   (501) staff       (20)      101 2023-04-18 14:56:34.000000 recfast4py-0.2.8/README.rst
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:40:47.533554 recfast4py-0.2.8/docs/
--rw-r--r--   0 uweschmitt   (501) staff       (20)        9 2017-03-14 15:09:54.000000 recfast4py-0.2.8/docs/.gitignore
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6777 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/Makefile
--rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/authors.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      515 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/check_sphinx.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8562 2019-05-09 14:45:36.000000 recfast4py-0.2.8/docs/conf.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)       32 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/contributing.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/history.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      607 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/index.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      230 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/installation.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6466 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/make.bat
--rw-r--r--   0 uweschmitt   (501) staff       (20)       67 2017-03-28 12:31:43.000000 recfast4py-0.2.8/docs/modules.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      481 2017-03-28 12:31:43.000000 recfast4py-0.2.8/docs/recfast4py.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      395 2017-03-14 14:59:53.000000 recfast4py-0.2.8/docs/usage.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2013 2023-04-20 09:40:37.000000 recfast4py-0.2.8/pyproject.toml
--rw-r--r--   0 uweschmitt   (501) staff       (20)       38 2023-04-20 09:40:47.538340 recfast4py-0.2.8/setup.cfg
--rw-r--r--   0 uweschmitt   (501) staff       (20)      723 2023-04-20 09:38:47.000000 recfast4py-0.2.8/setup.py
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:40:47.530301 recfast4py-0.2.8/src/
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:40:47.536917 recfast4py-0.2.8/src/recfast4py/
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3175 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/DM_annihilation.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1036 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/DM_annihilation.Recfast.h
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)    42560 2021-04-16 07:26:49.000000 recfast4py-0.2.8/src/recfast4py/ODE_solver.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2955 2020-02-13 17:11:51.000000 recfast4py-0.2.8/src/recfast4py/ODE_solver.Recfast.h
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3902 2018-04-10 15:58:01.000000 recfast4py-0.2.8/src/recfast4py/Rec_corrs_CT.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1278 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/Rec_corrs_CT.Recfast.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)      181 2023-04-18 14:51:17.000000 recfast4py-0.2.8/src/recfast4py/__init__.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)   242951 2023-04-18 15:43:50.000000 recfast4py-0.2.8/src/recfast4py/_recfast.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)   243343 2023-04-20 09:34:20.000000 recfast4py-0.2.8/src/recfast4py/_recfast.cpp
--rw-r--r--   0 uweschmitt   (501) staff       (20)      789 2023-04-20 09:34:20.000000 recfast4py-0.2.8/src/recfast4py/_recfast.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1750 2023-04-20 09:37:08.000000 recfast4py-0.2.8/src/recfast4py/_recfast.pyx
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     6675 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/constants.Recfast.h
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2485 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/cosmology.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1974 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/cosmology.Recfast.h
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:40:47.537770 recfast4py-0.2.8/src/recfast4py/data/
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)    23196 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/data/DXe_Xe.CT2010.dat
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     8479 2021-04-16 07:26:49.000000 recfast4py-0.2.8/src/recfast4py/evalode.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1627 2017-03-14 14:18:01.000000 recfast4py-0.2.8/src/recfast4py/evalode.Recfast.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1056 2023-04-18 14:44:01.000000 recfast4py-0.2.8/src/recfast4py/recfast.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)      200 2023-04-18 14:51:44.000000 recfast4py-0.2.8/src/recfast4py/recfast4py.py
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)    15164 2020-02-13 17:11:51.000000 recfast4py-0.2.8/src/recfast4py/recombination.Recfast.cpp
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2256 2019-05-09 11:00:46.000000 recfast4py-0.2.8/src/recfast4py/recombination.Recfast.h
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:40:47.537622 recfast4py-0.2.8/src/recfast4py.egg-info/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      893 2023-04-20 09:40:47.000000 recfast4py-0.2.8/src/recfast4py.egg-info/PKG-INFO
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1260 2023-04-20 09:40:47.000000 recfast4py-0.2.8/src/recfast4py.egg-info/SOURCES.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2023-04-20 09:40:47.000000 recfast4py-0.2.8/src/recfast4py.egg-info/dependency_links.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)      184 2023-04-20 09:40:47.000000 recfast4py-0.2.8/src/recfast4py.egg-info/requires.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)       11 2023-04-20 09:40:47.000000 recfast4py-0.2.8/src/recfast4py.egg-info/top_level.txt
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:40:47.537935 recfast4py-0.2.8/tests/
--rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1114 2023-04-18 14:51:35.000000 recfast4py-0.2.8/tests/test_recfast4py.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:57:19.265763 recfast4py-0.2.9/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      164 2017-09-08 11:49:33.000000 recfast4py-0.2.9/AUTHORS.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1569 2017-03-14 15:09:27.000000 recfast4py-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      314 2017-09-08 11:49:02.000000 recfast4py-0.2.9/HISTORY.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      514 2017-03-14 14:20:31.000000 recfast4py-0.2.9/LICENSE
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      246 2023-04-20 09:53:17.000000 recfast4py-0.2.9/MANIFEST.in
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1683 2023-04-18 14:57:39.000000 recfast4py-0.2.9/Makefile
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      893 2023-04-20 09:57:19.265587 recfast4py-0.2.9/PKG-INFO
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      101 2023-04-18 14:56:34.000000 recfast4py-0.2.9/README.rst
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:57:19.261058 recfast4py-0.2.9/docs/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        9 2017-03-14 15:09:54.000000 recfast4py-0.2.9/docs/.gitignore
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6777 2017-03-14 14:59:53.000000 recfast4py-0.2.9/docs/Makefile
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.9/docs/authors.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      515 2017-03-14 14:59:53.000000 recfast4py-0.2.9/docs/check_sphinx.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8562 2019-05-09 14:45:36.000000 recfast4py-0.2.9/docs/conf.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       32 2017-03-14 14:59:53.000000 recfast4py-0.2.9/docs/contributing.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       27 2017-03-14 14:59:53.000000 recfast4py-0.2.9/docs/history.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      607 2017-03-14 14:59:53.000000 recfast4py-0.2.9/docs/index.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      230 2017-03-14 14:59:53.000000 recfast4py-0.2.9/docs/installation.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6466 2017-03-14 14:59:53.000000 recfast4py-0.2.9/docs/make.bat
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       67 2017-03-28 12:31:43.000000 recfast4py-0.2.9/docs/modules.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      481 2017-03-28 12:31:43.000000 recfast4py-0.2.9/docs/recfast4py.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      395 2017-03-14 14:59:53.000000 recfast4py-0.2.9/docs/usage.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2008 2023-04-20 09:57:09.000000 recfast4py-0.2.9/pyproject.toml
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       38 2023-04-20 09:57:19.265807 recfast4py-0.2.9/setup.cfg
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      723 2023-04-20 09:38:47.000000 recfast4py-0.2.9/setup.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:57:19.257663 recfast4py-0.2.9/src/
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:57:19.264104 recfast4py-0.2.9/src/recfast4py/
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3175 2017-03-14 14:18:01.000000 recfast4py-0.2.9/src/recfast4py/DM_annihilation.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1036 2017-03-14 14:18:01.000000 recfast4py-0.2.9/src/recfast4py/DM_annihilation.Recfast.h
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)    42560 2021-04-16 07:26:49.000000 recfast4py-0.2.9/src/recfast4py/ODE_solver.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2955 2020-02-13 17:11:51.000000 recfast4py-0.2.9/src/recfast4py/ODE_solver.Recfast.h
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     3902 2018-04-10 15:58:01.000000 recfast4py-0.2.9/src/recfast4py/Rec_corrs_CT.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1278 2017-03-14 14:18:01.000000 recfast4py-0.2.9/src/recfast4py/Rec_corrs_CT.Recfast.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      181 2023-04-18 14:51:17.000000 recfast4py-0.2.9/src/recfast4py/__init__.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)   242951 2023-04-18 15:43:50.000000 recfast4py-0.2.9/src/recfast4py/_recfast.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)   239141 2023-04-20 09:53:53.000000 recfast4py-0.2.9/src/recfast4py/_recfast.cpp
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      789 2023-04-20 09:53:53.000000 recfast4py-0.2.9/src/recfast4py/_recfast.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1750 2023-04-20 09:37:08.000000 recfast4py-0.2.9/src/recfast4py/_recfast.pyx
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     6675 2017-03-14 14:18:01.000000 recfast4py-0.2.9/src/recfast4py/constants.Recfast.h
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2485 2017-03-14 14:18:01.000000 recfast4py-0.2.9/src/recfast4py/cosmology.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1974 2017-03-14 14:18:01.000000 recfast4py-0.2.9/src/recfast4py/cosmology.Recfast.h
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:57:19.265146 recfast4py-0.2.9/src/recfast4py/data/
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)    23196 2017-03-14 14:18:01.000000 recfast4py-0.2.9/src/recfast4py/data/DXe_Xe.CT2010.dat
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     8479 2021-04-16 07:26:49.000000 recfast4py-0.2.9/src/recfast4py/evalode.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1627 2017-03-14 14:18:01.000000 recfast4py-0.2.9/src/recfast4py/evalode.Recfast.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1056 2023-04-18 14:44:01.000000 recfast4py-0.2.9/src/recfast4py/recfast.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      200 2023-04-18 14:51:44.000000 recfast4py-0.2.9/src/recfast4py/recfast4py.py
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)    15164 2020-02-13 17:11:51.000000 recfast4py-0.2.9/src/recfast4py/recombination.Recfast.cpp
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     2256 2019-05-09 11:00:46.000000 recfast4py-0.2.9/src/recfast4py/recombination.Recfast.h
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:57:19.264799 recfast4py-0.2.9/src/recfast4py.egg-info/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      893 2023-04-20 09:57:19.000000 recfast4py-0.2.9/src/recfast4py.egg-info/PKG-INFO
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1260 2023-04-20 09:57:19.000000 recfast4py-0.2.9/src/recfast4py.egg-info/SOURCES.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2023-04-20 09:57:19.000000 recfast4py-0.2.9/src/recfast4py.egg-info/dependency_links.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      184 2023-04-20 09:57:19.000000 recfast4py-0.2.9/src/recfast4py.egg-info/requires.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       11 2023-04-20 09:57:19.000000 recfast4py-0.2.9/src/recfast4py.egg-info/top_level.txt
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-04-20 09:57:19.265354 recfast4py-0.2.9/tests/
+-rwxr-xr-x   0 uweschmitt   (501) staff       (20)     1114 2023-04-18 14:51:35.000000 recfast4py-0.2.9/tests/test_recfast4py.py
```

### Comparing `recfast4py-0.2.8/CONTRIBUTING.rst` & `recfast4py-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/LICENSE` & `recfast4py-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/Makefile` & `recfast4py-0.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/PKG-INFO` & `recfast4py-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recfast4py
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python wrapper for recfast++
 Author-email: Uwe Schmitt <uwe.schmitt@id.ethz.ch>
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `recfast4py-0.2.8/docs/Makefile` & `recfast4py-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/docs/check_sphinx.py` & `recfast4py-0.2.9/docs/check_sphinx.py`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/docs/conf.py` & `recfast4py-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/docs/index.rst` & `recfast4py-0.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/docs/make.bat` & `recfast4py-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/pyproject.toml` & `recfast4py-0.2.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 40.6.0", "wheel", "numpy", "Cython"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "recfast4py"
-version = "0.2.8"
+version = "0.2.9"
 license = {text = "GPLv3"}
 description = "Python wrapper for recfast++"
 authors = [
     {name = "Uwe Schmitt", email = "uwe.schmitt@id.ethz.ch"},
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -79,15 +79,15 @@
 testpaths = ["tests"]
 filterwarnings = ["ignore:invalid"]
 
 [tool.tox]
 legacy_tox_ini = '''
 [tox]
 isolated_build = true
-envlist = py38,py39,py310,py311
+envlist = py39,py310,py311
 setenv =
     PIP_EXTRA_INDEX_URL=https://cosmo-pypi.phys.ethz.ch/simple
     HTTP_PROXY=http://proxy.ethz.ch:3128
     HTTPS_PROXY=http://proxy.ethz.ch:3128
 
 [testenv]
 skip_install = false
```

### Comparing `recfast4py-0.2.8/setup.py` & `recfast4py-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/DM_annihilation.Recfast.cpp` & `recfast4py-0.2.9/src/recfast4py/DM_annihilation.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/DM_annihilation.Recfast.h` & `recfast4py-0.2.9/src/recfast4py/DM_annihilation.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/ODE_solver.Recfast.cpp` & `recfast4py-0.2.9/src/recfast4py/ODE_solver.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/ODE_solver.Recfast.h` & `recfast4py-0.2.9/src/recfast4py/ODE_solver.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/Rec_corrs_CT.Recfast.cpp` & `recfast4py-0.2.9/src/recfast4py/Rec_corrs_CT.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/Rec_corrs_CT.Recfast.h` & `recfast4py-0.2.9/src/recfast4py/Rec_corrs_CT.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/_recfast.c` & `recfast4py-0.2.9/src/recfast4py/_recfast.c`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/_recfast.cpp` & `recfast4py-0.2.9/src/recfast4py/_recfast.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,20 @@
-/* Generated by Cython 0.29.34 */
-
-/* BEGIN: Cython Metadata
-{
-    "distutils": {
-        "depends": [
-            "src/recfast4py/recombination.Recfast.h"
-        ],
-        "extra_compile_args": [
-            "-stdlib=libc++"
-        ],
-        "include_dirs": [
-            "src/recfast4py"
-        ],
-        "language": "c++",
-        "name": "recfast4py._recfast",
-        "sources": [
-            "src/recfast4py/_recfast.pyx",
-            "src/recfast4py/cosmology.Recfast.cpp",
-            "src/recfast4py/evalode.Recfast.cpp",
-            "src/recfast4py/recombination.Recfast.cpp",
-            "src/recfast4py/ODE_solver.Recfast.cpp",
-            "src/recfast4py/DM_annihilation.Recfast.cpp",
-            "src/recfast4py/Rec_corrs_CT.Recfast.cpp"
-        ]
-    },
-    "module_name": "recfast4py._recfast"
-}
-END: Cython Metadata */
+/* Generated by Cython 0.29.28 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_28"
+#define CYTHON_HEX_VERSION 0x001D1CF0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -73,15 +45,14 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -110,22 +81,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
-  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -155,67 +122,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
-  #endif
-#elif defined(PY_NOGIL)
-  #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
-  #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 1
-  #ifndef CYTHON_USE_TYPE_SLOTS
-    #define CYTHON_USE_TYPE_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYTYPE_LOOKUP
-  #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #ifndef CYTHON_USE_ASYNC_SLOTS
-    #define CYTHON_USE_ASYNC_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYLIST_INTERNALS
-  #define CYTHON_USE_PYLIST_INTERNALS 0
-  #ifndef CYTHON_USE_UNICODE_INTERNALS
-    #define CYTHON_USE_UNICODE_INTERNALS 1
-  #endif
-  #undef CYTHON_USE_UNICODE_WRITER
-  #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
-  #ifndef CYTHON_AVOID_BORROWED_REFS
-    #define CYTHON_AVOID_BORROWED_REFS 0
-  #endif
-  #ifndef CYTHON_ASSUME_SAFE_MACROS
-    #define CYTHON_ASSUME_SAFE_MACROS 1
-  #endif
-  #ifndef CYTHON_UNPACK_METHODS
-    #define CYTHON_UNPACK_METHODS 1
-  #endif
-  #undef CYTHON_FAST_THREAD_STATE
-  #define CYTHON_FAST_THREAD_STATE 0
-  #undef CYTHON_FAST_PYCALL
-  #define CYTHON_FAST_PYCALL 0
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE 1
-  #endif
-  #undef CYTHON_USE_DICT_VERSIONS
-  #define CYTHON_USE_DICT_VERSIONS 0
-  #undef CYTHON_USE_EXC_INFO_STACK
-  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -227,15 +145,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
+    #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -257,34 +175,31 @@
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 0
   #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
+    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
-  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -590,35 +505,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if PY_VERSION_HEX >= 0x030C0000
-    #define __Pyx_PyUnicode_READY(op)       (0)
+  #if defined(PyUnicode_IS_READY)
+  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                              0 : _PyUnicode_Ready((PyObject *)(op)))
   #else
-    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                                0 : _PyUnicode_Ready((PyObject *)(op)))
+  #define __Pyx_PyUnicode_READY(op)       (0)
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if PY_VERSION_HEX >= 0x030C0000
-    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
+  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
   #else
-    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-    #else
-    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-    #endif
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #endif
+  #else
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -742,18 +657,16 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
-  #if !defined(_USE_MATH_DEFINES)
-    #define _USE_MATH_DEFINES
-  #endif
+#if defined(WIN32) || defined(MS_WINDOWS)
+  #define _USE_MATH_DEFINES
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -1161,20 +1074,14 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1273,26 +1180,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  do {\
+#define __Pyx_GetModuleGlobalName(var, name)  {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-} while(0)
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
+}
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-} while(0)
+}
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1476,15 +1383,15 @@
 /* Module declarations from 'libc.stdlib' */
 
 /* Module declarations from 'libcpp.string' */
 
 /* Module declarations from 'recfast4py._recfast' */
 static PyTypeObject *__pyx_ptype_10recfast4py_8_recfast___pyx_scope_struct__recombination = 0;
 static PyTypeObject *__pyx_ptype_10recfast4py_8_recfast___pyx_scope_struct_1_genexpr = 0;
-__PYX_EXTERN_C DL_EXPORT(std::string) installPath;
+extern DL_EXPORT(std::string) installPath;
 static int __pyx_v_10recfast4py_8_recfast_DEBUG;
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
 #define __Pyx_MODULE_NAME "recfast4py._recfast"
 extern int __pyx_module_is_main_recfast4py___recfast;
 int __pyx_module_is_main_recfast4py___recfast = 0;
 
 /* Implementation of 'recfast4py._recfast' */
@@ -2658,15 +2565,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -2923,15 +2830,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_recfast4py___recfast) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -3743,28 +3650,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_FAST_THREAD_STATE
+#if CYTHON_COMPILING_IN_PYPY
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#else
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
-#else
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -3947,15 +3854,15 @@
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -4071,20 +3978,14 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -4140,32 +4041,22 @@
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
-        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) {
-            /* If the code object creation fails, then we should clear the
-               fetched exception references and propagate the new exception */
-            Py_XDECREF(ptype);
-            Py_XDECREF(pvalue);
-            Py_XDECREF(ptraceback);
-            goto bad;
-        }
-        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
+        if (!py_code) goto bad;
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -5040,20 +4931,14 @@
     if (unlikely(!method)) return NULL;
     return __Pyx__PyObject_CallMethod1(method, arg);
 }
 
 /* CoroutineBase */
 #include <structmember.h>
 #include <frameobject.h>
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
 #define __Pyx_Coroutine_Undelegate(gen) Py_CLEAR((gen)->yieldfrom)
 static int __Pyx_PyGen__FetchStopIterationValue(CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject **pvalue) {
     PyObject *et, *ev, *tb;
     PyObject *value = NULL;
     __Pyx_ErrFetch(&et, &ev, &tb);
     if (!et) {
         Py_XDECREF(tb);
@@ -6033,41 +5918,19 @@
         return -1;
     }
     return 0;
 }
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
-        }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
-            break;
-        }
-    }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    char ctversion[4], rtversion[4];
+    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
+    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
```

### Comparing `recfast4py-0.2.8/src/recfast4py/_recfast.h` & `recfast4py-0.2.9/src/recfast4py/_recfast.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.28 */
 
 #ifndef __PYX_HAVE__recfast4py___recfast
 #define __PYX_HAVE__recfast4py___recfast
 
 #include "Python.h"
 
 #ifndef __PYX_HAVE_API__recfast4py___recfast
```

### Comparing `recfast4py-0.2.8/src/recfast4py/_recfast.pyx` & `recfast4py-0.2.9/src/recfast4py/_recfast.pyx`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/constants.Recfast.h` & `recfast4py-0.2.9/src/recfast4py/constants.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/cosmology.Recfast.cpp` & `recfast4py-0.2.9/src/recfast4py/cosmology.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/cosmology.Recfast.h` & `recfast4py-0.2.9/src/recfast4py/cosmology.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/data/DXe_Xe.CT2010.dat` & `recfast4py-0.2.9/src/recfast4py/data/DXe_Xe.CT2010.dat`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/evalode.Recfast.cpp` & `recfast4py-0.2.9/src/recfast4py/evalode.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/evalode.Recfast.h` & `recfast4py-0.2.9/src/recfast4py/evalode.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/recfast.py` & `recfast4py-0.2.9/src/recfast4py/recfast.py`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/recombination.Recfast.cpp` & `recfast4py-0.2.9/src/recfast4py/recombination.Recfast.cpp`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py/recombination.Recfast.h` & `recfast4py-0.2.9/src/recfast4py/recombination.Recfast.h`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/src/recfast4py.egg-info/PKG-INFO` & `recfast4py-0.2.9/src/recfast4py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recfast4py
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python wrapper for recfast++
 Author-email: Uwe Schmitt <uwe.schmitt@id.ethz.ch>
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `recfast4py-0.2.8/src/recfast4py.egg-info/SOURCES.txt` & `recfast4py-0.2.9/src/recfast4py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recfast4py-0.2.8/tests/test_recfast4py.py` & `recfast4py-0.2.9/tests/test_recfast4py.py`

 * *Files identical despite different names*

