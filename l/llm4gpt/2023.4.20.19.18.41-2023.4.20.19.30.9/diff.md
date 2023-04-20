# Comparing `tmp/llm4gpt-2023.4.20.19.18.41.tar.gz` & `tmp/llm4gpt-2023.4.20.19.30.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4gpt-2023.4.20.19.18.41.tar", last modified: Thu Apr 20 11:18:41 2023, max compression
+gzip compressed data, was "llm4gpt-2023.4.20.19.30.9.tar", last modified: Thu Apr 20 11:30:09 2023, max compression
```

## Comparing `llm4gpt-2023.4.20.19.18.41.tar` & `llm4gpt-2023.4.20.19.30.9.tar`

### file list

```diff
@@ -1,67 +1,63 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:18:41.326010 llm4gpt-2023.4.20.19.18.41/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1206 2023-04-20 11:03:56.000000 llm4gpt-2023.4.20.19.18.41/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     2128 2023-04-20 11:18:41.326103 llm4gpt-2023.4.20.19.18.41/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1311 2023-04-20 11:18:40.000000 llm4gpt-2023.4.20.19.18.41/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:18:41.319455 llm4gpt-2023.4.20.19.18.41/data/
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.19.18.41/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.19.18.41/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.19.18.41/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.19.18.41/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:18:41.321886 llm4gpt-2023.4.20.19.18.41/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      379 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-11 04:38:41.000000 llm4gpt-2023.4.20.19.18.41/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:18:41.322740 llm4gpt-2023.4.20.19.18.41/llm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/llm/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1815 2023-04-20 10:41:14.000000 llm4gpt-2023.4.20.19.18.41/llm/chatllm.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:18:41.323339 llm4gpt-2023.4.20.19.18.41/llm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/llm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/llm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/llm/clis/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:18:41.323813 llm4gpt-2023.4.20.19.18.41/llm/kb/
--rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-04-20 10:20:30.000000 llm4gpt-2023.4.20.19.18.41/llm/kb/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 08:50:43.000000 llm4gpt-2023.4.20.19.18.41/llm/kb/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:18:41.324537 llm4gpt-2023.4.20.19.18.41/llm/models/
--rw-r--r--   0 betterme   (501) staff       (20)     1387 2023-04-20 10:20:57.000000 llm4gpt-2023.4.20.19.18.41/llm/models/ChatLLM.py
--rw-r--r--   0 betterme   (501) staff       (20)       31 2023-04-20 09:44:52.000000 llm4gpt-2023.4.20.19.18.41/llm/models/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1693 2023-04-20 10:20:57.000000 llm4gpt-2023.4.20.19.18.41/llm/models/gpt_service.py
--rw-r--r--   0 betterme   (501) staff       (20)     2509 2023-04-20 10:34:20.000000 llm4gpt-2023.4.20.19.18.41/llm/qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:18:41.324713 llm4gpt-2023.4.20.19.18.41/llm/uis/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.20.19.18.41/llm/uis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2923 2023-04-20 09:28:23.000000 llm4gpt-2023.4.20.19.18.41/llm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:18:41.325622 llm4gpt-2023.4.20.19.18.41/llm4gpt.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     2128 2023-04-20 11:18:41.000000 llm4gpt-2023.4.20.19.18.41/llm4gpt.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      976 2023-04-20 11:18:41.000000 llm4gpt-2023.4.20.19.18.41/llm4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 11:18:41.000000 llm4gpt-2023.4.20.19.18.41/llm4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-20 11:18:41.000000 llm4gpt-2023.4.20.19.18.41/llm4gpt.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 11:18:41.000000 llm4gpt-2023.4.20.19.18.41/llm4gpt.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       18 2023-04-20 11:18:41.000000 llm4gpt-2023.4.20.19.18.41/llm4gpt.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-20 11:18:41.000000 llm4gpt-2023.4.20.19.18.41/llm4gpt.egg-info/top_level.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-20 10:16:04.000000 llm4gpt-2023.4.20.19.18.41/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-20 11:18:41.326381 llm4gpt-2023.4.20.19.18.41/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.20.19.18.41/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:18:41.325875 llm4gpt-2023.4.20.19.18.41/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.18.41/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:30:09.899998 llm4gpt-2023.4.20.19.30.9/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1206 2023-04-20 11:03:56.000000 llm4gpt-2023.4.20.19.30.9/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     2129 2023-04-20 11:30:09.900097 llm4gpt-2023.4.20.19.30.9/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1313 2023-04-20 11:20:06.000000 llm4gpt-2023.4.20.19.30.9/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:30:09.893996 llm4gpt-2023.4.20.19.30.9/data/
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.19.30.9/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.19.30.9/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.19.30.9/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.19.30.9/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:30:09.896213 llm4gpt-2023.4.20.19.30.9/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      379 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4gpt-2023.4.20.19.30.9/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:30:09.897188 llm4gpt-2023.4.20.19.30.9/llm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/llm/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1815 2023-04-20 10:41:14.000000 llm4gpt-2023.4.20.19.30.9/llm/chatllm.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:30:09.897923 llm4gpt-2023.4.20.19.30.9/llm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/llm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/llm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/llm/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:30:09.898416 llm4gpt-2023.4.20.19.30.9/llm/kb/
+-rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-04-20 10:20:30.000000 llm4gpt-2023.4.20.19.30.9/llm/kb/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 08:50:43.000000 llm4gpt-2023.4.20.19.30.9/llm/kb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2509 2023-04-20 10:34:20.000000 llm4gpt-2023.4.20.19.30.9/llm/qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:30:09.898654 llm4gpt-2023.4.20.19.30.9/llm/uis/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.20.19.30.9/llm/uis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2923 2023-04-20 09:28:23.000000 llm4gpt-2023.4.20.19.30.9/llm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:30:09.899582 llm4gpt-2023.4.20.19.30.9/llm4gpt.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     2129 2023-04-20 11:30:09.000000 llm4gpt-2023.4.20.19.30.9/llm4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      905 2023-04-20 11:30:09.000000 llm4gpt-2023.4.20.19.30.9/llm4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 11:30:09.000000 llm4gpt-2023.4.20.19.30.9/llm4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-20 11:30:09.000000 llm4gpt-2023.4.20.19.30.9/llm4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 11:30:09.000000 llm4gpt-2023.4.20.19.30.9/llm4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       18 2023-04-20 11:30:09.000000 llm4gpt-2023.4.20.19.30.9/llm4gpt.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-20 11:30:09.000000 llm4gpt-2023.4.20.19.30.9/llm4gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-20 11:28:30.000000 llm4gpt-2023.4.20.19.30.9/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-20 11:30:09.900398 llm4gpt-2023.4.20.19.30.9/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.20.19.30.9/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 11:30:09.899864 llm4gpt-2023.4.20.19.30.9/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.19.30.9/tox.ini
```

### Comparing `llm4gpt-2023.4.20.19.18.41/.gitignore` & `llm4gpt-2023.4.20.19.30.9/.gitignore`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/.travis.yml` & `llm4gpt-2023.4.20.19.30.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/CONTRIBUTING.rst` & `llm4gpt-2023.4.20.19.30.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/LICENSE` & `llm4gpt-2023.4.20.19.30.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/Makefile` & `llm4gpt-2023.4.20.19.30.9/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/PKG-INFO` & `llm4gpt-2023.4.20.19.30.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.20.19.18.41
+Version: 2023.4.20.19.30.9
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -76,17 +76,17 @@
 
 - [x] 增加本地知识库组件
 
 - [ ] 增加互联网搜索组件
 
 - [ ] 增加知识图谱组件
 
--[ ] 增加微调模块
+- [ ] 增加微调模块
 
--[ ] 增加流式输出
+- [ ] 增加流式输出
 
 
 
 
 
 =======
 History
```

### Comparing `llm4gpt-2023.4.20.19.18.41/README.md` & `llm4gpt-2023.4.20.19.30.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,13 +54,13 @@
 
 - [x] 增加本地知识库组件
 
 - [ ] 增加互联网搜索组件
 
 - [ ] 增加知识图谱组件
 
--[ ] 增加微调模块
+- [ ] 增加微调模块
 
--[ ] 增加流式输出
+- [ ] 增加流式输出
```

### Comparing `llm4gpt-2023.4.20.19.18.41/README.rst` & `llm4gpt-2023.4.20.19.30.9/README.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/data/姚明.txt` & `llm4gpt-2023.4.20.19.30.9/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/data/王治郅.txt` & `llm4gpt-2023.4.20.19.30.9/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/data/科比.txt` & `llm4gpt-2023.4.20.19.30.9/data/科比.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/docs/Makefile` & `llm4gpt-2023.4.20.19.30.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/docs/conf.py` & `llm4gpt-2023.4.20.19.30.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/docs/installation.rst` & `llm4gpt-2023.4.20.19.30.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/docs/make.bat` & `llm4gpt-2023.4.20.19.30.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/llm/chatllm.py` & `llm4gpt-2023.4.20.19.30.9/llm/chatllm.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/llm/clis/cli.py` & `llm4gpt-2023.4.20.19.30.9/llm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/llm/kb/FaissANN.py` & `llm4gpt-2023.4.20.19.30.9/llm/kb/FaissANN.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/llm/qa.py` & `llm4gpt-2023.4.20.19.30.9/llm/qa.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/llm/utils.py` & `llm4gpt-2023.4.20.19.30.9/llm/utils.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/llm4gpt.egg-info/PKG-INFO` & `llm4gpt-2023.4.20.19.30.9/llm4gpt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.20.19.18.41
+Version: 2023.4.20.19.30.9
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -76,17 +76,17 @@
 
 - [x] 增加本地知识库组件
 
 - [ ] 增加互联网搜索组件
 
 - [ ] 增加知识图谱组件
 
--[ ] 增加微调模块
+- [ ] 增加微调模块
 
--[ ] 增加流式输出
+- [ ] 增加流式输出
 
 
 
 
 
 =======
 History
```

### Comparing `llm4gpt-2023.4.20.19.18.41/llm4gpt.egg-info/SOURCES.txt` & `llm4gpt-2023.4.20.19.30.9/llm4gpt.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -37,17 +37,14 @@
 llm/qa.py
 llm/utils.py
 llm/clis/README.md
 llm/clis/__init__.py
 llm/clis/cli.py
 llm/kb/FaissANN.py
 llm/kb/__init__.py
-llm/models/ChatLLM.py
-llm/models/__init__.py
-llm/models/gpt_service.py
 llm/uis/__init__.py
 llm4gpt.egg-info/PKG-INFO
 llm4gpt.egg-info/SOURCES.txt
 llm4gpt.egg-info/dependency_links.txt
 llm4gpt.egg-info/entry_points.txt
 llm4gpt.egg-info/not-zip-safe
 llm4gpt.egg-info/requires.txt
```

### Comparing `llm4gpt-2023.4.20.19.18.41/setup.py` & `llm4gpt-2023.4.20.19.30.9/setup.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.19.18.41/tests/test_llm4gpt.py` & `llm4gpt-2023.4.20.19.30.9/tests/test_llm4gpt.py`

 * *Files identical despite different names*

