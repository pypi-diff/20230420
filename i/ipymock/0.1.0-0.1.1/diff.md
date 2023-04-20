# Comparing `tmp/ipymock-0.1.0.tar.gz` & `tmp/ipymock-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-0.1.0.tar", last modified: Thu Apr 20 07:36:07 2023, max compression
+gzip compressed data, was "ipymock-0.1.1.tar", last modified: Thu Apr 20 07:58:46 2023, max compression
```

## Comparing `ipymock-0.1.0.tar` & `ipymock-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 07:36:07.155240 ipymock-0.1.0/
--rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.1.0/LICENSE
--rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.1.0/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-20 07:36:07.154814 ipymock-0.1.0/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     6783 2023-04-20 07:33:46.000000 ipymock-0.1.0/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 07:36:07.150506 ipymock-0.1.0/ipymock/
--rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-20 07:33:36.000000 ipymock-0.1.0/ipymock/__init__.py
--rw-r--r--   0 saintway   (501) staff       (20)     1196 2023-04-20 07:33:36.000000 ipymock-0.1.0/ipymock/_nbdev.py
--rw-r--r--   0 saintway   (501) staff       (20)     9416 2023-04-20 07:33:36.000000 ipymock-0.1.0/ipymock/mock.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 07:36:07.153001 ipymock-0.1.0/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 07:36:07.153926 ipymock-0.1.0/ipymock.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.1.0/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.1.0/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-20 07:36:07.000000 ipymock-0.1.0/ipymock.egg-info/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-20 07:36:07.000000 ipymock-0.1.0/ipymock.egg-info/SOURCES.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-20 07:36:07.000000 ipymock-0.1.0/ipymock.egg-info/dependency_links.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.1.0/ipymock.egg-info/not-zip-safe
--rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-20 07:36:07.000000 ipymock-0.1.0/ipymock.egg-info/requires.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-20 07:36:07.000000 ipymock-0.1.0/ipymock.egg-info/top_level.txt
--rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-20 07:35:39.000000 ipymock-0.1.0/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-20 07:36:07.155436 ipymock-0.1.0/setup.cfg
--rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.1.0/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 07:58:46.713326 ipymock-0.1.1/
+-rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.1.1/LICENSE
+-rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.1.1/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-20 07:58:46.713080 ipymock-0.1.1/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)     6783 2023-04-20 07:58:34.000000 ipymock-0.1.1/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 07:58:46.709849 ipymock-0.1.1/ipymock/
+-rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-20 07:58:25.000000 ipymock-0.1.1/ipymock/__init__.py
+-rw-r--r--   0 saintway   (501) staff       (20)     1196 2023-04-20 07:58:25.000000 ipymock-0.1.1/ipymock/_nbdev.py
+-rw-r--r--   0 saintway   (501) staff       (20)     9545 2023-04-20 07:58:25.000000 ipymock-0.1.1/ipymock/mock.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 07:58:46.711583 ipymock-0.1.1/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 07:58:46.712470 ipymock-0.1.1/ipymock.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.1.1/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.1.1/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-20 07:58:46.000000 ipymock-0.1.1/ipymock.egg-info/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-20 07:58:46.000000 ipymock-0.1.1/ipymock.egg-info/SOURCES.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-20 07:58:46.000000 ipymock-0.1.1/ipymock.egg-info/dependency_links.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.1.1/ipymock.egg-info/not-zip-safe
+-rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-20 07:58:46.000000 ipymock-0.1.1/ipymock.egg-info/requires.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-20 07:58:46.000000 ipymock-0.1.1/ipymock.egg-info/top_level.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-20 07:58:44.000000 ipymock-0.1.1/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-20 07:58:46.713414 ipymock-0.1.1/setup.cfg
+-rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.1.1/setup.py
```

### Comparing `ipymock-0.1.0/LICENSE` & `ipymock-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-0.1.0/PKG-INFO` & `ipymock-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-0.1.0/README.md` & `ipymock-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ipymock-0.1.0/ipymock/__init__.py` & `ipymock-0.1.1/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-0.1.0/ipymock/_nbdev.py` & `ipymock-0.1.1/ipymock/_nbdev.py`

 * *Files identical despite different names*

### Comparing `ipymock-0.1.0/ipymock/mock.py` & `ipymock-0.1.1/ipymock/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,19 @@
             'finish_reason': 'stop',
             'index': 0,
             'logprobs': None,
             'text': response,
         })
     return attributize({
         'choices': choices,
+        'usage': {
+            'completion_tokens': 0,
+            'prompt_tokens': 0,
+            'total_tokens': 0,
+        },
     })
 
 def chat_delta(prompt):
     res = ''
     for response in start_conversation(prompt):
         yield attributize({
             'choices': [
```

### Comparing `ipymock-0.1.0/ipymock.egg-info/PKG-INFO` & `ipymock-0.1.1/ipymock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-0.1.0/settings.ini` & `ipymock-0.1.1/settings.ini`

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
-version = 0.1.0
+version = 0.1.1
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `ipymock-0.1.0/setup.py` & `ipymock-0.1.1/setup.py`

 * *Files identical despite different names*

