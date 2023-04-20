# Comparing `tmp/aiopinecone-0.1.3.tar.gz` & `tmp/aiopinecone-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopinecone-0.1.3.tar", max compression
+gzip compressed data, was "aiopinecone-0.1.4.tar", max compression
```

## Comparing `aiopinecone-0.1.3.tar` & `aiopinecone-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-04-19 16:45:58.043208 aiopinecone-0.1.3/LICENSE
--rw-r--r--   0        0        0      114 2023-04-19 16:47:46.738483 aiopinecone-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-19 19:18:20.126249 aiopinecone-0.1.3/aiopinecone/__init__.py
--rw-r--r--   0        0        0     4969 2023-04-20 17:07:32.167731 aiopinecone-0.1.3/aiopinecone/client.py
--rw-r--r--   0        0        0     2020 2023-04-20 17:07:25.772983 aiopinecone-0.1.3/aiopinecone/retry.py
--rw-r--r--   0        0        0      392 2023-04-20 15:20:02.621488 aiopinecone-0.1.3/aiopinecone/schemas/__init__.py
--rw-r--r--   0        0        0      177 2023-04-19 19:27:41.637122 aiopinecone-0.1.3/aiopinecone/schemas/custom.py
--rw-r--r--   0        0        0    13709 2023-04-19 20:16:51.823525 aiopinecone-0.1.3/aiopinecone/schemas/generated.py
--rw-r--r--   0        0        0      821 2023-04-20 16:55:54.622360 aiopinecone-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 aiopinecone-0.1.3/setup.py
--rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 aiopinecone-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-19 16:45:58.043208 aiopinecone-0.1.4/LICENSE
+-rw-r--r--   0        0        0      114 2023-04-19 16:47:46.738483 aiopinecone-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 19:18:20.126249 aiopinecone-0.1.4/aiopinecone/__init__.py
+-rw-r--r--   0        0        0     5074 2023-04-20 18:41:57.076474 aiopinecone-0.1.4/aiopinecone/client.py
+-rw-r--r--   0        0        0     2020 2023-04-20 17:07:25.772983 aiopinecone-0.1.4/aiopinecone/retry.py
+-rw-r--r--   0        0        0      392 2023-04-20 15:20:02.621488 aiopinecone-0.1.4/aiopinecone/schemas/__init__.py
+-rw-r--r--   0        0        0      177 2023-04-19 19:27:41.637122 aiopinecone-0.1.4/aiopinecone/schemas/custom.py
+-rw-r--r--   0        0        0    13709 2023-04-19 20:16:51.823525 aiopinecone-0.1.4/aiopinecone/schemas/generated.py
+-rw-r--r--   0        0        0      821 2023-04-20 18:41:38.476375 aiopinecone-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 aiopinecone-0.1.4/setup.py
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 aiopinecone-0.1.4/PKG-INFO
```

### Comparing `aiopinecone-0.1.3/LICENSE` & `aiopinecone-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopinecone-0.1.3/aiopinecone/client.py` & `aiopinecone-0.1.4/aiopinecone/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from aiopinecone.schemas import FetchResponse
 from aiopinecone.schemas import IndexMeta
 from aiopinecone.schemas import QueryRequest
 from aiopinecone.schemas import QueryResponse
 from aiopinecone.schemas.custom import FetchParams
 from aiopinecone.schemas.generated import UpdateRequest
 from aiopinecone.schemas.generated import UpsertRequest
+from aiopinecone.schemas.generated import UpsertResponse
 from pydantic import BaseModel
 from pydantic import root_validator
 from tenacity import BaseRetrying
 
 PydanticModelT = TypeVar("PydanticModelT", bound=BaseModel)
 
 
@@ -30,14 +31,15 @@
     api_key: str
     region: str
     index: str
     project_id: str
     session: ClientSession
     retry: bool = False
     retryer: Optional[BaseRetrying] = None
+    parse: bool = True
 
     @root_validator(pre=True)
     def session_validation(cls, v):
         if "session" in v:
             v["session"].headers["Api-Key"] = v["api_key"]
         else:
             v["session"] = ClientSession(
@@ -128,15 +130,15 @@
         async with self.session.request(
             method,
             url,
             json=None
             if request_model_instance is None
             else request_model_instance.dict(),
         ) as resp:
-            if response_model:
+            if response_model and self.parse:
                 return response_model(**await resp.json())
 
     async def describe_index(self) -> IndexMeta:
         return await self._json_request(
             "GET", self.base_path(f"databases/{self.index}"), None, IndexMeta
         )
 
@@ -153,9 +155,9 @@
             f"vectors/fetch?{urlencode(params, doseq=True, quote_via=quote)}"
         )
         return await self._json_request("GET", url, None, FetchResponse)
 
     async def update(self, request: UpdateRequest) -> None:
         return await self._json_request("POST", self.path("vectors/update"), request)
 
-    async def upsert(self, request: UpsertRequest) -> None:
+    async def upsert(self, request: UpsertRequest) -> UpsertResponse:
         return await self._json_request("POST", self.path("vectors/upsert"), request)
```

### Comparing `aiopinecone-0.1.3/aiopinecone/retry.py` & `aiopinecone-0.1.4/aiopinecone/retry.py`

 * *Files identical despite different names*

### Comparing `aiopinecone-0.1.3/aiopinecone/schemas/generated.py` & `aiopinecone-0.1.4/aiopinecone/schemas/generated.py`

 * *Files identical despite different names*

### Comparing `aiopinecone-0.1.3/pyproject.toml` & `aiopinecone-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiopinecone"
-version = "0.1.3"
+version = "0.1.4"
 description = "An asyncio-compatible client for Pinecone DB"
 authors = ["Nikhil Shinday <nikhil@buildbetter.app>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "aiopinecone" }]
 
 [tool.poetry.dependencies]
```

### Comparing `aiopinecone-0.1.3/setup.py` & `aiopinecone-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['aiohttp>=3.8.4,<4.0.0',
  'pydantic>=1.10.7,<2.0.0',
  'tenacity>=8.2.2,<9.0.0',
  'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'aiopinecone',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'An asyncio-compatible client for Pinecone DB',
     'long_description': '# aiopinecone\nAn asynchronous Pinecone DB Client, completely unaffiliated with Pinecone or Pinecone Systems, Inc.\n',
     'author': 'Nikhil Shinday',
     'author_email': 'nikhil@buildbetter.app',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

