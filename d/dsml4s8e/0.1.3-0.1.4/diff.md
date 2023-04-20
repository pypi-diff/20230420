# Comparing `tmp/dsml4s8e-0.1.3.tar.gz` & `tmp/dsml4s8e-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsml4s8e-0.1.3.tar", last modified: Thu Mar 30 20:01:38 2023, max compression
+gzip compressed data, was "dsml4s8e-0.1.4.tar", last modified: Thu Apr 20 11:38:44 2023, max compression
```

## Comparing `dsml4s8e-0.1.3.tar` & `dsml4s8e-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-03-30 20:01:38.161506 dsml4s8e-0.1.3/
--rw-r--r--   0 jovyan    (1000) users      (100)      494 2023-03-30 20:01:38.159048 dsml4s8e-0.1.3/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     5878 2023-03-30 20:00:41.000000 dsml4s8e-0.1.3/README.md
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-03-30 20:01:37.986068 dsml4s8e-0.1.3/dsml4s8e/
--rw-r--r--   0 jovyan    (1000) users      (100)       22 2023-03-30 20:00:48.000000 dsml4s8e-0.1.3/dsml4s8e/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)     2344 2023-03-29 11:41:21.000000 dsml4s8e-0.1.3/dsml4s8e/dotted_urls_names.py
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-03-30 20:01:38.102730 dsml4s8e-0.1.3/dsml4s8e/dsmlcatalog/
--rw-r--r--   0 jovyan    (1000) users      (100)        0 2023-03-13 20:41:59.000000 dsml4s8e-0.1.3/dsml4s8e/dsmlcatalog/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1192 2023-03-28 16:37:07.000000 dsml4s8e-0.1.3/dsml4s8e/dsmlcatalog/dagster_home.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1379 2023-03-28 22:26:16.000000 dsml4s8e-0.1.3/dsml4s8e/dsmlcatalog/local_storage.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1029 2023-03-30 11:47:09.000000 dsml4s8e-0.1.3/dsml4s8e/nb_data_keys.py
--rw-r--r--   0 jovyan    (1000) users      (100)     4967 2023-03-30 12:03:55.000000 dsml4s8e-0.1.3/dsml4s8e/nb_op.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1608 2023-03-30 12:04:36.000000 dsml4s8e-0.1.3/dsml4s8e/op_params_from_nb.py
--rw-r--r--   0 jovyan    (1000) users      (100)      598 2023-03-29 09:55:19.000000 dsml4s8e-0.1.3/dsml4s8e/storage_catalog.py
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-03-30 20:01:38.141713 dsml4s8e-0.1.3/dsml4s8e/storage_rw/
--rw-r--r--   0 jovyan    (1000) users      (100)        0 2023-03-13 20:42:01.000000 dsml4s8e-0.1.3/dsml4s8e/storage_rw/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)      603 2023-03-13 20:41:59.000000 dsml4s8e-0.1.3/dsml4s8e/storage_rw/pandas_loacl.py
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-03-30 20:01:38.051603 dsml4s8e-0.1.3/dsml4s8e.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)      494 2023-03-30 20:01:37.000000 dsml4s8e-0.1.3/dsml4s8e.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)      505 2023-03-30 20:01:37.000000 dsml4s8e-0.1.3/dsml4s8e.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-03-30 20:01:37.000000 dsml4s8e-0.1.3/dsml4s8e.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       36 2023-03-30 20:01:37.000000 dsml4s8e-0.1.3/dsml4s8e.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        9 2023-03-30 20:01:37.000000 dsml4s8e-0.1.3/dsml4s8e.egg-info/top_level.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-03-30 20:01:38.161506 dsml4s8e-0.1.3/setup.cfg
--rw-r--r--   0 jovyan    (1000) users      (100)      835 2023-03-24 20:07:22.000000 dsml4s8e-0.1.3/setup.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-20 11:38:44.608852 dsml4s8e-0.1.4/
+-rw-r--r--   0 jovyan    (1000) users      (100)      494 2023-04-20 11:38:44.604852 dsml4s8e-0.1.4/PKG-INFO
+-rw-rw-r--   0 jovyan    (1000) users      (100)     8588 2023-04-20 11:22:43.000000 dsml4s8e-0.1.4/README.md
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-20 11:38:44.604852 dsml4s8e-0.1.4/dsml4s8e/
+-rw-rw-r--   0 jovyan    (1000) users      (100)       22 2023-04-20 11:34:17.000000 dsml4s8e-0.1.4/dsml4s8e/__init__.py
+-rw-rw-r--   0 jovyan    (1000) users      (100)     1155 2023-04-20 11:22:43.000000 dsml4s8e-0.1.4/dsml4s8e/data_catalog.py
+-rw-rw-r--   0 jovyan    (1000) users      (100)     1657 2023-04-20 11:22:43.000000 dsml4s8e-0.1.4/dsml4s8e/define_job.py
+-rw-rw-r--   0 jovyan    (1000) users      (100)     2345 2023-04-20 11:22:43.000000 dsml4s8e-0.1.4/dsml4s8e/dotted_catalog_path.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-20 11:38:44.604852 dsml4s8e-0.1.4/dsml4s8e/dsmlcatalog/
+-rw-rw-r--   0 jovyan    (1000) users      (100)        0 2023-04-20 11:22:43.000000 dsml4s8e-0.1.4/dsml4s8e/dsmlcatalog/__init__.py
+-rw-rw-r--   0 jovyan    (1000) users      (100)     1255 2023-04-20 11:22:43.000000 dsml4s8e-0.1.4/dsml4s8e/dsmlcatalog/dagster_home.py
+-rw-rw-r--   0 jovyan    (1000) users      (100)     1488 2023-04-20 11:22:43.000000 dsml4s8e-0.1.4/dsml4s8e/dsmlcatalog/local_storage.py
+-rw-rw-r--   0 jovyan    (1000) users      (100)     6499 2023-04-20 11:22:43.000000 dsml4s8e-0.1.4/dsml4s8e/nb_op.py
+-rw-rw-r--   0 jovyan    (1000) users      (100)     1813 2023-04-20 11:22:43.000000 dsml4s8e-0.1.4/dsml4s8e/op_params_from_nb.py
+-rw-rw-r--   0 jovyan    (1000) users      (100)      518 2023-04-20 11:22:43.000000 dsml4s8e-0.1.4/dsml4s8e/storage_catalog.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-20 11:38:44.604852 dsml4s8e-0.1.4/dsml4s8e/storage_rw/
+-rw-rw-r--   0 jovyan    (1000) users      (100)        0 2023-04-20 11:22:43.000000 dsml4s8e-0.1.4/dsml4s8e/storage_rw/__init__.py
+-rw-rw-r--   0 jovyan    (1000) users      (100)      615 2023-04-20 11:22:43.000000 dsml4s8e-0.1.4/dsml4s8e/storage_rw/pandas_loacl.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-04-20 11:38:44.604852 dsml4s8e-0.1.4/dsml4s8e.egg-info/
+-rw-r--r--   0 jovyan    (1000) users      (100)      494 2023-04-20 11:38:44.000000 dsml4s8e-0.1.4/dsml4s8e.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)      530 2023-04-20 11:38:44.000000 dsml4s8e-0.1.4/dsml4s8e.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-04-20 11:38:44.000000 dsml4s8e-0.1.4/dsml4s8e.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       26 2023-04-20 11:38:44.000000 dsml4s8e-0.1.4/dsml4s8e.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        9 2023-04-20 11:38:44.000000 dsml4s8e-0.1.4/dsml4s8e.egg-info/top_level.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-04-20 11:38:44.608852 dsml4s8e-0.1.4/setup.cfg
+-rw-rw-r--   0 jovyan    (1000) users      (100)      800 2023-04-20 11:22:43.000000 dsml4s8e-0.1.4/setup.py
```

### Comparing `dsml4s8e-0.1.3/dsml4s8e/dsmlcatalog/local_storage.py` & `dsml4s8e-0.1.4/dsml4s8e/dsmlcatalog/local_storage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from dsml4s8e import storage_catalog as sc
-from dsml4s8e.nb_data_keys import DataKeys
+from dsml4s8e.data_catalog import DataCatalogPaths
 from typing import List, Dict
 
 
-def _data_key2url(
-        key: str,
+def _catalog_path2storage_path(
+        catalog_path: str,
         run_id: str,
         prefix: str
         ) -> str:
     """
-    format of data_key: <pipeline>.<component>.<notebook>.<name_data_opj>
+    format of catalog_path: <pipeline>.<component>.<notebook>.<name_data_opj>
     cdlc_stage is a stage of component development life cycle: dev, test, ops
-    url: <prefix>/<pipeline>/<component>/<notebook>/<name_data_opj>
+    return a storage path
+    format of a storagr path: <prefix>/<pipeline>/<component>/<notebook>/<name_data_opj>
     """
-    p, c, nb, e = key.split('.')
+    p, c, nb, e = catalog_path.split('.')
     return f'{prefix}/{p}/{c}/{run_id}/{nb}/{e}'
 
 
 class LoacalStorageCatalog(sc.StorageCatalogABC):
 
     def __init__(self,
                  prefix: str,
@@ -32,18 +33,18 @@
     @property
     def url_prefix(self):
         return self._prefix
 
     def is_valid(self) -> bool:
         return True
 
-    def get_outs_data_urls(self, data_kyes: DataKeys) -> Dict[str, str]:
+    def get_outs_data_paths(self, catalog: DataCatalogPaths) -> Dict[str, str]:
         return dict(
                 [(
                     k,
-                    _data_key2url(
+                    _catalog_path2storage_path(
                         k,
                         self.run_id,
                         self.url_prefix
                         )
-                 ) for k in data_kyes.keys]
+                 ) for k in catalog.paths]
             )
```

### Comparing `dsml4s8e-0.1.3/dsml4s8e/nb_data_keys.py` & `dsml4s8e-0.1.4/dsml4s8e/data_catalog.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 from dataclasses import dataclass
 import json
-from typing import List, Dict
+from typing import List
 
 
 @dataclass(frozen=True)
-class DataKeys:
+class DataCatalogPaths:
     '''
-    format of key: <pipeline>.<component>.<notebook>.<data_obj_name>
-    ins: list of input data keys
-    outs: list of output data keys
+    list of catalog data paths
+    format of catalog path: <pipeline>.<component>.<notebook>.<data_obj_name>
     '''
-    keys: tuple[str]
+    paths: tuple[str]
 
 
-class NotebookDataKeys:
+def make_data_catalog_path(op_id: str, var_name):
+    return f'{op_id}.{var_name}'
+
+
+class NotebookPaths:
     def __init__(
             self,
-            ins_data_key_dag_name: Dict[str, dict],
-            outs: List[str],
+            ins_catalog_paths: List[str],
+            outs_vars: List[str],
             op_id: str
             ):
         '''
-        ins is a list of keys of input data objects
+        ins is a list of input data paths in catalog
         outs is a list of local names of out data objects
         format of keys of data obj:
         <pipeline>.<component>.<netebook>.<data_obj_name>
         '''
-        self.ins = DataKeys(ins_data_key_dag_name.keys())
-        self.outs = DataKeys([f'{op_id}.{a}' for a in outs])
+        self.ins = DataCatalogPaths(ins_catalog_paths)
+        self.outs = DataCatalogPaths(
+            [make_data_catalog_path(op_id, var_name) for
+             var_name in outs_vars])
 
     def __str__(self):
         interface_info = {
             "ins": self.ins,
             "outs": self.outs
         }
         return json.dumps(interface_info, indent=4)
```

### Comparing `dsml4s8e-0.1.3/dsml4s8e/nb_op.py` & `dsml4s8e-0.1.4/dsml4s8e/nb_op.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from dsml4s8e import dotted_urls_names
+from dsml4s8e import dotted_catalog_path
 from dsml4s8e.storage_catalog import StorageCatalogABC
-from dsml4s8e.nb_data_keys import NotebookDataKeys
+from dsml4s8e.data_catalog import NotebookPaths
 
 import dagstermill
 
 from pathlib import Path
-from typing import Dict
+from typing import Dict, Tuple
 from functools import cached_property
 from dagster import Field
 from dataclasses import dataclass
 
 
 def op_name_from_nb_path(nb_path, level_from_root=2):
     p = Path(nb_path)
@@ -30,122 +30,161 @@
         {op_parameters_ins}
         must be declared in cell 'parameters'
         """
         super().__init__(self.message)
 
 
 @dataclass(frozen=True)
-class NbDataUrls:
+class NbDataCatalog:
     ins: object
     outs: object
 
 
 class NbOp:
-    current_op_id = 'from_jupyter'
+    _current_op_id = None
+    _current_nb_path = None
     ops: Dict[str, dict] = {}
 
+    @classmethod
+    def dotted_path2path_varname(cls, path: str):
+        return '_'.join(['path'] + path.split('.')[-2:])
+
+    @classmethod
+    def set_current_nb_path(cls, nb_path: str):
+        cls._current_nb_path = nb_path
+
+    @classmethod
+    def params(cls):
+        return cls.ops[cls._current_op_id].copy()
+
+    @classmethod
+    def _op_name_and_id_from_nb_path(
+        cls,
+        nb_path: str,
+        level_from_root: int
+    ) -> Tuple[str, str]:
+        """
+        retrun op_name, op_id
+        """
+        p = Path(nb_path)
+        level_from_root += 1
+        op_name = p.stem
+        op_id = '.'.join(list(p.parts[-level_from_root:-1]) + [op_name])
+        return p.stem, op_id
+
     def __init__(self,
                  config_schema: Dict[str, Field] = None,
                  ins: Dict[str, dict] = None,
                  outs: Dict[str, dict] = None,
-                 path: str = None,
-                 level_from_root=2
+                 level_from_root=2,
                  ) -> None:
         self._op_params = {}
         self._level_from_root = level_from_root
-        if self.current_op_id == 'from_jupyter':
-            import ipynbname
-            try:
-                path = ipynbname.path()
-                self.current_op_id, self.nb_name = op_name_from_nb_path(
-                    nb_path=path,
-                    level_from_root=self._level_from_root
-                    )
-            except Exception:
-                ...
-        self._id = self.current_op_id
-        self.ops[self._id] = self._op_params
         if config_schema:
             self._op_params['config_schema'] = config_schema
         if ins:
             self._op_params['ins'] = ins
         if outs:
             self._op_params['outs'] = outs
+        if self._current_nb_path:
+            # If the static method set_current_nb_path has been called outside.
+            # This code is executed to extract op parameters from a notebook.
+            # For more details look op_params_nb.dagstermill_op_params_from_nb
+            (
+             self._op_params['name'],
+             NbOp._current_op_id
+             ) = self._op_name_and_id_from_nb_path(
+                nb_path=self._current_nb_path,
+                level_from_root=level_from_root
+            )
+            NbOp.ops[NbOp._current_op_id] = self._op_params
 
-    def set_locals(self, locals_: Dict[str, dict]):
-        self.dagster_context = locals_['context']
-        if 'notebook_path' in self.dagster_context.op_def.tags:
-            self._id, self.nb_name = op_name_from_nb_path(
-                        nb_path=self.dagster_context.op_def.tags['notebook_path'],
-                        level_from_root=self._level_from_root
-                        )
-
-    def get_ins_data_urls(self, locals_: Dict[str, dict]) -> Dict[str, str]:
-        """
-        op_parameters_ins = op_parameters['ins']
-        op_parameters is a dict from notebook cell with tag op_parameters
-        _locals = locals() # Local symbol Table
-        'ins': {'key': 'nb_data1'} -> {key: _locals['nb_data1']}
+    def _get_ins_data_paths(self, locals_: Dict[str, dict]) -> Dict[str, str]:
+        """
+        Create the data_paths dict with keys from ins and values from locals_
+        (join by data_path).
+        Variables with names from ins dict values must be in locals_
+        else the MissedInsParameters exсeption is raised:
+        'ins': {'data_path': 'nb_data1'} ->
+               {data_path: _locals['nb_data1']}.
+        Where locals_ is a Local symbol Table returning by
+        the Build-In Python function locals().
         """
         ins: Dict[str, dict] = self._op_params['ins']
-        urls_dict = {
+        paths_dict = {
             k: locals_.get(k_alias, '')
             for k, k_alias in ins.items()
         }
-        empty_vals = [k for k, url in urls_dict.items() if not url]
+        empty_vals = [k for k, path in paths_dict.items() if not path]
         if len(empty_vals) > 0:
             raise MissedInsParameters(empty_vals, ins)
-        return urls_dict
+        return paths_dict
 
-    def get_data_urls(
+    def get_catalog(
             self,
             locals_: Dict[str, dict],
             storage_catalog: StorageCatalogABC
-            ) -> NbDataUrls:
-        self.set_locals(locals_)
+            ) -> NbDataCatalog:
+        """
+        This metod calls from notebook.
+        locals_ is a Local symbol Table
+        returning by the Build-In Python function locals().
+        """
+        dagster_context = locals_['context']
+        if 'notebook_path' in dagster_context.op_def.tags:
+            # if a notebook is executed by dagstermill
+            nb_path = dagster_context.op_def.tags['notebook_path']
+        else:
+            # if a notebook is executed by jupyter
+            nb_path = locals_['__session__']
+
+        self.nb_name, self._id = self._op_name_and_id_from_nb_path(
+                    nb_path=nb_path,
+                    level_from_root=self._level_from_root
+                    )
         op_params = self._op_params
-        self.nb_data_keys = NotebookDataKeys(
-            ins_data_key_dag_name=op_params.get('ins', {}),
-            outs=op_params.get('outs', []),
+        self.nb_data_keys = NotebookPaths(
+            ins_catalog_paths=op_params.get('ins', {}),
+            outs_vars=op_params.get('outs', []),
             op_id=self._id
         )
         _ins_dict = {}
         self._outs_dict = {}
         if 'ins' in op_params:
-            _ins_dict = self.get_ins_data_urls(locals_)
+            _ins_dict = self._get_ins_data_paths(locals_)
         if 'outs' in op_params:
-            self._outs_dict = storage_catalog.get_outs_data_urls(
-                data_kyes=self.nb_data_keys.outs,
+            self._outs_dict = storage_catalog.get_outs_data_paths(
+                catalog=self.nb_data_keys.outs,
             )
-        return NbDataUrls(
-            ins=dotted_urls_names.do_dotted_urls_names(_ins_dict),
-            outs=dotted_urls_names.do_dotted_urls_names(self._outs_dict)
+        return NbDataCatalog(
+            ins=dotted_catalog_path.do_dotted_paths(_ins_dict),
+            outs=dotted_catalog_path.do_dotted_paths(self._outs_dict)
             )
 
-    def pass_outs_to_next_step(self):
-        print('outs:')
-        for data_obj_key, url in self._outs_dict.items():
-            url_name = self.data_key2url_name(data_obj_key)
-            print(f'{url_name} = "{url}"')
+    def pass_outs_to_next_steps(self):
+        out_paths = []
+
+        print("Strings below can be pasted in cells with tags 'parameters' of next notebooks.\n")
+        for dotted_path, storage_path in self._outs_dict.items():
+            path_varname = self.dotted_path2path_varname(dotted_path)
+            out_paths.append((f"'{dotted_path}'",
+                             f"'{path_varname}'"))
+            print(f"{path_varname} = '{storage_path}'")
             dagstermill.yield_result(
-                url,
-                output_name=url_name
+                storage_path,
+                output_name=path_varname
              )
+        print("\nStrings below can be pasted in code of declaration of NbOp")
+        print("in cells with tags 'op_parameters' of next notebooks.\n")
+        for path in out_paths:
+            print(f'{path[0]}:{path[1]},')
 
     def get_context(self):
         return dagstermill.get_context(op_config=self.config)
 
     @cached_property
     def config(self):
         config_schema: Dict[str, Field] = self._op_params['config_schema']
         return {
             k: v.default_value for k, v in
             config_schema.items()
         }
-
-    @classmethod
-    def data_key2url_name(cls, data_key: str):
-        return '_'.join(['url'] + data_key.split('.')[-2:])
-
-    @classmethod
-    def params(cls):
-        return cls.ops[cls.current_op_id].copy()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dsml4s8e-0.1.3/dsml4s8e/op_params_from_nb.py` & `dsml4s8e-0.1.4/dsml4s8e/op_params_from_nb.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dsml4s8e.nb_data_keys import NotebookDataKeys
+from dsml4s8e.data_catalog import NotebookPaths
 import dsml4s8e.nb_op as op
 
 from dagster import Out, In
 import nbformat
 
 
 def uniq_name(entity_id: str):
@@ -20,43 +20,46 @@
     return {
         dag_name: In(str)
         for dag_name in nb_ins.values()
     }
 
 
 def nb_outs2dagster_outs(outs, nb_id):
-    nb_data_keys = NotebookDataKeys(
-        ins_data_key_dag_name={},
-        outs=outs,
+    nb_catalog_paths = NotebookPaths(
+        ins_catalog_paths=[],
+        outs_vars=outs,
         op_id=nb_id
     )
     return {
-        op.NbOp.data_key2url_name(k): Out(str)
-        for k in nb_data_keys.outs.keys
+        op.NbOp.dotted_path2path_varname(p): Out(str)
+        for p in nb_catalog_paths.outs.paths
     }
 
 
 def dagstermill_op_params_from_nb(nb_path: str):
     nb = nbformat.read(nb_path, as_version=4)
-    op.NbOp.current_op_id, nb_name = op.op_name_from_nb_path(nb_path)
+    params = None
     for cell in nb.cells:
         tags = []
         if cell.cell_type == 'code':
             tags = get_cell_tags(cell)
         if 'op_parameters' in tags:
+            op.NbOp.set_current_nb_path(nb_path)
+            # In this cell the object of NbOp is creaded
+            # in NbOp.__init__
             exec(cell.source)
             params = op.NbOp.params()
-    if 'ins' in params:
-        params['ins'] = nb_ins2dagster_ins(
-            nb_ins=params['ins'],
-        )
-    if 'outs' in params:
-        params['outs'] = nb_outs2dagster_outs(
-            outs=params['outs'],
-            nb_id=op.NbOp.current_op_id
-        )
-    params['notebook_path'] = nb_path
-    params['name'] = nb_name
-    params['output_notebook_name'] = f"out_{nb_name}"
-    local_path = '/'.join(nb_path.split('/')[-2:])
-    params['description'] = f"path: {local_path}"
+            if 'ins' in params:
+                params['ins'] = nb_ins2dagster_ins(
+                    nb_ins=params['ins'],
+                )
+            if 'outs' in params:
+                params['outs'] = nb_outs2dagster_outs(
+                    outs=params['outs'],
+                    nb_id=op.NbOp._current_op_id
+                )
+            params['notebook_path'] = nb_path
+            params['output_notebook_name'] = f"out_{params['name']}"
+            local_path = '/'.join(nb_path.split('/')[-2:])
+            params['description'] = f"path: {local_path}"
+            return params
     return params
```

### Comparing `dsml4s8e-0.1.3/setup.py` & `dsml4s8e-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,15 @@
     url='https://github.com/dsml4/dsml4s8e',
     author='Aleksandr Motuzov',
     author_email='motuzov@gmail.com',
     license='Apache 2.0',
     packages=['dsml4s8e', 'dsml4s8e.dsmlcatalog', 'dsml4s8e.storage_rw'],
     install_requires=['dagster',
                       'dagstermill',
-                      'dagit',
-                      'ipynbname'
+                      'dagit'
                       ],
 
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
```

