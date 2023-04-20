# Comparing `tmp/mindee-3.7.0.tar.gz` & `tmp/mindee-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindee-3.7.0.tar", last modified: Tue Apr 18 16:25:36 2023, max compression
+gzip compressed data, was "mindee-3.7.1.tar", last modified: Thu Apr 20 15:50:58 2023, max compression
```

## Comparing `mindee-3.7.0.tar` & `mindee-3.7.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.375078 mindee-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-18 16:25:16.000000 mindee-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-18 16:25:36.375078 mindee-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-18 16:25:16.000000 mindee-3.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.343078 mindee-3.7.0/mindee/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.347078 mindee-3.7.0/mindee/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.347078 mindee-3.7.0/mindee/documents/cropper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/cropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/cropper/cropper_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.347078 mindee-3.7.0/mindee/documents/custom/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/custom/custom_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.347078 mindee-3.7.0/mindee/documents/eu/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/eu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.351078 mindee-3.7.0/mindee/documents/eu/license_plate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/eu/license_plate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/eu/license_plate/license_plate_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.351078 mindee-3.7.0/mindee/documents/financial/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/financial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/financial/financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/financial/financial_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.351078 mindee-3.7.0/mindee/documents/fr/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.351078 mindee-3.7.0/mindee/documents/fr/bank_account_details/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/bank_account_details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/bank_account_details/bank_account_details_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.351078 mindee-3.7.0/mindee/documents/fr/carte_grise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/carte_grise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/carte_grise/carte_grise_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.351078 mindee-3.7.0/mindee/documents/fr/carte_vitale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/carte_vitale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/carte_vitale/carte_vitale_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.355078 mindee-3.7.0/mindee/documents/fr/id_card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/id_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/id_card/id_card_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.355078 mindee-3.7.0/mindee/documents/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/invoice/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/invoice/invoice_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/invoice/invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/invoice/line_item_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/invoice/reconstruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.355078 mindee-3.7.0/mindee/documents/passport/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/passport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/passport/passport_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.355078 mindee-3.7.0/mindee/documents/proof_of_address/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/proof_of_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/proof_of_address/proof_of_address_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.359078 mindee-3.7.0/mindee/documents/receipt/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/receipt/line_item_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/receipt/receipt_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/receipt/receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/receipt/receipt_v5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.359078 mindee-3.7.0/mindee/documents/shipping_container/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/shipping_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/shipping_container/shipping_container_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.359078 mindee-3.7.0/mindee/documents/us/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/us/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.359078 mindee-3.7.0/mindee/documents/us/bank_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/us/bank_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/us/bank_check/bank_check_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.363078 mindee-3.7.0/mindee/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/api_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/company_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/payment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/tax.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.363078 mindee-3.7.0/mindee/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/input/page_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/input/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/response.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/version
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.347078 mindee-3.7.0/mindee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-18 16:25:36.000000 mindee-3.7.0/mindee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-18 16:25:36.000000 mindee-3.7.0/mindee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:25:36.000000 mindee-3.7.0/mindee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 16:25:36.000000 mindee-3.7.0/mindee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:25:20.000000 mindee-3.7.0/mindee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-18 16:25:36.000000 mindee-3.7.0/mindee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 16:25:36.000000 mindee-3.7.0/mindee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-18 16:25:16.000000 mindee-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-18 16:25:36.375078 mindee-3.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 16:25:16.000000 mindee-3.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.367078 mindee-3.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.371078 mindee-3.7.0/tests/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.371078 mindee-3.7.0/tests/documents/fr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/fr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/fr/test_bank_account_details_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/fr/test_carte_grise_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/fr/test_carte_vitale_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/fr/test_id_card_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_cropper_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_custom_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_financial_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_invoice_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_passport_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_proof_of_address_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_receipt_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_receipt_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_shipping_container_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.371078 mindee-3.7.0/tests/documents/us/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/us/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/us/test_bank_check_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.375078 mindee-3.7.0/tests/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_amount.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_payment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/test_pkg_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.204862 mindee-3.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 15:50:35.000000 mindee-3.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-20 15:50:58.204862 mindee-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-20 15:50:35.000000 mindee-3.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/cropper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/cropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/cropper/cropper_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/custom/custom_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/eu/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/eu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/eu/license_plate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/eu/license_plate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/eu/license_plate/license_plate_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/financial/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/financial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/financial/financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/financial/financial_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/fr/bank_account_details/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/bank_account_details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/bank_account_details/bank_account_details_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/fr/carte_grise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/carte_grise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/carte_grise/carte_grise_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.184860 mindee-3.7.1/mindee/documents/fr/carte_vitale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/carte_vitale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/carte_vitale/carte_vitale_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.184860 mindee-3.7.1/mindee/documents/fr/id_card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/id_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/id_card/id_card_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.184860 mindee-3.7.1/mindee/documents/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/invoice/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/invoice/invoice_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/invoice/invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/invoice/line_item_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/invoice/reconstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.184860 mindee-3.7.1/mindee/documents/passport/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/passport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/passport/passport_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.184860 mindee-3.7.1/mindee/documents/proof_of_address/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/proof_of_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/proof_of_address/proof_of_address_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.188861 mindee-3.7.1/mindee/documents/receipt/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/receipt/line_item_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/receipt/receipt_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/receipt/receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/receipt/receipt_v5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.188861 mindee-3.7.1/mindee/documents/shipping_container/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/shipping_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/shipping_container/shipping_container_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.188861 mindee-3.7.1/mindee/documents/us/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/us/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.188861 mindee-3.7.1/mindee/documents/us/bank_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/us/bank_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/us/bank_check/bank_check_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.192861 mindee-3.7.1/mindee/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/api_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/company_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.192861 mindee-3.7.1/mindee/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/input/page_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/input/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/version
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-20 15:50:58.000000 mindee-3.7.1/mindee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-20 15:50:58.000000 mindee-3.7.1/mindee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:50:58.000000 mindee-3.7.1/mindee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 15:50:58.000000 mindee-3.7.1/mindee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:50:39.000000 mindee-3.7.1/mindee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 15:50:58.000000 mindee-3.7.1/mindee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 15:50:58.000000 mindee-3.7.1/mindee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-20 15:50:35.000000 mindee-3.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-20 15:50:58.204862 mindee-3.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-20 15:50:35.000000 mindee-3.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.196861 mindee-3.7.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.200862 mindee-3.7.1/tests/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.200862 mindee-3.7.1/tests/documents/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/fr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/fr/test_bank_account_details_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/fr/test_carte_grise_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/fr/test_carte_vitale_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/fr/test_id_card_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_cropper_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_custom_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_financial_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_invoice_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_passport_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_proof_of_address_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_receipt_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_shipping_container_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.200862 mindee-3.7.1/tests/documents/us/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/us/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/us/test_bank_check_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.204862 mindee-3.7.1/tests/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/test_pkg_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/test_response.py
```

### Comparing `mindee-3.7.0/LICENSE` & `mindee-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/PKG-INFO` & `mindee-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 3.7.0
+Version: 3.7.1
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: devrel@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-3.7.0/README.md` & `mindee-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/cli.py` & `mindee-3.7.1/mindee/cli.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/client.py` & `mindee-3.7.1/mindee/client.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/__init__.py` & `mindee-3.7.1/mindee/documents/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from mindee.documents import fr, us
+from mindee.documents import eu, fr, us
 from mindee.documents.cropper import CropperV1, TypeCropperV1
 from mindee.documents.custom import CustomV1, TypeCustomV1
-from mindee.documents.eu import LicensePlateV1, TypeLicensePlateV1
 from mindee.documents.financial import (
     FinancialDocumentV1,
     FinancialV1,
     TypeFinancialDocumentV1,
     TypeFinancialV1,
 )
 from mindee.documents.invoice import InvoiceV3, InvoiceV4, TypeInvoiceV3, TypeInvoiceV4
```

### Comparing `mindee-3.7.0/mindee/documents/base.py` & `mindee-3.7.1/mindee/documents/base.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/config.py` & `mindee-3.7.1/mindee/documents/config.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/cropper/cropper_v1.py` & `mindee-3.7.1/mindee/documents/cropper/cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/custom/custom_v1.py` & `mindee-3.7.1/mindee/documents/custom/custom_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/eu/license_plate/license_plate_v1.py` & `mindee-3.7.1/mindee/documents/eu/license_plate/license_plate_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/financial/financial_document_v1.py` & `mindee-3.7.1/mindee/documents/financial/financial_document_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/financial/financial_v1.py` & `mindee-3.7.1/mindee/documents/financial/financial_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/fr/bank_account_details/bank_account_details_v1.py` & `mindee-3.7.1/mindee/documents/fr/bank_account_details/bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/fr/carte_grise/carte_grise_v1.py` & `mindee-3.7.1/mindee/documents/fr/carte_grise/carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/fr/carte_vitale/carte_vitale_v1.py` & `mindee-3.7.1/mindee/documents/fr/carte_vitale/carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/fr/id_card/id_card_v1.py` & `mindee-3.7.1/mindee/documents/fr/id_card/id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/invoice/checks.py` & `mindee-3.7.1/mindee/documents/invoice/checks.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/invoice/invoice_v3.py` & `mindee-3.7.1/mindee/documents/invoice/invoice_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/invoice/invoice_v4.py` & `mindee-3.7.1/mindee/documents/invoice/invoice_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/invoice/line_item_v4.py` & `mindee-3.7.1/mindee/documents/invoice/line_item_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/invoice/reconstruct.py` & `mindee-3.7.1/mindee/documents/invoice/reconstruct.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/passport/passport_v1.py` & `mindee-3.7.1/mindee/documents/passport/passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/proof_of_address/proof_of_address_v1.py` & `mindee-3.7.1/mindee/documents/proof_of_address/proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/receipt/line_item_v5.py` & `mindee-3.7.1/mindee/documents/receipt/line_item_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/receipt/receipt_v3.py` & `mindee-3.7.1/mindee/documents/receipt/receipt_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/receipt/receipt_v4.py` & `mindee-3.7.1/mindee/documents/receipt/receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/receipt/receipt_v5.py` & `mindee-3.7.1/mindee/documents/receipt/receipt_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/shipping_container/shipping_container_v1.py` & `mindee-3.7.1/mindee/documents/shipping_container/shipping_container_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/documents/us/bank_check/bank_check_v1.py` & `mindee-3.7.1/mindee/documents/us/bank_check/bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/endpoints.py` & `mindee-3.7.1/mindee/endpoints.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/fields/amount.py` & `mindee-3.7.1/mindee/fields/amount.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/fields/api_builder.py` & `mindee-3.7.1/mindee/fields/api_builder.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/fields/base.py` & `mindee-3.7.1/mindee/fields/base.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/fields/company_registration.py` & `mindee-3.7.1/mindee/fields/company_registration.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/fields/date.py` & `mindee-3.7.1/mindee/fields/date.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/fields/locale.py` & `mindee-3.7.1/mindee/fields/locale.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/fields/orientation.py` & `mindee-3.7.1/mindee/fields/orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/fields/payment_details.py` & `mindee-3.7.1/mindee/fields/payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/fields/position.py` & `mindee-3.7.1/mindee/fields/position.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/fields/tax.py` & `mindee-3.7.1/mindee/fields/tax.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/fields/text.py` & `mindee-3.7.1/mindee/fields/text.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/geometry.py` & `mindee-3.7.1/mindee/geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/input/page_options.py` & `mindee-3.7.1/mindee/input/page_options.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/input/sources.py` & `mindee-3.7.1/mindee/input/sources.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/response.py` & `mindee-3.7.1/mindee/response.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee/versions.py` & `mindee-3.7.1/mindee/versions.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/mindee.egg-info/PKG-INFO` & `mindee-3.7.1/mindee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 3.7.0
+Version: 3.7.1
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: devrel@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-3.7.0/mindee.egg-info/SOURCES.txt` & `mindee-3.7.1/mindee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/pyproject.toml` & `mindee-3.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/setup.cfg` & `mindee-3.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/documents/fr/test_bank_account_details_v1.py` & `mindee-3.7.1/tests/documents/fr/test_bank_account_details_v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.fr.bank_account_details.bank_account_details_v1 import (
-    BankAccountDetailsV1,
-)
+from mindee.documents.fr import BankAccountDetailsV1
 
 FR_BANK_ACCOUNT_DETAILS_DATA_DIR = "./tests/data/fr/bank_account_details"
 
 FILE_PATH_FR_BANK_ACCOUNT_DETAILS_V1_COMPLETE = (
     f"{ FR_BANK_ACCOUNT_DETAILS_DATA_DIR }/response_v1/complete.json"
 )
 FILE_PATH_FR_BANK_ACCOUNT_DETAILS_V1_EMPTY = (
```

### Comparing `mindee-3.7.0/tests/documents/fr/test_carte_grise_v1.py` & `mindee-3.7.1/tests/documents/fr/test_carte_grise_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.fr.carte_grise.carte_grise_v1 import CarteGriseV1
+from mindee.documents.fr import CarteGriseV1
 from tests import FR_CARTE_GRISE_DATA_DIR
 
 FILE_PATH_FR_CARTE_GRISE_V1_COMPLETE = (
     f"{FR_CARTE_GRISE_DATA_DIR}/response_v1/complete.json"
 )
 FILE_PATH_FR_CARTE_GRISE_V1_EMPTY = f"{FR_CARTE_GRISE_DATA_DIR}/response_v1/empty.json"
```

### Comparing `mindee-3.7.0/tests/documents/fr/test_carte_vitale_v1.py` & `mindee-3.7.1/tests/documents/fr/test_carte_vitale_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.fr.carte_vitale.carte_vitale_v1 import CarteVitaleV1
+from mindee.documents.fr import CarteVitaleV1
 
 FR_CARTE_VITALE_DATA_DIR = "./tests/data/fr/carte_vitale"
 
 FILE_PATH_FR_CARTE_VITALE_V1_COMPLETE = (
     f"{ FR_CARTE_VITALE_DATA_DIR }/response_v1/complete.json"
 )
 FILE_PATH_FR_CARTE_VITALE_V1_EMPTY = (
```

### Comparing `mindee-3.7.0/tests/documents/fr/test_id_card_v1.py` & `mindee-3.7.1/tests/documents/fr/test_id_card_v1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.fr.id_card.id_card_v1 import IdCardV1
+from mindee.documents.fr import IdCardV1
 
 FR_ID_CARD_DATA_DIR = "./tests/data/fr/id_card"
 
 FILE_PATH_FR_ID_CARD_V1_COMPLETE = f"{ FR_ID_CARD_DATA_DIR }/response_v1/complete.json"
 FILE_PATH_FR_ID_CARD_V1_EMPTY = f"{ FR_ID_CARD_DATA_DIR }/response_v1/empty.json"
```

### Comparing `mindee-3.7.0/tests/documents/test_cropper_v1.py` & `mindee-3.7.1/tests/documents/test_cropper_v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.cropper.cropper_v1 import CropperV1
+from mindee.documents import CropperV1
 from tests import CROPPER_DATA_DIR
 
 FILE_PATH_CROPPER_V1_COMPLETE = f"{CROPPER_DATA_DIR}/response_v1/complete.json"
 FILE_PATH_CROPPER_V1_EMPTY = f"{CROPPER_DATA_DIR}/response_v1/empty.json"
 
 
 @pytest.fixture
```

### Comparing `mindee-3.7.0/tests/documents/test_custom_v1.py` & `mindee-3.7.1/tests/documents/test_custom_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.custom.custom_v1 import CustomV1
+from mindee.documents import CustomV1
 from mindee.fields.api_builder import ClassificationField, ListField, ListFieldValue
 from tests import CUSTOM_DATA_DIR
 
 FILE_PATH_CUSTOM_V1_COMPLETE = f"{CUSTOM_DATA_DIR}/response_v1/complete.json"
 FILE_PATH_CUSTOM_V1_EMPTY = f"{CUSTOM_DATA_DIR}/response_v1/empty.json"
```

### Comparing `mindee-3.7.0/tests/documents/test_financial_document_v1.py` & `mindee-3.7.1/tests/documents/test_financial_document_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.financial.financial_document_v1 import FinancialDocumentV1
+from mindee.documents import FinancialDocumentV1
 from tests import FINANCIAL_DOC_DATA_DIR
 
 FILE_PATH_FINANCIAL_DOC_V1_INVOICE = (
     f"{FINANCIAL_DOC_DATA_DIR}/response_v1/complete_invoice.json"
 )
 FILE_PATH_FINANCIAL_DOC_V1_RECEIPT = (
     f"{FINANCIAL_DOC_DATA_DIR}/response_v1/complete_receipt.json"
```

### Comparing `mindee-3.7.0/tests/documents/test_financial_v1.py` & `mindee-3.7.1/tests/documents/test_financial_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.financial.financial_v1 import FinancialV1
+from mindee.documents import FinancialV1
 from tests.documents.test_invoice_v3 import (
     FILE_PATH_INVOICE_V3_COMPLETE,
     FILE_PATH_INVOICE_V3_EMPTY,
 )
 from tests.documents.test_receipt_v3 import (
     FILE_PATH_RECEIPT_V3_COMPLETE,
     FILE_PATH_RECEIPT_V3_EMPTY,
```

### Comparing `mindee-3.7.0/tests/documents/test_invoice_v3.py` & `mindee-3.7.1/tests/documents/test_invoice_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/documents/test_invoice_v4.py` & `mindee-3.7.1/tests/documents/test_invoice_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/documents/test_passport_v1.py` & `mindee-3.7.1/tests/documents/test_passport_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.passport.passport_v1 import PassportV1
+from mindee.documents import PassportV1
 from tests import PASSPORT_DATA_DIR
 
 FILE_PATH_PASSPORT_V1_COMPLETE = f"{PASSPORT_DATA_DIR}/response_v1/complete.json"
 
 
 @pytest.fixture
 def passport_v1_doc_object():
```

### Comparing `mindee-3.7.0/tests/documents/test_proof_of_address_v1.py` & `mindee-3.7.1/tests/documents/test_proof_of_address_v1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.proof_of_address.proof_of_address_v1 import ProofOfAddressV1
+from mindee.documents import ProofOfAddressV1
 
 PROOF_OF_ADDRESS_DATA_DIR = "./tests/data/proof_of_address"
 
 FILE_PATH_PROOF_OF_ADDRESS_V1_COMPLETE = (
     f"{ PROOF_OF_ADDRESS_DATA_DIR }/response_v1/complete.json"
 )
 FILE_PATH_PROOF_OF_ADDRESS_V1_EMPTY = (
```

### Comparing `mindee-3.7.0/tests/documents/test_receipt_v3.py` & `mindee-3.7.1/tests/documents/test_receipt_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.receipt.receipt_v3 import ReceiptV3
+from mindee.documents import ReceiptV3
 from tests import RECEIPT_DATA_DIR
 
 FILE_PATH_RECEIPT_V3_COMPLETE = f"{RECEIPT_DATA_DIR}/response_v3/complete.json"
 FILE_PATH_RECEIPT_V3_EMPTY = f"{RECEIPT_DATA_DIR}/response_v3/empty.json"
 
 
 @pytest.fixture
```

### Comparing `mindee-3.7.0/tests/documents/test_receipt_v4.py` & `mindee-3.7.1/tests/documents/test_receipt_v4.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.receipt.receipt_v4 import ReceiptV4
+from mindee.documents import ReceiptV4
 from tests import RECEIPT_DATA_DIR
 
 FILE_PATH_RECEIPT_V4_COMPLETE = f"{RECEIPT_DATA_DIR}/response_v4/complete.json"
 FILE_PATH_RECEIPT_V4_EMPTY = f"{RECEIPT_DATA_DIR}/response_v4/empty.json"
 
 
 @pytest.fixture
```

### Comparing `mindee-3.7.0/tests/documents/test_receipt_v5.py` & `mindee-3.7.1/tests/documents/test_receipt_v5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.receipt.receipt_v5 import ReceiptV5
+from mindee.documents import ReceiptV5
 from tests import RECEIPT_DATA_DIR
 
 FILE_PATH_RECEIPT_V5_COMPLETE = f"{RECEIPT_DATA_DIR}/response_v5/complete.json"
 FILE_PATH_RECEIPT_V5_EMPTY = f"{RECEIPT_DATA_DIR}/response_v5/empty.json"
 
 
 @pytest.fixture
```

### Comparing `mindee-3.7.0/tests/documents/test_shipping_container_v1.py` & `mindee-3.7.1/tests/documents/test_shipping_container_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.shipping_container.shipping_container_v1 import (
-    ShippingContainerV1,
-)
+from mindee.documents import ShippingContainerV1
 
 SHIPPING_CONTAINER_DATA_DIR = "./tests/data/shipping_container"
 
 FILE_PATH_SHIPPING_CONTAINER_V1_COMPLETE = (
     f"{ SHIPPING_CONTAINER_DATA_DIR }/response_v1/complete.json"
 )
 FILE_PATH_SHIPPING_CONTAINER_V1_EMPTY = (
```

### Comparing `mindee-3.7.0/tests/documents/us/test_bank_check_v1.py` & `mindee-3.7.1/tests/documents/us/test_bank_check_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from mindee.documents.us.bank_check.bank_check_v1 import BankCheckV1
+from mindee.documents.us import BankCheckV1
 from tests import US_BANK_CHECK_DATA_DIR
 
 FILE_PATH_US_BANK_CHECK_V1_COMPLETE = (
     f"{US_BANK_CHECK_DATA_DIR}/response_v1/complete.json"
 )
 FILE_PATH_US_BANK_CHECK_V1_EMPTY = f"{US_BANK_CHECK_DATA_DIR}/response_v1/empty.json"
```

### Comparing `mindee-3.7.0/tests/fields/test_amount.py` & `mindee-3.7.1/tests/fields/test_amount.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/fields/test_date.py` & `mindee-3.7.1/tests/fields/test_date.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/fields/test_field.py` & `mindee-3.7.1/tests/fields/test_field.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/fields/test_locale.py` & `mindee-3.7.1/tests/fields/test_locale.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/fields/test_orientation.py` & `mindee-3.7.1/tests/fields/test_orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/fields/test_payment_details.py` & `mindee-3.7.1/tests/fields/test_payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/fields/test_position.py` & `mindee-3.7.1/tests/fields/test_position.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/fields/test_tax.py` & `mindee-3.7.1/tests/fields/test_tax.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/test_cli.py` & `mindee-3.7.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/test_client.py` & `mindee-3.7.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/test_geometry.py` & `mindee-3.7.1/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/test_inputs.py` & `mindee-3.7.1/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/test_pkg_versions.py` & `mindee-3.7.1/tests/test_pkg_versions.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.0/tests/test_response.py` & `mindee-3.7.1/tests/test_response.py`

 * *Files identical despite different names*

