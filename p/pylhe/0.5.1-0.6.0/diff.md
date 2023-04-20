# Comparing `tmp/pylhe-0.5.1.tar.gz` & `tmp/pylhe-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylhe-0.5.1.tar", last modified: Tue Jan 24 22:42:02 2023, max compression
+gzip compressed data, was "pylhe-0.6.0.tar", last modified: Thu Apr 20 07:58:57 2023, max compression
```

## Comparing `pylhe-0.5.1.tar` & `pylhe-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 22:42:02.187014 pylhe-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-01-24 22:41:19.000000 pylhe-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-24 22:41:19.000000 pylhe-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-01-24 22:42:02.187014 pylhe-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-01-24 22:41:19.000000 pylhe-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-01-24 22:41:19.000000 pylhe-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-01-24 22:42:02.187014 pylhe-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-01-24 22:41:19.000000 pylhe-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 22:42:02.183014 pylhe-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 22:42:02.187014 pylhe-0.5.1/src/pylhe/
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-01-24 22:41:19.000000 pylhe-0.5.1/src/pylhe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-24 22:42:02.000000 pylhe-0.5.1/src/pylhe/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-01-24 22:41:19.000000 pylhe-0.5.1/src/pylhe/awkward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 22:42:02.187014 pylhe-0.5.1/src/pylhe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-01-24 22:42:02.000000 pylhe-0.5.1/src/pylhe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-01-24 22:42:02.000000 pylhe-0.5.1/src/pylhe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 22:42:02.000000 pylhe-0.5.1/src/pylhe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-01-24 22:42:02.000000 pylhe-0.5.1/src/pylhe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-24 22:42:02.000000 pylhe-0.5.1/src/pylhe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:58:57.340460 pylhe-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-04-20 07:58:25.000000 pylhe-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-20 07:58:25.000000 pylhe-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-04-20 07:58:57.340460 pylhe-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-20 07:58:25.000000 pylhe-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-20 07:58:25.000000 pylhe-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-20 07:58:57.340460 pylhe-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-20 07:58:25.000000 pylhe-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:58:57.340460 pylhe-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:58:57.340460 pylhe-0.6.0/src/pylhe/
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-04-20 07:58:25.000000 pylhe-0.6.0/src/pylhe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 07:58:57.000000 pylhe-0.6.0/src/pylhe/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-20 07:58:25.000000 pylhe-0.6.0/src/pylhe/awkward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:58:57.340460 pylhe-0.6.0/src/pylhe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-04-20 07:58:57.000000 pylhe-0.6.0/src/pylhe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-20 07:58:57.000000 pylhe-0.6.0/src/pylhe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:58:57.000000 pylhe-0.6.0/src/pylhe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-20 07:58:57.000000 pylhe-0.6.0/src/pylhe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 07:58:57.000000 pylhe-0.6.0/src/pylhe.egg-info/top_level.txt
```

### Comparing `pylhe-0.5.1/LICENSE` & `pylhe-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylhe-0.5.1/PKG-INFO` & `pylhe-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylhe
-Version: 0.5.1
+Version: 0.6.0
 Summary: small package to get structured data out of Les Houches Event files
 Home-page: https://github.com/scikit-hep/pylhe
 Author: Lukas Heinrich, Matthew Feickert, Eduardo Rodrigues
 Author-email: lukas.heinrich@cern.ch, matthew.feickert@cern.ch, eduardo.rodrigues@cern.ch
 License: Apache
 Project-URL: Source, https://github.com/scikit-hep/pylhe
 Project-URL: Tracker, https://github.com/scikit-hep/pylhe/issues
@@ -94,16 +94,16 @@
 ## Citation
 
 The preferred BibTeX entry for citation of `pylhe` is
 
 ```
 @software{pylhe,
   author = {Lukas Heinrich and Matthew Feickert and Eduardo Rodrigues},
-  title = "{pylhe: v0.5.1}",
-  version = {v0.5.1},
+  title = "{pylhe: v0.6.0}",
+  version = {v0.6.0},
   doi = {10.5281/zenodo.1217031},
   url = {https://github.com/scikit-hep/pylhe},
 }
 ```
 
 ## Contributors
```

### Comparing `pylhe-0.5.1/README.md` & `pylhe-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 ## Citation
 
 The preferred BibTeX entry for citation of `pylhe` is
 
 ```
 @software{pylhe,
   author = {Lukas Heinrich and Matthew Feickert and Eduardo Rodrigues},
-  title = "{pylhe: v0.5.1}",
-  version = {v0.5.1},
+  title = "{pylhe: v0.6.0}",
+  version = {v0.6.0},
   doi = {10.5281/zenodo.1217031},
   url = {https://github.com/scikit-hep/pylhe},
 }
 ```
 
 ## Contributors
```

#### html2text {}

```diff
@@ -29,15 +29,15 @@
 inspected as follows print(event.graph.source) # The graph is nicely displayed
 as SVG in Jupyter notebooks event # To save a DOT graph render the graph to a
 supported image format # (refer to the Graphviz documentation for more)
 event.graph.render(filename="test", format="png", cleanup=True)
 event.graph.render(filename="test", format="pdf", cleanup=True) ``` ## Citation
 The preferred BibTeX entry for citation of `pylhe` is ``` @software{pylhe,
 author = {Lukas Heinrich and Matthew Feickert and Eduardo Rodrigues}, title = "
-{pylhe: v0.5.1}", version = {v0.5.1}, doi = {10.5281/zenodo.1217031}, url =
+{pylhe: v0.6.0}", version = {v0.6.0}, doi = {10.5281/zenodo.1217031}, url =
 {https://github.com/scikit-hep/pylhe}, } ``` ## Contributors We hereby
 acknowledge the contributors that made this project possible ([emoji key]
 (https://allcontributors.org/docs/en/emoji-key)):
         [Matthew_Feickert]                        [Lukas]                  [Eduardo_Rodrigues]     [Johannes   [Henry   [ariaradick] [Junghwan
          Matthew_Feickert                          Lukas                    Eduardo_Rodrigues      Schumann] Schreiner]  ariaradick  John_Goh]
         ð§ ð¨ ð» �        ð§ ð¨ ð» �      ð§ ð» ð�Johannes    Henry        ð» Junghwan
                                                                                                    Schumann  Schreiner               John_Goh
```

### Comparing `pylhe-0.5.1/pyproject.toml` & `pylhe-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylhe-0.5.1/setup.cfg` & `pylhe-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylhe-0.5.1/setup.py` & `pylhe-0.6.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 extras_require = {}
 extras_require["lint"] = sorted({"flake8", "black"})
 extras_require["test"] = sorted(
     {
         "pytest~=6.0",
         "pytest-cov>=2.5.1",
-        "scikit-hep-testdata>=0.3.1",
+        "scikit-hep-testdata>=0.4.0",
         "pydocstyle",
     }
 )
 extras_require["develop"] = sorted(
     set(
         extras_require["lint"]
         + extras_require["test"]
```

### Comparing `pylhe-0.5.1/src/pylhe/__init__.py` & `pylhe-0.6.0/src/pylhe/__init__.py`

 * *Files identical despite different names*

### Comparing `pylhe-0.5.1/src/pylhe/awkward.py` & `pylhe-0.6.0/src/pylhe/awkward.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,20 +6,29 @@
 
 # Python 3.7+
 def __dir__():
     return __all__
 
 
 def register_awkward():
-    """Register Awkward behaviors for pylhe."""
-
-    vector.register_awkward()
-    ak.mixin_class(ak.behavior)(Particle)
-    ak.mixin_class(ak.behavior)(Event)
-    ak.mixin_class(ak.behavior)(EventInfo)
+    """
+    .. deprecated:: 0.6.0
+       Remove use of :func:`~pylhe.awkward.register_awkward` as registration
+       is automatic.
+    .. warning:: :func:`~pylhe.awkward.register_awkward` will be removed in
+     ``pylhe`` ``v0.8.0``.
+    """
+    import warnings
+
+    warnings.warn(
+        "pylhe.awkward.register_awkward is deprecated as of pylhe v0.6.0 and will be removed in pylhe v0.8.0."
+        + " Please remove use of pylhe.awkward.register_awkward in favor of automatic registration.",
+        category=DeprecationWarning,
+        stacklevel=2,  # Raise to user level
+    )
 
 
 def to_awkward(event_iterable):
     """Convert iterable of LHEEvent instances to Awkward-Array."""
 
     builder = ak.ArrayBuilder()
     for event in event_iterable:
@@ -54,7 +63,14 @@
 
 class Event:
     pass
 
 
 class EventInfo:
     pass
+
+
+# Register Awkward behaviors
+vector.register_awkward()
+ak.mixin_class(ak.behavior)(Particle)
+ak.mixin_class(ak.behavior)(Event)
+ak.mixin_class(ak.behavior)(EventInfo)
```

### Comparing `pylhe-0.5.1/src/pylhe.egg-info/PKG-INFO` & `pylhe-0.6.0/src/pylhe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylhe
-Version: 0.5.1
+Version: 0.6.0
 Summary: small package to get structured data out of Les Houches Event files
 Home-page: https://github.com/scikit-hep/pylhe
 Author: Lukas Heinrich, Matthew Feickert, Eduardo Rodrigues
 Author-email: lukas.heinrich@cern.ch, matthew.feickert@cern.ch, eduardo.rodrigues@cern.ch
 License: Apache
 Project-URL: Source, https://github.com/scikit-hep/pylhe
 Project-URL: Tracker, https://github.com/scikit-hep/pylhe/issues
@@ -94,16 +94,16 @@
 ## Citation
 
 The preferred BibTeX entry for citation of `pylhe` is
 
 ```
 @software{pylhe,
   author = {Lukas Heinrich and Matthew Feickert and Eduardo Rodrigues},
-  title = "{pylhe: v0.5.1}",
-  version = {v0.5.1},
+  title = "{pylhe: v0.6.0}",
+  version = {v0.6.0},
   doi = {10.5281/zenodo.1217031},
   url = {https://github.com/scikit-hep/pylhe},
 }
 ```
 
 ## Contributors
```

