# Comparing `tmp/pylipd-1.2.4.tar.gz` & `tmp/pylipd-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylipd-1.2.4.tar", last modified: Tue Apr 11 10:36:03 2023, max compression
+gzip compressed data, was "pylipd-1.3.0.tar", last modified: Thu Apr 20 10:17:31 2023, max compression
```

## Comparing `pylipd-1.2.4.tar` & `pylipd-1.3.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 10:36:03.443864 pylipd-1.2.4/
--rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.2.4/LICENSE
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 10:36:03.443935 pylipd-1.2.4/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.2.4/README.md
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 10:36:03.441003 pylipd-1.2.4/pylipd/
--rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-11 10:33:50.000000 pylipd-1.2.4/pylipd/__init__.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 10:36:03.442242 pylipd-1.2.4/pylipd/globals/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.2.4/pylipd/globals/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)      409 2023-04-10 19:03:17.000000 pylipd-1.2.4/pylipd/globals/blacklist.py
--rw-r--r--   0 varun      (502) staff       (20)     3673 2023-04-11 06:17:21.000000 pylipd-1.2.4/pylipd/globals/queries.py
--rw-r--r--   0 varun      (502) staff       (20)    14643 2023-04-10 19:06:28.000000 pylipd-1.2.4/pylipd/globals/schema.py
--rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.2.4/pylipd/globals/urls.py
--rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.2.4/pylipd/legacy_utils.py
--rw-r--r--   0 varun      (502) staff       (20)    30850 2023-04-11 10:33:34.000000 pylipd-1.2.4/pylipd/lipd.py
--rw-r--r--   0 varun      (502) staff       (20)    43172 2023-04-11 03:12:51.000000 pylipd-1.2.4/pylipd/lipd_to_rdf.py
--rw-r--r--   0 varun      (502) staff       (20)     1576 2023-04-11 03:11:49.000000 pylipd-1.2.4/pylipd/multi_processing.py
--rw-r--r--   0 varun      (502) staff       (20)    22021 2023-04-11 03:13:16.000000 pylipd-1.2.4/pylipd/rdf_to_lipd.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 10:36:03.442579 pylipd-1.2.4/pylipd/series/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.2.4/pylipd/series/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.2.4/pylipd/series/regexes.py
--rw-r--r--   0 varun      (502) staff       (20)     2259 2023-04-11 05:52:03.000000 pylipd-1.2.4/pylipd/test.py
--rw-r--r--   0 varun      (502) staff       (20)     5306 2023-04-11 06:31:14.000000 pylipd-1.2.4/pylipd/usage.py
--rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.2.4/pylipd/utils.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 10:36:03.443742 pylipd-1.2.4/pylipd.egg-info/
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 10:36:03.000000 pylipd-1.2.4/pylipd.egg-info/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      616 2023-04-11 10:36:03.000000 pylipd-1.2.4/pylipd.egg-info/SOURCES.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-11 10:36:03.000000 pylipd-1.2.4/pylipd.egg-info/dependency_links.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.2.4/pylipd.egg-info/not-zip-safe
--rw-r--r--   0 varun      (502) staff       (20)       35 2023-04-11 10:36:03.000000 pylipd-1.2.4/pylipd.egg-info/requires.txt
--rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-11 10:36:03.000000 pylipd-1.2.4/pylipd.egg-info/top_level.txt
--rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.2.4/pyproject.toml
--rw-r--r--   0 varun      (502) staff       (20)      693 2023-04-11 10:36:03.444295 pylipd-1.2.4/setup.cfg
--rw-r--r--   0 varun      (502) staff       (20)      973 2023-04-11 10:33:44.000000 pylipd-1.2.4/setup.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:17:31.205015 pylipd-1.3.0/
+-rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.3.0/LICENSE
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-20 10:17:31.205069 pylipd-1.3.0/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.3.0/README.md
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:17:31.202684 pylipd-1.3.0/pylipd/
+-rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-20 04:53:08.000000 pylipd-1.3.0/pylipd/__init__.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:17:31.203736 pylipd-1.3.0/pylipd/globals/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.3.0/pylipd/globals/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)      436 2023-04-20 09:57:39.000000 pylipd-1.3.0/pylipd/globals/blacklist.py
+-rw-r--r--   0 varun      (502) staff       (20)     7357 2023-04-20 09:59:20.000000 pylipd-1.3.0/pylipd/globals/queries.py
+-rw-r--r--   0 varun      (502) staff       (20)    14792 2023-04-20 09:57:33.000000 pylipd-1.3.0/pylipd/globals/schema.py
+-rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.3.0/pylipd/globals/urls.py
+-rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.3.0/pylipd/legacy_utils.py
+-rw-r--r--   0 varun      (502) staff       (20)    28437 2023-04-20 07:49:40.000000 pylipd-1.3.0/pylipd/lipd.py
+-rw-r--r--   0 varun      (502) staff       (20)     3344 2023-04-20 10:09:20.000000 pylipd-1.3.0/pylipd/lipd_series.py
+-rw-r--r--   0 varun      (502) staff       (20)    43566 2023-04-20 10:00:23.000000 pylipd-1.3.0/pylipd/lipd_to_rdf.py
+-rw-r--r--   0 varun      (502) staff       (20)     3009 2023-04-20 07:46:48.000000 pylipd-1.3.0/pylipd/multi_processing.py
+-rw-r--r--   0 varun      (502) staff       (20)     9307 2023-04-20 06:36:28.000000 pylipd-1.3.0/pylipd/rdf_graph.py
+-rw-r--r--   0 varun      (502) staff       (20)    22181 2023-04-20 09:57:04.000000 pylipd-1.3.0/pylipd/rdf_to_lipd.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:17:31.203945 pylipd-1.3.0/pylipd/series/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.3.0/pylipd/series/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.3.0/pylipd/series/regexes.py
+-rw-r--r--   0 varun      (502) staff       (20)     2259 2023-04-11 05:52:03.000000 pylipd-1.3.0/pylipd/test.py
+-rw-r--r--   0 varun      (502) staff       (20)     6004 2023-04-20 10:15:46.000000 pylipd-1.3.0/pylipd/usage.py
+-rw-r--r--   0 varun      (502) staff       (20)      928 2023-04-20 10:13:54.000000 pylipd-1.3.0/pylipd/usage_parallel.py
+-rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.3.0/pylipd/utils.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:17:31.204895 pylipd-1.3.0/pylipd.egg-info/
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-20 10:17:31.000000 pylipd-1.3.0/pylipd.egg-info/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      689 2023-04-20 10:17:31.000000 pylipd-1.3.0/pylipd.egg-info/SOURCES.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-20 10:17:31.000000 pylipd-1.3.0/pylipd.egg-info/dependency_links.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.3.0/pylipd.egg-info/not-zip-safe
+-rw-r--r--   0 varun      (502) staff       (20)       40 2023-04-20 10:17:31.000000 pylipd-1.3.0/pylipd.egg-info/requires.txt
+-rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-20 10:17:31.000000 pylipd-1.3.0/pylipd.egg-info/top_level.txt
+-rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.3.0/pyproject.toml
+-rw-r--r--   0 varun      (502) staff       (20)      699 2023-04-20 10:17:31.205335 pylipd-1.3.0/setup.cfg
+-rw-r--r--   0 varun      (502) staff       (20)      989 2023-04-20 04:53:08.000000 pylipd-1.3.0/setup.py
```

### Comparing `pylipd-1.2.4/LICENSE` & `pylipd-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.4/PKG-INFO` & `pylipd-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.2.4
+Version: 1.3.0
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.2.4
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.0
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.2.4/README.md` & `pylipd-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.4/pylipd/globals/schema.py` & `pylipd-1.3.0/pylipd/globals/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,19 +261,21 @@
             '{variableName|name}'
         ],
         '@fromJson': [
             '_set_variable_category',
             '_wrap_uncertainty',
             '_create_proxy_system',
             '_add_found_in_table',
+            '_add_found_in_dataset',
             '_add_variable_values',
             '_stringify_column_numbers_array'
         ],
         '@toJson_pre': [
             '_remove_found_in_table',
+            '_remove_found_in_dataset',
             #'_remove_depth_property'
         ],
         '@toJson': [
             '_set_variable_type',
             '_unwrap_uncertainty',
             '_extract_from_proxy_system',
             '_extract_variable_values',
@@ -362,14 +364,17 @@
         },
         'hasValues': {
             'type': 'string'
         },
         'foundInTable': {
             'type': 'Individual'
         },
+        'foundInDataset': {
+            'type': 'Individual'
+        },
         'hasProxySystem': {
             'type': 'Individual'
         },
         'takenAtDepth': {
             'type': 'Individual'
         },
         'inCompilationBeta': {
```

### Comparing `pylipd-1.2.4/pylipd/legacy_utils.py` & `pylipd-1.3.0/pylipd/legacy_utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.4/pylipd/lipd.py` & `pylipd-1.3.0/pylipd/lipd.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 """
 The LiPD class describes a `LiPD (Linked Paleo Data) <https://cp.copernicus.org/articles/12/1093/2016/cp-12-1093-2016.html>`_ object. It contains an `RDF <https://www.w3.org/RDF/>`_ Graph which is serialization of the LiPD data into an RDF graph containing terms from the `LiPD Ontology <http://linked.earth/Ontology/release/core/1.2.0/index-en.html>`
 How to browse and query LiPD objects is described in a short example below, while `this notebook <https://nbviewer.jupyter.org/github/LinkedEarth/pylipd/blob/master/example_notebooks/pylipd_tutorial.ipynb>`_ demonstrates how to use PyLiPD to view and query LiPD datasets.
 """
 
-import math
 import os
-import pickle
 import re
-import copy
 import os.path
 import tempfile
 import pandas as pd
 import random
 import string
 import io
 
-from rdflib import ConjunctiveGraph, Namespace, URIRef
-from pylipd.globals.queries import QUERY_BIBLIO, QUERY_DSID, QUERY_DSNAME, QUERY_ENSEMBLE_TABLE
-from pylipd.multi_processing import multi_convert_to_pickle, multi_convert_to_rdf
+from rdflib import ConjunctiveGraph, URIRef
+from tqdm import tqdm
+from pylipd.globals.queries import QUERY_ALL_VARIABLES_GRAPH, QUERY_BIBLIO, QUERY_DSID, QUERY_DSNAME, QUERY_ENSEMBLE_TABLE, QUERY_ENSEMBLE_TABLE_SHORT, QUERY_FILTER_ARCHIVE_TYPE, QUERY_FILTER_GEO, QUERY_VARIABLE, QUERY_VARIABLE_GRAPH
+from pylipd.lipd_series import LiPDSeries
+from pylipd.multi_processing import multi_convert_to_rdf, multi_load_lipd
+from pylipd.rdf_graph import RDFGraph
 
 from pylipd.rdf_to_lipd import RDFToLiPD
 from pylipd.legacy_utils import LiPD_Legacy
-from pylipd.utils import sanitizeId, sparql_results_to_df
+from pylipd.utils import sanitizeId
 
 #import bibtexparser
 #from bibtexparser.bibdatabase import BibDatabase
 from doi2bib import crossref
 from pybtex.database import BibliographyData, Entry
 
-from .globals.urls import NSURL, ONTONS
+from .globals.urls import NSURL
 
-from copy import deepcopy
-
-
-class LiPD:
+class LiPD(RDFGraph):
     '''The LiPD class describes a `LiPD (Linked Paleo Data) <https://cp.copernicus.org/articles/12/1093/2016/cp-12-1093-2016.html>`_ object. It contains an `RDF <https://www.w3.org/RDF/>`_ Graph which is serialization of the LiPD data into an RDF graph containing terms from the `LiPD Ontology <http://linked.earth/Ontology/release/core/1.2.0/index-en.html>`
     How to browse and query LiPD objects is described in a short example below.
 
     Examples
     --------
     In this example, we read an online LiPD file and convert it into a time series object dictionary.
 
@@ -54,58 +51,18 @@
 
         for dsname, tsos in ts_list.items():
             for tso in tsos:
                 if 'paleoData_variableName' in tso:
                     print(dsname+': '+tso['paleoData_variableName']+': '+tso['archiveType'])
     '''
     def __init__(self, graph=None):
-        if graph is None:
-            self._initialize_graph()
-        else:
-            self.graph = graph
-
-    def _initialize_graph(self):
-        self.graph = ConjunctiveGraph()
-        self.graph.bind("le", Namespace(ONTONS))        
-        #self.graph.bind("", Namespace(NS))
-
-    def copy(self):
-        '''
-        Makes a copy of the object
-
-        Returns
-        -------
-        pylipd.LiPD
-            a copy of the original object
-
-        '''
-        
-        return deepcopy(self)
-
-    def merge(self, lipd):
-        '''
-        Merges the current LiPD object with another LiPD object
-
-        Parameters
-        ----------
-        lipd : pylipd.LiPD
-            LiPD object to merge with
-
-        Returns
-        -------
-        pylipd.LiPD
-            merged LiPD object
+        super().__init__(graph)
 
-        '''
-
-        merged = self.copy()
-        merged.graph.addN(lipd.graph.quads())
-        return merged
     
-    def load_from_dir(self, dir_path, parallel=False):
+    def load_from_dir(self, dir_path, parallel=False, cutoff=None):
         '''Load LiPD files from a directory
         Note: This function creates multiple process to process lipd files in parallel, therefore it is important that this call be made under the "__main__" process
 
         Parameters
         ----------
 
         dir_path : str
@@ -134,14 +91,16 @@
             return
 
         lipdfiles = []
         for path in os.listdir(dir_path):
             file_path = os.path.join(dir_path, path)
             if os.path.isfile(file_path) and path.endswith(".lpd"):
                 lipdfiles.append(file_path)
+        if cutoff:
+            lipdfiles = lipdfiles[0:cutoff]
         self.load(lipdfiles, parallel)
 
 
     # Allows loading http locations
     def load(self, lipdfiles, parallel=False):
         '''Load LiPD files. 
         Note: This function creates multiple process to process lipd files in parallel, therefore it is important that this call be made under the "__main__" process
@@ -175,72 +134,20 @@
             ])            
 
             print(lipd.get_all_dataset_names())
         '''        
         if type(lipdfiles) is not list:
             lipdfiles = [lipdfiles]
             
-        filemap = {}
-        for lipdfile in lipdfiles:
-            if not os.path.isfile(lipdfile) and not lipdfile.startswith("http"):
-                print(f"File {lipdfile} does not exist")
-                continue
-
-            picklefile = tempfile.NamedTemporaryFile().name
-            filemap[lipdfile] = picklefile
-        
-        print(f"Loading {len(filemap.keys())} LiPD files")
-        
-        multi_convert_to_pickle(filemap, parallel)
-        print("Conversion to RDF done..")
-
-        print("Loading RDF into graph")
-        for lipdfile in lipdfiles:
-            picklefile = filemap[lipdfile]
-            if os.path.exists(picklefile):
-                with open(picklefile, 'rb') as f:
-                    subgraph = pickle.load(f)
-                    self.graph.addN(subgraph.quads())
-                os.remove(picklefile)
+        numfiles = len(lipdfiles)
+        print(f"Loading {numfiles} LiPD files")
+        self.graph = multi_load_lipd(self.graph, lipdfiles, parallel)
         print("Loaded..")
 
 
-    def clear(self):
-        '''Clears the graph'''
-        self._initialize_graph()
-
-
-    def set_endpoint(self, endpoint):
-        '''Sets a SparQL endpoint for a remote Knowledge Base (example: GraphDB)
-
-        Parameters
-        ----------
-
-        endpoint : str
-            URL for the SparQL endpoint 
-
-        Examples
-        --------
-        
-        .. ipython:: python
-            :okwarning:
-            :okexcept:
-
-            from pylipd.lipd import LiPD
-
-            # Fetch LiPD data from remote RDF Graph
-            lipd_remote = LiPD()
-            lipd_remote.set_endpoint("https://linkedearth.graphdb.mint.isi.edu/repositories/LiPDVerse2")
-            lipd_remote.load_remote_datasets(["Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001", "MD98_2181.Stott.2007", "Ant-WAIS-Divide.Severinghaus.2012"])
-            print(lipd_remote.get_all_dataset_names())
-
-        '''
-        self.endpoint = endpoint
-
-
     def convert_lipd_dir_to_rdf(self, lipd_dir, rdf_file, parallel=False):
         '''Convert a directory containing LiPD files into a single RDF file (to be used for uploading to Knowledge Bases like GraphDB)
 
         Parameters
         ----------
 
         lipd_dir : str
@@ -287,84 +194,14 @@
                     fin.close()
                     fout.write(data)
                     os.remove(tmp_rdf_file)
             fout.close()
         print("Written..")
 
 
-    def query(self, query, remote=False, result="sparql"):
-        '''Once LiPD files or loaded into the graph (or remote endpoint set), one can make SparQL queries to the graph
-
-        Parameters
-        ----------
-
-        query : str
-            SparQL query
-
-        remote: bool
-            (Optional) If set to True, the query will be made to the remote endpoint (if set)
-
-        result : str
-            (Optional) Result return type
-
-        Returns
-        -------
-
-        result : dict
-            Dictionary of sparql variable and binding values
-        
-        result_df : pandas.Dataframe
-            Return the dictionary above as a pandas.Dataframe
-    
-        Examples
-        --------
-
-        .. ipython:: python
-            :okwarning:
-            :okexcept:
-
-            from pylipd.lipd import LiPD
-
-            lipd = LiPD()
-            lipd.load([
-                "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
-                "../examples/data/MD98_2181.Stott.2007.lpd"
-            ])
-            query = """PREFIX le: <http://linked.earth/ontology#>
-                    select (count(distinct ?ds) as ?count) where { 
-                        ?ds a le:Dataset .
-                        ?ds le:hasUrl ?url
-                    }"""
-            result, result_df = lipd.query(query)
-            result_df
-        '''
-
-        if remote and self.endpoint:
-            print("Making remote query to endpoint: " + self.endpoint)
-            matches = re.match(r"(.*)\s*SELECT\s+(.+)\s+WHERE\s+{(.+)}\s*(.*)", query, re.DOTALL | re.IGNORECASE)
-            if matches:
-                prefix = matches.group(1)
-                vars = matches.group(2)
-                where = matches.group(3)
-                suffix = matches.group(4)
-                query = f"{prefix} SELECT {vars} WHERE {{ SERVICE <{self.endpoint}> {{ {where} }} }} {suffix}"   
-        
-        result = self.graph.query(query)
-        result_df = sparql_results_to_df(result)
-        
-        return result, result_df 
-
-    # def whatArchive(self):
-        
-    #     archive_query = """PREFIX le: <http://linked.earth/ontology#>
-    #             select ?archiveType (count(distinct ?archiveType) as ?count) where { 
-    #                 ?ds a le:Dataset .
-    #                 ?ds le:hasUrl ?url
-    #             }"""
-
     def load_remote_datasets(self, dsnames):
         '''Loads remote datasets into cache if a remote endpoint is set
 
         Parameters
         ----------
 
         dsnames : array
@@ -693,137 +530,122 @@
             ])
             dsname = lipd.get_all_dataset_names()[0]
             lipd.create_lipd(dsname, "test.lpd")
         '''           
         converter = RDFToLiPD(self.graph)
         return converter.convert(dsname, lipdfile)
     
-    def pop(self, dsnames):
-        '''Pops dataset(s) from the graph and returns the popped LiPD object
 
+    def get(self, dsnames):
+        '''Gets dataset(s) from the graph and returns the popped LiPD object
         Parameters
         ----------
-
         dsnames : str or list of str
-            dataset name(s) to be popped.
+            dataset name(s) to get.
+        
+        Returns
+        -------
 
+        pylipd.lipd.LiPD
+            LiPD object with the retrieved dataset(s)
 
         Examples
         --------
-
         .. ipython:: python
             :okwarning:
             :okexcept:
 
             from pylipd.lipd import LiPD
 
             # Fetch LiPD data from remote RDF Graph
             lipd = LiPD()
             lipd.load([
                 "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
                 "../examples/data/MD98_2181.Stott.2007.lpd"
             ])
+
             all_datasets = lipd.get_all_dataset_names()
             print("Loaded datasets: " + str(all_datasets))
-            popped = lipd.pop(all_datasets[0])
-            print("Loaded datasets after pop: " + str(lipd.get_all_dataset_names()))
-            print("Popped dataset: " + str(popped.get_all_dataset_names()))       
+            ds = lipd.get(all_datasets[0])
+            print("Got dataset: " + str(ds.get_all_dataset_names()))       
         '''
+        dsnames = [dsnames] if type(dsnames) is not list else dsnames
+        dsids = [(f"{NSURL}/{dsname}" if not dsname.startswith(NSURL) else dsname) for dsname in dsnames]
 
-        popped = LiPD()
-
-        if type(dsnames) is not list:
-            dsnames = [dsnames]
-        
-        graphurls=[]
-        for dsname in dsnames:
-            graphurls.append(NSURL + "/" + dsname)
-
-        # Match subgraphs
-        for ctx in self.graph.contexts():
-            id = str(ctx.identifier)
-            if id in graphurls:
-                subgraph = copy.deepcopy(self.graph.get_context(id))
-                for triple in subgraph.triples((None, None, None)):
-                    popped.graph.add((
-                        triple[0],
-                        triple[1],
-                        triple[2],
-                        URIRef(id)))
+        ds = super().get(dsids)
+        return LiPD(ds.graph)
 
-                self.graph.remove((None, None, None, id))
+    def pop(self, dsnames):
+        '''Pops dataset(s) from the graph and returns the popped LiPD object
         
-        return popped
-
-    def remove(self, dsnames):
-        '''Removes dataset(s) from the graph
-
         Parameters
         ----------
-
         dsnames : str or list of str
-            dataset name(s) to be removed
+            dataset name(s) to be popped.
+        
+        Returns
+        -------
+
+        pylipd.lipd.LiPD
+            LiPD object with the popped dataset(s)
 
         Examples
         --------
-
         .. ipython:: python
             :okwarning:
             :okexcept:
-
             from pylipd.lipd import LiPD
-
             # Fetch LiPD data from remote RDF Graph
             lipd = LiPD()
             lipd.load([
                 "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
                 "../examples/data/MD98_2181.Stott.2007.lpd"
             ])
             all_datasets = lipd.get_all_dataset_names()
             print("Loaded datasets: " + str(all_datasets))
-            lipd.remove(all_datasets[0])
-            print("Loaded datasets after remove: " + str(lipd.get_all_dataset_names()))
+            popped = lipd.pop(all_datasets[0])
+            print("Loaded datasets after pop: " + str(lipd.get_all_dataset_names()))
+            print("Popped dataset: " + str(popped.get_all_dataset_names()))       
         '''
-        
-        if type(dsnames) is not list:
-            dsnames = [dsnames]
-        
-        graphurls=[]
-        for dsname in dsnames:
-            graphurls.append(NSURL + "/" + dsname)
 
-        # Match subgraphs
-        for ctx in self.graph.contexts():
-            id = str(ctx.identifier)
-            if id in graphurls:
-                self.graph.remove((None, None, None, id))       
+        dsnames = [dsnames] if type(dsnames) is not list else dsnames
+        dsids = [(f"{NSURL}/{dsname}" if not dsname.startswith(NSURL) else dsname) for dsname in dsnames]
+        popped = super().pop(dsids)
+        return LiPD(popped.graph)
 
-
-    def get_rdf(self):
-        '''Returns RDF serialization of the current Graph
+    def remove(self, dsnames):
+        '''Removes dataset(s) from the graph
+        
+        Parameters
+        ----------
+        dsnames : str or list of str
+            dataset name(s) to be removed
+        
         Examples
         --------
-
         .. ipython:: python
             :okwarning:
             :okexcept:
-
             from pylipd.lipd import LiPD
-
             # Fetch LiPD data from remote RDF Graph
             lipd = LiPD()
             lipd.load([
+                "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
                 "../examples/data/MD98_2181.Stott.2007.lpd"
             ])
-            nquads = lipd.get_rdf()
-            print(nquads[:10000])
-            print("...")
+            all_datasets = lipd.get_all_dataset_names()
+            print("Loaded datasets: " + str(all_datasets))
+            lipd.remove(all_datasets[0])
+            print("Loaded datasets after remove: " + str(lipd.get_all_dataset_names()))
         '''
         
-        return self.graph.serialize(format='nquads')
+        dsnames = [dsnames] if type(dsnames) is not list else dsnames
+        dsids = [(f"{NSURL}/{dsname}" if not dsname.startswith(NSURL) else dsname) for dsname in dsnames]
+
+        super().remove(dsids)
 
 
     def get_all_dataset_names(self):
         '''Get all Dataset Names
         
         Returns
         -------
@@ -877,42 +699,28 @@
                 "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
                 "../examples/data/MD98_2181.Stott.2007.lpd"
             ])
             print(lipd.get_all_dataset_ids())
         '''
         qres, qres_df = self.query(QUERY_DSID)
         return [sanitizeId(row.dsid) for row in qres]
-    
 
-    def search_datasets(variableName=[ ], archiveType=[ ], proxy=[ ], resolution = [ ],
-                    ageUnits = [ ], ageBound = [ ], ageBoundType = [ ], 
-                    lat = [ ], lon = [ ], alt = [ ], 
-                    print_response = True, download_lipd = True,
-                    download_folder = 'default'):
-        pass
 
-
-    def get_ensemble_tables(self, archiveType, varName, timeVarName, depthVarName, ensembleVarName, ensembleDepthVarName):
+    def get_ensemble_tables(self, dsname = None, ensembleVarName = None, ensembleDepthVarName = 'depth'):
         '''Gets ensemble tables from the LiPD graph
 
         Parameters
         ----------
 
-        archiveType : str
-            archive type (Set to ".*" to match all archive types)
-        varName : str
-            variable name (Set to ".*" to match all variable names)
-        timeVarName : str
-            time variable name (Set to ".*" to match all time variable names)
-        depthVarName : str
-            depth variable name (Set to ".*" to match all depth variable names)
-        ensembleVarName : str
-            ensemble variable name (Set to ".*" to match all ensemble variable names)
+        dsname : str
+            The name of the dataset if you wish to analyse one at a time (Set to ".*" to match all datasets with a common root)
+        ensembleVarName : None or str
+            ensemble variable name. Default is None, which searches for names that contain "year" or "age" (Set to ".*" to match all ensemble variable names)
         ensembleDepthVarName : str
-            ensemble depth variable name (Set to ".*" to match all ensemble depth variable names)
+            ensemble depth variable name. Default is 'depth' (Set to ".*" to match all ensemble depth variable names)
 
         Returns
         -------
 
         ensemble_tables : dataframe
             A dataframe containing the ensemble tables
 
@@ -930,29 +738,126 @@
             lipd.load([
                 "../examples/data/ODP846.Lawrence.2006.lpd"
             ])
             all_datasets = lipd.get_all_dataset_names()
             print("Loaded datasets: " + str(all_datasets))
 
             ens_df = lipd.get_ensemble_tables(
-                archiveType=".*",
-                varName="c37",
-                timeVarName="age",
-                depthVarName="depth",
                 ensembleVarName="age",
                 ensembleDepthVarName="depth"
             )
             print("Ensemble tables:")
             print(ens_df)
         '''
+        
+        if dsname is None:
+            dsname = ''
+        
+        if ensembleVarName is None:
+            query = QUERY_ENSEMBLE_TABLE_SHORT
+            query = query.replace("[dsname]", dsname)
+            query = query.replace("[ensembleDepthVarName]", ensembleDepthVarName)
+        
+        else:
        
-        query = QUERY_ENSEMBLE_TABLE
-        query = query.replace("[archiveType]", archiveType)
-        query = query.replace("[varName]", varName)
-        query = query.replace("[timeVarName]", timeVarName)
-        query = query.replace("[depthVarName]", depthVarName)
-        query = query.replace("[ensembleVarName]", ensembleVarName)
-        query = query.replace("[ensembleDepthVarName]", ensembleDepthVarName)
+            query = QUERY_ENSEMBLE_TABLE
+            query = query.replace("[dsname]", dsname)
+            query = query.replace("[ensembleVarName]", ensembleVarName)
+            query = query.replace("[ensembleDepthVarName]", ensembleDepthVarName)
 
         qres, qres_df = self.query(query)
         return qres_df
 
+
+    def get_all_variables(self):
+        '''
+        Returns a list of all variables in the graph
+        
+        Returns
+        -------
+
+        pandas.DataFrame
+            A dataframe of all variables in the graph with columns uri, varid, varname
+
+        '''
+        return self.query(QUERY_VARIABLE)[1]
+
+
+    def to_lipd_series(self, parallel=False):
+        '''
+        Converts the LiPD object to a LiPDSeries object
+
+        Parameters
+        ----------
+        parallel : bool
+            Whether to use parallel processing to load the data. Default is False
+
+        Returns
+        -------
+        pylipd.lipd.LiPDSeries
+            A LiPDSeries object
+
+        '''
+        S = LiPDSeries()    
+        S.load(self, parallel)
+        return S
+
+
+    # bbox = left,bottom,right,top
+    # bbox = min Longitude , min Latitude , max Longitude , max Latitude 
+    def filter_by_geo_bbox(self, lonMin, latMin, lonMax, latMax):
+        '''
+        Filters datasets to return a new LiPD object that only keeps datasets that fall within the bounding box
+
+        Parameters
+        ----------
+        lonMin : float
+            Minimum longitude
+
+        latMin : float
+            Minimum latitude
+        
+        lonMax : float
+            Maximum longitude
+
+        latMax : float
+            Maximum latitude
+
+        Returns
+        -------
+
+        pylipd.lipd.LiPD
+            A new LiPD object that only contains datasets that fall within the bounding box
+
+        '''
+        query = QUERY_FILTER_GEO
+        query = query.replace("[lonMin]", str(lonMin))
+        query = query.replace("[latMin]", str(latMin))
+        query = query.replace("[lonMax]", str(lonMax))               
+        query = query.replace("[latMax]", str(latMax))
+        qres, qres_df = self.query(query)
+        dsnames = [sanitizeId(row.dsname) for row in qres]
+        return self.get(dsnames)
+
+
+    def filter_by_archive_type(self, archiveType):
+        '''
+        Filters datasets to return a new LiPD object that only keeps datasets that have the specified archive type
+
+        Parameters
+        ----------
+
+        archiveType : str
+            The archive type to filter by
+
+        Returns
+        -------
+        
+        pylipd.lipd.LiPD
+            A new LiPD object that only contains datasets that have the specified archive type (regex)
+
+        '''
+        query = QUERY_FILTER_ARCHIVE_TYPE
+        query = query.replace("[archiveType]", archiveType)
+        qres, qres_df = self.query(query)
+        dsnames = [sanitizeId(row.dsname) for row in qres]
+        return self.get(dsnames)
```

### Comparing `pylipd-1.2.4/pylipd/lipd_to_rdf.py` & `pylipd-1.3.0/pylipd/lipd_to_rdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,34 +32,28 @@
     It uses the SCHEMA dictionary (from globals/schema.py) to do the conversion
     """
 
     def __init__(self):
         self.graph = ConjunctiveGraph()
         self.lipd_csvs = {}
         self.graphurl = NSURL
-        self.namespace = NSURL + "#"
+        self.namespace = NSURL + "/"
         self.schema = expand_schema(copy.deepcopy(SCHEMA))  
 
 
-    def convert(self, lipdpath, topath, type="rdf"):
-        '''Convert LiPD file to RDF (or Pickled Graph)
+    def convert(self, lipdpath):
+        '''Convert LiPD file to RDF Graph
 
         Parameters
         ----------
 
         lipdpath : str
             path to lipd file (the path could also be a url)
 
-        topath : str
-            path to the output file
-
-        type : str
-            the output file type : rdf or pickle (we store the pickled rdf graph for efficiency sometimes)
         '''
-
         self.graph = ConjunctiveGraph()
         
         lpdname = os.path.basename(lipdpath).replace(".lpd", "")
         lpdname = re.sub("\?.+$", "", lpdname)
 
         self.graphurl = NSURL + "/" + lpdname
 
@@ -70,20 +64,36 @@
                 jsondir = os.path.dirname(jsonpath)
                 csvs = self._find_files_with_extension(jsondir, 'csv')
                 self.lipd_csvs = {}
                 for csvpath, _ in csvs:
                     csvname = os.path.basename(csvpath)        
                     self.lipd_csvs[csvname] = pd.read_csv(csvpath, header=None)
                 self._load_lipd_json_to_graph(jsonpath)                    
-                
-                if type == "rdf":
-                    self.graph.serialize(topath, format="nquads", encoding="utf-8")
-                elif type == "pickle":
-                    with open(topath, 'wb') as f:
-                        pickle.dump(self.graph, f)
+
+
+    def serialize(self, topath, type="rdf"):
+        '''Write LiPD RDF Graph to RDF file (or Pickle file)
+
+        Parameters
+        ----------
+
+        topath : str
+            path to the output file
+
+        type : str
+            the output file type : rdf or pickle (we store the pickled rdf graph for efficiency sometimes)
+        '''
+
+        if self.graph:
+            if type == "rdf":
+                self.graph.serialize(topath, format="nquads", encoding="utf-8")
+            elif type == "pickle":
+                with open(topath, 'wb') as f:
+                    pickle.dump(self.graph, f)
+
 
     def _unzip_lipd_file(self, lipdfile, unzipdir):
         if lipdfile.startswith("http"):
             # If this is a URL
             # Handle special characters in url (if any)
             res = urlparse(lipdfile)
             lipdurl = urlunparse(res._replace(path=quote(res.path)))
@@ -613,14 +623,23 @@
         
         return [obj, objhash, []]
     
     def _add_found_in_table(self, obj, objhash) :
         obj["foundInTable"] = obj["@parent"]["@id"]
         return [obj, objhash, []]
     
+    def _add_found_in_dataset(self, obj, objhash) :
+        parent = obj["@parent"]
+        top = parent
+        while (parent) :
+            top = parent
+            parent = parent["@parent"]
+        obj["foundInDataset"] = top["@id"]
+        return [obj, objhash, []]
+        
     # Unroll the list to a rdf first/rest structure
     def _unroll_values_list_to_rdf(self, lst: list, dtype):
         listitems = []
         for idx, item in enumerate(lst):
             listitems.append(Literal(item, datatype=(XSD[dtype] if dtype in XSD else None)))
 
         listid = BNode()
```

### Comparing `pylipd-1.2.4/pylipd/rdf_to_lipd.py` & `pylipd-1.3.0/pylipd/rdf_to_lipd.py`

 * *Files 1% similar despite different names*

```diff
@@ -449,14 +449,19 @@
         return url.replace("https://docs.google.com/spreadsheets/d/", "")
 
     def _remove_found_in_table(self, var, parent = None) :
         if "foundInTable" in var :
             del var["foundInTable"]
         return var
 
+    def _remove_found_in_dataset(self, var, parent = None) :
+        if "foundInDataset" in var :
+            del var["foundInDataset"]
+        return var
+    
     def __get_variable_archive_types(self, item, atypes) :
         if type(item) is dict:
             nitem = {}
             for key,value in item.items() :
                 if (key == "archiveType") :
                     atypes[value] = 1
                 else :
```

### Comparing `pylipd-1.2.4/pylipd/series/regexes.py` & `pylipd-1.3.0/pylipd/series/regexes.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.4/pylipd/test.py` & `pylipd-1.3.0/pylipd/test.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.4/pylipd/usage.py` & `pylipd-1.3.0/pylipd/usage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pylipd.lipd import LiPD
 import json
+from pylipd.lipd_series import LiPDSeries
 from pylipd.multi_processing import convert_to_rdf
 
 ####################
 # TODO:
 # - Edit local LiPD & update endpoint
 ####################
 
@@ -45,45 +46,73 @@
 
 # Load Datasets (from Local and Remote)
 dsnames = ["MD98_2181.Stott.2007"]
 remote_dsnames = ["Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001"]
 
 '''
 L = LiPD()
+
 #L.load(local_lipd_dir+"/"+"ODP1671017E.lpd")
 #L.set_endpoint("https://linkedearth.graphdb.mint.isi.edu/repositories/LiPDVerse2")    
 L.load([local_lipd_dir + "/" + dsname + ".lpd" for dsname in ["MD98_2181.Stott.2007","NAm-SmithersSkiArea.Schweingruber.1996", 
                         "NAm-CeaderBreaks.Briffa.1996", "ODP1671017E", 
                         "SPC14.Kahle.2021", "RC12-10.Poore.2003", 
-                        "MD02-2553.Poore.2009", "AD9117.Guinta.2001",
+                        "MD02-2553.Poore.2009", "AD9117.Guinta.2001", "SP10BEIN",
                         "SchellingsBog.Barron.2004", "Hidden.Tang.1999"]])
 #bibtex = L.get_bibtex()
 #print(bibtex)
 #exit()
+
+S = LiPDSeries()
+S.load(L)
+
+print(S)
+
+exit()
 '''
 
 # Load from local
 lipd = LiPD()
-lipdfiles = [local_lipd_dir + "/" + dsname + ".lpd" for dsname in dsnames]
+data_path = local_lipd_dir + '/Ocn-Palmyra.Nurhati.2011.lpd'
+lipd.load(data_path)
+print(lipd.get_all_dataset_names())
+
+#lipdfiles = [local_lipd_dir + "/" + dsname + ".lpd" for dsname in dsnames]
 #print(lipdfiles)
 
 #lipd.load(lipdfiles)
 lipd.load_from_dir("examples/data")
 print(lipd.get_all_dataset_names())
+
+lat = -77.08
+lon = 38.91
+radius = 50
+
+(result, result_df) = lipd.query("""
+PREFIX geo: <http://www.opengis.net/ont/geosparql#>
+PREFIX geof: <http://www.opengis.net/def/function/geosparql/>
+PREFIX wgs84: <http://www.w3.org/2003/01/geo/wgs84_pos#>
+
+SELECT ?what
+WHERE {
+  ?ds wgs84:lat ?lat .
+  ?ds wgs84:lon ?lon .
+  
+  FILTER(geof:sfWithin(?geometry,
+     "POLYGON((-77.089005 38.913574,-77.029953 38.913574,-77.029953 38.886321,-77.089005 38.886321,-77.089005 38.913574))"^^geo:wktLiteral))
+}
+""")
+
 #print(lipd.get_all_dataset_ids())
 ens_df = lipd.get_ensemble_tables(
-    archiveType=".*",
-    varName="c37",
-    timeVarName="age",
-    depthVarName="depth",
     ensembleVarName="age",
     ensembleDepthVarName="depth"
 )
 print(ens_df)
-exit()
+
 
 #lipd.load(["/Users/varun/Downloads/Arc-LakeNataujärvi.Ojala.2005.lpd"])
 #print(lipd.get_all_dataset_names())
 
 ts_list = lipd.get_timeseries(lipd.get_all_dataset_names())
 for dsname, tsos in ts_list.items():
     for tso in tsos:
@@ -117,16 +146,19 @@
 lpd2 = LiPD()
 lpd2.load([lipdfile])
 ts_list_remote = lpd2.get_timeseries(lpd2.get_all_dataset_names())
 for dsname, tsos in ts_list_remote.items():
     for tso in tsos:
         print(dsname+': '+str(tso['paleoData_variableName'])+': '+tso['archiveType'])
 
-print(lpd2.get_ensemble_tables())
-exit()
+ens_df2 = lpd2.get_ensemble_tables(
+    ensembleVarName="age",
+    ensembleDepthVarName="depth"
+)
+print(ens_df2)
 
 print("After popping..")
 print(lipd.get_all_dataset_names())
 ts_list_remote = lipd.get_timeseries(lipd.get_all_dataset_names())
 for dsname, tsos in ts_list_remote.items():
     for tso in tsos:
         print(dsname+': '+str(tso['paleoData_variableName'])+': '+tso['archiveType'])
```

### Comparing `pylipd-1.2.4/pylipd/utils.py` & `pylipd-1.3.0/pylipd/utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.4/pylipd.egg-info/PKG-INFO` & `pylipd-1.3.0/pylipd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.2.4
+Version: 1.3.0
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.2.4
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.0
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.2.4/pylipd.egg-info/SOURCES.txt` & `pylipd-1.3.0/pylipd.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 ./pylipd/__init__.py
 ./pylipd/legacy_utils.py
 ./pylipd/lipd.py
+./pylipd/lipd_series.py
 ./pylipd/lipd_to_rdf.py
 ./pylipd/multi_processing.py
+./pylipd/rdf_graph.py
 ./pylipd/rdf_to_lipd.py
 ./pylipd/test.py
 ./pylipd/usage.py
+./pylipd/usage_parallel.py
 ./pylipd/utils.py
 ./pylipd/globals/__init__.py
 ./pylipd/globals/blacklist.py
 ./pylipd/globals/queries.py
 ./pylipd/globals/schema.py
 ./pylipd/globals/urls.py
 ./pylipd/series/__init__.py
```

### Comparing `pylipd-1.2.4/setup.cfg` & `pylipd-1.3.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylipd
-version = 1.2.4
+version = 1.3.0
 author = Varun Ratnakar
 author_email = varunratnakar@gmail.com
 description = Python utilities for handling LiPD data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/linkedearth/pylipd
 project_urls = 
@@ -20,14 +20,15 @@
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	rdflib
 	pandas
 	doi2bib
 	pybtex
+	tqdm
 	bagit
 
 [options.packages.find]
 where = .
 
 [egg_info]
 tag_build =
```

### Comparing `pylipd-1.2.4/setup.py` & `pylipd-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import setup, find_packages
 
 
-version = '1.2.4'
+version = '1.3.0'
 
 # Read the readme file contents into variable
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pylipd',
@@ -27,11 +27,12 @@
     package_dir = {'':'.'},
     classifiers=[],
     install_requires=[
         "rdflib",
         "pandas",
         "doi2bib",
         "pybtex",
+        "tqdm",
         "bagit"
     ],
     python_requires=">=3.9.0"
 )
```

