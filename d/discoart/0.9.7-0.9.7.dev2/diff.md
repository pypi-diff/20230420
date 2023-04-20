# Comparing `tmp/discoart-0.9.7.tar.gz` & `tmp/discoart-0.9.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/discoart-0.9.7.tar", last modified: Sat Jul 30 15:29:54 2022, max compression
+gzip compressed data, was "discoart-0.9.7.dev2.tar", last modified: Sat Jul 30 15:28:39 2022, max compression
```

## Comparing `discoart-0.9.7.tar` & `discoart-0.9.7.dev2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 15:29:54.000000 discoart-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (121)     5234 2022-07-30 15:29:34.000000 discoart-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-07-30 15:29:34.000000 discoart-0.9.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    30285 2022-07-30 15:29:54.000000 discoart-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    23656 2022-07-30 15:29:34.000000 discoart-0.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 15:29:54.000000 discoart-0.9.7/discoart/
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6248 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    27262 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/create.py
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/executors.py
--rw-r--r--   0 runner    (1001) docker     (121)    23076 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 15:29:54.000000 discoart-0.9.7/discoart/nn/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/nn/losses.py
--rw-r--r--   0 runner    (1001) docker     (121)     6535 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/nn/make_cutouts.py
--rw-r--r--   0 runner    (1001) docker     (121)     3056 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/nn/perlin_noises.py
--rw-r--r--   0 runner    (1001) docker     (121)     4790 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/nn/sec_diff.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/nn/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4824 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/persist.py
--rw-r--r--   0 runner    (1001) docker     (121)     2557 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 15:29:54.000000 discoart-0.9.7/discoart/resources/
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/resources/cut-schedules.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/resources/default.yml
--rw-r--r--   0 runner    (1001) docker     (121)    21059 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/resources/docstrings.yml
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/resources/flow.yml
--rw-r--r--   0 runner    (1001) docker     (121)     7169 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/resources/models.yml
--rw-r--r--   0 runner    (1001) docker     (121)     9400 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/resources/vocab.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15656 2022-07-30 15:29:34.000000 discoart-0.9.7/discoart/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 15:29:54.000000 discoart-0.9.7/discoart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    30285 2022-07-30 15:29:54.000000 discoart-0.9.7/discoart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-07-30 15:29:54.000000 discoart-0.9.7/discoart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-30 15:29:54.000000 discoart-0.9.7/discoart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-30 15:29:54.000000 discoart-0.9.7/discoart.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-07-30 15:29:54.000000 discoart-0.9.7/discoart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-07-30 15:29:54.000000 discoart-0.9.7/discoart.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-30 15:29:54.000000 discoart-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3354 2022-07-30 15:29:34.000000 discoart-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 15:28:39.192894 discoart-0.9.7.dev2/
+-rw-r--r--   0 runner    (1001) docker     (121)     5234 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    30290 2022-07-30 15:28:39.192894 discoart-0.9.7.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    23656 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 15:28:39.188894 discoart-0.9.7.dev2/discoart/
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2022-07-30 15:28:38.000000 discoart-0.9.7.dev2/discoart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      702 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6248 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27262 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/executors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23076 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 15:28:39.188894 discoart-0.9.7.dev2/discoart/nn/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/nn/losses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6535 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/nn/make_cutouts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3056 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/nn/perlin_noises.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4790 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/nn/sec_diff.py
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/nn/transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4824 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/persist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2557 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 15:28:39.192894 discoart-0.9.7.dev2/discoart/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/resources/cut-schedules.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/resources/default.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    21059 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/resources/docstrings.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/resources/flow.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     7169 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/resources/models.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     9400 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/resources/vocab.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    15656 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/discoart/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 15:28:39.188894 discoart-0.9.7.dev2/discoart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    30290 2022-07-30 15:28:39.000000 discoart-0.9.7.dev2/discoart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      783 2022-07-30 15:28:39.000000 discoart-0.9.7.dev2/discoart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-30 15:28:39.000000 discoart-0.9.7.dev2/discoart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-30 15:28:39.000000 discoart-0.9.7.dev2/discoart.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2022-07-30 15:28:39.000000 discoart-0.9.7.dev2/discoart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-07-30 15:28:39.000000 discoart-0.9.7.dev2/discoart.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-30 15:28:39.192894 discoart-0.9.7.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3354 2022-07-30 15:28:34.000000 discoart-0.9.7.dev2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `discoart-0.9.7/LICENSE` & `discoart-0.9.7.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/PKG-INFO` & `discoart-0.9.7.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discoart
-Version: 0.9.7
+Version: 0.9.7.dev2
 Summary: Create Disco Diffusion artworks in one line
 Home-page: https://github.com/jina-ai/discoart
 Author: Jina AI
 Author-email: hello@jina.ai
 License: MIT
 Download-URL: https://github.com/jina-ai/discoart/tags
 Project-URL: Source, https://github.com/jina-ai/discoart/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discoart Version: 0.9.7 Summary: Create Disco
+Metadata-Version: 2.1 Name: discoart Version: 0.9.7.dev2 Summary: Create Disco
 Diffusion artworks in one line Home-page: https://github.com/jina-ai/discoart
 Author: Jina AI Author-email: hello@jina.ai License: MIT Download-URL: https://
 github.com/jina-ai/discoart/tags Project-URL: Source, https://github.com/jina-
 ai/discoart/ Project-URL: Tracker, https://github.com/jina-ai/discoart/issues
 Description: ![](.github/banner.png)
             Create compelling Disco Diffusion artworks in one line
  [PyPI] [Docker_Cloud_Build_Status] [https://img.shields.io/badge/Slack-3.1k-
```

### Comparing `discoart-0.9.7/README.md` & `discoart-0.9.7.dev2/README.md`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/api.py` & `discoart-0.9.7.dev2/discoart/api.py`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/config.py` & `discoart-0.9.7.dev2/discoart/config.py`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/create.py` & `discoart-0.9.7.dev2/discoart/create.py`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/executors.py` & `discoart-0.9.7.dev2/discoart/executors.py`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/helper.py` & `discoart-0.9.7.dev2/discoart/helper.py`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/nn/losses.py` & `discoart-0.9.7.dev2/discoart/nn/losses.py`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/nn/make_cutouts.py` & `discoart-0.9.7.dev2/discoart/nn/make_cutouts.py`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/nn/perlin_noises.py` & `discoart-0.9.7.dev2/discoart/nn/perlin_noises.py`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/nn/sec_diff.py` & `discoart-0.9.7.dev2/discoart/nn/sec_diff.py`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/parser.py` & `discoart-0.9.7.dev2/discoart/parser.py`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/persist.py` & `discoart-0.9.7.dev2/discoart/persist.py`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/prompt.py` & `discoart-0.9.7.dev2/discoart/prompt.py`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/resources/cut-schedules.yml` & `discoart-0.9.7.dev2/discoart/resources/cut-schedules.yml`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/resources/default.yml` & `discoart-0.9.7.dev2/discoart/resources/default.yml`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/resources/docstrings.yml` & `discoart-0.9.7.dev2/discoart/resources/docstrings.yml`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/resources/flow.yml` & `discoart-0.9.7.dev2/discoart/resources/flow.yml`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/resources/models.yml` & `discoart-0.9.7.dev2/discoart/resources/models.yml`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/resources/vocab.txt` & `discoart-0.9.7.dev2/discoart/resources/vocab.txt`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart/runner.py` & `discoart-0.9.7.dev2/discoart/runner.py`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/discoart.egg-info/PKG-INFO` & `discoart-0.9.7.dev2/discoart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discoart
-Version: 0.9.7
+Version: 0.9.7.dev2
 Summary: Create Disco Diffusion artworks in one line
 Home-page: https://github.com/jina-ai/discoart
 Author: Jina AI
 Author-email: hello@jina.ai
 License: MIT
 Download-URL: https://github.com/jina-ai/discoart/tags
 Project-URL: Source, https://github.com/jina-ai/discoart/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discoart Version: 0.9.7 Summary: Create Disco
+Metadata-Version: 2.1 Name: discoart Version: 0.9.7.dev2 Summary: Create Disco
 Diffusion artworks in one line Home-page: https://github.com/jina-ai/discoart
 Author: Jina AI Author-email: hello@jina.ai License: MIT Download-URL: https://
 github.com/jina-ai/discoart/tags Project-URL: Source, https://github.com/jina-
 ai/discoart/ Project-URL: Tracker, https://github.com/jina-ai/discoart/issues
 Description: ![](.github/banner.png)
             Create compelling Disco Diffusion artworks in one line
  [PyPI] [Docker_Cloud_Build_Status] [https://img.shields.io/badge/Slack-3.1k-
```

### Comparing `discoart-0.9.7/discoart.egg-info/SOURCES.txt` & `discoart-0.9.7.dev2/discoart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discoart-0.9.7/setup.py` & `discoart-0.9.7.dev2/setup.py`

 * *Files identical despite different names*

