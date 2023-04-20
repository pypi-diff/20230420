# Comparing `tmp/langchain-serve-0.0.9.dev14.tar.gz` & `tmp/langchain-serve-0.0.9.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-serve-0.0.9.dev14.tar", last modified: Thu Apr 20 07:31:49 2023, max compression
+gzip compressed data, was "langchain-serve-0.0.9.dev9.tar", last modified: Wed Apr 19 11:45:49 2023, max compression
```

## Comparing `langchain-serve-0.0.9.dev14.tar` & `langchain-serve-0.0.9.dev9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:31:49.146551 langchain-serve-0.0.9.dev14/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    28077 2023-04-20 07:31:49.146551 langchain-serve-0.0.9.dev14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26827 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:31:49.134551 langchain-serve-0.0.9.dev14/langchain_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28077 2023-04-20 07:31:49.000000 langchain-serve-0.0.9.dev14/langchain_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-20 07:31:49.000000 langchain-serve-0.0.9.dev14/langchain_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:31:49.000000 langchain-serve-0.0.9.dev14/langchain_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 07:31:49.000000 langchain-serve-0.0.9.dev14/langchain_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:31:49.000000 langchain-serve-0.0.9.dev14/langchain_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 07:31:49.000000 langchain-serve-0.0.9.dev14/langchain_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 07:31:49.000000 langchain-serve-0.0.9.dev14/langchain_serve.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:31:49.138551 langchain-serve-0.0.9.dev14/lcserve/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-20 07:31:48.000000 langchain-serve-0.0.9.dev14/lcserve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/agent-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:31:49.134551 langchain-serve-0.0.9.dev14/lcserve/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:31:49.138551 langchain-serve-0.0.9.dev14/lcserve/apps/babyagi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/apps/babyagi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/apps/babyagi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/apps/babyagi/babyagi.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/apps/babyagi/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:31:49.142551 langchain-serve-0.0.9.dev14/lcserve/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/backend/agentexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/backend/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/backend/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/backend/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:31:49.142551 langchain-serve-0.0.9.dev14/lcserve/backend/playground/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/backend/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/backend/playground/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/backend/playground/config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:31:49.146551 langchain-serve-0.0.9.dev14/lcserve/backend/playground/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/backend/playground/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/backend/playground/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/backend/playground/utils/langchain_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/backend/playground/utils/talk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/backend/playground/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/customgateway.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/customgateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17240 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/flow.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:31:49.134551 langchain-serve-0.0.9.dev14/lcserve/playground/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:31:49.146551 langchain-serve-0.0.9.dev14/lcserve/playground/babyagi/
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/playground/babyagi/playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/playground/babyagi/user_input.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/playgroundgateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/servinggateway.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/lcserve/servinggateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 07:31:49.146551 langchain-serve-0.0.9.dev14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-20 07:31:43.000000 langchain-serve-0.0.9.dev14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.140065 langchain-serve-0.0.9.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-04-19 11:45:49.140065 langchain-serve-0.0.9.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25905 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.136065 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-04-19 11:45:49.000000 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-19 11:45:49.000000 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:45:49.000000 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-19 11:45:49.000000 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:45:49.000000 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-19 11:45:49.000000 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 11:45:49.000000 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.136065 langchain-serve-0.0.9.dev9/lcserve/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-19 11:45:48.000000 langchain-serve-0.0.9.dev9/lcserve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/agent-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.136065 langchain-serve-0.0.9.dev9/lcserve/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.136065 langchain-serve-0.0.9.dev9/lcserve/apps/babyagi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/apps/babyagi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/apps/babyagi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/apps/babyagi/babyagi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/apps/babyagi/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.140065 langchain-serve-0.0.9.dev9/lcserve/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/agentexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.140065 langchain-serve-0.0.9.dev9/lcserve/backend/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.140065 langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/langchain_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/talk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/customgateway.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/customgateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/flow.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.136065 langchain-serve-0.0.9.dev9/lcserve/playground/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.140065 langchain-serve-0.0.9.dev9/lcserve/playground/babyagi/
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/playground/babyagi/playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/playground/babyagi/user_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/playgroundgateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/servinggateway.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/servinggateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 11:45:49.140065 langchain-serve-0.0.9.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/setup.py
```

### Comparing `langchain-serve-0.0.9.dev14/LICENSE` & `langchain-serve-0.0.9.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/PKG-INFO` & `langchain-serve-0.0.9.dev9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-serve
-Version: 0.0.9.dev14
+Version: 0.0.9.dev9
 Summary: Langchain Serve - serve your langchain apps on Jina AI Cloud.
 Home-page: https://github.com/jina-ai/langchain-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/langchain-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -549,21 +549,9 @@
 | [Sequential Chain](examples/sequential_chain.md) | [Link](https://langchain.readthedocs.io/en/latest/modules/chains/generic/sequential_chains.html#sequential-chain) | Expose `Chain` as RESTful/gRPC/WebSocket API locally |
 | [LLM Math Chain](examples/llm_math.md) | [Link](https://langchain.readthedocs.io/en/latest/modules/chains/examples/llm_math.html) | Expose `Chain` as RESTful/gRPC/WebSocket API locally |
 | [LLM Requests Chain](examples/llm_requests_chain.md) | [Link](https://langchain.readthedocs.io/en/latest/modules/chains/examples/llm_requests.html) | Expose `Chain` as RESTful/gRPC/WebSocket API locally |
 | [Custom Chain](examples/custom_chain.md) | [Link](https://langchain.readthedocs.io/en/latest/modules/chains/getting_started.html#create-a-custom-chain-with-the-chain-class) | Expose `Chain` as RESTful/gRPC/WebSocket API locally |
 | [Sequential Chains](examples/sequential_executors.md) | N/A | Build & scale `Chains` in separate `Executor`s |
 | [Branching Chains](examples/branching.md) | N/A | Branching `Chains` in separate `Executor`s to allow parallel execution |
 
-## Frequently Asked Questions
-
-- [My client that connects to the App gets timed-out, what should I do?](#my-client-that-connects-to-the-app-gets-timed-out-what-should-I-do)
-- [JCloud deployment failed at pushing image to Jina Hubble, what should I do?](#jcloud-deployment-failed-at-pushing-image-to-jina-hubble-what-should-i-di)
-
-### My client that connects to the App gets timed-out, what should I do?
-
-If you make long HTTP requests, you may experience timeouts due to limitations in the OSS we used in `langchain-serve`. While we are working to permanently address this issue, we recommend using HTTP/1.1 in your client as a temporary workaround.
-
-### JCloud deployment failed at pushing image to Jina Hubble, what should I do?
-
-Please use `--verbose` and retry to get more information. If you are operating on computer with `arm64` arch, please retry with `--platform linux/amd64` so the image can be built correctly.
```

### Comparing `langchain-serve-0.0.9.dev14/README.md` & `langchain-serve-0.0.9.dev9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -520,19 +520,7 @@
 | [Sequential Chain](examples/sequential_chain.md) | [Link](https://langchain.readthedocs.io/en/latest/modules/chains/generic/sequential_chains.html#sequential-chain) | Expose `Chain` as RESTful/gRPC/WebSocket API locally |
 | [LLM Math Chain](examples/llm_math.md) | [Link](https://langchain.readthedocs.io/en/latest/modules/chains/examples/llm_math.html) | Expose `Chain` as RESTful/gRPC/WebSocket API locally |
 | [LLM Requests Chain](examples/llm_requests_chain.md) | [Link](https://langchain.readthedocs.io/en/latest/modules/chains/examples/llm_requests.html) | Expose `Chain` as RESTful/gRPC/WebSocket API locally |
 | [Custom Chain](examples/custom_chain.md) | [Link](https://langchain.readthedocs.io/en/latest/modules/chains/getting_started.html#create-a-custom-chain-with-the-chain-class) | Expose `Chain` as RESTful/gRPC/WebSocket API locally |
 | [Sequential Chains](examples/sequential_executors.md) | N/A | Build & scale `Chains` in separate `Executor`s |
 | [Branching Chains](examples/branching.md) | N/A | Branching `Chains` in separate `Executor`s to allow parallel execution |
 
-## Frequently Asked Questions
-
-- [My client that connects to the App gets timed-out, what should I do?](#my-client-that-connects-to-the-app-gets-timed-out-what-should-I-do)
-- [JCloud deployment failed at pushing image to Jina Hubble, what should I do?](#jcloud-deployment-failed-at-pushing-image-to-jina-hubble-what-should-i-di)
-
-### My client that connects to the App gets timed-out, what should I do?
-
-If you make long HTTP requests, you may experience timeouts due to limitations in the OSS we used in `langchain-serve`. While we are working to permanently address this issue, we recommend using HTTP/1.1 in your client as a temporary workaround.
-
-### JCloud deployment failed at pushing image to Jina Hubble, what should I do?
-
-Please use `--verbose` and retry to get more information. If you are operating on computer with `arm64` arch, please retry with `--platform linux/amd64` so the image can be built correctly.
```

### Comparing `langchain-serve-0.0.9.dev14/langchain_serve.egg-info/PKG-INFO` & `langchain-serve-0.0.9.dev9/langchain_serve.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-serve
-Version: 0.0.9.dev14
+Version: 0.0.9.dev9
 Summary: Langchain Serve - serve your langchain apps on Jina AI Cloud.
 Home-page: https://github.com/jina-ai/langchain-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/langchain-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -549,21 +549,9 @@
 | [Sequential Chain](examples/sequential_chain.md) | [Link](https://langchain.readthedocs.io/en/latest/modules/chains/generic/sequential_chains.html#sequential-chain) | Expose `Chain` as RESTful/gRPC/WebSocket API locally |
 | [LLM Math Chain](examples/llm_math.md) | [Link](https://langchain.readthedocs.io/en/latest/modules/chains/examples/llm_math.html) | Expose `Chain` as RESTful/gRPC/WebSocket API locally |
 | [LLM Requests Chain](examples/llm_requests_chain.md) | [Link](https://langchain.readthedocs.io/en/latest/modules/chains/examples/llm_requests.html) | Expose `Chain` as RESTful/gRPC/WebSocket API locally |
 | [Custom Chain](examples/custom_chain.md) | [Link](https://langchain.readthedocs.io/en/latest/modules/chains/getting_started.html#create-a-custom-chain-with-the-chain-class) | Expose `Chain` as RESTful/gRPC/WebSocket API locally |
 | [Sequential Chains](examples/sequential_executors.md) | N/A | Build & scale `Chains` in separate `Executor`s |
 | [Branching Chains](examples/branching.md) | N/A | Branching `Chains` in separate `Executor`s to allow parallel execution |
 
-## Frequently Asked Questions
-
-- [My client that connects to the App gets timed-out, what should I do?](#my-client-that-connects-to-the-app-gets-timed-out-what-should-I-do)
-- [JCloud deployment failed at pushing image to Jina Hubble, what should I do?](#jcloud-deployment-failed-at-pushing-image-to-jina-hubble-what-should-i-di)
-
-### My client that connects to the App gets timed-out, what should I do?
-
-If you make long HTTP requests, you may experience timeouts due to limitations in the OSS we used in `langchain-serve`. While we are working to permanently address this issue, we recommend using HTTP/1.1 in your client as a temporary workaround.
-
-### JCloud deployment failed at pushing image to Jina Hubble, what should I do?
-
-Please use `--verbose` and retry to get more information. If you are operating on computer with `arm64` arch, please retry with `--platform linux/amd64` so the image can be built correctly.
```

### Comparing `langchain-serve-0.0.9.dev14/langchain_serve.egg-info/SOURCES.txt` & `langchain-serve-0.0.9.dev9/langchain_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/__main__.py` & `langchain-serve-0.0.9.dev9/lcserve/__main__.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/apps/babyagi/app.py` & `langchain-serve-0.0.9.dev9/lcserve/apps/babyagi/app.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/apps/babyagi/babyagi.py` & `langchain-serve-0.0.9.dev9/lcserve/apps/babyagi/babyagi.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/backend/agentexecutor.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/agentexecutor.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/backend/decorators.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/decorators.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/backend/gateway.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/gateway.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/backend/nginx.conf` & `langchain-serve-0.0.9.dev9/lcserve/backend/nginx.conf`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/backend/playground/app.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/playground/app.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/backend/playground/utils/helper.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/helper.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/backend/playground/utils/langchain_helper.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/langchain_helper.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/backend/playground/utils/talk.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/talk.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/backend/playground/utils/tools.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/tools.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/customgateway.Dockerfile` & `langchain-serve-0.0.9.dev9/lcserve/customgateway.Dockerfile`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/flow.py` & `langchain-serve-0.0.9.dev9/lcserve/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 from docarray import Document, DocumentArray
 from jina import Flow
 
 APP_NAME = 'langchain'
 BABYAGI_APP_NAME = 'babyagi'
 ServingGatewayConfigFile = 'servinggateway_config.yml'
 JCloudConfigFile = 'jcloud_config.yml'
-# TODO: this needs to be pulled from Jina Wolf API dynamically after the issue has been fixed on the API side
-APP_LOGS_URL = 'https://dashboard.wolf.jina.ai/d/flow/flow-monitor?var-flow={flow}&var-datasource=thanos&orgId=2&from=now-24h&to=now&viewPanel=85'
 
 
 def syncify(f):
     @wraps(f)
     def wrapper(*args, **kwargs):
         return asyncio.run(f(*args, **kwargs))
 
@@ -518,20 +516,17 @@
             return list(endpoints.values())[0] if endpoints else ''
 
         def _replace_wss_with_https(endpoint: str):
             return endpoint.replace('wss://', 'https://')
 
         status: Dict = app_status['status']
         endpoint = _get_endpoint(status)
-        flow_namespace = app_id.split("-")[-1]
-
-        _add_row('App ID', app_id, bold_key=True, bold_value=True)
+        _add_row('AppID', app_id, bold_key=True, bold_value=True)
         _add_row('Phase', status.get('phase', ''))
         _add_row('Endpoint', endpoint)
-        _add_row('App logs', APP_LOGS_URL.format(flow=flow_namespace))
         _add_row('Swagger UI', _replace_wss_with_https(f'{endpoint}/docs'))
         _add_row('OpenAPI JSON', _replace_wss_with_https(f'{endpoint}/openapi.json'))
         console.print(_t)
 
 
 async def list_apps_on_jcloud(phase: str, name: str):
     from jcloud.flow import CloudFlow
```

### Comparing `langchain-serve-0.0.9.dev14/lcserve/flow.yml` & `langchain-serve-0.0.9.dev9/lcserve/flow.yml`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/playground/babyagi/playground.py` & `langchain-serve-0.0.9.dev9/lcserve/playground/babyagi/playground.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/lcserve/playground/babyagi/user_input.py` & `langchain-serve-0.0.9.dev9/lcserve/playground/babyagi/user_input.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev14/setup.py` & `langchain-serve-0.0.9.dev9/setup.py`

 * *Files identical despite different names*

