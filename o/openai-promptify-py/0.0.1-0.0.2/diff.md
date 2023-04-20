# Comparing `tmp/openai-promptify-py-0.0.1.tar.gz` & `tmp/openai-promptify-py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-promptify-py-0.0.1.tar", last modified: Thu Apr 20 02:56:15 2023, max compression
+gzip compressed data, was "openai-promptify-py-0.0.2.tar", last modified: Thu Apr 20 03:13:00 2023, max compression
```

## Comparing `openai-promptify-py-0.0.1.tar` & `openai-promptify-py-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-04-20 02:56:15.663231 openai-promptify-py-0.0.1/
--rw-r--r--   0 maverick   (501) staff       (20)     1878 2023-04-20 02:56:15.663058 openai-promptify-py-0.0.1/PKG-INFO
--rw-r--r--   0 maverick   (501) staff       (20)     1512 2023-03-22 09:05:12.000000 openai-promptify-py-0.0.1/README.md
--rw-r--r--   0 maverick   (501) staff       (20)      620 2023-03-22 11:45:26.000000 openai-promptify-py-0.0.1/pyproject.toml
--rw-r--r--   0 maverick   (501) staff       (20)        7 2023-03-21 07:28:20.000000 openai-promptify-py-0.0.1/requirements.txt
--rw-r--r--   0 maverick   (501) staff       (20)       38 2023-04-20 02:56:15.663281 openai-promptify-py-0.0.1/setup.cfg
-drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-04-20 02:56:15.661435 openai-promptify-py-0.0.1/src/
--rw-r--r--   0 maverick   (501) staff       (20)     7527 2023-04-20 01:42:08.000000 openai-promptify-py-0.0.1/src/openai_promptify.py
-drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-04-20 02:56:15.662348 openai-promptify-py-0.0.1/src/openai_promptify_py.egg-info/
--rw-r--r--   0 maverick   (501) staff       (20)     1878 2023-04-20 02:56:15.000000 openai-promptify-py-0.0.1/src/openai_promptify_py.egg-info/PKG-INFO
--rw-r--r--   0 maverick   (501) staff       (20)      347 2023-04-20 02:56:15.000000 openai-promptify-py-0.0.1/src/openai_promptify_py.egg-info/SOURCES.txt
--rw-r--r--   0 maverick   (501) staff       (20)        1 2023-04-20 02:56:15.000000 openai-promptify-py-0.0.1/src/openai_promptify_py.egg-info/dependency_links.txt
--rw-r--r--   0 maverick   (501) staff       (20)        7 2023-04-20 02:56:15.000000 openai-promptify-py-0.0.1/src/openai_promptify_py.egg-info/requires.txt
--rw-r--r--   0 maverick   (501) staff       (20)       17 2023-04-20 02:56:15.000000 openai-promptify-py-0.0.1/src/openai_promptify_py.egg-info/top_level.txt
-drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-04-20 02:56:15.662740 openai-promptify-py-0.0.1/tests/
--rw-r--r--   0 maverick   (501) staff       (20)      613 2023-03-22 09:01:34.000000 openai-promptify-py-0.0.1/tests/test_e2e.py
--rw-r--r--   0 maverick   (501) staff       (20)     7377 2023-04-20 01:40:26.000000 openai-promptify-py-0.0.1/tests/test_openai_promptif.py
+drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-04-20 03:13:00.863076 openai-promptify-py-0.0.2/
+-rw-r--r--   0 maverick   (501) staff       (20)     1838 2023-04-20 03:13:00.862896 openai-promptify-py-0.0.2/PKG-INFO
+-rw-r--r--   0 maverick   (501) staff       (20)     1472 2023-04-20 03:08:20.000000 openai-promptify-py-0.0.2/README.md
+-rw-r--r--   0 maverick   (501) staff       (20)      620 2023-04-20 03:08:33.000000 openai-promptify-py-0.0.2/pyproject.toml
+-rw-r--r--   0 maverick   (501) staff       (20)        7 2023-03-21 07:28:20.000000 openai-promptify-py-0.0.2/requirements.txt
+-rw-r--r--   0 maverick   (501) staff       (20)       38 2023-04-20 03:13:00.863122 openai-promptify-py-0.0.2/setup.cfg
+drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-04-20 03:13:00.861054 openai-promptify-py-0.0.2/src/
+-rw-r--r--   0 maverick   (501) staff       (20)     7527 2023-04-20 01:42:08.000000 openai-promptify-py-0.0.2/src/openai_promptify.py
+drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-04-20 03:13:00.862017 openai-promptify-py-0.0.2/src/openai_promptify_py.egg-info/
+-rw-r--r--   0 maverick   (501) staff       (20)     1838 2023-04-20 03:13:00.000000 openai-promptify-py-0.0.2/src/openai_promptify_py.egg-info/PKG-INFO
+-rw-r--r--   0 maverick   (501) staff       (20)      347 2023-04-20 03:13:00.000000 openai-promptify-py-0.0.2/src/openai_promptify_py.egg-info/SOURCES.txt
+-rw-r--r--   0 maverick   (501) staff       (20)        1 2023-04-20 03:13:00.000000 openai-promptify-py-0.0.2/src/openai_promptify_py.egg-info/dependency_links.txt
+-rw-r--r--   0 maverick   (501) staff       (20)        7 2023-04-20 03:13:00.000000 openai-promptify-py-0.0.2/src/openai_promptify_py.egg-info/requires.txt
+-rw-r--r--   0 maverick   (501) staff       (20)       17 2023-04-20 03:13:00.000000 openai-promptify-py-0.0.2/src/openai_promptify_py.egg-info/top_level.txt
+drwxr-xr-x   0 maverick   (501) staff       (20)        0 2023-04-20 03:13:00.862532 openai-promptify-py-0.0.2/tests/
+-rw-r--r--   0 maverick   (501) staff       (20)      613 2023-03-22 09:01:34.000000 openai-promptify-py-0.0.2/tests/test_e2e.py
+-rw-r--r--   0 maverick   (501) staff       (20)     7377 2023-04-20 01:40:26.000000 openai-promptify-py-0.0.2/tests/test_openai_promptif.py
```

### Comparing `openai-promptify-py-0.0.1/PKG-INFO` & `openai-promptify-py-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-promptify-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: a utility wrapepr for openai calls [NOT OFFICIAL]
 Project-URL: Homepage, https://github.com/tumatrix/openai-promptify-py.git/README.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
@@ -19,17 +19,15 @@
 can then call the API with a "proxy model name" and get the results without having to provide all configurations again
 and again.
 
 ## Installation
 
 You can install OpenAI Promptify Py using pip:
 
-    pip install openai-promptify-py @ git+https://github.com/tumatrix/openai-promptify-py.git
-
-_pip repository coming soon_
+    pip install openai-promptify-py
 
 ## Usage
 
 Here's an example of how to use OpenAI Promptify Py:
 
     from openai_promptify_py import OpenAIPromptifyPy
 
@@ -41,12 +39,12 @@
         }
 
         feature = OpenAIPromptify(openai_key=os.environ.get('OPENAI_KEY'), model_repo=models)
         response = feature.get_response('foo', {'animal': 'fox', 'location': 'over the moon'})
 
 ## Contributing
 
-If you'd like to contribute to OpenAI Promptify Py, please open an issue or pull request on our GitHub repository.
+If you'd like to contribute to OpenAI Promptify Py, please open an issue or pull request on our GitHub repository: https://github.com/tumatrix/openai-promptify-py
 
 ## License
 
 OpenAI Promptify Py is licensed under the MIT License.
```

### Comparing `openai-promptify-py-0.0.1/README.md` & `openai-promptify-py-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 can then call the API with a "proxy model name" and get the results without having to provide all configurations again
 and again.
 
 ## Installation
 
 You can install OpenAI Promptify Py using pip:
 
-    pip install openai-promptify-py @ git+https://github.com/tumatrix/openai-promptify-py.git
-
-_pip repository coming soon_
+    pip install openai-promptify-py
 
 ## Usage
 
 Here's an example of how to use OpenAI Promptify Py:
 
     from openai_promptify_py import OpenAIPromptifyPy
 
@@ -31,12 +29,12 @@
         }
 
         feature = OpenAIPromptify(openai_key=os.environ.get('OPENAI_KEY'), model_repo=models)
         response = feature.get_response('foo', {'animal': 'fox', 'location': 'over the moon'})
 
 ## Contributing
 
-If you'd like to contribute to OpenAI Promptify Py, please open an issue or pull request on our GitHub repository.
+If you'd like to contribute to OpenAI Promptify Py, please open an issue or pull request on our GitHub repository: https://github.com/tumatrix/openai-promptify-py
 
 ## License
 
 OpenAI Promptify Py is licensed under the MIT License.
```

### Comparing `openai-promptify-py-0.0.1/pyproject.toml` & `openai-promptify-py-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools]
 #packages = ['.']
 package-dir = { "" = "src" }
 
 [project]
 name = "openai-promptify-py"
-version = "0.0.1"
+version = "0.0.2"
 description = "a utility wrapepr for openai calls [NOT OFFICIAL]"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
```

### Comparing `openai-promptify-py-0.0.1/src/openai_promptify.py` & `openai-promptify-py-0.0.2/src/openai_promptify.py`

 * *Files identical despite different names*

### Comparing `openai-promptify-py-0.0.1/src/openai_promptify_py.egg-info/PKG-INFO` & `openai-promptify-py-0.0.2/src/openai_promptify_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-promptify-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: a utility wrapepr for openai calls [NOT OFFICIAL]
 Project-URL: Homepage, https://github.com/tumatrix/openai-promptify-py.git/README.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
@@ -19,17 +19,15 @@
 can then call the API with a "proxy model name" and get the results without having to provide all configurations again
 and again.
 
 ## Installation
 
 You can install OpenAI Promptify Py using pip:
 
-    pip install openai-promptify-py @ git+https://github.com/tumatrix/openai-promptify-py.git
-
-_pip repository coming soon_
+    pip install openai-promptify-py
 
 ## Usage
 
 Here's an example of how to use OpenAI Promptify Py:
 
     from openai_promptify_py import OpenAIPromptifyPy
 
@@ -41,12 +39,12 @@
         }
 
         feature = OpenAIPromptify(openai_key=os.environ.get('OPENAI_KEY'), model_repo=models)
         response = feature.get_response('foo', {'animal': 'fox', 'location': 'over the moon'})
 
 ## Contributing
 
-If you'd like to contribute to OpenAI Promptify Py, please open an issue or pull request on our GitHub repository.
+If you'd like to contribute to OpenAI Promptify Py, please open an issue or pull request on our GitHub repository: https://github.com/tumatrix/openai-promptify-py
 
 ## License
 
 OpenAI Promptify Py is licensed under the MIT License.
```

### Comparing `openai-promptify-py-0.0.1/tests/test_e2e.py` & `openai-promptify-py-0.0.2/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `openai-promptify-py-0.0.1/tests/test_openai_promptif.py` & `openai-promptify-py-0.0.2/tests/test_openai_promptif.py`

 * *Files identical despite different names*

