# Comparing `tmp/tradingeconomics-4.2.2.tar.gz` & `tmp/tradingeconomics-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingeconomics-4.2.2.tar", last modified: Mon Mar 27 12:34:07 2023, max compression
+gzip compressed data, was "tradingeconomics-4.2.3.tar", last modified: Thu Apr 20 12:38:19 2023, max compression
```

## Comparing `tradingeconomics-4.2.2.tar` & `tradingeconomics-4.2.3.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 12:34:07.709241 tradingeconomics-4.2.2/
--rw-rw-rw-   0        0        0     1070 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0       18 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1547 2023-03-27 12:34:07.711229 tradingeconomics-4.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1597 2023-02-03 17:45:07.000000 tradingeconomics-4.2.2/README.md
--rw-rw-rw-   0        0        0      824 2023-02-03 17:45:07.000000 tradingeconomics-4.2.2/README.rst
--rw-rw-rw-   0        0        0       86 2023-03-27 12:34:07.722795 tradingeconomics-4.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-03-27 12:33:49.000000 tradingeconomics-4.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-27 12:34:07.596997 tradingeconomics-4.2.2/tradingeconomics/
--rw-rw-rw-   0        0        0     3616 2023-02-06 07:03:16.000000 tradingeconomics-4.2.2/tradingeconomics/__init__.py
--rw-rw-rw-   0        0        0    10861 2023-02-06 07:34:50.000000 tradingeconomics-4.2.2/tradingeconomics/calendar.py
--rw-rw-rw-   0        0        0    18335 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/tradingeconomics/comtrade.py
--rw-rw-rw-   0        0        0     4041 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/tradingeconomics/earnings.py
--rw-rw-rw-   0        0        0     7002 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/tradingeconomics/eurostat.py
--rw-rw-rw-   0        0        0    12372 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/tradingeconomics/federalReserve.py
--rw-rw-rw-   0        0        0     5532 2023-03-23 14:17:08.000000 tradingeconomics-4.2.2/tradingeconomics/financials.py
--rw-rw-rw-   0        0        0     5244 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/tradingeconomics/forecasts.py
--rw-rw-rw-   0        0        0     8634 2023-01-25 08:32:53.000000 tradingeconomics-4.2.2/tradingeconomics/functions.py
--rw-rw-rw-   0        0        0     1234 2023-02-03 17:45:07.000000 tradingeconomics-4.2.2/tradingeconomics/glob.py
--rw-rw-rw-   0        0        0    13237 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/tradingeconomics/historical.py
--rw-rw-rw-   0        0        0     4509 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/tradingeconomics/historicalDB.py
--rw-rw-rw-   0        0        0     3073 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/tradingeconomics/historicalEurostat.py
--rw-rw-rw-   0        0        0     2702 2023-02-06 07:05:48.000000 tradingeconomics-4.2.2/tradingeconomics/historicalFinancials.py
--rw-rw-rw-   0        0        0     4185 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/tradingeconomics/historicalMarkets.py
--rw-rw-rw-   0        0        0    16263 2023-03-23 14:19:39.000000 tradingeconomics-4.2.2/tradingeconomics/indicators.py
--rw-rw-rw-   0        0        0    22232 2023-03-23 14:18:15.000000 tradingeconomics-4.2.2/tradingeconomics/markets.py
--rw-rw-rw-   0        0        0    13802 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/tradingeconomics/news.py
--rw-rw-rw-   0        0        0     2243 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/tradingeconomics/search.py
--rw-rw-rw-   0        0        0     1969 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/tradingeconomics/stream.py
--rw-rw-rw-   0        0        0     9449 2022-11-21 15:26:59.000000 tradingeconomics-4.2.2/tradingeconomics/worldBank.py
-drwxrwxrwx   0        0        0        0 2023-03-27 12:34:07.702294 tradingeconomics-4.2.2/tradingeconomics.egg-info/
--rw-rw-rw-   0        0        0     1547 2023-03-27 12:34:06.000000 tradingeconomics-4.2.2/tradingeconomics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      908 2023-03-27 12:34:07.000000 tradingeconomics-4.2.2/tradingeconomics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 12:34:06.000000 tradingeconomics-4.2.2/tradingeconomics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-03-27 12:34:06.000000 tradingeconomics-4.2.2/tradingeconomics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-03-27 12:34:06.000000 tradingeconomics-4.2.2/tradingeconomics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 12:38:19.092090 tradingeconomics-4.2.3/
+-rw-rw-rw-   0        0        0     1070 2022-11-17 11:38:47.000000 tradingeconomics-4.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       18 2022-11-17 11:38:47.000000 tradingeconomics-4.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1570 2023-04-20 12:38:19.092090 tradingeconomics-4.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2023-03-21 14:47:23.000000 tradingeconomics-4.2.3/README.rst
+-rw-rw-rw-   0        0        0       86 2023-04-20 12:38:19.093089 tradingeconomics-4.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2023-04-20 12:38:03.000000 tradingeconomics-4.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:38:19.068090 tradingeconomics-4.2.3/tradingeconomics/
+-rw-rw-rw-   0        0        0     3627 2023-04-06 19:59:28.000000 tradingeconomics-4.2.3/tradingeconomics/__init__.py
+-rw-rw-rw-   0        0        0    10861 2023-03-21 14:47:23.000000 tradingeconomics-4.2.3/tradingeconomics/calendar.py
+-rw-rw-rw-   0        0        0    16631 2023-04-06 19:59:28.000000 tradingeconomics-4.2.3/tradingeconomics/comtrade.py
+-rw-rw-rw-   0        0        0     4113 2023-04-17 20:25:53.000000 tradingeconomics-4.2.3/tradingeconomics/earnings.py
+-rw-rw-rw-   0        0        0     7002 2022-11-17 11:38:47.000000 tradingeconomics-4.2.3/tradingeconomics/eurostat.py
+-rw-rw-rw-   0        0        0    12372 2022-11-17 11:38:47.000000 tradingeconomics-4.2.3/tradingeconomics/federalReserve.py
+-rw-rw-rw-   0        0        0     5532 2023-04-06 19:59:28.000000 tradingeconomics-4.2.3/tradingeconomics/financials.py
+-rw-rw-rw-   0        0        0     5244 2022-11-17 11:38:47.000000 tradingeconomics-4.2.3/tradingeconomics/forecasts.py
+-rw-rw-rw-   0        0        0     8630 2023-04-17 21:24:33.000000 tradingeconomics-4.2.3/tradingeconomics/functions.py
+-rw-rw-rw-   0        0        0     1234 2023-03-21 14:47:23.000000 tradingeconomics-4.2.3/tradingeconomics/glob.py
+-rw-rw-rw-   0        0        0    13237 2022-11-17 11:38:47.000000 tradingeconomics-4.2.3/tradingeconomics/historical.py
+-rw-rw-rw-   0        0        0     4509 2022-11-17 11:38:47.000000 tradingeconomics-4.2.3/tradingeconomics/historicalDB.py
+-rw-rw-rw-   0        0        0     3073 2022-11-17 11:38:47.000000 tradingeconomics-4.2.3/tradingeconomics/historicalEurostat.py
+-rw-rw-rw-   0        0        0     2702 2023-03-21 14:47:23.000000 tradingeconomics-4.2.3/tradingeconomics/historicalFinancials.py
+-rw-rw-rw-   0        0        0     4185 2022-11-17 11:38:47.000000 tradingeconomics-4.2.3/tradingeconomics/historicalMarkets.py
+-rw-rw-rw-   0        0        0    16263 2023-04-06 19:59:28.000000 tradingeconomics-4.2.3/tradingeconomics/indicators.py
+-rw-rw-rw-   0        0        0    22232 2023-04-06 19:59:28.000000 tradingeconomics-4.2.3/tradingeconomics/markets.py
+-rw-rw-rw-   0        0        0    13802 2022-11-17 11:38:47.000000 tradingeconomics-4.2.3/tradingeconomics/news.py
+-rw-rw-rw-   0        0        0     2243 2022-11-17 11:38:47.000000 tradingeconomics-4.2.3/tradingeconomics/search.py
+-rw-rw-rw-   0        0        0     1969 2022-11-17 11:38:47.000000 tradingeconomics-4.2.3/tradingeconomics/stream.py
+-rw-rw-rw-   0        0        0     9449 2022-11-17 11:38:47.000000 tradingeconomics-4.2.3/tradingeconomics/worldBank.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:38:19.091088 tradingeconomics-4.2.3/tradingeconomics.egg-info/
+-rw-rw-rw-   0        0        0     1570 2023-04-20 12:38:18.000000 tradingeconomics-4.2.3/tradingeconomics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      898 2023-04-20 12:38:18.000000 tradingeconomics-4.2.3/tradingeconomics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 12:38:18.000000 tradingeconomics-4.2.3/tradingeconomics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-20 12:38:18.000000 tradingeconomics-4.2.3/tradingeconomics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-20 12:38:18.000000 tradingeconomics-4.2.3/tradingeconomics.egg-info/top_level.txt
```

### Comparing `tradingeconomics-4.2.2/LICENSE.txt` & `tradingeconomics-4.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/PKG-INFO` & `tradingeconomics-4.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: tradingeconomics
-Version: 4.2.2
+Version: 4.2.3
 Summary: Trading Economics API
 Home-page: https://github.com/tradingeconomics/tradingeconomics/python
-Download-URL: https://github.com/tradingeconomics/tradingeconomics/raw/master/python/dist/tradingeconomics-4.2.2.zip
 Author: Trading Economics
 Author-email: support@tradingeconomics.com
 License: MIT
+Download-URL: https://github.com/tradingeconomics/tradingeconomics/raw/master/python/dist/tradingeconomics-4.2.3.zip
 Keywords: tradingeconomics,data
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -33,7 +34,9 @@
 
 Documentation
 ----------------------------------------
 
  - https://docs.tradingeconomics.com
 
 
+
+
```

### Comparing `tradingeconomics-4.2.2/README.rst` & `tradingeconomics-4.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/setup.py` & `tradingeconomics-4.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
     this_directory = path.abspath(path.dirname(__file__))
     with io.open(path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
       return f.read()
 
 setup(
   name = 'tradingeconomics',
   packages = find_packages(exclude=['tests*']),  
-  version = '4.2.2',
+  version = '4.2.3',
   description = 'Trading Economics API',
   long_description =readme(),
   long_description_content_type='text/x-rst',
   author = 'Trading Economics',
   author_email = 'support@tradingeconomics.com',
   license = 'MIT',
   url = 'https://github.com/tradingeconomics/tradingeconomics/python', 
-  download_url = 'https://github.com/tradingeconomics/tradingeconomics/raw/master/python/dist/tradingeconomics-4.2.2.zip',
+  download_url = 'https://github.com/tradingeconomics/tradingeconomics/raw/master/python/dist/tradingeconomics-4.2.3.zip',
   keywords = ['tradingeconomics', 'data'], 
   classifiers = [ 'Programming Language :: Python :: 3',
                 'Programming Language :: Python :: 3.2',
                 'Programming Language :: Python :: 3.3',
                 'Programming Language :: Python :: 3.4',
                 'Programming Language :: Python :: 3.8'],
   install_requires = ['pandas', 'websocket-client'],
```

### Comparing `tradingeconomics-4.2.2/tradingeconomics/__init__.py` & `tradingeconomics-4.2.3/tradingeconomics/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     from .markets import getMarketsData, getMarketsBySymbol, getMarketsIntraday, getMarketsPeers, getMarketsComponents, getMarketsSearch, getMarketsForecasts, getCurrencyCross, getMarketsIntradayByInterval, getMarketsStockDescriptions,getMarketsSymbology,getStocksByCountry
     from .historicalMarkets import fetchMarkets
     from .glob import login, subscribe
     from .stream import run
     from .earnings import getEarnings, getEarningsType
     from .news import getNews, getArticles, getArticleId 
     from .worldBank import getWBCategories, getWBIndicator, getWBCountry, getWBHistorical
-    from .comtrade import getCmtCategories, getCmtCountry, getCmtHistorical, getCmtTwoCountries, getCmtUpdates, getCmtCountryByCategory, getCmtTotalByType, getCmtCountryFilterByType,getCmtTotalByTypeAndMainCategory
+    from .comtrade import getCmtCategories, getCmtCountry, getCmtHistorical, getCmtTwoCountries, getCmtUpdates, getCmtCountryByCategory, getCmtTotalByType, getCmtCountryFilterByType, getCmtSnapshotByType
     from .federalReserve import getFedRStates, getFedRSnaps, getFedRHistorical, getFedRCounty
     from .eurostat import getEurostatData,getEurostatCountries,getEurostatCategoryGroups
     from .historicalEurostat import getHistoricalEurostat
     from .financials import getFinancialsData, getFinancialsCategoryList, getFinancialsDataByCategory
     from .historicalFinancials import getFinancialsHistorical
     from .search import getSearch
 
@@ -38,15 +38,15 @@
     from markets import getMarketsData, getMarketsBySymbol, getMarketsIntraday, getMarketsPeers, getMarketsComponents, getMarketsSearch, getMarketsForecasts, getCurrencyCross, getMarketsIntradayByInterval, getMarketsStockDescriptions
     from historicalMarkets import fetchMarkets
     from glob import login, subscribe
     from stream import run
     from earnings import getEarnings, getEarningsType
     from news import getNews, getArticles, getArticleId
     from worldBank import getWBCategories, getWBIndicator, getWBCountry, getWBHistorical
-    from comtrade import getCmtCategories, getCmtCountry, getCmtHistorical, getCmtTwoCountries, getCmtUpdates, getCmtCountryByCategory, getCmtTotalByType, getCmtCountryFilterByType
+    from comtrade import getCmtCategories, getCmtCountry, getCmtHistorical, getCmtTwoCountries, getCmtUpdates, getCmtCountryByCategory, getCmtTotalByType, getCmtCountryFilterByType, getCmtSnapshotByType
     from federalReserve import getFedRStates, getFedRSnaps, getFedRHistorical, getFedRCounty
     from eurostat import getEurostatData,getEurostatCountries,getEurostatCategoryGroups
     from historicalEurostat import getHistoricalEurostat
     from financials import getFinancialsData, getFinancialsCategoryList, getFinancialsDataByCategory
     from historicalFinancials import getFinancialsHistorical
     from search import getSearch
```

### Comparing `tradingeconomics-4.2.2/tradingeconomics/calendar.py` & `tradingeconomics-4.2.3/tradingeconomics/calendar.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/comtrade.py` & `tradingeconomics-4.2.3/tradingeconomics/comtrade.py`

 * *Files 6% similar despite different names*

```diff
@@ -353,15 +353,15 @@
 
     try:
         link_api += '?c=' + glob.apikey
     except AttributeError:
         raise LoginError('You need to do login before making any request')
 
     try:
-        print(link_api)
+        # print(link_api)
         return fn.dataRequest(api_request=link_api, output_type=output_type)
     except Exception as e:
         print(e)
         
 
 def getCmtTotalByType(country=None, type=None, output_type=None):
     """
@@ -408,15 +408,15 @@
         api_url_base = "https://api.tradingeconomics.com/comtrade"
 
         return f'{api_url_base}/{type}/{quote(country)}/totals/?c={glob.apikey}'
 
     link_api = getLinkApi(country, type)
 
     try:
-        print(link_api)
+        # print(link_api)
         return fn.dataRequest(api_request=link_api, output_type=output_type)
     except Exception as e:
         print(e)
 
 def getCmtCountryFilterByType(country1=None, country2=None, type=None, output_type=None):
     """
         Get detailed information about Comtrade Countries filter by type 'import' or 'export'
@@ -480,76 +480,20 @@
     try:
         link_api += f'&type={type}'
 
     except AttributeError:
         raise TypeError('type is missing. Choose "import" or "export"')
 
     try:
-        print(link_api)
+        # print(link_api)
         return fn.dataRequest(api_request=link_api, output_type=output_type)
     except Exception as e:
         print(e)
 
 
-
-
-def getCmtTotalByTypeAndMainCategory(country=None, type=None, output_type=None):
-    """
-        Get detailed information about Comtrade Country Total by Import or Exports and main category
-        =================================================================================
-
-        Parameters:
-        -----------
-        country:string.
-                    for example:
-                    country = 'country_name' ,
-
-        type: string.
-                for example:
-                    type = 'import'
-                    type = 'export'
-
-        output_type: string.
-                    'dict'(default) for dictionary format output, 'df' for data frame,
-                    'raw' for list of dictionaries directly from the web.
-
-        Notes
-        -----
-        country and type parameters are not optional.
-
-        Example
-        -------
-        getCmtTotalByType(country = 'Portugal', type = 'import', output_type = None )
-
-        getCmtTotalByType(country = 'United States', type = 'export', output_type = 'raw' )
-
-        getCmtTotalByType(country = 'Brazil', type = import, output_type = 'df' )
-
-        """
-
-
-    if country is None:
-        return f'country is missing'
-
-    if type is None:
-        return f"type is missing. Choose 'import' or 'export'"
-
-    def getLinkApi(country, type):
-        api_url_base = "https://api.tradingeconomics.com/comtrade"
-
-        return f'{api_url_base}/{type}/{quote(country)}?c={glob.apikey}'
-
-    link_api = getLinkApi(country, type)
-
-    try:
-        print(link_api)
-        return fn.dataRequest(api_request=link_api, output_type=output_type)
-    except Exception as e:
-        print(e)
-
 def getCmtSnapshotByType(country=None, type=None, output_type=None):
     """
         Get Snapshot of data per country filtered by type: import or export
         =================================================================================
 
         Parameters:
         -----------
@@ -591,11 +535,11 @@
         api_url_base = "https://api.tradingeconomics.com/comtrade/country"
 
         return f'{api_url_base}/{quote(country)}?type={type}&c={glob.apikey}'
 
     link_api = getLinkApi(country, type)
 
     try:
-        print(link_api)
+        # print(link_api)
         return fn.dataRequest(api_request=link_api, output_type=output_type)
     except Exception as e:
         print(e)
```

### Comparing `tradingeconomics-4.2.2/tradingeconomics/earnings.py` & `tradingeconomics-4.2.3/tradingeconomics/earnings.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,23 +67,24 @@
         _create_unverified_https_context = ssl._create_unverified_context
     except AttributeError:
         pass
     else:
         ssl._create_default_https_context = _create_unverified_https_context
         
     
-    linkAPI = 'https://api.tradingeconomics.com/earnings/' 
+    # linkAPI = 'https://api.tradingeconomics.com/earnings/' 
+    linkAPI = 'https://api.tradingeconomics.com/earnings-revenues'
     if symbols:
-        linkAPI += 'symbol/'
+        linkAPI += '/symbol/'
         if type(symbols) is not str:
             linkAPI += quote(",".join(symbols), safe='')
         else:
             linkAPI += quote(symbols)
     elif country:
-        linkAPI += 'country/'
+        linkAPI += '/country/'
         if type(country) is not str:
             linkAPI += quote(",".join(country), safe='')
         else:
             linkAPI += quote(country)
     try:
         linkAPI += '?c=' + glob.apikey
     except AttributeError:
```

### Comparing `tradingeconomics-4.2.2/tradingeconomics/eurostat.py` & `tradingeconomics-4.2.3/tradingeconomics/eurostat.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/federalReserve.py` & `tradingeconomics-4.2.3/tradingeconomics/federalReserve.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/financials.py` & `tradingeconomics-4.2.3/tradingeconomics/financials.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/forecasts.py` & `tradingeconomics-4.2.3/tradingeconomics/forecasts.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/functions.py` & `tradingeconomics-4.2.3/tradingeconomics/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,16 +206,16 @@
 
 def checkDates(baseLink, initDate=None, endDate=None):
     if (initDate is not None) and endDate == None :
         try: 
             validate(initDate)
         except ValueError:
             raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
-            if initDate > str(date.today()):
-                raise DateError ('Initial date out of range.')
+        # if initDate > str(date.today()):
+        #     raise DateError ('Initial date out of range.')
         baseLink += '&d1=' + quote(initDate)
 
     if (initDate is not None) and (endDate is not None) :
         try: 
             validate(initDate)
         except ValueError:
             raise DateError ('Incorrect initDate format, should be YYYY-MM-DD or MM-DD-YYYY.')
```

### Comparing `tradingeconomics-4.2.2/tradingeconomics/glob.py` & `tradingeconomics-4.2.3/tradingeconomics/glob.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/historical.py` & `tradingeconomics-4.2.3/tradingeconomics/historical.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/historicalDB.py` & `tradingeconomics-4.2.3/tradingeconomics/historicalDB.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/historicalEurostat.py` & `tradingeconomics-4.2.3/tradingeconomics/historicalEurostat.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/historicalFinancials.py` & `tradingeconomics-4.2.3/tradingeconomics/historicalFinancials.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/historicalMarkets.py` & `tradingeconomics-4.2.3/tradingeconomics/historicalMarkets.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/indicators.py` & `tradingeconomics-4.2.3/tradingeconomics/indicators.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/markets.py` & `tradingeconomics-4.2.3/tradingeconomics/markets.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/news.py` & `tradingeconomics-4.2.3/tradingeconomics/news.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/search.py` & `tradingeconomics-4.2.3/tradingeconomics/search.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/stream.py` & `tradingeconomics-4.2.3/tradingeconomics/stream.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics/worldBank.py` & `tradingeconomics-4.2.3/tradingeconomics/worldBank.py`

 * *Files identical despite different names*

### Comparing `tradingeconomics-4.2.2/tradingeconomics.egg-info/PKG-INFO` & `tradingeconomics-4.2.3/tradingeconomics.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: tradingeconomics
-Version: 4.2.2
+Version: 4.2.3
 Summary: Trading Economics API
 Home-page: https://github.com/tradingeconomics/tradingeconomics/python
-Download-URL: https://github.com/tradingeconomics/tradingeconomics/raw/master/python/dist/tradingeconomics-4.2.2.zip
 Author: Trading Economics
 Author-email: support@tradingeconomics.com
 License: MIT
+Download-URL: https://github.com/tradingeconomics/tradingeconomics/raw/master/python/dist/tradingeconomics-4.2.3.zip
 Keywords: tradingeconomics,data
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -33,7 +34,9 @@
 
 Documentation
 ----------------------------------------
 
  - https://docs.tradingeconomics.com
 
 
+
+
```

### Comparing `tradingeconomics-4.2.2/tradingeconomics.egg-info/SOURCES.txt` & `tradingeconomics-4.2.3/tradingeconomics.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE.txt
 MANIFEST.in
-README.md
 README.rst
 setup.cfg
 setup.py
 tradingeconomics/__init__.py
 tradingeconomics/calendar.py
 tradingeconomics/comtrade.py
 tradingeconomics/earnings.py
```

