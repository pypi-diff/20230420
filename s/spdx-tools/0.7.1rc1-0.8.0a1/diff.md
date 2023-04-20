# Comparing `tmp/spdx-tools-0.7.1rc1.tar.gz` & `tmp/spdx-tools-0.8.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spdx-tools-0.7.1rc1.tar", last modified: Tue Mar 14 09:29:16 2023, max compression
+gzip compressed data, was "spdx-tools-0.8.0a1.tar", last modified: Thu Apr 20 14:22:18 2023, max compression
```

## Comparing `spdx-tools-0.7.1rc1.tar` & `spdx-tools-0.8.0a1.tar`

### file list

```diff
@@ -1,144 +1,354 @@
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.899496 spdx-tools-0.7.1rc1/
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.890496 spdx-tools-0.7.1rc1/.circleci/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2772 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/.circleci/config.yml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)       34 2022-11-17 08:44:09.000000 spdx-tools-0.7.1rc1/.coveragerc
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      147 2022-11-17 08:44:09.000000 spdx-tools-0.7.1rc1/.editorconfig
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.889496 spdx-tools-0.7.1rc1/.github/
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.891496 spdx-tools-0.7.1rc1/.github/workflows/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1059 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/.github/workflows/install_and_test.yml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      419 2022-11-17 08:44:09.000000 spdx-tools-0.7.1rc1/.gitignore
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2664 2023-01-24 15:58:23.000000 spdx-tools-0.7.1rc1/CHANGELOG.md
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3306 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/CONTRIBUTING.md
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    11356 2022-11-17 08:44:09.000000 spdx-tools-0.7.1rc1/LICENSE
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      360 2022-11-17 08:44:09.000000 spdx-tools-0.7.1rc1/MANIFEST.in
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5577 2023-03-14 09:29:16.899496 spdx-tools-0.7.1rc1/PKG-INFO
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4482 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/README.md
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      549 2022-11-17 08:44:09.000000 spdx-tools-0.7.1rc1/appveyor.yml
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.891496 spdx-tools-0.7.1rc1/examples/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      612 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/examples/__init__.py
--rwxr-xr-x   0 mhuber    (1000) mhuber    (1000)      671 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/examples/pp_rdf.py
--rwxr-xr-x   0 mhuber    (1000) mhuber    (1000)     1179 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/examples/pp_tv.py
--rwxr-xr-x   0 mhuber    (1000) mhuber    (1000)     2009 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/examples/tv_to_rdf.py
--rwxr-xr-x   0 mhuber    (1000) mhuber    (1000)     4123 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/examples/write_tv.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2061 2023-03-03 13:38:16.000000 spdx-tools-0.7.1rc1/pyproject.toml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)       38 2023-03-14 09:29:16.899496 spdx-tools-0.7.1rc1/setup.cfg
--rwxr-xr-x   0 mhuber    (1000) mhuber    (1000)       88 2022-11-17 08:44:09.000000 spdx-tools-0.7.1rc1/setup.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.892496 spdx-tools-0.7.1rc1/spdx/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)       56 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/spdx/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3641 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/annotation.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4001 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/checksum.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.892496 spdx-tools-0.7.1rc1/spdx/cli_tools/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      612 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/cli_tools/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3861 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/cli_tools/convertor.py
--rwxr-xr-x   0 mhuber    (1000) mhuber    (1000)     5310 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/cli_tools/parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2558 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/config.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5268 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/creationinfo.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    11220 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/document.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    19777 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/spdx/exceptions.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     8724 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/file.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6390 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/license.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)   240843 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/spdx/licenses.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    13675 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/package.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.894496 spdx-tools-0.7.1rc1/spdx/parsers/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      615 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1075 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/builderexceptions.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1188 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/jsonparser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    78898 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/jsonyamlxml.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    11227 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/jsonyamlxmlbuilders.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.894496 spdx-tools-0.7.1rc1/spdx/parsers/lexers/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/spdx/parsers/lexers/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     7966 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/lexers/tagvalue.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1884 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/loggers.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1989 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/parse_anything.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    60423 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/rdf.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    23836 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/rdfbuilders.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    73509 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/tagvalue.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    60893 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/tagvaluebuilders.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     8430 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/validations.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2980 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/xmlparser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1193 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/parsers/yamlparser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3509 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/relationship.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2570 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/review.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4908 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/snippet.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6748 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/utils.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1861 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/version.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.894496 spdx-tools-0.7.1rc1/spdx/writers/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/spdx/writers/__init__.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1366 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/writers/json.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    25666 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/writers/jsonyamlxml.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    38054 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/writers/rdf.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    18435 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/writers/tagvalue.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1479 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/writers/write_anything.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1172 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/writers/xml.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1161 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/spdx/writers/yaml.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.895496 spdx-tools-0.7.1rc1/spdx_tools.egg-info/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5577 2023-03-14 09:29:16.000000 spdx-tools-0.7.1rc1/spdx_tools.egg-info/PKG-INFO
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3570 2023-03-14 09:29:16.000000 spdx-tools-0.7.1rc1/spdx_tools.egg-info/SOURCES.txt
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        1 2023-03-14 09:29:16.000000 spdx-tools-0.7.1rc1/spdx_tools.egg-info/dependency_links.txt
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      120 2023-03-14 09:29:16.000000 spdx-tools-0.7.1rc1/spdx_tools.egg-info/entry_points.txt
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        1 2023-01-25 14:42:05.000000 spdx-tools-0.7.1rc1/spdx_tools.egg-info/not-zip-safe
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)       58 2023-03-14 09:29:16.000000 spdx-tools-0.7.1rc1/spdx_tools.egg-info/requires.txt
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        5 2023-03-14 09:29:16.000000 spdx-tools-0.7.1rc1/spdx_tools.egg-info/top_level.txt
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)       93 2022-11-17 08:44:09.000000 spdx-tools-0.7.1rc1/stdeb.cfg
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.896496 spdx-tools-0.7.1rc1/tests/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2022-11-17 08:44:09.000000 spdx-tools-0.7.1rc1/tests/__init__.py
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.889496 spdx-tools-0.7.1rc1/tests/data/
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.896496 spdx-tools-0.7.1rc1/tests/data/doc_parse/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6061 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/doc_parse/SBOMexpected.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    18610 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/doc_parse/expected.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    18435 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/doc_parse/spdx-expected.json
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.897496 spdx-tools-0.7.1rc1/tests/data/doc_write/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1946 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/json-simple-multi-package.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2201 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/json-simple-plus.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2193 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/json-simple.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      366 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/rdf-mini.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3864 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/rdf-simple-plus.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3833 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/rdf-simple.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      133 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/tv-mini.tv
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1074 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/tv-simple-plus.tv
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1066 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/tv-simple.tv
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2528 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/xml-simple-multi-package.xml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2121 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/xml-simple-plus.xml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2113 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/xml-simple.xml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1475 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/yaml-simple-multi-package.yaml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1243 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/yaml-simple-plus.yaml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1236 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/doc_write/yaml-simple.yaml
-drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-03-14 09:29:16.899496 spdx-tools-0.7.1rc1/tests/data/formats/
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    20805 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXJSONExample-v2.2.spdx.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    21342 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    14182 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXJsonExample.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1566 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXJsonExampleEmptyArrays.json
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    18411 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXRdfExample.rdf
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2921 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXSBOMExample.spdx.yml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2577 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXSBOMExample.tag
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2956 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXSimpleTag.tag
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    18104 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXTagExample-v2.2.spdx
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    18516 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    12922 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXTagExample.tag
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    24020 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXXMLExample-v2.2.spdx.xml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    24755 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    15933 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXXmlExample.xml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    19895 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXYAMLExample-2.2.spdx.yaml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    20429 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXYAMLExample-2.3.spdx.yaml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    13908 2023-03-03 13:11:20.000000 spdx-tools-0.7.1rc1/tests/data/formats/SPDXYamlExample.yaml
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    35107 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_builder.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4424 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_checksum.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2821 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_cli_convertor.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2193 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_config.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    11359 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_conversion.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2547 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_creationinfo.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    25850 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_document.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1230 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_error_messages.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3018 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_jsonyamlxml_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6435 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/test_jsonyamlxml_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1266 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_package.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1437 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_parse_anything.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1398 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_parsers_validation.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1886 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_rdf_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4371 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_rdf_writer.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    23188 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_tag_value_parser.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3682 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/test_write_anything.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    26472 2023-01-25 14:37:33.000000 spdx-tools-0.7.1rc1/tests/testing_utils.LICENSE
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2856 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/testing_utils.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)    20253 2023-03-14 09:22:05.000000 spdx-tools-0.7.1rc1/tests/utils_test.py
--rw-r--r--   0 mhuber    (1000) mhuber    (1000)      940 2023-03-03 13:11:16.000000 spdx-tools-0.7.1rc1/tox.ini
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.469629 spdx-tools-0.8.0a1/
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.447628 spdx-tools-0.8.0a1/.circleci/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      316 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/.circleci/config.yml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      147 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a1/.editorconfig
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      123 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/.flake8
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.447628 spdx-tools-0.8.0a1/.github/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      502 2023-03-29 06:18:21.000000 spdx-tools-0.8.0a1/.github/dependabot.yml
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.447628 spdx-tools-0.8.0a1/.github/workflows/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      772 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/.github/workflows/check_codestyle.yml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1167 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/.github/workflows/install_and_test.yml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      442 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/.gitignore
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3709 2023-03-29 06:18:21.000000 spdx-tools-0.8.0a1/CHANGELOG.md
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4048 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/CONTRIBUTING.md
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    11356 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a1/LICENSE
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      360 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a1/MANIFEST.in
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    11784 2023-04-20 14:22:18.469629 spdx-tools-0.8.0a1/PKG-INFO
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    10830 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/README.md
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      549 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a1/appveyor.yml
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.447628 spdx-tools-0.8.0a1/assets/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)   147064 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/assets/SPDXJSONExample-v2.3.spdx.png
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.448628 spdx-tools-0.8.0a1/examples/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6181 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/examples/spdx2_document_from_scratch.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2181 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/pyproject.toml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)       38 2023-04-20 14:22:18.469629 spdx-tools-0.8.0a1/setup.cfg
+-rwxr-xr-x   0 mhuber    (1000) mhuber    (1000)       88 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a1/setup.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.445628 spdx-tools-0.8.0a1/src/
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.445628 spdx-tools-0.8.0a1/src/spdx_tools/
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.448628 spdx-tools-0.8.0a1/src/spdx_tools/common/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/common/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.448628 spdx-tools-0.8.0a1/src/spdx_tools/common/typing/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/common/typing/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      421 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/common/typing/constructor_type_errors.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2259 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/common/typing/dataclass_with_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1186 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/common/typing/type_checks.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.449628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      507 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/casing_tools.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.449628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/clitools/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/clitools/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4870 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/clitools/pyspdxtools.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      127 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/constants.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      599 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/datetime_conversions.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2309 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/document_utils.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      890 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/formats.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3367 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/graph_generation.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.450628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1334 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/annotation_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      322 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/annotation_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1223 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/checksum_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      269 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/checksum_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3263 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1505 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/creation_info_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      320 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/creation_info_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5260 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/document_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      583 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/document_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1559 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/external_document_ref_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      312 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/external_document_ref_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1363 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/external_package_ref_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      340 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/external_package_ref_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1775 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/extracted_licensing_info_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      346 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/extracted_licensing_info_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3341 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/file_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      619 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/file_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      429 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/json_property.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      449 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/optional_utils.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6050 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/package_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      950 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/package_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1254 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/package_verification_code_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      332 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/package_verification_code_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1286 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/relationship_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      337 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/relationship_properties.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3713 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/snippet_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      511 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/jsonschema/snippet_properties.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.451628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      941 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1068 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/actor.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      849 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/annotation.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      875 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/checksum.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2845 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/document.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      601 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/external_document_ref.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1082 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/extracted_licensing_info.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2711 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/file.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5547 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/package.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2145 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/relationship.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1880 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/relationship_filters.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1896 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/snippet.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      424 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/spdx_no_assertion.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      372 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/spdx_none.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1155 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/version.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.451628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2352 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/actor_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      317 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/error.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.451628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/json/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/json/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      451 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/json/json_parser.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.452628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4930 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/annotation_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1252 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/checksum_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5606 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/creation_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2830 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/dict_parsing_functions.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1576 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/extracted_licensing_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3934 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/file_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3903 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/json_like_dict_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1005 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/license_expression_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     9546 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/package_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     8696 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/relationship_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6292 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/jsonlikedict/snippet_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      511 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/logger.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1477 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/parse_anything.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1155 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/parsing_functions.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.453628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1903 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/annotation_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1517 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/checksum_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5514 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/creation_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2122 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/extracted_licensing_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3751 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/file_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5556 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/graph_parsing_functions.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2814 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/license_expression_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     8924 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/package_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4422 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/rdf_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2482 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/relationship_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6398 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/rdf/snippet_parser.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.453628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5259 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/helper_methods.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6949 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/lexer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    29288 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      388 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/tagvalue_parser.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.453628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/xml/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/xml/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2082 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/xml/xml_parser.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.453628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/yaml/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/yaml/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      457 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/yaml/yaml_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/py.typed
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.453628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/rdfschema/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/rdfschema/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      368 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/rdfschema/namespace.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.454628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1019 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/actor_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1244 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/annotation_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2729 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/checksum_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1692 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/creation_info_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4741 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/document_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1926 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/external_document_ref_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4664 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/external_package_ref_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1936 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/extracted_licensing_info_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3385 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/file_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2893 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/license_expression_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6514 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/package_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1281 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/package_verification_code_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1948 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/relationship_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3988 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/snippet_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3916 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/spdx_id_validators.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1427 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/uri_validators.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1038 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/validation/validation_message.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.454628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.454628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/json/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/json/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1474 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/json/json_writer.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.455628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1520 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/annotation_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1009 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/checksum_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2006 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/creation_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      991 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/external_document_ref_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1664 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/extracted_licensing_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2309 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/file_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3979 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/license_expression_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6537 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/package_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3026 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/rdf_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2001 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/relationship_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3246 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/snippet_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2257 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/rdf/writer_utils.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.456628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1319 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/annotation_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1485 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/checksum_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2452 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/creation_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1382 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/extracted_licensing_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2004 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/file_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4391 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/package_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1205 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/relationship_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1809 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/snippet_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4792 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4351 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/tagvalue/tagvalue_writer_helper_functions.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1184 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/write_anything.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.456628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/xml/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/xml/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1523 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/xml/xml_writer.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.456628 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/yaml/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/yaml/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1480 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/src/spdx_tools/spdx/writer/yaml/yaml_writer.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.469629 spdx-tools-0.8.0a1/src/spdx_tools.egg-info/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    14412 2023-04-20 14:22:18.000000 spdx-tools-0.8.0a1/src/spdx_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)       93 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a1/stdeb.cfg
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.456628 spdx-tools-0.8.0a1/tests/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2022-11-17 08:44:09.000000 spdx-tools-0.8.0a1/tests/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.457628 spdx-tools-0.8.0a1/tests/spdx/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.462628 spdx-tools-0.8.0a1/tests/spdx/data/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    20805 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXJSONExample-v2.2.spdx.json
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    21342 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1141 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXLite.spdx
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)   338588 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXRdfExample-v2.2.spdx.rdf.xml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)   342594 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    18104 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXTagExample-v2.2.spdx
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    18538 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    24020 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXXMLExample-v2.2.spdx.xml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    24884 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    19895 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXYAMLExample-v2.2.spdx.yaml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    20504 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/data/SPDXYAMLExample-v2.3.spdx.yaml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    10534 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/fixtures.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.463628 spdx-tools-0.8.0a1/tests/spdx/jsonschema/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1965 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_annotation_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1334 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_checksum_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2332 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2674 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_creation_info_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    10012 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_document_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2361 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_external_document_ref_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2020 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_external_package_ref_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3621 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_extracted_licensing_info_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     9534 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_file_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    15912 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_package_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2309 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_package_verification_code_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2722 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_relationship_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     8572 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/jsonschema/test_snippet_converter.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      601 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/mock_utils.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.464629 spdx-tools-0.8.0a1/tests/spdx/model/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/model/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1764 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_actor.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1762 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_annotation.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      592 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_checksum.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4008 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_creation_info.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3173 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_document.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1028 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_external_document_ref.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1210 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_external_package_reference.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1230 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_extracted_licensing_info.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4258 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_file.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     7323 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_package.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      666 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_package_verification_code.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1105 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_relationship.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3087 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_snippet.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      827 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/model/test_version.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.464629 spdx-tools-0.8.0a1/tests/spdx/parser/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/parser/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.464629 spdx-tools-0.8.0a1/tests/spdx/parser/all_formats/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/parser/all_formats/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2146 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/all_formats/test_parse_from_file.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.465628 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6439 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_annotation_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1587 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_checksum_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4968 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_creation_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1582 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_dict_parsing_functions.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3004 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_extracted_licensing_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     7138 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_file_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1560 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_license_expression_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    13446 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_package_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     8057 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_relationship_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5605 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_snippet_parser.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.465628 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.465628 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/data/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    13653 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/data/file_to_test_rdf_parser.rdf.xml
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1173 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_annotation_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2960 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_checksum_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3506 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_creation_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2258 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_extracted_licensing_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1575 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_file_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1314 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_graph_parsing_function.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1987 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_license_expression_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4256 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_package_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2492 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_relationship_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6750 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_snippet_parser.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.466629 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3016 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_annotation_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5452 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_creation_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3720 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_extracted_licensing_info_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2805 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_file_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5014 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_helper_methods.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6118 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_package_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2572 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_relationship_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     3489 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_snippet_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    16856 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_tag_value_lexer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2945 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_tag_value_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1875 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/test_actor_parser.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      788 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/test_casing_tools.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1286 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/test_cli.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      986 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/test_datetime_conversions.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4798 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/test_document_utils.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5244 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/test_graph_generation.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.467629 spdx-tools-0.8.0a1/tests/spdx/validation/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/validation/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1281 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_actor_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1415 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_annotation_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    12050 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_checksum_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1663 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_creation_info_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5938 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_document_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      639 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_external_document_ref_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)    13202 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_external_package_ref_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1675 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_extracted_licensing_info_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2443 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_file_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5644 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_license_expression_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5572 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_package_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1924 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_package_verification_code_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2937 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_relationship_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2596 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_snippet_validator.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     6481 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_spdx_id_validators.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5523 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/validation/test_uri_validators.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.467629 spdx-tools-0.8.0a1/tests/spdx/writer/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/writer/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.467629 spdx-tools-0.8.0a1/tests/spdx/writer/json/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/writer/json/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.467629 spdx-tools-0.8.0a1/tests/spdx/writer/json/expected_results/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/writer/json/expected_results/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5745 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/writer/json/expected_results/expected.json
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1400 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/json/test_json_writer.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.468629 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/__init__.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1133 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_annotation_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2419 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_checksum_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1573 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_creation_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1036 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_external_document_ref_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1307 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_extracted_licensing_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1612 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_file_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2719 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_license_expression_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     5264 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_package_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      632 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_rdf_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      942 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_relationship_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2340 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_snippet_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)      874 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/rdf/test_writer_utils.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.469629 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)        0 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/__init__.py
+drwxr-xr-x   0 mhuber    (1000) mhuber    (1000)        0 2023-04-20 14:22:18.469629 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/expected_results/
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1306 2023-04-17 14:07:29.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/expected_results/expected_tag_value.spdx
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1018 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_annotation_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1227 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_checksum_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2729 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_creation_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1165 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_extracted_licensing_info_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1617 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_file_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2905 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_package_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1537 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_relationship_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     1552 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_snippet_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     4996 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_tagvalue_writer.py
+-rw-r--r--   0 mhuber    (1000) mhuber    (1000)     2419 2023-04-20 13:58:41.000000 spdx-tools-0.8.0a1/tests/spdx/writer/tagvalue/test_tagvalue_writer_helper_functions.py
```

### Comparing `spdx-tools-0.7.1rc1/.github/workflows/install_and_test.yml` & `spdx-tools-0.8.0a1/.github/workflows/install_and_test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 name: Install and Test
 
-on: [ workflow_dispatch, pull_request ]
+on:
+  push:
+    branches:
+      - main
+  pull_request:
+  workflow_dispatch:
 
 jobs:
   install_and_test:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ ubuntu-latest, macos-latest, windows-latest ]
-        python-version: [ "3.7", "3.8", "3.9", "3.10" ]
+        python-version: [ "3.7", "3.8", "3.9", "3.10", "3.11" ]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
@@ -23,10 +28,13 @@
           python -m build -nwx .
           python -m pip install --upgrade ./dist/*.whl
           python -m pip install pytest
         shell: bash
       - name: Run tests
         run: pytest
       - name: Run CLI
-        run: |
-          pyspdxtools_parser --file ./tests/data/formats/SPDXJSONExample-v2.3.spdx.json
-          pyspdxtools_convertor --infile ./tests/data/formats/SPDXTagExample-v2.3.spdx -o temp.json
+        run: pyspdxtools -i ./tests/spdx/data/SPDXJSONExample-v2.3.spdx.json
+
+      - name: Install optional dependencies
+        run: python -m pip install networkx
+      - name: Run tests for graph generation
+        run: pytest tests/spdx/test_graph_generation.py
```

### Comparing `spdx-tools-0.7.1rc1/CHANGELOG.md` & `spdx-tools-0.8.0a1/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,39 @@
 # Changelog
 
+## v0.7.1 (2023-03-14)
+
+### New features and changes
+
+* added GitHub Actions workflow
+* added requirements.txt
+* added uritools for URI validation
+* Python >= 3.7 is now required
+* json/yaml/xml: added support for empty arrays for hasFiles and licenseInfoFromFiles
+* rdf: fixed writing of multiple packages
+* tag-value: enhanced parsing of snippet ranges to not mix it up with package version
+* tag-value: fixed parsing of whitespaces
+* tag-value: duplicates in LicenseInfoInFile are now removed during writing
+* account for supplier and originator to be NOASSERTION
+* checksum validation now requires lowercase values
+* during writing of a file, the encoding can be set (default is utf-8)
+* license list updated to version 3.20
+
+### Contributors
+
+This release was made possible by the following contributors. Thank you very much!
+
+* Christian Decker @chrisdecker1201
+* Marc-Etienne Vargenau @vargenau
+* John Vandenberg @jayvdb
+* Nicolaus Weidner @nicoweidner
+* Meret Behrens @meretp
+* Armin Tänzer @armintaenzertng
+* Maximilian Huber @maxhbr
+
 
 ## v0.7.0 (2022-12-08)
 
 Starting a Changelog.
 
 ### New features and changes
```

### Comparing `spdx-tools-0.7.1rc1/CONTRIBUTING.md` & `spdx-tools-0.8.0a1/CONTRIBUTING.md`

 * *Files 24% similar despite different names*

```diff
@@ -30,44 +30,57 @@
    and optionally follow the further steps described to sync your fork and the original repository.
 
 4. Create a new branch in your fork and set up environment:
    ```sh
    git checkout -b fix-or-improve-something
    python -m venv ./venv
    ./venv/bin/activate
-   pip install -e .
+   pip install -e ".[development]"
    ```
+   Note: By using the group `[development]` for the installation, all dependencies (including optional ones) will be 
+   installed. This way we make sure that all tests are executed. 
 5. Make some changes and commit them to the branch:
    ```sh
    git commit --signoff -m 'description of my changes'
    ```
 
    #### Licensing
 
    Please sign off in each of your commits that you license your contributions under the terms
    of [the Developer Certificate of Origin](https://developercertificate.org/). Git has utilities for signing off on
    commits: `git commit -s` or `--signoff` signs a current commit, and `git rebase --signoff <revision-range>`
    retroactively signs a range of past commits.
-
 6. Test your changes:
    ```sh
-   python setup.py test # in the repo root
+   pytest -vvs # in the repo root
    ```
-   You may use other test runners, such as `pytest` or `nose` at your preference.
-7. Push the branch to your fork on GitHub:
+
+7. Check your code style. When opening a pull request, your changes will automatically be checked with `isort`, `black` 
+   and `flake8` to make sure your changes fit with the rest of the code style. 
+    ```sh
+   # run the following commands in the repo root
+   isort src tests 
+   black src tests
+   flake8 src tests 
+   ```
+   `black` and `isort` will automatically format the code and sort the imports. The configuration for these linters 
+   can be found in the `pyproject.toml`. `flake8` lists all problems found which then need to be resolved manually.
+   The configuration for the linter can be found in the `.flake8` file.
+
+8. Push the branch to your fork on GitHub:
    ```sh
    git push origin fix-or-improve-something
    ```
-8. Make a pull request on GitHub.
-9. Continue making more changes and commits on the branch, with `git commit --signoff` and `git push`.
-10. When done, write a comment on the PR asking for a code review.
-11. Some other developer will review your changes and accept your PR. The merge should be done with `rebase`, if
+9. Make a pull request on GitHub.
+10. Continue making more changes and commits on the branch, with `git commit --signoff` and `git push`.
+11. When done, write a comment on the PR asking for a code review.
+12. Some other developer will review your changes and accept your PR. The merge should be done with `rebase`, if
     possible, or with `squash`.
-12. The temporary branch on GitHub should be deleted (there is a button for deleting it).
-13. Delete the local branch as well:
+13. The temporary branch on GitHub should be deleted (there is a button for deleting it).
+14. Delete the local branch as well:
     ```sh
     git checkout master
     git pull -p
     git branch -a
     git branch -d fix-or-improve-something
     ```
```

### Comparing `spdx-tools-0.7.1rc1/LICENSE` & `spdx-tools-0.8.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.7.1rc1/appveyor.yml` & `spdx-tools-0.8.0a1/appveyor.yml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.7.1rc1/pyproject.toml` & `spdx-tools-0.8.0a1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 [build-system]
 requires = ["setuptools>=61.2", "setuptools_scm[toml]>=3.4.3"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spdx-tools"
-authors = [
-    {name = "Ahmed H. Ismail", email = "ahm3d.hisham@gmail.com"},
-    {name = "Armin Tänzer", email = "armin.taenzer@tngtech.com"},
-    {name = "Meret Behrens", email = "meret.behrens@tngtech.com"},
-    {name = "Maximilian Huber", email = "maximilian.huber@tngtech.com"}
-]
+authors = [{ name = "Ahmed H. Ismail", email = "ahm3d.hisham@gmail.com" }]
 maintainers = [
-    {name = "Philippe Ombredanne", email = "pombredanne@gmail.com"},
-    {name = "Maximilian Huber", email = "maximilian.huber@tngtech.com"},
-    {name = "Jeff Licquia", email = "licquia@linuxfoundation.org"},
-    {name = "SPDX group at the Linux Foundation and others"},
+    { name = "Philippe Ombredanne", email = "pombredanne@gmail.com" },
+    { name = "SPDX group at the Linux Foundation and others" },
 ]
-license = {text = "Apache-2.0"}
+license = { text = "Apache-2.0" }
 description = "SPDX parser and tools."
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-urls = {Homepage = "https://github.com/spdx/tools-python"}
+urls = { Homepage = "https://github.com/spdx/tools-python" }
 requires-python = ">=3.7"
-dependencies = ["ply", "rdflib", "click", "pyyaml", "xmltodict", "uritools"]
+dependencies = ["click", "pyyaml", "xmltodict", "rdflib", "typeguard==2.13.3", "uritools", "license_expression", "ply"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = ["pytest"]
+code_style = ["isort", "black", "flake8"]
+graph_generation = ["pygraphviz", "networkx"]
+development = ["black", "flake8", "isort", "networkx", "pytest"]
 
 [project.scripts]
-pyspdxtools_convertor = "spdx.cli_tools.convertor:main"
-pyspdxtools_parser = "spdx.cli_tools.parser:main"
+pyspdxtools = "spdx_tools.spdx.clitools.pyspdxtools:main"
 
 [tool.setuptools]
 zip-safe = false  # because of the uses of __file__: https://github.com/spdx/tools-python/issues/257
 include-package-data = true
 
 [tool.setuptools.packages.find]
-include = ["spdx", "spdx.*"]
+where = ["src"]
+
+[tool.setuptools.package-data]
+"*" = ["py.typed"]
 
+# the default git describe resolves to the tag `python3.6` because the current release tag is not on main
+# by adding "v" the command resolves to the alpha release of 0.7.0 which leads to the desired name spdx-tools-0.7.0
 [tool.setuptools_scm]
-git_describe_command = ["git", "describe", "--dirty", "--tags", "--long", "--match",  "v[0-9]*"]  # `python3.6` tag falsely matches to the default one, clrearly a bug in setuptools_scm
+git_describe_command = ["git", "describe", "--dirty", "--tags", "--long", "--match", "v[0-9]*"]
 
 [tool.aliases]
 release = "clean --all sdist --formats=gztar bdist_wheel"
+
+[tool.black]
+line-length = 119
+include = "(^/src/.*.py|^/tests/.*.py)"
+
+[tool.isort]
+profile = "black"
+line_length = 119
+skip = ["__init__.py"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spdx-tools-0.7.1rc1/spdx/parsers/lexers/tagvalue.py` & `spdx-tools-0.8.0a1/src/spdx_tools/spdx/parser/tagvalue/lexer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,242 +1,199 @@
 # Copyright (c) 2014 Ahmed H. Ismail
+# Copyright (c) 2023 spdx contributors
 # SPDX-License-Identifier: Apache-2.0
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import re
 
 from ply import lex
+from ply.lex import TOKEN
 
 
-class Lexer(object):
+class SPDXLexer:
     reserved = {
         # Top level fields
         "SPDXVersion": "DOC_VERSION",
         "DataLicense": "DOC_LICENSE",
         "DocumentName": "DOC_NAME",
         "SPDXID": "SPDX_ID",
         "DocumentComment": "DOC_COMMENT",
         "DocumentNamespace": "DOC_NAMESPACE",
         "ExternalDocumentRef": "EXT_DOC_REF",
-        # Creation info
+        # Creation info fields
         "Creator": "CREATOR",
         "Created": "CREATED",
         "CreatorComment": "CREATOR_COMMENT",
-        "LicenseListVersion": "LIC_LIST_VER",
-        # Review info
-        "Reviewer": "REVIEWER",
-        "ReviewDate": "REVIEW_DATE",
-        "ReviewComment": "REVIEW_COMMENT",
-        # Annotation info
+        "LicenseListVersion": "LICENSE_LIST_VERSION",
+        # Annotation fields
         "Annotator": "ANNOTATOR",
         "AnnotationDate": "ANNOTATION_DATE",
         "AnnotationComment": "ANNOTATION_COMMENT",
         "AnnotationType": "ANNOTATION_TYPE",
         "SPDXREF": "ANNOTATION_SPDX_ID",
-        # Relationships
+        # Relationship fields
         "Relationship": "RELATIONSHIP",
         "RelationshipComment": "RELATIONSHIP_COMMENT",
-        # Package Fields
+        # Package fields
         "PackageName": "PKG_NAME",
         "PackageVersion": "PKG_VERSION",
-        "PackageDownloadLocation": "PKG_DOWN",
+        "PackageDownloadLocation": "PKG_DOWNLOAD_LOCATION",
         "FilesAnalyzed": "PKG_FILES_ANALYZED",
-        "PackageSummary": "PKG_SUM",
-        "PackageSourceInfo": "PKG_SRC_INFO",
+        "PackageSummary": "PKG_SUMMARY",
+        "PackageSourceInfo": "PKG_SOURCE_INFO",
         "PackageFileName": "PKG_FILE_NAME",
-        "PackageSupplier": "PKG_SUPPL",
-        "PackageOriginator": "PKG_ORIG",
-        "PackageChecksum": "PKG_CHKSUM",
-        "PackageVerificationCode": "PKG_VERF_CODE",
-        "PackageDescription": "PKG_DESC",
+        "PackageSupplier": "PKG_SUPPLIER",
+        "PackageOriginator": "PKG_ORIGINATOR",
+        "PackageChecksum": "PKG_CHECKSUM",
+        "PackageVerificationCode": "PKG_VERIFICATION_CODE",
+        "PackageDescription": "PKG_DESCRIPTION",
         "PackageComment": "PKG_COMMENT",
-        "PackageLicenseDeclared": "PKG_LICS_DECL",
-        "PackageLicenseConcluded": "PKG_LICS_CONC",
-        "PackageLicenseInfoFromFiles": "PKG_LICS_FFILE",
-        "PackageLicenseComments": "PKG_LICS_COMMENT",
-        "PackageCopyrightText": "PKG_CPY_TEXT",
-        "PackageHomePage": "PKG_HOME",
-        "ExternalRef": "PKG_EXT_REF",
-        "ExternalRefComment": "PKG_EXT_REF_COMMENT",
+        "PackageLicenseDeclared": "PKG_LICENSE_DECLARED",
+        "PackageLicenseConcluded": "PKG_LICENSE_CONCLUDED",
+        "PackageLicenseInfoFromFiles": "PKG_LICENSE_INFO",
+        "PackageLicenseComments": "PKG_LICENSE_COMMENT",
+        "PackageCopyrightText": "PKG_COPYRIGHT_TEXT",
+        "PackageHomePage": "PKG_HOMEPAGE",
+        "ExternalRef": "PKG_EXTERNAL_REF",
+        "ExternalRefComment": "PKG_EXTERNAL_REF_COMMENT",
         "PackageAttributionText": "PKG_ATTRIBUTION_TEXT",
         "PrimaryPackagePurpose": "PRIMARY_PACKAGE_PURPOSE",
         "BuiltDate": "BUILT_DATE",
         "ReleaseDate": "RELEASE_DATE",
         "ValidUntilDate": "VALID_UNTIL_DATE",
-        # Files
+        # File fields
         "FileName": "FILE_NAME",
         "FileType": "FILE_TYPE",
-        "FileChecksum": "FILE_CHKSUM",
-        "LicenseConcluded": "FILE_LICS_CONC",
-        "LicenseInfoInFile": "FILE_LICS_INFO",
-        "FileCopyrightText": "FILE_CR_TEXT",
-        "LicenseComments": "FILE_LICS_COMMENT",
+        "FileChecksum": "FILE_CHECKSUM",
+        "LicenseConcluded": "FILE_LICENSE_CONCLUDED",
+        "LicenseInfoInFile": "FILE_LICENSE_INFO",
+        "FileCopyrightText": "FILE_COPYRIGHT_TEXT",
+        "LicenseComments": "FILE_LICENSE_COMMENT",
         "FileComment": "FILE_COMMENT",
         "FileNotice": "FILE_NOTICE",
-        "FileContributor": "FILE_CONTRIB",
-        "FileDependency": "FILE_DEP",
-        "ArtifactOfProjectName": "ART_PRJ_NAME",
-        "ArtifactOfProjectHomePage": "ART_PRJ_HOME",
-        "ArtifactOfProjectURI": "ART_PRJ_URI",
+        "FileContributor": "FILE_CONTRIBUTOR",
         "FileAttributionText": "FILE_ATTRIBUTION_TEXT",
-        # License
-        "LicenseID": "LICS_ID",
-        "ExtractedText": "LICS_TEXT",
-        "LicenseName": "LICS_NAME",
-        "LicenseCrossReference": "LICS_CRS_REF",
-        "LicenseComment": "LICS_COMMENT",
-        # Snippet
+        # ExtractedLicensingInfo fields
+        "LicenseID": "LICENSE_ID",
+        "ExtractedText": "LICENSE_TEXT",
+        "LicenseName": "LICENSE_NAME",
+        "LicenseCrossReference": "LICENSE_CROSS_REF",
+        "LicenseComment": "LICENSE_COMMENT",
+        # Snippet fields
         "SnippetSPDXID": "SNIPPET_SPDX_ID",
         "SnippetName": "SNIPPET_NAME",
         "SnippetComment": "SNIPPET_COMMENT",
-        "SnippetCopyrightText": "SNIPPET_CR_TEXT",
-        "SnippetLicenseComments": "SNIPPET_LICS_COMMENT",
+        "SnippetCopyrightText": "SNIPPET_COPYRIGHT_TEXT",
+        "SnippetLicenseComments": "SNIPPET_LICENSE_COMMENT",
         "SnippetFromFileSPDXID": "SNIPPET_FILE_SPDXID",
-        "SnippetLicenseConcluded": "SNIPPET_LICS_CONC",
-        "LicenseInfoInSnippet": "SNIPPET_LICS_INFO",
+        "SnippetLicenseConcluded": "SNIPPET_LICENSE_CONCLUDED",
+        "LicenseInfoInSnippet": "SNIPPET_LICENSE_INFO",
         "SnippetAttributionText": "SNIPPET_ATTRIBUTION_TEXT",
         "SnippetByteRange": "SNIPPET_BYTE_RANGE",
         "SnippetLineRange": "SNIPPET_LINE_RANGE",
-        # Common
-        "NOASSERTION": "NO_ASSERT",
-        "UNKNOWN": "UN_KNOWN",
+        # Common fields
+        "NOASSERTION": "NO_ASSERTION",
         "NONE": "NONE",
-        "SOURCE": "SOURCE",
-        "BINARY": "BINARY",
-        "ARCHIVE": "ARCHIVE",
-        "APPLICATION": "APPLICATION",
-        "AUDIO": "AUDIO",
-        "IMAGE": "IMAGE",
-        "TEXT": "FILETYPE_TEXT",
-        "VIDEO": "VIDEO",
-        "DOCUMENTATION": "DOCUMENTATION",
-        "SPDX": "SPDX",
-        "OTHER": "OTHER",
-        "REVIEW": "REVIEW",
-        "FRAMEWORK": "FRAMEWORK",
-        "LIBRARY": "LIBRARY",
-        "CONTAINER": "CONTAINER",
-        "OPERATING-SYSTEM": "OPERATING_SYSTEM",
-        "DEVICE": "DEVICE",
-        "FIRMWARE": "FIRMWARE",
-        "FILE": "FILE",
-        "INSTALL": "INSTALL"
     }
     states = (("text", "exclusive"),)
 
     tokens = [
         "TEXT",
         "TOOL_VALUE",
         "UNKNOWN_TAG",
-        "ORG_VALUE",
+        "ORGANIZATION_VALUE",
         "PERSON_VALUE",
-        "DATE",
+        "ISO8601_DATE",
         "LINE",
-        "CHKSUM",
-        "DOC_REF_ID",
-        "DOC_URI",
-        "EXT_DOC_REF_CHKSUM",
+        "CHECKSUM",
     ] + list(reserved.values())
 
+    def __init__(self):
+        self.lexer = None
+
+    @TOKEN(r":\s*<text>")
     def t_text(self, t):
-        r":\s*<text>"
         t.lexer.text_start = t.lexer.lexpos - len("<text>")
         t.lexer.begin("text")
 
+    @TOKEN(r"</text>\s*")
     def t_text_end(self, t):
-        r"</text>\s*"
         t.type = "TEXT"
-        t.value = t.lexer.lexdata[t.lexer.text_start: t.lexer.lexpos]
+        t.value = t.lexer.lexdata[t.lexer.text_start : t.lexer.lexpos]
         t.lexer.lineno += t.value.count("\n")
         t.value = t.value.strip()
         t.lexer.begin("INITIAL")
         return t
 
+    @TOKEN(r".|\n")
     def t_text_any(self, t):
-        r".|\n"
         pass
 
     def t_text_error(self, t):
         print("Lexer error in text state")
 
-    def t_CHKSUM(self, t):
-        r":\s*(ADLER32|BLAKE2b-256|BLAKE2b-384|BLAKE2b-512|BLAKE3|MD2|MD4|MD5|MD6|" \
-        "SHA1|SHA224|SHA256|SHA384|SHA512|SHA3-256|SHA3-384|SHA3-512):\s*([a-f0-9]*)"
-        t.value = t.value[1:].strip()
-        return t
-
-
-    def t_DOC_REF_ID(self, t):
-        r":\s*DocumentRef-([A-Za-z0-9\+\.\-]+)"
-        t.value = t.value[1:].strip()
-        return t
-
-    def t_DOC_URI(self, t):
-        r"\s*((ht|f)tps?:\/\/\S*)"
-        t.value = t.value.strip()
-        return t
-
-    def t_EXT_DOC_REF_CHKSUM(self, t):
-        r"\s*SHA1:\s*[a-f0-9]{40,40}"
+    @TOKEN(
+        r":\s*(ADLER32|BLAKE2b-256|BLAKE2b-384|BLAKE2b-512|BLAKE3|MD2|MD4|MD5|MD6|SHA1|SHA224|SHA256|SHA384|SHA512|"
+        r"SHA3-256|SHA3-384|SHA3-512):\s*([a-f0-9]*)"
+    )
+    def t_CHECKSUM(self, t):
         t.value = t.value[1:].strip()
         return t
 
+    @TOKEN(r":\s*Tool:.+")
     def t_TOOL_VALUE(self, t):
-        r":\s*Tool:.+"
         t.value = t.value[1:].strip()
         return t
 
-    def t_ORG_VALUE(self, t):
-        r":\s*Organization:.+"
+    @TOKEN(r":\s*Organization:.+")
+    def t_ORGANIZATION_VALUE(self, t):
         t.value = t.value[1:].strip()
         return t
 
+    @TOKEN(r":\s*Person:.+")
     def t_PERSON_VALUE(self, t):
-        r":\s*Person:.+"
         t.value = t.value[1:].strip()
         return t
 
-    def t_DATE(self, t):
-        r":\s*\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\dZ"
+    @TOKEN(r":\s*\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\dZ")
+    def t_ISO8601_DATE(self, t):
         t.value = t.value[1:].strip()
         return t
 
+    @TOKEN(r"[a-zA-Z]+")
     def t_KEYWORD_AS_TAG(self, t):
-        r"[a-zA-Z]+"
         t.type = self.reserved.get(t.value, "UNKNOWN_TAG")
         t.value = t.value.strip()
         return t
 
+    @TOKEN(r":.+")
     def t_LINE_OR_KEYWORD_VALUE(self, t):
-        r":.+"
         t.value = t.value[1:].strip()
         if t.value in self.reserved.keys():
             t.type = self.reserved[t.value]
-            return t
         else:
             t.type = "LINE"
         return t
 
+    @TOKEN(r"\#.*")
     def t_comment(self, t):
-        r"\#.*"
         pass
 
+    @TOKEN(r"\n+")
     def t_newline(self, t):
-        r"\n+"
         t.lexer.lineno += len(t.value)
 
+    @TOKEN(r"[ \t]+")
     def t_whitespace(self, t):
-        r"[ \t]+"
         pass
 
     def build(self, **kwargs):
         self.lexer = lex.lex(module=self, **kwargs)
 
     def token(self):
         return self.lexer.token()
```

### Comparing `spdx-tools-0.7.1rc1/spdx/parsers/xmlparser.py` & `spdx-tools-0.8.0a1/tests/spdx/parser/tagvalue/test_file_parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,70 @@
-# Copyright (c) Xavier Figueroa
+# SPDX-FileCopyrightText: 2023 spdx contributors
+#
 # SPDX-License-Identifier: Apache-2.0
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#     http://www.apache.org/licenses/LICENSE-2.0
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from collections import OrderedDict
-
-import xmltodict
-
-from spdx.parsers import jsonyamlxml
-
-
-class Parser(jsonyamlxml.Parser):
-    """
-    Wrapper class for jsonyamlxml.Parser to provide an interface similar to
-    RDF and TV Parser classes (i.e., spdx.parsers.<format name>.Parser) for XML parser.
-    It also avoids to repeat jsonyamlxml.Parser.parse code for JSON, YAML and XML parsers
-    """
-
-    def __init__(self, builder, logger):
-        super(Parser, self).__init__(builder, logger)
-        self.LIST_LIKE_FIELDS = {
-            "creators",
-            "externalDocumentRefs",
-            "extractedLicenseInfos",
-            "seeAlsos",
-            "annotations",
-            "relationships",
-            "snippets",
-            "reviewers",
-            "fileTypes",
-            "licenseInfoFromFiles",
-            "licenseInfoInFiles",
-            "artifactOf",
-            "fileContributors",
-            "fileDependencies",
-            "files",
-            "documentDescribes",
-            "packages",
-            "checksums",
-            "hasFiles",
-            "externalRefs",
-            "ranges",
-            "licenseInfoInSnippets",
-            "packageVerificationCodeExcludedFiles",
-        }
-
-    def parse(self, file):
-        parsed_xml = xmltodict.parse(
-            file.read(), strip_whitespace=False, encoding="utf-8"
-        )
-        fixed_object = self._set_in_list(parsed_xml, self.LIST_LIKE_FIELDS)
-        self.document_object = fixed_object.get("Document")
-        return super(Parser, self).parse()
-
-    def _set_in_list(self, data, keys):
-        """
-        xmltodict parse list-like fields in different way when there is only one
-        of them than when there are several of them.
-        Set in lists those fields that are expected to be in them.
-        """
-        if isinstance(data, (dict, OrderedDict)):
-            new_data = OrderedDict()
-            for k, v in data.items():
-                if k in keys and not isinstance(v, list):
-                    new_data[k] = [self._set_in_list(v, keys)]
-                else:
-                    new_data[k] = self._set_in_list(v, keys)
-            return new_data
-        elif isinstance(data, list):
-            new_data = []
-            for element in data:
-                new_data.append(self._set_in_list(element, keys))
-            return new_data
-        return data
+import pytest
+from license_expression import get_spdx_licensing
+
+from spdx_tools.spdx.model import FileType, SpdxNoAssertion
+from spdx_tools.spdx.parser.error import SPDXParsingError
+from spdx_tools.spdx.parser.tagvalue.parser import Parser
+from tests.spdx.parser.tagvalue.test_creation_info_parser import DOCUMENT_STR
+
+
+def test_parse_file():
+    parser = Parser()
+    file_str = "\n".join(
+        [
+            "FileName: testfile.java",
+            "SPDXID: SPDXRef-File",
+            "FileType: SOURCE",
+            "FileType: TEXT",
+            "FileChecksum: SHA1: 2fd4e1c67a2d28fced849ee1bb76e7391b93eb12",
+            "LicenseConcluded: Apache-2.0",
+            "LicenseInfoInFile: Apache-2.0",
+            "LicenseInfoInFile: NOASSERTION",
+            "FileCopyrightText: <text>Copyright 2014 Acme Inc.</text>",
+            "FileComment: <text>Very long file</text>",
+            "FileAttributionText: <text>Acknowledgements that might be required to be communicated in some contexts."
+            "</text>",
+        ]
+    )
+    document = parser.parse("\n".join([DOCUMENT_STR, file_str]))
+    assert document is not None
+    assert len(document.files) == 1
+    spdx_file = document.files[0]
+    assert spdx_file.name == "testfile.java"
+    assert spdx_file.spdx_id == "SPDXRef-File"
+    assert spdx_file.file_types == [FileType.SOURCE, FileType.TEXT]
+    assert spdx_file.comment == "Very long file"
+    assert spdx_file.attribution_texts == [
+        "Acknowledgements that might be required to be communicated in some contexts."
+    ]
+    assert spdx_file.license_info_in_file == [get_spdx_licensing().parse("Apache-2.0"), SpdxNoAssertion()]
+    assert spdx_file.license_concluded == get_spdx_licensing().parse("Apache-2.0")
+
+
+def test_parse_invalid_file():
+    parser = Parser()
+    file_str = "\n".join(
+        [
+            "FileName: testfile.java",
+            "SPDXID: SPDXRef-File",
+            "FileType: SOUCE",
+            "FileType: TEXT",
+            "FileChecksum: SHA3: 2fd4e1c67a2d28fced849ee1bb76e7391b93eb12",
+            "LicenseConcluded: Apache-2.0",
+            "LicenseInfoInFile: Apache-2.0",
+            "FileCopyrightText: <text>Copyright 2014 Acme Inc.</text>",
+            "FileComment: <text>Very long file</text>",
+            "FileAttributionText: <text>Acknowledgements that might be required to be communicated in some contexts."
+            "</text>",
+        ]
+    )
+
+    with pytest.raises(SPDXParsingError) as err:
+        parser.parse(file_str)
+
+    assert err.value.get_messages() == [
+        "Error while parsing File: ['Invalid FileType: SOUCE. Line 3', 'Error while "
+        "parsing FileChecksum: Token did not match specified grammar rule. Line: 5']"
+    ]
```

### Comparing `spdx-tools-0.7.1rc1/spdx/version.py` & `spdx-tools-0.8.0a1/src/spdx_tools/spdx/model/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,40 @@
-# Copyright (c) 2014 Ahmed H. Ismail
+# SPDX-FileCopyrightText: 2022 spdx contributors
+#
 # SPDX-License-Identifier: Apache-2.0
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#     http://www.apache.org/licenses/LICENSE-2.0
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
 
-from functools import total_ordering
+
 import re
+from re import Pattern
+
 
+class Version:
+    VERSION_REGEX: Pattern = re.compile(r"^(\d+)\.(\d+)$")
 
-@total_ordering
-class Version(object):
-    """
-    Version number composed of major and minor.
-    Fields:
-    - major: Major number, int.
-    - minor: Minor number, int.
-    """
-
-    VERS_STR_REGEX = re.compile(r"(\d+)\.(\d+)")
-
-    def __init__(self, major, minor):
-        self.major = int(major)
-        self.minor = int(minor)
+    major: int
+    minor: int
 
     @classmethod
-    def from_str(cls, value):
-        """Constructs a Version from a string.
-        Returns None if string not in N.N form where N represents a
-        number.
-        """
-        m = cls.VERS_STR_REGEX.match(value)
-        if m is not None:
-            return cls(int(m.group(1)), int(m.group(2)))
-        else:
-            return None
+    def is_valid_version_string(cls, value: str) -> bool:
+        return cls.VERSION_REGEX.match(value) is not None
 
-    def __repr__(self):
-        return "Version" + repr((self.major, self.minor))
+    # No type hint for Python reasons.
+    # See https://stackoverflow.com/questions/33533148/how-do-i-type-hint-a-method-with-the-type-of-the-enclosing-class
+    @classmethod
+    def from_string(cls, value: str):
+        if not Version.is_valid_version_string(value):
+            raise ValueError(f"{value} is not a valid version string")
+
+        match = cls.VERSION_REGEX.match(value)
+        return cls(int(match.group(1)), int(match.group(2)))
+
+    def __init__(self, major: int, minor: int):
+        self.major = major
+        self.minor = minor
 
     def __str__(self):
-        return "SPDX-{major}.{minor}".format(**self.__dict__)
+        return f"{self.major}.{self.minor}"
 
     def __eq__(self, other):
-        return (
-            isinstance(other, self.__class__)
-            and self.major == other.major
-            and self.minor == other.minor
-        )
-
-    def __lt__(self, other):
-        return self.major < other.major or (
-            self.major == other.major and self.minor < other.minor
-        )
+        if not isinstance(other, Version):
+            return False
+        return self.major == other.major and self.minor == other.minor
```

### Comparing `spdx-tools-0.7.1rc1/tests/data/doc_parse/SBOMexpected.json` & `spdx-tools-0.8.0a1/tests/spdx/writer/json/expected_results/expected.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.20650470219435738%*

 * *Differences: {"'SPDXID'": "'SPDXRef-DOCUMENT'",*

 * * "'comment'": "'documentComment'",*

 * * "'creationInfo'": "OrderedDict([('comment', 'creatorComment'), ('created', "*

 * *                   "'2022-12-01T00:00:00Z'), ('creators', ['Person: creatorName "*

 * *                   "(some@mail.com)']), ('licenseListVersion', '3.19')])",*

 * * "'dataLicense'": "'CC0-1.0'",*

 * * "'documentNamespace'": "'https://some.namespace'",*

 * * "'externalDocumentRefs'": "[OrderedDict([('checksum', OrderedDict([('algorithm', 'SHA1'), "*

 * *                           "('c […]*

```diff
@@ -1,174 +1,178 @@
 {
-    "annotations": [],
-    "comment": null,
-    "created": "2020-07-23T18:30:22Z",
-    "creatorComment": null,
-    "creators": [
-        {
-            "email": null,
-            "name": "Example Inc.",
-            "type": "Organization"
-        },
-        {
-            "email": null,
-            "name": "Thomas Steenbergen",
-            "type": "Person"
-        }
-    ],
-    "dataLicense": {
-        "identifier": "CC0-1.0",
-        "name": "Creative Commons Zero v1.0 Universal",
-        "type": "Single"
+    "SPDXID": "SPDXRef-DOCUMENT",
+    "comment": "documentComment",
+    "creationInfo": {
+        "comment": "creatorComment",
+        "created": "2022-12-01T00:00:00Z",
+        "creators": [
+            "Person: creatorName (some@mail.com)"
+        ],
+        "licenseListVersion": "3.19"
     },
-    "documentNamespace": "http://spdx.org/spdxdocs/spdx-document-xyz",
-    "externalDocumentRefs": [],
-    "extractedLicenses": [],
-    "files": [],
-    "id": "SPDXRef-DOCUMENT",
-    "licenseListVersion": {
-        "major": 3,
-        "minor": 9
-    },
-    "name": "xyz-0.1.0",
-    "packages": [
+    "dataLicense": "CC0-1.0",
+    "documentNamespace": "https://some.namespace",
+    "externalDocumentRefs": [
+        {
+            "checksum": {
+                "algorithm": "SHA1",
+                "checksumValue": "71c4025dd9897b364f3ebbb42c484ff43d00791c"
+            },
+            "externalDocumentId": "DocumentRef-external",
+            "spdxDocument": "https://namespace.com"
+        }
+    ],
+    "files": [
         {
-            "checksums": [
+            "SPDXID": "SPDXRef-File",
+            "annotations": [
                 {
-                    "identifier": "SHA1",
-                    "value": "SOME-SHA1"
+                    "annotationDate": "2022-12-24T00:00:00Z",
+                    "annotationType": "REVIEW",
+                    "annotator": "Person: annotatorName (some@mail.com)",
+                    "comment": "annotationComment"
                 }
             ],
-            "copyrightText": "copyright 2004-2020 Example Inc. All Rights Reserved.",
-            "description": null,
-            "downloadLocation": "git+ssh://gitlab.example.com:3389/products/xyz.git@b2c358080011af6a366d2512a25a379fbe7b1f78",
-            "homepage": "https://example.com/products/xyz",
-            "id": "SPDXRef-Package-xyz",
-            "licenseComment": null,
-            "licenseConcluded": {
-                "identifier": "NOASSERTION",
-                "name": "NOASSERTION",
-                "type": "Single"
-            },
-            "licenseDeclared": {
-                "identifier": [
-                    "Apache-2.0",
-                    "LicenseRef-Proprietary-ExampleInc",
-                    "curl"
-                ],
-                "name": [
-                    "Apache License 2.0",
-                    "LicenseRef-Proprietary-ExampleInc",
-                    "curl License"
-                ],
-                "type": "Conjunction"
-            },
-            "licenseInfoFromFiles": [],
-            "name": "xyz",
-            "originator": null,
-            "packageFileName": null,
-            "sourceInfo": null,
-            "summary": "Awesome product created by Example Inc.",
-            "supplier": null,
-            "verificationCode": {
-                "excludedFilesNames": [],
-                "value": null
-            },
-            "versionInfo": "0.1.0"
-        },
-        {
+            "attributionTexts": [
+                "fileAttributionText"
+            ],
             "checksums": [
                 {
-                    "identifier": "SHA1",
-                    "value": "SOME-SHA1"
+                    "algorithm": "SHA1",
+                    "checksumValue": "71c4025dd9897b364f3ebbb42c484ff43d00791c"
                 }
             ],
-            "copyrightText": "Copyright (c) 1996 - 2020, Daniel Stenberg, <daniel@haxx.se>, and many contributors, see the THANKS file.",
-            "description": "A command line tool and library for transferring data with URL syntax, supporting HTTP, HTTPS, FTP, FTPS, GOPHER, TFTP, SCP, SFTP, SMB, TELNET, DICT, LDAP, LDAPS, MQTT, FILE, IMAP, SMTP, POP3, RTSP and RTMP. libcurl offers a myriad of powerful features.",
-            "downloadLocation": "https://github.com/curl/curl/releases/download/curl-7_70_0/curl-7.70.0.tar.gz",
-            "homepage": "https://curl.haxx.se/",
-            "id": "SPDXRef-Package-curl",
-            "licenseComment": null,
-            "licenseConcluded": {
-                "identifier": "NOASSERTION",
-                "name": "NOASSERTION",
-                "type": "Single"
-            },
-            "licenseDeclared": {
-                "identifier": "curl",
-                "name": "curl License",
-                "type": "Single"
-            },
-            "licenseInfoFromFiles": [],
-            "name": "curl",
-            "originator": null,
-            "packageFileName": "./libs/curl",
-            "sourceInfo": null,
-            "summary": null,
-            "supplier": null,
-            "verificationCode": {
-                "excludedFilesNames": [],
-                "value": null
-            },
-            "versionInfo": "7.70.0"
-        },
+            "comment": "fileComment",
+            "copyrightText": "copyrightText",
+            "fileContributors": [
+                "fileContributor"
+            ],
+            "fileName": "./fileName.py",
+            "fileTypes": [
+                "TEXT"
+            ],
+            "licenseComments": "licenseComment",
+            "licenseConcluded": "MIT AND GPL-2.0-only",
+            "licenseInfoInFiles": [
+                "MIT",
+                "GPL-2.0-only",
+                "NOASSERTION"
+            ],
+            "noticeText": "fileNotice"
+        }
+    ],
+    "hasExtractedLicensingInfos": [
+        {
+            "comment": "licenseComment",
+            "extractedText": "extractedText",
+            "licenseId": "LicenseRef-1",
+            "name": "licenseName",
+            "seeAlsos": [
+                "https://see.also"
+            ]
+        }
+    ],
+    "name": "documentName",
+    "packages": [
         {
+            "SPDXID": "SPDXRef-Package",
+            "attributionTexts": [
+                "packageAttributionText"
+            ],
+            "builtDate": "2022-11-02T00:00:00Z",
             "checksums": [
                 {
-                    "identifier": "SHA1",
-                    "value": "SOME-SHA1"
+                    "algorithm": "SHA1",
+                    "checksumValue": "71c4025dd9897b364f3ebbb42c484ff43d00791c"
                 }
             ],
-            "copyrightText": "copyright 2004-2020 The OpenSSL Project Authors. All Rights Reserved.",
-            "description": "OpenSSL is a robust, commercial-grade, full-featured Open Source Toolkit for the Transport Layer Security (TLS) protocol formerly known as the Secure Sockets Layer (SSL) protocol. The protocol implementation is based on a full-strength general purpose cryptographic library, which can also be used stand-alone.",
-            "downloadLocation": "git+ssh://github.com/openssl/openssl.git@e2e09d9fba1187f8d6aafaa34d4172f56f1ffb72",
-            "homepage": "https://www.openssl.org/",
-            "id": "SPDXRef-Package-openssl",
-            "licenseComment": null,
-            "licenseConcluded": {
-                "identifier": "NOASSERTION",
-                "name": "NOASSERTION",
-                "type": "Single"
-            },
-            "licenseDeclared": {
-                "identifier": "Apache-2.0",
-                "name": "Apache License 2.0",
-                "type": "Single"
-            },
-            "licenseInfoFromFiles": [],
-            "name": "openssl",
-            "originator": null,
-            "packageFileName": "./libs/openssl",
-            "sourceInfo": null,
-            "summary": null,
-            "supplier": null,
-            "verificationCode": {
-                "excludedFilesNames": [],
-                "value": null
+            "comment": "packageComment",
+            "copyrightText": "packageCopyrightText",
+            "description": "packageDescription",
+            "downloadLocation": "https://download.com",
+            "externalRefs": [
+                {
+                    "comment": "externalPackageRefComment",
+                    "referenceCategory": "PACKAGE_MANAGER",
+                    "referenceLocator": "org.apache.tomcat:tomcat:9.0.0.M4",
+                    "referenceType": "maven-central"
+                }
+            ],
+            "filesAnalyzed": true,
+            "homepage": "https://homepage.com",
+            "licenseComments": "packageLicenseComment",
+            "licenseConcluded": "MIT AND GPL-2.0-only",
+            "licenseDeclared": "MIT AND GPL-2.0-only",
+            "licenseInfoFromFiles": [
+                "MIT",
+                "GPL-2.0-only",
+                "NOASSERTION"
+            ],
+            "name": "packageName",
+            "originator": "Person: originatorName (some@mail.com)",
+            "packageFileName": "./packageFileName",
+            "packageVerificationCode": {
+                "packageVerificationCodeExcludedFiles": [
+                    "./exclude.py"
+                ],
+                "packageVerificationCodeValue": "85ed0817af83a24ad8da68c2b5094de69833983c"
             },
-            "versionInfo": "1.1.1g"
+            "primaryPackagePurpose": "SOURCE",
+            "releaseDate": "2022-11-01T00:00:00Z",
+            "sourceInfo": "sourceInfo",
+            "summary": "packageSummary",
+            "supplier": "Person: supplierName (some@mail.com)",
+            "validUntilDate": "2022-11-03T00:00:00Z",
+            "versionInfo": "12.2"
         }
     ],
     "relationships": [
         {
-            "related_spdx_element": "SPDXRef-Package-curl",
-            "relationship_type": "CONTAINS",
-            "spdx_element_id": "SPDXRef-Package-xyz"
-        },
-        {
-            "related_spdx_element": "SPDXRef-Package-openssl",
-            "relationship_type": "CONTAINS",
-            "spdx_element_id": "SPDXRef-Package-xyz"
-        },
-        {
-            "related_spdx_element": "SPDXRef-Package-xyz",
-            "relationship_type": "DESCRIBES",
-            "spdx_element_id": "SPDXRef-DOCUMENT"
-        }
-    ],
-    "reviews": [],
-    "snippets": [],
-    "specVersion": {
-        "major": 2,
-        "minor": 2
-    }
+            "comment": "relationshipComment",
+            "relatedSpdxElement": "SPDXRef-File",
+            "relationshipType": "DESCRIBES",
+            "spdxElementId": "SPDXRef-DOCUMENT"
+        }
+    ],
+    "snippets": [
+        {
+            "SPDXID": "SPDXRef-Snippet",
+            "attributionTexts": [
+                "snippetAttributionText"
+            ],
+            "comment": "snippetComment",
+            "copyrightText": "licenseCopyrightText",
+            "licenseComments": "snippetLicenseComment",
+            "licenseConcluded": "MIT AND GPL-2.0-only",
+            "licenseInfoInSnippets": [
+                "MIT",
+                "GPL-2.0-only",
+                "NONE"
+            ],
+            "name": "snippetName",
+            "ranges": [
+                {
+                    "endPointer": {
+                        "offset": 2,
+                        "reference": "SPDXRef-File"
+                    },
+                    "startPointer": {
+                        "offset": 1,
+                        "reference": "SPDXRef-File"
+                    }
+                },
+                {
+                    "endPointer": {
+                        "lineNumber": 4,
+                        "reference": "SPDXRef-File"
+                    },
+                    "startPointer": {
+                        "lineNumber": 3,
+                        "reference": "SPDXRef-File"
+                    }
+                }
+            ],
+            "snippetFromFile": "SPDXRef-File"
+        }
+    ],
+    "spdxVersion": "SPDX-2.3"
 }
```

### Comparing `spdx-tools-0.7.1rc1/tests/data/formats/SPDXJSONExample-v2.2.spdx.json` & `spdx-tools-0.8.0a1/tests/spdx/data/SPDXJSONExample-v2.2.spdx.json`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.7.1rc1/tests/data/formats/SPDXJSONExample-v2.3.spdx.json` & `spdx-tools-0.8.0a1/tests/spdx/data/SPDXJSONExample-v2.3.spdx.json`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.7.1rc1/tests/data/formats/SPDXJsonExample.json` & `spdx-tools-0.8.0a1/tests/spdx/parser/jsonlikedict/test_package_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,887 +1,841 @@
-00000000: 7b0a 2020 2263 6f6d 6d65 6e74 223a 2022  {.  "comment": "
-00000010: 5468 6973 2069 7320 6120 7361 6d70 6c65  This is a sample
-00000020: 2073 7072 6561 6473 6865 6574 222c 0a20   spreadsheet",. 
-00000030: 2022 6e61 6d65 223a 2022 5361 6d70 6c65   "name": "Sample
-00000040: 5f44 6f63 756d 656e 742d 5632 2e31 222c  _Document-V2.1",
-00000050: 0a20 2022 646f 6375 6d65 6e74 4465 7363  .  "documentDesc
-00000060: 7269 6265 7322 3a20 5b0a 2020 2020 2253  ribes": [.    "S
-00000070: 5044 5852 6566 2d50 6163 6b61 6765 220a  PDXRef-Package".
-00000080: 2020 5d2c 0a20 2022 7061 636b 6167 6573    ],.  "packages
-00000090: 223a 205b 0a20 2020 207b 0a20 2020 2020  ": [.    {.     
-000000a0: 2022 5350 4458 4944 223a 2022 5350 4458   "SPDXID": "SPDX
-000000b0: 5265 662d 5061 636b 6167 6522 2c0a 2020  Ref-Package",.  
-000000c0: 2020 2020 226f 7269 6769 6e61 746f 7222      "originator"
-000000d0: 3a20 224f 7267 616e 697a 6174 696f 6e3a  : "Organization:
-000000e0: 2053 5044 5822 2c0a 2020 2020 2020 2268   SPDX",.      "h
-000000f0: 6173 4669 6c65 7322 3a20 5b0a 2020 2020  asFiles": [.    
-00000100: 2020 2020 2253 5044 5852 6566 2d46 696c      "SPDXRef-Fil
-00000110: 6531 222c 0a20 2020 2020 2020 2022 5350  e1",.        "SP
-00000120: 4458 5265 662d 4669 6c65 3222 0a20 2020  DXRef-File2".   
-00000130: 2020 205d 2c0a 2020 2020 2020 226c 6963     ],.      "lic
-00000140: 656e 7365 496e 666f 4672 6f6d 4669 6c65  enseInfoFromFile
-00000150: 7322 3a20 5b0a 2020 2020 2020 2020 2241  s": [.        "A
-00000160: 7061 6368 652d 312e 3022 2c0a 2020 2020  pache-1.0",.    
-00000170: 2020 2020 224c 6963 656e 7365 5265 662d      "LicenseRef-
-00000180: 3322 2c0a 2020 2020 2020 2020 224d 504c  3",.        "MPL
-00000190: 2d31 2e31 222c 0a20 2020 2020 2020 2022  -1.1",.        "
-000001a0: 4c69 6365 6e73 6552 6566 2d32 222c 0a20  LicenseRef-2",. 
-000001b0: 2020 2020 2020 2022 4c69 6365 6e73 6552         "LicenseR
-000001c0: 6566 2d34 222c 0a20 2020 2020 2020 2022  ef-4",.        "
-000001d0: 4170 6163 6865 2d32 2e30 222c 0a20 2020  Apache-2.0",.   
-000001e0: 2020 2020 2022 4c69 6365 6e73 6552 6566       "LicenseRef
-000001f0: 2d31 220a 2020 2020 2020 5d2c 0a20 2020  -1".      ],.   
-00000200: 2020 2022 6e61 6d65 223a 2022 5350 4458     "name": "SPDX
-00000210: 2054 7261 6e73 6c61 746f 7222 2c0a 2020   Translator",.  
-00000220: 2020 2020 2270 6163 6b61 6765 4669 6c65      "packageFile
-00000230: 4e61 6d65 223a 2022 7370 6478 7472 616e  Name": "spdxtran
-00000240: 736c 6174 6f72 2d31 2e30 2e7a 6970 222c  slator-1.0.zip",
-00000250: 0a20 2020 2020 2022 6c69 6365 6e73 6543  .      "licenseC
-00000260: 6f6d 6d65 6e74 7322 3a20 2254 6865 2064  omments": "The d
-00000270: 6563 6c61 7265 6420 6c69 6365 6e73 6520  eclared license 
-00000280: 696e 666f 726d 6174 696f 6e20 6361 6e20  information can 
-00000290: 6265 2066 6f75 6e64 2069 6e20 7468 6520  be found in the 
-000002a0: 4e4f 5449 4345 2066 696c 6520 6174 2074  NOTICE file at t
-000002b0: 6865 2072 6f6f 7420 6f66 2074 6865 2061  he root of the a
-000002c0: 7263 6869 7665 2066 696c 6522 2c0a 2020  rchive file",.  
-000002d0: 2020 2020 2273 756d 6d61 7279 223a 2022      "summary": "
-000002e0: 5350 4458 2054 7261 6e73 6c61 746f 7220  SPDX Translator 
-000002f0: 7574 696c 6974 7922 2c0a 2020 2020 2020  utility",.      
-00000300: 2273 6f75 7263 6549 6e66 6f22 3a20 2256  "sourceInfo": "V
-00000310: 6572 7369 6f6e 2031 2e30 206f 6620 7468  ersion 1.0 of th
-00000320: 6520 5350 4458 2054 7261 6e73 6c61 746f  e SPDX Translato
-00000330: 7220 6170 706c 6963 6174 696f 6e22 2c0a  r application",.
-00000340: 2020 2020 2020 2263 6f70 7972 6967 6874        "copyright
-00000350: 5465 7874 223a 2022 2043 6f70 7972 6967  Text": " Copyrig
-00000360: 6874 2032 3031 302c 2032 3031 3120 536f  ht 2010, 2011 So
-00000370: 7572 6365 2041 7564 6974 6f72 2049 6e63  urce Auditor Inc
-00000380: 2e22 2c0a 2020 2020 2020 2270 6163 6b61  .",.      "packa
-00000390: 6765 5665 7269 6669 6361 7469 6f6e 436f  geVerificationCo
-000003a0: 6465 223a 207b 0a20 2020 2020 2020 2022  de": {.        "
-000003b0: 7061 636b 6167 6556 6572 6966 6963 6174  packageVerificat
-000003c0: 696f 6e43 6f64 6556 616c 7565 223a 2022  ionCodeValue": "
-000003d0: 3465 3332 3131 6336 3761 3264 3238 6663  4e3211c67a2d28fc
-000003e0: 6564 3834 3965 6531 6262 3736 6537 3339  ed849ee1bb76e739
-000003f0: 3162 3933 6665 6261 222c 0a20 2020 2020  1b93feba",.     
-00000400: 2020 2022 7061 636b 6167 6556 6572 6966     "packageVerif
-00000410: 6963 6174 696f 6e43 6f64 6545 7863 6c75  icationCodeExclu
-00000420: 6465 6446 696c 6573 223a 205b 0a20 2020  dedFiles": [.   
-00000430: 2020 2020 2020 2022 5370 6478 5472 616e         "SpdxTran
-00000440: 736c 6174 6f72 5370 6478 2e72 6466 222c  slatorSpdx.rdf",
-00000450: 0a20 2020 2020 2020 2020 2022 5370 6478  .          "Spdx
-00000460: 5472 616e 736c 6174 6f72 5370 6478 2e74  TranslatorSpdx.t
-00000470: 7874 220a 2020 2020 2020 2020 5d0a 2020  xt".        ].  
-00000480: 2020 2020 7d2c 0a20 2020 2020 2022 6c69      },.      "li
-00000490: 6365 6e73 6543 6f6e 636c 7564 6564 223a  censeConcluded":
-000004a0: 2022 2841 7061 6368 652d 312e 3020 414e   "(Apache-1.0 AN
-000004b0: 4420 4c69 6365 6e73 6552 6566 2d32 2041  D LicenseRef-2 A
-000004c0: 4e44 204d 504c 2d31 2e31 2041 4e44 204c  ND MPL-1.1 AND L
-000004d0: 6963 656e 7365 5265 662d 3320 414e 4420  icenseRef-3 AND 
-000004e0: 4c69 6365 6e73 6552 6566 2d34 2041 4e44  LicenseRef-4 AND
-000004f0: 2041 7061 6368 652d 322e 3020 414e 4420   Apache-2.0 AND 
-00000500: 4c69 6365 6e73 6552 6566 2d31 2922 2c0a  LicenseRef-1)",.
-00000510: 2020 2020 2020 2273 7570 706c 6965 7222        "supplier"
-00000520: 3a20 224f 7267 616e 697a 6174 696f 6e3a  : "Organization:
-00000530: 204c 696e 7578 2046 6f75 6e64 6174 696f   Linux Foundatio
-00000540: 6e22 2c0a 2020 2020 2020 2261 7474 7269  n",.      "attri
-00000550: 6275 7469 6f6e 5465 7874 7322 3a20 5b0a  butionTexts": [.
-00000560: 2020 2020 2020 2020 2254 6865 2047 4e55          "The GNU
-00000570: 2043 204c 6962 7261 7279 2069 7320 6672   C Library is fr
-00000580: 6565 2073 6f66 7477 6172 652e 2020 5365  ee software.  Se
-00000590: 6520 7468 6520 6669 6c65 2043 4f50 5949  e the file COPYI
-000005a0: 4e47 2e4c 4942 2066 6f72 2063 6f70 7969  NG.LIB for copyi
-000005b0: 6e67 2063 6f6e 6469 7469 6f6e 732c 2061  ng conditions, a
-000005c0: 6e64 204c 4943 454e 5345 5320 666f 7220  nd LICENSES for 
-000005d0: 6e6f 7469 6365 7320 6162 6f75 7420 6120  notices about a 
-000005e0: 6665 7720 636f 6e74 7269 6275 7469 6f6e  few contribution
-000005f0: 7320 7468 6174 2072 6571 7569 7265 2074  s that require t
-00000600: 6865 7365 2061 6464 6974 696f 6e61 6c20  hese additional 
-00000610: 6e6f 7469 6365 7320 746f 2062 6520 6469  notices to be di
-00000620: 7374 7269 6275 7465 642e 2020 4c69 6365  stributed.  Lice
-00000630: 6e73 6520 636f 7079 7269 6768 7420 7965  nse copyright ye
-00000640: 6172 7320 6d61 7920 6265 206c 6973 7465  ars may be liste
-00000650: 6420 7573 696e 6720 7261 6e67 6520 6e6f  d using range no
-00000660: 7461 7469 6f6e 2c20 652e 672e 2c20 3139  tation, e.g., 19
-00000670: 3936 2d32 3031 352c 2069 6e64 6963 6174  96-2015, indicat
-00000680: 696e 6720 7468 6174 2065 7665 7279 2079  ing that every y
-00000690: 6561 7220 696e 2074 6865 2072 616e 6765  ear in the range
-000006a0: 2c20 696e 636c 7573 6976 652c 2069 7320  , inclusive, is 
-000006b0: 6120 636f 7079 7269 6768 7461 626c 6520  a copyrightable 
-000006c0: 7965 6172 2074 6861 7420 776f 756c 6420  year that would 
-000006d0: 6f74 6865 7277 6973 6520 6265 206c 6973  otherwise be lis
-000006e0: 7465 6420 696e 6469 7669 6475 616c 6c79  ted individually
-000006f0: 2e22 0a20 2020 2020 205d 2c0a 2020 2020  .".      ],.    
-00000700: 2020 2263 6865 636b 7375 6d73 223a 205b    "checksums": [
-00000710: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-00000720: 2020 2020 2022 6368 6563 6b73 756d 5661       "checksumVa
-00000730: 6c75 6522 3a20 2232 6664 3465 3163 3637  lue": "2fd4e1c67
-00000740: 6132 6432 3866 6365 6438 3439 6565 3162  a2d28fced849ee1b
-00000750: 6237 3665 3733 3931 6239 3365 6231 3222  b76e7391b93eb12"
-00000760: 2c0a 2020 2020 2020 2020 2020 2261 6c67  ,.          "alg
-00000770: 6f72 6974 686d 223a 2022 5348 4131 220a  orithm": "SHA1".
-00000780: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000790: 5d2c 0a20 2020 2020 2022 7665 7273 696f  ],.      "versio
-000007a0: 6e49 6e66 6f22 3a20 2256 6572 7369 6f6e  nInfo": "Version
-000007b0: 2030 2e39 2e32 222c 0a20 2020 2020 2022   0.9.2",.      "
-000007c0: 6c69 6365 6e73 6544 6563 6c61 7265 6422  licenseDeclared"
-000007d0: 3a20 2228 4c69 6365 6e73 6552 6566 2d34  : "(LicenseRef-4
-000007e0: 2041 4e44 204c 6963 656e 7365 5265 662d   AND LicenseRef-
-000007f0: 3320 414e 4420 4170 6163 6865 2d32 2e30  3 AND Apache-2.0
-00000800: 2041 4e44 204c 6963 656e 7365 5265 662d   AND LicenseRef-
-00000810: 3220 414e 4420 4d50 4c2d 312e 3120 414e  2 AND MPL-1.1 AN
-00000820: 4420 4c69 6365 6e73 6552 6566 2d31 2922  D LicenseRef-1)"
-00000830: 2c0a 2020 2020 2020 2264 6f77 6e6c 6f61  ,.      "downloa
-00000840: 644c 6f63 6174 696f 6e22 3a20 2268 7474  dLocation": "htt
-00000850: 703a 2f2f 7777 772e 7370 6478 2e6f 7267  p://www.spdx.org
-00000860: 2f74 6f6f 6c73 222c 0a20 2020 2020 2022  /tools",.      "
-00000870: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
-00000880: 6869 7320 7574 696c 6974 7920 7472 616e  his utility tran
-00000890: 736c 6174 6573 2061 6e64 2053 5044 5820  slates and SPDX 
-000008a0: 5244 4620 584d 4c20 646f 6375 6d65 6e74  RDF XML document
-000008b0: 2074 6f20 6120 7370 7265 6164 7368 6565   to a spreadshee
-000008c0: 742c 2074 7261 6e73 6c61 7465 7320 6120  t, translates a 
-000008d0: 7370 7265 6164 7368 6565 7420 746f 2061  spreadsheet to a
-000008e0: 6e20 5350 4458 2052 4446 2058 4d4c 2064  n SPDX RDF XML d
-000008f0: 6f63 756d 656e 7420 616e 6420 7472 616e  ocument and tran
-00000900: 736c 6174 6573 2061 6e20 5350 4458 2052  slates an SPDX R
-00000910: 4446 6120 646f 6375 6d65 6e74 2074 6f20  DFa document to 
-00000920: 616e 2053 5044 5820 5244 4620 584d 4c20  an SPDX RDF XML 
-00000930: 646f 6375 6d65 6e74 2e22 2c0a 2020 2020  document.",.    
-00000940: 2020 2270 7269 6d61 7279 5061 636b 6167    "primaryPackag
-00000950: 6550 7572 706f 7365 223a 2022 4f50 4552  ePurpose": "OPER
-00000960: 4154 494e 472d 5359 5354 454d 222c 0a20  ATING-SYSTEM",. 
-00000970: 2020 2020 2022 6275 696c 7444 6174 6522       "builtDate"
-00000980: 3a20 2232 3032 302d 3031 2d30 3154 3132  : "2020-01-01T12
-00000990: 3a30 303a 3030 5a22 2c0a 2020 2020 2020  :00:00Z",.      
-000009a0: 2272 656c 6561 7365 4461 7465 223a 2022  "releaseDate": "
-000009b0: 3230 3231 2d30 312d 3031 5431 323a 3030  2021-01-01T12:00
-000009c0: 3a30 305a 222c 0a20 2020 2020 2022 7661  :00Z",.      "va
-000009d0: 6c69 6455 6e74 696c 4461 7465 223a 2022  lidUntilDate": "
-000009e0: 3230 3232 2d30 312d 3031 5431 323a 3030  2022-01-01T12:00
-000009f0: 3a30 305a 220a 2020 2020 7d0a 2020 5d2c  :00Z".    }.  ],
-00000a00: 0a20 2022 6669 6c65 7322 3a20 5b0a 2020  .  "files": [.  
-00000a10: 2020 7b0a 2020 2020 2020 2263 6f6d 6d65    {.      "comme
-00000a20: 6e74 223a 2022 5468 6973 2066 696c 6520  nt": "This file 
-00000a30: 6265 6c6f 6e67 7320 746f 204a 656e 6122  belongs to Jena"
-00000a40: 2c0a 2020 2020 2020 226c 6963 656e 7365  ,.      "license
-00000a50: 496e 666f 496e 4669 6c65 7322 3a20 5b0a  InfoInFiles": [.
-00000a60: 2020 2020 2020 2020 224c 6963 656e 7365          "License
-00000a70: 5265 662d 3122 0a20 2020 2020 205d 2c0a  Ref-1".      ],.
-00000a80: 2020 2020 2020 2266 696c 654e 616d 6522        "fileName"
-00000a90: 3a20 224a 656e 6e61 2d32 2e36 2e33 2f6a  : "Jenna-2.6.3/j
-00000aa0: 656e 612d 322e 362e 332d 736f 7572 6365  ena-2.6.3-source
-00000ab0: 732e 6a61 7222 2c0a 2020 2020 2020 2263  s.jar",.      "c
-00000ac0: 6f70 7972 6967 6874 5465 7874 223a 2022  opyrightText": "
-00000ad0: 2863 2920 436f 7079 7269 6768 7420 3230  (c) Copyright 20
-00000ae0: 3030 2c20 3230 3031 2c20 3230 3032 2c20  00, 2001, 2002, 
-00000af0: 3230 3033 2c20 3230 3034 2c20 3230 3035  2003, 2004, 2005
-00000b00: 2c20 3230 3036 2c20 3230 3037 2c20 3230  , 2006, 2007, 20
-00000b10: 3038 2c20 3230 3039 2048 6577 6c65 7474  08, 2009 Hewlett
-00000b20: 2d50 6163 6b61 7264 2044 6576 656c 6f70  -Packard Develop
-00000b30: 6d65 6e74 2043 6f6d 7061 6e79 2c20 4c50  ment Company, LP
-00000b40: 222c 0a20 2020 2020 2022 6172 7469 6661  ",.      "artifa
-00000b50: 6374 4f66 223a 205b 0a20 2020 2020 2020  ctOf": [.       
-00000b60: 207b 0a20 2020 2020 2020 2020 2022 6e61   {.          "na
-00000b70: 6d65 223a 2022 4a65 6e61 222c 0a20 2020  me": "Jena",.   
-00000b80: 2020 2020 2020 2022 686f 6d65 5061 6765         "homePage
-00000b90: 223a 2022 6874 7470 3a2f 2f77 7777 2e6f  ": "http://www.o
-00000ba0: 7065 6e6a 656e 612e 6f72 672f 222c 0a20  penjena.org/",. 
-00000bb0: 2020 2020 2020 2020 2022 7072 6f6a 6563           "projec
-00000bc0: 7455 7269 223a 2022 6874 7470 3a2f 2f73  tUri": "http://s
-00000bd0: 7562 7665 7273 696f 6e2e 6170 6163 6865  ubversion.apache
-00000be0: 2e6f 7267 2f64 6f61 702e 7264 6622 0a20  .org/doap.rdf". 
-00000bf0: 2020 2020 2020 207d 0a20 2020 2020 205d         }.      ]
-00000c00: 2c0a 2020 2020 2020 226c 6963 656e 7365  ,.      "license
-00000c10: 436f 6e63 6c75 6465 6422 3a20 224c 6963  Concluded": "Lic
-00000c20: 656e 7365 5265 662d 3122 2c0a 2020 2020  enseRef-1",.    
-00000c30: 2020 226c 6963 656e 7365 436f 6d6d 656e    "licenseCommen
-00000c40: 7473 223a 2022 5468 6973 206c 6963 656e  ts": "This licen
-00000c50: 7365 2069 7320 7573 6564 2062 7920 4a65  se is used by Je
-00000c60: 6e61 222c 0a20 2020 2022 6368 6563 6b73  na",.    "checks
-00000c70: 756d 7322 3a20 5b0a 2020 2020 2020 2020  ums": [.        
-00000c80: 7b0a 2020 2020 2020 2020 2020 2020 2263  {.            "c
-00000c90: 6865 636b 7375 6d56 616c 7565 223a 2022  hecksumValue": "
-00000ca0: 3361 6234 6531 6336 3761 3264 3238 6663  3ab4e1c67a2d28fc
-00000cb0: 6564 3834 3965 6531 6262 3736 6537 3339  ed849ee1bb76e739
-00000cc0: 3162 3933 6631 3235 222c 0a20 2020 2020  1b93f125",.     
-00000cd0: 2020 2020 2020 2022 616c 676f 7269 7468         "algorith
-00000ce0: 6d22 3a20 2253 4841 3122 0a20 2020 2020  m": "SHA1".     
-00000cf0: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
-00000d00: 2020 2020 2020 2020 2020 2020 2263 6865              "che
-00000d10: 636b 7375 6d56 616c 7565 223a 2022 3361  cksumValue": "3a
-00000d20: 6234 6531 6336 3761 3264 3238 6663 6564  b4e1c67a2d28fced
-00000d30: 3834 3965 6531 6262 3736 6537 3339 3162  849ee1bb76e7391b
-00000d40: 3933 6631 3235 3030 3030 3030 3030 3030  93f1250000000000
-00000d50: 3030 3030 3030 222c 0a20 2020 2020 2020  000000",.       
-00000d60: 2020 2020 2022 616c 676f 7269 7468 6d22       "algorithm"
-00000d70: 3a20 2253 4841 3235 3622 0a20 2020 2020  : "SHA256".     
-00000d80: 2020 207d 0a20 2020 2020 2020 205d 2c0a     }.        ],.
-00000d90: 2020 2020 2020 2266 696c 6554 7970 6573        "fileTypes
-00000da0: 223a 205b 0a20 2020 2020 2020 2022 4152  ": [.        "AR
-00000db0: 4348 4956 4522 2c0a 2020 2020 2020 2020  CHIVE",.        
-00000dc0: 224f 5448 4552 220a 2020 2020 2020 5d2c  "OTHER".      ],
-00000dd0: 0a20 2020 2020 2022 5350 4458 4944 223a  .      "SPDXID":
-00000de0: 2022 5350 4458 5265 662d 4669 6c65 3122   "SPDXRef-File1"
-00000df0: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
-00000e00: 2020 2020 226c 6963 656e 7365 496e 666f      "licenseInfo
-00000e10: 496e 4669 6c65 7322 3a20 5b0a 2020 2020  InFiles": [.    
-00000e20: 2020 2020 2241 7061 6368 652d 322e 3022      "Apache-2.0"
-00000e30: 0a20 2020 2020 205d 2c0a 2020 2020 2020  .      ],.      
-00000e40: 2266 696c 654e 616d 6522 3a20 2273 7263  "fileName": "src
-00000e50: 2f6f 7267 2f73 7064 782f 7061 7273 6572  /org/spdx/parser
-00000e60: 2f44 4f41 5050 726f 6a65 6374 2e6a 6176  /DOAPProject.jav
-00000e70: 6122 2c0a 2020 2020 2020 2263 6f70 7972  a",.      "copyr
-00000e80: 6967 6874 5465 7874 223a 2022 436f 7079  ightText": "Copy
-00000e90: 7269 6768 7420 3230 3130 2c20 3230 3131  right 2010, 2011
-00000ea0: 2053 6f75 7263 6520 4175 6469 746f 7220   Source Auditor 
-00000eb0: 496e 632e 222c 0a20 2020 2020 2022 6c69  Inc.",.      "li
-00000ec0: 6365 6e73 6543 6f6e 636c 7564 6564 223a  censeConcluded":
-00000ed0: 2022 4170 6163 6865 2d32 2e30 222c 0a20   "Apache-2.0",. 
-00000ee0: 2020 2020 2022 6368 6563 6b73 756d 7322       "checksums"
-00000ef0: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
-00000f00: 2020 2020 2020 2020 2263 6865 636b 7375          "checksu
-00000f10: 6d56 616c 7565 223a 2022 3266 6434 6531  mValue": "2fd4e1
-00000f20: 6336 3761 3264 3238 6663 6564 3834 3965  c67a2d28fced849e
-00000f30: 6531 6262 3736 6537 3339 3162 3933 6562  e1bb76e7391b93eb
-00000f40: 3132 222c 0a20 2020 2020 2020 2020 2022  12",.          "
-00000f50: 616c 676f 7269 7468 6d22 3a20 2253 4841  algorithm": "SHA
-00000f60: 3122 0a20 2020 2020 2020 207d 0a20 2020  1".        }.   
-00000f70: 2020 205d 2c0a 2020 2020 2020 2266 696c     ],.      "fil
-00000f80: 6554 7970 6573 223a 205b 0a20 2020 2020  eTypes": [.     
-00000f90: 2020 2022 534f 5552 4345 222c 0a20 2020     "SOURCE",.   
-00000fa0: 2020 2020 2022 5445 5854 220a 2020 2020       "TEXT".    
-00000fb0: 2020 5d2c 0a20 2020 2020 2022 5350 4458    ],.      "SPDX
-00000fc0: 4944 223a 2022 5350 4458 5265 662d 4669  ID": "SPDXRef-Fi
-00000fd0: 6c65 3222 0a20 2020 207d 0a20 205d 2c0a  le2".    }.  ],.
-00000fe0: 2020 2263 7265 6174 696f 6e49 6e66 6f22    "creationInfo"
-00000ff0: 3a20 7b0a 2020 2020 2263 6f6d 6d65 6e74  : {.    "comment
-00001000: 223a 2022 5468 6973 2069 7320 616e 2065  ": "This is an e
-00001010: 7861 6d70 6c65 206f 6620 616e 2053 5044  xample of an SPD
-00001020: 5820 7370 7265 6164 7368 6565 7420 666f  X spreadsheet fo
-00001030: 726d 6174 222c 0a20 2020 2022 6372 6561  rmat",.    "crea
-00001040: 746f 7273 223a 205b 0a20 2020 2020 2022  tors": [.      "
-00001050: 546f 6f6c 3a20 536f 7572 6365 4175 6469  Tool: SourceAudi
-00001060: 746f 722d 5631 2e32 222c 0a20 2020 2020  tor-V1.2",.     
-00001070: 2022 5065 7273 6f6e 3a20 4761 7279 204f   "Person: Gary O
-00001080: 274e 6561 6c6c 222c 0a20 2020 2020 2022  'Neall",.      "
-00001090: 4f72 6761 6e69 7a61 7469 6f6e 3a20 536f  Organization: So
-000010a0: 7572 6365 2041 7564 6974 6f72 2049 6e63  urce Auditor Inc
-000010b0: 2e22 0a20 2020 205d 2c0a 2020 2020 226c  .".    ],.    "l
-000010c0: 6963 656e 7365 4c69 7374 5665 7273 696f  icenseListVersio
-000010d0: 6e22 3a20 2233 2e32 3022 2c0a 2020 2020  n": "3.20",.    
-000010e0: 2263 7265 6174 6564 223a 2022 3230 3130  "created": "2010
-000010f0: 2d30 322d 3033 5430 303a 3030 3a30 305a  -02-03T00:00:00Z
-00001100: 220a 2020 7d2c 0a20 2022 6578 7465 726e  ".  },.  "extern
-00001110: 616c 446f 6375 6d65 6e74 5265 6673 223a  alDocumentRefs":
-00001120: 205b 0a20 2020 207b 0a20 2020 2020 2022   [.    {.      "
-00001130: 6368 6563 6b73 756d 223a 207b 0a20 2020  checksum": {.   
-00001140: 2020 2020 2022 6368 6563 6b73 756d 5661       "checksumVa
-00001150: 6c75 6522 3a20 2264 3661 3737 3062 6133  lue": "d6a770ba3
-00001160: 3835 3833 6564 3462 6234 3532 3562 6439  8583ed4bb4525bd9
-00001170: 3665 3530 3436 3136 3535 6432 3735 3922  6e50461655d2759"
-00001180: 2c0a 2020 2020 2020 2020 2261 6c67 6f72  ,.        "algor
-00001190: 6974 686d 223a 2022 5348 4131 220a 2020  ithm": "SHA1".  
-000011a0: 2020 2020 7d2c 0a20 2020 2020 2022 7370      },.      "sp
-000011b0: 6478 446f 6375 6d65 6e74 223a 2022 6874  dxDocument": "ht
-000011c0: 7470 733a 2f2f 7370 6478 2e6f 7267 2f73  tps://spdx.org/s
-000011d0: 7064 7864 6f63 732f 7370 6478 2d74 6f6f  pdxdocs/spdx-too
-000011e0: 6c73 2d76 322e 312d 3346 3235 3034 4530  ls-v2.1-3F2504E0
-000011f0: 2d34 4638 392d 3431 4433 2d39 4130 432d  -4F89-41D3-9A0C-
-00001200: 3033 3035 4538 3243 3333 3031 222c 0a20  0305E82C3301",. 
-00001210: 2020 2020 2022 6578 7465 726e 616c 446f       "externalDo
-00001220: 6375 6d65 6e74 4964 223a 2022 446f 6375  cumentId": "Docu
-00001230: 6d65 6e74 5265 662d 7370 6478 2d74 6f6f  mentRef-spdx-too
-00001240: 6c2d 322e 3122 0a20 2020 207d 0a20 205d  l-2.1".    }.  ]
-00001250: 2c0a 2020 2264 6f63 756d 656e 744e 616d  ,.  "documentNam
-00001260: 6573 7061 6365 223a 2022 6874 7470 733a  espace": "https:
-00001270: 2f2f 7370 6478 2e6f 7267 2f73 7064 7864  //spdx.org/spdxd
-00001280: 6f63 732f 7370 6478 2d65 7861 6d70 6c65  ocs/spdx-example
-00001290: 2d34 3434 3530 3445 302d 3446 3839 2d34  -444504E0-4F89-4
-000012a0: 3144 332d 3941 3043 2d30 3330 3545 3832  1D3-9A0C-0305E82
-000012b0: 4333 3330 3122 2c0a 2020 2261 6e6e 6f74  C3301",.  "annot
-000012c0: 6174 696f 6e73 223a 205b 0a20 2020 207b  ations": [.    {
-000012d0: 0a20 2020 2020 2022 636f 6d6d 656e 7422  .      "comment"
-000012e0: 3a20 2254 6869 7320 6973 206a 7573 7420  : "This is just 
-000012f0: 616e 2065 7861 6d70 6c65 2e20 536f 6d65  an example. Some
-00001300: 206f 6620 7468 6520 6e6f 6e2d 7374 616e   of the non-stan
-00001310: 6461 7264 206c 6963 656e 7365 7320 6c6f  dard licenses lo
-00001320: 6f6b 206c 696b 6520 7468 6579 2061 7265  ok like they are
-00001330: 2061 6374 7561 6c6c 7920 4253 4420 3320   actually BSD 3 
-00001340: 636c 6175 7365 206c 6963 656e 7365 7322  clause licenses"
-00001350: 2c0a 2020 2020 2020 2261 6e6e 6f74 6174  ,.      "annotat
-00001360: 696f 6e54 7970 6522 3a20 2252 4556 4945  ionType": "REVIE
-00001370: 5722 2c0a 2020 2020 2020 2261 6e6e 6f74  W",.      "annot
-00001380: 6174 696f 6e44 6174 6522 3a20 2232 3031  ationDate": "201
-00001390: 322d 3036 2d31 3354 3030 3a30 303a 3030  2-06-13T00:00:00
-000013a0: 5a22 2c0a 2020 2020 2020 2261 6e6e 6f74  Z",.      "annot
-000013b0: 6174 6f72 223a 2022 5065 7273 6f6e 3a20  ator": "Person: 
-000013c0: 4a69 6d20 5265 7669 6577 6572 220a 2020  Jim Reviewer".  
-000013d0: 2020 7d0a 2020 5d2c 0a20 2022 6461 7461    }.  ],.  "data
-000013e0: 4c69 6365 6e73 6522 3a20 2243 4330 2d31  License": "CC0-1
-000013f0: 2e30 222c 0a20 2022 7265 7669 6577 6572  .0",.  "reviewer
-00001400: 7322 3a20 5b0a 2020 2020 7b0a 2020 2020  s": [.    {.    
-00001410: 2020 2263 6f6d 6d65 6e74 223a 2022 5468    "comment": "Th
-00001420: 6973 2069 7320 6a75 7374 2061 6e20 6578  is is just an ex
-00001430: 616d 706c 652e 2020 536f 6d65 206f 6620  ample.  Some of 
-00001440: 7468 6520 6e6f 6e2d 7374 616e 6461 7264  the non-standard
-00001450: 206c 6963 656e 7365 7320 6c6f 6f6b 206c   licenses look l
-00001460: 696b 6520 7468 6579 2061 7265 2061 6374  ike they are act
-00001470: 7561 6c6c 7920 4253 4420 3320 636c 6175  ually BSD 3 clau
-00001480: 7365 206c 6963 656e 7365 7322 2c0a 2020  se licenses",.  
-00001490: 2020 2020 2272 6576 6965 7765 7222 3a20      "reviewer": 
-000014a0: 2250 6572 736f 6e3a 204a 6f65 2052 6576  "Person: Joe Rev
-000014b0: 6965 7765 7222 2c0a 2020 2020 2020 2272  iewer",.      "r
-000014c0: 6576 6965 7744 6174 6522 3a20 2232 3031  eviewDate": "201
-000014d0: 302d 3032 2d31 3054 3030 3a30 303a 3030  0-02-10T00:00:00
-000014e0: 5a22 0a20 2020 207d 2c0a 2020 2020 7b0a  Z".    },.    {.
-000014f0: 2020 2020 2020 2263 6f6d 6d65 6e74 223a        "comment":
-00001500: 2022 416e 6f74 6865 7220 6578 616d 706c   "Another exampl
-00001510: 6520 7265 7669 6577 6572 2e22 2c0a 2020  e reviewer.",.  
-00001520: 2020 2020 2272 6576 6965 7765 7222 3a20      "reviewer": 
-00001530: 2250 6572 736f 6e3a 2053 757a 616e 6e65  "Person: Suzanne
-00001540: 2052 6576 6965 7765 7222 2c0a 2020 2020   Reviewer",.    
-00001550: 2020 2272 6576 6965 7744 6174 6522 3a20    "reviewDate": 
-00001560: 2232 3031 312d 3033 2d31 3354 3030 3a30  "2011-03-13T00:0
-00001570: 303a 3030 5a22 0a20 2020 207d 0a20 205d  0:00Z".    }.  ]
-00001580: 2c0a 2020 2268 6173 4578 7472 6163 7465  ,.  "hasExtracte
-00001590: 644c 6963 656e 7369 6e67 496e 666f 7322  dLicensingInfos"
-000015a0: 3a20 5b0a 2020 2020 7b0a 2020 2020 2020  : [.    {.      
-000015b0: 2265 7874 7261 6374 6564 5465 7874 223a  "extractedText":
-000015c0: 2022 5468 6973 2070 6163 6b61 6765 2069   "This package i
-000015d0: 6e63 6c75 6465 7320 7468 6520 4752 4444  ncludes the GRDD
-000015e0: 4c20 7061 7273 6572 2064 6576 656c 6f70  L parser develop
-000015f0: 6564 2062 7920 4865 776c 6574 7420 5061  ed by Hewlett Pa
-00001600: 636b 6172 6420 756e 6465 7220 7468 6520  ckard under the 
-00001610: 666f 6c6c 6f77 696e 6720 6c69 6365 6e73  following licens
-00001620: 653a 5c6e 5c75 3030 6139 2043 6f70 7972  e:\n\u00a9 Copyr
-00001630: 6967 6874 2032 3030 3720 4865 776c 6574  ight 2007 Hewlet
-00001640: 742d 5061 636b 6172 6420 4465 7665 6c6f  t-Packard Develo
-00001650: 706d 656e 7420 436f 6d70 616e 792c 204c  pment Company, L
-00001660: 505c 6e5c 6e52 6564 6973 7472 6962 7574  P\n\nRedistribut
-00001670: 696f 6e20 616e 6420 7573 6520 696e 2073  ion and use in s
-00001680: 6f75 7263 6520 616e 6420 6269 6e61 7279  ource and binary
-00001690: 2066 6f72 6d73 2c20 7769 7468 206f 7220   forms, with or 
-000016a0: 7769 7468 6f75 7420 6d6f 6469 6669 6361  without modifica
-000016b0: 7469 6f6e 2c20 6172 6520 7065 726d 6974  tion, are permit
-000016c0: 7465 6420 7072 6f76 6964 6564 2074 6861  ted provided tha
-000016d0: 7420 7468 6520 666f 6c6c 6f77 696e 6720  t the following 
-000016e0: 636f 6e64 6974 696f 6e73 2061 7265 206d  conditions are m
-000016f0: 6574 3a5c 6e5c 6e52 6564 6973 7472 6962  et:\n\nRedistrib
-00001700: 7574 696f 6e73 206f 6620 736f 7572 6365  utions of source
-00001710: 2063 6f64 6520 6d75 7374 2072 6574 6169   code must retai
-00001720: 6e20 7468 6520 6162 6f76 6520 636f 7079  n the above copy
-00001730: 7269 6768 7420 6e6f 7469 6365 2c20 7468  right notice, th
-00001740: 6973 206c 6973 7420 6f66 2063 6f6e 6469  is list of condi
-00001750: 7469 6f6e 7320 616e 6420 7468 6520 666f  tions and the fo
-00001760: 6c6c 6f77 696e 6720 6469 7363 6c61 696d  llowing disclaim
-00001770: 6572 2e5c 6e52 6564 6973 7472 6962 7574  er.\nRedistribut
-00001780: 696f 6e73 2069 6e20 6269 6e61 7279 2066  ions in binary f
-00001790: 6f72 6d20 6d75 7374 2072 6570 726f 6475  orm must reprodu
-000017a0: 6365 2074 6865 2061 626f 7665 2063 6f70  ce the above cop
-000017b0: 7972 6967 6874 206e 6f74 6963 652c 2074  yright notice, t
-000017c0: 6869 7320 6c69 7374 206f 6620 636f 6e64  his list of cond
-000017d0: 6974 696f 6e73 2061 6e64 2074 6865 2066  itions and the f
-000017e0: 6f6c 6c6f 7769 6e67 2064 6973 636c 6169  ollowing disclai
-000017f0: 6d65 7220 696e 2074 6865 2064 6f63 756d  mer in the docum
-00001800: 656e 7461 7469 6f6e 2061 6e64 2f6f 7220  entation and/or 
-00001810: 6f74 6865 7220 6d61 7465 7269 616c 7320  other materials 
-00001820: 7072 6f76 6964 6564 2077 6974 6820 7468  provided with th
-00001830: 6520 6469 7374 7269 6275 7469 6f6e 2e5c  e distribution.\
-00001840: 6e54 6865 206e 616d 6520 6f66 2074 6865  nThe name of the
-00001850: 2061 7574 686f 7220 6d61 7920 6e6f 7420   author may not 
-00001860: 6265 2075 7365 6420 746f 2065 6e64 6f72  be used to endor
-00001870: 7365 206f 7220 7072 6f6d 6f74 6520 7072  se or promote pr
-00001880: 6f64 7563 7473 2064 6572 6976 6564 2066  oducts derived f
-00001890: 726f 6d20 7468 6973 2073 6f66 7477 6172  rom this softwar
-000018a0: 6520 7769 7468 6f75 7420 7370 6563 6966  e without specif
-000018b0: 6963 2070 7269 6f72 2077 7269 7474 656e  ic prior written
-000018c0: 2070 6572 6d69 7373 696f 6e2e 5c6e 5448   permission.\nTH
-000018d0: 4953 2053 4f46 5457 4152 4520 4953 2050  IS SOFTWARE IS P
-000018e0: 524f 5649 4445 4420 4259 2054 4845 2041  ROVIDED BY THE A
-000018f0: 5554 484f 5220 6060 4153 2049 5327 2720  UTHOR ``AS IS'' 
-00001900: 414e 4420 414e 5920 4558 5052 4553 5320  AND ANY EXPRESS 
-00001910: 4f52 2049 4d50 4c49 4544 2057 4152 5241  OR IMPLIED WARRA
-00001920: 4e54 4945 532c 2049 4e43 4c55 4449 4e47  NTIES, INCLUDING
-00001930: 2c20 4255 5420 4e4f 5420 4c49 4d49 5445  , BUT NOT LIMITE
-00001940: 4420 544f 2c20 5448 4520 494d 504c 4945  D TO, THE IMPLIE
-00001950: 4420 5741 5252 414e 5449 4553 204f 4620  D WARRANTIES OF 
-00001960: 4d45 5243 4841 4e54 4142 494c 4954 5920  MERCHANTABILITY 
-00001970: 414e 4420 4649 544e 4553 5320 464f 5220  AND FITNESS FOR 
-00001980: 4120 5041 5254 4943 554c 4152 2050 5552  A PARTICULAR PUR
-00001990: 504f 5345 2041 5245 2044 4953 434c 4149  POSE ARE DISCLAI
-000019a0: 4d45 442e 2049 4e20 4e4f 2045 5645 4e54  MED. IN NO EVENT
-000019b0: 2053 4841 4c4c 2054 4845 2041 5554 484f   SHALL THE AUTHO
-000019c0: 5220 4245 204c 4941 424c 4520 464f 5220  R BE LIABLE FOR 
-000019d0: 414e 5920 4449 5245 4354 2c20 494e 4449  ANY DIRECT, INDI
-000019e0: 5245 4354 2c20 494e 4349 4445 4e54 414c  RECT, INCIDENTAL
-000019f0: 2c20 5350 4543 4941 4c2c 2045 5845 4d50  , SPECIAL, EXEMP
-00001a00: 4c41 5259 2c20 4f52 2043 4f4e 5345 5155  LARY, OR CONSEQU
-00001a10: 454e 5449 414c 2044 414d 4147 4553 2028  ENTIAL DAMAGES (
-00001a20: 494e 434c 5544 494e 472c 2042 5554 204e  INCLUDING, BUT N
-00001a30: 4f54 204c 494d 4954 4544 2054 4f2c 2050  OT LIMITED TO, P
-00001a40: 524f 4355 5245 4d45 4e54 204f 4620 5355  ROCUREMENT OF SU
-00001a50: 4253 5449 5455 5445 2047 4f4f 4453 204f  BSTITUTE GOODS O
-00001a60: 5220 5345 5256 4943 4553 3b20 4c4f 5353  R SERVICES; LOSS
-00001a70: 204f 4620 5553 452c 2044 4154 412c 204f   OF USE, DATA, O
-00001a80: 5220 5052 4f46 4954 533b 204f 5220 4255  R PROFITS; OR BU
-00001a90: 5349 4e45 5353 2049 4e54 4552 5255 5054  SINESS INTERRUPT
-00001aa0: 494f 4e29 2048 4f57 4556 4552 2043 4155  ION) HOWEVER CAU
-00001ab0: 5345 4420 414e 4420 4f4e 2041 4e59 2054  SED AND ON ANY T
-00001ac0: 4845 4f52 5920 4f46 204c 4941 4249 4c49  HEORY OF LIABILI
-00001ad0: 5459 2c20 5748 4554 4845 5220 494e 2043  TY, WHETHER IN C
-00001ae0: 4f4e 5452 4143 542c 2053 5452 4943 5420  ONTRACT, STRICT 
-00001af0: 4c49 4142 494c 4954 592c 204f 5220 544f  LIABILITY, OR TO
-00001b00: 5254 2028 494e 434c 5544 494e 4720 4e45  RT (INCLUDING NE
-00001b10: 474c 4947 454e 4345 204f 5220 4f54 4845  GLIGENCE OR OTHE
-00001b20: 5257 4953 4529 2041 5249 5349 4e47 2049  RWISE) ARISING I
-00001b30: 4e20 414e 5920 5741 5920 4f55 5420 4f46  N ANY WAY OUT OF
-00001b40: 2054 4845 2055 5345 204f 4620 5448 4953   THE USE OF THIS
-00001b50: 2053 4f46 5457 4152 452c 2045 5645 4e20   SOFTWARE, EVEN 
-00001b60: 4946 2041 4456 4953 4544 204f 4620 5448  IF ADVISED OF TH
-00001b70: 4520 504f 5353 4942 494c 4954 5920 4f46  E POSSIBILITY OF
-00001b80: 2053 5543 4820 4441 4d41 4745 2e20 222c   SUCH DAMAGE. ",
-00001b90: 0a20 2020 2020 2022 6c69 6365 6e73 6549  .      "licenseI
-00001ba0: 6422 3a20 224c 6963 656e 7365 5265 662d  d": "LicenseRef-
-00001bb0: 3222 0a20 2020 207d 2c0a 2020 2020 7b0a  2".    },.    {.
-00001bc0: 2020 2020 2020 2265 7874 7261 6374 6564        "extracted
-00001bd0: 5465 7874 223a 2022 5468 6520 4379 6265  Text": "The Cybe
-00001be0: 724e 656b 6f20 536f 6674 7761 7265 204c  rNeko Software L
-00001bf0: 6963 656e 7365 2c20 5665 7273 696f 6e20  icense, Version 
-00001c00: 312e 305c 6e5c 6e5c 6e28 4329 2043 6f70  1.0\n\n\n(C) Cop
-00001c10: 7972 6967 6874 2032 3030 322d 3230 3035  yright 2002-2005
-00001c20: 2c20 416e 6479 2043 6c61 726b 2e20 2041  , Andy Clark.  A
-00001c30: 6c6c 2072 6967 6874 7320 7265 7365 7276  ll rights reserv
-00001c40: 6564 2e5c 6e5c 6e52 6564 6973 7472 6962  ed.\n\nRedistrib
-00001c50: 7574 696f 6e20 616e 6420 7573 6520 696e  ution and use in
-00001c60: 2073 6f75 7263 6520 616e 6420 6269 6e61   source and bina
-00001c70: 7279 2066 6f72 6d73 2c20 7769 7468 206f  ry forms, with o
-00001c80: 7220 7769 7468 6f75 745c 6e6d 6f64 6966  r without\nmodif
-00001c90: 6963 6174 696f 6e2c 2061 7265 2070 6572  ication, are per
-00001ca0: 6d69 7474 6564 2070 726f 7669 6465 6420  mitted provided 
-00001cb0: 7468 6174 2074 6865 2066 6f6c 6c6f 7769  that the followi
-00001cc0: 6e67 2063 6f6e 6469 7469 6f6e 735c 6e61  ng conditions\na
-00001cd0: 7265 206d 6574 3a5c 6e5c 6e31 2e20 5265  re met:\n\n1. Re
-00001ce0: 6469 7374 7269 6275 7469 6f6e 7320 6f66  distributions of
-00001cf0: 2073 6f75 7263 6520 636f 6465 206d 7573   source code mus
-00001d00: 7420 7265 7461 696e 2074 6865 2061 626f  t retain the abo
-00001d10: 7665 2063 6f70 7972 6967 6874 5c6e 2020  ve copyright\n  
-00001d20: 206e 6f74 6963 652c 2074 6869 7320 6c69   notice, this li
-00001d30: 7374 206f 6620 636f 6e64 6974 696f 6e73  st of conditions
-00001d40: 2061 6e64 2074 6865 2066 6f6c 6c6f 7769   and the followi
-00001d50: 6e67 2064 6973 636c 6169 6d65 722e 5c6e  ng disclaimer.\n
-00001d60: 5c6e 322e 2052 6564 6973 7472 6962 7574  \n2. Redistribut
-00001d70: 696f 6e73 2069 6e20 6269 6e61 7279 2066  ions in binary f
-00001d80: 6f72 6d20 6d75 7374 2072 6570 726f 6475  orm must reprodu
-00001d90: 6365 2074 6865 2061 626f 7665 2063 6f70  ce the above cop
-00001da0: 7972 6967 6874 5c6e 2020 206e 6f74 6963  yright\n   notic
-00001db0: 652c 2074 6869 7320 6c69 7374 206f 6620  e, this list of 
-00001dc0: 636f 6e64 6974 696f 6e73 2061 6e64 2074  conditions and t
-00001dd0: 6865 2066 6f6c 6c6f 7769 6e67 2064 6973  he following dis
-00001de0: 636c 6169 6d65 7220 696e 5c6e 2020 2074  claimer in\n   t
-00001df0: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
-00001e00: 2061 6e64 2f6f 7220 6f74 6865 7220 6d61   and/or other ma
-00001e10: 7465 7269 616c 7320 7072 6f76 6964 6564  terials provided
-00001e20: 2077 6974 6820 7468 655c 6e20 2020 6469   with the\n   di
-00001e30: 7374 7269 6275 7469 6f6e 2e5c 6e5c 6e33  stribution.\n\n3
-00001e40: 2e20 5468 6520 656e 642d 7573 6572 2064  . The end-user d
-00001e50: 6f63 756d 656e 7461 7469 6f6e 2069 6e63  ocumentation inc
-00001e60: 6c75 6465 6420 7769 7468 2074 6865 2072  luded with the r
-00001e70: 6564 6973 7472 6962 7574 696f 6e2c 5c6e  edistribution,\n
-00001e80: 2020 2069 6620 616e 792c 206d 7573 7420     if any, must 
-00001e90: 696e 636c 7564 6520 7468 6520 666f 6c6c  include the foll
-00001ea0: 6f77 696e 6720 6163 6b6e 6f77 6c65 6467  owing acknowledg
-00001eb0: 6d65 6e74 3a5c 6e20 2020 2020 5c22 5468  ment:\n     \"Th
-00001ec0: 6973 2070 726f 6475 6374 2069 6e63 6c75  is product inclu
-00001ed0: 6465 7320 736f 6674 7761 7265 2064 6576  des software dev
-00001ee0: 656c 6f70 6564 2062 7920 416e 6479 2043  eloped by Andy C
-00001ef0: 6c61 726b 2e5c 225c 6e20 2020 416c 7465  lark.\"\n   Alte
-00001f00: 726e 6174 656c 792c 2074 6869 7320 6163  rnately, this ac
-00001f10: 6b6e 6f77 6c65 6467 6d65 6e74 206d 6179  knowledgment may
-00001f20: 2061 7070 6561 7220 696e 2074 6865 2073   appear in the s
-00001f30: 6f66 7477 6172 6520 6974 7365 6c66 2c5c  oftware itself,\
-00001f40: 6e20 2020 6966 2061 6e64 2077 6865 7265  n   if and where
-00001f50: 7665 7220 7375 6368 2074 6869 7264 2d70  ver such third-p
-00001f60: 6172 7479 2061 636b 6e6f 776c 6564 676d  arty acknowledgm
-00001f70: 656e 7473 206e 6f72 6d61 6c6c 7920 6170  ents normally ap
-00001f80: 7065 6172 2e5c 6e5c 6e34 2e20 5468 6520  pear.\n\n4. The 
-00001f90: 6e61 6d65 7320 5c22 4379 6265 724e 656b  names \"CyberNek
-00001fa0: 6f5c 2220 616e 6420 5c22 4e65 6b6f 4854  o\" and \"NekoHT
-00001fb0: 4d4c 5c22 206d 7573 7420 6e6f 7420 6265  ML\" must not be
-00001fc0: 2075 7365 6420 746f 2065 6e64 6f72 7365   used to endorse
-00001fd0: 5c6e 2020 206f 7220 7072 6f6d 6f74 6520  \n   or promote 
-00001fe0: 7072 6f64 7563 7473 2064 6572 6976 6564  products derived
-00001ff0: 2066 726f 6d20 7468 6973 2073 6f66 7477   from this softw
-00002000: 6172 6520 7769 7468 6f75 7420 7072 696f  are without prio
-00002010: 725c 6e20 2020 7772 6974 7465 6e20 7065  r\n   written pe
-00002020: 726d 6973 7369 6f6e 2e20 466f 7220 7772  rmission. For wr
-00002030: 6974 7465 6e20 7065 726d 6973 7369 6f6e  itten permission
-00002040: 2c20 706c 6561 7365 2063 6f6e 7461 6374  , please contact
-00002050: 5c6e 2020 2061 6e64 7963 4063 7962 6572  \n   andyc@cyber
-00002060: 6e65 6b6f 2e6e 6574 2e5c 6e5c 6e35 2e20  neko.net.\n\n5. 
-00002070: 5072 6f64 7563 7473 2064 6572 6976 6564  Products derived
-00002080: 2066 726f 6d20 7468 6973 2073 6f66 7477   from this softw
-00002090: 6172 6520 6d61 7920 6e6f 7420 6265 2063  are may not be c
-000020a0: 616c 6c65 6420 5c22 4379 6265 724e 656b  alled \"CyberNek
-000020b0: 6f5c 222c 5c6e 2020 206e 6f72 206d 6179  o\",\n   nor may
-000020c0: 205c 2243 7962 6572 4e65 6b6f 5c22 2061   \"CyberNeko\" a
-000020d0: 7070 6561 7220 696e 2074 6865 6972 206e  ppear in their n
-000020e0: 616d 652c 2077 6974 686f 7574 2070 7269  ame, without pri
-000020f0: 6f72 2077 7269 7474 656e 5c6e 2020 2070  or written\n   p
-00002100: 6572 6d69 7373 696f 6e20 6f66 2074 6865  ermission of the
-00002110: 2061 7574 686f 722e 5c6e 5c6e 5448 4953   author.\n\nTHIS
-00002120: 2053 4f46 5457 4152 4520 4953 2050 524f   SOFTWARE IS PRO
-00002130: 5649 4445 4420 6060 4153 2049 5327 2720  VIDED ``AS IS'' 
-00002140: 414e 4420 414e 5920 4558 5052 4553 5345  AND ANY EXPRESSE
-00002150: 4420 4f52 2049 4d50 4c49 4544 5c6e 5741  D OR IMPLIED\nWA
-00002160: 5252 414e 5449 4553 2c20 494e 434c 5544  RRANTIES, INCLUD
-00002170: 494e 472c 2042 5554 204e 4f54 204c 494d  ING, BUT NOT LIM
-00002180: 4954 4544 2054 4f2c 2054 4845 2049 4d50  ITED TO, THE IMP
-00002190: 4c49 4544 2057 4152 5241 4e54 4945 535c  LIED WARRANTIES\
-000021a0: 6e4f 4620 4d45 5243 4841 4e54 4142 494c  nOF MERCHANTABIL
-000021b0: 4954 5920 414e 4420 4649 544e 4553 5320  ITY AND FITNESS 
-000021c0: 464f 5220 4120 5041 5254 4943 554c 4152  FOR A PARTICULAR
-000021d0: 2050 5552 504f 5345 2041 5245 5c6e 4449   PURPOSE ARE\nDI
-000021e0: 5343 4c41 494d 4544 2e20 2049 4e20 4e4f  SCLAIMED.  IN NO
-000021f0: 2045 5645 4e54 2053 4841 4c4c 2054 4845   EVENT SHALL THE
-00002200: 2041 5554 484f 5220 4f52 204f 5448 4552   AUTHOR OR OTHER
-00002210: 2043 4f4e 5452 4942 5554 4f52 535c 6e42   CONTRIBUTORS\nB
-00002220: 4520 4c49 4142 4c45 2046 4f52 2041 4e59  E LIABLE FOR ANY
-00002230: 2044 4952 4543 542c 2049 4e44 4952 4543   DIRECT, INDIREC
-00002240: 542c 2049 4e43 4944 454e 5441 4c2c 2053  T, INCIDENTAL, S
-00002250: 5045 4349 414c 2c20 4558 454d 504c 4152  PECIAL, EXEMPLAR
-00002260: 592c 5c6e 4f52 2043 4f4e 5345 5155 454e  Y,\nOR CONSEQUEN
-00002270: 5449 414c 2044 414d 4147 4553 2028 494e  TIAL DAMAGES (IN
-00002280: 434c 5544 494e 472c 2042 5554 204e 4f54  CLUDING, BUT NOT
-00002290: 204c 494d 4954 4544 2054 4f2c 2050 524f   LIMITED TO, PRO
-000022a0: 4355 5245 4d45 4e54 5c6e 4f46 2053 5542  CUREMENT\nOF SUB
-000022b0: 5354 4954 5554 4520 474f 4f44 5320 4f52  STITUTE GOODS OR
-000022c0: 2053 4552 5649 4345 533b 204c 4f53 5320   SERVICES; LOSS 
-000022d0: 4f46 2055 5345 2c20 4441 5441 2c20 4f52  OF USE, DATA, OR
-000022e0: 2050 524f 4649 5453 3b20 4f52 5c6e 4255   PROFITS; OR\nBU
-000022f0: 5349 4e45 5353 2049 4e54 4552 5255 5054  SINESS INTERRUPT
-00002300: 494f 4e29 2048 4f57 4556 4552 2043 4155  ION) HOWEVER CAU
-00002310: 5345 4420 414e 4420 4f4e 2041 4e59 2054  SED AND ON ANY T
-00002320: 4845 4f52 5920 4f46 204c 4941 4249 4c49  HEORY OF LIABILI
-00002330: 5459 2c5c 6e57 4845 5448 4552 2049 4e20  TY,\nWHETHER IN 
-00002340: 434f 4e54 5241 4354 2c20 5354 5249 4354  CONTRACT, STRICT
-00002350: 204c 4941 4249 4c49 5459 2c20 4f52 2054   LIABILITY, OR T
-00002360: 4f52 5420 2849 4e43 4c55 4449 4e47 204e  ORT (INCLUDING N
-00002370: 4547 4c49 4745 4e43 455c 6e4f 5220 4f54  EGLIGENCE\nOR OT
-00002380: 4845 5257 4953 4529 2041 5249 5349 4e47  HERWISE) ARISING
-00002390: 2049 4e20 414e 5920 5741 5920 4f55 5420   IN ANY WAY OUT 
-000023a0: 4f46 2054 4845 2055 5345 204f 4620 5448  OF THE USE OF TH
-000023b0: 4953 2053 4f46 5457 4152 452c 5c6e 4556  IS SOFTWARE,\nEV
-000023c0: 454e 2049 4620 4144 5649 5345 4420 4f46  EN IF ADVISED OF
-000023d0: 2054 4845 2050 4f53 5349 4249 4c49 5459   THE POSSIBILITY
-000023e0: 204f 4620 5355 4348 2044 414d 4147 452e   OF SUCH DAMAGE.
-000023f0: 222c 0a20 2020 2020 2022 636f 6d6d 656e  ",.      "commen
-00002400: 7422 3a20 2254 6869 7320 6973 2074 7965  t": "This is tye
-00002410: 2043 7970 6572 4e65 6b6f 204c 6963 656e   CyperNeko Licen
-00002420: 7365 222c 0a20 2020 2020 2022 6c69 6365  se",.      "lice
-00002430: 6e73 6549 6422 3a20 224c 6963 656e 7365  nseId": "License
-00002440: 5265 662d 3322 2c0a 2020 2020 2020 226e  Ref-3",.      "n
-00002450: 616d 6522 3a20 2243 7962 6572 4e65 6b6f  ame": "CyberNeko
-00002460: 204c 6963 656e 7365 222c 0a20 2020 2020   License",.     
-00002470: 2022 7365 6541 6c73 6f73 223a 205b 0a20   "seeAlsos": [. 
-00002480: 2020 2020 2020 2022 6874 7470 3a2f 2f6a         "http://j
-00002490: 7573 7461 7361 6d70 6c65 2e75 726c 2e63  ustasample.url.c
-000024a0: 6f6d 222c 0a20 2020 2020 2020 2022 6874  om",.        "ht
-000024b0: 7470 3a2f 2f70 656f 706c 652e 6170 6163  tp://people.apac
-000024c0: 6865 2e6f 7267 2f7e 616e 6479 632f 6e65  he.org/~andyc/ne
-000024d0: 6b6f 2f4c 4943 454e 5345 220a 2020 2020  ko/LICENSE".    
-000024e0: 2020 5d0a 2020 2020 7d2c 0a20 2020 207b    ].    },.    {
-000024f0: 0a20 2020 2020 2022 6578 7472 6163 7465  .      "extracte
-00002500: 6454 6578 7422 3a20 222f 2a5c 6e20 2a20  dText": "/*\n * 
-00002510: 2863 2920 436f 7079 7269 6768 7420 3230  (c) Copyright 20
-00002520: 3039 2055 6e69 7665 7273 6974 7920 6f66  09 University of
-00002530: 2042 7269 7374 6f6c 5c6e 202a 2041 6c6c   Bristol\n * All
-00002540: 2072 6967 6874 7320 7265 7365 7276 6564   rights reserved
-00002550: 2e5c 6e20 2a5c 6e20 2a20 5265 6469 7374  .\n *\n * Redist
-00002560: 7269 6275 7469 6f6e 2061 6e64 2075 7365  ribution and use
-00002570: 2069 6e20 736f 7572 6365 2061 6e64 2062   in source and b
-00002580: 696e 6172 7920 666f 726d 732c 2077 6974  inary forms, wit
-00002590: 6820 6f72 2077 6974 686f 7574 5c6e 202a  h or without\n *
-000025a0: 206d 6f64 6966 6963 6174 696f 6e2c 2061   modification, a
-000025b0: 7265 2070 6572 6d69 7474 6564 2070 726f  re permitted pro
-000025c0: 7669 6465 6420 7468 6174 2074 6865 2066  vided that the f
-000025d0: 6f6c 6c6f 7769 6e67 2063 6f6e 6469 7469  ollowing conditi
-000025e0: 6f6e 735c 6e20 2a20 6172 6520 6d65 743a  ons\n * are met:
-000025f0: 5c6e 202a 2031 2e20 5265 6469 7374 7269  \n * 1. Redistri
-00002600: 6275 7469 6f6e 7320 6f66 2073 6f75 7263  butions of sourc
-00002610: 6520 636f 6465 206d 7573 7420 7265 7461  e code must reta
-00002620: 696e 2074 6865 2061 626f 7665 2063 6f70  in the above cop
-00002630: 7972 6967 6874 5c6e 202a 2020 2020 6e6f  yright\n *    no
-00002640: 7469 6365 2c20 7468 6973 206c 6973 7420  tice, this list 
-00002650: 6f66 2063 6f6e 6469 7469 6f6e 7320 616e  of conditions an
-00002660: 6420 7468 6520 666f 6c6c 6f77 696e 6720  d the following 
-00002670: 6469 7363 6c61 696d 6572 2e5c 6e20 2a20  disclaimer.\n * 
-00002680: 322e 2052 6564 6973 7472 6962 7574 696f  2. Redistributio
-00002690: 6e73 2069 6e20 6269 6e61 7279 2066 6f72  ns in binary for
-000026a0: 6d20 6d75 7374 2072 6570 726f 6475 6365  m must reproduce
-000026b0: 2074 6865 2061 626f 7665 2063 6f70 7972   the above copyr
-000026c0: 6967 6874 5c6e 202a 2020 2020 6e6f 7469  ight\n *    noti
-000026d0: 6365 2c20 7468 6973 206c 6973 7420 6f66  ce, this list of
-000026e0: 2063 6f6e 6469 7469 6f6e 7320 616e 6420   conditions and 
-000026f0: 7468 6520 666f 6c6c 6f77 696e 6720 6469  the following di
-00002700: 7363 6c61 696d 6572 2069 6e20 7468 655c  sclaimer in the\
-00002710: 6e20 2a20 2020 2064 6f63 756d 656e 7461  n *    documenta
-00002720: 7469 6f6e 2061 6e64 2f6f 7220 6f74 6865  tion and/or othe
-00002730: 7220 6d61 7465 7269 616c 7320 7072 6f76  r materials prov
-00002740: 6964 6564 2077 6974 6820 7468 6520 6469  ided with the di
-00002750: 7374 7269 6275 7469 6f6e 2e5c 6e20 2a20  stribution.\n * 
-00002760: 332e 2054 6865 206e 616d 6520 6f66 2074  3. The name of t
-00002770: 6865 2061 7574 686f 7220 6d61 7920 6e6f  he author may no
-00002780: 7420 6265 2075 7365 6420 746f 2065 6e64  t be used to end
-00002790: 6f72 7365 206f 7220 7072 6f6d 6f74 6520  orse or promote 
-000027a0: 7072 6f64 7563 7473 5c6e 202a 2020 2020  products\n *    
-000027b0: 6465 7269 7665 6420 6672 6f6d 2074 6869  derived from thi
-000027c0: 7320 736f 6674 7761 7265 2077 6974 686f  s software witho
-000027d0: 7574 2073 7065 6369 6669 6320 7072 696f  ut specific prio
-000027e0: 7220 7772 6974 7465 6e20 7065 726d 6973  r written permis
-000027f0: 7369 6f6e 2e5c 6e20 2a5c 6e20 2a20 5448  sion.\n *\n * TH
-00002800: 4953 2053 4f46 5457 4152 4520 4953 2050  IS SOFTWARE IS P
-00002810: 524f 5649 4445 4420 4259 2054 4845 2041  ROVIDED BY THE A
-00002820: 5554 484f 5220 6060 4153 2049 5327 2720  UTHOR ``AS IS'' 
-00002830: 414e 4420 414e 5920 4558 5052 4553 5320  AND ANY EXPRESS 
-00002840: 4f52 5c6e 202a 2049 4d50 4c49 4544 2057  OR\n * IMPLIED W
-00002850: 4152 5241 4e54 4945 532c 2049 4e43 4c55  ARRANTIES, INCLU
-00002860: 4449 4e47 2c20 4255 5420 4e4f 5420 4c49  DING, BUT NOT LI
-00002870: 4d49 5445 4420 544f 2c20 5448 4520 494d  MITED TO, THE IM
-00002880: 504c 4945 4420 5741 5252 414e 5449 4553  PLIED WARRANTIES
-00002890: 5c6e 202a 204f 4620 4d45 5243 4841 4e54  \n * OF MERCHANT
-000028a0: 4142 494c 4954 5920 414e 4420 4649 544e  ABILITY AND FITN
-000028b0: 4553 5320 464f 5220 4120 5041 5254 4943  ESS FOR A PARTIC
-000028c0: 554c 4152 2050 5552 504f 5345 2041 5245  ULAR PURPOSE ARE
-000028d0: 2044 4953 434c 4149 4d45 442e 5c6e 202a   DISCLAIMED.\n *
-000028e0: 2049 4e20 4e4f 2045 5645 4e54 2053 4841   IN NO EVENT SHA
-000028f0: 4c4c 2054 4845 2041 5554 484f 5220 4245  LL THE AUTHOR BE
-00002900: 204c 4941 424c 4520 464f 5220 414e 5920   LIABLE FOR ANY 
-00002910: 4449 5245 4354 2c20 494e 4449 5245 4354  DIRECT, INDIRECT
-00002920: 2c5c 6e20 2a20 494e 4349 4445 4e54 414c  ,\n * INCIDENTAL
-00002930: 2c20 5350 4543 4941 4c2c 2045 5845 4d50  , SPECIAL, EXEMP
-00002940: 4c41 5259 2c20 4f52 2043 4f4e 5345 5155  LARY, OR CONSEQU
-00002950: 454e 5449 414c 2044 414d 4147 4553 2028  ENTIAL DAMAGES (
-00002960: 494e 434c 5544 494e 472c 2042 5554 5c6e  INCLUDING, BUT\n
-00002970: 202a 204e 4f54 204c 494d 4954 4544 2054   * NOT LIMITED T
-00002980: 4f2c 2050 524f 4355 5245 4d45 4e54 204f  O, PROCUREMENT O
-00002990: 4620 5355 4253 5449 5455 5445 2047 4f4f  F SUBSTITUTE GOO
-000029a0: 4453 204f 5220 5345 5256 4943 4553 3b20  DS OR SERVICES; 
-000029b0: 4c4f 5353 204f 4620 5553 452c 5c6e 202a  LOSS OF USE,\n *
-000029c0: 2044 4154 412c 204f 5220 5052 4f46 4954   DATA, OR PROFIT
-000029d0: 533b 204f 5220 4255 5349 4e45 5353 2049  S; OR BUSINESS I
-000029e0: 4e54 4552 5255 5054 494f 4e29 2048 4f57  NTERRUPTION) HOW
-000029f0: 4556 4552 2043 4155 5345 4420 414e 4420  EVER CAUSED AND 
-00002a00: 4f4e 2041 4e59 5c6e 202a 2054 4845 4f52  ON ANY\n * THEOR
-00002a10: 5920 4f46 204c 4941 4249 4c49 5459 2c20  Y OF LIABILITY, 
-00002a20: 5748 4554 4845 5220 494e 2043 4f4e 5452  WHETHER IN CONTR
-00002a30: 4143 542c 2053 5452 4943 5420 4c49 4142  ACT, STRICT LIAB
-00002a40: 494c 4954 592c 204f 5220 544f 5254 5c6e  ILITY, OR TORT\n
-00002a50: 202a 2028 494e 434c 5544 494e 4720 4e45   * (INCLUDING NE
-00002a60: 474c 4947 454e 4345 204f 5220 4f54 4845  GLIGENCE OR OTHE
-00002a70: 5257 4953 4529 2041 5249 5349 4e47 2049  RWISE) ARISING I
-00002a80: 4e20 414e 5920 5741 5920 4f55 5420 4f46  N ANY WAY OUT OF
-00002a90: 2054 4845 2055 5345 204f 465c 6e20 2a20   THE USE OF\n * 
-00002aa0: 5448 4953 2053 4f46 5457 4152 452c 2045  THIS SOFTWARE, E
-00002ab0: 5645 4e20 4946 2041 4456 4953 4544 204f  VEN IF ADVISED O
-00002ac0: 4620 5448 4520 504f 5353 4942 494c 4954  F THE POSSIBILIT
-00002ad0: 5920 4f46 2053 5543 4820 4441 4d41 4745  Y OF SUCH DAMAGE
-00002ae0: 2e5c 6e20 2a2f 2020 222c 0a20 2020 2020  .\n */  ",.     
-00002af0: 2022 6c69 6365 6e73 6549 6422 3a20 224c   "licenseId": "L
-00002b00: 6963 656e 7365 5265 662d 3422 0a20 2020  icenseRef-4".   
-00002b10: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
-00002b20: 2265 7874 7261 6374 6564 5465 7874 223a  "extractedText":
-00002b30: 2022 2f2a 5c6e 202a 2028 6329 2043 6f70   "/*\n * (c) Cop
-00002b40: 7972 6967 6874 2032 3030 302c 2032 3030  yright 2000, 200
-00002b50: 312c 2032 3030 322c 2032 3030 332c 2032  1, 2002, 2003, 2
-00002b60: 3030 342c 2032 3030 352c 2032 3030 362c  004, 2005, 2006,
-00002b70: 2032 3030 372c 2032 3030 382c 2032 3030   2007, 2008, 200
-00002b80: 3920 4865 776c 6574 742d 5061 636b 6172  9 Hewlett-Packar
-00002b90: 6420 4465 7665 6c6f 706d 656e 7420 436f  d Development Co
-00002ba0: 6d70 616e 792c 204c 505c 6e20 2a20 416c  mpany, LP\n * Al
-00002bb0: 6c20 7269 6768 7473 2072 6573 6572 7665  l rights reserve
-00002bc0: 642e 5c6e 202a 5c6e 202a 2052 6564 6973  d.\n *\n * Redis
-00002bd0: 7472 6962 7574 696f 6e20 616e 6420 7573  tribution and us
-00002be0: 6520 696e 2073 6f75 7263 6520 616e 6420  e in source and 
-00002bf0: 6269 6e61 7279 2066 6f72 6d73 2c20 7769  binary forms, wi
-00002c00: 7468 206f 7220 7769 7468 6f75 745c 6e20  th or without\n 
-00002c10: 2a20 6d6f 6469 6669 6361 7469 6f6e 2c20  * modification, 
-00002c20: 6172 6520 7065 726d 6974 7465 6420 7072  are permitted pr
-00002c30: 6f76 6964 6564 2074 6861 7420 7468 6520  ovided that the 
-00002c40: 666f 6c6c 6f77 696e 6720 636f 6e64 6974  following condit
-00002c50: 696f 6e73 5c6e 202a 2061 7265 206d 6574  ions\n * are met
-00002c60: 3a5c 6e20 2a20 312e 2052 6564 6973 7472  :\n * 1. Redistr
-00002c70: 6962 7574 696f 6e73 206f 6620 736f 7572  ibutions of sour
-00002c80: 6365 2063 6f64 6520 6d75 7374 2072 6574  ce code must ret
-00002c90: 6169 6e20 7468 6520 6162 6f76 6520 636f  ain the above co
-00002ca0: 7079 7269 6768 745c 6e20 2a20 2020 206e  pyright\n *    n
-00002cb0: 6f74 6963 652c 2074 6869 7320 6c69 7374  otice, this list
-00002cc0: 206f 6620 636f 6e64 6974 696f 6e73 2061   of conditions a
-00002cd0: 6e64 2074 6865 2066 6f6c 6c6f 7769 6e67  nd the following
-00002ce0: 2064 6973 636c 6169 6d65 722e 5c6e 202a   disclaimer.\n *
-00002cf0: 2032 2e20 5265 6469 7374 7269 6275 7469   2. Redistributi
-00002d00: 6f6e 7320 696e 2062 696e 6172 7920 666f  ons in binary fo
-00002d10: 726d 206d 7573 7420 7265 7072 6f64 7563  rm must reproduc
-00002d20: 6520 7468 6520 6162 6f76 6520 636f 7079  e the above copy
-00002d30: 7269 6768 745c 6e20 2a20 2020 206e 6f74  right\n *    not
-00002d40: 6963 652c 2074 6869 7320 6c69 7374 206f  ice, this list o
-00002d50: 6620 636f 6e64 6974 696f 6e73 2061 6e64  f conditions and
-00002d60: 2074 6865 2066 6f6c 6c6f 7769 6e67 2064   the following d
-00002d70: 6973 636c 6169 6d65 7220 696e 2074 6865  isclaimer in the
-00002d80: 5c6e 202a 2020 2020 646f 6375 6d65 6e74  \n *    document
-00002d90: 6174 696f 6e20 616e 642f 6f72 206f 7468  ation and/or oth
-00002da0: 6572 206d 6174 6572 6961 6c73 2070 726f  er materials pro
-00002db0: 7669 6465 6420 7769 7468 2074 6865 2064  vided with the d
-00002dc0: 6973 7472 6962 7574 696f 6e2e 5c6e 202a  istribution.\n *
-00002dd0: 2033 2e20 5468 6520 6e61 6d65 206f 6620   3. The name of 
-00002de0: 7468 6520 6175 7468 6f72 206d 6179 206e  the author may n
-00002df0: 6f74 2062 6520 7573 6564 2074 6f20 656e  ot be used to en
-00002e00: 646f 7273 6520 6f72 2070 726f 6d6f 7465  dorse or promote
-00002e10: 2070 726f 6475 6374 735c 6e20 2a20 2020   products\n *   
-00002e20: 2064 6572 6976 6564 2066 726f 6d20 7468   derived from th
-00002e30: 6973 2073 6f66 7477 6172 6520 7769 7468  is software with
-00002e40: 6f75 7420 7370 6563 6966 6963 2070 7269  out specific pri
-00002e50: 6f72 2077 7269 7474 656e 2070 6572 6d69  or written permi
-00002e60: 7373 696f 6e2e 5c6e 202a 5c6e 202a 2054  ssion.\n *\n * T
-00002e70: 4849 5320 534f 4654 5741 5245 2049 5320  HIS SOFTWARE IS 
-00002e80: 5052 4f56 4944 4544 2042 5920 5448 4520  PROVIDED BY THE 
-00002e90: 4155 5448 4f52 2060 6041 5320 4953 2727  AUTHOR ``AS IS''
-00002ea0: 2041 4e44 2041 4e59 2045 5850 5245 5353   AND ANY EXPRESS
-00002eb0: 204f 525c 6e20 2a20 494d 504c 4945 4420   OR\n * IMPLIED 
-00002ec0: 5741 5252 414e 5449 4553 2c20 494e 434c  WARRANTIES, INCL
-00002ed0: 5544 494e 472c 2042 5554 204e 4f54 204c  UDING, BUT NOT L
-00002ee0: 494d 4954 4544 2054 4f2c 2054 4845 2049  IMITED TO, THE I
-00002ef0: 4d50 4c49 4544 2057 4152 5241 4e54 4945  MPLIED WARRANTIE
-00002f00: 535c 6e20 2a20 4f46 204d 4552 4348 414e  S\n * OF MERCHAN
-00002f10: 5441 4249 4c49 5459 2041 4e44 2046 4954  TABILITY AND FIT
-00002f20: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
-00002f30: 4355 4c41 5220 5055 5250 4f53 4520 4152  CULAR PURPOSE AR
-00002f40: 4520 4449 5343 4c41 494d 4544 2e5c 6e20  E DISCLAIMED.\n 
-00002f50: 2a20 494e 204e 4f20 4556 454e 5420 5348  * IN NO EVENT SH
-00002f60: 414c 4c20 5448 4520 4155 5448 4f52 2042  ALL THE AUTHOR B
-00002f70: 4520 4c49 4142 4c45 2046 4f52 2041 4e59  E LIABLE FOR ANY
-00002f80: 2044 4952 4543 542c 2049 4e44 4952 4543   DIRECT, INDIREC
-00002f90: 542c 5c6e 202a 2049 4e43 4944 454e 5441  T,\n * INCIDENTA
-00002fa0: 4c2c 2053 5045 4349 414c 2c20 4558 454d  L, SPECIAL, EXEM
-00002fb0: 504c 4152 592c 204f 5220 434f 4e53 4551  PLARY, OR CONSEQ
-00002fc0: 5545 4e54 4941 4c20 4441 4d41 4745 5320  UENTIAL DAMAGES 
-00002fd0: 2849 4e43 4c55 4449 4e47 2c20 4255 545c  (INCLUDING, BUT\
-00002fe0: 6e20 2a20 4e4f 5420 4c49 4d49 5445 4420  n * NOT LIMITED 
-00002ff0: 544f 2c20 5052 4f43 5552 454d 454e 5420  TO, PROCUREMENT 
-00003000: 4f46 2053 5542 5354 4954 5554 4520 474f  OF SUBSTITUTE GO
-00003010: 4f44 5320 4f52 2053 4552 5649 4345 533b  ODS OR SERVICES;
-00003020: 204c 4f53 5320 4f46 2055 5345 2c5c 6e20   LOSS OF USE,\n 
-00003030: 2a20 4441 5441 2c20 4f52 2050 524f 4649  * DATA, OR PROFI
-00003040: 5453 3b20 4f52 2042 5553 494e 4553 5320  TS; OR BUSINESS 
-00003050: 494e 5445 5252 5550 5449 4f4e 2920 484f  INTERRUPTION) HO
-00003060: 5745 5645 5220 4341 5553 4544 2041 4e44  WEVER CAUSED AND
-00003070: 204f 4e20 414e 595c 6e20 2a20 5448 454f   ON ANY\n * THEO
-00003080: 5259 204f 4620 4c49 4142 494c 4954 592c  RY OF LIABILITY,
-00003090: 2057 4845 5448 4552 2049 4e20 434f 4e54   WHETHER IN CONT
-000030a0: 5241 4354 2c20 5354 5249 4354 204c 4941  RACT, STRICT LIA
-000030b0: 4249 4c49 5459 2c20 4f52 2054 4f52 545c  BILITY, OR TORT\
-000030c0: 6e20 2a20 2849 4e43 4c55 4449 4e47 204e  n * (INCLUDING N
-000030d0: 4547 4c49 4745 4e43 4520 4f52 204f 5448  EGLIGENCE OR OTH
-000030e0: 4552 5749 5345 2920 4152 4953 494e 4720  ERWISE) ARISING 
-000030f0: 494e 2041 4e59 2057 4159 204f 5554 204f  IN ANY WAY OUT O
-00003100: 4620 5448 4520 5553 4520 4f46 5c6e 202a  F THE USE OF\n *
-00003110: 2054 4849 5320 534f 4654 5741 5245 2c20   THIS SOFTWARE, 
-00003120: 4556 454e 2049 4620 4144 5649 5345 4420  EVEN IF ADVISED 
-00003130: 4f46 2054 4845 2050 4f53 5349 4249 4c49  OF THE POSSIBILI
-00003140: 5459 204f 4620 5355 4348 2044 414d 4147  TY OF SUCH DAMAG
-00003150: 452e 5c6e 202a 2f22 2c0a 2020 2020 2020  E.\n */",.      
-00003160: 226c 6963 656e 7365 4964 223a 2022 4c69  "licenseId": "Li
-00003170: 6365 6e73 6552 6566 2d31 220a 2020 2020  censeRef-1".    
-00003180: 7d0a 2020 5d2c 0a20 2022 7370 6478 5665  }.  ],.  "spdxVe
-00003190: 7273 696f 6e22 3a20 2253 5044 582d 322e  rsion": "SPDX-2.
-000031a0: 3122 2c0a 2020 2253 5044 5849 4422 3a20  1",.  "SPDXID": 
-000031b0: 2253 5044 5852 6566 2d44 4f43 554d 454e  "SPDXRef-DOCUMEN
-000031c0: 5422 2c0a 2020 2273 6e69 7070 6574 7322  T",.  "snippets"
-000031d0: 3a20 5b0a 2020 2020 7b0a 2020 2020 2020  : [.    {.      
-000031e0: 2263 6f6d 6d65 6e74 223a 2022 5468 6973  "comment": "This
-000031f0: 2073 6e69 7070 6574 2077 6173 2069 6465   snippet was ide
-00003200: 6e74 6966 6965 6420 6173 2073 6967 6e69  ntified as signi
-00003210: 6669 6361 6e74 2061 6e64 2068 6967 686c  ficant and highl
-00003220: 6967 6874 6564 2069 6e20 7468 6973 2041  ighted in this A
-00003230: 7061 6368 652d 322e 3020 6669 6c65 2c20  pache-2.0 file, 
-00003240: 7768 656e 2061 2063 6f6d 6d65 7263 6961  when a commercia
-00003250: 6c20 7363 616e 6e65 7220 6964 656e 7469  l scanner identi
-00003260: 6669 6564 2069 7420 6173 2062 6569 6e67  fied it as being
-00003270: 2064 6572 6976 6564 2066 726f 6d20 6669   derived from fi
-00003280: 6c65 2066 6f6f 2e63 2069 6e20 7061 636b  le foo.c in pack
-00003290: 6167 6520 7879 7a20 7768 6963 6820 6973  age xyz which is
-000032a0: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
-000032b0: 4750 4c2d 322e 302d 6f72 2d6c 6174 6572  GPL-2.0-or-later
-000032c0: 2e22 2c0a 2020 2020 2020 226e 616d 6522  .",.      "name"
-000032d0: 3a20 2266 726f 6d20 6c69 6e75 7820 6b65  : "from linux ke
-000032e0: 726e 656c 222c 0a20 2020 2020 2022 636f  rnel",.      "co
-000032f0: 7079 7269 6768 7454 6578 7422 3a20 2243  pyrightText": "C
-00003300: 6f70 7972 6967 6874 2032 3030 382d 3230  opyright 2008-20
-00003310: 3130 204a 6f68 6e20 536d 6974 6822 2c0a  10 John Smith",.
-00003320: 2020 2020 2020 226c 6963 656e 7365 436f        "licenseCo
-00003330: 6e63 6c75 6465 6422 3a20 2241 7061 6368  ncluded": "Apach
-00003340: 652d 322e 3022 2c0a 2020 2020 2020 226c  e-2.0",.      "l
-00003350: 6963 656e 7365 496e 666f 496e 536e 6970  icenseInfoInSnip
-00003360: 7065 7473 223a 205b 0a20 2020 2020 2020  pets": [.       
-00003370: 2022 4170 6163 6865 2d32 2e30 222c 0a20   "Apache-2.0",. 
-00003380: 2020 2020 2020 2022 4750 4c2d 322e 302d         "GPL-2.0-
-00003390: 6f6e 6c79 220a 2020 2020 2020 5d2c 0a20  only".      ],. 
-000033a0: 2020 2020 2022 6c69 6365 6e73 6543 6f6d       "licenseCom
-000033b0: 6d65 6e74 7322 3a20 2254 6865 2063 6f6e  ments": "The con
-000033c0: 636c 7564 6564 206c 6963 656e 7365 2077  cluded license w
-000033d0: 6173 2074 616b 656e 2066 726f 6d20 7061  as taken from pa
-000033e0: 636b 6167 6520 7879 7a2c 2066 726f 6d20  ckage xyz, from 
-000033f0: 7768 6963 6820 7468 6520 736e 6970 7065  which the snippe
-00003400: 7420 7761 7320 636f 7069 6564 2069 6e74  t was copied int
-00003410: 6f20 7468 6520 6375 7272 656e 7420 6669  o the current fi
-00003420: 6c65 2e20 5468 6520 636f 6e63 6c75 6465  le. The conclude
-00003430: 6420 6c69 6365 6e73 6520 696e 666f 726d  d license inform
-00003440: 6174 696f 6e20 7761 7320 666f 756e 6420  ation was found 
-00003450: 696e 2074 6865 2043 4f50 5949 4e47 2e74  in the COPYING.t
-00003460: 7874 2066 696c 6520 696e 2070 6163 6b61  xt file in packa
-00003470: 6765 2078 797a 2e22 2c0a 2020 2020 2020  ge xyz.",.      
-00003480: 2253 5044 5849 4422 3a20 2253 5044 5852  "SPDXID": "SPDXR
-00003490: 6566 2d53 6e69 7070 6574 222c 0a20 2020  ef-Snippet",.   
-000034a0: 2020 2022 736e 6970 7065 7446 726f 6d46     "snippetFromF
-000034b0: 696c 6522 3a20 2253 5044 5852 6566 2d44  ile": "SPDXRef-D
-000034c0: 6f61 7053 6f75 7263 6522 2c0a 2020 2020  oapSource",.    
-000034d0: 2020 2020 2272 616e 6765 7322 3a20 5b0a      "ranges": [.
-000034e0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-000034f0: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-00003500: 6e64 506f 696e 7465 7222 3a20 7b0a 2020  ndPointer": {.  
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 2020 226f 6666 7365 7422 3a20 3432 302c    "offset": 420,
-00003530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003540: 2020 2020 2022 7265 6665 7265 6e63 6522       "reference"
-00003550: 3a20 2253 5044 5852 6566 2d44 6f61 7053  : "SPDXRef-DoapS
-00003560: 6f75 7263 6522 0a20 2020 2020 2020 2020  ource".         
-00003570: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00003580: 2020 2020 2020 2020 2020 2273 7461 7274            "start
-00003590: 506f 696e 7465 7222 3a20 7b0a 2020 2020  Pointer": {.    
-000035a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035b0: 226f 6666 7365 7422 3a20 3331 302c 0a20  "offset": 310,. 
-000035c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035d0: 2020 2022 7265 6665 7265 6e63 6522 3a20     "reference": 
-000035e0: 2253 5044 5852 6566 2d44 6f61 7053 6f75  "SPDXRef-DoapSou
-000035f0: 7263 6522 0a20 2020 2020 2020 2020 2020  rce".           
-00003600: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00003610: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00003620: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00003630: 2020 2020 2265 6e64 506f 696e 7465 7222      "endPointer"
-00003640: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00003650: 2020 2020 2020 2020 226c 696e 654e 756d          "lineNum
-00003660: 6265 7222 3a20 3233 2c0a 2020 2020 2020  ber": 23,.      
-00003670: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00003680: 6566 6572 656e 6365 223a 2022 5350 4458  eference": "SPDX
-00003690: 5265 662d 446f 6170 536f 7572 6365 220a  Ref-DoapSource".
-000036a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036b0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-000036c0: 2020 2022 7374 6172 7450 6f69 6e74 6572     "startPointer
-000036d0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-000036e0: 2020 2020 2020 2020 2022 6c69 6e65 4e75           "lineNu
-000036f0: 6d62 6572 223a 2035 2c0a 2020 2020 2020  mber": 5,.      
-00003700: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00003710: 6566 6572 656e 6365 223a 2022 5350 4458  eference": "SPDX
-00003720: 5265 662d 446f 6170 536f 7572 6365 220a  Ref-DoapSource".
-00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003740: 7d0a 2020 2020 2020 2020 2020 2020 7d0a  }.            }.
-00003750: 2020 2020 2020 2020 5d0a 2020 2020 7d0a          ].    }.
-00003760: 2020 5d0a 7d0a                             ].}.
+00000000: 2320 5350 4458 2d46 696c 6543 6f70 7972  # SPDX-FileCopyr
+00000010: 6967 6874 5465 7874 3a20 3230 3232 2073  ightText: 2022 s
+00000020: 7064 7820 636f 6e74 7269 6275 746f 7273  pdx contributors
+00000030: 0a23 0a23 2053 5044 582d 4c69 6365 6e73  .#.# SPDX-Licens
+00000040: 652d 4964 656e 7469 6669 6572 3a20 4170  e-Identifier: Ap
+00000050: 6163 6865 2d32 2e30 0a66 726f 6d20 6461  ache-2.0.from da
+00000060: 7465 7469 6d65 2069 6d70 6f72 7420 6461  tetime import da
+00000070: 7465 7469 6d65 0a66 726f 6d20 756e 6974  tetime.from unit
+00000080: 7465 7374 2069 6d70 6f72 7420 5465 7374  test import Test
+00000090: 4361 7365 0a0a 696d 706f 7274 2070 7974  Case..import pyt
+000000a0: 6573 740a 6672 6f6d 206c 6963 656e 7365  est.from license
+000000b0: 5f65 7870 7265 7373 696f 6e20 696d 706f  _expression impo
+000000c0: 7274 204c 6963 656e 7369 6e67 0a0a 6672  rt Licensing..fr
+000000d0: 6f6d 2073 7064 785f 746f 6f6c 732e 7370  om spdx_tools.sp
+000000e0: 6478 2e6d 6f64 656c 2069 6d70 6f72 7420  dx.model import 
+000000f0: 280a 2020 2020 4163 746f 722c 0a20 2020  (.    Actor,.   
+00000100: 2041 6374 6f72 5479 7065 2c0a 2020 2020   ActorType,.    
+00000110: 4368 6563 6b73 756d 2c0a 2020 2020 4368  Checksum,.    Ch
+00000120: 6563 6b73 756d 416c 676f 7269 7468 6d2c  ecksumAlgorithm,
+00000130: 0a20 2020 2045 7874 6572 6e61 6c50 6163  .    ExternalPac
+00000140: 6b61 6765 5265 662c 0a20 2020 2045 7874  kageRef,.    Ext
+00000150: 6572 6e61 6c50 6163 6b61 6765 5265 6643  ernalPackageRefC
+00000160: 6174 6567 6f72 792c 0a20 2020 2050 6163  ategory,.    Pac
+00000170: 6b61 6765 5075 7270 6f73 652c 0a20 2020  kagePurpose,.   
+00000180: 2050 6163 6b61 6765 5665 7269 6669 6361   PackageVerifica
+00000190: 7469 6f6e 436f 6465 2c0a 2020 2020 5370  tionCode,.    Sp
+000001a0: 6478 4e6f 4173 7365 7274 696f 6e2c 0a20  dxNoAssertion,. 
+000001b0: 2020 2053 7064 784e 6f6e 652c 0a29 0a66     SpdxNone,.).f
+000001c0: 726f 6d20 7370 6478 5f74 6f6f 6c73 2e73  rom spdx_tools.s
+000001d0: 7064 782e 7061 7273 6572 2e65 7272 6f72  pdx.parser.error
+000001e0: 2069 6d70 6f72 7420 5350 4458 5061 7273   import SPDXPars
+000001f0: 696e 6745 7272 6f72 0a66 726f 6d20 7370  ingError.from sp
+00000200: 6478 5f74 6f6f 6c73 2e73 7064 782e 7061  dx_tools.spdx.pa
+00000210: 7273 6572 2e6a 736f 6e6c 696b 6564 6963  rser.jsonlikedic
+00000220: 742e 6469 6374 5f70 6172 7369 6e67 5f66  t.dict_parsing_f
+00000230: 756e 6374 696f 6e73 2069 6d70 6f72 7420  unctions import 
+00000240: 7061 7273 655f 6c69 7374 5f6f 665f 656c  parse_list_of_el
+00000250: 656d 656e 7473 0a66 726f 6d20 7370 6478  ements.from spdx
+00000260: 5f74 6f6f 6c73 2e73 7064 782e 7061 7273  _tools.spdx.pars
+00000270: 6572 2e6a 736f 6e6c 696b 6564 6963 742e  er.jsonlikedict.
+00000280: 7061 636b 6167 655f 7061 7273 6572 2069  package_parser i
+00000290: 6d70 6f72 7420 5061 636b 6167 6550 6172  mport PackagePar
+000002a0: 7365 720a 0a0a 4070 7974 6573 742e 6d61  ser...@pytest.ma
+000002b0: 726b 2e70 6172 616d 6574 7269 7a65 280a  rk.parametrize(.
+000002c0: 2020 2020 2268 6f6d 6570 6167 652c 2065      "homepage, e
+000002d0: 7870 6563 7465 645f 686f 6d65 7061 6765  xpected_homepage
+000002e0: 2c20 646f 776e 6c6f 6164 5f6c 6f63 6174  , download_locat
+000002f0: 696f 6e2c 2065 7870 6563 7465 645f 646f  ion, expected_do
+00000300: 776e 6c6f 6164 5f6c 6f63 6174 696f 6e2c  wnload_location,
+00000310: 2022 0a20 2020 2022 636f 7079 7269 6768   ".    "copyrigh
+00000320: 745f 7465 7874 2c20 6578 7065 6374 6564  t_text, expected
+00000330: 5f63 6f70 7972 6967 6874 5f74 6578 742c  _copyright_text,
+00000340: 206f 7269 6769 6e61 746f 722c 2065 7870   originator, exp
+00000350: 6563 7465 645f 6f72 6967 696e 6174 6f72  ected_originator
+00000360: 2c20 7375 7070 6c69 6572 2c20 6578 7065  , supplier, expe
+00000370: 6374 6564 5f73 7570 706c 6965 7222 2c0a  cted_supplier",.
+00000380: 2020 2020 5b0a 2020 2020 2020 2020 280a      [.        (.
+00000390: 2020 2020 2020 2020 2020 2020 2268 7474              "htt
+000003a0: 703a 2f2f 6674 702e 676e 752e 6f72 672f  p://ftp.gnu.org/
+000003b0: 676e 752f 676c 6962 6322 2c0a 2020 2020  gnu/glibc",.    
+000003c0: 2020 2020 2020 2020 2268 7474 703a 2f2f          "http://
+000003d0: 6674 702e 676e 752e 6f72 672f 676e 752f  ftp.gnu.org/gnu/
+000003e0: 676c 6962 6322 2c0a 2020 2020 2020 2020  glibc",.        
+000003f0: 2020 2020 224e 4f41 5353 4552 5449 4f4e      "NOASSERTION
+00000400: 222c 0a20 2020 2020 2020 2020 2020 2053  ",.            S
+00000410: 7064 784e 6f41 7373 6572 7469 6f6e 2829  pdxNoAssertion()
+00000420: 2c0a 2020 2020 2020 2020 2020 2020 224e  ,.            "N
+00000430: 4f4e 4522 2c0a 2020 2020 2020 2020 2020  ONE",.          
+00000440: 2020 5370 6478 4e6f 6e65 2829 2c0a 2020    SpdxNone(),.  
+00000450: 2020 2020 2020 2020 2020 224f 7267 616e            "Organ
+00000460: 697a 6174 696f 6e3a 2045 7861 6d70 6c65  ization: Example
+00000470: 436f 6465 496e 7370 6563 7420 2863 6f6e  CodeInspect (con
+00000480: 7461 6374 4065 7861 6d70 6c65 2e63 6f6d  tact@example.com
+00000490: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
+000004a0: 4163 746f 7228 4163 746f 7254 7970 652e  Actor(ActorType.
+000004b0: 4f52 4741 4e49 5a41 5449 4f4e 2c20 2245  ORGANIZATION, "E
+000004c0: 7861 6d70 6c65 436f 6465 496e 7370 6563  xampleCodeInspec
+000004d0: 7422 2c20 2263 6f6e 7461 6374 4065 7861  t", "contact@exa
+000004e0: 6d70 6c65 2e63 6f6d 2229 2c0a 2020 2020  mple.com"),.    
+000004f0: 2020 2020 2020 2020 224e 4f41 5353 4552          "NOASSER
+00000500: 5449 4f4e 222c 0a20 2020 2020 2020 2020  TION",.         
+00000510: 2020 2053 7064 784e 6f41 7373 6572 7469     SpdxNoAsserti
+00000520: 6f6e 2829 2c0a 2020 2020 2020 2020 292c  on(),.        ),
+00000530: 0a20 2020 2020 2020 2028 0a20 2020 2020  .        (.     
+00000540: 2020 2020 2020 2022 4e4f 4153 5345 5254         "NOASSERT
+00000550: 494f 4e22 2c0a 2020 2020 2020 2020 2020  ION",.          
+00000560: 2020 5370 6478 4e6f 4173 7365 7274 696f    SpdxNoAssertio
+00000570: 6e28 292c 0a20 2020 2020 2020 2020 2020  n(),.           
+00000580: 2022 4e4f 4e45 222c 0a20 2020 2020 2020   "NONE",.       
+00000590: 2020 2020 2053 7064 784e 6f6e 6528 292c       SpdxNone(),
+000005a0: 0a20 2020 2020 2020 2020 2020 2022 436f  .            "Co
+000005b0: 7079 7269 6768 7420 3230 3038 2d32 3031  pyright 2008-201
+000005c0: 3020 4a6f 686e 2053 6d69 7468 222c 0a20  0 John Smith",. 
+000005d0: 2020 2020 2020 2020 2020 2022 436f 7079             "Copy
+000005e0: 7269 6768 7420 3230 3038 2d32 3031 3020  right 2008-2010 
+000005f0: 4a6f 686e 2053 6d69 7468 222c 0a20 2020  John Smith",.   
+00000600: 2020 2020 2020 2020 204e 6f6e 652c 0a20           None,. 
+00000610: 2020 2020 2020 2020 2020 204e 6f6e 652c             None,
+00000620: 0a20 2020 2020 2020 2020 2020 204e 6f6e  .            Non
+00000630: 652c 0a20 2020 2020 2020 2020 2020 204e  e,.            N
+00000640: 6f6e 652c 0a20 2020 2020 2020 2029 2c0a  one,.        ),.
+00000650: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
+00000660: 2020 2020 2020 224e 4f4e 4522 2c0a 2020        "NONE",.  
+00000670: 2020 2020 2020 2020 2020 5370 6478 4e6f            SpdxNo
+00000680: 6e65 2829 2c0a 2020 2020 2020 2020 2020  ne(),.          
+00000690: 2020 2268 7474 703a 2f2f 6674 702e 676e    "http://ftp.gn
+000006a0: 752e 6f72 672f 676e 752f 676c 6962 632f  u.org/gnu/glibc/
+000006b0: 676c 6962 632d 706f 7274 732d 322e 3135  glibc-ports-2.15
+000006c0: 2e74 6172 2e67 7a22 2c0a 2020 2020 2020  .tar.gz",.      
+000006d0: 2020 2020 2020 2268 7474 703a 2f2f 6674        "http://ft
+000006e0: 702e 676e 752e 6f72 672f 676e 752f 676c  p.gnu.org/gnu/gl
+000006f0: 6962 632f 676c 6962 632d 706f 7274 732d  ibc/glibc-ports-
+00000700: 322e 3135 2e74 6172 2e67 7a22 2c0a 2020  2.15.tar.gz",.  
+00000710: 2020 2020 2020 2020 2020 224e 4f41 5353            "NOASS
+00000720: 4552 5449 4f4e 222c 0a20 2020 2020 2020  ERTION",.       
+00000730: 2020 2020 2053 7064 784e 6f41 7373 6572       SpdxNoAsser
+00000740: 7469 6f6e 2829 2c0a 2020 2020 2020 2020  tion(),.        
+00000750: 2020 2020 224e 4f41 5353 4552 5449 4f4e      "NOASSERTION
+00000760: 222c 0a20 2020 2020 2020 2020 2020 2053  ",.            S
+00000770: 7064 784e 6f41 7373 6572 7469 6f6e 2829  pdxNoAssertion()
+00000780: 2c0a 2020 2020 2020 2020 2020 2020 2250  ,.            "P
+00000790: 6572 736f 6e3a 204a 616e 6520 446f 6520  erson: Jane Doe 
+000007a0: 286a 616e 652e 646f 6540 6578 616d 706c  (jane.doe@exampl
+000007b0: 652e 636f 6d29 222c 0a20 2020 2020 2020  e.com)",.       
+000007c0: 2020 2020 2041 6374 6f72 2841 6374 6f72       Actor(Actor
+000007d0: 5479 7065 2e50 4552 534f 4e2c 2022 4a61  Type.PERSON, "Ja
+000007e0: 6e65 2044 6f65 222c 2022 6a61 6e65 2e64  ne Doe", "jane.d
+000007f0: 6f65 4065 7861 6d70 6c65 2e63 6f6d 2229  oe@example.com")
+00000800: 2c0a 2020 2020 2020 2020 292c 0a20 2020  ,.        ),.   
+00000810: 205d 2c0a 290a 6465 6620 7465 7374 5f70   ],.).def test_p
+00000820: 6172 7365 5f70 6163 6b61 6765 280a 2020  arse_package(.  
+00000830: 2020 686f 6d65 7061 6765 2c0a 2020 2020    homepage,.    
+00000840: 6578 7065 6374 6564 5f68 6f6d 6570 6167  expected_homepag
+00000850: 652c 0a20 2020 2064 6f77 6e6c 6f61 645f  e,.    download_
+00000860: 6c6f 6361 7469 6f6e 2c0a 2020 2020 6578  location,.    ex
+00000870: 7065 6374 6564 5f64 6f77 6e6c 6f61 645f  pected_download_
+00000880: 6c6f 6361 7469 6f6e 2c0a 2020 2020 636f  location,.    co
+00000890: 7079 7269 6768 745f 7465 7874 2c0a 2020  pyright_text,.  
+000008a0: 2020 6578 7065 6374 6564 5f63 6f70 7972    expected_copyr
+000008b0: 6967 6874 5f74 6578 742c 0a20 2020 206f  ight_text,.    o
+000008c0: 7269 6769 6e61 746f 722c 0a20 2020 2065  riginator,.    e
+000008d0: 7870 6563 7465 645f 6f72 6967 696e 6174  xpected_originat
+000008e0: 6f72 2c0a 2020 2020 7375 7070 6c69 6572  or,.    supplier
+000008f0: 2c0a 2020 2020 6578 7065 6374 6564 5f73  ,.    expected_s
+00000900: 7570 706c 6965 722c 0a29 3a0a 2020 2020  upplier,.):.    
+00000910: 7061 636b 6167 655f 7061 7273 6572 203d  package_parser =
+00000920: 2050 6163 6b61 6765 5061 7273 6572 2829   PackageParser()
+00000930: 0a0a 2020 2020 7061 636b 6167 655f 6469  ..    package_di
+00000940: 6374 203d 207b 0a20 2020 2020 2020 2022  ct = {.        "
+00000950: 5350 4458 4944 223a 2022 5350 4458 5265  SPDXID": "SPDXRe
+00000960: 662d 5061 636b 6167 6522 2c0a 2020 2020  f-Package",.    
+00000970: 2020 2020 2261 7474 7269 6275 7469 6f6e      "attribution
+00000980: 5465 7874 7322 3a20 5b0a 2020 2020 2020  Texts": [.      
+00000990: 2020 2020 2020 2254 6865 2047 4e55 2043        "The GNU C
+000009a0: 204c 6962 7261 7279 2069 7320 6672 6565   Library is free
+000009b0: 2073 6f66 7477 6172 652e 2020 5365 6520   software.  See 
+000009c0: 7468 6520 6669 6c65 2043 4f50 5949 4e47  the file COPYING
+000009d0: 2e4c 4942 2066 6f72 2063 6f70 7969 6e67  .LIB for copying
+000009e0: 2063 6f6e 6469 7469 6f6e 732c 2061 6e64   conditions, and
+000009f0: 204c 4943 454e 5345 5320 666f 7220 220a   LICENSES for ".
+00000a00: 2020 2020 2020 2020 2020 2020 226e 6f74              "not
+00000a10: 6963 6573 2061 626f 7574 2061 2066 6577  ices about a few
+00000a20: 2063 6f6e 7472 6962 7574 696f 6e73 2074   contributions t
+00000a30: 6861 7420 7265 7175 6972 6520 7468 6573  hat require thes
+00000a40: 6520 6164 6469 7469 6f6e 616c 206e 6f74  e additional not
+00000a50: 6963 6573 2074 6f20 6265 2064 6973 7472  ices to be distr
+00000a60: 6962 7574 6564 2e20 204c 6963 656e 7365  ibuted.  License
+00000a70: 2022 0a20 2020 2020 2020 2020 2020 2022   ".            "
+00000a80: 636f 7079 7269 6768 7420 7965 6172 7320  copyright years 
+00000a90: 6d61 7920 6265 206c 6973 7465 6420 7573  may be listed us
+00000aa0: 696e 6720 7261 6e67 6520 6e6f 7461 7469  ing range notati
+00000ab0: 6f6e 2c20 652e 672e 2c20 3139 3936 2d32  on, e.g., 1996-2
+00000ac0: 3031 352c 2069 6e64 6963 6174 696e 6720  015, indicating 
+00000ad0: 7468 6174 2065 7665 7279 2079 6561 7220  that every year 
+00000ae0: 696e 2074 6865 2022 0a20 2020 2020 2020  in the ".       
+00000af0: 2020 2020 2022 7261 6e67 652c 2069 6e63       "range, inc
+00000b00: 6c75 7369 7665 2c20 6973 2061 2063 6f70  lusive, is a cop
+00000b10: 7972 6967 6874 6162 6c65 2079 6561 7220  yrightable year 
+00000b20: 7468 6174 2077 6f75 6c64 206f 7468 6572  that would other
+00000b30: 7769 7365 2062 6520 6c69 7374 6564 2069  wise be listed i
+00000b40: 6e64 6976 6964 7561 6c6c 792e 220a 2020  ndividually.".  
+00000b50: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00000b60: 2022 6275 696c 7444 6174 6522 3a20 2232   "builtDate": "2
+00000b70: 3031 312d 3031 2d32 3954 3138 3a33 303a  011-01-29T18:30:
+00000b80: 3232 5a22 2c0a 2020 2020 2020 2020 2263  22Z",.        "c
+00000b90: 6865 636b 7375 6d73 223a 205b 0a20 2020  hecksums": [.   
+00000ba0: 2020 2020 2020 2020 207b 2261 6c67 6f72           {"algor
+00000bb0: 6974 686d 223a 2022 4d44 3522 2c20 2263  ithm": "MD5", "c
+00000bc0: 6865 636b 7375 6d56 616c 7565 223a 2022  hecksumValue": "
+00000bd0: 3632 3463 3161 6262 3336 3634 6634 6233  624c1abb3664f4b3
+00000be0: 3535 3437 6537 6337 3338 3634 6164 3234  5547e7c73864ad24
+00000bf0: 227d 2c0a 2020 2020 2020 2020 2020 2020  "},.            
+00000c00: 7b22 616c 676f 7269 7468 6d22 3a20 2253  {"algorithm": "S
+00000c10: 4841 3122 2c20 2263 6865 636b 7375 6d56  HA1", "checksumV
+00000c20: 616c 7565 223a 2022 3835 6564 3038 3137  alue": "85ed0817
+00000c30: 6166 3833 6132 3461 6438 6461 3638 6332  af83a24ad8da68c2
+00000c40: 6235 3039 3464 6536 3938 3333 3938 3363  b5094de69833983c
+00000c50: 227d 2c0a 2020 2020 2020 2020 2020 2020  "},.            
+00000c60: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000c70: 2020 2261 6c67 6f72 6974 686d 223a 2022    "algorithm": "
+00000c80: 5348 4132 3536 222c 0a20 2020 2020 2020  SHA256",.       
+00000c90: 2020 2020 2020 2020 2022 6368 6563 6b73           "checks
+00000ca0: 756d 5661 6c75 6522 3a20 2231 3162 3664  umValue": "11b6d
+00000cb0: 3365 6535 3534 6565 6466 3739 3239 3939  3ee554eedf792999
+00000cc0: 3035 6139 3866 3962 3961 3034 6534 3938  05a98f9b9a04e498
+00000cd0: 3231 3062 3539 6631 3530 3934 6339 3136  210b59f15094c916
+00000ce0: 6339 3164 3135 3065 6663 6422 2c0a 2020  c91d150efcd",.  
+00000cf0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00000d00: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00000d10: 2020 2020 2020 2020 2020 2022 616c 676f             "algo
+00000d20: 7269 7468 6d22 3a20 2242 4c41 4b45 3262  rithm": "BLAKE2b
+00000d30: 2d33 3834 222c 0a20 2020 2020 2020 2020  -384",.         
+00000d40: 2020 2020 2020 2022 6368 6563 6b73 756d         "checksum
+00000d50: 5661 6c75 6522 3a20 2261 6161 6264 3839  Value": "aaabd89
+00000d60: 6339 3236 6162 3532 3563 3234 3265 3636  c926ab525c242e66
+00000d70: 3231 6632 6635 6661 3733 6161 3461 6665  21f2f5fa73aa4afe
+00000d80: 3364 3965 3234 6165 6437 3237 6661 6161  3d9e24aed727faaa
+00000d90: 6464 3661 6633 3862 3632 3062 6462 3632  dd6af38b620bdb62
+00000da0: 3364 6432 6234 3738 3862 3163 3822 0a20  3dd2b4788b1c8". 
+00000db0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000dc0: 3038 3639 3834 6166 3837 3036 222c 0a20  086984af8706",. 
+00000dd0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00000de0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00000df0: 2022 636f 6d6d 656e 7422 3a20 2254 6869   "comment": "Thi
+00000e00: 7320 6973 2061 2063 6f6d 6d65 6e74 2e22  s is a comment."
+00000e10: 2c0a 2020 2020 2020 2020 2263 6f70 7972  ,.        "copyr
+00000e20: 6967 6874 5465 7874 223a 2063 6f70 7972  ightText": copyr
+00000e30: 6967 6874 5f74 6578 742c 0a20 2020 2020  ight_text,.     
+00000e40: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00000e50: 3a20 2254 6865 2047 4e55 2043 204c 6962  : "The GNU C Lib
+00000e60: 7261 7279 2064 6566 696e 6573 2066 756e  rary defines fun
+00000e70: 6374 696f 6e73 2074 6861 7420 6172 6520  ctions that are 
+00000e80: 7370 6563 6966 6965 6420 6279 2074 6865  specified by the
+00000e90: 2049 534f 2043 2073 7461 6e64 6172 642c   ISO C standard,
+00000ea0: 2061 7320 7765 6c6c 2061 7320 220a 2020   as well as ".  
+00000eb0: 2020 2020 2020 2261 6464 6974 696f 6e61        "additiona
+00000ec0: 6c20 6665 6174 7572 6573 2073 7065 6369  l features speci
+00000ed0: 6669 6320 746f 2050 4f53 4958 2061 6e64  fic to POSIX and
+00000ee0: 206f 7468 6572 2064 6572 6976 6174 6976   other derivativ
+00000ef0: 6573 206f 6620 7468 6520 556e 6978 206f  es of the Unix o
+00000f00: 7065 7261 7469 6e67 2073 7973 7465 6d2c  perating system,
+00000f10: 2061 6e64 2022 0a20 2020 2020 2020 2022   and ".        "
+00000f20: 6578 7465 6e73 696f 6e73 2073 7065 6369  extensions speci
+00000f30: 6669 6320 746f 2047 4e55 2073 7973 7465  fic to GNU syste
+00000f40: 6d73 2e22 2c0a 2020 2020 2020 2020 2264  ms.",.        "d
+00000f50: 6f77 6e6c 6f61 644c 6f63 6174 696f 6e22  ownloadLocation"
+00000f60: 3a20 646f 776e 6c6f 6164 5f6c 6f63 6174  : download_locat
+00000f70: 696f 6e2c 0a20 2020 2020 2020 2022 6578  ion,.        "ex
+00000f80: 7465 726e 616c 5265 6673 223a 205b 0a20  ternalRefs": [. 
+00000f90: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00000fa0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+00000fb0: 6665 7265 6e63 6543 6174 6567 6f72 7922  ferenceCategory"
+00000fc0: 3a20 2253 4543 5552 4954 5922 2c0a 2020  : "SECURITY",.  
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00000fe0: 6566 6572 656e 6365 4c6f 6361 746f 7222  eferenceLocator"
+00000ff0: 3a20 2263 7065 3a32 2e33 3a61 3a70 6976  : "cpe:2.3:a:piv
+00001000: 6f74 616c 5f73 6f66 7477 6172 653a 7370  otal_software:sp
+00001010: 7269 6e67 5f66 7261 6d65 776f 726b 3a34  ring_framework:4
+00001020: 2e31 2e30 3a2a 3a2a 3a2a 3a2a 3a2a 3a2a  .1.0:*:*:*:*:*:*
+00001030: 3a2a 222c 0a20 2020 2020 2020 2020 2020  :*",.           
+00001040: 2020 2020 2022 7265 6665 7265 6e63 6554       "referenceT
+00001050: 7970 6522 3a20 2263 7065 3233 5479 7065  ype": "cpe23Type
+00001060: 222c 0a20 2020 2020 2020 2020 2020 207d  ",.            }
+00001070: 2c0a 2020 2020 2020 2020 2020 2020 7b0a  ,.            {.
+00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001090: 2263 6f6d 6d65 6e74 223a 2022 5468 6973  "comment": "This
+000010a0: 2069 7320 7468 6520 6578 7465 726e 616c   is the external
+000010b0: 2072 6566 2066 6f72 2041 636d 6522 2c0a   ref for Acme",.
+000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010d0: 2272 6566 6572 656e 6365 4361 7465 676f  "referenceCatego
+000010e0: 7279 223a 2022 4f54 4845 5222 2c0a 2020  ry": "OTHER",.  
+000010f0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00001100: 6566 6572 656e 6365 4c6f 6361 746f 7222  eferenceLocator"
+00001110: 3a20 2261 636d 6563 6f72 702f 6163 6d65  : "acmecorp/acme
+00001120: 6e61 746f 722f 342e 312e 332d 616c 7068  nator/4.1.3-alph
+00001130: 6122 2c0a 2020 2020 2020 2020 2020 2020  a",.            
+00001140: 2020 2020 2272 6566 6572 656e 6365 5479      "referenceTy
+00001150: 7065 223a 2022 6874 7470 3a2f 2f73 7064  pe": "http://spd
+00001160: 782e 6f72 672f 7370 6478 646f 6373 2f73  x.org/spdxdocs/s
+00001170: 7064 782d 6578 616d 706c 652d 3434 3435  pdx-example-4445
+00001180: 3034 4530 2d34 4638 392d 3431 4433 2d39  04E0-4F89-41D3-9
+00001190: 4130 432d 3033 3035 4538 3243 3333 3031  A0C-0305E82C3301
+000011a0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000011b0: 2020 2223 4c6f 6361 7469 6f6e 5265 662d    "#LocationRef-
+000011c0: 6163 6d65 666f 7267 6522 2c0a 2020 2020  acmeforge",.    
+000011d0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000011e0: 2020 205d 2c0a 2020 2020 2020 2020 2266     ],.        "f
+000011f0: 696c 6573 416e 616c 797a 6564 223a 2054  ilesAnalyzed": T
+00001200: 7275 652c 0a20 2020 2020 2020 2022 686f  rue,.        "ho
+00001210: 6d65 7061 6765 223a 2068 6f6d 6570 6167  mepage": homepag
+00001220: 652c 0a20 2020 2020 2020 2022 6c69 6365  e,.        "lice
+00001230: 6e73 6543 6f6d 6d65 6e74 7322 3a20 2254  nseComments": "T
+00001240: 6865 206c 6963 656e 7365 2066 6f72 2074  he license for t
+00001250: 6869 7320 7072 6f6a 6563 7420 6368 616e  his project chan
+00001260: 6765 6420 7769 7468 2074 6865 2072 656c  ged with the rel
+00001270: 6561 7365 206f 6620 7665 7273 696f 6e20  ease of version 
+00001280: 782e 792e 2020 5468 6520 7665 7273 696f  x.y.  The versio
+00001290: 6e20 6f66 2074 6865 2022 0a20 2020 2020  n of the ".     
+000012a0: 2020 2022 7072 6f6a 6563 7420 696e 636c     "project incl
+000012b0: 7564 6564 2068 6572 6520 706f 7374 2d64  uded here post-d
+000012c0: 6174 6573 2074 6865 206c 6963 656e 7365  ates the license
+000012d0: 2063 6861 6e67 652e 222c 0a20 2020 2020   change.",.     
+000012e0: 2020 2022 6c69 6365 6e73 6543 6f6e 636c     "licenseConcl
+000012f0: 7564 6564 223a 2022 284c 4750 4c2d 322e  uded": "(LGPL-2.
+00001300: 302d 6f6e 6c79 204f 5220 4c69 6365 6e73  0-only OR Licens
+00001310: 6552 6566 2d33 2922 2c0a 2020 2020 2020  eRef-3)",.      
+00001320: 2020 226c 6963 656e 7365 4465 636c 6172    "licenseDeclar
+00001330: 6564 223a 2022 284c 4750 4c2d 322e 302d  ed": "(LGPL-2.0-
+00001340: 6f6e 6c79 2041 4e44 204c 6963 656e 7365  only AND License
+00001350: 5265 662d 3329 222c 0a20 2020 2020 2020  Ref-3)",.       
+00001360: 2022 6c69 6365 6e73 6549 6e66 6f46 726f   "licenseInfoFro
+00001370: 6d46 696c 6573 223a 205b 2247 504c 2d32  mFiles": ["GPL-2
+00001380: 2e30 2d6f 6e6c 7922 2c20 224c 6963 656e  .0-only", "Licen
+00001390: 7365 5265 662d 3222 2c20 224c 6963 656e  seRef-2", "Licen
+000013a0: 7365 5265 662d 3122 2c20 224e 4f41 5353  seRef-1", "NOASS
+000013b0: 4552 5449 4f4e 225d 2c0a 2020 2020 2020  ERTION"],.      
+000013c0: 2020 226e 616d 6522 3a20 2267 6c69 6263    "name": "glibc
+000013d0: 222c 0a20 2020 2020 2020 2022 6f72 6967  ",.        "orig
+000013e0: 696e 6174 6f72 223a 206f 7269 6769 6e61  inator": origina
+000013f0: 746f 722c 0a20 2020 2020 2020 2022 7061  tor,.        "pa
+00001400: 636b 6167 6546 696c 654e 616d 6522 3a20  ckageFileName": 
+00001410: 2267 6c69 6263 2d32 2e31 312e 312e 7461  "glibc-2.11.1.ta
+00001420: 722e 677a 222c 0a20 2020 2020 2020 2022  r.gz",.        "
+00001430: 7061 636b 6167 6556 6572 6966 6963 6174  packageVerificat
+00001440: 696f 6e43 6f64 6522 3a20 7b0a 2020 2020  ionCode": {.    
+00001450: 2020 2020 2020 2020 2270 6163 6b61 6765          "package
+00001460: 5665 7269 6669 6361 7469 6f6e 436f 6465  VerificationCode
+00001470: 4578 636c 7564 6564 4669 6c65 7322 3a20  ExcludedFiles": 
+00001480: 5b22 2e2f 7061 636b 6167 652e 7370 6478  ["./package.spdx
+00001490: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+000014a0: 2270 6163 6b61 6765 5665 7269 6669 6361  "packageVerifica
+000014b0: 7469 6f6e 436f 6465 5661 6c75 6522 3a20  tionCodeValue": 
+000014c0: 2264 3661 3737 3062 6133 3835 3833 6564  "d6a770ba38583ed
+000014d0: 3462 6234 3532 3562 6439 3665 3530 3436  4bb4525bd96e5046
+000014e0: 3136 3535 6432 3735 3822 2c0a 2020 2020  1655d2758",.    
+000014f0: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00001500: 7072 696d 6172 7950 6163 6b61 6765 5075  primaryPackagePu
+00001510: 7270 6f73 6522 3a20 2253 4f55 5243 4522  rpose": "SOURCE"
+00001520: 2c0a 2020 2020 2020 2020 2272 656c 6561  ,.        "relea
+00001530: 7365 4461 7465 223a 2022 3230 3132 2d30  seDate": "2012-0
+00001540: 312d 3239 5431 383a 3330 3a32 325a 222c  1-29T18:30:22Z",
+00001550: 0a20 2020 2020 2020 2022 736f 7572 6365  .        "source
+00001560: 496e 666f 223a 2022 7573 6573 2067 6c69  Info": "uses gli
+00001570: 6263 2d32 5f31 312d 6272 616e 6368 2066  bc-2_11-branch f
+00001580: 726f 6d20 6769 743a 2f2f 736f 7572 6365  rom git://source
+00001590: 7761 7265 2e6f 7267 2f67 6974 2f67 6c69  ware.org/git/gli
+000015a0: 6263 2e67 6974 2e22 2c0a 2020 2020 2020  bc.git.",.      
+000015b0: 2020 2273 756d 6d61 7279 223a 2022 474e    "summary": "GN
+000015c0: 5520 4320 6c69 6272 6172 792e 222c 0a20  U C library.",. 
+000015d0: 2020 2020 2020 2022 7375 7070 6c69 6572         "supplier
+000015e0: 223a 2073 7570 706c 6965 722c 0a20 2020  ": supplier,.   
+000015f0: 2020 2020 2022 7661 6c69 6455 6e74 696c       "validUntil
+00001600: 4461 7465 223a 2022 3230 3134 2d30 312d  Date": "2014-01-
+00001610: 3239 5431 383a 3330 3a32 325a 222c 0a20  29T18:30:22Z",. 
+00001620: 2020 2020 2020 2022 7665 7273 696f 6e49         "versionI
+00001630: 6e66 6f22 3a20 2232 2e31 312e 3122 2c0a  nfo": "2.11.1",.
+00001640: 2020 2020 7d0a 0a20 2020 2070 6163 6b61      }..    packa
+00001650: 6765 203d 2070 6163 6b61 6765 5f70 6172  ge = package_par
+00001660: 7365 722e 7061 7273 655f 7061 636b 6167  ser.parse_packag
+00001670: 6528 7061 636b 6167 655f 6469 6374 290a  e(package_dict).
+00001680: 0a20 2020 2061 7373 6572 7420 7061 636b  .    assert pack
+00001690: 6167 652e 7370 6478 5f69 6420 3d3d 2022  age.spdx_id == "
+000016a0: 5350 4458 5265 662d 5061 636b 6167 6522  SPDXRef-Package"
+000016b0: 0a20 2020 2061 7373 6572 7420 7061 636b  .    assert pack
+000016c0: 6167 652e 6e61 6d65 203d 3d20 2267 6c69  age.name == "gli
+000016d0: 6263 220a 2020 2020 6173 7365 7274 2070  bc".    assert p
+000016e0: 6163 6b61 6765 2e64 6f77 6e6c 6f61 645f  ackage.download_
+000016f0: 6c6f 6361 7469 6f6e 203d 3d20 6578 7065  location == expe
+00001700: 6374 6564 5f64 6f77 6e6c 6f61 645f 6c6f  cted_download_lo
+00001710: 6361 7469 6f6e 0a20 2020 2061 7373 6572  cation.    asser
+00001720: 7420 7061 636b 6167 652e 7665 7273 696f  t package.versio
+00001730: 6e20 3d3d 2022 322e 3131 2e31 220a 2020  n == "2.11.1".  
+00001740: 2020 6173 7365 7274 2070 6163 6b61 6765    assert package
+00001750: 2e66 696c 655f 6e61 6d65 203d 3d20 2267  .file_name == "g
+00001760: 6c69 6263 2d32 2e31 312e 312e 7461 722e  libc-2.11.1.tar.
+00001770: 677a 220a 2020 2020 6173 7365 7274 2070  gz".    assert p
+00001780: 6163 6b61 6765 2e73 7570 706c 6965 7220  ackage.supplier 
+00001790: 3d3d 2065 7870 6563 7465 645f 7375 7070  == expected_supp
+000017a0: 6c69 6572 0a20 2020 2061 7373 6572 7420  lier.    assert 
+000017b0: 7061 636b 6167 652e 6f72 6967 696e 6174  package.originat
+000017c0: 6f72 203d 3d20 6578 7065 6374 6564 5f6f  or == expected_o
+000017d0: 7269 6769 6e61 746f 720a 2020 2020 6173  riginator.    as
+000017e0: 7365 7274 2070 6163 6b61 6765 2e66 696c  sert package.fil
+000017f0: 6573 5f61 6e61 6c79 7a65 6420 6973 2054  es_analyzed is T
+00001800: 7275 650a 2020 2020 6173 7365 7274 2070  rue.    assert p
+00001810: 6163 6b61 6765 2e76 6572 6966 6963 6174  ackage.verificat
+00001820: 696f 6e5f 636f 6465 203d 3d20 5061 636b  ion_code == Pack
+00001830: 6167 6556 6572 6966 6963 6174 696f 6e43  ageVerificationC
+00001840: 6f64 6528 0a20 2020 2020 2020 2076 616c  ode(.        val
+00001850: 7565 3d22 6436 6137 3730 6261 3338 3538  ue="d6a770ba3858
+00001860: 3365 6434 6262 3435 3235 6264 3936 6535  3ed4bb4525bd96e5
+00001870: 3034 3631 3635 3564 3237 3538 222c 2065  0461655d2758", e
+00001880: 7863 6c75 6465 645f 6669 6c65 733d 5b22  xcluded_files=["
+00001890: 2e2f 7061 636b 6167 652e 7370 6478 225d  ./package.spdx"]
+000018a0: 0a20 2020 2029 0a20 2020 2061 7373 6572  .    ).    asser
+000018b0: 7420 6c65 6e28 7061 636b 6167 652e 6368  t len(package.ch
+000018c0: 6563 6b73 756d 7329 203d 3d20 340a 2020  ecksums) == 4.  
+000018d0: 2020 5465 7374 4361 7365 2829 2e61 7373    TestCase().ass
+000018e0: 6572 7443 6f75 6e74 4571 7561 6c28 0a20  ertCountEqual(. 
+000018f0: 2020 2020 2020 2070 6163 6b61 6765 2e63         package.c
+00001900: 6865 636b 7375 6d73 2c0a 2020 2020 2020  hecksums,.      
+00001910: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
+00001920: 4368 6563 6b73 756d 2843 6865 636b 7375  Checksum(Checksu
+00001930: 6d41 6c67 6f72 6974 686d 2e4d 4435 2c20  mAlgorithm.MD5, 
+00001940: 2236 3234 6331 6162 6233 3636 3466 3462  "624c1abb3664f4b
+00001950: 3335 3534 3765 3763 3733 3836 3461 6432  35547e7c73864ad2
+00001960: 3422 292c 0a20 2020 2020 2020 2020 2020  4"),.           
+00001970: 2043 6865 636b 7375 6d28 4368 6563 6b73   Checksum(Checks
+00001980: 756d 416c 676f 7269 7468 6d2e 5348 4131  umAlgorithm.SHA1
+00001990: 2c20 2238 3565 6430 3831 3761 6638 3361  , "85ed0817af83a
+000019a0: 3234 6164 3864 6136 3863 3262 3530 3934  24ad8da68c2b5094
+000019b0: 6465 3639 3833 3339 3833 6322 292c 0a20  de69833983c"),. 
+000019c0: 2020 2020 2020 2020 2020 2043 6865 636b             Check
+000019d0: 7375 6d28 4368 6563 6b73 756d 416c 676f  sum(ChecksumAlgo
+000019e0: 7269 7468 6d2e 5348 4132 3536 2c20 2231  rithm.SHA256, "1
+000019f0: 3162 3664 3365 6535 3534 6565 6466 3739  1b6d3ee554eedf79
+00001a00: 3239 3939 3035 6139 3866 3962 3961 3034  299905a98f9b9a04
+00001a10: 6534 3938 3231 3062 3539 6631 3530 3934  e498210b59f15094
+00001a20: 6339 3136 6339 3164 3135 3065 6663 6422  c916c91d150efcd"
+00001a30: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
+00001a40: 6865 636b 7375 6d28 0a20 2020 2020 2020  hecksum(.       
+00001a50: 2020 2020 2020 2020 2043 6865 636b 7375           Checksu
+00001a60: 6d41 6c67 6f72 6974 686d 2e42 4c41 4b45  mAlgorithm.BLAKE
+00001a70: 3242 5f33 3834 2c0a 2020 2020 2020 2020  2B_384,.        
+00001a80: 2020 2020 2020 2020 2261 6161 6264 3839          "aaabd89
+00001a90: 6339 3236 6162 3532 3563 3234 3265 3636  c926ab525c242e66
+00001aa0: 3231 6632 6635 6661 3733 6161 3461 6665  21f2f5fa73aa4afe
+00001ab0: 3364 3965 3234 6165 6437 3237 6661 6161  3d9e24aed727faaa
+00001ac0: 6464 3661 6633 3862 3632 3062 6462 3632  dd6af38b620bdb62
+00001ad0: 3364 6432 6234 3738 3862 3163 3830 3836  3dd2b4788b1c8086
+00001ae0: 3938 3461 6638 3730 3622 2c0a 2020 2020  984af8706",.    
+00001af0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00001b00: 2020 205d 2c0a 2020 2020 290a 2020 2020     ],.    ).    
+00001b10: 6173 7365 7274 2070 6163 6b61 6765 2e68  assert package.h
+00001b20: 6f6d 6570 6167 6520 3d3d 2065 7870 6563  omepage == expec
+00001b30: 7465 645f 686f 6d65 7061 6765 0a20 2020  ted_homepage.   
+00001b40: 2061 7373 6572 7420 7061 636b 6167 652e   assert package.
+00001b50: 736f 7572 6365 5f69 6e66 6f20 3d3d 2022  source_info == "
+00001b60: 7573 6573 2067 6c69 6263 2d32 5f31 312d  uses glibc-2_11-
+00001b70: 6272 616e 6368 2066 726f 6d20 6769 743a  branch from git:
+00001b80: 2f2f 736f 7572 6365 7761 7265 2e6f 7267  //sourceware.org
+00001b90: 2f67 6974 2f67 6c69 6263 2e67 6974 2e22  /git/glibc.git."
+00001ba0: 0a20 2020 2061 7373 6572 7420 7061 636b  .    assert pack
+00001bb0: 6167 652e 6c69 6365 6e73 655f 636f 6e63  age.license_conc
+00001bc0: 6c75 6465 6420 3d3d 204c 6963 656e 7369  luded == Licensi
+00001bd0: 6e67 2829 2e70 6172 7365 2822 284c 4750  ng().parse("(LGP
+00001be0: 4c2d 322e 302d 6f6e 6c79 204f 5220 4c69  L-2.0-only OR Li
+00001bf0: 6365 6e73 6552 6566 2d33 2922 290a 2020  censeRef-3)").  
+00001c00: 2020 5465 7374 4361 7365 2829 2e61 7373    TestCase().ass
+00001c10: 6572 7443 6f75 6e74 4571 7561 6c28 0a20  ertCountEqual(. 
+00001c20: 2020 2020 2020 2070 6163 6b61 6765 2e6c         package.l
+00001c30: 6963 656e 7365 5f69 6e66 6f5f 6672 6f6d  icense_info_from
+00001c40: 5f66 696c 6573 2c0a 2020 2020 2020 2020  _files,.        
+00001c50: 5b0a 2020 2020 2020 2020 2020 2020 4c69  [.            Li
+00001c60: 6365 6e73 696e 6728 292e 7061 7273 6528  censing().parse(
+00001c70: 2247 504c 2d32 2e30 2d6f 6e6c 7922 292c  "GPL-2.0-only"),
+00001c80: 0a20 2020 2020 2020 2020 2020 204c 6963  .            Lic
+00001c90: 656e 7369 6e67 2829 2e70 6172 7365 2822  ensing().parse("
+00001ca0: 4c69 6365 6e73 6552 6566 2d32 2229 2c0a  LicenseRef-2"),.
+00001cb0: 2020 2020 2020 2020 2020 2020 4c69 6365              Lice
+00001cc0: 6e73 696e 6728 292e 7061 7273 6528 224c  nsing().parse("L
+00001cd0: 6963 656e 7365 5265 662d 3122 292c 0a20  icenseRef-1"),. 
+00001ce0: 2020 2020 2020 2020 2020 2053 7064 784e             SpdxN
+00001cf0: 6f41 7373 6572 7469 6f6e 2829 2c0a 2020  oAssertion(),.  
+00001d00: 2020 2020 2020 5d2c 0a20 2020 2029 0a20        ],.    ). 
+00001d10: 2020 2061 7373 6572 7420 7061 636b 6167     assert packag
+00001d20: 652e 6c69 6365 6e73 655f 6465 636c 6172  e.license_declar
+00001d30: 6564 203d 3d20 4c69 6365 6e73 696e 6728  ed == Licensing(
+00001d40: 292e 7061 7273 6528 2228 4c47 504c 2d32  ).parse("(LGPL-2
+00001d50: 2e30 2d6f 6e6c 7920 414e 4420 4c69 6365  .0-only AND Lice
+00001d60: 6e73 6552 6566 2d33 2922 290a 2020 2020  nseRef-3)").    
+00001d70: 6173 7365 7274 2028 0a20 2020 2020 2020  assert (.       
+00001d80: 2070 6163 6b61 6765 2e6c 6963 656e 7365   package.license
+00001d90: 5f63 6f6d 6d65 6e74 0a20 2020 2020 2020  _comment.       
+00001da0: 203d 3d20 2254 6865 206c 6963 656e 7365   == "The license
+00001db0: 2066 6f72 2074 6869 7320 7072 6f6a 6563   for this projec
+00001dc0: 7420 6368 616e 6765 6420 7769 7468 2074  t changed with t
+00001dd0: 6865 2072 656c 6561 7365 206f 6620 7665  he release of ve
+00001de0: 7273 696f 6e20 782e 792e 2020 5468 6520  rsion x.y.  The 
+00001df0: 7665 7273 696f 6e20 6f66 2074 6865 2070  version of the p
+00001e00: 726f 6a65 6374 2069 6e63 6c75 6465 6422  roject included"
+00001e10: 0a20 2020 2020 2020 2022 2068 6572 6520  .        " here 
+00001e20: 706f 7374 2d64 6174 6573 2074 6865 206c  post-dates the l
+00001e30: 6963 656e 7365 2063 6861 6e67 652e 220a  icense change.".
+00001e40: 2020 2020 290a 2020 2020 6173 7365 7274      ).    assert
+00001e50: 2070 6163 6b61 6765 2e63 6f70 7972 6967   package.copyrig
+00001e60: 6874 5f74 6578 7420 3d3d 2065 7870 6563  ht_text == expec
+00001e70: 7465 645f 636f 7079 7269 6768 745f 7465  ted_copyright_te
+00001e80: 7874 0a20 2020 2061 7373 6572 7420 7061  xt.    assert pa
+00001e90: 636b 6167 652e 7375 6d6d 6172 7920 3d3d  ckage.summary ==
+00001ea0: 2022 474e 5520 4320 6c69 6272 6172 792e   "GNU C library.
+00001eb0: 220a 2020 2020 6173 7365 7274 2028 0a20  ".    assert (. 
+00001ec0: 2020 2020 2020 2070 6163 6b61 6765 2e64         package.d
+00001ed0: 6573 6372 6970 7469 6f6e 0a20 2020 2020  escription.     
+00001ee0: 2020 203d 3d20 2254 6865 2047 4e55 2043     == "The GNU C
+00001ef0: 204c 6962 7261 7279 2064 6566 696e 6573   Library defines
+00001f00: 2066 756e 6374 696f 6e73 2074 6861 7420   functions that 
+00001f10: 6172 6520 7370 6563 6966 6965 6420 6279  are specified by
+00001f20: 2074 6865 2049 534f 2043 2073 7461 6e64   the ISO C stand
+00001f30: 6172 642c 2061 7320 7765 6c6c 2061 7320  ard, as well as 
+00001f40: 6164 6469 7469 6f6e 616c 2022 0a20 2020  additional ".   
+00001f50: 2020 2020 2022 6665 6174 7572 6573 2073       "features s
+00001f60: 7065 6369 6669 6320 746f 2050 4f53 4958  pecific to POSIX
+00001f70: 2061 6e64 206f 7468 6572 2064 6572 6976   and other deriv
+00001f80: 6174 6976 6573 206f 6620 7468 6520 556e  atives of the Un
+00001f90: 6978 206f 7065 7261 7469 6e67 2073 7973  ix operating sys
+00001fa0: 7465 6d2c 2061 6e64 2065 7874 656e 7369  tem, and extensi
+00001fb0: 6f6e 7320 7370 6563 6966 6963 2022 0a20  ons specific ". 
+00001fc0: 2020 2020 2020 2022 746f 2047 4e55 2073         "to GNU s
+00001fd0: 7973 7465 6d73 2e22 0a20 2020 2029 0a20  ystems.".    ). 
+00001fe0: 2020 2061 7373 6572 7420 7061 636b 6167     assert packag
+00001ff0: 652e 636f 6d6d 656e 7420 3d3d 2022 5468  e.comment == "Th
+00002000: 6973 2069 7320 6120 636f 6d6d 656e 742e  is is a comment.
+00002010: 220a 2020 2020 6173 7365 7274 206c 656e  ".    assert len
+00002020: 2870 6163 6b61 6765 2e65 7874 6572 6e61  (package.externa
+00002030: 6c5f 7265 6665 7265 6e63 6573 2920 3d3d  l_references) ==
+00002040: 2032 0a20 2020 2054 6573 7443 6173 6528   2.    TestCase(
+00002050: 292e 6173 7365 7274 436f 756e 7445 7175  ).assertCountEqu
+00002060: 616c 280a 2020 2020 2020 2020 7061 636b  al(.        pack
+00002070: 6167 652e 6578 7465 726e 616c 5f72 6566  age.external_ref
+00002080: 6572 656e 6365 732c 0a20 2020 2020 2020  erences,.       
+00002090: 205b 0a20 2020 2020 2020 2020 2020 2045   [.            E
+000020a0: 7874 6572 6e61 6c50 6163 6b61 6765 5265  xternalPackageRe
+000020b0: 6628 0a20 2020 2020 2020 2020 2020 2020  f(.             
+000020c0: 2020 2045 7874 6572 6e61 6c50 6163 6b61     ExternalPacka
+000020d0: 6765 5265 6643 6174 6567 6f72 792e 5345  geRefCategory.SE
+000020e0: 4355 5249 5459 2c0a 2020 2020 2020 2020  CURITY,.        
+000020f0: 2020 2020 2020 2020 2263 7065 3233 5479          "cpe23Ty
+00002100: 7065 222c 0a20 2020 2020 2020 2020 2020  pe",.           
+00002110: 2020 2020 2022 6370 653a 322e 333a 613a       "cpe:2.3:a:
+00002120: 7069 766f 7461 6c5f 736f 6674 7761 7265  pivotal_software
+00002130: 3a73 7072 696e 675f 6672 616d 6577 6f72  :spring_framewor
+00002140: 6b3a 342e 312e 303a 2a3a 2a3a 2a3a 2a3a  k:4.1.0:*:*:*:*:
+00002150: 2a3a 2a3a 2a22 2c0a 2020 2020 2020 2020  *:*:*",.        
+00002160: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00002170: 2020 2045 7874 6572 6e61 6c50 6163 6b61     ExternalPacka
+00002180: 6765 5265 6628 0a20 2020 2020 2020 2020  geRef(.         
+00002190: 2020 2020 2020 2045 7874 6572 6e61 6c50         ExternalP
+000021a0: 6163 6b61 6765 5265 6643 6174 6567 6f72  ackageRefCategor
+000021b0: 792e 4f54 4845 522c 0a20 2020 2020 2020  y.OTHER,.       
+000021c0: 2020 2020 2020 2020 2022 6874 7470 3a2f           "http:/
+000021d0: 2f73 7064 782e 6f72 672f 7370 6478 646f  /spdx.org/spdxdo
+000021e0: 6373 2f73 7064 782d 6578 616d 706c 652d  cs/spdx-example-
+000021f0: 3434 3435 3034 4530 2d34 4638 392d 3431  444504E0-4F89-41
+00002200: 4433 2d39 4130 432d 3033 3035 4538 3243  D3-9A0C-0305E82C
+00002210: 3333 3031 234c 6f63 6174 696f 6e52 6566  3301#LocationRef
+00002220: 2d61 636d 6566 6f72 6765 222c 0a20 2020  -acmeforge",.   
+00002230: 2020 2020 2020 2020 2020 2020 206c 6f63               loc
+00002240: 6174 6f72 3d22 6163 6d65 636f 7270 2f61  ator="acmecorp/a
+00002250: 636d 656e 6174 6f72 2f34 2e31 2e33 2d61  cmenator/4.1.3-a
+00002260: 6c70 6861 222c 0a20 2020 2020 2020 2020  lpha",.         
+00002270: 2020 2020 2020 2063 6f6d 6d65 6e74 3d22         comment="
+00002280: 5468 6973 2069 7320 7468 6520 6578 7465  This is the exte
+00002290: 726e 616c 2072 6566 2066 6f72 2041 636d  rnal ref for Acm
+000022a0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+000022b0: 292c 0a20 2020 2020 2020 205d 2c0a 2020  ),.        ],.  
+000022c0: 2020 290a 2020 2020 6173 7365 7274 2070    ).    assert p
+000022d0: 6163 6b61 6765 2e61 7474 7269 6275 7469  ackage.attributi
+000022e0: 6f6e 5f74 6578 7473 203d 3d20 5b0a 2020  on_texts == [.  
+000022f0: 2020 2020 2020 2254 6865 2047 4e55 2043        "The GNU C
+00002300: 204c 6962 7261 7279 2069 7320 6672 6565   Library is free
+00002310: 2073 6f66 7477 6172 652e 2020 5365 6520   software.  See 
+00002320: 7468 6520 6669 6c65 2043 4f50 5949 4e47  the file COPYING
+00002330: 2e4c 4942 2066 6f72 2063 6f70 7969 6e67  .LIB for copying
+00002340: 2063 6f6e 6469 7469 6f6e 732c 2061 6e64   conditions, and
+00002350: 204c 4943 454e 5345 5320 666f 7220 220a   LICENSES for ".
+00002360: 2020 2020 2020 2020 226e 6f74 6963 6573          "notices
+00002370: 2061 626f 7574 2061 2066 6577 2063 6f6e   about a few con
+00002380: 7472 6962 7574 696f 6e73 2074 6861 7420  tributions that 
+00002390: 7265 7175 6972 6520 7468 6573 6520 6164  require these ad
+000023a0: 6469 7469 6f6e 616c 206e 6f74 6963 6573  ditional notices
+000023b0: 2074 6f20 6265 2064 6973 7472 6962 7574   to be distribut
+000023c0: 6564 2e20 204c 6963 656e 7365 2022 0a20  ed.  License ". 
+000023d0: 2020 2020 2020 2022 636f 7079 7269 6768         "copyrigh
+000023e0: 7420 7965 6172 7320 6d61 7920 6265 206c  t years may be l
+000023f0: 6973 7465 6420 7573 696e 6720 7261 6e67  isted using rang
+00002400: 6520 6e6f 7461 7469 6f6e 2c20 652e 672e  e notation, e.g.
+00002410: 2c20 3139 3936 2d32 3031 352c 2069 6e64  , 1996-2015, ind
+00002420: 6963 6174 696e 6720 7468 6174 2065 7665  icating that eve
+00002430: 7279 2079 6561 7220 696e 2074 6865 2022  ry year in the "
+00002440: 0a20 2020 2020 2020 2022 7261 6e67 652c  .        "range,
+00002450: 2069 6e63 6c75 7369 7665 2c20 6973 2061   inclusive, is a
+00002460: 2063 6f70 7972 6967 6874 6162 6c65 2079   copyrightable y
+00002470: 6561 7220 7468 6174 2077 6f75 6c64 206f  ear that would o
+00002480: 7468 6572 7769 7365 2062 6520 6c69 7374  therwise be list
+00002490: 6564 2069 6e64 6976 6964 7561 6c6c 792e  ed individually.
+000024a0: 220a 2020 2020 5d0a 2020 2020 6173 7365  ".    ].    asse
+000024b0: 7274 2070 6163 6b61 6765 2e70 7269 6d61  rt package.prima
+000024c0: 7279 5f70 6163 6b61 6765 5f70 7572 706f  ry_package_purpo
+000024d0: 7365 203d 3d20 5061 636b 6167 6550 7572  se == PackagePur
+000024e0: 706f 7365 2e53 4f55 5243 450a 2020 2020  pose.SOURCE.    
+000024f0: 6173 7365 7274 2070 6163 6b61 6765 2e72  assert package.r
+00002500: 656c 6561 7365 5f64 6174 6520 3d3d 2064  elease_date == d
+00002510: 6174 6574 696d 6528 3230 3132 2c20 312c  atetime(2012, 1,
+00002520: 2032 392c 2031 382c 2033 302c 2032 3229   29, 18, 30, 22)
+00002530: 0a20 2020 2061 7373 6572 7420 7061 636b  .    assert pack
+00002540: 6167 652e 6275 696c 745f 6461 7465 203d  age.built_date =
+00002550: 3d20 6461 7465 7469 6d65 2832 3031 312c  = datetime(2011,
+00002560: 2031 2c20 3239 2c20 3138 2c20 3330 2c20   1, 29, 18, 30, 
+00002570: 3232 290a 2020 2020 6173 7365 7274 2070  22).    assert p
+00002580: 6163 6b61 6765 2e76 616c 6964 5f75 6e74  ackage.valid_unt
+00002590: 696c 5f64 6174 6520 3d3d 2064 6174 6574  il_date == datet
+000025a0: 696d 6528 3230 3134 2c20 312c 2032 392c  ime(2014, 1, 29,
+000025b0: 2031 382c 2033 302c 2032 3229 0a0a 0a40   18, 30, 22)...@
+000025c0: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
+000025d0: 6d65 7472 697a 6528 0a20 2020 2022 696e  metrize(.    "in
+000025e0: 636f 6d70 6c65 7465 5f70 6163 6b61 6765  complete_package
+000025f0: 5f64 6963 742c 6578 7065 6374 6564 5f6d  _dict,expected_m
+00002600: 6573 7361 6765 222c 0a20 2020 205b 0a20  essage",.    [. 
+00002610: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
+00002620: 2020 2020 207b 2253 5044 5849 4422 3a20       {"SPDXID": 
+00002630: 2253 5044 5852 6566 2d50 6163 6b61 6765  "SPDXRef-Package
+00002640: 227d 2c0a 2020 2020 2020 2020 2020 2020  "},.            
+00002650: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00002660: 2020 2245 7272 6f72 2077 6869 6c65 2063    "Error while c
+00002670: 6f6e 7374 7275 6374 696e 6720 5061 636b  onstructing Pack
+00002680: 6167 653a 205b 2753 6574 7465 7245 7272  age: ['SetterErr
+00002690: 6f72 2050 6163 6b61 6765 3a20 7479 7065  or Package: type
+000026a0: 206f 6620 220a 2020 2020 2020 2020 2020   of ".          
+000026b0: 2020 2020 2020 2261 7267 756d 656e 7420        "argument 
+000026c0: 5c22 6e61 6d65 5c22 206d 7573 7420 6265  \"name\" must be
+000026d0: 2073 7472 3b20 676f 7420 4e6f 6e65 5479   str; got NoneTy
+000026e0: 7065 2069 6e73 7465 6164 3a20 4e6f 6e65  pe instead: None
+000026f0: 272c 2027 5365 7474 6572 4572 726f 7220  ', 'SetterError 
+00002700: 5061 636b 6167 653a 2074 7970 6520 6f66  Package: type of
+00002710: 2061 7267 756d 656e 7420 220a 2020 2020   argument ".    
+00002720: 2020 2020 2020 2020 2020 2020 2722 646f              '"do
+00002730: 776e 6c6f 6164 5f6c 6f63 6174 696f 6e22  wnload_location"
+00002740: 206d 7573 7420 6265 206f 6e65 206f 6620   must be one of 
+00002750: 2873 7472 2c20 7370 6478 5f74 6f6f 6c73  (str, spdx_tools
+00002760: 2e73 7064 782e 6d6f 6465 6c2e 7370 6478  .spdx.model.spdx
+00002770: 5f6e 6f5f 6173 7365 7274 696f 6e2e 5370  _no_assertion.Sp
+00002780: 6478 4e6f 4173 7365 7274 696f 6e2c 2027  dxNoAssertion, '
+00002790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000027a0: 2022 7370 6478 5f74 6f6f 6c73 2e73 7064   "spdx_tools.spd
+000027b0: 782e 6d6f 6465 6c2e 7370 6478 5f6e 6f6e  x.model.spdx_non
+000027c0: 652e 5370 6478 4e6f 6e65 293b 2022 0a20  e.SpdxNone); ". 
+000027d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000027e0: 676f 7420 4e6f 6e65 5479 7065 2069 6e73  got NoneType ins
+000027f0: 7465 6164 3a20 4e6f 6e65 275d 220a 2020  tead: None']".  
+00002800: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00002810: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+00002820: 280a 2020 2020 2020 2020 2020 2020 7b22  (.            {"
+00002830: 5350 4458 4944 223a 2022 5350 4458 5265  SPDXID": "SPDXRe
+00002840: 662d 5061 636b 6167 6522 2c20 226e 616d  f-Package", "nam
+00002850: 6522 3a20 352c 2022 646f 776e 6c6f 6164  e": 5, "download
+00002860: 4c6f 6361 7469 6f6e 223a 2022 4e4f 4e45  Location": "NONE
+00002870: 227d 2c0a 2020 2020 2020 2020 2020 2020  "},.            
+00002880: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00002890: 2020 2245 7272 6f72 2077 6869 6c65 2063    "Error while c
+000028a0: 6f6e 7374 7275 6374 696e 6720 5061 636b  onstructing Pack
+000028b0: 6167 653a 205b 2753 6574 7465 7245 7272  age: ['SetterErr
+000028c0: 6f72 2050 6163 6b61 6765 3a20 7479 7065  or Package: type
+000028d0: 206f 6620 6172 6775 6d65 6e74 2022 0a20   of argument ". 
+000028e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000028f0: 226e 616d 6522 206d 7573 7420 6265 2073  "name" must be s
+00002900: 7472 3b20 676f 7420 696e 7420 696e 7374  tr; got int inst
+00002910: 6561 643a 2035 5c27 5d27 0a20 2020 2020  ead: 5\']'.     
+00002920: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+00002930: 2020 292c 0a20 2020 205d 2c0a 290a 6465    ),.    ],.).de
+00002940: 6620 7465 7374 5f70 6172 7365 5f69 6e63  f test_parse_inc
+00002950: 6f6d 706c 6574 655f 7061 636b 6167 6528  omplete_package(
+00002960: 696e 636f 6d70 6c65 7465 5f70 6163 6b61  incomplete_packa
+00002970: 6765 5f64 6963 742c 2065 7870 6563 7465  ge_dict, expecte
+00002980: 645f 6d65 7373 6167 6529 3a0a 2020 2020  d_message):.    
+00002990: 7061 636b 6167 655f 7061 7273 6572 203d  package_parser =
+000029a0: 2050 6163 6b61 6765 5061 7273 6572 2829   PackageParser()
+000029b0: 0a0a 2020 2020 7769 7468 2070 7974 6573  ..    with pytes
+000029c0: 742e 7261 6973 6573 2853 5044 5850 6172  t.raises(SPDXPar
+000029d0: 7369 6e67 4572 726f 7229 2061 7320 6572  singError) as er
+000029e0: 723a 0a20 2020 2020 2020 2070 6163 6b61  r:.        packa
+000029f0: 6765 5f70 6172 7365 722e 7061 7273 655f  ge_parser.parse_
+00002a00: 7061 636b 6167 6528 696e 636f 6d70 6c65  package(incomple
+00002a10: 7465 5f70 6163 6b61 6765 5f64 6963 7429  te_package_dict)
+00002a20: 0a0a 2020 2020 5465 7374 4361 7365 2829  ..    TestCase()
+00002a30: 2e61 7373 6572 7443 6f75 6e74 4571 7561  .assertCountEqua
+00002a40: 6c28 6572 722e 7661 6c75 652e 6765 745f  l(err.value.get_
+00002a50: 6d65 7373 6167 6573 2829 2c20 6578 7065  messages(), expe
+00002a60: 6374 6564 5f6d 6573 7361 6765 290a 0a0a  cted_message)...
+00002a70: 6465 6620 7465 7374 5f70 6172 7365 5f69  def test_parse_i
+00002a80: 6e76 616c 6964 5f70 6163 6b61 6765 2829  nvalid_package()
+00002a90: 3a0a 2020 2020 7061 636b 6167 655f 7061  :.    package_pa
+00002aa0: 7273 6572 203d 2050 6163 6b61 6765 5061  rser = PackagePa
+00002ab0: 7273 6572 2829 0a20 2020 2070 6163 6b61  rser().    packa
+00002ac0: 6765 5f64 6963 7420 3d20 7b0a 2020 2020  ge_dict = {.    
+00002ad0: 2020 2020 2253 5044 5849 4422 3a20 2253      "SPDXID": "S
+00002ae0: 5044 5852 6566 2d50 6163 6b61 6765 222c  PDXRef-Package",
+00002af0: 0a20 2020 2020 2020 2022 6e61 6d65 223a  .        "name":
+00002b00: 2022 4578 616d 706c 6520 5061 636b 6167   "Example Packag
+00002b10: 6522 2c0a 2020 2020 2020 2020 2264 6f77  e",.        "dow
+00002b20: 6e6c 6f61 644c 6f63 6174 696f 6e22 3a20  nloadLocation": 
+00002b30: 224e 4f4e 4522 2c0a 2020 2020 2020 2020  "NONE",.        
+00002b40: 2263 6865 636b 7375 6d73 223a 205b 7b22  "checksums": [{"
+00002b50: 616c 676f 7269 7468 6d22 3a20 2253 4841  algorithm": "SHA
+00002b60: 222c 2022 7661 6c75 6522 3a20 2231 3233  ", "value": "123
+00002b70: 3422 7d5d 2c0a 2020 2020 7d0a 0a20 2020  4"}],.    }..   
+00002b80: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
+00002b90: 7365 7328 5350 4458 5061 7273 696e 6745  ses(SPDXParsingE
+00002ba0: 7272 6f72 2920 6173 2065 7272 3a0a 2020  rror) as err:.  
+00002bb0: 2020 2020 2020 7061 636b 6167 655f 7061        package_pa
+00002bc0: 7273 6572 2e70 6172 7365 5f70 6163 6b61  rser.parse_packa
+00002bd0: 6765 2870 6163 6b61 6765 5f64 6963 7429  ge(package_dict)
+00002be0: 0a0a 2020 2020 5465 7374 4361 7365 2829  ..    TestCase()
+00002bf0: 2e61 7373 6572 7443 6f75 6e74 4571 7561  .assertCountEqua
+00002c00: 6c28 0a20 2020 2020 2020 2065 7272 2e76  l(.        err.v
+00002c10: 616c 7565 2e67 6574 5f6d 6573 7361 6765  alue.get_message
+00002c20: 7328 292c 0a20 2020 2020 2020 205b 2245  s(),.        ["E
+00002c30: 7272 6f72 2077 6869 6c65 2070 6172 7369  rror while parsi
+00002c40: 6e67 2050 6163 6b61 6765 3a20 5b5c 2245  ng Package: [\"E
+00002c50: 7272 6f72 2077 6869 6c65 2070 6172 7369  rror while parsi
+00002c60: 6e67 2043 6865 636b 7375 6d3a 205b 2749  ng Checksum: ['I
+00002c70: 6e76 616c 6964 2043 6865 636b 7375 6d41  nvalid ChecksumA
+00002c80: 6c67 6f72 6974 686d 3a20 5348 4127 5d5c  lgorithm: SHA']\
+00002c90: 225d 225d 2c0a 2020 2020 290a 0a0a 6465  "]"],.    )...de
+00002ca0: 6620 7465 7374 5f70 6172 7365 5f70 6163  f test_parse_pac
+00002cb0: 6b61 6765 7328 293a 0a20 2020 2070 6163  kages():.    pac
+00002cc0: 6b61 6765 5f70 6172 7365 7220 3d20 5061  kage_parser = Pa
+00002cd0: 636b 6167 6550 6172 7365 7228 290a 2020  ckageParser().  
+00002ce0: 2020 7061 636b 6167 6573 5f6c 6973 7420    packages_list 
+00002cf0: 3d20 5b0a 2020 2020 2020 2020 7b0a 2020  = [.        {.  
+00002d00: 2020 2020 2020 2020 2020 2253 5044 5849            "SPDXI
+00002d10: 4422 3a20 2253 5044 5852 6566 2d50 6163  D": "SPDXRef-Pac
+00002d20: 6b61 6765 222c 0a20 2020 2020 2020 2020  kage",.         
+00002d30: 2020 2022 6e61 6d65 223a 2022 4578 616d     "name": "Exam
+00002d40: 706c 6520 5061 636b 6167 6522 2c0a 2020  ple Package",.  
+00002d50: 2020 2020 2020 2020 2020 2264 6f77 6e6c            "downl
+00002d60: 6f61 644c 6f63 6174 696f 6e22 3a20 224e  oadLocation": "N
+00002d70: 4f4e 4522 2c0a 2020 2020 2020 2020 2020  ONE",.          
+00002d80: 2020 2263 6865 636b 7375 6d73 223a 205b    "checksums": [
+00002d90: 7b22 616c 676f 7269 7468 6d22 3a20 2253  {"algorithm": "S
+00002da0: 4841 222c 2022 7661 6c75 6522 3a20 2231  HA", "value": "1
+00002db0: 3233 3422 7d5d 2c0a 2020 2020 2020 2020  234"}],.        
+00002dc0: 7d2c 0a20 2020 2020 2020 207b 2253 5044  },.        {"SPD
+00002dd0: 5849 4422 3a20 2253 5044 5852 6566 2d50  XID": "SPDXRef-P
+00002de0: 6163 6b61 6765 222c 2022 6e61 6d65 223a  ackage", "name":
+00002df0: 2035 2c20 2264 6f77 6e6c 6f61 644c 6f63   5, "downloadLoc
+00002e00: 6174 696f 6e22 3a20 224e 4f4e 4522 7d2c  ation": "NONE"},
+00002e10: 0a20 2020 2020 2020 207b 2253 5044 5849  .        {"SPDXI
+00002e20: 4422 3a20 2253 5044 5852 6566 2d50 6163  D": "SPDXRef-Pac
+00002e30: 6b61 6765 222c 2022 6e61 6d65 223a 2022  kage", "name": "
+00002e40: 4578 616d 706c 6520 5061 636b 6167 6522  Example Package"
+00002e50: 2c20 2264 6f77 6e6c 6f61 644c 6f63 6174  , "downloadLocat
+00002e60: 696f 6e22 3a20 224e 4f4e 4522 7d2c 0a20  ion": "NONE"},. 
+00002e70: 2020 205d 0a0a 2020 2020 7769 7468 2070     ]..    with p
+00002e80: 7974 6573 742e 7261 6973 6573 2853 5044  ytest.raises(SPD
+00002e90: 5850 6172 7369 6e67 4572 726f 7229 2061  XParsingError) a
+00002ea0: 7320 6572 723a 0a20 2020 2020 2020 2070  s err:.        p
+00002eb0: 6172 7365 5f6c 6973 745f 6f66 5f65 6c65  arse_list_of_ele
+00002ec0: 6d65 6e74 7328 7061 636b 6167 6573 5f6c  ments(packages_l
+00002ed0: 6973 742c 2070 6163 6b61 6765 5f70 6172  ist, package_par
+00002ee0: 7365 722e 7061 7273 655f 7061 636b 6167  ser.parse_packag
+00002ef0: 6529 0a0a 2020 2020 5465 7374 4361 7365  e)..    TestCase
+00002f00: 2829 2e61 7373 6572 7443 6f75 6e74 4571  ().assertCountEq
+00002f10: 7561 6c28 0a20 2020 2020 2020 2065 7272  ual(.        err
+00002f20: 2e76 616c 7565 2e67 6574 5f6d 6573 7361  .value.get_messa
+00002f30: 6765 7328 292c 0a20 2020 2020 2020 205b  ges(),.        [
+00002f40: 0a20 2020 2020 2020 2020 2020 2027 4572  .            'Er
+00002f50: 726f 7220 7768 696c 6520 7061 7273 696e  ror while parsin
+00002f60: 6720 5061 636b 6167 653a 205b 2245 7272  g Package: ["Err
+00002f70: 6f72 2077 6869 6c65 2070 6172 7369 6e67  or while parsing
+00002f80: 2043 6865 636b 7375 6d3a 2027 2022 5b27   Checksum: ' "['
+00002f90: 496e 7661 6c69 6420 4368 6563 6b73 756d  Invalid Checksum
+00002fa0: 416c 676f 7269 7468 6d3a 2053 4841 275d  Algorithm: SHA']
+00002fb0: 5c22 5d22 2c0a 2020 2020 2020 2020 2020  \"]",.          
+00002fc0: 2020 2245 7272 6f72 2077 6869 6c65 2063    "Error while c
+00002fd0: 6f6e 7374 7275 6374 696e 6720 5061 636b  onstructing Pack
+00002fe0: 6167 653a 205b 2753 6574 7465 7245 7272  age: ['SetterErr
+00002ff0: 6f72 2050 6163 6b61 6765 3a20 7479 7065  or Package: type
+00003000: 206f 6620 6172 6775 6d65 6e74 2022 0a20   of argument ". 
+00003010: 2020 2020 2020 2020 2020 2027 226e 616d             '"nam
+00003020: 6522 206d 7573 7420 6265 2073 7472 3b20  e" must be str; 
+00003030: 676f 7420 696e 7420 696e 7374 6561 643a  got int instead:
+00003040: 2035 5c27 5d27 2c0a 2020 2020 2020 2020   5\']',.        
+00003050: 5d2c 0a20 2020 2029 0a0a 0a64 6566 2074  ],.    )...def t
+00003060: 6573 745f 7061 7273 655f 6578 7465 726e  est_parse_extern
+00003070: 616c 5f72 6566 2829 3a0a 2020 2020 7061  al_ref():.    pa
+00003080: 636b 6167 655f 7061 7273 6572 203d 2050  ckage_parser = P
+00003090: 6163 6b61 6765 5061 7273 6572 2829 0a20  ackageParser(). 
+000030a0: 2020 2065 7874 6572 6e61 6c5f 7265 6620     external_ref 
+000030b0: 3d20 7b22 7265 6665 7265 6e63 6554 7970  = {"referenceTyp
+000030c0: 6522 3a20 2266 6978 227d 0a0a 2020 2020  e": "fix"}..    
+000030d0: 7769 7468 2070 7974 6573 742e 7261 6973  with pytest.rais
+000030e0: 6573 2853 5044 5850 6172 7369 6e67 4572  es(SPDXParsingEr
+000030f0: 726f 7229 2061 7320 6572 723a 0a20 2020  ror) as err:.   
+00003100: 2020 2020 2070 6163 6b61 6765 5f70 6172       package_par
+00003110: 7365 722e 7061 7273 655f 6578 7465 726e  ser.parse_extern
+00003120: 616c 5f72 6566 2865 7874 6572 6e61 6c5f  al_ref(external_
+00003130: 7265 6629 0a0a 2020 2020 5465 7374 4361  ref)..    TestCa
+00003140: 7365 2829 2e61 7373 6572 7443 6f75 6e74  se().assertCount
+00003150: 4571 7561 6c28 0a20 2020 2020 2020 2065  Equal(.        e
+00003160: 7272 2e76 616c 7565 2e67 6574 5f6d 6573  rr.value.get_mes
+00003170: 7361 6765 7328 292c 0a20 2020 2020 2020  sages(),.       
+00003180: 205b 0a20 2020 2020 2020 2020 2020 2022   [.            "
+00003190: 4572 726f 7220 7768 696c 6520 636f 6e73  Error while cons
+000031a0: 7472 7563 7469 6e67 2045 7874 6572 6e61  tructing Externa
+000031b0: 6c50 6163 6b61 6765 5265 663a 205b 2753  lPackageRef: ['S
+000031c0: 6574 7465 7245 7272 6f72 2022 0a20 2020  etterError ".   
+000031d0: 2020 2020 2020 2020 2027 4578 7465 726e           'Extern
+000031e0: 616c 5061 636b 6167 6552 6566 3a20 7479  alPackageRef: ty
+000031f0: 7065 206f 6620 6172 6775 6d65 6e74 2022  pe of argument "
+00003200: 6361 7465 676f 7279 2220 6d75 7374 2062  category" must b
+00003210: 6520 270a 2020 2020 2020 2020 2020 2020  e '.            
+00003220: 2273 7064 785f 746f 6f6c 732e 7370 6478  "spdx_tools.spdx
+00003230: 2e6d 6f64 656c 2e70 6163 6b61 6765 2e45  .model.package.E
+00003240: 7874 6572 6e61 6c50 6163 6b61 6765 5265  xternalPackageRe
+00003250: 6643 6174 6567 6f72 793b 2067 6f74 204e  fCategory; got N
+00003260: 6f6e 6554 7970 6520 696e 7374 6561 643a  oneType instead:
+00003270: 204e 6f6e 6527 2c20 220a 2020 2020 2020   None', ".      
+00003280: 2020 2020 2020 275c 2753 6574 7465 7245        '\'SetterE
+00003290: 7272 6f72 2045 7874 6572 6e61 6c50 6163  rror ExternalPac
+000032a0: 6b61 6765 5265 663a 2074 7970 6520 6f66  kageRef: type of
+000032b0: 2061 7267 756d 656e 7420 226c 6f63 6174   argument "locat
+000032c0: 6f72 2220 6d75 7374 2062 6520 7374 723b  or" must be str;
+000032d0: 2027 0a20 2020 2020 2020 2020 2020 2022   '.            "
+000032e0: 676f 7420 4e6f 6e65 5479 7065 2069 6e73  got NoneType ins
+000032f0: 7465 6164 3a20 4e6f 6e65 275d 220a 2020  tead: None']".  
+00003300: 2020 2020 2020 5d2c 0a20 2020 2029 0a0a        ],.    )..
+00003310: 0a64 6566 2074 6573 745f 7061 7273 655f  .def test_parse_
+00003320: 696e 7661 6c69 645f 6578 7465 726e 616c  invalid_external
+00003330: 5f70 6163 6b61 6765 5f72 6566 5f63 6174  _package_ref_cat
+00003340: 6567 6f72 7928 293a 0a20 2020 2070 6163  egory():.    pac
+00003350: 6b61 6765 5f70 6172 7365 7220 3d20 5061  kage_parser = Pa
+00003360: 636b 6167 6550 6172 7365 7228 290a 2020  ckageParser().  
+00003370: 2020 6578 7465 726e 616c 5f70 6163 6b61    external_packa
+00003380: 6765 5f72 6566 5f63 6174 6567 6f72 7920  ge_ref_category 
+00003390: 3d20 2254 4553 5422 0a0a 2020 2020 7769  = "TEST"..    wi
+000033a0: 7468 2070 7974 6573 742e 7261 6973 6573  th pytest.raises
+000033b0: 2853 5044 5850 6172 7369 6e67 4572 726f  (SPDXParsingErro
+000033c0: 7229 2061 7320 6572 723a 0a20 2020 2020  r) as err:.     
+000033d0: 2020 2070 6163 6b61 6765 5f70 6172 7365     package_parse
+000033e0: 722e 7061 7273 655f 6578 7465 726e 616c  r.parse_external
+000033f0: 5f72 6566 5f63 6174 6567 6f72 7928 6578  _ref_category(ex
+00003400: 7465 726e 616c 5f70 6163 6b61 6765 5f72  ternal_package_r
+00003410: 6566 5f63 6174 6567 6f72 7929 0a0a 2020  ef_category)..  
+00003420: 2020 5465 7374 4361 7365 2829 2e61 7373    TestCase().ass
+00003430: 6572 7443 6f75 6e74 4571 7561 6c28 6572  ertCountEqual(er
+00003440: 722e 7661 6c75 652e 6765 745f 6d65 7373  r.value.get_mess
+00003450: 6167 6573 2829 2c20 5b22 496e 7661 6c69  ages(), ["Invali
+00003460: 6420 4578 7465 726e 616c 5061 636b 6167  d ExternalPackag
+00003470: 6552 6566 4361 7465 676f 7279 3a20 5445  eRefCategory: TE
+00003480: 5354 225d 290a                           ST"]).
```

### Comparing `spdx-tools-0.7.1rc1/tests/data/formats/SPDXTagExample-v2.2.spdx` & `spdx-tools-0.8.0a1/tests/spdx/data/SPDXTagExample-v2.2.spdx`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.7.1rc1/tests/data/formats/SPDXTagExample-v2.3.spdx` & `spdx-tools-0.8.0a1/tests/spdx/data/SPDXTagExample-v2.3.spdx`

 * *Files 1% similar despite different names*

```diff
@@ -1145,14 +1145,15 @@
 00004780: 5920 4f46 2053 5543 4820 4441 4d41 4745  Y OF SUCH DAMAGE
 00004790: 2e3c 2f74 6578 743e 0a4c 6963 656e 7365  .</text>.License
 000047a0: 4e61 6d65 3a20 4379 6265 724e 656b 6f20  Name: CyberNeko 
 000047b0: 4c69 6365 6e73 650a 4c69 6365 6e73 6543  License.LicenseC
 000047c0: 726f 7373 5265 6665 7265 6e63 653a 2068  rossReference: h
 000047d0: 7474 703a 2f2f 7065 6f70 6c65 2e61 7061  ttp://people.apa
 000047e0: 6368 652e 6f72 672f 7e61 6e64 7963 2f6e  che.org/~andyc/n
-000047f0: 656b 6f2f 4c49 4345 4e53 452c 2068 7474  eko/LICENSE, htt
-00004800: 703a 2f2f 6a75 7374 6173 616d 706c 652e  p://justasample.
-00004810: 7572 6c2e 636f 6d0a 4c69 6365 6e73 6543  url.com.LicenseC
-00004820: 6f6d 6d65 6e74 3a20 3c74 6578 743e 5468  omment: <text>Th
-00004830: 6973 2069 7320 7479 6520 4379 7065 724e  is is tye CyperN
-00004840: 656b 6f20 4c69 6365 6e73 653c 2f74 6578  eko License</tex
-00004850: 743e 0a0a                                t>..
+000047f0: 656b 6f2f 4c49 4345 4e53 450a 4c69 6365  eko/LICENSE.Lice
+00004800: 6e73 6543 726f 7373 5265 6665 7265 6e63  nseCrossReferenc
+00004810: 653a 2068 7474 703a 2f2f 6a75 7374 6173  e: http://justas
+00004820: 616d 706c 652e 7572 6c2e 636f 6d0a 4c69  ample.url.com.Li
+00004830: 6365 6e73 6543 6f6d 6d65 6e74 3a20 3c74  censeComment: <t
+00004840: 6578 743e 5468 6973 2069 7320 7479 6520  ext>This is tye 
+00004850: 4379 7065 724e 656b 6f20 4c69 6365 6e73  CyperNeko Licens
+00004860: 653c 2f74 6578 743e 0a0a                 e</text>..
```

### Comparing `spdx-tools-0.7.1rc1/tests/data/formats/SPDXXMLExample-v2.2.spdx.xml` & `spdx-tools-0.8.0a1/tests/spdx/data/SPDXXMLExample-v2.2.spdx.xml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.7.1rc1/tests/data/formats/SPDXXMLExample-v2.3.spdx.xml` & `spdx-tools-0.8.0a1/tests/spdx/data/SPDXXMLExample-v2.3.spdx.xml`

 * *Files 1% similar despite different names*

#### Comparing `spdx-tools-0.7.1rc1/tests/data/formats/SPDXXMLExample-v2.3.spdx.xml` & `spdx-tools-0.8.0a1/tests/spdx/data/SPDXXMLExample-v2.3.spdx.xml`

```diff
@@ -167,14 +167,15 @@
   <annotations>
     <annotationDate>2011-03-13T00:00:00Z</annotationDate>
     <annotationType>REVIEW</annotationType>
     <annotator>Person: Suzanne Reviewer</annotator>
     <comment>Another example reviewer.</comment>
   </annotations>
   <documentDescribes>SPDXRef-File</documentDescribes>
+  <documentDescribes>SPDXRef-File</documentDescribes>
   <documentDescribes>SPDXRef-Package</documentDescribes>
   <documentNamespace>http://spdx.org/spdxdocs/spdx-example-444504E0-4F89-41D3-9A0C-0305E82C3301</documentNamespace>
   <packages>
     <SPDXID>SPDXRef-Package</SPDXID>
     <annotations>
       <annotationDate>2011-01-29T18:30:22Z</annotationDate>
       <annotationType>OTHER</annotationType>
@@ -262,15 +263,15 @@
   </packages>
   <packages>
     <SPDXID>SPDXRef-fromDoap-0</SPDXID>
     <downloadLocation>https://search.maven.org/remotecontent?filepath=org/apache/jena/apache-jena/3.12.0/apache-jena-3.12.0.tar.gz</downloadLocation>
     <externalRefs>
       <referenceCategory>PACKAGE-MANAGER</referenceCategory>
       <referenceLocator>pkg:maven/org.apache.jena/apache-jena@3.12.0</referenceLocator>
-      <referenceType>purl</referenceType>
+      <referenceType>http://spdx.org/spdxdocs/spdx-example-444504E0-4F89-41D3-9A0C-0305E82C3301#purl</referenceType>
     </externalRefs>
     <filesAnalyzed>false</filesAnalyzed>
     <homepage>http://www.openjena.org/</homepage>
     <name>Jena</name>
     <versionInfo>3.12.0</versionInfo>
   </packages>
   <packages>
```

### Comparing `spdx-tools-0.7.1rc1/tests/data/formats/SPDXYAMLExample-2.2.spdx.yaml` & `spdx-tools-0.8.0a1/tests/spdx/data/SPDXYAMLExample-v2.2.spdx.yaml`

 * *Files identical despite different names*

### Comparing `spdx-tools-0.7.1rc1/tests/data/formats/SPDXYAMLExample-2.3.spdx.yaml` & `spdx-tools-0.8.0a1/tests/spdx/data/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,15 @@
   licenseDeclared: "NOASSERTION"
   name: "Apache Commons Lang"
 - SPDXID: "SPDXRef-fromDoap-0"
   downloadLocation: "https://search.maven.org/remotecontent?filepath=org/apache/jena/apache-jena/3.12.0/apache-jena-3.12.0.tar.gz"
   externalRefs:
   - referenceCategory: "PACKAGE-MANAGER"
     referenceLocator: "pkg:maven/org.apache.jena/apache-jena@3.12.0"
-    referenceType: "purl"
+    referenceType: "http://spdx.org/spdxdocs/spdx-example-444504E0-4F89-41D3-9A0C-0305E82C3301#purl"
   filesAnalyzed: false
   homepage: "http://www.openjena.org/"
   name: "Jena"
   versionInfo: "3.12.0"
 - SPDXID: "SPDXRef-Saxon"
   checksums:
   - algorithm: "SHA1"
```

### Comparing `spdx-tools-0.7.1rc1/tests/test_rdf_writer.py` & `spdx-tools-0.8.0a1/tests/spdx/parser/rdf/test_package_parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,117 +1,97 @@
+# SPDX-FileCopyrightText: 2023 spdx contributors
+#
+# SPDX-License-Identifier: Apache-2.0
 import os
-from typing import Optional
 from unittest import TestCase
 
 import pytest
-from rdflib import URIRef
+from license_expression import get_spdx_licensing
+from rdflib import RDF, BNode, Graph, Literal, URIRef
 
-from spdx.document import Document
-from spdx.license import License
-from spdx.package import Package, ExternalPackageRef
-from spdx.parsers.loggers import StandardLogger
-from spdx.parsers.parse_anything import parse_file
-from spdx.parsers.rdf import Parser
-from spdx.parsers.rdfbuilders import Builder
-from spdx.utils import NoAssert
-from spdx.writers.rdf import Writer
-
-
-@pytest.fixture
-def temporary_file_path() -> str:
-    temporary_file_path = "temp_accept_provided_doc_node.rdf.xml"
-    yield temporary_file_path
-    os.remove(temporary_file_path)
-
-
-# This test is really clunky since it's hard to isolate features of the rdf writer to test. Should be improved when
-# that part is refactored.
-def test_accept_provided_doc_node(temporary_file_path) -> None:
-    doc_node = URIRef("http://www.spdx.org/tools#SPDXRef-DOCUMENT")
-    document: Document = minimal_document_with_package()
-
-    with open(temporary_file_path, "wb") as out:
-        writer = Writer(document, out)
-        writer.write(doc_node)
-    parser = Parser(Builder(), StandardLogger())
-    with open(temporary_file_path, "r") as file:
-        parsed_document: Document = parser.parse(file)[0]
-
-    # These properties are set automatically if no doc_node is provided. Instead, we provided an empty one
-    assert parsed_document.data_license is None
-    assert parsed_document.namespace is None
-    assert parsed_document.spdx_id is None
-
-
-def test_external_package_references(temporary_file_path) -> None:
-    document: Document = minimal_document_with_package()
-    package: Package = document.packages[0]
-    first_ref = ExternalPackageRef(category="PACKAGE-MANAGER")
-    second_ref = ExternalPackageRef(category="SECURITY")
-    package.add_pkg_ext_refs(first_ref)
-    package.add_pkg_ext_refs(second_ref)
-
-    # Not using write_anything here because we don't want to deal with validation
-    with open(temporary_file_path, "wb") as out:
-        writer = Writer(document, out)
-        writer.write()
-
-    parsed_document = parse_file(temporary_file_path)[0]
-    parsed_package: Package = parsed_document.packages[0]
-
-    assert len(parsed_package.pkg_ext_refs) is 2
-    parsed_reference_categories = list(map(lambda x: x.category, parsed_package.pkg_ext_refs))
-    assert first_ref.category in parsed_reference_categories
-    assert second_ref.category in parsed_reference_categories
-
-
-# This test is really clunky since it's hard to isolate features of the rdf writer to test. Should be improved when
-# that part is refactored.
-def test_multiple_packages_in_one_document(temporary_file_path) -> None:
-    doc_node = URIRef("http://www.spdx.org/tools#SPDXRef-DOCUMENT")
-    document = Document()
-    document.creation_info.set_created_now()
-    package = Package()
-    package.spdx_id = "SPDXRef-Package"
-    package.version = "2.1"
-    document.add_package(package)
-    package2 = Package()
-    package2.spdx_id = "SPDXRef-Another-Package"
-    package2.version = "2.3"
-    document.add_package(package2)
-
-    with open(temporary_file_path, "wb") as out:
-        writer = Writer(document, out)
-        writer.write(doc_node)
-    parser = Parser(Builder(), StandardLogger())
-    with open(temporary_file_path, "r") as file:
-        parsed_document: Document = parser.parse(file)[0]
-
-    assert len(parsed_document.packages) == 2
-    first_package = get_package_by_spdx_id("SPDXRef-Package", document)
-    assert first_package.version == "2.1"
-    second_package = get_package_by_spdx_id("SPDXRef-Another-Package", document)
-    assert second_package.version == "2.3"
-
-
-def minimal_document_with_package() -> Document:
-    document = Document(data_license=License.from_identifier('CC0-1.0'))
-    document.creation_info.set_created_now()
-    package: Package = minimal_package()
-    document.add_package(package)
-    return document
-
-
-def minimal_package() -> Package:
-    package = Package()
-    package.spdx_id = "SPDXRef-Package"
-    package.conc_lics = NoAssert()
-    package.license_declared = NoAssert()
-    package.add_lics_from_file(NoAssert())
-    return package
-
-
-def get_package_by_spdx_id(package_spdx_id: str, document: Document) -> Optional[Package]:
-    for package in document.packages:
-        if package.spdx_id == package_spdx_id:
-            return package
-    return None
+from spdx_tools.spdx.model import (
+    Actor,
+    ActorType,
+    Checksum,
+    ChecksumAlgorithm,
+    ExternalPackageRefCategory,
+    PackagePurpose,
+    PackageVerificationCode,
+    SpdxNoAssertion,
+)
+from spdx_tools.spdx.parser.rdf.package_parser import parse_external_package_ref, parse_package
+from spdx_tools.spdx.rdfschema.namespace import SPDX_NAMESPACE
+
+
+def test_package_parser():
+    graph = Graph().parse(os.path.join(os.path.dirname(__file__), "data/file_to_test_rdf_parser.rdf.xml"))
+    # we have two packages in the test file, graph.value() will return the first package
+    package_node = graph.value(predicate=RDF.type, object=SPDX_NAMESPACE.Package)
+    doc_namespace = "https://some.namespace"
+    assert isinstance(package_node, URIRef)
+
+    package = parse_package(package_node, graph, doc_namespace)
+
+    assert package.spdx_id == "SPDXRef-Package"
+    assert package.name == "packageName"
+    assert package.download_location == "https://download.com"
+    assert package.version == "12.2"
+    assert package.file_name == "./packageFileName"
+    assert package.homepage == "https://homepage.com"
+    assert package.files_analyzed is True
+    assert package.checksums == [Checksum(ChecksumAlgorithm.SHA1, "71c4025dd9897b364f3ebbb42c484ff43d00791c")]
+    assert package.source_info == "sourceInfo"
+    assert package.license_concluded == get_spdx_licensing().parse("MIT AND GPL-2.0")
+    assert package.license_declared == get_spdx_licensing().parse("MIT AND GPL-2.0")
+    TestCase().assertCountEqual(
+        package.license_info_from_files,
+        [get_spdx_licensing().parse("MIT"), get_spdx_licensing().parse("GPL-2.0"), SpdxNoAssertion()],
+    )
+    assert package.license_comment == "packageLicenseComment"
+    assert package.copyright_text == "packageCopyrightText"
+    assert package.verification_code == PackageVerificationCode(
+        value="85ed0817af83a24ad8da68c2b5094de69833983c", excluded_files=["./exclude.py"]
+    )
+    assert len(package.external_references) == 1
+    assert package.summary == "packageSummary"
+    assert package.description == "packageDescription"
+    assert package.comment == "packageComment"
+    assert package.attribution_texts == ["packageAttributionText"]
+    assert package.primary_package_purpose == PackagePurpose.SOURCE
+    assert package.supplier == Actor(ActorType.PERSON, "supplierName", "some@mail.com")
+    assert package.originator == Actor(ActorType.PERSON, "originatorName", "some@mail.com")
+
+
+@pytest.mark.parametrize(
+    "download_location,category,locator,type,comment",
+    [
+        (
+            "https://download.com",
+            ExternalPackageRefCategory.PACKAGE_MANAGER,
+            "org.apache.tomcat:tomcat:9.0.0.M4",
+            "maven-central",
+            "externalPackageRefComment",
+        ),
+        (
+            "http://differentdownload.com",
+            ExternalPackageRefCategory.OTHER,
+            "acmecorp/acmenator/4.1.3-alpha",
+            "LocationRef-acmeforge",
+            "This is the external ref for Acme",
+        ),
+    ],
+)
+def test_external_package_ref_parser(download_location, category, locator, type, comment):
+    graph = Graph().parse(os.path.join(os.path.dirname(__file__), "data/file_to_test_rdf_parser.rdf.xml"))
+    doc_namespace = "https://some.namespace"
+    # we use the download location to identify the package node
+    # in the test file we have two different external package refs depending on the package
+    package_node = graph.value(predicate=SPDX_NAMESPACE.downloadLocation, object=Literal(download_location))
+    external_package_ref_node = graph.value(package_node, SPDX_NAMESPACE.externalRef)
+    assert isinstance(external_package_ref_node, BNode)
+
+    external_package_ref = parse_external_package_ref(external_package_ref_node, graph, doc_namespace)
+
+    assert external_package_ref.category == category
+    assert external_package_ref.locator == locator
+    assert external_package_ref.reference_type == type
+    assert external_package_ref.comment == comment
```

