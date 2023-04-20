# Comparing `tmp/ipymock-0.0.6.tar.gz` & `tmp/ipymock-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-0.0.6.tar", last modified: Thu Apr 20 04:16:36 2023, max compression
+gzip compressed data, was "ipymock-0.0.7.tar", last modified: Thu Apr 20 06:41:03 2023, max compression
```

## Comparing `ipymock-0.0.6.tar` & `ipymock-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 04:16:36.934500 ipymock-0.0.6/
--rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.0.6/LICENSE
--rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.0.6/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-20 04:16:36.934201 ipymock-0.0.6/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     6783 2023-04-20 04:15:56.000000 ipymock-0.0.6/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 04:16:36.930061 ipymock-0.0.6/ipymock/
--rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-20 04:15:46.000000 ipymock-0.0.6/ipymock/__init__.py
--rw-r--r--   0 saintway   (501) staff       (20)     1116 2023-04-20 04:15:46.000000 ipymock-0.0.6/ipymock/_nbdev.py
--rw-r--r--   0 saintway   (501) staff       (20)     8236 2023-04-20 04:15:46.000000 ipymock-0.0.6/ipymock/mock.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 04:16:36.932361 ipymock-0.0.6/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 04:16:36.933354 ipymock-0.0.6/ipymock.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.0.6/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.0.6/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-20 04:16:36.000000 ipymock-0.0.6/ipymock.egg-info/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-20 04:16:36.000000 ipymock-0.0.6/ipymock.egg-info/SOURCES.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-20 04:16:36.000000 ipymock-0.0.6/ipymock.egg-info/dependency_links.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.0.6/ipymock.egg-info/not-zip-safe
--rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-20 04:16:36.000000 ipymock-0.0.6/ipymock.egg-info/requires.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-20 04:16:36.000000 ipymock-0.0.6/ipymock.egg-info/top_level.txt
--rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-20 04:15:37.000000 ipymock-0.0.6/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-20 04:16:36.934633 ipymock-0.0.6/setup.cfg
--rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.0.6/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 06:41:03.140434 ipymock-0.0.7/
+-rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.0.7/LICENSE
+-rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.0.7/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-20 06:41:03.140137 ipymock-0.0.7/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)     6783 2023-04-20 06:38:12.000000 ipymock-0.0.7/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 06:41:03.136140 ipymock-0.0.7/ipymock/
+-rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-20 06:38:02.000000 ipymock-0.0.7/ipymock/__init__.py
+-rw-r--r--   0 saintway   (501) staff       (20)     1196 2023-04-20 06:38:02.000000 ipymock-0.0.7/ipymock/_nbdev.py
+-rw-r--r--   0 saintway   (501) staff       (20)     9171 2023-04-20 06:38:02.000000 ipymock-0.0.7/ipymock/mock.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 06:41:03.138460 ipymock-0.0.7/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 06:41:03.139398 ipymock-0.0.7/ipymock.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.0.7/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.0.7/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-20 06:41:02.000000 ipymock-0.0.7/ipymock.egg-info/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-20 06:41:03.000000 ipymock-0.0.7/ipymock.egg-info/SOURCES.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-20 06:41:02.000000 ipymock-0.0.7/ipymock.egg-info/dependency_links.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.0.7/ipymock.egg-info/not-zip-safe
+-rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-20 06:41:02.000000 ipymock-0.0.7/ipymock.egg-info/requires.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-20 06:41:02.000000 ipymock-0.0.7/ipymock.egg-info/top_level.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-20 06:39:15.000000 ipymock-0.0.7/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-20 06:41:03.140549 ipymock-0.0.7/setup.cfg
+-rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.0.7/setup.py
```

### Comparing `ipymock-0.0.6/LICENSE` & `ipymock-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.6/PKG-INFO` & `ipymock-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.0.6
+Version: 0.0.7
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-0.0.6/README.md` & `ipymock-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.6/ipymock/__init__.py` & `ipymock-0.0.7/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.6/ipymock/_nbdev.py` & `ipymock-0.0.7/ipymock/_nbdev.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
          "clear_conversations": "mock.ipynb",
          "chat_gpt_base_url": "mock.ipynb",
          "common": "mock.ipynb",
          "attrdict": "mock.ipynb",
          "attributize": "mock.ipynb",
          "delta": "mock.ipynb",
          "mock_create": "mock.ipynb",
+         "chat_delta": "mock.ipynb",
+         "mock_chat_create": "mock.ipynb",
          "mock_openai": "mock.ipynb"}
 
 modules = ["__init__.py",
            "mock.py"]
 
 doc_url = "https://seii-saintway.github.io/ipymock/"
```

### Comparing `ipymock-0.0.6/ipymock/mock.py` & `ipymock-0.0.7/ipymock/mock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/mock.ipynb (unless otherwise specified).
 
 __all__ = ['get_conversations', 'get_conversation', 'handle_conversation_detail', 'start_conversation',
            'generate_title', 'rename_title', 'delete_conversation', 'recover_conversation', 'clear_conversations',
-           'chat_gpt_base_url', 'common', 'attrdict', 'attributize', 'delta', 'mock_create', 'mock_openai']
+           'chat_gpt_base_url', 'common', 'attrdict', 'attributize', 'delta', 'mock_create', 'chat_delta',
+           'mock_chat_create', 'mock_openai']
 
 # Internal Cell
 from queue import Queue
 
 class Common:
     chat_gpt_model = 'gpt-3.5-turbo'
     role_user = 'user'
@@ -208,31 +209,66 @@
 def delta(prompt):
     res = ''
     for response in start_conversation(prompt):
         yield attributize({
             'choices': [
                 {
                     'index': 0,
+                    'logprobs': None,
+                    'text': response[len(res):],
+                }
+            ],
+        })
+        res = response
+
+def mock_create(*args, **kwargs):
+    prompt = kwargs['prompt'].strip()
+
+    if kwargs.get('stream', False):
+        return delta(prompt)
+
+    response = ''
+    for response in start_conversation(prompt):
+        pass
+    return attributize({
+        'choices': [
+            {
+                'finish_reason': 'stop',
+                'index': 0,
+                'logprobs': None,
+                'text': response,
+            }
+        ],
+    })
+
+def chat_delta(prompt):
+    res = ''
+    for response in start_conversation(prompt):
+        yield attributize({
+            'choices': [
+                {
+                    'index': 0,
                     'delta': {
                         'content': response[len(res):],
                     }
                 }
             ],
         })
         res = response
 
-def mock_create(*args, **kwargs):
+def mock_chat_create(*args, **kwargs):
     summarized_prompt = ''
     for message in kwargs['messages']:
         summarized_prompt += f"{message['role']}:\n\n{message['content']}\n\n\n"
     summarized_prompt.strip()
 
     if kwargs.get('stream', False):
-        return delta(summarized_prompt)
+        return chat_delta(summarized_prompt)
 
+    response = ''
     for response in start_conversation(summarized_prompt):
         pass
     return attributize({
         'choices': [
             {
                 'finish_reason': 'stop',
                 'index': 0,
@@ -246,8 +282,9 @@
 
 # Internal Cell
 import openai, pytest
 
 # Cell
 @pytest.fixture
 def mock_openai(monkeypatch):
-    monkeypatch.setattr(openai.ChatCompletion, 'create', mock_create)
+    monkeypatch.setattr(openai.Completion, 'create', mock_create)
+    monkeypatch.setattr(openai.ChatCompletion, 'create', mock_chat_create)
```

### Comparing `ipymock-0.0.6/ipymock.egg-info/PKG-INFO` & `ipymock-0.0.7/ipymock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.0.6
+Version: 0.0.7
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-0.0.6/settings.ini` & `ipymock-0.0.7/settings.ini`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 user = seii-saintway
 description = A pytest plugin that let you run pytest within Jupyter Notebook cells.
 keywords = pytest interactive jupyter
 author = andrew
 author_email = andrew.saintway@gmail.com
 copyright = Neuro Spirit, DAO.
 branch = main
-version = 0.0.6
+version = 0.0.7
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `ipymock-0.0.6/setup.py` & `ipymock-0.0.7/setup.py`

 * *Files identical despite different names*

