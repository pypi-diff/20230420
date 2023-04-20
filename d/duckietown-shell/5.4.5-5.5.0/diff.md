# Comparing `tmp/duckietown-shell-5.4.5.tar.gz` & `tmp/duckietown-shell-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckietown-shell-5.4.5.tar", last modified: Sun Dec 18 07:10:33 2022, max compression
+gzip compressed data, was "duckietown-shell-5.5.0.tar", last modified: Thu Apr 20 04:24:53 2023, max compression
```

## Comparing `duckietown-shell-5.4.5.tar` & `duckietown-shell-5.5.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-12-18 07:10:33.100383 duckietown-shell-5.4.5/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    75933 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/LICENSE.pdf
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2022-12-18 07:10:33.100383 duckietown-shell-5.4.5/PKG-INFO
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-12-18 07:10:33.096383 duckietown-shell-5.4.5/lib/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-12-18 07:10:33.100383 duckietown-shell-5.4.5/lib/dt_shell/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1128 2022-12-18 07:10:31.000000 duckietown-shell-5.4.5/lib/dt_shell/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    12772 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/cli.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1306 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/cli_options.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1694 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/col_logging.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5550 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/commands_.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4285 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/config.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      889 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/constants.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2984 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/dt_command_abs.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      201 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/dt_command_placeholder.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3835 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/duckietown_tokens.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4741 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/env_checks.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      683 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      664 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/logging.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5749 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/main.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2467 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/package_version_check.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1994 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/tokens_cli.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3239 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/utils.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4528 2022-11-29 22:47:08.000000 duckietown-shell-5.4.5/lib/dt_shell/version_check.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2022-12-18 07:10:33.100383 duckietown-shell-5.4.5/lib/duckietown_shell.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2022-12-18 07:10:33.000000 duckietown-shell-5.4.5/lib/duckietown_shell.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      825 2022-12-18 07:10:33.000000 duckietown-shell-5.4.5/lib/duckietown_shell.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2022-12-18 07:10:33.000000 duckietown-shell-5.4.5/lib/duckietown_shell.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       43 2022-12-18 07:10:33.000000 duckietown-shell-5.4.5/lib/duckietown_shell.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2022-12-13 02:38:04.000000 duckietown-shell-5.4.5/lib/duckietown_shell.egg-info/not-zip-safe
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      249 2022-12-18 07:10:33.000000 duckietown-shell-5.4.5/lib/duckietown_shell.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        9 2022-12-18 07:10:33.000000 duckietown-shell-5.4.5/lib/duckietown_shell.egg-info/top_level.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2022-12-18 07:10:33.100383 duckietown-shell-5.4.5/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1990 2022-12-18 07:10:09.000000 duckietown-shell-5.4.5/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 04:24:53.536965 duckietown-shell-5.5.0/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    75933 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/LICENSE.pdf
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2023-04-20 04:24:53.536965 duckietown-shell-5.5.0/PKG-INFO
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 04:24:53.532965 duckietown-shell-5.5.0/lib/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 04:24:53.536965 duckietown-shell-5.5.0/lib/dt_shell/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1128 2023-04-20 04:24:24.000000 duckietown-shell-5.5.0/lib/dt_shell/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    13053 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/cli.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1306 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/cli_options.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1680 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/col_logging.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2307 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/commands_.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4291 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/config.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      895 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/constants.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2984 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/dt_command_abs.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      201 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/dt_command_placeholder.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3835 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/duckietown_tokens.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4741 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/env_checks.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      683 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      664 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/logging.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5530 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/main.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2467 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/package_version_check.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1994 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/tokens_cli.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4610 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/update_utils.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3239 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/utils.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4528 2023-04-19 20:12:13.000000 duckietown-shell-5.5.0/lib/dt_shell/version_check.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 04:24:53.536965 duckietown-shell-5.5.0/lib/duckietown_shell.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2023-04-20 04:24:53.000000 duckietown-shell-5.5.0/lib/duckietown_shell.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      854 2023-04-20 04:24:53.000000 duckietown-shell-5.5.0/lib/duckietown_shell.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-20 04:24:53.000000 duckietown-shell-5.5.0/lib/duckietown_shell.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       43 2023-04-20 04:24:53.000000 duckietown-shell-5.5.0/lib/duckietown_shell.egg-info/entry_points.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-20 04:24:53.000000 duckietown-shell-5.5.0/lib/duckietown_shell.egg-info/not-zip-safe
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      259 2023-04-20 04:24:53.000000 duckietown-shell-5.5.0/lib/duckietown_shell.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        9 2023-04-20 04:24:53.000000 duckietown-shell-5.5.0/lib/duckietown_shell.egg-info/top_level.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-20 04:24:53.536965 duckietown-shell-5.5.0/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2008 2023-04-20 04:21:42.000000 duckietown-shell-5.5.0/setup.py
```

### Comparing `duckietown-shell-5.4.5/LICENSE.pdf` & `duckietown-shell-5.5.0/LICENSE.pdf`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/__init__.py` & `duckietown-shell-5.5.0/lib/dt_shell/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional
 
 logging.basicConfig()
 
 dtslogger = logging.getLogger("dts")
 dtslogger.setLevel(logging.INFO)
 
-__version__ = "5.4.5"
+__version__ = "5.5.0"
 
 
 dtslogger.debug(f"duckietown-shell {__version__}")
 
 import sys
 
 if sys.version_info < (3, 6):
```

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/cli.py` & `duckietown-shell-5.5.0/lib/dt_shell/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from os.path import exists, isfile, join
 from typing import Mapping, Optional, Sequence, List
 
 from . import dtslogger
 from .commands_ import (
     _get_commands,
     _init_commands,
-    check_commands_outdated,
+    _ensure_commands_exist,
+    _ensure_commands_updated,
     InvalidRemote,
-    update_commands,
 )
 from .config import (
     get_config_path,
     RepoInfo,
     RepoInfo_for_version,
     ShellConfig,
     write_shell_config,
@@ -29,14 +29,17 @@
 from .dt_command_abs import DTCommandAbs
 from .dt_command_placeholder import DTCommandPlaceholder
 from .exceptions import CommandsLoadingException, UserError
 from .logging import dts_print
 from .version_check import check_if_outdated
 
 
+BILLBOARDS_VERSION: str = "v1"
+
+
 @dataclass
 class CommandsInfo:
     commands_path: str  # commands path
     leave_alone: bool  # whether to leave this alone (local)
 
 
 def get_local_commands_info() -> CommandsInfo:
@@ -101,14 +104,15 @@
         sys.path.insert(0, self.commands_path)
         # add third-party libraries dir to the path of this session
         sys.path.insert(0, os.path.join(self.commands_path, "lib"))
 
         # init commands
         cmds_just_initialized = False
 
+        # check if the commands path exists
         if exists(commands_path) and isfile(commands_path):
             remove(commands_path)
         if not exists(commands_path):
             msg = "I cannot find the command path %s" % commands_path
             if self.local_commands_info.leave_alone:
                 raise Exception(msg)
             dtslogger.warning(msg)
@@ -129,20 +133,20 @@
         # check for updates (if needed)
         # Do not check it if we are using custom commands_path_leave_alone
         if (
             not cmds_just_initialized
             and not self.local_commands_info.leave_alone
             and "update" not in sys.argv
         ):
-            check_commands_outdated(self.commands_path, self.repo_info)
+            self.update_commands()
 
         # show billboard (if any)
         billboard: Optional[str] = self.get_billboard()
         if billboard:
-            print(self.get_billboard())
+            print(billboard)
 
         self.reload_commands()
 
     def save_config(self):
         write_shell_config(self.shell_config)
 
     def postcmd(self, stop, line):
@@ -324,15 +328,16 @@
     def sprint(self, msg: str, color: Optional[str] = None, attrs: Sequence[str] = None) -> None:
         attrs = attrs or []
         return dts_print(msg=msg, color=color, attrs=attrs)
 
     @staticmethod
     def get_billboard() -> Optional[str]:
         # find billboards directory
-        billboard_dir: str = os.path.join(os.path.expanduser(DTShellConstants.ROOT), "billboards")
+        dts_dir: str = os.path.expanduser(DTShellConstants.ROOT)
+        billboard_dir: str = os.path.join(dts_dir, "billboards", BILLBOARDS_VERSION)
         if (not os.path.exists(billboard_dir)) or (not os.path.isdir(billboard_dir)):
             return None
         # get all sources of ads from the billboards directory
         sources: List[str] = os.listdir(billboard_dir)
         if len(sources) <= 0:
             return None
         # pick one source at random
@@ -343,15 +348,18 @@
         except:
             dtslogger.debug("Error occurred while loading billboard. Skipping...")
             return None
         # ---
         return content
 
     def update_commands(self) -> bool:
-        return update_commands(self.commands_path, self.repo_info)
+        # check that the repo is initialized in the commands path
+        _ensure_commands_exist(self.commands_path, self.repo_info)
+        # update the commands if they are outdated
+        return _ensure_commands_updated(self.commands_path, self.repo_info)
 
 
 def _touch(path: str) -> None:
     with open(path, "a"):
         utime(path, None)
```

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/cli_options.py` & `duckietown-shell-5.5.0/lib/dt_shell/cli_options.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/col_logging.py` & `duckietown-shell-5.5.0/lib/dt_shell/col_logging.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import logging
 
-__all__ = []
-
 
 def setup_logging_format():
     from logging import Logger, StreamHandler, Formatter
     import logging
 
     FORMAT = "%(name)15s|ds|%(filename)15s:%(lineno)-4s - %(funcName)-15s| %(message)s"
```

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/config.py` & `duckietown-shell-5.5.0/lib/dt_shell/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 @dataclass
 class ShellConfig:
     token_dt1: Optional[str]  ## key
     docker_username: Optional[str]
     docker_password: Optional[str]
-    duckietown_version: Optional[str]  # daffy, master19, ...
+    duckietown_version: Optional[str]  # ente, daffy, master19, ...
     docker_credentials: Dict[str, Dict[str, str]]  # username, secret
 
 
 @dataclass
 class RepoInfo:
     username: str
     project: str
```

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/constants.py` & `duckietown-shell-5.5.0/lib/dt_shell/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,22 @@
     CONFIG_DOCKER_CREDENTIALS = "docker_credentials"
 
 
 ALLOWED_BRANCHES = ["ente(-[\w]+)?", "daffy(-[\w]+)?", "master19(-[\w]+)?", "devel(-[\w]+)?"]
 
 DEBUG = False
 
-CHECK_CMDS_UPDATE_EVERY_MINS = 5
+CHECK_CMDS_UPDATE_MINS = 5
 
 DNAME = "Duckietown Shell"
 
 
 def INTRO(extra: Optional[str] = None) -> str:
     return """
 
-Welcome to the {Duckietown} ({version}).
+Welcome to the interactive {Duckietown} ({version}).
 {extra}
 Type "help" or "?" to list commands.
 
 """.format(
         Duckietown=termcolor.colored(DNAME, "yellow", attrs=["bold"]), version=__version__, extra=extra or ""
     ).lstrip()
```

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/dt_command_abs.py` & `duckietown-shell-5.5.0/lib/dt_shell/dt_command_abs.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/duckietown_tokens.py` & `duckietown-shell-5.5.0/lib/dt_shell/duckietown_tokens.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/env_checks.py` & `duckietown-shell-5.5.0/lib/dt_shell/env_checks.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/exceptions.py` & `duckietown-shell-5.5.0/lib/dt_shell/exceptions.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/logging.py` & `duckietown-shell-5.5.0/lib/dt_shell/logging.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/main.py` & `duckietown-shell-5.5.0/lib/dt_shell/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import os
 import re
 import sys
 from typing import Dict, Union
 
 import dt_shell
+import termcolor
 import yaml
 
 from . import __version__, dtslogger
 from .cli import DTShell, get_local_commands_info
 from .cli_options import get_cli_options
 from .config import get_shell_config_default, read_shell_config, write_shell_config
 from .constants import ALLOWED_BRANCHES
@@ -18,15 +19,15 @@
     CommandsLoadingException,
     ConfigInvalid,
     ConfigNotPresent,
     InvalidEnvironment,
     UserError,
 )
 from .logging import dts_print
-from .utils import format_exception, href, replace_spaces
+from .utils import format_exception, replace_spaces
 from .package_version_check import _get_installed_distributions
 
 
 class OtherVersions:
     name2versions: Dict[str, Union[str, Dict[str, str]]] = {}
 
 
@@ -101,49 +102,29 @@
         f.write(versions)
     msg = f"""\
 To report a bug, please also include the contents of {fn}
 """
     dts_print(msg, "red")
 
 
-def print_info_command() -> None:
-    url = href("https://github.com/duckietown/duckietown-shell-commands/issues")
-    msg = """
-
-    Problems with a command?
-
-    Report here: {url}
-
-    Troubleshooting:
-
-    - If some commands update fail, delete ~/.dt-shell/commands
-
-    - To reset the shell to "factory settings", delete ~/.dt-shell
-
-      (Note: you will have to re-configure.)
-
-        """.format(
-        url=url
-    )
-    dts_print(msg)
-
-
 def cli_main_() -> None:
     abort_if_running_with_sudo()
 
     # Problems with a step in the Duckiebot operation manual?
     #
     #     Report here: https://github.com/duckietown/docs-opmanual_duckiebot/issues
 
     # TODO: register handler for Ctrl-C
     cli_arguments = sys.argv[1:]
     cli_options, arguments = get_cli_options(cli_arguments)
 
     if not cli_options.quiet:
-        print_info_command()
+        print("{name} (v{version})".format(
+            name=termcolor.colored("Duckietown Shell", "yellow", attrs=["bold"]), version=__version__)
+        )
 
     # process options here
     if cli_options.debug:
         dtslogger.setLevel(logging.DEBUG)
 
     try:
         shell_config = read_shell_config()
@@ -166,14 +147,15 @@
     if v is not None:
         if not is_allowed_branch(v):
             allowed_braches = [b.split("(")[0] for b in ALLOWED_BRANCHES]
             msg = f"Given version {v!r} is not one of {allowed_braches}."
             raise UserError(msg)
         shell_config.duckietown_version = v
         write_shell_config(shell_config)
+        dtslogger.info(f"Configured dts to version: {shell_config.duckietown_version}\n")
         # need this so we can use in non-interactive settings
         sys.exit(0)
 
     if shell_config.duckietown_version is None:
         msg = """You have not specified a Duckietown version. Please use:
 
         dts --set-version <version>
```

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/package_version_check.py` & `duckietown-shell-5.5.0/lib/dt_shell/package_version_check.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/tokens_cli.py` & `duckietown-shell-5.5.0/lib/dt_shell/tokens_cli.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/utils.py` & `duckietown-shell-5.5.0/lib/dt_shell/utils.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.4.5/lib/dt_shell/version_check.py` & `duckietown-shell-5.5.0/lib/dt_shell/version_check.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.4.5/lib/duckietown_shell.egg-info/SOURCES.txt` & `duckietown-shell-5.5.0/lib/duckietown_shell.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 lib/dt_shell/duckietown_tokens.py
 lib/dt_shell/env_checks.py
 lib/dt_shell/exceptions.py
 lib/dt_shell/logging.py
 lib/dt_shell/main.py
 lib/dt_shell/package_version_check.py
 lib/dt_shell/tokens_cli.py
+lib/dt_shell/update_utils.py
 lib/dt_shell/utils.py
 lib/dt_shell/version_check.py
 lib/duckietown_shell.egg-info/PKG-INFO
 lib/duckietown_shell.egg-info/SOURCES.txt
 lib/duckietown_shell.egg-info/dependency_links.txt
 lib/duckietown_shell.egg-info/entry_points.txt
 lib/duckietown_shell.egg-info/not-zip-safe
```

### Comparing `duckietown-shell-5.4.5/setup.py` & `duckietown-shell-5.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     'duckietown-docker-utils-{}>=6.0.90'.format(distro),
     'zeroconf',
     'requests',
     'pytz',
     'dt-authentication-{}'.format(distro),
     'dt-data-api-{}>=1.2.0'.format(distro),
     "pip",
-    "dockertown>=0.1.1"
+    "dockertown>=0.1.1",
+    "dtproject",
 ]
 
 system_version = tuple(sys.version_info)[:3]
 if system_version < (3, 7):
     install_requires.append('dataclasses')
 
 setup(
```

