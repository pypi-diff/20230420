# Comparing `tmp/pylipd-1.3.0.tar.gz` & `tmp/pylipd-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylipd-1.3.0.tar", last modified: Thu Apr 20 10:17:31 2023, max compression
+gzip compressed data, was "pylipd-1.3.1.tar", last modified: Thu Apr 20 10:42:32 2023, max compression
```

## Comparing `pylipd-1.3.0.tar` & `pylipd-1.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:17:31.205015 pylipd-1.3.0/
--rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.3.0/LICENSE
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-20 10:17:31.205069 pylipd-1.3.0/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.3.0/README.md
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:17:31.202684 pylipd-1.3.0/pylipd/
--rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-20 04:53:08.000000 pylipd-1.3.0/pylipd/__init__.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:17:31.203736 pylipd-1.3.0/pylipd/globals/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.3.0/pylipd/globals/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)      436 2023-04-20 09:57:39.000000 pylipd-1.3.0/pylipd/globals/blacklist.py
--rw-r--r--   0 varun      (502) staff       (20)     7357 2023-04-20 09:59:20.000000 pylipd-1.3.0/pylipd/globals/queries.py
--rw-r--r--   0 varun      (502) staff       (20)    14792 2023-04-20 09:57:33.000000 pylipd-1.3.0/pylipd/globals/schema.py
--rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.3.0/pylipd/globals/urls.py
--rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.3.0/pylipd/legacy_utils.py
--rw-r--r--   0 varun      (502) staff       (20)    28437 2023-04-20 07:49:40.000000 pylipd-1.3.0/pylipd/lipd.py
--rw-r--r--   0 varun      (502) staff       (20)     3344 2023-04-20 10:09:20.000000 pylipd-1.3.0/pylipd/lipd_series.py
--rw-r--r--   0 varun      (502) staff       (20)    43566 2023-04-20 10:00:23.000000 pylipd-1.3.0/pylipd/lipd_to_rdf.py
--rw-r--r--   0 varun      (502) staff       (20)     3009 2023-04-20 07:46:48.000000 pylipd-1.3.0/pylipd/multi_processing.py
--rw-r--r--   0 varun      (502) staff       (20)     9307 2023-04-20 06:36:28.000000 pylipd-1.3.0/pylipd/rdf_graph.py
--rw-r--r--   0 varun      (502) staff       (20)    22181 2023-04-20 09:57:04.000000 pylipd-1.3.0/pylipd/rdf_to_lipd.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:17:31.203945 pylipd-1.3.0/pylipd/series/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.3.0/pylipd/series/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.3.0/pylipd/series/regexes.py
--rw-r--r--   0 varun      (502) staff       (20)     2259 2023-04-11 05:52:03.000000 pylipd-1.3.0/pylipd/test.py
--rw-r--r--   0 varun      (502) staff       (20)     6004 2023-04-20 10:15:46.000000 pylipd-1.3.0/pylipd/usage.py
--rw-r--r--   0 varun      (502) staff       (20)      928 2023-04-20 10:13:54.000000 pylipd-1.3.0/pylipd/usage_parallel.py
--rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.3.0/pylipd/utils.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:17:31.204895 pylipd-1.3.0/pylipd.egg-info/
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-20 10:17:31.000000 pylipd-1.3.0/pylipd.egg-info/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      689 2023-04-20 10:17:31.000000 pylipd-1.3.0/pylipd.egg-info/SOURCES.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-20 10:17:31.000000 pylipd-1.3.0/pylipd.egg-info/dependency_links.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.3.0/pylipd.egg-info/not-zip-safe
--rw-r--r--   0 varun      (502) staff       (20)       40 2023-04-20 10:17:31.000000 pylipd-1.3.0/pylipd.egg-info/requires.txt
--rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-20 10:17:31.000000 pylipd-1.3.0/pylipd.egg-info/top_level.txt
--rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.3.0/pyproject.toml
--rw-r--r--   0 varun      (502) staff       (20)      699 2023-04-20 10:17:31.205335 pylipd-1.3.0/setup.cfg
--rw-r--r--   0 varun      (502) staff       (20)      989 2023-04-20 04:53:08.000000 pylipd-1.3.0/setup.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:42:32.584532 pylipd-1.3.1/
+-rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.3.1/LICENSE
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-20 10:42:32.584582 pylipd-1.3.1/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.3.1/README.md
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:42:32.582030 pylipd-1.3.1/pylipd/
+-rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-20 10:37:56.000000 pylipd-1.3.1/pylipd/__init__.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:42:32.583072 pylipd-1.3.1/pylipd/globals/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.3.1/pylipd/globals/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)      436 2023-04-20 09:57:39.000000 pylipd-1.3.1/pylipd/globals/blacklist.py
+-rw-r--r--   0 varun      (502) staff       (20)     7357 2023-04-20 09:59:20.000000 pylipd-1.3.1/pylipd/globals/queries.py
+-rw-r--r--   0 varun      (502) staff       (20)    14792 2023-04-20 09:57:33.000000 pylipd-1.3.1/pylipd/globals/schema.py
+-rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.3.1/pylipd/globals/urls.py
+-rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.3.1/pylipd/legacy_utils.py
+-rw-r--r--   0 varun      (502) staff       (20)    28453 2023-04-20 10:40:15.000000 pylipd-1.3.1/pylipd/lipd.py
+-rw-r--r--   0 varun      (502) staff       (20)     3349 2023-04-20 10:37:20.000000 pylipd-1.3.1/pylipd/lipd_series.py
+-rw-r--r--   0 varun      (502) staff       (20)    43566 2023-04-20 10:00:23.000000 pylipd-1.3.1/pylipd/lipd_to_rdf.py
+-rw-r--r--   0 varun      (502) staff       (20)     3009 2023-04-20 07:46:48.000000 pylipd-1.3.1/pylipd/multi_processing.py
+-rw-r--r--   0 varun      (502) staff       (20)     9324 2023-04-20 10:34:40.000000 pylipd-1.3.1/pylipd/rdf_graph.py
+-rw-r--r--   0 varun      (502) staff       (20)    22181 2023-04-20 09:57:04.000000 pylipd-1.3.1/pylipd/rdf_to_lipd.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:42:32.583417 pylipd-1.3.1/pylipd/series/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.3.1/pylipd/series/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.3.1/pylipd/series/regexes.py
+-rw-r--r--   0 varun      (502) staff       (20)     2259 2023-04-11 05:52:03.000000 pylipd-1.3.1/pylipd/test.py
+-rw-r--r--   0 varun      (502) staff       (20)     6004 2023-04-20 10:15:46.000000 pylipd-1.3.1/pylipd/usage.py
+-rw-r--r--   0 varun      (502) staff       (20)      928 2023-04-20 10:13:54.000000 pylipd-1.3.1/pylipd/usage_parallel.py
+-rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.3.1/pylipd/utils.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:42:32.584433 pylipd-1.3.1/pylipd.egg-info/
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-20 10:42:32.000000 pylipd-1.3.1/pylipd.egg-info/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      689 2023-04-20 10:42:32.000000 pylipd-1.3.1/pylipd.egg-info/SOURCES.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-20 10:42:32.000000 pylipd-1.3.1/pylipd.egg-info/dependency_links.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.3.1/pylipd.egg-info/not-zip-safe
+-rw-r--r--   0 varun      (502) staff       (20)       40 2023-04-20 10:42:32.000000 pylipd-1.3.1/pylipd.egg-info/requires.txt
+-rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-20 10:42:32.000000 pylipd-1.3.1/pylipd.egg-info/top_level.txt
+-rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.3.1/pyproject.toml
+-rw-r--r--   0 varun      (502) staff       (20)      699 2023-04-20 10:42:32.584840 pylipd-1.3.1/setup.cfg
+-rw-r--r--   0 varun      (502) staff       (20)      989 2023-04-20 10:37:46.000000 pylipd-1.3.1/setup.py
```

### Comparing `pylipd-1.3.0/LICENSE` & `pylipd-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.0/PKG-INFO` & `pylipd-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.0
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.1
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.3.0/README.md` & `pylipd-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.0/pylipd/globals/queries.py` & `pylipd-1.3.1/pylipd/globals/queries.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.0/pylipd/globals/schema.py` & `pylipd-1.3.1/pylipd/globals/schema.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.0/pylipd/legacy_utils.py` & `pylipd-1.3.1/pylipd/legacy_utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.0/pylipd/lipd.py` & `pylipd-1.3.1/pylipd/lipd.py`

 * *Files 0% similar despite different names*

```diff
@@ -589,15 +589,17 @@
             LiPD object with the popped dataset(s)
 
         Examples
         --------
         .. ipython:: python
             :okwarning:
             :okexcept:
+
             from pylipd.lipd import LiPD
+
             # Fetch LiPD data from remote RDF Graph
             lipd = LiPD()
             lipd.load([
                 "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
                 "../examples/data/MD98_2181.Stott.2007.lpd"
             ])
             all_datasets = lipd.get_all_dataset_names()
@@ -621,15 +623,17 @@
             dataset name(s) to be removed
         
         Examples
         --------
         .. ipython:: python
             :okwarning:
             :okexcept:
+
             from pylipd.lipd import LiPD
+            
             # Fetch LiPD data from remote RDF Graph
             lipd = LiPD()
             lipd.load([
                 "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
                 "../examples/data/MD98_2181.Stott.2007.lpd"
             ])
             all_datasets = lipd.get_all_dataset_names()
```

### Comparing `pylipd-1.3.0/pylipd/lipd_series.py` & `pylipd-1.3.1/pylipd/lipd_series.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         :okwarning:
         :okexcept:
 
         from pylipd.lipd_series import LiPDSeries
 
         lipd = LiPD()
         lipd.load(["https://lipdverse.org/data/LCf20b99dfe8d78840ca60dfb1f832b9ec/1_0_1//Nunalleq.Ledger.2018.lpd"])
-        lipd_series = lipd.to_series()
+        lipd_series = lipd.to_lipd_series()
     '''
     def __init__(self, graph=None):
         super().__init__(graph)
         self.lipds = {}
 
 
     def load(self, lipd, parallel=False):
```

### Comparing `pylipd-1.3.0/pylipd/lipd_to_rdf.py` & `pylipd-1.3.1/pylipd/lipd_to_rdf.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.0/pylipd/multi_processing.py` & `pylipd-1.3.1/pylipd/multi_processing.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.0/pylipd/rdf_graph.py` & `pylipd-1.3.1/pylipd/rdf_graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         :okwarning:
         :okexcept:
 
         from pylipd.rdf_graph import RDFGraph
 
         # Load RDF file into graph
         rdf = RDFGraph()
-        rdf.load(["examples/rdf/graph.rdf"])
+        rdf.load(["../examples/rdf/graph.ttl"])
         (result, result_df) = rdf.query("SELECT ?s ?p ?o WHERE {?s ?p ?o} LIMIT 10")
         result_df    
 
     '''
 
     def __init__(self, graph=None):
         if graph is None:
@@ -58,15 +58,15 @@
             :okwarning:
             :okexcept:
 
             from pylipd.rdf_graph import RDFGraph
 
             # Load RDF file into graph
             rdf = RDFGraph()
-            rdf.load(["examples/data/graph.rdf"])
+            rdf.load(["../examples/rdf/graph.ttl"])
             (result, result_df) = rdf.query("SELECT ?s ?p ?o WHERE {?s ?p ?o} LIMIT 10")
             result_df
         '''
 
         for file in files:
             self.graph.parse(file, publicID=graphid)
 
@@ -166,15 +166,15 @@
         .. ipython:: python
             :okwarning:
             :okexcept:
 
             from pylipd.rdf_graph import RDFGraph
 
             rdf = RDFGraph()
-            rdf.load(["examples/data/graph.rdf"])
+            rdf.load(["../examples/rdf/graph.ttl"])
             query = """PREFIX le: <http://linked.earth/ontology#>
                     select ?s ?p ?o where { 
                         ?s ?p ?o 
                     } LIMIT 10 """
             result, result_df = rdf.query(query)
             result_df
         '''
@@ -210,15 +210,15 @@
             :okwarning:
             :okexcept:
 
             from pylipd.rdf_graph import RDFGraph
 
             # Remove RDF graph data for given id(s)
             rdf = RDFGraph()
-            rdf.load(["examples/data/graph.rdf"], graphid="http://example.org/graph")
+            rdf.load(["../examples/rdf/graph.ttl"], graphid="http://example.org/graph")
             rdf.remove("http://example.org/graph")
         '''
         
         if type(ids) is not list:
             ids = [ids]
 
         # Match subgraphs
@@ -250,15 +250,15 @@
             :okwarning:
             :okexcept:
 
             from pylipd.rdf_graph import RDFGraph
 
             # Fetch RDF graph data for given id(s)
             rdf = RDFGraph()
-            rdf.load(["examples/data/graph.rdf"], graphid="http://example.org/graph")
+            rdf.load(["../examples/rdf/graph.ttl"], graphid="http://example.org/graph")
             rdf.get("http://example.org/graph")  
         '''
 
         graphds = RDFGraph()
 
         if type(ids) is not list:
             ids = [ids]
@@ -298,15 +298,15 @@
             :okwarning:
             :okexcept:
 
             from pylipd.rdf_graph import RDFGraph
 
             # Pop RDF graph data for given id(s)
             rdf = RDFGraph()
-            rdf.load(["examples/data/graph.rdf"], graphid="http://example.org/graph")
+            rdf.load(["../examples/rdf/graph.ttl"], graphid="http://example.org/graph")
             popped = rdf.pop("http://example.org/graph")      
         '''
 
         popped = self.get(ids)
         self.remove(ids)
         
         return popped
@@ -329,15 +329,15 @@
             :okwarning:
             :okexcept:
 
             from pylipd.rdf_graph import RDFGraph
 
             # Fetch RDF Graph Data
             rdf = RDFGraph()
-            rdf.load(["examples/data/graph.rdf"], graphid="http://example.org/graph")
+            rdf.load(["../examples/rdf/graph.ttl"], graphid="http://example.org/graph")
             print(rdf.get_all_graph_ids())
         '''        
         ids = [str(ctx.identifier) for ctx in self.graph.contexts()]
         return ids
     
 
     def serialize(self):
@@ -349,14 +349,14 @@
             :okwarning:
             :okexcept:
 
             from pylipd.rdf_graph import RDFGraph
 
             # Fetch RDF data
             rdf = RDFGraph()
-            rdf.load(["examples/data/graph.rdf"], graphid="http://example.org/graph")
+            rdf.load(["../examples/rdf/graph.ttl"], graphid="http://example.org/graph")
             nquads = rdf.serialize()
             print(nquads[:10000])
             print("...")
         '''
         
         return self.graph.serialize(format='nquads')
```

### Comparing `pylipd-1.3.0/pylipd/rdf_to_lipd.py` & `pylipd-1.3.1/pylipd/rdf_to_lipd.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.0/pylipd/series/regexes.py` & `pylipd-1.3.1/pylipd/series/regexes.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.0/pylipd/test.py` & `pylipd-1.3.1/pylipd/test.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.0/pylipd/usage.py` & `pylipd-1.3.1/pylipd/usage.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.0/pylipd/usage_parallel.py` & `pylipd-1.3.1/pylipd/usage_parallel.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.0/pylipd/utils.py` & `pylipd-1.3.1/pylipd/utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.0/pylipd.egg-info/PKG-INFO` & `pylipd-1.3.1/pylipd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.0
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.1
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.3.0/pylipd.egg-info/SOURCES.txt` & `pylipd-1.3.1/pylipd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.0/setup.cfg` & `pylipd-1.3.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylipd
-version = 1.3.0
+version = 1.3.1
 author = Varun Ratnakar
 author_email = varunratnakar@gmail.com
 description = Python utilities for handling LiPD data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/linkedearth/pylipd
 project_urls =
```

### Comparing `pylipd-1.3.0/setup.py` & `pylipd-1.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import setup, find_packages
 
 
-version = '1.3.0'
+version = '1.3.1'
 
 # Read the readme file contents into variable
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pylipd',
```

