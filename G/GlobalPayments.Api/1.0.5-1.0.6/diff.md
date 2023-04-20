# Comparing `tmp/GlobalPayments.Api-1.0.5.tar.gz` & `tmp/GlobalPayments.Api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\GlobalPayments.Api-1.0.5.tar", last modified: Thu Apr 29 12:58:51 2021, max compression
+gzip compressed data, was "GlobalPayments.Api-1.0.6.tar", last modified: Thu Apr 20 12:36:27 2023, max compression
```

## Comparing `GlobalPayments.Api-1.0.5.tar` & `GlobalPayments.Api-1.0.6.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxrwx   0        0        0        0 2021-04-29 12:58:50.961867 GlobalPayments.Api-1.0.5/
-drwxrwxrwx   0        0        0        0 2021-04-29 12:58:49.242873 GlobalPayments.Api-1.0.5/GlobalPayments.Api.egg-info/
--rw-rw-rw-   0        0        0     1092 2021-04-29 12:58:47.000000 GlobalPayments.Api-1.0.5/GlobalPayments.Api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2774 2021-04-29 12:58:48.000000 GlobalPayments.Api-1.0.5/GlobalPayments.Api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-29 12:58:47.000000 GlobalPayments.Api-1.0.5/GlobalPayments.Api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2021-04-29 12:58:47.000000 GlobalPayments.Api-1.0.5/GlobalPayments.Api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2021-04-29 12:58:47.000000 GlobalPayments.Api-1.0.5/GlobalPayments.Api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2021-04-29 12:58:50.939885 GlobalPayments.Api-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      548 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/README.txt
-drwxrwxrwx   0        0        0        0 2021-04-29 12:58:49.272873 GlobalPayments.Api-1.0.5/globalpayments/
--rw-rw-rw-   0        0        0       36 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-29 12:58:49.302868 GlobalPayments.Api-1.0.5/globalpayments/api/
--rw-rw-rw-   0        0        0    10064 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-29 12:58:49.361868 GlobalPayments.Api-1.0.5/globalpayments/api/builders/
--rw-rw-rw-   0        0        0    13943 2021-03-26 14:40:54.000000 GlobalPayments.Api-1.0.5/globalpayments/api/builders/__init__.py
--rw-rw-rw-   0        0        0     2807 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/builders/management_builder.py
-drwxrwxrwx   0        0        0        0 2021-04-29 12:58:49.509868 GlobalPayments.Api-1.0.5/globalpayments/api/builders/validations/
--rw-rw-rw-   0        0        0      322 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/builders/validations/__init__.py
--rw-rw-rw-   0        0        0     2742 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/builders/validations/validation_clause.py
--rw-rw-rw-   0        0        0     1125 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/builders/validations/validation_target.py
--rw-rw-rw-   0        0        0     2194 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/builders/validations/validations.py
-drwxrwxrwx   0        0        0        0 2021-04-29 12:58:49.889870 GlobalPayments.Api-1.0.5/globalpayments/api/entities/
--rw-rw-rw-   0        0        0    15101 2021-04-29 12:52:33.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/__init__.py
--rw-rw-rw-   0        0        0    18729 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/address.py
--rw-rw-rw-   0        0        0      176 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/batch_summary.py
--rw-rw-rw-   0        0        0      244 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/debit_mac.py
--rw-rw-rw-   0        0        0      658 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/ecommerce_info.py
--rw-rw-rw-   0        0        0      601 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/encryption_data.py
--rw-rw-rw-   0        0        0    12685 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/enums.py
--rw-rw-rw-   0        0        0     1837 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/exceptions.py
--rw-rw-rw-   0        0        0      300 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/hosted_payment_data.py
-drwxrwxrwx   0        0        0        0 2021-04-29 12:58:50.137867 GlobalPayments.Api-1.0.5/globalpayments/api/entities/table_service/
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/table_service/__init__.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/table_service/base_table_service_response.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/table_service/bump_status_collection.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/table_service/login_response.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/table_service/server_assignment_response.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/table_service/server_list_response.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/table_service/shift_assignments.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/table_service/table_service_response.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/table_service/ticket.py
--rw-rw-rw-   0        0        0      211 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/three_d_secure.py
--rw-rw-rw-   0        0        0      640 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/entities/transaction_summary.py
-drwxrwxrwx   0        0        0        0 2021-04-29 12:58:50.244876 GlobalPayments.Api-1.0.5/globalpayments/api/gateways/
--rw-rw-rw-   0        0        0    98689 2021-04-29 12:52:33.000000 GlobalPayments.Api-1.0.5/globalpayments/api/gateways/__init__.py
--rw-rw-rw-   0        0        0       81 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/gateways/gateway_response.py
--rw-rw-rw-   0        0        0       48 2020-11-19 17:23:36.000000 GlobalPayments.Api-1.0.5/globalpayments/api/gateways/table_service_connector.py
-drwxrwxrwx   0        0        0        0 2021-04-29 12:58:50.525869 GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/
--rw-rw-rw-   0        0        0      583 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/__init__.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/cash.py
--rw-rw-rw-   0        0        0     7998 2021-04-13 01:20:30.000000 GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/credit.py
--rw-rw-rw-   0        0        0     2256 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/debit.py
--rw-rw-rw-   0        0        0     2202 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/ebt.py
--rw-rw-rw-   0        0        0     1259 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/echeck.py
--rw-rw-rw-   0        0        0     3302 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/giftcard.py
--rw-rw-rw-   0        0        0     1274 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/payment_interfaces.py
--rw-rw-rw-   0        0        0      173 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/transaction_reference.py
-drwxrwxrwx   0        0        0        0 2021-04-29 12:58:50.877869 GlobalPayments.Api-1.0.5/globalpayments/api/services/
--rw-rw-rw-   0        0        0      220 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/services/__init__.py
--rw-rw-rw-   0        0        0      354 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/services/batch_service.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/services/credit_service.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/services/debit_service.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/services/device_service.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/services/ebt_service.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/services/gift_service.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/services/hosted_service.py
--rw-rw-rw-   0        0        0     1127 2021-03-25 15:39:48.000000 GlobalPayments.Api-1.0.5/globalpayments/api/services/recurring_service.py
--rw-rw-rw-   0        0        0      589 2021-03-26 15:01:28.000000 GlobalPayments.Api-1.0.5/globalpayments/api/services/reporting_service.py
--rw-rw-rw-   0        0        0        0 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/services/table_service.py
-drwxrwxrwx   0        0        0        0 2021-04-29 12:58:50.898865 GlobalPayments.Api-1.0.5/globalpayments/api/utils/
--rw-rw-rw-   0        0        0     6127 2020-11-19 17:23:37.000000 GlobalPayments.Api-1.0.5/globalpayments/api/utils/__init__.py
--rw-rw-rw-   0        0        0       42 2021-04-29 12:58:50.963866 GlobalPayments.Api-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1159 2021-04-29 12:56:39.000000 GlobalPayments.Api-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.978104 GlobalPayments.Api-1.0.6/
+drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.664688 GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/
+-rw-rw-rw-   0        0        0      910 2023-04-20 12:36:26.000000 GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2785 2023-04-20 12:36:27.000000 GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 12:36:26.000000 GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-04-20 12:36:26.000000 GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-20 12:36:26.000000 GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    15439 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/LICENSE.md
+-rw-rw-rw-   0        0        0      910 2023-04-20 12:36:27.976103 GlobalPayments.Api-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.672671 GlobalPayments.Api-1.0.6/globalpayments/
+-rw-rw-rw-   0        0        0       36 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.678668 GlobalPayments.Api-1.0.6/globalpayments/api/
+-rw-rw-rw-   0        0        0    10064 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.694668 GlobalPayments.Api-1.0.6/globalpayments/api/builders/
+-rw-rw-rw-   0        0        0    13980 2023-04-13 15:28:43.000000 GlobalPayments.Api-1.0.6/globalpayments/api/builders/__init__.py
+-rw-rw-rw-   0        0        0     2807 2023-04-13 15:30:21.000000 GlobalPayments.Api-1.0.6/globalpayments/api/builders/management_builder.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.725690 GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/
+-rw-rw-rw-   0        0        0      322 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/__init__.py
+-rw-rw-rw-   0        0        0     2742 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/validation_clause.py
+-rw-rw-rw-   0        0        0     1125 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/validation_target.py
+-rw-rw-rw-   0        0        0     2194 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/validations.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.802850 GlobalPayments.Api-1.0.6/globalpayments/api/entities/
+-rw-rw-rw-   0        0        0    15101 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/__init__.py
+-rw-rw-rw-   0        0        0    18729 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/address.py
+-rw-rw-rw-   0        0        0      176 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/batch_summary.py
+-rw-rw-rw-   0        0        0      244 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/debit_mac.py
+-rw-rw-rw-   0        0        0      658 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/ecommerce_info.py
+-rw-rw-rw-   0        0        0      601 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/encryption_data.py
+-rw-rw-rw-   0        0        0    12813 2023-04-13 17:43:34.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/enums.py
+-rw-rw-rw-   0        0        0     1837 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/exceptions.py
+-rw-rw-rw-   0        0        0      300 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/hosted_payment_data.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.834811 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/base_table_service_response.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/bump_status_collection.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/login_response.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/server_assignment_response.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/server_list_response.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/shift_assignments.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/table_service_response.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/ticket.py
+-rw-rw-rw-   0        0        0      211 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/three_d_secure.py
+-rw-rw-rw-   0        0        0      640 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/transaction_summary.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.852836 GlobalPayments.Api-1.0.6/globalpayments/api/gateways/
+-rw-rw-rw-   0        0        0   100297 2023-04-14 18:53:27.000000 GlobalPayments.Api-1.0.6/globalpayments/api/gateways/__init__.py
+-rw-rw-rw-   0        0        0       81 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/gateways/gateway_response.py
+-rw-rw-rw-   0        0        0       48 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/gateways/table_service_connector.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.911812 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/
+-rw-rw-rw-   0        0        0      583 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/cash.py
+-rw-rw-rw-   0        0        0     8601 2023-04-14 18:52:05.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/credit.py
+-rw-rw-rw-   0        0        0     2256 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/debit.py
+-rw-rw-rw-   0        0        0     2202 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/ebt.py
+-rw-rw-rw-   0        0        0     1259 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/echeck.py
+-rw-rw-rw-   0        0        0     3302 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/giftcard.py
+-rw-rw-rw-   0        0        0     1274 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/payment_interfaces.py
+-rw-rw-rw-   0        0        0      173 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/transaction_reference.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.966110 GlobalPayments.Api-1.0.6/globalpayments/api/services/
+-rw-rw-rw-   0        0        0      220 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/__init__.py
+-rw-rw-rw-   0        0        0      354 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/batch_service.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/credit_service.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/debit_service.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/device_service.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/ebt_service.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/gift_service.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/hosted_service.py
+-rw-rw-rw-   0        0        0     1127 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/recurring_service.py
+-rw-rw-rw-   0        0        0      589 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/reporting_service.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/table_service.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.971143 GlobalPayments.Api-1.0.6/globalpayments/api/utils/
+-rw-rw-rw-   0        0        0     6127 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/utils/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 12:36:27.980104 GlobalPayments.Api-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1159 2023-04-20 12:32:44.000000 GlobalPayments.Api-1.0.6/setup.py
```

### Comparing `GlobalPayments.Api-1.0.5/GlobalPayments.Api.egg-info/SOURCES.txt` & `GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 README.txt
 setup.py
 GlobalPayments.Api.egg-info/PKG-INFO
 GlobalPayments.Api.egg-info/SOURCES.txt
 GlobalPayments.Api.egg-info/dependency_links.txt
 GlobalPayments.Api.egg-info/requires.txt
 GlobalPayments.Api.egg-info/top_level.txt
```

### Comparing `GlobalPayments.Api-1.0.5/README.txt` & `GlobalPayments.Api-1.0.6/README.txt`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/__init__.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/builders/__init__.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/builders/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,16 +307,16 @@
         return self
 
     def with_tax_type(self, value):
         self.transaction_modifier = TransactionModifier.LevelII
         self.tax_type = value
         return self
 
-    def __init__(self, transaction_type):
-        TransactionBuilder.__init__(self, transaction_type)
+    def __init__(self, transaction_type, payment_method=None):
+        TransactionBuilder.__init__(self, transaction_type, payment_method)
 
     def execute(self, config_name=None):
         """
         Executes the builder against the gateway.
         :return: Transaction
         """
```

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/builders/management_builder.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/builders/management_builder.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/builders/validations/validation_clause.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/validation_clause.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/builders/validations/validation_target.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/validation_target.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/builders/validations/validations.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/validations.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/entities/__init__.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/entities/address.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/entities/address.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/entities/ecommerce_info.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/entities/ecommerce_info.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/entities/encryption_data.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/entities/encryption_data.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/entities/enums.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/entities/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,18 @@
     Hold = 1 << 21
     #  Indicates a release
     Release = 1 << 22
     #  Indicates a 3DSecure signature verification
     VerifySignature = 1 << 23
     #  Indicates a 3DSecure enrollment verification
     VerifyEnrolled = 1 << 24
+    #  Indicates update Multi-Use Token
+    TokenUpdate = 1 << 25
+    #  Delete a Multi-Use Token
+    TokenDelete = 1 << 26
 
 
 class TransactionModifier(IntEnum):
     """
     Indicates if a transaction should be specialized.
     """
```

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/entities/exceptions.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/entities/transaction_summary.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/entities/transaction_summary.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/gateways/__init__.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/gateways/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1019,15 +1019,17 @@
 
             # gratuity
             if builder.gratuity is not None:
                 et.SubElement(root, 'GratuityAmtInfo').text = str(
                     builder.gratuity)
 
             # transaction id
-            et.SubElement(root, 'GatewayTxnId').text = builder.transaction_id
+            if builder.transaction_type != TransactionType.TokenUpdate\
+                    and builder.transaction_type != TransactionType.TokenDelete:
+                et.SubElement(root, 'GatewayTxnId').text = builder.transaction_id
 
             # client transaction id
             if builder.transaction_type == TransactionType.Reversal and builder.client_transaction_id:
                 et.SubElement(
                     root, 'ClientTxnId').text = builder.client_transaction_id
 
             # cpc data
@@ -1039,16 +1041,47 @@
                     et.SubElement(cpc,
                                   'CardHolderPONbr').text = builder.po_number
                 if builder.tax_type:
                     et.SubElement(cpc, 'TaxType').text = builder.tax_type.value
                 if builder.tax_amount:
                     et.SubElement(cpc, 'TaxAmt').text = str(builder.tax_amount)
 
+        if builder.transaction_type == TransactionType.TokenUpdate:
+            et.SubElement(transaction, 'TokenValue').text = builder.payment_method.token
+
+            token_actions = et.SubElement(transaction, 'TokenActions')
+
+            set = et.SubElement(token_actions, 'Set')
+
+            set_month_attribute = et.SubElement(set, 'Attribute')
+
+            et.SubElement(set_month_attribute, 'Name').text = 'ExpMonth'
+
+            et.SubElement(set_month_attribute, 'Value').text = builder.payment_method.exp_month
+
+            set_year_attribute = et.SubElement(set, 'Attribute')
+
+            et.SubElement(set_year_attribute, 'Name').text = 'ExpYear'
+
+            et.SubElement(set_year_attribute, 'Value').text = builder.payment_method.exp_year
+
+        if builder.transaction_type == TransactionType.TokenDelete:
+            et.SubElement(transaction, 'TokenValue').text = builder.payment_method.token
+
+            token_actions = et.SubElement(transaction, 'TokenActions')
+
+            et.SubElement(token_actions, 'Delete')
+
         response = self.do_transaction(
             self._build_envelope(transaction, builder.client_transaction_id))
+
+        if builder.transaction_type == TransactionType.TokenUpdate\
+                or builder.transaction_type == TransactionType.TokenDelete:
+            return True
+
         return self._map_response(response, builder.payment_method)
 
     def process_report(self, builder):
         transaction = et.Element(self._map_report_type(builder.report_type))
         if builder.timezone_conversion:
             et.SubElement(transaction,
                           'TzConversion').text = builder.timezone_conversion
@@ -1409,14 +1442,18 @@
             ret = 'GiftCardAlias'
         elif builder.transaction_type == TransactionType.Deactivate:
             ret = 'GiftCardDeactivate'
         elif builder.transaction_type == TransactionType.Replace:
             ret = 'GiftCardReplace'
         elif builder.transaction_type == TransactionType.Reward:
             ret = 'GiftCardReward'
+        elif builder.transaction_type == TransactionType.TokenUpdate:
+            ret = 'ManageTokens'
+        elif builder.transaction_type == TransactionType.TokenDelete:
+            ret = 'ManageTokens'
 
         if ret is None:
             raise UnsupportedTransactionException()
 
         return ret
 
     @staticmethod
```

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/__init__.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/credit.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/credit.py`

 * *Files 3% similar despite different names*

```diff
@@ -178,14 +178,35 @@
         @rtype: L{AuthorizationBuilder}
         @return: The builder
         '''
 
         return gp.api.builders.AuthorizationBuilder(TransactionType.Verify,
                                                     self)
 
+    def update_token_expiry(self):
+        '''
+        Updates expiration date contained within a Multi-Use Token
+
+        @rtype: L{ManagementBuilder}
+        @return: The builder
+        '''
+
+        return gp.api.builders.ManagementBuilder(TransactionType.TokenUpdate, self)\
+            .execute()
+
+    def delete_token(self):
+        '''
+        Deletes a Multi-Use Token from the gateway
+
+        @rtype: L{ManagementBuilder}
+        @return: The builder
+        '''
+
+        return gp.api.builders.ManagementBuilder(TransactionType.TokenDelete, self)\
+            .execute()
 
 class CreditCardData(Credit):
     '''
     Use credit tokens or manual entry data as a payment method.
     '''
 
     _cvn = None
```

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/debit.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/debit.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/ebt.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/ebt.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/echeck.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/echeck.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/giftcard.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/giftcard.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/payment_methods/payment_interfaces.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/payment_interfaces.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/services/recurring_service.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/services/recurring_service.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/services/reporting_service.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/services/reporting_service.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/globalpayments/api/utils/__init__.py` & `GlobalPayments.Api-1.0.6/globalpayments/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.5/setup.py` & `GlobalPayments.Api-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='GlobalPayments.Api',
-    version='1.0.5',
+    version='1.0.6',
     author='Heartland Payment Systems',
     author_email='EntApp_DevPortal@e-hps.com',
     packages=[
         'globalpayments', 'globalpayments.api', 'globalpayments.api.builders',
         'globalpayments.api.builders.validations',
         'globalpayments.api.entities',
         'globalpayments.api.entities.table_service',
```

