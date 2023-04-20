# Comparing `tmp/aiopinecone-0.1.1.tar.gz` & `tmp/aiopinecone-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopinecone-0.1.1.tar", max compression
+gzip compressed data, was "aiopinecone-0.1.2.tar", max compression
```

## Comparing `aiopinecone-0.1.1.tar` & `aiopinecone-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-04-19 16:45:58.043208 aiopinecone-0.1.1/LICENSE
--rw-r--r--   0        0        0      114 2023-04-19 16:47:46.738483 aiopinecone-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-19 19:18:20.126249 aiopinecone-0.1.1/aiopinecone/__init__.py
--rw-r--r--   0        0        0     3636 2023-04-19 20:26:02.107703 aiopinecone-0.1.1/aiopinecone/client.py
--rw-r--r--   0        0        0       47 2023-04-19 16:46:30.018766 aiopinecone-0.1.1/aiopinecone/schemas/__init__.py
--rw-r--r--   0        0        0      177 2023-04-19 19:27:41.637122 aiopinecone-0.1.1/aiopinecone/schemas/custom.py
--rw-r--r--   0        0        0    13709 2023-04-19 20:16:51.823525 aiopinecone-0.1.1/aiopinecone/schemas/generated.py
--rw-r--r--   0        0        0      801 2023-04-19 20:27:33.667467 aiopinecone-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 aiopinecone-0.1.1/setup.py
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 aiopinecone-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-19 16:45:58.043208 aiopinecone-0.1.2/LICENSE
+-rw-r--r--   0        0        0      114 2023-04-19 16:47:46.738483 aiopinecone-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 19:18:20.126249 aiopinecone-0.1.2/aiopinecone/__init__.py
+-rw-r--r--   0        0        0     3771 2023-04-19 20:32:24.679491 aiopinecone-0.1.2/aiopinecone/client.py
+-rw-r--r--   0        0        0      392 2023-04-20 15:20:02.621488 aiopinecone-0.1.2/aiopinecone/schemas/__init__.py
+-rw-r--r--   0        0        0      177 2023-04-19 19:27:41.637122 aiopinecone-0.1.2/aiopinecone/schemas/custom.py
+-rw-r--r--   0        0        0    13709 2023-04-19 20:16:51.823525 aiopinecone-0.1.2/aiopinecone/schemas/generated.py
+-rw-r--r--   0        0        0      801 2023-04-20 15:20:16.418383 aiopinecone-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 aiopinecone-0.1.2/setup.py
+-rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 aiopinecone-0.1.2/PKG-INFO
```

### Comparing `aiopinecone-0.1.1/LICENSE` & `aiopinecone-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopinecone-0.1.1/aiopinecone/client.py` & `aiopinecone-0.1.2/aiopinecone/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,20 @@
         return f"https://{self.index}-{self.project_id}.svc.{self.region}.pinecone.io"
 
     def base_path(self, path: str) -> str:
         return f"{self.base_url}/{path}"
 
     def path(self, path: str) -> str:
         return f"{self.index_url}/{path}"
+    
+    async def __aenter__(self):
+        return self
+    
+    async def __aexit__(self, *args):
+        await self.session.close()
 
     @overload
     async def _json_request(
         self,
         method,
         path,
         request_model_instance: None = None,
```

### Comparing `aiopinecone-0.1.1/aiopinecone/schemas/generated.py` & `aiopinecone-0.1.2/aiopinecone/schemas/generated.py`

 * *Files identical despite different names*

### Comparing `aiopinecone-0.1.1/pyproject.toml` & `aiopinecone-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiopinecone"
-version = "0.1.1"
+version = "0.1.2"
 description = "An asyncio-compatible client for Pinecone DB"
 authors = ["Nikhil Shinday <nikhil@buildbetter.app>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "aiopinecone" }]
 
 [tool.poetry.dependencies]
```

### Comparing `aiopinecone-0.1.1/setup.py` & `aiopinecone-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0',
  'pydantic>=1.10.7,<2.0.0',
  'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'aiopinecone',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'An asyncio-compatible client for Pinecone DB',
     'long_description': '# aiopinecone\nAn asynchronous Pinecone DB Client, completely unaffiliated with Pinecone or Pinecone Systems, Inc.\n',
     'author': 'Nikhil Shinday',
     'author_email': 'nikhil@buildbetter.app',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `aiopinecone-0.1.1/PKG-INFO` & `aiopinecone-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopinecone
-Version: 0.1.1
+Version: 0.1.2
 Summary: An asyncio-compatible client for Pinecone DB
 License: MIT
 Author: Nikhil Shinday
 Author-email: nikhil@buildbetter.app
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

