# Comparing `tmp/compress_gpt-0.1.1.tar.gz` & `tmp/compress_gpt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compress_gpt-0.1.1.tar", max compression
+gzip compressed data, was "compress_gpt-0.1.2.tar", max compression
```

## Comparing `compress_gpt-0.1.1.tar` & `compress_gpt-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1132 2023-04-19 18:06:12.449465 compress_gpt-0.1.1/README.md
--rw-r--r--   0        0        0     1110 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/__init__.py
--rw-r--r--   0        0        0     9622 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/compress.py
--rw-r--r--   0        0        0      120 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/langchain/__init__.py
--rw-r--r--   0        0        0      942 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/langchain/prompt.py
--rw-r--r--   0        0        0     1380 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/__init__.py
--rw-r--r--   0        0        0     2003 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/compare_prompts.py
--rw-r--r--   0        0        0     2818 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/compress_chunks.py
--rw-r--r--   0        0        0     1260 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/decompress.py
--rw-r--r--   0        0        0     1482 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/diff_prompts.py
--rw-r--r--   0        0        0     1692 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/fix.py
--rw-r--r--   0        0        0     1019 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/fix_json.py
--rw-r--r--   0        0        0     2984 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/identify_format.py
--rw-r--r--   0        0        0     2958 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/identify_static.py
--rw-r--r--   0        0        0     2197 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/output_parser.py
--rw-r--r--   0        0        0        0 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/tests/__init__.py
--rw-r--r--   0        0        0    15483 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/tests/test_compress.py
--rw-r--r--   0        0        0     2049 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/utils.py
--rw-r--r--   0        0        0      699 2023-04-19 18:06:12.481465 compress_gpt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 compress_gpt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1262 2023-04-20 19:44:57.238826 compress_gpt-0.1.2/README.md
+-rw-r--r--   0        0        0     1155 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/__init__.py
+-rw-r--r--   0        0        0     9622 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/compress.py
+-rw-r--r--   0        0        0      120 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/langchain/__init__.py
+-rw-r--r--   0        0        0      942 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/langchain/prompt.py
+-rw-r--r--   0        0        0     1380 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/prompts/__init__.py
+-rw-r--r--   0        0        0     2003 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/prompts/compare_prompts.py
+-rw-r--r--   0        0        0     2818 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/prompts/compress_chunks.py
+-rw-r--r--   0        0        0     1260 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/prompts/decompress.py
+-rw-r--r--   0        0        0     1482 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/prompts/diff_prompts.py
+-rw-r--r--   0        0        0     1692 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/prompts/fix.py
+-rw-r--r--   0        0        0     1019 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/prompts/fix_json.py
+-rw-r--r--   0        0        0     2984 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/prompts/identify_format.py
+-rw-r--r--   0        0        0     2958 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/prompts/identify_static.py
+-rw-r--r--   0        0        0     2197 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/prompts/output_parser.py
+-rw-r--r--   0        0        0        0 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/tests/__init__.py
+-rw-r--r--   0        0        0    15483 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/tests/test_compress.py
+-rw-r--r--   0        0        0     2049 2023-04-20 19:44:57.262827 compress_gpt-0.1.2/compress_gpt/utils.py
+-rw-r--r--   0        0        0      717 2023-04-20 19:44:57.266827 compress_gpt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 compress_gpt-0.1.2/PKG-INFO
```

### Comparing `compress_gpt-0.1.1/compress_gpt/__init__.py` & `compress_gpt-0.1.2/compress_gpt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from redis import Redis
 
 from compress_gpt.utils import has_redis
 
 nest_asyncio.apply()
 
 CACHE_DIR = Path(os.getenv("XDG_CACHE_HOME", "~/.cache")).expanduser() / "compress-gpt"
+CACHE_DIR.mkdir(parents=True, exist_ok=True)
 
 if has_redis():
     langchain.llm_cache = RedisCache(redis_=Redis())
     cache = partial(
         cached,
         ttl=timedelta(days=7),
         cache=Cache.REDIS,
```

### Comparing `compress_gpt-0.1.1/compress_gpt/compress.py` & `compress_gpt-0.1.2/compress_gpt/compress.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.1/compress_gpt/langchain/prompt.py` & `compress_gpt-0.1.2/compress_gpt/langchain/prompt.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.1/compress_gpt/prompts/__init__.py` & `compress_gpt-0.1.2/compress_gpt/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.1/compress_gpt/prompts/compare_prompts.py` & `compress_gpt-0.1.2/compress_gpt/prompts/compare_prompts.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.1/compress_gpt/prompts/compress_chunks.py` & `compress_gpt-0.1.2/compress_gpt/prompts/compress_chunks.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.1/compress_gpt/prompts/decompress.py` & `compress_gpt-0.1.2/compress_gpt/prompts/decompress.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.1/compress_gpt/prompts/diff_prompts.py` & `compress_gpt-0.1.2/compress_gpt/prompts/diff_prompts.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.1/compress_gpt/prompts/fix.py` & `compress_gpt-0.1.2/compress_gpt/prompts/fix.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.1/compress_gpt/prompts/fix_json.py` & `compress_gpt-0.1.2/compress_gpt/prompts/fix_json.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.1/compress_gpt/prompts/identify_format.py` & `compress_gpt-0.1.2/compress_gpt/prompts/identify_format.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.1/compress_gpt/prompts/identify_static.py` & `compress_gpt-0.1.2/compress_gpt/prompts/identify_static.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.1/compress_gpt/prompts/output_parser.py` & `compress_gpt-0.1.2/compress_gpt/prompts/output_parser.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.1/compress_gpt/tests/test_compress.py` & `compress_gpt-0.1.2/compress_gpt/tests/test_compress.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.1/compress_gpt/utils.py` & `compress_gpt-0.1.2/compress_gpt/utils.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.1/pyproject.toml` & `compress_gpt-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "compress-gpt"
-version = "0.1.1"
+version = "0.1.2"
 description = "Self-extracting GPT prompts for ~70% token savings."
 authors = ["Yasyf Mohamedali <yasyfm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "compress_gpt" }]
 
 [tool.poetry.dependencies]
@@ -17,14 +17,15 @@
 hiredis = "^2.2.2"
 redis = "^4.5.4"
 dill = "^0.3.6"
 rich = "^13.3.3"
 tiktoken = "^0.3.3"
 nest-asyncio = "^1.5.6"
 nltk = "^3.8.1"
+jinja2 = "^3.1.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = "^0.21.0"
 pytest = "^7.2.2"
 
 [build-system]
```

### Comparing `compress_gpt-0.1.1/PKG-INFO` & `compress_gpt-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: compress-gpt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Self-extracting GPT prompts for ~70% token savings.
 License: MIT
 Author: Yasyf Mohamedali
 Author-email: yasyfm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocache (>=0.12.0,<0.13.0)
 Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: dirtyjson (>=1.0.8,<2.0.0)
 Requires-Dist: hiredis (>=2.2.2,<3.0.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: langchain (>=0.0.132,<0.0.133)
 Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: redis (>=4.5.4,<5.0.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Description-Content-Type: text/markdown
 
 # CompressGPT
 ## Self-extracting GPT prompts for ~70% token savings
 
-Check out the accompanying blog post [here]().
+Check out the accompanying blog post [here](https://musings.yasyf.com/compressgpt-decrease-token-usage-by-70/).
 
 ### Installation
 
 ```shell
 $ pip install compress-gpt
 ```
 
@@ -59,11 +60,11 @@
 ### Demo
 
 [![asciicast](https://asciinema.org/a/578285.svg)](https://asciinema.org/a/578285)
 
 
 ### How CompressGPT Works
 
-My [blog post]() helps explain the below image.
+My [blog post](https://musings.yasyf.com/compressgpt-decrease-token-usage-by-70/) helps explain the below image.
 
 ![CompressGPT Pipeline](assets/pipeline.svg)
```

