# Comparing `tmp/aiopinecone-0.1.5.tar.gz` & `tmp/aiopinecone-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopinecone-0.1.5.tar", max compression
+gzip compressed data, was "aiopinecone-0.1.6.tar", max compression
```

## Comparing `aiopinecone-0.1.5.tar` & `aiopinecone-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-04-19 16:45:58.043208 aiopinecone-0.1.5/LICENSE
--rw-r--r--   0        0        0      114 2023-04-19 16:47:46.738483 aiopinecone-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-19 19:18:20.126249 aiopinecone-0.1.5/aiopinecone/__init__.py
--rw-r--r--   0        0        0     5090 2023-04-20 18:50:02.209149 aiopinecone-0.1.5/aiopinecone/client.py
--rw-r--r--   0        0        0     2020 2023-04-20 17:07:25.772983 aiopinecone-0.1.5/aiopinecone/retry.py
--rw-r--r--   0        0        0      392 2023-04-20 15:20:02.621488 aiopinecone-0.1.5/aiopinecone/schemas/__init__.py
--rw-r--r--   0        0        0      177 2023-04-19 19:27:41.637122 aiopinecone-0.1.5/aiopinecone/schemas/custom.py
--rw-r--r--   0        0        0    13709 2023-04-19 20:16:51.823525 aiopinecone-0.1.5/aiopinecone/schemas/generated.py
--rw-r--r--   0        0        0      821 2023-04-20 18:50:45.433078 aiopinecone-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 aiopinecone-0.1.5/setup.py
--rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 aiopinecone-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-19 16:45:58.043208 aiopinecone-0.1.6/LICENSE
+-rw-r--r--   0        0        0      114 2023-04-19 16:47:46.738483 aiopinecone-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 19:18:20.126249 aiopinecone-0.1.6/aiopinecone/__init__.py
+-rw-r--r--   0        0        0     5243 2023-04-20 19:04:54.985685 aiopinecone-0.1.6/aiopinecone/client.py
+-rw-r--r--   0        0        0     2020 2023-04-20 17:07:25.772983 aiopinecone-0.1.6/aiopinecone/retry.py
+-rw-r--r--   0        0        0      392 2023-04-20 15:20:02.621488 aiopinecone-0.1.6/aiopinecone/schemas/__init__.py
+-rw-r--r--   0        0        0      177 2023-04-19 19:27:41.637122 aiopinecone-0.1.6/aiopinecone/schemas/custom.py
+-rw-r--r--   0        0        0    13709 2023-04-19 20:16:51.823525 aiopinecone-0.1.6/aiopinecone/schemas/generated.py
+-rw-r--r--   0        0        0      821 2023-04-20 19:05:11.997951 aiopinecone-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 aiopinecone-0.1.6/setup.py
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 aiopinecone-0.1.6/PKG-INFO
```

### Comparing `aiopinecone-0.1.5/LICENSE` & `aiopinecone-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopinecone-0.1.5/aiopinecone/client.py` & `aiopinecone-0.1.6/aiopinecone/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,16 @@
         async with self.session.request(
             method,
             url,
             json=None
             if request_model_instance is None
             else request_model_instance.dict(),
         ) as resp:
+            if not (200 <= resp.status < 300):
+                raise Exception(f"Request failed with status {resp.status} and body {await resp.text()}")
             if response_model and self.parse:
                 return response_model(**await resp.json())
 
     async def describe_index(self) -> IndexMeta:
         return await self._json_request(
             "GET", self.base_path(f"databases/{self.index}"), None, IndexMeta
         )
```

### Comparing `aiopinecone-0.1.5/aiopinecone/retry.py` & `aiopinecone-0.1.6/aiopinecone/retry.py`

 * *Files identical despite different names*

### Comparing `aiopinecone-0.1.5/aiopinecone/schemas/generated.py` & `aiopinecone-0.1.6/aiopinecone/schemas/generated.py`

 * *Files identical despite different names*

### Comparing `aiopinecone-0.1.5/pyproject.toml` & `aiopinecone-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiopinecone"
-version = "0.1.5"
+version = "0.1.6"
 description = "An asyncio-compatible client for Pinecone DB"
 authors = ["Nikhil Shinday <nikhil@buildbetter.app>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "aiopinecone" }]
 
 [tool.poetry.dependencies]
```

### Comparing `aiopinecone-0.1.5/setup.py` & `aiopinecone-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['aiohttp>=3.8.4,<4.0.0',
  'pydantic>=1.10.7,<2.0.0',
  'tenacity>=8.2.2,<9.0.0',
  'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'aiopinecone',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'An asyncio-compatible client for Pinecone DB',
     'long_description': '# aiopinecone\nAn asynchronous Pinecone DB Client, completely unaffiliated with Pinecone or Pinecone Systems, Inc.\n',
     'author': 'Nikhil Shinday',
     'author_email': 'nikhil@buildbetter.app',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `aiopinecone-0.1.5/PKG-INFO` & `aiopinecone-0.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopinecone
-Version: 0.1.5
+Version: 0.1.6
 Summary: An asyncio-compatible client for Pinecone DB
 License: MIT
 Author: Nikhil Shinday
 Author-email: nikhil@buildbetter.app
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

