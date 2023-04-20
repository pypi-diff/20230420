# Comparing `tmp/bconv-1.2.0.tar.gz` & `tmp/bconv-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bconv-1.2.0.tar", last modified: Mon May 24 09:29:08 2021, max compression
+gzip compressed data, was "bconv-1.2.1.tar", max compression
```

## Comparing `bconv-1.2.0.tar` & `bconv-1.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1068 2020-02-02 22:08:00.037564 bconv-1.2.0/LICENSE
--rw-r--r--   0        0        0     3347 2021-05-24 09:20:53.226240 bconv-1.2.0/README.md
--rw-r--r--   0        0        0      244 2021-05-24 09:20:53.226240 bconv-1.2.0/bconv/__init__.py
--rw-r--r--   0        0        0        0 2018-08-24 06:57:40.988318 bconv-1.2.0/bconv/doc/__init__.py
--rw-r--r--   0        0        0    22589 2021-05-24 08:52:59.624455 bconv-1.2.0/bconv/doc/document.py
--rw-r--r--   0        0        0     4188 2021-03-15 23:05:39.893824 bconv-1.2.0/bconv/fmt/__init__.py
--rw-r--r--   0        0        0     4008 2021-05-24 08:54:34.893346 bconv-1.2.0/bconv/fmt/_export.py
--rw-r--r--   0        0        0     2376 2021-02-12 11:56:55.261744 bconv-1.2.0/bconv/fmt/_load.py
--rw-r--r--   0        0        0    19298 2021-05-24 08:54:34.897346 bconv-1.2.0/bconv/fmt/bioc.py
--rw-r--r--   0        0        0     5612 2021-05-24 08:54:34.897346 bconv-1.2.0/bconv/fmt/brat.py
--rw-r--r--   0        0        0     8579 2021-05-24 08:54:34.897346 bconv-1.2.0/bconv/fmt/conll.py
--rw-r--r--   0        0        0     5553 2021-05-24 08:54:34.897346 bconv-1.2.0/bconv/fmt/csv_.py
--rw-r--r--   0        0        0     4424 2021-05-24 08:54:34.897346 bconv-1.2.0/bconv/fmt/europepmc.py
--rw-r--r--   0        0        0    11336 2021-05-24 08:54:34.897346 bconv-1.2.0/bconv/fmt/pubanno.py
--rw-r--r--   0        0        0    10191 2021-03-15 23:00:21.287319 bconv-1.2.0/bconv/fmt/pubmed.py
--rw-r--r--   0        0        0     7494 2021-05-24 08:54:34.897346 bconv-1.2.0/bconv/fmt/pubtator.py
--rw-r--r--   0        0        0     5242 2021-03-15 23:00:52.647539 bconv-1.2.0/bconv/fmt/txt.py
--rw-r--r--   0        0        0        0 2018-08-24 06:57:40.988318 bconv-1.2.0/bconv/nlp/__init__.py
--rw-r--r--   0        0        0     2131 2021-02-12 11:56:55.253744 bconv-1.2.0/bconv/nlp/tokenize.py
--rw-r--r--   0        0        0        0 2018-08-24 06:57:41.016319 bconv-1.2.0/bconv/util/__init__.py
--rw-r--r--   0        0        0     3461 2021-01-06 14:53:39.646170 bconv-1.2.0/bconv/util/iterate.py
--rw-r--r--   0        0        0     2832 2020-05-24 18:55:26.254928 bconv-1.2.0/bconv/util/misc.py
--rw-r--r--   0        0        0     1826 2021-03-15 23:04:55.645359 bconv-1.2.0/bconv/util/stream.py
--rw-r--r--   0        0        0      488 2021-05-24 09:20:53.226240 bconv-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4138 2021-05-24 09:29:08.221896 bconv-1.2.0/setup.py
--rw-r--r--   0        0        0     4108 2021-05-24 09:29:08.222395 bconv-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2020-02-02 22:08:00.037564 bconv-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3347 2021-05-24 09:20:53.226240 bconv-1.2.1/README.md
+-rw-r--r--   0        0        0      244 2023-04-20 21:02:01.582351 bconv-1.2.1/bconv/__init__.py
+-rw-r--r--   0        0        0        0 2018-08-24 06:57:40.988318 bconv-1.2.1/bconv/doc/__init__.py
+-rw-r--r--   0        0        0    22589 2021-05-24 08:52:59.624455 bconv-1.2.1/bconv/doc/document.py
+-rw-r--r--   0        0        0     4188 2021-03-15 23:05:39.893824 bconv-1.2.1/bconv/fmt/__init__.py
+-rw-r--r--   0        0        0     4008 2021-05-24 08:54:34.893346 bconv-1.2.1/bconv/fmt/_export.py
+-rw-r--r--   0        0        0     2376 2021-02-12 11:56:55.261744 bconv-1.2.1/bconv/fmt/_load.py
+-rw-r--r--   0        0        0    19320 2023-04-20 20:55:56.104623 bconv-1.2.1/bconv/fmt/bioc.py
+-rw-r--r--   0        0        0     5612 2021-05-24 08:54:34.897346 bconv-1.2.1/bconv/fmt/brat.py
+-rw-r--r--   0        0        0     8579 2021-05-24 08:54:34.897346 bconv-1.2.1/bconv/fmt/conll.py
+-rw-r--r--   0        0        0     5553 2021-05-24 08:54:34.897346 bconv-1.2.1/bconv/fmt/csv_.py
+-rw-r--r--   0        0        0     4424 2021-05-24 08:54:34.897346 bconv-1.2.1/bconv/fmt/europepmc.py
+-rw-r--r--   0        0        0    11336 2021-05-24 08:54:34.897346 bconv-1.2.1/bconv/fmt/pubanno.py
+-rw-r--r--   0        0        0    10191 2021-03-15 23:00:21.287319 bconv-1.2.1/bconv/fmt/pubmed.py
+-rw-r--r--   0        0        0     7494 2021-05-24 08:54:34.897346 bconv-1.2.1/bconv/fmt/pubtator.py
+-rw-r--r--   0        0        0     5242 2021-03-15 23:00:52.647539 bconv-1.2.1/bconv/fmt/txt.py
+-rw-r--r--   0        0        0        0 2018-08-24 06:57:40.988318 bconv-1.2.1/bconv/nlp/__init__.py
+-rw-r--r--   0        0        0     2131 2021-02-12 11:56:55.253744 bconv-1.2.1/bconv/nlp/tokenize.py
+-rw-r--r--   0        0        0        0 2018-08-24 06:57:41.016319 bconv-1.2.1/bconv/util/__init__.py
+-rw-r--r--   0        0        0     3461 2021-01-06 14:53:39.646170 bconv-1.2.1/bconv/util/iterate.py
+-rw-r--r--   0        0        0     2832 2020-05-24 18:55:26.254928 bconv-1.2.1/bconv/util/misc.py
+-rw-r--r--   0        0        0     1826 2021-03-15 23:04:55.645359 bconv-1.2.1/bconv/util/stream.py
+-rw-r--r--   0        0        0      490 2023-04-20 21:02:12.990279 bconv-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4142 1970-01-01 00:00:00.000000 bconv-1.2.1/setup.py
+-rw-r--r--   0        0        0     4160 1970-01-01 00:00:00.000000 bconv-1.2.1/PKG-INFO
```

### Comparing `bconv-1.2.0/LICENSE` & `bconv-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/README.md` & `bconv-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/doc/document.py` & `bconv-1.2.1/bconv/doc/document.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/fmt/__init__.py` & `bconv-1.2.1/bconv/fmt/__init__.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/fmt/_export.py` & `bconv-1.2.1/bconv/fmt/_export.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/fmt/_load.py` & `bconv-1.2.1/bconv/fmt/_load.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/fmt/bioc.py` & `bconv-1.2.1/bconv/fmt/bioc.py`

 * *Files 1% similar despite different names*

```diff
@@ -597,15 +597,16 @@
         return unit.start
 
     @staticmethod
     def entity(entity):
         """
         Calculate start and length of this annotation.
         """
-        return entity.start, entity.end-entity.start
+        for start, end in entity.spans:
+            yield start, end-start
 
     # Aliases for backward compatibility.
     def passage(self, unit):
         """New passage/section: get the start offset."""
         return self.start(unit)
 
     def sentence(self, unit):
```

### Comparing `bconv-1.2.0/bconv/fmt/brat.py` & `bconv-1.2.1/bconv/fmt/brat.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/fmt/conll.py` & `bconv-1.2.1/bconv/fmt/conll.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/fmt/csv_.py` & `bconv-1.2.1/bconv/fmt/csv_.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/fmt/europepmc.py` & `bconv-1.2.1/bconv/fmt/europepmc.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/fmt/pubanno.py` & `bconv-1.2.1/bconv/fmt/pubanno.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/fmt/pubmed.py` & `bconv-1.2.1/bconv/fmt/pubmed.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/fmt/pubtator.py` & `bconv-1.2.1/bconv/fmt/pubtator.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/fmt/txt.py` & `bconv-1.2.1/bconv/fmt/txt.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/nlp/tokenize.py` & `bconv-1.2.1/bconv/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/util/iterate.py` & `bconv-1.2.1/bconv/util/iterate.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/util/misc.py` & `bconv-1.2.1/bconv/util/misc.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/bconv/util/stream.py` & `bconv-1.2.1/bconv/util/stream.py`

 * *Files identical despite different names*

### Comparing `bconv-1.2.0/setup.py` & `bconv-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['lxml>=4.3,<5.0', 'nltk>=3.4,<4.0']
 
 setup_kwargs = {
     'name': 'bconv',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': 'Convert between BioNLP formats',
     'long_description': "# `bconv`: Python library for converting between BioNLP formats\n\n`bconv` offers format conversion and manipulation of documents with text and annotations.\nIt supports various popular formats used in natural-language processing for biomedical texts.\n\n\n## Supported formats\n\nThe following formats are currently supported:\n\n| Name                               | I | O | T | A | Description |\n| ---------------------------------- | - | - | - | - | ----------- |\n| `bioc_xml`, `bioc_json`            | ✓ | ✓ | ✓ | ✓ | [BioC][1] |\n| `bionlp`                           |   | ✓ |   | ✓ | [BioNLP stand-off][2] |\n| `brat`                             |   | ✓ |   | ✓ | [brat stand-off][2] |\n| `conll`                            | ✓ | ✓ | ✓ | ✓ | [CoNLL][3] |\n| `europepmc`, `europepmc.zip`       |   | ✓ |   | ✓ | [Europe-PMC JSON][4] |\n| `pubtator`, `pubtator_fbk`         | ✓ | ✓ | ✓ | ✓ | [PubTator][5] |\n| `pubmed`, `pxml`                   | ✓ |   | ✓ |   | [PubMed abstracts][6] |\n| `pmc`, `nxml`                      | ✓ |   | ✓ |   | [PMC full-text][6] |\n| `pubanno_json`, `pubanno_json.tgz` | ✓ | ✓ | ✓ | ✓ | [PubAnnotation JSON][7] |\n| `csv`, `tsv`                       |   | ✓ |   | ✓ | [comma/tab-separated values][8] |\n| `text_csv`, `text_tsv`             |   | ✓ | ✓ | ✓ | [comma/tab-separated values][8] |\n| `txt`                              | ✓ | ✓ | ✓ |   | [plain text][9] |\n| `txt.json`                         | ✓ | ✓ | ✓ |   | [collection of plain-text documents][9] |\n\n**I**: input format;\n**O**: output format;\n**T**: can represent text;\n**A**: can represent annotations (entities).\n\n[1]: https://github.com/lfurrer/bconv/wiki/BioC\n[2]: https://github.com/lfurrer/bconv/wiki/Brat\n[3]: https://github.com/lfurrer/bconv/wiki/CoNLL\n[4]: https://github.com/lfurrer/bconv/wiki/EuropePMC\n[5]: https://github.com/lfurrer/bconv/wiki/PubTator\n[6]: https://github.com/lfurrer/bconv/wiki/PubMed\n[7]: https://github.com/lfurrer/bconv/wiki/PubAnnotation\n[8]: https://github.com/lfurrer/bconv/wiki/CSV\n[9]: https://github.com/lfurrer/bconv/wiki/TXT\n\n\n## Installation\n\n`bconv` is hosted on [PyPI](https://pypi.org/project/bconv/), so you can use `pip` to install it:\n```sh\n$ pip install bconv\n```\n\n\n## Usage\n\nLoad an annotated collection in BioC XML format:\n```pycon\n>>> import bconv\n>>> coll = bconv.load('path/to/example.xml', fmt='bioc_xml')\n>>> coll\n<Collection with 37 documents at 0x7f1966e4b3c8>\n```\nA Collection is a sequence of Document objects:\n```pycon\n>>> coll[0]\n<Document with 12 sections at 0x7f1966e2f6d8>\n```\nDocuments contain Sections, which contain Sentences:\n```pycon\n>>> sent = coll[0][3][5]\n>>> sent.text\n'A Live cell imaging reveals that expression of GFP‐KSHV‐TK, but not GFP induces contraction of HeLa cells.'\n```\nFind the first annotation for this sentence:\n```pycon\n>>> e = next(sent.iter_entities())\n>>> e.start, e.end, e.text\n(571, 578, 'KSHV‐TK')\n>>> e.metadata\n{'type': 'gene/protein', 'ui': 'Uniprot:F5HB62'}\n```\nWrite the whole collection to a new file in CoNLL format:\n```pycon\n>>> with open('path/to/example.conll', 'w', encoding='utf8') as f:\n...     bconv.dump(coll, f, fmt='conll', tagset='IOBES', include_offsets=True)\n```\n\n\n## Documentation\n\n`bconv` is documented in the [GitHub wiki](https://github.com/lfurrer/bconv/wiki).\n",
     'author': 'Lenz Furrer',
     'author_email': 'lenz.furrer@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/lfurrer/bconv',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `bconv-1.2.0/PKG-INFO` & `bconv-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: bconv
-Version: 1.2.0
+Version: 1.2.1
 Summary: Convert between BioNLP formats
 Home-page: https://github.com/lfurrer/bconv
 License: MIT
 Author: Lenz Furrer
 Author-email: lenz.furrer@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lxml (>=4.3,<5.0)
 Requires-Dist: nltk (>=3.4,<4.0)
 Project-URL: Documentation, https://github.com/lfurrer/bconv/wiki
 Project-URL: Repository, https://github.com/lfurrer/bconv
 Description-Content-Type: text/markdown
 
 # `bconv`: Python library for converting between BioNLP formats
```

