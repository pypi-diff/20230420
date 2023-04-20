# Comparing `tmp/autocog-0.0.3.tar.gz` & `tmp/autocog-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocog-0.0.3.tar", last modified: Tue Apr 18 20:09:29 2023, max compression
+gzip compressed data, was "autocog-0.0.4.tar", last modified: Thu Apr 20 11:14:14 2023, max compression
```

## Comparing `autocog-0.0.3.tar` & `autocog-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:09:29.965244 autocog-0.0.3/
--rw-r--r--   0 andreas    (501) staff       (20)       24 2023-04-18 15:13:54.000000 autocog-0.0.3/.gitignore
--rw-r--r--   0 andreas    (501) staff       (20)     1180 2023-04-18 20:09:29.965087 autocog-0.0.3/PKG-INFO
--rw-r--r--   0 andreas    (501) staff       (20)     1135 2023-04-18 20:03:23.000000 autocog-0.0.3/README.md
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:09:29.935119 autocog-0.0.3/autocog/
--rw-r--r--   0 andreas    (501) staff       (20)    17478 2023-04-18 20:03:31.000000 autocog-0.0.3/autocog/autocog.py
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:09:29.964861 autocog-0.0.3/autocog.egg-info/
--rw-r--r--   0 andreas    (501) staff       (20)     1180 2023-04-18 20:09:29.000000 autocog-0.0.3/autocog.egg-info/PKG-INFO
--rw-r--r--   0 andreas    (501) staff       (20)      236 2023-04-18 20:09:29.000000 autocog-0.0.3/autocog.egg-info/SOURCES.txt
--rw-r--r--   0 andreas    (501) staff       (20)        1 2023-04-18 20:09:29.000000 autocog-0.0.3/autocog.egg-info/dependency_links.txt
--rw-r--r--   0 andreas    (501) staff       (20)       52 2023-04-18 20:09:29.000000 autocog-0.0.3/autocog.egg-info/entry_points.txt
--rw-r--r--   0 andreas    (501) staff       (20)       20 2023-04-18 20:09:29.000000 autocog-0.0.3/autocog.egg-info/requires.txt
--rw-r--r--   0 andreas    (501) staff       (20)        1 2023-04-18 20:09:29.000000 autocog-0.0.3/autocog.egg-info/top_level.txt
--rw-r--r--   0 andreas    (501) staff       (20)       38 2023-04-18 20:09:29.965287 autocog-0.0.3/setup.cfg
--rw-r--r--   0 andreas    (501) staff       (20)      746 2023-04-18 20:09:12.000000 autocog-0.0.3/setup.py
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-20 11:14:14.410949 autocog-0.0.4/
+-rw-r--r--   0 andreas    (501) staff       (20)       24 2023-04-18 15:13:54.000000 autocog-0.0.4/.gitignore
+-rw-r--r--   0 andreas    (501) staff       (20)     1312 2023-04-20 11:14:14.410757 autocog-0.0.4/PKG-INFO
+-rw-r--r--   0 andreas    (501) staff       (20)     1267 2023-04-18 20:12:23.000000 autocog-0.0.4/README.md
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-20 11:14:14.375450 autocog-0.0.4/autocog/
+-rw-r--r--   0 andreas    (501) staff       (20)        0 2023-04-20 11:13:20.000000 autocog-0.0.4/autocog/__init__.py
+-rw-r--r--   0 andreas    (501) staff       (20)    17478 2023-04-18 20:03:31.000000 autocog-0.0.4/autocog/autocog.py
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-20 11:14:14.410535 autocog-0.0.4/autocog.egg-info/
+-rw-r--r--   0 andreas    (501) staff       (20)     1312 2023-04-20 11:14:14.000000 autocog-0.0.4/autocog.egg-info/PKG-INFO
+-rw-r--r--   0 andreas    (501) staff       (20)      256 2023-04-20 11:14:14.000000 autocog-0.0.4/autocog.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas    (501) staff       (20)        1 2023-04-20 11:14:14.000000 autocog-0.0.4/autocog.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas    (501) staff       (20)       52 2023-04-20 11:14:14.000000 autocog-0.0.4/autocog.egg-info/entry_points.txt
+-rw-r--r--   0 andreas    (501) staff       (20)       20 2023-04-20 11:14:14.000000 autocog-0.0.4/autocog.egg-info/requires.txt
+-rw-r--r--   0 andreas    (501) staff       (20)        8 2023-04-20 11:14:14.000000 autocog-0.0.4/autocog.egg-info/top_level.txt
+-rw-r--r--   0 andreas    (501) staff       (20)       38 2023-04-20 11:14:14.410997 autocog-0.0.4/setup.cfg
+-rw-r--r--   0 andreas    (501) staff       (20)      746 2023-04-20 11:14:09.000000 autocog-0.0.4/setup.py
```

### Comparing `autocog-0.0.3/PKG-INFO` & `autocog-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 Metadata-Version: 2.1
 Name: autocog
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/andreasjansson/AutoCog
 Description-Content-Type: text/markdown
 
 # AutoCog
 
+[![PyPI version](https://badge.fury.io/py/autocog.svg)](https://badge.fury.io/py/autocog)
+
 _Generate [predict.py and cog.yaml](https://github.com/replicate/cog) automatically using GPT4_
 
 
+## Install
+
+```
+pip install autocog
+```
+
 ## Usage
 
 First, set your OpenAI API key in an environment variable
 
 ```
 OPENAI_API_KEY=sk-...
 ```
```

### Comparing `autocog-0.0.3/README.md` & `autocog-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # AutoCog
 
+[![PyPI version](https://badge.fury.io/py/autocog.svg)](https://badge.fury.io/py/autocog)
+
 _Generate [predict.py and cog.yaml](https://github.com/replicate/cog) automatically using GPT4_
 
 ![Screen recording](https://github.com/andreasjansson/AutoCog/raw/main/assets/screen-recording.gif)
 
+## Install
+
+```
+pip install autocog
+```
+
 ## Usage
 
 First, set your OpenAI API key in an environment variable
 
 ```
 OPENAI_API_KEY=sk-...
 ```
```

### Comparing `autocog-0.0.3/autocog/autocog.py` & `autocog-0.0.4/autocog/autocog.py`

 * *Files identical despite different names*

### Comparing `autocog-0.0.3/autocog.egg-info/PKG-INFO` & `autocog-0.0.4/autocog.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 Metadata-Version: 2.1
 Name: autocog
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/andreasjansson/AutoCog
 Description-Content-Type: text/markdown
 
 # AutoCog
 
+[![PyPI version](https://badge.fury.io/py/autocog.svg)](https://badge.fury.io/py/autocog)
+
 _Generate [predict.py and cog.yaml](https://github.com/replicate/cog) automatically using GPT4_
 
 
+## Install
+
+```
+pip install autocog
+```
+
 ## Usage
 
 First, set your OpenAI API key in an environment variable
 
 ```
 OPENAI_API_KEY=sk-...
 ```
```

### Comparing `autocog-0.0.3/setup.py` & `autocog-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (this_directory / "README.md").read_text()
 long_description = long_description.replace("![Screen recording](https://github.com/andreasjansson/AutoCog/raw/main/assets/screen-recording.gif)\n", "")
 
 setup(
     name="autocog",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.0.3",
+    version="0.0.4",
     url="https://github.com/andreasjansson/AutoCog",
     packages=find_packages(),
     install_requires=[
         "openai",
         "click",
         "Pillow",
     ],
```

