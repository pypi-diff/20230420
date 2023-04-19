# Comparing `tmp/nmodl_preprocessor-1.0.1.tar.gz` & `tmp/nmodl_preprocessor-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmodl_preprocessor-1.0.1.tar", last modified: Mon Apr 17 16:54:47 2023, max compression
+gzip compressed data, was "nmodl_preprocessor-1.0.2.tar", last modified: Wed Apr 19 23:45:51 2023, max compression
```

## Comparing `nmodl_preprocessor-1.0.1.tar` & `nmodl_preprocessor-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-17 16:54:47.035674 nmodl_preprocessor-1.0.1/
--rw-rw-r--   0 dm        (1000) dm        (1000)       31 2023-04-08 16:15:16.000000 nmodl_preprocessor-1.0.1/.gitignore
--rw-rw-r--   0 dm        (1000) dm        (1000)    37759 2023-04-17 15:40:58.000000 nmodl_preprocessor-1.0.1/DETAILS.pdf
--rw-rw-r--   0 dm        (1000) dm        (1000)     1076 2023-03-28 16:31:04.000000 nmodl_preprocessor-1.0.1/LICENSE.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)     1830 2023-04-17 16:54:47.035674 nmodl_preprocessor-1.0.1/PKG-INFO
--rw-rw-r--   0 dm        (1000) dm        (1000)     1089 2023-04-17 16:48:55.000000 nmodl_preprocessor-1.0.1/README.md
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-17 16:54:47.035674 nmodl_preprocessor-1.0.1/nmodl_preprocessor/
--rw-rw-r--   0 dm        (1000) dm        (1000)    14400 2023-04-17 15:59:48.000000 nmodl_preprocessor-1.0.1/nmodl_preprocessor/__main__.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     2355 2023-04-09 23:42:01.000000 nmodl_preprocessor-1.0.1/nmodl_preprocessor/nmodl_to_python.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     2734 2023-04-08 16:02:06.000000 nmodl_preprocessor-1.0.1/nmodl_preprocessor/rw_patterns.py
--rw-rw-r--   0 dm        (1000) dm        (1000)      305 2023-04-05 13:58:59.000000 nmodl_preprocessor-1.0.1/nmodl_preprocessor/utils.py
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-17 16:54:47.035674 nmodl_preprocessor-1.0.1/nmodl_preprocessor.egg-info/
--rw-rw-r--   0 dm        (1000) dm        (1000)     1830 2023-04-17 16:54:46.000000 nmodl_preprocessor-1.0.1/nmodl_preprocessor.egg-info/PKG-INFO
--rw-rw-r--   0 dm        (1000) dm        (1000)      444 2023-04-17 16:54:46.000000 nmodl_preprocessor-1.0.1/nmodl_preprocessor.egg-info/SOURCES.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)        1 2023-04-17 16:54:46.000000 nmodl_preprocessor-1.0.1/nmodl_preprocessor.egg-info/dependency_links.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)       80 2023-04-17 16:54:46.000000 nmodl_preprocessor-1.0.1/nmodl_preprocessor.egg-info/entry_points.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)        6 2023-04-17 16:54:46.000000 nmodl_preprocessor-1.0.1/nmodl_preprocessor.egg-info/requires.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)       19 2023-04-17 16:54:46.000000 nmodl_preprocessor-1.0.1/nmodl_preprocessor.egg-info/top_level.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)      971 2023-04-17 16:54:21.000000 nmodl_preprocessor-1.0.1/pyproject.toml
--rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-17 16:54:47.035674 nmodl_preprocessor-1.0.1/setup.cfg
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-19 23:45:51.358063 nmodl_preprocessor-1.0.2/
+-rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-19 23:44:54.000000 nmodl_preprocessor-1.0.2/.gitignore
+-rw-rw-r--   0 dm        (1000) dm        (1000)    37883 2023-04-19 23:02:12.000000 nmodl_preprocessor-1.0.2/DETAILS.pdf
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1076 2023-03-28 16:31:04.000000 nmodl_preprocessor-1.0.2/LICENSE.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1830 2023-04-19 23:45:51.358063 nmodl_preprocessor-1.0.2/PKG-INFO
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1089 2023-04-17 16:48:55.000000 nmodl_preprocessor-1.0.2/README.md
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-19 23:45:51.358063 nmodl_preprocessor-1.0.2/nmodl_preprocessor/
+-rw-rw-r--   0 dm        (1000) dm        (1000)    14444 2023-04-19 23:31:48.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor/__main__.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     3664 2023-04-19 22:43:58.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor/nmodl_to_python.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     2994 2023-04-19 23:30:29.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor/rw_patterns.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)      480 2023-04-19 21:45:07.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor/utils.py
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-19 23:45:51.358063 nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1830 2023-04-19 23:45:51.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/PKG-INFO
+-rw-rw-r--   0 dm        (1000) dm        (1000)      444 2023-04-19 23:45:51.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/SOURCES.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)        1 2023-04-19 23:45:51.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/dependency_links.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)       80 2023-04-19 23:45:51.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/entry_points.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)        6 2023-04-19 23:45:51.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/requires.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)       19 2023-04-19 23:45:51.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/top_level.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)      971 2023-04-19 23:36:20.000000 nmodl_preprocessor-1.0.2/pyproject.toml
+-rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-19 23:45:51.358063 nmodl_preprocessor-1.0.2/setup.cfg
```

### Comparing `nmodl_preprocessor-1.0.1/DETAILS.pdf` & `nmodl_preprocessor-1.0.2/DETAILS.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 15% similar despite different names*

#### pdftotext {} -

```diff
@@ -29,15 +29,17 @@
 }
 
 INITIAL {
 Q10 = 3^((celsius - temp) / 10)
 }
 
 INITIAL {
-assert(celsius == 37.0)
+VERBATIM
+assert(celsius == 37.0);
+ENDVERBATIM
 }
 
 Q10 = 3^(( 37.0(degC) - 23.0(degC) ) / 10)
 
 Hard-code the parameters
 and the temperature
 
```

### Comparing `nmodl_preprocessor-1.0.1/LICENSE.txt` & `nmodl_preprocessor-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.1/PKG-INFO` & `nmodl_preprocessor-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmodl_preprocessor
-Version: 1.0.1
+Version: 1.0.2
 Summary: Optimize NMODL files for the NEURON simulator
 Author-email: David McDougall <dam1784@rit.edu>
 License: MIT
 Project-URL: homepage, https://github.com/ctrl-z-9000-times/nmodl_preprocessor
 Keywords: nmodl,neuron
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
```

### Comparing `nmodl_preprocessor-1.0.1/README.md` & `nmodl_preprocessor-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.1/nmodl_preprocessor/__main__.py` & `nmodl_preprocessor-1.0.2/nmodl_preprocessor/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,17 @@
     inlined_blocks      = [x for x in (functions | procedures) if x not in solve_blocks]
     # Find all symbols that are referenced in VERBATIM blocks.
     verbatim_vars = set()
     for stmt in lookup(ANT.VERBATIM):
         for symbol in re.finditer(r'\b\w+\b', nmodl.to_nmodl(stmt)):
             verbatim_vars.add(symbol.group())
     # Let's get this warning out of the way. As chunks of C/C++ code, VERBATIM
-    # statements can not be analysed correctly. Assume that all symbols in
-    # VERBATIM blocks are both read from and written to. Do not attempt to
-    # alter the source code in any VERBATIM statements.
+    # statements can not be analysed. Assume that all symbols in VERBATIM
+    # blocks are both read from and written to. Do not attempt to alter the
+    # source code inside of VERBATIM blocks.
     if lookup(ANT.VERBATIM):
         print_verbose('warning: VERBATIM may prevent optimization')
     # Find all symbols which are provided by or are visible to the larger NEURON simulation.
     external_vars = (
             neuron_vars |
             read_ion_vars |
             write_ion_vars |
@@ -138,15 +138,15 @@
     rw.visit_program(AST)
     # Split the document into its top-level blocks for easier manipulation.
     blocks_list = [SimpleNamespace(node=x, text=nmodl.to_nmodl(x)) for x in AST.blocks]
     blocks      = {get_block_name(x.node): x for x in blocks_list}
 
     # Inline the parameters.
     parameters = {}
-    for name in (parameter_vars - external_vars - verbatim_vars):
+    for name in (parameter_vars - external_vars - verbatim_vars - rw.all_writes):
         for node in sym_table.lookup(name).get_nodes():
             if node.is_param_assign() and node.value is not None:
                 value = float(STR(node.value))
                 units = ('('+STR(node.unit.name)+')') if node.unit else ''
                 parameters[name] = (value, units)
                 print_verbose(f'inline PARAMETER: {name} = {value} {units}')
 
@@ -168,29 +168,29 @@
             can_exec = True
         except nmodl_to_python.VerbatimError:
             can_exec = False
         except nmodl_to_python.ComplexityError:
             can_exec = False
             print_verbose('warning: complex INITIAL block may prevent optimization')
         # 
-        global_scope  = {}
+        global_scope  = {"math": math} # Include the standard math library.
         initial_scope = {}
         # Represent unknown external input values as NaN's.
         for name in external_vars:
             global_scope[name] = math.nan
         # 
         for name, (value, units) in parameters.items():
             global_scope[name] = value
         # 
         if can_exec:
             try:
                 exec(x.pycode, global_scope, initial_scope)
             except:
-                pycode = '\n'.join(str(i+1).rjust(2) + ": " + line for i, line in enumerate(x.pycode.split('\n'))) # Prepend line numbers.
-                print("While exec'ing:\n"+pycode)
+                pycode = prepend_line_numbers(x.pycode.rstrip())
+                print_verbose("error: while executing INITIAL block:\n" + pycode)
                 raise
         # Filter out any assignments that were made with unknown input values.
         initial_scope = dict(x for x in initial_scope.items() if not math.isnan(x[1]))
         # Do not inline variables if they are written to in other blocks besides the INITIAL block.
         runtime_writes_to = set()
         for block_name, variables in rw.writes.items():
             if block_name != 'INITIAL':
@@ -269,15 +269,15 @@
             value = str(value) + units
             block.text = re.sub(rf'\b{name}\b', value, block.text)
 
     # Check the temperature in the INITIAL block.
     if args.celsius is not None:
         if block := blocks.get('INITIAL', None):
             signature, start, body = block.text.partition('{')
-            check_temp = f"\n    assert(celsius == {args.celsius})\n"
+            check_temp = f"\n    VERBATIM\n    assert(celsius == {args.celsius});\n    ENDVERBATIM\n"
             block.text = signature + start + check_temp + body
 
     # Insert new LOCAL statements to replace the removed assigned variables.
     new_locals = {} # Maps from block name to set of names of new local variables.
     if assigned_const_value:
         new_locals['INITIAL'] = set(assigned_const_value.keys())
     for block_name, write_variables in rw.writes.items():
```

### Comparing `nmodl_preprocessor-1.0.1/nmodl_preprocessor/rw_patterns.py` & `nmodl_preprocessor-1.0.2/nmodl_preprocessor/rw_patterns.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,21 @@
     """ Determines which symbols each top-level block reads from and writes to. """
     def __init__(self):
         super().__init__()
         self.current_block = None
         # Maps from block name to set of symbol names.
         self.reads = {}
         self.writes = {}
+        # Set of all variables which are assigned to.
+        self.all_writes = set()
+
+    def visit_program(self, node):
+        node.visit_children(self)
+        for block_name, var_names in self.writes.items():
+            self.all_writes.update(var_names)
 
     def visit_statement_block(self, node):
         # Look for top level code blocks.
         if self.current_block is None:
             self.current_block = get_block_name(node.parent)
             self.reads[self.current_block]  = set()
             self.writes[self.current_block] = set()
```

### Comparing `nmodl_preprocessor-1.0.1/nmodl_preprocessor.egg-info/PKG-INFO` & `nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmodl-preprocessor
-Version: 1.0.1
+Version: 1.0.2
 Summary: Optimize NMODL files for the NEURON simulator
 Author-email: David McDougall <dam1784@rit.edu>
 License: MIT
 Project-URL: homepage, https://github.com/ctrl-z-9000-times/nmodl_preprocessor
 Keywords: nmodl,neuron
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
```

### Comparing `nmodl_preprocessor-1.0.1/pyproject.toml` & `nmodl_preprocessor-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nmodl_preprocessor"
-version = "1.0.1"
+version = "1.0.2"
 description = "Optimize NMODL files for the NEURON simulator"
 readme = "README.md"
 authors = [
     {name = "David McDougall", email = "dam1784@rit.edu"},
 ]
 license = {text = "MIT"}
 keywords = ["nmodl", "neuron"]
```

