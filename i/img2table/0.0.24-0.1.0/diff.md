# Comparing `tmp/img2table-0.0.24.tar.gz` & `tmp/img2table-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/img2table-0.0.24.tar", last modified: Tue Apr 11 08:05:20 2023, max compression
+gzip compressed data, was "dist/img2table-0.1.0.tar", last modified: Thu Apr 20 06:49:02 2023, max compression
```

## Comparing `img2table-0.0.24.tar` & `img2table-0.1.0.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 08:03:24.000000 img2table-0.0.24/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-11 08:03:24.000000 img2table-0.0.24/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-11 08:03:24.000000 img2table-0.0.24/.github/workflows/test_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 08:03:24.000000 img2table-0.0.24/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-11 08:03:24.000000 img2table-0.0.24/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-04-11 08:05:20.000000 img2table-0.0.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-04-11 08:03:24.000000 img2table-0.0.24/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-11 08:03:24.000000 img2table-0.0.24/activate_venv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    46045 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/Basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    32897 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/Implicit_rows.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/borderless.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)    71022 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/data/borderless_aws.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/data/borderless_ocr.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/data/tables.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/data/tables.png
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-11 08:03:24.000000 img2table-0.0.24/examples/data/tables.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 08:03:24.000000 img2table-0.0.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-11 08:03:24.000000 img2table-0.0.24/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-11 08:03:24.000000 img2table-0.0.24/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-11 08:03:24.000000 img2table-0.0.24/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-11 08:05:20.000000 img2table-0.0.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 08:03:24.000000 img2table-0.0.24/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/document/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/document/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/document/base/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/document/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/document/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/aws_textract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/google_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/paddle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/ocr/tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/objects/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/objects/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/objects/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/objects/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/cells/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/column_delimiters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/table/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/borderless_tables/table/table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-11 08:03:24.000000 img2table-0.0.24/src/img2table/tables/processing/text/titles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 08:05:20.000000 img2table-0.0.24/src/img2table.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/_mock_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/_mock_data/azure.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/_mock_data/tesseract_hocr.html
--rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/_mock_data/textract.json
--rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/_mock_data/vision.json
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/_mock_data/vision.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/document/base/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/base/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/base/test_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/document/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/document/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/image/test_data/expected.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/image/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/document/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/document/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/document/pdf/test_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/aws_textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/aws_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/aws_textract/test_aws_textract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/aws_textract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/aws_textract/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/aws_textract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/aws_textract/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/azure/test_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/azure/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/azure/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/azure/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/data/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/data/test_data/expected_table.json
--rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/data/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/data/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/data/test_ocr_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/google_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/google_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/google_vision/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/google_vision/test_data/expected_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/google_vision/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/google_vision/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/google_vision/test_google_vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/paddle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/paddle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/paddle/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/paddle/test_data/hocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/paddle/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/paddle/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/paddle/test_paddle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    35369 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/pdf/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/pdf/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/pdf/test_pdf_ocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/tesseract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/tesseract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/ocr/tesseract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/tesseract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/tesseract/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/ocr/tesseract/test_tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/image/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/image/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/image/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/objects/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/test_data/tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/test_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/test_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/objects/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/cells.json
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/implicit_ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/lines/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/table/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/table/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/borderless_tables/table/test_table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/common/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/common/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/common/test_data/test.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/prepare_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/prepare_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/prepare_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/prepare_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/prepare_image/test_prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:05:20.000000 img2table-0.0.24/tests/tables/processing/text/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/text/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/text/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/text/test_data/test.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-11 08:03:24.000000 img2table-0.0.24/tests/tables/processing/text/test_titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-20 06:47:06.000000 img2table-0.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-20 06:47:06.000000 img2table-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-20 06:47:06.000000 img2table-0.1.0/.github/workflows/test_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 06:47:06.000000 img2table-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-20 06:47:06.000000 img2table-0.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    19971 2023-04-20 06:49:02.000000 img2table-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-04-20 06:47:06.000000 img2table-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-20 06:47:06.000000 img2table-0.1.0/activate_venv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    46045 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/Basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/Implicit_rows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18538 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/borderless.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    71022 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/data/borderless_aws.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/data/borderless_ocr.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/data/tables.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/data/tables.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-20 06:47:06.000000 img2table-0.1.0/examples/data/tables.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 06:47:06.000000 img2table-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-20 06:47:06.000000 img2table-0.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-20 06:47:06.000000 img2table-0.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-20 06:47:06.000000 img2table-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-20 06:49:02.000000 img2table-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 06:47:06.000000 img2table-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/document/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/document/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/document/base/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/document/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/document/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/aws_textract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/google_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/ocr/tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/objects/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/objects/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/objects/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/objects/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/cells/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/column_delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/table/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/borderless_tables/table/table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-20 06:47:06.000000 img2table-0.1.0/src/img2table/tables/processing/text/titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19971 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 06:49:02.000000 img2table-0.1.0/src/img2table.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/_mock_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/_mock_data/azure.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/_mock_data/tesseract_hocr.html
+-rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/_mock_data/textract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/_mock_data/vision.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/_mock_data/vision.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/document/base/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/base/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/base/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/document/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/document/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/image/test_data/dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/image/test_data/expected.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/image/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/document/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/document/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/document/pdf/test_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/aws_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/aws_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/aws_textract/test_aws_textract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/aws_textract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/aws_textract/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/aws_textract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/aws_textract/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/azure/test_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/azure/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/azure/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/azure/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/data/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/data/test_data/expected_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/data/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/data/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/data/test_ocr_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/google_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/google_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/google_vision/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/google_vision/test_data/expected_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/google_vision/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/google_vision/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/google_vision/test_google_vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/paddle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/paddle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/paddle/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/paddle/test_data/hocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/paddle/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/paddle/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/paddle/test_paddle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/pdf/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/pdf/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/pdf/test_pdf_ocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/tesseract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/tesseract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/ocr/tesseract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/tesseract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/tesseract/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/ocr/tesseract/test_tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/image/test_data/expected_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/image/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/image/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/image/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/objects/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/test_data/expected_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/test_data/tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/test_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/objects/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/table/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/table/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/borderless_tables/table/test_table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/common/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/common/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/common/test_data/test.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/prepare_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/prepare_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/prepare_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/prepare_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/prepare_image/test_prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:49:02.000000 img2table-0.1.0/tests/tables/processing/text/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/text/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/text/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/text/test_data/test.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-20 06:47:06.000000 img2table-0.1.0/tests/tables/processing/text/test_titles.py
```

### Comparing `img2table-0.0.24/LICENSE.txt` & `img2table-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/Makefile` & `img2table-0.1.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 VENV = ./activate_venv
 DIR := $(shell pwd)
 export PYTHONPATH := $(DIR)/src
 
 # Virtual environment commands
 venv:
 	python -m venv ./venv || true
-	. $(VENV); python -m pip install pip --upgrade;
+	. $(VENV); python -m pip install pip wheel --upgrade;
 	. $(VENV); python -m pip install -r requirements-dev.txt
 
 update: venv
 	. $(VENV); python -m pip install -r requirements-dev.txt
 
 # Test commands
 test:
```

### Comparing `img2table-0.0.24/PKG-INFO` & `img2table-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 0.0.24
+Version: 0.1.0
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image 
@@ -66,14 +66,18 @@
         
         ## Supported file formats <a name="supported-file-formats"></a>
         
         ### Images <a name="images-formats"></a>
         
         Images are loaded using the `opencv-python` library, supported formats are listed below.
         
+        <details>
+        <summary>Supported image formats</summary>
+        <br>
+        
         <blockquote>
         <ul>
         <li>Windows bitmaps - <em>.bmp, </em>.dib</li>
         <li>JPEG files - <em>.jpeg, </em>.jpg, *.jpe</li>
         <li>JPEG 2000 files - *.jp2</li>
         <li>Portable Network Graphics - *.png</li>
         <li>WebP - *.webp</li>
@@ -83,15 +87,16 @@
         <li>TIFF files - <em>.tiff, </em>.tif</li>
         <li>OpenEXR Image files - *.exr</li>
         <li>Radiance HDR - <em>.hdr, </em>.pic</li>
         <li>Raster and Vector geospatial data supported by GDAL<br>
         <cite><a href="https://docs.opencv.org/4.x/d4/da8/group__imgcodecs.html#ga288b8b3da0892bd651fce07b3bbd3a56">OpenCV: Image file reading and writing</a></cite></li>
         </ul>
         </blockquote>
-        
+        </details>
+        <br>
         Multi-page images are not supported.
         
         ---
         
         ### PDF <a name="pdf-formats"></a>
         
         Both native and scanned PDF files are supported.
@@ -102,61 +107,58 @@
         
         #### Images <a name="images-doc"></a>
         Images are instantiated as follows :
         ```python
         from img2table.document import Image
         
         image = Image(src, 
-                      dpi=200,
                       detect_rotation=False)
         ```
         
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>src : str, <code>pathlib.Path</code>, bytes or <code>io.BytesIO</code>, required</dt>
         >    <dd style="font-style: italic;">Image source</dd>
-        >    <dt>dpi : int, optional, default <code>200</code></dt>
-        >    <dd style="font-style: italic;">Estimated image dpi, used to adapt OpenCV algorithm parameters</dd>
         >    <dt>detect_rotation : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Detect and correct skew/rotation of the image</dd>
         ></dl>
-        
         <br>
-        
         The implemented method to handle skewed/rotated images supports skew angles up to 45° and is
         based on the publication by <a href="https://www.mdpi.com/2079-9292/9/1/55">Huang, 2020</a>.<br>
-        Setting the `detect_rotation` parameter to `True`, image coordinates and bounding boxes returned by other 
+        Setting the <code>detect_rotation</code> parameter to <code>True</code>, image coordinates and bounding boxes returned by other 
         methods might not correspond to the original image.
         
         #### PDF <a name="pdf-doc"></a>
         PDF files are instantiated as follows :
         ```python
         from img2table.document import PDF
         
-        pdf = PDF(src, dpi=200, pages=[0, 2])
+        pdf = PDF(src, pages=[0, 2])
         ```
         
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>src : str, <code>pathlib.Path</code>, bytes or <code>io.BytesIO</code>, required</dt>
         >    <dd style="font-style: italic;">PDF source</dd>
-        >    <dt>dpi : int, optional, default <code>200</code></dt>
-        >    <dd style="font-style: italic;">Dpi used for conversion of PDF pages to images</dd>
         >    <dt>pages : list, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">List of PDF page indexes to be processed. If None, all pages are processed</dd>
         ></dl>
         
+        PDF pages are converted to images with a 200 DPI for table identification.
+        
         ---
         
         ### OCR <a name="ocr"></a>
         
         `img2table` provides an interface for several OCR services and tools in order to parse table content.<br>
         If possible (i.e for searchable PDF), PDF text will be extracted directly from the file and the OCR service/tool will not be called.
         
-        #### Tesseract <a name="tesseract"></a>
+        <details>
+        <summary>Tesseract<a name="tesseract"></a></summary>
+        <br>
         
         ```python
         from img2table.ocr import TesseractOCR
         
         ocr = TesseractOCR(n_threads=1, 
                            lang="eng", 
                            psm=11,
@@ -174,21 +176,24 @@
         >    <dt>tessdata_dir : str, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">Directory containing Tesseract traineddata files. If None, the <code>TESSDATA_PREFIX</code> env variable is used.</dd>
         ></dl>
         
         
         *Usage of [Tesseract-OCR](https://github.com/tesseract-ocr/tesseract) requires prior installation. 
         Check [documentation](https://tesseract-ocr.github.io/tessdoc/) for instructions.*
+        <br>
+        </details>
         
-        
-        #### <a href="https://github.com/PaddlePaddle/PaddleOCR">PaddleOCR</a> <a name="paddle"></a>
+        <details>
+        <summary>PaddleOCR<a name="paddle"></a></summary>
+        <br>
         
         *Available for Python versions <= 3.10*
         
-        PaddleOCR is an open-source OCR based on Deep Learning models.<br>
+        <a href="https://github.com/PaddlePaddle/PaddleOCR">PaddleOCR</a> is an open-source OCR based on Deep Learning models.<br>
         At first use, relevant languages models will be downloaded.
         
         ```python
         from img2table.ocr import PaddleOCR
         
         ocr = PaddleOCR(lang="en")
         ```
@@ -196,16 +201,20 @@
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>lang : str, optional, default <code>"en"</code></dt>
         >    <dd style="font-style: italic;">Lang parameter used in Paddle for text extraction, check <a href="https://github.com/Mushroomcat9998/PaddleOCR/blob/main/doc/doc_en/multi_languages_en.md#5-support-languages-and-abbreviations">documentation for available languages</a></dd>
         ></dl>
         
         *Released in version 0.0.13*
+        <br>
+        </details>
         
-        #### Google Vision <a name="vision"></a>
+        <details>
+        <summary>Google Vision<a name="vision"></a></summary>
+        <br>
         
         Authentication to GCP can be done by setting the standard `GOOGLE_APPLICATION_CREDENTIALS` environment variable.<br>
         If this variable is missing, an API key should be provided via the `api_key` parameter.
         
         ```python
         from img2table.ocr import VisionOCR
         
@@ -215,16 +224,20 @@
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>api_key : str, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">Google Vision API key</dd>
         >    <dt>timeout : int, optional, default <code>15</code></dt>
         >    <dd style="font-style: italic;">API requests timeout, in seconds</dd>
         ></dl>
+        <br>
+        </details>
         
-        #### AWS Textract <a name="textract"></a>
+        <details>
+        <summary>AWS Textract<a name="textract"></a></summary>
+        <br>
         
         When using AWS Textract, the DetectDocumentText API is exclusively called.
         
         Authentication to AWS can be done by passing credentials to the `TextractOCR` class.<br>
         If credentials are not provided, authentication is done using environment variables or configuration files. 
         Check `boto3` [documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) for more details.
         
@@ -244,17 +257,20 @@
         >    <dt>aws_secret_access_key : str, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">AWS secret access key</dd>
         >    <dt>aws_session_token : str, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">AWS temporary session token</dd>
         >    <dt>region : str, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">AWS server region</dd>
         ></dl>
+        <br>
+        </details>
         
-        
-        #### Azure Cognitive Services <a name="azure"></a>
+        <details>
+        <summary>Azure Cognitive Services<a name="azure"></a></summary>
+        <br>
         
         ```python
         from img2table.ocr import AzureOCR
         
         ocr = AzureOCR(endpoint="abc.azure.com",
                        subscription_key="***")
         ```
@@ -262,15 +278,16 @@
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>endpoint : str, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">Azure Cognitive Services endpoint. If None, inferred from the <code>COMPUTER_VISION_ENDPOINT</code> environment variable.</dd>
         >    <dt>subscription_key : str, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">Azure Cognitive Services subscription key. If None, inferred from the <code>COMPUTER_VISION_SUBSCRIPTION_KEY</code> environment variable.</dd>
         ></dl>
-        
+        <br>
+        </details>
         
         ---
         
         ### Table extraction <a name="table-extract"></a>
         
         Multiple tables can be extracted at once from a PDF page/ an image using the `extract_tables` method of a document.
         
@@ -278,15 +295,15 @@
         from img2table.ocr import TesseractOCR
         from img2table.document import Image
         
         # Instantiation of OCR
         ocr = TesseractOCR(n_threads=1, lang="eng")
         
         # Instantiation of document, either an image or a PDF
-        doc = Image(src, dpi=200)
+        doc = Image(src)
         
         # Table extraction
         extracted_tables = doc.extract_tables(ocr=ocr,
                                               implicit_rows=True,
                                               borderless_tables=False,
                                               min_confidence=50)
         ```
@@ -349,15 +366,15 @@
         from img2table.ocr import TesseractOCR
         from img2table.document import Image
         
         # Instantiation of OCR
         ocr = TesseractOCR(n_threads=1, lang="eng")
         
         # Instantiation of document, either an image or a PDF
-        doc = Image(src, dpi=200)
+        doc = Image(src)
         
         # Extraction of tables and creation of an xlsx file containing tables
         doc.to_xlsx(dest=dest,
                     ocr=ocr,
                     implicit_rows=True,
                     borderless_tables=False,
                     min_confidence=50)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 0.0.24 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 0.1.0 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
@@ -24,96 +24,106 @@
 files, including bounding boxes at the table cell level * Handling of complex
 table structures such as merged cells * Handling of implicit rows - see
 [example](/examples/Implicit_rows.ipynb) * Table content extraction by
 providing support for OCR services / tools * Extracted tables are returned as a
 simple object, including a Pandas DataFrame representation * Export extracted
 tables to an Excel file, preserving their original structure ## Supported file
 formats  ### Images  Images are loaded using the `opencv-python` library,
-supported formats are listed below.
+supported formats are listed below.  Supported image formats
          * Windows bitmaps - .bmp,.dib
          * JPEG files - .jpeg,.jpg, *.jpe
          * JPEG 2000 files - *.jp2
          * Portable Network Graphics - *.png
          * WebP - *.webp
          * Portable image format - .pbm,.pgm, .ppm.pxm, *.pnm
          * PFM files - *.pfm
          * Sun rasters - .sr,.ras
          * TIFF files - .tiff,.tif
          * OpenEXR Image files - *.exr
          * Radiance HDR - .hdr,.pic
          * Raster and Vector geospatial data supported by GDAL
            OpenCV:_Image_file_reading_and_writing
+
 Multi-page images are not supported. --- ### PDF  Both native and scanned PDF
 files are supported. ## Usage  ### Documents  #### Images  Images are
 instantiated as follows : ```python from img2table.document import Image image
-= Image(src, dpi=200, detect_rotation=False) ``` >
+= Image(src, detect_rotation=False) ``` >
 *** Parameters ***
 >
 >
 
 The implemented method to handle skewed/rotated images supports skew angles up
 to 45Â° and is based on the publication by Huang,_2020.
-Setting the `detect_rotation` parameter to `True`, image coordinates and
-bounding boxes returned by other methods might not correspond to the original
-image. #### PDF  PDF files are instantiated as follows : ```python from
-img2table.document import PDF pdf = PDF(src, dpi=200, pages=[0, 2]) ``` >
+Setting the detect_rotation parameter to True, image coordinates and bounding
+boxes returned by other methods might not correspond to the original image.
+#### PDF  PDF files are instantiated as follows : ```python from
+img2table.document import PDF pdf = PDF(src, pages=[0, 2]) ``` >
 *** Parameters ***
 >
 >
---- ### OCR  `img2table` provides an interface for several OCR services and
-tools in order to parse table content.
+PDF pages are converted to images with a 200 DPI for table identification. --
+- ### OCR  `img2table` provides an interface for several OCR services and tools
+in order to parse table content.
 If possible (i.e for searchable PDF), PDF text will be extracted directly from
-the file and the OCR service/tool will not be called. #### Tesseract  ```python
-from img2table.ocr import TesseractOCR ocr = TesseractOCR(n_threads=1,
-lang="eng", psm=11, tessdata_dir="...") ``` >
+the file and the OCR service/tool will not be called.  Tesseract
+```python from img2table.ocr import TesseractOCR ocr = TesseractOCR
+(n_threads=1, lang="eng", psm=11, tessdata_dir="...") ``` >
 *** Parameters ***
 >
 >
 *Usage of [Tesseract-OCR](https://github.com/tesseract-ocr/tesseract) requires
 prior installation. Check [documentation](https://tesseract-ocr.github.io/
-tessdoc/) for instructions.* #### PaddleOCR  *Available for Python versions <=
-3.10* PaddleOCR is an open-source OCR based on Deep Learning models.
+tessdoc/) for instructions.*
+  PaddleOCR
+*Available for Python versions <= 3.10* PaddleOCR is an open-source OCR based
+on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import PaddleOCR ocr = PaddleOCR(lang="en") ``` >
 *** Parameters ***
 >
 >
-*Released in version 0.0.13* #### Google Vision  Authentication to GCP can be
-done by setting the standard `GOOGLE_APPLICATION_CREDENTIALS` environment
-variable.
+*Released in version 0.0.13*
+  Google Vision
+Authentication to GCP can be done by setting the standard
+`GOOGLE_APPLICATION_CREDENTIALS` environment variable.
 If this variable is missing, an API key should be provided via the `api_key`
 parameter. ```python from img2table.ocr import VisionOCR ocr = VisionOCR
 (api_key="api_key", timeout=15) ``` >
 *** Parameters ***
 >
 >
-#### AWS Textract  When using AWS Textract, the DetectDocumentText API is
-exclusively called. Authentication to AWS can be done by passing credentials to
-the `TextractOCR` class.
+
+  AWS Textract
+When using AWS Textract, the DetectDocumentText API is exclusively called.
+Authentication to AWS can be done by passing credentials to the `TextractOCR`
+class.
 If credentials are not provided, authentication is done using environment
 variables or configuration files. Check `boto3` [documentation](https://
 boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) for
 more details. ```python from img2table.ocr import TextractOCR ocr = TextractOCR
 (aws_access_key_id="***", aws_secret_access_key="***", aws_session_token="***",
 region="eu-west-1") ``` >
 *** Parameters ***
 >
 >
-#### Azure Cognitive Services  ```python from img2table.ocr import AzureOCR ocr
-= AzureOCR(endpoint="abc.azure.com", subscription_key="***") ``` >
+
+  Azure Cognitive Services
+```python from img2table.ocr import AzureOCR ocr = AzureOCR
+(endpoint="abc.azure.com", subscription_key="***") ``` >
 *** Parameters ***
 >
 >
---- ### Table extraction  Multiple tables can be extracted at once from a PDF
+
+ --- ### Table extraction  Multiple tables can be extracted at once from a PDF
 page/ an image using the `extract_tables` method of a document. ```python from
 img2table.ocr import TesseractOCR from img2table.document import Image #
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
-Instantiation of document, either an image or a PDF doc = Image(src, dpi=200) #
-Table extraction extracted_tables = doc.extract_tables(ocr=ocr,
-implicit_rows=True, borderless_tables=False, min_confidence=50) ``` >
+Instantiation of document, either an image or a PDF doc = Image(src) # Table
+extraction extracted_tables = doc.extract_tables(ocr=ocr, implicit_rows=True,
+borderless_tables=False, min_confidence=50) ``` >
 *** Parameters ***
 >
 >
 *Borderless table extraction released in version 0.0.14* #### Method return The
 [`ExtractedTable`](/src/img2table/tables/objects/extraction.py#L35) class is
 used to model extracted tables from documents. >
 *** Attributes ***
@@ -129,15 +139,15 @@
 output = { 0: [ExtractedTable(...), ...], 1: [], ... last_page: [ExtractedTable
 (...), ...] } ``` ### Excel export  Tables extracted from a document can be
 exported to a xlsx file. The resulting file is composed of one worksheet per
 extracted table.
 Method arguments are mostly common with the `extract_tables` method. ```python
 from img2table.ocr import TesseractOCR from img2table.document import Image #
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
-Instantiation of document, either an image or a PDF doc = Image(src, dpi=200) #
+Instantiation of document, either an image or a PDF doc = Image(src) #
 Extraction of tables and creation of an xlsx file containing tables doc.to_xlsx
 (dest=dest, ocr=ocr, implicit_rows=True, borderless_tables=False,
 min_confidence=50) ``` >
 *** Parameters ***
 >
 >
 >
```

### Comparing `img2table-0.0.24/README.md` & `img2table-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,18 @@
 
 ## Supported file formats <a name="supported-file-formats"></a>
 
 ### Images <a name="images-formats"></a>
 
 Images are loaded using the `opencv-python` library, supported formats are listed below.
 
+<details>
+<summary>Supported image formats</summary>
+<br>
+
 <blockquote>
 <ul>
 <li>Windows bitmaps - <em>.bmp, </em>.dib</li>
 <li>JPEG files - <em>.jpeg, </em>.jpg, *.jpe</li>
 <li>JPEG 2000 files - *.jp2</li>
 <li>Portable Network Graphics - *.png</li>
 <li>WebP - *.webp</li>
@@ -76,15 +80,16 @@
 <li>TIFF files - <em>.tiff, </em>.tif</li>
 <li>OpenEXR Image files - *.exr</li>
 <li>Radiance HDR - <em>.hdr, </em>.pic</li>
 <li>Raster and Vector geospatial data supported by GDAL<br>
 <cite><a href="https://docs.opencv.org/4.x/d4/da8/group__imgcodecs.html#ga288b8b3da0892bd651fce07b3bbd3a56">OpenCV: Image file reading and writing</a></cite></li>
 </ul>
 </blockquote>
-
+</details>
+<br>
 Multi-page images are not supported.
 
 ---
 
 ### PDF <a name="pdf-formats"></a>
 
 Both native and scanned PDF files are supported.
@@ -95,61 +100,58 @@
 
 #### Images <a name="images-doc"></a>
 Images are instantiated as follows :
 ```python
 from img2table.document import Image
 
 image = Image(src, 
-              dpi=200,
               detect_rotation=False)
 ```
 
 > <h4>Parameters</h4>
 ><dl>
 >    <dt>src : str, <code>pathlib.Path</code>, bytes or <code>io.BytesIO</code>, required</dt>
 >    <dd style="font-style: italic;">Image source</dd>
->    <dt>dpi : int, optional, default <code>200</code></dt>
->    <dd style="font-style: italic;">Estimated image dpi, used to adapt OpenCV algorithm parameters</dd>
 >    <dt>detect_rotation : bool, optional, default <code>False</code></dt>
 >    <dd style="font-style: italic;">Detect and correct skew/rotation of the image</dd>
 ></dl>
-
 <br>
-
 The implemented method to handle skewed/rotated images supports skew angles up to 45° and is
 based on the publication by <a href="https://www.mdpi.com/2079-9292/9/1/55">Huang, 2020</a>.<br>
-Setting the `detect_rotation` parameter to `True`, image coordinates and bounding boxes returned by other 
+Setting the <code>detect_rotation</code> parameter to <code>True</code>, image coordinates and bounding boxes returned by other 
 methods might not correspond to the original image.
 
 #### PDF <a name="pdf-doc"></a>
 PDF files are instantiated as follows :
 ```python
 from img2table.document import PDF
 
-pdf = PDF(src, dpi=200, pages=[0, 2])
+pdf = PDF(src, pages=[0, 2])
 ```
 
 > <h4>Parameters</h4>
 ><dl>
 >    <dt>src : str, <code>pathlib.Path</code>, bytes or <code>io.BytesIO</code>, required</dt>
 >    <dd style="font-style: italic;">PDF source</dd>
->    <dt>dpi : int, optional, default <code>200</code></dt>
->    <dd style="font-style: italic;">Dpi used for conversion of PDF pages to images</dd>
 >    <dt>pages : list, optional, default <code>None</code></dt>
 >    <dd style="font-style: italic;">List of PDF page indexes to be processed. If None, all pages are processed</dd>
 ></dl>
 
+PDF pages are converted to images with a 200 DPI for table identification.
+
 ---
 
 ### OCR <a name="ocr"></a>
 
 `img2table` provides an interface for several OCR services and tools in order to parse table content.<br>
 If possible (i.e for searchable PDF), PDF text will be extracted directly from the file and the OCR service/tool will not be called.
 
-#### Tesseract <a name="tesseract"></a>
+<details>
+<summary>Tesseract<a name="tesseract"></a></summary>
+<br>
 
 ```python
 from img2table.ocr import TesseractOCR
 
 ocr = TesseractOCR(n_threads=1, 
                    lang="eng", 
                    psm=11,
@@ -167,21 +169,24 @@
 >    <dt>tessdata_dir : str, optional, default <code>None</code></dt>
 >    <dd style="font-style: italic;">Directory containing Tesseract traineddata files. If None, the <code>TESSDATA_PREFIX</code> env variable is used.</dd>
 ></dl>
 
 
 *Usage of [Tesseract-OCR](https://github.com/tesseract-ocr/tesseract) requires prior installation. 
 Check [documentation](https://tesseract-ocr.github.io/tessdoc/) for instructions.*
+<br>
+</details>
 
-
-#### <a href="https://github.com/PaddlePaddle/PaddleOCR">PaddleOCR</a> <a name="paddle"></a>
+<details>
+<summary>PaddleOCR<a name="paddle"></a></summary>
+<br>
 
 *Available for Python versions <= 3.10*
 
-PaddleOCR is an open-source OCR based on Deep Learning models.<br>
+<a href="https://github.com/PaddlePaddle/PaddleOCR">PaddleOCR</a> is an open-source OCR based on Deep Learning models.<br>
 At first use, relevant languages models will be downloaded.
 
 ```python
 from img2table.ocr import PaddleOCR
 
 ocr = PaddleOCR(lang="en")
 ```
@@ -189,16 +194,20 @@
 > <h4>Parameters</h4>
 ><dl>
 >    <dt>lang : str, optional, default <code>"en"</code></dt>
 >    <dd style="font-style: italic;">Lang parameter used in Paddle for text extraction, check <a href="https://github.com/Mushroomcat9998/PaddleOCR/blob/main/doc/doc_en/multi_languages_en.md#5-support-languages-and-abbreviations">documentation for available languages</a></dd>
 ></dl>
 
 *Released in version 0.0.13*
+<br>
+</details>
 
-#### Google Vision <a name="vision"></a>
+<details>
+<summary>Google Vision<a name="vision"></a></summary>
+<br>
 
 Authentication to GCP can be done by setting the standard `GOOGLE_APPLICATION_CREDENTIALS` environment variable.<br>
 If this variable is missing, an API key should be provided via the `api_key` parameter.
 
 ```python
 from img2table.ocr import VisionOCR
 
@@ -208,16 +217,20 @@
 > <h4>Parameters</h4>
 ><dl>
 >    <dt>api_key : str, optional, default <code>None</code></dt>
 >    <dd style="font-style: italic;">Google Vision API key</dd>
 >    <dt>timeout : int, optional, default <code>15</code></dt>
 >    <dd style="font-style: italic;">API requests timeout, in seconds</dd>
 ></dl>
+<br>
+</details>
 
-#### AWS Textract <a name="textract"></a>
+<details>
+<summary>AWS Textract<a name="textract"></a></summary>
+<br>
 
 When using AWS Textract, the DetectDocumentText API is exclusively called.
 
 Authentication to AWS can be done by passing credentials to the `TextractOCR` class.<br>
 If credentials are not provided, authentication is done using environment variables or configuration files. 
 Check `boto3` [documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) for more details.
 
@@ -237,17 +250,20 @@
 >    <dt>aws_secret_access_key : str, optional, default <code>None</code></dt>
 >    <dd style="font-style: italic;">AWS secret access key</dd>
 >    <dt>aws_session_token : str, optional, default <code>None</code></dt>
 >    <dd style="font-style: italic;">AWS temporary session token</dd>
 >    <dt>region : str, optional, default <code>None</code></dt>
 >    <dd style="font-style: italic;">AWS server region</dd>
 ></dl>
+<br>
+</details>
 
-
-#### Azure Cognitive Services <a name="azure"></a>
+<details>
+<summary>Azure Cognitive Services<a name="azure"></a></summary>
+<br>
 
 ```python
 from img2table.ocr import AzureOCR
 
 ocr = AzureOCR(endpoint="abc.azure.com",
                subscription_key="***")
 ```
@@ -255,15 +271,16 @@
 > <h4>Parameters</h4>
 ><dl>
 >    <dt>endpoint : str, optional, default <code>None</code></dt>
 >    <dd style="font-style: italic;">Azure Cognitive Services endpoint. If None, inferred from the <code>COMPUTER_VISION_ENDPOINT</code> environment variable.</dd>
 >    <dt>subscription_key : str, optional, default <code>None</code></dt>
 >    <dd style="font-style: italic;">Azure Cognitive Services subscription key. If None, inferred from the <code>COMPUTER_VISION_SUBSCRIPTION_KEY</code> environment variable.</dd>
 ></dl>
-
+<br>
+</details>
 
 ---
 
 ### Table extraction <a name="table-extract"></a>
 
 Multiple tables can be extracted at once from a PDF page/ an image using the `extract_tables` method of a document.
 
@@ -271,15 +288,15 @@
 from img2table.ocr import TesseractOCR
 from img2table.document import Image
 
 # Instantiation of OCR
 ocr = TesseractOCR(n_threads=1, lang="eng")
 
 # Instantiation of document, either an image or a PDF
-doc = Image(src, dpi=200)
+doc = Image(src)
 
 # Table extraction
 extracted_tables = doc.extract_tables(ocr=ocr,
                                       implicit_rows=True,
                                       borderless_tables=False,
                                       min_confidence=50)
 ```
@@ -342,15 +359,15 @@
 from img2table.ocr import TesseractOCR
 from img2table.document import Image
 
 # Instantiation of OCR
 ocr = TesseractOCR(n_threads=1, lang="eng")
 
 # Instantiation of document, either an image or a PDF
-doc = Image(src, dpi=200)
+doc = Image(src)
 
 # Extraction of tables and creation of an xlsx file containing tables
 doc.to_xlsx(dest=dest,
             ocr=ocr,
             implicit_rows=True,
             borderless_tables=False,
             min_confidence=50)
```

#### html2text {}

```diff
@@ -20,96 +20,106 @@
 and PDF files, including bounding boxes at the table cell level * Handling of
 complex table structures such as merged cells * Handling of implicit rows - see
 [example](/examples/Implicit_rows.ipynb) * Table content extraction by
 providing support for OCR services / tools * Extracted tables are returned as a
 simple object, including a Pandas DataFrame representation * Export extracted
 tables to an Excel file, preserving their original structure ## Supported file
 formats  ### Images  Images are loaded using the `opencv-python` library,
-supported formats are listed below.
+supported formats are listed below.  Supported image formats
          * Windows bitmaps - .bmp,.dib
          * JPEG files - .jpeg,.jpg, *.jpe
          * JPEG 2000 files - *.jp2
          * Portable Network Graphics - *.png
          * WebP - *.webp
          * Portable image format - .pbm,.pgm, .ppm.pxm, *.pnm
          * PFM files - *.pfm
          * Sun rasters - .sr,.ras
          * TIFF files - .tiff,.tif
          * OpenEXR Image files - *.exr
          * Radiance HDR - .hdr,.pic
          * Raster and Vector geospatial data supported by GDAL
            OpenCV:_Image_file_reading_and_writing
+
 Multi-page images are not supported. --- ### PDF  Both native and scanned PDF
 files are supported. ## Usage  ### Documents  #### Images  Images are
 instantiated as follows : ```python from img2table.document import Image image
-= Image(src, dpi=200, detect_rotation=False) ``` >
+= Image(src, detect_rotation=False) ``` >
 *** Parameters ***
 >
 >
 
 The implemented method to handle skewed/rotated images supports skew angles up
 to 45Â° and is based on the publication by Huang,_2020.
-Setting the `detect_rotation` parameter to `True`, image coordinates and
-bounding boxes returned by other methods might not correspond to the original
-image. #### PDF  PDF files are instantiated as follows : ```python from
-img2table.document import PDF pdf = PDF(src, dpi=200, pages=[0, 2]) ``` >
+Setting the detect_rotation parameter to True, image coordinates and bounding
+boxes returned by other methods might not correspond to the original image.
+#### PDF  PDF files are instantiated as follows : ```python from
+img2table.document import PDF pdf = PDF(src, pages=[0, 2]) ``` >
 *** Parameters ***
 >
 >
---- ### OCR  `img2table` provides an interface for several OCR services and
-tools in order to parse table content.
+PDF pages are converted to images with a 200 DPI for table identification. --
+- ### OCR  `img2table` provides an interface for several OCR services and tools
+in order to parse table content.
 If possible (i.e for searchable PDF), PDF text will be extracted directly from
-the file and the OCR service/tool will not be called. #### Tesseract  ```python
-from img2table.ocr import TesseractOCR ocr = TesseractOCR(n_threads=1,
-lang="eng", psm=11, tessdata_dir="...") ``` >
+the file and the OCR service/tool will not be called.  Tesseract
+```python from img2table.ocr import TesseractOCR ocr = TesseractOCR
+(n_threads=1, lang="eng", psm=11, tessdata_dir="...") ``` >
 *** Parameters ***
 >
 >
 *Usage of [Tesseract-OCR](https://github.com/tesseract-ocr/tesseract) requires
 prior installation. Check [documentation](https://tesseract-ocr.github.io/
-tessdoc/) for instructions.* #### PaddleOCR  *Available for Python versions <=
-3.10* PaddleOCR is an open-source OCR based on Deep Learning models.
+tessdoc/) for instructions.*
+  PaddleOCR
+*Available for Python versions <= 3.10* PaddleOCR is an open-source OCR based
+on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import PaddleOCR ocr = PaddleOCR(lang="en") ``` >
 *** Parameters ***
 >
 >
-*Released in version 0.0.13* #### Google Vision  Authentication to GCP can be
-done by setting the standard `GOOGLE_APPLICATION_CREDENTIALS` environment
-variable.
+*Released in version 0.0.13*
+  Google Vision
+Authentication to GCP can be done by setting the standard
+`GOOGLE_APPLICATION_CREDENTIALS` environment variable.
 If this variable is missing, an API key should be provided via the `api_key`
 parameter. ```python from img2table.ocr import VisionOCR ocr = VisionOCR
 (api_key="api_key", timeout=15) ``` >
 *** Parameters ***
 >
 >
-#### AWS Textract  When using AWS Textract, the DetectDocumentText API is
-exclusively called. Authentication to AWS can be done by passing credentials to
-the `TextractOCR` class.
+
+  AWS Textract
+When using AWS Textract, the DetectDocumentText API is exclusively called.
+Authentication to AWS can be done by passing credentials to the `TextractOCR`
+class.
 If credentials are not provided, authentication is done using environment
 variables or configuration files. Check `boto3` [documentation](https://
 boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) for
 more details. ```python from img2table.ocr import TextractOCR ocr = TextractOCR
 (aws_access_key_id="***", aws_secret_access_key="***", aws_session_token="***",
 region="eu-west-1") ``` >
 *** Parameters ***
 >
 >
-#### Azure Cognitive Services  ```python from img2table.ocr import AzureOCR ocr
-= AzureOCR(endpoint="abc.azure.com", subscription_key="***") ``` >
+
+  Azure Cognitive Services
+```python from img2table.ocr import AzureOCR ocr = AzureOCR
+(endpoint="abc.azure.com", subscription_key="***") ``` >
 *** Parameters ***
 >
 >
---- ### Table extraction  Multiple tables can be extracted at once from a PDF
+
+ --- ### Table extraction  Multiple tables can be extracted at once from a PDF
 page/ an image using the `extract_tables` method of a document. ```python from
 img2table.ocr import TesseractOCR from img2table.document import Image #
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
-Instantiation of document, either an image or a PDF doc = Image(src, dpi=200) #
-Table extraction extracted_tables = doc.extract_tables(ocr=ocr,
-implicit_rows=True, borderless_tables=False, min_confidence=50) ``` >
+Instantiation of document, either an image or a PDF doc = Image(src) # Table
+extraction extracted_tables = doc.extract_tables(ocr=ocr, implicit_rows=True,
+borderless_tables=False, min_confidence=50) ``` >
 *** Parameters ***
 >
 >
 *Borderless table extraction released in version 0.0.14* #### Method return The
 [`ExtractedTable`](/src/img2table/tables/objects/extraction.py#L35) class is
 used to model extracted tables from documents. >
 *** Attributes ***
@@ -125,15 +135,15 @@
 output = { 0: [ExtractedTable(...), ...], 1: [], ... last_page: [ExtractedTable
 (...), ...] } ``` ### Excel export  Tables extracted from a document can be
 exported to a xlsx file. The resulting file is composed of one worksheet per
 extracted table.
 Method arguments are mostly common with the `extract_tables` method. ```python
 from img2table.ocr import TesseractOCR from img2table.document import Image #
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
-Instantiation of document, either an image or a PDF doc = Image(src, dpi=200) #
+Instantiation of document, either an image or a PDF doc = Image(src) #
 Extraction of tables and creation of an xlsx file containing tables doc.to_xlsx
 (dest=dest, ocr=ocr, implicit_rows=True, borderless_tables=False,
 min_confidence=50) ``` >
 *** Parameters ***
 >
 >
 >
```

### Comparing `img2table-0.0.24/examples/Basic_usage.ipynb` & `img2table-0.1.0/examples/Basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/examples/Implicit_rows.ipynb` & `img2table-0.1.0/examples/Implicit_rows.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9869791666666667%*

 * *Differences: {"'cells'": "{1: {'metadata': {delete: ['collapsed']}}, insert: [(2, OrderedDict([('cell_type', "*

 * *            "'markdown'), ('id', '4ec5c901'), ('metadata', OrderedDict()), ('source', ['The "*

 * *            '<code>implicit_rows</code> parameter is used to split existing rows into smaller ones '*

 * *            "if:\\n', '1. The row contains multi-line cells\\n', '2. Vertical separation between "*

 * *            "elements of the cell is large enough'])]))]}"}*

```diff
@@ -9,15 +9,14 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "eb649b04",
             "metadata": {
-                "collapsed": true,
                 "execution": {
                     "iopub.execute_input": "2023-03-28T20:35:06.576337Z",
                     "iopub.status.busy": "2023-03-28T20:35:06.576337Z",
                     "iopub.status.idle": "2023-03-28T20:35:09.448694Z",
                     "shell.execute_reply": "2023-03-28T20:35:09.448694Z"
                 }
             },
@@ -38,14 +37,24 @@
                 "\n",
                 "from img2table.document import Image\n",
                 "from img2table.ocr import TesseractOCR"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "4ec5c901",
+            "metadata": {},
+            "source": [
+                "The <code>implicit_rows</code> parameter is used to split existing rows into smaller ones if:\n",
+                "1. The row contains multi-line cells\n",
+                "2. Vertical separation between elements of the cell is large enough"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "21336bb3",
             "metadata": {},
             "source": [
                 "### Image used for the example"
             ]
         },
         {
```

### Comparing `img2table-0.0.24/examples/borderless.ipynb` & `img2table-0.1.0/examples/borderless.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988839285714286%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'An algorithm for identification and extraction of "*

 * *            'borderless tables (i.e not fully bordered). However, the detection might not be as '*

 * *            'reliable as the one for bordered tables, especially for tables with multi-line '*

 * *            "cells.')], delete: [2]}}}"}*

```diff
@@ -43,15 +43,15 @@
         {
             "cell_type": "markdown",
             "id": "7030a68c",
             "metadata": {},
             "source": [
                 "### Borderless table extraction\n",
                 "\n",
-                "In order to extract borderless tables, an OCR should be provided to the <code>extract_tables</code> method as the algorithm relies on OCR results for table identification. If no OCR is provided, borderless table extraction will not be performed."
+                "An algorithm for identification and extraction of borderless tables (i.e not fully bordered). However, the detection might not be as reliable as the one for bordered tables, especially for tables with multi-line cells."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d13d2df0",
             "metadata": {},
             "source": [
```

### Comparing `img2table-0.0.24/examples/data/borderless_aws.jpg` & `img2table-0.1.0/examples/data/borderless_aws.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/examples/data/borderless_ocr.jpg` & `img2table-0.1.0/examples/data/borderless_ocr.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/examples/data/implicit.png` & `img2table-0.1.0/examples/data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/examples/data/tables.pdf` & `img2table-0.1.0/examples/data/tables.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/examples/data/tables.png` & `img2table-0.1.0/examples/data/tables.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/examples/data/tables.xlsx` & `img2table-0.1.0/examples/data/tables.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/setup.cfg` & `img2table-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/__init__.py` & `img2table-0.1.0/src/img2table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/document/base/__init__.py` & `img2table-0.1.0/src/img2table/document/base/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # coding: utf-8
 import io
 from dataclasses import dataclass
+try:
+    from functools import cached_property
+except ImportError:
+    from cached_property import cached_property
 from pathlib import Path
 from typing import Union, Iterator, Dict, List, Optional
 
 import numpy as np
 import xlsxwriter
 
 from img2table import Validations
 from img2table.tables.objects.extraction import ExtractedTable
 
 
 @dataclass
 class Document(Validations):
     src: Union[str, Path, io.BytesIO, bytes]
-    dpi: int = 200
 
     def validate_src(self, value, **_) -> Union[str, Path, io.BytesIO, bytes]:
         if not isinstance(value, (str, Path, io.BytesIO, bytes)):
             raise TypeError(f"Invalid type {type(value)} for src argument")
         return value
 
     def validate_dpi(self, value, **_) -> int:
@@ -30,15 +33,15 @@
         super(Document, self).__post_init__()
         # Initialize ocr_df
         self.ocr_df = None
 
         if isinstance(self.pages, list):
             self.pages = sorted(self.pages)
 
-    @property
+    @cached_property
     def bytes(self) -> bytes:
         if isinstance(self.src, bytes):
             return self.src
         elif isinstance(self.src, io.BytesIO):
             self.src.seek(0)
             return self.src.read()
         elif isinstance(self.src, str):
@@ -62,15 +65,14 @@
         # If possible, apply ocr to document
         if self.ocr_df is None and ocr is not None:
             self.ocr_df = ocr.of(document=self)
 
         # Extract tables from document
         from img2table.tables.image import TableImage
         tables = {idx: TableImage(img=img,
-                                  dpi=self.dpi,
                                   ocr_df=self.ocr_df.page(page_number=idx) if self.ocr_df else None,
                                   min_confidence=min_confidence).extract_tables(implicit_rows=implicit_rows,
                                                                                 borderless_tables=borderless_tables)
                   for idx, img in enumerate(self.images)}
 
         # If pages have been defined, modify tables keys
         if self.pages:
```

### Comparing `img2table-0.0.24/src/img2table/document/image.py` & `img2table-0.1.0/src/img2table/document/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # coding: utf-8
 from dataclasses import dataclass
-from typing import Iterator, List
+try:
+    from functools import cached_property
+except ImportError:
+    from cached_property import cached_property
+from typing import List
 
 import cv2
 import numpy as np
 
 from img2table.document.base import Document
 from img2table.document.base.rotation import fix_rotation_image
 from img2table.tables.objects.extraction import ExtractedTable
@@ -20,18 +24,18 @@
         return value
 
     def __post_init__(self):
         self.pages = None
 
         super(Image, self).__post_init__()
 
-    @property
-    def images(self) -> Iterator[np.ndarray]:
+    @cached_property
+    def images(self) -> List[np.ndarray]:
         img = cv2.imdecode(np.frombuffer(self.bytes, np.uint8), cv2.IMREAD_GRAYSCALE)
-        yield fix_rotation_image(img=img) if self.detect_rotation else img
+        return [fix_rotation_image(img=img) if self.detect_rotation else img]
 
     def extract_tables(self, ocr: "OCRInstance" = None, implicit_rows: bool = True, borderless_tables: bool = False,
                        min_confidence: int = 50) -> List[ExtractedTable]:
         """
         Extract tables from document
         :param ocr: OCRInstance object used to extract table content
         :param implicit_rows: boolean indicating if implicit rows are splitted
```

### Comparing `img2table-0.0.24/src/img2table/document/pdf.py` & `img2table-0.1.0/src/img2table/document/pdf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 # coding: utf-8
 from dataclasses import dataclass
+try:
+    from functools import cached_property
+except ImportError:
+    from cached_property import cached_property
 from typing import Dict, List, Optional
 
 import cv2
 import fitz
 import numpy as np
 
 from img2table.document.base import Document
 from img2table.ocr.pdf import PdfOCR
 from img2table.tables.objects.extraction import ExtractedTable
 
 
 @dataclass
 class PDF(Document):
     pages: List[int] = None
-    _images: List[np.ndarray] = None
 
     def validate_pages(self, value, **_) -> Optional[List[int]]:
         if value is not None:
             if not isinstance(value, list):
                 raise TypeError(f"Invalid type {type(value)} for pages argument")
             if not all(isinstance(x, int) for x in value):
                 raise TypeError("All values in pages argument should be integers")
         return value
 
     def validate__images(self, value, **_) -> Optional[List[int]]:
         return value
 
-    @property
+    @cached_property
     def images(self) -> List[np.ndarray]:
-        if self._images is not None:
-            return self._images
-
-        mat = fitz.Matrix(self.dpi / 72, self.dpi / 72)
+        mat = fitz.Matrix(200 / 72, 200 / 72)
         doc = fitz.Document(stream=self.bytes, filetype='pdf')
 
         # Get all images
         images = list()
         for page_number in self.pages or range(doc.page_count):
             page = doc.load_page(page_id=page_number)
             pix = page.get_pixmap(matrix=mat)
             img = np.frombuffer(buffer=pix.samples, dtype=np.uint8).reshape((pix.height, pix.width, 3))
             images.append(cv2.cvtColor(img, cv2.COLOR_BGR2GRAY))
 
-        # Set _images variable
-        self._images = images
         return images
 
     def extract_tables(self, ocr: "OCRInstance" = None, implicit_rows: bool = True, borderless_tables: bool = False,
                        min_confidence: int = 50) -> Dict[int, List[ExtractedTable]]:
         """
         Extract tables from document
         :param ocr: OCRInstance object used to extract table content
```

### Comparing `img2table-0.0.24/src/img2table/ocr/aws_textract.py` & `img2table-0.1.0/src/img2table/ocr/aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/ocr/azure.py` & `img2table-0.1.0/src/img2table/ocr/azure.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/ocr/base.py` & `img2table-0.1.0/src/img2table/ocr/base.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/ocr/data.py` & `img2table-0.1.0/src/img2table/ocr/data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # coding: utf-8
 from dataclasses import dataclass
+try:
+    from functools import cached_property
+except ImportError:
+    from cached_property import cached_property
 
 import polars as pl
 
 from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.table import Table
 
 
@@ -12,76 +16,14 @@
     df: pl.LazyFrame
 
     def page(self, page_number: int = 0) -> "OCRDataframe":
         # Filter dataframe on specific page
         df_page = self.df.filter(pl.col('page') == page_number)
         return OCRDataframe(df=df_page)
 
-    @property
-    def median_line_sep(self) -> float:
-        """
-        Get median of vertical line separation in pixels
-        :return: median of vertical line separation in pixels
-        """
-        # Get only words
-        df_words = self.df.filter(pl.col('class') == "ocrx_word")
-
-        # Check if there are some words
-        if df_words.collect().height <= 1:
-            return None
-
-        # Cross join to get corresponding words and filter on words that corresponds horizontally
-        df_h_words = (df_words.join(df_words, how='cross')
-                      .filter(pl.col('id') != pl.col('id_right'))
-                      .filter(pl.min([pl.col('x2'), pl.col('x2_right')])
-                              - pl.max([pl.col('x1'), pl.col('x1_right')]) > 0)
-                      )
-
-        # Get word which is directly below
-        df_words_below = (df_h_words.filter(pl.col('y1') < pl.col('y1_right'))
-                          .sort(['id', 'y1_right'])
-                          .with_columns(pl.lit(1).alias('ones'))
-                          .with_columns(pl.col('ones').cumsum().over(["id"]).alias('rk'))
-                          .filter(pl.col('rk') == 1)
-                          )
-
-        # Check if there are some correspondence
-        if df_words_below.collect().height <= 1:
-            return None
-
-        # Compute median vertical distance between words
-        median_v_dist = (df_words_below.with_columns(((pl.col('y1_right') + pl.col('y2_right')
-                                                       - pl.col('y1') - pl.col('y2')) / 2).alias('y_diff'))
-                         .select(pl.median('y_diff'))
-                         .collect()
-                         .to_dicts()
-                         .pop()
-                         .get('y_diff')
-                         )
-
-        return median_v_dist
-
-    @property
-    def char_length(self) -> float:
-        """
-        Get average character length in pixels
-        :return: average character length in pixels
-        """
-        try:
-            # Compute average text size
-            df_text_size = (self.df.filter(pl.col('value').is_not_null())
-                            .with_columns([pl.col('value').str.lengths().alias('str_length'),
-                                           (pl.col('x2') - pl.col('x1')).alias('width')])
-                            .select((pl.sum('width') / pl.sum('str_length')).alias('char_length'))
-                            )
-
-            return df_text_size.collect().to_dicts().pop().get('char_length')
-        except Exception:
-            return None
-
     def get_text_cell(self, cell: Cell, margin: int = 0, page_number: int = None, min_confidence: int = 50) -> str:
         """
         Get text corresponding to cell
         :param cell: Cell object in document
         :param margin: margin to take around cell
         :param page_number: page number of the cell
         :param min_confidence: minimum confidence in order to include a word, from 0 (worst) to 99 (best)
@@ -134,15 +76,15 @@
                                 pl.col('y2').max(),
                                 pl.col('value').alias('value')])
                           .sort([pl.col("y1"), pl.col("x1")])
                           )
 
         # Concatenate all lines
         text_lines = (df_text_parent.select(pl.col('value'))
-                      .collect()
+                      .collect(streaming=True)
                       .get_column('value')
                       .to_list()
                       )
 
         return "\n".join([" ".join(line).strip() for line in text_lines]).strip() or None
 
     def get_text_table(self, table: Table, page_number: int = None, min_confidence: int = 50) -> Table:
@@ -201,20 +143,20 @@
                                 pl.col('value').apply(lambda x: ' '.join(x), return_dtype=str).alias('value')])
                           .sort([pl.col("row"), pl.col("col"), pl.col('y1'), pl.col('x1')])
                           .groupby(['row', 'col'])
                           .agg(pl.col('value').apply(lambda x: '\n'.join(x).strip(), return_dtype=str).alias('text'))
                           )
 
         # Implement found values to table cells content
-        for rec in df_text_parent.collect().to_dicts():
+        for rec in df_text_parent.collect(streaming=True).to_dicts():
             table.items[rec.get('row')].items[rec.get('col')].content = rec.get('text') or None
 
         return table
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             try:
-                assert self.df.collect().frame_equal(other.df.collect())
+                assert self.df.collect(streaming=True).frame_equal(other.df.collect(streaming=True))
                 return True
             except AssertionError:
                 return False
         return False
```

### Comparing `img2table-0.0.24/src/img2table/ocr/google_vision.py` & `img2table-0.1.0/src/img2table/ocr/google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/ocr/paddle.py` & `img2table-0.1.0/src/img2table/ocr/paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/ocr/pdf.py` & `img2table-0.1.0/src/img2table/ocr/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/ocr/tesseract.py` & `img2table-0.1.0/src/img2table/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/tables/image.py` & `img2table-0.1.0/src/img2table/tables/image.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 # coding: utf-8
 import copy
 from dataclasses import dataclass
+
+from img2table.tables.metrics import compute_img_metrics
+from img2table.tables.objects.cell import Cell
+
+try:
+    from functools import cached_property
+except ImportError:
+    from cached_property import cached_property
 from typing import List
 
 import cv2
 import numpy as np
 
 from img2table.tables.objects.extraction import ExtractedTable
 from img2table.tables.objects.line import Line
@@ -17,91 +25,122 @@
 from img2table.tables.processing.prepare_image import prepare_image
 from img2table.tables.processing.text.titles import get_title_tables
 
 
 @dataclass
 class TableImage:
     img: np.ndarray
-    dpi: int
+    dpi: int = 200
     ocr_df: "OCRDataframe" = None
     min_confidence: int = 50
+    char_length: float = None
+    median_line_sep: float = None
+    contours: List[Cell] = None
     lines: List[Line] = None
     tables: List[Table] = None
 
     def __post_init__(self):
         # Prepare image by removing eventual black background
         self.img = prepare_image(img=self.img)
 
-    @property
+        # Compute image metrics
+        self.char_length, self.median_line_sep, self.contours = compute_img_metrics(img=self.img)
+
+    @cached_property
     def white_img(self) -> np.ndarray:
         white_img = copy.deepcopy(self.img)
 
         # Draw white lines on detected lines
-        for line in self.lines:
-            cv2.rectangle(white_img, (line.x1, line.y1), (line.x2, line.y2), (255, 255, 255), 3)
+        for l in self.lines:
+            if l.horizontal:
+                cv2.rectangle(white_img, (l.x1 - l.thickness, l.y1), (l.x2 + l.thickness, l.y2), (255, 255, 255),
+                              3 * l.thickness)
+            elif l.vertical:
+                cv2.rectangle(white_img, (l.x1, l.y1 - l.thickness), (l.x2, l.y2 + l.thickness), (255, 255, 255),
+                              2 * l.thickness)
 
         return white_img
 
-    def extract_tables(self, implicit_rows: bool = True, borderless_tables: bool = False) -> List[ExtractedTable]:
+    def extract_bordered_tables(self, implicit_rows: bool = True):
         """
-        Identify and extract tables from image
+        Identify and extract bordered tables from image
         :param implicit_rows: boolean indicating if implicit rows are splitted
-        :param borderless_tables: boolean indicating if borderless tables should be detected
-        :return: list of identified tables
+        :return:
         """
-        # If an OCR is provided, compute parameters base on it
-        if self.ocr_df is not None:
-            minLinLength = maxLineGap = round(0.33 * self.ocr_df.median_line_sep) if self.ocr_df.median_line_sep is not None else self.dpi // 20
-            kernel_size = round(0.66 * self.ocr_df.median_line_sep) if self.ocr_df.median_line_sep is not None else self.dpi // 10
-        else:
-            minLinLength = maxLineGap = self.dpi // 20
-            kernel_size = self.dpi // 10
+        # Compute parameters for line detection
+        minLinLength = maxLineGap = round(0.33 * self.median_line_sep) if self.median_line_sep else self.dpi // 20
+        kernel_size = round(0.66 * self.median_line_sep) if self.median_line_sep else self.dpi // 10
 
         # Detect lines in image
         h_lines, v_lines = detect_lines(image=self.img,
+                                        contours=self.contours,
+                                        char_length=self.char_length,
                                         rho=0.3,
                                         theta=np.pi / 180,
                                         threshold=10,
                                         minLinLength=minLinLength,
                                         maxLineGap=maxLineGap,
-                                        kernel_size=kernel_size,
-                                        ocr_df=self.ocr_df)
+                                        kernel_size=kernel_size)
         self.lines = h_lines + v_lines
 
         # Create cells from lines
         cells = get_cells(horizontal_lines=h_lines,
                           vertical_lines=v_lines)
 
         # Create tables from lines
         self.tables = get_tables(cells=cells)
 
         # If necessary, detect implicit rows
         if implicit_rows:
             self.tables = handle_implicit_rows(img=self.white_img,
-                                               tables=self.tables,
-                                               ocr_df=self.ocr_df)
+                                               tables=self.tables)
 
-        # If ocr_df is available, get titles and tables content
+        # If ocr_df is available, get tables content
         if self.ocr_df is not None:
             # Get content
             self.tables = [table.get_content(ocr_df=self.ocr_df, min_confidence=self.min_confidence)
                            for table in self.tables]
-            self.tables = [table for table in self.tables if table.nb_rows * table.nb_columns > 1]
 
-            if borderless_tables:
-                # Extract borderless tables
-                borderless_tbs = identify_borderless_tables(img=self.img,
-                                                            ocr_df=self.ocr_df,
-                                                            lines=self.lines,
-                                                            existing_tables=self.tables)
+        self.tables = [table for table in self.tables if table.nb_rows * table.nb_columns > 1]
+
+    def extract_borderless_tables(self):
+        """
+        Identify and extract borderless tables from image
+        :return:
+        """
+        # Median line separation needs to be not null to extract borderless tables
+        if self.median_line_sep is not None:
+            # Extract borderless tables
+            borderless_tbs = identify_borderless_tables(img=self.img,
+                                                        char_length=self.char_length,
+                                                        median_line_sep=self.median_line_sep,
+                                                        lines=self.lines,
+                                                        existing_tables=self.tables)
 
+            # If ocr_df is available, get tables content
+            if self.ocr_df is not None:
                 # Get content
                 borderless_tbs = [table.get_content(ocr_df=self.ocr_df, min_confidence=self.min_confidence)
                                   for table in borderless_tbs]
 
-                # Add to tables
-                self.tables += [tb for tb in borderless_tbs if min(tb.nb_rows, tb.nb_columns) >= 2]
+            # Add to tables
+            self.tables += [tb for tb in borderless_tbs if min(tb.nb_rows, tb.nb_columns) >= 2]
 
-            # Get title
+    def extract_tables(self, implicit_rows: bool = True, borderless_tables: bool = False) -> List[ExtractedTable]:
+        """
+        Identify and extract tables from image
+        :param implicit_rows: boolean indicating if implicit rows are splitted
+        :param borderless_tables: boolean indicating if borderless tables should be detected
+        :return: list of identified tables
+        """
+        # Extract bordered tables
+        self.extract_bordered_tables(implicit_rows=implicit_rows)
+
+        if borderless_tables:
+            # Extract borderless tables
+            self.extract_borderless_tables()
+
+        # If ocr_df is available, get tables titles
+        if self.ocr_df is not None:
             self.tables = get_title_tables(img=self.img, tables=self.tables, ocr_df=self.ocr_df)
 
         return [table.extracted_table for table in self.tables]
```

### Comparing `img2table-0.0.24/src/img2table/tables/objects/__init__.py` & `img2table-0.1.0/src/img2table/tables/objects/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 # coding: utf-8
+try:
+    from functools import cached_property
+except ImportError:
+    from cached_property import cached_property
+
 
 class TableObject:
     def bbox(self, margin: int = 0, height_margin: int = 0, width_margin: int = 0) -> tuple:
         """
         Return bounding box corresponding to the object
         :param margin: general margin used for the bounding box
         :param height_margin: vertical margin used for the bounding box
@@ -19,18 +24,18 @@
             bbox = (self.x1 - width_margin,
                     self.y1 - height_margin,
                     self.x2 + width_margin,
                     self.y2 + height_margin)
 
         return bbox
 
-    @property
+    @cached_property
     def height(self) -> int:
         return self.y2 - self.y1
 
-    @property
+    @cached_property
     def width(self) -> int:
         return self.x2 - self.x1
 
-    @property
+    @cached_property
     def area(self) -> int:
         return self.height * self.width
```

### Comparing `img2table-0.0.24/src/img2table/tables/objects/extraction.py` & `img2table-0.1.0/src/img2table/tables/objects/extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/tables/objects/line.py` & `img2table-0.1.0/src/img2table/tables/objects/line.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/tables/objects/row.py` & `img2table-0.1.0/src/img2table/tables/objects/row.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,14 @@
         self._contours = []
 
     @property
     def items(self) -> List[Cell]:
         return self._items
 
     @property
-    def contours(self) -> List[Cell]:
-        return self._contours
-
-    @property
     def nb_columns(self) -> int:
         return len(self.items)
 
     @property
     def x1(self) -> int:
         return min(map(lambda x: x.x1, self.items))
```

### Comparing `img2table-0.0.24/src/img2table/tables/objects/table.py` & `img2table-0.1.0/src/img2table/tables/objects/table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/cells/__init__.py` & `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/cells/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     :return: list of all cells in image
     """
     # Create dataframe with cells from horizontal and vertical lines
     df_cells = get_cells_dataframe(horizontal_lines=horizontal_lines,
                                    vertical_lines=vertical_lines)
     
     # Handle case of empty cells
-    if df_cells.collect().height == 0:
+    if df_cells.collect(streaming=True).height == 0:
         return []
 
     # Deduplicate cells
     df_cells_dedup = deduplicate_cells(df_cells=df_cells)
 
     # Convert to Cell objects
     cells = [Cell(x1=row["x1"], x2=row["x2"], y1=row["y1"], y2=row["y2"])
-             for row in df_cells_dedup.collect().to_dicts()]
+             for row in df_cells_dedup.collect(streaming=True).to_dicts()]
 
     return cells
```

### Comparing `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/cells/deduplication.py` & `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/cells/deduplication.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                           )
     df_cross_cells = (df_cross_cells.with_columns(condition_adjacent.alias('adjacent'))
                       .with_columns((pl.col('contained') & pl.col('adjacent')).alias('redundant'))
                       )
 
     # Get list of redundant cells and remove them from original cell dataframe
     redundant_cells = (df_cross_cells.filter(pl.col('redundant'))
-                       .collect()
+                       .collect(streaming=True)
                        .get_column('index_')
                        .unique()
                        .to_list()
                        )
     df_final_cells = (df_cells.with_row_count(name="cnt")
                       .filter(~pl.col('cnt').is_in(redundant_cells))
                       .drop('cnt')
```

### Comparing `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/cells/identification.py` & `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/cells/identification.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/lines.py` & `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/lines.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 # coding: utf-8
-from typing import List
+from typing import List, Optional
 
 import cv2
 import numpy as np
 import polars as pl
 
-from img2table.ocr.data import OCRDataframe
+from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.line import Line
 
 
-def threshold_dark_areas(img: np.ndarray, ocr_df: OCRDataframe) -> np.ndarray:
+def threshold_dark_areas(img: np.ndarray, char_length: Optional[float]) -> np.ndarray:
     """
     Threshold image by differentiating areas with light and dark backgrounds
     :param img: image array
-    :param ocr_df: OCRDataframe object
+    :param char_length: average character length
     :return: threshold image
     """
     # Get threshold on image and binary image
     blur = cv2.GaussianBlur(img, (3, 3), 0)
     thresh = cv2.adaptiveThreshold(blur, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, 21, 10)
     binary_thresh = cv2.adaptiveThreshold(255 - blur, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, 21, 10)
 
     # Mask on areas with dark background
-    try:
-        blur_size = int(2 * ocr_df.char_length) + 1 - int(2 * ocr_df.char_length) % 2 if ocr_df.char_length else 11
-    except Exception as e:
-        blur_size = 11
+    blur_size = int(2 * char_length) + 1 - int(2 * char_length) % 2 if char_length else 11
     blur = cv2.medianBlur(img, blur_size)
     mask = cv2.inRange(blur, 0, 100)
 
     # Get contours of dark areas
     contours, _ = cv2.findContours(mask, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
 
     # For each dark area, use binary threshold instead of regular threshold
     for c in contours:
         x, y, w, h = cv2.boundingRect(c)
-        
-        try:
-            margin = int(ocr_df.char_length)
-        except Exception as e:
-            margin = 5
+
+        margin = int(char_length)
         if min(w, h) > 2 * margin and w * h / np.prod(img.shape[:2]) < 0.9:
             thresh[y+margin:y+h-margin, x+margin:x+w-margin] = binary_thresh[y+margin:y+h-margin, x+margin:x+w-margin]
 
     return thresh
 
 
 def overlapping_filter(lines: List[Line], max_gap: int = 5) -> List[Line]:
@@ -113,43 +107,41 @@
     # If not horizontal, transpose all lines
     if not horizontal:
         final_lines = [line.transpose for line in final_lines]
 
     return final_lines
 
 
-def remove_word_lines(lines: List[Line], ocr_df: OCRDataframe) -> List[Line]:
+def remove_word_lines(lines: List[Line], contours: List[Cell]) -> List[Line]:
     """
-    Remove lines that corresponds to words in image
+    Remove lines that corresponds to contours in image
     :param lines: list of lines
-    :param ocr_df: OCRDataframe object
+    :param contours: list of image contours as cell objects
     :return: list of lines not intersecting with words
     """
-    # Get words from dataframe
-    df_words = (ocr_df.df.filter(pl.col('class') == "ocrx_word")
-                .filter(pl.col('confidence') >= 50)
-                )
+    # Get contours dataframe
+    df_cnts = pl.LazyFrame(data=[{"x1": c.x1, "y1": c.y1, "x2": c.x2, "y2": c.y2} for c in contours])
 
-    # If there are no lines or no words, do nothing
-    if len(lines) == 0 or df_words.collect().height == 0:
+    # If there are no lines or no contours, do nothing
+    if len(lines) == 0 or df_cnts.collect(streaming=True).height == 0:
         return lines
 
     # Create dataframe containing lines
     df_lines = (pl.LazyFrame(data=[line.dict for line in lines])
                 .with_columns([pl.max([pl.col('width'), pl.col('height')]).alias('length'),
                                (pl.col('x1') == pl.col('x2')).alias('vertical')]
                               )
                 .with_row_count(name="line_id")
                 .rename({"x1": "x1_line", "x2": "x2_line", "y1": "y1_line", "y2": "y2_line"})
                 )
 
     # Merge both dataframes
-    df_words_lines = df_words.join(df_lines, how='cross')
+    df_words_lines = df_cnts.join(df_lines, how='cross')
 
-    # Compute intersection between words bbox and lines
+    # Compute intersection between contours bbox and lines
     # - vertical case
     vert_int = (
         (((pl.col('x1') + pl.col('x2')) / 2 - pl.col('x1_line')).abs() / (pl.col('x2') - pl.col('x1')) < 0.45)
         * pl.max([(pl.min([pl.col('y2'), pl.col('y2_line')]) - pl.max([pl.col('y1'), pl.col('y1_line')])), pl.lit(0)])
     )
     # - horizontal case
     hor_int = (
@@ -161,44 +153,45 @@
                                                  )
 
     # Compute total intersection for each line
     df_inter = (df_words_lines.groupby(['line_id', 'length'])
                 .agg(pl.col('intersection').sum().alias('intersection'))
                 )
 
-    # Identify lines that intersect words
+    # Identify lines that intersect contours
     intersecting_lines = (df_inter.filter(pl.col('intersection') / pl.col('length') > 0.5)
-                          .collect()
+                          .collect(streaming=True)
                           .get_column('line_id')
                           .to_list()
                           )
 
     return [line for idx, line in enumerate(lines) if idx not in intersecting_lines]
 
 
-def detect_lines(image: np.ndarray, rho: float = 1, theta: float = np.pi / 180, threshold: int = 50,
-                 minLinLength: int = 290, maxLineGap: int = 6, kernel_size: int = 20,
-                 ocr_df: OCRDataframe = None) -> (List[Line], List[Line]):
+def detect_lines(image: np.ndarray, contours: Optional[List[Cell]], char_length: Optional[float], rho: float = 1,
+                 theta: float = np.pi / 180, threshold: int = 50, minLinLength: int = 290, maxLineGap: int = 6,
+                 kernel_size: int = 20) -> (List[Line], List[Line]):
     """
     Detect horizontal and vertical lines on image
     :param image: image array
+    :param contours: list of image contours as cell objects
+    :param char_length: average character length
     :param rho: rho parameter for Hough line transform
     :param theta: theta parameter for Hough line transform
     :param threshold: threshold parameter for Hough line transform
     :param minLinLength: minLinLength parameter for Hough line transform
     :param maxLineGap: maxLineGap parameter for Hough line transform
     :param kernel_size: kernel size to filter on horizontal / vertical lines
-    :param ocr_df: OCRDataframe object
     :return: horizontal and vertical lines
     """
     # Create copy of image
     img = image.copy()
 
     # Apply thresholding
-    thresh = threshold_dark_areas(img=img, ocr_df=ocr_df)
+    thresh = threshold_dark_areas(img=img, char_length=char_length)
 
     # Identify both vertical and horizontal lines
     for kernel_tup, gap in [((kernel_size, 1), 2 * maxLineGap), ((1, kernel_size), maxLineGap)]:
         # Apply masking on image
         kernel = cv2.getStructuringElement(cv2.MORPH_RECT, kernel_tup)
         mask = cv2.morphologyEx(thresh, cv2.MORPH_OPEN, kernel, iterations=1)
 
@@ -215,11 +208,11 @@
         # Remove lines that are not horizontal or vertical
         lines = [line for line in lines if line.horizontal or line.vertical]
 
         # Merge lines
         merged_lines = overlapping_filter(lines=lines, max_gap=gap)
 
         # If possible, remove lines that corresponds to words
-        if ocr_df is not None:
-            merged_lines = remove_word_lines(lines=merged_lines, ocr_df=ocr_df)
+        if contours is not None:
+            merged_lines = remove_word_lines(lines=merged_lines, contours=contours)
 
         yield merged_lines
```

### Comparing `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/__init__.py` & `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py` & `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/tables/processing/bordered_tables/tables/table_creation.py` & `img2table-0.1.0/src/img2table/tables/processing/bordered_tables/tables/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/__init__.py` & `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # coding: utf-8
 from typing import List
 
 import numpy as np
 
-from img2table.ocr.data import OCRDataframe
 from img2table.tables.objects.line import Line
 from img2table.tables.objects.table import Table
 from img2table.tables.processing.borderless_tables.column_delimiters import get_whitespace_column_delimiters
 from img2table.tables.processing.borderless_tables.lines import identify_line_groups
 from img2table.tables.processing.borderless_tables.segment_image import segment_image
 from img2table.tables.processing.borderless_tables.table import identify_table
 from img2table.tables.processing.common import is_contained_cell
@@ -30,27 +29,38 @@
                         is_contained_cell(inner_cell=tb.cell, outer_cell=table.cell, percentage=0.1))
                     for tb in existing_tables + final_tables]):
             final_tables.append(table)
 
     return final_tables
 
 
-def identify_borderless_tables(img: np.ndarray, lines: List[Line], ocr_df: OCRDataframe,
+def identify_borderless_tables(img: np.ndarray, lines: List[Line], char_length: float, median_line_sep: float,
                                existing_tables: List[Table]) -> List[Table]:
+    """
+    Identify borderless tables in image
+    :param img: image array
+    :param lines: list of lines detected in image
+    :param char_length: average character length
+    :param median_line_sep: median line separation
+    :param existing_tables: list of detected bordered tables
+    :return: list of detected borderless tables
+    """
     # Segment image
     img_segments = segment_image(img=img,
                                  lines=lines,
-                                 ocr_df=ocr_df)
+                                 char_length=char_length,
+                                 median_line_sep=median_line_sep)
 
     # In each segment, create groups of lines and identify tables
     tables = list()
     for seg in img_segments:
         # Identify line groups in segment
         seg_line_groups = identify_line_groups(segment=seg,
-                                               ocr_df=ocr_df)
+                                               char_length=char_length,
+                                               median_line_sep=median_line_sep)
 
         # For each line group, identify column delimiters and create tables
         for line_gp in seg_line_groups.line_groups:
             # Get column delimiters
             col_delimiters = get_whitespace_column_delimiters(line_group=line_gp,
                                                               segment_elements=seg_line_groups.elements)
```

### Comparing `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/column_delimiters.py` & `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/column_delimiters.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,14 @@
     y2: int
 
     @classmethod
     def from_cell(cls, cell: Cell) -> "Rectangle":
         return cls(x1=cell.x1, y1=cell.y1, x2=cell.x2, y2=cell.y2)
 
     @property
-    def height(self):
-        return self.y2 - self.y1
-
-    @property
-    def width(self):
-        return self.x2 - self.x1
-
-    @property
     def area(self):
         return (self.x2 - self.x1) * (self.y2 - self.y1)
 
     @property
     def center(self):
         return (self.x1 + self.x2) / 2, (self.y1 + self.y2) / 2
 
@@ -43,18 +35,15 @@
 
     def overlaps(self, other):
         x_left = max(self.x1, other.x1)
         y_top = max(self.y1, other.y1)
         x_right = min(self.x2, other.x2)
         y_bottom = min(self.y2, other.y2)
 
-        if x_right < x_left or y_bottom < y_top:
-            return False
-
-        return (x_right - x_left) * (y_bottom - y_top) > 0
+        return max(x_right - x_left, 0) * max(y_bottom - y_top, 0) > 0
 
 
 def identify_trivial_delimiters(line_group: LineGroup, elements: List[Cell]) -> List[Cell]:
     """
     Get trivial whitespace delimiters spanning the entire line group height
     :param line_group: cluster of lines
     :param elements: Cell elements from image
@@ -88,24 +77,20 @@
     group_rect = Rectangle(x1=line_group.x1, y1=line_group.y1, x2=line_group.x2, y2=line_group.y2)
     obstacles = [Rectangle.from_cell(cell=element) for element in elements]
 
     # Initiate queue
     queue = PriorityQueue()
     queue.put([-group_rect.area, group_rect, obstacles])
 
-    # Get covered area
-    covered_area = sum([o.area for o in obstacles])
-
     whitespaces = list()
     while not queue.qsize() == 0:
         q, r, obs = queue.get()
         if len(obs) == 0:
             # Update whitespaces and covered area
             whitespaces.append(r)
-            covered_area += r.area
 
             # Update elements in queue
             for element in queue.queue:
                 if element[1].overlaps(r):
                     element[2] += [r]
 
             continue
```

### Comparing `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/lines.py` & `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/lines.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # coding: utf-8
 from typing import List
 
-from img2table.ocr.data import OCRDataframe
 from img2table.tables.objects.cell import Cell
 from img2table.tables.processing.borderless_tables.model import TableLine, LineGroup, ImageSegment
 
 
 def identify_lines(elements: List[Cell], ref_size: int) -> List[TableLine]:
     """
     Identify lines from Cell elements
@@ -101,55 +100,56 @@
 
         # Add groups to line groups
         line_groups += [gp for gp in gps if max([len(line.cells) for line in gp.lines]) > 1]
 
     return line_groups
 
 
-def is_text_block(line_group: LineGroup, ocr_df: OCRDataframe) -> bool:
+def is_text_block(line_group: LineGroup, char_length: float) -> bool:
     """
     Check if the line group corresponds to a text block
     :param line_group: LineGroup object
-    :param ocr_df: OCRDataframe object
+    :param char_length: average character length
     :return: boolean indicating if the line group is a text block
     """
     # Get list of lines and if they are complete text
     nb_lines_text = 0
 
     for line in line_group.lines:
         text_line = True
         # Check difference in pixels between each element of the line
         cells = sorted(line.cells, key=lambda c: (c.x1, c.x2))
 
         for prev, nextt in zip(cells, cells[1:]):
             x_diff = nextt.x1 - prev.x2
-            if x_diff >= 2 * ocr_df.char_length:
+            if x_diff >= 2 * char_length:
                 text_line = False
                 break
 
         nb_lines_text += int(text_line)
 
     return nb_lines_text / len(line_group.lines) >= 0.5
 
 
-def identify_line_groups(segment: ImageSegment, ocr_df: OCRDataframe) -> ImageSegment:
+def identify_line_groups(segment: ImageSegment, char_length: float, median_line_sep: float) -> ImageSegment:
     """
     From elements of the segment, identify lines that are coherent together
     :param segment: ImageSegment object
-    :param ocr_df: OCRDataframe object
+    :param char_length: average character length
+    :param median_line_sep: median line separation
     :return: segment with its groups of lines
     """
     # Identify lines in segment
     lines = identify_lines(elements=segment.elements,
-                           ref_size=int(ocr_df.median_line_sep // 4))
+                           ref_size=int(median_line_sep // 4))
 
     # Create line groups
     line_groups = [line_group for h_group in create_h_pos_groups(lines=lines)
-                   for line_group in vertically_coherent_groups(lines=h_group, max_gap=ocr_df.median_line_sep)
-                   if line_group.size > 1 and not is_text_block(line_group=line_group, ocr_df=ocr_df)]
+                   for line_group in vertically_coherent_groups(lines=h_group, max_gap=median_line_sep)
+                   if line_group.size > 1 and not is_text_block(line_group=line_group, char_length=char_length)]
 
     return ImageSegment(x1=segment.x1,
                         y1=segment.y1,
                         x2=segment.x2,
                         y2=segment.y2,
                         elements=segment.elements,
                         line_groups=line_groups)
```

### Comparing `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/model.py` & `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/model.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/segment_image.py` & `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/segment_image.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 # coding: utf-8
 import operator
 from typing import List
 
 import cv2
 import numpy as np
 
-from img2table.ocr.data import OCRDataframe
 from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.line import Line
 from img2table.tables.processing.borderless_tables.model import ImageSegment
 from img2table.tables.processing.common import is_contained_cell, merge_contours
 
 
-def create_image_segments(img: np.ndarray, ocr_df: OCRDataframe) -> List[ImageSegment]:
+def create_image_segments(img: np.ndarray, median_line_sep: float) -> List[ImageSegment]:
     """
     Create segmentation of the image into specific parts
     :param img: image array
-    :param ocr_df: OCRDataframe object
+    :param median_line_sep: median line separation
     :return: list of image segments as Cell objects
     """
     # Reprocess images
     blur = cv2.GaussianBlur(img, (5, 5), 0)
     thresh = cv2.Canny(blur, 0, 0)
 
-    # Define kernel size by using most stable metric between different OCRs
-    if ocr_df.median_line_sep is not None:
-        kernel_size = round(ocr_df.median_line_sep / 3)
-    else:
-        kernel_size = 20
+    # Define kernel size by using median line separation
+    kernel_size = round(median_line_sep / 3)
 
     # Dilate to combine adjacent text contours
     kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (kernel_size, kernel_size))
     dilate = cv2.dilate(thresh, kernel, iterations=4)
 
     # Create new image by adding black borders
     margin = 10
@@ -54,38 +50,39 @@
     # Add contours to row
     img_segments = merge_contours(contours=list_cnts_cell,
                                   vertically=None)
 
     return [ImageSegment(x1=seg.x1, y1=seg.y1, x2=seg.x2, y2=seg.y2) for seg in img_segments]
 
 
-def get_segment_elements(img: np.ndarray, lines: List[Line], img_segments: List[ImageSegment], ocr_df: OCRDataframe,
-                         blur_size: int = 3) -> List[ImageSegment]:
+def get_segment_elements(img: np.ndarray, lines: List[Line], img_segments: List[ImageSegment], char_length: float,
+                         median_line_sep: float, blur_size: int = 3) -> List[ImageSegment]:
     """
     Identify image elements that correspond to each segment
     :param img: image array
     :param lines: list of image lines
     :param img_segments: list of ImageSegment objects
+    :param char_length: average character length
+    :param median_line_sep: median line separation
     :param blur_size: kernel size for blurring operation
-    :param kernel: kernel for dilate operation
     :return: list of ImageSegment objects with corresponding elements
     """
     # Reprocess image
     blur = cv2.GaussianBlur(img, (blur_size, blur_size), 0)
     thresh = cv2.Canny(blur, 85, 255)
 
     # Mask lines
     for l in lines:
         if l.horizontal:
             cv2.rectangle(thresh, (l.x1 - l.thickness, l.y1), (l.x2 + l.thickness, l.y2), (0, 0, 0), 3 * l.thickness)
         elif l.vertical:
             cv2.rectangle(thresh, (l.x1, l.y1 - l.thickness), (l.x2, l.y2 + l.thickness), (0, 0, 0), 2 * l.thickness)
 
     # Dilate to combine adjacent text contours
-    kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (int(1.5 * ocr_df.char_length), int(ocr_df.median_line_sep // 6)))
+    kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (int(1.5 * char_length), int(median_line_sep // 6)))
     dilate = cv2.dilate(thresh, kernel, iterations=1)
 
     # Find contours, highlight text areas, and extract ROIs
     cnts = cv2.findContours(dilate, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
     cnts = cnts[0] if len(cnts) == 2 else cnts[1]
 
     # Get list of contours
@@ -102,28 +99,30 @@
     for seg in img_segments:
         segment_elements = [cnt for cnt in elements if is_contained_cell(inner_cell=cnt, outer_cell=seg)]
         seg.set_elements(elements=segment_elements)
 
     return img_segments
 
 
-def segment_image(img: np.ndarray, lines: List[Line], ocr_df: OCRDataframe) -> List[ImageSegment]:
+def segment_image(img: np.ndarray, lines: List[Line], char_length: float, median_line_sep: float) -> List[ImageSegment]:
     """
     Segment image and its elements
     :param img: image array
     :param lines: list of Line objects of the image
-    :param ocr_df: OCRDataframe object
+    :param char_length: average character length
+    :param median_line_sep: median line separation
     :return: list of ImageSegment objects with corresponding elements
     """
     # Create image segments
     image_segments = create_image_segments(img=img,
-                                           ocr_df=ocr_df)
+                                           median_line_sep=median_line_sep)
 
     # Detect elements corresponding to each segment
     image_segments = get_segment_elements(img=img,
                                           lines=lines,
                                           img_segments=image_segments,
-                                          blur_size=3,
-                                          ocr_df=ocr_df)
+                                          char_length=char_length,
+                                          median_line_sep=median_line_sep,
+                                          blur_size=3)
 
     return image_segments
```

### Comparing `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/table/__init__.py` & `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/table/headers.py` & `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/table/headers.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/tables/processing/borderless_tables/table/table_creation.py` & `img2table-0.1.0/src/img2table/tables/processing/borderless_tables/table/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/tables/processing/prepare_image.py` & `img2table-0.1.0/src/img2table/tables/processing/prepare_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table/tables/processing/text/titles.py` & `img2table-0.1.0/src/img2table/tables/processing/text/titles.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/src/img2table.egg-info/PKG-INFO` & `img2table-0.1.0/src/img2table.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 0.0.24
+Version: 0.1.0
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image 
@@ -66,14 +66,18 @@
         
         ## Supported file formats <a name="supported-file-formats"></a>
         
         ### Images <a name="images-formats"></a>
         
         Images are loaded using the `opencv-python` library, supported formats are listed below.
         
+        <details>
+        <summary>Supported image formats</summary>
+        <br>
+        
         <blockquote>
         <ul>
         <li>Windows bitmaps - <em>.bmp, </em>.dib</li>
         <li>JPEG files - <em>.jpeg, </em>.jpg, *.jpe</li>
         <li>JPEG 2000 files - *.jp2</li>
         <li>Portable Network Graphics - *.png</li>
         <li>WebP - *.webp</li>
@@ -83,15 +87,16 @@
         <li>TIFF files - <em>.tiff, </em>.tif</li>
         <li>OpenEXR Image files - *.exr</li>
         <li>Radiance HDR - <em>.hdr, </em>.pic</li>
         <li>Raster and Vector geospatial data supported by GDAL<br>
         <cite><a href="https://docs.opencv.org/4.x/d4/da8/group__imgcodecs.html#ga288b8b3da0892bd651fce07b3bbd3a56">OpenCV: Image file reading and writing</a></cite></li>
         </ul>
         </blockquote>
-        
+        </details>
+        <br>
         Multi-page images are not supported.
         
         ---
         
         ### PDF <a name="pdf-formats"></a>
         
         Both native and scanned PDF files are supported.
@@ -102,61 +107,58 @@
         
         #### Images <a name="images-doc"></a>
         Images are instantiated as follows :
         ```python
         from img2table.document import Image
         
         image = Image(src, 
-                      dpi=200,
                       detect_rotation=False)
         ```
         
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>src : str, <code>pathlib.Path</code>, bytes or <code>io.BytesIO</code>, required</dt>
         >    <dd style="font-style: italic;">Image source</dd>
-        >    <dt>dpi : int, optional, default <code>200</code></dt>
-        >    <dd style="font-style: italic;">Estimated image dpi, used to adapt OpenCV algorithm parameters</dd>
         >    <dt>detect_rotation : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Detect and correct skew/rotation of the image</dd>
         ></dl>
-        
         <br>
-        
         The implemented method to handle skewed/rotated images supports skew angles up to 45° and is
         based on the publication by <a href="https://www.mdpi.com/2079-9292/9/1/55">Huang, 2020</a>.<br>
-        Setting the `detect_rotation` parameter to `True`, image coordinates and bounding boxes returned by other 
+        Setting the <code>detect_rotation</code> parameter to <code>True</code>, image coordinates and bounding boxes returned by other 
         methods might not correspond to the original image.
         
         #### PDF <a name="pdf-doc"></a>
         PDF files are instantiated as follows :
         ```python
         from img2table.document import PDF
         
-        pdf = PDF(src, dpi=200, pages=[0, 2])
+        pdf = PDF(src, pages=[0, 2])
         ```
         
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>src : str, <code>pathlib.Path</code>, bytes or <code>io.BytesIO</code>, required</dt>
         >    <dd style="font-style: italic;">PDF source</dd>
-        >    <dt>dpi : int, optional, default <code>200</code></dt>
-        >    <dd style="font-style: italic;">Dpi used for conversion of PDF pages to images</dd>
         >    <dt>pages : list, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">List of PDF page indexes to be processed. If None, all pages are processed</dd>
         ></dl>
         
+        PDF pages are converted to images with a 200 DPI for table identification.
+        
         ---
         
         ### OCR <a name="ocr"></a>
         
         `img2table` provides an interface for several OCR services and tools in order to parse table content.<br>
         If possible (i.e for searchable PDF), PDF text will be extracted directly from the file and the OCR service/tool will not be called.
         
-        #### Tesseract <a name="tesseract"></a>
+        <details>
+        <summary>Tesseract<a name="tesseract"></a></summary>
+        <br>
         
         ```python
         from img2table.ocr import TesseractOCR
         
         ocr = TesseractOCR(n_threads=1, 
                            lang="eng", 
                            psm=11,
@@ -174,21 +176,24 @@
         >    <dt>tessdata_dir : str, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">Directory containing Tesseract traineddata files. If None, the <code>TESSDATA_PREFIX</code> env variable is used.</dd>
         ></dl>
         
         
         *Usage of [Tesseract-OCR](https://github.com/tesseract-ocr/tesseract) requires prior installation. 
         Check [documentation](https://tesseract-ocr.github.io/tessdoc/) for instructions.*
+        <br>
+        </details>
         
-        
-        #### <a href="https://github.com/PaddlePaddle/PaddleOCR">PaddleOCR</a> <a name="paddle"></a>
+        <details>
+        <summary>PaddleOCR<a name="paddle"></a></summary>
+        <br>
         
         *Available for Python versions <= 3.10*
         
-        PaddleOCR is an open-source OCR based on Deep Learning models.<br>
+        <a href="https://github.com/PaddlePaddle/PaddleOCR">PaddleOCR</a> is an open-source OCR based on Deep Learning models.<br>
         At first use, relevant languages models will be downloaded.
         
         ```python
         from img2table.ocr import PaddleOCR
         
         ocr = PaddleOCR(lang="en")
         ```
@@ -196,16 +201,20 @@
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>lang : str, optional, default <code>"en"</code></dt>
         >    <dd style="font-style: italic;">Lang parameter used in Paddle for text extraction, check <a href="https://github.com/Mushroomcat9998/PaddleOCR/blob/main/doc/doc_en/multi_languages_en.md#5-support-languages-and-abbreviations">documentation for available languages</a></dd>
         ></dl>
         
         *Released in version 0.0.13*
+        <br>
+        </details>
         
-        #### Google Vision <a name="vision"></a>
+        <details>
+        <summary>Google Vision<a name="vision"></a></summary>
+        <br>
         
         Authentication to GCP can be done by setting the standard `GOOGLE_APPLICATION_CREDENTIALS` environment variable.<br>
         If this variable is missing, an API key should be provided via the `api_key` parameter.
         
         ```python
         from img2table.ocr import VisionOCR
         
@@ -215,16 +224,20 @@
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>api_key : str, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">Google Vision API key</dd>
         >    <dt>timeout : int, optional, default <code>15</code></dt>
         >    <dd style="font-style: italic;">API requests timeout, in seconds</dd>
         ></dl>
+        <br>
+        </details>
         
-        #### AWS Textract <a name="textract"></a>
+        <details>
+        <summary>AWS Textract<a name="textract"></a></summary>
+        <br>
         
         When using AWS Textract, the DetectDocumentText API is exclusively called.
         
         Authentication to AWS can be done by passing credentials to the `TextractOCR` class.<br>
         If credentials are not provided, authentication is done using environment variables or configuration files. 
         Check `boto3` [documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) for more details.
         
@@ -244,17 +257,20 @@
         >    <dt>aws_secret_access_key : str, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">AWS secret access key</dd>
         >    <dt>aws_session_token : str, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">AWS temporary session token</dd>
         >    <dt>region : str, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">AWS server region</dd>
         ></dl>
+        <br>
+        </details>
         
-        
-        #### Azure Cognitive Services <a name="azure"></a>
+        <details>
+        <summary>Azure Cognitive Services<a name="azure"></a></summary>
+        <br>
         
         ```python
         from img2table.ocr import AzureOCR
         
         ocr = AzureOCR(endpoint="abc.azure.com",
                        subscription_key="***")
         ```
@@ -262,15 +278,16 @@
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>endpoint : str, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">Azure Cognitive Services endpoint. If None, inferred from the <code>COMPUTER_VISION_ENDPOINT</code> environment variable.</dd>
         >    <dt>subscription_key : str, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">Azure Cognitive Services subscription key. If None, inferred from the <code>COMPUTER_VISION_SUBSCRIPTION_KEY</code> environment variable.</dd>
         ></dl>
-        
+        <br>
+        </details>
         
         ---
         
         ### Table extraction <a name="table-extract"></a>
         
         Multiple tables can be extracted at once from a PDF page/ an image using the `extract_tables` method of a document.
         
@@ -278,15 +295,15 @@
         from img2table.ocr import TesseractOCR
         from img2table.document import Image
         
         # Instantiation of OCR
         ocr = TesseractOCR(n_threads=1, lang="eng")
         
         # Instantiation of document, either an image or a PDF
-        doc = Image(src, dpi=200)
+        doc = Image(src)
         
         # Table extraction
         extracted_tables = doc.extract_tables(ocr=ocr,
                                               implicit_rows=True,
                                               borderless_tables=False,
                                               min_confidence=50)
         ```
@@ -349,15 +366,15 @@
         from img2table.ocr import TesseractOCR
         from img2table.document import Image
         
         # Instantiation of OCR
         ocr = TesseractOCR(n_threads=1, lang="eng")
         
         # Instantiation of document, either an image or a PDF
-        doc = Image(src, dpi=200)
+        doc = Image(src)
         
         # Extraction of tables and creation of an xlsx file containing tables
         doc.to_xlsx(dest=dest,
                     ocr=ocr,
                     implicit_rows=True,
                     borderless_tables=False,
                     min_confidence=50)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 0.0.24 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 0.1.0 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
@@ -24,96 +24,106 @@
 files, including bounding boxes at the table cell level * Handling of complex
 table structures such as merged cells * Handling of implicit rows - see
 [example](/examples/Implicit_rows.ipynb) * Table content extraction by
 providing support for OCR services / tools * Extracted tables are returned as a
 simple object, including a Pandas DataFrame representation * Export extracted
 tables to an Excel file, preserving their original structure ## Supported file
 formats  ### Images  Images are loaded using the `opencv-python` library,
-supported formats are listed below.
+supported formats are listed below.  Supported image formats
          * Windows bitmaps - .bmp,.dib
          * JPEG files - .jpeg,.jpg, *.jpe
          * JPEG 2000 files - *.jp2
          * Portable Network Graphics - *.png
          * WebP - *.webp
          * Portable image format - .pbm,.pgm, .ppm.pxm, *.pnm
          * PFM files - *.pfm
          * Sun rasters - .sr,.ras
          * TIFF files - .tiff,.tif
          * OpenEXR Image files - *.exr
          * Radiance HDR - .hdr,.pic
          * Raster and Vector geospatial data supported by GDAL
            OpenCV:_Image_file_reading_and_writing
+
 Multi-page images are not supported. --- ### PDF  Both native and scanned PDF
 files are supported. ## Usage  ### Documents  #### Images  Images are
 instantiated as follows : ```python from img2table.document import Image image
-= Image(src, dpi=200, detect_rotation=False) ``` >
+= Image(src, detect_rotation=False) ``` >
 *** Parameters ***
 >
 >
 
 The implemented method to handle skewed/rotated images supports skew angles up
 to 45Â° and is based on the publication by Huang,_2020.
-Setting the `detect_rotation` parameter to `True`, image coordinates and
-bounding boxes returned by other methods might not correspond to the original
-image. #### PDF  PDF files are instantiated as follows : ```python from
-img2table.document import PDF pdf = PDF(src, dpi=200, pages=[0, 2]) ``` >
+Setting the detect_rotation parameter to True, image coordinates and bounding
+boxes returned by other methods might not correspond to the original image.
+#### PDF  PDF files are instantiated as follows : ```python from
+img2table.document import PDF pdf = PDF(src, pages=[0, 2]) ``` >
 *** Parameters ***
 >
 >
---- ### OCR  `img2table` provides an interface for several OCR services and
-tools in order to parse table content.
+PDF pages are converted to images with a 200 DPI for table identification. --
+- ### OCR  `img2table` provides an interface for several OCR services and tools
+in order to parse table content.
 If possible (i.e for searchable PDF), PDF text will be extracted directly from
-the file and the OCR service/tool will not be called. #### Tesseract  ```python
-from img2table.ocr import TesseractOCR ocr = TesseractOCR(n_threads=1,
-lang="eng", psm=11, tessdata_dir="...") ``` >
+the file and the OCR service/tool will not be called.  Tesseract
+```python from img2table.ocr import TesseractOCR ocr = TesseractOCR
+(n_threads=1, lang="eng", psm=11, tessdata_dir="...") ``` >
 *** Parameters ***
 >
 >
 *Usage of [Tesseract-OCR](https://github.com/tesseract-ocr/tesseract) requires
 prior installation. Check [documentation](https://tesseract-ocr.github.io/
-tessdoc/) for instructions.* #### PaddleOCR  *Available for Python versions <=
-3.10* PaddleOCR is an open-source OCR based on Deep Learning models.
+tessdoc/) for instructions.*
+  PaddleOCR
+*Available for Python versions <= 3.10* PaddleOCR is an open-source OCR based
+on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import PaddleOCR ocr = PaddleOCR(lang="en") ``` >
 *** Parameters ***
 >
 >
-*Released in version 0.0.13* #### Google Vision  Authentication to GCP can be
-done by setting the standard `GOOGLE_APPLICATION_CREDENTIALS` environment
-variable.
+*Released in version 0.0.13*
+  Google Vision
+Authentication to GCP can be done by setting the standard
+`GOOGLE_APPLICATION_CREDENTIALS` environment variable.
 If this variable is missing, an API key should be provided via the `api_key`
 parameter. ```python from img2table.ocr import VisionOCR ocr = VisionOCR
 (api_key="api_key", timeout=15) ``` >
 *** Parameters ***
 >
 >
-#### AWS Textract  When using AWS Textract, the DetectDocumentText API is
-exclusively called. Authentication to AWS can be done by passing credentials to
-the `TextractOCR` class.
+
+  AWS Textract
+When using AWS Textract, the DetectDocumentText API is exclusively called.
+Authentication to AWS can be done by passing credentials to the `TextractOCR`
+class.
 If credentials are not provided, authentication is done using environment
 variables or configuration files. Check `boto3` [documentation](https://
 boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) for
 more details. ```python from img2table.ocr import TextractOCR ocr = TextractOCR
 (aws_access_key_id="***", aws_secret_access_key="***", aws_session_token="***",
 region="eu-west-1") ``` >
 *** Parameters ***
 >
 >
-#### Azure Cognitive Services  ```python from img2table.ocr import AzureOCR ocr
-= AzureOCR(endpoint="abc.azure.com", subscription_key="***") ``` >
+
+  Azure Cognitive Services
+```python from img2table.ocr import AzureOCR ocr = AzureOCR
+(endpoint="abc.azure.com", subscription_key="***") ``` >
 *** Parameters ***
 >
 >
---- ### Table extraction  Multiple tables can be extracted at once from a PDF
+
+ --- ### Table extraction  Multiple tables can be extracted at once from a PDF
 page/ an image using the `extract_tables` method of a document. ```python from
 img2table.ocr import TesseractOCR from img2table.document import Image #
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
-Instantiation of document, either an image or a PDF doc = Image(src, dpi=200) #
-Table extraction extracted_tables = doc.extract_tables(ocr=ocr,
-implicit_rows=True, borderless_tables=False, min_confidence=50) ``` >
+Instantiation of document, either an image or a PDF doc = Image(src) # Table
+extraction extracted_tables = doc.extract_tables(ocr=ocr, implicit_rows=True,
+borderless_tables=False, min_confidence=50) ``` >
 *** Parameters ***
 >
 >
 *Borderless table extraction released in version 0.0.14* #### Method return The
 [`ExtractedTable`](/src/img2table/tables/objects/extraction.py#L35) class is
 used to model extracted tables from documents. >
 *** Attributes ***
@@ -129,15 +139,15 @@
 output = { 0: [ExtractedTable(...), ...], 1: [], ... last_page: [ExtractedTable
 (...), ...] } ``` ### Excel export  Tables extracted from a document can be
 exported to a xlsx file. The resulting file is composed of one worksheet per
 extracted table.
 Method arguments are mostly common with the `extract_tables` method. ```python
 from img2table.ocr import TesseractOCR from img2table.document import Image #
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
-Instantiation of document, either an image or a PDF doc = Image(src, dpi=200) #
+Instantiation of document, either an image or a PDF doc = Image(src) #
 Extraction of tables and creation of an xlsx file containing tables doc.to_xlsx
 (dest=dest, ocr=ocr, implicit_rows=True, borderless_tables=False,
 min_confidence=50) ``` >
 *** Parameters ***
 >
 >
 >
```

### Comparing `img2table-0.0.24/src/img2table.egg-info/SOURCES.txt` & `img2table-0.1.0/src/img2table.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 src/img2table/ocr/data.py
 src/img2table/ocr/google_vision.py
 src/img2table/ocr/paddle.py
 src/img2table/ocr/pdf.py
 src/img2table/ocr/tesseract.py
 src/img2table/tables/__init__.py
 src/img2table/tables/image.py
+src/img2table/tables/metrics.py
 src/img2table/tables/objects/__init__.py
 src/img2table/tables/objects/cell.py
 src/img2table/tables/objects/extraction.py
 src/img2table/tables/objects/line.py
 src/img2table/tables/objects/row.py
 src/img2table/tables/objects/table.py
 src/img2table/tables/processing/__init__.py
@@ -82,14 +83,15 @@
 tests/document/__init__.py
 tests/document/base/__init__.py
 tests/document/base/test_rotation.py
 tests/document/base/test_data/test.png
 tests/document/image/__init__.py
 tests/document/image/test_image.py
 tests/document/image/test_data/blank.png
+tests/document/image/test_data/dark.png
 tests/document/image/test_data/expected.xlsx
 tests/document/image/test_data/test.png
 tests/document/pdf/__init__.py
 tests/document/pdf/test_pdf.py
 tests/document/pdf/test_data/test.pdf
 tests/ocr/__init__.py
 tests/ocr/aws_textract/__init__.py
@@ -124,14 +126,16 @@
 tests/ocr/tesseract/__init__.py
 tests/ocr/tesseract/test_tesseract.py
 tests/ocr/tesseract/test_data/ocr_df.csv
 tests/ocr/tesseract/test_data/test.png
 tests/tables/__init__.py
 tests/tables/image/__init__.py
 tests/tables/image/test_image.py
+tests/tables/image/test_metrics.py
+tests/tables/image/test_data/blank.png
 tests/tables/image/test_data/expected_tables.json
 tests/tables/image/test_data/ocr.csv
 tests/tables/image/test_data/test.png
 tests/tables/objects/__init__.py
 tests/tables/objects/test_extraction.py
 tests/tables/objects/test_line.py
 tests/tables/objects/test_row.py
@@ -148,47 +152,43 @@
 tests/tables/processing/bordered_tables/cells/test_data/expected.csv
 tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
 tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
 tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
 tests/tables/processing/bordered_tables/cells/test_data/lines.json
 tests/tables/processing/bordered_tables/lines/__init__.py
 tests/tables/processing/bordered_tables/lines/test_lines.py
+tests/tables/processing/bordered_tables/lines/test_data/contours.json
 tests/tables/processing/bordered_tables/lines/test_data/expected.json
-tests/tables/processing/bordered_tables/lines/test_data/ocr.csv
 tests/tables/processing/bordered_tables/lines/test_data/test.png
 tests/tables/processing/bordered_tables/tables/__init__.py
 tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
 tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
 tests/tables/processing/bordered_tables/tables/test_table_creation.py
 tests/tables/processing/bordered_tables/tables/test_tables.py
 tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
 tests/tables/processing/bordered_tables/tables/test_data/cells.json
 tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
 tests/tables/processing/bordered_tables/tables/test_data/expected.json
 tests/tables/processing/bordered_tables/tables/test_data/implicit.png
-tests/tables/processing/bordered_tables/tables/test_data/implicit_ocr_df.csv
 tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
 tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
 tests/tables/processing/bordered_tables/tables/test_data/word_image.png
 tests/tables/processing/borderless_tables/__init__.py
 tests/tables/processing/borderless_tables/borderless_table/__init__.py
 tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
 tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
-tests/tables/processing/borderless_tables/borderless_table/test_data/ocr_df.csv
 tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
 tests/tables/processing/borderless_tables/column_delimiters/__init__.py
 tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
 tests/tables/processing/borderless_tables/lines/__init__.py
 tests/tables/processing/borderless_tables/lines/test_lines.py
 tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
-tests/tables/processing/borderless_tables/lines/test_data/ocr_df.csv
 tests/tables/processing/borderless_tables/segment_image/__init__.py
 tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
 tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
-tests/tables/processing/borderless_tables/segment_image/test_data/ocr_df.csv
 tests/tables/processing/borderless_tables/segment_image/test_data/test.png
 tests/tables/processing/borderless_tables/table/__init__.py
 tests/tables/processing/borderless_tables/table/test_headers.py
 tests/tables/processing/borderless_tables/table/test_table.py
 tests/tables/processing/borderless_tables/table/test_table_creation.py
 tests/tables/processing/common/__init__.py
 tests/tables/processing/common/test_common.py
```

### Comparing `img2table-0.0.24/tests/_mock_data/azure.pkl` & `img2table-0.1.0/tests/_mock_data/azure.pkl`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/_mock_data/tesseract_hocr.html` & `img2table-0.1.0/tests/_mock_data/tesseract_hocr.html`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/_mock_data/textract.json` & `img2table-0.1.0/tests/_mock_data/textract.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/_mock_data/vision.json` & `img2table-0.1.0/tests/_mock_data/vision.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/_mock_data/vision.pkl` & `img2table-0.1.0/tests/_mock_data/vision.pkl`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/conftest.py` & `img2table-0.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/document/base/test_data/test.png` & `img2table-0.1.0/tests/document/base/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/document/base/test_rotation.py` & `img2table-0.1.0/tests/document/base/test_rotation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 # coding: utf-8
 import cv2
 import numpy as np
 from sewar import ssim
 
 from img2table.document.base.rotation import rotate_img_with_border, fix_rotation_image, get_connected_components, \
-    get_relevant_slopes
+    get_relevant_angles, angle_dixon_q_test
 
 
 def test_get_connected_components():
     img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
 
-    cc, thresh = get_connected_components(img=img)
+    cc, ref_height, thresh = get_connected_components(img=img)
 
     assert len(cc) == 98
 
 
-def test_get_relevant_slopes():
+def test_get_relevant_angles():
     centroids = [[35.8676, 5473.6768],
                  [45.4648, 8734.32],
                  [476.386, 98.437],
                  [9834.4648, 468.47],
                  [746.746, 7348.43],
                  [846.462, 8474.48],
                  [2983.846, 94483.46],
                  [1093.46, 8473.46],
                  [3676.77, 84783.64]]
 
-    result = get_relevant_slopes(centroids=np.array(centroids), n_max=7)
+    result = get_relevant_angles(centroids=np.array(centroids), ref_height=1000, n_max=5)
 
-    assert len(result) == 7
+    assert len(result) == 5
+
+
+def test_angle_dixon_q_test():
+    result = angle_dixon_q_test(angles=[12.23, 12.78, 12.79, 12.82], confidence=0.9)
+
+    assert round(result, 3) == 12.797
 
 
 def test_fix_rotation_image():
     def crop_to_orig_img(img, orig_img):
         # Get original dimensions
         orig_height, orig_width = orig_img.shape
 
@@ -52,8 +58,8 @@
         test_img = rotate_img_with_border(img=img.copy(), angle=angle)
         result = crop_to_orig_img(img=fix_rotation_image(img=test_img),
                                   orig_img=img)
 
         # Compute similarity between original image and result
         similarities.append(ssim(GT=img, P=result)[0])
 
-    assert np.mean(similarities) >= 0.9
+    assert np.mean(similarities) >= 0.85
```

### Comparing `img2table-0.0.24/tests/document/image/test_data/blank.png` & `img2table-0.1.0/tests/document/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/document/image/test_data/expected.xlsx` & `img2table-0.1.0/tests/document/image/test_data/expected.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/document/image/test_data/test.png` & `img2table-0.1.0/tests/document/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/document/image/test_image.py` & `img2table-0.1.0/tests/document/image/test_image.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 
 
 def test_validators():
     with pytest.raises(TypeError) as e_info:
         img = Image(src=1)
 
     with pytest.raises(TypeError) as e_info:
-        img = Image(src="img", dpi="8")
-
-    with pytest.raises(TypeError) as e_info:
         img = Image(src="img", detect_rotation=3)
 
 
 def test_load_image():
     # Load from path
     img_from_path = Image(src="test_data/test.png")
 
@@ -35,27 +32,40 @@
     assert img_from_path.bytes == img_from_bytes.bytes == img_from_bytesio.bytes
 
     assert list(img_from_path.images)[0].shape == (417, 1365)
 
 
 def test_blank_image(mock_tesseract):
     ocr = TesseractOCR()
-    img = Image(src="test_data/blank.png")
+    img = Image(src="test_data/blank.png",
+                detect_rotation=True)
 
     result = img.extract_tables(ocr=ocr,
                                 implicit_rows=True,
                                 borderless_tables=True,
                                 min_confidence=50)
 
     assert result == []
 
 
+def test_blank_no_ocr():
+    img = Image(src="test_data/blank.png",
+                detect_rotation=True)
+
+    result = img.extract_tables(implicit_rows=True,
+                                borderless_tables=True,
+                                min_confidence=50)
+
+    assert result == []
+
+
 def test_image_tables(mock_tesseract):
     ocr = TesseractOCR()
-    img = Image(src="test_data/test.png")
+    img = Image(src="test_data/test.png",
+                detect_rotation=True)
 
     result = img.extract_tables(ocr=ocr, implicit_rows=True, min_confidence=50)
 
     assert len(result) == 2
 
     assert result[0].title is None
     assert result[0].bbox == BBox(x1=35, y1=20, x2=770, y2=327)
@@ -64,17 +74,32 @@
 
     assert result[1].title is None
     assert result[1].bbox == BBox(x1=962, y1=21, x2=1154, y2=123)
     assert len(result[1].content) == 2
     assert len(result[1].content[0]) == 2
 
 
+def test_no_ocr():
+    img = Image(src="test_data/dark.png",
+                detect_rotation=True)
+
+    result = img.extract_tables(implicit_rows=True, min_confidence=50)
+
+    assert len(result) == 1
+
+    assert result[0].title is None
+    assert result[0].bbox == BBox(x1=36, y1=40, x2=840, y2=529)
+    assert len(result[0].content) == 19
+    assert len(result[0].content[0]) == 7
+
+
 def test_image_excel(mock_tesseract):
     ocr = TesseractOCR()
-    img = Image(src="test_data/test.png")
+    img = Image(src="test_data/test.png",
+                detect_rotation=True)
 
     result = img.to_xlsx(dest=BytesIO(), ocr=ocr, implicit_rows=True, min_confidence=50)
 
     expected = load_workbook(filename="test_data/expected.xlsx")
     result_wb = load_workbook(filename=result)
 
     for idx, ws in enumerate(result_wb.worksheets):
```

### Comparing `img2table-0.0.24/tests/document/pdf/test_data/test.pdf` & `img2table-0.1.0/tests/document/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/document/pdf/test_pdf.py` & `img2table-0.1.0/tests/document/pdf/test_pdf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 # coding: utf-8
+import sys
 from io import BytesIO
 
 import pytest
 
 from img2table.document.pdf import PDF
 from img2table.ocr import TesseractOCR
 from img2table.tables.objects.extraction import BBox
 
 
 def test_validators():
     with pytest.raises(TypeError) as e_info:
         pdf = PDF(src=1)
 
     with pytest.raises(TypeError) as e_info:
-        pdf = PDF(src="img", dpi="8")
+        pdf = PDF(src="img", pages=12)
 
     with pytest.raises(TypeError) as e_info:
-        pdf = PDF(src="img", dpi=200, pages=12)
-
-    with pytest.raises(TypeError) as e_info:
-        pdf = PDF(src="img", dpi=200, pages=["12"])
+        pdf = PDF(src="img", pages=["12"])
 
 
 def test_load_pdf():
     # Load from path
-    pdf_from_path = PDF(src="test_data/test.pdf", dpi=300)
+    pdf_from_path = PDF(src="test_data/test.pdf")
 
     # Load from bytes
     with open("test_data/test.pdf", "rb") as f:
-        pdf_from_bytes = PDF(src=f.read(), dpi=300)
+        pdf_from_bytes = PDF(src=f.read())
 
     # Load from BytesIO
     with open("test_data/test.pdf", "rb") as f:
-        pdf_from_bytesio = PDF(src=BytesIO(f.read()), dpi=300)
+        pdf_from_bytesio = PDF(src=BytesIO(f.read()))
 
     assert pdf_from_path.bytes == pdf_from_bytes.bytes == pdf_from_bytesio.bytes
 
-    assert list(pdf_from_path.images)[0].shape == (3300, 2550)
+    assert list(pdf_from_path.images)[0].shape == (2200, 1700)
 
 
 def test_pdf_pages():
     assert len(list(PDF(src="test_data/test.pdf").images)) == 2
     assert len(list(PDF(src="test_data/test.pdf", pages=[0]).images)) == 1
 
 
 def test_pdf_tables(mock_tesseract):
     ocr = TesseractOCR()
     pdf = PDF(src="test_data/test.pdf")
 
     result = pdf.extract_tables(ocr=ocr, implicit_rows=True, min_confidence=50)
 
     assert result[0][0].title == "Example of Data Table 1"
-    assert result[0][0].bbox == BBox(x1=236, y1=249, x2=1442, y2=543)
+    if sys.version_info.minor < 11:
+        assert result[0][0].bbox == BBox(x1=236, y1=249, x2=1442, y2=543)
     assert (len(result[0][0].content), len(result[0][0].content[0])) == (5, 4)
 
     assert result[0][1].title == "Example of Data Table 2"
-    assert result[0][1].bbox == BBox(x1=235, y1=671, x2=1451, y2=971)
+    if sys.version_info.minor < 11:
+        assert result[0][1].bbox == BBox(x1=235, y1=671, x2=1451, y2=971)
     assert (len(result[0][1].content), len(result[0][1].content[0])) == (5, 4)
 
     assert result[1][0].title == "Example of Data Table 3"
-    assert result[1][0].bbox == BBox(x1=236, y1=249, x2=1442, y2=543)
+    if sys.version_info.minor < 11:
+        assert result[1][0].bbox == BBox(x1=236, y1=249, x2=1442, y2=543)
     assert (len(result[1][0].content), len(result[1][0].content[0])) == (5, 4)
 
     assert result[1][1].title == "Example of Data Table 4"
-    assert result[1][1].bbox == BBox(x1=235, y1=671, x2=1451, y2=971)
+    if sys.version_info.minor < 11:
+        assert result[1][1].bbox == BBox(x1=235, y1=671, x2=1451, y2=971)
     assert (len(result[1][1].content), len(result[1][1].content[0])) == (5, 4)
```

### Comparing `img2table-0.0.24/tests/ocr/aws_textract/test_aws_textract.py` & `img2table-0.1.0/tests/ocr/aws_textract/test_aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/aws_textract/test_data/content.json` & `img2table-0.1.0/tests/ocr/aws_textract/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/aws_textract/test_data/ocr_df.csv` & `img2table-0.1.0/tests/ocr/aws_textract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/aws_textract/test_data/test.png` & `img2table-0.1.0/tests/ocr/aws_textract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/azure/test_azure.py` & `img2table-0.1.0/tests/ocr/azure/test_azure.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/azure/test_data/ocr_df.csv` & `img2table-0.1.0/tests/ocr/azure/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/azure/test_data/test.png` & `img2table-0.1.0/tests/ocr/azure/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/data/test_data/expected_table.json` & `img2table-0.1.0/tests/ocr/data/test_data/expected_table.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/data/test_data/ocr_df.csv` & `img2table-0.1.0/tests/ocr/data/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/data/test_ocr_data.py` & `img2table-0.1.0/tests/ocr/data/test_ocr_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,14 @@
 
 from img2table.ocr.data import OCRDataframe
 from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.row import Row
 from img2table.tables.objects.table import Table
 
 
-def test_text_sizes():
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
-
-    assert round(ocr_df.median_line_sep, 2) == 51.0
-    assert round(ocr_df.char_length, 2) == 24.2
-
-
 def test_pages():
     ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     ocr_df_page_0 = ocr_df.page(page_number=0)
     ocr_df_page_1 = ocr_df.page(page_number=1)
 
     assert isinstance(ocr_df_page_0, OCRDataframe)
```

### Comparing `img2table-0.0.24/tests/ocr/google_vision/test_data/expected_content.json` & `img2table-0.1.0/tests/ocr/google_vision/test_data/expected_content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/google_vision/test_data/ocr_df.csv` & `img2table-0.1.0/tests/ocr/google_vision/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/google_vision/test_data/test.png` & `img2table-0.1.0/tests/ocr/google_vision/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/google_vision/test_google_vision.py` & `img2table-0.1.0/tests/ocr/google_vision/test_google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/paddle/test_data/hocr.json` & `img2table-0.1.0/tests/ocr/paddle/test_data/hocr.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/paddle/test_data/ocr_df.csv` & `img2table-0.1.0/tests/ocr/paddle/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/paddle/test_data/test.png` & `img2table-0.1.0/tests/ocr/paddle/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/paddle/test_paddle.py` & `img2table-0.1.0/tests/ocr/paddle/test_paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/pdf/test_data/content.json` & `img2table-0.1.0/tests/ocr/pdf/test_data/content.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7999999999999983%*

 * *Differences: {'0': "{0: {'x1': 648, 'y1': 200, 'x2': 793, 'y2': 248}, 1: {'x1': 801, 'y1': 200, 'x2': 835, "*

 * *      "'y2': 248}, 2: {'x1': 842, 'y1': 200, 'x2': 925, 'y2': 248}, 3: {'x1': 932, 'y1': 200, "*

 * *      "'x2': 1026, 'y2': 248}, 4: {'x1': 1033, 'y1': 200, 'x2': 1054, 'y2': 248}, 5: {'x1': 251, "*

 * *      "'y1': 250, 'x2': 352, 'y2': 290}, 6: {'x1': 599, 'y1': 250, 'x2': 660, 'y2': 290}, 7: "*

 * *      "{'x1': 668, 'y1': 250, 'x2': 722, 'y2': 290}, 8: {'x1': 729, 'y1': 250, 'x2': 804, 'y2': "*

 * *      "290}, 9: {'x1': 881,  […]*

```diff
@@ -3,2608 +3,2608 @@
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_0_0_0",
             "page": 0,
             "parent": "line_1_0_0",
             "value": "Example",
-            "x1": 973,
-            "x2": 1190,
-            "y1": 300,
-            "y2": 371
+            "x1": 648,
+            "x2": 793,
+            "y1": 200,
+            "y2": 248
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_0_0_1",
             "page": 0,
             "parent": "line_1_0_0",
             "value": "of",
-            "x1": 1201,
-            "x2": 1252,
-            "y1": 300,
-            "y2": 371
+            "x1": 801,
+            "x2": 835,
+            "y1": 200,
+            "y2": 248
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_0_0_2",
             "page": 0,
             "parent": "line_1_0_0",
             "value": "Data",
-            "x1": 1263,
-            "x2": 1388,
-            "y1": 300,
-            "y2": 371
+            "x1": 842,
+            "x2": 925,
+            "y1": 200,
+            "y2": 248
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_0_0_3",
             "page": 0,
             "parent": "line_1_0_0",
             "value": "Table",
-            "x1": 1399,
-            "x2": 1539,
-            "y1": 300,
-            "y2": 371
+            "x1": 932,
+            "x2": 1026,
+            "y1": 200,
+            "y2": 248
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_0_0_4",
             "page": 0,
             "parent": "line_1_0_0",
             "value": "1",
-            "x1": 1550,
-            "x2": 1581,
-            "y1": 300,
-            "y2": 371
+            "x1": 1033,
+            "x2": 1054,
+            "y1": 200,
+            "y2": 248
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_1_0_0",
             "page": 0,
             "parent": "line_1_1_0",
             "value": "sample",
-            "x1": 377,
-            "x2": 528,
-            "y1": 374,
-            "y2": 435
+            "x1": 251,
+            "x2": 352,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_1_1_0",
             "page": 0,
             "parent": "line_1_1_1",
             "value": "blue",
-            "x1": 898,
-            "x2": 991,
-            "y1": 374,
-            "y2": 435
+            "x1": 599,
+            "x2": 660,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_1_1_1",
             "page": 0,
             "parent": "line_1_1_1",
             "value": "LED",
-            "x1": 1001,
-            "x2": 1083,
-            "y1": 374,
-            "y2": 435
+            "x1": 668,
+            "x2": 722,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_1_1_2",
             "page": 0,
             "parent": "line_1_1_1",
             "value": "value",
-            "x1": 1093,
-            "x2": 1206,
-            "y1": 374,
-            "y2": 435
+            "x1": 729,
+            "x2": 804,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_1_2_0",
             "page": 0,
             "parent": "line_1_1_2",
             "value": "green",
-            "x1": 1322,
-            "x2": 1444,
-            "y1": 374,
-            "y2": 435
+            "x1": 881,
+            "x2": 963,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_1_2_1",
             "page": 0,
             "parent": "line_1_1_2",
             "value": "LED",
-            "x1": 1454,
-            "x2": 1536,
-            "y1": 374,
-            "y2": 435
+            "x1": 970,
+            "x2": 1024,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_1_2_2",
             "page": 0,
             "parent": "line_1_1_2",
             "value": "value",
-            "x1": 1546,
-            "x2": 1659,
-            "y1": 374,
-            "y2": 435
+            "x1": 1031,
+            "x2": 1106,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_1_3_0",
             "page": 0,
             "parent": "line_1_1_3",
             "value": "red",
-            "x1": 1791,
-            "x2": 1861,
-            "y1": 374,
-            "y2": 435
+            "x1": 1194,
+            "x2": 1241,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_1_3_1",
             "page": 0,
             "parent": "line_1_1_3",
             "value": "LED",
-            "x1": 1872,
-            "x2": 1953,
-            "y1": 374,
-            "y2": 435
+            "x1": 1248,
+            "x2": 1302,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_1_3_2",
             "page": 0,
             "parent": "line_1_1_3",
             "value": "value",
-            "x1": 1964,
-            "x2": 2076,
-            "y1": 374,
-            "y2": 435
+            "x1": 1309,
+            "x2": 1384,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_2_0_0",
             "page": 0,
             "parent": "line_1_2_0",
             "value": "clear",
-            "x1": 377,
-            "x2": 477,
-            "y1": 438,
-            "y2": 499
+            "x1": 251,
+            "x2": 318,
+            "y1": 292,
+            "y2": 332
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_2_0_1",
             "page": 0,
             "parent": "line_1_2_0",
             "value": "water",
-            "x1": 487,
-            "x2": 606,
-            "y1": 438,
-            "y2": 499
+            "x1": 325,
+            "x2": 404,
+            "y1": 292,
+            "y2": 332
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_2_1_0",
             "page": 0,
             "parent": "line_1_2_1",
             "value": "97",
-            "x1": 1026,
-            "x2": 1078,
-            "y1": 438,
-            "y2": 499
+            "x1": 684,
+            "x2": 718,
+            "y1": 292,
+            "y2": 332
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_2_2_0",
             "page": 0,
             "parent": "line_1_2_2",
             "value": "19",
-            "x1": 1465,
-            "x2": 1516,
-            "y1": 438,
-            "y2": 499
+            "x1": 976,
+            "x2": 1011,
+            "y1": 292,
+            "y2": 332
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_2_3_0",
             "page": 0,
             "parent": "line_1_2_3",
             "value": "79",
-            "x1": 1908,
-            "x2": 1959,
-            "y1": 438,
-            "y2": 499
+            "x1": 1272,
+            "x2": 1306,
+            "y1": 292,
+            "y2": 332
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_3_0_0",
             "page": 0,
             "parent": "line_1_3_0",
             "value": "blue",
-            "x1": 377,
-            "x2": 470,
-            "y1": 532,
-            "y2": 593
+            "x1": 251,
+            "x2": 313,
+            "y1": 355,
+            "y2": 395
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_3_0_1",
             "page": 0,
             "parent": "line_1_3_0",
             "value": "water",
-            "x1": 480,
-            "x2": 599,
-            "y1": 532,
-            "y2": 593
+            "x1": 320,
+            "x2": 400,
+            "y1": 355,
+            "y2": 395
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_3_1_0",
             "page": 0,
             "parent": "line_1_3_1",
             "value": "73",
-            "x1": 1026,
-            "x2": 1078,
-            "y1": 532,
-            "y2": 593
+            "x1": 684,
+            "x2": 718,
+            "y1": 355,
+            "y2": 395
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_3_2_0",
             "page": 0,
             "parent": "line_1_3_2",
             "value": "11",
-            "x1": 1465,
-            "x2": 1516,
-            "y1": 532,
-            "y2": 593
+            "x1": 976,
+            "x2": 1011,
+            "y1": 355,
+            "y2": 395
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_3_3_0",
             "page": 0,
             "parent": "line_1_3_3",
             "value": "13",
-            "x1": 1908,
-            "x2": 1959,
-            "y1": 532,
-            "y2": 593
+            "x1": 1272,
+            "x2": 1306,
+            "y1": 355,
+            "y2": 395
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_4_0_0",
             "page": 0,
             "parent": "line_1_4_0",
             "value": "green",
-            "x1": 377,
-            "x2": 499,
-            "y1": 627,
-            "y2": 688
+            "x1": 251,
+            "x2": 333,
+            "y1": 418,
+            "y2": 458
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_4_0_1",
             "page": 0,
             "parent": "line_1_4_0",
             "value": "water",
-            "x1": 510,
-            "x2": 629,
-            "y1": 627,
-            "y2": 688
+            "x1": 340,
+            "x2": 419,
+            "y1": 418,
+            "y2": 458
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_4_1_0",
             "page": 0,
             "parent": "line_1_4_1",
             "value": "35",
-            "x1": 1026,
-            "x2": 1078,
-            "y1": 627,
-            "y2": 688
+            "x1": 684,
+            "x2": 718,
+            "y1": 418,
+            "y2": 458
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_4_2_0",
             "page": 0,
             "parent": "line_1_4_2",
             "value": "15",
-            "x1": 1465,
-            "x2": 1516,
-            "y1": 627,
-            "y2": 688
+            "x1": 976,
+            "x2": 1011,
+            "y1": 418,
+            "y2": 458
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_4_3_0",
             "page": 0,
             "parent": "line_1_4_3",
             "value": "14",
-            "x1": 1908,
-            "x2": 1959,
-            "y1": 627,
-            "y2": 688
+            "x1": 1272,
+            "x2": 1306,
+            "y1": 418,
+            "y2": 458
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_5_0_0",
             "page": 0,
             "parent": "line_1_5_0",
             "value": "tea",
-            "x1": 377,
-            "x2": 443,
-            "y1": 721,
-            "y2": 781
+            "x1": 251,
+            "x2": 295,
+            "y1": 481,
+            "y2": 521
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_5_0_1",
             "page": 0,
             "parent": "line_1_5_0",
             "value": "water",
-            "x1": 453,
-            "x2": 572,
-            "y1": 721,
-            "y2": 781
+            "x1": 302,
+            "x2": 381,
+            "y1": 481,
+            "y2": 521
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_5_1_0",
             "page": 0,
             "parent": "line_1_5_1",
             "value": "33",
-            "x1": 1026,
-            "x2": 1078,
-            "y1": 721,
-            "y2": 781
+            "x1": 684,
+            "x2": 718,
+            "y1": 481,
+            "y2": 521
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_5_2_0",
             "page": 0,
             "parent": "line_1_5_2",
             "value": "13",
-            "x1": 1465,
-            "x2": 1516,
-            "y1": 721,
-            "y2": 781
+            "x1": 976,
+            "x2": 1011,
+            "y1": 481,
+            "y2": 521
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_5_3_0",
             "page": 0,
             "parent": "line_1_5_3",
             "value": "70",
-            "x1": 1908,
-            "x2": 1959,
-            "y1": 721,
-            "y2": 781
+            "x1": 1272,
+            "x2": 1306,
+            "y1": 481,
+            "y2": 521
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_7_0_0",
             "page": 0,
             "parent": "line_1_7_0",
             "value": "Example",
-            "x1": 983,
-            "x2": 1200,
-            "y1": 935,
-            "y2": 1007
+            "x1": 655,
+            "x2": 800,
+            "y1": 623,
+            "y2": 671
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_7_0_1",
             "page": 0,
             "parent": "line_1_7_0",
             "value": "of",
-            "x1": 1211,
-            "x2": 1263,
-            "y1": 935,
-            "y2": 1007
+            "x1": 808,
+            "x2": 842,
+            "y1": 623,
+            "y2": 671
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_7_0_2",
             "page": 0,
             "parent": "line_1_7_0",
             "value": "Data",
-            "x1": 1274,
-            "x2": 1398,
-            "y1": 935,
-            "y2": 1007
+            "x1": 849,
+            "x2": 932,
+            "y1": 623,
+            "y2": 671
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_7_0_3",
             "page": 0,
             "parent": "line_1_7_0",
             "value": "Table",
-            "x1": 1409,
-            "x2": 1549,
-            "y1": 935,
-            "y2": 1007
+            "x1": 940,
+            "x2": 1033,
+            "y1": 623,
+            "y2": 671
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_7_0_4",
             "page": 0,
             "parent": "line_1_7_0",
             "value": "2",
-            "x1": 1560,
-            "x2": 1592,
-            "y1": 935,
-            "y2": 1007
+            "x1": 1040,
+            "x2": 1061,
+            "y1": 623,
+            "y2": 671
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_8_0_0",
             "page": 0,
             "parent": "line_1_8_0",
             "value": "sample",
-            "x1": 377,
-            "x2": 528,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 251,
+            "x2": 352,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_8_1_0",
             "page": 0,
             "parent": "line_1_8_1",
             "value": "blue",
-            "x1": 839,
-            "x2": 932,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 560,
+            "x2": 622,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_8_1_1",
             "page": 0,
             "parent": "line_1_8_1",
             "value": "%",
-            "x1": 943,
-            "x2": 982,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 629,
+            "x2": 655,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_8_1_2",
             "page": 0,
             "parent": "line_1_8_1",
             "value": "transmitted",
-            "x1": 993,
-            "x2": 1237,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 662,
+            "x2": 825,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_8_2_0",
             "page": 0,
             "parent": "line_1_8_2",
             "value": "green",
-            "x1": 1293,
-            "x2": 1415,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 862,
+            "x2": 943,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_8_2_1",
             "page": 0,
             "parent": "line_1_8_2",
             "value": "%",
-            "x1": 1426,
-            "x2": 1465,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 950,
+            "x2": 977,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_8_2_2",
             "page": 0,
             "parent": "line_1_8_2",
             "value": "transmitted",
-            "x1": 1476,
-            "x2": 1720,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 984,
+            "x2": 1147,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_8_3_0",
             "page": 0,
             "parent": "line_1_8_3",
             "value": "red",
-            "x1": 1775,
-            "x2": 1845,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 1183,
+            "x2": 1230,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_8_3_1",
             "page": 0,
             "parent": "line_1_8_3",
             "value": "%",
-            "x1": 1855,
-            "x2": 1895,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 1237,
+            "x2": 1263,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_8_3_2",
             "page": 0,
             "parent": "line_1_8_3",
             "value": "transmitted",
-            "x1": 1905,
-            "x2": 2150,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 1270,
+            "x2": 1433,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_9_0_0",
             "page": 0,
             "parent": "line_1_9_0",
             "value": "clear",
-            "x1": 377,
-            "x2": 477,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 251,
+            "x2": 318,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_9_0_1",
             "page": 0,
             "parent": "line_1_9_0",
             "value": "water",
-            "x1": 487,
-            "x2": 606,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 325,
+            "x2": 404,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_9_1_0",
             "page": 0,
             "parent": "line_1_9_1",
             "value": "97/97",
-            "x1": 895,
-            "x2": 1015,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 597,
+            "x2": 676,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_9_1_1",
             "page": 0,
             "parent": "line_1_9_1",
             "value": "=",
-            "x1": 1025,
-            "x2": 1055,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 683,
+            "x2": 703,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_9_1_2",
             "page": 0,
             "parent": "line_1_9_1",
             "value": "100%",
-            "x1": 1066,
-            "x2": 1182,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 710,
+            "x2": 788,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_9_2_0",
             "page": 0,
             "parent": "line_1_9_2",
             "value": "19/19",
-            "x1": 1363,
-            "x2": 1483,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 909,
+            "x2": 988,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_9_2_1",
             "page": 0,
             "parent": "line_1_9_2",
             "value": "=",
-            "x1": 1493,
-            "x2": 1523,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 996,
+            "x2": 1015,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_9_2_2",
             "page": 0,
             "parent": "line_1_9_2",
             "value": "100%",
-            "x1": 1534,
-            "x2": 1650,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 1022,
+            "x2": 1100,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_9_3_0",
             "page": 0,
             "parent": "line_1_9_3",
             "value": "79/79",
-            "x1": 1819,
-            "x2": 1938,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 1212,
+            "x2": 1292,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_9_3_1",
             "page": 0,
             "parent": "line_1_9_3",
             "value": "=",
-            "x1": 1949,
-            "x2": 1979,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 1299,
+            "x2": 1319,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_9_3_2",
             "page": 0,
             "parent": "line_1_9_3",
             "value": "100%",
-            "x1": 1989,
-            "x2": 2106,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 1326,
+            "x2": 1404,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_10_0_0",
             "page": 0,
             "parent": "line_1_10_0",
             "value": "blue",
-            "x1": 377,
-            "x2": 470,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 251,
+            "x2": 313,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_10_0_1",
             "page": 0,
             "parent": "line_1_10_0",
             "value": "water",
-            "x1": 480,
-            "x2": 599,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 320,
+            "x2": 400,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_10_1_0",
             "page": 0,
             "parent": "line_1_10_1",
             "value": "73/97",
-            "x1": 908,
-            "x2": 1027,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 605,
+            "x2": 685,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_10_1_1",
             "page": 0,
             "parent": "line_1_10_1",
             "value": "=",
-            "x1": 1038,
-            "x2": 1068,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 692,
+            "x2": 712,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_10_1_2",
             "page": 0,
             "parent": "line_1_10_1",
             "value": "75%",
-            "x1": 1078,
-            "x2": 1169,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 719,
+            "x2": 779,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_10_2_0",
             "page": 0,
             "parent": "line_1_10_2",
             "value": "11/19",
-            "x1": 1376,
-            "x2": 1496,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 917,
+            "x2": 997,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_10_2_1",
             "page": 0,
             "parent": "line_1_10_2",
             "value": "=",
-            "x1": 1506,
-            "x2": 1536,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 1004,
+            "x2": 1024,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_10_2_2",
             "page": 0,
             "parent": "line_1_10_2",
             "value": "58%",
-            "x1": 1547,
-            "x2": 1637,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 1031,
+            "x2": 1092,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_10_3_0",
             "page": 0,
             "parent": "line_1_10_3",
             "value": "13/79",
-            "x1": 1832,
-            "x2": 1951,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 1221,
+            "x2": 1301,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_10_3_1",
             "page": 0,
             "parent": "line_1_10_3",
             "value": "=",
-            "x1": 1962,
-            "x2": 1992,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 1308,
+            "x2": 1328,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_10_3_2",
             "page": 0,
             "parent": "line_1_10_3",
             "value": "17%",
-            "x1": 2002,
-            "x2": 2093,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 1335,
+            "x2": 1395,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_11_0_0",
             "page": 0,
             "parent": "line_1_11_0",
             "value": "green",
-            "x1": 377,
-            "x2": 499,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 251,
+            "x2": 333,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_11_0_1",
             "page": 0,
             "parent": "line_1_11_0",
             "value": "water",
-            "x1": 510,
-            "x2": 629,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 340,
+            "x2": 419,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_11_1_0",
             "page": 0,
             "parent": "line_1_11_1",
             "value": "35/97",
-            "x1": 908,
-            "x2": 1027,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 605,
+            "x2": 685,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_11_1_1",
             "page": 0,
             "parent": "line_1_11_1",
             "value": "=",
-            "x1": 1038,
-            "x2": 1068,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 692,
+            "x2": 712,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_11_1_2",
             "page": 0,
             "parent": "line_1_11_1",
             "value": "36%",
-            "x1": 1078,
-            "x2": 1169,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 719,
+            "x2": 779,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_11_2_0",
             "page": 0,
             "parent": "line_1_11_2",
             "value": "15/19",
-            "x1": 1376,
-            "x2": 1496,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 917,
+            "x2": 997,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_11_2_1",
             "page": 0,
             "parent": "line_1_11_2",
             "value": "=",
-            "x1": 1506,
-            "x2": 1536,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 1004,
+            "x2": 1024,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_11_2_2",
             "page": 0,
             "parent": "line_1_11_2",
             "value": "79%",
-            "x1": 1547,
-            "x2": 1637,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 1031,
+            "x2": 1092,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_11_3_0",
             "page": 0,
             "parent": "line_1_11_3",
             "value": "14/79",
-            "x1": 1832,
-            "x2": 1951,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 1221,
+            "x2": 1301,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_11_3_1",
             "page": 0,
             "parent": "line_1_11_3",
             "value": "=",
-            "x1": 1962,
-            "x2": 1992,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 1308,
+            "x2": 1328,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_11_3_2",
             "page": 0,
             "parent": "line_1_11_3",
             "value": "18%",
-            "x1": 2002,
-            "x2": 2093,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 1335,
+            "x2": 1395,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_12_0_0",
             "page": 0,
             "parent": "line_1_12_0",
             "value": "tea",
-            "x1": 377,
-            "x2": 443,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 251,
+            "x2": 295,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_12_0_1",
             "page": 0,
             "parent": "line_1_12_0",
             "value": "water",
-            "x1": 453,
-            "x2": 572,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 302,
+            "x2": 381,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_12_1_0",
             "page": 0,
             "parent": "line_1_12_1",
             "value": "33/97",
-            "x1": 908,
-            "x2": 1027,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 605,
+            "x2": 685,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_12_1_1",
             "page": 0,
             "parent": "line_1_12_1",
             "value": "=",
-            "x1": 1038,
-            "x2": 1068,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 692,
+            "x2": 712,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_12_1_2",
             "page": 0,
             "parent": "line_1_12_1",
             "value": "34%",
-            "x1": 1078,
-            "x2": 1169,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 719,
+            "x2": 779,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_12_2_0",
             "page": 0,
             "parent": "line_1_12_2",
             "value": "13/19",
-            "x1": 1376,
-            "x2": 1496,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 917,
+            "x2": 997,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_12_2_1",
             "page": 0,
             "parent": "line_1_12_2",
             "value": "=",
-            "x1": 1506,
-            "x2": 1536,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 1004,
+            "x2": 1024,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_12_2_2",
             "page": 0,
             "parent": "line_1_12_2",
             "value": "68%",
-            "x1": 1547,
-            "x2": 1637,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 1031,
+            "x2": 1092,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_12_3_0",
             "page": 0,
             "parent": "line_1_12_3",
             "value": "70/79",
-            "x1": 1832,
-            "x2": 1951,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 1221,
+            "x2": 1301,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_12_3_1",
             "page": 0,
             "parent": "line_1_12_3",
             "value": "=",
-            "x1": 1962,
-            "x2": 1992,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 1308,
+            "x2": 1328,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_12_3_2",
             "page": 0,
             "parent": "line_1_12_3",
             "value": "91%",
-            "x1": 2002,
-            "x2": 2093,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 1335,
+            "x2": 1395,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_14_0_0",
             "page": 0,
             "parent": "line_1_14_0",
             "value": "Example",
-            "x1": 732,
-            "x2": 949,
-            "y1": 1577,
-            "y2": 1649
+            "x1": 488,
+            "x2": 633,
+            "y1": 1051,
+            "y2": 1099
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_14_0_1",
             "page": 0,
             "parent": "line_1_14_0",
             "value": "of",
-            "x1": 960,
-            "x2": 1012,
-            "y1": 1577,
-            "y2": 1649
+            "x1": 640,
+            "x2": 675,
+            "y1": 1051,
+            "y2": 1099
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_14_0_2",
             "page": 0,
             "parent": "line_1_14_0",
             "value": "Measuring",
-            "x1": 1023,
-            "x2": 1291,
-            "y1": 1577,
-            "y2": 1649
+            "x1": 682,
+            "x2": 861,
+            "y1": 1051,
+            "y2": 1099
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_14_0_3",
             "page": 0,
             "parent": "line_1_14_0",
             "value": "Ocean",
-            "x1": 1302,
-            "x2": 1463,
-            "y1": 1577,
-            "y2": 1649
+            "x1": 868,
+            "x2": 975,
+            "y1": 1051,
+            "y2": 1099
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_14_0_4",
             "page": 0,
             "parent": "line_1_14_0",
             "value": "Color",
-            "x1": 1474,
-            "x2": 1610,
-            "y1": 1577,
-            "y2": 1649
+            "x1": 983,
+            "x2": 1073,
+            "y1": 1051,
+            "y2": 1099
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_14_0_5",
             "page": 0,
             "parent": "line_1_14_0",
             "value": "Graph",
-            "x1": 1621,
-            "x2": 1780,
-            "y1": 1577,
-            "y2": 1649
+            "x1": 1081,
+            "x2": 1186,
+            "y1": 1051,
+            "y2": 1099
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_1_14_0_6",
             "page": 0,
             "parent": "line_1_14_0",
             "value": "1",
-            "x1": 1790,
-            "x2": 1822,
-            "y1": 1577,
-            "y2": 1649
+            "x1": 1194,
+            "x2": 1215,
+            "y1": 1051,
+            "y2": 1099
         }
     ],
     [
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_0_0_0",
             "page": 1,
             "parent": "line_2_0_0",
             "value": "Example",
-            "x1": 973,
-            "x2": 1190,
-            "y1": 300,
-            "y2": 371
+            "x1": 648,
+            "x2": 793,
+            "y1": 200,
+            "y2": 248
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_0_0_1",
             "page": 1,
             "parent": "line_2_0_0",
             "value": "of",
-            "x1": 1201,
-            "x2": 1252,
-            "y1": 300,
-            "y2": 371
+            "x1": 801,
+            "x2": 835,
+            "y1": 200,
+            "y2": 248
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_0_0_2",
             "page": 1,
             "parent": "line_2_0_0",
             "value": "Data",
-            "x1": 1263,
-            "x2": 1388,
-            "y1": 300,
-            "y2": 371
+            "x1": 842,
+            "x2": 925,
+            "y1": 200,
+            "y2": 248
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_0_0_3",
             "page": 1,
             "parent": "line_2_0_0",
             "value": "Table",
-            "x1": 1399,
-            "x2": 1539,
-            "y1": 300,
-            "y2": 371
+            "x1": 932,
+            "x2": 1026,
+            "y1": 200,
+            "y2": 248
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_0_0_4",
             "page": 1,
             "parent": "line_2_0_0",
             "value": "3",
-            "x1": 1550,
-            "x2": 1581,
-            "y1": 300,
-            "y2": 371
+            "x1": 1033,
+            "x2": 1054,
+            "y1": 200,
+            "y2": 248
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_1_0_0",
             "page": 1,
             "parent": "line_2_1_0",
             "value": "sample",
-            "x1": 377,
-            "x2": 528,
-            "y1": 374,
-            "y2": 435
+            "x1": 251,
+            "x2": 352,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_1_1_0",
             "page": 1,
             "parent": "line_2_1_1",
             "value": "blue",
-            "x1": 898,
-            "x2": 991,
-            "y1": 374,
-            "y2": 435
+            "x1": 599,
+            "x2": 660,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_1_1_1",
             "page": 1,
             "parent": "line_2_1_1",
             "value": "LED",
-            "x1": 1001,
-            "x2": 1083,
-            "y1": 374,
-            "y2": 435
+            "x1": 668,
+            "x2": 722,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_1_1_2",
             "page": 1,
             "parent": "line_2_1_1",
             "value": "value",
-            "x1": 1093,
-            "x2": 1206,
-            "y1": 374,
-            "y2": 435
+            "x1": 729,
+            "x2": 804,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_1_2_0",
             "page": 1,
             "parent": "line_2_1_2",
             "value": "green",
-            "x1": 1322,
-            "x2": 1444,
-            "y1": 374,
-            "y2": 435
+            "x1": 881,
+            "x2": 963,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_1_2_1",
             "page": 1,
             "parent": "line_2_1_2",
             "value": "LED",
-            "x1": 1454,
-            "x2": 1536,
-            "y1": 374,
-            "y2": 435
+            "x1": 970,
+            "x2": 1024,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_1_2_2",
             "page": 1,
             "parent": "line_2_1_2",
             "value": "value",
-            "x1": 1546,
-            "x2": 1659,
-            "y1": 374,
-            "y2": 435
+            "x1": 1031,
+            "x2": 1106,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_1_3_0",
             "page": 1,
             "parent": "line_2_1_3",
             "value": "red",
-            "x1": 1791,
-            "x2": 1861,
-            "y1": 374,
-            "y2": 435
+            "x1": 1194,
+            "x2": 1241,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_1_3_1",
             "page": 1,
             "parent": "line_2_1_3",
             "value": "LED",
-            "x1": 1872,
-            "x2": 1953,
-            "y1": 374,
-            "y2": 435
+            "x1": 1248,
+            "x2": 1302,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_1_3_2",
             "page": 1,
             "parent": "line_2_1_3",
             "value": "value",
-            "x1": 1964,
-            "x2": 2076,
-            "y1": 374,
-            "y2": 435
+            "x1": 1309,
+            "x2": 1384,
+            "y1": 250,
+            "y2": 290
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_2_0_0",
             "page": 1,
             "parent": "line_2_2_0",
             "value": "+",
-            "x1": 377,
-            "x2": 407,
-            "y1": 438,
-            "y2": 499
+            "x1": 251,
+            "x2": 271,
+            "y1": 292,
+            "y2": 332
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_2_0_1",
             "page": 1,
             "parent": "line_2_2_0",
             "value": "1",
-            "x1": 417,
-            "x2": 443,
-            "y1": 438,
-            "y2": 499
+            "x1": 278,
+            "x2": 295,
+            "y1": 292,
+            "y2": 332
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_2_0_2",
             "page": 1,
             "parent": "line_2_2_0",
             "value": "tsp",
-            "x1": 454,
-            "x2": 518,
-            "y1": 438,
-            "y2": 499
+            "x1": 302,
+            "x2": 346,
+            "y1": 292,
+            "y2": 332
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_2_0_3",
             "page": 1,
             "parent": "line_2_2_0",
             "value": "milk",
-            "x1": 529,
-            "x2": 618,
-            "y1": 438,
-            "y2": 499
+            "x1": 353,
+            "x2": 412,
+            "y1": 292,
+            "y2": 332
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_2_1_0",
             "page": 1,
             "parent": "line_2_2_1",
             "value": "13",
-            "x1": 1026,
-            "x2": 1078,
-            "y1": 438,
-            "y2": 499
+            "x1": 684,
+            "x2": 718,
+            "y1": 292,
+            "y2": 332
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_2_2_0",
             "page": 1,
             "parent": "line_2_2_2",
             "value": "14",
-            "x1": 1465,
-            "x2": 1516,
-            "y1": 438,
-            "y2": 499
+            "x1": 976,
+            "x2": 1011,
+            "y1": 292,
+            "y2": 332
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_2_3_0",
             "page": 1,
             "parent": "line_2_2_3",
             "value": "12",
-            "x1": 1908,
-            "x2": 1959,
-            "y1": 438,
-            "y2": 499
+            "x1": 1272,
+            "x2": 1306,
+            "y1": 292,
+            "y2": 332
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_3_0_0",
             "page": 1,
             "parent": "line_2_3_0",
             "value": "+1tsp",
-            "x1": 377,
-            "x2": 497,
-            "y1": 532,
-            "y2": 593
+            "x1": 251,
+            "x2": 332,
+            "y1": 355,
+            "y2": 395
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_3_0_1",
             "page": 1,
             "parent": "line_2_3_0",
             "value": "milk",
-            "x1": 508,
-            "x2": 597,
-            "y1": 532,
-            "y2": 593
+            "x1": 339,
+            "x2": 398,
+            "y1": 355,
+            "y2": 395
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_3_0_2",
             "page": 1,
             "parent": "line_2_3_0",
             "value": "+",
-            "x1": 607,
-            "x2": 637,
-            "y1": 532,
-            "y2": 593
+            "x1": 405,
+            "x2": 425,
+            "y1": 355,
+            "y2": 395
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_3_0_3",
             "page": 1,
             "parent": "line_2_3_0",
             "value": "blue",
-            "x1": 648,
-            "x2": 740,
-            "y1": 532,
-            "y2": 593
+            "x1": 432,
+            "x2": 494,
+            "y1": 355,
+            "y2": 395
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_3_1_0",
             "page": 1,
             "parent": "line_2_3_1",
             "value": "10",
-            "x1": 1026,
-            "x2": 1078,
-            "y1": 532,
-            "y2": 593
+            "x1": 684,
+            "x2": 718,
+            "y1": 355,
+            "y2": 395
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_3_2_0",
             "page": 1,
             "parent": "line_2_3_2",
             "value": "9",
-            "x1": 1477,
-            "x2": 1503,
-            "y1": 532,
-            "y2": 593
+            "x1": 985,
+            "x2": 1002,
+            "y1": 355,
+            "y2": 395
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_3_3_0",
             "page": 1,
             "parent": "line_2_3_3",
             "value": "6",
-            "x1": 1921,
-            "x2": 1947,
-            "y1": 532,
-            "y2": 593
+            "x1": 1281,
+            "x2": 1298,
+            "y1": 355,
+            "y2": 395
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_4_0_0",
             "page": 1,
             "parent": "line_2_4_0",
             "value": "+1tsp",
-            "x1": 377,
-            "x2": 497,
-            "y1": 627,
-            "y2": 688
+            "x1": 251,
+            "x2": 332,
+            "y1": 418,
+            "y2": 458
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_4_0_1",
             "page": 1,
             "parent": "line_2_4_0",
             "value": "milk",
-            "x1": 508,
-            "x2": 597,
-            "y1": 627,
-            "y2": 688
+            "x1": 339,
+            "x2": 398,
+            "y1": 418,
+            "y2": 458
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_4_0_2",
             "page": 1,
             "parent": "line_2_4_0",
             "value": "+green",
-            "x1": 607,
-            "x2": 759,
-            "y1": 627,
-            "y2": 688
+            "x1": 405,
+            "x2": 506,
+            "y1": 418,
+            "y2": 458
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_4_1_0",
             "page": 1,
             "parent": "line_2_4_1",
             "value": "9",
-            "x1": 1039,
-            "x2": 1065,
-            "y1": 627,
-            "y2": 688
+            "x1": 693,
+            "x2": 710,
+            "y1": 418,
+            "y2": 458
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_4_2_0",
             "page": 1,
             "parent": "line_2_4_2",
             "value": "13",
-            "x1": 1465,
-            "x2": 1516,
-            "y1": 627,
-            "y2": 688
+            "x1": 976,
+            "x2": 1011,
+            "y1": 418,
+            "y2": 458
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_4_3_0",
             "page": 1,
             "parent": "line_2_4_3",
             "value": "7",
-            "x1": 1921,
-            "x2": 1947,
-            "y1": 627,
-            "y2": 688
+            "x1": 1281,
+            "x2": 1298,
+            "y1": 418,
+            "y2": 458
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_5_0_0",
             "page": 1,
             "parent": "line_2_5_0",
             "value": "+1tsp",
-            "x1": 377,
-            "x2": 497,
-            "y1": 721,
-            "y2": 781
+            "x1": 251,
+            "x2": 332,
+            "y1": 481,
+            "y2": 521
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_5_0_1",
             "page": 1,
             "parent": "line_2_5_0",
             "value": "milk",
-            "x1": 508,
-            "x2": 597,
-            "y1": 721,
-            "y2": 781
+            "x1": 339,
+            "x2": 398,
+            "y1": 481,
+            "y2": 521
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_5_0_2",
             "page": 1,
             "parent": "line_2_5_0",
             "value": "+",
-            "x1": 607,
-            "x2": 637,
-            "y1": 721,
-            "y2": 781
+            "x1": 405,
+            "x2": 425,
+            "y1": 481,
+            "y2": 521
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_5_0_3",
             "page": 1,
             "parent": "line_2_5_0",
             "value": "tea",
-            "x1": 648,
-            "x2": 713,
-            "y1": 721,
-            "y2": 781
+            "x1": 432,
+            "x2": 475,
+            "y1": 481,
+            "y2": 521
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_5_1_0",
             "page": 1,
             "parent": "line_2_5_1",
             "value": "7",
-            "x1": 1039,
-            "x2": 1065,
-            "y1": 721,
-            "y2": 781
+            "x1": 693,
+            "x2": 710,
+            "y1": 481,
+            "y2": 521
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_5_2_0",
             "page": 1,
             "parent": "line_2_5_2",
             "value": "9",
-            "x1": 1477,
-            "x2": 1503,
-            "y1": 721,
-            "y2": 781
+            "x1": 985,
+            "x2": 1002,
+            "y1": 481,
+            "y2": 521
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_5_3_0",
             "page": 1,
             "parent": "line_2_5_3",
             "value": "9",
-            "x1": 1921,
-            "x2": 1947,
-            "y1": 721,
-            "y2": 781
+            "x1": 1281,
+            "x2": 1298,
+            "y1": 481,
+            "y2": 521
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_7_0_0",
             "page": 1,
             "parent": "line_2_7_0",
             "value": "Example",
-            "x1": 983,
-            "x2": 1200,
-            "y1": 935,
-            "y2": 1007
+            "x1": 655,
+            "x2": 800,
+            "y1": 623,
+            "y2": 671
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_7_0_1",
             "page": 1,
             "parent": "line_2_7_0",
             "value": "of",
-            "x1": 1211,
-            "x2": 1263,
-            "y1": 935,
-            "y2": 1007
+            "x1": 808,
+            "x2": 842,
+            "y1": 623,
+            "y2": 671
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_7_0_2",
             "page": 1,
             "parent": "line_2_7_0",
             "value": "Data",
-            "x1": 1274,
-            "x2": 1398,
-            "y1": 935,
-            "y2": 1007
+            "x1": 849,
+            "x2": 932,
+            "y1": 623,
+            "y2": 671
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_7_0_3",
             "page": 1,
             "parent": "line_2_7_0",
             "value": "Table",
-            "x1": 1409,
-            "x2": 1549,
-            "y1": 935,
-            "y2": 1007
+            "x1": 940,
+            "x2": 1033,
+            "y1": 623,
+            "y2": 671
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_7_0_4",
             "page": 1,
             "parent": "line_2_7_0",
             "value": "4",
-            "x1": 1560,
-            "x2": 1592,
-            "y1": 935,
-            "y2": 1007
+            "x1": 1040,
+            "x2": 1061,
+            "y1": 623,
+            "y2": 671
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_8_0_0",
             "page": 1,
             "parent": "line_2_8_0",
             "value": "Water",
-            "x1": 377,
-            "x2": 501,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 251,
+            "x2": 334,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_8_0_1",
             "page": 1,
             "parent": "line_2_8_0",
             "value": "sample",
-            "x1": 512,
-            "x2": 663,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 341,
+            "x2": 442,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_8_1_0",
             "page": 1,
             "parent": "line_2_8_1",
             "value": "blue",
-            "x1": 839,
-            "x2": 932,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 560,
+            "x2": 622,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_8_1_1",
             "page": 1,
             "parent": "line_2_8_1",
             "value": "%",
-            "x1": 943,
-            "x2": 982,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 629,
+            "x2": 655,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_8_1_2",
             "page": 1,
             "parent": "line_2_8_1",
             "value": "transmitted",
-            "x1": 993,
-            "x2": 1237,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 662,
+            "x2": 825,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_8_2_0",
             "page": 1,
             "parent": "line_2_8_2",
             "value": "green",
-            "x1": 1293,
-            "x2": 1415,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 862,
+            "x2": 943,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_8_2_1",
             "page": 1,
             "parent": "line_2_8_2",
             "value": "%",
-            "x1": 1426,
-            "x2": 1465,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 950,
+            "x2": 977,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_8_2_2",
             "page": 1,
             "parent": "line_2_8_2",
             "value": "transmitted",
-            "x1": 1476,
-            "x2": 1720,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 984,
+            "x2": 1147,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_8_3_0",
             "page": 1,
             "parent": "line_2_8_3",
             "value": "red",
-            "x1": 1775,
-            "x2": 1845,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 1183,
+            "x2": 1230,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_8_3_1",
             "page": 1,
             "parent": "line_2_8_3",
             "value": "%",
-            "x1": 1855,
-            "x2": 1895,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 1237,
+            "x2": 1263,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_8_3_2",
             "page": 1,
             "parent": "line_2_8_3",
             "value": "transmitted",
-            "x1": 1905,
-            "x2": 2150,
-            "y1": 1007,
-            "y2": 1068
+            "x1": 1270,
+            "x2": 1433,
+            "y1": 672,
+            "y2": 712
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_9_0_0",
             "page": 1,
             "parent": "line_2_9_0",
             "value": "+",
-            "x1": 377,
-            "x2": 407,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 251,
+            "x2": 271,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_9_0_1",
             "page": 1,
             "parent": "line_2_9_0",
             "value": "1",
-            "x1": 417,
-            "x2": 443,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 278,
+            "x2": 295,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_9_0_2",
             "page": 1,
             "parent": "line_2_9_0",
             "value": "tsp",
-            "x1": 454,
-            "x2": 518,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 302,
+            "x2": 346,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_9_0_3",
             "page": 1,
             "parent": "line_2_9_0",
             "value": "milk",
-            "x1": 529,
-            "x2": 618,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 353,
+            "x2": 412,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_9_1_0",
             "page": 1,
             "parent": "line_2_9_1",
             "value": "13/13",
-            "x1": 895,
-            "x2": 1015,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 597,
+            "x2": 676,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_9_1_1",
             "page": 1,
             "parent": "line_2_9_1",
             "value": "=",
-            "x1": 1025,
-            "x2": 1055,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 683,
+            "x2": 703,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_9_1_2",
             "page": 1,
             "parent": "line_2_9_1",
             "value": "100%",
-            "x1": 1066,
-            "x2": 1182,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 710,
+            "x2": 788,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_9_2_0",
             "page": 1,
             "parent": "line_2_9_2",
             "value": "14/14",
-            "x1": 1363,
-            "x2": 1483,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 909,
+            "x2": 988,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_9_2_1",
             "page": 1,
             "parent": "line_2_9_2",
             "value": "=",
-            "x1": 1493,
-            "x2": 1523,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 996,
+            "x2": 1015,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_9_2_2",
             "page": 1,
             "parent": "line_2_9_2",
             "value": "100%",
-            "x1": 1534,
-            "x2": 1650,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 1022,
+            "x2": 1100,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_9_3_0",
             "page": 1,
             "parent": "line_2_9_3",
             "value": "12/12",
-            "x1": 1819,
-            "x2": 1938,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 1212,
+            "x2": 1292,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_9_3_1",
             "page": 1,
             "parent": "line_2_9_3",
             "value": "=",
-            "x1": 1949,
-            "x2": 1979,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 1299,
+            "x2": 1319,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_9_3_2",
             "page": 1,
             "parent": "line_2_9_3",
             "value": "100%",
-            "x1": 1989,
-            "x2": 2106,
-            "y1": 1089,
-            "y2": 1150
+            "x1": 1326,
+            "x2": 1404,
+            "y1": 726,
+            "y2": 766
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_10_0_0",
             "page": 1,
             "parent": "line_2_10_0",
             "value": "+1tsp",
-            "x1": 377,
-            "x2": 497,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 251,
+            "x2": 332,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_10_0_1",
             "page": 1,
             "parent": "line_2_10_0",
             "value": "milk",
-            "x1": 508,
-            "x2": 597,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 339,
+            "x2": 398,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_10_0_2",
             "page": 1,
             "parent": "line_2_10_0",
             "value": "+",
-            "x1": 607,
-            "x2": 637,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 405,
+            "x2": 425,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_10_0_3",
             "page": 1,
             "parent": "line_2_10_0",
             "value": "blue",
-            "x1": 648,
-            "x2": 740,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 432,
+            "x2": 494,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_10_1_0",
             "page": 1,
             "parent": "line_2_10_1",
             "value": "10/13",
-            "x1": 908,
-            "x2": 1027,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 605,
+            "x2": 685,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_10_1_1",
             "page": 1,
             "parent": "line_2_10_1",
             "value": "=",
-            "x1": 1038,
-            "x2": 1068,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 692,
+            "x2": 712,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_10_1_2",
             "page": 1,
             "parent": "line_2_10_1",
             "value": "77%",
-            "x1": 1078,
-            "x2": 1169,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 719,
+            "x2": 779,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_10_2_0",
             "page": 1,
             "parent": "line_2_10_2",
             "value": "9/14",
-            "x1": 1389,
-            "x2": 1483,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 926,
+            "x2": 988,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_10_2_1",
             "page": 1,
             "parent": "line_2_10_2",
             "value": "=",
-            "x1": 1493,
-            "x2": 1523,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 996,
+            "x2": 1015,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_10_2_2",
             "page": 1,
             "parent": "line_2_10_2",
             "value": "64%",
-            "x1": 1534,
-            "x2": 1625,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 1022,
+            "x2": 1083,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_10_3_0",
             "page": 1,
             "parent": "line_2_10_3",
             "value": "6/12",
-            "x1": 1844,
-            "x2": 1938,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 1230,
+            "x2": 1292,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_10_3_1",
             "page": 1,
             "parent": "line_2_10_3",
             "value": "=",
-            "x1": 1949,
-            "x2": 1979,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 1299,
+            "x2": 1319,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_10_3_2",
             "page": 1,
             "parent": "line_2_10_3",
             "value": "50%",
-            "x1": 1989,
-            "x2": 2080,
-            "y1": 1181,
-            "y2": 1241
+            "x1": 1326,
+            "x2": 1387,
+            "y1": 788,
+            "y2": 828
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_11_0_0",
             "page": 1,
             "parent": "line_2_11_0",
             "value": "+1tsp",
-            "x1": 377,
-            "x2": 497,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 251,
+            "x2": 332,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_11_0_1",
             "page": 1,
             "parent": "line_2_11_0",
             "value": "milk",
-            "x1": 508,
-            "x2": 597,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 339,
+            "x2": 398,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_11_0_2",
             "page": 1,
             "parent": "line_2_11_0",
             "value": "+green",
-            "x1": 607,
-            "x2": 759,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 405,
+            "x2": 506,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_11_1_0",
             "page": 1,
             "parent": "line_2_11_1",
             "value": "9/13",
-            "x1": 920,
-            "x2": 1015,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 614,
+            "x2": 676,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_11_1_1",
             "page": 1,
             "parent": "line_2_11_1",
             "value": "=",
-            "x1": 1025,
-            "x2": 1055,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 683,
+            "x2": 703,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_11_1_2",
             "page": 1,
             "parent": "line_2_11_1",
             "value": "69%",
-            "x1": 1066,
-            "x2": 1156,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 710,
+            "x2": 771,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_11_2_0",
             "page": 1,
             "parent": "line_2_11_2",
             "value": "13/14",
-            "x1": 1376,
-            "x2": 1496,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 917,
+            "x2": 997,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_11_2_1",
             "page": 1,
             "parent": "line_2_11_2",
             "value": "=",
-            "x1": 1506,
-            "x2": 1536,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 1004,
+            "x2": 1024,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_11_2_2",
             "page": 1,
             "parent": "line_2_11_2",
             "value": "93%",
-            "x1": 1547,
-            "x2": 1637,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 1031,
+            "x2": 1092,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_11_3_0",
             "page": 1,
             "parent": "line_2_11_3",
             "value": "7/12",
-            "x1": 1844,
-            "x2": 1938,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 1230,
+            "x2": 1292,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_11_3_1",
             "page": 1,
             "parent": "line_2_11_3",
             "value": "=",
-            "x1": 1949,
-            "x2": 1979,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 1299,
+            "x2": 1319,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_11_3_2",
             "page": 1,
             "parent": "line_2_11_3",
             "value": "58%",
-            "x1": 1989,
-            "x2": 2080,
-            "y1": 1273,
-            "y2": 1334
+            "x1": 1326,
+            "x2": 1387,
+            "y1": 849,
+            "y2": 889
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_12_0_0",
             "page": 1,
             "parent": "line_2_12_0",
             "value": "+1tsp",
-            "x1": 377,
-            "x2": 497,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 251,
+            "x2": 332,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_12_0_1",
             "page": 1,
             "parent": "line_2_12_0",
             "value": "milk",
-            "x1": 508,
-            "x2": 597,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 339,
+            "x2": 398,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_12_0_2",
             "page": 1,
             "parent": "line_2_12_0",
             "value": "+",
-            "x1": 607,
-            "x2": 637,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 405,
+            "x2": 425,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_12_0_3",
             "page": 1,
             "parent": "line_2_12_0",
             "value": "tea",
-            "x1": 648,
-            "x2": 713,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 432,
+            "x2": 475,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_12_1_0",
             "page": 1,
             "parent": "line_2_12_1",
             "value": "7/13",
-            "x1": 920,
-            "x2": 1015,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 614,
+            "x2": 676,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_12_1_1",
             "page": 1,
             "parent": "line_2_12_1",
             "value": "=",
-            "x1": 1025,
-            "x2": 1055,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 683,
+            "x2": 703,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_12_1_2",
             "page": 1,
             "parent": "line_2_12_1",
             "value": "54%",
-            "x1": 1066,
-            "x2": 1156,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 710,
+            "x2": 771,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_12_2_0",
             "page": 1,
             "parent": "line_2_12_2",
             "value": "9/14",
-            "x1": 1389,
-            "x2": 1483,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 926,
+            "x2": 988,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_12_2_1",
             "page": 1,
             "parent": "line_2_12_2",
             "value": "=",
-            "x1": 1493,
-            "x2": 1523,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 996,
+            "x2": 1015,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_12_2_2",
             "page": 1,
             "parent": "line_2_12_2",
             "value": "69%",
-            "x1": 1534,
-            "x2": 1625,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 1022,
+            "x2": 1083,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_12_3_0",
             "page": 1,
             "parent": "line_2_12_3",
             "value": "9/12",
-            "x1": 1844,
-            "x2": 1938,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 1230,
+            "x2": 1292,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_12_3_1",
             "page": 1,
             "parent": "line_2_12_3",
             "value": "=",
-            "x1": 1949,
-            "x2": 1979,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 1299,
+            "x2": 1319,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_12_3_2",
             "page": 1,
             "parent": "line_2_12_3",
             "value": "75%",
-            "x1": 1989,
-            "x2": 2080,
-            "y1": 1365,
-            "y2": 1425
+            "x1": 1326,
+            "x2": 1387,
+            "y1": 910,
+            "y2": 950
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_14_0_0",
             "page": 1,
             "parent": "line_2_14_0",
             "value": "Example",
-            "x1": 732,
-            "x2": 949,
-            "y1": 1577,
-            "y2": 1649
+            "x1": 488,
+            "x2": 633,
+            "y1": 1051,
+            "y2": 1099
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_14_0_1",
             "page": 1,
             "parent": "line_2_14_0",
             "value": "of",
-            "x1": 960,
-            "x2": 1012,
-            "y1": 1577,
-            "y2": 1649
+            "x1": 640,
+            "x2": 675,
+            "y1": 1051,
+            "y2": 1099
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_14_0_2",
             "page": 1,
             "parent": "line_2_14_0",
             "value": "Measuring",
-            "x1": 1023,
-            "x2": 1291,
-            "y1": 1577,
-            "y2": 1649
+            "x1": 682,
+            "x2": 861,
+            "y1": 1051,
+            "y2": 1099
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_14_0_3",
             "page": 1,
             "parent": "line_2_14_0",
             "value": "Ocean",
-            "x1": 1302,
-            "x2": 1463,
-            "y1": 1577,
-            "y2": 1649
+            "x1": 868,
+            "x2": 975,
+            "y1": 1051,
+            "y2": 1099
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_14_0_4",
             "page": 1,
             "parent": "line_2_14_0",
             "value": "Color",
-            "x1": 1474,
-            "x2": 1610,
-            "y1": 1577,
-            "y2": 1649
+            "x1": 983,
+            "x2": 1073,
+            "y1": 1051,
+            "y2": 1099
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_14_0_5",
             "page": 1,
             "parent": "line_2_14_0",
             "value": "Graph",
-            "x1": 1621,
-            "x2": 1780,
-            "y1": 1577,
-            "y2": 1649
+            "x1": 1081,
+            "x2": 1186,
+            "y1": 1051,
+            "y2": 1099
         },
         {
             "class": "ocrx_word",
             "confidence": 99,
             "id": "word_2_14_0_6",
             "page": 1,
             "parent": "line_2_14_0",
             "value": "2",
-            "x1": 1790,
-            "x2": 1822,
-            "y1": 1577,
-            "y2": 1649
+            "x1": 1194,
+            "x2": 1215,
+            "y1": 1051,
+            "y2": 1099
         }
     ]
 ]
```

### Comparing `img2table-0.0.24/tests/ocr/pdf/test_data/test.pdf` & `img2table-0.1.0/tests/ocr/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/pdf/test_pdf_ocr.py` & `img2table-0.1.0/tests/ocr/pdf/test_pdf_ocr.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from img2table.document.pdf import PDF
 from img2table.ocr.data import OCRDataframe
 from img2table.ocr.pdf import PdfOCR
 
 
 def test_pdf_content(mock_tesseract):
     instance = PdfOCR()
-    doc = PDF(src="test_data/test.pdf", dpi=300)
+    doc = PDF(src="test_data/test.pdf")
 
     result = instance.content(document=doc)
 
     with open("test_data/content.json", "r") as f:
         expected = json.load(f)
 
     assert result == expected
@@ -32,15 +32,15 @@
     expected = OCRDataframe(df=df_expected)
 
     assert result == expected
 
 
 def test_pdf_document():
     instance = PdfOCR()
-    doc = PDF(src="test_data/test.pdf", dpi=300)
+    doc = PDF(src="test_data/test.pdf")
 
     result = instance.of(document=doc)
 
     df_expected = pl.read_csv("test_data/ocr_df.csv", separator=";").lazy()
     expected = OCRDataframe(df=df_expected)
 
     assert result == expected
```

### Comparing `img2table-0.0.24/tests/ocr/tesseract/test_data/ocr_df.csv` & `img2table-0.1.0/tests/ocr/tesseract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/tesseract/test_data/test.png` & `img2table-0.1.0/tests/ocr/tesseract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/ocr/tesseract/test_tesseract.py` & `img2table-0.1.0/tests/ocr/tesseract/test_tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/image/test_data/expected_tables.json` & `img2table-0.1.0/tests/tables/image/test_data/expected_tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/image/test_data/ocr.csv` & `img2table-0.1.0/tests/tables/image/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/image/test_data/test.png` & `img2table-0.1.0/tests/tables/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/image/test_image.py` & `img2table-0.1.0/tests/tables/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/objects/test_data/expected_tables.json` & `img2table-0.1.0/tests/tables/objects/test_data/expected_tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/objects/test_data/ocr.csv` & `img2table-0.1.0/tests/tables/objects/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/objects/test_data/tables.json` & `img2table-0.1.0/tests/tables/objects/test_data/tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/objects/test_extraction.py` & `img2table-0.1.0/tests/tables/objects/test_extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/objects/test_line.py` & `img2table-0.1.0/tests/tables/objects/test_line.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/objects/test_row.py` & `img2table-0.1.0/tests/tables/objects/test_row.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/objects/test_table.py` & `img2table-0.1.0/tests/tables/objects/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_cells.py` & `img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/expected.csv` & `img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/expected.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_data/lines.json` & `img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py` & `img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/cells/test_identification_cells.py` & `img2table-0.1.0/tests/tables/processing/bordered_tables/cells/test_identification_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_data/expected.json` & `img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_data/test.png` & `img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/lines/test_lines.py` & `img2table-0.1.0/tests/tables/processing/bordered_tables/lines/test_lines.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # coding: utf-8
 import json
 
 import cv2
-import polars as pl
 
-from img2table.ocr.data import OCRDataframe
+from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.line import Line
 from img2table.tables.processing.bordered_tables.lines import overlapping_filter, detect_lines, remove_word_lines
 
 
 def test_overlapping_filter():
     # Create lines
     lines = [Line(x1=10, x2=10, y1=10, y2=100),
@@ -22,33 +21,36 @@
                 Line(x1=12, x2=12, y1=210, y2=255, thickness=1),
                 Line(x1=20, x2=20, y1=10, y2=100, thickness=1)]
 
     assert result == expected
 
 
 def test_remove_word_lines():
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr.csv", separator=";").lazy())
+    with open("test_data/contours.json", "r") as f:
+        contours = [Cell(**el) for el in json.load(f)]
     lines = [Line(x1=10, x2=10, y1=10, y2=100),
              Line(x1=975, x2=975, y1=40, y2=60)]
 
-    result = remove_word_lines(lines=lines, ocr_df=ocr_df)
+    result = remove_word_lines(lines=lines, contours=contours)
 
     assert result == [Line(x1=10, x2=10, y1=10, y2=100)]
 
 
 def test_detect_lines():
     img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr.csv", separator=";").lazy())
+    with open("test_data/contours.json", "r") as f:
+        contours = [Cell(**el) for el in json.load(f)]
 
     h_lines, v_lines = detect_lines(image=img,
                                     rho=0.3,
                                     threshold=10,
                                     minLinLength=10,
                                     maxLineGap=10,
-                                    ocr_df=ocr_df)
+                                    contours=contours,
+                                    char_length=8.44)
 
     with open("test_data/expected.json", 'r') as f:
         data = json.load(f)
     h_lines_expected = [Line(**el) for el in data.get('h_lines')]
     v_lines_expected = [Line(**el) for el in data.get('v_lines')]
 
     assert (h_lines, v_lines) == (h_lines_expected, v_lines_expected)
```

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py` & `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json` & `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/cells.json` & `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/cells.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json` & `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/expected.json` & `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json` & `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_data/word_image.png` & `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_data/word_image.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py` & `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,34 @@
 # coding: utf-8
 import json
 
 import cv2
-import numpy as np
-import polars as pl
 
-from img2table.ocr.data import OCRDataframe
 from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.row import Row
 from img2table.tables.objects.table import Table
-from img2table.tables.processing.bordered_tables.tables.implicit_rows import create_word_image, \
-    handle_implicit_rows_table, handle_implicit_rows
-
-
-def test_create_word_image():
-    img = cv2.imread("test_data/implicit.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/implicit_ocr_df.csv", separator=";").lazy())
-
-    result = create_word_image(img=img, ocr_df=ocr_df)
-
-    expected = cv2.imread("test_data/word_image.png", cv2.IMREAD_GRAYSCALE)
-
-    assert np.array_equal(result, expected)
+from img2table.tables.processing.bordered_tables.tables.implicit_rows import handle_implicit_rows_table, \
+    handle_implicit_rows
 
 
 def test_handle_implicit_rows_table():
-    img = cv2.imread("test_data/word_image.png", cv2.IMREAD_GRAYSCALE)
+    img = cv2.imread("test_data/implicit.png", cv2.IMREAD_GRAYSCALE)
 
     with open("test_data/implicit_table.json", 'r') as f:
         table = Table(rows=[Row(cells=[Cell(**el) for el in row]) for row in json.load(f)])
 
     result = handle_implicit_rows_table(img=img, table=table)
 
     # Check that 2 more lines have been created
     assert result.nb_rows == table.nb_rows + 2
 
 
 def test_handle_implicit_rows():
     img = cv2.imread("test_data/implicit.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/implicit_ocr_df.csv", separator=";").lazy())
 
     with open("test_data/implicit_table.json", 'r') as f:
         table = Table(rows=[Row(cells=[Cell(**el) for el in row]) for row in json.load(f)])
 
-    result = handle_implicit_rows(img=img, tables=[table], ocr_df=ocr_df)
+    result = handle_implicit_rows(img=img, tables=[table])
 
     # Check that 2 more lines have been created
     assert result[0].nb_rows == table.nb_rows + 2
```

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_table_creation.py` & `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/bordered_tables/tables/test_tables.py` & `img2table-0.1.0/tests/tables/processing/bordered_tables/tables/test_tables.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py` & `img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # coding: utf-8
 import json
 
 import cv2
-import polars as pl
 
-from img2table.ocr.data import OCRDataframe
 from img2table.tables.objects.line import Line
 from img2table.tables.processing.borderless_tables import identify_borderless_tables
 
 
 def test_identify_borderless_tables():
     img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     with open("test_data/lines.json", 'r') as f:
         data = json.load(f)
     lines = [Line(**el) for el in data.get('h_lines') + data.get('v_lines')]
 
     result = identify_borderless_tables(img=img,
-                                        ocr_df=ocr_df,
+                                        char_length=8.44,
+                                        median_line_sep=51,
                                         lines=lines,
                                         existing_tables=[])
 
     assert len(result) == 2
     assert (result[0].nb_columns, result[0].nb_rows) == (3, 6)
     assert (result[1].nb_columns, result[1].nb_rows) == (2, 2)
```

### Comparing `img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json` & `img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png` & `img2table-0.1.0/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py` & `img2table-0.1.0/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json` & `img2table-0.1.0/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/borderless_tables/lines/test_lines.py` & `img2table-0.1.0/tests/tables/processing/borderless_tables/lines/test_lines.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # coding: utf-8
 
 import json
 
-import polars as pl
-
-from img2table.ocr.data import OCRDataframe
 from img2table.tables.objects.cell import Cell
 from img2table.tables.processing.borderless_tables.lines import identify_lines, create_h_pos_groups, \
     vertically_coherent_groups, is_text_block, identify_line_groups
 from img2table.tables.processing.borderless_tables.model import ImageSegment, TableLine, LineGroup
 
 
 def test_identify_lines():
@@ -63,38 +60,35 @@
                          TableLine(cells=[Cell(x1=0, x2=20, y1=63, y2=73), Cell(x1=20, x2=40, y1=63, y2=73)])])
     ]
 
     assert result == expected
 
 
 def test_is_text_block():
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
-
     line_group = LineGroup(lines=[TableLine(cells=[Cell(x1=0, x2=20, y1=0, y2=10), Cell(x1=20, x2=40, y1=0, y2=10)]),
                                   TableLine(cells=[Cell(x1=0, x2=20, y1=13, y2=23), Cell(x1=20, x2=40, y1=13, y2=23)])])
-    assert is_text_block(line_group=line_group, ocr_df=ocr_df)
+    assert is_text_block(line_group=line_group, char_length=8.44)
 
     line_group = LineGroup(lines=[TableLine(cells=[Cell(x1=0, x2=20, y1=0, y2=10), Cell(x1=40, x2=60, y1=0, y2=10)]),
                                   TableLine(cells=[Cell(x1=0, x2=20, y1=13, y2=23), Cell(x1=40, x2=60, y1=13, y2=23)])])
-    assert not is_text_block(line_group=line_group, ocr_df=ocr_df)
+    assert not is_text_block(line_group=line_group, char_length=8.44)
 
 
 def test_identify_line_groups():
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
-
     with open("test_data/image_segment.json", "r") as f:
         data = json.load(f)
     img_segment = ImageSegment(x1=data.get('x1'),
                                y1=data.get('y1'),
                                x2=data.get('x2'),
                                y2=data.get('y2'),
                                elements=[Cell(**c) for c in data.get('elements')])
 
     result = identify_line_groups(segment=img_segment,
-                                  ocr_df=ocr_df)
+                                  median_line_sep=51,
+                                  char_length=8.44)
 
     assert isinstance(result, ImageSegment)
     assert result.x1 == img_segment.x1
     assert result.y1 == img_segment.y1
     assert result.x2 == img_segment.x2
     assert result.y2 == img_segment.y2
     assert result.elements == img_segment.elements
```

### Comparing `img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json` & `img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_data/test.png` & `img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py` & `img2table-0.1.0/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 # coding: utf-8
 import json
 
 import cv2
-import polars as pl
 
-from img2table.ocr.data import OCRDataframe
 from img2table.tables.objects.line import Line
 from img2table.tables.processing.borderless_tables.model import ImageSegment
 from img2table.tables.processing.borderless_tables.segment_image import create_image_segments, get_segment_elements, \
     segment_image
 
 
 def test_create_image_segments():
     img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
-    result = create_image_segments(img=img, ocr_df=ocr_df)
+    result = create_image_segments(img=img, median_line_sep=51)
 
-    assert result == [ImageSegment(x1=2, y1=0, x2=804, y2=361), ImageSegment(x1=928, y1=0, x2=1188, y2=157)]
+    assert set(result) == {ImageSegment(x1=2, y1=0, x2=804, y2=361), ImageSegment(x1=928, y1=0, x2=1188, y2=157)}
 
 
 def test_get_segment_elements():
     img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
     img_segments = [ImageSegment(x1=2, y1=0, x2=804, y2=361),
                     ImageSegment(x1=928, y1=0, x2=1188, y2=157)]
 
     with open("test_data/lines.json", 'r') as f:
         data = json.load(f)
     lines = [Line(**el) for el in data.get('h_lines') + data.get('v_lines')]
 
     result = get_segment_elements(img=img,
                                   lines=lines,
                                   img_segments=img_segments,
                                   blur_size=3,
-                                  ocr_df=ocr_df)
+                                  char_length=8.44,
+                                  median_line_sep=51)
 
     assert len(result[0].elements) == 14
     assert len(result[1].elements) == 4
 
 
 def test_segment_image():
     img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
     with open("test_data/lines.json", 'r') as f:
         data = json.load(f)
     lines = [Line(**el) for el in data.get('h_lines') + data.get('v_lines')]
 
     result = segment_image(img=img,
-                           ocr_df=ocr_df,
+                           char_length=8.44,
+                           median_line_sep=51,
                            lines=lines)
 
-    assert len(result[0].elements) == 14
-    assert len(result[1].elements) == 4
+    assert {len(result[0].elements), len(result[1].elements)} == {14, 4}
```

### Comparing `img2table-0.0.24/tests/tables/processing/borderless_tables/table/test_headers.py` & `img2table-0.1.0/tests/tables/processing/borderless_tables/table/test_headers.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/borderless_tables/table/test_table.py` & `img2table-0.1.0/tests/tables/processing/borderless_tables/table/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/borderless_tables/table/test_table_creation.py` & `img2table-0.1.0/tests/tables/processing/borderless_tables/table/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/common/test_common.py` & `img2table-0.1.0/tests/tables/processing/common/test_common.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/common/test_data/test.jpg` & `img2table-0.1.0/tests/tables/processing/common/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/prepare_image/test_data/test.png` & `img2table-0.1.0/tests/tables/processing/prepare_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/text/test_data/ocr.csv` & `img2table-0.1.0/tests/tables/processing/text/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/text/test_data/table.json` & `img2table-0.1.0/tests/tables/processing/text/test_data/table.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/text/test_data/test.jpg` & `img2table-0.1.0/tests/tables/processing/text/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.24/tests/tables/processing/text/test_titles.py` & `img2table-0.1.0/tests/tables/processing/text/test_titles.py`

 * *Files identical despite different names*

