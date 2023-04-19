# Comparing `tmp/up_fmap-0.0.3.tar.gz` & `tmp/up_fmap-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_fmap-0.0.3.tar", last modified: Tue Apr 18 10:39:17 2023, max compression
+gzip compressed data, was "up_fmap-0.0.4.tar", last modified: Wed Apr 19 23:00:49 2023, max compression
```

## Comparing `up_fmap-0.0.3.tar` & `up_fmap-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:39:17.111011 up_fmap-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 10:39:05.000000 up_fmap-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 10:39:17.111011 up_fmap-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-18 10:39:05.000000 up_fmap-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 10:39:17.111011 up_fmap-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-18 10:39:05.000000 up_fmap-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:39:17.111011 up_fmap-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-04-18 10:39:05.000000 up_fmap-0.0.3/test/test_up_fmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:39:17.111011 up_fmap-0.0.3/up_fmap/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-18 10:39:05.000000 up_fmap-0.0.3/up_fmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-18 10:39:05.000000 up_fmap-0.0.3/up_fmap/fmap_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:39:17.111011 up_fmap-0.0.3/up_fmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 10:39:17.000000 up_fmap-0.0.3/up_fmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-18 10:39:17.000000 up_fmap-0.0.3/up_fmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:39:17.000000 up_fmap-0.0.3/up_fmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 10:39:17.000000 up_fmap-0.0.3/up_fmap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:00:49.002207 up_fmap-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 23:00:39.000000 up_fmap-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-19 23:00:49.002207 up_fmap-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-19 23:00:39.000000 up_fmap-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:00:49.002207 up_fmap-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-19 23:00:39.000000 up_fmap-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:00:48.998207 up_fmap-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-04-19 23:00:39.000000 up_fmap-0.0.4/test/test_up_fmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:00:48.998207 up_fmap-0.0.4/up_fmap/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 23:00:39.000000 up_fmap-0.0.4/up_fmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-04-19 23:00:39.000000 up_fmap-0.0.4/up_fmap/fmap_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:00:49.002207 up_fmap-0.0.4/up_fmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-19 23:00:48.000000 up_fmap-0.0.4/up_fmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 23:00:48.000000 up_fmap-0.0.4/up_fmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:00:48.000000 up_fmap-0.0.4/up_fmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 23:00:48.000000 up_fmap-0.0.4/up_fmap.egg-info/top_level.txt
```

### Comparing `up_fmap-0.0.3/LICENSE` & `up_fmap-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `up_fmap-0.0.3/README.md` & `up_fmap-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `up_fmap-0.0.3/setup.py` & `up_fmap-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def run(self):
         install_FMAP()
         develop.run(self)
 
 
 setup(
     name="up_fmap",
-    version="0.0.3",
+    version="0.0.4",
     description="up_fmap",
     author="Alejandro Torreño, Eva Onaindia and Oscar Sapena",
     author_email="onaindia@dsic.upv.es",
     packages=["up_fmap"],
     package_data={"": ["FMAP/FMAP.jar"]},
     cmdclass={"build_py": InstallFMAP, "develop": InstallFMAPdevelop},
     license="APACHE",
```

### Comparing `up_fmap-0.0.3/test/test_up_fmap.py` & `up_fmap-0.0.4/test/test_up_fmap.py`

 * *Files identical despite different names*

### Comparing `up_fmap-0.0.3/up_fmap/fmap_planner.py` & `up_fmap-0.0.4/up_fmap/fmap_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,18 +96,16 @@
     def supported_kind() -> "ProblemKind":
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED_MULTI_AGENT")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
-        supported_kind.set_conditions_kind("EQUALITY")
-        supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
+        supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
-        supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
         return supported_kind
 
     @staticmethod
     def supports(problem_kind: "ProblemKind") -> bool:
         return problem_kind <= FMAPsolver.supported_kind()
```

