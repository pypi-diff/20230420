# Comparing `tmp/tap_exact-0.2.3.tar.gz` & `tmp/tap_exact-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_exact-0.2.3.tar", max compression
+gzip compressed data, was "tap_exact-0.3.0.tar", max compression
```

## Comparing `tap_exact-0.2.3.tar` & `tap_exact-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      932 2023-04-20 13:26:22.089328 tap_exact-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.2.3/tap_exact/__init__.py
--rw-r--r--   0        0        0      842 2023-04-20 11:44:26.669328 tap_exact-0.2.3/tap_exact/client.py
--rw-r--r--   0        0        0    30438 2023-04-20 13:26:14.609328 tap_exact-0.2.3/tap_exact/streams.py
--rw-r--r--   0        0        0     1677 2023-04-19 14:49:52.622465 tap_exact-0.2.3/tap_exact/tap.py
--rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.2.3/tap_exact/tests/__init__.py
--rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.2.3/tap_exact/tests/test_core.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.2.3/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      932 2023-04-20 17:21:29.969328 tap_exact-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.3.0/tap_exact/__init__.py
+-rw-r--r--   0        0        0      842 2023-04-20 11:44:26.669328 tap_exact-0.3.0/tap_exact/client.py
+-rw-r--r--   0        0        0    33031 2023-04-20 17:20:13.789328 tap_exact-0.3.0/tap_exact/streams.py
+-rw-r--r--   0        0        0     1723 2023-04-20 17:21:53.919328 tap_exact-0.3.0/tap_exact/tap.py
+-rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.3.0/tap_exact/tests/__init__.py
+-rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.3.0/tap_exact/tests/test_core.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.3.0/setup.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.3.0/PKG-INFO
```

### Comparing `tap_exact-0.2.3/pyproject.toml` & `tap_exact-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-exact"
-version = "0.2.3"
+version = "0.3.0"
 description = "`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK."
 authors = ["Janick Otten"]
 keywords = [
     "ELT",
     "Exact Online",
 ]
 license = "Apache 2.0"
```

### Comparing `tap_exact-0.2.3/tap_exact/client.py` & `tap_exact-0.3.0/tap_exact/client.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.2.3/tap_exact/streams.py` & `tap_exact-0.3.0/tap_exact/streams.py`

 * *Files 4% similar despite different names*

```diff
@@ -893,8 +893,79 @@
 
         for row in resp:
             
             # We loop through the keys that should be modified
             for key in keys:
                 row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
 
+            yield row
+
+class SystemUsersStream(ExactOnlineStream):
+    """Define custom stream."""
+
+    name = "system_users"
+    primary_keys = ["UserID"]
+    replication_key = "Modified"
+    # Optionally, you may also use `schema_filepath` in place of `schema`:
+    # schema_filepath = SCHEMAS_DIR / "users.json"
+    schema = th.PropertiesList(
+        th.Property(
+            "UserID",
+            th.StringType,
+            description="The unique identifier of the user"
+        ),
+        th.Property(
+            "FullName",
+            th.StringType,
+            description="The name of the user"
+        ),
+        th.Property(
+            "Email",
+            th.StringType,
+            description="The e-mailaddress of the user"
+        ),
+        th.Property(
+            "StartDate",
+            th.DateTimeType,
+            description="The start date the user was allowed to log in"
+        ),
+        th.Property(
+            "EndDate",
+            th.DateTimeType,
+            description="The date after which the user login is disabled"
+        ),
+        th.Property(
+            "Modified",
+            th.DateTimeType,
+            description="Last modified date"
+        ),
+    ).to_dict()
+
+    def get_path(self, context: Optional[dict]) -> str:
+        """Return the path of the Exact API"""
+
+        # This stream should disregard the start_date as earliest starting timestamp
+        if datetime.strptime(self.config.get("start_date"), '%Y-%m-%d').strftime('%Y-%m-%d') != self.get_starting_timestamp(context).strftime('%Y-%m-%d'):
+            replication_key_value = self.get_starting_timestamp(context).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
+            
+            filter_path = f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&"
+        
+        path = f"/system/Users?{filter_path if 'filter_path' in locals() else ''}" \
+            "$select=UserID,FullName,Email,StartDate,EndDate,Modified"
+
+        return path
+
+    def get_records(self, context: Optional[dict]) -> Iterable[dict]:
+        """Return a generator or row-type dictionary objects"""
+        
+        resp = self.conn.rest(GET('v1/%d/%s' % (self.division, self.get_path(context) )))
+        
+        # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
+        keys = ['StartDate', 'EndDate', 'Modified']
+
+        for row in resp:
+            
+            # We loop through the keys that should be modified
+            for key in keys:
+                row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
+
             yield row
```

### Comparing `tap_exact-0.2.3/tap_exact/tap.py` & `tap_exact-0.3.0/tap_exact/tap.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,28 +11,30 @@
     PurchaseInvoicesStream,
     GeneralLedgerAccountsStream,
     BankEntryLinesStream,
     CashEntryLinesStream,
     GeneralJournalEntryLinesStream,
     PurchaseEntriesStream,
     SalesEntriesStream,
-    CrmAccountsStream
+    CrmAccountsStream,
+    SystemUsersStream
 )
 # TODO: Compile a list of custom stream types here
 #       OR rewrite discover_streams() below with your custom logic.
 STREAM_TYPES = [
     SalesInvoicesStream,
     PurchaseInvoicesStream,
     GeneralLedgerAccountsStream,
     BankEntryLinesStream,
     CashEntryLinesStream,
     GeneralJournalEntryLinesStream,
     PurchaseEntriesStream,
     SalesEntriesStream,
-    CrmAccountsStream
+    CrmAccountsStream,
+    SystemUsersStream
 ]
 
 
 class TapExactOnline(Tap):
     """ExactOnline tap class."""
     name = "tap-exact"
```

### Comparing `tap_exact-0.2.3/tap_exact/tests/test_core.py` & `tap_exact-0.3.0/tap_exact/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.2.3/setup.py` & `tap_exact-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'s3': ['fs-s3fs>=1.1.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['tap-exact = tap_exact.tap:TapExactOnline.cli']}
 
 setup_kwargs = {
     'name': 'tap-exact',
-    'version': '0.2.3',
+    'version': '0.3.0',
     'description': '`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.',
     'long_description': 'None',
     'author': 'Janick Otten',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tap_exact-0.2.3/PKG-INFO` & `tap_exact-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-exact
-Version: 0.2.3
+Version: 0.3.0
 Summary: `tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Exact Online
 Author: Janick Otten
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

