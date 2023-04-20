# Comparing `tmp/currensees-1.0.6.tar.gz` & `tmp/currensees-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/currensees-1.0.6.tar", last modified: Wed Apr 19 18:12:16 2023, max compression
+gzip compressed data, was "dist/currensees-1.0.7.tar", last modified: Thu Apr 20 00:31:08 2023, max compression
```

## Comparing `currensees-1.0.6.tar` & `currensees-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-19 18:12:16.756792 currensees-1.0.6/
--rw-r--r--   0 finn       (501) staff       (20)     6309 2023-04-19 18:12:16.757166 currensees-1.0.6/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     3148 2023-04-19 18:03:57.000000 currensees-1.0.6/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-19 18:12:16.749677 currensees-1.0.6/currensees/
--rw-r--r--   0 finn       (501) staff       (20)      163 2023-04-05 11:07:01.000000 currensees-1.0.6/currensees/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)      584 2023-04-16 20:45:41.000000 currensees-1.0.6/currensees/auth.py
--rw-r--r--   0 finn       (501) staff       (20)      781 2023-04-05 16:54:46.000000 currensees-1.0.6/currensees/convert.py
--rw-r--r--   0 finn       (501) staff       (20)      671 2023-04-05 16:57:18.000000 currensees-1.0.6/currensees/convert_all.py
--rw-r--r--   0 finn       (501) staff       (20)      940 2023-04-19 17:49:11.000000 currensees-1.0.6/currensees/currencies.py
--rw-r--r--   0 finn       (501) staff       (20)      440 2023-04-19 18:04:01.000000 currensees-1.0.6/currensees/daily_average.py
--rw-r--r--   0 finn       (501) staff       (20)     1030 2023-04-05 17:02:43.000000 currensees-1.0.6/currensees/historical.py
--rw-r--r--   0 finn       (501) staff       (20)     1060 2023-04-19 18:04:05.000000 currensees-1.0.6/currensees/margins_spreads.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-19 18:10:17.000000 currensees-1.0.6/currensees/version.py
--rw-r--r--   0 finn       (501) staff       (20)      518 2023-04-19 17:59:07.000000 currensees-1.0.6/currensees/weekly_average.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-19 18:12:16.755990 currensees-1.0.6/currensees.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     6309 2023-04-19 18:12:16.000000 currensees-1.0.6/currensees.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-19 18:12:16.000000 currensees-1.0.6/currensees.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-19 18:12:16.000000 currensees-1.0.6/currensees.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-19 18:12:00.000000 currensees-1.0.6/currensees.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-19 18:12:16.000000 currensees-1.0.6/currensees.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       11 2023-04-19 18:12:16.000000 currensees-1.0.6/currensees.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-19 18:12:16.758298 currensees-1.0.6/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2646 2023-04-19 18:10:17.000000 currensees-1.0.6/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-20 00:31:08.971408 currensees-1.0.7/
+-rw-r--r--   0 finn       (501) staff       (20)     5937 2023-04-20 00:31:08.971759 currensees-1.0.7/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2897 2023-04-20 00:30:00.000000 currensees-1.0.7/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-20 00:31:08.966244 currensees-1.0.7/currensees/
+-rw-r--r--   0 finn       (501) staff       (20)      292 2023-04-20 00:30:20.000000 currensees-1.0.7/currensees/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)      908 2023-04-19 23:42:50.000000 currensees-1.0.7/currensees/auth.py
+-rw-r--r--   0 finn       (501) staff       (20)      711 2023-04-19 23:51:19.000000 currensees-1.0.7/currensees/convert.py
+-rw-r--r--   0 finn       (501) staff       (20)      665 2023-04-19 23:53:31.000000 currensees-1.0.7/currensees/convert_all.py
+-rw-r--r--   0 finn       (501) staff       (20)     1149 2023-04-19 23:47:05.000000 currensees-1.0.7/currensees/currencies.py
+-rw-r--r--   0 finn       (501) staff       (20)      493 2023-04-19 23:55:16.000000 currensees-1.0.7/currensees/daily_average.py
+-rw-r--r--   0 finn       (501) staff       (20)     1261 2023-04-19 23:49:50.000000 currensees-1.0.7/currensees/historical.py
+-rw-r--r--   0 finn       (501) staff       (20)     1218 2023-04-19 23:59:06.000000 currensees-1.0.7/currensees/margins_spreads.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-20 00:30:36.000000 currensees-1.0.7/currensees/version.py
+-rw-r--r--   0 finn       (501) staff       (20)      530 2023-04-19 23:56:35.000000 currensees-1.0.7/currensees/weekly_average.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-20 00:31:08.970683 currensees-1.0.7/currensees.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     5937 2023-04-20 00:31:08.000000 currensees-1.0.7/currensees.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-20 00:31:08.000000 currensees-1.0.7/currensees.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-20 00:31:08.000000 currensees-1.0.7/currensees.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-20 00:30:54.000000 currensees-1.0.7/currensees.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-20 00:31:08.000000 currensees-1.0.7/currensees.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       11 2023-04-20 00:31:08.000000 currensees-1.0.7/currensees.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-20 00:31:08.972506 currensees-1.0.7/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2646 2023-04-20 00:30:36.000000 currensees-1.0.7/setup.py
```

### Comparing `currensees-1.0.6/PKG-INFO` & `currensees-1.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currensees
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python library for integrating with the Currency API.
 Home-page: https://moatsystems.com/currency-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/moatsystems/currensees_sdk/issues
 Project-URL: Changes, https://github.com/moatsystems/currensees_sdk/blob/main/CHANGELOG.md
@@ -48,70 +48,60 @@
         -------------
         
         .. code-block:: python
         
             import currensees
         
             # Authenticate and log in
-            username = '<username>'
-            password = '<password>'
-            auth = CurrenseesAuth(username, password)
-            login_response = auth.login()
-        
-            # Currency conversion
-            converter = CurrencyConverter("GBP", "CAD", "500", "2023_04_02")
-            print(converter.convert())
-        
-            # Convert all available currencies
-            converter = ConvertAllCurrencies("GBP", 120, "2023_04_02")
-            print(converter.convert())
-        
-            # Retrieve all available currencies
-            currencies = Currencies(username, '02', '04', '2023')
-            print(currencies.get_currencies())
-        
-            # Retrieve a currency by uuid
-            currencies = Currencies(username, '02', '04', '2023')
-            print(currencies.get_currency_by_uuid('594bffc4-d095-11ed-9e30-acde48001122'))
-        
-            # Retrieve currencies historical rates
-            historical_rates = HistoricalRates(username, '2023_04_02', '02', '04', '2023')
-            print(historical_rates.get_historical_rates())
-        
-            # Retrieve currencies historical rates by uuid
-            historical_rates = HistoricalRates(username, '2023_04_02', '02', '04', '2023')
-            print(historical_rates.get_historical_rate_by_uuid('fe86014c-d162-11ed-a2dc-acde48001122'))
-        
-            # Retrieve a daily average of all the currencies
-            date = "2023_04_10"
-            daily_average = DailyAverage(date)
-            print(daily_average.fetch_daily_average())
-        
-            # Retrieve weekly average of all the currencies
-            date_from = "2023_04_03"
-            date_to = "2023_04_07"
-            weekly_average = WeeklyAverage(date_from, date_to)
-            print(weekly_average.fetch_weekly_average())
-        
-            # Initialize the MarginsSpreads class with a username and date
-            day = 19
-            month = 4
-            year = 2023
-            margins_spreads_instance = MarginsSpreads(username, day, month, year)
-        
-            # Fetch all margins and spreads data for the given user and date
-            all_margins_spreads = margins_spreads_instance.get_margins_spreads()
-            print("All Margins and Spreads:")
-            print(all_margins_spreads)
-        
-            # Fetch margin and spread data for a specific UUID
-            uuid = "data_uuid"
-            margin_spread = margins_spreads_instance.get_margin_spread_by_uuid(uuid)
-            print(f"Margin and Spread for UUID {uuid}:")
-            print(margin_spread)
+            currensees.auth = Auth()
+            username = "your_username"
+            password = "your_password"
+        
+            result = auth.login(username, password)
+            print("Login successful:", result)
+        
+            currencies = currensees.Currencies(auth.headers)
+            result = currencies.get_currencies(username, "19", "04", "2023")
+            print("Currencies:", result)
+        
+            uuid = "currency_uuid"
+            result = currencies.get_currency(uuid, username, "19", "04", "2023")
+            print("Currency:", result)
+        
+            historical = currensees.Historical(auth.headers)
+            result = historical.get_historical(username, "2023_04_19", "19", "04", "2023")
+            print("Historical data:", result)
+        
+            uuid = "historical_uuid"
+            result = historical.get_historical_currency(uuid, username, "19", "04", "2023", "2023_04_19")
+            print("Historical currency:", result)
+        
+            convert = currensees.Convert(auth.headers)
+            result = convert.convert_currency("2023_04_19", "GBP", "EUR", "500")
+            print("Converted amount:", result)
+        
+            convert_all = currensees.ConvertAll(auth.headers)
+            result = convert_all.convert_all_currencies("GBP", 120, "2023_04_19")
+            print("Converted amounts:", result)
+        
+            daily_average = currensees.DailyAverage(auth.headers)
+            result = daily_average.get_daily_average("2023_04_19")
+            print("Daily average:", result)
+        
+            weekly_average = currensees.WeeklyAverage(auth.headers)
+            result = weekly_average.get_weekly_average("2023_04_03", "2023_04_07")
+            print("Weekly average:", result)
+        
+            margins_spreads = currensees.MarginsSpreads(auth.headers)
+            result = margins_spreads.get_margins_spreads(username, "19", "04", "2023")
+            print("Margins and spreads:", result)
+        
+            uuid = "margins_spreads_uuid"
+            result = margins_spreads.get_margins_spreads_currency(uuid, username, "19", "04", "2023")
+            print("Margins and spreads for currency:", result)
         
         
         Setting up Currency API Account
         -------------------------------
         
         Subscribe here for a `user account`_.
```

### Comparing `currensees-1.0.6/README.md` & `currensees-1.0.7/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -27,70 +27,61 @@
 Usage Example
 -------------
 
 ```python
 import currensees
 
 # Authenticate and log in
-username = '<username>'
-password = '<password>'
-auth = CurrenseesAuth(username, password)
-login_response = auth.login()
-
-# Currency conversion
-converter = CurrencyConverter("GBP", "CAD", "500", "2023_04_02")
-print(converter.convert())
-
-# Convert all available currencies
-converter = ConvertAllCurrencies("GBP", 120, "2023_04_02")
-print(converter.convert())
-
-# Retrieve all available currencies
-currencies = Currencies(username, '02', '04', '2023')
-print(currencies.get_currencies())
-
-# Retrieve a currency by uuid
-currencies = Currencies(username, '02', '04', '2023')
-print(currencies.get_currency_by_uuid('594bffc4-d095-11ed-9e30-acde48001122'))
-
-# Retrieve currencies historical rates
-historical_rates = HistoricalRates(username, '2023_04_02', '02', '04', '2023')
-print(historical_rates.get_historical_rates())
-
-# Retrieve currencies historical rates by uuid
-historical_rates = HistoricalRates(username, '2023_04_02', '02', '04', '2023')
-print(historical_rates.get_historical_rate_by_uuid('fe86014c-d162-11ed-a2dc-acde48001122'))
-
-# Retrieve a daily average of all the currencies
-date = "2023_04_10"
-daily_average = DailyAverage(date)
-print(daily_average.fetch_daily_average())
-
-# Retrieve weekly average of all the currencies
-date_from = "2023_04_03"
-date_to = "2023_04_07"
-weekly_average = WeeklyAverage(date_from, date_to)
-print(weekly_average.fetch_weekly_average())
-
-# Initialize the MarginsSpreads class with a username and date
-day = 19
-month = 4
-year = 2023
-margins_spreads_instance = MarginsSpreads(username, day, month, year)
-
-# Fetch all margins and spreads data for the given user and date
-all_margins_spreads = margins_spreads_instance.get_margins_spreads()
-print("All Margins and Spreads:")
-print(all_margins_spreads)
-
-# Fetch margin and spread data for a specific UUID
-uuid = "data_uuid"
-margin_spread = margins_spreads_instance.get_margin_spread_by_uuid(uuid)
-print(f"Margin and Spread for UUID {uuid}:")
-print(margin_spread)
+currensees.auth = Auth()
+
+username = "your_username"
+password = "your_password"
+
+result = auth.login(username, password)
+print("Login successful:", result)
+
+currencies = currensees.Currencies(auth.headers)
+result = currencies.get_currencies(username, "19", "04", "2023")
+print("Currencies:", result)
+
+uuid = "currency_uuid"
+result = currencies.get_currency(uuid, username, "19", "04", "2023")
+print("Currency:", result)
+
+historical = currensees.Historical(auth.headers)
+result = historical.get_historical(username, "2023_04_19", "19", "04", "2023")
+print("Historical data:", result)
+
+uuid = "historical_uuid"
+result = historical.get_historical_currency(uuid, username, "19", "04", "2023", "2023_04_19")
+print("Historical currency:", result)
+
+convert = currensees.Convert(auth.headers)
+result = convert.convert_currency("2023_04_19", "GBP", "EUR", "500")
+print("Converted amount:", result)
+
+convert_all = currensees.ConvertAll(auth.headers)
+result = convert_all.convert_all_currencies("GBP", 120, "2023_04_19")
+print("Converted amounts:", result)
+
+daily_average = currensees.DailyAverage(auth.headers)
+result = daily_average.get_daily_average("2023_04_19")
+print("Daily average:", result)
+
+weekly_average = currensees.WeeklyAverage(auth.headers)
+result = weekly_average.get_weekly_average("2023_04_03", "2023_04_07")
+print("Weekly average:", result)
+
+margins_spreads = currensees.MarginsSpreads(auth.headers)
+result = margins_spreads.get_margins_spreads(username, "19", "04", "2023")
+print("Margins and spreads:", result)
+
+uuid = "margins_spreads_uuid"
+result = margins_spreads.get_margins_spreads_currency(uuid, username, "19", "04", "2023")
+print("Margins and spreads for currency:", result)
 ```
 
 ## Setting up Currency API Account
 
 Subscribe here for a [user account](https://moatsystems.com/currency-api/).
```

### Comparing `currensees-1.0.6/currensees/historical.py` & `currensees-1.0.7/currensees/auth.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import requests
+import json
 
-class HistoricalRates:
-    def __init__(self, username, date, day, month, year):
-        self.username = username
-        self.date = date
-        self.day = day
-        self.month = month
-        self.year = year
-
-    def get_historical_rates(self):
-        url = f"https://currensees.com/v1/historical?username={self.username}&date={self.date}&day={self.day}&month={self.month}&year={self.year}"
-
-        payload = {}
-        headers = {
-            'Accept': 'application/json'
+class Auth:
+    def __init__(self):
+        self.base_url = 'https://currensees.com/v1'
+        self.headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
         }
 
-        response = requests.request("GET", url, headers=headers, data=payload)
-        return response.text
-
-    def get_historical_rate_by_uuid(self, uuid):
-        url = f"https://currensees.com/v1/historical/{uuid}?username={self.username}&day={self.day}&month={self.month}&year={self.year}&date_string={self.date}"
-
-        payload = {}
-        headers = {
-            'Accept': 'application/json'
+    def login(self, username, password):
+        url = f'{self.base_url}/login'
+        data = {
+            'username': username,
+            'password': password
         }
-
-        response = requests.request("GET", url, headers=headers, data=payload)
-        return response.text
+        response = requests.post(url, headers=self.headers, data=json.dumps(data))
+        
+        if response.status_code == 200:
+            user_type = response.cookies.get('user_type')
+            username_cookie = response.cookies.get('username')
+            self.headers.update({
+                'Cookie': f'user_type={user_type}; username={username_cookie}'
+            })
+            return response.json()
+        else:
+            raise Exception(f"Login failed: {response.text}")
```

### Comparing `currensees-1.0.6/currensees/margins_spreads.py` & `currensees-1.0.7/currensees/margins_spreads.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import requests
+import json
 
 class MarginsSpreads:
-    def __init__(self, username, day, month, year):
-        self.username = username
-        self.day = day
-        self.month = month
-        self.year = year
-
-    def get_margins_spreads(self):
-        url = f"https://currensees.com/v1/margins_spreads?username={self.username}&day={self.day}&month={self.month}&year={self.year}"
-
-        payload = {}
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
+    def __init__(self, headers):
+        self.base_url = 'https://currensees.com/v1'
+        self.headers = headers
+
+    def get_margins_spreads(self, username, day, month, year):
+        url = f'{self.base_url}/margins_spreads'
+        params = {
+            'username': username,
+            'day': day,
+            'month': month,
+            'year': year
         }
-
-        response = requests.request("GET", url, headers=headers, data=payload)
-        return response.text
-
-    def get_margin_spread_by_uuid(self, uuid):
-        url = f"https://currensees.com/v1/margins_spreads/{uuid}?username={self.username}&day={self.day}&month={self.month}&year={self.year}"
-
-        payload = {}
-        headers = {
-            'Content-Type': 'application/json',
-            'Accept': 'application/json'
+        response = requests.get(url, headers=self.headers, params=params)
+        
+        if response.status_code == 200:
+            return response.json()
+        else:
+            raise Exception(f"Failed to get margins and spreads: {response.text}")
+
+    def get_margins_spreads_currency(self, uuid, username, day, month, year):
+        url = f'{self.base_url}/margins_spreads/{uuid}'
+        params = {
+            'username': username,
+            'day': day,
+            'month': month,
+            'year': year
         }
-
-        response = requests.request("GET", url, headers=headers, data=payload)
-        return response.text
+        response = requests.get(url, headers=self.headers, params=params)
+        
+        if response.status_code == 200:
+            return response.json()
+        else:
+            raise Exception(f"Failed to get margins and spreads for currency: {response.text}")
```

### Comparing `currensees-1.0.6/currensees.egg-info/PKG-INFO` & `currensees-1.0.7/currensees.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currensees
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python library for integrating with the Currency API.
 Home-page: https://moatsystems.com/currency-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/moatsystems/currensees_sdk/issues
 Project-URL: Changes, https://github.com/moatsystems/currensees_sdk/blob/main/CHANGELOG.md
@@ -48,70 +48,60 @@
         -------------
         
         .. code-block:: python
         
             import currensees
         
             # Authenticate and log in
-            username = '<username>'
-            password = '<password>'
-            auth = CurrenseesAuth(username, password)
-            login_response = auth.login()
-        
-            # Currency conversion
-            converter = CurrencyConverter("GBP", "CAD", "500", "2023_04_02")
-            print(converter.convert())
-        
-            # Convert all available currencies
-            converter = ConvertAllCurrencies("GBP", 120, "2023_04_02")
-            print(converter.convert())
-        
-            # Retrieve all available currencies
-            currencies = Currencies(username, '02', '04', '2023')
-            print(currencies.get_currencies())
-        
-            # Retrieve a currency by uuid
-            currencies = Currencies(username, '02', '04', '2023')
-            print(currencies.get_currency_by_uuid('594bffc4-d095-11ed-9e30-acde48001122'))
-        
-            # Retrieve currencies historical rates
-            historical_rates = HistoricalRates(username, '2023_04_02', '02', '04', '2023')
-            print(historical_rates.get_historical_rates())
-        
-            # Retrieve currencies historical rates by uuid
-            historical_rates = HistoricalRates(username, '2023_04_02', '02', '04', '2023')
-            print(historical_rates.get_historical_rate_by_uuid('fe86014c-d162-11ed-a2dc-acde48001122'))
-        
-            # Retrieve a daily average of all the currencies
-            date = "2023_04_10"
-            daily_average = DailyAverage(date)
-            print(daily_average.fetch_daily_average())
-        
-            # Retrieve weekly average of all the currencies
-            date_from = "2023_04_03"
-            date_to = "2023_04_07"
-            weekly_average = WeeklyAverage(date_from, date_to)
-            print(weekly_average.fetch_weekly_average())
-        
-            # Initialize the MarginsSpreads class with a username and date
-            day = 19
-            month = 4
-            year = 2023
-            margins_spreads_instance = MarginsSpreads(username, day, month, year)
-        
-            # Fetch all margins and spreads data for the given user and date
-            all_margins_spreads = margins_spreads_instance.get_margins_spreads()
-            print("All Margins and Spreads:")
-            print(all_margins_spreads)
-        
-            # Fetch margin and spread data for a specific UUID
-            uuid = "data_uuid"
-            margin_spread = margins_spreads_instance.get_margin_spread_by_uuid(uuid)
-            print(f"Margin and Spread for UUID {uuid}:")
-            print(margin_spread)
+            currensees.auth = Auth()
+            username = "your_username"
+            password = "your_password"
+        
+            result = auth.login(username, password)
+            print("Login successful:", result)
+        
+            currencies = currensees.Currencies(auth.headers)
+            result = currencies.get_currencies(username, "19", "04", "2023")
+            print("Currencies:", result)
+        
+            uuid = "currency_uuid"
+            result = currencies.get_currency(uuid, username, "19", "04", "2023")
+            print("Currency:", result)
+        
+            historical = currensees.Historical(auth.headers)
+            result = historical.get_historical(username, "2023_04_19", "19", "04", "2023")
+            print("Historical data:", result)
+        
+            uuid = "historical_uuid"
+            result = historical.get_historical_currency(uuid, username, "19", "04", "2023", "2023_04_19")
+            print("Historical currency:", result)
+        
+            convert = currensees.Convert(auth.headers)
+            result = convert.convert_currency("2023_04_19", "GBP", "EUR", "500")
+            print("Converted amount:", result)
+        
+            convert_all = currensees.ConvertAll(auth.headers)
+            result = convert_all.convert_all_currencies("GBP", 120, "2023_04_19")
+            print("Converted amounts:", result)
+        
+            daily_average = currensees.DailyAverage(auth.headers)
+            result = daily_average.get_daily_average("2023_04_19")
+            print("Daily average:", result)
+        
+            weekly_average = currensees.WeeklyAverage(auth.headers)
+            result = weekly_average.get_weekly_average("2023_04_03", "2023_04_07")
+            print("Weekly average:", result)
+        
+            margins_spreads = currensees.MarginsSpreads(auth.headers)
+            result = margins_spreads.get_margins_spreads(username, "19", "04", "2023")
+            print("Margins and spreads:", result)
+        
+            uuid = "margins_spreads_uuid"
+            result = margins_spreads.get_margins_spreads_currency(uuid, username, "19", "04", "2023")
+            print("Margins and spreads for currency:", result)
         
         
         Setting up Currency API Account
         -------------------------------
         
         Subscribe here for a `user account`_.
```

### Comparing `currensees-1.0.6/setup.py` & `currensees-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "currensees"
-VERSION = "1.0.6"
+VERSION = "1.0.7"
 REQUIRES = ["requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

