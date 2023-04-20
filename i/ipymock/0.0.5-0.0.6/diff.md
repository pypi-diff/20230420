# Comparing `tmp/ipymock-0.0.5.tar.gz` & `tmp/ipymock-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-0.0.5.tar", last modified: Wed Apr 19 07:24:14 2023, max compression
+gzip compressed data, was "ipymock-0.0.6.tar", last modified: Thu Apr 20 04:16:36 2023, max compression
```

## Comparing `ipymock-0.0.5.tar` & `ipymock-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 07:24:14.655642 ipymock-0.0.5/
--rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.0.5/LICENSE
--rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.0.5/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-19 07:24:14.655370 ipymock-0.0.5/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     6783 2023-04-19 07:24:01.000000 ipymock-0.0.5/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 07:24:14.651910 ipymock-0.0.5/ipymock/
--rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-19 07:23:52.000000 ipymock-0.0.5/ipymock/__init__.py
--rw-r--r--   0 saintway   (501) staff       (20)     1116 2023-04-19 07:23:52.000000 ipymock-0.0.5/ipymock/_nbdev.py
--rw-r--r--   0 saintway   (501) staff       (20)     8418 2023-04-19 07:23:52.000000 ipymock-0.0.5/ipymock/mock.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 07:24:14.653942 ipymock-0.0.5/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 07:24:14.654715 ipymock-0.0.5/ipymock.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.0.5/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.0.5/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-19 07:24:14.000000 ipymock-0.0.5/ipymock.egg-info/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-19 07:24:14.000000 ipymock-0.0.5/ipymock.egg-info/SOURCES.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-19 07:24:14.000000 ipymock-0.0.5/ipymock.egg-info/dependency_links.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.0.5/ipymock.egg-info/not-zip-safe
--rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-19 07:24:14.000000 ipymock-0.0.5/ipymock.egg-info/requires.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-19 07:24:14.000000 ipymock-0.0.5/ipymock.egg-info/top_level.txt
--rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-19 07:23:43.000000 ipymock-0.0.5/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-19 07:24:14.655757 ipymock-0.0.5/setup.cfg
--rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.0.5/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 04:16:36.934500 ipymock-0.0.6/
+-rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.0.6/LICENSE
+-rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.0.6/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-20 04:16:36.934201 ipymock-0.0.6/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)     6783 2023-04-20 04:15:56.000000 ipymock-0.0.6/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 04:16:36.930061 ipymock-0.0.6/ipymock/
+-rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-20 04:15:46.000000 ipymock-0.0.6/ipymock/__init__.py
+-rw-r--r--   0 saintway   (501) staff       (20)     1116 2023-04-20 04:15:46.000000 ipymock-0.0.6/ipymock/_nbdev.py
+-rw-r--r--   0 saintway   (501) staff       (20)     8236 2023-04-20 04:15:46.000000 ipymock-0.0.6/ipymock/mock.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 04:16:36.932361 ipymock-0.0.6/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 04:16:36.933354 ipymock-0.0.6/ipymock.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.0.6/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.0.6/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-20 04:16:36.000000 ipymock-0.0.6/ipymock.egg-info/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-20 04:16:36.000000 ipymock-0.0.6/ipymock.egg-info/SOURCES.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-20 04:16:36.000000 ipymock-0.0.6/ipymock.egg-info/dependency_links.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.0.6/ipymock.egg-info/not-zip-safe
+-rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-20 04:16:36.000000 ipymock-0.0.6/ipymock.egg-info/requires.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-20 04:16:36.000000 ipymock-0.0.6/ipymock.egg-info/top_level.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-20 04:15:37.000000 ipymock-0.0.6/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-20 04:16:36.934633 ipymock-0.0.6/setup.cfg
+-rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.0.6/setup.py
```

### Comparing `ipymock-0.0.5/LICENSE` & `ipymock-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.5/PKG-INFO` & `ipymock-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.0.5
+Version: 0.0.6
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-0.0.5/README.md` & `ipymock-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.5/ipymock/__init__.py` & `ipymock-0.0.6/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.5/ipymock/_nbdev.py` & `ipymock-0.0.6/ipymock/_nbdev.py`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.5/ipymock/mock.py` & `ipymock-0.0.6/ipymock/mock.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/mock.ipynb (unless otherwise specified).
 
 __all__ = ['get_conversations', 'get_conversation', 'handle_conversation_detail', 'start_conversation',
            'generate_title', 'rename_title', 'delete_conversation', 'recover_conversation', 'clear_conversations',
            'chat_gpt_base_url', 'common', 'attrdict', 'attributize', 'delta', 'mock_create', 'mock_openai']
 
 # Internal Cell
+from queue import Queue
+
 class Common:
     chat_gpt_model = 'gpt-3.5-turbo'
     role_user = 'user'
     role_assistant = 'assistant'
 
     question_answer_map = {}
-    message_channel = []
-    exit_for_loop_channel = []
-    response_text_channel = []
-    conversation_done_channel = []
+    message_channel = Queue()
+    exit_for_loop_channel = Queue()
+    response_text_channel = Queue()
+    conversation_done_channel = Queue()
     parent_message_id = ''
     conversation_id = ''
-    reload_conversations_channel = []
-    current_node = None
+    reload_conversations_channel = Queue()
 
 # Internal Cell
 import json, os, requests, uuid
 
 # Cell
 chat_gpt_base_url = 'http://127.0.0.1:8080'
 
@@ -39,35 +40,34 @@
 
 def get_conversation(conversation_id):
     response = requests.get(f'{chat_gpt_base_url}/conversation/{conversation_id}', headers = {'Authorization': access_token})
     conversation = response.json()
     current_node = conversation['current_node']
     common.parent_message_id = current_node
     handle_conversation_detail(current_node, conversation['mapping'])
-    common.exit_for_loop_channel.append(True)
+    common.exit_for_loop_channel.put(True)
 
 def handle_conversation_detail(current_node, mapping):
     conversation_detail = mapping[current_node]
     parent_id = conversation_detail.get('parent', '')
     if parent_id != '':
         common.question_answer_map[parent_id] = conversation_detail['message']['content']['parts'][0].strip()
         handle_conversation_detail(parent_id, mapping)
     if 'message' not in conversation_detail:
         return
     message = conversation_detail['message']
     parts = message['content']['parts']
     if len(parts) > 0 and parts[0] != '':
         if message['author']['role'] == common.role_user:
-            common.message_channel.append(message)
+            common.message_channel.put(message)
 
 def start_conversation(content):
-    parent_message_id = common.parent_message_id
-    if parent_message_id == '' or common.conversation_id == '':
+    if common.parent_message_id == '' or common.conversation_id == '':
         common.conversation_id = ''
-        parent_message_id = str(uuid.uuid4())
+        common.parent_message_id = str(uuid.uuid4())
     response = requests.post(
         f'{chat_gpt_base_url}/conversation',
         headers = {
             'Authorization': access_token,
             'Content-Type': 'application/json',
             'Accept': 'text/event-stream'
         },
@@ -80,53 +80,50 @@
                 },
                 'role': common.role_user,
                 'content': {
                     'content_type': 'text',
                     'parts': [content]
                 }
             }],
-            'parent_message_id': parent_message_id,
+            'parent_message_id': common.parent_message_id,
             'model': common.chat_gpt_model,
             'conversation_id': common.conversation_id,
-            'continue_text': 'continue'
+            'continue_text': ''
         }),
         stream=True
     )
 
-    # get it again from response
-    common.parent_message_id = ''
     temp_conversation_id = ''
-
     for line in response.iter_lines():
         if not line.startswith(b'data: '):
             continue
 
+        if line.endswith(b'[DONE]'):
+            common.conversation_done_channel.put(True)
+            continue
+
         make_conversation_response = json.loads(line.decode('utf-8')[len('data: '):])
-        if common.parent_message_id == '':
-            common.parent_message_id = make_conversation_response['message']['id']
+        if make_conversation_response is None:
+            continue
+        parts = make_conversation_response['message']['content']['parts']
+        if len(parts) > 0:
+            common.response_text_channel.put(parts[0])
+            yield parts[0]
         if common.conversation_id == '':
             temp_conversation_id = make_conversation_response['conversation_id']
-        if make_conversation_response is not None:
-            parts = make_conversation_response['message']['content']['parts']
-            if len(parts) > 0:
-                common.response_text_channel.append(parts[0])
-                yield parts[0]
-            if make_conversation_response['message']['end_turn'] == True:
-                common.conversation_done_channel.append(True)
-                break
-
-        if line.endswith(b'[DONE]'):
-            common.conversation_done_channel.append(True)
-            break
+        common.parent_message_id = make_conversation_response['message']['id']
+        if make_conversation_response['message']['end_turn'] == True:
+            common.conversation_done_channel.put(True)
+            continue
 
     if common.conversation_id == '' and temp_conversation_id != '':
         common.conversation_id = temp_conversation_id
         generate_title(common.conversation_id)
     else:
-        common.reload_conversations_channel.append(True)
+        common.reload_conversations_channel.put(True)
 
 def generate_title(conversation_id):
     requests.post(
         f'{chat_gpt_base_url}/conversation/gen_title/{conversation_id}',
         headers = {
             'Authorization': access_token,
             'Content-Type': 'application/json'
@@ -173,16 +170,15 @@
         })
     )
 
 def clear_conversations():
     requests.patch(f'{chat_gpt_base_url}/conversations', headers = {'Authorization': access_token}, data = {'is_visible': False})
 
     common.conversation_id = ''
-    common.current_node = None
-    common.reload_conversations_channel.append(True)
+    common.reload_conversations_channel.put(True)
 
 # Internal Cell
 # open the JSON file and read the conversation_id
 with open(os.path.expanduser('~/.config/revChatGPT/config.json'), 'r') as f:
     conversation_id = json.load(f).get('conversation_id', None)
 
 # Internal Cell
```

### Comparing `ipymock-0.0.5/ipymock.egg-info/PKG-INFO` & `ipymock-0.0.6/ipymock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.0.5
+Version: 0.0.6
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-0.0.5/settings.ini` & `ipymock-0.0.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 user = seii-saintway
 description = A pytest plugin that let you run pytest within Jupyter Notebook cells.
 keywords = pytest interactive jupyter
 author = andrew
 author_email = andrew.saintway@gmail.com
 copyright = Neuro Spirit, DAO.
 branch = main
-version = 0.0.5
+version = 0.0.6
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `ipymock-0.0.5/setup.py` & `ipymock-0.0.6/setup.py`

 * *Files identical despite different names*

