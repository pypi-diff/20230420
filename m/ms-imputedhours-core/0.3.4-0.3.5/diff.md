# Comparing `tmp/ms_imputedhours_core-0.3.4.tar.gz` & `tmp/ms_imputedhours_core-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_imputedhours_core-0.3.4.tar", max compression
+gzip compressed data, was "ms_imputedhours_core-0.3.5.tar", max compression
```

## Comparing `ms_imputedhours_core-0.3.4.tar` & `ms_imputedhours_core-0.3.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35149 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/LICENSE
--rw-r--r--   0        0        0     2401 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/README.md
--rw-r--r--   0        0        0       22 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/__init__.py
--rw-r--r--   0        0        0     3238 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/agreements/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/agreements/__tests__/__init__.py
--rw-r--r--   0        0        0     3228 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/agreements/__tests__/test_agreements.py
--rw-r--r--   0        0        0     4113 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/__tests__/__init__.py
--rw-r--r--   0        0        0     6179 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/__tests__/test_employee.py
--rw-r--r--   0        0        0     6933 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/__tests__/__init__.py
--rw-r--r--   0        0        0     9019 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/__tests__/test_data.py
--rw-r--r--   0        0        0    10444 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/bigquery.py
--rw-r--r--   0        0        0      171 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/constants.py
--rw-r--r--   0        0        0        0 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__tests__/__init__.py
--rw-r--r--   0        0        0     4491 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py
--rw-r--r--   0        0        0     6206 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py
--rw-r--r--   0        0        0      776 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py
--rw-r--r--   0        0        0      655 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/alert.py
--rw-r--r--   0        0        0     3599 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/bigquery.py
--rw-r--r--   0        0        0      423 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/dates.py
--rw-r--r--   0        0        0        0 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/transformers/__init__.py
--rw-r--r--   0        0        0     3828 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/transformers/hours.py
--rw-r--r--   0        0        0      203 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/office/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/office/__tests__/__init__.py
--rw-r--r--   0        0        0      678 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/office/__tests__/test_office.py
--rw-r--r--   0        0        0      950 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 ms_imputedhours_core-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-20 11:36:24.207517 ms_imputedhours_core-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2401 2023-04-20 11:36:24.207517 ms_imputedhours_core-0.3.5/README.md
+-rw-r--r--   0        0        0       22 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/__init__.py
+-rw-r--r--   0        0        0     3238 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/agreements/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/agreements/__tests__/__init__.py
+-rw-r--r--   0        0        0     3228 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/agreements/__tests__/test_agreements.py
+-rw-r--r--   0        0        0     4113 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/__tests__/__init__.py
+-rw-r--r--   0        0        0     6179 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/__tests__/test_employee.py
+-rw-r--r--   0        0        0     6933 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/__tests__/__init__.py
+-rw-r--r--   0        0        0     9019 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/__tests__/test_data.py
+-rw-r--r--   0        0        0    10444 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/bigquery.py
+-rw-r--r--   0        0        0      171 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/constants.py
+-rw-r--r--   0        0        0        0 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__tests__/__init__.py
+-rw-r--r--   0        0        0     4491 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py
+-rw-r--r--   0        0        0     6206 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py
+-rw-r--r--   0        0        0      776 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py
+-rw-r--r--   0        0        0      654 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/alert.py
+-rw-r--r--   0        0        0     3599 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/bigquery.py
+-rw-r--r--   0        0        0      423 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/dates.py
+-rw-r--r--   0        0        0        0 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/transformers/__init__.py
+-rw-r--r--   0        0        0     3828 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/transformers/hours.py
+-rw-r--r--   0        0        0      203 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/office/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/office/__tests__/__init__.py
+-rw-r--r--   0        0        0      678 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/office/__tests__/test_office.py
+-rw-r--r--   0        0        0      950 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 ms_imputedhours_core-0.3.5/PKG-INFO
```

### Comparing `ms_imputedhours_core-0.3.4/LICENSE` & `ms_imputedhours_core-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/README.md` & `ms_imputedhours_core-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/ms_imputedhours_core/agreements/__init__.py` & `ms_imputedhours_core-0.3.5/ms_imputedhours_core/agreements/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/ms_imputedhours_core/agreements/__tests__/test_agreements.py` & `ms_imputedhours_core-0.3.5/ms_imputedhours_core/agreements/__tests__/test_agreements.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/__init__.py` & `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/__tests__/test_employee.py` & `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/__tests__/test_employee.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/__init__.py` & `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/__tests__/test_data.py` & `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/__tests__/test_data.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/bigquery.py` & `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py` & `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py` & `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py` & `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/alert.py` & `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/alert.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 def should_exclude_employee(email, date, hired_date, end_date):
     is_email_excluded = email in EXCLUDE_ALERT_EMAILS
 
     is_personal_email = "@makingscience" not in email
 
-    is_enddate_before_date = end_date and (end_date.year, end_date.month) <= (
+    is_enddate_before_date = end_date and (end_date.year, end_date.month) < (
         date.year,
         date.month,
     )
 
     is_hired_date_after_date = hired_date and (
         hired_date.year,
         hired_date.month,
```

### Comparing `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/bigquery.py` & `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/transformers/hours.py` & `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/transformers/hours.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/ms_imputedhours_core/office/__tests__/test_office.py` & `ms_imputedhours_core-0.3.5/ms_imputedhours_core/office/__tests__/test_office.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.4/pyproject.toml` & `ms_imputedhours_core-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-imputedhours-core"
-version = "0.3.4"
+version = "0.3.5"
 description = "Python library to collect data about jira imputed hours and employee agreements"
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_imputedhours_core"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_imputedhours_core-0.3.4/PKG-INFO` & `ms_imputedhours_core-0.3.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-imputedhours-core
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python library to collect data about jira imputed hours and employee agreements
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

