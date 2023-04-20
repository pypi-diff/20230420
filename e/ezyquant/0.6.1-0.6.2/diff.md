# Comparing `tmp/ezyquant-0.6.1.tar.gz` & `tmp/ezyquant-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezyquant-0.6.1.tar", last modified: Thu Apr 20 05:46:03 2023, max compression
+gzip compressed data, was "ezyquant-0.6.2.tar", last modified: Thu Apr 20 12:13:28 2023, max compression
```

## Comparing `ezyquant-0.6.1.tar` & `ezyquant-0.6.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:46:03.178913 ezyquant-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-20 05:45:47.000000 ezyquant-0.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-20 05:46:03.178913 ezyquant-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-20 05:45:47.000000 ezyquant-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:46:03.174913 ezyquant-0.6.1/ezyquant/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:46:03.178913 ezyquant-0.6.1/ezyquant/backtesting/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/backtesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/backtesting/_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/backtesting/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/backtesting/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/backtesting/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/backtesting/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/backtesting/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/indicators.py
--rw-r--r--   0 runner    (1001) docker     (123)    81847 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-20 05:45:47.000000 ezyquant-0.6.1/ezyquant/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:46:03.174913 ezyquant-0.6.1/ezyquant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-20 05:46:03.000000 ezyquant-0.6.1/ezyquant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 05:46:03.000000 ezyquant-0.6.1/ezyquant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 05:46:03.000000 ezyquant-0.6.1/ezyquant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 05:46:03.000000 ezyquant-0.6.1/ezyquant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 05:46:03.000000 ezyquant-0.6.1/ezyquant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 05:46:03.178913 ezyquant-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-20 05:45:47.000000 ezyquant-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:46:03.178913 ezyquant-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-04-20 05:45:47.000000 ezyquant-0.6.1/tests/test_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-04-20 05:45:47.000000 ezyquant-0.6.1/tests/test_indicators.py
--rw-r--r--   0 runner    (1001) docker     (123)    60298 2023-04-20 05:45:47.000000 ezyquant-0.6.1/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-20 05:45:47.000000 ezyquant-0.6.1/tests/test_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-04-20 05:45:47.000000 ezyquant-0.6.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:13:28.672164 ezyquant-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-20 12:13:05.000000 ezyquant-0.6.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-20 12:13:28.672164 ezyquant-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-20 12:13:05.000000 ezyquant-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:13:28.672164 ezyquant-0.6.2/ezyquant/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:13:28.672164 ezyquant-0.6.2/ezyquant/backtesting/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/backtesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/backtesting/_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/backtesting/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/backtesting/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/backtesting/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/backtesting/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/backtesting/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81847 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:13:28.672164 ezyquant-0.6.2/ezyquant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-20 12:13:28.000000 ezyquant-0.6.2/ezyquant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 12:13:28.000000 ezyquant-0.6.2/ezyquant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:13:28.000000 ezyquant-0.6.2/ezyquant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 12:13:28.000000 ezyquant-0.6.2/ezyquant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 12:13:28.000000 ezyquant-0.6.2/ezyquant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 12:13:28.676164 ezyquant-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-20 12:13:05.000000 ezyquant-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:13:28.672164 ezyquant-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-04-20 12:13:06.000000 ezyquant-0.6.2/tests/test_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-04-20 12:13:06.000000 ezyquant-0.6.2/tests/test_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60298 2023-04-20 12:13:06.000000 ezyquant-0.6.2/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-20 12:13:06.000000 ezyquant-0.6.2/tests/test_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-04-20 12:13:06.000000 ezyquant-0.6.2/tests/test_utils.py
```

### Comparing `ezyquant-0.6.1/LICENSE.txt` & `ezyquant-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/PKG-INFO` & `ezyquant-0.6.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant
-Version: 0.6.1
+Version: 0.6.2
 Summary: Powerful backtest python library for Thai stocks
 Home-page: https://www.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-0.6.1/README.md` & `ezyquant-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/ezyquant/backtesting/_backtesting.py` & `ezyquant-0.6.2/ezyquant/backtesting/_backtesting.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/ezyquant/backtesting/account.py` & `ezyquant-0.6.2/ezyquant/backtesting/account.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/ezyquant/backtesting/backtesting.py` & `ezyquant-0.6.2/ezyquant/backtesting/backtesting.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/ezyquant/backtesting/context.py` & `ezyquant-0.6.2/ezyquant/backtesting/context.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/ezyquant/backtesting/position.py` & `ezyquant-0.6.2/ezyquant/backtesting/position.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/ezyquant/backtesting/trade.py` & `ezyquant-0.6.2/ezyquant/backtesting/trade.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/ezyquant/connect.py` & `ezyquant-0.6.2/ezyquant/connect.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/ezyquant/creator.py` & `ezyquant-0.6.2/ezyquant/creator.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/ezyquant/fields.py` & `ezyquant-0.6.2/ezyquant/fields.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/ezyquant/indicators.py` & `ezyquant-0.6.2/ezyquant/indicators.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/ezyquant/reader.py` & `ezyquant-0.6.2/ezyquant/reader.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/ezyquant/report.py` & `ezyquant-0.6.2/ezyquant/report.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/ezyquant/utils.py` & `ezyquant-0.6.2/ezyquant/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -206,14 +206,17 @@
     def wrapped(
         *,
         symbol_list: Optional[List[str]] = None,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
         **kwargs,
     ):
+        if symbol_list:
+            symbol_list = list(symbol_list)
+
         call_key = tuple(sorted(kwargs.items()))
 
         if call_key not in call_dict:
             c_symbol_list = symbol_list
             c_start_date = start_date
             c_end_date = end_date
         else:
```

### Comparing `ezyquant-0.6.1/ezyquant/validators.py` & `ezyquant-0.6.2/ezyquant/validators.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/ezyquant.egg-info/PKG-INFO` & `ezyquant-0.6.2/ezyquant.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant
-Version: 0.6.1
+Version: 0.6.2
 Summary: Powerful backtest python library for Thai stocks
 Home-page: https://www.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-0.6.1/ezyquant.egg-info/SOURCES.txt` & `ezyquant-0.6.2/ezyquant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/setup.py` & `ezyquant-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/tests/test_creator.py` & `ezyquant-0.6.2/tests/test_creator.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/tests/test_indicators.py` & `ezyquant-0.6.2/tests/test_indicators.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/tests/test_reader.py` & `ezyquant-0.6.2/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/tests/test_test_utils.py` & `ezyquant-0.6.2/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.1/tests/test_utils.py` & `ezyquant-0.6.2/tests/test_utils.py`

 * *Files identical despite different names*

