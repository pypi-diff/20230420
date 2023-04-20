# Comparing `tmp/bigraph-schema-0.0.2.tar.gz` & `tmp/bigraph-schema-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigraph-schema-0.0.2.tar", last modified: Wed Apr 12 21:55:38 2023, max compression
+gzip compressed data, was "bigraph-schema-0.0.3.tar", last modified: Thu Apr 20 03:14:45 2023, max compression
```

## Comparing `bigraph-schema-0.0.2.tar` & `bigraph-schema-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-12 21:55:38.493119 bigraph-schema-0.0.2/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1081 2023-04-12 21:55:38.493119 bigraph-schema-0.0.2/PKG-INFO
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      151 2023-04-11 21:38:33.000000 bigraph-schema-0.0.2/README.md
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-12 21:55:38.493119 bigraph-schema-0.0.2/bigraph_schema/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      109 2023-04-11 21:34:23.000000 bigraph-schema-0.0.2/bigraph_schema/__init__.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2140 2023-04-11 21:34:23.000000 bigraph-schema-0.0.2/bigraph_schema/parse.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    17514 2023-04-12 21:52:57.000000 bigraph-schema-0.0.2/bigraph_schema/registry.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    15754 2023-04-12 21:54:50.000000 bigraph-schema-0.0.2/bigraph_schema/schema.py
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-12 21:55:38.493119 bigraph-schema-0.0.2/bigraph_schema.egg-info/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1081 2023-04-12 21:55:38.000000 bigraph-schema-0.0.2/bigraph_schema.egg-info/PKG-INFO
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      310 2023-04-12 21:55:38.000000 bigraph-schema-0.0.2/bigraph_schema.egg-info/SOURCES.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)        1 2023-04-12 21:55:38.000000 bigraph-schema-0.0.2/bigraph_schema.egg-info/dependency_links.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       18 2023-04-12 21:55:38.000000 bigraph-schema-0.0.2/bigraph_schema.egg-info/requires.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       15 2023-04-12 21:55:38.000000 bigraph-schema-0.0.2/bigraph_schema.egg-info/top_level.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       38 2023-04-12 21:55:38.493119 bigraph-schema-0.0.2/setup.cfg
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-04-12 21:55:21.000000 bigraph-schema-0.0.2/setup.py
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-20 03:14:45.892244 bigraph-schema-0.0.3/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1081 2023-04-20 03:14:45.892244 bigraph-schema-0.0.3/PKG-INFO
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      151 2023-04-11 21:38:33.000000 bigraph-schema-0.0.3/README.md
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-20 03:14:45.892244 bigraph-schema-0.0.3/bigraph_schema/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      106 2023-04-19 21:19:48.000000 bigraph-schema-0.0.3/bigraph_schema/__init__.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2140 2023-04-11 21:34:23.000000 bigraph-schema-0.0.3/bigraph_schema/parse.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    18007 2023-04-20 03:13:20.000000 bigraph-schema-0.0.3/bigraph_schema/registry.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    18411 2023-04-20 03:07:04.000000 bigraph-schema-0.0.3/bigraph_schema/schema.py
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-20 03:14:45.892244 bigraph-schema-0.0.3/bigraph_schema.egg-info/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1081 2023-04-20 03:14:45.000000 bigraph-schema-0.0.3/bigraph_schema.egg-info/PKG-INFO
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      310 2023-04-20 03:14:45.000000 bigraph-schema-0.0.3/bigraph_schema.egg-info/SOURCES.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)        1 2023-04-20 03:14:45.000000 bigraph-schema-0.0.3/bigraph_schema.egg-info/dependency_links.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       18 2023-04-20 03:14:45.000000 bigraph-schema-0.0.3/bigraph_schema.egg-info/requires.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       15 2023-04-20 03:14:45.000000 bigraph-schema-0.0.3/bigraph_schema.egg-info/top_level.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       38 2023-04-20 03:14:45.892244 bigraph-schema-0.0.3/setup.cfg
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-04-20 03:14:28.000000 bigraph-schema-0.0.3/setup.py
```

### Comparing `bigraph-schema-0.0.2/PKG-INFO` & `bigraph-schema-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigraph-schema
-Version: 0.0.2
+Version: 0.0.3
 Summary: A serializable type schema for compositional systems biology
 Home-page: https://github.com/vivarium-collective/bigraph-schema
 Author: Eran Agmon, Ryan Spangler
 Author-email: agmon.eran@gmail.com, ryan.spangler@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigraph-schema-0.0.2/bigraph_schema/parse.py` & `bigraph-schema-0.0.3/bigraph_schema/parse.py`

 * *Files identical despite different names*

### Comparing `bigraph-schema-0.0.2/bigraph_schema/registry.py` & `bigraph-schema-0.0.3/bigraph_schema/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 class Registry(object):
     def __init__(self):
         """A Registry holds a collection of functions or objects."""
         self.registry = {}
         self.main_keys = []
 
-    def register(self, key, item, alternate_keys=tuple()):
+    def register(self, key, item, alternate_keys=tuple(), force=False):
         """Add an item to the registry.
 
         Args:
             key: Item key.
             item: The item to add.
             alternate_keys: Additional keys under which to register the
                 item. These keys will not be included in the list
@@ -118,15 +118,15 @@
 
                 This may be useful if you want to be able to look up an
                 item in the registry under multiple keys.
         """
         keys = [key]
         keys.extend(alternate_keys)
         for registry_key in keys:
-            if registry_key in self.registry:
+            if registry_key in self.registry and not force:
                 if item != self.registry[registry_key]:
                     raise Exception(
                         'registry already contains an entry for {}: {} --> {}'.format(
                             registry_key, self.registry[key], item))
             else:
                 self.registry[registry_key] = item
         self.main_keys.append(key)
@@ -144,33 +144,37 @@
 
 class TypeRegistry(Registry):
 
     def __init__(self):
         super().__init__()
 
         self.supers = {}
-        self.register('any', {})
+        self.register('', {})
 
 
-    def register(self, key, item, alternate_keys=tuple()):
+    def register(self, key, item, alternate_keys=tuple(), force=False):
         item = copy.deepcopy(item)
         if isinstance(item, dict):
-            supers = item.get('_super', ['any']) # list of immediate supers
+            supers = item.get('_super', ['']) # list of immediate supers
             if isinstance(supers, str):
                 supers = [supers]
                 item['_super'] = supers
             for su in supers:
                 assert isinstance(
                     su, str), f"super for {key} must be a string, not {su}"
             self.supers[key] = supers
             for su in supers:
                 su_type = self.registry.get(su, {})
-                item = type_merge(item, su_type, merge_supers=False)
+                new_item = copy.deepcopy(su_type)
+                item = type_merge(
+                    new_item,
+                    item,
+                    merge_supers=False)
 
-        super().register(key, item, alternate_keys)
+        super().register(key, item, alternate_keys, force)
 
 
     def resolve_parameters(self, qualified_type):
         type_name, parameter_types = qualified_type
         outer_type = self.registry.get(type_name)
 
         if outer_type is None:
@@ -205,14 +209,16 @@
             schema.pop('_type')
             schema.update(type_schema)
 
         return schema
 
 
     def expand_schema(self, schema):
+        # make this only show the types at the leaves
+
         step = self.substitute_type(schema)
         for key, subschema in step.items():
             if key not in type_schema_keys:
                 step[key] = self.expand_schema(subschema)
         return step
         
 
@@ -263,14 +269,15 @@
         return typ
 
 
     def lookup(type_key, attribute):
         return self.access(type_key).get(attribute)
 
 
+    # description should come from type
     def is_descendent(self, key, ancestor):
         for sup in self.supers.get(key, []):
             if sup == ancestor:
                 return True
             else:
                 found = self.is_descendent(sup, ancestor)
                 if found:
@@ -393,14 +400,15 @@
 deserialize_registry.register('float', float)
 deserialize_registry.register('int', int)
 deserialize_registry.register('str', str)
 deserialize_registry.register('eval', eval)
 
 # if super type is re-registered, propagate changes to subtypes (?)
 
+# remove shape types
 type_library = {
     # abstract number type
     'number': {
         '_apply': 'accumulate',
         '_serialize': 'str',
         '_description': 'abstract base type for numbers',
     },
@@ -599,9 +607,20 @@
         {'_type': 'cube'})
 
     assert 'width' in cube_default
     assert 'height' in cube_default
     assert 'depth' in cube_default
 
 
+def test_expand_schema():
+    schema = {'_type': 'cube'}
+    expanded = type_registry.expand(schema)
+
+    assert len(schema) == 1
+    assert 'height' in expanded
+
+    import ipdb; ipdb.set_trace()
+
+
 if __name__ == '__main__':
     test_generate_default()
+    test_expand_schema()
```

### Comparing `bigraph-schema-0.0.2/bigraph_schema/schema.py` & `bigraph-schema-0.0.3/bigraph_schema/schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -40,51 +40,51 @@
                     report[key] = f'no entry in the {key} registry for: {value}'
         else:
             branches.add(key)
             branch_report = validate_schema(value)
             if len(branch_report) > 0:
                 report[key] = branch_report
 
-    # # We will need this when building instances to check to see if we are
+    # # We will need this when building states to check to see if we are
     # # trying to instantiate an abstract type, but we can still register
     # # register abstract types so it is not invalid
     # if len(schema_keys) > 0 and len(branches) == 0:
     #     undeclared = set(type_schema_keys) - schema_keys
     #     if len(undeclared) > 0:
     #         for key in undeclared:
     #             if not key in optional_schema_keys:
     #                 report[key] = f'missing required key: {key} for declaring atomic type'
 
     return report
 
 
-def validate_instance(schema, instance):
+def validate_state(schema, state):
     schema = type_registry.substitute_type(schema)
     validation = {}
 
     if '_serialize' in schema:
         if '_deserialize' not in schema:
             validation = {
                 '_deserialize': f'serialize found in type without deserialize: {schema}'
             }
         else:
             serialize = serialize_registry.access(schema['_serialize'])
             deserialize = deserialize_registry.access(schema['_deserialize'])
-            serial = serialize(instance)
+            serial = serialize(state)
             pass_through = deserialize(serial)
 
-            if instance != pass_through:
-                validation = f'instance and pass_through are not the same: {serial}'
+            if state != pass_through:
+                validation = f'state and pass_through are not the same: {serial}'
     else:
         for key, subschema in schema.items():
             if key not in type_schema_keys:
-                if key not in instance:
-                    validation[key] = f'key present in schema but not in instance: {key}\nschema: {schema}\ninstance: {instance}\n'
+                if key not in state:
+                    validation[key] = f'key present in schema but not in state: {key}\nschema: {schema}\nstate: {state}\n'
                 else:
-                    subvalidation = validate_instance(subschema, instance[key])
+                    subvalidation = validate_state(subschema, state[key])
                     if not (subvalidation is None or len(subvalidation) == 0):
                         validation[key] = subvalidation
 
     return validation
 
 
 def get_path(tree, path):
@@ -124,34 +124,34 @@
             return establish_path(
                 tree[head],
                 path[1:],
                 top=top,
                 cursor=cursor + (head,))
 
 
-def fill_ports(schema, wires=None, instance=None, top=None, path=()):
+def fill_ports(schema, wires=None, state=None, top=None, path=()):
     # deal with wires
     if wires is None:
         wires = {}
-    if instance is None:
-        instance = {}
+    if state is None:
+        state = {}
     if top is None:
-        top = instance
+        top = state
 
-    more_wires = instance.get('wires', {})
+    more_wires = state.get('wires', {})
     wires = deep_merge(wires, more_wires)
 
     for port_key, port_schema in schema.items():
         if port_key in wires:
             subwires = wires[port_key]
             if isinstance(subwires, dict):
-                instance[port_key] = fill_ports(
+                state[port_key] = fill_ports(
                     port_schema,
                     wires=subwires,
-                    instance=instance.get(port_key),
+                    state=state.get(port_key),
                     top=top,
                     path=path)
             else:
                 if isinstance(subwires, str):
                     subwires = (subwires,)
 
                 if len(path) == 0:
@@ -169,80 +169,84 @@
                     top=top,
                     cursor=path[:-1])
 
                 destination_key = subwires[-1]
 
                 if destination_key in destination:
                     pass
-                    # validate_instance(
+                    # validate_state(
                     #     port_schema,
                     #     destination[destination_key])
                 else:
                     destination[destination_key] = type_registry.generate_default(
                         port_schema)
         else:
             # handle unconnected ports
             pass
 
-    return instance
+    return state
 
 
-def fill_instance(schema, instance=None, top=None, path=(), type_key=None, context=None):
+def fill_state(schema, state=None, top=None, path=(), type_key=None, context=None):
     # if a port is disconnected, build a store
     # for it under the '_open' key in the current
     # node
 
     # inform the user that they have disconnected
     # ports somehow
 
     if top is None:
-        top = instance
+        top = state
 
     schema = type_registry.substitute_type(schema)
 
-    if instance is None:
+    if state is None:
         if '_default' in schema:
-            instance = type_registry.generate_default(schema)
+            state = type_registry.generate_default(schema)
         else:
-            instance = {}
+            state = {}
 
     if isinstance(schema, str):
         raise Exception(
             f'schema cannot be a str: {str}'
         )
 
     for key, subschema in schema.items():
         if key == '_ports':
-            wires = instance.get('wires', {})
-            instance = fill_ports(
+            wires = state.get('wires', {})
+            state = fill_ports(
                 subschema,
                 wires=wires,
-                instance=instance,
+                state=state,
                 top=top,
                 path=path)
 
         elif key not in type_schema_keys:
             subpath = path + (key,)
-            if isinstance(instance, dict):
-                instance[key] = fill_instance(
+            if isinstance(state, dict):
+                state[key] = fill_state(
                     subschema,
-                    instance=instance.get(key),
+                    state=state.get(key),
                     top=top,
                     path=subpath)
         
-    return instance
+    return state
 
 
-def fill(schema, instance=None):
-    if instance is not None:
-        instance = copy.deepcopy(instance)
-    return fill_instance(schema, instance=instance)
+def fill(schema, state=None):
+    if state is not None:
+        state = copy.deepcopy(state)
+    return fill_state(schema, state=state)
 
 
-def merge(a, b):
+def apply_update(schema, state, update):
+    pass
+
+
+def link_place(place, link):
     pass
 
 
 def compose(a, b):
     pass
 
 
@@ -251,19 +255,23 @@
     return {}
     
 
 def dehydrate(schema):
     return {}
 
 
-def query(schema, redex):
+def query(schema, state, redex):
     subschema = {}
     return subschema
 
 
+def substitute(schema, state, reactum):
+    return state
+
+
 def react(schema, redex, reactum):
     return {}
 
 
 def print_schema_validation(library, should_pass):
     for key, declaration in library.items():
         report = validate_schema(declaration)
@@ -326,61 +334,61 @@
 
 
 def test_fill_int():
     test_schema = {
         '_type': 'int'
     }
 
-    full_instance = fill(test_schema)
+    full_state = fill(test_schema)
 
-    assert full_instance == 0
+    assert full_state == 0
 
 
 def test_fill_cube():
     test_schema = {
         '_type': 'cube'
     }
 
-    partial_instance = {
+    partial_state = {
         'height': 5,
     }
 
-    full_instance = fill(
+    full_state = fill(
         test_schema,
-        instance=partial_instance)
+        state=partial_state)
 
-    assert 'width' in full_instance
-    assert 'height' in full_instance
-    assert 'depth' in full_instance
-    assert full_instance['height'] == 5
-    assert full_instance['depth'] == 0
+    assert 'width' in full_state
+    assert 'height' in full_state
+    assert 'depth' in full_state
+    assert full_state['height'] == 5
+    assert full_state['depth'] == 0
 
 
 def test_fill_in_missing_nodes():
     test_schema = {
         'edge 1': {
             # this could become a process_edge type
             '_type': 'edge',
             '_ports': {
                 'port A': {'_type': 'float'},
             },
         }
     }
 
-    test_instance = {
+    test_state = {
         'edge 1': {
             'wires': {
                 'port A': 'a',
             }
         }
     }
 
     filled = fill(
         test_schema,
-        test_instance
+        test_state
     )
 
     assert filled == {
         'a': 0.0,
         'edge 1': {
             'wires': {
                 'port A': 'a'
@@ -394,15 +402,15 @@
             '_type': 'edge',
             '_ports': {
                 '1': {'_type': 'float'},
             },
         }
     }
 
-    test_instance = {}
+    test_state = {}
 
     import ipdb; ipdb.set_trace()
 
 
 def test_fill_type_mismatch():
     test_schema = {
         'a': {'_type': 'int', '_value': 2},
@@ -473,22 +481,14 @@
          'made',
          'of',
          'light'))
 
     assert tree['some']['where']['deep']['inside']['lives']['a']['tiny']['creature']['made']['of']['light'] == destination
 
 
-def test_expand_schema():
-    schema = {'_type': 'cube'}
-    expanded = type_registry.expand(schema)
-
-    assert len(schema) == 1
-    assert 'height' in expanded
-
-
 def test_expected_schema():
     # equivalent to previous schema:
 
     # expected = {
     #     'store1': {
     #         'store1.1': {
     #             '_value': 1.1,
@@ -542,24 +542,24 @@
     }    
 
     type_registry.register(
         'dual_process',
         dual_process_schema,
     )
 
-    expected_schema = {
+    test_schema = {
         'store1': 'dual_process',
         'process3': {
             '_ports': {
                 'port1': 'dual_process'
             }
         }
     }
 
-    expected_instance = {
+    test_state = {
         'store1': {
             'process1': {
                 'wires': {
                     'port1': 'store1.1',
                     'port2': 'store1.2',
                 }
             },
@@ -573,15 +573,15 @@
         'process3': {
             'wires': {
                 'port1': 'store1',
             }
         },
     }
     
-    outcome = fill(expected_schema, expected_instance)
+    outcome = fill(test_schema, test_state)
 
     assert outcome == {
         'process3': {
             'wires': {
                 'port1': 'store1'
             }
         },
@@ -600,24 +600,132 @@
             },
             'store1.1': 0.0,
             'store1.2': 0
         }
     }
 
 
+def test_link_place():
+    bigraph = {
+        'nodes': {
+            ('v0',): {
+                '_type': 'int',
+                '_value': 3},
+            ('v0', 'v1'): {
+                '_type': 'int',
+                '_value': 3},
+            ('v0', 'v2'): {
+                '_type': 'int',
+                '_value': 3},
+            ('v0', 'v2', 'v3'): {
+                '_type': 'int',
+                '_value': 3},
+            ('v4',): {
+                '_type': 'int',
+                '_value': 3},
+            ('v4', 'v5'): {
+                '_type': 'int',
+                '_value': 3},
+            ('e0',): {
+                '_type': 'edge',
+                '_ports': {
+                    'e0.0': 'int',
+                    'e0.1': 'int',
+                    'e0.2': 'int'}},
+            ('e1',): {
+                '_type': 'edge',
+                '_ports': {
+                    'e0.0': 'int',
+                    'e0.1': 'int'}},
+            ('e2',): {
+                '_type': 'edge',
+                '_ports': {
+                    'e0.0': 'int',
+                    'e0.1': 'int',
+                    'e0.2': 'int'}}},
+        'place': {
+            'v0': {
+                'v1': {},
+                'v2': {
+                    'v3': {}}},
+            'v4': {
+                'v5': {}},
+            'e0': {},
+            'e1': {},
+            'e2': {}},
+        'link': {
+            'e0': {
+                'e0.0': ('v0',),
+                'e0.1': ('v0', 'v1'),
+                'e0.2': ('v4',)},
+            'e1': {
+                'e0.0': ('v0', 'v1', 'v3'),
+                'e0.1': ('v0', 'v1')},
+            'e2': {
+                'e0.0': ('v0', 'v1', 'v3'),
+                'e0.1': ('v4',),
+                'e0.2': ('v4', 'v5')}}}
+
+    placegraph = {
+        'v0': {
+            'v1': {},
+            'v2': {
+                'v3': {}}},
+        'v4': {
+            'v5': {}}}
+
+    hypergraph = {
+        'e0': {
+            'wires': {
+                'e0.0': 'v0',
+                'e0.1': 'v1',
+                'e0.2': 'v4'}},
+        'e1': {
+            'wires': {
+                'e0.0': 'v3',
+                'e0.1': 'v1'}},
+        'e2': {
+            'wires': {
+                'e0.0': 'v3',
+                'e0.1': 'v4',
+                'e0.2': 'v5'}}}
+
+    merged = {
+        'v0': {
+            'v1': {},
+            'v2': {
+                'v3': {}}},
+        'v4': {
+            'v5': {}},
+        'e0': {
+            'wires': {
+                'e0.0': 'v0',
+                'e0.1': ('v0', 'v1'),
+                'e0.2': 'v4'}},
+        'e1': {
+            'wires': {
+                'e0.0': ('v0', 'v2', 'v3'),
+                'e0.1': ('v0', 'v1')}},
+        'e2': {
+            'wires': {
+                'e0.0': ('v0', 'v2', 'v3'),
+                'e0.1': 'v4',
+                'e0.2': ('v4', 'v5')}}}    
+
+    result = link_place(placegraph, linkgraph)
+    assert result == merged
 
 
 if __name__ == '__main__':
     test_validate_schema()
     test_fill_int()
     test_fill_cube()
     test_establish_path()
     test_fill_in_missing_nodes()
     test_expected_schema()
-    test_expand_schema()
```

### Comparing `bigraph-schema-0.0.2/bigraph_schema.egg-info/PKG-INFO` & `bigraph-schema-0.0.3/bigraph_schema.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigraph-schema
-Version: 0.0.2
+Version: 0.0.3
 Summary: A serializable type schema for compositional systems biology
 Home-page: https://github.com/vivarium-collective/bigraph-schema
 Author: Eran Agmon, Ryan Spangler
 Author-email: agmon.eran@gmail.com, ryan.spangler@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigraph-schema-0.0.2/setup.py` & `bigraph-schema-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 
 with open("README.md", "r") as readme:
     description = readme.read()
 
 
 setup(
```

