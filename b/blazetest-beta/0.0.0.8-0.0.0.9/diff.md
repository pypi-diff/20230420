# Comparing `tmp/blazetest-beta-0.0.0.8.tar.gz` & `tmp/blazetest-beta-0.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blazetest-beta-0.0.0.8.tar", last modified: Thu Feb  2 12:41:46 2023, max compression
+gzip compressed data, was "blazetest-beta-0.0.0.9.tar", last modified: Thu Feb  2 14:38:40 2023, max compression
```

## Comparing `blazetest-beta-0.0.0.8.tar` & `blazetest-beta-0.0.0.9.tar`

### file list

```diff
@@ -1,39 +1,37 @@
-drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 12:41:46.905719 blazetest-beta-0.0.0.8/
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      277 2023-01-22 00:42:45.000000 blazetest-beta-0.0.0.8/MANIFEST.in
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      126 2023-02-02 12:41:46.905719 blazetest-beta-0.0.0.8/PKG-INFO
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     5052 2022-12-23 16:33:54.000000 blazetest-beta-0.0.0.8/README.md
-drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 12:41:46.901719 blazetest-beta-0.0.0.8/blazetest/
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      442 2023-01-24 15:20:47.000000 blazetest-beta-0.0.0.8/blazetest/Dockerfile
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)       24 2023-02-02 12:41:40.000000 blazetest-beta-0.0.0.8/blazetest/__init__.py
-drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 12:41:46.905719 blazetest-beta-0.0.0.8/blazetest/core/
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)        0 2022-12-20 15:32:59.000000 blazetest-beta-0.0.0.8/blazetest/core/__init__.py
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     1283 2023-01-29 02:29:45.000000 blazetest-beta-0.0.0.8/blazetest/core/config.py
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      452 2023-01-24 15:20:47.000000 blazetest-beta-0.0.0.8/blazetest/core/exceptions.py
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     2599 2023-01-30 21:05:08.000000 blazetest-beta-0.0.0.8/blazetest/core/lambda_config.py
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     4287 2023-02-02 12:32:00.000000 blazetest-beta-0.0.0.8/blazetest/core/lambda_function.py
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     3827 2023-01-13 13:52:14.000000 blazetest-beta-0.0.0.8/blazetest/core/license_manager.py
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     1236 2023-01-30 21:13:43.000000 blazetest-beta-0.0.0.8/blazetest/core/logging_config.py
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     4667 2023-01-30 21:05:08.000000 blazetest-beta-0.0.0.8/blazetest/core/pulumi_manager.py
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     4300 2023-02-02 12:32:25.000000 blazetest-beta-0.0.0.8/blazetest/core/tests_runner.py
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     4179 2023-01-30 21:05:08.000000 blazetest-beta-0.0.0.8/blazetest/core/utils.py
-drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 12:41:46.897719 blazetest-beta-0.0.0.8/blazetest/deployment/
-drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 12:41:46.905719 blazetest-beta-0.0.0.8/blazetest/deployment/aws/
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     1432 2023-01-16 22:31:06.000000 blazetest-beta-0.0.0.8/blazetest/deployment/aws/.envignore
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     7910 2023-01-25 09:23:17.000000 blazetest-beta-0.0.0.8/blazetest/deployment/aws/__main__.py
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)       38 2023-01-18 22:55:19.000000 blazetest-beta-0.0.0.8/blazetest/deployment/aws/requirements.txt
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     4919 2023-01-30 21:13:43.000000 blazetest-beta-0.0.0.8/blazetest/runner.py
-drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 12:41:46.905719 blazetest-beta-0.0.0.8/blazetest/scripts/
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      374 2023-01-15 17:55:41.000000 blazetest-beta-0.0.0.8/blazetest/scripts/install_chromedriver.sh
-drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 12:41:46.905719 blazetest-beta-0.0.0.8/blazetest/tests_runner_handler/
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)        0 2022-12-20 15:32:59.000000 blazetest-beta-0.0.0.8/blazetest/tests_runner_handler/__init__.py
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     1852 2023-01-16 21:26:31.000000 blazetest-beta-0.0.0.8/blazetest/tests_runner_handler/handler.py
-drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 12:41:46.905719 blazetest-beta-0.0.0.8/blazetest_beta.egg-info/
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      126 2023-02-02 12:41:46.000000 blazetest-beta-0.0.0.8/blazetest_beta.egg-info/PKG-INFO
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      892 2023-02-02 12:41:46.000000 blazetest-beta-0.0.0.8/blazetest_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)        1 2023-02-02 12:41:46.000000 blazetest-beta-0.0.0.8/blazetest_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)       57 2023-02-02 12:41:46.000000 blazetest-beta-0.0.0.8/blazetest_beta.egg-info/entry_points.txt
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      109 2023-02-02 12:41:46.000000 blazetest-beta-0.0.0.8/blazetest_beta.egg-info/requires.txt
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)       10 2023-02-02 12:41:46.000000 blazetest-beta-0.0.0.8/blazetest_beta.egg-info/top_level.txt
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)       90 2022-12-20 15:32:59.000000 blazetest-beta-0.0.0.8/pyproject.toml
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)       79 2023-02-02 12:41:46.905719 blazetest-beta-0.0.0.8/setup.cfg
--rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      946 2023-02-02 12:41:29.000000 blazetest-beta-0.0.0.8/setup.py
+drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 14:38:40.499502 blazetest-beta-0.0.0.9/
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      277 2023-01-22 00:42:45.000000 blazetest-beta-0.0.0.9/MANIFEST.in
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      126 2023-02-02 14:38:40.499502 blazetest-beta-0.0.0.9/PKG-INFO
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     5052 2022-12-23 16:33:54.000000 blazetest-beta-0.0.0.9/README.md
+drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 14:38:40.483502 blazetest-beta-0.0.0.9/blazetest/
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      442 2023-01-24 15:20:47.000000 blazetest-beta-0.0.0.9/blazetest/Dockerfile
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)       24 2023-02-02 14:38:30.000000 blazetest-beta-0.0.0.9/blazetest/__init__.py
+drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 14:38:40.495502 blazetest-beta-0.0.0.9/blazetest/core/
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)        0 2022-12-20 15:32:59.000000 blazetest-beta-0.0.0.9/blazetest/core/__init__.py
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     1244 2023-02-02 12:57:29.000000 blazetest-beta-0.0.0.9/blazetest/core/config.py
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      497 2023-02-02 14:19:38.000000 blazetest-beta-0.0.0.9/blazetest/core/exceptions.py
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     2599 2023-01-30 21:05:08.000000 blazetest-beta-0.0.0.9/blazetest/core/lambda_config.py
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     4287 2023-02-02 12:32:00.000000 blazetest-beta-0.0.0.9/blazetest/core/lambda_function.py
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     3827 2023-01-13 13:52:14.000000 blazetest-beta-0.0.0.9/blazetest/core/license_manager.py
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     1174 2023-02-02 14:36:37.000000 blazetest-beta-0.0.0.9/blazetest/core/logging_config.py
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     4621 2023-02-02 14:36:37.000000 blazetest-beta-0.0.0.9/blazetest/core/pulumi_manager.py
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     4300 2023-02-02 12:32:25.000000 blazetest-beta-0.0.0.9/blazetest/core/tests_runner.py
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     4181 2023-02-02 12:57:29.000000 blazetest-beta-0.0.0.9/blazetest/core/utils.py
+drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 14:38:40.483502 blazetest-beta-0.0.0.9/blazetest/deployment/
+drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 14:38:40.499502 blazetest-beta-0.0.0.9/blazetest/deployment/aws/
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     1432 2023-01-16 22:31:06.000000 blazetest-beta-0.0.0.9/blazetest/deployment/aws/.envignore
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     7687 2023-02-02 14:22:31.000000 blazetest-beta-0.0.0.9/blazetest/deployment/aws/__main__.py
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)       38 2023-01-18 22:55:19.000000 blazetest-beta-0.0.0.9/blazetest/deployment/aws/requirements.txt
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     4919 2023-01-30 21:13:43.000000 blazetest-beta-0.0.0.9/blazetest/runner.py
+drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 14:38:40.499502 blazetest-beta-0.0.0.9/blazetest/tests_runner_handler/
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)        0 2022-12-20 15:32:59.000000 blazetest-beta-0.0.0.9/blazetest/tests_runner_handler/__init__.py
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)     1852 2023-01-16 21:26:31.000000 blazetest-beta-0.0.0.9/blazetest/tests_runner_handler/handler.py
+drwxrwxr-x   0 reginaqueen  (1000) reginaqueen  (1000)        0 2023-02-02 14:38:40.499502 blazetest-beta-0.0.0.9/blazetest_beta.egg-info/
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      126 2023-02-02 14:38:40.000000 blazetest-beta-0.0.0.9/blazetest_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      850 2023-02-02 14:38:40.000000 blazetest-beta-0.0.0.9/blazetest_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)        1 2023-02-02 14:38:40.000000 blazetest-beta-0.0.0.9/blazetest_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)       57 2023-02-02 14:38:40.000000 blazetest-beta-0.0.0.9/blazetest_beta.egg-info/entry_points.txt
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      109 2023-02-02 14:38:40.000000 blazetest-beta-0.0.0.9/blazetest_beta.egg-info/requires.txt
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)       10 2023-02-02 14:38:40.000000 blazetest-beta-0.0.0.9/blazetest_beta.egg-info/top_level.txt
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)       90 2022-12-20 15:32:59.000000 blazetest-beta-0.0.0.9/pyproject.toml
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)       79 2023-02-02 14:38:40.503502 blazetest-beta-0.0.0.9/setup.cfg
+-rw-rw-r--   0 reginaqueen  (1000) reginaqueen  (1000)      946 2023-02-02 14:38:30.000000 blazetest-beta-0.0.0.9/setup.py
```

### Comparing `blazetest-beta-0.0.0.8/README.md` & `blazetest-beta-0.0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `blazetest-beta-0.0.0.8/blazetest/core/config.py` & `blazetest-beta-0.0.0.9/blazetest/core/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,10 +29,9 @@
     "nH95890EL80dl/OH/K5O+CYTaHrKJ+zUcY7MxLqsmCw==</Modulus><Exponent>"
     "AQAB</Exponent></RSAKeyValue>"
 )
 
 EXECUTABLE_FILES = [
     "tests_runner_handler/__init__.py",
     "tests_runner_handler/handler.py",
-    "scripts/install_chromedriver.sh",
     "Dockerfile",
 ]
```

### Comparing `blazetest-beta-0.0.0.8/blazetest/core/lambda_config.py` & `blazetest-beta-0.0.0.9/blazetest/core/lambda_config.py`

 * *Files identical despite different names*

### Comparing `blazetest-beta-0.0.0.8/blazetest/core/lambda_function.py` & `blazetest-beta-0.0.0.9/blazetest/core/lambda_function.py`

 * *Files identical despite different names*

### Comparing `blazetest-beta-0.0.0.8/blazetest/core/license_manager.py` & `blazetest-beta-0.0.0.9/blazetest/core/license_manager.py`

 * *Files identical despite different names*

### Comparing `blazetest-beta-0.0.0.8/blazetest/core/logging_config.py` & `blazetest-beta-0.0.0.9/blazetest/core/logging_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import sys
 import uuid
 
 import logging_loki
 
 from blazetest.core.config import LOKI_URL, CWD
 
 
@@ -16,30 +17,27 @@
     """
     Sets up basic logging.
     If stdout_enabled, stdout is shown to the user. Otherwise, saved to the file.
     If loki_api_key is provided, logs are sent to Loki.
     """
     level = logging.DEBUG if debug else logging.INFO
 
-    handlers = None
+    handlers = []
     if loki_api_key:
         logging_loki.emitter.LokiEmitter.level_tag = "level"
         handler = logging_loki.LokiHandler(
             url=LOKI_URL.format(loki_api_key=loki_api_key),
             tags={"service": "blazetest", "session_uuid": session_uuid},
             version="1",
         )
-        handlers = [handler]
+        handlers.append(handler)
 
     if stdout_enabled:
-        logging.basicConfig(
-            format="%(process)d-%(levelname)s-%(message)s",
-            level=level,
-            handlers=handlers,
-        )
+        handlers.append(logging.StreamHandler(stream=sys.stdout))
     else:
-        logging.basicConfig(
-            filename=os.path.join(CWD, "blazetest.log"),
-            format="%(process)d-%(levelname)s-%(message)s",
-            level=level,
-            handlers=handlers,
-        )
+        handlers.append(logging.FileHandler(filename=os.path.join(CWD, "blazetest.log")))
+
+    logging.basicConfig(
+        format="%(process)d-%(levelname)s-%(message)s",
+        level=level,
+        handlers=handlers,
+    )
```

### Comparing `blazetest-beta-0.0.0.8/blazetest/core/pulumi_manager.py` & `blazetest-beta-0.0.0.9/blazetest/core/pulumi_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,61 @@
 import logging
 import os
 import subprocess
+import sys
 from typing import Dict, List
 
 import yaml
 
 from blazetest.core.config import BUILD_FOLDER_PATH, DEFAULT_ENCODING
+from blazetest.core.exceptions import PulumiException
 
 logger = logging.getLogger(__name__)
 
 
-class CommandResult:
-    def __init__(
-        self, completed_process: subprocess.CompletedProcess, allowed_return_codes: List
-    ):
-        if completed_process.returncode not in allowed_return_codes:
-            raise Exception(
-                f"Pulumi error with return code {completed_process.returncode}, "
-                f"stdout: {completed_process.stdout.decode(DEFAULT_ENCODING)}"
-            )
-
-        self.stdout = completed_process.stdout.decode(DEFAULT_ENCODING)
-        logger.debug(self.stdout)
-
-
 class CommandExecutor:
     def __init__(self, executable: str, command: str, arguments: Dict):
         """
         :param executable:
             Executable service or module, for example: sam
         :param command:
             Command for the executable, for example: sam build
         :param arguments:
             Arguments needed to be added to the command
         """
         self.executable = executable
         self.command = command
         self.arguments: List = self.__join_arguments(arguments=arguments)
 
-    def execute_command(self, allowed_return_codes=None) -> CommandResult:
+    def execute_command(self, allowed_return_codes=None) -> int:
         if allowed_return_codes is None:
             allowed_return_codes = [0]
 
         logger.debug(
             f"Command: {self.executable} {self.command} {' '.join(self.arguments)}"
         )
-        return CommandResult(
-            subprocess.run(
+        try:
+            subprocess.check_call(
                 [
                     self.executable,
                     self.command,
                 ]
                 + self.arguments,
-                stdout=subprocess.PIPE,
-            ),
-            allowed_return_codes=allowed_return_codes,
-        )
+                stdout=sys.stdout,
+                stderr=subprocess.STDOUT,
+            )
+        except subprocess.CalledProcessError as process:
+            if process.returncode not in allowed_return_codes:
+                stdout = process.stdout.decode(DEFAULT_ENCODING)
+                logger.error(f"Pulumi error with return code {process.returncode}, stdout: {stdout}")
+                raise PulumiException(
+                    f"Pulumi error with return code {process.returncode}, "
+                    f"stdout: {stdout}"
+                )
+        return 0
 
     @staticmethod
     def __join_arguments(arguments: Dict) -> List:
         arguments_list = []
         for arg_key in arguments:
             arg_value = arguments[arg_key]
 
@@ -120,27 +116,27 @@
             arguments={
                 "--local": None,
             },
         )
 
     def __execute(
         self, command: str, arguments: Dict, allowed_return_codes=None
-    ) -> str:
+    ) -> int:
         if allowed_return_codes is None:
             allowed_return_codes = [0]
 
         command_executor = CommandExecutor(
             executable=self.EXECUTABLE,
             command=command,
             arguments=arguments,
         )
-        command_result: CommandResult = command_executor.execute_command(
+        command_result = command_executor.execute_command(
             allowed_return_codes=allowed_return_codes
         )
-        return command_result.stdout
+        return command_result
 
     def create_config_files(self):
         pulumi_yaml = {
             "name": "blazetest-aws",
             "runtime": {
                 "name": "python",
                 "options": {
```

### Comparing `blazetest-beta-0.0.0.8/blazetest/core/tests_runner.py` & `blazetest-beta-0.0.0.9/blazetest/core/tests_runner.py`

 * *Files identical despite different names*

### Comparing `blazetest-beta-0.0.0.8/blazetest/core/utils.py` & `blazetest-beta-0.0.0.9/blazetest/core/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     """Create a build folder and copy necessary files to it.
 
     The `__main__.py` file in the `deployment/aws` directory will also be copied
     to the build folder.
     """
     # Create build folder and necessary subdirectories
     Path(BUILD_FOLDER_PATH).mkdir(parents=True, exist_ok=True)
-    Path(os.path.join(BUILD_FOLDER_PATH, "scripts")).mkdir(parents=True, exist_ok=True)
+    # Path(os.path.join(BUILD_FOLDER_PATH, "scripts")).mkdir(parents=True, exist_ok=True)
     Path(os.path.join(BUILD_FOLDER_PATH, "tests_runner_handler")).mkdir(
         parents=True, exist_ok=True
     )
 
     # Create list of source-destination file pairs for the files in EXECUTABLE_FILES
     src_dst_pairs = [
         (os.path.join(PWD, file), os.path.join(BUILD_FOLDER_PATH, file))
```

### Comparing `blazetest-beta-0.0.0.8/blazetest/deployment/aws/.envignore` & `blazetest-beta-0.0.0.9/blazetest/deployment/aws/.envignore`

 * *Files identical despite different names*

### Comparing `blazetest-beta-0.0.0.8/blazetest/deployment/aws/__main__.py` & `blazetest-beta-0.0.0.9/blazetest/deployment/aws/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 import string
 from typing import Dict
 
 import pulumi
 import pulumi_aws as aws
 from pulumi_docker import DockerBuild, Image, ImageRegistry
 
-logger = logging.getLogger(__name__)
-
 ENVIGNORE = ".envignore"
 CWD: str = os.environ.get("PROJECT_CWD")
 BUILD_FOLDER_PATH = os.path.join(CWD, ".blazetest")
 DOCKER_FILE_PATH = os.path.join(BUILD_FOLDER_PATH, "Dockerfile")
 
 ECR_REPOSITORY_NAME = os.environ.get("ECR_REPOSITORY_NAME")
 S3_BUCKET = os.environ.get("S3_BUCKET")
@@ -217,20 +215,15 @@
     with open(ENVIGNORE, "r") as f:
         env_ignore = [line.strip() for line in f.readlines()]
 
     return {k: v for k, v in os.environ.items() if k not in env_ignore}
 
 
 if __name__ == "__main__":
-    logging.basicConfig(
-        level=logging.INFO,
-        format="%(asctime)s %(levelname)-8s %(message)s",
-    )
     environment_variables = get_env_vars()
-    logger.debug(f"Environment variables: {environment_variables}")
     workflow = Workflow(
         ecr_repository_name=ECR_REPOSITORY_NAME,
         s3_bucket_name=S3_BUCKET,
         stack_name=pulumi.get_stack(),
         env_vars=environment_variables,
     )
     workflow.deploy()
```

### Comparing `blazetest-beta-0.0.0.8/blazetest/runner.py` & `blazetest-beta-0.0.0.9/blazetest/runner.py`

 * *Files identical despite different names*

### Comparing `blazetest-beta-0.0.0.8/blazetest/tests_runner_handler/handler.py` & `blazetest-beta-0.0.0.9/blazetest/tests_runner_handler/handler.py`

 * *Files identical despite different names*

### Comparing `blazetest-beta-0.0.0.8/blazetest_beta.egg-info/SOURCES.txt` & `blazetest-beta-0.0.0.9/blazetest_beta.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 blazetest/core/logging_config.py
 blazetest/core/pulumi_manager.py
 blazetest/core/tests_runner.py
 blazetest/core/utils.py
 blazetest/deployment/aws/.envignore
 blazetest/deployment/aws/__main__.py
 blazetest/deployment/aws/requirements.txt
-blazetest/scripts/install_chromedriver.sh
 blazetest/tests_runner_handler/__init__.py
 blazetest/tests_runner_handler/handler.py
 blazetest_beta.egg-info/PKG-INFO
 blazetest_beta.egg-info/SOURCES.txt
 blazetest_beta.egg-info/dependency_links.txt
 blazetest_beta.egg-info/entry_points.txt
 blazetest_beta.egg-info/requires.txt
```

### Comparing `blazetest-beta-0.0.0.8/setup.py` & `blazetest-beta-0.0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.0.8"
+VERSION = "0.0.0.9"
 
 setup(
     name="blazetest-beta",
     version=VERSION,
     author="Abrorjon Ruziboev",
     author_email="abror.ruzibayev@gmail.com",
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
```

