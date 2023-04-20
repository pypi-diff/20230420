# Comparing `tmp/embedbase-1.0.3.tar.gz` & `tmp/embedbase-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.0.3.tar", max compression
+gzip compressed data, was "embedbase-1.0.4.tar", max compression
```

## Comparing `embedbase-1.0.3.tar` & `embedbase-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-19 16:10:05.171109 embedbase-1.0.3/LICENSE
--rw-r--r--   0        0        0     5733 2023-04-19 16:10:05.171109 embedbase-1.0.3/README.md
--rw-r--r--   0        0        0      121 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/__init__.py
--rw-r--r--   0        0        0     3388 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/api.py
--rw-r--r--   0        0        0    16171 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/database/__init__.py
--rw-r--r--   0        0        0     2398 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/database/base.py
--rw-r--r--   0        0        0     1164 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/database/db_utils.py
--rw-r--r--   0        0        0     4701 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/database/memory_db.py
--rw-r--r--   0        0        0      504 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/database/pinecone_db.py
--rw-r--r--   0        0        0     7938 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     4084 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0      411 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/database/weaviate_db.py
--rw-r--r--   0        0        0       77 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2049 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      575 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/logging_utils.py
--rw-r--r--   0        0        0      661 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     2101 2023-04-19 16:10:05.243109 embedbase-1.0.3/embedbase/utils.py
--rw-r--r--   0        0        0     3540 2023-04-19 16:10:05.243109 embedbase-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     7214 1970-01-01 00:00:00.000000 embedbase-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-20 14:25:59.598282 embedbase-1.0.4/LICENSE
+-rw-r--r--   0        0        0     5879 2023-04-20 14:25:59.598282 embedbase-1.0.4/README.md
+-rw-r--r--   0        0        0      121 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/__init__.py
+-rw-r--r--   0        0        0     3388 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/api.py
+-rw-r--r--   0        0        0    16171 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     2398 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/base.py
+-rw-r--r--   0        0        0     1164 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/db_utils.py
+-rw-r--r--   0        0        0     4701 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0      504 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/pinecone_db.py
+-rw-r--r--   0        0        0     7938 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     4084 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0      411 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/database/weaviate_db.py
+-rw-r--r--   0        0        0       77 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      575 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      661 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     2101 2023-04-20 14:25:59.666282 embedbase-1.0.4/embedbase/utils.py
+-rw-r--r--   0        0        0     3585 2023-04-20 14:25:59.670282 embedbase-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7360 1970-01-01 00:00:00.000000 embedbase-1.0.4/PKG-INFO
```

### Comparing `embedbase-1.0.3/LICENSE` & `embedbase-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/README.md` & `embedbase-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 <h3 align="center">The end to end platform to help you ship embeddings-powered apps.</h3>
 
   <p align="center">
     <br />
     <a href="https://discord.gg/pMNeuGrDky"><img alt="Discord" src="https://img.shields.io/discord/1066022656845025310?color=black&style=for-the-badge"></a>
     <a href="https://badge.fury.io/py/embedbase"><img alt="PyPI" src="https://img.shields.io/pypi/v/embedbase?color=black&style=for-the-badge"></a>
-    <a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase">
+    <!--<a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase">
     <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
-  </a>
+  </a>-->
     <p align="center">Open-source API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings</p>
     <p align="center">Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
     <div align="center">
       <a href="https://app.embedbase.xyz/signup">Try Embedbase Cloud now</a>
       ·
       <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
       ·
@@ -64,15 +64,17 @@
 
 Run a local-first instance of Embedbase:
 
 ```bash
 embedbase run
 ```
 
-🔥 Embedbase now runs! [Time to ship your product](#sdk)
+![pika-1681921124330-1x](https://user-images.githubusercontent.com/25003283/233138132-cf42ec0f-3821-495f-8e29-2067e643d6db.png)
+
+🔥 Embedbase now runs! [Look here to see how to use the sdk](#sdk)
 
 ℹ️ Look at the code you just ran [here](./embedbase/__main__.py), feel free to modify it to your needs.
 
 ### Managed Instance
 
 The fastest way to get started with Embedbase is signing up for free to [Embedbase Cloud](https://app.embedbase.xyz/).
```

### Comparing `embedbase-1.0.3/embedbase/__main__.py` & `embedbase-1.0.4/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/api.py` & `embedbase-1.0.4/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/app.py` & `embedbase-1.0.4/embedbase/app.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/database/base.py` & `embedbase-1.0.4/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/database/db_utils.py` & `embedbase-1.0.4/embedbase/database/db_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/database/memory_db.py` & `embedbase-1.0.4/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/database/postgres_db.py` & `embedbase-1.0.4/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/database/supabase_db.py` & `embedbase-1.0.4/embedbase/database/supabase_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/embedding/base.py` & `embedbase-1.0.4/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/embedding/cohere.py` & `embedbase-1.0.4/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/embedding/openai.py` & `embedbase-1.0.4/embedbase/embedding/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union
+from typing import List, Union, Optional
 
 from tenacity import (
     retry,
     retry_if_not_exception_type,
     stop_after_attempt,
     wait_exponential,
 )
```

### Comparing `embedbase-1.0.3/embedbase/firebase_auth.py` & `embedbase-1.0.4/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/logging_utils.py` & `embedbase-1.0.4/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/models.py` & `embedbase-1.0.4/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/settings.py` & `embedbase-1.0.4/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/strings.py` & `embedbase-1.0.4/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/embedbase/utils.py` & `embedbase-1.0.4/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.3/pyproject.toml` & `embedbase-1.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.0.3"
+version = "1.0.4"
 description = "API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 
@@ -47,21 +47,23 @@
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.10.1"}
 mypy = "^0.910"
 mypy-extensions = "^0.4.3"
 pre-commit = "^2.15.0"
 pydocstyle = "^6.1.1"
 pylint = "^2.11.1"
-pytest = "^6.2.5"
+pytest = "^7.3.1"
 pyupgrade = "^2.29.1"
 safety = "^1.10.3"
 coverage = "^6.1.2"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.1.1"
 pytest-cov = "^3.0.0"
+httpx = "^0.24.0"
+pytest-asyncio = "^0.21.0"
 
 [project.optional-dependencies]
 minimal = []
 firebase = ["firebase_admin"]
 observability = ["sentry-sdk[fastapi]"]
 pinecone = ["pinecone-client"]
 supabase = ["supabase"]
```

### Comparing `embedbase-1.0.3/PKG-INFO` & `embedbase-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.0.3
+Version: 1.0.4
 Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
@@ -42,17 +42,17 @@
 
 <h3 align="center">The end to end platform to help you ship embeddings-powered apps.</h3>
 
   <p align="center">
     <br />
     <a href="https://discord.gg/pMNeuGrDky"><img alt="Discord" src="https://img.shields.io/discord/1066022656845025310?color=black&style=for-the-badge"></a>
     <a href="https://badge.fury.io/py/embedbase"><img alt="PyPI" src="https://img.shields.io/pypi/v/embedbase?color=black&style=for-the-badge"></a>
-    <a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase">
+    <!--<a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase">
     <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
-  </a>
+  </a>-->
     <p align="center">Open-source API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings</p>
     <p align="center">Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
     <div align="center">
       <a href="https://app.embedbase.xyz/signup">Try Embedbase Cloud now</a>
       ·
       <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
       ·
@@ -98,15 +98,17 @@
 
 Run a local-first instance of Embedbase:
 
 ```bash
 embedbase run
 ```
 
-🔥 Embedbase now runs! [Time to ship your product](#sdk)
+![pika-1681921124330-1x](https://user-images.githubusercontent.com/25003283/233138132-cf42ec0f-3821-495f-8e29-2067e643d6db.png)
+
+🔥 Embedbase now runs! [Look here to see how to use the sdk](#sdk)
 
 ℹ️ Look at the code you just ran [here](./embedbase/__main__.py), feel free to modify it to your needs.
 
 ### Managed Instance
 
 The fastest way to get started with Embedbase is signing up for free to [Embedbase Cloud](https://app.embedbase.xyz/).
```

