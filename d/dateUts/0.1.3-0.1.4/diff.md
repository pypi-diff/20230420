# Comparing `tmp/dateUts-0.1.3.tar.gz` & `tmp/dateUts-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dateUts-0.1.3.tar", last modified: Wed Jan 18 14:26:06 2023, max compression
+gzip compressed data, was "dist\dateUts-0.1.4.tar", last modified: Thu Apr 20 19:57:57 2023, max compression
```

## Comparing `dateUts-0.1.3.tar` & `dateUts-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-18 14:26:06.051984 dateUts-0.1.3/
--rw-rw-rw-   0        0        0      526 2023-01-18 14:14:42.000000 dateUts-0.1.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2022-05-25 14:00:44.000000 dateUts-0.1.3/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2022-05-25 22:21:08.000000 dateUts-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5688 2023-01-18 14:26:06.050985 dateUts-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2952 2023-01-18 14:13:56.000000 dateUts-0.1.3/README.md
--rw-rw-rw-   0        0        0      122 2022-10-03 19:44:47.000000 dateUts-0.1.3/commands.txt
-drwxrwxrwx   0        0        0        0 2023-01-18 14:26:06.030988 dateUts-0.1.3/dateUts/
--rw-rw-rw-   0        0        0     4416 2023-01-18 14:09:47.000000 dateUts-0.1.3/dateUts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-18 14:26:06.048990 dateUts-0.1.3/dateUts.egg-info/
--rw-rw-rw-   0        0        0     5688 2023-01-18 14:26:05.000000 dateUts-0.1.3/dateUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-01-18 14:26:05.000000 dateUts-0.1.3/dateUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-18 14:26:05.000000 dateUts-0.1.3/dateUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-01-18 14:26:05.000000 dateUts-0.1.3/dateUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-18 14:26:06.052987 dateUts-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-01-18 14:24:35.000000 dateUts-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:57:57.994744 dateUts-0.1.4/
+-rw-rw-rw-   0        0        0      583 2023-04-20 19:55:45.000000 dateUts-0.1.4/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 19:57:57.971745 dateUts-0.1.4/DateUts/
+-rw-rw-rw-   0        0        0     4751 2023-04-20 19:55:03.000000 dateUts-0.1.4/DateUts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:57:57.990745 dateUts-0.1.4/DateUts.egg-info/
+-rw-rw-rw-   0        0        0     6136 2023-04-20 19:57:57.000000 dateUts-0.1.4/DateUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-04-20 19:57:57.000000 dateUts-0.1.4/DateUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 19:57:57.000000 dateUts-0.1.4/DateUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-20 19:57:57.000000 dateUts-0.1.4/DateUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1058 2022-05-25 14:00:44.000000 dateUts-0.1.4/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2022-05-25 22:21:08.000000 dateUts-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6136 2023-04-20 19:57:57.993741 dateUts-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3159 2023-04-20 19:57:17.000000 dateUts-0.1.4/README.md
+-rw-rw-rw-   0        0        0      122 2022-10-03 19:44:47.000000 dateUts-0.1.4/commands.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 19:57:57.994744 dateUts-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-04-20 19:57:55.000000 dateUts-0.1.4/setup.py
```

### Comparing `dateUts-0.1.3/CHANGELOG.txt` & `dateUts-0.1.4/CHANGELOG.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,7 +29,11 @@
 ------------------
 - Add Hours,Minutes and Seconds
 
 0.1.1 (2023-01-18)
 ------------------
 - Next Working Day
 
+0.1.2 (2024-04-20)
+------------------
+- is_weeekend
+
```

### Comparing `dateUts-0.1.3/LICENCE.txt` & `dateUts-0.1.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.3/PKG-INFO` & `dateUts-0.1.4/DateUts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dateUts
-Version: 0.1.3
+Version: 0.1.4
 Summary: Date package
 Home-page: UNKNOWN
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Description: # Sql Uts
         #
@@ -176,14 +176,33 @@
         print(dt)
         ```
         ```py
         True
         True
         ```
         
+        #### IsWeekend
+        ```py
+        #Preteend today is sunday
+        from dateUts import today,tomorrow
+        
+        dt = today()
+        print(dt.is_weekend())
+        
+        dt = tomorrow()
+        print(dt.is_weekend())
+        
+        ```
+        ```py
+        True
+        False
+        ```
+        
+        
+        
         Change Log
         ==========
         
         0.0.1 (2022-06-10)
         ------------------
         - First Release
         
@@ -211,14 +230,18 @@
         ------------------
         - Add Hours,Minutes and Seconds
         
         0.1.1 (2023-01-18)
         ------------------
         - Next Working Day
         
+        0.1.2 (2024-04-20)
+        ------------------
+        - is_weeekend
+        
         
 Keywords: dateUts
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dateUts-0.1.3/README.md` & `dateUts-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -166,8 +166,26 @@
 
 dt = dateMatch('2022-01-01','%Y-%m-%d')
 print(dt)
 ```
 ```py
 True
 True
-```
+```
+
+#### IsWeekend
+```py
+#Preteend today is sunday
+from dateUts import today,tomorrow
+
+dt = today()
+print(dt.is_weekend())
+
+dt = tomorrow()
+print(dt.is_weekend())
+
+```
+```py
+True
+False
+```
+
```

### Comparing `dateUts-0.1.3/dateUts/__init__.py` & `dateUts-0.1.4/DateUts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,41 @@
 from datetime import date, datetime as dt, timedelta as td
-from datetime import datetime
+
+
+class DateUts():
+    date = None
+
+    def __init__(self,date):
+        self.date = date
+
+    def is_weekend(self):
+        return self.date.weekday() in [5, 6]
+
+    def __repr__(self):
+        return f"<DateUts {self.date.strftime('%Y-%m-%d %H:%M:%S')}>"
+
+
+# output: True (2023-04-22 is a Saturday)
 
 
 #========= USAGE ============
 #Ex1:
 # > sqlToDate('yyyy-MM-dd')
 # > <datetime>
 
 def sqlToDate(dt:str):
-    return datetime.strptime(dt,"%Y-%m-%d")
+    return DateUts(dt.strptime(dt,"%Y-%m-%d"))
 
 #========= USAGE ============
 #Ex1:
 # > dateToSql(<datetime>)
 # > 'yyyy-MM-dd'
 
 def dateToSql(dt:date):
-    return datetime.strftime(dt,"%Y-%m-%d")
+    return DateUts(dt.strftime(dt,"%Y-%m-%d"))
 
 #========= USAGE ============
 #Ex1:
 # > now()  ,  now(fmt='%Y-%m-%d')   ,   now(fmt='sql')
 # > <datetime>, 'yyyy-MM-dd',  'yyyy-MM-dd'
 
 def now(fmt=None):
@@ -118,28 +133,28 @@
 #========= USAGE ============
 #Ex1:
 # > today()  ,  today(fmt='%Y-%m-%d')   ,   today(fmt='sql')
 # > <datetime>, 'yyyy-MM-dd',  'yyyy-MM-dd'
 
 def fmtDate(dt:date,fmt:str):
     fmt= fmt if not fmt else ("%Y-%m-%d" if fmt == "sql" else fmt)
-    return dt if not fmt else dt.strftime(fmt)
+    return DateUts(dt if not fmt else dt.strftime(fmt))
 
 def dateMatch(dt:str,fmt:str):
     fmt = "%Y-%m-%d" if fmt == "sql" else fmt
 
     try:
         dt = datetime.strptime(dt,fmt)
     except ValueError:
         return False
 
     return True
 
 
 Fnc_noWeekends = lambda dt:dt.weekday() not in [5,6]
 
-
-
-#a = lastWorkingDate(fmt="%Y-%m-%d")
+# a = DateUts(dt.now())
+# print(a)
+# a = lastWorkingDate(fmt="%Y-%m-%d")
 # rng = dateRange(sqlToDate("2022-05-01"),sqlToDate("2022-05-10"))
 # rng = dateRange(sqlToDate("2022-05-10"),sqlToDate("2022-05-01"))
 # a=1
```

### Comparing `dateUts-0.1.3/dateUts.egg-info/PKG-INFO` & `dateUts-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dateUts
-Version: 0.1.3
+Version: 0.1.4
 Summary: Date package
 Home-page: UNKNOWN
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Description: # Sql Uts
         #
@@ -176,14 +176,33 @@
         print(dt)
         ```
         ```py
         True
         True
         ```
         
+        #### IsWeekend
+        ```py
+        #Preteend today is sunday
+        from dateUts import today,tomorrow
+        
+        dt = today()
+        print(dt.is_weekend())
+        
+        dt = tomorrow()
+        print(dt.is_weekend())
+        
+        ```
+        ```py
+        True
+        False
+        ```
+        
+        
+        
         Change Log
         ==========
         
         0.0.1 (2022-06-10)
         ------------------
         - First Release
         
@@ -211,14 +230,18 @@
         ------------------
         - Add Hours,Minutes and Seconds
         
         0.1.1 (2023-01-18)
         ------------------
         - Next Working Day
         
+        0.1.2 (2024-04-20)
+        ------------------
+        - is_weeekend
+        
         
 Keywords: dateUts
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dateUts-0.1.3/setup.py` & `dateUts-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='dateUts',
-  version='0.1.3',
+  version='0.1.4',
   description='Date package',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

