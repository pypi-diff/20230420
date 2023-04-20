# Comparing `tmp/zoho_analytics_connector-1.4.1.tar.gz` & `tmp/zoho_analytics_connector-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoho_analytics_connector-1.4.1.tar", last modified: Tue Apr 18 12:05:14 2023, max compression
+gzip compressed data, was "zoho_analytics_connector-1.4.2.tar", last modified: Thu Apr 20 06:17:20 2023, max compression
```

## Comparing `zoho_analytics_connector-1.4.1.tar` & `zoho_analytics_connector-1.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-18 12:05:14.208942 zoho_analytics_connector-1.4.1/
--rw-rw-r--   0 tim       (1000) tim       (1000)      217 2022-07-14 03:04:02.000000 zoho_analytics_connector-1.4.1/LICENSE
--rw-rw-r--   0 tim       (1000) tim       (1000)    14323 2023-04-18 12:05:14.208942 zoho_analytics_connector-1.4.1/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)    13499 2023-04-18 12:04:14.000000 zoho_analytics_connector-1.4.1/README.md
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-04-18 12:05:14.208942 zoho_analytics_connector-1.4.1/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)     1747 2023-04-18 12:04:14.000000 zoho_analytics_connector-1.4.1/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-18 12:05:14.208942 zoho_analytics_connector-1.4.1/zoho_analytics_connector/
--rw-rw-r--   0 tim       (1000) tim       (1000)   100603 2022-11-23 02:51:47.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector/analytics_client_upstream.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     9920 2023-04-18 12:02:16.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector/enhanced_report_client.py
--rw-rw-r--   0 tim       (1000) tim       (1000)   113880 2023-03-14 04:40:03.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector/report_client.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-18 12:05:14.208942 zoho_analytics_connector-1.4.1/zoho_analytics_connector.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)    14323 2023-04-18 12:05:14.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)      412 2023-04-18 12:05:14.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-04-18 12:05:14.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       15 2023-04-18 12:05:14.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       25 2023-04-18 12:05:14.000000 zoho_analytics_connector-1.4.1/zoho_analytics_connector.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-20 06:17:20.880615 zoho_analytics_connector-1.4.2/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      217 2022-07-14 03:04:02.000000 zoho_analytics_connector-1.4.2/LICENSE
+-rw-rw-r--   0 tim       (1000) tim       (1000)    14383 2023-04-20 06:17:20.880615 zoho_analytics_connector-1.4.2/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)    13559 2023-04-20 06:16:45.000000 zoho_analytics_connector-1.4.2/README.md
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-04-20 06:17:20.880615 zoho_analytics_connector-1.4.2/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1747 2023-04-20 06:16:45.000000 zoho_analytics_connector-1.4.2/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-20 06:17:20.876615 zoho_analytics_connector-1.4.2/zoho_analytics_connector/
+-rw-rw-r--   0 tim       (1000) tim       (1000)   100603 2022-11-23 02:51:47.000000 zoho_analytics_connector-1.4.2/zoho_analytics_connector/analytics_client_upstream.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    10019 2023-04-20 06:14:57.000000 zoho_analytics_connector-1.4.2/zoho_analytics_connector/enhanced_report_client.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)   113880 2023-03-14 04:40:03.000000 zoho_analytics_connector-1.4.2/zoho_analytics_connector/report_client.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-20 06:17:20.880615 zoho_analytics_connector-1.4.2/zoho_analytics_connector.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)    14383 2023-04-20 06:17:20.000000 zoho_analytics_connector-1.4.2/zoho_analytics_connector.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)      412 2023-04-20 06:17:20.000000 zoho_analytics_connector-1.4.2/zoho_analytics_connector.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-04-20 06:17:20.000000 zoho_analytics_connector-1.4.2/zoho_analytics_connector.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       15 2023-04-20 06:17:20.000000 zoho_analytics_connector-1.4.2/zoho_analytics_connector.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       25 2023-04-20 06:17:20.000000 zoho_analytics_connector-1.4.2/zoho_analytics_connector.egg-info/top_level.txt
```

### Comparing `zoho_analytics_connector-1.4.1/PKG-INFO` & `zoho_analytics_connector-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoho_analytics_connector
-Version: 1.4.1
+Version: 1.4.2
 Summary: Zoho Analytics connector
 Home-page: https://github.com/timrichardson/zoho_analytics_connector
 Author: Tim Richardson
 Author-email: tim@growthpath.com.au
 License: MPL-2.0
 Keywords: zoho analytics
 Platform: UNKNOWN
@@ -300,14 +300,15 @@
 
 
 Changes
 -------------
 
 next_version Test updates
 
+1.4.2 Added reporting_currency to enhanced_reporting_client
 1.4.1 Something seems to changed with the UTF encoding returned by the export endpoint. Change decoding to use utf-8-sig 
 1.4.0 some adaptation towards new API from Zoho
 
 1.3.6 Documentation updates, test updates. Added a 'pre-delete function' to calculate how many rows should be deleted.
     deleteData returns an int not a string for the number of rows deleted.
 
 1.3.3 - 1.3.5 Handle some more Zoho exceptions
```

### Comparing `zoho_analytics_connector-1.4.1/README.md` & `zoho_analytics_connector-1.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -277,14 +277,15 @@
 
 
 Changes
 -------------
 
 next_version Test updates
 
+1.4.2 Added reporting_currency to enhanced_reporting_client
 1.4.1 Something seems to changed with the UTF encoding returned by the export endpoint. Change decoding to use utf-8-sig 
 1.4.0 some adaptation towards new API from Zoho
 
 1.3.6 Documentation updates, test updates. Added a 'pre-delete function' to calculate how many rows should be deleted.
     deleteData returns an int not a string for the number of rows deleted.
 
 1.3.3 - 1.3.5 Handle some more Zoho exceptions
```

### Comparing `zoho_analytics_connector-1.4.1/setup.py` & `zoho_analytics_connector-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 cmdclass = {'build_sphinx': BuildDoc}
 
 # https://pypi.org/classifiers/
 
 name = 'zoho_analytics_connector'
 keywords = 'zoho analytics'
-version = '1.4.1'
+version = '1.4.2'
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name=name,
     keywords=keywords,
```

### Comparing `zoho_analytics_connector-1.4.1/zoho_analytics_connector/analytics_client_upstream.py` & `zoho_analytics_connector-1.4.2/zoho_analytics_connector/analytics_client_upstream.py`

 * *Files identical despite different names*

### Comparing `zoho_analytics_connector-1.4.1/zoho_analytics_connector/enhanced_report_client.py` & `zoho_analytics_connector-1.4.2/zoho_analytics_connector/enhanced_report_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,21 @@
                     else:
                         col_data[col['columnName']] = col
 
         return table_data
 
     def __init__(self, login_email_id: str, token: str, default_databasename: str = None, clientId=None,
                  clientSecret=None, serverURL=None, reportServerURL=None, default_retries=None,
+                 reporting_currency:str=None,
                  error_email_list: Optional[List[str]]=None):
         """ error email list is not used by the client, but it is available for callers as a convenience"""
         self.login_email_id = login_email_id
         self.default_databasename = default_databasename
         self.error_email_list = error_email_list or [login_email_id]
+        self.reporting_currency = reporting_currency
         super().__init__(token=token, clientId=clientId, clientSecret=clientSecret, serverURL=serverURL,
                          reportServerURL=reportServerURL, default_retries=default_retries)
 
     def get_database_catalog(self, database_name: str = None) -> MutableMapping:
         db_uri = self.getDBURI(self.login_email_id, database_name or self.default_databasename)
         catalog_info = self.getDatabaseMetadata(requestURI=db_uri, metadata="ZOHO_CATALOG_INFO")
         return catalog_info
```

### Comparing `zoho_analytics_connector-1.4.1/zoho_analytics_connector/report_client.py` & `zoho_analytics_connector-1.4.2/zoho_analytics_connector/report_client.py`

 * *Files identical despite different names*

### Comparing `zoho_analytics_connector-1.4.1/zoho_analytics_connector.egg-info/PKG-INFO` & `zoho_analytics_connector-1.4.2/zoho_analytics_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoho-analytics-connector
-Version: 1.4.1
+Version: 1.4.2
 Summary: Zoho Analytics connector
 Home-page: https://github.com/timrichardson/zoho_analytics_connector
 Author: Tim Richardson
 Author-email: tim@growthpath.com.au
 License: MPL-2.0
 Keywords: zoho analytics
 Platform: UNKNOWN
@@ -300,14 +300,15 @@
 
 
 Changes
 -------------
 
 next_version Test updates
 
+1.4.2 Added reporting_currency to enhanced_reporting_client
 1.4.1 Something seems to changed with the UTF encoding returned by the export endpoint. Change decoding to use utf-8-sig 
 1.4.0 some adaptation towards new API from Zoho
 
 1.3.6 Documentation updates, test updates. Added a 'pre-delete function' to calculate how many rows should be deleted.
     deleteData returns an int not a string for the number of rows deleted.
 
 1.3.3 - 1.3.5 Handle some more Zoho exceptions
```

