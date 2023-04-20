# Comparing `tmp/sphinx_probs_rdf-0.3.0.tar.gz` & `tmp/sphinx_probs_rdf-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_probs_rdf-0.3.0.tar", last modified: Thu Oct 27 10:39:29 2022, max compression
+gzip compressed data, was "sphinx_probs_rdf-0.4.0.tar", last modified: Thu Apr 20 10:10:03 2023, max compression
```

## Comparing `sphinx_probs_rdf-0.3.0.tar` & `sphinx_probs_rdf-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,32 @@
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2022-10-27 10:39:29.362468 sphinx_probs_rdf-0.3.0/
--rw-r--r--   0 rcl38      (502) staff       (20)     1078 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.3.0/LICENSE
--rw-r--r--   0 rcl38      (502) staff       (20)       50 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.3.0/MANIFEST.in
--rw-r--r--   0 rcl38      (502) staff       (20)     1238 2022-10-27 10:39:29.362594 sphinx_probs_rdf-0.3.0/PKG-INFO
--rw-r--r--   0 rcl38      (502) staff       (20)      485 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.3.0/README.rst
--rw-r--r--   0 rcl38      (502) staff       (20)      357 2022-10-27 10:39:29.366046 sphinx_probs_rdf-0.3.0/setup.cfg
--rw-r--r--   0 rcl38      (502) staff       (20)     1718 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.3.0/setup.py
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2022-10-27 10:39:29.349600 sphinx_probs_rdf-0.3.0/src/
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2022-10-27 10:39:29.358330 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf/
--rw-r--r--   0 rcl38      (502) staff       (20)     2259 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf/__init__.py
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2022-10-27 10:39:29.361948 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf/_static/
--rw-r--r--   0 rcl38      (502) staff       (20)     2003 2022-09-21 23:03:52.000000 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf/_static/system-definitions.css
--rw-r--r--   0 rcl38      (502) staff       (20)     1339 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf/builder.py
--rw-r--r--   0 rcl38      (502) staff       (20)    30437 2022-09-21 23:13:25.000000 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf/directives.py
--rw-r--r--   0 rcl38      (502) staff       (20)     1106 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf/postprocess.py
--rw-r--r--   0 rcl38      (502) staff       (20)       27 2022-10-27 10:38:44.000000 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf/version.py
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2022-10-27 10:39:29.361324 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf.egg-info/
--rw-r--r--   0 rcl38      (502) staff       (20)     1238 2022-10-27 10:39:29.000000 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf.egg-info/PKG-INFO
--rw-r--r--   0 rcl38      (502) staff       (20)      531 2022-10-27 10:39:29.000000 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf.egg-info/SOURCES.txt
--rw-r--r--   0 rcl38      (502) staff       (20)        1 2022-10-27 10:39:29.000000 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf.egg-info/dependency_links.txt
--rw-r--r--   0 rcl38      (502) staff       (20)        1 2022-09-21 10:32:32.000000 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf.egg-info/not-zip-safe
--rw-r--r--   0 rcl38      (502) staff       (20)       71 2022-10-27 10:39:29.000000 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf.egg-info/requires.txt
--rw-r--r--   0 rcl38      (502) staff       (20)       17 2022-10-27 10:39:29.000000 sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf.egg-info/top_level.txt
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-04-20 10:10:03.979920 sphinx_probs_rdf-0.4.0/
+-rw-r--r--   0 rcl38      (502) staff       (20)     1078 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/LICENSE
+-rw-r--r--   0 rcl38      (502) staff       (20)       50 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/MANIFEST.in
+-rw-r--r--   0 rcl38      (502) staff       (20)     1238 2023-04-20 10:10:03.979978 sphinx_probs_rdf-0.4.0/PKG-INFO
+-rw-r--r--   0 rcl38      (502) staff       (20)      485 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/README.rst
+-rw-r--r--   0 rcl38      (502) staff       (20)      357 2023-04-20 10:10:03.982246 sphinx_probs_rdf-0.4.0/setup.cfg
+-rw-r--r--   0 rcl38      (502) staff       (20)     1718 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/setup.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-04-20 10:10:03.963709 sphinx_probs_rdf-0.4.0/src/
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-04-20 10:10:03.971367 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/
+-rw-r--r--   0 rcl38      (502) staff       (20)     4995 2023-04-20 10:09:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/__init__.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-04-20 10:10:03.975383 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/_static/
+-rw-r--r--   0 rcl38      (502) staff       (20)     2007 2023-04-20 10:09:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/_static/system-definitions.css
+-rw-r--r--   0 rcl38      (502) staff       (20)     1236 2023-04-18 17:07:21.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/builder.py
+-rw-r--r--   0 rcl38      (502) staff       (20)    30726 2023-04-20 10:09:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/directives.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     1106 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/postprocess.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     7867 2023-04-20 10:09:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/resolve.py
+-rw-r--r--   0 rcl38      (502) staff       (20)       27 2023-04-20 10:09:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/version.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-04-20 10:10:03.975004 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/
+-rw-r--r--   0 rcl38      (502) staff       (20)     1238 2023-04-20 10:10:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/PKG-INFO
+-rw-r--r--   0 rcl38      (502) staff       (20)      805 2023-04-20 10:10:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 rcl38      (502) staff       (20)        1 2023-04-20 10:10:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 rcl38      (502) staff       (20)        1 2022-09-21 10:32:32.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/not-zip-safe
+-rw-r--r--   0 rcl38      (502) staff       (20)       71 2023-04-20 10:10:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/requires.txt
+-rw-r--r--   0 rcl38      (502) staff       (20)       17 2023-04-20 10:10:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/top_level.txt
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-04-20 10:10:03.979363 sphinx_probs_rdf-0.4.0/tests/
+-rw-r--r--   0 rcl38      (502) staff       (20)     2843 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/tests/test_directive_options.py
+-rw-r--r--   0 rcl38      (502) staff       (20)      661 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/tests/test_missing_process.py
+-rw-r--r--   0 rcl38      (502) staff       (20)      892 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/tests/test_postprocess.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     1360 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/tests/test_probs_rdf_builder_basic.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     3989 2023-04-20 10:09:03.000000 sphinx_probs_rdf-0.4.0/tests/test_probs_rdf_builder_myst.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     1204 2023-03-08 21:16:17.000000 sphinx_probs_rdf-0.4.0/tests/test_probs_rdf_builder_prefixes.py
+-rw-r--r--   0 rcl38      (502) staff       (20)      848 2023-04-20 10:09:03.000000 sphinx_probs_rdf-0.4.0/tests/test_probs_system_directives.py
```

### Comparing `sphinx_probs_rdf-0.3.0/LICENSE` & `sphinx_probs_rdf-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.3.0/PKG-INFO` & `sphinx_probs_rdf-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_probs_rdf
-Version: 0.3.0
+Version: 0.4.0
 Summary: sphinx_probs_rdf is a sphinx extension which outputs RDF describing Processes and Objects using the PRObs ontology.
 Home-page: https://github.com/ricklupton/sphinx_probs_rdf
 Download-URL: https://pypi.org/project/sphinx_probs_rdf/
 Author: Rick Lupton
 Author-email: mail@ricklupton.name
 License: BSD
 Platform: any
```

### Comparing `sphinx_probs_rdf-0.3.0/setup.py` & `sphinx_probs_rdf-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf/_static/system-definitions.css` & `sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/_static/system-definitions.css`

 * *Files 9% similar despite different names*

```diff
@@ -27,36 +27,36 @@
 }
 
 @media (min-width: 575.98px) {
     .system.process.nested-1,
     .system.object.nested-1,
     .system.end-sub-objects.nested-1,
     .system.end-sub-processes.nested-1 {
-        margin-left: 1.5em;
+        margin-left: 1.5rem;
     }
 
     .system.process.nested-2,
     .system.object.nested-2,
     .system.end-sub-objects.nested-2,
     .system.end-sub-processes.nested-2  {
-        margin-left: 3em;
+        margin-left: 3.0rem;
     }
 
     .system.process.nested-3,
     .system.object.nested-3,
     .system.end-sub-objects.nested-3,
     .system.end-sub-processes.nested-3  {
-        margin-left: 4.5em;
+        margin-left: 4.5rem;
     }
 
     .system.process.nested-4,
     .system.object.nested-4,
     .system.end-sub-objects.nested-4,
     .system.end-sub-processes.nested-4 {
-        margin-left: 6em;
+        margin-left: 6.0rem;
     }
 }
 
 .admonition.system.object {
     border-color: #fff6dd;
 }
 .admonition.system.object .admonition-title {
@@ -88,10 +88,10 @@
     border-left: 2px solid #ffc107;
 }
 .system.end-sub-processes {
     border-left: 2px solid #007bff;
 }
 
 /* Fix issue with toggle dropdown admonitions not hiding tables */
-.toggle-hidden.admonition .admonition-title ~ table {
+.toggle-hidden.admonition .admonition-title ~ * {
   display: none;
 }
```

### Comparing `sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf/builder.py` & `sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os.path
-from typing import Set
+from typing import Set, cast
 
 from docutils.nodes import Node
 from sphinx.builders import Builder
 from sphinx.locale import __
 from sphinx.util import logging
 
 from .postprocess import postprocess
+from .directives import SystemDomain
 
 logger = logging.getLogger(__name__)
 
 
 class ProbsSystemRDFBuilder(Builder):
     """
     Extracts RDF from system definitions
@@ -32,17 +33,13 @@
     def write_doc(self, docname: str, doctree: Node) -> None:
         return
 
     def finish(self) -> None:
         assert self.app.builder
         env = self.app.builder.env
         assert env is not None
+        domain = cast(SystemDomain, env.get_domain("system"))
         filename = os.path.join(self.outdir, 'output.ttl')
-        if hasattr(env, 'probs_graph'):
-            graph = env.probs_graph  # type: ignore
-            postprocess(graph)
-            with open(filename, 'wb') as f:
-                graph.serialize(f, format="turtle")
-        else:
-            logger.warning('No graph found!')
-            with open(filename, 'wb') as f:
-                f.write(b"")
+        graph = domain.graph
+        postprocess(graph)
+        with open(filename, 'wb') as f:
+            graph.serialize(f, format="turtle")
```

### Comparing `sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf/directives.py` & `sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/directives.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from collections import defaultdict
-from typing import Any, List
+from typing import Any, List, Dict, Iterator, Tuple, Optional, NamedTuple, cast
 import re
 import yaml
 
 from docutils import nodes
-from docutils.nodes import Node
+from docutils.nodes import Node, Element
 from docutils.parsers.rst import directives  # type: ignore
-from rdflib import Graph, URIRef, Literal, BNode, Namespace  # type: ignore
+from rdflib import Graph, ConjunctiveGraph, URIRef, Literal, BNode, Namespace  # type: ignore
 from rdflib.namespace import RDF, RDFS  # type: ignore
 from sphinx import addnodes
+from sphinx.addnodes import desc_signature, pending_xref
+from sphinx.builders import Builder
+from sphinx.locale import _, __
 from sphinx.directives import ObjectDescription
 from sphinx.directives.code import CodeBlock
-from sphinx.domains import Domain, Index
+from sphinx.domains import Domain, Index, ObjType
+from sphinx.environment import BuildEnvironment
 from sphinx.roles import XRefRole
 from sphinx.util.docfields import DocFieldTransformer
 from sphinx.util.docutils import SphinxDirective
-from sphinx.util.nodes import make_refnode
+from sphinx.util.nodes import make_refnode, find_pending_xref_condition, make_id
 from sphinx.util import logging
 
 logger = logging.getLogger(__name__)
 
 
 def parse_composed_of(value):
     """Parse composed_of option."""
@@ -129,15 +133,16 @@
     return item
 
 
 class TTL(CodeBlock):
     has_content = True
 
     def run(self):
-        g = get_or_setup_graph(self.env, self.config)
+        domain = cast(SystemDomain, self.env.get_domain("system"))
+        g = domain.get_graph(self.env.docname)
         preamble = "\n".join('@prefix %s: <%s> .\n' % (prefix, uri)
                              for prefix, uri in g.namespaces())
         input_data = preamble + "\n" + "\n".join(self.content)
         try:
             g.parse(data=input_data, format="text/turtle")
         except SyntaxError as err:
             logger.warning("Cannot parse TTL block: %s", err,
@@ -147,363 +152,312 @@
         self.arguments = ["turtle"]
         return super().run()
 
 
 class StartSubProcessesDirective(SphinxDirective):
     required_arguments = 1
 
-    @property
-    def SYS(self) -> Namespace:
-        """Return the system namespace."""
-        return Namespace(self.config.probs_rdf_system_prefix)
-
     def run(self):
-        if not hasattr(self.env, "probs_parent"):
-            self.env.probs_parent = []
-
-        uri = getattr(self.SYS, self.arguments[0])
-        self.env.probs_parent.append(uri)
+        uri = parse_uri(self.config, self.arguments[0])
+        self.env.ref_context["system:process"] = uri
+        parents = self.env.ref_context.setdefault("system:processes", [])
+        parents.append(uri)
 
         paragraph_node = nodes.literal_block(text=f'Starting sub processes of "{uri}"')
         return [paragraph_node]
 
 
 class StartSubObjectsDirective(SphinxDirective):
     required_arguments = 1
 
-    @property
-    def SYS(self) -> Namespace:
-        """Return the system namespace."""
-        return Namespace(self.config.probs_rdf_system_prefix)
-
     def run(self):
-        if not hasattr(self.env, "probs_parent_object"):
-            self.env.probs_parent_object = []
-
-        uri = getattr(self.SYS, self.arguments[0])
-        self.env.probs_parent_object.append(uri)
+        uri = parse_uri(self.config, self.arguments[0])
+        self.env.ref_context["system:object"] = uri
+        parents = self.env.ref_context.setdefault("system:objects", [])
+        parents.append(uri)
 
         paragraph_node = nodes.literal_block(text=f'Starting sub objects of "{uri}"')
         return [paragraph_node]
 
 
 class EndSubProcessesDirective(SphinxDirective):
     def run(self):
-        if not hasattr(self.env, "probs_parent"):
-            self.env.probs_parent = []
-        if self.env.probs_parent:
-            leaving = self.env.probs_parent.pop()
+        parents = self.env.ref_context.setdefault("system:processes", [])
+        if parents:
+            nesting_depth = len(parents)
+            leaving = parents.pop()
             _, _, leaving_id = leaving.rpartition("/")
-            nesting_depth = len(self.env.probs_parent)
             paragraph_node = nodes.paragraph(
                 text=f'Ending sub processes of "{leaving_id}"',
                 classes=["system", "end-sub-processes", f"nested-{nesting_depth}"],
             )
         else:
             paragraph_node = nodes.literal_block(text="Nothing to end!")
-        return [paragraph_node]
 
+        self.env.ref_context["system:process"] = (
+            parents[-1] if parents else None
+        )
+
+        return [paragraph_node]
 
 
 class EndSubObjectsDirective(SphinxDirective):
     def run(self):
-        if not hasattr(self.env, "probs_parent_object"):
-            self.env.probs_parent_object = []
-        if self.env.probs_parent_object:
-            leaving = self.env.probs_parent_object.pop()
+        parents = self.env.ref_context.setdefault("system:objects", [])
+        if parents:
+            nesting_depth = len(parents)
+            leaving = parents.pop()
             _, _, leaving_id = leaving.rpartition("/")
-            nesting_depth = len(self.env.probs_parent_object)
             paragraph_node = nodes.paragraph(
                 text=f'Ending sub objects of "{leaving_id}"',
                 classes=["system", "end-sub-objects", f"nested-{nesting_depth}"],
             )
         else:
             paragraph_node = nodes.literal_block(text="Nothing to end!")
+
+        self.env.ref_context["system:object"] = (
+            parents[-1] if parents else None
+        )
+
         return [paragraph_node]
 
 
 PROBS = Namespace("https://ukfires.org/probs/ontology/")
 PROBS_RECIPE = Namespace("https://ukfires.org/probs/ontology/recipe/")
 QUANTITYKIND = Namespace("http://qudt.org/vocab/quantitykind/")
 
 
-def remove_ns(ns, uri):
-    if uri[: len(ns)] == ns:
-        return uri[len(ns) :]
-
-
-def get_or_setup_graph(env, config):
-    """Return the rdflib Graph or set up a new one as needed."""
-    if env is None or not hasattr(env, "probs_graph"):
-        g = Graph()
-        g.bind("sys", Namespace(config.probs_rdf_system_prefix))
-        g.bind("probs", PROBS)
-        g.bind("rec", PROBS_RECIPE)
-        for prefix, uri in config.probs_rdf_extra_prefixes.items():
-            g.bind(prefix, uri)
-        if env is not None:
-            env.probs_graph = g
-    else:
-        g = env.probs_graph
-    return g
+class probs_info(nodes.Element, nodes.General):
+    """Node for PRObs info.
+    """
+
+
+class rdf_reference(nodes.reference):
+    """Reference to RDF object.
+    """
+
+
+class probs_process_info(probs_info):
+    pass
+
+
+class probs_object_info(probs_info):
+    pass
+
+
+class ObjectEquivalentTo(SphinxDirective):
+    required_arguments = 2
+    option_spec = {
+        "confidence": directives.unchanged,
+        'class': directives.class_option,
+    }
+    has_content = True
+
+    def run(self):
+        if not self.options.get('class'):
+            self.options['class'] = ['admonition-object-equivalent-to']
+
+        # self.assert_has_content()
+        uri1 = parse_uri(self.config, self.arguments[0])
+        uri2 = parse_uri(self.config, self.arguments[1])
+
+        node = nodes.admonition()
+
+        title = nodes.title("", "")
+        title += [
+            nodes.strong("Object equivalence: ", "Object equivalence: "),
+            rdf_reference(uri1, target=uri1, include_label=True),
+            nodes.Text(" ⇔ "),
+            rdf_reference(uri2, target=uri2, include_label=True),
+        ]
+
+        self.indexnode = addnodes.index(entries=[])
+
+        contentnode = nodes.paragraph()  # desc_content?
+        node += [title, contentnode]
+        self.state.nested_parse(self.content, self.content_offset, contentnode)
+
+        g = self.env.get_domain("system").get_graph(self.env.docname)
+        g.add((uri1, PROBS.objectEquivalentTo, uri2))
+
+        return [self.indexnode, node]
+
 
 
 class SystemObjectDescription(ObjectDescription):
     has_content = True
     required_arguments = 1
-    # option_spec = {
-    #     'label': directives.unchanged_required,
-    #     'become_parent': directives.flag,
-    #     'consumes': directives.unchanged,
-    #     'produces': directives.unchanged,
-    # }
-
-    @property
-    def SYS(self) -> Namespace:
-        """Return the system namespace."""
-        return Namespace(self.config.probs_rdf_system_prefix)
 
     def run(self) -> List[Node]:
-        """
-        Main directive entry function, called by docutils upon encountering the
-        directive.
+        """Override to return admonitions rather than descs.
 
-        This directive is meant to be quite easily subclassable, so it
-        delegates to several additional methods.  What it does:
-
-        * find out if called as a domain-specific directive, set self.domain
-        * create a `desc` node to fit all description inside
-        * parse standard options, currently `noindex`
-        * create an index node if needed as self.indexnode
-        * parse all given signatures (as returned by self.get_signatures())
-          using self.handle_signature(), which should either return a name
-          or raise ValueError
-        * add index entries using self.add_target_and_index()
-        * parse the content and handle doc fields in it
+        This is a hacky way of getting a collapsible/togglable block, rather
+        than inline descriptions.
 
         """
-        if ":" in self.name:
-            self.domain, self.objtype = self.name.split(":", 1)
-        else:
-            self.domain, self.objtype = "", self.name
-        self.indexnode = addnodes.index(entries=[])
-
         nest_depth = "nested-%d" % self.get_nesting_depth()
-        node = nodes.admonition(classes=["toggle", self.objtype, nest_depth])
-        node.document = self.state.document
-        node["domain"] = self.domain
-        # 'desctype' is a backwards compatible attribute
-        node["objtype"] = node["desctype"] = self.objtype
-        node["noindex"] = noindex = "noindex" in self.options
-        if self.domain:
-            node["classes"].append(self.domain)
 
-        self.names = []  # type: List[Any]
-        signatures = self.get_signatures()
-        assert len(signatures) == 1, "only assuming 1 signature can be given"
-        for i, sig in enumerate(signatures):
-            # add a signature node for each signature in the current unit
-            # and add a reference target for it
-            signode = nodes.title(sig, "")
-            self.set_source_info(signode)
-            node.append(signode)
-            try:
-                # name can also be a tuple, e.g. (classname, objname);
-                # this is strictly domain-specific (i.e. no assumptions may
-                # be made in this base class)
-                name = self.handle_signature(sig, signode)
-            except ValueError:
-                # signature parsing failed
-                signode.clear()
-                signode += addnodes.desc_name(sig, sig)
-                continue  # we don't want an index entry here
-            if name not in self.names:
-                self.names.append(name)
-                if not noindex:
-                    # only add target and index entry if this is the first
-                    # description of the object with this name in this desc
-                    # block
-                    self.add_target_and_index(name, sig, signode)
+        indexnode, node = super().run()
 
-        contentnode = nodes.paragraph()
-        node.append(contentnode)
-        if self.names:
-            # needed for association of version{added,changed} directives
-            self.env.temp_data["object"] = self.names[0]
-        self.before_content()
-        self.state.nested_parse(self.content, self.content_offset, contentnode)
-        self.transform_content(contentnode)
-        self.env.app.emit(
-            "object-description-transform", self.domain, self.objtype, contentnode
-        )
-        DocFieldTransformer(self).transform_all(contentnode)
-        self.env.temp_data["object"] = None
-        self.after_content()
+        # Replace `desc` with `admonition`
+        new_node = nodes.admonition("", *node.children)
+        new_node["classes"] = node["classes"] + ["toggle", nest_depth]
+
+        # Replace desc_content with paragraph and desc_signature with title
+        for sig in new_node.findall(addnodes.desc_signature):
+            sig.replace_self([nodes.title("", "", *sig.children)])
+        for content in new_node.findall(addnodes.desc_content):
+            content.replace_self(content.children)
+
+        return [indexnode, new_node]
+
+    def get_signatures(self) -> List[str]:
+        signatures = super().get_signatures()
+        if len(signatures) > 1:
+            logger.warning("Multiple signatures not supported")
+        return signatures[:1]
 
-        # Do this here so `become_parent` hasn't taken effect too early
-        self.define_graph(signatures[0])
+    def handle_signature(self, sig: str, signode: desc_signature) -> str:
+        """Transform a "signature" (i.e. name for this thing) into RST nodes.
 
-        return [self.indexnode, node]
+        Return URI of the thing.
+        """
+        uri = parse_uri(self.config, sig)
+        signode["uri"] = uri
 
-    def handle_signature(self, sig, signode):
+        # XXX is there is a better desc_XXX node for this?
         signode += nodes.emphasis(self.signature_prefix, self.signature_prefix)
         signode += addnodes.desc_name(sig, sig)
         if "label" in self.options:
-            signode += nodes.emphasis(
+            signode += addnodes.desc_addname(
                 self.options["label"], " / " + self.options["label"]
             )
-        return sig
 
-    def _system_id_link(self, sys_id, within=None):
-        """Insert a cross reference to another object/process."""
-        refnode = addnodes.pending_xref('', refdomain="system", refexplicit=False,
-                                        reftype="ref", reftarget=sys_id)
-        refnode += nodes.inline(sys_id, sys_id)
-        if within is not None:
-            wrapper = within("", "")
-            wrapper += refnode
-            return wrapper
-        return refnode
+        g = self.env.get_domain("system").get_graph(self.env.docname)
+        self.define_graph(g, uri, sig)
+
+        return uri
 
 
 class Process(SystemObjectDescription):
-    # has_content = True
-    # required_arguments = 1
     option_spec = {
         "label": directives.unchanged_required,
         "become_parent": directives.flag,
         "consumes": parse_consumes_or_produces,
         "produces": parse_consumes_or_produces,
         "composed_of": parse_composed_of,
         "defs": directives.unchanged,
     }
     signature_prefix = "Process: "
 
-    def transform_content(self, contentnode):
-        # XXX Should refactor this to reduce duplication and/or read from the
-        # graph
-        defs = self.options.get("defs", "")
-        consumes, produces = expand_consumes_produces_amounts(
-            defs, self.options.get("consumes", []), self.options.get("produces", []))
-
-        if consumes:
-            contentnode += nodes.paragraph("Consumes: ", "Consumes: ")
-            contentnode += self._recipe_table(consumes)
-        if produces:
-            contentnode += nodes.paragraph("Produces: ", "Produces: ")
-            contentnode += self._recipe_table(produces)
-        if hasattr(self.env, "probs_parent") and self.env.probs_parent:
-            _, _, parent_id = self.env.probs_parent[-1].rpartition("/")
-            p = nodes.paragraph("", "Parent: ")
-            p += self._system_id_link(parent_id)
-            contentnode += p
-
-    def _recipe_table(self, objects):
-        header_rows = [[nodes.literal("", "Object"), nodes.literal("", "Amount")]]
-        table_data = [
-            [self._system_id_link(obj["object"], nodes.paragraph),
-             nodes.literal("", "%.1f %s" % (obj["amount"], obj["unit"]))
-             if "amount" in obj else ""]
-            for obj in objects
-        ]
-        return build_table_from_list(header_rows + table_data, header_rows=1)
-
     def get_nesting_depth(self):
-        if hasattr(self.env, "probs_parent"):
-            return len(self.env.probs_parent)
-        return 0
-
-    def add_target_and_index(self, name_cls, sig, signode):
-        # print('add_target_and_index', name_cls, sig, signode)
-        # print(self.options)
-        signode["ids"].append("process" + "-" + sig)
-        if "noindex" not in self.options:
-            recipes = self.env.get_domain("system")
-            recipes.add_process(
-                sig,
-                self.options.get("consumes", []),
-                self.options.get("produces", []),
-            )
+        return len(self.env.ref_context.get('system:processes', []))
+
+    def add_target_and_index(self, uri, sig, signode):
+        node_id = make_id(self.env, self.state.document, '', uri)
+        signode["ids"].append(node_id)
+        domain = cast(SystemDomain, self.env.get_domain("system"))
+        # XXX maybe label should come from RDF later
+        domain.note_thing(
+            uri, "process", self.options.get("label", sig), node_id, location=signode
+        )
+        # XXX avoid parse_uri too many times?
+        domain.note_process_recipe(
+            uri,
+            [parse_uri(self.config, obj["object"]) for obj in self.options.get("consumes", [])],
+            [parse_uri(self.config, obj["object"]) for obj in self.options.get("produces", [])],
+        )
 
-    def define_graph(self, uri_str):
-        g = get_or_setup_graph(self.env, self.config)
+    def before_content(self):
+        """Handle object nesting before content."""
+        if self.names:
+            uri = self.names[-1]
+            self.env.ref_context["system:process"] = uri
+            parents = self.env.ref_context.setdefault("system:processes", [])
+            parents.append(uri)
 
-        if not hasattr(self.env, "probs_parent"):
-            self.env.probs_parent = []
+    def transform_content(self, contentnode):
+        if self.names:
+            uri = self.names[0]
+            info = probs_process_info("", uri=uri)
+            contentnode.insert(0, info)
+
+    def after_content(self):
+        """Handle object de-nesting after content."""
+        parents = self.env.ref_context.setdefault("system:processes", [])
+        if parents and "become_parent" not in self.options:
+            parents.pop()
+        self.env.ref_context["system:process"] = (
+            parents[-1] if parents else None
+        )
 
-        uri = getattr(self.SYS, uri_str)
+    def define_graph(self, g, uri, sig: str):
+        label = self.options.get("label", sig)
 
         g.add((uri, RDF.type, PROBS.Process))
-        if "label" in self.options:
-            g.add((uri, RDFS.label, Literal(self.options["label"])))
-            g.add((uri, PROBS.processName, Literal(self.options["label"])))
-        else:
-            g.add((uri, RDFS.label, Literal(uri_str)))
-            g.add((uri, PROBS.processName, Literal(uri_str)))
+        g.add((uri, RDFS.label, Literal(label)))
+        g.add((uri, PROBS.processName, Literal(label)))
 
         # ComposedOf relationships
-        if self.env.probs_parent:
-            g.add((self.env.probs_parent[-1], PROBS.processComposedOf, uri))
+        # determine parent
+        if "parent" in self.options:
+            parent = parse_uri(self.config, self.options["parent"])
+        else:
+            parent = self.env.ref_context.get("system:process")
+        if parent:
+            g.add((parent, PROBS.processComposedOf, uri))
         for child in self.options.get("composed_of", []):
             if child.startswith("*"):
                 # include children of the named process -- this is expanded
                 # later as a postprocessing step once all processes are defined.
-                child_uri = self.SYS[child[1:]]
+                child_uri = parse_uri(self.config, child[1:])
                 g.add((uri, PROBS.processComposedOfChildrenOf, child_uri))
             else:
-                child_uri = self.SYS[child]
+                child_uri = parse_uri(self.config, child)
                 g.add((uri, PROBS.processComposedOf, child_uri))
 
         # Recipes (inputs and outputs)
         # First expand any expressions
         defs = self.options.get("defs", "")
         consumes, produces = expand_consumes_produces_amounts(
             defs, self.options.get("consumes", []), self.options.get("produces", []))
 
         recipe_consumes, recipe_produces = [], []
-        _process_inputs_outputs(g, self.SYS, uri, "consumes", consumes, recipe_consumes)
-        _process_inputs_outputs(g, self.SYS, uri, "produces", produces, recipe_produces)
+        _process_inputs_outputs(g, self.config, uri, "consumes", consumes, recipe_consumes)
+        _process_inputs_outputs(g, self.config, uri, "produces", produces, recipe_produces)
         if recipe_consumes or recipe_produces:
             recipe = BNode()
             g.add((uri, PROBS_RECIPE.hasRecipe, recipe))
             for item in recipe_consumes:
                 g.add((recipe, PROBS_RECIPE.consumes, item))
             for item in recipe_produces:
                 g.add((recipe, PROBS_RECIPE.produces, item))
 
-        if "become_parent" in self.options:
-            # print("xxx become parent")
-            self.env.probs_parent.append(uri)
-
-
-SUPPORTED_UNIT_METRICS = {
-    "kg": QUANTITYKIND.Mass,
-    "m2": QUANTITYKIND.Area,
-    "m3": QUANTITYKIND.Volume,
-    "-": QUANTITYKIND.Dimensionless,
-}
 
-
-def _process_inputs_outputs(g, SYS, uri, relation, objects, recipe_items):
+def _process_inputs_outputs(g, config, uri, relation, objects, recipe_items):
+    units = config.probs_rdf_units
     for obj in objects:
-        obj_uri = getattr(SYS, obj["object"])
+        obj_uri = parse_uri(config, obj["object"])
         g.add((uri, PROBS[relation], obj_uri))
 
         if "amount" in obj:
             # Have a recipe
 
             # XXX only support a few units for now, this could be more general.
-            if "unit" in obj and obj["unit"] not in SUPPORTED_UNIT_METRICS:
-                logger.error("Unsupported unit %r for object %r in recipe for %r",
-                             obj["unit"], obj["object"], uri)
+            if "unit" in obj and obj["unit"] not in units:
+                logger.error("Unsupported unit %r for object %r in recipe for %r -- treating as 'kg'",
+                             obj["unit"], obj["object"], str(uri))
+                scale, metric = units["kg"]
+            else:
+                scale, metric = units[obj["unit"]]
 
             item = BNode()
             g.add((item, PROBS_RECIPE.object, obj_uri))
-            g.add((item, PROBS_RECIPE.quantity, Literal(obj["amount"])))
-            g.add((item, PROBS_RECIPE.metric, SUPPORTED_UNIT_METRICS[obj["unit"]]))
+            g.add((item, PROBS_RECIPE.quantity, Literal(scale * obj["amount"])))
+            g.add((item, PROBS_RECIPE.metric, metric))
             recipe_items.append(item)
 
 
 def parse_traded(value):
     """Check the value of the :traded: option is valid."""
     if value is None:
         return (False, False)
@@ -520,332 +474,410 @@
     """Convert list of uris."""
     if value is None:
         value = ""
     items = [x.strip() for x in value.split()]
     return items
 
 
+def parse_uri(config, item, default=None):
+    """Convert a string to a URIRef.
+
+    A blank prefix or bare id refers to the namespace given by the
+    `probs_rdf_system_prefix` config variable.
+
+    A missing suffix means the same as the object currently being defined.
+
+    """
+    if item and item[0] == "<" and item[-1] == ">":
+        return URIRef(item[1:-1])
+    prefix, _, item_id = item.rpartition(":")
+    if not prefix:
+        ns = Namespace(config.probs_rdf_system_prefix)
+    else:
+        ns = Namespace(config.probs_rdf_extra_prefixes[prefix])
+    if not item_id:
+        item_id = default if default is not None else ""
+    return getattr(ns, item_id)
+
+
 class Object(SystemObjectDescription):
     has_content = True
     required_arguments = 1
     option_spec = {
         "label": directives.unchanged,
         "become_parent": directives.flag,
         "parent_object": directives.unchanged,
+        "composed_of": parse_composed_of,
         "traded": parse_traded,
         "equivalent": parse_equivalent,
     }
     signature_prefix = "Object: "
 
-    # def handle_signature(self, sig, signode):
-    #     signode += nodes.emphasis("Object: ", "Object: ")
-    #     signode += addnodes.desc_name(sig, sig)
-    #     if "label" in self.options:
-    #         signode += addnodes.desc_addname(self.options["label"],
-    #                                          self.options["label"])
-    #     return sig
-
-    def transform_content(self, contentnode):
-        if hasattr(self.env, "probs_parent_object") and self.env.probs_parent_object:
-            _, _, parent_id = self.env.probs_parent_object[-1].rpartition("/")
-            p = nodes.paragraph("", "Parent: ")
-            p += self._system_id_link(parent_id)
-            contentnode += p
-
     def get_nesting_depth(self):
-        if hasattr(self.env, "probs_parent_object"):
-            return len(self.env.probs_parent_object)
-        return 0
-
-    def add_target_and_index(self, name_cls, sig, signode):
-        # print('add_target_and_index', name_cls, sig, signode)
-        # print(self.options)
-        signode["ids"].append("object" + "-" + sig)
-        if "noindex" not in self.options:
-            recipes = self.env.get_domain("system")
-            recipes.add_object(sig, [])
+        return len(self.env.ref_context.get("system:objects", []))
 
-    def define_graph(self, uri_str):
-        g = get_or_setup_graph(self.env, self.config)
+    def add_target_and_index(self, uri, sig, signode):
+        node_id = make_id(self.env, self.state.document, '', uri)
+        signode["ids"].append(node_id)
+        domain = cast(SystemDomain, self.env.get_domain("system"))
+        # XXX maybe label should come from RDF later
+        domain.note_thing(
+            uri, "object", self.options.get("label", sig), node_id, location=signode
+        )
 
-        if not hasattr(self.env, "probs_parent_object"):
-            self.env.probs_parent_object = []
+    def before_content(self):
+        """Handle object nesting before content."""
+        if self.names:
+            uri = self.names[-1]
+            self.env.ref_context["system:object"] = uri
+            parents = self.env.ref_context.setdefault("system:objects", [])
+            parents.append(uri)
 
-        uri = getattr(self.SYS, uri_str)
+    def transform_content(self, contentnode):
+        if self.names:
+            uri = self.names[0]
+            info = probs_object_info("", uri=uri)
+            contentnode.insert(0, info)
+
+    def after_content(self):
+        """Handle object de-nesting after content."""
+        parents = self.env.ref_context.setdefault("system:objects", [])
+        if parents and "become_parent" not in self.options:
+            parents.pop()
+        self.env.ref_context["system:object"] = (
+            parents[-1] if parents else None
+        )
+
+    def define_graph(self, g, uri, sig: str):
+        label = self.options.get("label", sig)
 
         g.add((uri, RDF.type, PROBS.Object))
         g.add((uri, RDF.type, PROBS.ReferenceObject))
-        if "label" in self.options:
-            g.add((uri, RDFS.label, Literal(self.options["label"])))
-            g.add((uri, PROBS.objectName, Literal(self.options["label"])))
-        else:
-            g.add((uri, RDFS.label, Literal(uri_str)))
-            g.add((uri, PROBS.objectName, Literal(uri_str)))
+        g.add((uri, RDFS.label, Literal(label)))
+        g.add((uri, PROBS.objectName, Literal(label)))
 
+        # ComposedOf relationships
         if "parent_object" in self.options:
-            parent_uri = getattr(self.SYS, self.options["parent_object"])
-            g.add((parent_uri, PROBS.objectComposedOf, uri))
-        elif self.env.probs_parent_object:
-            g.add((self.env.probs_parent_object[-1], PROBS.objectComposedOf, uri))
-
-        if "become_parent" in self.options:
-            # print("xxx become parent object")
-            self.env.probs_parent_object.append(uri)
+            parent = parse_uri(self.config, self.options["parent_object"])
+        else:
+            parent = self.env.ref_context.get("system:object")
+        if parent:
+            g.add((parent, PROBS.objectComposedOf, uri))
+        for child in self.options.get("composed_of", []):
+            if child.startswith("*"):
+                # include children of the named object -- this is expanded later
+                # as a postprocessing step once all processes are defined.
+                child_uri = parse_uri(self.config, child[1:])
+                g.add((uri, PROBS.objectComposedOfChildrenOf, child_uri))
+            else:
+                child_uri = parse_uri(self.config, child)
+                g.add((uri, PROBS.objectComposedOf, child_uri))
 
         if "traded" in self.options:
             imp, exp = self.options["traded"]
             if imp != exp:
                 logger.error("Currently objects must be either fully traded"
                              "(imports and exports) or not at all")
             g.add((uri, PROBS.objectIsTraded, Literal(imp or exp)))
 
         if "equivalent" in self.options:
             for item in self.options["equivalent"]:
                 item_uri = self.parse_uri(item)
                 g.add((uri, PROBS.objectEquivalentTo, item_uri))
 
-
     def parse_uri(self, item):
         """Convert a string to a URIRef.
 
         A blank prefix or bare id refers to the namespace given by the
         `probs_rdf_system_prefix` config variable.
 
         A missing suffix means the same as the object currently being defined.
 
         """
-        if item and item[0] == "<" and item[-1] == ">":
-            return URIRef(item[1:-1])
-        prefix, _, item_id = item.rpartition(":")
-        if not prefix:
-            ns = Namespace(self.config.probs_rdf_system_prefix)
-        else:
-            ns = Namespace(self.config.probs_rdf_extra_prefixes[prefix])
-        if not item_id:
-            signatures = self.get_signatures()
-            assert len(signatures) == 1, "only assuming 1 signature can be given"
-            item_id = signatures[0]
-        return getattr(ns, item_id)
+        signatures = self.get_signatures()
+        assert len(signatures) == 1, "only assuming 1 signature can be given"
+        default_item_id = signatures[0]
+        return parse_uri(self.config, item, default_item_id)
 
 
 class ObjectIndex(Index):
     """Index of objects."""
 
-    name = "object"
+    name = "objectindex"
     localname = "Object Index"
-    shortname = "Object"
+    shortname = "objects"
 
     def generate(self, docnames=None):
         content = defaultdict(list)
 
         objects = {
-            name: (dispname, typ, docname, anchor)
-            for name, dispname, typ, docname, anchor, _ in self.domain.data["objects"]
+            uri: thing
+            for uri, thing in self.domain.things.items()
+            if thing.thing_type == "object"
         }
         processes = {
-            name: (dispname, typ, docname, anchor)
-            for name, dispname, typ, docname, anchor, _ in self.domain.data["processes"]
+            uri: thing
+            for uri, thing in self.domain.things.items()
+            if thing.thing_type == "process"
         }
-        process_consumes = self.domain.data["process_consumes"]
-        process_produces = self.domain.data["process_produces"]
+        # processes = {
+        #     name: (dispname, typ, docname, anchor)
+        #     for name, dispname, typ, docname, anchor, _ in self.domain.data["processes"]
+        # }
+        process_recipe = self.domain.process_recipe
         object_processes = defaultdict(list)
 
         # Add the objects initially; this is necessary for any objects which are
         # NOT linked to processes to be included.
-        for obj in objects.values():
-            dispname = obj[0]
-            object_processes[dispname] = []
+        for obj_uri in objects:
+            object_processes[obj_uri] = []
 
         # Add in all the places that an object is consumed or produced by a
         # process
-        for process_name, objs in process_consumes.items():
-            for obj in objs:
-                if ("object." + obj["object"]) not in objects:
+        for process_uri, objs in process_recipe.items():
+            if process_uri not in processes:
+                logger.error(
+                    "Process %s that %s object %s is not defined",
+                    process_uri,
+                    direction,
+                    obj_uri,
+                    # location=(self.env.docname, self.lineno)
+                )
+                continue
+            for obj_uri, direction in objs:
+                if obj_uri not in objects:
                     logger.error(
-                        "Object %s consumed by process %s is not defined",
-                        obj["object"],
-                        process_name,
+                        "Object %s %s by process %s is not defined",
+                        obj_uri,
+                        direction[:-1] + "d",
+                        process_uri,
                         # location=(self.env.docname, self.lineno)
                     )
                     continue
-                object_processes[obj["object"]].append((process_name, "consumed"))
-        for process_name, objs in process_produces.items():
-            for obj in objs:
-                if ("object." + obj["object"]) not in objects:
-                    logger.error(
-                        "Object %s produced by process %s is not defined",
-                        obj["object"],
-                        process_name,
-                        # location=(self.env.docname, self.lineno)
-                    )
-                    continue
-                object_processes[obj["object"]].append((process_name, "produced"))
+                object_processes[obj_uri].append((process_uri, direction))
 
         # convert the mapping of objects to processes to produce the expected
         # output, shown below, using the object name as a key to group
         #
         # name, subtype, docname, anchor, extra, qualifier, description
-        for obj, process_names in object_processes.items():
-            dispname, typ, docname, anchor = objects["object." + obj]
-            k = dispname[0].lower()
-            content[k].append((dispname, 1, docname, anchor, docname, "", typ))
-
-            for process_name, direction in process_names:
-                dispname, typ, docname, anchor = processes[process_name]
-                content[k].append((dispname, 2, docname, anchor, direction, "", typ))
+        for obj_uri, process_uris in object_processes.items():
+            obj = objects[obj_uri]
+            k = obj.label.upper()[0]
+            content[k].append((obj.label, 1, obj.docname, obj.node_id, obj.docname, "", obj.thing_type))
+
+            for process_uri, direction in process_uris:
+                if process_uri in processes:
+                    p = processes[process_uri]
+                    content[k].append((p.label, 2, p.docname, p.node_id, direction, "", p.thing_type))
+                else:
+                    logger.debug("Missing process in domain: %s", process_uri)
 
         # convert the dict to the sorted list of tuples expected
         content = sorted(content.items())
 
         return content, True
 
 
 class ProcessIndex(Index):
     """Index of processes."""
 
-    name = "process"
+    name = "processindex"
     localname = "Process Index"
-    shortname = "Process"
+    shortname = "processes"
 
     def generate(self, docnames=None):
         content = defaultdict(list)
 
         # sort the list of processes in alphabetical order
-        processes = self.domain.data["processes"]
-        processes = sorted(processes, key=lambda process: process[0])
+        processes = {
+            uri: thing
+            for uri, thing in self.domain.things.items()
+            if thing.thing_type == "process"
+        }
 
         # generate the expected output, shown below, from the above using the
         # first letter of the recipe as a key to group thing
         #
         # name, subtype, docname, anchor, extra, qualifier, description
-        for name, dispname, typ, docname, anchor, _ in processes:
-            content[dispname[0].lower()].append(
-                (dispname, 0, docname, anchor, docname, "", typ)
+        for process_uri, thing in processes.items():
+            k = thing.label.upper()[0]
+            content[k].append(
+                (thing.label, 0, thing.docname, thing.node_id, thing.docname, "", thing.thing_type)
             )
 
         # convert the dict to the sorted list of tuples expected
         content = sorted(content.items())
 
         return content, True
 
 
+class ThingEntry(NamedTuple):
+    docname: str
+    node_id: str
+    thing_type: str
+    label: str
+
+
 class SystemDomain(Domain):
 
     name = "system"
     label = "System definition"
-    roles = {"ref": XRefRole()}
+
+    # These are the different types of things that we can keep track of, and
+    # which roles can cross-reference to them.
+    object_types = {
+        'process': ObjType(_('process'), 'ref'),
+        'object':  ObjType(_('object'),  'ref'),
+    }
+    roles = {
+        "ref": XRefRole()
+    }
     directives = {
         "process": Process,
         "object": Object,
-        # 'startSubProcesses': StartSubProcessesDirective,
+        "object-equivalent-to": ObjectEquivalentTo,
     }
     indices = [ProcessIndex, ObjectIndex]
     initial_data: dict = {
-        "processes": [],  # object list
-        "objects": [],  # object list
-        "process_consumes": {},
-        "process_produces": {},
+        "things": {},
+        "process_recipe": {},
+        "graph": None,
     }
 
-    def get_full_qualified_name(self, node):
-        if node.get("refdomain") == "system":
-            return "{}.{}".format("system", node.get("reftarget"))
-        return None
+    ### Keeping track of where things are defined
 
-    def get_objects(self):
-        for obj in self.data["processes"]:
-            yield (obj)
-        for obj in self.data["objects"]:
-            yield (obj)
-
-    def resolve_xref(self, env, fromdocname, builder, typ, target, node, contnode):
-        match = [
-            (docname, anchor)
-            for name, sig, typ, docname, anchor, prio in self.get_objects()
-            if sig == target
-        ]
+    @property
+    def things(self) -> Dict[str, ThingEntry]:
+        return self.data.setdefault('things', {})  # uri -> ThingEntry
 
-        if len(match) > 0:
-            todocname = match[0][0]
-            targ = match[0][1]
+    @property
+    def graph(self) -> ConjunctiveGraph:
+        if self.data.get("graph") is None:
+            g = self.data["graph"] = ConjunctiveGraph()
+            config = self.env.config
+            g.bind("sys", Namespace(config.probs_rdf_system_prefix))
+            g.bind("probs", PROBS)
+            g.bind("rec", PROBS_RECIPE)
+            for prefix, uri in config.probs_rdf_extra_prefixes.items():
+                g.bind(prefix, uri)
+        return self.data["graph"]
 
-            # print("system domain: found %s %s %r xref" % (todocname, targ, target))
-            return make_refnode(builder, fromdocname, todocname, targ, contnode, targ)
+    @property
+    def process_recipe(self) -> Dict[str, list]:
+        return self.data.setdefault('process_recipe', {})  # uri -> list
 
-        return None
+    def get_graph(self, graph_id):
+        return self.graph.get_context(graph_id)
 
-    def add_process(self, signature, consumes, produces):
-        """Add a new process to the domain."""
-        name = "{}.{}".format("process", signature)
-        anchor = "process-{}".format(signature)
-
-        # self.data['recipe_ingredients'][name] = ingredients
-        # name, dispname, type, docname, anchor, priority
-        self.data["processes"].append(
-            (name, signature, "Process", self.env.docname, anchor, 0)
+    def note_thing(self, uri: str, thing_type: str, label: str, node_id: str, location: Any = None):
+        """Note the definition of a thing (what Sphinx calls an "object")."""
+        if uri in self.things:
+            # duplicated
+            other = self.things[uri]
+            logger.warning(__('duplicate description of %s, '
+                              'other instance in %s, use :noindex: for one of them'),
+                           uri, other.docname, location=location)
+        self.things[uri] = ThingEntry(self.env.docname, node_id, thing_type, label)
+
+    def note_process_recipe(self, uri: str, consumes: list, produces: list):
+        self.process_recipe[uri] = (
+            [(k, "consumes") for k in consumes] +
+            [(k, "produces") for k in produces]
         )
-        self.data["process_consumes"][name] = consumes
-        self.data["process_produces"][name] = produces
 
-    def add_object(self, signature, ingredients):
-        """Add a new object to the domain."""
-        name = "{}.{}".format("object", signature)
-        anchor = "object-{}".format(signature)
-
-        # self.data['recipe_ingredients'][name] = ingredients
-        # name, dispname, type, docname, anchor, priority
-        self.data["objects"].append(
-            (name, signature, "Object", self.env.docname, anchor, 0)
-        )
+    def clear_doc(self, docname: str) -> None:
+        for uri, thing in list(self.things.items()):
+            if thing.docname == docname:
+                del self.things[uri]
+
+        g = self.get_graph(docname)
+        g.remove((None, None, None))
+
+    def merge_domaindata(self, docnames: List[str], otherdata: Dict) -> None:
+        # XXX check duplicates?
+        for uri, thing in otherdata['things'].items():
+            if thing.docname in docnames:
+                self.things[uri] = thing
+        if "graph" in otherdata:
+            self.graph += otherdata["graph"]
+
+    def find_thing(
+        self,
+        name: str,
+        base_uri: Optional[str] = None,
+        current_thing: Optional[str] = None,
+        thing_type: Optional[str] = None,
+    ) -> List[Tuple[str, ThingEntry]]:
+        """Find a thing definition for "name", perhaps using the configured
+        prefixes. Returns a list of (uri, thing entry) tuples.
+        """
+        # XXX this could be more flexible, e.g. parsing prefixes, allowing
+        # relative URIs or absolute URIs -- or looking first for names that
+        # feature within the current process's inputs or outputs.
 
+        if thing_type is None:
+            thing_types = list(self.object_types)
+        else:
+            thing_types = self.objtypes_for_role(thing_type)
 
-# Adapted from docutils ListTable directive
-def build_table_from_list(table_data,
-                          # col_widths,
-                          header_rows, stub_columns=0, widths="auto"):
-    """
-    :param table_data: list of lists giving table data
-    :param header_rows: list of header rows
-    :param stub_columns: number of columns to mark as "stubs"
-    """
+        matches = [
+            (uri, thing)
+            for uri, thing in self.things.items()
+            if uri.endswith(name) and thing.thing_type in thing_types
+        ]
 
-    table = nodes.table()
+        return matches
 
-    max_cols = len(table_data[0])
-    col_widths = [100 // max_cols] * max_cols
-    # if widths == 'auto':
-    #     table['classes'] += ['colwidths-auto']
-    # elif widths: # "grid" or list of integers
-    #     table['classes'] += ['colwidths-given']
-    table['classes'] += ['colwidths-auto']
-
-    tgroup = nodes.tgroup(cols=max_cols)
-    table += tgroup
-
-    for col_width in col_widths:
-        colspec = nodes.colspec()
-        # if col_width is not None:
-        #     colspec.attributes['colwidth'] = col_width
-        if stub_columns:
-            colspec.attributes['stub'] = 1
-            stub_columns -= 1
-        tgroup += colspec
-
-    rows = []
-    for row in table_data:
-        row_node = nodes.row()
-        for cell in row:
-            entry = nodes.entry()
-            entry += cell
-            row_node += entry
-        rows.append(row_node)
-
-    if header_rows:
-        thead = nodes.thead()
-        thead.extend(rows[:header_rows])
-        tgroup += thead
-
-    tbody = nodes.tbody()
-    tbody.extend(rows[header_rows:])
-    tgroup += tbody
+    def resolve_xref(
+        self,
+        env: BuildEnvironment,
+        fromdocname: str,
+        builder: Builder,
+        thing_type: str,
+        target: str,
+        node: pending_xref,
+        contnode: Element,
+    ) -> Optional[Element]:
+
+        matches = self.find_thing(target, thing_type=thing_type)
+
+        if not matches:
+            return None
+        elif len(matches) > 1:
+            logger.warning(__('more than one target found for cross-reference %r: %s'),
+                           target, ', '.join(match[0] for match in matches),
+                           type='ref', subtype='system', location=node)
+        uri, thing = matches[0]
+
+        # determine the content of the reference by conditions
+        content = find_pending_xref_condition(node, 'resolved')
+        if content:
+            children = content.children
+        else:
+            # if not found, use contnode
+            children = [contnode]
 
-    return table
+        return make_refnode(builder, fromdocname, thing.docname, thing.node_id, children, uri)
+
+    # TODO: implement `resolve_any_xref`?
+
+    def get_objects(self) -> Iterator[Tuple[str, str, str, str, str, int]]:
+        # Returns:
+        # - name: fully qualified name
+        # - dispname: Name to display when searching/linking.
+        # - type: Object type, a key in ``self.object_types``
+        # - docname: The document where it is to be found.
+        # - anchor: The anchor name for the object.
+        # - priority: determines placement in search results:
+        #   1 = default (before full-text matches)
+        #   0 = important (before default-priority)
+        #   2 = unimportant (after full-text matches)
+        #   -1 = don't show in search at all
+
+        for uri, thing in self.things.items():
+            yield (uri, thing.label, thing.thing_type, thing.docname, thing.node_id, 1)
+
+    def get_full_qualified_name(self, node):
+        # XXX Fix me to return URI
+        if node.get("refdomain") == "system":
+            return "{}.{}".format("system", node.get("reftarget"))
+        return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf/postprocess.py` & `sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/postprocess.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf.egg-info/PKG-INFO` & `sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-probs-rdf
-Version: 0.3.0
+Version: 0.4.0
 Summary: sphinx_probs_rdf is a sphinx extension which outputs RDF describing Processes and Objects using the PRObs ontology.
 Home-page: https://github.com/ricklupton/sphinx_probs_rdf
 Download-URL: https://pypi.org/project/sphinx_probs_rdf/
 Author: Rick Lupton
 Author-email: mail@ricklupton.name
 License: BSD
 Platform: any
```

### Comparing `sphinx_probs_rdf-0.3.0/src/sphinx_probs_rdf.egg-info/SOURCES.txt` & `sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,23 @@
 README.rst
 setup.cfg
 setup.py
 src/sphinx_probs_rdf/__init__.py
 src/sphinx_probs_rdf/builder.py
 src/sphinx_probs_rdf/directives.py
 src/sphinx_probs_rdf/postprocess.py
+src/sphinx_probs_rdf/resolve.py
 src/sphinx_probs_rdf/version.py
 src/sphinx_probs_rdf.egg-info/PKG-INFO
 src/sphinx_probs_rdf.egg-info/SOURCES.txt
 src/sphinx_probs_rdf.egg-info/dependency_links.txt
 src/sphinx_probs_rdf.egg-info/not-zip-safe
 src/sphinx_probs_rdf.egg-info/requires.txt
 src/sphinx_probs_rdf.egg-info/top_level.txt
-src/sphinx_probs_rdf/_static/system-definitions.css
+src/sphinx_probs_rdf/_static/system-definitions.css
+tests/test_directive_options.py
+tests/test_missing_process.py
+tests/test_postprocess.py
+tests/test_probs_rdf_builder_basic.py
+tests/test_probs_rdf_builder_myst.py
+tests/test_probs_rdf_builder_prefixes.py
+tests/test_probs_system_directives.py
```

