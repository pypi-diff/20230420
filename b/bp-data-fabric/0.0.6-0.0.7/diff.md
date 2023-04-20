# Comparing `tmp/bp_data_fabric-0.0.6.tar.gz` & `tmp/bp_data_fabric-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_fabric-0.0.6.tar", last modified: Wed Apr 19 07:23:18 2023, max compression
+gzip compressed data, was "bp_data_fabric-0.0.7.tar", last modified: Thu Apr 20 09:47:40 2023, max compression
```

## Comparing `bp_data_fabric-0.0.6.tar` & `bp_data_fabric-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:23:18.926349 bp_data_fabric-0.0.6/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-0.0.6/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      286 2023-04-19 07:23:18.926037 bp_data_fabric-0.0.6/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-0.0.6/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:23:18.924640 bp_data_fabric-0.0.6/bp_data_fabric.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      286 2023-04-19 07:23:18.000000 bp_data_fabric-0.0.6/bp_data_fabric.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      239 2023-04-19 07:23:18.000000 bp_data_fabric-0.0.6/bp_data_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-19 07:23:18.000000 bp_data_fabric-0.0.6/bp_data_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-19 07:23:18.000000 bp_data_fabric-0.0.6/bp_data_fabric.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-04-19 07:23:18.000000 bp_data_fabric-0.0.6/bp_data_fabric.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:23:18.925130 bp_data_fabric-0.0.6/data_fabric/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1071 2023-04-18 05:57:17.000000 bp_data_fabric-0.0.6/data_fabric/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-19 07:23:18.926452 bp_data_fabric-0.0.6/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      602 2023-04-19 07:22:15.000000 bp_data_fabric-0.0.6/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 09:47:40.726180 bp_data_fabric-0.0.7/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-0.0.7/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      286 2023-04-20 09:47:40.725901 bp_data_fabric-0.0.7/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-0.0.7/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 09:47:40.724706 bp_data_fabric-0.0.7/bp_data_fabric.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      286 2023-04-20 09:47:40.000000 bp_data_fabric-0.0.7/bp_data_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-04-20 09:47:40.000000 bp_data_fabric-0.0.7/bp_data_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-20 09:47:40.000000 bp_data_fabric-0.0.7/bp_data_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-20 09:47:40.000000 bp_data_fabric-0.0.7/bp_data_fabric.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-04-20 09:47:40.000000 bp_data_fabric-0.0.7/bp_data_fabric.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 09:47:40.725445 bp_data_fabric-0.0.7/data_fabric/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      920 2023-04-20 07:20:57.000000 bp_data_fabric-0.0.7/data_fabric/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2184 2023-04-20 07:22:51.000000 bp_data_fabric-0.0.7/data_fabric/components.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-20 09:47:40.726269 bp_data_fabric-0.0.7/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      602 2023-04-20 09:47:33.000000 bp_data_fabric-0.0.7/setup.py
```

### Comparing `bp_data_fabric-0.0.6/LICENSE` & `bp_data_fabric-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-0.0.6/data_fabric/__init__.py` & `bp_data_fabric-0.0.7/data_fabric/components.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,87 @@
 from typing import List
 import query_tool as qt
 import data_grid as dg
 import data_visualization as dv
+import streamlit as st
 
-def data_fabric(
-    query: str = "",
-    query_tool_title: str = "",
-    data_grid_title: str = "",
-    data_visualization_title: str = "",
-    databases: List[str] = [],
-    tables: List[dict] = [],
-    columns: List[dict] = [],
-    on_database_change=None,
-    on_table_change=None,
-    on_generate_query=None,
-    on_copy_query=None,
-    data={},
-):
+def main(
+        query: str = "",
+        query_tool_title: str = "",
+        data_grid_title: str = "",
+        data_visualization_title: str = "",
+        databases: List[str] = [],
+        tables: List[dict] = [],
+        columns: List[dict] = [],
+        data={},
+        on_database_change=None,
+        on_table_change=None,
+        on_generate_query=None,
+        on_copy_query=None,
+        on_execute=None
+    ):
     
-    qt.query_tool(
+
+    render_query_tool(
         query=query,
         title=query_tool_title,
         databases=databases,
         tables=tables,
         columns=columns,
         on_database_change=on_database_change,
         on_table_change=on_table_change,
         on_generate_query=on_generate_query,
         on_copy_query=on_copy_query,
-        key="query_builder",
     )
 
-    dg.data_grid(
+    if query != "":
+      st.button("Execute", on_click=on_execute)
+
+    render_data_grid(
         title=data_grid_title,
         rows=data.get("rows", []),
         columns=data.get("columns", []),
+    )
+
+    render_data_visualizer(
+        title=data_visualization_title,
+        rows=data.get("rows", []),
+    )
+
+def render_query_tool(
+        query: str = "",
+        title: str = "",
+        databases: List[str] = [],
+        tables: List[dict] = [],
+        columns: List[dict] = [],
+        on_database_change=None,
+        on_table_change=None,
+        on_generate_query=None,
+        on_copy_query=None,
+):
+    qt.query_tool(
+        query=query,
+        title=title,
+        databases=databases,
+        tables=tables,
+        columns=columns,
+        on_database_change=on_database_change,
+        on_table_change=on_table_change,
+        on_generate_query=on_generate_query,
+        on_copy_query=on_copy_query,
+        key="query_builder",
+    )  
+
+def render_data_grid(title: str="", rows: List = [], columns: List = []):
+    dg.data_grid(
+        title=title,
+        rows=rows,
+        columns=columns,
         key="data_grid",
     )
 
+def render_data_visualizer(title="", rows=[]):
     dv.data_visualizer(
-        data=data.get("rows", []),
+        title=title,
+        data=rows,
         key="data_visualizer",
-    )
+    )
```

### Comparing `bp_data_fabric-0.0.6/setup.py` & `bp_data_fabric-0.0.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="bp_data_fabric",
-    version="0.0.6",
+    version="0.0.7",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

