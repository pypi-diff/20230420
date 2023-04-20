# Comparing `tmp/wicked_expressions-0.4.4.tar.gz` & `tmp/wicked_expressions-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wicked_expressions-0.4.4.tar", max compression
+gzip compressed data, was "wicked_expressions-0.5.0.tar", max compression
```

## Comparing `wicked_expressions-0.4.4.tar` & `wicked_expressions-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1061 2023-03-25 16:48:45.139931 wicked_expressions-0.4.4/LICENSE
--rw-r--r--   0        0        0     2119 2023-03-25 16:48:45.139931 wicked_expressions-0.4.4/README.md
--rw-r--r--   0        0        0     1219 2023-03-25 16:49:48.651670 wicked_expressions-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      321 2023-03-25 16:49:48.635670 wicked_expressions-0.4.4/wicked_expressions/__init__.py
--rw-r--r--   0        0        0      776 2023-03-25 16:48:45.147931 wicked_expressions-0.4.4/wicked_expressions/modules/api.bolt
--rw-r--r--   0        0        0     7953 2023-03-25 16:48:45.147931 wicked_expressions-0.4.4/wicked_expressions/modules/comparison.bolt
--rw-r--r--   0        0        0     8213 2023-03-25 16:48:45.147931 wicked_expressions-0.4.4/wicked_expressions/modules/datastash.bolt
--rw-r--r--   0        0        0     2131 2023-03-25 16:48:45.147931 wicked_expressions-0.4.4/wicked_expressions/modules/internal_api.bolt
--rw-r--r--   0        0        0     8500 2023-03-25 16:48:45.147931 wicked_expressions-0.4.4/wicked_expressions/modules/low_level.bolt
--rw-r--r--   0        0        0      341 2023-03-25 16:48:45.147931 wicked_expressions-0.4.4/wicked_expressions/modules/nbtlib_tag.bolt
--rw-r--r--   0        0        0     2981 2023-03-25 16:48:45.147931 wicked_expressions-0.4.4/wicked_expressions/modules/sources.bolt
--rw-r--r--   0        0        0      705 2023-03-25 16:48:45.147931 wicked_expressions-0.4.4/wicked_expressions/modules/utils.bolt
--rw-r--r--   0        0        0     1260 2023-03-25 16:48:45.147931 wicked_expressions-0.4.4/wicked_expressions/modules/var.bolt
--rw-r--r--   0        0        0     5957 2023-03-25 16:48:45.147931 wicked_expressions-0.4.4/wicked_expressions/modules/var_sources.bolt
--rw-r--r--   0        0        0        0 2023-03-25 16:48:45.147931 wicked_expressions-0.4.4/wicked_expressions/py.typed
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-20 10:31:37.876722 wicked_expressions-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2119 2023-04-20 10:31:37.876722 wicked_expressions-0.5.0/README.md
+-rw-r--r--   0        0        0     1219 2023-04-20 10:33:04.640740 wicked_expressions-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-04-20 10:33:04.620740 wicked_expressions-0.5.0/wicked_expressions/__init__.py
+-rw-r--r--   0        0        0      783 2023-04-20 10:31:37.884722 wicked_expressions-0.5.0/wicked_expressions/modules/api.bolt
+-rw-r--r--   0        0        0     7975 2023-04-20 10:31:37.884722 wicked_expressions-0.5.0/wicked_expressions/modules/comparison.bolt
+-rw-r--r--   0        0        0      304 2023-04-20 10:31:37.884722 wicked_expressions-0.5.0/wicked_expressions/modules/config.bolt
+-rw-r--r--   0        0        0     8309 2023-04-20 10:31:37.884722 wicked_expressions-0.5.0/wicked_expressions/modules/datastash.bolt
+-rw-r--r--   0        0        0     1875 2023-04-20 10:31:37.884722 wicked_expressions-0.5.0/wicked_expressions/modules/internal_api.bolt
+-rw-r--r--   0        0        0      341 2023-04-20 10:31:37.884722 wicked_expressions-0.5.0/wicked_expressions/modules/nbtlib.bolt
+-rw-r--r--   0        0        0     8524 2023-04-20 10:31:37.884722 wicked_expressions-0.5.0/wicked_expressions/modules/raw_operations.bolt
+-rw-r--r--   0        0        0     3127 2023-04-20 10:31:37.884722 wicked_expressions-0.5.0/wicked_expressions/modules/sources.bolt
+-rw-r--r--   0        0        0     1181 2023-04-20 10:31:37.884722 wicked_expressions-0.5.0/wicked_expressions/modules/utils.bolt
+-rw-r--r--   0        0        0     1220 2023-04-20 10:31:37.884722 wicked_expressions-0.5.0/wicked_expressions/modules/var.bolt
+-rw-r--r--   0        0        0     5701 2023-04-20 10:31:37.884722 wicked_expressions-0.5.0/wicked_expressions/modules/var_sources.bolt
+-rw-r--r--   0        0        0        0 2023-04-20 10:31:37.884722 wicked_expressions-0.5.0/wicked_expressions/py.typed
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.5.0/PKG-INFO
```

### Comparing `wicked_expressions-0.4.4/LICENSE` & `wicked_expressions-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.4.4/README.md` & `wicked_expressions-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.4.4/pyproject.toml` & `wicked_expressions-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wicked_expressions"
-version = "0.4.4"
+version = "0.5.0"
 description = "Extension of bolt-expressions written in Bolt."
 authors = ["Yeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/wicked-expressions"
 readme = "README.md"
```

### Comparing `wicked_expressions-0.4.4/wicked_expressions/modules/api.bolt` & `wicked_expressions-0.5.0/wicked_expressions/modules/api.bolt`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from bolt_expressions.node import ExpressionNode
 from bolt_expressions import Expression
 
-import ./internal_api as internal_api
 from ./sources import ScoreSource, DataSource
 from ./comparison import ExpressionComparison
-from ./low_level import StoreRaw, GetRaw
+from ./raw_operations import StoreExpressionValue, GetExpressionValue
 from ./var import Var, StaticVar
-from ./nbtlib_tag import Bool, Byte, Short, Int, Long, Float, Double, String, List
+from ./nbtlib import Bool, Byte, Short, Int, Long, Float, Double, String, List
 from ./datastash import DataStash
 
+import ./internal_api as internal_api
+
 
 Scoreboard = ctx.inject(internal_api.Scoreboard)
 Data = ctx.inject(internal_api.Data)
 
-is_expression = internal_api.is_expression
 this = Data.entity('@s')
 
 
 ExpressionComparison.monkeypatch(Scoreboard, Data, ScoreSource, DataSource)
-StoreRaw.monkeypatch(ScoreSource, DataSource)
-GetRaw.monkeypatch(ScoreSource, DataSource)
+StoreExpressionValue.monkeypatch(ScoreSource, DataSource)
+GetExpressionValue.monkeypatch(ScoreSource, DataSource)
 DataStash.monkeypatch(Scoreboard, Data)
```

### Comparing `wicked_expressions-0.4.4/wicked_expressions/modules/comparison.bolt` & `wicked_expressions-0.5.0/wicked_expressions/modules/comparison.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from contextlib import contextmanager
+
 from ./utils import Rebindable, parse_holder
+from ./config import Config
 
 
 class ExpressionComparison(Rebindable):
     _INVERTED_OPERATOR = {
         '==': '!=',
         '!=': '==',
         '<': '>=',
@@ -19,16 +21,16 @@
         self.initialized = initialized
         self.check_exists = check_exists
 
     @classmethod
     def monkeypatch(cls, Scoreboard, Data, ScoreSource, DataSource):
         cls.ScoreSource = ScoreSource
         cls.DataSource = DataSource
-        cls.temp_scoreboard = Scoreboard('wicked_expressions')
-        cls.temp_storage = Data.storage('wicked_expressions:private')
+        cls.temp_scoreboard = Scoreboard(Config.SCOREBOARD_ROOT)
+        cls.temp_storage = Data.storage(Config.STORAGE_ROOT)
 
     @contextmanager
     def __branch__(self):
         score_count = 0
         
         if isinstance(self.arg_0, self.ScoreSource):
             score_count += 1
```

### Comparing `wicked_expressions-0.4.4/wicked_expressions/modules/datastash.bolt` & `wicked_expressions-0.5.0/wicked_expressions/modules/datastash.bolt`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from contextlib import contextmanager
 import nbtlib
 import json
 
 from ./utils import Rebindable
+from ./config import Config
 
 
 class DataStash(Rebindable):
-    _MARKER_PLAYER_TAG = 'wicked_expressions.datastash.stash.player'
-    _MARKER_MOB_TAG = 'wicked_expressions.datastash.stash.mob'
-    _REGISTERED_TAG = 'wicked_expressions.datastash.registered'
-    _LOCAL_PATH = generate_path('wicked_expressions/datastash')
-    _GLOBAL_PATH = 'wicked_expressions:datastash'
-    _CACHE_INDEX = -1
+    _MARKER_PLAYER_TAG = f"{Config.TAG_ROOT}.datastash.stash.player"
+    _MARKER_MOB_TAG = f"{Config.TAG_ROOT}.datastash.stash.mob"
+    _REGISTERED_TAG = f"{Config.TAG_ROOT}.datastash.registered"
+    _GLOBAL_PATH = f"{Config.ROOT}/datastash"
+    _cache_index = -1
     _initialized = False
 
     def __init__(self, nbt_path: str):
         self.nbt_path = nbtlib.Path(nbt_path)
 
         if not DataStash._initialized:
             DataStash._initialized = True
+            self._init_scoreboard()
             self._garbage_collector()
             self._generate_unregister_mcfunc()
             # self._portal_fix()
 
     def __str__(self):
         return f"DataStash {self.nbt_path}"
 
     def get(self, index=None):
-        temp_data = self._Data.storage('wicked_expressions:private').datastash.temp
+        temp_data = self._Data.storage(Config.STORAGE_ROOT).datastash.temp
         with self._use_stash_selector():
             if index is None:
                 temp_data = self._this[self.nbt_path]
             else:
                 temp_data = self._this[self.nbt_path][index]
         return temp_data
 
@@ -63,15 +64,15 @@
             if index is None:
                 self._this[self.nbt_path].remove()
             else:
                 self._this[self.nbt_path][index].remove()
 
     @contextmanager
     def _use_stash_selector(self):
-        cache_path = f"{self._LOCAL_PATH}/cache/{self._get_next_cache_index()}"
+        cache_path = f"{Config.ROOT_LOCAL}/datastash/cache/{self._get_next_cache_index()}"
 
         self._check_register_status()
 
         function f"{cache_path}_payload":
             yield True
 
         if entity @s[type=marker]:
@@ -86,16 +87,16 @@
                                 function cache_path
                 if entity @s[type=!player]:
                     on passengers if entity @s[type=marker,tag=self._MARKER_MOB_TAG]:
                         function cache_path
 
     @classmethod
     def _get_next_cache_index(cls):
-        cls._CACHE_INDEX += 1
-        return cls._CACHE_INDEX
+        cls._cache_index += 1
+        return cls._cache_index
 
     @classmethod
     def _check_register_status(cls):
         if entity @s[type=!marker, tag=!cls._REGISTERED_TAG]:         # "@s markers" use their builtin data nbt, can skip registration
             execute function f"{cls._GLOBAL_PATH}/register":
                 if entity @s[type=player]:
                     cls._register_player()
@@ -187,9 +188,13 @@
 
     #                 # tp @s @e[type=armor_stand,tag=portal_guide_tag,limit=1]
     #                 # kill @e[type=armor_stand,tag=portal_guide_tag]       
 
     @classmethod
     def monkeypatch(cls, Scoreboard, Data):
         cls._this = Data.entity('@s')
+        cls._Scoreboard = Scoreboard
         cls._Data = Data
-        cls._datastash_scb = Scoreboard('wicked_expressions.datastash')
+
+    @classmethod
+    def _init_scoreboard(cls):
+        cls._datastash_scb = cls._Scoreboard(f"{Config.SCOREBOARD_ROOT}.datastash")
```

### Comparing `wicked_expressions-0.4.4/wicked_expressions/modules/internal_api.bolt` & `wicked_expressions-0.5.0/wicked_expressions/modules/internal_api.bolt`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 from typing import Any
-
 import bolt_expressions.node as be_node
 import bolt_expressions.api as be_api
 
+from ./config import Config
 import ./sources as sources
 
 
 class Scoreboard(be_api.Scoreboard):
-    OBJECTIVE_DISPLAY_COLOR = 'aqua'
-
     def objective(self, name: str, criteria: str = 'dummy', prefixed=True, display_name=None):
-        """Get a Score instance through the Scoreboard API"""
-
         if prefixed:
             name = self._expr.opts.objective_prefix + name
 
         if criteria == None:
             criteria = 'dummy'
-        
+
         if name not in self.added_objectives:
             self.added_objectives.add(name)
             self.create_objective(name, criteria, display_name)
-        
+
         return Score(self, name)
 
     def create_objective(self, objective_id: str, criteria: str, display_name: str | dict):
-        mcfunc_path = generate_path('wicked_expressions/scoreboard/setup')
+        setup_path = f"{Config.ROOT_LOCAL}/scoreboard_setup"
 
         if display_name == None:
             display_name = objective_id
 
         if isinstance(display_name, str):
-            display_name = {"text": display_name, "color": self.OBJECTIVE_DISPLAY_COLOR}
-        
-        merge function_tag minecraft:load {"values": [mcfunc_path]}
-        append function mcfunc_path:
+            display_name = display_name
+
+        merge function_tag minecraft:load {"values": [setup_path]}
+        append function setup_path:
             scoreboard objectives add objective_id criteria display_name
 
 class Score(be_api.Score):
     def __getitem__(self, scoreholder: str | list[str]) -> sources.ScoreSource | list[sources.ScoreSource]:
         if isinstance(scoreholder, str):
             return sources.ScoreSource.create(scoreholder, self.objective)
 
@@ -52,10 +48,7 @@
         return sources.DataSource.create("storage", resource_location)
 
     def entity(self, entity: str):
         return sources.DataSource.create("entity", entity)
 
     def block(self, position: str):
         return sources.DataSource.create("block", position)
-
-def is_expression(value: Any) -> bool:
-    return isinstance(value, be_node.ExpressionNode)
```

### Comparing `wicked_expressions-0.4.4/wicked_expressions/modules/low_level.bolt` & `wicked_expressions-0.5.0/wicked_expressions/modules/raw_operations.bolt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from contextlib import contextmanager
 from ./utils import Rebindable, parse_holder
 
 
-class StoreRaw(Rebindable):
+class StoreExpressionValue(Rebindable):
     @contextmanager
     def __call__(self, expression, mode='result', type='int', scale=1):
         if isinstance(expression, self.ScoreSource):
             holder = parse_holder(expression.holder)
 
             if mode == 'result':
                 store result score holder expression.obj:
@@ -137,15 +137,15 @@
                             yield True
 
     @classmethod
     def monkeypatch(cls, ScoreSource, DataSource):
         cls.ScoreSource = ScoreSource
         cls.DataSource = DataSource
 
-class GetRaw(Rebindable):
+class GetExpressionValue(Rebindable):
     def __call__(self, expression, scale=1):
         if isinstance(expression, self.ScoreSource):
             holder = parse_holder(expression.holder)
             scoreboard players get holder expression.obj
         elif isinstance(expression, self.DataSource):
             if expression._type == 'storage':
                 if scale is None:
```

### Comparing `wicked_expressions-0.4.4/wicked_expressions/modules/sources.bolt` & `wicked_expressions-0.5.0/wicked_expressions/modules/sources.bolt`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from contextlib import contextmanager
 import bolt_expressions.sources as sources
 import inspect
 import re
 
-from ./low_level import StoreRaw, GetRaw
+from ./raw_operations import StoreExpressionValue, GetExpressionValue
 from ./comparison import ExpressionComparison
 
-store_raw = StoreRaw()
-get_raw = GetRaw()
+
+store_expression_value = StoreExpressionValue()
+get_expression_value = GetExpressionValue()
 
 
 class ScoreSource(sources.ScoreSource):
     def __eq__(self, other):
         if is_comparison_case():
             return ExpressionComparison(self, '==', other)
         return super().__eq__(other)
@@ -42,19 +43,19 @@
         return ExpressionComparison(self, '!=', None)
 
     def exists(self):
         return ExpressionComparison(self, '==', None, check_exists=True)
 
     @contextmanager
     def store(self, mode='result', type='int', scale=1):
-        with store_raw(self, mode, type, scale):
+        with store_expression_value(self, mode, type, scale):
             yield True
 
     def get(self, scale=None):
-        get_raw(self, scale)
+        return get_expression_value(self, scale)
 
 class DataSource(sources.DataSource):
     def __eq__(self, other):
         if is_comparison_case():
             return ExpressionComparison(self, '==', other)
         return super().__eq__(other)
 
@@ -84,23 +85,22 @@
         return ExpressionComparison(self, '!=', None)
 
     def exists(self):
         return ExpressionComparison(self, '==', None, check_exists=True)
 
     @contextmanager
     def store(self, mode='result', type='int', scale=1):
-        with store_raw(self, mode, type, scale):
+        with store_expression_value(self, mode, type, scale):
             yield True
 
     def get(self, scale=None):
-        get_raw(self, scale)
-
+        return get_expression_value(self, scale)
 
 def is_comparison_case() -> bool:
-    """Determines whether a comparison dunder method call was intended to compare"""
+    """Determines whether a comparison dunder method call was intended to compare."""
 
     frame = inspect.getouterframes(inspect.currentframe(), 2)[2]
     output = re.compile(r"sources.|optimizer.").search(frame.filename) == None
     # print([' ', '+'][output], frame.filename)
     return output
```

### Comparing `wicked_expressions-0.4.4/wicked_expressions/modules/var.bolt` & `wicked_expressions-0.5.0/wicked_expressions/modules/var.bolt`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,9 @@
 import ./var_sources as sources
-from ./nbtlib_tag import
-    Bool,
-    Byte,
-    Short,
-    Int,
-    Long,
-    Float,
-    Double,
-    String,
-    List
+from ./nbtlib import Bool, Byte, Short, Int, Long, Float, Double, String, List
 
 
 class Var:
     is_static = False
 
     def __new__(self, type_annotation):
         if type_annotation == Bool:
```

### Comparing `wicked_expressions-0.4.4/wicked_expressions/modules/var_sources.bolt` & `wicked_expressions-0.5.0/wicked_expressions/modules/var_sources.bolt`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 from bolt_expressions.node import ExpressionNode
 import base64
 import inspect
 import nbtlib
 
 from ./sources import ScoreSource, DataSource
 from ./utils import logger, defer
-
-
-STORAGE_TARGET = 'wicked_expressions:private'
-OBJECTIVE = 'wicked_expressions'
+from ./config import Config
 
 
 class BaseVar:
-    _scoreboard_location = 'wicked_expressions'
-    _storage_location = 'wicked_expressions:private'
-    _VAR_TYPE = ''
+    _var_type = ''
     _location_index = -1
     _static_cache = {}
 
     @classmethod
     def _evaluate_location_index(cls, is_static: bool) -> int:
         if not is_static:
             cls._location_index += 1
@@ -34,157 +29,153 @@
             cls._static_cache[cache_key] = cls._location_index
             return cls._location_index
 
         return retrieved_index
 
     @classmethod
     def _monkeypatch(cls, Scoreboard, Data):
-        cls._main_scoreboard = Scoreboard(cls._scoreboard_location)
-        cls._main_storage = Data.storage(cls._storage_location)
+        cls._main_scoreboard = Scoreboard(Config.SCOREBOARD_ROOT)
+        cls._main_storage = Data.storage(Config.STORAGE_ROOT)
 
     @staticmethod
     def _get_frame_context() -> tuple:
         frame = inspect.getouterframes(inspect.currentframe(), 2)[4]
         path = frame.filename[len(str(ctx.directory)):]
         return (frame.lineno, path)
 
+    @defer
+    @staticmethod
+    def flush_variables_setup():
+        BoolSource._flush_on_load()
+        ByteSource._flush_on_load()
+        ShortSource._flush_on_load()
+        IntSource._flush_on_load()
+        LongSource._flush_on_load()
+        FloatSource._flush_on_load()
+        DoubleSource._flush_on_load()
+        StringSource._flush_on_load()
+        ListSource._flush_on_load()
+
 
 class VarScoreSource(ScoreSource, BaseVar):
     @classmethod
     def create(cls, is_static: bool):
         location_index = cls._evaluate_location_index(is_static)
-        return cls(f"${ctx.project_id}#{cls._VAR_TYPE}${location_index}", OBJECTIVE)
+        return cls(f"${ctx.project_id}#{cls._var_type}${location_index}", Config.SCOREBOARD_ROOT)
 
     @classmethod
     def _flush_on_load(cls):
-        mcfunc_path = generate_path('wicked_expressions/flush_variables')
+        mcfunc_path = f"{Config.ROOT_LOCAL}/runtime_var_flush_score"
 
         for index in range(cls._location_index+1):
             merge function_tag minecraft:load {"values": [mcfunc_path]}
             append function mcfunc_path:
-                scoreboard players reset f"${ctx.project_id}#{cls._VAR_TYPE}${index}" OBJECTIVE
+                scoreboard players reset f"${ctx.project_id}#{cls._var_type}${index}" Config.SCOREBOARD_ROOT
 
 class VarStorageSource(DataSource, BaseVar):
     @classmethod
     def create(cls, is_static: bool):
         location_index = cls._evaluate_location_index(is_static)
-        return cls('storage', STORAGE_TARGET)[ctx.project_id]['data'][cls._VAR_TYPE][location_index]
+        return cls('storage', Config.STORAGE_ROOT)[ctx.project_id]['data'][cls._var_type][location_index]
 
     @classmethod
     def _flush_on_load(cls):
-        mcfunc_path = generate_path('wicked_expressions/flush_variables')
+        mcfunc_path = f"{Config.ROOT_LOCAL}/runtime_var_flush_storage"
 
         if cls._location_index < 0:
             return 0
 
         fresh_slots = []
         for n in range(cls._location_index+1):
-            fresh_slots.append(cls._DEFAULT_SLOT_VALUE)
+            fresh_slots.append(cls._default_slot_value)
 
+        merge function_tag minecraft:load {"values": [mcfunc_path]}
         append function mcfunc_path:
-            nbt_path = f"{ctx.project_id}.data.{cls._VAR_TYPE}"
-            data modify storage STORAGE_TARGET nbt_path set value fresh_slots
+            nbt_path = f"{ctx.project_id}.data.{cls._var_type}"
+            data modify storage Config.STORAGE_ROOT nbt_path set value fresh_slots
 
 class BoolSource(VarScoreSource):
-    _VAR_TYPE = 'bool'
+    _var_type = 'bool'
 
     def _rebind(self, score, value):
         if not isinstance(value, ExpressionNode):
             value = int(value)
             
             if value not in (0, 1):
                 return logger.error(f"Invalid assignment attempt of value {value} to a Bool variable.")
 
         return super()._rebind(score, value)
 
 class ByteSource(VarStorageSource):
     _default_nbt_type = 'byte'
-    _DEFAULT_SLOT_VALUE = nbtlib.Byte(0)
-    _VAR_TYPE = 'byte'
+    _default_slot_value = nbtlib.Byte(0)
+    _var_type = 'byte'
 
     def _rebind(self, source, value):
         if not isinstance(value, ExpressionNode):
             value = nbtlib.Byte(value)
         return super()._rebind(source, value)
 
 class ShortSource(VarStorageSource):
     _default_nbt_type = 'short'
-    _DEFAULT_SLOT_VALUE = nbtlib.Short(0)
-    _VAR_TYPE = 'short'
+    _default_slot_value = nbtlib.Short(0)
+    _var_type = 'short'
 
     def _rebind(self, source, value):
         if not isinstance(value, ExpressionNode):
             value = nbtlib.Short(value)
         return super()._rebind(source, value)
 
 class IntSource(VarScoreSource):
-    _VAR_TYPE = 'int'
+    _var_type = 'int'
 
 class LongSource(VarStorageSource):
     _default_nbt_type = 'long'
-    _DEFAULT_SLOT_VALUE = nbtlib.Long(0)
-    _VAR_TYPE = 'long'
+    _default_slot_value = nbtlib.Long(0)
+    _var_type = 'long'
 
     def _rebind(self, source, value):
         if not isinstance(value, ExpressionNode):
             value = nbtlib.Long(value)
         return super()._rebind(source, value)
 
 # float <-> double
 # 0.000000953674316
 # 1048576
 
 class FloatSource(VarStorageSource):
     _default_nbt_type = 'float'
-    _DEFAULT_SLOT_VALUE = nbtlib.Float(0)
-    _VAR_TYPE = 'float'
+    _default_slot_value = nbtlib.Float(0)
+    _var_type = 'float'
 
     def _rebind(self, source, value):
         if not isinstance(value, ExpressionNode):
             value = nbtlib.Float(value)
         return super()._rebind(source, value)
 
 class DoubleSource(VarStorageSource):
     _default_nbt_type = 'double'
-    _DEFAULT_SLOT_VALUE = nbtlib.Double(0)
-    _VAR_TYPE = 'double'
+    _default_slot_value = nbtlib.Double(0)
+    _var_type = 'double'
 
     def _rebind(self, source, value):
         if not isinstance(value, ExpressionNode):
             value = nbtlib.Double(value)
         return super()._rebind(source, value)
 
 class StringSource(VarStorageSource):
     _default_nbt_type = 'string'
-    _DEFAULT_SLOT_VALUE = nbtlib.String('')
-    _VAR_TYPE = 'string'
+    _default_slot_value = nbtlib.String('')
+    _var_type = 'string'
 
     def _rebind(self, source, value):
         if not isinstance(value, ExpressionNode):
             value = nbtlib.String(value)
         return super()._rebind(source, value)
 
 class ListSource(VarStorageSource):
     _default_nbt_type = 'list'
-    _VAR_TYPE = 'list'
-    _DEFAULT_SLOT_VALUE = []
-
-@defer
-def setup():
-    # patchy fix, ensures `create_objectives` will run before flushing
-    mcfunc_path = generate_path('wicked_expressions/scoreboard/setup')
-    merge function_tag minecraft:load {"values": [mcfunc_path]}
-    function mcfunc_path:
-        help    # placeholder contents
-
-    BoolSource._flush_on_load()
-    ByteSource._flush_on_load()
-    ShortSource._flush_on_load()
-    IntSource._flush_on_load()
-    LongSource._flush_on_load()
-    FloatSource._flush_on_load()
-    DoubleSource._flush_on_load()
-    StringSource._flush_on_load()
-    ListSource._flush_on_load()
+    _var_type = 'list'
+    _default_slot_value = []
 
 def base64_encode(s: str) -> str:
     return base64.b64encode(s.encode()).decode()
```

### Comparing `wicked_expressions-0.4.4/PKG-INFO` & `wicked_expressions-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicked-expressions
-Version: 0.4.4
+Version: 0.5.0
 Summary: Extension of bolt-expressions written in Bolt.
 Home-page: https://github.com/reapermc/wicked-expressions
 License: MIT
 Keywords: beet,bolt,minecraft,minecraft-commands,mcfunction
 Author: Yeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

