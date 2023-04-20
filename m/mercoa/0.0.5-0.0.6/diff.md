# Comparing `tmp/mercoa-0.0.5.tar.gz` & `tmp/mercoa-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercoa-0.0.5.tar", max compression
+gzip compressed data, was "mercoa-0.0.6.tar", max compression
```

## Comparing `mercoa-0.0.5.tar` & `mercoa-0.0.6.tar`

### file list

```diff
@@ -1,124 +1,126 @@
--rw-r--r--   0        0        0      410 2023-04-12 20:57:21.026861 mercoa-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4245 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/__init__.py
--rw-r--r--   0        0        0     4216 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/client.py
--rw-r--r--   0        0        0      348 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/core/__init__.py
--rw-r--r--   0        0        0      326 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      157 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/environment.py
--rw-r--r--   0        0        0        0 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/py.typed
--rw-r--r--   0        0        0     4354 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/__init__.py
--rw-r--r--   0        0        0      165 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/bank_lookup/__init__.py
--rw-r--r--   0        0        0     2582 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/bank_lookup/client.py
--rw-r--r--   0        0        0      205 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/bank_lookup/types/__init__.py
--rw-r--r--   0        0        0      960 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/bank_lookup/types/bank_address.py
--rw-r--r--   0        0        0      946 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
--rw-r--r--   0        0        0      359 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/commons/__init__.py
--rw-r--r--   0        0        0      148 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      216 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/commons/errors/unauthorized_error.py
--rw-r--r--   0        0        0      407 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/commons/types/address.py
--rw-r--r--   0        0        0      824 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/commons/types/birth_date.py
--rw-r--r--   0        0        0      994 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/commons/types/full_name.py
--rw-r--r--   0        0        0      850 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/commons/types/individual_government_id.py
--rw-r--r--   0        0        0      857 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/commons/types/itin.py
--rw-r--r--   0        0        0      855 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      856 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/commons/types/ssn.py
--rw-r--r--   0        0        0      141 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/counterparty/__init__.py
--rw-r--r--   0        0        0     4542 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/counterparty/client.py
--rw-r--r--   0        0        0      157 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/counterparty/types/__init__.py
--rw-r--r--   0        0        0     1022 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/counterparty/types/counterparty_response.py
--rw-r--r--   0        0        0      753 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/__init__.py
--rw-r--r--   0        0        0    16466 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/client.py
--rw-r--r--   0        0        0     1104 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/__init__.py
--rw-r--r--   0        0        0      487 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/account_type.py
--rw-r--r--   0        0        0     1535 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/business_profile_request.py
--rw-r--r--   0        0        0     1492 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/business_profile_response.py
--rw-r--r--   0        0        0     1917 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/business_type.py
--rw-r--r--   0        0        0      741 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/ein.py
--rw-r--r--   0        0        0       80 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/entity_id.py
--rw-r--r--   0        0        0     1262 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/entity_request.py
--rw-r--r--   0        0        0     1497 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/entity_response.py
--rw-r--r--   0        0        0     1084 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/entity_status.py
--rw-r--r--   0        0        0     1302 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/entity_update_request.py
--rw-r--r--   0        0        0     1372 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/individual_profile_request.py
--rw-r--r--   0        0        0     1206 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/individual_profile_response.py
--rw-r--r--   0        0        0      974 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/profile_request.py
--rw-r--r--   0        0        0      981 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/profile_response.py
--rw-r--r--   0        0        0      761 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/entity/types/tax_id.py
--rw-r--r--   0        0        0      459 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/invoice/__init__.py
--rw-r--r--   0        0        0    12453 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/invoice/client.py
--rw-r--r--   0        0        0      639 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/invoice/types/__init__.py
--rw-r--r--   0        0        0     1048 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/invoice/types/create_vendor_request.py
--rw-r--r--   0        0        0      955 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/invoice/types/document_response.py
--rw-r--r--   0        0        0       81 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/invoice/types/invoice_id.py
--rw-r--r--   0        0        0     2721 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/invoice/types/invoice_request.py
--rw-r--r--   0        0        0     2717 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/invoice/types/invoice_response.py
--rw-r--r--   0        0        0     1332 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/invoice/types/invoice_status.py
--rw-r--r--   0        0        0     1060 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/invoice/types/transaction_response.py
--rw-r--r--   0        0        0     1261 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/invoice/types/transaction_status.py
--rw-r--r--   0        0        0      213 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/ocr/__init__.py
--rw-r--r--   0        0        0     4443 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/ocr/client.py
--rw-r--r--   0        0        0      298 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/ocr/types/__init__.py
--rw-r--r--   0        0        0     1068 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/ocr/types/attachments.py
--rw-r--r--   0        0        0     1969 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/ocr/types/email_ocr_request.py
--rw-r--r--   0        0        0      891 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/ocr/types/ocr_mailbox.py
--rw-r--r--   0        0        0     1234 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/ocr/types/ocr_response.py
--rw-r--r--   0        0        0      881 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/__init__.py
--rw-r--r--   0        0        0     7158 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/client.py
--rw-r--r--   0        0        0     1305 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/__init__.py
--rw-r--r--   0        0        0      981 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/email_log_response.py
--rw-r--r--   0        0        0      932 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/email_provider_request.py
--rw-r--r--   0        0        0      936 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/email_provider_response.py
--rw-r--r--   0        0        0      656 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/email_sender_provider.py
--rw-r--r--   0        0        0     1052 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/email_sender_request.py
--rw-r--r--   0        0        0     1044 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/email_sender_response.py
--rw-r--r--   0        0        0       86 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/organization_id.py
--rw-r--r--   0        0        0     1318 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/organization_request.py
--rw-r--r--   0        0        0     1431 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/organization_response.py
--rw-r--r--   0        0        0     1142 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/payment_methods_request.py
--rw-r--r--   0        0        0     1148 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/payment_methods_response.py
--rw-r--r--   0        0        0      849 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/payment_rail_markup.py
--rw-r--r--   0        0        0      482 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/payment_rail_markup_type.py
--rw-r--r--   0        0        0     1009 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/payment_rail_request.py
--rw-r--r--   0        0        0      797 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/organization/types/payment_rail_response.py
--rw-r--r--   0        0        0      943 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/__init__.py
--rw-r--r--   0        0        0    12242 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/client.py
--rw-r--r--   0        0        0     1411 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/__init__.py
--rw-r--r--   0        0        0       85 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/bank_account_id.py
--rw-r--r--   0        0        0     1147 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/bank_account_request.py
--rw-r--r--   0        0        0     1318 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/bank_account_response.py
--rw-r--r--   0        0        0      960 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/bank_status.py
--rw-r--r--   0        0        0      632 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/bank_type.py
--rw-r--r--   0        0        0      819 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/card_brand.py
--rw-r--r--   0        0        0       78 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/card_id.py
--rw-r--r--   0        0        0     1120 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/card_request.py
--rw-r--r--   0        0        0     1217 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/card_response.py
--rw-r--r--   0        0        0      750 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/card_type.py
--rw-r--r--   0        0        0       79 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/check_id.py
--rw-r--r--   0        0        0     1152 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/check_request.py
--rw-r--r--   0        0        0     1327 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/check_response.py
--rw-r--r--   0        0        0       80 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/custom_id.py
--rw-r--r--   0        0        0     1568 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
--rw-r--r--   0        0        0     1922 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
--rw-r--r--   0        0        0       87 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/payment_method_id.py
--rw-r--r--   0        0        0     1296 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/payment_method_request.py
--rw-r--r--   0        0        0     1508 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/payment_method_response.py
--rw-r--r--   0        0        0     1229 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method/types/payment_method_type.py
--rw-r--r--   0        0        0      425 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method_schema/__init__.py
--rw-r--r--   0        0        0     6115 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method_schema/client.py
--rw-r--r--   0        0        0      589 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method_schema/types/__init__.py
--rw-r--r--   0        0        0     1160 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
--rw-r--r--   0        0        0      682 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
--rw-r--r--   0        0        0       93 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method_schema/types/payment_method_schema_id.py
--rw-r--r--   0        0        0     1249 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
--rw-r--r--   0        0        0     1468 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
--rw-r--r--   0        0        0      269 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/representative/__init__.py
--rw-r--r--   0        0        0     8182 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/representative/client.py
--rw-r--r--   0        0        0      381 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/representative/types/__init__.py
--rw-r--r--   0        0        0       88 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/representative/types/representative_id.py
--rw-r--r--   0        0        0     1370 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/representative/types/representative_request.py
--rw-r--r--   0        0        0     1539 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/representative/types/representative_response.py
--rw-r--r--   0        0        0     1100 2023-04-12 20:57:21.026861 mercoa-0.0.5/src/mercoa/resources/representative/types/responsibilities.py
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 mercoa-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      410 2023-04-20 17:45:56.381406 mercoa-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4363 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/__init__.py
+-rw-r--r--   0        0        0     4216 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/client.py
+-rw-r--r--   0        0        0      348 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/core/__init__.py
+-rw-r--r--   0        0        0      326 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      157 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/environment.py
+-rw-r--r--   0        0        0        0 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/py.typed
+-rw-r--r--   0        0        0     4472 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/__init__.py
+-rw-r--r--   0        0        0      165 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/bank_lookup/__init__.py
+-rw-r--r--   0        0        0     2582 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/bank_lookup/client.py
+-rw-r--r--   0        0        0      205 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/bank_lookup/types/__init__.py
+-rw-r--r--   0        0        0      960 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/bank_lookup/types/bank_address.py
+-rw-r--r--   0        0        0      946 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
+-rw-r--r--   0        0        0      359 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/__init__.py
+-rw-r--r--   0        0        0      148 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      216 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      407 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1093 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/address.py
+-rw-r--r--   0        0        0      824 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/birth_date.py
+-rw-r--r--   0        0        0      994 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/full_name.py
+-rw-r--r--   0        0        0      850 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/individual_government_id.py
+-rw-r--r--   0        0        0      857 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/itin.py
+-rw-r--r--   0        0        0      855 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      856 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/commons/types/ssn.py
+-rw-r--r--   0        0        0      141 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/counterparty/__init__.py
+-rw-r--r--   0        0        0     4542 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/counterparty/client.py
+-rw-r--r--   0        0        0      157 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/counterparty/types/__init__.py
+-rw-r--r--   0        0        0     1022 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/counterparty/types/counterparty_response.py
+-rw-r--r--   0        0        0      753 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/__init__.py
+-rw-r--r--   0        0        0    16466 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/client.py
+-rw-r--r--   0        0        0     1104 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/__init__.py
+-rw-r--r--   0        0        0      487 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/account_type.py
+-rw-r--r--   0        0        0     1535 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/business_profile_request.py
+-rw-r--r--   0        0        0     1492 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/business_profile_response.py
+-rw-r--r--   0        0        0     1917 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/business_type.py
+-rw-r--r--   0        0        0      741 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/ein.py
+-rw-r--r--   0        0        0       80 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/entity_id.py
+-rw-r--r--   0        0        0     1262 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/entity_request.py
+-rw-r--r--   0        0        0     1497 2023-04-20 17:45:56.381406 mercoa-0.0.6/src/mercoa/resources/entity/types/entity_response.py
+-rw-r--r--   0        0        0     1084 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/entity/types/entity_status.py
+-rw-r--r--   0        0        0     1302 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/entity/types/entity_update_request.py
+-rw-r--r--   0        0        0     1372 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/entity/types/individual_profile_request.py
+-rw-r--r--   0        0        0     1206 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/entity/types/individual_profile_response.py
+-rw-r--r--   0        0        0      974 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/entity/types/profile_request.py
+-rw-r--r--   0        0        0      981 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/entity/types/profile_response.py
+-rw-r--r--   0        0        0      761 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/entity/types/tax_id.py
+-rw-r--r--   0        0        0      577 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    12453 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/client.py
+-rw-r--r--   0        0        0      826 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/__init__.py
+-rw-r--r--   0        0        0     1048 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/create_vendor_request.py
+-rw-r--r--   0        0        0      955 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/document_response.py
+-rw-r--r--   0        0        0       81 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_id.py
+-rw-r--r--   0        0        0     1255 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0     1182 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_line_item_response.py
+-rw-r--r--   0        0        0     3076 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_request.py
+-rw-r--r--   0        0        0     3075 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_response.py
+-rw-r--r--   0        0        0     1332 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_status.py
+-rw-r--r--   0        0        0     1060 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/transaction_response.py
+-rw-r--r--   0        0        0     1261 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/invoice/types/transaction_status.py
+-rw-r--r--   0        0        0      213 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/ocr/__init__.py
+-rw-r--r--   0        0        0     4443 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/ocr/client.py
+-rw-r--r--   0        0        0      298 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/ocr/types/__init__.py
+-rw-r--r--   0        0        0     1068 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/ocr/types/attachments.py
+-rw-r--r--   0        0        0     1969 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/ocr/types/email_ocr_request.py
+-rw-r--r--   0        0        0      891 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/ocr/types/ocr_mailbox.py
+-rw-r--r--   0        0        0     1234 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/ocr/types/ocr_response.py
+-rw-r--r--   0        0        0      881 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/__init__.py
+-rw-r--r--   0        0        0     7158 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/client.py
+-rw-r--r--   0        0        0     1305 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/__init__.py
+-rw-r--r--   0        0        0      981 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/email_log_response.py
+-rw-r--r--   0        0        0      932 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/email_provider_request.py
+-rw-r--r--   0        0        0      936 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/email_provider_response.py
+-rw-r--r--   0        0        0      656 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/email_sender_provider.py
+-rw-r--r--   0        0        0     1052 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/email_sender_request.py
+-rw-r--r--   0        0        0     1044 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/email_sender_response.py
+-rw-r--r--   0        0        0       86 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/organization_id.py
+-rw-r--r--   0        0        0     1318 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/organization_request.py
+-rw-r--r--   0        0        0     1431 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/organization_response.py
+-rw-r--r--   0        0        0     1142 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/payment_methods_request.py
+-rw-r--r--   0        0        0     1148 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/payment_methods_response.py
+-rw-r--r--   0        0        0      849 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/payment_rail_markup.py
+-rw-r--r--   0        0        0      482 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/payment_rail_markup_type.py
+-rw-r--r--   0        0        0     1009 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/payment_rail_request.py
+-rw-r--r--   0        0        0      797 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/organization/types/payment_rail_response.py
+-rw-r--r--   0        0        0      943 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/__init__.py
+-rw-r--r--   0        0        0    12242 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/client.py
+-rw-r--r--   0        0        0     1411 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_account_id.py
+-rw-r--r--   0        0        0     1147 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_account_request.py
+-rw-r--r--   0        0        0     1318 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_account_response.py
+-rw-r--r--   0        0        0      960 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_status.py
+-rw-r--r--   0        0        0      632 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_type.py
+-rw-r--r--   0        0        0      819 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_brand.py
+-rw-r--r--   0        0        0       78 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_id.py
+-rw-r--r--   0        0        0     1120 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_request.py
+-rw-r--r--   0        0        0     1217 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_response.py
+-rw-r--r--   0        0        0      750 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_type.py
+-rw-r--r--   0        0        0       79 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/check_id.py
+-rw-r--r--   0        0        0     1152 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/check_request.py
+-rw-r--r--   0        0        0     1327 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/check_response.py
+-rw-r--r--   0        0        0       80 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/custom_id.py
+-rw-r--r--   0        0        0     1568 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
+-rw-r--r--   0        0        0     1922 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
+-rw-r--r--   0        0        0       87 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/payment_method_id.py
+-rw-r--r--   0        0        0     1296 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/payment_method_request.py
+-rw-r--r--   0        0        0     1508 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/payment_method_response.py
+-rw-r--r--   0        0        0     1229 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method/types/payment_method_type.py
+-rw-r--r--   0        0        0      425 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/__init__.py
+-rw-r--r--   0        0        0     6115 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/client.py
+-rw-r--r--   0        0        0      589 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/__init__.py
+-rw-r--r--   0        0        0     1160 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
+-rw-r--r--   0        0        0      682 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
+-rw-r--r--   0        0        0       93 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_id.py
+-rw-r--r--   0        0        0     1249 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
+-rw-r--r--   0        0        0     1468 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
+-rw-r--r--   0        0        0      269 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/representative/__init__.py
+-rw-r--r--   0        0        0     8182 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/representative/client.py
+-rw-r--r--   0        0        0      381 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/representative/types/__init__.py
+-rw-r--r--   0        0        0       88 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/representative/types/representative_id.py
+-rw-r--r--   0        0        0     1370 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/representative/types/representative_request.py
+-rw-r--r--   0        0        0     1539 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/representative/types/representative_response.py
+-rw-r--r--   0        0        0     1100 2023-04-20 17:45:56.385406 mercoa-0.0.6/src/mercoa/resources/representative/types/responsibilities.py
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 mercoa-0.0.6/PKG-INFO
```

### Comparing `mercoa-0.0.5/src/mercoa/__init__.py` & `mercoa-0.0.6/src/mercoa/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,16 @@
     EntityStatus,
     EntityUpdateRequest,
     FullName,
     IndividualGovernmentID,
     IndividualProfileRequest,
     IndividualProfileResponse,
     InvoiceId,
+    InvoiceLineItemRequest,
+    InvoiceLineItemResponse,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
     OcrMailbox,
     OCRResponse,
     OrganizationId,
     OrganizationRequest,
@@ -140,14 +142,16 @@
     "EntityUpdateRequest",
     "FullName",
     "ITIN",
     "IndividualGovernmentID",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
     "InvoiceId",
+    "InvoiceLineItemRequest",
+    "InvoiceLineItemResponse",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
     "MercoaEnvironment",
     "OCRResponse",
     "OcrMailbox",
     "OrganizationId",
```

### Comparing `mercoa-0.0.5/src/mercoa/client.py` & `mercoa-0.0.6/src/mercoa/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/core/datetime_utils.py` & `mercoa-0.0.6/src/mercoa/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/core/jsonable_encoder.py` & `mercoa-0.0.6/src/mercoa/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/__init__.py` & `mercoa-0.0.6/src/mercoa/resources/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     ProfileResponse,
     TaxID,
 )
 from .invoice import (
     CreateVendorRequest,
     DocumentResponse,
     InvoiceId,
+    InvoiceLineItemRequest,
+    InvoiceLineItemResponse,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
     TransactionResponse,
     TransactionStatus,
 )
 from .ocr import Attachments, EmailOcrRequest, OcrMailbox, OCRResponse
@@ -135,14 +137,16 @@
     "EntityUpdateRequest",
     "FullName",
     "ITIN",
     "IndividualGovernmentID",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
     "InvoiceId",
+    "InvoiceLineItemRequest",
+    "InvoiceLineItemResponse",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
     "OCRResponse",
     "OcrMailbox",
     "OrganizationId",
     "OrganizationRequest",
```

### Comparing `mercoa-0.0.5/src/mercoa/resources/bank_lookup/client.py` & `mercoa-0.0.6/src/mercoa/resources/bank_lookup/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/bank_lookup/types/bank_address.py` & `mercoa-0.0.6/src/mercoa/resources/bank_lookup/types/bank_address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py` & `mercoa-0.0.6/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/commons/types/address.py` & `mercoa-0.0.6/src/mercoa/resources/commons/types/address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/commons/types/birth_date.py` & `mercoa-0.0.6/src/mercoa/resources/commons/types/birth_date.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/commons/types/full_name.py` & `mercoa-0.0.6/src/mercoa/resources/commons/types/full_name.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/commons/types/individual_government_id.py` & `mercoa-0.0.6/src/mercoa/resources/commons/types/individual_government_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/commons/types/itin.py` & `mercoa-0.0.6/src/mercoa/resources/commons/types/itin.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/commons/types/phone_number.py` & `mercoa-0.0.6/src/mercoa/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/commons/types/ssn.py` & `mercoa-0.0.6/src/mercoa/resources/commons/types/ssn.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/counterparty/client.py` & `mercoa-0.0.6/src/mercoa/resources/counterparty/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/counterparty/types/counterparty_response.py` & `mercoa-0.0.6/src/mercoa/resources/counterparty/types/counterparty_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/__init__.py` & `mercoa-0.0.6/src/mercoa/resources/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/client.py` & `mercoa-0.0.6/src/mercoa/resources/entity/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/types/__init__.py` & `mercoa-0.0.6/src/mercoa/resources/entity/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/types/business_profile_request.py` & `mercoa-0.0.6/src/mercoa/resources/entity/types/business_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/types/business_profile_response.py` & `mercoa-0.0.6/src/mercoa/resources/entity/types/business_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/types/business_type.py` & `mercoa-0.0.6/src/mercoa/resources/entity/types/business_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/types/ein.py` & `mercoa-0.0.6/src/mercoa/resources/entity/types/ein.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/types/entity_request.py` & `mercoa-0.0.6/src/mercoa/resources/entity/types/entity_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/types/entity_response.py` & `mercoa-0.0.6/src/mercoa/resources/entity/types/entity_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/types/entity_status.py` & `mercoa-0.0.6/src/mercoa/resources/entity/types/entity_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/types/entity_update_request.py` & `mercoa-0.0.6/src/mercoa/resources/entity/types/entity_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/types/individual_profile_request.py` & `mercoa-0.0.6/src/mercoa/resources/entity/types/individual_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/types/individual_profile_response.py` & `mercoa-0.0.6/src/mercoa/resources/entity/types/individual_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/types/profile_request.py` & `mercoa-0.0.6/src/mercoa/resources/entity/types/profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/types/profile_response.py` & `mercoa-0.0.6/src/mercoa/resources/entity/types/profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/entity/types/tax_id.py` & `mercoa-0.0.6/src/mercoa/resources/entity/types/tax_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/invoice/client.py` & `mercoa-0.0.6/src/mercoa/resources/invoice/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/invoice/types/__init__.py` & `mercoa-0.0.6/src/mercoa/resources/invoice/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .create_vendor_request import CreateVendorRequest
-from .document_response import DocumentResponse
-from .invoice_id import InvoiceId
-from .invoice_request import InvoiceRequest
-from .invoice_response import InvoiceResponse
-from .invoice_status import InvoiceStatus
-from .transaction_response import TransactionResponse
-from .transaction_status import TransactionStatus
+from .types import (
+    CreateVendorRequest,
+    DocumentResponse,
+    InvoiceId,
+    InvoiceLineItemRequest,
+    InvoiceLineItemResponse,
+    InvoiceRequest,
+    InvoiceResponse,
+    InvoiceStatus,
+    TransactionResponse,
+    TransactionStatus,
+)
 
 __all__ = [
     "CreateVendorRequest",
     "DocumentResponse",
     "InvoiceId",
+    "InvoiceLineItemRequest",
+    "InvoiceLineItemResponse",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
     "TransactionResponse",
     "TransactionStatus",
 ]
```

### Comparing `mercoa-0.0.5/src/mercoa/resources/invoice/types/create_vendor_request.py` & `mercoa-0.0.6/src/mercoa/resources/invoice/types/create_vendor_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/invoice/types/document_response.py` & `mercoa-0.0.6/src/mercoa/resources/invoice/types/document_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/invoice/types/invoice_request.py` & `mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from ...entity.types.entity_id import EntityId
 from ...payment_method.types.payment_method_id import PaymentMethodId
 from .create_vendor_request import CreateVendorRequest
+from .invoice_line_item_request import InvoiceLineItemRequest
 from .invoice_status import InvoiceStatus
 
 
 class InvoiceRequest(pydantic.BaseModel):
     status: typing.Optional[InvoiceStatus]
     amount: typing.Optional[float]
     currency: typing.Optional[str]
     deduction_date: typing.Optional[dt.datetime] = pydantic.Field(alias="deductionDate")
     funded_date: typing.Optional[dt.datetime] = pydantic.Field(alias="fundedDate")
     due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate")
     invoice_number: typing.Optional[str] = pydantic.Field(alias="invoiceNumber")
     note_to_self: typing.Optional[str] = pydantic.Field(alias="noteToSelf")
+    service_start_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceStartDate")
+    service_end_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceEndDate")
     payer_id: typing.Optional[EntityId] = pydantic.Field(alias="payerId")
     payment_source_id: typing.Optional[PaymentMethodId] = pydantic.Field(alias="paymentSourceId")
     vendor_id: typing.Optional[EntityId] = pydantic.Field(alias="vendorId")
     payment_destination_id: typing.Optional[PaymentMethodId] = pydantic.Field(alias="paymentDestinationId")
     create_vendor: typing.Optional[CreateVendorRequest] = pydantic.Field(
         alias="createVendor",
         description=(
@@ -33,14 +36,15 @@
     )
     update_vendor: typing.Optional[CreateVendorRequest] = pydantic.Field(
         alias="updateVendor",
         description=(
             "When paying to an existing vendor with an incomplete profile, use the updateVendor object. Mercoa will update the vendor entity tied to this invoice. This object is ignored if the vendor already has already been created with complete information and when creating a new invoice.\n"
         ),
     )
+    line_items: typing.Optional[typing.List[InvoiceLineItemRequest]] = pydantic.Field(alias="lineItems")
     uploaded_image: typing.Optional[str] = pydantic.Field(alias="uploadedImage")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mercoa-0.0.5/src/mercoa/resources/invoice/types/invoice_response.py` & `mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,38 +7,42 @@
 
 from ....core.datetime_utils import serialize_datetime
 from ...entity.types.entity_id import EntityId
 from ...entity.types.entity_response import EntityResponse
 from ...payment_method.types.payment_method_id import PaymentMethodId
 from ...payment_method.types.payment_method_response import PaymentMethodResponse
 from .invoice_id import InvoiceId
+from .invoice_line_item_response import InvoiceLineItemResponse
 from .invoice_status import InvoiceStatus
 from .transaction_response import TransactionResponse
 
 
 class InvoiceResponse(pydantic.BaseModel):
     id: InvoiceId
     status: InvoiceStatus
     amount: typing.Optional[float]
     currency: typing.Optional[str]
     deduction_date: typing.Optional[dt.datetime] = pydantic.Field(alias="deductionDate")
     funded_date: typing.Optional[dt.datetime] = pydantic.Field(alias="fundedDate")
     due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate")
     invoice_number: typing.Optional[str] = pydantic.Field(alias="invoiceNumber")
     note_to_self: typing.Optional[str] = pydantic.Field(alias="noteToSelf")
+    service_start_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceStartDate")
+    service_end_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceEndDate")
     payer_id: typing.Optional[EntityId] = pydantic.Field(alias="payerId")
     payer: typing.Optional[EntityResponse]
     payment_source: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentSource")
     payment_source_id: typing.Optional[PaymentMethodId] = pydantic.Field(alias="paymentSourceId")
     vendor_id: typing.Optional[EntityId] = pydantic.Field(alias="vendorId")
     vendor: typing.Optional[EntityResponse]
     payment_destination: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentDestination")
     payment_destination_id: typing.Optional[PaymentMethodId] = pydantic.Field(alias="paymentDestinationId")
     payment_destination_confirmed: bool = pydantic.Field(alias="paymentDestinationConfirmed")
     transactions: typing.Optional[typing.List[TransactionResponse]]
+    line_items: typing.Optional[typing.List[InvoiceLineItemResponse]] = pydantic.Field(alias="lineItems")
     processed_at: typing.Optional[dt.datetime] = pydantic.Field(alias="processedAt")
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.0.5/src/mercoa/resources/invoice/types/invoice_status.py` & `mercoa-0.0.6/src/mercoa/resources/invoice/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/invoice/types/transaction_response.py` & `mercoa-0.0.6/src/mercoa/resources/invoice/types/transaction_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/invoice/types/transaction_status.py` & `mercoa-0.0.6/src/mercoa/resources/invoice/types/transaction_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/ocr/client.py` & `mercoa-0.0.6/src/mercoa/resources/ocr/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/ocr/types/attachments.py` & `mercoa-0.0.6/src/mercoa/resources/ocr/types/attachments.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/ocr/types/email_ocr_request.py` & `mercoa-0.0.6/src/mercoa/resources/ocr/types/email_ocr_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/ocr/types/ocr_mailbox.py` & `mercoa-0.0.6/src/mercoa/resources/ocr/types/ocr_mailbox.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/ocr/types/ocr_response.py` & `mercoa-0.0.6/src/mercoa/resources/ocr/types/ocr_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/__init__.py` & `mercoa-0.0.6/src/mercoa/resources/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/client.py` & `mercoa-0.0.6/src/mercoa/resources/organization/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/types/__init__.py` & `mercoa-0.0.6/src/mercoa/resources/organization/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/types/email_log_response.py` & `mercoa-0.0.6/src/mercoa/resources/organization/types/email_log_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/types/email_provider_request.py` & `mercoa-0.0.6/src/mercoa/resources/organization/types/email_provider_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/types/email_provider_response.py` & `mercoa-0.0.6/src/mercoa/resources/organization/types/email_provider_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/types/email_sender_provider.py` & `mercoa-0.0.6/src/mercoa/resources/organization/types/email_sender_provider.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/types/email_sender_request.py` & `mercoa-0.0.6/src/mercoa/resources/organization/types/email_sender_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/types/email_sender_response.py` & `mercoa-0.0.6/src/mercoa/resources/organization/types/email_sender_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/types/organization_request.py` & `mercoa-0.0.6/src/mercoa/resources/organization/types/organization_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/types/organization_response.py` & `mercoa-0.0.6/src/mercoa/resources/organization/types/organization_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/types/payment_methods_request.py` & `mercoa-0.0.6/src/mercoa/resources/organization/types/payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/types/payment_methods_response.py` & `mercoa-0.0.6/src/mercoa/resources/organization/types/payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/types/payment_rail_markup.py` & `mercoa-0.0.6/src/mercoa/resources/organization/types/payment_rail_markup.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/types/payment_rail_request.py` & `mercoa-0.0.6/src/mercoa/resources/organization/types/payment_rail_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/organization/types/payment_rail_response.py` & `mercoa-0.0.6/src/mercoa/resources/organization/types/payment_rail_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/__init__.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/client.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/__init__.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/bank_account_request.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_account_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/bank_account_response.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_account_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/bank_status.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/bank_type.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/bank_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/card_brand.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/card_request.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/card_response.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/card_type.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/card_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/check_request.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/check_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/check_response.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/check_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/custom_payment_method_request.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/custom_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/custom_payment_method_response.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/custom_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/payment_method_request.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/payment_method_response.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method/types/payment_method_type.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method/types/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method_schema/client.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method_schema/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method_schema/types/__init__.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py` & `mercoa-0.0.6/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/representative/client.py` & `mercoa-0.0.6/src/mercoa/resources/representative/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/representative/types/representative_request.py` & `mercoa-0.0.6/src/mercoa/resources/representative/types/representative_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/representative/types/representative_response.py` & `mercoa-0.0.6/src/mercoa/resources/representative/types/representative_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/src/mercoa/resources/representative/types/responsibilities.py` & `mercoa-0.0.6/src/mercoa/resources/representative/types/responsibilities.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.5/PKG-INFO` & `mercoa-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercoa
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

