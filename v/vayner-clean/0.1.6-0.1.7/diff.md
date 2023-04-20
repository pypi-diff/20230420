# Comparing `tmp/vayner_clean-0.1.6.tar.gz` & `tmp/vayner_clean-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vayner_clean-0.1.6.tar", last modified: Fri Apr 14 08:57:55 2023, max compression
+gzip compressed data, was "vayner_clean-0.1.7.tar", last modified: Thu Apr 20 07:25:50 2023, max compression
```

## Comparing `vayner_clean-0.1.6.tar` & `vayner_clean-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-04-14 08:57:55.620161 vayner_clean-0.1.6/
--rw-r--r--   0 willbutler   (502) staff       (20)     1399 2023-04-14 08:57:55.620020 vayner_clean-0.1.6/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      703 2023-03-14 11:27:46.000000 vayner_clean-0.1.6/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-04-14 08:57:55.620210 vayner_clean-0.1.6/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1314 2023-04-14 08:57:46.000000 vayner_clean-0.1.6/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-04-14 08:57:55.619430 vayner_clean-0.1.6/vayner_clean.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)     1399 2023-04-14 08:57:55.000000 vayner_clean-0.1.6/vayner_clean.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      251 2023-04-14 08:57:55.000000 vayner_clean-0.1.6/vayner_clean.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-04-14 08:57:55.000000 vayner_clean-0.1.6/vayner_clean.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       27 2023-04-14 08:57:55.000000 vayner_clean-0.1.6/vayner_clean.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-04-14 08:57:55.000000 vayner_clean-0.1.6/vayner_clean.egg-info/top_level.txt
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-04-14 08:57:55.619662 vayner_clean-0.1.6/vee_clean/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-23 14:12:51.000000 vayner_clean-0.1.6/vee_clean/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    15751 2023-04-14 08:55:46.000000 vayner_clean-0.1.6/vee_clean/cleaning_functions.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-04-20 07:25:50.200290 vayner_clean-0.1.7/
+-rw-r--r--   0 willbutler   (502) staff       (20)     1379 2023-04-20 07:25:50.200063 vayner_clean-0.1.7/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      703 2023-03-14 11:27:46.000000 vayner_clean-0.1.7/README.md
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-04-20 07:25:50.200365 vayner_clean-0.1.7/setup.cfg
+-rw-r--r--   0 willbutler   (502) staff       (20)     1314 2023-04-20 07:25:39.000000 vayner_clean-0.1.7/setup.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-04-20 07:25:50.199292 vayner_clean-0.1.7/vayner_clean.egg-info/
+-rw-r--r--   0 willbutler   (502) staff       (20)     1379 2023-04-20 07:25:50.000000 vayner_clean-0.1.7/vayner_clean.egg-info/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      251 2023-04-20 07:25:50.000000 vayner_clean-0.1.7/vayner_clean.egg-info/SOURCES.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-04-20 07:25:50.000000 vayner_clean-0.1.7/vayner_clean.egg-info/dependency_links.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       27 2023-04-20 07:25:50.000000 vayner_clean-0.1.7/vayner_clean.egg-info/requires.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-04-20 07:25:50.000000 vayner_clean-0.1.7/vayner_clean.egg-info/top_level.txt
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-04-20 07:25:50.199559 vayner_clean-0.1.7/vee_clean/
+-rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-23 14:12:51.000000 vayner_clean-0.1.7/vee_clean/__init__.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    15754 2023-04-20 07:20:21.000000 vayner_clean-0.1.7/vee_clean/cleaning_functions.py
```

### Comparing `vayner_clean-0.1.6/PKG-INFO` & `vayner_clean-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: vayner_clean
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library for cleaning advertising data from Tracer
 Home-page: 
 Author: Will Butler
 Author-email: will.butler@vaynermedia.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -40,9 +39,7 @@
 
 ## Usage in code
 In this example we will be using the cleaning library to clean and standardise column names in a dataframe 
 
 ```
 fb_organic = clean.clean_column_names(fb_organic_temp)
 ```
-
-
```

### Comparing `vayner_clean-0.1.6/README.md` & `vayner_clean-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `vayner_clean-0.1.6/setup.py` & `vayner_clean-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="vayner_clean",
-    version="0.1.6",
+    version="0.1.7",
     description="Library for cleaning advertising data from Tracer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Will Butler",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
```

### Comparing `vayner_clean-0.1.6/vayner_clean.egg-info/PKG-INFO` & `vayner_clean-0.1.7/vayner_clean.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: vayner-clean
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library for cleaning advertising data from Tracer
 Home-page: 
 Author: Will Butler
 Author-email: will.butler@vaynermedia.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -40,9 +39,7 @@
 
 ## Usage in code
 In this example we will be using the cleaning library to clean and standardise column names in a dataframe 
 
 ```
 fb_organic = clean.clean_column_names(fb_organic_temp)
 ```
-
-
```

### Comparing `vayner_clean-0.1.6/vee_clean/cleaning_functions.py` & `vayner_clean-0.1.7/vee_clean/cleaning_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         elif (column == 'reach') or (('impressions' in column) and ('unique' in column)):
             column = 'reach'
         elif ('campaign'in column) and ('name' in column):
             column = 'campaign_name'
         elif (('adset' in column) or ('group' in column)) and ('name' in column):
             column = 'group_name'
         elif ('ad' in column) and ('name' in column):
-            column = 'name' # for tt_organic
+            column = 'ad_name' # for tt_organic
         elif ('creative' in column) and ('name' in column):
             column = 'creative_name'
         elif ('video' in column) and ('impression' in column):                       
             column = 'video_impressions'
         elif ('shares' in column) or ('retweet' in column):
             column = 'shares'
         elif (('conversion' in column) or ('lifetime'in column)) and ('save' in column): #_1d_click_onsite_conversion_post_save in fb_ig_paid data
```

