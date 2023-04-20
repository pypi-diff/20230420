# Comparing `tmp/llama_api_server-0.2.2.tar.gz` & `tmp/llama_api_server-0.2.3.tar.gz`

## Comparing `llama_api_server-0.2.2.tar` & `llama_api_server-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/.gitattributes
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/Makefile
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/SECURITY.md
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/version.txt
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/.github/dependabot.yml
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/.github/workflows/release.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/__main__.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/app.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/config.py
--rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/model_pool.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/utils.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/models/llama_cpp.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/models/pyllama.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/models/pyllama_quant.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/LICENSE
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/README.md
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/.gitattributes
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/Makefile
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/SECURITY.md
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/version.txt
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/llama_api_server/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/llama_api_server/__main__.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/llama_api_server/app.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/llama_api_server/config.py
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/llama_api_server/model_pool.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/llama_api_server/utils.py
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/llama_api_server/models/llama_cpp.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/llama_api_server/models/pyllama.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/llama_api_server/models/pyllama_quant.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/README.md
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 llama_api_server-0.2.3/PKG-INFO
```

### Comparing `llama_api_server-0.2.2/SECURITY.md` & `llama_api_server-0.2.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.2/requirements.txt` & `llama_api_server-0.2.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.2/.github/FUNDING.yml` & `llama_api_server-0.2.3/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md` & `llama_api_server-0.2.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md` & `llama_api_server-0.2.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.2/.github/workflows/release.yml` & `llama_api_server-0.2.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.2/llama_api_server/app.py` & `llama_api_server-0.2.3/llama_api_server/app.py`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.2/llama_api_server/model_pool.py` & `llama_api_server-0.2.3/llama_api_server/model_pool.py`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.2/llama_api_server/models/llama_cpp.py` & `llama_api_server-0.2.3/llama_api_server/models/llama_cpp.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         temp = args["temperature"]
         echo = args["echo"]
         max_tokens = args["max_tokens"]
         suffix = args["suffix"]
         repeat_penalty = 1.3
 
         prompt = args["prompt"]
-        if isinstanceof(prompt, list):
+        if isinstance(prompt, list):
             prompt = prompt[0]
         prompt_tokens = self.model.str_to_token(prompt, True).tolist()
         n_past = _eval_token(
             self.model, prompt_tokens[:-1], 0, self.n_batch, self.n_thread
         )
 
         result = prompt if echo else ""
```

### Comparing `llama_api_server-0.2.2/llama_api_server/models/pyllama.py` & `llama_api_server-0.2.3/llama_api_server/models/pyllama.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class PyLlama:
     def __init__(self, params):
         try:
             import llama
             import torch
         except ImportError:
             raise ImportError(
-                'To run model with pyllama, please run "python -m pip install pyllama transformers" first'
+                'To run model with pyllama, please run "python -m pip install \'llama-api-server[pyllama]\'" first'
             )
         local_rank = 0
         world_size = 1
         max_seq_len = params.get("max_seq_len", None) or 2048
         max_batch_size = params.get("max_batch_size", None) or 2
         ckpt_dir = params["ckpt_dir"]
         tokenizer_path = params["tokenizer_path"]
@@ -44,15 +44,15 @@
         model = llama.Transformer(model_args)
         torch.set_default_tensor_type(torch.FloatTensor)
         model.load_state_dict(checkpoint, strict=False)
         self.model = llama.LLaMA(model, tokenizer)
 
     def completions(self, args):
         prompt = args["prompt"]
-        if isinstanceof(prompt, list):
+        if isinstance(prompt, list):
             prompt = prompt[0]
         top_p = args["top_p"]
         suffix = args["suffix"]
         echo = args["echo"]
         temp = args["temperature"]
         max_tokens = args["max_tokens"]
         result = self.model.generate(
```

### Comparing `llama_api_server-0.2.2/llama_api_server/models/pyllama_quant.py` & `llama_api_server-0.2.3/llama_api_server/models/pyllama_quant.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
             import llama
             import torch
             from llama.hf import LLaMATokenizer
             from llama.hf.utils import get_llama
             from llama.llama_quant import load_quant
         except ImportError:
             raise ImportError(
-                'To run model with pyllama, please run "python -m pip install pyllama transformers" first'
+                'To run model with pyllama, please run "python -m pip install \'llama-api-server[pyllama]\'" first'
             )
         max_seq_len = params.get("max_seq_len", None) or 2048
         max_batch_size = params.get("max_batch_size", None) or 16
         wbits = params.get("wbits", None) or 4
         path = params["path"]
         device = params.get("device", "cuda")
         model_name = params.get("model_name", "decapoda-research/llama-7b-hf")
@@ -27,15 +27,15 @@
         self.model.to(self.dev)
         self.tokenizer = LLaMATokenizer.from_pretrained(model_name)
 
     def completions(self, args):
         import torch
 
         prompt = args["prompt"]
-        if isinstanceof(prompt, list):
+        if isinstance(prompt, list):
             prompt = prompt[0]
         top_p = args["top_p"]
         suffix = args["suffix"]
         echo = args["echo"]
         temp = args["temperature"]
         max_tokens = args["max_tokens"]
```

### Comparing `llama_api_server-0.2.2/.gitignore` & `llama_api_server-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.2/LICENSE` & `llama_api_server-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.2/README.md` & `llama_api_server-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -74,22 +74,24 @@
 
 curl -X POST http://127.0.0.1:5000/v1/embeddings -H 'Content-Type: application/json' -d '{"model":"text-embedding-ada-002", "input":"It is good."}'  -H "Authorization: Bearer SOME_TOKEN"
 ```
 
 # 🛣️Roadmap
 
 ### Tested with
-- [X] openai-python
+- [X] [openai-python](https://github.com/openai/openai-python)
     - [X] OPENAI\_API\_TYPE=default
     - [X] OPENAI\_API\_TYPE=azure
+- [X] [llama-index](https://github.com/jerryjliu/llama_index)
 
 ### Supported APIs
 - [X] Completions
     - [X] set `temperature`, `top_p`, and `top_k`
     - [X] set `max_tokens`
+    - [ ] set `echo`
     - [ ] set `stop`
     - [ ] set `stream`
     - [ ] set `n`
     - [ ] set `presence_penalty` and `frequency_penalty`
     - [ ] set `logit_bias`
 - [X] Embeddings
     - [X] batch process
```

### Comparing `llama_api_server-0.2.2/pyproject.toml` & `llama_api_server-0.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "llama_api_server"
-version = "0.2.2"
+version = "0.2.3"
 description = "A OpenAI API compatible REST server for llama."
 authors = [
     {name = "iaalm", email= "iaalmsimon@gmail.com"}
 ]
 license = {text = "MIT"}
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 
 classifiers = [
   "Development Status :: 3 - Alpha",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
   "llamacpp>=0.1.11",
@@ -31,12 +29,13 @@
   "pyyaml",
 ]
 
 [project.optional-dependencies]
 pyllama = [
     "pyllama>=0.0.9",
     "transformers>=4.27.4",
+    "gptq",
 ]
 
 [project.urls]
 homepage = "https://github.com/iaalm/llama-api-server"
 repository = "https://github.com/iaalm/llama-api-server"
```

### Comparing `llama_api_server-0.2.2/PKG-INFO` & `llama_api_server-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: llama_api_server
-Version: 0.2.2
+Version: 0.2.3
 Summary: A OpenAI API compatible REST server for llama.
 Project-URL: homepage, https://github.com/iaalm/llama-api-server
 Project-URL: repository, https://github.com/iaalm/llama-api-server
 Author-email: iaalm <iaalmsimon@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Requires-Dist: flask>=2.0.0
 Requires-Dist: llamacpp>=0.1.11
 Requires-Dist: numpy
 Requires-Dist: pyyaml
 Provides-Extra: pyllama
+Requires-Dist: gptq; extra == 'pyllama'
 Requires-Dist: pyllama>=0.0.9; extra == 'pyllama'
 Requires-Dist: transformers>=4.27.4; extra == 'pyllama'
 Description-Content-Type: text/markdown
 
 🎭🦙 llama-api-server
 =======
 
@@ -101,22 +100,24 @@
 
 curl -X POST http://127.0.0.1:5000/v1/embeddings -H 'Content-Type: application/json' -d '{"model":"text-embedding-ada-002", "input":"It is good."}'  -H "Authorization: Bearer SOME_TOKEN"
 ```
 
 # 🛣️Roadmap
 
 ### Tested with
-- [X] openai-python
+- [X] [openai-python](https://github.com/openai/openai-python)
     - [X] OPENAI\_API\_TYPE=default
     - [X] OPENAI\_API\_TYPE=azure
+- [X] [llama-index](https://github.com/jerryjliu/llama_index)
 
 ### Supported APIs
 - [X] Completions
     - [X] set `temperature`, `top_p`, and `top_k`
     - [X] set `max_tokens`
+    - [ ] set `echo`
     - [ ] set `stop`
     - [ ] set `stream`
     - [ ] set `n`
     - [ ] set `presence_penalty` and `frequency_penalty`
     - [ ] set `logit_bias`
 - [X] Embeddings
     - [X] batch process
```

