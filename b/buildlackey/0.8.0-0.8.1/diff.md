# Comparing `tmp/buildlackey-0.8.0.tar.gz` & `tmp/buildlackey-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildlackey-0.8.0.tar", last modified: Wed Apr 19 20:36:28 2023, max compression
+gzip compressed data, was "buildlackey-0.8.1.tar", last modified: Thu Apr 20 03:11:23 2023, max compression
```

## Comparing `buildlackey-0.8.0.tar` & `buildlackey-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-19 20:36:28.056637 buildlackey-0.8.0/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-04-07 13:32:43.000000 buildlackey-0.8.0/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43932 2023-04-19 20:36:28.056497 buildlackey-0.8.0/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3752 2023-04-10 18:32:21.000000 buildlackey-0.8.0/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-19 20:36:28.054820 buildlackey-0.8.0/buildlackey/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8853 2023-04-19 20:34:54.000000 buildlackey-0.8.0/buildlackey/Commands.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1224 2023-04-13 00:43:49.000000 buildlackey-0.8.0/buildlackey/Environment.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-04-08 19:28:49.000000 buildlackey-0.8.0/buildlackey/Version.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-31 14:31:31.000000 buildlackey-0.8.0/buildlackey/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-19 20:36:28.055939 buildlackey-0.8.0/buildlackey/exceptions/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       51 2023-02-25 02:47:03.000000 buildlackey-0.8.0/buildlackey/exceptions/ProjectNotSetException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       56 2023-02-25 02:28:42.000000 buildlackey-0.8.0/buildlackey/exceptions/ProjectsBaseNotSetException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 01:41:26.000000 buildlackey-0.8.0/buildlackey/exceptions/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-19 20:36:28.056271 buildlackey-0.8.0/buildlackey/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 02:21:22.000000 buildlackey-0.8.0/buildlackey/resources/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      856 2023-04-13 00:43:13.000000 buildlackey-0.8.0/buildlackey/resources/loggingConfiguration.json
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        5 2023-04-19 14:51:17.000000 buildlackey-0.8.0/buildlackey/resources/version.txt
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-19 20:36:28.055594 buildlackey-0.8.0/buildlackey.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43932 2023-04-19 20:36:28.000000 buildlackey-0.8.0/buildlackey.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      590 2023-04-19 20:36:28.000000 buildlackey-0.8.0/buildlackey.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-19 20:36:28.000000 buildlackey-0.8.0/buildlackey.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      215 2023-04-19 20:36:28.000000 buildlackey-0.8.0/buildlackey.egg-info/entry_points.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-04-19 20:36:28.000000 buildlackey-0.8.0/buildlackey.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-19 20:36:28.000000 buildlackey-0.8.0/buildlackey.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-19 20:36:28.056670 buildlackey-0.8.0/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1331 2023-04-10 17:51:20.000000 buildlackey-0.8.0/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-20 03:11:23.900416 buildlackey-0.8.1/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-04-07 13:32:43.000000 buildlackey-0.8.1/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43932 2023-04-20 03:11:23.900277 buildlackey-0.8.1/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3752 2023-04-10 18:32:21.000000 buildlackey-0.8.1/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-20 03:11:23.898061 buildlackey-0.8.1/buildlackey/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8732 2023-04-20 03:07:29.000000 buildlackey-0.8.1/buildlackey/Commands.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1224 2023-04-13 00:43:49.000000 buildlackey-0.8.1/buildlackey/Environment.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-04-08 19:28:49.000000 buildlackey-0.8.1/buildlackey/Version.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-31 14:31:31.000000 buildlackey-0.8.1/buildlackey/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-20 03:11:23.899521 buildlackey-0.8.1/buildlackey/exceptions/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       51 2023-02-25 02:47:03.000000 buildlackey-0.8.1/buildlackey/exceptions/ProjectNotSetException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       56 2023-02-25 02:28:42.000000 buildlackey-0.8.1/buildlackey/exceptions/ProjectsBaseNotSetException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 01:41:26.000000 buildlackey-0.8.1/buildlackey/exceptions/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-20 03:11:23.900038 buildlackey-0.8.1/buildlackey/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 02:21:22.000000 buildlackey-0.8.1/buildlackey/resources/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      856 2023-04-13 00:43:13.000000 buildlackey-0.8.1/buildlackey/resources/loggingConfiguration.json
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        5 2023-04-20 03:07:43.000000 buildlackey-0.8.1/buildlackey/resources/version.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-20 03:11:23.898843 buildlackey-0.8.1/buildlackey.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43932 2023-04-20 03:11:23.000000 buildlackey-0.8.1/buildlackey.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      590 2023-04-20 03:11:23.000000 buildlackey-0.8.1/buildlackey.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-20 03:11:23.000000 buildlackey-0.8.1/buildlackey.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      215 2023-04-20 03:11:23.000000 buildlackey-0.8.1/buildlackey.egg-info/entry_points.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-04-20 03:11:23.000000 buildlackey-0.8.1/buildlackey.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-20 03:11:23.000000 buildlackey-0.8.1/buildlackey.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-20 03:11:23.900450 buildlackey-0.8.1/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1331 2023-04-10 17:51:20.000000 buildlackey-0.8.1/setup.py
```

### Comparing `buildlackey-0.8.0/LICENSE` & `buildlackey-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `buildlackey-0.8.0/PKG-INFO` & `buildlackey-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildlackey
-Version: 0.8.0
+Version: 0.8.1
 Summary: Project Maintenance Scripts
 Home-page: https://github.com/buildlackey
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
```

### Comparing `buildlackey-0.8.0/README.md` & `buildlackey-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `buildlackey-0.8.0/buildlackey/Commands.py` & `buildlackey-0.8.1/buildlackey/Commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,31 +86,28 @@
     \b
     Use the -i/--input-file option to list a set of module names to execute as your
     unit tests
     \b
 
         PROJECTS_BASE -  The local directory where the python projects are based
         PROJECT       -  The name of the project;  It should be a directory name
-    
+
     \b
     \b
     However, if one or the other is not defined the command assumes it is executing in a CI
     environment and thus the current working directory is the project base directory.
 
     \b
     By default, buildlackey runs the module named tests.TestAll
 
     """
     setUpLogging()
     envBase: EnvironmentBase = EnvironmentBase()
     if envBase.validProjectsBase is True and envBase.validProjectDirectory() is True:
         changeToProjectRoot(projectsBase=envBase.projectsBase, project=envBase.projectDirectory)
-    else:
-        secho(f'{MESSAGE_MISSING_ENVIRONMENT_VARIABLE}')
-        exit(STATUS_MISSING_ENVIRONMENT_VARIABLE)
 
     if input_file is None:
         secho(f'{UNIT_TEST_CLI}')
         status: int = osSystem(f'{UNIT_TEST_CLI}')
         secho(f'{status=}')
     else:
         path: Path = Path(input_file)
```

### Comparing `buildlackey-0.8.0/buildlackey/Environment.py` & `buildlackey-0.8.1/buildlackey/Environment.py`

 * *Files identical despite different names*

### Comparing `buildlackey-0.8.0/buildlackey/resources/loggingConfiguration.json` & `buildlackey-0.8.1/buildlackey/resources/loggingConfiguration.json`

 * *Files identical despite different names*

### Comparing `buildlackey-0.8.0/buildlackey.egg-info/PKG-INFO` & `buildlackey-0.8.1/buildlackey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildlackey
-Version: 0.8.0
+Version: 0.8.1
 Summary: Project Maintenance Scripts
 Home-page: https://github.com/buildlackey
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
```

### Comparing `buildlackey-0.8.0/buildlackey.egg-info/SOURCES.txt` & `buildlackey-0.8.1/buildlackey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildlackey-0.8.0/setup.py` & `buildlackey-0.8.1/setup.py`

 * *Files identical despite different names*

