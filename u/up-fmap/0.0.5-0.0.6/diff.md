# Comparing `tmp/up_fmap-0.0.5.tar.gz` & `tmp/up_fmap-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_fmap-0.0.5.tar", last modified: Wed Apr 19 23:30:51 2023, max compression
+gzip compressed data, was "up_fmap-0.0.6.tar", last modified: Wed Apr 19 23:40:58 2023, max compression
```

## Comparing `up_fmap-0.0.5.tar` & `up_fmap-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:30:51.037651 up_fmap-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 23:30:42.000000 up_fmap-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-19 23:30:51.037651 up_fmap-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-19 23:30:42.000000 up_fmap-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:30:51.041651 up_fmap-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-19 23:30:42.000000 up_fmap-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:30:51.037651 up_fmap-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-04-19 23:30:42.000000 up_fmap-0.0.5/test/test_up_fmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:30:51.037651 up_fmap-0.0.5/up_fmap/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 23:30:42.000000 up_fmap-0.0.5/up_fmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-04-19 23:30:42.000000 up_fmap-0.0.5/up_fmap/fmap_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:30:51.037651 up_fmap-0.0.5/up_fmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-19 23:30:51.000000 up_fmap-0.0.5/up_fmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 23:30:51.000000 up_fmap-0.0.5/up_fmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:30:51.000000 up_fmap-0.0.5/up_fmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 23:30:51.000000 up_fmap-0.0.5/up_fmap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:40:58.371481 up_fmap-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 23:40:47.000000 up_fmap-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-19 23:40:58.371481 up_fmap-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-19 23:40:47.000000 up_fmap-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:40:58.371481 up_fmap-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-19 23:40:47.000000 up_fmap-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:40:58.371481 up_fmap-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-04-19 23:40:47.000000 up_fmap-0.0.6/test/test_up_fmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:40:58.371481 up_fmap-0.0.6/up_fmap/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 23:40:47.000000 up_fmap-0.0.6/up_fmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12421 2023-04-19 23:40:47.000000 up_fmap-0.0.6/up_fmap/fmap_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:40:58.371481 up_fmap-0.0.6/up_fmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-19 23:40:58.000000 up_fmap-0.0.6/up_fmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 23:40:58.000000 up_fmap-0.0.6/up_fmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:40:58.000000 up_fmap-0.0.6/up_fmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 23:40:58.000000 up_fmap-0.0.6/up_fmap.egg-info/top_level.txt
```

### Comparing `up_fmap-0.0.5/LICENSE` & `up_fmap-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `up_fmap-0.0.5/README.md` & `up_fmap-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `up_fmap-0.0.5/setup.py` & `up_fmap-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def run(self):
         install_FMAP()
         develop.run(self)
 
 
 setup(
     name="up_fmap",
-    version="0.0.5",
+    version="0.0.6",
     description="up_fmap",
     author="Alejandro Torreño, Eva Onaindia and Oscar Sapena",
     author_email="onaindia@dsic.upv.es",
     packages=["up_fmap"],
     package_data={"": ["FMAP/FMAP.jar"]},
     cmdclass={"build_py": InstallFMAP, "develop": InstallFMAPdevelop},
     license="APACHE",
```

### Comparing `up_fmap-0.0.5/test/test_up_fmap.py` & `up_fmap-0.0.6/test/test_up_fmap.py`

 * *Files identical despite different names*

### Comparing `up_fmap-0.0.5/up_fmap/fmap_planner.py` & `up_fmap-0.0.6/up_fmap/fmap_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,16 @@
         elif plan is None:
             return PlanGenerationResultStatus.UNSOLVABLE_PROVEN
         else:
             return PlanGenerationResultStatus.SOLVED_SATISFICING
 
     @staticmethod
     def supported_kind() -> "ProblemKind":
+        supported_kind = ProblemKind()
+        supported_kind.set_problem_class("ACTION_BASED_MULTI_AGENT")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
         supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
```

