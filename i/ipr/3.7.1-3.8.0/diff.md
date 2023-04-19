# Comparing `tmp/ipr-3.7.1.tar.gz` & `tmp/ipr-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipr-3.7.1.tar", last modified: Fri Mar 31 16:30:49 2023, max compression
+gzip compressed data, was "ipr-3.8.0.tar", last modified: Wed Apr 19 23:25:21 2023, max compression
```

## Comparing `ipr-3.7.1.tar` & `ipr-3.8.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:30:49.333495 ipr-3.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-31 16:30:39.000000 ipr-3.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-31 16:30:39.000000 ipr-3.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-31 16:30:49.333495 ipr-3.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-31 16:30:39.000000 ipr-3.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:30:49.333495 ipr-3.7.1/ipr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:30:39.000000 ipr-3.7.1/ipr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-03-31 16:30:39.000000 ipr-3.7.1/ipr/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-03-31 16:30:39.000000 ipr-3.7.1/ipr/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-31 16:30:39.000000 ipr-3.7.1/ipr/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    47688 2023-03-31 16:30:39.000000 ipr-3.7.1/ipr/content.spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    20227 2023-03-31 16:30:39.000000 ipr-3.7.1/ipr/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15299 2023-03-31 16:30:39.000000 ipr-3.7.1/ipr/ipr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-03-31 16:30:39.000000 ipr-3.7.1/ipr/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:30:39.000000 ipr-3.7.1/ipr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-03-31 16:30:39.000000 ipr-3.7.1/ipr/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-03-31 16:30:39.000000 ipr-3.7.1/ipr/therapeutic_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-03-31 16:30:39.000000 ipr-3.7.1/ipr/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-03-31 16:30:39.000000 ipr-3.7.1/ipr/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:30:49.333495 ipr-3.7.1/ipr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-31 16:30:49.000000 ipr-3.7.1/ipr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-31 16:30:49.000000 ipr-3.7.1/ipr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-31 16:30:49.000000 ipr-3.7.1/ipr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-31 16:30:49.000000 ipr-3.7.1/ipr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-31 16:30:49.000000 ipr-3.7.1/ipr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-31 16:30:49.000000 ipr-3.7.1/ipr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-31 16:30:39.000000 ipr-3.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 16:30:49.333495 ipr-3.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 16:30:39.000000 ipr-3.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:30:49.333495 ipr-3.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:30:39.000000 ipr-3.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-31 16:30:39.000000 ipr-3.7.1/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-03-31 16:30:39.000000 ipr-3.7.1/tests/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-03-31 16:30:39.000000 ipr-3.7.1/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-03-31 16:30:39.000000 ipr-3.7.1/tests/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-03-31 16:30:39.000000 ipr-3.7.1/tests/test_ipr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-03-31 16:30:39.000000 ipr-3.7.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-03-31 16:30:39.000000 ipr-3.7.1/tests/test_probe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-03-31 16:30:39.000000 ipr-3.7.1/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-31 16:30:39.000000 ipr-3.7.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-31 16:30:39.000000 ipr-3.7.1/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:25:21.828331 ipr-3.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-19 23:25:08.000000 ipr-3.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 23:25:08.000000 ipr-3.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-19 23:25:21.828331 ipr-3.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-19 23:25:08.000000 ipr-3.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:25:21.828331 ipr-3.8.0/ipr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50360 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/content.spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20267 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/ipr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/therapeutic_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:25:21.828331 ipr-3.8.0/ipr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-19 23:25:21.000000 ipr-3.8.0/ipr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-19 23:25:21.000000 ipr-3.8.0/ipr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-19 23:25:21.000000 ipr-3.8.0/ipr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 23:25:21.000000 ipr-3.8.0/ipr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-19 23:25:21.000000 ipr-3.8.0/ipr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 23:25:21.000000 ipr-3.8.0/ipr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-19 23:25:08.000000 ipr-3.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-19 23:25:21.828331 ipr-3.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:25:08.000000 ipr-3.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:25:21.828331 ipr-3.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_ipr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_probe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/util.py
```

### Comparing `ipr-3.7.1/LICENSE` & `ipr-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/PKG-INFO` & `ipr-3.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipr
-Version: 3.7.1
+Version: 3.8.0
 Author: ipr
 Author-email: ipr@bcgsc.ca
 Maintainer: ipr
 Maintainer-email: ipr@bcgsc.ca
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: deploy
```

### Comparing `ipr-3.7.1/README.md` & `ipr-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/ipr/annotate.py` & `ipr-3.8.0/ipr/annotate.py`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/ipr/connection.py` & `ipr-3.8.0/ipr/connection.py`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/ipr/content.spec.json` & `ipr-3.8.0/ipr/content.spec.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999457427003723%*

 * *Differences: {"'properties'": "{'copyVariants': {'items': {'properties': {'size': OrderedDict([('description', "*

 * *                 "'size of the copy change segment in the chromosome'), ('type', ['number', "*

 * *                 "'null'])])}}}, 'hlaTypes': {'items': {'properties': {'library': "*

 * *                 "OrderedDict([('description', 'Library id string'), ('example', 'P01234'), "*

 * *                 "('type', ['string', 'null'])])}}}, 'smallMutations': {'items': {'properties': "*

 * *                 "{'tumourAltCopies': Orde […]*

```diff
@@ -186,14 +186,21 @@
                         ]
                     },
                     "lohState": {
                         "description": "the loss-of-heterozygosity category for this gene region",
                         "example": "HET",
                         "type": "string"
                     },
+                    "size": {
+                        "description": "size of the copy change segment in the chromosome",
+                        "type": [
+                            "number",
+                            "null"
+                        ]
+                    },
                     "start": {
                         "description": "the genomic start position of the copy segment this gene copy number was called from",
                         "type": [
                             "integer",
                             "null"
                         ]
                     }
@@ -498,14 +505,22 @@
                         "type": "string"
                     },
                     "c2": {
                         "example": "C*07:02",
                         "pattern": "^C\\*[0-9]+:[0-9]+$",
                         "type": "string"
                     },
+                    "library": {
+                        "description": "Library id string",
+                        "example": "P01234",
+                        "type": [
+                            "string",
+                            "null"
+                        ]
+                    },
                     "pathology": {
                         "description": "the disease state of this sample",
                         "example": "normal",
                         "type": "string"
                     },
                     "protocol": {
                         "description": "the sequencing protocol used for ths sample",
@@ -989,14 +1004,22 @@
                         "description": "the transcript name",
                         "example": "ENST00001.2",
                         "type": [
                             "string",
                             "null"
                         ]
                     },
+                    "tumourAltCopies": {
+                        "description": "the number of gene copies in the tumour genome supporting the mutation",
+                        "example": 1,
+                        "type": [
+                            "integer",
+                            "null"
+                        ]
+                    },
                     "tumourAltCount": {
                         "description": "the number of alternate reads in the tumour genome supporting the mutation",
                         "example": 1,
                         "type": [
                             "integer",
                             "null"
                         ]
@@ -1005,14 +1028,22 @@
                         "description": "the total number of reads at this position in the tumour genome, if not given this will be inferred based on the ref and alt count sum",
                         "example": 2,
                         "type": [
                             "integer",
                             "null"
                         ]
                     },
+                    "tumourRefCopies": {
+                        "description": "the number of wildtype gene copies in tumour genome",
+                        "example": 1,
+                        "type": [
+                            "integer",
+                            "null"
+                        ]
+                    },
                     "tumourRefCount": {
                         "description": "the number of reference reads in the tumour genome",
                         "example": 1,
                         "type": [
                             "integer",
                             "null"
                         ]
@@ -1095,14 +1126,22 @@
                         "description": "the 3' (c-terminal) exon",
                         "example": 2,
                         "type": [
                             "integer",
                             "null"
                         ]
                     },
+                    "frame": {
+                        "description": "Optional descriptive string for in-frame vs frame-shift SV",
+                        "example": "frame-shift",
+                        "type": [
+                            "string",
+                            "null"
+                        ]
+                    },
                     "gene1": {
                         "description": "the 5' (n-terminal) gene name",
                         "example": "EWSR1",
                         "pattern": "^((\\w|-)+)?$",
                         "type": "string"
                     },
                     "gene2": {
@@ -1129,14 +1168,23 @@
                         "description": "Library id string",
                         "example": "P01234",
                         "type": [
                             "string",
                             "null"
                         ]
                     },
+                    "mavis_product_id": {
+                        "default": null,
+                        "description": "mavis product id / other tool description strings",
+                        "example": "MAVIS-2.5.35-RT3556GHTR",
+                        "type": [
+                            "string",
+                            "null"
+                        ]
+                    },
                     "ntermTranscript": {
                         "default": null,
                         "description": "the 3' transcript name",
                         "example": "ENST0001.2",
                         "type": [
                             "string",
                             "null"
@@ -1158,14 +1206,30 @@
                     },
                     "svgTitle": {
                         "description": "The title to accompany this SV",
                         "type": [
                             "string",
                             "null"
                         ]
+                    },
+                    "tumourAltCount": {
+                        "description": "the number of alternate reads in the tumour genome supporting the mutation",
+                        "example": 1,
+                        "type": [
+                            "integer",
+                            "null"
+                        ]
+                    },
+                    "tumourDepth": {
+                        "description": "the total number of reads at this position in the tumour genome",
+                        "example": 2,
+                        "type": [
+                            "integer",
+                            "null"
+                        ]
                     }
                 },
                 "required": [
                     "eventType",
                     "breakpoint",
                     "gene1",
                     "gene2",
```

### Comparing `ipr-3.7.1/ipr/inputs.py` & `ipr-3.8.0/ipr/inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,14 +138,16 @@
     'omicSupport',
     'highQuality',
     'comments',
     'library',
     # GERO-307 - tumourAltCount and tumourDepth are available but not rnaAltCount and rnaDepth
     'tumourAltCount',
     'tumourDepth',
+    'germline',
+    'mavis_product_id',
 ]
 
 
 def validate_variant_rows(
     rows: Iterable[Dict], required: List[str], optional: List[str], row_to_key: Callable
 ) -> List[IprVariant]:
     """
```

### Comparing `ipr-3.7.1/ipr/ipr.py` & `ipr-3.8.0/ipr/ipr.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,43 +4,29 @@
 """
 from graphkb import GraphKBConnection
 from graphkb import statement as gkb_statement
 from graphkb import vocab as gkb_vocab
 from graphkb.types import Record
 from typing import Dict, Iterable, List, Sequence, Set, Tuple
 
-from .constants import APPROVED_EVIDENCE_LEVELS, GERMLINE_BASE_TERMS, VARIANT_CLASSES
+from .constants import GERMLINE_BASE_TERMS, VARIANT_CLASSES
 from .types import GkbStatement, ImageDefinition, IprFusionVariant, IprGene, IprVariant, KbMatch
 from .util import convert_to_rid_set, find_variant, logger
 
 
 def display_evidence_levels(statement: GkbStatement) -> str:
     result = []
     for evidence_level in statement.get('evidenceLevel', []) or []:
         if isinstance(evidence_level, str):
             result.append(evidence_level)
         elif 'displayName' in evidence_level:
             result.append(evidence_level['displayName'])
     return ';'.join(sorted(result))
 
 
-def get_approved_evidence_levels(graphkb_conn: GraphKBConnection) -> List[Record]:
-    filters = []
-    for source, names in APPROVED_EVIDENCE_LEVELS.items():
-        filters.append(
-            {
-                'AND': [
-                    {'source': {'target': 'Source', 'filters': {'name': source}}},
-                    {'name': names, 'operator': 'IN'},
-                ]
-            }
-        )
-    return graphkb_conn.query({'target': 'EvidenceLevel', 'filters': {'OR': filters}})
-
-
 def filter_structural_variants(
     structural_variants: List[IprFusionVariant],
     kb_matches: List[KbMatch],
     gene_annotations: List[IprGene],
 ) -> List[IprFusionVariant]:
     """
     Filter structural variants to remove non-high quality events unless they are matched/annotated or
@@ -82,15 +68,15 @@
     # Map EvidenceLevel RIDs to list of incoming CrossReferenceOf
     evidence_levels_mapping = dict(
         map(lambda d: (d["@rid"], d.get("in_CrossReferenceOf", [])), evidence_levels)
     )
 
     # Filter IPR EvidenceLevel and map each outgoing CrossReferenceOf to displayName
     ipr_source_rid = graphkb_conn.get_source("ipr")["@rid"]
-    ipr_evidence_levels = filter(lambda d: d["source"] == ipr_source_rid, evidence_levels)
+    ipr_evidence_levels = filter(lambda d: d.get("source") == ipr_source_rid, evidence_levels)
     cross_references_mapping: Dict[str, str] = dict()
     ipr_rids_to_displayname = dict()
     for level in ipr_evidence_levels:
         d = map(lambda i: (i, level["displayName"]), level.get("out_CrossReferenceOf", []))
         cross_references_mapping.update(d)
         ipr_rids_to_displayname[level["@rid"]] = level["displayName"]
 
@@ -137,17 +123,17 @@
         for r in gkb_vocab.get_term_tree(graphkb_conn, disease_name, ontology_class='Disease')
     }
 
     if not disease_matches:
         raise ValueError(f'failed to match disease ({disease_name}) to graphkb')
 
     rows = []
-
-    approved = convert_to_rid_set(get_approved_evidence_levels(graphkb_conn))
     ev_map = get_evidencelevel_mapping(graphkb_conn)
+    # GERO-318 - add all IPR-A evidence equivalents to the approvedTherapy flag
+    approved = set([ev for (ev, ipr) in ev_map.items() if ipr == 'IPR-A'])
 
     for statement in statements:
         variants = [c for c in statement['conditions'] if c['@class'] in VARIANT_CLASSES]
         diseases = [c for c in statement['conditions'] if c['@class'] == 'Disease']
         disease_match = len(diseases) == 1 and diseases[0]['@rid'] in disease_matches
         pmid = ';'.join([e['displayName'] for e in statement['evidence']])
```

### Comparing `ipr-3.7.1/ipr/main.py` & `ipr-3.8.0/ipr/main.py`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/ipr/summary.py` & `ipr-3.8.0/ipr/summary.py`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/ipr/therapeutic_options.py` & `ipr-3.8.0/ipr/therapeutic_options.py`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/ipr/types.py` & `ipr-3.8.0/ipr/types.py`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/ipr/util.py` & `ipr-3.8.0/ipr/util.py`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/ipr.egg-info/PKG-INFO` & `ipr-3.8.0/ipr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipr
-Version: 3.7.1
+Version: 3.8.0
 Author: ipr
 Author-email: ipr@bcgsc.ca
 Maintainer: ipr
 Maintainer-email: ipr@bcgsc.ca
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: deploy
```

### Comparing `ipr-3.7.1/ipr.egg-info/SOURCES.txt` & `ipr-3.8.0/ipr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/setup.cfg` & `ipr-3.8.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 line_length = 100
 multi_line_output = 3
 include_trailing_comma = true
 known_standard_library = requests
 
 [metadata]
 name = ipr
-version = 3.7.1
+version = 3.8.0
 author_email = ipr@bcgsc.ca
 author = ipr
 maintainer_email = ipr@bcgsc.ca
 maintainer = ipr
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `ipr-3.7.1/tests/test_annotate.py` & `ipr-3.8.0/tests/test_annotate.py`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/tests/test_connection.py` & `ipr-3.8.0/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/tests/test_inputs.py` & `ipr-3.8.0/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/tests/test_ipr.py` & `ipr-3.8.0/tests/test_ipr.py`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/tests/test_main.py` & `ipr-3.8.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/tests/test_probe.py` & `ipr-3.8.0/tests/test_probe.py`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/tests/test_summary.py` & `ipr-3.8.0/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `ipr-3.7.1/tests/test_util.py` & `ipr-3.8.0/tests/test_util.py`

 * *Files identical despite different names*

