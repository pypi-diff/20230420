# Comparing `tmp/aiopinecone-0.1.2.tar.gz` & `tmp/aiopinecone-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopinecone-0.1.2.tar", max compression
+gzip compressed data, was "aiopinecone-0.1.3.tar", max compression
```

## Comparing `aiopinecone-0.1.2.tar` & `aiopinecone-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-04-19 16:45:58.043208 aiopinecone-0.1.2/LICENSE
--rw-r--r--   0        0        0      114 2023-04-19 16:47:46.738483 aiopinecone-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-19 19:18:20.126249 aiopinecone-0.1.2/aiopinecone/__init__.py
--rw-r--r--   0        0        0     3771 2023-04-19 20:32:24.679491 aiopinecone-0.1.2/aiopinecone/client.py
--rw-r--r--   0        0        0      392 2023-04-20 15:20:02.621488 aiopinecone-0.1.2/aiopinecone/schemas/__init__.py
--rw-r--r--   0        0        0      177 2023-04-19 19:27:41.637122 aiopinecone-0.1.2/aiopinecone/schemas/custom.py
--rw-r--r--   0        0        0    13709 2023-04-19 20:16:51.823525 aiopinecone-0.1.2/aiopinecone/schemas/generated.py
--rw-r--r--   0        0        0      801 2023-04-20 15:20:16.418383 aiopinecone-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 aiopinecone-0.1.2/setup.py
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 aiopinecone-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-19 16:45:58.043208 aiopinecone-0.1.3/LICENSE
+-rw-r--r--   0        0        0      114 2023-04-19 16:47:46.738483 aiopinecone-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 19:18:20.126249 aiopinecone-0.1.3/aiopinecone/__init__.py
+-rw-r--r--   0        0        0     4969 2023-04-20 17:07:32.167731 aiopinecone-0.1.3/aiopinecone/client.py
+-rw-r--r--   0        0        0     2020 2023-04-20 17:07:25.772983 aiopinecone-0.1.3/aiopinecone/retry.py
+-rw-r--r--   0        0        0      392 2023-04-20 15:20:02.621488 aiopinecone-0.1.3/aiopinecone/schemas/__init__.py
+-rw-r--r--   0        0        0      177 2023-04-19 19:27:41.637122 aiopinecone-0.1.3/aiopinecone/schemas/custom.py
+-rw-r--r--   0        0        0    13709 2023-04-19 20:16:51.823525 aiopinecone-0.1.3/aiopinecone/schemas/generated.py
+-rw-r--r--   0        0        0      821 2023-04-20 16:55:54.622360 aiopinecone-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 aiopinecone-0.1.3/setup.py
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 aiopinecone-0.1.3/PKG-INFO
```

### Comparing `aiopinecone-0.1.2/LICENSE` & `aiopinecone-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopinecone-0.1.2/aiopinecone/schemas/generated.py` & `aiopinecone-0.1.3/aiopinecone/schemas/generated.py`

 * *Files identical despite different names*

### Comparing `aiopinecone-0.1.2/pyproject.toml` & `aiopinecone-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "aiopinecone"
-version = "0.1.2"
+version = "0.1.3"
 description = "An asyncio-compatible client for Pinecone DB"
 authors = ["Nikhil Shinday <nikhil@buildbetter.app>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "aiopinecone" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8.4"
 pydantic = "^1.10.7"
 typing-extensions = "^4.5.0"
+tenacity = "^8.2.2"
 
 [tool.poetry.group.dev.dependencies]
 datamodel-code-generator = "^0.18.0"
 requests = "^2.28.2"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 pydantic = {extras = ["dotenv"], version = "^1.10.7"}
```

### Comparing `aiopinecone-0.1.2/setup.py` & `aiopinecone-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0',
  'pydantic>=1.10.7,<2.0.0',
+ 'tenacity>=8.2.2,<9.0.0',
  'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'aiopinecone',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'An asyncio-compatible client for Pinecone DB',
     'long_description': '# aiopinecone\nAn asynchronous Pinecone DB Client, completely unaffiliated with Pinecone or Pinecone Systems, Inc.\n',
     'author': 'Nikhil Shinday',
     'author_email': 'nikhil@buildbetter.app',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `aiopinecone-0.1.2/PKG-INFO` & `aiopinecone-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: aiopinecone
-Version: 0.1.2
+Version: 0.1.3
 Summary: An asyncio-compatible client for Pinecone DB
 License: MIT
 Author: Nikhil Shinday
 Author-email: nikhil@buildbetter.app
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # aiopinecone
 An asynchronous Pinecone DB Client, completely unaffiliated with Pinecone or Pinecone Systems, Inc.
```

