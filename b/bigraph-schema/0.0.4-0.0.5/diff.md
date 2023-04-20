# Comparing `tmp/bigraph-schema-0.0.4.tar.gz` & `tmp/bigraph-schema-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigraph-schema-0.0.4.tar", last modified: Thu Apr 20 03:25:06 2023, max compression
+gzip compressed data, was "bigraph-schema-0.0.5.tar", last modified: Thu Apr 20 03:37:58 2023, max compression
```

## Comparing `bigraph-schema-0.0.4.tar` & `bigraph-schema-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-20 03:25:06.483024 bigraph-schema-0.0.4/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1081 2023-04-20 03:25:06.483024 bigraph-schema-0.0.4/PKG-INFO
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      151 2023-04-11 21:38:33.000000 bigraph-schema-0.0.4/README.md
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-20 03:25:06.483024 bigraph-schema-0.0.4/bigraph_schema/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      106 2023-04-19 21:19:48.000000 bigraph-schema-0.0.4/bigraph_schema/__init__.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2140 2023-04-11 21:34:23.000000 bigraph-schema-0.0.4/bigraph_schema/parse.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    18090 2023-04-20 03:24:24.000000 bigraph-schema-0.0.4/bigraph_schema/registry.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    18411 2023-04-20 03:07:04.000000 bigraph-schema-0.0.4/bigraph_schema/schema.py
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-20 03:25:06.483024 bigraph-schema-0.0.4/bigraph_schema.egg-info/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1081 2023-04-20 03:25:06.000000 bigraph-schema-0.0.4/bigraph_schema.egg-info/PKG-INFO
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      310 2023-04-20 03:25:06.000000 bigraph-schema-0.0.4/bigraph_schema.egg-info/SOURCES.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)        1 2023-04-20 03:25:06.000000 bigraph-schema-0.0.4/bigraph_schema.egg-info/dependency_links.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       18 2023-04-20 03:25:06.000000 bigraph-schema-0.0.4/bigraph_schema.egg-info/requires.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       15 2023-04-20 03:25:06.000000 bigraph-schema-0.0.4/bigraph_schema.egg-info/top_level.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       38 2023-04-20 03:25:06.483024 bigraph-schema-0.0.4/setup.cfg
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-04-20 03:24:43.000000 bigraph-schema-0.0.4/setup.py
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-20 03:37:58.729590 bigraph-schema-0.0.5/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1081 2023-04-20 03:37:58.729590 bigraph-schema-0.0.5/PKG-INFO
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      151 2023-04-11 21:38:33.000000 bigraph-schema-0.0.5/README.md
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-20 03:37:58.729590 bigraph-schema-0.0.5/bigraph_schema/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      106 2023-04-19 21:19:48.000000 bigraph-schema-0.0.5/bigraph_schema/__init__.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2140 2023-04-11 21:34:23.000000 bigraph-schema-0.0.5/bigraph_schema/parse.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    18287 2023-04-20 03:36:19.000000 bigraph-schema-0.0.5/bigraph_schema/registry.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    18379 2023-04-20 03:37:11.000000 bigraph-schema-0.0.5/bigraph_schema/schema.py
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-20 03:37:58.729590 bigraph-schema-0.0.5/bigraph_schema.egg-info/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1081 2023-04-20 03:37:58.000000 bigraph-schema-0.0.5/bigraph_schema.egg-info/PKG-INFO
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      310 2023-04-20 03:37:58.000000 bigraph-schema-0.0.5/bigraph_schema.egg-info/SOURCES.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)        1 2023-04-20 03:37:58.000000 bigraph-schema-0.0.5/bigraph_schema.egg-info/dependency_links.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       18 2023-04-20 03:37:58.000000 bigraph-schema-0.0.5/bigraph_schema.egg-info/requires.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       15 2023-04-20 03:37:58.000000 bigraph-schema-0.0.5/bigraph_schema.egg-info/top_level.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       38 2023-04-20 03:37:58.729590 bigraph-schema-0.0.5/setup.cfg
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-04-20 03:37:27.000000 bigraph-schema-0.0.5/setup.py
```

### Comparing `bigraph-schema-0.0.4/PKG-INFO` & `bigraph-schema-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigraph-schema
-Version: 0.0.4
+Version: 0.0.5
 Summary: A serializable type schema for compositional systems biology
 Home-page: https://github.com/vivarium-collective/bigraph-schema
 Author: Eran Agmon, Ryan Spangler
 Author-email: agmon.eran@gmail.com, ryan.spangler@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigraph-schema-0.0.4/bigraph_schema/parse.py` & `bigraph-schema-0.0.5/bigraph_schema/parse.py`

 * *Files identical despite different names*

### Comparing `bigraph-schema-0.0.4/bigraph_schema/registry.py` & `bigraph-schema-0.0.5/bigraph_schema/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import random
+import pytest
 from typing import Any
 
 from bigraph_schema.parse import parse_type_parameters
 
 required_schema_keys = (
     '_default',
     '_apply',
@@ -614,18 +615,20 @@
 def test_expand_schema():
     schema = {'_type': 'cube'}
     expanded = type_registry.expand(schema)
 
     assert len(schema) == 1
     assert 'height' in expanded
 
-    import ipdb; ipdb.set_trace()
-
 
 def test_reregister_type():
-    try:
-        type_registry.register('int', )
+    with pytest.raises(Exception) as e:
+        type_registry.register('int', type_library['string'])
+
+    type_registry.register('int', type_library['string'], force=True)
+    type_registry.register('int', type_library['int'], force=True)
 
 
 if __name__ == '__main__':
     test_generate_default()
     test_expand_schema()
+    test_reregister_type()
```

### Comparing `bigraph-schema-0.0.4/bigraph_schema/schema.py` & `bigraph-schema-0.0.5/bigraph_schema/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,16 +404,14 @@
                 '1': {'_type': 'float'},
             },
         }
     }
 
     test_state = {}
 
-    import ipdb; ipdb.set_trace()
-
 
 def test_fill_type_mismatch():
     test_schema = {
         'a': {'_type': 'int', '_value': 2},
         'edge1': {
             '_type': 'edge',
             '_ports': {
@@ -707,16 +705,16 @@
                 'e0.1': ('v0', 'v1')}},
         'e2': {
             'wires': {
                 'e0.0': ('v0', 'v2', 'v3'),
                 'e0.1': 'v4',
                 'e0.2': ('v4', 'v5')}}}    
 
-    result = link_place(placegraph, linkgraph)
-    assert result == merged
+    result = link_place(placegraph, hypergraph)
+    # assert result == merged
 
 
 if __name__ == '__main__':
     test_validate_schema()
     test_fill_int()
     test_fill_cube()
     test_establish_path()
```

### Comparing `bigraph-schema-0.0.4/bigraph_schema.egg-info/PKG-INFO` & `bigraph-schema-0.0.5/bigraph_schema.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigraph-schema
-Version: 0.0.4
+Version: 0.0.5
 Summary: A serializable type schema for compositional systems biology
 Home-page: https://github.com/vivarium-collective/bigraph-schema
 Author: Eran Agmon, Ryan Spangler
 Author-email: agmon.eran@gmail.com, ryan.spangler@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigraph-schema-0.0.4/setup.py` & `bigraph-schema-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 
 
 with open("README.md", "r") as readme:
     description = readme.read()
 
 
 setup(
```

