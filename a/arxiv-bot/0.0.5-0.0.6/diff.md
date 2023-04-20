# Comparing `tmp/arxiv_bot-0.0.5.tar.gz` & `tmp/arxiv_bot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv_bot-0.0.5.tar", max compression
+gzip compressed data, was "arxiv_bot-0.0.6.tar", max compression
```

## Comparing `arxiv_bot-0.0.5.tar` & `arxiv_bot-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       12 2023-02-05 03:03:40.410331 arxiv_bot-0.0.5/README.md
--rw-r--r--   0        0        0      142 2023-04-17 04:53:42.192930 arxiv_bot-0.0.5/arxiv_bot/__init__.py
--rw-r--r--   0        0        0        0 2023-02-27 04:42:53.940169 arxiv_bot-0.0.5/arxiv_bot/knowledge_base/__init__.py
--rw-r--r--   0        0        0      193 2023-02-27 10:27:55.374860 arxiv_bot-0.0.5/arxiv_bot/knowledge_base/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      175 2023-03-01 06:21:23.731532 arxiv_bot-0.0.5/arxiv_bot/knowledge_base/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    14645 2023-02-27 10:27:55.376048 arxiv_bot-0.0.5/arxiv_bot/knowledge_base/__pycache__/constructor.cpython-311.pyc
--rw-r--r--   0        0        0    14741 2023-03-01 06:07:46.313553 arxiv_bot-0.0.5/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-311.pyc
--rw-r--r--   0        0        0    14290 2023-03-17 15:27:14.374433 arxiv_bot-0.0.5/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-39.pyc
--rw-r--r--   0        0        0    10129 2023-03-01 06:15:26.092472 arxiv_bot-0.0.5/arxiv_bot/knowledge_base/__pycache__/database.cpython-311.pyc
--rw-r--r--   0        0        0     6626 2023-03-03 15:51:03.434969 arxiv_bot-0.0.5/arxiv_bot/knowledge_base/__pycache__/database.cpython-39.pyc
--rw-r--r--   0        0        0    16326 2023-04-17 04:52:43.006677 arxiv_bot-0.0.5/arxiv_bot/knowledge_base/constructors.py
--rw-r--r--   0        0        0     6955 2023-04-14 09:52:17.541131 arxiv_bot-0.0.5/arxiv_bot/knowledge_base/database.py
--rw-r--r--   0        0        0        0 2023-04-17 04:53:04.582888 arxiv_bot-0.0.5/arxiv_bot/manager/__init__.py
--rw-r--r--   0        0        0     6487 2023-04-17 05:48:27.664736 arxiv_bot-0.0.5/arxiv_bot/manager/bots.py
--rw-r--r--   0        0        0     1643 2023-02-27 10:51:36.468949 arxiv_bot-0.0.5/arxiv_bot/templates.py
--rw-r--r--   0        0        0      849 2023-04-17 05:15:10.448888 arxiv_bot-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 arxiv_bot-0.0.5/setup.py
--rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 arxiv_bot-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-02-05 03:03:40.410331 arxiv_bot-0.0.6/README.md
+-rw-r--r--   0        0        0      142 2023-04-20 09:17:28.416291 arxiv_bot-0.0.6/arxiv_bot/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-27 04:42:53.940169 arxiv_bot-0.0.6/arxiv_bot/knowledge_base/__init__.py
+-rw-r--r--   0        0        0      193 2023-02-27 10:27:55.374860 arxiv_bot-0.0.6/arxiv_bot/knowledge_base/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      175 2023-03-01 06:21:23.731532 arxiv_bot-0.0.6/arxiv_bot/knowledge_base/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    14645 2023-02-27 10:27:55.376048 arxiv_bot-0.0.6/arxiv_bot/knowledge_base/__pycache__/constructor.cpython-311.pyc
+-rw-r--r--   0        0        0    14741 2023-03-01 06:07:46.313553 arxiv_bot-0.0.6/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-311.pyc
+-rw-r--r--   0        0        0    14290 2023-03-17 15:27:14.374433 arxiv_bot-0.0.6/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-39.pyc
+-rw-r--r--   0        0        0    10129 2023-03-01 06:15:26.092472 arxiv_bot-0.0.6/arxiv_bot/knowledge_base/__pycache__/database.cpython-311.pyc
+-rw-r--r--   0        0        0     6626 2023-03-03 15:51:03.434969 arxiv_bot-0.0.6/arxiv_bot/knowledge_base/__pycache__/database.cpython-39.pyc
+-rw-r--r--   0        0        0    16326 2023-04-17 04:52:43.006677 arxiv_bot-0.0.6/arxiv_bot/knowledge_base/constructors.py
+-rw-r--r--   0        0        0     6955 2023-04-14 09:52:17.541131 arxiv_bot-0.0.6/arxiv_bot/knowledge_base/database.py
+-rw-r--r--   0        0        0        0 2023-04-17 04:53:04.582888 arxiv_bot-0.0.6/arxiv_bot/manager/__init__.py
+-rw-r--r--   0        0        0    10627 2023-04-19 12:12:40.290840 arxiv_bot-0.0.6/arxiv_bot/manager/bots.py
+-rw-r--r--   0        0        0     1643 2023-02-27 10:51:36.468949 arxiv_bot-0.0.6/arxiv_bot/templates.py
+-rw-r--r--   0        0        0      849 2023-04-20 09:17:19.312107 arxiv_bot-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 arxiv_bot-0.0.6/setup.py
+-rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 arxiv_bot-0.0.6/PKG-INFO
```

### Comparing `arxiv_bot-0.0.5/arxiv_bot/knowledge_base/__pycache__/constructor.cpython-311.pyc` & `arxiv_bot-0.0.6/arxiv_bot/knowledge_base/__pycache__/constructor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `arxiv_bot-0.0.5/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-311.pyc` & `arxiv_bot-0.0.6/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `arxiv_bot-0.0.5/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-39.pyc` & `arxiv_bot-0.0.6/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `arxiv_bot-0.0.5/arxiv_bot/knowledge_base/__pycache__/database.cpython-311.pyc` & `arxiv_bot-0.0.6/arxiv_bot/knowledge_base/__pycache__/database.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `arxiv_bot-0.0.5/arxiv_bot/knowledge_base/__pycache__/database.cpython-39.pyc` & `arxiv_bot-0.0.6/arxiv_bot/knowledge_base/__pycache__/database.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `arxiv_bot-0.0.5/arxiv_bot/knowledge_base/constructors.py` & `arxiv_bot-0.0.6/arxiv_bot/knowledge_base/constructors.py`

 * *Files identical despite different names*

### Comparing `arxiv_bot-0.0.5/arxiv_bot/knowledge_base/database.py` & `arxiv_bot-0.0.6/arxiv_bot/knowledge_base/database.py`

 * *Files identical despite different names*

### Comparing `arxiv_bot-0.0.5/arxiv_bot/templates.py` & `arxiv_bot-0.0.6/arxiv_bot/templates.py`

 * *Files identical despite different names*

### Comparing `arxiv_bot-0.0.5/pyproject.toml` & `arxiv_bot-0.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arxiv-bot"
-version = "0.0.5"
+version = "0.0.6"
 description = "ArXiv component of AI assistant"
 authors = ["James Briggs <james@aurelio.ai>"]
 readme = "README.md"
 packages = [
     {include = "arxiv_bot"},
     {include = "arxiv_bot/knowledge_base"}
 ]
```

### Comparing `arxiv_bot-0.0.5/setup.py` & `arxiv_bot-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'pypdf2>=3.0.1,<4.0.0',
  'tiktoken>=0.2.0,<0.3.0',
  'tqdm>=4.64.1,<5.0.0',
  'transformers>=4.26.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'arxiv-bot',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'ArXiv component of AI assistant',
     'long_description': '# Arxiv Bot\n',
     'author': 'James Briggs',
     'author_email': 'james@aurelio.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `arxiv_bot-0.0.5/PKG-INFO` & `arxiv_bot-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv-bot
-Version: 0.0.5
+Version: 0.0.6
 Summary: ArXiv component of AI assistant
 Author: James Briggs
 Author-email: james@aurelio.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

