# Comparing `tmp/exceltotable-0.1.tar.gz` & `tmp/exceltotable-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exceltotable-0.1.tar", last modified: Thu Apr 20 04:03:31 2023, max compression
+gzip compressed data, was "exceltotable-1.1.0.tar", last modified: Thu Apr 20 07:19:41 2023, max compression
```

## Comparing `exceltotable-0.1.tar` & `exceltotable-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 abocide    (501) staff       (20)        0 2023-04-20 04:03:31.427841 exceltotable-0.1/
--rw-r--r--   0 abocide    (501) staff       (20)      580 2023-04-20 04:03:31.427538 exceltotable-0.1/PKG-INFO
-drwxr-xr-x   0 abocide    (501) staff       (20)        0 2023-04-20 04:03:31.425382 exceltotable-0.1/exceltotable/
--rw-r--r--   0 abocide    (501) staff       (20)      811 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/1onlinechecksum.py
--rw-r--r--   0 abocide    (501) staff       (20)     3203 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/MYS_LT.py
--rw-r--r--   0 abocide    (501) staff       (20)      664 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/RetailProConsumerLoyaltyTransactionChecksum_SGP.py
--rw-r--r--   0 abocide    (501) staff       (20)     3198 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/SG_LT.py
--rw-r--r--   0 abocide    (501) staff       (20)        0 2023-04-20 02:07:29.000000 exceltotable-0.1/exceltotable/__init__.py
--rw-r--r--   0 abocide    (501) staff       (20)      675 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/csmchecksum.py
--rw-r--r--   0 abocide    (501) staff       (20)      816 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/csvLoyalty.py
--rw-r--r--   0 abocide    (501) staff       (20)      812 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/db1.py
--rw-r--r--   0 abocide    (501) staff       (20)     2040 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/demo.py
--rw-r--r--   0 abocide    (501) staff       (20)      729 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/filetodb.py
--rw-r--r--   0 abocide    (501) staff       (20)      807 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/frontier_CTL.py
--rw-r--r--   0 abocide    (501) staff       (20)      833 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/frontiers.py
--rw-r--r--   0 abocide    (501) staff       (20)     1245 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/frontiesTodb.py
--rw-r--r--   0 abocide    (501) staff       (20)      808 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/frontiesTodbcsv.py
--rw-r--r--   0 abocide    (501) staff       (20)      809 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/frontiesTodbexcel.py
--rw-r--r--   0 abocide    (501) staff       (20)     1321 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/graph.py
--rw-r--r--   0 abocide    (501) staff       (20)     1017 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/login_outlook.py
--rw-r--r--   0 abocide    (501) staff       (20)     1018 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/loyalty.py
--rw-r--r--   0 abocide    (501) staff       (20)      946 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/loyaltyls.py
--rw-r--r--   0 abocide    (501) staff       (20)     1590 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/ms_graph.py
--rw-r--r--   0 abocide    (501) staff       (20)     1530 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/offline.py
--rw-r--r--   0 abocide    (501) staff       (20)     1009 2023-04-20 01:42:27.000000 exceltotable-0.1/exceltotable/onlineauto.py
-drwxr-xr-x   0 abocide    (501) staff       (20)        0 2023-04-20 04:03:31.427093 exceltotable-0.1/exceltotable.egg-info/
--rw-r--r--   0 abocide    (501) staff       (20)      580 2023-04-20 04:03:31.000000 exceltotable-0.1/exceltotable.egg-info/PKG-INFO
--rw-r--r--   0 abocide    (501) staff       (20)      802 2023-04-20 04:03:31.000000 exceltotable-0.1/exceltotable.egg-info/SOURCES.txt
--rw-r--r--   0 abocide    (501) staff       (20)        1 2023-04-20 04:03:31.000000 exceltotable-0.1/exceltotable.egg-info/dependency_links.txt
--rw-r--r--   0 abocide    (501) staff       (20)       68 2023-04-20 04:03:31.000000 exceltotable-0.1/exceltotable.egg-info/requires.txt
--rw-r--r--   0 abocide    (501) staff       (20)       13 2023-04-20 04:03:31.000000 exceltotable-0.1/exceltotable.egg-info/top_level.txt
--rw-r--r--   0 abocide    (501) staff       (20)       38 2023-04-20 04:03:31.427935 exceltotable-0.1/setup.cfg
--rw-r--r--   0 abocide    (501) staff       (20)     1612 2023-04-20 03:47:14.000000 exceltotable-0.1/setup.py
+drwxr-xr-x   0 abocide    (501) staff       (20)        0 2023-04-20 07:19:41.750413 exceltotable-1.1.0/
+-rw-r--r--   0 abocide    (501) staff       (20)      580 2023-04-20 07:19:41.749976 exceltotable-1.1.0/PKG-INFO
+-rw-r--r--   0 abocide    (501) staff       (20)       41 2023-04-20 06:45:04.000000 exceltotable-1.1.0/README.md
+drwxr-xr-x   0 abocide    (501) staff       (20)        0 2023-04-20 07:19:41.748464 exceltotable-1.1.0/exceltotable/
+-rw-r--r--   0 abocide    (501) staff       (20)      811 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/1onlinechecksum.py
+-rw-r--r--   0 abocide    (501) staff       (20)     3203 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/MYS_LT.py
+-rw-r--r--   0 abocide    (501) staff       (20)      664 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/RetailProConsumerLoyaltyTransactionChecksum_SGP.py
+-rw-r--r--   0 abocide    (501) staff       (20)     3198 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/SG_LT.py
+-rw-r--r--   0 abocide    (501) staff       (20)       51 2023-04-20 06:32:01.000000 exceltotable-1.1.0/exceltotable/__init__.py
+-rw-r--r--   0 abocide    (501) staff       (20)      675 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/csmchecksum.py
+-rw-r--r--   0 abocide    (501) staff       (20)      816 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/csvLoyalty.py
+-rw-r--r--   0 abocide    (501) staff       (20)      812 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/db1.py
+-rw-r--r--   0 abocide    (501) staff       (20)     2040 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/demo.py
+-rw-r--r--   0 abocide    (501) staff       (20)      761 2023-04-20 06:30:59.000000 exceltotable-1.1.0/exceltotable/filetodb.py
+-rw-r--r--   0 abocide    (501) staff       (20)      807 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/frontier_CTL.py
+-rw-r--r--   0 abocide    (501) staff       (20)      833 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/frontiers.py
+-rw-r--r--   0 abocide    (501) staff       (20)     1245 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/frontiesTodb.py
+-rw-r--r--   0 abocide    (501) staff       (20)      808 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/frontiesTodbcsv.py
+-rw-r--r--   0 abocide    (501) staff       (20)      809 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/frontiesTodbexcel.py
+-rw-r--r--   0 abocide    (501) staff       (20)     1321 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/graph.py
+-rw-r--r--   0 abocide    (501) staff       (20)     1017 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/login_outlook.py
+-rw-r--r--   0 abocide    (501) staff       (20)     1018 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/loyalty.py
+-rw-r--r--   0 abocide    (501) staff       (20)      946 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/loyaltyls.py
+-rw-r--r--   0 abocide    (501) staff       (20)     1590 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/ms_graph.py
+-rw-r--r--   0 abocide    (501) staff       (20)     1530 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/offline.py
+-rw-r--r--   0 abocide    (501) staff       (20)     1009 2023-04-20 01:42:27.000000 exceltotable-1.1.0/exceltotable/onlineauto.py
+drwxr-xr-x   0 abocide    (501) staff       (20)        0 2023-04-20 07:19:41.749680 exceltotable-1.1.0/exceltotable.egg-info/
+-rw-r--r--   0 abocide    (501) staff       (20)      580 2023-04-20 07:19:41.000000 exceltotable-1.1.0/exceltotable.egg-info/PKG-INFO
+-rw-r--r--   0 abocide    (501) staff       (20)      812 2023-04-20 07:19:41.000000 exceltotable-1.1.0/exceltotable.egg-info/SOURCES.txt
+-rw-r--r--   0 abocide    (501) staff       (20)        1 2023-04-20 07:19:41.000000 exceltotable-1.1.0/exceltotable.egg-info/dependency_links.txt
+-rw-r--r--   0 abocide    (501) staff       (20)       59 2023-04-20 07:19:41.000000 exceltotable-1.1.0/exceltotable.egg-info/requires.txt
+-rw-r--r--   0 abocide    (501) staff       (20)       13 2023-04-20 07:19:41.000000 exceltotable-1.1.0/exceltotable.egg-info/top_level.txt
+-rw-r--r--   0 abocide    (501) staff       (20)       38 2023-04-20 07:19:41.750494 exceltotable-1.1.0/setup.cfg
+-rw-r--r--   0 abocide    (501) staff       (20)     1595 2023-04-20 07:18:23.000000 exceltotable-1.1.0/setup.py
```

### Comparing `exceltotable-0.1/PKG-INFO` & `exceltotable-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: exceltotable
-Version: 0.1
+Version: 1.1.0
 Summary: the way transfer excel,csv,file to database table
 Home-page: https://github.com/user/excel_to_table
-Download-URL: https://github.com/abocidee/excel_to_table/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/abocidee/excel_to_table/archive/refs/tags/v1.1.tar.gz
 Author: lunongyun
 Author-email: 770190990@qq.com
 License: MIT
 Keywords: excel,table
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `exceltotable-0.1/exceltotable/1onlinechecksum.py` & `exceltotable-1.1.0/exceltotable/1onlinechecksum.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/MYS_LT.py` & `exceltotable-1.1.0/exceltotable/MYS_LT.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/RetailProConsumerLoyaltyTransactionChecksum_SGP.py` & `exceltotable-1.1.0/exceltotable/RetailProConsumerLoyaltyTransactionChecksum_SGP.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/SG_LT.py` & `exceltotable-1.1.0/exceltotable/SG_LT.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/csmchecksum.py` & `exceltotable-1.1.0/exceltotable/csmchecksum.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/csvLoyalty.py` & `exceltotable-1.1.0/exceltotable/csvLoyalty.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/db1.py` & `exceltotable-1.1.0/exceltotable/db1.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/demo.py` & `exceltotable-1.1.0/exceltotable/demo.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/filetodb.py` & `exceltotable-1.1.0/exceltotable/frontiers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import pandas as pd
 import mysql.connector as msql
 from sqlalchemy import create_engine, types
 import sys
 import argparse
+import os
+
 parser = argparse.ArgumentParser(description='Show top lines from each file')
-parser.add_argument('filepath',type=str,help='enter the table name you want to generate')
+parser.add_argument('path',type=str,help='enter the path you want to generate')
 parser.add_argument('database',type=str,help='enter the database')
 args = parser.parse_args()
-print(args)
-df = pd.read_csv(args.filepath,index_col=False,delimiter=',')
 engine = create_engine('mysql+pymysql://root:Lly486597@localhost/'+args.database) # enter your password and database names here
-df.to_sql(args.filepath.split('/')[-1].split('.')[0],con=engine,index=False,if_exists='replace') # Replace Table_name with your sql table name
+print(args)
+for root,d_names,f_names in os.walk(args.path):
+  for filename in f_names:
+    f = os.path.join(root, filename)
+    print(f)
+    if("_2023" in f and ".csv" in f): 
+      df = pd.read_csv(f,index_col=False,delimiter=',')
+      df.to_sql(filename.split('_2023')[0],con=engine,index=False,if_exists='append')
```

### Comparing `exceltotable-0.1/exceltotable/frontier_CTL.py` & `exceltotable-1.1.0/exceltotable/frontier_CTL.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/frontiers.py` & `exceltotable-1.1.0/exceltotable/loyalty.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,11 +10,19 @@
 parser.add_argument('database',type=str,help='enter the database')
 args = parser.parse_args()
 engine = create_engine('mysql+pymysql://root:Lly486597@localhost/'+args.database) # enter your password and database names here
 print(args)
 for root,d_names,f_names in os.walk(args.path):
   for filename in f_names:
     f = os.path.join(root, filename)
-    print(f)
-    if("_2023" in f and ".csv" in f): 
+    if(".xls" in f): 
+      print(f)
+      df = pd.read_excel(f,sheet_name='Sheet1' ,index_col=False)
+      df.to_sql(filename.split('.')[0],con=engine,index=False,if_exists='replace') 
+      continue
+    if(".csv" in f): 
+      print(f)
       df = pd.read_csv(f,index_col=False,delimiter=',')
-      df.to_sql(filename.split('_2023')[0],con=engine,index=False,if_exists='append')  
+      df.to_sql(filename.split('.')[0],con=engine,index=False,if_exists='replace') 
+
+
+
```

### Comparing `exceltotable-0.1/exceltotable/frontiesTodb.py` & `exceltotable-1.1.0/exceltotable/frontiesTodb.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/frontiesTodbcsv.py` & `exceltotable-1.1.0/exceltotable/frontiesTodbcsv.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/frontiesTodbexcel.py` & `exceltotable-1.1.0/exceltotable/frontiesTodbexcel.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/graph.py` & `exceltotable-1.1.0/exceltotable/graph.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/login_outlook.py` & `exceltotable-1.1.0/exceltotable/login_outlook.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/loyalty.py` & `exceltotable-1.1.0/exceltotable/loyaltyls.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from sqlalchemy import create_engine, types
 import sys
 import argparse
 import os
 
 parser = argparse.ArgumentParser(description='Show top lines from each file')
 parser.add_argument('path',type=str,help='enter the path you want to generate')
-parser.add_argument('database',type=str,help='enter the database')
 args = parser.parse_args()
-engine = create_engine('mysql+pymysql://root:Lly486597@localhost/'+args.database) # enter your password and database names here
+engine = create_engine('mysql+pymysql://root:Lly486597@localhost/loyaltyls') # enter your password and database names here
 print(args)
 for root,d_names,f_names in os.walk(args.path):
   for filename in f_names:
     f = os.path.join(root, filename)
     if(".xls" in f): 
       print(f)
       df = pd.read_excel(f,sheet_name='Sheet1' ,index_col=False)
```

### Comparing `exceltotable-0.1/exceltotable/ms_graph.py` & `exceltotable-1.1.0/exceltotable/ms_graph.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/offline.py` & `exceltotable-1.1.0/exceltotable/offline.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable/onlineauto.py` & `exceltotable-1.1.0/exceltotable/onlineauto.py`

 * *Files identical despite different names*

### Comparing `exceltotable-0.1/exceltotable.egg-info/PKG-INFO` & `exceltotable-1.1.0/exceltotable.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: exceltotable
-Version: 0.1
+Version: 1.1.0
 Summary: the way transfer excel,csv,file to database table
 Home-page: https://github.com/user/excel_to_table
-Download-URL: https://github.com/abocidee/excel_to_table/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/abocidee/excel_to_table/archive/refs/tags/v1.1.tar.gz
 Author: lunongyun
 Author-email: 770190990@qq.com
 License: MIT
 Keywords: excel,table
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `exceltotable-0.1/exceltotable.egg-info/SOURCES.txt` & `exceltotable-1.1.0/exceltotable.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 exceltotable/1onlinechecksum.py
 exceltotable/MYS_LT.py
 exceltotable/RetailProConsumerLoyaltyTransactionChecksum_SGP.py
 exceltotable/SG_LT.py
 exceltotable/__init__.py
 exceltotable/csmchecksum.py
```

### Comparing `exceltotable-0.1/setup.py` & `exceltotable-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 
 from distutils.core import setup
 setup(
   name = 'exceltotable',         # How you named your package folder (MyLib)
   packages = ['exceltotable'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '1.1.0',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'the way transfer excel,csv,file to database table',   # Give a short description about your library
   author = 'lunongyun',                   # Type in your name
   author_email = '770190990@qq.com',      # Type in your E-Mail
   url = 'https://github.com/user/excel_to_table',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/abocidee/excel_to_table/archive/refs/tags/v1.0.0.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/abocidee/excel_to_table/archive/refs/tags/v1.1.tar.gz',    # I explain this later on
   keywords = ['excel', 'table' ],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
-          'validators',
-          'beautifulsoup4',
+        'validators',
+        'beautifulsoup4',
        	'argparse',
 	'sqlalchemy',
 	'pandas',
-	'numpy',
-	'ms_graph'
+	'numpy'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
```

