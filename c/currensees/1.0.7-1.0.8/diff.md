# Comparing `tmp/currensees-1.0.7.tar.gz` & `tmp/currensees-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/currensees-1.0.7.tar", last modified: Thu Apr 20 00:31:08 2023, max compression
+gzip compressed data, was "dist/currensees-1.0.8.tar", last modified: Thu Apr 20 00:46:30 2023, max compression
```

## Comparing `currensees-1.0.7.tar` & `currensees-1.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-20 00:31:08.971408 currensees-1.0.7/
--rw-r--r--   0 finn       (501) staff       (20)     5937 2023-04-20 00:31:08.971759 currensees-1.0.7/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2897 2023-04-20 00:30:00.000000 currensees-1.0.7/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-20 00:31:08.966244 currensees-1.0.7/currensees/
--rw-r--r--   0 finn       (501) staff       (20)      292 2023-04-20 00:30:20.000000 currensees-1.0.7/currensees/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)      908 2023-04-19 23:42:50.000000 currensees-1.0.7/currensees/auth.py
--rw-r--r--   0 finn       (501) staff       (20)      711 2023-04-19 23:51:19.000000 currensees-1.0.7/currensees/convert.py
--rw-r--r--   0 finn       (501) staff       (20)      665 2023-04-19 23:53:31.000000 currensees-1.0.7/currensees/convert_all.py
--rw-r--r--   0 finn       (501) staff       (20)     1149 2023-04-19 23:47:05.000000 currensees-1.0.7/currensees/currencies.py
--rw-r--r--   0 finn       (501) staff       (20)      493 2023-04-19 23:55:16.000000 currensees-1.0.7/currensees/daily_average.py
--rw-r--r--   0 finn       (501) staff       (20)     1261 2023-04-19 23:49:50.000000 currensees-1.0.7/currensees/historical.py
--rw-r--r--   0 finn       (501) staff       (20)     1218 2023-04-19 23:59:06.000000 currensees-1.0.7/currensees/margins_spreads.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-20 00:30:36.000000 currensees-1.0.7/currensees/version.py
--rw-r--r--   0 finn       (501) staff       (20)      530 2023-04-19 23:56:35.000000 currensees-1.0.7/currensees/weekly_average.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-20 00:31:08.970683 currensees-1.0.7/currensees.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     5937 2023-04-20 00:31:08.000000 currensees-1.0.7/currensees.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-20 00:31:08.000000 currensees-1.0.7/currensees.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-20 00:31:08.000000 currensees-1.0.7/currensees.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-20 00:30:54.000000 currensees-1.0.7/currensees.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-20 00:31:08.000000 currensees-1.0.7/currensees.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       11 2023-04-20 00:31:08.000000 currensees-1.0.7/currensees.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-20 00:31:08.972506 currensees-1.0.7/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2646 2023-04-20 00:30:36.000000 currensees-1.0.7/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-20 00:46:30.788519 currensees-1.0.8/
+-rw-r--r--   0 finn       (501) staff       (20)     6279 2023-04-20 00:46:30.788835 currensees-1.0.8/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     3154 2023-04-20 00:45:27.000000 currensees-1.0.8/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-20 00:46:30.782690 currensees-1.0.8/currensees/
+-rw-r--r--   0 finn       (501) staff       (20)      292 2023-04-20 00:30:20.000000 currensees-1.0.8/currensees/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)      908 2023-04-19 23:42:50.000000 currensees-1.0.8/currensees/auth.py
+-rw-r--r--   0 finn       (501) staff       (20)      711 2023-04-19 23:51:19.000000 currensees-1.0.8/currensees/convert.py
+-rw-r--r--   0 finn       (501) staff       (20)      665 2023-04-19 23:53:31.000000 currensees-1.0.8/currensees/convert_all.py
+-rw-r--r--   0 finn       (501) staff       (20)     1149 2023-04-19 23:47:05.000000 currensees-1.0.8/currensees/currencies.py
+-rw-r--r--   0 finn       (501) staff       (20)      493 2023-04-19 23:55:16.000000 currensees-1.0.8/currensees/daily_average.py
+-rw-r--r--   0 finn       (501) staff       (20)     1261 2023-04-19 23:49:50.000000 currensees-1.0.8/currensees/historical.py
+-rw-r--r--   0 finn       (501) staff       (20)     1218 2023-04-19 23:59:06.000000 currensees-1.0.8/currensees/margins_spreads.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-20 00:45:55.000000 currensees-1.0.8/currensees/version.py
+-rw-r--r--   0 finn       (501) staff       (20)      530 2023-04-19 23:56:35.000000 currensees-1.0.8/currensees/weekly_average.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-20 00:46:30.787857 currensees-1.0.8/currensees.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     6279 2023-04-20 00:46:30.000000 currensees-1.0.8/currensees.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-20 00:46:30.000000 currensees-1.0.8/currensees.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-20 00:46:30.000000 currensees-1.0.8/currensees.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-20 00:46:17.000000 currensees-1.0.8/currensees.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-20 00:46:30.000000 currensees-1.0.8/currensees.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       11 2023-04-20 00:46:30.000000 currensees-1.0.8/currensees.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-20 00:46:30.789793 currensees-1.0.8/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2646 2023-04-20 00:45:55.000000 currensees-1.0.8/setup.py
```

### Comparing `currensees-1.0.7/PKG-INFO` & `currensees-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currensees
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python library for integrating with the Currency API.
 Home-page: https://moatsystems.com/currency-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/moatsystems/currensees_sdk/issues
 Project-URL: Changes, https://github.com/moatsystems/currensees_sdk/blob/main/CHANGELOG.md
@@ -45,57 +45,64 @@
         
         
         Usage Example
         -------------
         
         .. code-block:: python
         
-            import currensees
+            from currensees.auth import Auth
+            from currensees.currencies import Currencies
+            from currensees.historical import Historical
+            from currensees.convert import Convert
+            from currensees.convert_all import ConvertAll
+            from currensees.daily_average import DailyAverage
+            from currensees.weekly_average import WeeklyAverage
+            from currensees.margins_spreads import MarginsSpreads
         
             # Authenticate and log in
-            currensees.auth = Auth()
+            auth = Auth()
             username = "your_username"
             password = "your_password"
         
             result = auth.login(username, password)
             print("Login successful:", result)
         
-            currencies = currensees.Currencies(auth.headers)
+            currencies = Currencies(auth.headers)
             result = currencies.get_currencies(username, "19", "04", "2023")
             print("Currencies:", result)
         
             uuid = "currency_uuid"
             result = currencies.get_currency(uuid, username, "19", "04", "2023")
             print("Currency:", result)
         
-            historical = currensees.Historical(auth.headers)
+            historical = Historical(auth.headers)
             result = historical.get_historical(username, "2023_04_19", "19", "04", "2023")
             print("Historical data:", result)
         
             uuid = "historical_uuid"
             result = historical.get_historical_currency(uuid, username, "19", "04", "2023", "2023_04_19")
             print("Historical currency:", result)
         
-            convert = currensees.Convert(auth.headers)
+            convert = Convert(auth.headers)
             result = convert.convert_currency("2023_04_19", "GBP", "EUR", "500")
             print("Converted amount:", result)
         
-            convert_all = currensees.ConvertAll(auth.headers)
+            convert_all = ConvertAll(auth.headers)
             result = convert_all.convert_all_currencies("GBP", 120, "2023_04_19")
             print("Converted amounts:", result)
         
-            daily_average = currensees.DailyAverage(auth.headers)
+            daily_average = DailyAverage(auth.headers)
             result = daily_average.get_daily_average("2023_04_19")
             print("Daily average:", result)
         
-            weekly_average = currensees.WeeklyAverage(auth.headers)
+            weekly_average = WeeklyAverage(auth.headers)
             result = weekly_average.get_weekly_average("2023_04_03", "2023_04_07")
             print("Weekly average:", result)
         
-            margins_spreads = currensees.MarginsSpreads(auth.headers)
+            margins_spreads = MarginsSpreads(auth.headers)
             result = margins_spreads.get_margins_spreads(username, "19", "04", "2023")
             print("Margins and spreads:", result)
         
             uuid = "margins_spreads_uuid"
             result = margins_spreads.get_margins_spreads_currency(uuid, username, "19", "04", "2023")
             print("Margins and spreads for currency:", result)
```

### Comparing `currensees-1.0.7/README.md` & `currensees-1.0.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -24,58 +24,64 @@
 ## or `sudo python setup.py install` to install the package for all users
 ```
 
 Usage Example
 -------------
 
 ```python
-import currensees
+from currensees.auth import Auth
+from currensees.currencies import Currencies
+from currensees.historical import Historical
+from currensees.convert import Convert
+from currensees.convert_all import ConvertAll
+from currensees.daily_average import DailyAverage
+from currensees.weekly_average import WeeklyAverage
+from currensees.margins_spreads import MarginsSpreads
 
 # Authenticate and log in
-currensees.auth = Auth()
-
+auth = Auth()
 username = "your_username"
 password = "your_password"
 
 result = auth.login(username, password)
 print("Login successful:", result)
 
-currencies = currensees.Currencies(auth.headers)
+currencies = Currencies(auth.headers)
 result = currencies.get_currencies(username, "19", "04", "2023")
 print("Currencies:", result)
 
 uuid = "currency_uuid"
 result = currencies.get_currency(uuid, username, "19", "04", "2023")
 print("Currency:", result)
 
-historical = currensees.Historical(auth.headers)
+historical = Historical(auth.headers)
 result = historical.get_historical(username, "2023_04_19", "19", "04", "2023")
 print("Historical data:", result)
 
 uuid = "historical_uuid"
 result = historical.get_historical_currency(uuid, username, "19", "04", "2023", "2023_04_19")
 print("Historical currency:", result)
 
-convert = currensees.Convert(auth.headers)
+convert = Convert(auth.headers)
 result = convert.convert_currency("2023_04_19", "GBP", "EUR", "500")
 print("Converted amount:", result)
 
-convert_all = currensees.ConvertAll(auth.headers)
+convert_all = ConvertAll(auth.headers)
 result = convert_all.convert_all_currencies("GBP", 120, "2023_04_19")
 print("Converted amounts:", result)
 
-daily_average = currensees.DailyAverage(auth.headers)
+daily_average = DailyAverage(auth.headers)
 result = daily_average.get_daily_average("2023_04_19")
 print("Daily average:", result)
 
-weekly_average = currensees.WeeklyAverage(auth.headers)
+weekly_average = WeeklyAverage(auth.headers)
 result = weekly_average.get_weekly_average("2023_04_03", "2023_04_07")
 print("Weekly average:", result)
 
-margins_spreads = currensees.MarginsSpreads(auth.headers)
+margins_spreads = MarginsSpreads(auth.headers)
 result = margins_spreads.get_margins_spreads(username, "19", "04", "2023")
 print("Margins and spreads:", result)
 
 uuid = "margins_spreads_uuid"
 result = margins_spreads.get_margins_spreads_currency(uuid, username, "19", "04", "2023")
 print("Margins and spreads for currency:", result)
 ```
```

### Comparing `currensees-1.0.7/currensees/auth.py` & `currensees-1.0.8/currensees/auth.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.7/currensees/convert.py` & `currensees-1.0.8/currensees/convert.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.7/currensees/convert_all.py` & `currensees-1.0.8/currensees/convert_all.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.7/currensees/currencies.py` & `currensees-1.0.8/currensees/currencies.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.7/currensees/historical.py` & `currensees-1.0.8/currensees/historical.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.7/currensees/margins_spreads.py` & `currensees-1.0.8/currensees/margins_spreads.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.7/currensees/weekly_average.py` & `currensees-1.0.8/currensees/weekly_average.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.7/currensees.egg-info/PKG-INFO` & `currensees-1.0.8/currensees.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currensees
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python library for integrating with the Currency API.
 Home-page: https://moatsystems.com/currency-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/moatsystems/currensees_sdk/issues
 Project-URL: Changes, https://github.com/moatsystems/currensees_sdk/blob/main/CHANGELOG.md
@@ -45,57 +45,64 @@
         
         
         Usage Example
         -------------
         
         .. code-block:: python
         
-            import currensees
+            from currensees.auth import Auth
+            from currensees.currencies import Currencies
+            from currensees.historical import Historical
+            from currensees.convert import Convert
+            from currensees.convert_all import ConvertAll
+            from currensees.daily_average import DailyAverage
+            from currensees.weekly_average import WeeklyAverage
+            from currensees.margins_spreads import MarginsSpreads
         
             # Authenticate and log in
-            currensees.auth = Auth()
+            auth = Auth()
             username = "your_username"
             password = "your_password"
         
             result = auth.login(username, password)
             print("Login successful:", result)
         
-            currencies = currensees.Currencies(auth.headers)
+            currencies = Currencies(auth.headers)
             result = currencies.get_currencies(username, "19", "04", "2023")
             print("Currencies:", result)
         
             uuid = "currency_uuid"
             result = currencies.get_currency(uuid, username, "19", "04", "2023")
             print("Currency:", result)
         
-            historical = currensees.Historical(auth.headers)
+            historical = Historical(auth.headers)
             result = historical.get_historical(username, "2023_04_19", "19", "04", "2023")
             print("Historical data:", result)
         
             uuid = "historical_uuid"
             result = historical.get_historical_currency(uuid, username, "19", "04", "2023", "2023_04_19")
             print("Historical currency:", result)
         
-            convert = currensees.Convert(auth.headers)
+            convert = Convert(auth.headers)
             result = convert.convert_currency("2023_04_19", "GBP", "EUR", "500")
             print("Converted amount:", result)
         
-            convert_all = currensees.ConvertAll(auth.headers)
+            convert_all = ConvertAll(auth.headers)
             result = convert_all.convert_all_currencies("GBP", 120, "2023_04_19")
             print("Converted amounts:", result)
         
-            daily_average = currensees.DailyAverage(auth.headers)
+            daily_average = DailyAverage(auth.headers)
             result = daily_average.get_daily_average("2023_04_19")
             print("Daily average:", result)
         
-            weekly_average = currensees.WeeklyAverage(auth.headers)
+            weekly_average = WeeklyAverage(auth.headers)
             result = weekly_average.get_weekly_average("2023_04_03", "2023_04_07")
             print("Weekly average:", result)
         
-            margins_spreads = currensees.MarginsSpreads(auth.headers)
+            margins_spreads = MarginsSpreads(auth.headers)
             result = margins_spreads.get_margins_spreads(username, "19", "04", "2023")
             print("Margins and spreads:", result)
         
             uuid = "margins_spreads_uuid"
             result = margins_spreads.get_margins_spreads_currency(uuid, username, "19", "04", "2023")
             print("Margins and spreads for currency:", result)
```

### Comparing `currensees-1.0.7/setup.py` & `currensees-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "currensees"
-VERSION = "1.0.7"
+VERSION = "1.0.8"
 REQUIRES = ["requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

