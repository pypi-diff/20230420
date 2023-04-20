# Comparing `tmp/basaran-0.16.1.tar.gz` & `tmp/basaran-0.16.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basaran-0.16.1.tar", last modified: Wed Apr 19 14:06:54 2023, max compression
+gzip compressed data, was "basaran-0.16.2.tar", last modified: Thu Apr 20 04:37:49 2023, max compression
```

## Comparing `basaran-0.16.1.tar` & `basaran-0.16.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:06:54.599532 basaran-0.16.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-19 14:04:05.000000 basaran-0.16.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-19 14:04:05.000000 basaran-0.16.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-19 14:06:54.599532 basaran-0.16.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-19 14:04:05.000000 basaran-0.16.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:06:54.595532 basaran-0.16.1/basaran/
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-19 14:04:05.000000 basaran-0.16.1/basaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-19 14:04:05.000000 basaran-0.16.1/basaran/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-19 14:04:05.000000 basaran-0.16.1/basaran/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-04-19 14:04:05.000000 basaran-0.16.1/basaran/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:06:54.595532 basaran-0.16.1/basaran/static/
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-19 14:04:05.000000 basaran-0.16.1/basaran/static/playground.css
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-04-19 14:04:05.000000 basaran-0.16.1/basaran/static/playground.js
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-19 14:04:05.000000 basaran-0.16.1/basaran/static/presets.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:06:54.595532 basaran-0.16.1/basaran/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-19 14:04:05.000000 basaran-0.16.1/basaran/templates/playground.html
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-19 14:04:05.000000 basaran-0.16.1/basaran/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:06:54.595532 basaran-0.16.1/basaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-19 14:06:54.000000 basaran-0.16.1/basaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-19 14:06:54.000000 basaran-0.16.1/basaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:06:54.000000 basaran-0.16.1/basaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-19 14:06:54.000000 basaran-0.16.1/basaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 14:06:54.000000 basaran-0.16.1/basaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 14:06:54.599532 basaran-0.16.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-19 14:04:05.000000 basaran-0.16.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:06:54.595532 basaran-0.16.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-19 14:04:05.000000 basaran-0.16.1/tests/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-19 14:04:05.000000 basaran-0.16.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-19 14:04:05.000000 basaran-0.16.1/tests/test_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:06:54.595532 basaran-0.16.1/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-19 14:04:05.000000 basaran-0.16.1/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-19 14:04:05.000000 basaran-0.16.1/utils/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:37:49.184005 basaran-0.16.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-20 04:35:16.000000 basaran-0.16.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 04:35:16.000000 basaran-0.16.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-20 04:37:49.184005 basaran-0.16.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-20 04:35:16.000000 basaran-0.16.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:37:49.180005 basaran-0.16.2/basaran/
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:37:49.184005 basaran-0.16.2/basaran/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/static/playground.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/static/playground.js
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/static/presets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:37:49.184005 basaran-0.16.2/basaran/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/templates/playground.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-20 04:35:16.000000 basaran-0.16.2/basaran/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:37:49.180005 basaran-0.16.2/basaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-20 04:37:49.000000 basaran-0.16.2/basaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-20 04:37:49.000000 basaran-0.16.2/basaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 04:37:49.000000 basaran-0.16.2/basaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 04:37:49.000000 basaran-0.16.2/basaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 04:37:49.000000 basaran-0.16.2/basaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 04:37:49.184005 basaran-0.16.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-20 04:35:16.000000 basaran-0.16.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:37:49.184005 basaran-0.16.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-20 04:35:17.000000 basaran-0.16.2/tests/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-20 04:35:17.000000 basaran-0.16.2/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-20 04:35:17.000000 basaran-0.16.2/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 04:37:49.184005 basaran-0.16.2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-20 04:35:17.000000 basaran-0.16.2/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-20 04:35:17.000000 basaran-0.16.2/utils/render.py
```

### Comparing `basaran-0.16.1/LICENSE` & `basaran-0.16.2/LICENSE`

 * *Files identical despite different names*

### Comparing `basaran-0.16.1/PKG-INFO` & `basaran-0.16.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.16.1
+Version: 0.16.2
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.16.1/README.md` & `basaran-0.16.2/README.md`

 * *Files identical despite different names*

### Comparing `basaran-0.16.1/basaran/__init__.py` & `basaran-0.16.2/basaran/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 SERVER_CONNECTION_LIMIT = int(os.getenv("SERVER_CONNECTION_LIMIT", "512"))
 SERVER_CHANNEL_TIMEOUT = int(os.getenv("SERVER_CHANNEL_TIMEOUT", "300"))
 SERVER_MODEL_NAME = os.getenv("SERVER_MODEL_NAME", "") or MODEL
 SERVER_NO_PLAYGROUND = is_true(os.getenv("SERVER_NO_PLAYGROUND", ""))
 SERVER_CORS_ORIGINS = os.getenv("SERVER_CORS_ORIGINS", "*")
 
 # Completion-related arguments:
-COMPLETION_MAX_PROMPT = int(os.getenv("COMPLETION_MAX_PROMPT", "4096"))
-COMPLETION_MAX_TOKENS = int(os.getenv("COMPLETION_MAX_TOKENS", "4096"))
+COMPLETION_MAX_PROMPT = int(os.getenv("COMPLETION_MAX_PROMPT", "32768"))
+COMPLETION_MAX_TOKENS = int(os.getenv("COMPLETION_MAX_TOKENS", "8192"))
 COMPLETION_MAX_N = int(os.getenv("COMPLETION_MAX_N", "5"))
 COMPLETION_MAX_LOGPROBS = int(os.getenv("COMPLETION_MAX_LOGPROBS", "5"))
 COMPLETION_MAX_INTERVAL = int(os.getenv("COMPLETION_MAX_INTERVAL", "50"))
 
 # CUDA-related arguments:
 CUDA_MEMORY_FRACTION = float(os.getenv("CUDA_MEMORY_FRACTION", "1.0"))
```

### Comparing `basaran-0.16.1/basaran/__main__.py` & `basaran-0.16.2/basaran/__main__.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.1/basaran/choice.py` & `basaran-0.16.2/basaran/choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.1/basaran/model.py` & `basaran-0.16.2/basaran/model.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.1/basaran/static/playground.css` & `basaran-0.16.2/basaran/static/playground.css`

 * *Files identical despite different names*

### Comparing `basaran-0.16.1/basaran/static/playground.js` & `basaran-0.16.2/basaran/static/playground.js`

 * *Files identical despite different names*

### Comparing `basaran-0.16.1/basaran/static/presets.json` & `basaran-0.16.2/basaran/static/presets.json`

 * *Files identical despite different names*

### Comparing `basaran-0.16.1/basaran/templates/playground.html` & `basaran-0.16.2/basaran/templates/playground.html`

 * *Files identical despite different names*

### Comparing `basaran-0.16.1/basaran/tokenizer.py` & `basaran-0.16.2/basaran/tokenizer.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.1/basaran.egg-info/PKG-INFO` & `basaran-0.16.2/basaran.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.16.1
+Version: 0.16.2
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.16.1/setup.py` & `basaran-0.16.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Script for building and distributing Python packages.
 """
 from setuptools import find_packages, setup
 
-VERSION = "0.16.1"
+VERSION = "0.16.2"
 
 setup(
     name="basaran",
     version=VERSION,
     description="Open-source alternative to the OpenAI text completion API",
     long_description="Basaran is an open-source alternative to the OpenAI "
     "text completion API. It provides a compatible streaming API for your "
```

### Comparing `basaran-0.16.1/tests/test_choice.py` & `basaran-0.16.2/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.1/tests/test_model.py` & `basaran-0.16.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.1/tests/test_tokenizer.py` & `basaran-0.16.2/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.1/utils/download.py` & `basaran-0.16.2/utils/download.py`

 * *Files identical despite different names*

### Comparing `basaran-0.16.1/utils/render.py` & `basaran-0.16.2/utils/render.py`

 * *Files identical despite different names*

