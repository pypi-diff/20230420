# Comparing `tmp/gptloop-0.0.2.tar.gz` & `tmp/gptloop-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptloop-0.0.2.tar", last modified: Thu Apr 20 07:01:13 2023, max compression
+gzip compressed data, was "gptloop-0.0.3.tar", last modified: Thu Apr 20 07:40:52 2023, max compression
```

## Comparing `gptloop-0.0.2.tar` & `gptloop-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 itecgo     (501) staff       (20)        0 2023-04-20 07:01:13.517239 gptloop-0.0.2/
--rw-r--r--   0 itecgo     (501) staff       (20)     1067 2023-04-20 05:20:57.000000 gptloop-0.0.2/LICENSE
--rw-r--r--   0 itecgo     (501) staff       (20)     3771 2023-04-20 07:01:13.517043 gptloop-0.0.2/PKG-INFO
--rw-r--r--   0 itecgo     (501) staff       (20)     2798 2023-04-20 05:17:52.000000 gptloop-0.0.2/README.md
-drwxr-xr-x   0 itecgo     (501) staff       (20)        0 2023-04-20 07:01:13.515489 gptloop-0.0.2/gptloop/
--rw-r--r--   0 itecgo     (501) staff       (20)        0 2023-04-20 05:49:12.000000 gptloop-0.0.2/gptloop/__init__.py
--rw-r--r--   0 itecgo     (501) staff       (20)      857 2023-04-20 07:00:28.000000 gptloop-0.0.2/gptloop/cli.py
-drwxr-xr-x   0 itecgo     (501) staff       (20)        0 2023-04-20 07:01:13.516750 gptloop-0.0.2/gptloop.egg-info/
--rw-r--r--   0 itecgo     (501) staff       (20)     3771 2023-04-20 07:01:13.000000 gptloop-0.0.2/gptloop.egg-info/PKG-INFO
--rw-r--r--   0 itecgo     (501) staff       (20)      249 2023-04-20 07:01:13.000000 gptloop-0.0.2/gptloop.egg-info/SOURCES.txt
--rw-r--r--   0 itecgo     (501) staff       (20)        1 2023-04-20 07:01:13.000000 gptloop-0.0.2/gptloop.egg-info/dependency_links.txt
--rw-r--r--   0 itecgo     (501) staff       (20)       45 2023-04-20 07:01:13.000000 gptloop-0.0.2/gptloop.egg-info/entry_points.txt
--rw-r--r--   0 itecgo     (501) staff       (20)       34 2023-04-20 07:01:13.000000 gptloop-0.0.2/gptloop.egg-info/requires.txt
--rw-r--r--   0 itecgo     (501) staff       (20)        8 2023-04-20 07:01:13.000000 gptloop-0.0.2/gptloop.egg-info/top_level.txt
--rw-r--r--   0 itecgo     (501) staff       (20)       38 2023-04-20 07:01:13.517283 gptloop-0.0.2/setup.cfg
--rw-r--r--   0 itecgo     (501) staff       (20)     1354 2023-04-20 07:00:44.000000 gptloop-0.0.2/setup.py
+drwxr-xr-x   0 itecgo     (501) staff       (20)        0 2023-04-20 07:40:52.321396 gptloop-0.0.3/
+-rw-r--r--   0 itecgo     (501) staff       (20)     1067 2023-04-20 05:20:57.000000 gptloop-0.0.3/LICENSE
+-rw-r--r--   0 itecgo     (501) staff       (20)     3847 2023-04-20 07:40:52.321122 gptloop-0.0.3/PKG-INFO
+-rw-r--r--   0 itecgo     (501) staff       (20)     2874 2023-04-20 07:26:33.000000 gptloop-0.0.3/README.md
+drwxr-xr-x   0 itecgo     (501) staff       (20)        0 2023-04-20 07:40:52.318997 gptloop-0.0.3/gptloop/
+-rw-r--r--   0 itecgo     (501) staff       (20)        0 2023-04-20 05:49:12.000000 gptloop-0.0.3/gptloop/__init__.py
+-rw-r--r--   0 itecgo     (501) staff       (20)      878 2023-04-20 07:38:53.000000 gptloop-0.0.3/gptloop/cli.py
+drwxr-xr-x   0 itecgo     (501) staff       (20)        0 2023-04-20 07:40:52.320706 gptloop-0.0.3/gptloop.egg-info/
+-rw-r--r--   0 itecgo     (501) staff       (20)     3847 2023-04-20 07:40:52.000000 gptloop-0.0.3/gptloop.egg-info/PKG-INFO
+-rw-r--r--   0 itecgo     (501) staff       (20)      249 2023-04-20 07:40:52.000000 gptloop-0.0.3/gptloop.egg-info/SOURCES.txt
+-rw-r--r--   0 itecgo     (501) staff       (20)        1 2023-04-20 07:40:52.000000 gptloop-0.0.3/gptloop.egg-info/dependency_links.txt
+-rw-r--r--   0 itecgo     (501) staff       (20)       45 2023-04-20 07:40:52.000000 gptloop-0.0.3/gptloop.egg-info/entry_points.txt
+-rw-r--r--   0 itecgo     (501) staff       (20)       34 2023-04-20 07:40:52.000000 gptloop-0.0.3/gptloop.egg-info/requires.txt
+-rw-r--r--   0 itecgo     (501) staff       (20)        8 2023-04-20 07:40:52.000000 gptloop-0.0.3/gptloop.egg-info/top_level.txt
+-rw-r--r--   0 itecgo     (501) staff       (20)       38 2023-04-20 07:40:52.321471 gptloop-0.0.3/setup.cfg
+-rw-r--r--   0 itecgo     (501) staff       (20)     1354 2023-04-20 07:40:07.000000 gptloop-0.0.3/setup.py
```

### Comparing `gptloop-0.0.2/LICENSE` & `gptloop-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gptloop-0.0.2/PKG-INFO` & `gptloop-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptloop
-Version: 0.0.2
+Version: 0.0.3
 Summary: GPTLoop is a versatile AI-powered assistant to enhance work quality and efficiency
 Home-page: https://github.com/mcai/GPTLoop
 Author: Min Cai
 Author-email: min.cai.china@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -33,22 +33,23 @@
 -   **Multilingual Support**: GPTLoop works with various languages, thanks to the language capabilities of large language models, making it suitable for users from diverse linguistic backgrounds.
 
 ## Installation
 
 To install GPTLoop using pip, open your terminal or command prompt and run:
 
 ```bash
-pip install gptloop
+pip install --upgrade gptloop
 ```
 
 ## Usage
 
 Once GPTLoop is installed, you can run it from the command line:
 
 ```bash
+export OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 gptloop
 ```
 
 Follow the on-screen prompts to provide initial input and any subsequent feedback for refining the AI's output.
 
 ## Considerations
```

### Comparing `gptloop-0.0.2/README.md` & `gptloop-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 -   **Multilingual Support**: GPTLoop works with various languages, thanks to the language capabilities of large language models, making it suitable for users from diverse linguistic backgrounds.
 
 ## Installation
 
 To install GPTLoop using pip, open your terminal or command prompt and run:
 
 ```bash
-pip install gptloop
+pip install --upgrade gptloop
 ```
 
 ## Usage
 
 Once GPTLoop is installed, you can run it from the command line:
 
 ```bash
+export OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 gptloop
 ```
 
 Follow the on-screen prompts to provide initial input and any subsequent feedback for refining the AI's output.
 
 ## Considerations
```

### Comparing `gptloop-0.0.2/gptloop.egg-info/PKG-INFO` & `gptloop-0.0.3/gptloop.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptloop
-Version: 0.0.2
+Version: 0.0.3
 Summary: GPTLoop is a versatile AI-powered assistant to enhance work quality and efficiency
 Home-page: https://github.com/mcai/GPTLoop
 Author: Min Cai
 Author-email: min.cai.china@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -33,22 +33,23 @@
 -   **Multilingual Support**: GPTLoop works with various languages, thanks to the language capabilities of large language models, making it suitable for users from diverse linguistic backgrounds.
 
 ## Installation
 
 To install GPTLoop using pip, open your terminal or command prompt and run:
 
 ```bash
-pip install gptloop
+pip install --upgrade gptloop
 ```
 
 ## Usage
 
 Once GPTLoop is installed, you can run it from the command line:
 
 ```bash
+export OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 gptloop
 ```
 
 Follow the on-screen prompts to provide initial input and any subsequent feedback for refining the AI's output.
 
 ## Considerations
```

### Comparing `gptloop-0.0.2/setup.py` & `gptloop-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="gptloop",
-    version="0.0.2",
+    version="0.0.3",
     author="Min Cai",
     author_email="min.cai.china@gmail.com",
     description="GPTLoop is a versatile AI-powered assistant to enhance work quality and efficiency",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/mcai/GPTLoop",
     packages=find_packages(),
```

