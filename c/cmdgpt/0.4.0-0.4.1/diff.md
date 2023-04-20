# Comparing `tmp/cmdgpt-0.4.0.tar.gz` & `tmp/cmdgpt-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdgpt-0.4.0.tar", last modified: Thu Apr 20 12:14:10 2023, max compression
+gzip compressed data, was "cmdgpt-0.4.1.tar", last modified: Thu Apr 20 12:27:22 2023, max compression
```

## Comparing `cmdgpt-0.4.0.tar` & `cmdgpt-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:14:10.008402 cmdgpt-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-20 12:13:59.000000 cmdgpt-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-20 12:14:10.008402 cmdgpt-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-20 12:13:59.000000 cmdgpt-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:14:10.008402 cmdgpt-0.4.0/cmdgpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:13:59.000000 cmdgpt-0.4.0/cmdgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-20 12:13:59.000000 cmdgpt-0.4.0/cmdgpt/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-20 12:13:59.000000 cmdgpt-0.4.0/cmdgpt/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-20 12:13:59.000000 cmdgpt-0.4.0/cmdgpt/openai_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-20 12:13:59.000000 cmdgpt-0.4.0/cmdgpt/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-20 12:13:59.000000 cmdgpt-0.4.0/cmdgpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:14:10.008402 cmdgpt-0.4.0/cmdgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-20 12:14:09.000000 cmdgpt-0.4.0/cmdgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 12:14:09.000000 cmdgpt-0.4.0/cmdgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:14:09.000000 cmdgpt-0.4.0/cmdgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 12:14:09.000000 cmdgpt-0.4.0/cmdgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 12:14:09.000000 cmdgpt-0.4.0/cmdgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 12:14:09.000000 cmdgpt-0.4.0/cmdgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:14:10.008402 cmdgpt-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-20 12:13:59.000000 cmdgpt-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:22.734359 cmdgpt-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-20 12:27:12.000000 cmdgpt-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-20 12:27:22.734359 cmdgpt-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-20 12:27:12.000000 cmdgpt-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:22.734359 cmdgpt-0.4.1/cmdgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:12.000000 cmdgpt-0.4.1/cmdgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-20 12:27:12.000000 cmdgpt-0.4.1/cmdgpt/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-20 12:27:12.000000 cmdgpt-0.4.1/cmdgpt/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-20 12:27:12.000000 cmdgpt-0.4.1/cmdgpt/openai_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-20 12:27:12.000000 cmdgpt-0.4.1/cmdgpt/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-20 12:27:12.000000 cmdgpt-0.4.1/cmdgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:22.734359 cmdgpt-0.4.1/cmdgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-20 12:27:22.000000 cmdgpt-0.4.1/cmdgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 12:27:22.000000 cmdgpt-0.4.1/cmdgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:27:22.000000 cmdgpt-0.4.1/cmdgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 12:27:22.000000 cmdgpt-0.4.1/cmdgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 12:27:22.000000 cmdgpt-0.4.1/cmdgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 12:27:22.000000 cmdgpt-0.4.1/cmdgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:27:22.734359 cmdgpt-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-20 12:27:12.000000 cmdgpt-0.4.1/setup.py
```

### Comparing `cmdgpt-0.4.0/LICENSE` & `cmdgpt-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdgpt-0.4.0/PKG-INFO` & `cmdgpt-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdgpt
-Version: 0.4.0
+Version: 0.4.1
 Summary: Interact with the command line using natural language | 用自然语言操控命令行
 Home-page: https://github.com/MZhao-ouo/CMDGPT
 Author: MZhao
 Author-email: mzhao.ouo@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cmdgpt-0.4.0/README.md` & `cmdgpt-0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 你只需要填host即可，例如：
 ```sh
 cmdgpt --api_host "api.openai.com"
 ```
 
 ## 已知问题
 - 无法使用`cd`和`source`等命令。
-- Windows上的CMDGPT仅支持提供命令，无法执行命令。
 
 ## 本地调试
 1. Clone本仓库
 ```sh
 git clone https://github.com/MZhao-ouo/CMDGPT.git
 cd CMDGPT
 ```
```

### Comparing `cmdgpt-0.4.0/cmdgpt/functions.py` & `cmdgpt-0.4.1/cmdgpt/functions.py`

 * *Files identical despite different names*

### Comparing `cmdgpt-0.4.0/cmdgpt/main.py` & `cmdgpt-0.4.1/cmdgpt/main.py`

 * *Files identical despite different names*

### Comparing `cmdgpt-0.4.0/cmdgpt/openai_func.py` & `cmdgpt-0.4.1/cmdgpt/openai_func.py`

 * *Files identical despite different names*

### Comparing `cmdgpt-0.4.0/cmdgpt/presets.py` & `cmdgpt-0.4.1/cmdgpt/presets.py`

 * *Files identical despite different names*

### Comparing `cmdgpt-0.4.0/cmdgpt/utils.py` & `cmdgpt-0.4.1/cmdgpt/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         output_str = output_data.decode("utf-8")
         lines = output_str.splitlines(keepends=True)
         return lines
     
     
 def get_cmd_history(current_shell, user_home):
     cmd_history = ""
-    if "PowerShell" in current_shell:
+    if "CMD" in current_shell:
         return ""
     elif "zsh" in current_shell:
         history_filename = os.path.join(user_home, ".zsh_history")
         cmd_history_list = process_file(history_filename)[-17:-1]
         for _ in cmd_history_list:
             cmd_history += _[15:]
     else:
```

### Comparing `cmdgpt-0.4.0/cmdgpt.egg-info/PKG-INFO` & `cmdgpt-0.4.1/cmdgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdgpt
-Version: 0.4.0
+Version: 0.4.1
 Summary: Interact with the command line using natural language | 用自然语言操控命令行
 Home-page: https://github.com/MZhao-ouo/CMDGPT
 Author: MZhao
 Author-email: mzhao.ouo@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cmdgpt-0.4.0/setup.py` & `cmdgpt-0.4.1/setup.py`

 * *Files identical despite different names*

