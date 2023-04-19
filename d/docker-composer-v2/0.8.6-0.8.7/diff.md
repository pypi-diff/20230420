# Comparing `tmp/docker_composer_v2-0.8.6.tar.gz` & `tmp/docker_composer_v2-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_composer_v2-0.8.6.tar", max compression
+gzip compressed data, was "docker_composer_v2-0.8.7.tar", max compression
```

## Comparing `docker_composer_v2-0.8.6.tar` & `docker_composer_v2-0.8.7.tar`

### file list

```diff
@@ -1,66 +1,36 @@
--rwxr-xr-x   0        0        0    11358 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/LICENSE.txt
--rwxr-xr-x   0        0        0     2347 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/README.md
--rwxr-xr-x   0        0        0     1489 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/pyproject.toml
--rwxr-xr-x   0        0        0       60 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/__init__.py
--rwxr-xr-x   0        0        0        0 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/_utils/__init__.py
--rw-r--r--   0        0        0      184 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/_utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7902 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/_utils/__pycache__/argument.cpython-311.pyc
--rw-r--r--   0        0        0    14761 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/_utils/__pycache__/generate_class.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0    14876 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/_utils/__pycache__/generate_class.cpython-311.pyc
--rwxr-xr-x   0        0        0     4482 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/_utils/argument.py
--rwxr-xr-x   0        0        0     7724 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/_utils/generate_class.py
--rwxr-xr-x   0        0        0     3997 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/base.py
--rwxr-xr-x   0        0        0        0 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/py.typed
--rw-r--r--   0        0        0    36637 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/__pycache__/root.cpython-311.pyc
--rw-r--r--   0        0        0     1123 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/build.cpython-311.pyc
--rw-r--r--   0        0        0     1226 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     1243 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/cp.cpython-311.pyc
--rw-r--r--   0        0        0     1064 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/create.cpython-311.pyc
--rw-r--r--   0        0        0     1194 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/down.cpython-311.pyc
--rw-r--r--   0        0        0     1067 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/events.cpython-311.pyc
--rw-r--r--   0        0        0     1339 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/exec.cpython-311.pyc
--rw-r--r--   0        0        0     1135 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/images.cpython-311.pyc
--rw-r--r--   0        0        0     1124 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/kill.cpython-311.pyc
--rw-r--r--   0        0        0     1192 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/logs.cpython-311.pyc
--rw-r--r--   0        0        0     1097 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/ls.cpython-311.pyc
--rw-r--r--   0        0        0      936 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/pause.cpython-311.pyc
--rw-r--r--   0        0        0     1054 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/port.cpython-311.pyc
--rw-r--r--   0        0        0     1100 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/ps.cpython-311.pyc
--rw-r--r--   0        0        0     1123 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/pull.cpython-311.pyc
--rw-r--r--   0        0        0     1126 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/push.cpython-311.pyc
--rw-r--r--   0        0        0     1129 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/restart.cpython-311.pyc
--rw-r--r--   0        0        0     1413 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/rm.cpython-311.pyc
--rw-r--r--   0        0        0     1691 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/run.cpython-311.pyc
--rw-r--r--   0        0        0      936 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/start.cpython-311.pyc
--rw-r--r--   0        0        0     1016 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/stop.cpython-311.pyc
--rw-r--r--   0        0        0      944 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/top.cpython-311.pyc
--rw-r--r--   0        0        0      946 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/unpause.cpython-311.pyc
--rw-r--r--   0        0        0     1315 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/up.cpython-311.pyc
--rw-r--r--   0        0        0     1044 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0     1150 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/build.py
--rw-r--r--   0        0        0     1506 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/config.py
--rw-r--r--   0        0        0      923 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/cp.py
--rw-r--r--   0        0        0     1226 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/create.py
--rw-r--r--   0        0        0     1048 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/down.py
--rw-r--r--   0        0        0      606 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/events.py
--rw-r--r--   0        0        0     1236 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/exec.py
--rw-r--r--   0        0        0      695 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/images.py
--rw-r--r--   0        0        0      734 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/kill.py
--rw-r--r--   0        0        0     1157 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/logs.py
--rw-r--r--   0        0        0      799 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/ls.py
--rw-r--r--   0        0        0      461 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/pause.py
--rw-r--r--   0        0        0      674 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/port.py
--rw-r--r--   0        0        0     1069 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/ps.py
--rw-r--r--   0        0        0      869 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/pull.py
--rw-r--r--   0        0        0      826 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/push.py
--rw-r--r--   0        0        0      687 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/restart.py
--rw-r--r--   0        0        0     1012 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/rm.py
--rw-r--r--   0        0        0     2111 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/run.py
--rw-r--r--   0        0        0      461 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/start.py
--rw-r--r--   0        0        0      562 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/stop.py
--rw-r--r--   0        0        0      471 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/top.py
--rw-r--r--   0        0        0      469 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/unpause.py
--rw-r--r--   0        0        0     2979 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/up.py
--rw-r--r--   0        0        0      667 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/version.py
--rw-r--r--   0        0        0    25842 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/root.py
--rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 docker_composer_v2-0.8.6/PKG-INFO
+-rwxr-xr-x   0        0        0    11358 2023-04-19 22:25:00.981589 docker_composer_v2-0.8.7/LICENSE.txt
+-rwxr-xr-x   0        0        0     2356 2023-04-19 22:25:00.981589 docker_composer_v2-0.8.7/README.md
+-rwxr-xr-x   0        0        0     1492 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/pyproject.toml
+-rwxr-xr-x   0        0        0       60 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/_utils/__init__.py
+-rwxr-xr-x   0        0        0     4482 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/_utils/argument.py
+-rwxr-xr-x   0        0        0     7763 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/_utils/generate_class.py
+-rwxr-xr-x   0        0        0     3997 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/base.py
+-rwxr-xr-x   0        0        0        0 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/py.typed
+-rw-r--r--   0        0        0     1159 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/build.py
+-rw-r--r--   0        0        0     1515 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/config.py
+-rw-r--r--   0        0        0      932 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/cp.py
+-rw-r--r--   0        0        0     1235 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/create.py
+-rw-r--r--   0        0        0     1057 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/down.py
+-rw-r--r--   0        0        0      615 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/events.py
+-rw-r--r--   0        0        0     1245 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/exec.py
+-rw-r--r--   0        0        0      704 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/images.py
+-rw-r--r--   0        0        0      743 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/kill.py
+-rw-r--r--   0        0        0     1166 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/logs.py
+-rw-r--r--   0        0        0      808 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/ls.py
+-rw-r--r--   0        0        0      470 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/pause.py
+-rw-r--r--   0        0        0      683 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/port.py
+-rw-r--r--   0        0        0     1078 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/ps.py
+-rw-r--r--   0        0        0      878 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/pull.py
+-rw-r--r--   0        0        0      835 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/push.py
+-rw-r--r--   0        0        0      696 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/restart.py
+-rw-r--r--   0        0        0     1021 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/rm.py
+-rw-r--r--   0        0        0     2120 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/run.py
+-rw-r--r--   0        0        0      470 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/start.py
+-rw-r--r--   0        0        0      571 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/stop.py
+-rw-r--r--   0        0        0      480 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/top.py
+-rw-r--r--   0        0        0      478 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/unpause.py
+-rw-r--r--   0        0        0     2988 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/up.py
+-rw-r--r--   0        0        0      676 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/version.py
+-rw-r--r--   0        0        0    26076 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/root.py
+-rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 docker_composer_v2-0.8.7/PKG-INFO
```

### Comparing `docker_composer_v2-0.8.6/LICENSE.txt` & `docker_composer_v2-0.8.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.6/README.md` & `docker_composer_v2-0.8.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Docker Composer
+# Docker Composer V2
 
 A library to interact with `docker compose` (Compose V2) from a python Program.
 All commands and parameters are exposed as python classes and attributes
 to allow for full auto-completion of its parameters with IDEs
 that support it. 
 
 This project is based off the open source project: https://github.com/schollm/docker-composer
@@ -11,28 +11,28 @@
 
 ## Install
 ```shell script
 pip install docker-composer-v2
 ```
 
 ## Usage
-The main class is `docker_composer.DockerCompose`. Its parameters are
+The main class is `docker_compose_v2r.DockerCompose`. Its parameters are
 all options from `docker compose`.
 
 Each `docker compose` subcommand has a corresponding function, e.g. 
 `DockerCompose.run` or `DockerCompose.scale`. Their arguments again mirror 
 the options of the corresponding command.
 
 The resulting object has a `call` function. 
 It takes arbitrary strings as input, as well as all keyword arguments from 
 `subprocess.run`, and returns a `subprocess.CompletedProcess`
 
 ```python
 import os
-from docker_composer import DockerCompose
+from docker_composer_v2 import DockerCompose
 
 # set log level and verbose
 os.environ["DOCKER_COMPOSE_LOG_LEVEL"] = "info"
 # Set the logging level ("debug"|"info"|"warn"|"error"|"fatal") (default "info")
 
 base = DockerCompose(file="docker-compose.yml")
 base.run(detach=True, workdir="/tmp").call("app")
```

### Comparing `docker_composer_v2-0.8.6/pyproject.toml` & `docker_composer_v2-0.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "docker-composer-v2"
-version = "0.8.6"
+version = "0.8.7"
 description = "Use `docker compose` from within Python. This is a branch forked from https://github.com/schollm/docker-composer to support Docker Compose V2."
 authors = ["Micha <schollm-git@gmx.com>", "Jensen <jensen@kairosaerospace.com>"]
 readme = "README.md"
 homepage = "https://github.com/jensenkairos/docker-composer-v2"
 repository = "https://github.com/jensenkairos/docker-composer-v2"
 license = "Apache-2.0"
 packages = [
-    { include = "docker_composer", from = "src" },
+    { include = "docker_composer_v2", from = "src" },
 ]
 classifiers = [
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3",
   "Topic :: Software Development :: Build Tools",
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/_utils/argument.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/_utils/argument.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/_utils/generate_class.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/_utils/generate_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from typing import Iterable, Iterator, List, Mapping, Optional, Set, Tuple, Union
 
 import black
 import isort
 from isort.exceptions import ISortError
 from loguru import logger
 
-from docker_composer._utils.argument import Argument, parse_dc_argument
-from docker_composer.base import check_v2
+from docker_composer_v2._utils.argument import Argument, parse_dc_argument
+from docker_composer_v2.base import check_v2
 
 
 @lru_cache()
 def project_root():
     for path in Path(__file__).parents:
         if "pyproject.toml" in (p.name for p in path.iterdir()):
             logger.debug("Project Path root: {}", path)
@@ -132,17 +132,19 @@
         nl = level + 4
         sections, arguments = parse_help(docker_lines)
         args = ",".join(type_arg(arg)[0] for arg in arguments)
         arg_docs = "\n".join(
             f":param {arg.arg}: {arg.description}" for arg in arguments
         )
 
-        class_name = f"docker_composer.runner.cmd.{cmd}.DockerCompose{cmd.capitalize()}"
+        class_name = (
+            f"docker_composer_v2.runner.cmd.{cmd}.DockerCompose{cmd.capitalize()}"
+        )
         new_imports = [
-            f"import docker_composer.runner.cmd.{cmd}",
+            f"import docker_composer_v2.runner.cmd.{cmd}",
         ]
         yield f'''
 def {cmd}(self, {args}) -> {class_name}:
     """
 {indent(sections["general"], nl)}
 {indent(sections.get("usage", ""), nl)}
 {indent(arg_docs, nl)}
@@ -174,15 +176,15 @@
     res = indent(
         f'''
 # DO NOT EDIT: Autogenerated by {__file__}
 # for {_version()}
 
 import attr
 from typing import Optional, List
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 {new_line.join(add_imports)}
 
 @attr.s(auto_attribs=True)
 class {class_name}(DockerBaseRunner):
     """
 {indent(get_docstring(sections), level=nl)}
     """
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/base.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/base.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/build.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/build.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeBuild(DockerBaseRunner):
     """
 
     Usage:  docker compose build [OPTIONS] [SERVICE...]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/config.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeConfig(DockerBaseRunner):
     """
 
     Usage:  docker compose config [OPTIONS] [SERVICE...]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/cp.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/cp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeCp(DockerBaseRunner):
     """
 
     Usage:  docker compose cp [OPTIONS] SERVICE:SRC_PATH DEST_PATH|-
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/create.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/create.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeCreate(DockerBaseRunner):
     """
 
     Usage:  docker compose create [OPTIONS] [SERVICE...]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/down.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/down.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeDown(DockerBaseRunner):
     """
 
     Usage:  docker compose down [OPTIONS]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/events.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeEvents(DockerBaseRunner):
     """
 
     Usage:  docker compose events [OPTIONS] [SERVICE...]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/exec.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/exec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeExec(DockerBaseRunner):
     """
 
     Usage:  docker compose exec [OPTIONS] SERVICE COMMAND [ARGS...]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/images.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/restart.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposeImages(DockerBaseRunner):
+class DockerComposeRestart(DockerBaseRunner):
     """
 
-    Usage:  docker compose images [OPTIONS] [SERVICE...]
+    Usage:  docker compose restart [OPTIONS] [SERVICE...]
 
-    List images used by the created containers
+    Restart service containers
 
     """
 
-    format: Optional[str] = None
-    """Format the output. Values: [table | json].
-       (default "table")"""
-    quiet: Optional[bool] = None
-    """Only display IDs"""
-    _cmd: str = "images"
+    no_deps: Optional[bool] = None
+    """Don't restart dependent services."""
+    timeout: Optional[int] = None
+    """Specify a shutdown timeout in seconds (default 10)"""
+    _cmd: str = "restart"
     _options: List[str] = [
-        "quiet",
+        "no_deps",
     ]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/kill.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/kill.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeKill(DockerBaseRunner):
     """
 
     Usage:  docker compose kill [OPTIONS] [SERVICE...]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/logs.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeLogs(DockerBaseRunner):
     """
 
     Usage:  docker compose logs [OPTIONS] [SERVICE...]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/ls.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/ls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeLs(DockerBaseRunner):
     """
 
     Usage:  docker compose ls [OPTIONS]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/port.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/port.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposePort(DockerBaseRunner):
     """
 
     Usage:  docker compose port [OPTIONS] SERVICE PRIVATE_PORT
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/ps.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/ps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposePs(DockerBaseRunner):
     """
 
     Usage:  docker compose ps [OPTIONS] [SERVICE...]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/pull.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposePull(DockerBaseRunner):
     """
 
     Usage:  docker compose pull [OPTIONS] [SERVICE...]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/push.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/push.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposePush(DockerBaseRunner):
     """
 
     Usage:  docker compose push [OPTIONS] [SERVICE...]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/restart.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/rm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,37 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposeRestart(DockerBaseRunner):
+class DockerComposeRm(DockerBaseRunner):
     """
 
-    Usage:  docker compose restart [OPTIONS] [SERVICE...]
+    Usage:  docker compose rm [OPTIONS] [SERVICE...]
 
-    Restart service containers
+    Removes stopped service containers
+
+    By default, anonymous volumes attached to containers will not be removed. You
+    can override this with -v. To list all volumes, use "docker volume ls".
+
+    Any data which is not in a volume will be lost.
 
     """
 
-    no_deps: Optional[bool] = None
-    """Don't restart dependent services."""
-    timeout: Optional[int] = None
-    """Specify a shutdown timeout in seconds (default 10)"""
-    _cmd: str = "restart"
+    force: Optional[bool] = None
+    """Don't ask to confirm removal"""
+    stop: Optional[bool] = None
+    """Stop the containers, if required, before removing"""
+    volumes: Optional[bool] = None
+    """Remove any anonymous volumes attached to containers"""
+    _cmd: str = "rm"
     _options: List[str] = [
-        "no_deps",
+        "force",
+        "stop",
+        "volumes",
     ]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/run.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeRun(DockerBaseRunner):
     """
 
     Usage:  docker compose run [OPTIONS] SERVICE [COMMAND] [ARGS...]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/stop.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/stop.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeStop(DockerBaseRunner):
     """
 
     Usage:  docker compose stop [OPTIONS] [SERVICE...]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/up.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/up.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeUp(DockerBaseRunner):
     """
 
     Usage:  docker compose up [OPTIONS] [SERVICE...]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/version.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-from docker_composer.base import DockerBaseRunner
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeVersion(DockerBaseRunner):
     """
 
     Usage:  docker compose version [OPTIONS]
```

### Comparing `docker_composer_v2-0.8.6/src/docker_composer/runner/root.py` & `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/root.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer/src/docker_composer/_utils/generate_class.py
+# DO NOT EDIT: Autogenerated by /Users/jensen/kairos/docker-composer-v2/src/docker_composer_v2/_utils/generate_class.py
 # for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
-import docker_composer.runner.cmd.build
-import docker_composer.runner.cmd.config
-import docker_composer.runner.cmd.cp
-import docker_composer.runner.cmd.create
-import docker_composer.runner.cmd.down
-import docker_composer.runner.cmd.events
-import docker_composer.runner.cmd.exec
-import docker_composer.runner.cmd.images
-import docker_composer.runner.cmd.kill
-import docker_composer.runner.cmd.logs
-import docker_composer.runner.cmd.ls
-import docker_composer.runner.cmd.pause
-import docker_composer.runner.cmd.port
-import docker_composer.runner.cmd.ps
-import docker_composer.runner.cmd.pull
-import docker_composer.runner.cmd.push
-import docker_composer.runner.cmd.restart
-import docker_composer.runner.cmd.rm
-import docker_composer.runner.cmd.run
-import docker_composer.runner.cmd.start
-import docker_composer.runner.cmd.stop
-import docker_composer.runner.cmd.top
-import docker_composer.runner.cmd.unpause
-import docker_composer.runner.cmd.up
-import docker_composer.runner.cmd.version
-from docker_composer.base import DockerBaseRunner
+import docker_composer_v2.runner.cmd.build
+import docker_composer_v2.runner.cmd.config
+import docker_composer_v2.runner.cmd.cp
+import docker_composer_v2.runner.cmd.create
+import docker_composer_v2.runner.cmd.down
+import docker_composer_v2.runner.cmd.events
+import docker_composer_v2.runner.cmd.exec
+import docker_composer_v2.runner.cmd.images
+import docker_composer_v2.runner.cmd.kill
+import docker_composer_v2.runner.cmd.logs
+import docker_composer_v2.runner.cmd.ls
+import docker_composer_v2.runner.cmd.pause
+import docker_composer_v2.runner.cmd.port
+import docker_composer_v2.runner.cmd.ps
+import docker_composer_v2.runner.cmd.pull
+import docker_composer_v2.runner.cmd.push
+import docker_composer_v2.runner.cmd.restart
+import docker_composer_v2.runner.cmd.rm
+import docker_composer_v2.runner.cmd.run
+import docker_composer_v2.runner.cmd.start
+import docker_composer_v2.runner.cmd.stop
+import docker_composer_v2.runner.cmd.top
+import docker_composer_v2.runner.cmd.unpause
+import docker_composer_v2.runner.cmd.up
+import docker_composer_v2.runner.cmd.version
+from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeRoot(DockerBaseRunner):
     """
 
     Usage:  docker compose [OPTIONS] COMMAND
@@ -60,15 +60,15 @@
     project_name: Optional[str] = None
     """Project name"""
     _cmd: str = ""
     _options: List[str] = []
 
     def build(
         self, build_arg: Optional[str] = None, quiet: Optional[bool] = None
-    ) -> docker_composer.runner.cmd.build.DockerComposeBuild:
+    ) -> docker_composer_v2.runner.cmd.build.DockerComposeBuild:
         """
 
         Usage:  docker compose build [OPTIONS] [SERVICE...]
 
         Build or rebuild services
 
 
@@ -80,26 +80,26 @@
            the image.
            --push                    Push service images.
         :param quiet: Don't print anything to STDOUT
            --ssh string              Set SSH authentications used when
            building service images. (use 'default'
            for using your default SSH Agent)
         """
-        runner = docker_composer.runner.cmd.build.DockerComposeBuild(
+        runner = docker_composer_v2.runner.cmd.build.DockerComposeBuild(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def config(
         self,
         format: Optional[str] = None,
         output: Optional[str] = None,
         quiet: Optional[bool] = None,
-    ) -> docker_composer.runner.cmd.config.DockerComposeConfig:
+    ) -> docker_composer_v2.runner.cmd.config.DockerComposeConfig:
         """
 
         Usage:  docker compose config [OPTIONS] [SERVICE...]
 
         Parse, resolve and render compose file in canonical format
 
 
@@ -115,45 +115,45 @@
            --profiles                Print the profile names, one per line.
         :param quiet: Only validate the configuration, don't
            print anything.
            --resolve-image-digests   Pin image tags to digests.
            --services                Print the service names, one per line.
            --volumes                 Print the volume names, one per line.
         """
-        runner = docker_composer.runner.cmd.config.DockerComposeConfig(
+        runner = docker_composer_v2.runner.cmd.config.DockerComposeConfig(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def cp(
         self, archive: Optional[bool] = None, follow_link: Optional[bool] = None
-    ) -> docker_composer.runner.cmd.cp.DockerComposeCp:
+    ) -> docker_composer_v2.runner.cmd.cp.DockerComposeCp:
         """
 
         Usage:  docker compose cp [OPTIONS] SERVICE:SRC_PATH DEST_PATH|-
                 docker compose cp [OPTIONS] SRC_PATH|- SERVICE:DEST_PATH
 
         Copy files/folders between a service container and the local filesystem
 
 
         :param archive: Archive mode (copy all uid/gid information)
         :param follow_link: Always follow symbol link in SRC_PATH
            --index int     Index of the container if there are multiple
            instances of a service .
         """
-        runner = docker_composer.runner.cmd.cp.DockerComposeCp(
+        runner = docker_composer_v2.runner.cmd.cp.DockerComposeCp(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def create(
         self, build: Optional[bool] = None
-    ) -> docker_composer.runner.cmd.create.DockerComposeCreate:
+    ) -> docker_composer_v2.runner.cmd.create.DockerComposeCreate:
         """
 
         Usage:  docker compose create [OPTIONS] [SERVICE...]
 
         Creates containers for a service.
 
 
@@ -166,26 +166,26 @@
            --pull string      Pull image before running
            ("always"|"missing"|"never") (default "missing")
            --remove-orphans   Remove containers for services not defined in
            the Compose file.
            --scale scale      Scale SERVICE to NUM instances. Overrides the
            scale setting in the Compose file if present.
         """
-        runner = docker_composer.runner.cmd.create.DockerComposeCreate(
+        runner = docker_composer_v2.runner.cmd.create.DockerComposeCreate(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def down(
         self,
         remove_orphans: Optional[bool] = None,
         timeout: Optional[int] = None,
         volumes: Optional[str] = None,
-    ) -> docker_composer.runner.cmd.down.DockerComposeDown:
+    ) -> docker_composer_v2.runner.cmd.down.DockerComposeDown:
         """
 
         Usage:  docker compose down [OPTIONS]
 
         Stop and remove containers, networks
 
 
@@ -195,46 +195,46 @@
            only images that don't have a custom tag
            ("local"|"all")
         :param timeout: Specify a shutdown timeout in seconds (default 10)
         :param volumes: Remove named volumes declared in the volumes
            section of the Compose file and anonymous
            volumes attached to containers.
         """
-        runner = docker_composer.runner.cmd.down.DockerComposeDown(
+        runner = docker_composer_v2.runner.cmd.down.DockerComposeDown(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def events(
         self, json: Optional[bool] = None
-    ) -> docker_composer.runner.cmd.events.DockerComposeEvents:
+    ) -> docker_composer_v2.runner.cmd.events.DockerComposeEvents:
         """
 
         Usage:  docker compose events [OPTIONS] [SERVICE...]
 
         Receive real time events from containers.
 
 
         :param json: Output events as a stream of json objects
         """
-        runner = docker_composer.runner.cmd.events.DockerComposeEvents(
+        runner = docker_composer_v2.runner.cmd.events.DockerComposeEvents(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def exec(
         self,
         detach: Optional[bool] = None,
         env: Optional[str] = None,
         no_TTY: Optional[str] = None,
         user: Optional[str] = None,
         workdir: Optional[str] = None,
-    ) -> docker_composer.runner.cmd.exec.DockerComposeExec:
+    ) -> docker_composer_v2.runner.cmd.exec.DockerComposeExec:
         """
 
         Usage:  docker compose exec [OPTIONS] SERVICE COMMAND [ARGS...]
 
         Execute a command in a running container.
 
 
@@ -248,66 +248,66 @@
            default docker compose exec
            allocates a TTY. (default true)
            --privileged                   Give extended privileges to the process.
         :param user: Run the command as this user.
         :param workdir: Path to workdir directory for this
            command.
         """
-        runner = docker_composer.runner.cmd.exec.DockerComposeExec(
+        runner = docker_composer_v2.runner.cmd.exec.DockerComposeExec(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def images(
         self, format: Optional[str] = None, quiet: Optional[bool] = None
-    ) -> docker_composer.runner.cmd.images.DockerComposeImages:
+    ) -> docker_composer_v2.runner.cmd.images.DockerComposeImages:
         """
 
         Usage:  docker compose images [OPTIONS] [SERVICE...]
 
         List images used by the created containers
 
 
         :param format: Format the output. Values: [table | json].
            (default "table")
         :param quiet: Only display IDs
         """
-        runner = docker_composer.runner.cmd.images.DockerComposeImages(
+        runner = docker_composer_v2.runner.cmd.images.DockerComposeImages(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def kill(
         self, remove_orphans: Optional[bool] = None, signal: Optional[str] = None
-    ) -> docker_composer.runner.cmd.kill.DockerComposeKill:
+    ) -> docker_composer_v2.runner.cmd.kill.DockerComposeKill:
         """
 
         Usage:  docker compose kill [OPTIONS] [SERVICE...]
 
         Force stop service containers.
 
 
         :param remove_orphans: Remove containers for services not defined in
            the Compose file.
         :param signal: SIGNAL to send to the container. (default "SIGKILL")
         """
-        runner = docker_composer.runner.cmd.kill.DockerComposeKill(
+        runner = docker_composer_v2.runner.cmd.kill.DockerComposeKill(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def logs(
         self,
         follow: Optional[bool] = None,
         tail: Optional[str] = None,
         timestamps: Optional[bool] = None,
-    ) -> docker_composer.runner.cmd.logs.DockerComposeLogs:
+    ) -> docker_composer_v2.runner.cmd.logs.DockerComposeLogs:
         """
 
         Usage:  docker compose logs [OPTIONS] [SERVICE...]
 
         View output from containers
 
 
@@ -320,83 +320,83 @@
         :param tail: Number of lines to show from the end of the logs
            for each container. (default "all")
         :param timestamps: Show timestamps.
            --until string    Show logs before a timestamp (e.g.
            2013-01-02T13:23:37Z) or relative (e.g. 42m for
            42 minutes)
         """
-        runner = docker_composer.runner.cmd.logs.DockerComposeLogs(
+        runner = docker_composer_v2.runner.cmd.logs.DockerComposeLogs(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def ls(
         self, all: Optional[bool] = None, quiet: Optional[bool] = None
-    ) -> docker_composer.runner.cmd.ls.DockerComposeLs:
+    ) -> docker_composer_v2.runner.cmd.ls.DockerComposeLs:
         """
 
         Usage:  docker compose ls [OPTIONS]
 
         List running compose projects
 
 
         :param all: Show all stopped Compose projects
            --filter filter   Filter output based on conditions provided.
            --format string   Format the output. Values: [table | json].
            (default "table")
         :param quiet: Only display IDs.
         """
-        runner = docker_composer.runner.cmd.ls.DockerComposeLs(
+        runner = docker_composer_v2.runner.cmd.ls.DockerComposeLs(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def pause(
         self,
-    ) -> docker_composer.runner.cmd.pause.DockerComposePause:
+    ) -> docker_composer_v2.runner.cmd.pause.DockerComposePause:
         """
 
         Usage:  docker compose pause [SERVICE...]
 
         Pause services
 
 
 
         """
-        runner = docker_composer.runner.cmd.pause.DockerComposePause(
+        runner = docker_composer_v2.runner.cmd.pause.DockerComposePause(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def port(
         self, index: Optional[int] = None
-    ) -> docker_composer.runner.cmd.port.DockerComposePort:
+    ) -> docker_composer_v2.runner.cmd.port.DockerComposePort:
         """
 
         Usage:  docker compose port [OPTIONS] SERVICE PRIVATE_PORT
 
         Print the public port for a port binding.
 
 
         :param index: index of the container if service has multiple
            replicas (default 1)
            --protocol string   tcp or udp (default "tcp")
         """
-        runner = docker_composer.runner.cmd.port.DockerComposePort(
+        runner = docker_composer_v2.runner.cmd.port.DockerComposePort(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def ps(
         self, all: Optional[bool] = None, quiet: Optional[bool] = None
-    ) -> docker_composer.runner.cmd.ps.DockerComposePs:
+    ) -> docker_composer_v2.runner.cmd.ps.DockerComposePs:
         """
 
         Usage:  docker compose ps [OPTIONS] [SERVICE...]
 
         List containers
 
 
@@ -408,89 +408,89 @@
            (default "table")
         :param quiet: Only display IDs
            --services             Display services
            --status stringArray   Filter services by status. Values: [paused |
            restarting | removing | running | dead |
            created | exited]
         """
-        runner = docker_composer.runner.cmd.ps.DockerComposePs(
+        runner = docker_composer_v2.runner.cmd.ps.DockerComposePs(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def pull(
         self, ignore_buildable: Optional[bool] = None, quiet: Optional[bool] = None
-    ) -> docker_composer.runner.cmd.pull.DockerComposePull:
+    ) -> docker_composer_v2.runner.cmd.pull.DockerComposePull:
         """
 
         Usage:  docker compose pull [OPTIONS] [SERVICE...]
 
         Pull service images
 
 
         :param ignore_buildable: Ignore images that can be built.
            --ignore-pull-failures   Pull what it can and ignores images with
            pull failures.
            --include-deps           Also pull services declared as dependencies.
         :param quiet: Pull without printing progress information.
         """
-        runner = docker_composer.runner.cmd.pull.DockerComposePull(
+        runner = docker_composer_v2.runner.cmd.pull.DockerComposePull(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def push(
         self, ignore_push_failures: Optional[bool] = None, quiet: Optional[bool] = None
-    ) -> docker_composer.runner.cmd.push.DockerComposePush:
+    ) -> docker_composer_v2.runner.cmd.push.DockerComposePush:
         """
 
         Usage:  docker compose push [OPTIONS] [SERVICE...]
 
         Push service images
 
 
         :param ignore_push_failures: Push what it can and ignores images with
            push failures
            --include-deps           Also push images of services declared as
            dependencies
         :param quiet: Push without printing progress information
         """
-        runner = docker_composer.runner.cmd.push.DockerComposePush(
+        runner = docker_composer_v2.runner.cmd.push.DockerComposePush(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def restart(
         self, no_deps: Optional[bool] = None, timeout: Optional[int] = None
-    ) -> docker_composer.runner.cmd.restart.DockerComposeRestart:
+    ) -> docker_composer_v2.runner.cmd.restart.DockerComposeRestart:
         """
 
         Usage:  docker compose restart [OPTIONS] [SERVICE...]
 
         Restart service containers
 
 
         :param no_deps: Don't restart dependent services.
         :param timeout: Specify a shutdown timeout in seconds (default 10)
         """
-        runner = docker_composer.runner.cmd.restart.DockerComposeRestart(
+        runner = docker_composer_v2.runner.cmd.restart.DockerComposeRestart(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def rm(
         self,
         force: Optional[bool] = None,
         stop: Optional[bool] = None,
         volumes: Optional[bool] = None,
-    ) -> docker_composer.runner.cmd.rm.DockerComposeRm:
+    ) -> docker_composer_v2.runner.cmd.rm.DockerComposeRm:
         """
 
         Usage:  docker compose rm [OPTIONS] [SERVICE...]
 
         Removes stopped service containers
 
         By default, anonymous volumes attached to containers will not be removed. You
@@ -499,15 +499,15 @@
         Any data which is not in a volume will be lost.
 
 
         :param force: Don't ask to confirm removal
         :param stop: Stop the containers, if required, before removing
         :param volumes: Remove any anonymous volumes attached to containers
         """
-        runner = docker_composer.runner.cmd.rm.DockerComposeRm(
+        runner = docker_composer_v2.runner.cmd.rm.DockerComposeRm(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def run(
         self,
@@ -517,15 +517,15 @@
         interactive: Optional[bool] = None,
         label: Optional[str] = None,
         no_TTY: Optional[bool] = None,
         publish: Optional[str] = None,
         user: Optional[str] = None,
         volume: Optional[str] = None,
         workdir: Optional[str] = None,
-    ) -> docker_composer.runner.cmd.run.DockerComposeRun:
+    ) -> docker_composer_v2.runner.cmd.run.DockerComposeRun:
         """
 
         Usage:  docker compose run [OPTIONS] SERVICE [COMMAND] [ARGS...]
 
         Run a one-off command on a service.
 
 
@@ -550,99 +550,99 @@
            enabled and mapped to the host.
            --use-aliases           Use the service's network useAliases in the
            network(s) the container connects to.
         :param user: Run as specified username or uid
         :param volume: Bind mount a volume.
         :param workdir: Working directory inside the container
         """
-        runner = docker_composer.runner.cmd.run.DockerComposeRun(
+        runner = docker_composer_v2.runner.cmd.run.DockerComposeRun(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def start(
         self,
-    ) -> docker_composer.runner.cmd.start.DockerComposeStart:
+    ) -> docker_composer_v2.runner.cmd.start.DockerComposeStart:
         """
 
         Usage:  docker compose start [SERVICE...]
 
         Start services
 
 
 
         """
-        runner = docker_composer.runner.cmd.start.DockerComposeStart(
+        runner = docker_composer_v2.runner.cmd.start.DockerComposeStart(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def stop(
         self, timeout: Optional[int] = None
-    ) -> docker_composer.runner.cmd.stop.DockerComposeStop:
+    ) -> docker_composer_v2.runner.cmd.stop.DockerComposeStop:
         """
 
         Usage:  docker compose stop [OPTIONS] [SERVICE...]
 
         Stop services
 
 
         :param timeout: Specify a shutdown timeout in seconds (default 10)
         """
-        runner = docker_composer.runner.cmd.stop.DockerComposeStop(
+        runner = docker_composer_v2.runner.cmd.stop.DockerComposeStop(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def top(
         self,
-    ) -> docker_composer.runner.cmd.top.DockerComposeTop:
+    ) -> docker_composer_v2.runner.cmd.top.DockerComposeTop:
         """
 
         Usage:  docker compose top [SERVICES...]
 
         Display the running processes
 
 
 
         """
-        runner = docker_composer.runner.cmd.top.DockerComposeTop(
+        runner = docker_composer_v2.runner.cmd.top.DockerComposeTop(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def unpause(
         self,
-    ) -> docker_composer.runner.cmd.unpause.DockerComposeUnpause:
+    ) -> docker_composer_v2.runner.cmd.unpause.DockerComposeUnpause:
         """
 
         Usage:  docker compose unpause [SERVICE...]
 
         Unpause services
 
 
 
         """
-        runner = docker_composer.runner.cmd.unpause.DockerComposeUnpause(
+        runner = docker_composer_v2.runner.cmd.unpause.DockerComposeUnpause(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def up(
         self,
         abort_on_container_exit: Optional[bool] = None,
         detach: Optional[bool] = None,
         renew_anon_volumes: Optional[bool] = None,
         waitTimeout: Optional[int] = None,
-    ) -> docker_composer.runner.cmd.up.DockerComposeUp:
+    ) -> docker_composer_v2.runner.cmd.up.DockerComposeUp:
         """
 
         Usage:  docker compose up [OPTIONS] [SERVICE...]
 
         Create and start containers
 
 
@@ -688,32 +688,32 @@
            --wait-timeout int          timeout waiting for application to be
            running|healthy.
         :param waitTimeout: Use this waitTimeout in seconds for
            container shutdown when attached or
            when containers are already running.
            (default 10)
         """
-        runner = docker_composer.runner.cmd.up.DockerComposeUp(
+        runner = docker_composer_v2.runner.cmd.up.DockerComposeUp(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def version(
         self, format: Optional[str] = None
-    ) -> docker_composer.runner.cmd.version.DockerComposeVersion:
+    ) -> docker_composer_v2.runner.cmd.version.DockerComposeVersion:
         """
 
         Usage:  docker compose version [OPTIONS]
 
         Show the Docker Compose version information
 
 
         :param format: Format the output. Values: [pretty | json].
            (Default: pretty)
            --short           Shows only Compose's version number.
         """
-        runner = docker_composer.runner.cmd.version.DockerComposeVersion(
+        runner = docker_composer_v2.runner.cmd.version.DockerComposeVersion(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
```

### Comparing `docker_composer_v2-0.8.6/PKG-INFO` & `docker_composer_v2-0.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-composer-v2
-Version: 0.8.6
+Version: 0.8.7
 Summary: Use `docker compose` from within Python. This is a branch forked from https://github.com/schollm/docker-composer to support Docker Compose V2.
 Home-page: https://github.com/jensenkairos/docker-composer-v2
 License: Apache-2.0
 Author: Micha
 Author-email: schollm-git@gmx.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -23,15 +23,15 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: attrs (>=20.3.0,<21.0.0)
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Project-URL: Repository, https://github.com/jensenkairos/docker-composer-v2
 Description-Content-Type: text/markdown
 
-# Docker Composer
+# Docker Composer V2
 
 A library to interact with `docker compose` (Compose V2) from a python Program.
 All commands and parameters are exposed as python classes and attributes
 to allow for full auto-completion of its parameters with IDEs
 that support it. 
 
 This project is based off the open source project: https://github.com/schollm/docker-composer
@@ -40,28 +40,28 @@
 
 ## Install
 ```shell script
 pip install docker-composer-v2
 ```
 
 ## Usage
-The main class is `docker_composer.DockerCompose`. Its parameters are
+The main class is `docker_compose_v2r.DockerCompose`. Its parameters are
 all options from `docker compose`.
 
 Each `docker compose` subcommand has a corresponding function, e.g. 
 `DockerCompose.run` or `DockerCompose.scale`. Their arguments again mirror 
 the options of the corresponding command.
 
 The resulting object has a `call` function. 
 It takes arbitrary strings as input, as well as all keyword arguments from 
 `subprocess.run`, and returns a `subprocess.CompletedProcess`
 
 ```python
 import os
-from docker_composer import DockerCompose
+from docker_composer_v2 import DockerCompose
 
 # set log level and verbose
 os.environ["DOCKER_COMPOSE_LOG_LEVEL"] = "info"
 # Set the logging level ("debug"|"info"|"warn"|"error"|"fatal") (default "info")
 
 base = DockerCompose(file="docker-compose.yml")
 base.run(detach=True, workdir="/tmp").call("app")
```

