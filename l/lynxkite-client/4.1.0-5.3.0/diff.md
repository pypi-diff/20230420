# Comparing `tmp/lynxkite-client-4.1.0.tar.gz` & `tmp/lynxkite_client-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lynxkite-client-4.1.0.tar", last modified: Wed Oct 14 13:25:14 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `lynxkite-client-4.1.0.tar` & `lynxkite_client-5.3.0.tar`

### file list

```diff
@@ -1,15 +1,33 @@
-drwxr-xr-x   0 darabos   (1000) darabos   (1000)        0 2020-10-14 13:25:14.000000 lynxkite-client-4.1.0/
--rw-r--r--   0 darabos   (1000) darabos   (1000)       38 2020-10-14 13:25:14.000000 lynxkite-client-4.1.0/setup.cfg
--rw-r--r--   0 darabos   (1000) darabos   (1000)      913 2020-10-14 13:24:54.000000 lynxkite-client-4.1.0/setup.py
-drwxr-xr-x   0 darabos   (1000) darabos   (1000)        0 2020-10-14 13:25:14.000000 lynxkite-client-4.1.0/src/
-drwxr-xr-x   0 darabos   (1000) darabos   (1000)        0 2020-10-14 13:25:14.000000 lynxkite-client-4.1.0/src/lynx/
--rw-r--r--   0 darabos   (1000) darabos   (1000)    74255 2020-10-14 13:22:26.000000 lynxkite-client-4.1.0/src/lynx/kite.py
--rw-r--r--   0 darabos   (1000) darabos   (1000)   136611 2020-08-12 15:57:02.000000 lynxkite-client-4.1.0/src/lynx/operations.py
-drwxr-xr-x   0 darabos   (1000) darabos   (1000)        0 2020-10-14 13:25:14.000000 lynxkite-client-4.1.0/src/lynxkite_client.egg-info/
--rw-r--r--   0 darabos   (1000) darabos   (1000)        1 2020-10-14 13:25:14.000000 lynxkite-client-4.1.0/src/lynxkite_client.egg-info/dependency_links.txt
--rw-r--r--   0 darabos   (1000) darabos   (1000)       53 2020-10-14 13:25:14.000000 lynxkite-client-4.1.0/src/lynxkite_client.egg-info/requires.txt
--rw-r--r--   0 darabos   (1000) darabos   (1000)      272 2020-10-14 13:25:14.000000 lynxkite-client-4.1.0/src/lynxkite_client.egg-info/SOURCES.txt
--rw-r--r--   0 darabos   (1000) darabos   (1000)      705 2020-10-14 13:25:14.000000 lynxkite-client-4.1.0/src/lynxkite_client.egg-info/PKG-INFO
--rw-r--r--   0 darabos   (1000) darabos   (1000)        5 2020-10-14 13:25:14.000000 lynxkite-client-4.1.0/src/lynxkite_client.egg-info/top_level.txt
--rw-r--r--   0 darabos   (1000) darabos   (1000)      705 2020-10-14 13:25:14.000000 lynxkite-client-4.1.0/PKG-INFO
--rw-r--r--   0 darabos   (1000) darabos   (1000)      175 2020-06-29 17:36:45.000000 lynxkite-client-4.1.0/README.md
+-rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/test.sh
+-rwxr-xr-x   0        0        0      225 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/managed_tests/run.sh
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/managed_tests/test_start_stop.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/src/lynx/__init__.py
+-rw-r--r--   0        0        0    79539 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/src/lynx/kite.py
+-rw-r--r--   0        0        0   175339 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/src/lynx/operations.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/api_test_in_docker.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/strings.csv
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_boxpath.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_cleaner.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_download.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_escaping_strings.py
+-rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_external_computation.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_hive_export.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_pandas_conversion.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_spark_conversion.py
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_sql_shorthand.py
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_subworkspace_decorator.py
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_tutorials.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_workspace.py
+-rw-r--r--   0        0        0    15988 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_workspace_builder.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_workspace_decorator.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/test_workspace_with_side_effects.py
+-rw-r--r--   0        0        0  2077488 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/data/03_Airlines_Edge.csv
+-rw-r--r--   0        0        0   771231 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/data/03_Airlines_Vertex.csv
+-rw-r--r--   0        0        0   236358 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/data/beno_facebook_edges.csv
+-rw-r--r--   0        0        0    53472 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/data/beno_facebook_vertices.csv
+-rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/data/tutorial-02-test.yaml
+-rw-r--r--   0        0        0    17059 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/tests/data/tutorial-03-test.yaml
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/.gitignore
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/README.md
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 lynxkite_client-5.3.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lynxkite-client-4.1.0/src/lynx/kite.py` & `lynxkite_client-5.3.0/src/lynx/kite.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,33 +14,37 @@
 
 Example usage::
 
     import lynx.kite
     lk = lynx.kite.LynxKite()
     lk.createExampleGraph().sql('select * from graph_attributes').df()
 '''
+import atexit
 import copy
 import functools
 import json
 import os
 import random
 import sys
 import types
 import datetime
 import inspect
 import re
 import itertools
 from collections import deque, defaultdict, Counter
 from typing import (Dict, List, Union, Callable, Any, Tuple, Iterable, Set, NewType, Iterator,
-                    TypeVar, Optional, Collection)
+                    TypeVar, Optional, Collection, TYPE_CHECKING)
 import requests
 from tempfile import NamedTemporaryFile, TemporaryDirectory, mkstemp
 import textwrap
 import shutil
+import socketserver
 import lynx.operations
+if TYPE_CHECKING:
+  from pyspark.sql import SparkSession
 
 
 if sys.version_info.major < 3 or (sys.version_info.major == 3 and sys.version_info.minor < 6):
   raise Exception('At least Python version 3.6 is needed!')
 
 
 def random_filename() -> str:
@@ -177,15 +181,16 @@
   '''
   signature = inspect.signature(fn, follow_wrapped=False)
   secs = [p.name for p in signature.parameters.values()
           if p.default is SideEffectCollector.AUTO]
   assert len(secs) <= 1, f'More than one SideEffectCollector parameters found for {fn}'
 
   @functools.wraps(fn)
-  def wrapper(*args, _ws_params: List[WorkspaceParameter] = [], _ws_name: str = None, **kwargs):
+  def wrapper(*args, _ws_params: List[WorkspaceParameter] = [],
+              _ws_name: Optional[str] = None, **kwargs):
     # create a new signature on every call since we will bind different arguments per call
     signature = inspect.signature(fn, follow_wrapped=False)
     # Separate workspace parameters from the normal Python parameters.
     ws_param_bindings = {wp.name: kwargs[wp.name] for wp in _ws_params if wp.name in kwargs}
     for wp in _ws_params:
       if wp.name in signature.parameters:
         kwargs[wp.name] = pp('$' + wp.name)
@@ -320,19 +325,31 @@
   '''A connection to a LynxKite instance.
 
   Some LynxKite API methods take a connection argument which can be used to communicate with
   multiple LynxKite instances from the same session. If no arguments to the constructor are
   provided, then a connection is created using the following environment variables:
   ``LYNXKITE_ADDRESS``, ``LYNXKITE_USERNAME``, ``LYNXKITE_PASSWORD``,
   ``LYNXKITE_PUBLIC_SSL_CERT``, ``LYNXKITE_OAUTH_TOKEN``, ``LYNXKITE_SIGNED_TOKEN``.
+
+  It can also be used without a running LynxKite instance. In this case pass in a SparkSession
+  as ``spark``. This class will start a temporary LynxKite instance automatically.
+  The SparkSession must be configured with the LynxKite jar. There are two ways to do this::
+
+    pyspark --jars lynxkite-X.X.X.jar my_script.py
+
+  Or within your Python code::
+
+    spark = SparkSession.builder.config('spark.jars', 'lynxkite-X.X.X.jar').getOrCreate()
   '''
 
-  def __init__(self, username: str = None, password: str = None, address: str = None,
-               certfile: str = None, oauth_token: str = None, signed_token: str = None,
-               box_catalog: BoxCatalog = None) -> None:
+  _managed = None
+
+  def __init__(self, username: Optional[str] = None, password: Optional[str] = None, address: Optional[str] = None,
+               certfile: Optional[str] = None, oauth_token: Optional[str] = None, signed_token: Optional[str] = None,
+               box_catalog: Optional[BoxCatalog] = None, spark: Optional['SparkSession'] = None) -> None:
     '''Creates a connection object.'''
     # Authentication and querying environment variables is deferred until the
     # first request.
     self._address = address
     self._username = username
     self._password = password
     self._certfile = certfile
@@ -350,14 +367,29 @@
         'exportToCSV', 'exportToJSON', 'exportToParquet',
         'exportToJDBC', 'exportToORC', 'exportToHive',
         'exportToAVRO', 'exportToDelta',
         'exportVertexAttributesToNeo4j', 'exportEdgeAttributesToNeo4j',
         'exportGraphToNeo4j']
     self._box_catalog = box_catalog  # TODO: create standard offline box catalog
 
+    self._lynxkite = None
+    if spark:
+      assert address is None, \
+          'Do not specify connection parameters when this class is responsible for starting LynxKite.'
+      if LynxKite._managed:
+        assert LynxKite._managed.spark == spark, 'LynxKite is already running in another Spark session.'
+      else:
+        LynxKite._managed = ManagedLynxKite(spark)
+        LynxKite._managed.start()
+        # Play Framework runs on non-daemon threads. We have to shut it down when
+        # Python is finished.
+        atexit.register(LynxKite._managed.stop)
+      self._lynxkite = LynxKite._managed
+      self._address = self._lynxkite.address
+
   def home(self) -> str:
     return f'Users/{self.username()}/'
 
   def operation_names(self) -> List[str]:
     if not self._operation_names:
       box_names = self.box_catalog().box_names()
       self._operation_names = box_names + self.import_operation_names() + self.export_operation_names()
@@ -449,15 +481,15 @@
     inputs = _to_input_map(box_name, self.box_catalog().inputs(box_name), input_states)
     kwargs['sql'] = dedent(sql)
     # Use default names for unnamed inputs, custom names for the named ones.
     kwargs['input_names'] = ', '.join(self.box_catalog().inputs(box_name)[:len(args)] + input_names)
     return _new_box(self.box_catalog(), self, box_name, inputs=inputs, parameters=kwargs)
 
   def address(self) -> str:
-    return self._address or os.environ['LYNXKITE_ADDRESS']
+    return self._address or os.environ['LYNXKITE_ADDRESS'] or 'http://localhost:2200/'
 
   def username(self) -> str:
     username = self._username or os.environ.get('LYNXKITE_USERNAME')
     if not username:
       signed_token = self.signed_token()
       assert signed_token, 'Can not determine username. Either set username or signed token.'
       return signed_token.split('|')[0]
@@ -587,29 +619,29 @@
 
   def list_dir(self, dir: str = '') -> List[types.SimpleNamespace]:
     '''List the objects in a directory, with their names, types, notes,
     and other optional data about graphs.'''
 
     return self._send('/remote/list', dict(path=dir)).entries
 
-  def upload(self, data: bytes, name: str = None):
+  def upload(self, data: bytes, name: Optional[str] = None):
     '''Uploads a file that can then be used in import methods.
 
       prefixed_path = lk.upload('id,name\\n1,Bob')
     '''
     if name is None:
       name = 'remote-api-upload'  # A hash will be added anyway.
     return self._post('/ajax/upload', files=dict(file=(name, data))).text
 
-  def uploadCSVNow(self, data: bytes, name: str = None):
+  def uploadCSVNow(self, data: bytes, name: Optional[str] = None):
     '''Uploads CSV data and returns a table state.'''
     filename = self.upload(data, name)
     return self.importCSVNow(filename=filename)
 
-  def uploadParquetNow(self, data: bytes, name: str = None):
+  def uploadParquetNow(self, data: bytes, name: Optional[str] = None):
     '''Uploads Parquet file and returns a table state.'''
     filename = self.upload(data, name)
     return self.importParquetNow(filename=filename)
 
   def clean_file_system(self):
     """Deletes the data files which are not referenced anymore."""
     return self._send('/remote/cleanFileSystem')
@@ -634,15 +666,15 @@
   def fetch_states(self, boxes: List[SerializedBox],
                    parameters: Dict = dict()) -> Dict[Tuple[str, str], types.SimpleNamespace]:
     res = self._send(
         '/ajax/runWorkspace', dict(workspace=dict(boxes=boxes), parameters=parameters))
     return {(o.boxOutput.boxId, o.boxOutput.id): o for o in res.outputs}
 
   def save_workspace_recursively(self, ws: 'Workspace',
-                                 save_under_root: str = None) -> Tuple[str, str]:
+                                 save_under_root: Optional[str] = None) -> Tuple[str, str]:
     if save_under_root is None:
       ws_root = _random_ws_folder()
     else:
       ws_root = save_under_root
     main_name = ws.safename()
     needed_custom_boxes = self.recursively_collect_customboxes(ws, main_name)
     needed_ws = {(path, box.workspace) for path, box in needed_custom_boxes}
@@ -677,15 +709,15 @@
       if (box_path, box.workspace) in collected:
         continue
       collected.add((box_path, box))
       collected.update(self.recursively_collect_customboxes(box.workspace, box_path))
     return collected
 
   def fetch_workspace_output_states(self, ws: 'Workspace',
-                                    save_under_root: str = None,
+                                    save_under_root: Optional[str] = None,
                                     ) -> Dict[Tuple[str, str], types.SimpleNamespace]:
     ws_root, _ = self.save_workspace_recursively(ws, save_under_root)
     return self.fetch_states(ws.to_json(ws_root, ws.safename()))
     # TODO: clean up saved workspaces if save_under_root is not set.
 
   def get_state_id(self, state: 'State') -> str:
     ws = Workspace(terminal_boxes=[state.box], name='Anonymous')
@@ -759,17 +791,17 @@
 
   def create_dir(self, path: str, privacy: str = 'public-read'):
     return self._send(
         '/ajax/createDirectory',
         dict(name=path, privacy=privacy))
 
   def _workspace(self,
-                 name: str = None,
+                 name: Optional[str] = None,
                  parameters: List[WorkspaceParameter] = [],
-                 inputs: List[str] = None,
+                 inputs: Optional[List[str]] = None,
                  with_side_effects: bool = False
                  ) -> Callable[[Callable[..., Dict[str, 'State']]], 'Workspace']:
     se_collector = SideEffectCollector()
 
     def ws_decorator(builder_fn):
       real_name = builder_fn.__name__ if not name else name
       if inputs:
@@ -788,24 +820,24 @@
                        terminal_boxes=outputs + se_collector.top_level_side_effects,
                        side_effect_paths=list(se_collector.all_triggerables()),
                        input_boxes=input_boxes,
                        ws_parameters=parameters)
     return ws_decorator
 
   def workspace(self,
-                name: str = None,
+                name: Optional[str] = None,
                 parameters: List[WorkspaceParameter] = [],
-                inputs: List[str] = None,
+                inputs: Optional[List[str]] = None,
                 ) -> Callable[[Callable[..., Dict[str, 'State']]], 'Workspace']:
     return self._workspace(name, parameters, inputs, with_side_effects=False)
 
   def workspace_with_side_effects(self,
-                                  name: str = None,
+                                  name: Optional[str] = None,
                                   parameters: List[WorkspaceParameter] = [],
-                                  inputs: List[str] = None,
+                                  inputs: Optional[List[str]] = None,
                                   ) -> Callable[[Callable[..., Dict[str, 'State']]], 'Workspace']:
     return self._workspace(name, parameters, inputs, with_side_effects=True)
 
   def trigger_box(self,
                   workspace_name: str,
                   box_id: str,
                   custom_box_stack: List[str] = []):
@@ -839,18 +871,105 @@
         warnings.warn(msg)
     else:
       kwargs = {'index': index}
     with NamedTemporaryFile() as f:
       df.to_parquet(f.name, **kwargs)
       return self.uploadParquetNow(f.read())
 
+  def from_spark(self, df, *, write_parquet=False):
+    '''
+    Converts a Spark DataFrame to a LynxKite table.
+
+    Set "write_parquet" to pass in the DataFrame by writing it as a Parquet file.
+    This is slower, but works even if LynxKite and PySpark are in separate Spark sessions.
+    '''
+    if write_parquet:
+      filename = 'DATA$/python-imports/' + datetime.datetime.now().strftime('%Y-%d-%m_%H%M%S.%f')
+      resolved = self.get_prefixed_path(filename).resolved
+      df.write.parquet(resolved)
+      return self.importParquetNow(filename=filename)
+    else:
+      assert self._lynxkite, 'Run LynxKite in the same Spark session, or use "write_parquet".'
+      guid = self._lynxkite.importDataFrame(df)
+      return SingleOutputAtomicBox(
+          self.box_catalog(), self, 'importParquet', inputs={}, parameters={
+              'filename': 'from PySpark',
+              'imported_table': guid,
+              'last_settings': json.dumps({
+                  'filename': 'from PySpark',
+                  'sql': '', 'eager': 'yes', 'imported_columns': '', 'schema': '', 'limit': '',
+              }),
+          },
+          output_name='table')
+
   def set_executors(self, count):
     return self._send('/remote/setExecutors', {'count': count})
 
 
+def _get_free_ports(n):
+  '''Returns n port numbers that are currently free.'''
+  servers = [socketserver.TCPServer(('localhost', 0), None) for _ in range(n)]
+  for s in servers:
+    s.__enter__()
+  ports = [s.server_address[1] for s in servers]
+  for s in servers:
+    s.__exit__()
+  return ports
+
+
+class ManagedLynxKite:
+  '''Takes care of starting and stopping LynxKite in a SparkSession.'''
+
+  def __init__(self, spark, **kwargs):
+    self.assert_jar_is_loaded(spark)
+    self.spark = spark
+    self.storage = TemporaryDirectory()
+    tmp = self.storage.name
+    kite_http_port, kite_https_port, sphynx_port = _get_free_ports(3)
+    self.set_env(
+        KITE_META_DIR=f'{tmp}/meta',
+        KITE_DATA_DIR=f'file:{tmp}/data',
+        KITE_HTTP_PORT=kite_http_port,
+        KITE_HTTPS_PORT=kite_https_port,
+        SPHYNX_HOST='localhost',
+        SPHYNX_PORT=sphynx_port,
+        ORDERED_SPHYNX_DATA_DIR=f'{tmp}/sphynx/ordered',
+        UNORDERED_SPHYNX_DATA_DIR=f'{tmp}/sphynx/unordered',
+        **kwargs)
+    self.address = f'http://localhost:{kite_http_port}'
+
+  def assert_jar_is_loaded(self, spark):
+    assert (
+        not isinstance(spark._jvm.com.lynxanalytics.biggraph.LynxKite, type(spark._jvm.com.nonexistent.package))), \
+        'The LynxKite jar has not been loaded in this SparkSession.'
+
+  def set_env(self, **kwargs):
+    jvm = self.spark._jvm
+    cfg = jvm.java.util.ArrayList()
+    for k, v in kwargs.items():
+      cfg.append(jvm.Tuple2(k, str(v)))
+    cfg = jvm.scala.collection.JavaConversions.asScalaBuffer(cfg)
+    jvm.com.lynxanalytics.biggraph.Environment.set(cfg)
+
+  def start(self):
+    '''Returns when LynxKite is ready to be used.'''
+    self.spark._jvm.com.lynxanalytics.biggraph.LynxKite.start()
+
+  def stop(self):
+    self.spark._jvm.com.lynxanalytics.biggraph.LynxKite.stop()
+
+  def importDataFrame(self, df):
+    return self.spark._jvm.com.lynxanalytics.biggraph.LynxKite.importDataFrame(df._jdf)
+
+  def getDataFrame(self, guid):
+    jdf = self.spark._jvm.com.lynxanalytics.biggraph.LynxKite.getDataFrame(guid)
+    from pyspark.sql import DataFrame
+    return DataFrame(jdf, self.spark)
+
+
 class State:
   '''Represents a named output plug of a box.
 
   It can recursively store the boxes which are connected to the input plugs of
   the box of this state.
   '''
 
@@ -911,14 +1030,15 @@
   def segmentation(self, name: str) -> 'SingleOutputAtomicBox':
     '''Returns the named segmentation as a base project.
 
     Example usage:
     ```
     graph = lk.createExampleGraph().findConnectedComponents(name='seg1')
     segmentation = graph.segmentation('seg1')
+    ```
     '''
     return self.takeSegmentationAsBaseGraph(apply_to_graph='.' + name)
 
   def _select_all(self, table):
     return self.sql(f'select * from `{table}`')
 
   def __dir__(self) -> Iterable[str]:
@@ -950,41 +1070,58 @@
 
     table = self.get_table_data(limit)
     header = [c.name for c in table.header]
     types = [c.dataType for c in table.header]
     data = [[get(c, t) for (c, t) in zip(r, types)] for r in table.data]
     return pandas.DataFrame(data, columns=header)
 
+  def spark(self, spark: Optional['SparkSession'] = None):
+    '''
+    Returns the table as a Spark DataFrame.
+    The "spark" parameter must be set if LynxKite was not started from Python.
+    In this case the DataFrame is read from a Parquet file.
+    '''
+    lk = self.box.lk
+    if spark:
+      t = self.persist()
+      t.compute()
+      guid = t._get_state_id()  # The TableOutputState ID is the table GUID.
+      path = lk.get_prefixed_path('DATA$/tables/' + guid)
+      return spark.read.parquet(path.resolved)
+    else:
+      assert lk._lynxkite, 'Must provide "spark" parameter if LynxKite was not started from Python.'
+      guid = self._get_state_id()
+      return lk._lynxkite.getDataFrame(guid)
+
   def columns(self):
     '''Returns a list of columns if this state is a table.'''
     return list(self.df(0).columns)
 
   def get_table_data(self, limit: int = -1) -> types.SimpleNamespace:
     '''Returns the "raw" table data if this state is a table.'''
-    return self.box.lk.get_table_data(self.box.lk.get_state_id(self), limit)
+    return self.box.lk.get_table_data(self._get_state_id(), limit)
 
   def get_graph(self) -> types.SimpleNamespace:
     '''Returns the graph metadata if this state is a graph.'''
-    return self.box.lk.get_graph(self.box.lk.get_state_id(self))
+    return self.box.lk.get_graph(self._get_state_id())
 
   def get_progress(self):
     '''Returns progress info about the state.'''
-    lk = self.box.lk
-    state_id = lk.get_state_id(self)
-    progress = lk._ask('/ajax/long-poll', dict(syncedUntil=0, stateIds=[state_id]))
+    state_id = self._get_state_id()
+    progress = self.box.lk._ask('/ajax/long-poll', dict(syncedUntil=0, stateIds=[state_id]))
     return progress.progress.__dict__[state_id]
 
   def run_export(self) -> str:
     '''Triggers the export if this state is an ``exportResult``.
 
     Returns the prefixed path of the exported file. This method is deprecated,
     only used in tests, where we need the export path.
     '''
     lk = self.box.lk
-    state_id = lk.get_state_id(self)
+    state_id = self._get_state_id()
     export = lk.get_export_result(state_id)
     if export.result.computeProgress != 1:
       scalar = lk.get_graph_attribute(export.result.id)
       assert scalar.string == 'Export done.', scalar.string
       export = lk.get_export_result(state_id)
       assert export.result.computeProgress == 1, 'Failed to compute export result graph attribute.'
     return export.parameters.path
@@ -994,24 +1131,23 @@
 
     Uses a temporary folder to save a temporary workspace for this computation.
     '''
     self.computeInputs().trigger()
 
   def save_snapshot(self, path: str) -> None:
     '''Save this state as a snapshot under path.'''
-    lk = self.box.lk
-    state_id = lk.get_state_id(self)
-    lk.save_snapshot(path, state_id)
+    self.box.lk.save_snapshot(path, self._get_state_id())
 
   def save_to_sequence(self, tss, date: datetime.datetime) -> None:
     '''Save this state to the ``tss`` TableSnapshotSequence with ``date`` as
     the date of the snapshot.'''
-    lk = self.box.lk
-    state_id = lk.get_state_id(self)
-    tss.save_to_sequence(state_id, date)
+    tss.save_to_sequence(self._get_state_id(), date)
+
+  def _get_state_id(self):
+    return self.box.lk.get_state_id(self)
 
 
 class Placeholder:
   '''Universal placeholder. Use it whenever you need to hold a place.'''
 
   def __init__(self, value=None) -> None:
     self.value = value
@@ -1167,15 +1303,15 @@
 
   def pandas(self):
     '''Returns a Pandas DataFrame.'''
     import pandas
     downloaded = self.lk_table.download()
     return pandas.read_parquet(downloaded)
 
-  def spark(self, spark):
+  def spark(self, spark: 'SparkSession'):
     '''Takes a SparkSession as the argument and returns the table as a Spark DataFrame.'''
     downloaded = self.lk_table.download()
     return spark.read.parquet("file://" + downloaded)
 
   def lk(self) -> State:
     '''Returns a LynxKite State.'''
     return self._lk.importParquetNow(filename=self.lk_table.lk_path)
@@ -1201,15 +1337,15 @@
   '''Represents a box in a workspace segment.
 
   It can store workspace segments, connected to its input plugs.
   '''
 
   def __init__(self, box_catalog: BoxCatalog, lk: LynxKite,
                inputs: Dict[str, State], parameters: Dict[str, Any],
-               manual_box_id: str = None) -> None:
+               manual_box_id: Optional[str] = None) -> None:
     self.bc = box_catalog
     self.lk = lk
     self.inputs = inputs
     self.all_parameters = parameters
     self.parameters: Dict[str, str] = {}
     self.parametric_parameters: Dict[str, str] = {}
     self.outputs: Set[str] = set()
@@ -1291,15 +1427,15 @@
   '''
   An ``AtomicBox`` is a ``Box`` that can not be further decomposed. It corresponds to a single
   frontend operation.
   '''
 
   def __init__(self, box_catalog: BoxCatalog, lk: LynxKite, operation: str,
                inputs: Dict[str, State], parameters: Dict[str, Any],
-               manual_box_id: str = None) -> None:
+               manual_box_id: Optional[str] = None) -> None:
     super().__init__(box_catalog, lk, inputs, parameters, manual_box_id)
     self.operation = operation
     self.outputs = set(self.bc.outputs(operation))
     exp_inputs = set(self.bc.inputs(operation))
     got_inputs = inputs.keys()
     assert got_inputs == exp_inputs, 'Got box inputs: {}. Expected: {}'.format(
         got_inputs, exp_inputs)
@@ -1324,15 +1460,15 @@
   '''
   An ``AtomicBox`` with a single output. This makes chaining multiple operations after each other
   possible.
   '''
 
   def __init__(self, box_catalog: BoxCatalog, lk: LynxKite, operation: str,
                inputs: Dict[str, State], parameters: Dict[str, Any], output_name: str,
-               manual_box_id: str = None) -> None:
+               manual_box_id: Optional[str] = None) -> None:
     AtomicBox.__init__(self, box_catalog, lk, operation, inputs, parameters, manual_box_id)
     State.__init__(self, self, output_name)
 
 
 class DataFrameSender:
   '''Class to send some dataframe to LynxKite in Parquet format.
     We do this by saving the dataframe to a local Parquet file
@@ -1379,15 +1515,15 @@
 class ExternalComputationBox(SingleOutputAtomicBox):
   '''
   A box that runs external computation when triggered. Use it via ``@external``.
   '''
 
   def __init__(self, box_catalog: BoxCatalog, lk: LynxKite,
                inputs: List[State], parameters: Dict[str, Any],
-               fn: Callable, args: inspect.BoundArguments, manual_box_id: str = None) -> None:
+               fn: Callable, args: inspect.BoundArguments, manual_box_id: Optional[str] = None) -> None:
     SingleOutputAtomicBox.__init__(
         self, box_catalog, lk, f'externalComputation{len(inputs)}',
         {str(i + 1): inputs[i] for i in range(len(inputs))}, parameters, 'table', manual_box_id)
     self.fn = fn
     self.args = args
 
   def _trigger_in_ws(self, wsname: str, box: str, stack: List[str]) -> None:
@@ -1438,15 +1574,15 @@
 class CustomBox(Box):
   '''
   A ``CustomBox`` is a ``Box`` composed of multiple other boxes.
   '''
 
   def __init__(self, box_catalog: BoxCatalog, lk: LynxKite, workspace: 'Workspace',
                inputs: Dict[str, State], parameters: Dict[str, Any],
-               manual_box_id: str = None) -> None:
+               manual_box_id: Optional[str] = None) -> None:
     super().__init__(box_catalog, lk, inputs, parameters, manual_box_id)
     self.workspace = workspace
     self.outputs = set(workspace.outputs)
     exp_inputs = set(workspace.inputs)
     got_inputs = inputs.keys()
     assert got_inputs == exp_inputs, 'Got box inputs: {}. Expected: {}'.format(
         got_inputs, exp_inputs)
@@ -1489,15 +1625,15 @@
   '''
   An ``CustomBox`` with a single output. This makes chaining multiple operations after each other
   possible.
   '''
 
   def __init__(self, box_catalog: BoxCatalog, lk: LynxKite, workspace: 'Workspace',
                inputs: Dict[str, State], parameters: Dict[str, Any], output_name: str,
-               manual_box_id: str = None) -> None:
+               manual_box_id: Optional[str] = None) -> None:
     CustomBox.__init__(self, box_catalog, lk, workspace, inputs, parameters, manual_box_id)
     State.__init__(self, self, output_name)
 
 
 def _python_name(name: str) -> str:
   '''Transforms a space separated string into a camelCase format.
 
@@ -2004,15 +2140,7 @@
     return obj.__dict__
   return obj
 
 
 def to_simple_dicts(obj):
   '''Converts a SimpleNamespace structure (as returned from LynxKite requests) into simple dicts.'''
   return json.loads(json.dumps(obj, default=_json_encode))
-
-
-class PizzaBox(LynxKite):
-
-  def __init__(self):
-    super().__init__(address='https://pizzabox.lynxanalytics.com/')
-    assert self.oauth_token() or self.signed_token(), \
-        'Please set LYNXKITE_OAUTH_TOKEN or LYNXKITE_SIGNED_TOKEN.'
```

### Comparing `lynxkite-client-4.1.0/src/lynx/operations.py` & `lynxkite_client-5.3.0/src/lynx/operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -280,48 +280,79 @@
   You can use this operation for example to evaluate different colocation results against
   a reference result.
 
   :param golden:   Segmentation containing the golden edges.
   :param test:   Segmentation containing the test edges.
   '''
 
-def computeCentrality(name, maxdiameter, algorithm, bits, direction):
-  '''  Calculates an approximation of the centrality for every vertex. Higher centrality means that
+def computeAssortativity(name, attr):
+  '''  Assortativity is the correlation in the values of an attribute
+  along the edges of the graph. A high assortativity means connected vertices
+  often have similar attribute values.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1Assortativity.html>`_ implementation.
+
+  :param name:   The new graph attribute will be created under this name.
+  :param attr:   The attribute in which you are interested in correlations along the edges.
+  '''
+
+def computeCentrality(name, algorithm, direction, weight, samples, maxdiameter, bits):
+  '''  Calculates a centrality metric for every vertex. Higher centrality means that
   the vertex is more embedded in the graph. Multiple different centrality measures have been defined
   in the literature. You can choose the specific centrality measure as a parameter to this operation.
 
   :param name:   The new attribute will be created under this name.
-  :param maxdiameter:   The algorithm works by counting the shortest paths up to a certain length in each iteration.
+  :param algorithm:   - **Average distance**
+    (or `closeness centrality <https://en.wikipedia.org/wiki/Centrality#Closeness_centrality>`_)
+    of the vertex A is the sum of the shortest paths to A divided by the size of its coreachable set.
+    - The https://en.wikipedia.org/wiki/Betweenness_centrality
+  :param direction:   - `incoming edges`: Calculating paths *from* vertices.
+     - `outgoing edges`: Calculating paths *to* vertices.
+     - `all edges`: Calculating paths to both directions - effectively on an undirected graph.
+  :param weight:   Some of the centrality algorithms can take the selected edge weights into account.
+  :param samples:   Some of the estimation methods are based on picking a sample of vertices. This parameter
+    controls the size of this sample. A bigger sample leads to a more accurate estimate
+    and a longer computation time.
+  :param maxdiameter:   Some algorithms (harmonic, Lin, and average distance)
+    work by counting the shortest paths up to a certain length in each iteration.
     This parameter sets the maximal length to check, so it has a strong influence over the run
     time of the operation.
     +
     A setting lower than the actual diameter of the graph can theoretically introduce unbounded error
     to the results. In typical small world graphs this effect may be acceptable, however.
-  :param algorithm:   - The https://en.wikipedia.org/wiki/Centrality#Harmonic_centrality
-  :param bits:   The centrality algorithm is an approximation. This parameter sets the trade-off between
+  :param bits:   Some centrality algorithms (harmonic, Lin, and average distance) are approximations.
+    This parameter sets the trade-off between
     the quality of the approximation and the memory and time consumption of the algorithm.
     In most cases the default value is good enough. On very large graphs it may help to use
     a lower number in order to speed up the algorithm or meet memory constraints.
-  :param direction:   - `incoming edges`: Calculating paths *from* vertices.
-     - `outgoing edges`: Calculating paths *to* vertices.
-     - `all edges`: Calculating paths to both directions - effectively on an undirected graph.
   '''
 
 def computeClusteringCoefficient(name):
   '''  Calculates the local
   `clustering coefficient <http://en.wikipedia.org/wiki/Clustering_coefficient>`_
   attribute for every vertex. It quantifies how close the
   vertex's neighbors are to being a clique. In practice a high (close to
   1.0) clustering coefficient means that the neighbors of a vertex are
   highly interconnected, 0.0 means there are no edges between the
   neighbors of the vertex.
 
   :param name:   The new attribute will be created under this name.
   '''
 
+def computeCoverageOfSegmentation(name, weight):
+  '''  Computes a scalar for a non-overlapping segmentation.
+  Coverage is the fraction of edges that connect vertices within the same segment.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1Coverage.html>`_
+  implementation.
+
+  :param name:   This box creates a new vertex attribute on the segmentation by this name.
+  :param weight:   An edge attribute can be used to weight the edges in the coverage computation.
+  '''
+
 def computeDegree(name, direction):
   '''  For every vertex, this operation calculates either the number of edges it is connected to
   or the number of neighboring vertices it is connected to.
   You can use the `Count` parameter to control this calculation:
   choosing one of the 'edges' settings can result in a neighboring
   vertex being counted several times (depending on the number of edges between
   the vertex and the neighboring vertex); whereas choosing one of the 'neighbors' settings
@@ -341,14 +372,30 @@
        that have an incoming edge from A.
      - `all neighbors`: For each vertex A, count those vertices
        that either have an outgoing edge to or an incoming edge from A.
      - `symmetric neighbors`: For each vertex A, count those vertices
        that have both an outgoing edge to and an incoming edge from A.
   '''
 
+def computeDiameter(name, max_error):
+  '''  The diameter of a graph is the maximal shortest-distance path length
+  between two vertices. All vertex pairs are at most this far from each
+  other.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1Diameter.html>`_
+  implementation.
+
+  :param name:   The new graph attribute will be created under this name.
+  :param max_error:   Set to 0 to get the exact diameter. This may require a lot of computation, however.
+    +
+    Set to a value greater than 0 to use a faster computation that gives lower and
+    upper bounds on the diameter. With 0.1 maximum relative error, for example, the
+    upper bound will be no more than 10% greater than the true diameter.
+  '''
+
 def computeDispersion(name):
   '''  Calculates the extent to which two people's mutual friends are not themselves well-connected.
   The dispersion attribute for an A→B edge is the number of pairs of nodes that are both
   connected to A and B but are not directly connected to each other.
 
   Dispersion ignores edge directions.
 
@@ -378,21 +425,77 @@
   :param starting_distance:   A numeric attribute that specifies the initial distances of the vertices that we
     consider already reachable before starting this operation. (In the above example,
     specify this for the elements of the starting set, and leave this undefined for
     the rest of the vertices.)
   :param iterations:   The maximum number of edges considered for a shortest-distance path.
   '''
 
+def computeEdgeCutOfSegmentation(name, weight):
+  '''  Computes a scalar for a non-overlapping segmentation.
+  Edge cut is the total weight of the edges going between different segments.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1EdgeCut.html>`_
+  implementation.
+
+  :param name:   This box creates a new vertex attribute on the segmentation by this name.
+  :param weight:   An edge attribute can be used as edge weight.
+  '''
+
+def computeEffectiveDiameter(name, ratio, algorithm, bits, approximations):
+  '''  The effective diameter is a distance within which a given portion
+  of vertices can be found from each other.
+
+  For example, at most
+  `six degrees of separation <https://en.wikipedia.org/wiki/Six*degrees*of_separation>`_
+  are between most people on Earth. There may be hermits and lost tribes
+  that would push the true diameter above 6, but they are a minority. If we ignore 1%
+  of the population and find that the remaining 99% have a true diameter of 6,
+  we can say that the graph has an *effective* diameter of 6.
+
+  Uses the
+  `exact <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1EffectiveDiameter.html>`_
+  and
+  `estimated <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1EffectiveDiameterApproximation.html>`_
+  NetworKit implementations.
+
+  :param name:   The new graph attribute will be created under this name.
+  :param ratio:   The fraction of the vertices to keep.
+  :param algorithm:   Whether to compute the effective diameter exactly (slower) or approximately (faster).
+  :param bits:   For estimating the effective diameter the
+    http://www.cs.cmu.edu/~christos/PUBLICATIONS/kdd02-anf.pdf
+  :param approximations:   For estimating the effective diameter the
+    http://www.cs.cmu.edu/~christos/PUBLICATIONS/kdd02-anf.pdf
+  '''
+
 def computeEmbeddedness(name):
   '''  `Edge embeddedness <https://arxiv.org/abs/1009.1686>`_ is the overlap size of vertex neighborhoods along
   the edges. If an A→B edge has an embeddedness of `N`, it means A and B have `N` common neighbors.
 
   :param name:   The new attribute will be created under this name.
   '''
 
+def computeHubDominance(name):
+  '''  Computes the hub dominance metric for each segment in a segmentation.
+  The hub dominance of a segment is the highest internal degree in the segment
+  divided by the highest *possible* internal degree. (The segment size minus one.)
+
+  If a segment has a vertex that is connected to all other vertices in that segment
+  then its hub dominance will be 1. This metric is useful for comparing the structures
+  that make up the different segments in a segmentation.
+
+  For further analysis and theory see
+  `Characterizing the community structure of complex networks <https://arxiv.org/abs/1005.4376>`_
+  by Lancichinetti et al.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1CoverHubDominance.html>`_
+  implementation.
+
+  :param name:   This box creates a new vertex attribute on the segmentation by this name.
+  '''
+
 def computeHyperbolicEdgeProbability(radial, angular):
   '''  Adds edge attribute *hyperbolic edge probability* based on
   hyperbolic distances between vertices. This indicates
   how likely that edge would be to exist if the input graph was
   probability x similarity-grown.
   On a general level it is a metric of *edge strength*.
   Probabilities are guaranteed to be 0
@@ -429,14 +532,35 @@
    - For table inputs, it computes the table.
    - For graph inputs, it computes the vertices and edges, all attributes,
      and the same transitively for all segments plus the segmentation links.
 
 
   '''
 
+def computeModularityOfSegmentation(name, weight):
+  '''  Computes a scalar for a non-overlapping segmentation.
+  If the vertices were connected randomly while preserving the degrees,
+  a certain fraction of all edges would fall within each segment.
+  We subtract this from the observed fraction of edges that fall within
+  the segments. Modularity is the total observed difference.
+
+  A modularity of 0 means the relationship between internal edges and
+  external edges is consistent with randomly selected edges or segments.
+  A positive modularity means more internal edges than would be expected
+  by chance. A negative modularity means less internal edges than would
+  be expected by chance.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1Modularity.html>`_
+  implementation.
+
+  :param name:   This box creates a new vertex attribute on the segmentation by this name.
+  :param weight:   An edge attribute can be used to weight the edges instead of just looking at
+    edge counts.
+  '''
+
 def computePagerank(name, weights, iterations, damping, direction):
   '''  Calculates `PageRank <http://en.wikipedia.org/wiki/PageRank>`_ for every vertex.
   PageRank is calculated by simulating random walks on the graph. Its PageRank
   reflects the likelihood that the walk leads to a specific vertex.
 
   Let's imagine a social graph with information flowing along the edges. In this case high
   PageRank means that the vertex is more likely to be the target of the information.
@@ -455,28 +579,112 @@
   :param direction:   - `incoming edges`: Simulate random walk in the reverse edge direction.
        Finds the most influential sources.
      - `outgoing edges`: Simulate random walk in the original edge direction.
        Finds the most popular destinations.
      - `all edges`: Simulate random walk in both directions.
   '''
 
+def computeSegmentConductance(name, weight):
+  '''  Computes the conductance of each segment in a non-overlapping segmentation.
+  The conductance of a segment is the number of edges going between the segment
+  and the rest of the graph divided by sum of the degrees in the segment or the rest
+  of the graph (whichever is smaller).
+
+  A high conductance value indicates a segment that is strongly connected to the rest
+  of the graph. A value over 0.5 means more edges going out of the segment than
+  edges inside it.
+
+  See `Experiments on Density-Constrained Graph Clustering <https://arxiv.org/abs/1112.2143>`_
+  by Görke et al for details and analysis.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1IsolatedInterpartitionConductance.html>`_
+  implementation.
+
+  :param name:   This box creates a new vertex attribute on the segmentation by this name.
+  :param weight:   The definition can be rephrased to apply to weighted graphs. In this case
+    the total weight of the cut is compared to the weighted degrees.
+  '''
+
+def computeSegmentDensity(name):
+  '''  Computes the density of each segment in a non-overlapping segmentation.
+  The density of a segment is the number of internal edges divided by the
+  number of possible internal edges.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1IntrapartitionDensity.html>`_
+  implementation.
+
+  :param name:   This box creates a new vertex attribute on the segmentation by this name.
+  '''
+
+def computeSegmentExpansion(name, weight):
+  '''  Computes the expansion of each segment in a non-overlapping segmentation.
+  The expansion of a segment is the number of edges going between the segment
+  and the rest of the graph divided by the number of vertices in the segment or 
+  in the rest of the graph (whichever is smaller).
+
+  A high expansion value indicates a segment that is strongly connected to the rest
+  of the graph. A value over 1 means the vertices in this segment have more than
+  one external neighbor on average.
+
+  See `Experiments on Density-Constrained Graph Clustering <https://arxiv.org/abs/1112.2143>`_
+  by Görke et al for details and analysis.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1IsolatedInterpartitionExpansion.html>`_
+  implementation.
+
+  :param name:   This box creates a new vertex attribute on the segmentation by this name.
+  :param weight:   The definition can be rephrased to apply to weighted graphs. In this case
+    the total weight of the cut is compared to the weighted degrees.
+  '''
+
+def computeSegmentFragmentation(name):
+  '''  Computes the fragmentation of each segment in a non-overlapping segmentation.
+  The fragmentation of a segment is one minus the ratio of the size of its largest
+  component and the whole segment.
+
+  A segment that is entirely connected will have a fragmentation of zero.
+  If the fragmentation approaches one, it will be made up of smaller and
+  smaller components.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1PartitionFragmentation.html>`_
+  implementation.
+
+  :param name:   This box creates a new vertex attribute on the segmentation by this name.
+  '''
+
+def computeSegmentStability(name):
+  '''  Computes the stability of each segment in a non-overlapping segmentation.
+  A vertex is considered stable if it has more neighbors inside the
+  segment than outside. The stability of a segment is the fraction of
+  its vertices that are stable.
+
+  A high stability value (close to 1) indicates a segment where vertices are
+  more connected internally than externally. A stability lower than 0.5 means
+  that the majority of neighbors are external for more than half of the vertices.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1StablePartitionNodes.html>`_
+  implementation.
+
+  :param name:   This box creates a new vertex attribute on the segmentation by this name.
+  '''
+
 def connectVerticesOnAttribute(fromattr, toattr):
   '''  Creates edges between vertices that are equal in a chosen attribute. If the source attribute of A
   equals the destination attribute of B, an A→B edge will be generated.
 
   The two attributes must be of the same data type.
 
   For example, if you connect nodes based on the "name" attribute, then everyone called "John
   Smith" will be connected to all the other "John Smiths".
 
   :param fromattr:   An A→B edge is generated when this attribute on A matches the destination attribute on B.
   :param toattr:   An A→B edge is generated when the source attribute on A matches this attribute on B.
   '''
 
-def convertEdgeAttributeToDouble(attr):
+def convertEdgeAttributeToNumber(attr):
   '''  Converts the selected `String` typed edge attributes to the `number` type.
 
   The attributes will be converted in-place. If you want to keep the original `String` attribute as
   well, make a copy first!
 
   :param attr:   The attributes to be converted.
   '''
@@ -486,15 +694,15 @@
 
   The attributes will be converted in-place. If you want to keep the original String attribute as
   well, make a copy first!
 
   :param attr:   The attributes to be converted.
   '''
 
-def convertVertexAttributeToDouble(attr):
+def convertVertexAttributeToNumber(attr):
   '''  Converts the selected `String` typed vertex attributes to the `number` type.
 
   The attributes will be converted in-place. If you want to keep the original `String` attribute as
   well, make a copy first!
 
   :param attr:   The attributes to be converted.
   '''
@@ -597,14 +805,76 @@
   Note that correlation is undefined if at least one of the
   attributes is a constant.
 
   :param attra:   The correlation of these two attributes will be calculated.
   :param attrb:   The correlation of these two attributes will be calculated.
   '''
 
+def createAGraphWithCertainDegrees(size, degrees, algorithm, seed):
+  '''  Creates a graph in which the distribution of vertex degrees is as specified.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1StaticDegreeSequenceGenerator.html>`_ implementation.
+
+  :param size:   The created graph will have this many vertices.
+  :param degrees:   The algorithm will try to ensure that an equal number of vertices will
+    have each of the listed degrees. For example, generating 30 vertices with a degree list
+    of "1, 1, 5" will result in 20 vertices having degree 1 and 10 vertices having degree 5.
+  :param algorithm:   The algorithm to use.
+    - **Chung–Lu:** An extension of the Erdős–Rényi random graph model
+      with edge probabilities dependent on vertex "weights".
+      See `Efficient Generation of Networks with Given Expected Degrees <http://aric.hagberg.org/papers/miller-2011-efficient.pdf>`_.
+    - **https://en.wikipedia.org/wiki/Havel%E2%80%93Hakimi_algorithm
+  :param seed:   The random seed.
+    +
+  '''
+
+def createBarabSiAlbertGraph(size, attachments_per_vertex, connected_at_start, seed):
+  '''  Creates a random graph using the https://en.wikipedia.org/wiki/Barab%C3%A1si%E2%80%93Albert_model[Barabási–Albert model].
+  The vertices are created one by one and connected to a set number of randomly chosen
+  previously created vertices. This ensures a skewed degree distribution with "older" vertices
+  tending to have a higher degree.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1BarabasiAlbertGenerator.html>`_ implementation.
+
+  :param size:   The created graph will have this many vertices.
+  :param attachments_per_vertex:   As each vertex is added, it will be connected to this many existing vertices.
+  :param connected_at_start:   This many vertices will be connected in a circle at the start of the algorithm.
+  :param seed:   The random seed.
+    +
+  '''
+
+def createClusteredRandomGraph(size, clusters, probability_in, probability_out, seed):
+  '''  Creates a random graph with a given number of clusters.
+  It randomly places each vertex into one of the clusters then adds an edge for each
+  vertex pair with the given probabilities.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1ClusteredRandomGraphGenerator.html>`_ implementation.
+
+  :param size:   The created graph will have this many vertices.
+  :param clusters:   The created graph will have this many clusters.
+    Each vertex will be randomly placed into one of the clusters with equal probability.
+  :param probability_in:   The probablity for adding an edge between two vertices if they are in the same cluster.
+  :param probability_out:   The probablity for adding an edge between two vertices if they are in different clusters.
+  :param seed:   The random seed.
+    +
+  '''
+
+def createDorogovtsevMendesRandomGraph(size, seed):
+  '''  Creates a planar random graph with a power-law distribution. Starts with a triangle and in each
+  step adds a new node that is connected to the two endpoints of a randomly selected edge.
+
+  See `Modern architecture of random graphs: Constructions and correlations <https://arxiv.org/abs/cond-mat/0206467>`_ by Dorogovtsev et al.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1DorogovtsevMendesGenerator.html>`_ implementation.
+
+  :param size:   The created graph will have this many vertices.
+  :param seed:   The random seed.
+    +
+  '''
+
 def createEdgesFromCoOccurrence():
   '''  Connects vertices in the base graph if they co-occur in any segments.
   Multiple co-occurrences will result in multiple parallel edges. Loop edges
   are generated for each segment that a vertex belongs to. The attributes of
   the segment are copied to the edges created from it.
 
   This operation has a potential to create trillions of edges or more.
@@ -616,14 +886,27 @@
 
 def createEdgesFromSetOverlaps(minoverlap):
   '''  Connects segments with large enough overlaps.
 
   :param minoverlap:   Two segments will be connected if they have at least this many members in common.
   '''
 
+def createErdSRNyiGraph(size, probability, seed):
+  '''  Creates a random graph using the https://en.wikipedia.org/wiki/Erd%C5%91s%E2%80%93R%C3%A9nyi_model[Erdős–Rényi model].
+  In this model each pair of vertices is connected independently with the same probability.
+  It creates a very uniform graph with no tendency to skewed degree distributions or clustering.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1ErdosRenyiGenerator.html>`_ implementation.
+
+  :param size:   The created graph will have this many vertices.
+  :param probability:   Each pair of vertices is connected with this probability.
+  :param seed:   The random seed.
+    +
+  '''
+
 def createExampleGraph():
   '''  Creates small test graph with 4 people and 4 edges between them.
 
 
   '''
 
 def createGraphInPython(code, outputs):
@@ -639,14 +922,112 @@
 
   :param code:   The Python code you want to run. See the operation description for details.
   :param outputs:   A comma-separated list of attributes that your code generates.
     These must be annotated with the type of the attribute.
     For example, `vs.my*new*attribute: str, vs.another*new*attribute: float, graph_attributes.also_new: str`.
   '''
 
+def createHyperbolicRandomGraph(size, avg_degree, exponent, temperature, seed):
+  '''  Creates a random graph based on randomly placed points on the hyperbolic plane.
+  The points corresponding to vertices are placed on a disk.
+  If two points are closer than a threshold (by the hyperbolic distance metric),
+  an edge will be created between those two vertices.
+
+  The motivation for this is to reflect popularity (how close the point is to the center)
+  and interest (in which direction the point lies). This leads to realistic clustering
+  properties in the generated random graph.
+
+  The radius of the disk and the neighborhood radius can be chosen to ensure a
+  desired average and power-law exponent for the degree distribution.
+
+  Instead of a strict neighborhood radius, within which edges are always created and
+  outside of which they never are, we can also consider probabilistic
+  edge generation. In this case the shorter the distance between two points, the
+  more likely that an edge should be generated.
+
+  The temperature parameter is defined in a way that makes the strict neighborhood
+  radius case an edge case (T
+
+  :param size:   The created graph will have this many vertices.
+  :param avg_degree:   The expected value of the degree distribution.
+  :param exponent:   The exponent of the degree distribution.
+  :param temperature:   When zero, vertices are connected if they lie within a fixed threshold on the hyperbolic disk.
+    Larger values add randomness while trying to preserve the degree distribution.
+  :param seed:   The random seed.
+    +
+  '''
+
+def createLfrRandomGraph(size, avg_degree, max_degree, degree_exponent, min_community, max_community, community_exponent, avg_mixing, seed):
+  '''  LFR stands for Lancichinetti, Fortunato, and Radicchi, the authors of
+  `Benchmark graphs for testing community detection algorithms <https://arxiv.org/abs/0805.4770>`_
+  and `Benchmarks for testing community detection algorithms on directed and weighted graphs with overlapping communities <https://arxiv.org/abs/0904.3940>`_
+  upon which this generator is based.
+
+  The LFR random graph features overlapping communities.
+  Each vertex is randomized into multiple communities while
+  ensuring a desired power-law community size distribution.
+  Then edges within communities are generated to match the
+  desired power-law vertex degree distribution.
+  Finally edges are swapped around to create cross-community
+  connections.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1LFRGenerator.html>`_ implementation.
+
+  :param size:   The created graph will have this many vertices.
+  :param avg_degree:   The expected value of the desired vertex degree distribution.
+  :param max_degree:   The maximum of the desired vertex degree distribution.
+  :param degree_exponent:   The power-law exponent of the desired vertex degree distribution.
+    A higher number means a more skewed distribution.
+  :param min_community:   The minimum of the desired community size distribution.
+  :param max_community:   The maximum of the desired community size distribution.
+  :param community_exponent:   The power-law exponent of the desired community size distribution.
+    A higher number means a more skewed distribution.
+  :param avg_mixing:   What ratio of the neighbors of each vertex should on average be of other communities.
+  :param seed:   The random seed.
+    +
+  '''
+
+def createMocnikRandomGraph(size, dimension, density, seed):
+  '''  Creates a random graph as described in
+  https://www.mocnik-science.net/publications/2015c%20-%20Franz-Benjamin%20Mocnik%20-%20Modelling%20Spatial%20Structures.pdf[Modelling Spatial Structures] by Mocnik et al.
+  The model is based on randomly placing the vertices in Euclidean space
+  and generating edges with a higher probability for pairs of vertices
+  that are closer together.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1MocnikGenerator.html>`_ implementation.
+
+  :param size:   The created graph will have this many vertices.
+  :param dimension:   The vertices are placed randomly in a space with this many dimensions.
+  :param density:   The desired ratio of edges to nodes.
+  :param seed:   The random seed.
+    +
+  '''
+
+def createP2pRandomGraph(size, dense_areas, max_degree, neighborhood_radius, seed):
+  '''  Creates a random graph using the model described in `A distributed diffusive heuristic for clustering a virtual P2P supercomputer <http://parco.iti.kit.edu/henningm/data/distribClust.pdf>`_ by Gehweiler et al.
+
+  The vertices are randomly placed in a 2-dimensional unit square with a torus topology.
+  Vertices within a set radius are connected when permitted by the maximum degree constraint.
+
+  Some dense circular areas within the unit suqare are picked at the beginning
+  and these are populated first. Any remaining vertices are then placed uniformly.
+  This leads to a clustering effect that models the internal networks of companies
+  and institutions as observed in real peer-to-peer network topologies.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1PubWebGenerator.html>`_ implementation.
+
+  :param size:   The created graph will have this many vertices.
+  :param dense_areas:   How many dense areas to pick. These will vary in size and will be populated first.
+  :param max_degree:   Each vertex will be connected to at most this many neighbors.
+  :param neighborhood_radius:   The model works by placing points on the unit square. Points within this radius
+    will be connected to each other.
+  :param seed:   The random seed.
+    +
+  '''
+
 def createRandomEdges(degree, seed):
   '''  Creates edges randomly, so that each vertex will have a degree uniformly chosen between 0 and
   2 * the provided parameter.
 
   For example, you can create a random graph by first applying operation <<Create vertices>>
   and then creating the random edges.
 
@@ -846,14 +1227,91 @@
   :param dimensions:   The size of each embedding vector.
   :param walks_per_node:   Number of random walks collected for each vertex.
   :param walk_length:   Length of the random walks collected for each vertex.
   :param context_size:   The random walks will be cut with a rolling window of this size.
     This allows reusing the same walk for multiple vertices.
   '''
 
+def exportEdgeAttributesToNeo4j(url, username, password, version, labels, keys):
+  '''  Exports edge attributes from a graph in LynxKite to a
+  corresponding graph in `Neo4j <https://neo4j.com/>`_.
+
+  The relationships in Neo4j are identified by a key property (or properties).
+  You must have a corresponding edge attribute in LynxKite by the same name.
+  This will be used to find the right relationship to update in Neo4j.
+
+  The properties of the Neo4j relationships will be updated with the exported edge attributes
+  using a Cypher query like this:
+
+      UNWIND $events as event
+      MATCH ()-[r:TYPE {`key`: event.`key`}]-()
+      SET r +
+
+  :param url:   The Neo4j connection string of the form `bolt://localhost:7687`.
+  :param username:   Username for the connection.
+  :param password:   Password for the connection. It will be saved in the workspace and visible to anyone with
+    access to the workspace.
+  :param version:   LynxKite only re-computes outputs if parameters or inputs have changed.
+    This is true for exports too. If you want to repeat a previous export, you can increase this
+    export repetition ID parameter.
+  :param labels:   Makes it possible to restrict the export to one relationship type in Neo4j.
+    This is useful to make sure no other relationship type is accidentally affected.
+    The format is as in Cypher: `:TYPE`. Leave empty to allow updating any node.
+  :param keys:   Select the attribute (or attributes) to identify the Neo4j relationships by.
+    The attribute name must match the property name in Neo4j.
+  '''
+
+def exportGraphToNeo4j(url, username, password, version, node_labels, relationship_type):
+  '''  Exports a graph from LynxKite to `Neo4j <https://neo4j.com/>`_.
+  The whole graph will be copied to Neo4j with all attributes.
+  No existing data is modified in Neo4j.
+
+  A `!LynxKite export timestamp` property is added to each new
+  node and relationship in Neo4j. This helps clean up the export if needed.
+
+  The Cypher query to export nodes is, depending on whether an attribute specifies the node labels:
+
+      UNWIND $events AS event
+      // Without node labels:
+      CREATE (n)
+      SET n +
+
+  :param url:   The Neo4j connection string of the form `bolt://localhost:7687`.
+  :param username:   Username for the connection.
+  :param password:   Password for the connection. It will be saved in the workspace and visible to anyone with
+    access to the workspace.
+  :param version:   LynxKite only re-computes outputs if parameters or inputs have changed.
+    This is true for exports too. If you want to repeat a previous export, you can increase this
+    export repetition ID parameter.
+  :param node_labels:   A string vertex attribute that is a comma-separated list of labels to apply to the newly
+    created nodes. Optional. You must have `Neo4j APOC <https://neo4j.com/developer/neo4j-apoc/>`_
+    installed on the Neo4j instance to use this.
+  :param relationship_type:   A string edge attribute that specifies the relationship type for each newly created relationship.
+    Optional. You must have `Neo4j APOC <https://neo4j.com/developer/neo4j-apoc/>`_
+    installed on the Neo4j instance to use this.
+  '''
+
+def exportToAvro(path, version, for_download):
+  '''  `Apache AVRO <https://avro.apache.org/>`_ is a row-oriented remote procedure call and data serialization framework.
+
+  :param path:   The distributed file-system path of the output file. It defaults to `<auto>`, in which case the
+    path is auto generated from the parameters and the type of export (e.g. `Export to CSV`).
+    This means that the same export operation with the same parameters always generates the same path.
+  :param version:   Version is the version number of the result of the export operation. It is a non negative integer.
+    LynxKite treats export operations as other operations: it remembers the result (which in this case
+    is the knowledge that the export was successfully done) and won't repeat the calculation. However,
+    there might be a need to export an already exported table with the same set of parameters (e.g. the
+    exported file is lost). In this case you need to change the version number, making that parameters
+    are not the same as in the previous export.
+  :param for_download:   Set this to "true" if the purpose of this export is file download: in this case LynxKite will
+    repartition the data into one single file, which will be downloaded. The default "no" will
+    result in no such repartition: this performs much better when other, partition-aware tools
+    are used to import the exported data.
+  '''
+
 def exportToCsv(path, delimiter, quote, quote_all, header, escape, null_value, date_format, timestamp_format, drop_leading_white_space, drop_trailing_white_space, version, for_download):
   '''  CSV stands for comma-separated values. It is a common human-readable file format where each record
   is on a separate line and fields of the record are simply separated with a comma or other delimiter.
   CSV does not store data types, so all fields become strings when importing from this format.
 
   :param path:   The distributed file-system path of the output file. It defaults to `<auto>`, in which case the
     path is auto generated from the parameters and the type of export (e.g. `Export to CSV`).
@@ -882,14 +1340,32 @@
     are not the same as in the previous export.
   :param for_download:   Set this to "true" if the purpose of this export is file download: in this case LynxKite will
     repartition the data into one single file, which will be downloaded. The default "no" will
     result in no such repartition: this performs much better when other, partition-aware tools
     are used to import the exported data.
   '''
 
+def exportToDelta(path, version, for_download):
+  '''  Export data to a Delta table.
+
+  :param path:   The distributed file-system path of the output file. It defaults to `<auto>`, in which case the
+    path is auto generated from the parameters and the type of export (e.g. `Export to CSV`).
+    This means that the same export operation with the same parameters always generates the same path.
+  :param version:   Version is the version number of the result of the export operation. It is a non negative integer.
+    LynxKite treats export operations as other operations: it remembers the result (which in this case
+    is the knowledge that the export was successfully done) and won't repeat the calculation. However,
+    there might be a need to export an already exported table with the same set of parameters (e.g. the
+    exported file is lost). In this case you need to change the version number, making that parameters
+    are not the same as in the previous export.
+  :param for_download:   Set this to "true" if the purpose of this export is file download: in this case LynxKite will
+    repartition the data into one single file, which will be downloaded. The default "no" will
+    result in no such repartition: this performs much better when other, partition-aware tools
+    are used to import the exported data.
+  '''
+
 def exportToHive(table, mode, partition_by):
   '''  Export a table directly to `Apache Hive <https://hive.apache.org/>`_.
 
   :param table:   The name of the database table to export to.
   :param mode:   Describes whether LynxKite should expect a table to already exist and how to handle this case.
     +
     **The table must not exist** means the table will be created and it is an error if it already
@@ -978,14 +1454,43 @@
     are not the same as in the previous export.
   :param for_download:   Set this to "true" if the purpose of this export is file download: in this case LynxKite will
     repartition the data into one single file, which will be downloaded. The default "no" will
     result in no such repartition: this performs much better when other, partition-aware tools
     are used to import the exported data.
   '''
 
+def exportVertexAttributesToNeo4j(url, username, password, version, labels, keys):
+  '''  Exports vertex attributes from a graph in LynxKite to a
+  corresponding graph in `Neo4j <https://neo4j.com/>`_.
+
+  The nodes in Neo4j are identified by a key property (or properties).
+  You must have a corresponding vertex attribute in LynxKite by the same name.
+  This will be used to find the right nodes to update in Neo4j.
+
+  The properties of the Neo4j nodes will be updated with the exported vertex attributes using
+  a Cypher query like this:
+
+      UNWIND $events as event
+      MATCH (n:Label1:Label2 {`key`: event.`key`})
+      SET n +
+
+  :param url:   The Neo4j connection string of the form `bolt://localhost:7687`.
+  :param username:   Username for the connection.
+  :param password:   Password for the connection. It will be saved in the workspace and visible to anyone with
+    access to the workspace.
+  :param version:   LynxKite only re-computes outputs if parameters or inputs have changed.
+    This is true for exports too. If you want to repeat a previous export, you can increase this
+    export repetition ID parameter.
+  :param labels:   Makes it possible to restrict the export to one label (or combination of labels) in Neo4j.
+    This is useful to make sure no other node type is accidentally affected.
+    The format is as in Cypher: `:Label1:Label2`. Leave empty to allow updating any node.
+  :param keys:   Select the attribute (or attributes) to identify the Neo4j nodes by.
+    The attribute name must match the property name in Neo4j.
+  '''
+
 def exposeInternalEdgeId(name):
   '''  Exposes the internal edge ID as an attribute. Useful if you want to identify edges, for example in
   an exported dataset.
 
   :param name:   The ID attribute will be saved under this name.
   '''
 
@@ -1128,14 +1633,79 @@
     restrict to those vertices/edges where the String attribute is defined and its value is not empty
     string. Remember, all filters work on defined values only, so `!*` will not match any
     vertices/edges.
   :param ref9:   If you need a string filter that contains a character with a special meaning (e.g., `>`), use double quotes around
     the string. E.g., `>"
   '''
 
+def filterWithSql(vertex_filter, edge_filter, filter):
+  '''  Filters a graph or table with SQL expressions.
+
+  This has the same effect as using a SQL box with
+  ``select * from vertices where <FILTER>`` and ``select * from edge_attributes where <FILTER>``
+  and then recombining the tables into a graph. But it is more efficient.
+
+  When used with a table input it is identical to a SQL box with
+  ``select * from input where <FILTER>``. But it saves a bit of typing.
+
+  :param vertex_filter:   Filter the vertices with this SQL expression when the input is a graph.
+    For example you could write ``age > 30 and income < age * 2000``.
+  :param edge_filter:   Filter the edges with this SQL expression when the input is a graph.
+    For example you could write ``duration > count * 10 or kind like '%*message*%'``.
+  :param filter:   Filter with this SQL expression when the input is a table.
+    For example you could write ``age > 30 and income < age * 2000``.
+  '''
+
+def findCommunitiesWithLabelPropagation(name, weight, variant):
+  '''  Uses the `label propagation algorithm <https://en.wikipedia.org/wiki/Label*propagation*algorithm>`_
+  to identify communities in the graph. The communities are represented as a segmentation on
+  the graph.
+
+  Label propagation starts with assigning a unique label to each vertex.
+  Then each vertex takes on the most common label in their neighborhood.
+  This step is repeated until the labels stabilize.
+
+  Uses the NetworKit implementations of
+  `PLP <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1PLP.html>`_ and
+  `LPDegreeOrdered <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1LPDegreeOrdered.html>`_.
+
+  :param name:   The name of the newly created segmentation.
+  :param weight:   The neighboring labels are weighted with the edge weight. A bigger weight
+    results in that neighbor having a bigger influence in the label update step.
+  :param variant:   The results of label propagation depend greatly on the order of the updates.
+    The available options are:
+    - **classic:** An efficient method that uses an arbitrary ordering and parallel updates.
+    - **degree-ordered:** A more predictable method that performs the updates in increasing
+      order of degree.
+  '''
+
+def findCommunitiesWithTheLouvainMethod(name, weight, resolution):
+  '''  Uses the `Louvain method <https://en.wikipedia.org/wiki/Louvain_method>`_ to identify
+  communities in the graph. The communities are represented as a segmentation on
+  the graph.
+
+  The Louvain method is a greedy optimization toward maximal *modularity*.
+  High modularity means many edges within communities and few edges between communities.
+  Specifically we compare the edge counts to what we would expect if the clusters
+  were chosen at random.
+
+  Uses the `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1PLM.html>`_ implementation.
+
+  :param name:   The name of the newly created segmentation.
+  :param weight:   Edges can be weighted to contribute more or less to modularity.
+  :param resolution:   A lower resolution will result in bigger communities.
+    +
+    Also known as the 𝛾 parameter, the expected edge probabilities in the modularity
+    calculation are multiplied by this number.
+    +
+    For details of the physical basis of this parameter see
+    `Statistical Mechanics of Community Detection <https://arxiv.org/abs/cond-mat/0603718>`_
+    by Joerg Reichardt and Stefan Bornholdt.
+  '''
+
 def findConnectedComponents(name, directions):
   '''  Creates a segment for every connected component of the graph.
 
   Connected components are maximal vertex sets where a path exists between each pair of vertices.
 
   :param name:   The new segmentation will be saved under this name.
   :param directions:   Ignore directions:::
@@ -1160,14 +1730,28 @@
     +
     This improves the performance of the algorithm, and small cliques are often not
     a good indicator anyway.
   :param adjacency_threshold:   Clique overlap is a measure of the overlap between two cliques relative to
     their sizes. It is normalized to
   '''
 
+def findKCoreDecomposition(name):
+  '''  If we deleted all parts of a graph outside of the **k**-core, all vertices would
+  still have a degree of at least *k*. More visually, the 0-core is the whole graph.
+  If we discard the isolated vertices we get the 1-core. If we repeatedly discard
+  all degree-1 vertices, we get the 2-core. And so on.
+
+  Read more on `Wikipedia <https://en.wikipedia.org/wiki/Degeneracy_(graph_theory)#k-Cores>`_.
+
+  This operation outputs the number of the highest core that each vertex belongs to
+  as a vertex attribute.
+
+  :param name:   The new attribute will be created under this name.
+  '''
+
 def findMaximalCliques(name, bothdir, min):
   '''  Creates a segmentation of vertices based on the maximal cliques they are the member of.
   A maximal clique is a maximal set of vertices where there is an edge between every two vertex.
   Since one vertex can be part of multiple maximal cliques this segmentation might be overlapping.
 
   :param name:   The new segmentation will be saved under this name.
   :param bothdir:   Whether edges have to exist in both directions between all members of a clique.
@@ -1190,14 +1774,34 @@
   :param name:   The new segmentation will be saved under this name.
   :param weights:   The attribute to use as edge weights.
   :param max_iterations:   After this number of iterations we stop regardless of modularity increment. Use -1 for unlimited.
   :param min_increment_per_iteration:   If the average modularity increment in the last few iterations goes below this then we stop
     the algorithm and settle with the clustering found.
   '''
 
+def findOptimalSpanningTree(name, weight, optimize, seed):
+  '''  Finds the https://en.wikipedia.org/wiki/Minimum*spanning*tree[minimum (or maximum) spanning tree]
+  in a graph. The edges marked by the emitted edge attribute (``in_tree`` by default)
+  form a tree for each component in the graph. This tree will have the lowest
+  (or highest) possible total edge weight.
+
+  Uses the
+  `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1RandomMaximumSpanningForest.html>`_
+  implementation.
+
+  :param name:   The new edge attribute will be created under this name.
+    Its value will be 1 for the edges that make up the tree
+    and undefined for the edges that are not part of the tree.
+  :param weight:   Choose a numerical attribute that represents the cost or value of the edges.
+    With unit weights the result is just a random tree for each component.
+  :param optimize:   Whether to find the tree with the lowest or highest possible total edge weight.
+  :param seed:   When multiple trees have the optimal weight, one is chosen at random.
+    +
+  '''
+
 def findSteinerTree(ename, vname, pname, rname, edge_costs, root_costs, gain):
   '''  Given a directed graph in which each vertex has two associated quantities, the "gain",
   and the "root cost", and each edge has an associated quantity, the "cost",
   this operation will yield a forest (a set of trees) that is a subgraph of the given
   graph. Furthermore, in this subgraph, the sum of the gains
   minus the sum of the (edge and root) costs approximate the maximal possible value.
 
@@ -1359,14 +1963,21 @@
   up in the graph. He can also apply hashing to the phone numbers of all the knights of the round
   table and see which knight has Guinevere been making calls to.
 
   :param attr:   The attribute(s) which will be hashed.
   :param salt:   The value of the salt.
   '''
 
+def importAvro(filename):
+  '''  `Apache AVRO <https://avro.apache.org/>`_ is a row-oriented remote procedure call and data serialization framework.
+
+  :param filename:   The distributed file-system path of the file. See <<prefixed-paths>> for more details on specifying
+    paths.
+  '''
+
 def importCsv(filename, columns, delimiter, quote, escape, null_value, date_format, timestamp_format, ignore_leading_white_space, ignore_trailing_white_space, comment, error_handling, infer):
   '''  CSV stands for comma-separated values. It is a common human-readable file format where each record
   is on a separate line and fields of the record are simply separated with a comma or other delimiter.
   CSV does not store data types, so all fields become strings when importing from this format.
 
   :param filename:   Upload a file by clicking the
     +++<label class
@@ -1395,20 +2006,54 @@
     +
     **Salvage malformed lines: truncate or fill with nulls** will still import the problematic lines,
     dropping some data or inserting undefined values.
   :param infer:   Automatically detects data types in the CSV. For example a column full of numbers will become a
     `Double`. If disabled, all columns are imported as ``String``s.
   '''
 
+def importDelta(filename, version_as_of):
+  '''  Import a Delta Table.
+
+  :param filename:   The distributed file-system path of the file. See <<prefixed-paths>> for more details on specifying
+    paths.
+  :param version_as_of:   Version of the Delta table to be imported. The empty string corresponds to the latest version.
+  '''
+
 def importFromHive(table_name):
   '''  Import an `Apache Hive <https://hive.apache.org/>`_ table directly to LynxKite.
 
   :param table_name:   The name of the Hive table to import.
   '''
 
+def importFromNeo4j(url, username, password, vertex_query, edge_query):
+  '''  Import a graph from the `Neo4j <https://neo4j.com/>`_ graph database.
+
+  Neo4j does not have a strict schema. Different nodes may have different attributes.
+  In LynxKite the list of vertex attributes is defined for the whole graph.
+  But each vertex may leave any attribute undefined.
+
+  If you import Neo4j nodes that have different attributes, such as movies that have
+  a `title` and actors that have a `name`, the resulting graph will have both `title` and
+  `name` attributes. `title` will only be defined on movies, `name` will only be defined
+  on actors.
+
+  The same happens with edges.
+
+  If multiple node types have attributes of the same name, those attributes need to have
+  the same type. If this is not the case, you can narrow down the query by node label.
+
+  :param url:   The connection URI for Neo4j.
+  :param username:   The username to use for the connection.
+  :param password:   The password to use for the connection.
+  :param vertex_query:   The Cypher query to run on Neo4j to get the vertices. This query must return a node named `node`.
+    The default query imports all the nodes from Neo4j. Leave empty to not import vertex attributes.
+  :param edge_query:   The Cypher query to run on Neo4j to get the edges. This query must return a relationship named `rel`.
+    The default query imports all the relationships from Neo4j. Leave empty to not import edges.
+  '''
+
 def importJdbc(jdbc_url, jdbc_table, key_column, num_partitions, partition_predicates):
   '''  JDBC is used to connect to relational databases such as MySQL. See <<jdbc-details>> for setup steps
   required for connecting to a database.
 
   :param jdbc_url:   The connection URL for the database. This typically includes the username and password. The exact
     syntax entirely depends on the database type. Please consult the documentation of the database.
   :param jdbc_table:   The name of the database table to import.
@@ -1451,47 +2096,14 @@
   data types. Each line of the file in this format stores one record encoded as a
   `JSON <https://en.wikipedia.org/wiki/JSON>`_ object.
 
   :param filename:   Upload a file by clicking the
     +++<label class
   '''
 
-def importNeo4j(node_label, relationship_type, num_partitions, infer):
-  '''  Import data from an existing Neo4j database. The connection can be configured through the following
-  variables in the .kiterc file:
-
-  * `NEO4J_URI`: URI to connect to Neo4j, only bolt protocol is supported. The URI has to follow the
-     `bolt://<host>:<port>` structure.
-  * `NEO4J_PASSWORD`: Password to connect to Neo4j. You can leave it empty in case no password is required
-  * `NEO4J_USER`: User used to connect to Neo4j
-
-  In case you want to change the values of the variables, you will have to restart LynxKite for the
-  changes to take effect.
-
-  :param node_label:   The label for the type of node that you want to import from Neo4j. All the nodes with that label will be
-    imported as a table, with each property as a column. You can specify the properties to import using the
-    `Columns to import` parameter. The id ( `id()` function of Neo4j) of the node will be automatically included
-    in the import as the special variable `id$`.
-    Only one of node label or relationship type can be specified.
-  :param relationship_type:   The type of the relationship that you want to import from Neo4j. The relationship will be imported
-    as a table, with each property as a column. You can specify the properties to import using the
-    `Columns to import` parameter.
-    If you want to import properties from the source or the destination (target) nodes you can do it
-    by adding the prefix `source_` or `target_` to the property. The id ( `id()` function of Neo4j) of
-    both the source and the destination nodes, will be automatically included in the import as the special
-    variables `source_id$` and `target_id$`.
-    Only one of node label or relationship type can be specified.
-  :param num_partitions:   LynxKite will perform this many queries in parallel to get the data. Leave at zero to let
-    LynxKite automatically decide. Set a specific value if you want to control the level of
-    parallelism.
-  :param infer:   Automatically tries to cast data types from Neo4j. For example a column full of numbers will become a
-    `number`. If disabled, all columns are imported as ``String``. It is recommended to set this to false,
-    as Neo4j types do not integrate very well with Spark (Eg. Date types from Neo4j are not supported).
-  '''
-
 def importOrc(filename):
   '''  `Apache ORC <https://orc.apache.org/>`_ is a columnar data storage format.
 
   :param filename:   The distributed file-system path of the file. See <<prefixed-paths>> for more details on specifying
     paths.
   '''
 
@@ -1696,14 +2308,50 @@
   Output boxes without a name are ignored. Each output box must have a different name.
 
   See the section on <<custom-boxes>> on how to use this box.
 
   :param name:   The name of the output, when the workspace is used as a custom box.
   '''
 
+def placeVerticesWithEdgeLengths(name, dimensions, length, algorithm, pivots, radius, tolerance):
+  '''  These methods create a graph layout as a new ``Vector[number]`` vertex attribute
+  where the edges have the given lengths, or as close to those as possible.
+
+  Uses the NetworKit implementations for
+  `PivotMDS <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1PivotMDS.html>`_ and
+  `MaxentStress <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1MaxentStress.html>`_.
+
+  :param name:   The position attribute will be saved under this name.
+  :param dimensions:   The dimensions of the space where the vertices are placed.
+    The created ``Vector``s will be this long.
+  :param length:   This edge attribute can specify the length that each edge should be.
+  :param algorithm:   The algorithms offered are:
+    - **Pivot MDS** picks a number of pivot vertices (spread out as much as possible) and
+      finds a solution that puts all other vertices the right distance from the pivots
+      through an iterative matrix eigendecomposition method.
+      +
+      See `Eigensolver Methods for Progressive Multidimensional Scaling of Large Data <https://kops.uni-konstanz.de/bitstream/handle/123456789/5741/bp*empmdsld*06.pdf>`_
+      by Ulrik Brandes and Christian Pich for the detailed definition and analysis.
+    - **Maxent-Stress** is recommended when there are many different ways to
+      satisfy the edge length constraints. (Such as in graphs with low degrees or in
+      high-dimensional spaces.) It picks from the large solution space by
+      maximizing the solution's entropy.
+      +
+      Cannot handle disconnected graphs.
+      +
+      See `A Maxent-Stress Model for Graph Layout <http://yifanhu.net/PUB/maxent.pdf>`_
+      by Gansner et al for the detailed definition and analysis.
+  :param pivots:   The number of pivots to choose for Pivot MDS.
+    More pivots result in a more accurate layout and a longer computation time.
+  :param radius:   Maxent-Stress applies the stress model between vertices within this many
+    hops from each other.
+  :param tolerance:   Maxent-Stress uses an algebraic solver to optimize the vertex positions.
+    This parameter allows tuning the solver to provide faster but less accurate solutions.
+  '''
+
 def predictEdgesWithHyperbolicPositions(size, externaldegree, internaldegree, exponent, radial, angular):
   '''  Creates additional edges in a graph based on
   hyperbolic distances between vertices.
    *2 * size* edges will be added because
   the new edges are undirected.
   Vertices must have two *number* vertex attributes to be
   used as radial and angular coordinates.
@@ -1881,14 +2529,18 @@
   metrics can be found in the following publication,
   https://cs.stanford.edu/people/jure/pubs/sampling-kdd06.pdf.
 
   The output of the operation is a vertex and an edge attribute which describes which was the first
   step that ended at the given vertex / traversed the given edge. The attributes are not defined on
   vertices that were never reached or edges that were never traversed.
 
+  Use the <<Filter by attributes>> box to discard the part of the graph outside of the sample.
+  Applying the `*` filter for `first_reached` will discard the vertices where the attribute is
+  undefined.
+
   If the resulting sample is still too large, it can be quickly reduced by keeping only the low index
   nodes and edges. Obtaining a sample with exactly `n` vertices is also possible with the
   following procedure.
 
   . Run this operation. Let us denote the computed vertex attribute by `first_reached` and edge
   attribute by `first_traversed`.
   . Rank the vertices by `first_reached`.
@@ -1915,14 +2567,53 @@
 def saveToSnapshot(path):
   '''  Saves the input to a snapshot. The location of the snapshot has to be specified as
   a full path.
 
   :param path:   The full path of the target snapshot in the LynxKite directory system.
   '''
 
+def scoreEdgesWithTheForestFireModel(name, spread_prob, burn_ratio, seed):
+  '''  Produces an edge attribute that reflects the importance of each edge in
+  the spread of information or other communicable effects across the network.
+
+  A simple summary of the algorithm would be:
+
+  1. Pick a random vertex. The fire starts here.
+  2. With probability *p* jump to step 4.
+  3. Set a neighbor on fire and mark the edge as burnt. Jump to step 2.
+  4. This vertex has burnt out. Pick another vertex that is on fire and jump to step 2.
+
+  These steps are repeated until the total number of edges burnt reaches the
+  desired multiple of the total edge count.
+  The score for each edge is proportional to the number of simulations
+  in which it was burnt. It is normalized to have a maximum of 1.
+
+  The forest fire model was introduced in
+  http://www.cs.cmu.edu/~jure/pubs/powergrowth-tkdd.pdf[Graph Evolution: Densification and Shrinking Diameters]
+  by Leskovec et al.
+
+  Uses the
+  `NetworKit <https://networkit.github.io/dev-docs/cpp_api/classNetworKit*1*1ForestFireScore.html>`_
+  implementation.
+
+  :param name:   The new graph attribute will be created under this name.
+  :param spread_prob:   The probability that a vertex on fire will light another neighbor on fire.
+    This would be _1 − p_ in the simple summary in the operation's description.
+  :param burn_ratio:   The simulations are repeated until the total number of edges burnt
+    reaches the total number of edges in the graph multiplied by this factor.
+    +
+    Increase to make sure all edges receive a non-zero score.
+    This will also increase the run time.
+  :param seed:   The seed used for picking where the fires start, which way they spread,
+    and when they stop spreading.
+    +
+    Due to parallelization the algorithm may give different results even with the same seed.
+    +
+  '''
+
 def segmentByDoubleAttribute(name, attr, interval_size, overlap):
   '''  Segments the vertices by a `number` vertex attribute.
 
   The domain of the attribute is split into intervals of the given size and every vertex that
   belongs to a given interval will belong to one segment. Empty segments are not created.
 
   :param name:   The new segmentation will be saved under this name.
@@ -2574,15 +3265,15 @@
   It is possible to import the graph itself as segmentation. But even in this
   special case, there will be no connections between the segments and the base vertices.
   Another operation, <<Use base graph as segmentation>> can be used if edges are desired.
 
 
   '''
 
-def useTableAsEdgeAttributes(id_attr, id_column, prefix, unique_keys):
+def useTableAsEdgeAttributes(id_attr, id_column, prefix, unique_keys, if_exists):
   '''  Imports edge attributes for existing edges from a table. This is
   useful when you already have edges and just want to import one or more attributes.
 
   There are two different use cases for this operation:
   - Import using unique edge attribute values. For example if the edges represent relationships
   between people (identified by `src` and `dst` IDs) we can import the number of total calls between
   each two people. In this case the operation fails for duplicate attribute values - i.e.
@@ -2594,14 +3285,26 @@
   :param id_attr:   The edge attribute which is used to join with the table's ID column.
   :param id_column:   The ID column name in the table. This should be a String column that uses the values
     of the chosen edge attribute as IDs.
   :param prefix:   Prepend this prefix string to the new edge attribute names. This can be used to avoid
     accidentally overwriting existing attributes.
   :param unique_keys:   Assert that the edge attribute values have to be unique if set true. The values of the
     matching ID column in the table have to be unique in both cases.
+  :param if_exists:   If the attribute from the table clashes with an existing attribute of the graph,
+    you can select how to handle this:
+    - **Merge, prefer the table's version**: Where the table defines new values, those will be used.
+      Elsewhere the existing values are kept.
+    - **Merge, prefer the graph's version**: Where the edge attribute is already defined, it is left
+      unchanged. Elsewhere the value from the table is used.
+    - **Merge, report error on conflict**: An assertion is made to ensure that the values in the table
+      are identical to the values in the graph on edges where both are defined.
+    - **Keep the graph's version**: The data in the table is ignored.
+    - **Use the table's version**: The attribute is deleted from the graph and replaced with
+      the attribute imported from the table.
+    - **Disallow this**: A name conflict is treated as an error.
   '''
 
 def useTableAsEdges(attr, src, dst):
   '''  Imports edges from a table. Your vertices must have an identifying attribute, by which
   the edges can be attached to them.
 
   :param attr:   The IDs that are used in the file when defining the edges.
@@ -2645,15 +3348,15 @@
 
   :param name:   The imported segmentation will be created under this name.
   :param base_id_attr:   The `String` vertex attribute that identifies the base vertices.
   :param base_id_column:   The table column that identifies vertices.
   :param seg_id_column:   The table column that identifies segments.
   '''
 
-def useTableAsVertexAttributes(id_attr, id_column, prefix, unique_keys):
+def useTableAsVertexAttributes(id_attr, id_column, prefix, unique_keys, if_exists):
   '''  Imports vertex attributes for existing vertices from a table. This is
   useful when you already have vertices and just want to import one or more attributes.
 
   There are two different use cases for this operation:
   - Import using unique vertex attribute values. For example if the vertices represent people
   this attribute can be a personal ID. In this case the operation fails in case of duplicate
   attribute values (either among vertices or in the table).
@@ -2664,14 +3367,26 @@
   :param id_attr:   The String vertex attribute which is used to join with the table's ID column.
   :param id_column:   The ID column name in the table. This should be a String column that uses the values
     of the chosen vertex attribute as IDs.
   :param prefix:   Prepend this prefix string to the new vertex attribute names. This can be used to avoid
     accidentally overwriting existing attributes.
   :param unique_keys:   Assert that the vertex attribute values have to be unique if set true. The values of the
     matching ID column in the table have to be unique in both cases.
+  :param if_exists:   If the attribute from the table clashes with an existing attribute of the graph,
+    you can select how to handle this:
+    - **Merge, prefer the table's version**: Where the table defines new values, those will be used.
+      Elsewhere the existing values are kept.
+    - **Merge, prefer the graph's version**: Where the vertex attribute is already defined, it is left
+      unchanged. Elsewhere the value from the table is used.
+    - **Merge, report error on conflict**: An assertion is made to ensure that the values in the table
+      are identical to the values in the graph on vertices where both are defined.
+    - **Keep the graph's version**: The data in the table is ignored.
+    - **Use the table's version**: The attribute is deleted from the graph and replaced with
+      the attribute imported from the table.
+    - **Disallow this**: A name conflict is treated as an error.
   '''
 
 def useTableAsVertices():
   '''  Imports vertices (no edges) from a table.
   Each column in the table will be accessible as a vertex attribute.
```

### Comparing `lynxkite-client-4.1.0/src/lynxkite_client.egg-info/PKG-INFO` & `lynxkite_client-5.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: lynxkite-client
-Version: 4.1.0
+Version: 5.3.0
 Summary: Python API for LynxKite
-Home-page: https://lynxkite.com/
-Author: Lynx Analytics
-Author-email: lynxkite@lynxkite.com
-License: UNKNOWN
-Description: # LynxKite Python API
-        
-        This is the official Python client API for [LynxKite](https://lynxkite.com/) from Lynx Analytics.
-        See the LynxKite documentation for usage instructions.
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Project-URL: Homepage, https://lynxkite.com/
+Project-URL: Repository, https://github.com/lynxkite/lynxkite
+Author-email: Lynx Analytics <lynxkite@lynxkite.com>
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
+Requires-Dist: pandas
+Requires-Dist: requests
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+
+# LynxKite Python API
+
+This is the official Python client API for [LynxKite](https://lynxkite.com/) from Lynx Analytics.
+See the LynxKite documentation for usage instructions.
```

