# Comparing `tmp/llm4gpt-2023.4.20.20.13.36.tar.gz` & `tmp/llm4gpt-2023.4.20.20.13.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4gpt-2023.4.20.20.13.36.tar", last modified: Thu Apr 20 12:13:36 2023, max compression
+gzip compressed data, was "llm4gpt-2023.4.20.20.13.57.tar", last modified: Thu Apr 20 12:13:57 2023, max compression
```

## Comparing `llm4gpt-2023.4.20.20.13.36.tar` & `llm4gpt-2023.4.20.20.13.57.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:36.953383 llm4gpt-2023.4.20.20.13.36/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4gpt-2023.4.20.20.13.36/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     2121 2023-04-20 12:13:36.953487 llm4gpt-2023.4.20.20.13.36/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4gpt-2023.4.20.20.13.36/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:36.934134 llm4gpt-2023.4.20.20.13.36/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:36.937845 llm4gpt-2023.4.20.20.13.36/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4gpt-2023.4.20.20.13.36/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4gpt-2023.4.20.20.13.36/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.20.13.36/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.20.13.36/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.20.13.36/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.20.13.36/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:36.949708 llm4gpt-2023.4.20.20.13.36/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4gpt-2023.4.20.20.13.36/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4gpt-2023.4.20.20.13.36/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4gpt-2023.4.20.20.13.36/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:36.950376 llm4gpt-2023.4.20.20.13.36/llm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/llm/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-04-20 12:07:40.000000 llm4gpt-2023.4.20.20.13.36/llm/chatllm.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:36.951070 llm4gpt-2023.4.20.20.13.36/llm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/llm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/llm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/llm/clis/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:36.951496 llm4gpt-2023.4.20.20.13.36/llm/kb/
--rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-04-20 10:20:30.000000 llm4gpt-2023.4.20.20.13.36/llm/kb/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4gpt-2023.4.20.20.13.36/llm/kb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4gpt-2023.4.20.20.13.36/llm/qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:36.951776 llm4gpt-2023.4.20.20.13.36/llm/uis/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.20.20.13.36/llm/uis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2923 2023-04-20 09:28:23.000000 llm4gpt-2023.4.20.20.13.36/llm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:36.952890 llm4gpt-2023.4.20.20.13.36/llm4gpt.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     2121 2023-04-20 12:13:36.000000 llm4gpt-2023.4.20.20.13.36/llm4gpt.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      988 2023-04-20 12:13:36.000000 llm4gpt-2023.4.20.20.13.36/llm4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 12:13:36.000000 llm4gpt-2023.4.20.20.13.36/llm4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-20 12:13:36.000000 llm4gpt-2023.4.20.20.13.36/llm4gpt.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 12:13:36.000000 llm4gpt-2023.4.20.20.13.36/llm4gpt.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       18 2023-04-20 12:13:36.000000 llm4gpt-2023.4.20.20.13.36/llm4gpt.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-20 12:13:36.000000 llm4gpt-2023.4.20.20.13.36/llm4gpt.egg-info/top_level.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-20 11:28:30.000000 llm4gpt-2023.4.20.20.13.36/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-20 12:13:36.953791 llm4gpt-2023.4.20.20.13.36/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.20.20.13.36/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:36.953217 llm4gpt-2023.4.20.20.13.36/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.36/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.720235 llm4gpt-2023.4.20.20.13.57/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4gpt-2023.4.20.20.13.57/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     2121 2023-04-20 12:13:57.720331 llm4gpt-2023.4.20.20.13.57/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4gpt-2023.4.20.20.13.57/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.711121 llm4gpt-2023.4.20.20.13.57/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.713259 llm4gpt-2023.4.20.20.13.57/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4gpt-2023.4.20.20.13.57/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4gpt-2023.4.20.20.13.57/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.20.13.57/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.20.13.57/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.20.13.57/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.20.13.57/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.717766 llm4gpt-2023.4.20.20.13.57/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4gpt-2023.4.20.20.13.57/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4gpt-2023.4.20.20.13.57/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4gpt-2023.4.20.20.13.57/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.718258 llm4gpt-2023.4.20.20.13.57/llm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/llm/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-04-20 12:07:40.000000 llm4gpt-2023.4.20.20.13.57/llm/chatllm.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.718644 llm4gpt-2023.4.20.20.13.57/llm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/llm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/llm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/llm/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.718882 llm4gpt-2023.4.20.20.13.57/llm/kb/
+-rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-04-20 10:20:30.000000 llm4gpt-2023.4.20.20.13.57/llm/kb/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4gpt-2023.4.20.20.13.57/llm/kb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4gpt-2023.4.20.20.13.57/llm/qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.719002 llm4gpt-2023.4.20.20.13.57/llm/uis/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.20.20.13.57/llm/uis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2923 2023-04-20 09:28:23.000000 llm4gpt-2023.4.20.20.13.57/llm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.719809 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     2121 2023-04-20 12:13:57.000000 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      988 2023-04-20 12:13:57.000000 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 12:13:57.000000 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-20 12:13:57.000000 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 12:13:57.000000 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       18 2023-04-20 12:13:57.000000 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-20 12:13:57.000000 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-20 11:28:30.000000 llm4gpt-2023.4.20.20.13.57/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-20 12:13:57.720635 llm4gpt-2023.4.20.20.13.57/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.20.20.13.57/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.720096 llm4gpt-2023.4.20.20.13.57/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/tox.ini
```

### Comparing `llm4gpt-2023.4.20.20.13.36/.gitignore` & `llm4gpt-2023.4.20.20.13.57/.gitignore`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/.travis.yml` & `llm4gpt-2023.4.20.20.13.57/.travis.yml`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/CONTRIBUTING.rst` & `llm4gpt-2023.4.20.20.13.57/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/LICENSE` & `llm4gpt-2023.4.20.20.13.57/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/Makefile` & `llm4gpt-2023.4.20.20.13.57/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/PKG-INFO` & `llm4gpt-2023.4.20.20.13.57/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.20.20.13.36
+Version: 2023.4.20.20.13.57
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.20.20.13.36/README.md` & `llm4gpt-2023.4.20.20.13.57/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/README.rst` & `llm4gpt-2023.4.20.20.13.57/README.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/data/医/500种中药现代研究.txt` & `llm4gpt-2023.4.20.20.13.57/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/data/医/古今医统大全.txt` & `llm4gpt-2023.4.20.20.13.57/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/data/姚明.txt` & `llm4gpt-2023.4.20.20.13.57/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/data/王治郅.txt` & `llm4gpt-2023.4.20.20.13.57/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/data/科比.txt` & `llm4gpt-2023.4.20.20.13.57/data/科比.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/docs/Makefile` & `llm4gpt-2023.4.20.20.13.57/docs/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/docs/README.md` & `llm4gpt-2023.4.20.20.13.57/docs/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/docs/conf.py` & `llm4gpt-2023.4.20.20.13.57/docs/conf.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/docs/img.png` & `llm4gpt-2023.4.20.20.13.57/docs/img.png`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/docs/installation.rst` & `llm4gpt-2023.4.20.20.13.57/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/docs/make.bat` & `llm4gpt-2023.4.20.20.13.57/docs/make.bat`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/llm/chatllm.py` & `llm4gpt-2023.4.20.20.13.57/llm/chatllm.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/llm/clis/cli.py` & `llm4gpt-2023.4.20.20.13.57/llm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/llm/kb/FaissANN.py` & `llm4gpt-2023.4.20.20.13.57/llm/kb/FaissANN.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/llm/qa.py` & `llm4gpt-2023.4.20.20.13.57/llm/qa.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/llm/utils.py` & `llm4gpt-2023.4.20.20.13.57/llm/utils.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/llm4gpt.egg-info/PKG-INFO` & `llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.20.20.13.36
+Version: 2023.4.20.20.13.57
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.20.20.13.36/llm4gpt.egg-info/SOURCES.txt` & `llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/setup.py` & `llm4gpt-2023.4.20.20.13.57/setup.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.36/tests/test_llm4gpt.py` & `llm4gpt-2023.4.20.20.13.57/tests/test_llm4gpt.py`

 * *Files identical despite different names*

