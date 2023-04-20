# Comparing `tmp/raga-cli-0.0.5.tar.gz` & `tmp/raga-cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-cli-0.0.5.tar", last modified: Wed Mar 29 11:22:07 2023, max compression
+gzip compressed data, was "raga-cli-0.0.6.tar", last modified: Thu Apr 20 11:36:48 2023, max compression
```

## Comparing `raga-cli-0.0.5.tar` & `raga-cli-0.0.6.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-03-29 11:22:07.643594 raga-cli-0.0.5/
--rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-03-29 10:00:38.000000 raga-cli-0.0.5/.gitignore
--rw-r--r--   0 manabroy   (501) staff       (20)    11350 2022-12-29 10:54:27.000000 raga-cli-0.0.5/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-03-29 11:22:07.643303 raga-cli-0.0.5/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2022-12-29 10:49:04.000000 raga-cli-0.0.5/README.rst
--rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-03-29 11:21:49.000000 raga-cli-0.0.5/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-03-29 11:22:07.635515 raga-cli-0.0.5/raga_cli.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-03-29 11:22:07.000000 raga-cli-0.0.5/raga_cli.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      595 2023-03-29 11:22:07.000000 raga-cli-0.0.5/raga_cli.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-03-29 11:22:07.000000 raga-cli-0.0.5/raga_cli.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-03-29 11:22:07.000000 raga-cli-0.0.5/raga_cli.egg-info/entry_points.txt
--rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-03-29 11:22:07.000000 raga-cli-0.0.5/raga_cli.egg-info/requires.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-03-29 11:22:07.000000 raga-cli-0.0.5/raga_cli.egg-info/top_level.txt
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-03-29 11:22:07.636852 raga-cli-0.0.5/rc/
--rw-r--r--   0 manabroy   (501) staff       (20)      211 2023-03-24 05:33:27.000000 raga-cli-0.0.5/rc/_rc_version.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-03-29 11:22:07.637999 raga-cli-0.0.5/rc/cli/
--rw-r--r--   0 manabroy   (501) staff       (20)     3216 2023-03-29 09:28:56.000000 raga-cli-0.0.5/rc/cli/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-01-09 07:20:52.000000 raga-cli-0.0.5/rc/cli/command.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2055 2023-03-23 13:59:15.000000 raga-cli-0.0.5/rc/cli/parser.py
--rw-r--r--   0 manabroy   (501) staff       (20)     4816 2023-03-29 10:42:43.000000 raga-cli-0.0.5/rc/cli/utils.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-03-29 11:22:07.639203 raga-cli-0.0.5/rc/commands/
--rw-r--r--   0 manabroy   (501) staff       (20)     2085 2023-03-29 10:49:49.000000 raga-cli-0.0.5/rc/commands/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     3465 2023-03-29 11:21:53.000000 raga-cli-0.0.5/rc/commands/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)     6301 2023-03-29 10:31:23.000000 raga-cli-0.0.5/rc/commands/repo.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-03-23 15:06:29.000000 raga-cli-0.0.5/rc/exceptions.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-03-23 14:47:13.000000 raga-cli-0.0.5/rc/prompt.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-03-29 11:22:07.640255 raga-cli-0.0.5/rc/repo/
--rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-03-23 15:20:16.000000 raga-cli-0.0.5/rc/repo/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-03-23 13:57:35.000000 raga-cli-0.0.5/rc/repo/repo.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-03-29 11:22:07.640644 raga-cli-0.0.5/rc/stage/
--rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-03-23 14:59:27.000000 raga-cli-0.0.5/rc/stage/exceptions.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-03-29 11:22:07.642743 raga-cli-0.0.5/rc/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-03-29 10:54:53.000000 raga-cli-0.0.5/rc/utils/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-02-24 12:25:08.000000 raga-cli-0.0.5/rc/utils/auditLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-03-25 07:24:39.000000 raga-cli-0.0.5/rc/utils/fileLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)     4473 2023-03-29 05:22:55.000000 raga-cli-0.0.5/rc/utils/request.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-03-27 04:36:03.000000 raga-cli-0.0.5/rc/utils/sshKeyGen.py
--rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-03-23 14:24:47.000000 raga-cli-0.0.5/rc/version.py
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-03-29 11:22:07.643655 raga-cli-0.0.5/setup.cfg
--rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-03-23 13:58:11.000000 raga-cli-0.0.5/setup.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.829249 raga-cli-0.0.6/
+-rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.0.6/.gitignore
+-rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.0.6/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-20 11:36:48.828411 raga-cli-0.0.6/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.0.6/README.rst
+-rw-r--r--   0 manabroy   (501) staff       (20)     2504 2023-04-12 11:10:34.000000 raga-cli-0.0.6/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.820402 raga-cli-0.0.6/raga_cli.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-20 11:36:48.000000 raga-cli-0.0.6/raga_cli.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      612 2023-04-20 11:36:48.000000 raga-cli-0.0.6/raga_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-20 11:36:48.000000 raga-cli-0.0.6/raga_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-04-20 11:36:48.000000 raga-cli-0.0.6/raga_cli.egg-info/entry_points.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)     1029 2023-04-20 11:36:48.000000 raga-cli-0.0.6/raga_cli.egg-info/requires.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-04-20 11:36:48.000000 raga-cli-0.0.6/raga_cli.egg-info/top_level.txt
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.821416 raga-cli-0.0.6/rc/
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.822805 raga-cli-0.0.6/rc/cli/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/cli/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.0.6/rc/cli/command.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2074 2023-04-12 11:10:34.000000 raga-cli-0.0.6/rc/cli/parser.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9323 2023-04-20 11:09:18.000000 raga-cli-0.0.6/rc/cli/utils.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.824224 raga-cli-0.0.6/rc/commands/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3226 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/commands/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.0.6/rc/commands/list.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1735 2023-04-13 04:42:45.000000 raga-cli-0.0.6/rc/commands/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     7737 2023-04-13 09:14:16.000000 raga-cli-0.0.6/rc/commands/repo.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/exceptions.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/prompt.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.825804 raga-cli-0.0.6/rc/repo/
+-rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/repo/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     5050 2023-04-20 11:10:27.000000 raga-cli-0.0.6/rc/repo/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/repo/repo.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.826141 raga-cli-0.0.6/rc/stage/
+-rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/stage/exceptions.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.827789 raga-cli-0.0.6/rc/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/utils/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/utils/auditLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/utils/fileLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     6464 2023-04-19 07:04:43.000000 raga-cli-0.0.6/rc/utils/request.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/utils/sshKeyGen.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/version.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-04-20 11:36:48.829350 raga-cli-0.0.6/setup.cfg
+-rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.0.6/setup.py
```

### Comparing `raga-cli-0.0.5/.gitignore` & `raga-cli-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.5/LICENSE` & `raga-cli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.5/PKG-INFO` & `raga-cli-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.0.5/pyproject.toml` & `raga-cli-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raga-cli"
-version = "0.0.5"
+version = "0.0.6"
 description = "Git for data scientists - manage your code and data together"
 readme = "README.rst"
 requires-python = ">=3.7"
 keywords = [
     "data-science",
     "data-version-control",
     "machine-learning",
@@ -20,15 +20,16 @@
     "raga",
 ]
 license = { text = "Apache License 2.0" }
 authors = [{ name = "Manab Roy", email = "manabr@observancegroup.com" }]
 maintainers = [{ name = "Manab Roy", email = "support@observancegroup.com" }]
 dependencies = [
     "dvc==2.38.1",
-    "dvc_s3==2.21.0"
+    "dvc_s3==2.21.0",
+    "boto3==1.16.28"
 ]
 [project.optional-dependencies]
 azure = ["dvc-azure==2.20.5"]
 gdrive = ["dvc-gdrive==2.19.1"]
 gs = ["dvc-gs==2.20.0"]
 hdfs = ["dvc-hdfs==2.19.0"]
 oss = ["dvc-oss==2.19.0"]
```

### Comparing `raga-cli-0.0.5/raga_cli.egg-info/PKG-INFO` & `raga-cli-0.0.6/raga_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.0.5/raga_cli.egg-info/SOURCES.txt` & `raga-cli-0.0.6/raga_cli.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 setup.py
 raga_cli.egg-info/PKG-INFO
 raga_cli.egg-info/SOURCES.txt
 raga_cli.egg-info/dependency_links.txt
 raga_cli.egg-info/entry_points.txt
 raga_cli.egg-info/requires.txt
 raga_cli.egg-info/top_level.txt
-rc/_rc_version.py
 rc/exceptions.py
 rc/prompt.py
 rc/version.py
 rc/cli/__init__.py
 rc/cli/command.py
 rc/cli/parser.py
 rc/cli/utils.py
 rc/commands/get.py
+rc/commands/list.py
 rc/commands/put.py
 rc/commands/repo.py
 rc/repo/get.py
+rc/repo/put.py
 rc/repo/repo.py
 rc/stage/exceptions.py
 rc/utils/__init__.py
 rc/utils/auditLog.py
 rc/utils/fileLog.py
 rc/utils/request.py
 rc/utils/sshKeyGen.py
```

### Comparing `raga-cli-0.0.5/raga_cli.egg-info/requires.txt` & `raga-cli-0.0.6/raga_cli.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 dvc==2.38.1
 dvc_s3==2.21.0
+boto3==1.16.28
 
 [all]
 dvc[azure,gdrive,gs,hdfs,oss,s3,ssh,webdav,webhdfs]
 
 [azure]
 dvc-azure==2.20.5
```

### Comparing `raga-cli-0.0.5/rc/cli/__init__.py` & `raga-cli-0.0.6/rc/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import json
 import logging
 import os
 import subprocess
 from rc.cli.utils import get_repo
 from rc.utils.request import RctlValidRequestError, get_config_value_by_key, update_repo_lock
 from rc.utils import DEBUG
-
 logger = logging.getLogger(__name__)
 level = logging.INFO
-if DEBUG:
-    level = logging.DEBUG
-logging.basicConfig(level=level, format='%(asctime)s - %(levelname)s - %(message)s', datefmt='%d-%b-%y %H:%M:%S') 
 
+def log_setup(args = None):
+    if DEBUG:
+        level = logging.DEBUG
+        logging.basicConfig(level=level, format='%(asctime)s - %(levelname)s - %(message)s', datefmt='%d-%b-%y %H:%M:%S')     
+    if args:
+        if args.output:
+            level = logging.DEBUG
+            logging.basicConfig(level=level, format='%(asctime)s - %(levelname)s - %(message)s', datefmt='%d-%b-%y %H:%M:%S') 
 
+log_setup()
 class RctlParserError(Exception):
     """Base class for CLI parser errors."""
     def __init__(self):
         logger.error("Parser error")
         super().__init__("Parser error")
 
 class RctlValidReqError(Exception):
```

### Comparing `raga-cli-0.0.5/rc/cli/parser.py` & `raga-cli-0.0.6/rc/cli/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import argparse
 import logging
 
 from rc.commands import (
     get,
     put,
-    repo,    
+    repo,
+    list,    
 )
 
 from . import RctlParserError
 logger = logging.getLogger(__name__)
 
 COMMANDS = [
     repo,
     put,
-    get,    
+    get, 
+    list,  
 ]
 
 def _find_parser(parser, cmd_cls):
     defaults = parser._defaults
     if not cmd_cls or cmd_cls == defaults.get("func"):
         parser.print_help()
         raise RctlParserError
```

### Comparing `raga-cli-0.0.5/rc/commands/get.py` & `raga-cli-0.0.6/rc/commands/get.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,64 @@
 import argparse
 import logging
 from datetime import timedelta 
 from timeit import default_timer as timer
 import json
+from rc.cli import log_setup
 
 from rc.cli.command import CmdBase
-from rc.cli.utils import run_command_on_subprocess
+from rc.cli.utils import run_command_on_subprocess,branch_commit_checkout
 from rc.cli.utils import *
-from rc.utils.request import get_repo_commit_id
+from rc.utils.request import get_repo_commit_id, get_repository
 
 logger = logging.getLogger(__name__)
 
 class CmdGet(CmdBase):
     def __init__(self, args):
         super().__init__(args)
     def run(self):
+        log_setup(self.args)
         start = timer()
         repo = get_repo()
+        
+        tag = get_repository(repo)
+       
         version = self.args.version
         if not version:
             print("Files downloading...") 
             run_command_on_subprocess('git pull') 
-            run_command_on_subprocess('dvc pull -f') 
+            if tag == "dataset":
+                run_command_on_subprocess('dvc pull -f') 
             print("Files downloaded successfully") 
             logger.debug('DOWNLOAD TIME {0}'.format(timedelta(seconds=timer()-start))) 
-        else:
-            commit_id = get_repo_commit_id(json.dumps({"repo_name":repo, "version":version}))
-            
-            user_input = input("Are you sure you want to get it? [y/n]").lower()
-            if user_input == 'y':
-                print("Files downloading...") 
-                run_command_on_subprocess('git reset --hard {}'.format(commit_id)) 
-                run_command_on_subprocess('dvc pull -f') 
-                print("Files downloaded successfully") 
-                logger.debug('DOWNLOAD TIME {0}'.format(timedelta(seconds=timer()-start))) 
+        else:  
+            if tag == "model":
+                user_input = input("Are you sure you want to get it? [y/n]").lower()
+                if user_input == 'y':
+                    version = self.args.version
+                    commit = get_repo_commit_id(json.dumps({"repo_name":repo, "version":version}))
+
+                    run_command_on_subprocess('git reset --hard')
+                    run_command_on_subprocess('git checkout {0}'.format(commit['branch']))
+                    run_command_on_subprocess('git reset --hard {0}'.format(commit['commit_id']))
+                else:
+                    print("Please enter valid input")
             else:
-                print("Please enter valid input")
+                commit_id = get_repo_commit_id(json.dumps({"repo_name":repo, "version":version}))
+            
+                user_input = input("Are you sure you want to get it? [y/n]").lower()
+                if user_input == 'y':
+                    print("Files downloading...") 
+                    run_command_on_subprocess('git reset --hard {}'.format(commit_id['commit_id'])) 
+                    run_command_on_subprocess('dvc pull -f') 
+                    run_command_on_subprocess('git clean -df') 
+                    print("Files downloaded successfully") 
+                    logger.debug('DOWNLOAD TIME {0}'.format(timedelta(seconds=timer()-start))) 
+                else:
+                    print("Please enter valid input")
 
         return 0
 
 
 def add_parser(subparsers, parent_parser):
     REPO_HELP = "Get File or folder. Use: `rctl get`"
     REPO_DESCRIPTION = (
@@ -57,8 +76,18 @@
         "-v", 
         "--version", 
         nargs="?", 
         default=None,
         type=int,
         help="Repo commit version",
     )
+
+    repo_parser.add_argument(
+        "-o", 
+        "--output", 
+        type=bool, 
+        nargs='?',
+        const=True, 
+        default=False,
+        help="Output debug",
+    )
     repo_parser.set_defaults(func=CmdGet)
```

### Comparing `raga-cli-0.0.5/rc/commands/repo.py` & `raga-cli-0.0.6/rc/commands/repo.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 from datetime import timedelta
 import sys 
 from timeit import default_timer as timer
 import os, pwd
 
 from rc.cli.command import CmdBase
 from rc.cli.utils import run_command_on_subprocess, repo_name_valid, get_git_url
-from rc.utils.request import get_config_value_by_key, create_repository, create_repo_lock
-from rc.utils.sshKeyGen import ssh_key_set_up
-from rc.cli import RctlValidReqError
+from rc.utils.request import get_config_value_by_key, create_repository, create_repo_lock, get_repository
+from rc.cli import RctlValidReqError, log_setup
 
 logger = logging.getLogger(__name__)
    
  
 
 """
 ----------------------------
@@ -36,75 +35,98 @@
         self.CLOUD_STORAGE_LOCATION = f"s3://{self.CLOUD_STORAGE_BUCKET}/{self.CLOUD_STORAGE_DIR}"
         self.INITIAL_COMMIT = get_config_value_by_key('git_initial_commit')
         self.GIT_BRANCH = get_config_value_by_key('git_initial_branch')
         self.GIT_ORG = get_config_value_by_key('git_org')
         self.TAGS = {"dataset", "model"}
         self.created_by = pwd.getpwuid(os.getuid()).pw_name 
 
-    def run_repo_create_subprocesses(self,repo_name):     
+    def run_repo_create_subprocesses(self,repo_name, repo_tag):     
         logger.debug(f"Repository Name: {repo_name}")
-        
-        run_command_on_subprocess("gh config set git_protocol ssh")  
-        run_command_on_subprocess("gh repo create {0}/{1} --private --clone".format(self.GIT_ORG, repo_name))    
-        run_command_on_subprocess("dvc init", repo_name)    
-        run_command_on_subprocess("dvc remote add -d {0} {1}/{2} -f".format(self.CLOUD_STORAGE_BUCKET, self.CLOUD_STORAGE_LOCATION, repo_name), repo_name)           
-        run_command_on_subprocess("dvc remote modify {0} secret_access_key {1}".format(self.CLOUD_STORAGE_BUCKET, get_config_value_by_key('remote_storage_secret_key')), repo_name)         
-        run_command_on_subprocess("dvc remote modify {0} access_key_id {1}".format(self.CLOUD_STORAGE_BUCKET, get_config_value_by_key('remote_storage_access_key')), repo_name)        
-        run_command_on_subprocess("dvc config core.autostage true", repo_name)           
-        run_command_on_subprocess("git commit -m '{0}' -a".format(self.INITIAL_COMMIT), repo_name)    
-        run_command_on_subprocess("git branch -M {0}".format(self.GIT_BRANCH), repo_name)    
-        run_command_on_subprocess("git push --set-upstream origin {0}".format(self.GIT_BRANCH), repo_name)       
 
+        if repo_tag =="dataset":
+            run_command_on_subprocess("gh config set git_protocol ssh")  
+            run_command_on_subprocess("gh repo create {0}/{1} --private --clone".format(self.GIT_ORG, repo_name))    
+            run_command_on_subprocess("dvc init", repo_name)    
+            run_command_on_subprocess("dvc remote add -d {0} {1}/{2} -f".format(self.CLOUD_STORAGE_BUCKET, self.CLOUD_STORAGE_LOCATION, repo_name), repo_name)           
+            run_command_on_subprocess("dvc remote modify {0} secret_access_key {1}".format(self.CLOUD_STORAGE_BUCKET, get_config_value_by_key('remote_storage_secret_key')), repo_name)         
+            run_command_on_subprocess("dvc remote modify {0} access_key_id {1}".format(self.CLOUD_STORAGE_BUCKET, get_config_value_by_key('remote_storage_access_key')), repo_name)        
+            run_command_on_subprocess("dvc config core.autostage true", repo_name)           
+            run_command_on_subprocess("git commit -m '{0}' -a".format(self.INITIAL_COMMIT), repo_name)    
+            run_command_on_subprocess("git branch -M {0}".format(self.GIT_BRANCH), repo_name)    
+            run_command_on_subprocess("git push --set-upstream origin {0}".format(self.GIT_BRANCH), repo_name)   
+        if repo_tag == "model":
+            run_command_on_subprocess("gh config set git_protocol ssh")  
+            run_command_on_subprocess("gh repo create {0}/{1} --private --clone".format(self.GIT_ORG, repo_name)) 
+            run_command_on_subprocess("touch README.md", repo_name)      
+            run_command_on_subprocess("git add README.md", repo_name)      
+            run_command_on_subprocess("git commit -m '{0}' -a".format("Model repo init"), repo_name)  
+            run_command_on_subprocess("git branch -M {0}".format(self.GIT_BRANCH), repo_name)    
+            run_command_on_subprocess("git push --set-upstream origin {0}".format(self.GIT_BRANCH), repo_name)    
+
+    
     def create_repo(self, args):
         print("Repo creating...")   
         logger.debug(f"START CREATE REPO COMMAND")
         repository_name = args.name       
         repository_tag = args.tag  
         if repository_tag not in self.TAGS:
-            logger.error("'{0}' tag is not available. Please choice from {1}".format(repository_tag, self.TAGS))
+            logger.error("'{0}' tag is not available. Please select from {1}".format(repository_tag, self.TAGS))
             sys.exit(50)                      
-        self.run_repo_create_subprocesses(repository_name)
+        self.run_repo_create_subprocesses(repository_name, repository_tag)
+
         git_repo = get_git_url(repository_name)
-        s3_repo = "{1}/{2}".format(self.CLOUD_STORAGE_BUCKET, self.CLOUD_STORAGE_LOCATION, repository_name)    
-        req_body = json.dumps({
-            "repo_name":repository_name,
-            "tag":repository_tag,
-            "created_by":self.created_by,
-            "git_repo":git_repo.replace('\n', ''),
-            "remote_storage_url":s3_repo,
-        })
-        logger.debug(req_body)
+        if repository_tag == "dataset":
+            s3_repo = "{1}/{2}".format(self.CLOUD_STORAGE_BUCKET, self.CLOUD_STORAGE_LOCATION, repository_name)    
+            req_body = json.dumps({
+                "repo_name":repository_name,
+                "tag":repository_tag,
+                "created_by":self.created_by,
+                "git_repo":git_repo.replace('\n', ''),
+                "remote_storage_url":s3_repo,
+            })
+            logger.debug(req_body)
+        if repository_tag == "model":
+            req_body = json.dumps({
+                "repo_name":repository_name,
+                "tag":repository_tag,
+                "created_by":self.created_by,
+                "git_repo":git_repo.replace('\n', ''),
+            })
+            logger.debug(req_body)
 
         create_repository(req_body)
         create_repo_lock(json.dumps({"repo_name":repository_name, "user_name":self.created_by, "locked":False}))
 
         print("Repository has been created. `cd {}`".format(repository_name))    
         logger.debug(f"END CREATE REPO COMMAND")
 
     def clone_repo(self, args):
         start = timer()
         repository_name = args.name     
         print('Cloning...')
-        run_command_on_subprocess("gh repo clone {0}/{1}".format(self.GIT_ORG, repository_name), None, True)      
-        run_command_on_subprocess("dvc pull", repository_name, True) 
+        run_command_on_subprocess("gh repo clone {0}/{1}".format(self.GIT_ORG, repository_name), None, True)    
+        tag = get_repository(repository_name)
+        if tag == "dataset":
+            run_command_on_subprocess("dvc pull", repository_name, True) 
         print("Repository cloned successfully")
         end = timer()
         logger.debug('CLONE TIME {0}'.format(timedelta(seconds=end-start)))    
 
 
 class CmdRepo(CmdBase):
     def __init__(self, args):
         super().__init__(args)        
         if getattr(self.args, "name", None):
             self.args.name = self.args.name.lower()            
             repo_name_valid(self.args.name)
         else:
             raise RctlValidReqError("Error: Please provide a valid name, -n")
 class CmdRepoCreate(CmdRepo):
-    def run(self):     
+    def run(self):   
+        log_setup(self.args)  
         repo = RepoMain()        
         if self.args.create:
             repo.create_repo(self.args)
         if self.args.clone:
             repo.clone_repo(self.args)                                    
         return 0
 
@@ -149,9 +171,19 @@
 
     repo_parser.add_argument(
         "-tag", 
         "--tag", 
         nargs="?", 
         help="Tag of the repo",
     )
+
+    repo_parser.add_argument(
+        "-o", 
+        "--output", 
+        type=bool, 
+        nargs='?',
+        const=True, 
+        default=False,
+        help="Output debug",
+    )
     
     repo_parser.set_defaults(func=CmdRepoCreate)
```

### Comparing `raga-cli-0.0.5/rc/exceptions.py` & `raga-cli-0.0.6/rc/exceptions.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.5/rc/prompt.py` & `raga-cli-0.0.6/rc/prompt.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.5/rc/repo/get.py` & `raga-cli-0.0.6/rc/repo/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.5/rc/utils/__init__.py` & `raga-cli-0.0.6/rc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.5/rc/utils/sshKeyGen.py` & `raga-cli-0.0.6/rc/utils/sshKeyGen.py`

 * *Files identical despite different names*

