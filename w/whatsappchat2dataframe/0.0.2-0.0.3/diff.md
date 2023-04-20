# Comparing `tmp/whatsappchat2dataframe-0.0.2.tar.gz` & `tmp/whatsappchat2dataframe-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsappchat2dataframe-0.0.2.tar", last modified: Thu Apr 20 19:29:56 2023, max compression
+gzip compressed data, was "whatsappchat2dataframe-0.0.3.tar", last modified: Thu Apr 20 20:57:37 2023, max compression
```

## Comparing `whatsappchat2dataframe-0.0.2.tar` & `whatsappchat2dataframe-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 19:29:56.455076 whatsappchat2dataframe-0.0.2/
--rw-rw-rw-   0        0        0     1087 2023-04-20 19:12:16.000000 whatsappchat2dataframe-0.0.2/LICENCE
--rw-rw-rw-   0        0        0      844 2023-04-20 19:29:56.454063 whatsappchat2dataframe-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-20 12:30:20.000000 whatsappchat2dataframe-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 19:29:56.455076 whatsappchat2dataframe-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1081 2023-04-20 19:29:42.000000 whatsappchat2dataframe-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 19:29:56.442872 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe/
--rw-rw-rw-   0        0        0       59 2023-04-20 12:54:20.000000 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe/__init__.py
--rw-rw-rw-   0        0        0     1552 2023-04-20 12:54:48.000000 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe/chat2dataframe.py
-drwxrwxrwx   0        0        0        0 2023-04-20 19:29:56.453549 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe.egg-info/
--rw-rw-rw-   0        0        0      844 2023-04-20 19:29:56.000000 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-04-20 19:29:56.000000 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 19:29:56.000000 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-20 19:29:56.000000 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-04-20 19:29:56.000000 whatsappchat2dataframe-0.0.2/whatsappchat2dataframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 20:57:37.668117 whatsappchat2dataframe-0.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-04-20 19:12:16.000000 whatsappchat2dataframe-0.0.3/LICENCE
+-rw-rw-rw-   0        0        0     1074 2023-04-20 20:57:37.668117 whatsappchat2dataframe-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-04-20 20:55:19.000000 whatsappchat2dataframe-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 20:57:37.668117 whatsappchat2dataframe-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-04-20 20:55:58.000000 whatsappchat2dataframe-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:57:37.650116 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe/
+-rw-rw-rw-   0        0        0       59 2023-04-20 12:54:20.000000 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe/__init__.py
+-rw-rw-rw-   0        0        0     2002 2023-04-20 19:43:39.000000 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe/chat2dataframe.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:57:37.667123 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe.egg-info/
+-rw-rw-rw-   0        0        0     1074 2023-04-20 20:57:37.000000 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-04-20 20:57:37.000000 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 20:57:37.000000 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-20 20:57:37.000000 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-20 20:57:37.000000 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe.egg-info/top_level.txt
```

### Comparing `whatsappchat2dataframe-0.0.2/LICENCE` & `whatsappchat2dataframe-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `whatsappchat2dataframe-0.0.2/PKG-INFO` & `whatsappchat2dataframe-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: whatsappchat2dataframe
-Version: 0.0.2
-Summary: Converting a Whatsapp chat into a pandas DataFrame
+Version: 0.0.3
+Summary: Converts a Whatsapp chat (.txt file) into a pandas DataFrame
 Author: Kiran Busch
 Author-email: <kiranbusch@t-online.de>
 Keywords: python,whatsapp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -14,21 +14,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 
 # whatsappChat2dataFrame
 
 
-Under construction! Not ready for use yet! Currently experimenting and planning!
+Currently experimenting and planning!
 
 Developed by Kiran Busch 2023
 
 ## Examples of How To Use (Buggy Alpha Version)
 
-Creating A Server
+Creating a Converter and calling chat2dataframe function
 
 ```python
-bla
-
-# Other Code
-
+#load package with converter
+from whatsappchat2dataframe import Converter
+#create converter
+conv = Converter()
+#create dataframe from whatsapp .txt file
+file_path = 'data/_chat.txt'
+df = conv.chat2dataframe(path_to_filename = file_path)
 ```
```

### Comparing `whatsappchat2dataframe-0.0.2/setup.py` & `whatsappchat2dataframe-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
-DESCRIPTION = 'Converting a Whatsapp chat into a pandas DataFrame'
-LONG_DESCRIPTION = 'A package that allows...'
+VERSION = '0.0.3'
+DESCRIPTION = 'Converts a Whatsapp chat (.txt file) into a pandas DataFrame'
+LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="whatsappchat2dataframe",
     version=VERSION,
     author="Kiran Busch",
     author_email="<kiranbusch@t-online.de>",
```

### Comparing `whatsappchat2dataframe-0.0.2/whatsappchat2dataframe/chat2dataframe.py` & `whatsappchat2dataframe-0.0.3/whatsappchat2dataframe/chat2dataframe.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,20 +8,31 @@
 import pandas as pd
 
 class Converter:
     def __init__(self) -> None:
         pass
 
     def chat2dataframe(self,path_to_filename:str):
+        """converts a whatsappchat (.txt file) into a pandas dataframe
+
+        Args:
+            path_to_filename (str): path to file e.g. data/chat.txt
+
+        Returns:
+            pd.DataFrame: return a pandas DataFrame of the .txt file
+        """
         self.DATE_TIME = re.compile(r"([\[]).*?([\]])")
         self.AUTHOR = re.compile(r"((( [a-zA-ZöäüÖÄÜ]+)+):)")
         self.LTR = chr(8206)
-
-        with open(path_to_filename, 'r') as file:
-            self.data = file.read().replace('\n', '')
+        try:
+            with open(path_to_filename, 'r') as file:
+                self.data = file.read().replace('\n', '')
+        except Exception as e:
+            print(f"Could not process {path_to_filename}, because the following error occured: {type(e).__name__}: {str(e)}")
+        
 
         df = pd.DataFrame(self.__chat2df(data=self.data), columns=["DateTime", "Author", "Message"])
         df['DateTime'] = df['DateTime'] + pd.to_timedelta(df.groupby('DateTime').cumcount(), unit='ms')
         df['numMessage']=1
         return df
 
     def __to_pd_row(self, s):
```

### Comparing `whatsappchat2dataframe-0.0.2/whatsappchat2dataframe.egg-info/PKG-INFO` & `whatsappchat2dataframe-0.0.3/whatsappchat2dataframe.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: whatsappchat2dataframe
-Version: 0.0.2
-Summary: Converting a Whatsapp chat into a pandas DataFrame
+Version: 0.0.3
+Summary: Converts a Whatsapp chat (.txt file) into a pandas DataFrame
 Author: Kiran Busch
 Author-email: <kiranbusch@t-online.de>
 Keywords: python,whatsapp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -14,21 +14,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 
 # whatsappChat2dataFrame
 
 
-Under construction! Not ready for use yet! Currently experimenting and planning!
+Currently experimenting and planning!
 
 Developed by Kiran Busch 2023
 
 ## Examples of How To Use (Buggy Alpha Version)
 
-Creating A Server
+Creating a Converter and calling chat2dataframe function
 
 ```python
-bla
-
-# Other Code
-
+#load package with converter
+from whatsappchat2dataframe import Converter
+#create converter
+conv = Converter()
+#create dataframe from whatsapp .txt file
+file_path = 'data/_chat.txt'
+df = conv.chat2dataframe(path_to_filename = file_path)
 ```
```

