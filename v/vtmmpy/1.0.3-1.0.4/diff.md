# Comparing `tmp/vtmmpy-1.0.3.tar.gz` & `tmp/vtmmpy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtmmpy-1.0.3.tar", last modified: Wed Apr 19 13:22:49 2023, max compression
+gzip compressed data, was "vtmmpy-1.0.4.tar", last modified: Thu Apr 20 09:07:34 2023, max compression
```

## Comparing `vtmmpy-1.0.3.tar` & `vtmmpy-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:22:49.339610 vtmmpy-1.0.3/
--rw-rw-r--   0 tony      (1000) tony      (1000)    35149 2023-04-19 12:45:40.000000 vtmmpy-1.0.3/LICENSE
--rw-rw-r--   0 tony      (1000) tony      (1000)     3693 2023-04-19 13:22:49.339610 vtmmpy-1.0.3/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)     3218 2023-04-19 13:22:05.000000 vtmmpy-1.0.3/README.md
--rw-r--r--   0 tony      (1000) tony      (1000)      103 2023-03-18 14:25:35.000000 vtmmpy-1.0.3/pyproject.toml
--rw-r--r--   0 tony      (1000) tony      (1000)      611 2023-04-19 13:22:49.339610 vtmmpy-1.0.3/setup.cfg
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:22:49.339610 vtmmpy-1.0.3/src/
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:22:49.339610 vtmmpy-1.0.3/src/vtmmpy/
--rw-r--r--   0 tony      (1000) tony      (1000)     8279 2023-04-18 14:04:08.000000 vtmmpy-1.0.3/src/vtmmpy/__init__.py
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:22:49.339610 vtmmpy-1.0.3/src/vtmmpy.egg-info/
--rw-r--r--   0 tony      (1000) tony      (1000)     3693 2023-04-19 13:22:49.000000 vtmmpy-1.0.3/src/vtmmpy.egg-info/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)      201 2023-04-19 13:22:49.000000 vtmmpy-1.0.3/src/vtmmpy.egg-info/SOURCES.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-04-19 13:22:49.000000 vtmmpy-1.0.3/src/vtmmpy.egg-info/dependency_links.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        7 2023-04-19 13:22:49.000000 vtmmpy-1.0.3/src/vtmmpy.egg-info/top_level.txt
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-20 09:07:34.453828 vtmmpy-1.0.4/
+-rw-rw-r--   0 tony      (1000) tony      (1000)    35149 2023-04-19 12:45:40.000000 vtmmpy-1.0.4/LICENSE
+-rw-rw-r--   0 tony      (1000) tony      (1000)     3693 2023-04-20 09:07:34.453828 vtmmpy-1.0.4/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)     3218 2023-04-19 13:22:05.000000 vtmmpy-1.0.4/README.md
+-rw-r--r--   0 tony      (1000) tony      (1000)      103 2023-03-18 14:25:35.000000 vtmmpy-1.0.4/pyproject.toml
+-rw-r--r--   0 tony      (1000) tony      (1000)      611 2023-04-20 09:07:34.453828 vtmmpy-1.0.4/setup.cfg
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-20 09:07:34.453828 vtmmpy-1.0.4/src/
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-20 09:07:34.453828 vtmmpy-1.0.4/src/vtmmpy/
+-rw-r--r--   0 tony      (1000) tony      (1000)     8883 2023-04-20 09:00:06.000000 vtmmpy-1.0.4/src/vtmmpy/__init__.py
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-20 09:07:34.453828 vtmmpy-1.0.4/src/vtmmpy.egg-info/
+-rw-r--r--   0 tony      (1000) tony      (1000)     3693 2023-04-20 09:07:34.000000 vtmmpy-1.0.4/src/vtmmpy.egg-info/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)      201 2023-04-20 09:07:34.000000 vtmmpy-1.0.4/src/vtmmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-04-20 09:07:34.000000 vtmmpy-1.0.4/src/vtmmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        7 2023-04-20 09:07:34.000000 vtmmpy-1.0.4/src/vtmmpy.egg-info/top_level.txt
```

### Comparing `vtmmpy-1.0.3/LICENSE` & `vtmmpy-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vtmmpy-1.0.3/PKG-INFO` & `vtmmpy-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtmmpy
-Version: 1.0.3
+Version: 1.0.4
 Summary: A vectorized implementation of the transfer matrix method
 Home-page: https://github.com/AI-Tony/vtmmpy/tree/main
 Author: Tony
 Author-email: tk_87@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `vtmmpy-1.0.3/README.md` & `vtmmpy-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vtmmpy-1.0.3/setup.cfg` & `vtmmpy-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vtmmpy
-version = 1.0.3
+version = 1.0.4
 author = Tony
 author_email = tk_87@hotmail.com
 description = A vectorized implementation of the transfer matrix method
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AI-Tony/vtmmpy/tree/main
 project_urls =
```

### Comparing `vtmmpy-1.0.3/src/vtmmpy/__init__.py` & `vtmmpy-1.0.4/src/vtmmpy/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,69 @@
+import time
 import numpy as np
 import pandas as pd
 import refidx as ri 
 from IPython.display import clear_output 
 
 
 class RefractiveIndex:
     def __init__(self):
-        # self.shelf = "main"
         self.__shelfs = ["main", "organic", "glass", "other"] 
         self.__db = ri.DataBase()
 
     def index(self, symbol): 
         if symbol=="air": return 1
         return self.__refractiveIndexInfo(symbol) 
 
     def epsilon(self, symbol):
-        return self.index(symbol)**2
+        return self.index(symbol)**2 
 
     def __refractiveIndexInfo(self, book): 
-        wavelength = 1e6 * 2 * np.pi * 3e8 / self.w 
+        wavelength = 1e6 * 2 * np.pi * 3e8 / self.w[:,0] 
+        pages = self.__findPages(book)
+        df = self.__constructPagesDF(pages, wavelength)
+        i = self.__userSeletPage(df, book) 
+        mat = pages[df.iloc[i].Page] 
+        index = mat.get_index(wavelength) 
+        return np.conjugate(index) 
+    
+    def __userSeletPage(self, df, book):
+        print("\nSelect an index [0-{}] for {} and press enter. Check refractiveindex.info for more details.\n".format(len(df)-1, book)) 
+        display(df) 
+        time.sleep(1)
+        i = int(input()) 
+        clear_output()
+        return i
+    
+    def __constructPagesDF(self, pages, wavelength):
         df = pd.DataFrame(columns=["Page", "Wavelength Range (μm)", "Comments"]) 
+        for i, (key, value) in enumerate(pages.items()): 
+            wr = pages[key].wavelength_range
+            info = pages[key].info["comments"]
+            if wr[0] < wavelength[-1] and wr[-1] > wavelength[0]: 
+                df.loc[i] = [key, wr, info] 
+        df = df.reset_index(drop=True)
+        return df
+    
+    def __findPages(self, book):
         for shelf in self.__shelfs:
             try:
                 pages = self.__db.materials[shelf][book]
                 print("{} found in {}".format(book, shelf))
-                break
+                return pages
             except:
                 print("{} not in {}".format(book, shelf)) 
                 for parentbook in self.__db.materials[shelf].keys():
                     try:
                         pages = self.__db.materials[shelf][parentbook][book] 
                         print("{} found in {}/{}".format(book, shelf, parentbook))
-                        break
+                        return pages
                     except:
                         continue
-        for i, (key, value) in enumerate(pages.items()): 
-            df.loc[i] = [key, pages[key].wavelength_range, pages[key].info["comments"]] 
-        print("\nSelect an index [0-{}] for {} and press enter. Check refractiveindex.info for more details.\n".format(len(df)-1, book)) 
-        display(df) 
-        i = int(input()) 
-        clear_output()
-        mat = pages[df.iloc[i].Page] 
-        index = mat.get_index(wavelength) 
-        return np.conjugate(index) 
+        print("{} not found. Check refractiveindex.info to make sure you have the right symbol".format(book))
 
 
 class TMM(RefractiveIndex): 
     def __init__(self, 
             freq, 
             theta, 
             f_scale=1e12,
```

### Comparing `vtmmpy-1.0.3/src/vtmmpy.egg-info/PKG-INFO` & `vtmmpy-1.0.4/src/vtmmpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtmmpy
-Version: 1.0.3
+Version: 1.0.4
 Summary: A vectorized implementation of the transfer matrix method
 Home-page: https://github.com/AI-Tony/vtmmpy/tree/main
 Author: Tony
 Author-email: tk_87@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

