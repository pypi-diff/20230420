# Comparing `tmp/cohere-4.1.7.tar.gz` & `tmp/cohere-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-4.1.7.tar", max compression
+gzip compressed data, was "cohere-4.2.0.tar", max compression
```

## Comparing `cohere-4.1.7.tar` & `cohere-4.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1063 2023-04-18 16:01:52.972673 cohere-4.1.7/LICENSE
--rw-r--r--   0        0        0     4480 2023-04-18 16:01:52.972673 cohere-4.1.7/README.md
--rw-r--r--   0        0        0      739 2023-04-18 16:01:52.972673 cohere-4.1.7/cohere/__init__.py
--rw-r--r--   0        0        0    35868 2023-04-18 16:01:52.972673 cohere-4.1.7/cohere/client.py
--rw-r--r--   0        0        0    27195 2023-04-18 16:01:52.972673 cohere-4.1.7/cohere/client_async.py
--rw-r--r--   0        0        0     1187 2023-04-18 16:01:52.972673 cohere-4.1.7/cohere/error.py
--rw-r--r--   0        0        0      529 2023-04-18 16:01:52.972673 cohere-4.1.7/cohere/logging.py
--rw-r--r--   0        0        0      792 2023-04-18 16:01:52.976673 cohere-4.1.7/cohere/responses/__init__.py
--rw-r--r--   0        0        0     2678 2023-04-18 16:01:52.976673 cohere-4.1.7/cohere/responses/base.py
--rw-r--r--   0        0        0     3438 2023-04-18 16:01:52.976673 cohere-4.1.7/cohere/responses/bulk_embed.py
--rw-r--r--   0        0        0     3142 2023-04-18 16:01:52.976673 cohere-4.1.7/cohere/responses/chat.py
--rw-r--r--   0        0        0     1461 2023-04-18 16:01:52.976673 cohere-4.1.7/cohere/responses/classify.py
--rw-r--r--   0        0        0     4826 2023-04-18 16:01:52.976673 cohere-4.1.7/cohere/responses/cluster.py
--rw-r--r--   0        0        0      552 2023-04-18 16:01:52.976673 cohere-4.1.7/cohere/responses/detectlang.py
--rw-r--r--   0        0        0      442 2023-04-18 16:01:52.976673 cohere-4.1.7/cohere/responses/embeddings.py
--rw-r--r--   0        0        0      342 2023-04-18 16:01:52.976673 cohere-4.1.7/cohere/responses/feedback.py
--rw-r--r--   0        0        0     5990 2023-04-18 16:01:52.976673 cohere-4.1.7/cohere/responses/generation.py
--rw-r--r--   0        0        0     2057 2023-04-18 16:01:52.976673 cohere-4.1.7/cohere/responses/rerank.py
--rw-r--r--   0        0        0      667 2023-04-18 16:01:52.976673 cohere-4.1.7/cohere/responses/summarize.py
--rw-r--r--   0        0        0     1221 2023-04-18 16:01:52.976673 cohere-4.1.7/cohere/responses/tokenize.py
--rw-r--r--   0        0        0     2614 2023-04-18 16:01:52.976673 cohere-4.1.7/cohere/utils.py
--rw-r--r--   0        0        0      653 2023-04-18 16:01:52.976673 cohere-4.1.7/pyproject.toml
--rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 cohere-4.1.7/setup.py
--rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 cohere-4.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-20 07:11:58.851364 cohere-4.2.0/LICENSE
+-rw-r--r--   0        0        0     4480 2023-04-20 07:11:58.851364 cohere-4.2.0/README.md
+-rw-r--r--   0        0        0      739 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/__init__.py
+-rw-r--r--   0        0        0    34457 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/client.py
+-rw-r--r--   0        0        0    25945 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/client_async.py
+-rw-r--r--   0        0        0     1187 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/error.py
+-rw-r--r--   0        0        0      529 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/logging.py
+-rw-r--r--   0        0        0      792 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/responses/__init__.py
+-rw-r--r--   0        0        0     2678 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/responses/base.py
+-rw-r--r--   0        0        0     3438 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/responses/bulk_embed.py
+-rw-r--r--   0        0        0     3508 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/responses/chat.py
+-rw-r--r--   0        0        0     1461 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/responses/classify.py
+-rw-r--r--   0        0        0     4826 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/responses/cluster.py
+-rw-r--r--   0        0        0      552 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/responses/detectlang.py
+-rw-r--r--   0        0        0      442 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/responses/embeddings.py
+-rw-r--r--   0        0        0      342 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/responses/feedback.py
+-rw-r--r--   0        0        0     5990 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/responses/generation.py
+-rw-r--r--   0        0        0     2057 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/responses/rerank.py
+-rw-r--r--   0        0        0      667 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/responses/summarize.py
+-rw-r--r--   0        0        0     1221 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/responses/tokenize.py
+-rw-r--r--   0        0        0     2614 2023-04-20 07:11:58.851364 cohere-4.2.0/cohere/utils.py
+-rw-r--r--   0        0        0      653 2023-04-20 07:11:58.851364 cohere-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 cohere-4.2.0/setup.py
+-rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 cohere-4.2.0/PKG-INFO
```

### Comparing `cohere-4.1.7/LICENSE` & `cohere-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/README.md` & `cohere-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/cohere/__init__.py` & `cohere-4.2.0/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/cohere/client.py` & `cohere-4.2.0/cohere/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,116 +151,92 @@
             return StreamingGenerations(response)
         else:
             return Generations.from_dict(response=response, return_likelihoods=return_likelihoods)
 
     def chat(
         self,
         query: str,
-        session_id: str = "",
         conversation_id: str = "",
         model: Optional[str] = None,
         return_chatlog: bool = False,
         return_prompt: bool = False,
         return_preamble: bool = False,
         chatlog_override: List[Dict[str, str]] = None,
-        persona_name: str = None,
-        persona_prompt: str = None,
         preamble_override: str = None,
         user_name: str = None,
         temperature: float = 0.8,
         max_tokens: int = 200,
         stream: bool = False,
     ) -> Union[Chat, StreamingChat]:
         """Returns a Chat object with the query reply.
 
         Args:
             query (str): The query to send to the chatbot.
-            session_id (str): Deprecated, use conversation_id instead.
             conversation_id (str): (Optional) The conversation id to continue the conversation.
             model (str): (Optional) The model to use for generating the next reply.
             return_chatlog (bool): (Optional) Whether to return the chatlog.
             return_prompt (bool): (Optional) Whether to return the prompt.
             return_preamble (bool): (Optional) Whether to return the preamble.
             chatlog_override (List[Dict[str, str]]): (Optional) A list of chatlog entries to override the chatlog.
-            persona_name (str): Deprecated.
-            persona_prompt (str): Deprecated, use preamble_override instead.
             preamble_override (str): (Optional) A string to override the preamble.
-            user_name (str): Deprecated.
+            user_name (str): (Optional) A string to override the username.
             temperature (float): (Optional) The temperature to use for the next reply. The higher the temperature, the more random the reply.
             max_tokens (int): (Optional) The max tokens generated for the next reply.
             stream (bool): Return streaming tokens.
         Returns:
             a Chat object if stream=False, or a StreamingChat object if stream=True
 
         Examples:
             A simple chat messsage:
                 >>> res = co.chat(query="Hey! How are you doing today?")
-                >>> print(res.reply)
+                >>> print(res.text)
                 >>> print(res.conversation_id)
             Continuing a session using a specific model:
                 >>> res = co.chat(
                 >>>     query="Hey! How are you doing today?",
                 >>>     conversation_id="1234",
                 >>>     model="command-xlarge",
                 >>>     return_chatlog=True)
-                >>> print(res.reply)
+                >>> print(res.text)
                 >>> print(res.chatlog)
             Overriding a chat log:
                 >>> res = co.chat(
                 >>>     query="What about you?",
                 >>>     conversation_id="1234",
                 >>>     chatlog_override=[
                 >>>         {'Bot': 'Hey!'},
                 >>>         {'User': 'I am doing great!'},
                 >>>         {'Bot': 'That is great to hear!'},
                 >>>     ],
                 >>>     return_chatlog=True)
-                >>> print(res.reply)
+                >>> print(res.text)
                 >>> print(res.chatlog)
             Streaming chat:
                 >>> res = co.chat(
                 >>>     query="Hey! How are you doing today?",
                 >>>     stream=True)
                 >>> for token in res:
                 >>>     print(token)
         """
         if chatlog_override is not None:
             self._validate_chatlog_override(chatlog_override)
 
-        if session_id != "":
-            conversation_id = session_id
-            logger.warning(
-                "The 'session_id' parameter is deprecated and will be removed in a future version of this function. Use 'conversation_id' instead.",
-            )
-        if persona_prompt is not None:
-            preamble_override = persona_prompt
-            logger.warning(
-                "The 'persona_prompt' parameter is deprecated and will be removed in a future version of this function. Use 'preamble_override' instead.",
-            )
-        if persona_name is not None:
-            logger.warning(
-                "The 'persona_name' parameter is deprecated and will be removed in a future version of this function.",
-            )
-        if user_name is not None:
-            logger.warning(
-                "The 'user_name' parameter is deprecated and will be removed in a future version of this function.",
-            )
-
         json_body = {
             "query": query,
             "conversation_id": conversation_id,
             "model": model,
             "return_chatlog": return_chatlog,
             "return_prompt": return_prompt,
             "return_preamble": return_preamble,
             "chatlog_override": chatlog_override,
             "preamble_override": preamble_override,
             "temperature": temperature,
             "max_tokens": max_tokens,
             "stream": stream,
+            "user_name": user_name,
         }
         response = self._request(cohere.CHAT_URL, json=json_body, stream=stream)
 
         if stream:
             return StreamingChat(response)
         else:
             return Chat.from_dict(response, query=query, client=self)
@@ -642,39 +618,35 @@
 
             self._check_response(json_response, response.headers, response.status_code)
         return json_response
 
     def create_cluster_job(
         self,
         embeddings_url: str,
-        threshold: Optional[float] = None,
         min_cluster_size: Optional[int] = None,
         n_neighbors: Optional[int] = None,
         is_deterministic: Optional[bool] = None,
     ) -> CreateClusterJobResponse:
         """Create clustering job.
 
         Args:
             embeddings_url (str): File with embeddings to cluster.
-            threshold (Optional[float], optional): Similarity threshold above which two texts are deemed to belong in
-                the same cluster. Defaults to 0.75.
             min_cluster_size (Optional[int], optional): Minimum number of elements in a cluster. Defaults to 10.
             n_neighbors (Optional[int], optional): Number of nearest neighbors used by UMAP to establish the
                 local structure of the data. Defaults to 15. For more information, please refer to
                 https://umap-learn.readthedocs.io/en/latest/parameters.html#n-neighbors
             is_deterministic (Optional[bool], optional): Determines whether the output of the cluster job is
                 deterministic. Defaults to True.
 
         Returns:
             CreateClusterJobResponse: Created clustering job handler
         """
 
         json_body = {
             "embeddings_url": embeddings_url,
-            "threshold": threshold,
             "min_cluster_size": min_cluster_size,
             "n_neighbors": n_neighbors,
             "is_deterministic": is_deterministic,
         }
 
         response = self._request(cohere.CLUSTER_JOBS_URL, json=json_body)
         return CreateClusterJobResponse.from_dict(
```

### Comparing `cohere-4.1.7/cohere/client_async.py` & `cohere-4.2.0/cohere/client_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,63 +167,42 @@
             return StreamingGenerations(response)
         else:
             return Generations.from_dict(response=response, return_likelihoods=return_likelihoods)
 
     async def chat(
         self,
         query: str,
-        session_id: str = "",
         conversation_id: str = "",
         model: Optional[str] = None,
         return_chatlog: bool = False,
         return_prompt: bool = False,
         return_preamble: bool = False,
         chatlog_override: List[Dict[str, str]] = None,
-        persona_name: str = None,
-        persona_prompt: str = None,
         preamble_override: str = None,
         user_name: str = None,
         temperature: float = 0.8,
         max_tokens: int = 200,
         stream: bool = False,
     ) -> Union[AsyncChat, StreamingChat]:
         if chatlog_override is not None:
             self._validate_chatlog_override(chatlog_override)
 
-        if session_id != "":
-            conversation_id = session_id
-            logger.warning(
-                "The 'session_id' parameter is deprecated and will be removed in a future version of this function. Use 'conversation_id' instead.",
-            )
-        if persona_prompt is not None:
-            preamble_override = persona_prompt
-            logger.warning(
-                "The 'persona_prompt' parameter is deprecated and will be removed in a future version of this function. Use 'preamble_override' instead.",
-            )
-        if persona_name is not None:
-            logger.warning(
-                "The 'persona_name' parameter is deprecated and will be removed in a future version of this function.",
-            )
-        if user_name is not None:
-            logger.warning(
-                "The 'user_name' parameter is deprecated and will be removed in a future version of this function.",
-            )
-
         json_body = {
             "query": query,
             "conversation_id": conversation_id,
             "model": model,
             "return_chatlog": return_chatlog,
             "return_prompt": return_prompt,
             "return_preamble": return_preamble,
             "chatlog_override": chatlog_override,
             "preamble_override": preamble_override,
             "temperature": temperature,
             "max_tokens": max_tokens,
             "stream": stream,
+            "user_name": user_name,
         }
 
         response = await self._request(cohere.CHAT_URL, json=json_body, stream=stream)
 
         if stream:
             return StreamingChat(response)
         else:
@@ -402,39 +381,35 @@
         for rank in reranking.results:
             rank.document = parsed_docs[rank.index]
         return reranking
 
     async def create_cluster_job(
         self,
         embeddings_url: str,
-        threshold: Optional[float] = None,
         min_cluster_size: Optional[int] = None,
         n_neighbors: Optional[int] = None,
         is_deterministic: Optional[bool] = None,
     ) -> AsyncCreateClusterJobResponse:
         """Create clustering job.
 
         Args:
             embeddings_url (str): File with embeddings to cluster.
-            threshold (Optional[float], optional): Similarity threshold above which two texts are deemed to belong in
-                the same cluster. Defaults to 0.75.
             min_cluster_size (Optional[int], optional): Minimum number of elements in a cluster. Defaults to 10.
             n_neighbors (Optional[int], optional): Number of nearest neighbors used by UMAP to establish the
                 local structure of the data. Defaults to 15. For more information, please refer to
                 https://umap-learn.readthedocs.io/en/latest/parameters.html#n-neighbors
             is_deterministic (Optional[bool], optional): Determines whether the output of the cluster job is
                 deterministic. Defaults to True.
 
         Returns:
             CreateClusterJobResponse: Created clustering job handler
         """
 
         json_body = {
             "embeddings_url": embeddings_url,
-            "threshold": threshold,
             "min_cluster_size": min_cluster_size,
             "n_neighbors": n_neighbors,
             "is_deterministic": is_deterministic,
         }
         response = await self._request(cohere.CLUSTER_JOBS_URL, json=json_body)
         return AsyncCreateClusterJobResponse.from_dict(
             response,
```

### Comparing `cohere-4.1.7/cohere/error.py` & `cohere-4.2.0/cohere/error.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/cohere/logging.py` & `cohere-4.2.0/cohere/logging.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/cohere/responses/__init__.py` & `cohere-4.2.0/cohere/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/cohere/responses/base.py` & `cohere-4.2.0/cohere/responses/base.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/cohere/responses/bulk_embed.py` & `cohere-4.2.0/cohere/responses/bulk_embed.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/cohere/responses/chat.py` & `cohere-4.2.0/cohere/responses/chat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,71 @@
 import json
+import logging
 from typing import Any, Dict, Generator, List, NamedTuple, Optional
 
 import requests
 
 from cohere.responses.base import CohereObject
 
 
 class Chat(CohereObject):
     def __init__(
         self,
         response_id: str,
+        generation_id: str,
         query: str,
-        reply: str,
+        text: str,
         conversation_id: str,
         meta: Optional[Dict[str, Any]] = None,
         prompt: Optional[str] = None,
         chatlog: Optional[List[Dict[str, str]]] = None,
         client=None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.response_id = response_id
+        self.generation_id = generation_id
         self.query = query
-        self.reply = reply
+        self.text = text
         self.conversation_id = conversation_id
         self.prompt = prompt  # optional
         self.chatlog = chatlog  # optional
         self.client = client
         self.meta = meta
 
     @classmethod
     def from_dict(cls, response: Dict[str, Any], query: str, client) -> "Chat":
         return cls(
             id=response["response_id"],
             response_id=response["response_id"],
+            generation_id=response["generation_id"],
             query=query,
             conversation_id=response["conversation_id"],
-            reply=response["reply"],
+            text=response["text"],
             prompt=response.get("prompt"),  # optional
             chatlog=response.get("chatlog"),  # optional
             client=client,
             meta=response.get("meta"),
         )
 
     def respond(self, response: str) -> "Chat":
         return self.client.chat(
             query=response,
             conversation_id=self.conversation_id,
             return_chatlog=self.chatlog is not None,
             return_prompt=self.prompt is not None,
         )
 
+    @property
+    def reply(self) -> str:
+        logging.warning(
+            "The 'reply' attribute is deprecated and will be removed in a future version of this function. Use 'text' instead.",
+        )
+        return self.text
+
 
 class AsyncChat(Chat):
     async def respond(self, response: str) -> "AsyncChat":
         return await self.client.chat(
             query=response,
             conversation_id=self.conversation_id,
             return_chatlog=self.chatlog is not None,
```

### Comparing `cohere-4.1.7/cohere/responses/classify.py` & `cohere-4.2.0/cohere/responses/classify.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/cohere/responses/cluster.py` & `cohere-4.2.0/cohere/responses/cluster.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/cohere/responses/detectlang.py` & `cohere-4.2.0/cohere/responses/detectlang.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/cohere/responses/generation.py` & `cohere-4.2.0/cohere/responses/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/cohere/responses/rerank.py` & `cohere-4.2.0/cohere/responses/rerank.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/cohere/responses/summarize.py` & `cohere-4.2.0/cohere/responses/summarize.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/cohere/responses/tokenize.py` & `cohere-4.2.0/cohere/responses/tokenize.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/cohere/utils.py` & `cohere-4.2.0/cohere/utils.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.7/pyproject.toml` & `cohere-4.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cohere"
-version = "4.1.7"
+version = "4.2.0"
 description = ""
 authors = ["Cohere"]
 readme = "README.md"
 
 [tool.black]
 line-length = 120
 target_version = ['py38']
```

### Comparing `cohere-4.1.7/setup.py` & `cohere-4.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.0,<4.0', 'backoff>=2.0,<3.0', 'requests>=2.0,<3.0']
 
 setup_kwargs = {
     'name': 'cohere',
-    'version': '4.1.7',
+    'version': '4.2.0',
     'description': '',
     'long_description': '![ci badge](https://github.com/cohere-ai/cohere-python/actions/workflows/test.yaml/badge.svg)\n![version badge](https://img.shields.io/pypi/v/cohere)\n![license badge](https://img.shields.io/github/license/cohere-ai/cohere-python)\n\n# Cohere Python SDK\n\nThis package provides functionality developed to simplify interfacing with the [Cohere API](https://docs.cohere.ai/) in Python 3.\n\n## Documentation\n\n* SDK Documentation is hosted on [Read the docs](https://cohere-sdk.readthedocs.io/en/latest/).\n  * You can build SDK documentation locally using `cd docs; make clean html`.\n* For more details on advanced parameters, you can also consult the [API documentation](https://docs.cohere.ai/reference/about).\n* See the [examples](examples/) directory for examples, including  some additional functionality for visualizations in Jupyter notebooks.\n\n## Installation\n\nThe package can be installed with `pip`:\n\n```bash\npip install --upgrade cohere\n```\n\nInstall from source:\n\n```bash\npip install .\n```\n\n### Requirements\n\n- Python 3.7+\n\n## Quick Start\n\nTo use this library, you must have an API key and specify it as a string when creating the `cohere.Client` object. API keys can be created through the [platform](https://os.cohere.ai). This is a basic example of the creating the client and using the `generate` endpoint.\n\n```python\nimport cohere\n\n# initialize the Cohere Client with an API Key\nco = cohere.Client(\'YOUR_API_KEY\')\n\n# generate a prediction for a prompt\nprediction = co.generate(\n            model=\'large\',\n            prompt=\'co:here\',\n            max_tokens=10)\n\n# print the predicted text\nprint(\'prediction: {}\'.format(prediction.generations[0].text))\n```\n\nThere is also an asyncio compatible client called `cohere.AsyncClient` with an equivalent interface. Consult the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) for more details.\n\n## Versioning\n\nEach SDK release is only compatible with the latest version of the Cohere API at the time of release. To use the SDK with an older API version, you need to download a version of the SDK tied to the API version you want. Look at the [Changelog](https://github.com/cohere-ai/cohere-python/blob/main/CHANGELOG.md) to see which SDK version to download.\n\n\n## Endpoints\n\nFor a full breakdown of endpoints and arguments, please consult the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) and [Cohere API Docs](https://docs.cohere.ai/).\n\n| Cohere Endpoint  | Function             |\n| ---------------- | -------------------- |\n| /generate        | co.generate()        |\n| /embed           | co.embed()           |\n| /classify        | co.classify()        |\n| /tokenize        | co.tokenize()        |\n| /detokenize      | co.detokenize()      |\n| /detect-language | co.detect_language() |\n\n## Models\n\nWhen you call Cohere\'s APIs we decide on a good default model for your use-case behind the scenes. The default model is great to get you started, but in production environments we recommend that you specify the model size yourself via the `model` parameter. Learn more about the available models here(https://os.cohere.ai)\n\n## Responses\n\nAll of the endpoint functions will return a Cohere object corresponding to the endpoint (e.g. for generation, it would be `Generation`). The responses can be found as instance variables of the object (e.g. generation would be `Generation.text`). The names of these instance variables and a detailed breakdown of the response body can be found in the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) and [Cohere Docs](https://docs.cohere.ai/). Printing the Cohere response object itself will display an organized view of the instance variables.\n\n## Exceptions\n\nUnsuccessful API calls from the SDK will raise an exception. Please see the documentation\'s page on [errors](https://docs.cohere.ai/errors-reference) for more information about what the errors mean.\n\n## Contributing\n\nTo set up a development environment, run:\n\n```\npoetry shell    # any time you want to run code or tests\npoetry install  # install and update dependencies in your environment, the first time\n```\n\nIn addition, to ensure your code is formatted correctly, install pre-commit hooks using:\n\n```bash\npre-commit install\n```\n\nYou can run tests locally using:\n```\npython -m pytest\n```\n\nYou can configure a different base url with:\n```bash\nCO_API_URL="https://localhost:8050" python3 foo.py\n```\nor\n```python\ncohere.COHERE_API_URL = "https://localhost:8050" # Place before client initilization\n```\n',
     'author': 'Cohere',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cohere-4.1.7/PKG-INFO` & `cohere-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 4.1.7
+Version: 4.2.0
 Summary: 
 Author: Cohere
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

