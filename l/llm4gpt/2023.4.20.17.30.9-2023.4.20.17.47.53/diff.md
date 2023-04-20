# Comparing `tmp/llm4gpt-2023.4.20.17.30.9.tar.gz` & `tmp/llm4gpt-2023.4.20.17.47.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4gpt-2023.4.20.17.30.9.tar", last modified: Thu Apr 20 09:30:09 2023, max compression
+gzip compressed data, was "llm4gpt-2023.4.20.17.47.53.tar", last modified: Thu Apr 20 09:47:53 2023, max compression
```

## Comparing `llm4gpt-2023.4.20.17.30.9.tar` & `llm4gpt-2023.4.20.17.47.53.tar`

### file list

```diff
@@ -1,57 +1,63 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.713052 llm4gpt-2023.4.20.17.30.9/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1206 2023-04-11 04:36:04.000000 llm4gpt-2023.4.20.17.30.9/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1369 2023-04-20 09:30:09.713141 llm4gpt-2023.4.20.17.30.9/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      553 2023-04-11 06:33:00.000000 llm4gpt-2023.4.20.17.30.9/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.710512 llm4gpt-2023.4.20.17.30.9/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      379 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-11 04:38:41.000000 llm4gpt-2023.4.20.17.30.9/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.710900 llm4gpt-2023.4.20.17.30.9/llm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/llm/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1497 2023-04-20 07:47:11.000000 llm4gpt-2023.4.20.17.30.9/llm/chatllm.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.711327 llm4gpt-2023.4.20.17.30.9/llm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/llm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/llm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/llm/clis/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.711594 llm4gpt-2023.4.20.17.30.9/llm/kb/
--rw-r--r--   0 betterme   (501) staff       (20)     1458 2023-04-20 09:28:22.000000 llm4gpt-2023.4.20.17.30.9/llm/kb/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 08:50:43.000000 llm4gpt-2023.4.20.17.30.9/llm/kb/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.711712 llm4gpt-2023.4.20.17.30.9/llm/uis/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.20.17.30.9/llm/uis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2923 2023-04-20 09:28:23.000000 llm4gpt-2023.4.20.17.30.9/llm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.712634 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     1369 2023-04-20 09:30:09.000000 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      825 2023-04-20 09:30:09.000000 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 09:30:09.000000 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-20 09:30:09.000000 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 09:30:09.000000 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       31 2023-04-20 09:30:09.000000 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-20 09:30:09.000000 llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/top_level.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       32 2023-04-13 05:31:18.000000 llm4gpt-2023.4.20.17.30.9/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-20 09:30:09.713420 llm4gpt-2023.4.20.17.30.9/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.20.17.30.9/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:30:09.712903 llm4gpt-2023.4.20.17.30.9/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.30.9/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:47:53.692806 llm4gpt-2023.4.20.17.47.53/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1206 2023-04-11 04:36:04.000000 llm4gpt-2023.4.20.17.47.53/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1370 2023-04-20 09:47:53.692919 llm4gpt-2023.4.20.17.47.53/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      553 2023-04-11 06:33:00.000000 llm4gpt-2023.4.20.17.47.53/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:47:53.688865 llm4gpt-2023.4.20.17.47.53/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      379 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-11 04:38:41.000000 llm4gpt-2023.4.20.17.47.53/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:47:53.689442 llm4gpt-2023.4.20.17.47.53/llm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/llm/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1586 2023-04-20 09:42:26.000000 llm4gpt-2023.4.20.17.47.53/llm/chatllm.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:47:53.690065 llm4gpt-2023.4.20.17.47.53/llm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/llm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/llm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/llm/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:47:53.690775 llm4gpt-2023.4.20.17.47.53/llm/kb/
+-rw-r--r--   0 betterme   (501) staff       (20)     1458 2023-04-20 09:28:22.000000 llm4gpt-2023.4.20.17.47.53/llm/kb/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 08:50:43.000000 llm4gpt-2023.4.20.17.47.53/llm/kb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2316 2023-04-20 09:45:22.000000 llm4gpt-2023.4.20.17.47.53/llm/kb/source_service_.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:47:53.691169 llm4gpt-2023.4.20.17.47.53/llm/models/
+-rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-04-20 09:44:52.000000 llm4gpt-2023.4.20.17.47.53/llm/models/ChatLLM.py
+-rw-r--r--   0 betterme   (501) staff       (20)       31 2023-04-20 09:44:52.000000 llm4gpt-2023.4.20.17.47.53/llm/models/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1693 2023-04-20 09:44:52.000000 llm4gpt-2023.4.20.17.47.53/llm/models/gpt_service.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2556 2023-04-20 09:47:46.000000 llm4gpt-2023.4.20.17.47.53/llm/qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:47:53.691290 llm4gpt-2023.4.20.17.47.53/llm/uis/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.20.17.47.53/llm/uis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2923 2023-04-20 09:28:23.000000 llm4gpt-2023.4.20.17.47.53/llm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:47:53.692320 llm4gpt-2023.4.20.17.47.53/llm4gpt.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1370 2023-04-20 09:47:53.000000 llm4gpt-2023.4.20.17.47.53/llm4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      932 2023-04-20 09:47:53.000000 llm4gpt-2023.4.20.17.47.53/llm4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 09:47:53.000000 llm4gpt-2023.4.20.17.47.53/llm4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-20 09:47:53.000000 llm4gpt-2023.4.20.17.47.53/llm4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 09:47:53.000000 llm4gpt-2023.4.20.17.47.53/llm4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       31 2023-04-20 09:47:53.000000 llm4gpt-2023.4.20.17.47.53/llm4gpt.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-20 09:47:53.000000 llm4gpt-2023.4.20.17.47.53/llm4gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       32 2023-04-13 05:31:18.000000 llm4gpt-2023.4.20.17.47.53/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-20 09:47:53.693247 llm4gpt-2023.4.20.17.47.53/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.20.17.47.53/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 09:47:53.692650 llm4gpt-2023.4.20.17.47.53/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.17.47.53/tox.ini
```

### Comparing `llm4gpt-2023.4.20.17.30.9/.gitignore` & `llm4gpt-2023.4.20.17.47.53/.gitignore`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/.travis.yml` & `llm4gpt-2023.4.20.17.47.53/.travis.yml`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/CONTRIBUTING.rst` & `llm4gpt-2023.4.20.17.47.53/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/LICENSE` & `llm4gpt-2023.4.20.17.47.53/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/Makefile` & `llm4gpt-2023.4.20.17.47.53/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/PKG-INFO` & `llm4gpt-2023.4.20.17.47.53/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.20.17.30.9
+Version: 2023.4.20.17.47.53
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.20.17.30.9/README.md` & `llm4gpt-2023.4.20.17.47.53/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/README.rst` & `llm4gpt-2023.4.20.17.47.53/README.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/docs/Makefile` & `llm4gpt-2023.4.20.17.47.53/docs/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/docs/conf.py` & `llm4gpt-2023.4.20.17.47.53/docs/conf.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/docs/installation.rst` & `llm4gpt-2023.4.20.17.47.53/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/docs/make.bat` & `llm4gpt-2023.4.20.17.47.53/docs/make.bat`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/llm/chatllm.py` & `llm4gpt-2023.4.20.17.47.53/llm/chatllm.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,19 +35,20 @@
     def _call(self, prompt: str, stop: Optional[List[str]] = None) -> str:
         cuda_empty_cache()  # todo: 减少调用次数
 
         response, _ = self.chat_func(query=prompt, history=self.history[-self.max_turns:])
         if stop:
             response = enforce_stop_tokens(response, stop)
         self.history += [(None, response)]
-        return response
+        return response  # todo: 增加流失输出
 
     def set_chat_kwargs(self, **kwargs):
         self.chat_func = partial(self.chat_func, **kwargs)
 
 
 if __name__ == '__main__':
     from llm.utils import llm_load
 
     model, tokenizer = llm_load("/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm")
     glm = ChatLLM()
-    glm.chat_func = model.chat  # partial(self.chat_func, **kwargs)
+    glm.chat_func = partial(model.chat, tokenizer=tokenizer)
+    glm.chat_func = partial(model.stream_chat, tokenizer=tokenizer)
```

### Comparing `llm4gpt-2023.4.20.17.30.9/llm/clis/cli.py` & `llm4gpt-2023.4.20.17.47.53/llm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/llm/kb/FaissANN.py` & `llm4gpt-2023.4.20.17.47.53/llm/kb/FaissANN.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/llm/utils.py` & `llm4gpt-2023.4.20.17.47.53/llm/utils.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/PKG-INFO` & `llm4gpt-2023.4.20.17.47.53/llm4gpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.20.17.30.9
+Version: 2023.4.20.17.47.53
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.20.17.30.9/llm4gpt.egg-info/SOURCES.txt` & `llm4gpt-2023.4.20.17.47.53/llm4gpt.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -26,20 +26,25 @@
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 llm/__init__.py
 llm/chatllm.py
+llm/qa.py
 llm/utils.py
 llm/clis/README.md
 llm/clis/__init__.py
 llm/clis/cli.py
 llm/kb/FaissANN.py
 llm/kb/__init__.py
+llm/kb/source_service_.py
+llm/models/ChatLLM.py
+llm/models/__init__.py
+llm/models/gpt_service.py
 llm/uis/__init__.py
 llm4gpt.egg-info/PKG-INFO
 llm4gpt.egg-info/SOURCES.txt
 llm4gpt.egg-info/dependency_links.txt
 llm4gpt.egg-info/entry_points.txt
 llm4gpt.egg-info/not-zip-safe
 llm4gpt.egg-info/requires.txt
```

### Comparing `llm4gpt-2023.4.20.17.30.9/setup.py` & `llm4gpt-2023.4.20.17.47.53/setup.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.17.30.9/tests/test_llm4gpt.py` & `llm4gpt-2023.4.20.17.47.53/tests/test_llm4gpt.py`

 * *Files identical despite different names*

