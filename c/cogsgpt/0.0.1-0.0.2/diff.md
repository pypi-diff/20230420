# Comparing `tmp/cogsgpt-0.0.1.tar.gz` & `tmp/cogsgpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogsgpt-0.0.1.tar", last modified: Sat Apr 15 08:51:16 2023, max compression
+gzip compressed data, was "cogsgpt-0.0.2.tar", last modified: Thu Apr 20 12:26:36 2023, max compression
```

## Comparing `cogsgpt-0.0.1.tar` & `cogsgpt-0.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-15 08:51:16.816487 cogsgpt-0.0.1/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-12 05:29:48.000000 cogsgpt-0.0.1/LICENSE
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       43 2023-04-15 06:53:57.000000 cogsgpt-0.0.1/MANIFEST.in
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5360 2023-04-15 08:51:16.816487 cogsgpt-0.0.1/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3616 2023-04-15 08:46:57.000000 cogsgpt-0.0.1/README.md
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-15 08:51:16.800487 cogsgpt-0.0.1/cogsgpt/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      104 2023-04-14 02:13:40.000000 cogsgpt-0.0.1/cogsgpt/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     8845 2023-04-15 07:07:39.000000 cogsgpt-0.0.1/cogsgpt/awesome_chat.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1876 2023-04-14 14:34:46.000000 cogsgpt-0.0.1/cogsgpt/awesome_prompts.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-15 08:51:16.804487 cogsgpt-0.0.1/cogsgpt/cogsmodel/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       92 2023-04-13 04:29:18.000000 cogsgpt-0.0.1/cogsgpt/cogsmodel/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      166 2023-04-11 09:46:43.000000 cogsgpt-0.0.1/cogsgpt/cogsmodel/base_model.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-15 08:51:16.804487 cogsgpt-0.0.1/cogsgpt/cogsmodel/cv/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      267 2023-04-13 09:30:09.000000 cogsgpt-0.0.1/cogsgpt/cogsmodel/cv/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3929 2023-04-13 14:26:53.000000 cogsgpt-0.0.1/cogsgpt/cogsmodel/cv/image_analysis.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2061 2023-04-13 14:42:27.000000 cogsgpt-0.0.1/cogsgpt/cogsmodel/cv/ocr.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-15 08:51:16.808487 cogsgpt-0.0.1/cogsgpt/cogsmodel/nlp/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      427 2023-04-14 03:16:26.000000 cogsgpt-0.0.1/cogsgpt/cogsmodel/nlp/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3188 2023-04-13 15:01:36.000000 cogsgpt-0.0.1/cogsgpt/cogsmodel/nlp/text_analysis.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1582 2023-04-14 03:45:33.000000 cogsgpt-0.0.1/cogsgpt/cogsmodel/nlp/text_generation.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2150 2023-04-13 15:05:49.000000 cogsgpt-0.0.1/cogsgpt/cogsmodel/nlp/text_summarize.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1676 2023-04-13 15:11:04.000000 cogsgpt-0.0.1/cogsgpt/cogsmodel/nlp/text_translation.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-15 08:51:16.808487 cogsgpt-0.0.1/cogsgpt/cogsmodel/speech/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       73 2023-04-12 13:18:32.000000 cogsgpt-0.0.1/cogsgpt/cogsmodel/speech/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3795 2023-04-13 14:49:00.000000 cogsgpt-0.0.1/cogsgpt/cogsmodel/speech/speech.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1178 2023-04-14 07:07:25.000000 cogsgpt-0.0.1/cogsgpt/llm.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-15 08:51:16.812487 cogsgpt-0.0.1/cogsgpt/metas/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      316 2023-04-12 04:35:32.000000 cogsgpt-0.0.1/cogsgpt/metas/generate_response_presteps.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2750 2023-04-14 10:03:47.000000 cogsgpt-0.0.1/cogsgpt/metas/parse_task_examples.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     7470 2023-04-14 12:14:14.000000 cogsgpt-0.0.1/cogsgpt/metas/task_metas.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      799 2023-04-13 14:25:46.000000 cogsgpt-0.0.1/cogsgpt/utils.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-15 08:51:16.804487 cogsgpt-0.0.1/cogsgpt.egg-info/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5360 2023-04-15 08:51:16.000000 cogsgpt-0.0.1/cogsgpt.egg-info/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1059 2023-04-15 08:51:16.000000 cogsgpt-0.0.1/cogsgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-15 08:51:16.000000 cogsgpt-0.0.1/cogsgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      136 2023-04-15 08:51:16.000000 cogsgpt-0.0.1/cogsgpt.egg-info/requires.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        8 2023-04-15 08:51:16.000000 cogsgpt-0.0.1/cogsgpt.egg-info/top_level.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      867 2023-04-15 07:09:17.000000 cogsgpt-0.0.1/pyproject.toml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-15 08:51:16.816487 cogsgpt-0.0.1/setup.cfg
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-15 08:51:16.812487 cogsgpt-0.0.1/tests/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      251 2023-04-14 13:22:18.000000 cogsgpt-0.0.1/tests/test_awesome_chat.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      360 2023-04-15 07:30:49.000000 cogsgpt-0.0.1/tests/test_image_analisys.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      347 2023-04-15 07:30:38.000000 cogsgpt-0.0.1/tests/test_ocr.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      601 2023-04-13 14:19:29.000000 cogsgpt-0.0.1/tests/test_speech.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1441 2023-04-13 14:19:32.000000 cogsgpt-0.0.1/tests/test_text_analysis.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      576 2023-04-14 03:20:51.000000 cogsgpt-0.0.1/tests/test_text_generation.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1970 2023-04-13 14:19:36.000000 cogsgpt-0.0.1/tests/test_text_summarize.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1168 2023-04-14 03:20:35.000000 cogsgpt-0.0.1/tests/test_text_translation.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 12:26:36.611819 cogsgpt-0.0.2/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-12 05:29:48.000000 cogsgpt-0.0.2/LICENSE
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       43 2023-04-15 06:53:57.000000 cogsgpt-0.0.2/MANIFEST.in
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5729 2023-04-20 12:26:36.611819 cogsgpt-0.0.2/PKG-INFO
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3985 2023-04-20 10:29:29.000000 cogsgpt-0.0.2/README.md
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 12:26:36.579819 cogsgpt-0.0.2/cogsgpt/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      127 2023-04-20 12:24:47.000000 cogsgpt-0.0.2/cogsgpt/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     9827 2023-04-20 12:17:50.000000 cogsgpt-0.0.2/cogsgpt/awesome_chat.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1876 2023-04-20 08:45:10.000000 cogsgpt-0.0.2/cogsgpt/awesome_prompts.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 12:26:36.587819 cogsgpt-0.0.2/cogsgpt/cogsgpt.egg-info/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5729 2023-04-20 12:26:36.000000 cogsgpt-0.0.2/cogsgpt/cogsgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1099 2023-04-20 12:26:36.000000 cogsgpt-0.0.2/cogsgpt/cogsgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-20 12:26:36.000000 cogsgpt-0.0.2/cogsgpt/cogsgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      136 2023-04-20 12:26:36.000000 cogsgpt-0.0.2/cogsgpt/cogsgpt.egg-info/requires.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       64 2023-04-20 12:26:36.000000 cogsgpt-0.0.2/cogsgpt/cogsgpt.egg-info/top_level.txt
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 12:26:36.587819 cogsgpt-0.0.2/cogsgpt/cogsmodel/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       92 2023-04-13 04:29:18.000000 cogsgpt-0.0.2/cogsgpt/cogsmodel/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      166 2023-04-11 09:46:43.000000 cogsgpt-0.0.2/cogsgpt/cogsmodel/base_model.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 12:26:36.591819 cogsgpt-0.0.2/cogsgpt/cogsmodel/cv/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      267 2023-04-13 09:30:09.000000 cogsgpt-0.0.2/cogsgpt/cogsmodel/cv/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3929 2023-04-13 14:26:53.000000 cogsgpt-0.0.2/cogsgpt/cogsmodel/cv/image_analysis.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2061 2023-04-13 14:42:27.000000 cogsgpt-0.0.2/cogsgpt/cogsmodel/cv/ocr.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 12:26:36.595819 cogsgpt-0.0.2/cogsgpt/cogsmodel/nlp/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      427 2023-04-14 03:16:26.000000 cogsgpt-0.0.2/cogsgpt/cogsmodel/nlp/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3188 2023-04-13 15:01:36.000000 cogsgpt-0.0.2/cogsgpt/cogsmodel/nlp/text_analysis.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1684 2023-04-20 12:10:44.000000 cogsgpt-0.0.2/cogsgpt/cogsmodel/nlp/text_generation.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2150 2023-04-13 15:05:49.000000 cogsgpt-0.0.2/cogsgpt/cogsmodel/nlp/text_summarize.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1676 2023-04-13 15:11:04.000000 cogsgpt-0.0.2/cogsgpt/cogsmodel/nlp/text_translation.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 12:26:36.599819 cogsgpt-0.0.2/cogsgpt/cogsmodel/speech/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       73 2023-04-12 13:18:32.000000 cogsgpt-0.0.2/cogsgpt/cogsmodel/speech/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3795 2023-04-13 14:49:00.000000 cogsgpt-0.0.2/cogsgpt/cogsmodel/speech/speech.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1339 2023-04-20 11:56:11.000000 cogsgpt-0.0.2/cogsgpt/llm.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 12:26:36.603819 cogsgpt-0.0.2/cogsgpt/metas/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      316 2023-04-12 04:35:32.000000 cogsgpt-0.0.2/cogsgpt/metas/generate_response_presteps.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2750 2023-04-20 08:45:10.000000 cogsgpt-0.0.2/cogsgpt/metas/parse_task_examples.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     7470 2023-04-20 08:45:10.000000 cogsgpt-0.0.2/cogsgpt/metas/task_metas.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1074 2023-04-20 11:56:04.000000 cogsgpt-0.0.2/cogsgpt/utils.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      917 2023-04-20 12:25:02.000000 cogsgpt-0.0.2/pyproject.toml
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-20 12:26:36.611819 cogsgpt-0.0.2/setup.cfg
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 12:26:36.607819 cogsgpt-0.0.2/tests/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      251 2023-04-14 13:22:18.000000 cogsgpt-0.0.2/tests/test_awesome_chat.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      360 2023-04-15 07:30:49.000000 cogsgpt-0.0.2/tests/test_image_analisys.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      347 2023-04-15 07:30:38.000000 cogsgpt-0.0.2/tests/test_ocr.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      601 2023-04-13 14:19:29.000000 cogsgpt-0.0.2/tests/test_speech.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1441 2023-04-13 14:19:32.000000 cogsgpt-0.0.2/tests/test_text_analysis.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      576 2023-04-14 03:20:51.000000 cogsgpt-0.0.2/tests/test_text_generation.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1970 2023-04-13 14:19:36.000000 cogsgpt-0.0.2/tests/test_text_summarize.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1168 2023-04-14 03:20:35.000000 cogsgpt-0.0.2/tests/test_text_translation.py
```

### Comparing `cogsgpt-0.0.1/LICENSE` & `cogsgpt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.1/PKG-INFO` & `cogsgpt-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogsgpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: A multi-modal LLM integrated ChatGPT with Azure Cognitive Service
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,24 +61,21 @@
 
 First, you need to register an [OpenAI](https://platform.openai.com/) account or deploy an [Azure OpenAI Service](https://azure.microsoft.com/en-us/products/cognitive-services/openai-service). Follow the official documents to obtain the API key and other resources. 
 
 If you want to use OpenAI API, you need to set these environment variables:
 ```bash
 export OPENAI_API_TYPE="openai"
 export OPENAI_API_KEY="<OpenAI API Key>"
-export OPENAI_MODEL_NAME="<OpenAI Model Name>"
 ```
 
 If you want to use Azure OpenAI Service, you need to set these environment variables:
 ```bash
 export OPENAI_API_TYPE="azure"
 export OPENAI_API_BASE="<Azure OpenAI Service Endpoint>"
 export OPENAI_API_KEY="<Azure OpenAI Service Key>"
-export OPENAI_MODEL_NAME="<Deployment Name>"
-export OPENAI_MODEL_VERSION="<Model Version>"
 ```
 
 #### Azure Cognitive Service Requirements
 
 Next, you need also to deploy an [Azure Cognitive Service](https://azure.microsoft.com/en-us/products/cognitive-services/). Follow the official documents to obtain the deployment key and other resources, and set these environment variables:
 ```bash
 export COGS_ENDPOINT="<Azure Cognitive Service Endpoint>"
@@ -95,28 +92,40 @@
 You can now install CogsGPT with pip:
 ```bash
 pip install cogsgpt
 ```
 
 ### Usage
 
-You can use CogsGPT in your own application to process image or audio inputs within 3 lines of codes:
+You can use CogsGPT in your own application to process image or audio inputs within several lines of codes:
 ```python
 from cogsgpt import CogsGPT
 
-agent = CogsGPT()
+if os.environ["OPENAI_API_TYPE"] == "openai":
+    agent = CogsGPT(model_name="gpt-3.5-turbo")
+elif os.environ["OPENAI_API_TYPE"] == "azure":
+    agent = CogsGPT(deployment_name="<YOUR DEPLOYMENT NAME>", openai_api_version="<YOUR DEPLOYMENT VERSION>")
+
 agent.chat("What's the content in a.jpg?")
 ```
 
 Or you can experience an interactive console application with the following command:
 ```bash
 python ./tests/test_awesome_chat.py
 ```
 
-Enjoy your chat!
+### Gradio App
+
+The Gradio demo is now hosted on [Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT). You can also run the following commands to start the demo locally:
+```bash
+pip install gradio
+python app.py
+```
+
+Now open your favorite browser and ENJOY THE CHAT!
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
 
 ## Contributing
```

### Comparing `cogsgpt-0.0.1/README.md` & `cogsgpt-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -25,24 +25,21 @@
 
 First, you need to register an [OpenAI](https://platform.openai.com/) account or deploy an [Azure OpenAI Service](https://azure.microsoft.com/en-us/products/cognitive-services/openai-service). Follow the official documents to obtain the API key and other resources. 
 
 If you want to use OpenAI API, you need to set these environment variables:
 ```bash
 export OPENAI_API_TYPE="openai"
 export OPENAI_API_KEY="<OpenAI API Key>"
-export OPENAI_MODEL_NAME="<OpenAI Model Name>"
 ```
 
 If you want to use Azure OpenAI Service, you need to set these environment variables:
 ```bash
 export OPENAI_API_TYPE="azure"
 export OPENAI_API_BASE="<Azure OpenAI Service Endpoint>"
 export OPENAI_API_KEY="<Azure OpenAI Service Key>"
-export OPENAI_MODEL_NAME="<Deployment Name>"
-export OPENAI_MODEL_VERSION="<Model Version>"
 ```
 
 #### Azure Cognitive Service Requirements
 
 Next, you need also to deploy an [Azure Cognitive Service](https://azure.microsoft.com/en-us/products/cognitive-services/). Follow the official documents to obtain the deployment key and other resources, and set these environment variables:
 ```bash
 export COGS_ENDPOINT="<Azure Cognitive Service Endpoint>"
@@ -59,28 +56,40 @@
 You can now install CogsGPT with pip:
 ```bash
 pip install cogsgpt
 ```
 
 ### Usage
 
-You can use CogsGPT in your own application to process image or audio inputs within 3 lines of codes:
+You can use CogsGPT in your own application to process image or audio inputs within several lines of codes:
 ```python
 from cogsgpt import CogsGPT
 
-agent = CogsGPT()
+if os.environ["OPENAI_API_TYPE"] == "openai":
+    agent = CogsGPT(model_name="gpt-3.5-turbo")
+elif os.environ["OPENAI_API_TYPE"] == "azure":
+    agent = CogsGPT(deployment_name="<YOUR DEPLOYMENT NAME>", openai_api_version="<YOUR DEPLOYMENT VERSION>")
+
 agent.chat("What's the content in a.jpg?")
 ```
 
 Or you can experience an interactive console application with the following command:
 ```bash
 python ./tests/test_awesome_chat.py
 ```
 
-Enjoy your chat!
+### Gradio App
+
+The Gradio demo is now hosted on [Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT). You can also run the following commands to start the demo locally:
+```bash
+pip install gradio
+python app.py
+```
+
+Now open your favorite browser and ENJOY THE CHAT!
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
 
 ## Contributing
```

### Comparing `cogsgpt-0.0.1/cogsgpt/awesome_chat.py` & `cogsgpt-0.0.2/cogsgpt/awesome_chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import json
+import os
 from typing import Dict, List
 import colorlog
 import pkg_resources
 
 from langchain import PromptTemplate
 from langchain.prompts.chat import (
     ChatPromptTemplate,
     SystemMessagePromptTemplate,
     AIMessagePromptTemplate,
     HumanMessagePromptTemplate,
 )
 from langchain.schema import BaseMessage
 from langchain.memory import ConversationBufferMemory
 
-from cogsgpt import awesome_prompts, ArgsType, LanguageType, llm_manager
+from cogsgpt import awesome_prompts, ArgsType, LanguageType, LLMManager
 from cogsgpt.cogsmodel import *
 
 
 handler = colorlog.StreamHandler()
 handler.setFormatter(colorlog.ColoredFormatter(
 	"%(log_color)s%(levelname)-8s %(message)s",
 	datefmt=None,
@@ -52,25 +53,48 @@
     "personally-identifiable-information": PIIModel,
     "text-translation": TextTranslationModel,
     "text-generation": TextGenerationModel,
 }
 
 
 class CogsGPT():
-    def __init__(self) -> None:
+    # Optional Env Vars
+    OPENAI_MODEL_NAME = os.environ.get("OPENAI_MODEL_NAME", "")
+    OPENAI_MODEL_VERSION = os.environ.get("OPENAI_MODEL_VERSION", "")
+
+    def __init__(self,
+                 model_name: str = OPENAI_MODEL_NAME,
+                 deployment_name: str = OPENAI_MODEL_NAME,
+                 deployment_version: str = OPENAI_MODEL_VERSION,
+                 temperature: float = 0.7,
+                 request_timeout: int = 60,
+                 max_retries: int = 6,
+                 max_tokens: int | None = None,
+                 verbose: bool = False,
+                 ) -> None:
         self.task_metas = json.load(open(pkg_resources.resource_filename('cogsgpt', 'metas/task_metas.json'), "r"))
         self.parse_task_examples = json.load(open(pkg_resources.resource_filename('cogsgpt', 'metas/parse_task_examples.json'), 'r'))
         self.generate_response_presteps = json.load(open(pkg_resources.resource_filename('cogsgpt', 'metas/generate_response_presteps.json'), 'r'))
 
         self.parse_task_prompt = self._create_parse_task_prompt()
         self.generate_response_prompt = self._create_generate_response_prompt()
 
         self.memory = ConversationBufferMemory(memory_key='history')
 
-        self.chat_model = llm_manager.LLM
+        # NOTE: LLMManager is a singleton class. It will be instantiated here.
+        self.chat_model = LLMManager(
+            model_name=model_name,
+            deployment_name=deployment_name,
+            deployment_version=deployment_version,
+            temperature=temperature,
+            request_timeout=request_timeout,
+            max_retries=max_retries,
+            max_tokens=max_tokens,
+            verbose=verbose,
+        ).LLM
 
     def _save_context(self, human_input: str, ai_response: str) -> None:
         self.memory.chat_memory.add_user_message(human_input)
         self.memory.chat_memory.add_ai_message(ai_response)
 
     def _load_context(self) -> str:
         return self.memory.load_memory_variables({})['history']
```

### Comparing `cogsgpt-0.0.1/cogsgpt/awesome_prompts.py` & `cogsgpt-0.0.2/cogsgpt/awesome_prompts.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.1/cogsgpt/cogsmodel/cv/image_analysis.py` & `cogsgpt-0.0.2/cogsgpt/cogsmodel/cv/image_analysis.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.1/cogsgpt/cogsmodel/cv/ocr.py` & `cogsgpt-0.0.2/cogsgpt/cogsmodel/cv/ocr.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.1/cogsgpt/cogsmodel/nlp/text_analysis.py` & `cogsgpt-0.0.2/cogsgpt/cogsmodel/nlp/text_analysis.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.1/cogsgpt/cogsmodel/nlp/text_generation.py` & `cogsgpt-0.0.2/cogsgpt/cogsmodel/nlp/text_generation.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 from langchain import PromptTemplate
 from langchain.prompts.chat import (
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
 )
 from langchain.schema import BaseMessage
 
-from cogsgpt import llm_manager
+from cogsgpt import LLMManager
 from cogsgpt.cogsmodel import BaseModel
 
 
 class TextGenerationModel(BaseModel):
     def __init__(self) -> None:
         super().__init__()
         self._task_name = "text-generation"
 
-        self._llm = llm_manager.LLM
+        # NOTE: LLMManger is a singleton class. It should have been instantiated in the main process.
+        self._llm = LLMManager().LLM
         self._prompt = self._create_prompt()
 
     def _create_prompt(self) -> ChatPromptTemplate:
         human_message_prompt = HumanMessagePromptTemplate(
             prompt=PromptTemplate(
                 template="The user request [ {{human_input}} ] contains a {{ task_name }} task. Now you are a {{ task_name }} system, the arguments are {{ task_args }}. Just help me do {{ task_name }} and give me the result. The result should focus more on the {{ task_name}} task, no additional notes, and must be in text form without any urls.",
                 input_variables=["human_input", "task_name", "task_args"],
```

### Comparing `cogsgpt-0.0.1/cogsgpt/cogsmodel/nlp/text_summarize.py` & `cogsgpt-0.0.2/cogsgpt/cogsmodel/nlp/text_summarize.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.1/cogsgpt/cogsmodel/nlp/text_translation.py` & `cogsgpt-0.0.2/cogsgpt/cogsmodel/nlp/text_translation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.1/cogsgpt/cogsmodel/speech/speech.py` & `cogsgpt-0.0.2/cogsgpt/cogsmodel/speech/speech.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.1/cogsgpt/metas/parse_task_examples.json` & `cogsgpt-0.0.2/cogsgpt/metas/parse_task_examples.json`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.1/cogsgpt/metas/task_metas.json` & `cogsgpt-0.0.2/cogsgpt/metas/task_metas.json`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.1/cogsgpt/utils.py` & `cogsgpt-0.0.2/cogsgpt/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,28 @@
 
 
 class FileSource(Enum):
     LOCAL = "local"
     REMOTE = "remote"
 
 
+def singleton(cls):
+    """
+    decorator to make a class a singleton
+    """
+    instances = {}
+
+    def getinstance(*args, **kwargs):
+        if cls not in instances:
+            instances[cls] = cls(*args, **kwargs)
+        return instances[cls]
+
+    return getinstance
+
+
 def detect_file_source(file_path: str) -> Optional[str]:
     # Check if the input is a local file path
     if os.path.isfile(file_path):
         return FileSource.LOCAL
 
     # Check if the input is a web URL
     parsed_url = urlparse(file_path)
```

### Comparing `cogsgpt-0.0.1/cogsgpt.egg-info/PKG-INFO` & `cogsgpt-0.0.2/cogsgpt/cogsgpt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogsgpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: A multi-modal LLM integrated ChatGPT with Azure Cognitive Service
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,24 +61,21 @@
 
 First, you need to register an [OpenAI](https://platform.openai.com/) account or deploy an [Azure OpenAI Service](https://azure.microsoft.com/en-us/products/cognitive-services/openai-service). Follow the official documents to obtain the API key and other resources. 
 
 If you want to use OpenAI API, you need to set these environment variables:
 ```bash
 export OPENAI_API_TYPE="openai"
 export OPENAI_API_KEY="<OpenAI API Key>"
-export OPENAI_MODEL_NAME="<OpenAI Model Name>"
 ```
 
 If you want to use Azure OpenAI Service, you need to set these environment variables:
 ```bash
 export OPENAI_API_TYPE="azure"
 export OPENAI_API_BASE="<Azure OpenAI Service Endpoint>"
 export OPENAI_API_KEY="<Azure OpenAI Service Key>"
-export OPENAI_MODEL_NAME="<Deployment Name>"
-export OPENAI_MODEL_VERSION="<Model Version>"
 ```
 
 #### Azure Cognitive Service Requirements
 
 Next, you need also to deploy an [Azure Cognitive Service](https://azure.microsoft.com/en-us/products/cognitive-services/). Follow the official documents to obtain the deployment key and other resources, and set these environment variables:
 ```bash
 export COGS_ENDPOINT="<Azure Cognitive Service Endpoint>"
@@ -95,28 +92,40 @@
 You can now install CogsGPT with pip:
 ```bash
 pip install cogsgpt
 ```
 
 ### Usage
 
-You can use CogsGPT in your own application to process image or audio inputs within 3 lines of codes:
+You can use CogsGPT in your own application to process image or audio inputs within several lines of codes:
 ```python
 from cogsgpt import CogsGPT
 
-agent = CogsGPT()
+if os.environ["OPENAI_API_TYPE"] == "openai":
+    agent = CogsGPT(model_name="gpt-3.5-turbo")
+elif os.environ["OPENAI_API_TYPE"] == "azure":
+    agent = CogsGPT(deployment_name="<YOUR DEPLOYMENT NAME>", openai_api_version="<YOUR DEPLOYMENT VERSION>")
+
 agent.chat("What's the content in a.jpg?")
 ```
 
 Or you can experience an interactive console application with the following command:
 ```bash
 python ./tests/test_awesome_chat.py
 ```
 
-Enjoy your chat!
+### Gradio App
+
+The Gradio demo is now hosted on [Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT). You can also run the following commands to start the demo locally:
+```bash
+pip install gradio
+python app.py
+```
+
+Now open your favorite browser and ENJOY THE CHAT!
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
 
 ## Contributing
```

### Comparing `cogsgpt-0.0.1/cogsgpt.egg-info/SOURCES.txt` & `cogsgpt-0.0.2/cogsgpt/cogsgpt.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 README.md
 pyproject.toml
 cogsgpt/__init__.py
 cogsgpt/awesome_chat.py
 cogsgpt/awesome_prompts.py
 cogsgpt/llm.py
 cogsgpt/utils.py
-cogsgpt.egg-info/PKG-INFO
-cogsgpt.egg-info/SOURCES.txt
-cogsgpt.egg-info/dependency_links.txt
-cogsgpt.egg-info/requires.txt
-cogsgpt.egg-info/top_level.txt
+cogsgpt/cogsgpt.egg-info/PKG-INFO
+cogsgpt/cogsgpt.egg-info/SOURCES.txt
+cogsgpt/cogsgpt.egg-info/dependency_links.txt
+cogsgpt/cogsgpt.egg-info/requires.txt
+cogsgpt/cogsgpt.egg-info/top_level.txt
 cogsgpt/cogsmodel/__init__.py
 cogsgpt/cogsmodel/base_model.py
 cogsgpt/cogsmodel/cv/__init__.py
 cogsgpt/cogsmodel/cv/image_analysis.py
 cogsgpt/cogsmodel/cv/ocr.py
 cogsgpt/cogsmodel/nlp/__init__.py
 cogsgpt/cogsmodel/nlp/text_analysis.py
```

### Comparing `cogsgpt-0.0.1/pyproject.toml` & `cogsgpt-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cogsgpt"
-version = "0.0.1"
+version = "0.0.2"
 description = "A multi-modal LLM integrated ChatGPT with Azure Cognitive Service"
 readme = "README.md"
 authors = [{ name = "weitian", email = "weitian.bnu@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -26,8 +26,11 @@
     "openai",
     "jinja2",
     "colorlog",
 ]
 requires-python = ">=3.8"
 
 [project.urls]
-Homepage = "https://github.com/whiskyboy/cogsgpt"
+Homepage = "https://github.com/whiskyboy/cogsgpt"
+
+[tool.setuptools]
+package-dir = {"" = "cogsgpt"}
```

### Comparing `cogsgpt-0.0.1/tests/test_speech.py` & `cogsgpt-0.0.2/tests/test_speech.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.1/tests/test_text_analysis.py` & `cogsgpt-0.0.2/tests/test_text_analysis.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.1/tests/test_text_generation.py` & `cogsgpt-0.0.2/tests/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.1/tests/test_text_summarize.py` & `cogsgpt-0.0.2/tests/test_text_summarize.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.1/tests/test_text_translation.py` & `cogsgpt-0.0.2/tests/test_text_translation.py`

 * *Files identical despite different names*

