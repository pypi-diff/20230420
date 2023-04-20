# Comparing `tmp/adata-0.0.3b0.tar.gz` & `tmp/adata-0.0.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adata-0.0.3b0.tar", last modified: Wed Apr 19 16:00:43 2023, max compression
+gzip compressed data, was "adata-0.0.4b0.tar", last modified: Thu Apr 20 16:20:11 2023, max compression
```

## Comparing `adata-0.0.3b0.tar` & `adata-0.0.4b0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.931081 adata-0.0.3b0/
--rw-rw-rw-   0        0        0      186 2023-04-06 11:14:06.000000 adata-0.0.3b0/HISTORY.md
--rw-rw-rw-   0        0        0    11558 2023-04-05 02:53:34.000000 adata-0.0.3b0/LICENSE
--rw-rw-rw-   0        0        0       27 2023-04-06 11:14:06.000000 adata-0.0.3b0/MANIFEST.in
--rw-rw-rw-   0        0        0     6780 2023-04-19 16:00:43.930106 adata-0.0.3b0/PKG-INFO
--rw-rw-rw-   0        0        0     6141 2023-04-18 15:14:02.000000 adata-0.0.3b0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.776573 adata-0.0.3b0/adata/
--rw-rw-rw-   0        0        0      545 2023-04-05 04:59:22.000000 adata-0.0.3b0/adata/__init__.py
--rw-rw-rw-   0        0        0      756 2023-04-19 15:43:41.000000 adata-0.0.3b0/adata/__version__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.789563 adata-0.0.3b0/adata/bond/
--rw-rw-rw-   0        0        0      122 2023-04-06 11:14:06.000000 adata-0.0.3b0/adata/bond/__init__.py
--rw-rw-rw-   0        0        0      203 2023-04-05 09:48:31.000000 adata-0.0.3b0/adata/bond/bond_market.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.790563 adata-0.0.3b0/adata/common/
--rw-rw-rw-   0        0        0      150 2023-04-05 09:48:31.000000 adata-0.0.3b0/adata/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.797563 adata-0.0.3b0/adata/common/headers/
--rw-rw-rw-   0        0        0      104 2023-04-05 09:48:30.000000 adata-0.0.3b0/adata/common/headers/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-05 09:48:28.000000 adata-0.0.3b0/adata/common/headers/baidu_headers.py
--rw-rw-rw-   0        0        0      602 2023-04-18 15:14:02.000000 adata-0.0.3b0/adata/common/headers/sina_headers.py
--rw-rw-rw-   0        0        0     2999 2023-04-05 09:48:30.000000 adata-0.0.3b0/adata/common/headers/ths_headers.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.907106 adata-0.0.3b0/adata/common/utils/
--rw-rw-rw-   0        0        0      205 2023-04-05 09:53:12.000000 adata-0.0.3b0/adata/common/utils/__init__.py
--rw-rw-rw-   0        0        0     3046 2023-04-05 09:48:27.000000 adata-0.0.3b0/adata/common/utils/snowflake.py
--rw-rw-rw-   0        0        0      972 2023-04-19 14:58:23.000000 adata-0.0.3b0/adata/common/utils/sunrequests.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.910106 adata-0.0.3b0/adata/etf/
--rw-rw-rw-   0        0        0      118 2023-04-06 11:14:06.000000 adata-0.0.3b0/adata/etf/__init__.py
--rw-rw-rw-   0        0        0      201 2023-04-05 09:48:28.000000 adata-0.0.3b0/adata/etf/etf_market.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.912106 adata-0.0.3b0/adata/message/
--rw-rw-rw-   0        0        0      103 2023-04-05 09:48:30.000000 adata-0.0.3b0/adata/message/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.913106 adata-0.0.3b0/adata/stock/
--rw-rw-rw-   0        0        0      333 2023-04-06 11:14:06.000000 adata-0.0.3b0/adata/stock/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.915106 adata-0.0.3b0/adata/stock/index/
--rw-rw-rw-   0        0        0      105 2023-04-06 11:14:06.000000 adata-0.0.3b0/adata/stock/index/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.919106 adata-0.0.3b0/adata/stock/info/
--rw-rw-rw-   0        0        0      322 2023-04-13 14:47:15.000000 adata-0.0.3b0/adata/stock/info/__init__.py
--rw-rw-rw-   0        0        0     2524 2023-04-19 14:07:29.000000 adata-0.0.3b0/adata/stock/info/stock_code.py
--rw-rw-rw-   0        0        0     4193 2023-04-19 14:07:29.000000 adata-0.0.3b0/adata/stock/info/stock_concept.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.927139 adata-0.0.3b0/adata/stock/market/
--rw-rw-rw-   0        0        0      408 2023-04-13 14:47:15.000000 adata-0.0.3b0/adata/stock/market/__init__.py
--rw-rw-rw-   0        0        0     2710 2023-04-19 14:07:29.000000 adata-0.0.3b0/adata/stock/market/stock_dividend.py
--rw-rw-rw-   0        0        0     9769 2023-04-19 15:40:50.000000 adata-0.0.3b0/adata/stock/market/stock_market.py
--rw-rw-rw-   0        0        0     5740 2023-04-19 15:24:26.000000 adata-0.0.3b0/adata/stock/market/stock_market_concept.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.928107 adata-0.0.3b0/adata/stock/sentiment/
--rw-rw-rw-   0        0        0      115 2023-04-06 11:14:06.000000 adata-0.0.3b0/adata/stock/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.785563 adata-0.0.3b0/adata.egg-info/
--rw-rw-rw-   0        0        0     6780 2023-04-19 16:00:43.000000 adata-0.0.3b0/adata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      964 2023-04-19 16:00:43.000000 adata-0.0.3b0/adata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 16:00:43.000000 adata-0.0.3b0/adata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-19 16:00:43.000000 adata-0.0.3b0/adata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 16:00:43.000000 adata-0.0.3b0/adata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       69 2023-04-06 11:14:06.000000 adata-0.0.3b0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 16:00:43.931081 adata-0.0.3b0/setup.cfg
--rw-rw-rw-   0        0        0     1790 2023-04-18 15:37:51.000000 adata-0.0.3b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.120330 adata-0.0.4b0/
+-rw-rw-rw-   0        0        0      186 2023-04-06 11:14:06.000000 adata-0.0.4b0/HISTORY.md
+-rw-rw-rw-   0        0        0    11558 2023-04-05 02:53:34.000000 adata-0.0.4b0/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-04-06 11:14:06.000000 adata-0.0.4b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6780 2023-04-20 16:20:11.120330 adata-0.0.4b0/PKG-INFO
+-rw-rw-rw-   0        0        0     6141 2023-04-18 15:14:02.000000 adata-0.0.4b0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.070330 adata-0.0.4b0/adata/
+-rw-rw-rw-   0        0        0      545 2023-04-05 04:59:22.000000 adata-0.0.4b0/adata/__init__.py
+-rw-rw-rw-   0        0        0      756 2023-04-20 16:19:38.000000 adata-0.0.4b0/adata/__version__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.080331 adata-0.0.4b0/adata/bond/
+-rw-rw-rw-   0        0        0      122 2023-04-06 11:14:06.000000 adata-0.0.4b0/adata/bond/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-04-05 09:48:31.000000 adata-0.0.4b0/adata/bond/bond_market.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.080331 adata-0.0.4b0/adata/common/
+-rw-rw-rw-   0        0        0      150 2023-04-05 09:48:31.000000 adata-0.0.4b0/adata/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.090330 adata-0.0.4b0/adata/common/headers/
+-rw-rw-rw-   0        0        0      104 2023-04-05 09:48:30.000000 adata-0.0.4b0/adata/common/headers/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-05 09:48:28.000000 adata-0.0.4b0/adata/common/headers/baidu_headers.py
+-rw-rw-rw-   0        0        0      602 2023-04-18 15:14:02.000000 adata-0.0.4b0/adata/common/headers/sina_headers.py
+-rw-rw-rw-   0        0        0     2999 2023-04-05 09:48:30.000000 adata-0.0.4b0/adata/common/headers/ths_headers.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.090330 adata-0.0.4b0/adata/common/utils/
+-rw-rw-rw-   0        0        0      205 2023-04-05 09:53:12.000000 adata-0.0.4b0/adata/common/utils/__init__.py
+-rw-rw-rw-   0        0        0     3046 2023-04-05 09:48:27.000000 adata-0.0.4b0/adata/common/utils/snowflake.py
+-rw-rw-rw-   0        0        0      972 2023-04-19 14:58:23.000000 adata-0.0.4b0/adata/common/utils/sunrequests.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.100330 adata-0.0.4b0/adata/etf/
+-rw-rw-rw-   0        0        0      118 2023-04-06 11:14:06.000000 adata-0.0.4b0/adata/etf/__init__.py
+-rw-rw-rw-   0        0        0      201 2023-04-05 09:48:28.000000 adata-0.0.4b0/adata/etf/etf_market.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.100330 adata-0.0.4b0/adata/message/
+-rw-rw-rw-   0        0        0      103 2023-04-05 09:48:30.000000 adata-0.0.4b0/adata/message/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.100330 adata-0.0.4b0/adata/stock/
+-rw-rw-rw-   0        0        0      333 2023-04-06 11:14:06.000000 adata-0.0.4b0/adata/stock/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.100330 adata-0.0.4b0/adata/stock/index/
+-rw-rw-rw-   0        0        0      105 2023-04-06 11:14:06.000000 adata-0.0.4b0/adata/stock/index/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.110330 adata-0.0.4b0/adata/stock/info/
+-rw-rw-rw-   0        0        0      322 2023-04-13 14:47:15.000000 adata-0.0.4b0/adata/stock/info/__init__.py
+-rw-rw-rw-   0        0        0     2524 2023-04-19 14:07:29.000000 adata-0.0.4b0/adata/stock/info/stock_code.py
+-rw-rw-rw-   0        0        0     4193 2023-04-19 14:07:29.000000 adata-0.0.4b0/adata/stock/info/stock_concept.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.110330 adata-0.0.4b0/adata/stock/market/
+-rw-rw-rw-   0        0        0      408 2023-04-13 14:47:15.000000 adata-0.0.4b0/adata/stock/market/__init__.py
+-rw-rw-rw-   0        0        0     2941 2023-04-20 13:03:47.000000 adata-0.0.4b0/adata/stock/market/stock_dividend.py
+-rw-rw-rw-   0        0        0    10288 2023-04-20 13:12:32.000000 adata-0.0.4b0/adata/stock/market/stock_market.py
+-rw-rw-rw-   0        0        0     5740 2023-04-19 15:24:26.000000 adata-0.0.4b0/adata/stock/market/stock_market_concept.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.120330 adata-0.0.4b0/adata/stock/sentiment/
+-rw-rw-rw-   0        0        0      115 2023-04-06 11:14:06.000000 adata-0.0.4b0/adata/stock/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.080331 adata-0.0.4b0/adata.egg-info/
+-rw-rw-rw-   0        0        0     6780 2023-04-20 16:20:10.000000 adata-0.0.4b0/adata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      964 2023-04-20 16:20:10.000000 adata-0.0.4b0/adata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 16:20:10.000000 adata-0.0.4b0/adata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-20 16:20:10.000000 adata-0.0.4b0/adata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 16:20:10.000000 adata-0.0.4b0/adata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       69 2023-04-06 11:14:06.000000 adata-0.0.4b0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 16:20:11.120330 adata-0.0.4b0/setup.cfg
+-rw-rw-rw-   0        0        0     1790 2023-04-18 15:37:51.000000 adata-0.0.4b0/setup.py
```

### Comparing `adata-0.0.3b0/LICENSE` & `adata-0.0.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `adata-0.0.3b0/PKG-INFO` & `adata-0.0.4b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata
-Version: 0.0.3b0
+Version: 0.0.4b0
 Summary: A Data,A Stock,ETF,Bond,Quant
 Home-page: https://gitee.com/inchaos/adata
 Author: 1nchaos
 Author-email: 9527@1nchaos.com
 License: Apache License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `adata-0.0.3b0/README.md` & `adata-0.0.4b0/README.md`

 * *Files identical despite different names*

### Comparing `adata-0.0.3b0/adata/__init__.py` & `adata-0.0.4b0/adata/__init__.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.3b0/adata/__version__.py` & `adata-0.0.4b0/adata/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-VERSION = (0, 0, 3)
+VERSION = (0, 0, 4)
 # PRERELEASE = None  # alpha, beta or rc
 PRERELEASE = 'beta'  # alpha, beta or rc
 REVISION = None
 
 
 def generate_version(version, prerelease=None, revision=None):
     version_parts = [".".join(map(str, version))]
```

### Comparing `adata-0.0.3b0/adata/common/headers/baidu_headers.py` & `adata-0.0.4b0/adata/common/headers/baidu_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.3b0/adata/common/headers/sina_headers.py` & `adata-0.0.4b0/adata/common/headers/sina_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.3b0/adata/common/headers/ths_headers.py` & `adata-0.0.4b0/adata/common/headers/ths_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.3b0/adata/common/utils/snowflake.py` & `adata-0.0.4b0/adata/common/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.3b0/adata/common/utils/sunrequests.py` & `adata-0.0.4b0/adata/common/utils/sunrequests.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.3b0/adata/stock/info/stock_code.py` & `adata-0.0.4b0/adata/stock/info/stock_code.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.3b0/adata/stock/info/stock_concept.py` & `adata-0.0.4b0/adata/stock/info/stock_concept.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.3b0/adata/stock/market/stock_dividend.py` & `adata-0.0.4b0/adata/stock/market/stock_dividend.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,37 +34,43 @@
         """
         获取百度的股票分红数据：公告日；分红方案；除权除息日
         web： https://gushitong.baidu.com/stock/ab-300033
         url： https://gushitong.baidu.com/opendata?openapi=1&dspName=iphone&tn=tangram&client=app&query=300033&code=300033&word=300033&resource_id=5429&ma_ver=4&finClientType=pc
         :param stock_code: 6位股票代码
         :return: 股票分红信息
         """
+        columns = ['report_date', 'dividend_plan', 'ex_dividend_date']
+        null_df = pd.DataFrame(data=[], columns=columns)
         # 1.请求接口 url
         api_url = f"https://gushitong.baidu.com/opendata?openapi=1&dspName=iphone&tn=tangram&client=app&" \
                   f"query={stock_code}&code={stock_code}&word={stock_code}&resource_id=5429&ma_ver=4&finClientType=pc"
         res = requests.request('get', api_url, headers=baidu_headers.text_headers)
 
         # 2. 判断结果是否正确
         if len(res.text) < 1 or res.status_code != 200:
             return pd.DataFrame()
         res_json = res.json()
         if res_json['ResultCode'] != '0':
-            return pd.DataFrame()
+            return null_df
         # 3.解析数据
         # 3.1 空数据时返回为空
         result = res_json['Result']
         if not result:
-            return pd.DataFrame()
+            return null_df
 
         # 3.2 正常解析数据 basicInfo,shareholderEquity,organRating,executiveInfo,bonusTransfer
-        new_company = result[-1]['DisplayData']['resultData']['tplData']['result']['tabs'][-1]['content'][
-            'newCompany']
-        bonus_transfer = new_company['bonusTransfer']
-        header = bonus_transfer['header']
-        body = bonus_transfer['body']
+        try:
+            new_company = result[-1]['DisplayData']['resultData']['tplData']['result']['tabs'][-1]['content'][
+                'newCompany']
+            bonus_transfer = new_company['bonusTransfer']
+            header = bonus_transfer['header']
+            body = bonus_transfer['body']
+        except KeyError:
+            # TODO logger
+            return null_df
 
         # 4. 封装数据
         result_df = pd.DataFrame(data=body, columns=header)[['公告日', '分红方案', '除权除息日']]
         result_df['stock_code'] = stock_code
         rename_columns = {'公告日': 'report_date', '分红方案': 'dividend_plan', '除权除息日': 'ex_dividend_date'}
         return result_df.rename(columns=rename_columns)
```

### Comparing `adata-0.0.3b0/adata/stock/market/stock_market.py` & `adata-0.0.4b0/adata/stock/market/stock_market.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 from adata.common.utils import requests
 
 
 class StockMarket(object):
     """
     股票行情
     """
+    MARKET_COLUMNS = ['trade_time', 'open', 'close', 'volume', 'high', 'low', 'amount', 'change', 'change_pct',
+                      'turnover_ratio', 'pre_close']
+    MARKET_MIN_COLUMNS = ['stock_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount']
+    MARKET_CURRENT_COLUMNS = ['stock_code', 'short_name', 'price', 'change', 'change_pct', 'volume', 'amount']
 
     def __init__(self) -> None:
         super().__init__()
 
     def get_market(self, stock_code: str = '000001', start_date='1990-01-01', k_type=1, adjust_type: int = 1):
         """
         获取单个股票的行情
@@ -80,33 +84,35 @@
             if res_json['ResultCode'] == '0':
                 break
             time.sleep(2)
         # 3.解析数据
         # 3.1 空数据时返回为空
         result = res_json['Result']
         if not result:
-            return pd.DataFrame()
+            return pd.DataFrame(data=[], columns=self.MARKET_COLUMNS)
 
         # 3.2. 正常解析数据
         keys = res_json['Result']['newMarketData']['keys']
         market_data = res_json['Result']['newMarketData']['marketData']
         market_data_list = str(market_data).split(';')
         data = []
         for one in market_data_list:
             data.append(one.split(','))
 
         # 4. 封装数据
-        field = ['time', 'open', 'close', 'volume', 'high', 'low', 'amount', 'range', 'ratio', 'turnoverratio',
-                 'preClose']
         rename_columns = {'turnoverratio': 'turnover_ratio', 'preClose': 'pre_close', 'range': 'change',
                           'ratio': 'change_pct', 'time': 'trade_time'}
-        result_df = pd.DataFrame(data=data, columns=keys)[field].rename(columns=rename_columns)
+        result_df = pd.DataFrame(data=data, columns=keys).rename(columns=rename_columns)[self.MARKET_COLUMNS]
         result_df['stock_code'] = stock_code
         result_df['trade_date'] = result_df['trade_time']
         result_df['trade_time'] = pd.to_datetime(result_df['trade_time']).dt.strftime('%Y-%m-%d %H:%M:%S')
+        result_df.replace('--', None, inplace=True)
+        result_df.replace('', None, inplace=True)
+        result_df['change'] = result_df['change'].str.replace('+', '', regex=True)
+        result_df['change_pct'] = result_df['change_pct'].str.replace('+', '', regex=True)
         return result_df
 
     def __market_baidu_today_min(self, stock_code):
         """
         获取百度的股票行情数据
         web： https://gushitong.baidu.com/stock/ab-002926
         url: https://finance.pae.baidu.com/selfselect/getstockquotation?all=1&code=601318&isIndex=false&isBk=false&isBlock=false&isFutures=false&isStock=true&newFormat=1&group=quotation_minute_ab&finClientType=pc
@@ -127,15 +133,15 @@
             if res_json['ResultCode'] == '0':
                 break
             time.sleep(2)
         # 3.解析数据
         # 3.1 空数据时返回为空
         result = res_json['Result']
         if not result:
-            return pd.DataFrame()
+            return pd.DataFrame(data=[], columns=self.MARKET_MIN_COLUMNS)
 
         # 3.2. 正常解析数据
         market_data_list = res_json['Result']['priceinfo']
 
         # 4. 封装数据
         field = ['time', 'price', 'ratio', 'increase', 'volume', 'avgPrice', 'amount', 'timeKey', 'datetime',
                  'oriAmount']
@@ -146,15 +152,15 @@
         result_df['stock_code'] = stock_code
         # 这里是分钟均价，数据存在四舍五入的情况
         result_df['volume'] = result_df['volume'].astype(int) * 100
         result_df['trade_time'] = pd.to_datetime(result_df['time'], unit='s', utc=True).dt.tz_convert(
             'Asia/Shanghai')
         result_df['trade_time'] = pd.to_datetime(result_df['trade_time']).dt.strftime("%Y-%m-%d %H:%M:%S")
         result_df['trade_date'] = result_df['trade_time'].str[:10]
-        return result_df[['stock_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount']]
+        return result_df[self.MARKET_MIN_COLUMNS]
 
     def __market_sina_current(self, code_list):
         """
         获取新浪的最新股票行情
         url : https://hq.sinajs.cn/list=s_sh600905,s_sz000725,s_sz000100,s_sh601919
         :param code_list:  代码列表
         :return: 最新行情数据：代码,简称,当前价格(元),涨跌额(元),涨跌幅(%),成交量(股),成交额(元)
@@ -170,15 +176,15 @@
                 api_url += 's_bj' + code + ','
 
         # 1.请求接口
         res = requests.request('get', api_url, headers=sina_headers.c_headers)
 
         # 2. 判断结果是否正确
         if len(res.text) < 1 or res.status_code != 200:
-            return pd.DataFrame()
+            return pd.DataFrame(data=[], columns=self.MARKET_CURRENT_COLUMNS)
         # 3.解析数据
 
         # 正常解析数据 var hq_str_s_bj872925="平安银行,14.840,0.480,3.343,374847,5483780.180";
         data_list = res.text.split(';')
         data = []
         for data_str in data_list:
             if len(data_str) < 8:
@@ -186,16 +192,15 @@
             idx = data_str.index('=')
             code = [data_str[idx - 6:idx]]
             code.extend(data_str[idx + 2:-1].split(','))
             if len(code) == 7:
                 data.append(code)
 
         # 4. 封装数据
-        columns = ['stock_code', 'short_name', 'price', 'change', 'change_pct', 'volume', 'amount']
-        result_df = pd.DataFrame(data=data, columns=columns)
+        result_df = pd.DataFrame(data=data, columns=self.MARKET_CURRENT_COLUMNS)
         # 北京的单位是股和万元
         mask = result_df['stock_code'].str.startswith(('0', '3', '6', '9'))
         result_df.loc[mask, 'volume'] = result_df['volume'].astype(int) * 100
         result_df.loc[mask, 'amount'] = result_df['amount'].astype(float) * 10000
         return result_df
```

### Comparing `adata-0.0.3b0/adata/stock/market/stock_market_concept.py` & `adata-0.0.4b0/adata/stock/market/stock_market_concept.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.3b0/adata.egg-info/PKG-INFO` & `adata-0.0.4b0/adata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata
-Version: 0.0.3b0
+Version: 0.0.4b0
 Summary: A Data,A Stock,ETF,Bond,Quant
 Home-page: https://gitee.com/inchaos/adata
 Author: 1nchaos
 Author-email: 9527@1nchaos.com
 License: Apache License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `adata-0.0.3b0/adata.egg-info/SOURCES.txt` & `adata-0.0.4b0/adata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adata-0.0.3b0/setup.py` & `adata-0.0.4b0/setup.py`

 * *Files identical despite different names*

