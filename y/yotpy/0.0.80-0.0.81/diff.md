# Comparing `tmp/yotpy-0.0.80.tar.gz` & `tmp/yotpy-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.80.tar", last modified: Thu Apr 20 17:01:37 2023, max compression
+gzip compressed data, was "yotpy-0.0.81.tar", last modified: Thu Apr 20 17:17:06 2023, max compression
```

## Comparing `yotpy-0.0.80.tar` & `yotpy-0.0.81.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.80/.github/workflows/static.yml
--rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.80/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.80/LICENSE
--rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.80/README.md
--rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.80/docs/index.html
--rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.80/docs/search.js
--rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.80/docs/yotpy.html
--rw-r--r--   0        0        0      830 2023-04-13 22:15:48.351075 yotpy-0.0.80/pyproject.toml
--rw-r--r--   0        0        0      318 2023-04-20 17:00:37.055298 yotpy-0.0.80/yotpy/__init__.py
--rw-r--r--   0        0        0    32082 2023-04-20 17:01:07.154465 yotpy-0.0.80/yotpy/core.py
--rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.80/yotpy/exceptions.py
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 yotpy-0.0.80/PKG-INFO
+-rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.81/.github/workflows/static.yml
+-rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.81/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.81/LICENSE
+-rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.81/README.md
+-rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.81/docs/index.html
+-rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.81/docs/search.js
+-rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.81/docs/yotpy.html
+-rw-r--r--   0        0        0      830 2023-04-13 22:15:48.351075 yotpy-0.0.81/pyproject.toml
+-rw-r--r--   0        0        0      318 2023-04-20 17:14:22.981057 yotpy-0.0.81/yotpy/__init__.py
+-rw-r--r--   0        0        0    32236 2023-04-20 17:15:32.936299 yotpy-0.0.81/yotpy/core.py
+-rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.81/yotpy/exceptions.py
+-rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 yotpy-0.0.81/PKG-INFO
```

### Comparing `yotpy-0.0.80/.github/workflows/static.yml` & `yotpy-0.0.81/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.80/LICENSE` & `yotpy-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.80/docs/search.js` & `yotpy-0.0.81/docs/search.js`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.80/docs/yotpy.html` & `yotpy-0.0.81/docs/yotpy.html`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.80/pyproject.toml` & `yotpy-0.0.81/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.80/yotpy/core.py` & `yotpy-0.0.81/yotpy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 import asyncio
 import aiohttp
 
 from json import loads as json_loads
 from csv import DictWriter
-from io import StringIO, BytesIO
+from io import StringIO, BytesIO, TextIOWrapper
 from typing import AsyncGenerator, Iterator, Union, Optional, Callable, Union
 from html import unescape
 from urllib.parse import urlencode
 from math import ceil
 from itertools import chain
 from .exceptions import CustomException, SessionNotCreatedError, FailedToGetTokenError, PreflightException, UploadException, SendException, UserNotFound, AppNotFound
 
@@ -326,26 +326,31 @@
             rows (list[dict]): A list of rows to convert into a CSV formatted BytesIO object.
 
         Returns:
             BytesIO: A CSV formatted BytesIO object.
         """
         # Create a BytesIO object to write the CSV data to.
         csv_bytesio = BytesIO()
-        # Create a csv writer and write the rows to the BytesIO object.
-        writer = DictWriter(csv_bytesio, fieldnames=headers)
+        
+        # Wrap the BytesIO object with a TextIOWrapper using utf-8-sig encoding.
+        csv_textio = TextIOWrapper(csv_bytesio, encoding='utf-8-sig')
+
+        # Create a csv writer and write the rows to the wrapped BytesIO object.
+        writer = DictWriter(csv_textio, fieldnames=headers)
         writer.writeheader()
         writer.writerows(rows)
 
+        # Flush the TextIOWrapper to ensure all data is written to the underlying BytesIO object
+        csv_textio.flush()
+
         # Reset the BytesIO object's position to the beginning
         csv_bytesio.seek(0)
 
         return csv_bytesio
 
-    # NOTE: If you need to add another in-memory file format, maybe just refactor the above methods into a single method that accepts a memory buffer object.
-
 class YotpoAPIWrapper:
     # NOTE: Update docstring if more methods are added to account for any added functionality outside of the defined scope.
     """
     A class for interacting with the Yotpo API to fetch app and account information, review data, and send manual review requests.
 
     The YotpoAPIWrapper uses the provided app_key and secret for authentication and constructs the necessary API endpoints for making requests.
```

### Comparing `yotpy-0.0.80/yotpy/exceptions.py` & `yotpy-0.0.81/yotpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.80/PKG-INFO` & `yotpy-0.0.81/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.80
+Version: 0.0.81
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
```

