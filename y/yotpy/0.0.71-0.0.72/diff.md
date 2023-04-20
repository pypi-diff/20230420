# Comparing `tmp/yotpy-0.0.71.tar.gz` & `tmp/yotpy-0.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.71.tar", last modified: Thu Apr 13 22:28:44 2023, max compression
+gzip compressed data, was "yotpy-0.0.72.tar", last modified: Thu Apr 20 14:56:54 2023, max compression
```

## Comparing `yotpy-0.0.71.tar` & `yotpy-0.0.72.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.71/.github/workflows/static.yml
--rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.71/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.71/LICENSE
--rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.71/README.md
--rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.71/docs/index.html
--rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.71/docs/search.js
--rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.71/docs/yotpy.html
--rw-r--r--   0        0        0      830 2023-04-13 22:15:48.351075 yotpy-0.0.71/pyproject.toml
--rw-r--r--   0        0        0      318 2023-04-13 22:27:56.610493 yotpy-0.0.71/yotpy/__init__.py
--rw-r--r--   0        0        0    30788 2023-04-13 22:27:35.135323 yotpy-0.0.71/yotpy/core.py
--rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.71/yotpy/exceptions.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 yotpy-0.0.71/PKG-INFO
+-rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.72/.github/workflows/static.yml
+-rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.72/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.72/LICENSE
+-rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.72/README.md
+-rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.72/docs/index.html
+-rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.72/docs/search.js
+-rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.72/docs/yotpy.html
+-rw-r--r--   0        0        0      830 2023-04-13 22:15:48.351075 yotpy-0.0.72/pyproject.toml
+-rw-r--r--   0        0        0      318 2023-04-20 14:55:47.944591 yotpy-0.0.72/yotpy/__init__.py
+-rw-r--r--   0        0        0    30788 2023-04-20 14:54:55.382613 yotpy-0.0.72/yotpy/core.py
+-rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.72/yotpy/exceptions.py
+-rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 yotpy-0.0.72/PKG-INFO
```

### Comparing `yotpy-0.0.71/.github/workflows/static.yml` & `yotpy-0.0.72/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.71/LICENSE` & `yotpy-0.0.72/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.71/docs/search.js` & `yotpy-0.0.72/docs/search.js`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.71/docs/yotpy.html` & `yotpy-0.0.72/docs/yotpy.html`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.71/pyproject.toml` & `yotpy-0.0.72/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.71/yotpy/core.py` & `yotpy-0.0.72/yotpy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,25 +281,25 @@
         # Flatten the JSON object into a list of dictionaries using the flatten method.
         for item in JSONTransformer.flatten_list(json_list, sep, exclude, include):
             rows.append(item)
             headers.update(item.keys())
         return rows, headers
 
     @staticmethod
-    def to_csv_stringio(rows: list[dict], headers: set) -> StringIO:
+    def to_csv_stringio(headers: set, rows: list[dict]) -> StringIO:
         """
         Convert a list of rows into a CSV formatted StringIO object.
 
         This method takes a list of rows (dictionaries) and a set of headers, and writes them into
         a CSV formatted StringIO object. It can be used to create a CSV file-like object without
         creating an actual file on the filesystem.
 
         Args:
-            rows (list[dict]): A list of rows to convert into a CSV formatted StringIO object.
             headers (set): A set of headers to use for the CSV data.
+            rows (list[dict]): A list of rows to convert into a CSV formatted StringIO object.
 
         Returns:
             StringIO: A CSV formatted StringIO object.
         """
         # Create a StringIO object to write the CSV data to.
         csv_stringio = StringIO()
         # Create a csv writer and write the rows to the StringIO object.
```

### Comparing `yotpy-0.0.71/yotpy/exceptions.py` & `yotpy-0.0.72/yotpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.71/PKG-INFO` & `yotpy-0.0.72/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.71
+Version: 0.0.72
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
@@ -24,7 +24,12 @@
 ## Installation
 
 Install `yotpy` using pip:
 
 ```bash
 pip install yotpy
 ```
+
+## Documentation
+
+The current documentation is updated on every update to main and can be found [here](https://wlk-dev.github.io/yotpy/yotpy.html).
+
```

