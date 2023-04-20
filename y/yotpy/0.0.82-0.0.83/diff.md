# Comparing `tmp/yotpy-0.0.82.tar.gz` & `tmp/yotpy-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.82.tar", last modified: Thu Apr 20 17:31:54 2023, max compression
+gzip compressed data, was "yotpy-0.0.83.tar", last modified: Thu Apr 20 17:48:02 2023, max compression
```

## Comparing `yotpy-0.0.82.tar` & `yotpy-0.0.83.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.82/.github/workflows/static.yml
--rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.82/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.82/LICENSE
--rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.82/README.md
--rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.82/docs/index.html
--rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.82/docs/search.js
--rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.82/docs/yotpy.html
--rw-r--r--   0        0        0      830 2023-04-13 22:15:48.351075 yotpy-0.0.82/pyproject.toml
--rw-r--r--   0        0        0      318 2023-04-20 17:30:36.037575 yotpy-0.0.82/yotpy/__init__.py
--rw-r--r--   0        0        0    32349 2023-04-20 17:29:42.126840 yotpy-0.0.82/yotpy/core.py
--rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.82/yotpy/exceptions.py
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 yotpy-0.0.82/PKG-INFO
+-rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.83/.github/workflows/static.yml
+-rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.83/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.83/LICENSE
+-rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.83/README.md
+-rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.83/docs/index.html
+-rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.83/docs/search.js
+-rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.83/docs/yotpy.html
+-rw-r--r--   0        0        0      830 2023-04-13 22:15:48.351075 yotpy-0.0.83/pyproject.toml
+-rw-r--r--   0        0        0      318 2023-04-20 17:40:51.083668 yotpy-0.0.83/yotpy/__init__.py
+-rw-r--r--   0        0        0    32289 2023-04-20 17:45:58.216705 yotpy-0.0.83/yotpy/core.py
+-rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.83/yotpy/exceptions.py
+-rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 yotpy-0.0.83/PKG-INFO
```

### Comparing `yotpy-0.0.82/.github/workflows/static.yml` & `yotpy-0.0.83/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.82/LICENSE` & `yotpy-0.0.83/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.82/docs/search.js` & `yotpy-0.0.83/docs/search.js`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.82/docs/yotpy.html` & `yotpy-0.0.83/docs/yotpy.html`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.82/pyproject.toml` & `yotpy-0.0.83/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.82/yotpy/core.py` & `yotpy-0.0.83/yotpy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,17 +337,16 @@
         # Create a csv writer and write the rows to the wrapped BytesIO object.
         writer = DictWriter(csv_textio, fieldnames=headers)
         writer.writeheader()
         writer.writerows(rows)
 
         # Flush the TextIOWrapper to ensure all data is written to the underlying BytesIO object
         csv_textio.flush()
-
-        # Detach the TextIOWrapper from the BytesIO object to prevent closing it
-        csv_textio.detach()
+        
+        csv_bytesio = csv_textio.detach()
 
         # Reset the BytesIO object's position to the beginning
         csv_bytesio.seek(0)
 
         return csv_bytesio
 
 class YotpoAPIWrapper:
```

### Comparing `yotpy-0.0.82/yotpy/exceptions.py` & `yotpy-0.0.83/yotpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.82/PKG-INFO` & `yotpy-0.0.83/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.82
+Version: 0.0.83
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
```

