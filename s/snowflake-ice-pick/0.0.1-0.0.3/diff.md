# Comparing `tmp/snowflake_ice_pick-0.0.1.tar.gz` & `tmp/snowflake_ice_pick-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake_ice_pick-0.0.1.tar", last modified: Mon Apr 10 02:21:08 2023, max compression
+gzip compressed data, was "snowflake_ice_pick-0.0.3.tar", last modified: Thu Apr 20 02:03:35 2023, max compression
```

## Comparing `snowflake_ice_pick-0.0.1.tar` & `snowflake_ice_pick-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 02:21:08.150486 snowflake_ice_pick-0.0.1/
--rw-rw-rw-   0        0        0     1110 2023-03-19 15:29:52.000000 snowflake_ice_pick-0.0.1/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-19 15:06:48.000000 snowflake_ice_pick-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5053 2023-04-10 02:21:08.150486 snowflake_ice_pick-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3097 2023-04-10 01:29:36.000000 snowflake_ice_pick-0.0.1/README.md
--rw-rw-rw-   0        0        0     1167 2023-04-05 02:51:30.000000 snowflake_ice_pick-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      842 2023-04-10 02:21:08.156485 snowflake_ice_pick-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-19 16:32:29.000000 snowflake_ice_pick-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 02:21:08.113486 snowflake_ice_pick-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 02:21:08.137485 snowflake_ice_pick-0.0.1/src/ice_pick/
--rw-rw-rw-   0        0        0      580 2023-04-09 20:58:35.000000 snowflake_ice_pick-0.0.1/src/ice_pick/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-07 03:34:14.000000 snowflake_ice_pick-0.0.1/src/ice_pick/account_object.py
--rw-rw-rw-   0        0        0     1855 2023-04-09 21:19:14.000000 snowflake_ice_pick-0.0.1/src/ice_pick/extension.py
--rw-rw-rw-   0        0        0    10148 2023-04-10 01:46:52.000000 snowflake_ice_pick-0.0.1/src/ice_pick/filter.py
--rw-rw-rw-   0        0        0     4958 2023-04-10 01:41:37.000000 snowflake_ice_pick-0.0.1/src/ice_pick/schema_object.py
--rw-rw-rw-   0        0        0     6499 2023-04-10 01:44:32.000000 snowflake_ice_pick-0.0.1/src/ice_pick/utils.py
--rw-rw-rw-   0        0        0      156 2023-04-05 02:27:12.000000 snowflake_ice_pick-0.0.1/src/ice_pick/version.py
-drwxrwxrwx   0        0        0        0 2023-04-10 02:21:08.148987 snowflake_ice_pick-0.0.1/src/snowflake_ice_pick.egg-info/
--rw-rw-rw-   0        0        0     5053 2023-04-10 02:21:08.000000 snowflake_ice_pick-0.0.1/src/snowflake_ice_pick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-04-10 02:21:08.000000 snowflake_ice_pick-0.0.1/src/snowflake_ice_pick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 02:21:08.000000 snowflake_ice_pick-0.0.1/src/snowflake_ice_pick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      143 2023-04-10 02:21:08.000000 snowflake_ice_pick-0.0.1/src/snowflake_ice_pick.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-10 02:21:08.000000 snowflake_ice_pick-0.0.1/src/snowflake_ice_pick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 02:03:35.982477 snowflake_ice_pick-0.0.3/
+-rw-rw-rw-   0        0        0     1103 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-19 15:06:48.000000 snowflake_ice_pick-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5550 2023-04-20 02:03:35.982977 snowflake_ice_pick-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3601 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.3/README.md
+-rw-rw-rw-   0        0        0     1167 2023-04-20 02:02:50.000000 snowflake_ice_pick-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      842 2023-04-20 02:03:35.984974 snowflake_ice_pick-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-19 16:32:29.000000 snowflake_ice_pick-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:03:35.944975 snowflake_ice_pick-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 02:03:35.963984 snowflake_ice_pick-0.0.3/src/ice_pick/
+-rw-rw-rw-   0        0        0      781 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.3/src/ice_pick/__init__.py
+-rw-rw-rw-   0        0        0    19806 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.3/src/ice_pick/account_object.py
+-rw-rw-rw-   0        0        0     2746 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.3/src/ice_pick/extension.py
+-rw-rw-rw-   0        0        0    10718 2023-04-20 02:00:08.000000 snowflake_ice_pick-0.0.3/src/ice_pick/filter.py
+-rw-rw-rw-   0        0        0     6473 2023-04-20 01:50:52.000000 snowflake_ice_pick-0.0.3/src/ice_pick/schema_object.py
+-rw-rw-rw-   0        0        0     8914 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.3/src/ice_pick/utils.py
+-rw-rw-rw-   0        0        0      158 2023-04-20 01:22:53.000000 snowflake_ice_pick-0.0.3/src/ice_pick/version.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:03:35.980976 snowflake_ice_pick-0.0.3/src/snowflake_ice_pick.egg-info/
+-rw-rw-rw-   0        0        0     5550 2023-04-20 02:03:35.000000 snowflake_ice_pick-0.0.3/src/snowflake_ice_pick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-04-20 02:03:35.000000 snowflake_ice_pick-0.0.3/src/snowflake_ice_pick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 02:03:35.000000 snowflake_ice_pick-0.0.3/src/snowflake_ice_pick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      143 2023-04-20 02:03:35.000000 snowflake_ice_pick-0.0.3/src/snowflake_ice_pick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 02:03:35.000000 snowflake_ice_pick-0.0.3/src/snowflake_ice_pick.egg-info/top_level.txt
```

### Comparing `snowflake_ice_pick-0.0.1/LICENSE` & `snowflake_ice_pick-0.0.3/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2004 Holger Krekel and others
+Copyright (c) 2023 Preston Blackburn
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `snowflake_ice_pick-0.0.1/PKG-INFO` & `snowflake_ice_pick-0.0.3/src/snowflake_ice_pick.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: snowflake_ice_pick
-Version: 0.0.1
+Name: snowflake-ice-pick
+Version: 0.0.3
 Summary: Snowpark extension to cover additional objects and higher level functions
 Author: Preston Blackburn
 License: The MIT License (MIT)
         
-        Copyright (c) 2004 Holger Krekel and others
+        Copyright (c) 2023 Preston Blackburn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
         of the Software, and to permit persons to whom the Software is furnished to do
         so, subject to the following conditions:
@@ -33,18 +33,20 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
-![ice pick logo](./docs/img/ice_pick_logo_mountain.png)
+![ice pick logo](https://github.com/PrestonBlackburn/ice_pick/blob/main/docs/img/ice_pick_logo_mountain.png?raw=true)
 
 # Ice Pick
-
+[![PyPI Latest Release](https://img.shields.io/pypi/v/snowflake-ice-pick.svg)](https://pypi.org/project/snowflake-ice-pick/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/PrestonBlackburn/ice_pick/blob/main/LICENSE)
+[![Codestyle Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 **Ice Pick** is a Python package that provides utilities for common operations done on a Snowflake warehouse. Operations range from getting Snowflake object ddl, getting table statistics, and returning account level information.
 
 Many utilities can be automatically packaged and deployed as stored procedures, so they can be executed natively in Snowflake.
 
 
 ## Main Features
@@ -53,19 +55,23 @@
 In this initial development two data classes are available: `SchemaObject` and `SchemaObjectFilter`. The `SchemaObject` allows you to interact and retrieve information on the schema object, such as ddl, description, and grants.  
 <br/>
 The `SchemaObjectFilter` allows you to quickly return and inspect many schema objects. With the `SchemaObjectFilter` you can filter on specific databases, schemas, objects or object types using regex. Alternatively you can specify ignore filters to return all objects not in the filter.  
 <br/>
 
 
 ## Getting Started
-(before pushed to pypi)
+
+### Read the docs: https://ice-pick.readthedocs.io/en/latest/
+
+<br/>
+<br/>
 
 ### install the library
 ```bash
-python -m pip install -e .
+python -m pip install snowflake-ice-pick
 ```
 
 ### create a snowpark session
 Ice pick extends the session to add the additional functionality
 ```python
 from snowflake.snowpark import Session
 from ice_pick import extend_session
```

### Comparing `snowflake_ice_pick-0.0.1/README.md` & `snowflake_ice_pick-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-![ice pick logo](./docs/img/ice_pick_logo_mountain.png)
+![ice pick logo](https://github.com/PrestonBlackburn/ice_pick/blob/main/docs/img/ice_pick_logo_mountain.png?raw=true)
 
 # Ice Pick
-
+[![PyPI Latest Release](https://img.shields.io/pypi/v/snowflake-ice-pick.svg)](https://pypi.org/project/snowflake-ice-pick/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/PrestonBlackburn/ice_pick/blob/main/LICENSE)
+[![Codestyle Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 **Ice Pick** is a Python package that provides utilities for common operations done on a Snowflake warehouse. Operations range from getting Snowflake object ddl, getting table statistics, and returning account level information.
 
 Many utilities can be automatically packaged and deployed as stored procedures, so they can be executed natively in Snowflake.
 
 
 ## Main Features
@@ -14,19 +16,23 @@
 In this initial development two data classes are available: `SchemaObject` and `SchemaObjectFilter`. The `SchemaObject` allows you to interact and retrieve information on the schema object, such as ddl, description, and grants.  
 <br/>
 The `SchemaObjectFilter` allows you to quickly return and inspect many schema objects. With the `SchemaObjectFilter` you can filter on specific databases, schemas, objects or object types using regex. Alternatively you can specify ignore filters to return all objects not in the filter.  
 <br/>
 
 
 ## Getting Started
-(before pushed to pypi)
+
+### Read the docs: https://ice-pick.readthedocs.io/en/latest/
+
+<br/>
+<br/>
 
 ### install the library
 ```bash
-python -m pip install -e .
+python -m pip install snowflake-ice-pick
 ```
 
 ### create a snowpark session
 Ice pick extends the session to add the additional functionality
 ```python
 from snowflake.snowpark import Session
 from ice_pick import extend_session
```

### Comparing `snowflake_ice_pick-0.0.1/pyproject.toml` & `snowflake_ice_pick-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools>=65.5.1", "wheel"]  # PEP 518 specifications.
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "snowflake_ice_pick"
 description = "Snowpark extension to cover additional objects and higher level functions"
-version = "0.0.1"
+version = "0.0.3"
 readme = "README.md"
 authors = [{name = "Preston Blackburn"}]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `snowflake_ice_pick-0.0.1/setup.cfg` & `snowflake_ice_pick-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `snowflake_ice_pick-0.0.1/src/ice_pick/filter.py` & `snowflake_ice_pick-0.0.3/src/ice_pick/filter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from dataclasses import dataclass, field
 from typing import List
 import copy
 import re
 import configparser
+import warnings
+import logging
 
 from snowflake.snowpark import Session
 import snowflake.snowpark as snowpark
 from snowflake.snowpark.row import Row
 
 import pandas as pd
 import numpy as np
@@ -20,19 +22,19 @@
 
 
 @dataclass
 class SchemaObjectFilter:
     """
     A filter that can be used to return multiple SchemaObjects
 
-    Apply selection first, then filter out ingore objects.  
-    
+    Apply selection first, then filter out ingore objects.
+
     Filters are applied by:
-        database -> ignore_dbs -> schema -> ignore_schemas -> object type -> object name    
-        
+        database -> ignore_dbs -> schema -> ignore_schemas -> object type -> object name
+
     ".*" can be used to return all (regex supported)
 
     Attributes
     ----------
     session: Session
         Snowpark Session
     databases: list
@@ -43,227 +45,271 @@
         the name of the objects to be searched for
     object_types: list
         the type of schema objects to be searched for
     ignore_dbs: list
         databases to be ignored in search
     ignore_schemas: list
         schemas to be ignored in search
-    
 
-    
+
+
     """
+
     session: Session
-    databases: list           # ex: [".*"]
-    schemas: list             # ex: ["schema_*"]
-    object_names: list       # ex: [".*"]
-    object_types: list       # ex: [".*"]
-    
-    ignore_dbs:list = _default_field(["SNOWFLAKE_SAMPLE_DATA", "SNOWFLAKE"])    # ex: ("SNOWFLAKE", "SNOWFLAKE_*")
-    ignore_schemas:list = _default_field(["INFORMATION_SCHEMA"]) # ex: ("SNOWFLAKE.*") # requires fully specified name
-            
-    
-    def _filter_schema_objects_helper(
-                                      self,
-                                      objects_df:pd.DataFrame,
-                                      filtered_dbs:str,
-                                      filtered_schemas:str,
-                                      obj_type:str
-                                      ) -> pd.DataFrame:
+    databases: list  # ex: [".*"]
+    schemas: list  # ex: ["schema_*"]
+    object_names: list  # ex: [".*"]
+    object_types: list  # ex: [".*"]
+
+    ignore_dbs: list = _default_field(
+        ["SNOWFLAKE_SAMPLE_DATA", "SNOWFLAKE"]
+    )  # ex: ("SNOWFLAKE", "SNOWFLAKE_*")
+    ignore_schemas: list = _default_field(
+        ["INFORMATION_SCHEMA"]
+    )  # ex: ("SNOWFLAKE.*") # requires fully specified name
 
-        """ 
+    def _filter_schema_objects_helper(
+        self,
+        objects_df: pd.DataFrame,
+        filtered_dbs: str,
+        filtered_schemas: str,
+        obj_type: str,
+    ) -> pd.DataFrame:
+        """
         a helper function for filtering dataframe for objects
         """
-        filtered_dbs_str = '|'.join(filtered_dbs)
-        obj_filtered_db_df = objects_df[objects_df['database_name'].str.contains(filtered_dbs_str)]
+        filtered_dbs_str = "|".join(filtered_dbs)
+        obj_filtered_db_df = objects_df[
+            objects_df["database_name"].str.contains(filtered_dbs_str)
+        ]
+
+        filtered_schemas_str = "|".join(filtered_schemas)
+        obj_filtered_schema_df = obj_filtered_db_df[
+            obj_filtered_db_df["schema_name"].str.contains(filtered_schemas_str)
+        ]
 
-        filtered_schemas_str = '|'.join(filtered_schemas)
-        obj_filtered_schema_df = obj_filtered_db_df[obj_filtered_db_df['schema_name'].str.contains(filtered_schemas_str)]
-        obj_filtered_schema_df["object_type"] = obj_type.split("S", -1)[0]
+        obj_filtered_schema_df["object_type"] = obj_type.rsplit("S", 1)[0]
 
         return obj_filtered_schema_df
 
-
-
-    def _filter_schema_objects(self,
-                               filtered_dbs:str,
-                               filtered_schemas:str) -> pd.DataFrame:
+    def _filter_schema_objects(
+        self, filtered_dbs: str, filtered_schemas: str
+    ) -> pd.DataFrame:
         """
         helper function to get all schema level object info
          - get the object types that are selected
          - get the object info (database, schema, object type, object name)
          - The object info returned depends on the selected object types (see schema_level_exceptions)
 
 
         """
 
-
         # (almost) all schema level objects:
-        schema_level_objects = ["ALERTS", 
-                                "EXTERNAL FUNCTIONS", 
-                                "EXTERNAL TABLES",
-                                "FILE FORMATS",
-                                "MATERIALIZED VIEWS",
-                                "MASKING POLICIES",
-                                "PASSWORD POLICIES",
-                                "PIPES",
-                                "PROCEDURES",
-                                "ROW ACCESS POLICIES",
-                                "SECRETS",
-                                "SESSION POLICIES",
-                                "SEQUENCES",
-                                "STAGES",
-                                "STREAMS",
-                                "TABLES",
-                                "TAGS", 
-                                "TASKS",
-                                "USER FUNCTIONS",
-                                "VIEWS"]
+        schema_level_objects = [
+            "ALERTS",
+            "EXTERNAL FUNCTIONS",
+            "EXTERNAL TABLES",
+            "FILE FORMATS",
+            "MATERIALIZED VIEWS",
+            "MASKING POLICIES",
+            "PASSWORD POLICIES",
+            "PIPES",
+            "PROCEDURES",
+            "ROW ACCESS POLICIES",
+            "SECRETS",
+            "SESSION POLICIES",
+            "SEQUENCES",
+            "STAGES",
+            "STREAMS",
+            "TABLES",
+            "TAGS",
+            "TASKS",
+            "USER FUNCTIONS",
+            "VIEWS",
+        ]
 
         # Schema level objects with some exceptions
-        schema_level_exceptions = ["EXTERNAL FUNCTIONS",
-                                   "PROCEDURES",
-                                   "USER FUNCTIONS"]
-
-
+        schema_level_exceptions = ["EXTERNAL FUNCTIONS", "PROCEDURES", "USER FUNCTIONS"]
 
         # get the objects to execute "show" on:
         obj_type_filter = []
         for type_obj in self.object_types:
-
             # to upper or not to upper..
             type_obj = type_obj.upper()
             r = re.compile(type_obj)
-            obj_list = list(filter(r.match, schema_level_objects)) 
+            obj_list = list(filter(r.match, schema_level_objects))
             obj_type_filter.extend(obj_list)
 
-
-        # loop through object types for show
+        # loop through object types for "show" query
         obj_df_list = []
         for obj_type in obj_type_filter:
-
-            objects_sql = f""" show {obj_type} in account; """
-            objects_df = snowpark_query(self.session, objects_sql, non_select=True)
-
+            try:
+                objects_sql = f""" show {obj_type} in account; """
+                objects_df = snowpark_query(self.session, objects_sql, non_select=True)
+            except Exception as e:
+                logging.warning("Some objects require a Enterprise or Buisness Critial account to access")
+                objects_df = pd.DataFrame()
             # g4t dfs to format: name, schema_name, database_name
             # need to filter based on name and type:
-            if obj_type not in schema_level_exceptions:
+            if objects_df.empty:
+                warnings.warn(f"No objects found for: {obj_type}", UserWarning)
+                continue
 
+            if obj_type not in schema_level_exceptions:
                 objects_df = objects_df[["database_name", "schema_name", "name"]]
 
-                obj_filtered_schema_df = self._filter_schema_objects_helper(objects_df,
-                                                                          filtered_dbs,
-                                                                          filtered_schemas,
-                                                                          obj_type)
+                obj_filtered_schema_df = self._filter_schema_objects_helper(
+                    objects_df, filtered_dbs, filtered_schemas, obj_type
+                )
 
                 obj_df_list.append(obj_filtered_schema_df)
 
-
-
             else:
                 # handle the exceptions
                 # In these cases database_name = catalog_name
                 # Also, we need the input arguments with the name, but not the output arguments
-                func_df = objects_df[['catalog_name', 'schema_name', 'arguments']]
-                func_df = func_df.rename({'catalog_name': 'database_name', 'arguments': 'name'}, axis=1)
+                func_df = objects_df[["catalog_name", "schema_name", "arguments"]]
+                func_df = func_df.rename(
+                    {"catalog_name": "database_name", "arguments": "name"}, axis=1
+                )
                 # Get just the function name + input arguments
-                func_df['name'] = func_df['name'].apply(lambda x: x.split(" RETURN ")[0])
+                func_df["name"] = func_df["name"].apply(
+                    lambda x: x.split(" RETURN ")[0]
+                )
 
                 # now we can filter down:
-                obj_filtered_schema_df = self._filter_schema_objects_helper(func_df,
-                                                                          filtered_dbs,
-                                                                          filtered_schemas,
-                                                                          obj_type)
+                obj_filtered_schema_df = self._filter_schema_objects_helper(
+                    func_df, filtered_dbs, filtered_schemas, obj_type
+                )
 
                 obj_df_list.append(obj_filtered_schema_df)
 
+        if obj_df_list == []:
+            warnings.warn(
+                f"""No objects found with filter:
+                            databases: {self.databases}
+                            schemas: {self.schemas}
+                            object_types: {self.object_types}
+                            object_names: {self.object_names}
+                            ingore_dbs: {self.ignore_dbs} 
+                            ignore_schemas: {self.ignore_schemas}""",
+                UserWarning,
+            )
+            return []
 
+        else:
+            all_objs_df = pd.concat(obj_df_list)
 
-        all_objs_df = pd.concat(obj_df_list)
-
-        return all_objs_df
-
-
+            return all_objs_df
 
     def return_schema_objects(self) -> List[SchemaObject]:
         """
         Filter objects based on input objects
         If the property is a wildcard ".*", then search all objects at that level
         (inputs are passed as regex)
 
         If exclude is set to true, everything matched will be ignored, and all non-matches are returned
 
         Parameters
         ----------
-        None : 
-             
+        None :
+
 
         Returns
         -------
         List[SchemaObjects]
             a list of schema objects that matched the filter cases
 
         Example
         -------
-        | Get all procedures in all databases:  
+        | Get all procedures in all databases:
         | >> SchemaObjectFilter([".*"], [".*"], [".*"], ["procedure"])
 
-        | Get all tables and vies in a single database:  
+        | Get all tables and vies in a single database:
         | >> SchemaObjectFilter(["TEST_DB"], [".*"], [".*"], ["table", "view"])
 
-        | Get all tables except for the sample tables:  
+        | Get all tables except for the sample tables:
         | >> SchemaObjectFilter([".*"], [".*"],[".*"], ["table"], ingore_dbs = ["SNOWFLAKE", "SNOWFLAKE_SAMPLE_DATA"]
 
-        | Get specific tables:  
+        | Get specific tables:
         | >> SchemaObjectFilter(["snowflake"], ["sample_data"], ["customer", "transactions"], ["table"])
 
         """
 
-
         # create select / ignore strings for filtering
-        db_select_str = '|'.join(self.databases)
-        db_ignore_str = '|'.join(self.ignore_dbs)
-
-        schema_select_str = '|'.join(self.schemas)
-        schema_ignore_str = '|'.join(self.ignore_schemas)
-
-        object_select_str = '|'.join(self.object_names)
-        type_select_str = '|'.join(self.object_types)
+        db_select_str = "|".join(self.databases)
+        db_ignore_str = "|".join(self.ignore_dbs)
 
+        schema_select_str = "|".join(self.schemas)
+        schema_ignore_str = "|".join(self.ignore_schemas)
 
+        object_select_str = "|".join(self.object_names)
+        type_select_str = "|".join(self.object_types)
 
         # Return Databases
         dbs_sql = f""" show databases in account; """
         dbs_df = snowpark_query(self.session, dbs_sql, non_select=True)
 
-        db_select_filter_df = dbs_df[dbs_df['name'].str.contains(db_select_str)]
-        db_ignore_filter_df = db_select_filter_df[~db_select_filter_df['name'].str.contains(db_ignore_str)]
-        filtered_dbs = db_ignore_filter_df['name'].tolist()
-
-
-
+        db_select_filter_df = dbs_df[dbs_df["name"].str.contains(db_select_str)]
+        db_ignore_filter_df = db_select_filter_df[
+            ~db_select_filter_df["name"].str.contains(db_ignore_str)
+        ]
+        filtered_dbs = db_ignore_filter_df["name"].tolist()
 
         # Return Schemas
         schemas_sql = f""" show schemas in account; """
         schemas_df = snowpark_query(self.session, schemas_sql, non_select=True)
 
-        filtered_dbs_str = '|'.join(filtered_dbs)
-        db_filtered_schemas_df = schemas_df[schemas_df['database_name'].str.contains(filtered_dbs_str)]
-
-        schema_select_filter_df = db_filtered_schemas_df[db_filtered_schemas_df['name'].str.contains(schema_select_str)]
-        schema_ignore_filter_df = schema_select_filter_df[~schema_select_filter_df['name'].str.contains(schema_ignore_str)]
-        filtered_schemas = schema_ignore_filter_df['name'].tolist()
-
+        filtered_dbs_str = "|".join(filtered_dbs)
+        db_filtered_schemas_df = schemas_df[
+            schemas_df["database_name"].str.contains(filtered_dbs_str)
+        ]
+
+        schema_select_filter_df = db_filtered_schemas_df[
+            db_filtered_schemas_df["name"].str.contains(schema_select_str)
+        ]
+        schema_ignore_filter_df = schema_select_filter_df[
+            ~schema_select_filter_df["name"].str.contains(schema_ignore_str)
+        ]
+        filtered_schemas = schema_ignore_filter_df["name"].tolist()
 
         # Return Objects
-        all_objs_df = self._filter_schema_objects(
-                                               filtered_dbs,
-                                               filtered_schemas
-                                               )
+        all_objs_df = self._filter_schema_objects(filtered_dbs, filtered_schemas)
 
         # Construct the SchemaObject:
         #    database, schema, object_name, object_type
+        # print(all_objs_df)
+
+        # return all_objs_df
 
-        schema_object_series = all_objs_df.apply(lambda x: SchemaObject(self.session, x["database_name"], x["schema_name"], x["name"], x["object_type"]), axis=1)
+        # handle the case when there are no objects:
+        if isinstance(all_objs_df, list):
+            return []
+
+        # otherwise create schema objects for the dataframe
+        schema_object_series = all_objs_df.apply(
+            lambda x: SchemaObject(
+                self.session,
+                x["database_name"],
+                x["schema_name"],
+                x["name"],
+                x["object_type"],
+            ),
+            axis=1,
+        )
 
         schema_object_list = schema_object_series.tolist()
 
         return schema_object_list
+
+
+@dataclass
+class AccountObjectFilter:
+    session: Session
+    object_names: list  # ex: [".*"]
+    object_types: list  # ex: [".*"]
+
+    def return_account_objects():
+        """
+        Return all account objects matching the filter
+        """
+        return
```

### Comparing `snowflake_ice_pick-0.0.1/src/ice_pick/schema_object.py` & `snowflake_ice_pick-0.0.3/src/ice_pick/schema_object.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from dataclasses import dataclass, field
 from typing import List
 import copy
 import re
-import configparser
+from pathlib import Path
+
 
 from snowflake.snowpark import Session
 import snowflake.snowpark as snowpark
 from snowflake.snowpark.row import Row
 
 import pandas as pd
 import numpy as np
 
 from ice_pick.utils import snowpark_query
 
 
-
-
 @dataclass
 class SchemaObject:
     """Represents a Snowflake Schema object.
 
     Schema Objects Include: ALERTS, EXTERNAL FUNCTIONS, EXTERNAL TABLES, FILE FORMATS,
     MATERIALIZED VIEWS, MASKING POLICIES, PASSWORD POLICIES, PIPES, PROCEDURES,
     ROW ACCESS POLICIES, SECRETS, SESSION POLICIES, SEQUENCES, STAGES, STREAMS,
     TABLES, TAGS, TASKS, USER FUNCTIONS,  VIEWS, *EXTERNAL FUNCTIONS,
      *PROCEDURES, *USER FUNCTIONS
+     ** Also note some of these objects require the enterprise account
 
     Attributes
     ----------
     session: Session
         Snowpark Session
     database: str
         database that the object is in
@@ -37,122 +37,161 @@
     object_name: str
         the name of the object
     object_type: str
         the type of schema object
 
 
     """
+
     # Schema Objects: Table, View, Stream, Stored Proc, File Format, UDF, etc..
     session: Session
     database: str = "SNOWFLAKE"
     schema: str = ""
     object_name: str = ""
     object_type: str = ""
-    
 
-    
-    # Which functions should be a part of the class, and 
+    # Which functions should be a part of the class, and
     # which should be outside teh class?
-    def get_ddl(self) -> str:
+    def get_ddl(self, save: bool = False) -> str:
         """
         Return the ddl of the schema object as a string
-        """
-        ddl_sql = f"""select get_ddl('{self.object_type}',
+        if save = True: save the ddl locally
+        The default save path is:
+        DDL/database/schema/object_type/database.schema.object_name.sql
+
+        Parameters
+        ----------
+        save : bool = False
+            save the ddl as a file locally
+
+        Returns
+        -------
+        str
+            A string with the ddl
+
+        """
+        ddl_exception_list = ["USER FUNCTION", "USER POLICY"]
+        ddl_exception_map = {"USER FUNCTION": "FUNCTION", "USER POLICY": "POLICY"}
+
+        if self.object_type in ddl_exception_list:
+            self.ddl_object_type = ddl_exception_map[self.object_type]
+        else:
+            self.ddl_object_type = self.object_type
+
+        ddl_sql = f"""select get_ddl('{self.ddl_object_type}',
                 '{self.database}.{self.schema}.{self.object_name}' );"""
         ddl_df = snowpark_query(self.session, ddl_sql)
-        
+
         ddl_str = ddl_df.iloc[0][0]
-        
-        return ddl_str
 
+        # load to state to help create object
+        self.ddl_str = ddl_str
+
+        if save:
+            path = f"DDL/{self.database}/{self.schema}/{self.object_type}"
+            filename = f"{self.database}.{self.schema}.{self.object_name}.sql"
+            output_file = Path(f"{path}/{filename}")
+            output_file.parent.mkdir(exist_ok=True, parents=True)
+            output_file.write_text(ddl_str)
+
+        return ddl_str
 
     def get_description(self) -> str:
         """
         Return the description of the schema object as a string
         """
         desc_sql = f"""describe {self.object_type} 
                     "{self.database}"."{self.schema}"."{self.object_name}";"""
         desc_df = snowpark_query(self.session, desc_sql, non_select=True)
-        
+
         return desc_df
 
-    
     def get_grants_on(self) -> list:
         """
         Return a list of grants on the schema object as a list
         """
         grants_sql = f"""show grants on {self.object_type} 
                     "{self.database}"."{self.schema}"."{self.object_name}";"""
         grants_df = snowpark_query(self.session, grants_sql, non_select=True)
-        
+
         return grants_df
-    
-    
-    def grant(self, privilege:list, grantee:str) -> str:
-        """ grant access on object, return status
-
-        | -- For TABLE  
-        |   { SELECT | INSERT | UPDATE | DELETE | TRUNCATE | REFERENCES } [ , ... ]  
-        | -- For VIEW  
-        |   { SELECT | REFERENCES } [ , ... ]  
-        | -- For MATERIALIZED VIEW  
-        |   { SELECT | REFERENCES } [ , ... ]  
-        | -- For SEQUENCE, FUNCTION (UDF or external function), PROCEDURE, or FILE FORMAT  
-        |     USAGE  
-        | -- For internal STAGE  
-        |     READ [ , WRITE ]  
-        | -- For external STAGE  
-        |     USAGE  
-        | -- For PIPE  
-        |    { MONITOR | OPERATE } [ , ... ]  
-        | -- For STREAM  
-        |     SELECT  
-        | -- For TASK  
-        |    { MONITOR | OPERATE } [ , ... ]  
-        | -- For MASKING POLICY  
-        |     APPLY  
-        | -- For PASSWORD POLICY  
-        |      APPLY  
-        | -- For ROW ACCESS POLICY  
-        |     APPLY  
-        | -- For SESSION POLICY  
-        |     APPLY  
-        | -- For TAG  
-        |     APPLY  
-        | -- For ALERT  
-        |     OPERATE  
-        | -- For SECRET  
-        |     USAGE  
+
+    def grant(self, privilege: list, grantee: str) -> str:
+        """grant access on object, return status
+
+        | -- For TABLE
+        |   { SELECT | INSERT | UPDATE | DELETE | TRUNCATE | REFERENCES } [ , ... ]
+        | -- For VIEW
+        |   { SELECT | REFERENCES } [ , ... ]
+        | -- For MATERIALIZED VIEW
+        |   { SELECT | REFERENCES } [ , ... ]
+        | -- For SEQUENCE, FUNCTION (UDF or external function), PROCEDURE, or FILE FORMAT
+        |     USAGE
+        | -- For internal STAGE
+        |     READ [ , WRITE ]
+        | -- For external STAGE
+        |     USAGE
+        | -- For PIPE
+        |    { MONITOR | OPERATE } [ , ... ]
+        | -- For STREAM
+        |     SELECT
+        | -- For TASK
+        |    { MONITOR | OPERATE } [ , ... ]
+        | -- For MASKING POLICY
+        |     APPLY
+        | -- For PASSWORD POLICY
+        |      APPLY
+        | -- For ROW ACCESS POLICY
+        |     APPLY
+        | -- For SESSION POLICY
+        |     APPLY
+        | -- For TAG
+        |     APPLY
+        | -- For ALERT
+        |     OPERATE
+        | -- For SECRET
+        |     USAGE
 
         """
 
         grant_sql = f"""grant {", ".join(privilege)} on {self.object_type} 
                     "{self.database}"."{self.schema}"."{self.object_name}"
                     to ROLE {grantee};"""
         grant_df = snowpark_query(self.session, grant_sql, non_select=True)
-        
+
         grant_status_str = grant_df.iloc[0][0]
-        
+
         return grant_status_str
-    
-    def create(self, sql_ext:str = ""):
-        """ create in snowflake if not exists. For now this is very dependant on object type. 
-        Usualy the additional stuff comes after the object name, which can be provided by the sql_ext param. 
+
+    def create(
+        self,
+        create_method: str = "default",
+        ddl: str = "",
+        sql_ext: str = "",
+        create_if_exists: bool = False,
+    ):
+        """create in snowflake if not exists. For now this is very dependant on object type.
+        Usualy the additional stuff comes after the object name, which can be provided by the sql_ext param.
         (todo: sql ext could just make more confusing - maybe need to create specific extension objects)
-        """
-        
-        create_sql = f""" create {self.object_type} if not exists
-                       "{self.database}"."{self.schema}"."{self.object_name}"
-                       {sql_ext}; """
-        
-        create_df = snowpark_query(self.session, create_sql, non_select=True)
-        
-        create_status_str = create_df.iloc[0][0]
-        
-        return create_status_str
-    
 
+        create_methods:
+            - default:
+            - ddl:        user provided ddl string
+            - ddl_state:  use ddl from get_ddl() function
+        """
+
+        if create_method == "default":
+            create_sql = f""" create {self.object_type} if not exists
+                        "{self.database}"."{self.schema}"."{self.object_name}"
+                        {sql_ext}; """
 
+        if create_method == "ddl_state":
+            create_sql = self.ddl_str
 
+        if create_method == "ddl":
+            create_sql = ddl
 
+        create_df = snowpark_query(self.session, create_sql, non_select=True)
 
+        create_status_str = create_df.iloc[0][0]
 
+        return create_status_str
```

### Comparing `snowflake_ice_pick-0.0.1/src/ice_pick/utils.py` & `snowflake_ice_pick-0.0.3/src/ice_pick/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,185 +3,282 @@
 import copy
 import re
 import configparser
 
 from snowflake.snowpark import Session
 import snowflake.snowpark as snowpark
 from snowflake.snowpark.row import Row
-from snowflake.snowpark.types import IntegerType, StringType, StructField, StructType, FloatType, NullType
+from snowflake.snowpark.types import (
+    IntegerType,
+    StringType,
+    StructField,
+    StructType,
+    FloatType,
+    NullType,
+)
 from snowflake.snowpark.functions import lit
 
 import pandas as pd
 import numpy as np
 
 
+# maybe add an option to log all sql executions
+# could be nice to have more transparency
+# (at least add logging for debugging)
 def snowpark_query(session, sql, non_select=False):
-    """ 
-    non-select queries include things like: 
+    """
+    non-select queries include things like:
      "show databases;"
-    
-    
+
+
     """
-    
+
     if non_select:
         # apply the Row function "as_dict" to all rows then conver to pandas
         row_objs = session.sql(sql).collect()
 
         dict_array = np.array(list(map(Row.as_dict, row_objs)))
 
         df = pd.DataFrame.from_records(dict_array)
 
         return df
-    
+
     else:
-        
         df = session.sql(sql).to_pandas()
-        
+
         return df
-        
+
 
 ### Auto union
-def _get_schemas(union_dfs:list) -> list:
+def _get_schemas(union_dfs: list) -> list:
     # get a flat list of all structs in all dataframes
     struct_field_list = []
-    for df in  union_dfs:
+    for df in union_dfs:
         structs = df.schema.fields
         for struct in structs:
             struct_field_list.append(struct)
-            
+
     return struct_field_list
 
-def _get_unique_struct_fields(struct_field_list:list) -> list:
+
+def _get_unique_struct_fields(struct_field_list: list) -> list:
     # only get ge the unique structs
     unique_structs_list = []
     for struct in struct_field_list:
         if struct not in unique_structs_list:
             unique_structs_list.append(struct)
-            
+
     return unique_structs_list
 
-def _handle_struct_name_type_mismatch(unique_structs_list:list) -> list:
+
+def _handle_struct_name_type_mismatch(unique_structs_list: list) -> list:
     # handle when columns with the same name have different data types
     # for now just pick the first data type, and discard the others
     unique_structs_type_list = []
     struct_name_list = []
     for struct in unique_structs_list:
         if struct.name not in struct_name_list:
             struct_name_list.append(struct.name)
             unique_structs_type_list.append(struct)
-            
+
     return unique_structs_type_list
 
 
-def _create_union_dataframe(session:Session, unique_structs_type_list:list) -> snowpark.DataFrame:
+def _create_union_dataframe(
+    session: Session, unique_structs_type_list: list
+) -> snowpark.DataFrame:
     # create the union dataframe from the unique schema structs
     union_schema = StructType(unique_structs_type_list)
-    
+
     union_df = session.create_dataframe([], union_schema)
-    
+
     return union_df
 
 
-def _extend_schema(df: snowpark.DataFrame, union_df:snowpark.DataFrame) -> snowpark.DataFrame:
-    
-    col_names =  {struct.name: struct for struct in df.schema.fields}
+def _extend_schema(
+    df: snowpark.DataFrame, union_df: snowpark.DataFrame
+) -> snowpark.DataFrame:
+    col_names = {struct.name: struct for struct in df.schema.fields}
     union_col_names = {struct.name: struct for struct in union_df.schema.fields}
-    
+
     # get struct for col not in the dataframe
     structs_to_null = []
     for key in union_col_names:
         if key not in col_names:
             structs_to_null.append(union_col_names[key])
-    
+
     # add struct as null col
     for struct in structs_to_null:
-        
         df = df.with_column(struct.name, lit(None))
-        
+
         # cast to the correct data type
-        
-    
+
     return df
-    
 
-def _add_null_cols(union_dfs:list, union_df: snowpark.DataFrame) -> list:
+
+def _add_null_cols(union_dfs: list, union_df: snowpark.DataFrame) -> list:
     # add null columns for the inclusive case
     # (the number of columns must match between tables, so null cols need to be added)
     ext_dfs = []
     for df in union_dfs:
         df = _extend_schema(df, union_df)
         ext_dfs.append(df)
-    
-    return ext_dfs
 
+    return ext_dfs
 
 
-def _populate_union_df(ext_dfs:list, union_df: snowpark.DataFrame) -> snowpark.DataFrame:
-    
+def _populate_union_df(
+    ext_dfs: list, union_df: snowpark.DataFrame
+) -> snowpark.DataFrame:
     for df in ext_dfs:
         union_df = union_df.union_all_by_name(df)
-  
+
     return union_df
 
 
-def auto_union_standalone(session:Session, union_dfs:list) -> snowpark.DataFrame:
+# Might move these to a "pandas_func" module
+def concat_standalone(session: Session, union_dfs: list) -> snowpark.DataFrame:
     """
-    Returns a unioned dataframe from the input list of dataframes based on column names. 
-    Primarly to handle cases where the number of columns do not match, 
+    Returns a unioned dataframe from the input list of dataframes based on column names.
+    Primarly to handle cases where the number of columns do not match,
     which is not suppored by the base union function.
     If columns do not match, non-matching columns are added with null values to the base dataframes.
 
     Parameters
     ----------
     session : Session
         session object
     union_dfs : list
         A list of the input snowpark dataframes to union
 
     Returns
     -------
     snowpark.DataFrame
         A snowpark dataframe with the unioned input dataframes
-    
+
     Example
     -------
-        | >> schema_1 = StructType([StructField("a", IntegerType()), StructField("b", StringType())])  
-        | >> schema_2 = StructType([StructField("a", FloatType()), StructField("c", StringType())])  
-        | >> schema_3 = StructType([StructField("a", IntegerType()), StructField("c", StringType())])  
-        | >> schema_4 = StructType([StructField("c", StringType()), StructField("d", StringType())])  
-
-        | >> df_1 = session.create_dataframe([[1, "snow"], [3, "flake"]], schema_1)  
-        | >> df_2 = session.create_dataframe([[2.0, "ice"], [4.0, "pick"]], schema_2)  
-        | >> df_3 = session.create_dataframe([[6, "test_1"], [7, "test_2"]], schema_3)  
-        | >> df_4 = session.create_dataframe([["testing_d", "testing_f"], ["testing_g", "testing_h"]], schema_4)  
-
-        | >> union_dfs = [df_1, df_2, df_3, df_4]  
-        | >> unioned_df = auto_union(session, union_dfs)  
-        | >> unioned_df.show()  
-        | ----------------------------------------  
-        | |"A"   |"B"    |"C"        |"D"        |  
-        | ----------------------------------------  
-        | |1.0   |snow   |NULL       |NULL       |  
-        | |3.0   |flake  |NULL       |NULL       |  
-        | |2.0   |NULL   |ice        |NULL       |  
-        | |4.0   |NULL   |pick       |NULL       |  
-        | |6.0   |NULL   |test_1     |NULL       |  
-        | |7.0   |NULL   |test_2     |NULL       |  
-        | |NULL  |NULL   |testing_d  |testing_f  |  
-        | |NULL  |NULL   |testing_g  |testing_h  |  
-        | ----------------------------------------  
-    
+        | >> schema_1 = StructType([StructField("a", IntegerType()), StructField("b", StringType())])
+        | >> schema_2 = StructType([StructField("a", FloatType()), StructField("c", StringType())])
+        | >> schema_3 = StructType([StructField("a", IntegerType()), StructField("c", StringType())])
+        | >> schema_4 = StructType([StructField("c", StringType()), StructField("d", StringType())])
+
+        | >> df_1 = session.create_dataframe([[1, "snow"], [3, "flake"]], schema_1)
+        | >> df_2 = session.create_dataframe([[2.0, "ice"], [4.0, "pick"]], schema_2)
+        | >> df_3 = session.create_dataframe([[6, "test_1"], [7, "test_2"]], schema_3)
+        | >> df_4 = session.create_dataframe([["testing_d", "testing_f"], ["testing_g", "testing_h"]], schema_4)
+
+        | >> union_dfs = [df_1, df_2, df_3, df_4]
+        | >> unioned_df = auto_union(session, union_dfs)
+        | >> unioned_df.show()
+        | ----------------------------------------
+        | |"A"   |"B"    |"C"        |"D"        |
+        | ----------------------------------------
+        | |1.0   |snow   |NULL       |NULL       |
+        | |3.0   |flake  |NULL       |NULL       |
+        | |2.0   |NULL   |ice        |NULL       |
+        | |4.0   |NULL   |pick       |NULL       |
+        | |6.0   |NULL   |test_1     |NULL       |
+        | |7.0   |NULL   |test_2     |NULL       |
+        | |NULL  |NULL   |testing_d  |testing_f  |
+        | |NULL  |NULL   |testing_g  |testing_h  |
+        | ----------------------------------------
+
     """
-    
+
     struct_field_list = _get_schemas(union_dfs)
-    
+
     unique_structs_list = _get_unique_struct_fields(struct_field_list)
-    
+
     unique_structs_type_list = _handle_struct_name_type_mismatch(unique_structs_list)
-    
+
     union_df = _create_union_dataframe(session, unique_structs_type_list)
-    
+
     ext_dfs = _add_null_cols(union_dfs, union_df)
 
     union_df = _populate_union_df(ext_dfs, union_df)
-    
-    return union_df
+
+    return union_df
+
+
+def melt_standalone(
+    session: Session,
+    df: snowpark.DataFrame,
+    id_vars: list,
+    value_vars: list,
+    var_name: str = "variable",
+    value_name: str = "value",
+) -> snowpark.DataFrame:
+    """
+    Returns a unioned dataframe from the input list of dataframes based on column names.
+    Primarly to handle cases where the number of columns do not match,
+    which is not suppored by the base union function.
+    If columns do not match, non-matching columns are added with null values to the base dataframes.
+
+    Parameters
+    ----------
+    session : Session
+        session object
+    df : snowpark.DataFrame
+        A snowpark dataframe to melt
+    id_vars: list
+        Column names to use as identifiers
+    value_vars: list
+        Column names to unpivot
+    var_name: str, default 'variable'
+        Name of the variable column
+    value_name: str, default 'value'
+        Name of the value column
+
+
+    Returns
+    -------
+    snowpark.DataFrame
+        A snowpark dataframe with the unpivoted dataframes
+
+    Example
+    -------
+        | >> schema = StructType([StructField("A", StringType()), StructField("B", IntegerType()), StructField("C", IntegerType())])
+        | >> df = session.create_dataframe([['a', 1, 2], ['b', 3, 4], ['c', 5, 6]], schema)
+        | >> melt_df = session.melt(df, ['A'], ['B', 'C'])
+        | >> melt_df.show()
+
+        | ------------------------------
+        | |"A"  |"VALUE"  |"VARIABLE"  |
+        | ------------------------------
+        | |a    |1        |B           |
+        | |b    |3        |B           |
+        | |c    |5        |B           |
+        | |a    |2        |C           |
+        | |b    |4        |C           |
+        | |c    |6        |C           |
+        | ------------------------------
+
+    """
+
+    melt_dfs_list = []
+    for value_var in value_vars:
+        filtered_cols = id_vars + [value_var]
+        melt_subset_df = df[filtered_cols]
+        melt_subset_df = melt_subset_df.rename(value_var, value_name)
+        melt_subset_df = melt_subset_df.with_column(var_name, lit(value_var))
+        melt_dfs_list.append(melt_subset_df)
+
+    melt_df = concat_standalone(session, melt_dfs_list)
+
+    return melt_df
+
+
+def isna():
+    return
+
+
+def isnull():
+    return
+
+
+def pivot():
+    return
+
+
+def get_dummies():
+    return
```

### Comparing `snowflake_ice_pick-0.0.1/src/snowflake_ice_pick.egg-info/PKG-INFO` & `snowflake_ice_pick-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: snowflake-ice-pick
-Version: 0.0.1
+Name: snowflake_ice_pick
+Version: 0.0.3
 Summary: Snowpark extension to cover additional objects and higher level functions
 Author: Preston Blackburn
 License: The MIT License (MIT)
         
-        Copyright (c) 2004 Holger Krekel and others
+        Copyright (c) 2023 Preston Blackburn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
         of the Software, and to permit persons to whom the Software is furnished to do
         so, subject to the following conditions:
@@ -33,18 +33,20 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
-![ice pick logo](./docs/img/ice_pick_logo_mountain.png)
+![ice pick logo](https://github.com/PrestonBlackburn/ice_pick/blob/main/docs/img/ice_pick_logo_mountain.png?raw=true)
 
 # Ice Pick
-
+[![PyPI Latest Release](https://img.shields.io/pypi/v/snowflake-ice-pick.svg)](https://pypi.org/project/snowflake-ice-pick/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/PrestonBlackburn/ice_pick/blob/main/LICENSE)
+[![Codestyle Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 **Ice Pick** is a Python package that provides utilities for common operations done on a Snowflake warehouse. Operations range from getting Snowflake object ddl, getting table statistics, and returning account level information.
 
 Many utilities can be automatically packaged and deployed as stored procedures, so they can be executed natively in Snowflake.
 
 
 ## Main Features
@@ -53,19 +55,23 @@
 In this initial development two data classes are available: `SchemaObject` and `SchemaObjectFilter`. The `SchemaObject` allows you to interact and retrieve information on the schema object, such as ddl, description, and grants.  
 <br/>
 The `SchemaObjectFilter` allows you to quickly return and inspect many schema objects. With the `SchemaObjectFilter` you can filter on specific databases, schemas, objects or object types using regex. Alternatively you can specify ignore filters to return all objects not in the filter.  
 <br/>
 
 
 ## Getting Started
-(before pushed to pypi)
+
+### Read the docs: https://ice-pick.readthedocs.io/en/latest/
+
+<br/>
+<br/>
 
 ### install the library
 ```bash
-python -m pip install -e .
+python -m pip install snowflake-ice-pick
 ```
 
 ### create a snowpark session
 Ice pick extends the session to add the additional functionality
 ```python
 from snowflake.snowpark import Session
 from ice_pick import extend_session
```

