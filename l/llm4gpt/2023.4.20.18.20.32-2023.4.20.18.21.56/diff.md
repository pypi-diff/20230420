# Comparing `tmp/llm4gpt-2023.4.20.18.20.32.tar.gz` & `tmp/llm4gpt-2023.4.20.18.21.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4gpt-2023.4.20.18.20.32.tar", last modified: Thu Apr 20 10:20:32 2023, max compression
+gzip compressed data, was "llm4gpt-2023.4.20.18.21.56.tar", last modified: Thu Apr 20 10:21:56 2023, max compression
```

## Comparing `llm4gpt-2023.4.20.18.20.32.tar` & `llm4gpt-2023.4.20.18.21.56.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:20:32.625940 llm4gpt-2023.4.20.18.20.32/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1206 2023-04-11 04:36:04.000000 llm4gpt-2023.4.20.18.20.32/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1370 2023-04-20 10:20:32.626039 llm4gpt-2023.4.20.18.20.32/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      553 2023-04-11 06:33:00.000000 llm4gpt-2023.4.20.18.20.32/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:20:32.622558 llm4gpt-2023.4.20.18.20.32/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      379 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-11 04:38:41.000000 llm4gpt-2023.4.20.18.20.32/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:20:32.623066 llm4gpt-2023.4.20.18.20.32/llm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/llm/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1783 2023-04-20 10:14:58.000000 llm4gpt-2023.4.20.18.20.32/llm/chatllm.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:20:32.623419 llm4gpt-2023.4.20.18.20.32/llm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/llm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/llm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/llm/clis/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:20:32.623780 llm4gpt-2023.4.20.18.20.32/llm/kb/
--rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-04-20 10:20:30.000000 llm4gpt-2023.4.20.18.20.32/llm/kb/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 08:50:43.000000 llm4gpt-2023.4.20.18.20.32/llm/kb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2316 2023-04-20 09:45:22.000000 llm4gpt-2023.4.20.18.20.32/llm/kb/source_service_.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:20:32.624133 llm4gpt-2023.4.20.18.20.32/llm/models/
--rw-r--r--   0 betterme   (501) staff       (20)     1387 2023-04-20 10:16:32.000000 llm4gpt-2023.4.20.18.20.32/llm/models/ChatLLM.py
--rw-r--r--   0 betterme   (501) staff       (20)       31 2023-04-20 09:44:52.000000 llm4gpt-2023.4.20.18.20.32/llm/models/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1693 2023-04-20 09:44:52.000000 llm4gpt-2023.4.20.18.20.32/llm/models/gpt_service.py
--rw-r--r--   0 betterme   (501) staff       (20)     2504 2023-04-20 10:20:30.000000 llm4gpt-2023.4.20.18.20.32/llm/qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:20:32.624255 llm4gpt-2023.4.20.18.20.32/llm/uis/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.20.18.20.32/llm/uis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2923 2023-04-20 09:28:23.000000 llm4gpt-2023.4.20.18.20.32/llm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:20:32.625398 llm4gpt-2023.4.20.18.20.32/llm4gpt.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     1370 2023-04-20 10:20:32.000000 llm4gpt-2023.4.20.18.20.32/llm4gpt.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      932 2023-04-20 10:20:32.000000 llm4gpt-2023.4.20.18.20.32/llm4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 10:20:32.000000 llm4gpt-2023.4.20.18.20.32/llm4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-20 10:20:32.000000 llm4gpt-2023.4.20.18.20.32/llm4gpt.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 10:20:32.000000 llm4gpt-2023.4.20.18.20.32/llm4gpt.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       18 2023-04-20 10:20:32.000000 llm4gpt-2023.4.20.18.20.32/llm4gpt.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-20 10:20:32.000000 llm4gpt-2023.4.20.18.20.32/llm4gpt.egg-info/top_level.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-20 10:16:04.000000 llm4gpt-2023.4.20.18.20.32/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-20 10:20:32.626365 llm4gpt-2023.4.20.18.20.32/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.20.18.20.32/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:20:32.625776 llm4gpt-2023.4.20.18.20.32/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.20.32/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:21:56.619608 llm4gpt-2023.4.20.18.21.56/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1206 2023-04-11 04:36:04.000000 llm4gpt-2023.4.20.18.21.56/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1370 2023-04-20 10:21:56.619694 llm4gpt-2023.4.20.18.21.56/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      553 2023-04-11 06:33:00.000000 llm4gpt-2023.4.20.18.21.56/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:21:56.616894 llm4gpt-2023.4.20.18.21.56/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      379 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-11 04:38:41.000000 llm4gpt-2023.4.20.18.21.56/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:21:56.617359 llm4gpt-2023.4.20.18.21.56/llm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/llm/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1783 2023-04-20 10:14:58.000000 llm4gpt-2023.4.20.18.21.56/llm/chatllm.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:21:56.617712 llm4gpt-2023.4.20.18.21.56/llm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/llm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/llm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/llm/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:21:56.617943 llm4gpt-2023.4.20.18.21.56/llm/kb/
+-rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-04-20 10:20:30.000000 llm4gpt-2023.4.20.18.21.56/llm/kb/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 08:50:43.000000 llm4gpt-2023.4.20.18.21.56/llm/kb/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:21:56.618303 llm4gpt-2023.4.20.18.21.56/llm/models/
+-rw-r--r--   0 betterme   (501) staff       (20)     1387 2023-04-20 10:20:57.000000 llm4gpt-2023.4.20.18.21.56/llm/models/ChatLLM.py
+-rw-r--r--   0 betterme   (501) staff       (20)       31 2023-04-20 09:44:52.000000 llm4gpt-2023.4.20.18.21.56/llm/models/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1693 2023-04-20 10:20:57.000000 llm4gpt-2023.4.20.18.21.56/llm/models/gpt_service.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 10:21:48.000000 llm4gpt-2023.4.20.18.21.56/llm/qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:21:56.618418 llm4gpt-2023.4.20.18.21.56/llm/uis/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.20.18.21.56/llm/uis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2923 2023-04-20 09:28:23.000000 llm4gpt-2023.4.20.18.21.56/llm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:21:56.619253 llm4gpt-2023.4.20.18.21.56/llm4gpt.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1370 2023-04-20 10:21:56.000000 llm4gpt-2023.4.20.18.21.56/llm4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      906 2023-04-20 10:21:56.000000 llm4gpt-2023.4.20.18.21.56/llm4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 10:21:56.000000 llm4gpt-2023.4.20.18.21.56/llm4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-20 10:21:56.000000 llm4gpt-2023.4.20.18.21.56/llm4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 10:21:56.000000 llm4gpt-2023.4.20.18.21.56/llm4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       18 2023-04-20 10:21:56.000000 llm4gpt-2023.4.20.18.21.56/llm4gpt.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-20 10:21:56.000000 llm4gpt-2023.4.20.18.21.56/llm4gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-20 10:16:04.000000 llm4gpt-2023.4.20.18.21.56/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-20 10:21:56.619983 llm4gpt-2023.4.20.18.21.56/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.20.18.21.56/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 10:21:56.619495 llm4gpt-2023.4.20.18.21.56/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.18.21.56/tox.ini
```

### Comparing `llm4gpt-2023.4.20.18.20.32/.gitignore` & `llm4gpt-2023.4.20.18.21.56/.gitignore`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/.travis.yml` & `llm4gpt-2023.4.20.18.21.56/.travis.yml`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/CONTRIBUTING.rst` & `llm4gpt-2023.4.20.18.21.56/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/LICENSE` & `llm4gpt-2023.4.20.18.21.56/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/Makefile` & `llm4gpt-2023.4.20.18.21.56/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/PKG-INFO` & `llm4gpt-2023.4.20.18.21.56/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.20.18.20.32
+Version: 2023.4.20.18.21.56
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.20.18.20.32/README.md` & `llm4gpt-2023.4.20.18.21.56/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/README.rst` & `llm4gpt-2023.4.20.18.21.56/README.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/docs/Makefile` & `llm4gpt-2023.4.20.18.21.56/docs/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/docs/conf.py` & `llm4gpt-2023.4.20.18.21.56/docs/conf.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/docs/installation.rst` & `llm4gpt-2023.4.20.18.21.56/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/docs/make.bat` & `llm4gpt-2023.4.20.18.21.56/docs/make.bat`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/llm/chatllm.py` & `llm4gpt-2023.4.20.18.21.56/llm/chatllm.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/llm/clis/cli.py` & `llm4gpt-2023.4.20.18.21.56/llm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/llm/kb/FaissANN.py` & `llm4gpt-2023.4.20.18.21.56/llm/kb/FaissANN.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/llm/models/ChatLLM.py` & `llm4gpt-2023.4.20.18.21.56/llm/models/ChatLLM.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/llm/models/gpt_service.py` & `llm4gpt-2023.4.20.18.21.56/llm/models/gpt_service.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/llm/qa.py` & `llm4gpt-2023.4.20.18.21.56/llm/qa.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
         """
 
         :param chatllm:
         """
         self.chatllm = chatllm
         self.document_prompt = document_prompt if document_prompt else self.default_document_prompt
 
-        assert faiss_ann
         self.faiss_ann = faiss_ann
 
     @property
     def default_document_prompt(self) -> PromptTemplate:
         prompt_template = """
         基于以下已知信息，简洁和专业的来回答用户的问题。
         如果无法从中得到答案，请说 "根据已知信息无法回答该问题" 或 "没有提供足够的相关信息"，不允许在答案中添加编造成分，答案请使用中文。
@@ -41,14 +40,16 @@
         问题:
         {question}
         """.strip()
 
         return PromptTemplate(template=prompt_template, input_variables=["context", "question"])
 
     def get_knowledge_based_answer(self, query, max_turns=3, top_k=4, **kwargs):
+        assert self.faiss_ann
+
         # 设置chatllm参数，# history会被储存？
         self.chatllm.set_chat_kwargs(**kwargs)
         self.chatllm.max_turns = max_turns
 
         llm_chain = RetrievalQA.from_llm(
             llm=self.chatllm,
             retriever=self.faiss_ann.as_retriever(search_kwargs={"k": top_k}),  # todo: 重复实例化优化
```

### Comparing `llm4gpt-2023.4.20.18.20.32/llm/utils.py` & `llm4gpt-2023.4.20.18.21.56/llm/utils.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/llm4gpt.egg-info/PKG-INFO` & `llm4gpt-2023.4.20.18.21.56/llm4gpt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.20.18.20.32
+Version: 2023.4.20.18.21.56
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.20.18.20.32/llm4gpt.egg-info/SOURCES.txt` & `llm4gpt-2023.4.20.18.21.56/llm4gpt.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 llm/qa.py
 llm/utils.py
 llm/clis/README.md
 llm/clis/__init__.py
 llm/clis/cli.py
 llm/kb/FaissANN.py
 llm/kb/__init__.py
-llm/kb/source_service_.py
 llm/models/ChatLLM.py
 llm/models/__init__.py
 llm/models/gpt_service.py
 llm/uis/__init__.py
 llm4gpt.egg-info/PKG-INFO
 llm4gpt.egg-info/SOURCES.txt
 llm4gpt.egg-info/dependency_links.txt
```

### Comparing `llm4gpt-2023.4.20.18.20.32/setup.py` & `llm4gpt-2023.4.20.18.21.56/setup.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.18.20.32/tests/test_llm4gpt.py` & `llm4gpt-2023.4.20.18.21.56/tests/test_llm4gpt.py`

 * *Files identical despite different names*

