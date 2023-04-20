# Comparing `tmp/requestsbankrko-0.1.98.tar.gz` & `tmp/requestsbankrko-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requestsbankrko-0.1.98.tar", last modified: Tue Jan 31 13:50:25 2023, max compression
+gzip compressed data, was "requestsbankrko-0.1.99.tar", last modified: Thu Apr 20 06:16:28 2023, max compression
```

## Comparing `requestsbankrko-0.1.98.tar` & `requestsbankrko-0.1.99.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:50:25.196660 requestsbankrko-0.1.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-31 13:50:05.000000 requestsbankrko-0.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-01-31 13:50:25.196660 requestsbankrko-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-31 13:50:05.000000 requestsbankrko-0.1.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-31 13:50:05.000000 requestsbankrko-0.1.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 13:50:25.196660 requestsbankrko-0.1.98/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:50:25.196660 requestsbankrko-0.1.98/src/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 13:50:05.000000 requestsbankrko-0.1.98/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25976 2023-01-31 13:50:05.000000 requestsbankrko-0.1.98/src/bank_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-01-31 13:50:05.000000 requestsbankrko-0.1.98/src/open_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:50:25.196660 requestsbankrko-0.1.98/src/requestsbankrko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-01-31 13:50:25.000000 requestsbankrko-0.1.98/src/requestsbankrko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-31 13:50:25.000000 requestsbankrko-0.1.98/src/requestsbankrko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 13:50:25.000000 requestsbankrko-0.1.98/src/requestsbankrko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-31 13:50:25.000000 requestsbankrko-0.1.98/src/requestsbankrko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-31 13:50:25.000000 requestsbankrko-0.1.98/src/requestsbankrko.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-01-31 13:50:05.000000 requestsbankrko-0.1.98/src/zip_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:16:28.928221 requestsbankrko-0.1.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-20 06:16:08.000000 requestsbankrko-0.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-20 06:16:28.928221 requestsbankrko-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-20 06:16:08.000000 requestsbankrko-0.1.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-20 06:16:08.000000 requestsbankrko-0.1.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 06:16:28.928221 requestsbankrko-0.1.99/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:16:28.928221 requestsbankrko-0.1.99/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:16:08.000000 requestsbankrko-0.1.99/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25977 2023-04-20 06:16:08.000000 requestsbankrko-0.1.99/src/bank_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-20 06:16:08.000000 requestsbankrko-0.1.99/src/open_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:16:28.928221 requestsbankrko-0.1.99/src/requestsbankrko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-20 06:16:28.000000 requestsbankrko-0.1.99/src/requestsbankrko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-20 06:16:28.000000 requestsbankrko-0.1.99/src/requestsbankrko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:16:28.000000 requestsbankrko-0.1.99/src/requestsbankrko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-20 06:16:28.000000 requestsbankrko-0.1.99/src/requestsbankrko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 06:16:28.000000 requestsbankrko-0.1.99/src/requestsbankrko.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-20 06:16:08.000000 requestsbankrko-0.1.99/src/zip_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:16:28.928221 requestsbankrko-0.1.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    51539 2023-04-20 06:16:08.000000 requestsbankrko-0.1.99/tests/test_bank_methods.py
```

### Comparing `requestsbankrko-0.1.98/LICENSE` & `requestsbankrko-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.1.98/PKG-INFO` & `requestsbankrko-0.1.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.1.98
+Version: 0.1.99
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `requestsbankrko-0.1.98/pyproject.toml` & `requestsbankrko-0.1.99/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "requestsbankrko"
-version = "0.1.98"
+version = "0.1.99"
 description = "Гарантированно успешные web-запросы в Банки РКО"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = [ "requestsgarant>=0.0.7", "requests>=2.28", "jsoncustom>=0.0.2", "python-dotenv>=0.20.0",]
 [[project.authors]]
 name = "plp-kolyan"
```

### Comparing `requestsbankrko-0.1.98/src/bank_methods.py` & `requestsbankrko-0.1.99/src/bank_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -621,15 +621,15 @@
 class MoeDelo(RequestsGarantTestHeaders):
     headers = {'Content-Type': 'application/json; charset=UTF-8'}
     username = os.environ.get('moedelo_username')
     user_key = os.environ.get('moedelo_user_key')
 
     def __init__(self, test=test):
         super().__init__()
-        self.custom_test = True
+        self.custom_test = False
         self.test = test
         self.url = 'https://public.moedelo.org/Home/api/Registration/ExternalRegistration/V2'
         self.dict_key = self.genheaders(self.username, self.user_key)
         self.dict_key_test = self.dict_key
 
     @staticmethod
     def genheaders(user_name, user_key):
```

### Comparing `requestsbankrko-0.1.98/src/open_methods.py` & `requestsbankrko-0.1.99/src/open_methods.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.1.98/src/requestsbankrko.egg-info/PKG-INFO` & `requestsbankrko-0.1.99/src/requestsbankrko.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.1.98
+Version: 0.1.99
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `requestsbankrko-0.1.98/src/zip_functions.py` & `requestsbankrko-0.1.99/src/zip_functions.py`

 * *Files identical despite different names*

