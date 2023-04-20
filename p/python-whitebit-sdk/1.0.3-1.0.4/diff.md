# Comparing `tmp/python-whitebit-sdk-1.0.3.tar.gz` & `tmp/python-whitebit-sdk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-whitebit-sdk-1.0.3.tar", last modified: Thu Apr 20 12:09:00 2023, max compression
+gzip compressed data, was "python-whitebit-sdk-1.0.4.tar", last modified: Thu Apr 20 12:40:42 2023, max compression
```

## Comparing `python-whitebit-sdk-1.0.3.tar` & `python-whitebit-sdk-1.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.683591 python-whitebit-sdk-1.0.3/
--rw-r--r--   0 Artur      (502) staff       (20)     1075 2023-04-20 07:31:18.000000 python-whitebit-sdk-1.0.3/LICENSE
--rw-r--r--   0 Artur      (502) staff       (20)     4605 2023-04-20 12:09:00.683446 python-whitebit-sdk-1.0.3/PKG-INFO
--rw-r--r--   0 Artur      (502) staff       (20)     3813 2023-04-20 10:31:11.000000 python-whitebit-sdk-1.0.3/README.md
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.679431 python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/
--rw-r--r--   0 Artur      (502) staff       (20)     4605 2023-04-20 12:09:00.000000 python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/PKG-INFO
--rw-r--r--   0 Artur      (502) staff       (20)      932 2023-04-20 12:09:00.000000 python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 Artur      (502) staff       (20)        1 2023-04-20 12:09:00.000000 python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 Artur      (502) staff       (20)      107 2023-04-20 12:09:00.000000 python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/requires.txt
--rw-r--r--   0 Artur      (502) staff       (20)        9 2023-04-20 12:09:00.000000 python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/top_level.txt
--rw-r--r--   0 Artur      (502) staff       (20)       38 2023-04-20 12:09:00.683640 python-whitebit-sdk-1.0.3/setup.cfg
--rwxr-xr-x   0 Artur      (502) staff       (20)     5623 2023-04-20 12:08:52.000000 python-whitebit-sdk-1.0.3/setup.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.679770 python-whitebit-sdk-1.0.3/whitebit/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:08:18.000000 python-whitebit-sdk-1.0.3/whitebit/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)      109 2023-04-20 12:08:52.000000 python-whitebit-sdk-1.0.3/whitebit/__version__.py
--rw-r--r--   0 Artur      (502) staff       (20)     3193 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/client.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.680013 python-whitebit-sdk-1.0.3/whitebit/collateral/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:08:18.000000 python-whitebit-sdk-1.0.3/whitebit/collateral/__init__.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.680232 python-whitebit-sdk-1.0.3/whitebit/collateral/account/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/collateral/account/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)     2261 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/collateral/account/account.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.680643 python-whitebit-sdk-1.0.3/whitebit/collateral/market/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/collateral/market/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)      481 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/collateral/market/market.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.680966 python-whitebit-sdk-1.0.3/whitebit/collateral/order/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/collateral/order/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)     3347 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/collateral/order/order.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.681222 python-whitebit-sdk-1.0.3/whitebit/main/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:08:18.000000 python-whitebit-sdk-1.0.3/whitebit/main/__init__.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.681444 python-whitebit-sdk-1.0.3/whitebit/main/account/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/main/account/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)     3645 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/main/account/account.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.681736 python-whitebit-sdk-1.0.3/whitebit/stream/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/stream/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)    21217 2023-04-19 15:02:27.000000 python-whitebit-sdk-1.0.3/whitebit/stream/ws.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.682201 python-whitebit-sdk-1.0.3/whitebit/trade/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:08:18.000000 python-whitebit-sdk-1.0.3/whitebit/trade/__init__.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.682480 python-whitebit-sdk-1.0.3/whitebit/trade/account/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/trade/account/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)     3217 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/trade/account/account.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.682850 python-whitebit-sdk-1.0.3/whitebit/trade/market/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/trade/market/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)     3437 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/trade/market/market.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.683149 python-whitebit-sdk-1.0.3/whitebit/trade/order/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/trade/order/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)     2862 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/trade/order/order.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:40:42.002768 python-whitebit-sdk-1.0.4/
+-rw-r--r--   0 Artur      (502) staff       (20)     1075 2023-04-20 07:31:18.000000 python-whitebit-sdk-1.0.4/LICENSE
+-rw-r--r--   0 Artur      (502) staff       (20)     4605 2023-04-20 12:40:42.002632 python-whitebit-sdk-1.0.4/PKG-INFO
+-rw-r--r--   0 Artur      (502) staff       (20)     3813 2023-04-20 10:31:11.000000 python-whitebit-sdk-1.0.4/README.md
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:40:41.997882 python-whitebit-sdk-1.0.4/python_whitebit_sdk.egg-info/
+-rw-r--r--   0 Artur      (502) staff       (20)     4605 2023-04-20 12:40:41.000000 python-whitebit-sdk-1.0.4/python_whitebit_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 Artur      (502) staff       (20)      932 2023-04-20 12:40:41.000000 python-whitebit-sdk-1.0.4/python_whitebit_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 Artur      (502) staff       (20)        1 2023-04-20 12:40:41.000000 python-whitebit-sdk-1.0.4/python_whitebit_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 Artur      (502) staff       (20)      107 2023-04-20 12:40:41.000000 python-whitebit-sdk-1.0.4/python_whitebit_sdk.egg-info/requires.txt
+-rw-r--r--   0 Artur      (502) staff       (20)        9 2023-04-20 12:40:41.000000 python-whitebit-sdk-1.0.4/python_whitebit_sdk.egg-info/top_level.txt
+-rw-r--r--   0 Artur      (502) staff       (20)       38 2023-04-20 12:40:42.002808 python-whitebit-sdk-1.0.4/setup.cfg
+-rwxr-xr-x   0 Artur      (502) staff       (20)     5623 2023-04-20 12:08:52.000000 python-whitebit-sdk-1.0.4/setup.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:40:41.998339 python-whitebit-sdk-1.0.4/whitebit/
+-rw-r--r--   0 Artur      (502) staff       (20)       89 2023-04-20 12:40:12.000000 python-whitebit-sdk-1.0.4/whitebit/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)      109 2023-04-20 12:40:20.000000 python-whitebit-sdk-1.0.4/whitebit/__version__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     3193 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.4/whitebit/client.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:40:41.998576 python-whitebit-sdk-1.0.4/whitebit/collateral/
+-rw-r--r--   0 Artur      (502) staff       (20)       66 2023-04-20 12:40:12.000000 python-whitebit-sdk-1.0.4/whitebit/collateral/__init__.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:40:41.999015 python-whitebit-sdk-1.0.4/whitebit/collateral/account/
+-rw-r--r--   0 Artur      (502) staff       (20)       23 2023-04-20 12:40:12.000000 python-whitebit-sdk-1.0.4/whitebit/collateral/account/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     2261 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.4/whitebit/collateral/account/account.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:40:41.999389 python-whitebit-sdk-1.0.4/whitebit/collateral/market/
+-rw-r--r--   0 Artur      (502) staff       (20)       22 2023-04-20 12:40:12.000000 python-whitebit-sdk-1.0.4/whitebit/collateral/market/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)      481 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.4/whitebit/collateral/market/market.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:40:41.999760 python-whitebit-sdk-1.0.4/whitebit/collateral/order/
+-rw-r--r--   0 Artur      (502) staff       (20)       21 2023-04-20 12:40:12.000000 python-whitebit-sdk-1.0.4/whitebit/collateral/order/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     3347 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.4/whitebit/collateral/order/order.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:40:42.000010 python-whitebit-sdk-1.0.4/whitebit/main/
+-rw-r--r--   0 Artur      (502) staff       (20)       23 2023-04-20 12:40:12.000000 python-whitebit-sdk-1.0.4/whitebit/main/__init__.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:40:42.000393 python-whitebit-sdk-1.0.4/whitebit/main/account/
+-rw-r--r--   0 Artur      (502) staff       (20)       39 2023-04-20 12:35:42.000000 python-whitebit-sdk-1.0.4/whitebit/main/account/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     3645 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.4/whitebit/main/account/account.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:40:42.000752 python-whitebit-sdk-1.0.4/whitebit/stream/
+-rw-r--r--   0 Artur      (502) staff       (20)       33 2023-04-20 12:35:42.000000 python-whitebit-sdk-1.0.4/whitebit/stream/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)    21154 2023-04-20 12:20:57.000000 python-whitebit-sdk-1.0.4/whitebit/stream/ws.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:40:42.001128 python-whitebit-sdk-1.0.4/whitebit/trade/
+-rw-r--r--   0 Artur      (502) staff       (20)      177 2023-04-20 12:34:13.000000 python-whitebit-sdk-1.0.4/whitebit/trade/__init__.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:40:42.001561 python-whitebit-sdk-1.0.4/whitebit/trade/account/
+-rw-r--r--   0 Artur      (502) staff       (20)       40 2023-04-20 12:34:13.000000 python-whitebit-sdk-1.0.4/whitebit/trade/account/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     3217 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.4/whitebit/trade/account/account.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:40:42.002006 python-whitebit-sdk-1.0.4/whitebit/trade/market/
+-rw-r--r--   0 Artur      (502) staff       (20)       37 2023-04-20 12:34:13.000000 python-whitebit-sdk-1.0.4/whitebit/trade/market/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     3315 2023-04-20 12:20:57.000000 python-whitebit-sdk-1.0.4/whitebit/trade/market/market.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:40:42.002396 python-whitebit-sdk-1.0.4/whitebit/trade/order/
+-rw-r--r--   0 Artur      (502) staff       (20)       36 2023-04-20 12:34:13.000000 python-whitebit-sdk-1.0.4/whitebit/trade/order/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     2862 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.4/whitebit/trade/order/order.py
```

### Comparing `python-whitebit-sdk-1.0.3/LICENSE` & `python-whitebit-sdk-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.3/PKG-INFO` & `python-whitebit-sdk-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-whitebit-sdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: Clients and methods to interact with the Whitebit exchange.
 Home-page: https://github.com/whitebit-exchange/python-sdk
 Author: UAB Clear White Technologies
 Author-email: support@whitebit.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `python-whitebit-sdk-1.0.3/README.md` & `python-whitebit-sdk-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/PKG-INFO` & `python-whitebit-sdk-1.0.4/python_whitebit_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-whitebit-sdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: Clients and methods to interact with the Whitebit exchange.
 Home-page: https://github.com/whitebit-exchange/python-sdk
 Author: UAB Clear White Technologies
 Author-email: support@whitebit.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/SOURCES.txt` & `python-whitebit-sdk-1.0.4/python_whitebit_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.3/setup.py` & `python-whitebit-sdk-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.3/whitebit/client.py` & `python-whitebit-sdk-1.0.4/whitebit/client.py`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.3/whitebit/collateral/account/account.py` & `python-whitebit-sdk-1.0.4/whitebit/collateral/account/account.py`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.3/whitebit/collateral/order/order.py` & `python-whitebit-sdk-1.0.4/whitebit/collateral/order/order.py`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.3/whitebit/main/account/account.py` & `python-whitebit-sdk-1.0.4/whitebit/main/account/account.py`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.3/whitebit/stream/ws.py` & `python-whitebit-sdk-1.0.4/whitebit/stream/ws.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-'''Module that implements the kraken Spot websocket clients'''
 import logging
 import json
 import time
 import asyncio
 from enum import Enum
 from random import random
 import traceback
```

### Comparing `python-whitebit-sdk-1.0.3/whitebit/trade/account/account.py` & `python-whitebit-sdk-1.0.4/whitebit/trade/account/account.py`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.3/whitebit/trade/market/market.py` & `python-whitebit-sdk-1.0.4/whitebit/trade/market/market.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-'''Module that implements the Kraken Spot market client'''
 import whitebit
 from whitebit.client import Whitebit
 
 
 class TradeMarketClient(Whitebit):
     __MARKETS_URL = "/api/v2/public/markets"
     __MARKET_ACTIVITY_URL = "/api/v2/public/ticker"
@@ -15,16 +14,14 @@
     __FEE_LIST_URL = "/api/v4/public/fee"
     __DEPTH_URL = "/api/v2/public/depth/"
     __ORDERBOOK_URL = "/api/v4/public/orderbook/"
     __DEALS_URL = "/api/v4/public/trades/"
     __TRADE_HISTORY_URL = "/api/v1/public/history"
     __ASSETS_URL = "/api/v4/public/assets"
 
-    '''Class that implements the Kraken Spot market client'''
-
     def __init__(self, api_key: str = '', api_secret: str = ''):
         super().__init__(api_key, api_secret)
 
     def get_markets_info(self):
         return self._request(method='GET', uri=self.__MARKETS_URL, auth=False)
 
     def get_tickers(self):
```

### Comparing `python-whitebit-sdk-1.0.3/whitebit/trade/order/order.py` & `python-whitebit-sdk-1.0.4/whitebit/trade/order/order.py`

 * *Files identical despite different names*

