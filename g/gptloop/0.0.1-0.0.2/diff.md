# Comparing `tmp/gptloop-0.0.1.tar.gz` & `tmp/gptloop-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptloop-0.0.1.tar", last modified: Thu Apr 20 06:18:36 2023, max compression
+gzip compressed data, was "gptloop-0.0.2.tar", last modified: Thu Apr 20 07:01:13 2023, max compression
```

## Comparing `gptloop-0.0.1.tar` & `gptloop-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 itecgo     (501) staff       (20)        0 2023-04-20 06:18:36.575538 gptloop-0.0.1/
--rw-r--r--   0 itecgo     (501) staff       (20)     1067 2023-04-20 05:20:57.000000 gptloop-0.0.1/LICENSE
--rw-r--r--   0 itecgo     (501) staff       (20)     3771 2023-04-20 06:18:36.575352 gptloop-0.0.1/PKG-INFO
--rw-r--r--   0 itecgo     (501) staff       (20)     2798 2023-04-20 05:17:52.000000 gptloop-0.0.1/README.md
-drwxr-xr-x   0 itecgo     (501) staff       (20)        0 2023-04-20 06:18:36.573552 gptloop-0.0.1/gptloop/
--rw-r--r--   0 itecgo     (501) staff       (20)        0 2023-04-20 05:49:12.000000 gptloop-0.0.1/gptloop/__init__.py
--rw-r--r--   0 itecgo     (501) staff       (20)      930 2023-04-20 06:15:56.000000 gptloop-0.0.1/gptloop/cli.py
-drwxr-xr-x   0 itecgo     (501) staff       (20)        0 2023-04-20 06:18:36.574949 gptloop-0.0.1/gptloop.egg-info/
--rw-r--r--   0 itecgo     (501) staff       (20)     3771 2023-04-20 06:18:36.000000 gptloop-0.0.1/gptloop.egg-info/PKG-INFO
--rw-r--r--   0 itecgo     (501) staff       (20)      249 2023-04-20 06:18:36.000000 gptloop-0.0.1/gptloop.egg-info/SOURCES.txt
--rw-r--r--   0 itecgo     (501) staff       (20)        1 2023-04-20 06:18:36.000000 gptloop-0.0.1/gptloop.egg-info/dependency_links.txt
--rw-r--r--   0 itecgo     (501) staff       (20)       45 2023-04-20 06:18:36.000000 gptloop-0.0.1/gptloop.egg-info/entry_points.txt
--rw-r--r--   0 itecgo     (501) staff       (20)       55 2023-04-20 06:18:36.000000 gptloop-0.0.1/gptloop.egg-info/requires.txt
--rw-r--r--   0 itecgo     (501) staff       (20)        8 2023-04-20 06:18:36.000000 gptloop-0.0.1/gptloop.egg-info/top_level.txt
--rw-r--r--   0 itecgo     (501) staff       (20)       38 2023-04-20 06:18:36.575584 gptloop-0.0.1/setup.cfg
--rw-r--r--   0 itecgo     (501) staff       (20)     1354 2023-04-20 05:54:12.000000 gptloop-0.0.1/setup.py
+drwxr-xr-x   0 itecgo     (501) staff       (20)        0 2023-04-20 07:01:13.517239 gptloop-0.0.2/
+-rw-r--r--   0 itecgo     (501) staff       (20)     1067 2023-04-20 05:20:57.000000 gptloop-0.0.2/LICENSE
+-rw-r--r--   0 itecgo     (501) staff       (20)     3771 2023-04-20 07:01:13.517043 gptloop-0.0.2/PKG-INFO
+-rw-r--r--   0 itecgo     (501) staff       (20)     2798 2023-04-20 05:17:52.000000 gptloop-0.0.2/README.md
+drwxr-xr-x   0 itecgo     (501) staff       (20)        0 2023-04-20 07:01:13.515489 gptloop-0.0.2/gptloop/
+-rw-r--r--   0 itecgo     (501) staff       (20)        0 2023-04-20 05:49:12.000000 gptloop-0.0.2/gptloop/__init__.py
+-rw-r--r--   0 itecgo     (501) staff       (20)      857 2023-04-20 07:00:28.000000 gptloop-0.0.2/gptloop/cli.py
+drwxr-xr-x   0 itecgo     (501) staff       (20)        0 2023-04-20 07:01:13.516750 gptloop-0.0.2/gptloop.egg-info/
+-rw-r--r--   0 itecgo     (501) staff       (20)     3771 2023-04-20 07:01:13.000000 gptloop-0.0.2/gptloop.egg-info/PKG-INFO
+-rw-r--r--   0 itecgo     (501) staff       (20)      249 2023-04-20 07:01:13.000000 gptloop-0.0.2/gptloop.egg-info/SOURCES.txt
+-rw-r--r--   0 itecgo     (501) staff       (20)        1 2023-04-20 07:01:13.000000 gptloop-0.0.2/gptloop.egg-info/dependency_links.txt
+-rw-r--r--   0 itecgo     (501) staff       (20)       45 2023-04-20 07:01:13.000000 gptloop-0.0.2/gptloop.egg-info/entry_points.txt
+-rw-r--r--   0 itecgo     (501) staff       (20)       34 2023-04-20 07:01:13.000000 gptloop-0.0.2/gptloop.egg-info/requires.txt
+-rw-r--r--   0 itecgo     (501) staff       (20)        8 2023-04-20 07:01:13.000000 gptloop-0.0.2/gptloop.egg-info/top_level.txt
+-rw-r--r--   0 itecgo     (501) staff       (20)       38 2023-04-20 07:01:13.517283 gptloop-0.0.2/setup.cfg
+-rw-r--r--   0 itecgo     (501) staff       (20)     1354 2023-04-20 07:00:44.000000 gptloop-0.0.2/setup.py
```

### Comparing `gptloop-0.0.1/LICENSE` & `gptloop-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gptloop-0.0.1/PKG-INFO` & `gptloop-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptloop
-Version: 0.0.1
+Version: 0.0.2
 Summary: GPTLoop is a versatile AI-powered assistant to enhance work quality and efficiency
 Home-page: https://github.com/mcai/GPTLoop
 Author: Min Cai
 Author-email: min.cai.china@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gptloop-0.0.1/README.md` & `gptloop-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gptloop-0.0.1/gptloop/cli.py` & `gptloop-0.0.2/gptloop/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import argparse
 import os
-from dotenv import load_dotenv
 import openai
 
 def get_llm_response(prompt, api_key):
     openai.api_key = api_key
 
     response = openai.Completion.create(
         engine="text-davinci-002",
@@ -19,21 +18,18 @@
 
 def main():
     parser = argparse.ArgumentParser(description="Get a response from an LLM for a given prompt.")
     parser.add_argument("prompt", help="text prompt for the LLM")
 
     args = parser.parse_args()
 
-    # Load the .env file
-    load_dotenv()
-
     # Get API key from environment variable
     api_key = os.getenv("OPENAI_API_KEY")
     if not api_key:
-        print("Error: OPENAI_API_KEY is not set in the .env file.")
+        print("Error: OPENAI_API_KEY is not set in the environment.")
         return
 
     response = get_llm_response(args.prompt, api_key)
     print(response)
 
 if __name__ == "__main__":
     main()
```

### Comparing `gptloop-0.0.1/gptloop.egg-info/PKG-INFO` & `gptloop-0.0.2/gptloop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptloop
-Version: 0.0.1
+Version: 0.0.2
 Summary: GPTLoop is a versatile AI-powered assistant to enhance work quality and efficiency
 Home-page: https://github.com/mcai/GPTLoop
 Author: Min Cai
 Author-email: min.cai.china@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gptloop-0.0.1/setup.py` & `gptloop-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="gptloop",
-    version="0.0.1",
+    version="0.0.2",
     author="Min Cai",
     author_email="min.cai.china@gmail.com",
     description="GPTLoop is a versatile AI-powered assistant to enhance work quality and efficiency",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/mcai/GPTLoop",
     packages=find_packages(),
```

