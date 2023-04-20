# Comparing `tmp/cogsgpt-0.0.3.tar.gz` & `tmp/cogsgpt-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogsgpt-0.0.3.tar", last modified: Thu Apr 20 13:22:10 2023, max compression
+gzip compressed data, was "cogsgpt-0.0.3.1.tar", last modified: Thu Apr 20 13:38:32 2023, max compression
```

## Comparing `cogsgpt-0.0.3.tar` & `cogsgpt-0.0.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:22:10.162054 cogsgpt-0.0.3/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-12 05:29:48.000000 cogsgpt-0.0.3/LICENSE
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       43 2023-04-15 06:53:57.000000 cogsgpt-0.0.3/MANIFEST.in
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5729 2023-04-20 13:22:10.162054 cogsgpt-0.0.3/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3985 2023-04-20 10:29:29.000000 cogsgpt-0.0.3/README.md
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:22:10.158054 cogsgpt-0.0.3/cogsgpt/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      127 2023-04-20 13:21:07.000000 cogsgpt-0.0.3/cogsgpt/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     9827 2023-04-20 12:17:50.000000 cogsgpt-0.0.3/cogsgpt/awesome_chat.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1876 2023-04-20 08:45:10.000000 cogsgpt-0.0.3/cogsgpt/awesome_prompts.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:22:10.162054 cogsgpt-0.0.3/cogsgpt/cogsmodel/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       92 2023-04-13 04:29:18.000000 cogsgpt-0.0.3/cogsgpt/cogsmodel/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      166 2023-04-11 09:46:43.000000 cogsgpt-0.0.3/cogsgpt/cogsmodel/base_model.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:22:10.162054 cogsgpt-0.0.3/cogsgpt/cogsmodel/cv/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      267 2023-04-13 09:30:09.000000 cogsgpt-0.0.3/cogsgpt/cogsmodel/cv/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3929 2023-04-13 14:26:53.000000 cogsgpt-0.0.3/cogsgpt/cogsmodel/cv/image_analysis.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2061 2023-04-13 14:42:27.000000 cogsgpt-0.0.3/cogsgpt/cogsmodel/cv/ocr.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:22:10.162054 cogsgpt-0.0.3/cogsgpt/cogsmodel/nlp/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      427 2023-04-14 03:16:26.000000 cogsgpt-0.0.3/cogsgpt/cogsmodel/nlp/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3188 2023-04-13 15:01:36.000000 cogsgpt-0.0.3/cogsgpt/cogsmodel/nlp/text_analysis.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1684 2023-04-20 12:10:44.000000 cogsgpt-0.0.3/cogsgpt/cogsmodel/nlp/text_generation.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2150 2023-04-13 15:05:49.000000 cogsgpt-0.0.3/cogsgpt/cogsmodel/nlp/text_summarize.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1676 2023-04-13 15:11:04.000000 cogsgpt-0.0.3/cogsgpt/cogsmodel/nlp/text_translation.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:22:10.162054 cogsgpt-0.0.3/cogsgpt/cogsmodel/speech/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       73 2023-04-12 13:18:32.000000 cogsgpt-0.0.3/cogsgpt/cogsmodel/speech/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3795 2023-04-13 14:49:00.000000 cogsgpt-0.0.3/cogsgpt/cogsmodel/speech/speech.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1339 2023-04-20 11:56:11.000000 cogsgpt-0.0.3/cogsgpt/llm.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:22:10.162054 cogsgpt-0.0.3/cogsgpt/metas/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      316 2023-04-12 04:35:32.000000 cogsgpt-0.0.3/cogsgpt/metas/generate_response_presteps.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2750 2023-04-20 08:45:10.000000 cogsgpt-0.0.3/cogsgpt/metas/parse_task_examples.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     7470 2023-04-20 08:45:10.000000 cogsgpt-0.0.3/cogsgpt/metas/task_metas.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1074 2023-04-20 11:56:04.000000 cogsgpt-0.0.3/cogsgpt/utils.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:22:10.158054 cogsgpt-0.0.3/cogsgpt.egg-info/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5729 2023-04-20 13:22:10.000000 cogsgpt-0.0.3/cogsgpt.egg-info/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1059 2023-04-20 13:22:10.000000 cogsgpt-0.0.3/cogsgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-20 13:22:10.000000 cogsgpt-0.0.3/cogsgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      136 2023-04-20 13:22:10.000000 cogsgpt-0.0.3/cogsgpt.egg-info/requires.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        8 2023-04-20 13:22:10.000000 cogsgpt-0.0.3/cogsgpt.egg-info/top_level.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      867 2023-04-20 13:20:46.000000 cogsgpt-0.0.3/pyproject.toml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-20 13:22:10.162054 cogsgpt-0.0.3/setup.cfg
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:22:10.162054 cogsgpt-0.0.3/tests/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      251 2023-04-14 13:22:18.000000 cogsgpt-0.0.3/tests/test_awesome_chat.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      360 2023-04-15 07:30:49.000000 cogsgpt-0.0.3/tests/test_image_analisys.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      347 2023-04-15 07:30:38.000000 cogsgpt-0.0.3/tests/test_ocr.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      601 2023-04-13 14:19:29.000000 cogsgpt-0.0.3/tests/test_speech.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1441 2023-04-13 14:19:32.000000 cogsgpt-0.0.3/tests/test_text_analysis.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      576 2023-04-14 03:20:51.000000 cogsgpt-0.0.3/tests/test_text_generation.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1970 2023-04-13 14:19:36.000000 cogsgpt-0.0.3/tests/test_text_summarize.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1168 2023-04-14 03:20:35.000000 cogsgpt-0.0.3/tests/test_text_translation.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.665611 cogsgpt-0.0.3.1/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-12 05:29:48.000000 cogsgpt-0.0.3.1/LICENSE
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       43 2023-04-15 06:53:57.000000 cogsgpt-0.0.3.1/MANIFEST.in
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5731 2023-04-20 13:38:32.665611 cogsgpt-0.0.3.1/PKG-INFO
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3985 2023-04-20 10:29:29.000000 cogsgpt-0.0.3.1/README.md
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.661611 cogsgpt-0.0.3.1/cogsgpt/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      129 2023-04-20 13:37:32.000000 cogsgpt-0.0.3.1/cogsgpt/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     9863 2023-04-20 13:36:33.000000 cogsgpt-0.0.3.1/cogsgpt/awesome_chat.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1876 2023-04-20 08:45:10.000000 cogsgpt-0.0.3.1/cogsgpt/awesome_prompts.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.661611 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       92 2023-04-13 04:29:18.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      166 2023-04-11 09:46:43.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/base_model.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.661611 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/cv/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      267 2023-04-13 09:30:09.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/cv/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3929 2023-04-13 14:26:53.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/cv/image_analysis.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2061 2023-04-13 14:42:27.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/cv/ocr.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.661611 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      427 2023-04-14 03:16:26.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3188 2023-04-13 15:01:36.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_analysis.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1684 2023-04-20 12:10:44.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_generation.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2150 2023-04-13 15:05:49.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_summarize.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1676 2023-04-13 15:11:04.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_translation.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.661611 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/speech/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       73 2023-04-12 13:18:32.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/speech/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3795 2023-04-13 14:49:00.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/speech/speech.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1339 2023-04-20 11:56:11.000000 cogsgpt-0.0.3.1/cogsgpt/llm.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.665611 cogsgpt-0.0.3.1/cogsgpt/metas/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      316 2023-04-12 04:35:32.000000 cogsgpt-0.0.3.1/cogsgpt/metas/generate_response_presteps.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2750 2023-04-20 08:45:10.000000 cogsgpt-0.0.3.1/cogsgpt/metas/parse_task_examples.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     7470 2023-04-20 08:45:10.000000 cogsgpt-0.0.3.1/cogsgpt/metas/task_metas.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1074 2023-04-20 11:56:04.000000 cogsgpt-0.0.3.1/cogsgpt/utils.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.661611 cogsgpt-0.0.3.1/cogsgpt.egg-info/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5731 2023-04-20 13:38:32.000000 cogsgpt-0.0.3.1/cogsgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1059 2023-04-20 13:38:32.000000 cogsgpt-0.0.3.1/cogsgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-20 13:38:32.000000 cogsgpt-0.0.3.1/cogsgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      136 2023-04-20 13:38:32.000000 cogsgpt-0.0.3.1/cogsgpt.egg-info/requires.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)        8 2023-04-20 13:38:32.000000 cogsgpt-0.0.3.1/cogsgpt.egg-info/top_level.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      869 2023-04-20 13:37:23.000000 cogsgpt-0.0.3.1/pyproject.toml
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-20 13:38:32.665611 cogsgpt-0.0.3.1/setup.cfg
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.665611 cogsgpt-0.0.3.1/tests/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      251 2023-04-14 13:22:18.000000 cogsgpt-0.0.3.1/tests/test_awesome_chat.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      360 2023-04-15 07:30:49.000000 cogsgpt-0.0.3.1/tests/test_image_analisys.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      347 2023-04-15 07:30:38.000000 cogsgpt-0.0.3.1/tests/test_ocr.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      601 2023-04-13 14:19:29.000000 cogsgpt-0.0.3.1/tests/test_speech.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1441 2023-04-13 14:19:32.000000 cogsgpt-0.0.3.1/tests/test_text_analysis.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      576 2023-04-14 03:20:51.000000 cogsgpt-0.0.3.1/tests/test_text_generation.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1970 2023-04-13 14:19:36.000000 cogsgpt-0.0.3.1/tests/test_text_summarize.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1168 2023-04-14 03:20:35.000000 cogsgpt-0.0.3.1/tests/test_text_translation.py
```

### Comparing `cogsgpt-0.0.3/LICENSE` & `cogsgpt-0.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/PKG-INFO` & `cogsgpt-0.0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogsgpt
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: A multi-modal LLM integrated ChatGPT with Azure Cognitive Service
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cogsgpt-0.0.3/README.md` & `cogsgpt-0.0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/cogsgpt/awesome_chat.py` & `cogsgpt-0.0.3.1/cogsgpt/awesome_chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 import os
 from typing import Dict, List
 import colorlog
 import pkg_resources
 
 from langchain import PromptTemplate
```

### Comparing `cogsgpt-0.0.3/cogsgpt/awesome_prompts.py` & `cogsgpt-0.0.3.1/cogsgpt/awesome_prompts.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/cogsgpt/cogsmodel/cv/image_analysis.py` & `cogsgpt-0.0.3.1/cogsgpt/cogsmodel/cv/image_analysis.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/cogsgpt/cogsmodel/cv/ocr.py` & `cogsgpt-0.0.3.1/cogsgpt/cogsmodel/cv/ocr.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/cogsgpt/cogsmodel/nlp/text_analysis.py` & `cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_analysis.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/cogsgpt/cogsmodel/nlp/text_generation.py` & `cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_generation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/cogsgpt/cogsmodel/nlp/text_summarize.py` & `cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_summarize.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/cogsgpt/cogsmodel/nlp/text_translation.py` & `cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_translation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/cogsgpt/cogsmodel/speech/speech.py` & `cogsgpt-0.0.3.1/cogsgpt/cogsmodel/speech/speech.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/cogsgpt/llm.py` & `cogsgpt-0.0.3.1/cogsgpt/llm.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/cogsgpt/metas/parse_task_examples.json` & `cogsgpt-0.0.3.1/cogsgpt/metas/parse_task_examples.json`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/cogsgpt/metas/task_metas.json` & `cogsgpt-0.0.3.1/cogsgpt/metas/task_metas.json`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/cogsgpt/utils.py` & `cogsgpt-0.0.3.1/cogsgpt/utils.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/cogsgpt.egg-info/PKG-INFO` & `cogsgpt-0.0.3.1/cogsgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogsgpt
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: A multi-modal LLM integrated ChatGPT with Azure Cognitive Service
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cogsgpt-0.0.3/cogsgpt.egg-info/SOURCES.txt` & `cogsgpt-0.0.3.1/cogsgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/pyproject.toml` & `cogsgpt-0.0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cogsgpt"
-version = "0.0.3"
+version = "0.0.3.1"
 description = "A multi-modal LLM integrated ChatGPT with Azure Cognitive Service"
 readme = "README.md"
 authors = [{ name = "weitian", email = "weitian.bnu@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `cogsgpt-0.0.3/tests/test_speech.py` & `cogsgpt-0.0.3.1/tests/test_speech.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/tests/test_text_analysis.py` & `cogsgpt-0.0.3.1/tests/test_text_analysis.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/tests/test_text_generation.py` & `cogsgpt-0.0.3.1/tests/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/tests/test_text_summarize.py` & `cogsgpt-0.0.3.1/tests/test_text_summarize.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3/tests/test_text_translation.py` & `cogsgpt-0.0.3.1/tests/test_text_translation.py`

 * *Files identical despite different names*

