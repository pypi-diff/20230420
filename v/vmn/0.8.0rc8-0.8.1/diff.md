# Comparing `tmp/vmn-0.8.0rc8-py3-none-any.whl.zip` & `tmp/vmn-0.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 42228 bytes, number of entries: 10
+Zip file size: 44970 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      152 b- defN 21-Jul-06 16:25 version_stamp/__init__.py
--rw-r--r--  2.0 unx    45924 b- defN 23-Feb-25 23:00 version_stamp/stamp_utils.py
--rw-r--r--  2.0 unx       58 b- defN 23-Feb-26 14:20 version_stamp/version.py
--rw-r--r--  2.0 unx    97730 b- defN 23-Feb-26 08:26 version_stamp/vmn.py
--rw-r--r--  2.0 unx    35127 b- defN 23-Feb-26 14:20 vmn-0.8.0rc8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      460 b- defN 23-Feb-26 14:20 vmn-0.8.0rc8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-26 14:20 vmn-0.8.0rc8.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Feb-26 14:20 vmn-0.8.0rc8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Feb-26 14:20 vmn-0.8.0rc8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      803 b- defN 23-Feb-26 14:20 vmn-0.8.0rc8.dist-info/RECORD
-10 files, 180408 bytes uncompressed, 40858 bytes compressed:  77.4%
+-rw-r--r--  2.0 unx    53098 b- defN 23-Apr-16 14:06 version_stamp/stamp_utils.py
+-rw-r--r--  2.0 unx       50 b- defN 23-Apr-20 15:47 version_stamp/version.py
+-rw-r--r--  2.0 unx   109439 b- defN 23-Apr-20 12:54 version_stamp/vmn.py
+-rw-r--r--  2.0 unx    35127 b- defN 23-Apr-20 15:47 vmn-0.8.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      468 b- defN 23-Apr-20 15:47 vmn-0.8.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 15:47 vmn-0.8.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Apr-20 15:47 vmn-0.8.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-20 15:47 vmn-0.8.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      786 b- defN 23-Apr-20 15:47 vmn-0.8.1.dist-info/RECORD
+10 files, 199273 bytes uncompressed, 43636 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: version_stamp/version.py
 Comment: 
 
 Filename: version_stamp/vmn.py
 Comment: 
 
-Filename: vmn-0.8.0rc8.dist-info/LICENSE.txt
+Filename: vmn-0.8.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: vmn-0.8.0rc8.dist-info/METADATA
+Filename: vmn-0.8.1.dist-info/METADATA
 Comment: 
 
-Filename: vmn-0.8.0rc8.dist-info/WHEEL
+Filename: vmn-0.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: vmn-0.8.0rc8.dist-info/entry_points.txt
+Filename: vmn-0.8.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: vmn-0.8.0rc8.dist-info/top_level.txt
+Filename: vmn-0.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: vmn-0.8.0rc8.dist-info/RECORD
+Filename: vmn-0.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## version_stamp/stamp_utils.py

```diff
@@ -5,14 +5,16 @@
 import logging
 import os
 import pathlib
 import re
 import sys
 import time
 from logging.handlers import RotatingFileHandler
+import io
+from functools import wraps
 
 import git
 import yaml
 
 INIT_COMMIT_MESSAGE = "Initialized vmn tracking"
 
 VMN_VERSION_FORMAT = (
@@ -70,18 +72,102 @@
 RELATIVE_TO_CURRENT_VCS_BRANCH_TYPE = "branch"
 RELATIVE_TO_GLOBAL_TYPE = "global"
 
 VMN_USER_NAME = "vmn"
 VMN_BE_TYPE_GIT = "git"
 VMN_BE_TYPE_LOCAL_FILE = "local_file"
 
-LOGGER = None
+GLOBAL_LOG_FILENAME = "global_vmn.log"
+VMN_LOGGER = None
 
 
-VMN_GLOBAL_RESULTS_CACHE = {}
+# Create a custom execute function
+def custom_execute(self, *args, **kwargs):
+    global VMN_LOGGER
+
+    if VMN_LOGGER is not None:
+        VMN_LOGGER.debug(
+            f"{'  ' * (len(call_stack) - 1)}{' '.join(str(v) for v in args[0])}"
+        )
+
+    original_execute = getattr(self.__class__, "_execute")
+    originally_extended_output = "with_extended_output" in kwargs
+    kwargs["with_extended_output"] = True
+
+    start_time = time.perf_counter()
+    ret = original_execute(self, *args, **kwargs)
+    end_time = time.perf_counter()
+
+    ret_code = 0
+    sout = ""
+    serr = ""
+    if not originally_extended_output:
+        if type(ret) is tuple:
+            ret_code = ret[0]
+            sout = ret[1]
+            serr = ret[2]
+            ret = sout
+    elif type(ret) is not tuple:
+        sout = ret.stdout.read()
+        serr = ret.stdout.read()
+        ret_code = 0
+        if serr:
+            ret_code = 1
+
+    time_took = end_time - start_time
+
+    if VMN_LOGGER is not None:
+        VMN_LOGGER.debug(
+            f"{'  ' * (len(call_stack) - 1)}return code: {ret_code}, git cmd took: {time_took:.6f} seconds.\n"
+            f"{'  ' * (len(call_stack) - 1)}stdout: {sout}\n"
+            f"{'  ' * (len(call_stack) - 1)}stderr: {serr}"
+        )
+
+    return ret
+
+
+# Monkey-patch the Git class
+git.cmd.Git._execute = git.cmd.Git.execute
+git.cmd.Git.execute = custom_execute
+
+# Maintain a stack to keep track of nested function calls
+call_stack = []
+
+
+def measure_runtime_decorator(func):
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        global call_stack
+        global VMN_LOGGER
+
+        call_stack.append(func.__name__)
+        fcode = func.__code__
+
+        if VMN_LOGGER is not None:
+            VMN_LOGGER.debug(
+                f"{'  ' * (len(call_stack) - 1)}--> Entering {func.__name__} at {fcode.co_filename}:{fcode.co_firstlineno}"
+            )
+
+        start_time = time.perf_counter()
+        # Call the actual function
+        result = func(*args, **kwargs)
+        end_time = time.perf_counter()
+
+        elapsed_time = end_time - start_time
+
+        if VMN_LOGGER is not None:
+            VMN_LOGGER.debug(
+                f"{'  ' * (len(call_stack) - 1)}<-- Exiting {func.__name__} took {elapsed_time:.6f} seconds at {fcode.co_filename}:{fcode.co_firstlineno}"
+            )
+
+        call_stack.pop()
+
+        return result
+
+    return wrapper
 
 
 class WrongTagFormatException(Exception):
     pass
 
 
 def resolve_root_path():
@@ -104,15 +190,15 @@
             if prev_path == root_path:
                 raise RuntimeError()
 
             exist = os.path.exists(os.path.join(root_path, ".vmn")) or os.path.exists(
                 os.path.join(root_path, ".git")
             )
         except Exception as exc:
-            LOGGER.debug(f"Logged exception: ", exc_info=True)
+            VMN_LOGGER.debug(f"Logged exception: ", exc_info=True)
             root_path = None
             break
     if root_path is None:
         raise RuntimeError("Running from an unmanaged directory")
 
     return root_path
 
@@ -126,73 +212,91 @@
     def filter(self, record):
         if self._low <= record.levelno <= self._high:
             return True
         return False
 
 
 def init_stamp_logger(rotating_log_path=None, debug=False):
-    global LOGGER
+    global VMN_LOGGER
 
-    LOGGER = logging.getLogger(VMN_USER_NAME)
-    hlen = len(LOGGER.handlers)
-    for h in range(hlen):
-        LOGGER.handlers[0].close()
-        LOGGER.removeHandler(LOGGER.handlers[0])
-    flen = len(LOGGER.filters)
-    for f in range(flen):
-        LOGGER.removeFilter(LOGGER.filters[0])
+    VMN_LOGGER = logging.getLogger(VMN_USER_NAME)
+    clear_logger_handlers(VMN_LOGGER)
+    glob_logger = logging.getLogger()
+    clear_logger_handlers(glob_logger)
 
-    LOGGER.setLevel(logging.DEBUG)
+    glob_logger.setLevel(logging.DEBUG)
+    logging.getLogger("git").setLevel(logging.WARNING)
 
     fmt = "[%(levelname)s] %(message)s"
     formatter = logging.Formatter(fmt, "%Y-%m-%d %H:%M:%S")
 
     stdout_handler = logging.StreamHandler(sys.stdout)
     stdout_handler.setFormatter(formatter)
 
     min_stdout_level = logging.INFO
     if debug:
         min_stdout_level = logging.DEBUG
 
     stdout_handler.addFilter(LevelFilter(min_stdout_level, logging.INFO))
-    LOGGER.addHandler(stdout_handler)
+    VMN_LOGGER.addHandler(stdout_handler)
 
     stderr_handler = logging.StreamHandler(sys.stderr)
     stderr_handler.setFormatter(formatter)
     stderr_handler.setLevel(logging.WARNING)
-    LOGGER.addHandler(stderr_handler)
+    VMN_LOGGER.addHandler(stderr_handler)
 
     if rotating_log_path is None:
-        return LOGGER
+        return
+
+    rotating_file_handler = init_log_file_handler(rotating_log_path)
+    VMN_LOGGER.addHandler(rotating_file_handler)
+
+    global_log_path = os.path.join(
+        os.path.dirname(rotating_log_path), GLOBAL_LOG_FILENAME
+    )
+    global_file_handler = init_log_file_handler(global_log_path)
+    glob_logger.addHandler(global_file_handler)
+
 
+def init_log_file_handler(rotating_log_path):
     rotating_file_handler = RotatingFileHandler(
         rotating_log_path,
-        maxBytes=1024 * 1024 * 10,
+        maxBytes=1024 * 1024 * 50,
         backupCount=1,
     )
     rotating_file_handler.setLevel(logging.DEBUG)
-
-    fmt = f"%(filename)s:%(lineno)d => %(asctime)s - [%(levelname)s] %(message)s"
+    fmt = f"[%(levelname)s] %(asctime)s %(pathname)s:%(lineno)d =>\n%(message)s"
     formatter = logging.Formatter(fmt, "%Y-%m-%d %H:%M:%S")
     rotating_file_handler.setFormatter(formatter)
-    LOGGER.addHandler(rotating_file_handler)
+    return rotating_file_handler
 
-    return LOGGER
+
+def clear_logger_handlers(logger_obj):
+    hlen = len(logger_obj.handlers)
+    for h in range(hlen):
+        logger_obj.handlers[0].close()
+        logger_obj.removeHandler(logger_obj.handlers[0])
+    flen = len(logger_obj.filters)
+    for f in range(flen):
+        logger_obj.removeFilter(logger_obj.filters[0])
 
 
 class VMNBackend(object):
     def __init__(self, type):
         self._type = type
 
     def __del__(self):
         pass
 
     def type(self):
         return self._type
 
+    def prepare_for_remote_operation(self):
+        return 0
+
     def get_first_reachable_version_info(
         self, app_name, root=False, type=RELATIVE_TO_GLOBAL_TYPE
     ):
         return {}
 
     def get_active_branch(self):
         return "none"
@@ -250,14 +354,15 @@
         root_app_name = name.split("/")
         if len(root_app_name) == 1:
             return None
 
         return "/".join(root_app_name[:-1])
 
     @staticmethod
+    @measure_runtime_decorator
     def serialize_vmn_tag_name(
         app_name,
         version,
         hide_zero_hotfix,
         prerelease=None,
         prerelease_count=None,
         buildmetadata=None,
@@ -273,15 +378,15 @@
         )
 
         verstr = f"{app_name}_{verstr}"
 
         match = re.search(VMN_TAG_REGEX, verstr)
         if match is None:
             err = f"Tag {verstr} doesn't comply with: " f"{VMN_TAG_REGEX} format"
-            LOGGER.error(err)
+            VMN_LOGGER.error(err)
 
             raise RuntimeError(err)
 
         return verstr
 
     @staticmethod
     def serialize_vmn_version(
@@ -308,34 +413,34 @@
 
             match = re.search(VMN_REGEX, vmn_version)
             if match is None:
                 err = (
                     f"Tag {vmn_version} doesn't comply with: "
                     f"{VMN_VERSION_FORMAT} format"
                 )
-                LOGGER.error(err)
+                VMN_LOGGER.error(err)
 
                 raise RuntimeError(err)
         except AssertionError:
-            LOGGER.error(
+            VMN_LOGGER.error(
                 f"{prerelease} doesn't appear in {prerelease_count} "
                 "Turn on debug mode to see traceback"
             )
-            LOGGER.debug("Exception info: ", exc_info=True)
+            VMN_LOGGER.debug("Exception info: ", exc_info=True)
 
         if buildmetadata is not None:
             vmn_version = f"{vmn_version}+{buildmetadata}"
 
             match = re.search(VMN_REGEX, vmn_version)
             if match is None:
                 err = (
                     f"Tag {vmn_version} doesn't comply with: "
                     f"{VMN_VERSION_FORMAT} format"
                 )
-                LOGGER.error(err)
+                VMN_LOGGER.error(err)
                 raise RuntimeError(err)
 
         return vmn_version
 
     @staticmethod
     def serialize_vmn_version_hotfix(
         hide_zero_hotfix, major, minor, patch, hotfix=None
@@ -417,14 +522,15 @@
         if gdict["buildmetadata"] is not None:
             ret["buildmetadata"] = gdict["buildmetadata"]
             ret["type"] = "buildmetadata"
 
         return ret
 
     @staticmethod
+    @measure_runtime_decorator
     def enhance_ver_info(ver_infos):
         all_tags = {}
         for tag, ver_info_c in ver_infos.items():
             tagd = VMNBackend.deserialize_vmn_tag_name(tag)
             tagd.update({"tag": tag})
             tagd["message"] = ver_info_c["ver_info"]
 
@@ -439,26 +545,27 @@
                 )
             elif "app" not in v["ver_info"]["stamping"] and "version" in all_tags:
                 v["ver_info"]["stamping"].update(
                     all_tags["version"]["message"]["stamping"]
                 )
 
     @staticmethod
+    @measure_runtime_decorator
     def deserialize_vmn_tag_name(vmn_tag):
         try:
             return VMNBackend.deserialize_tag_name(vmn_tag)
         except WrongTagFormatException as exc:
-            LOGGER.error(
+            VMN_LOGGER.error(
                 f"Tag {vmn_tag} doesn't comply to vmn version format",
                 exc_info=True,
             )
 
             raise exc
         except Exception as exc:
-            LOGGER.error(
+            VMN_LOGGER.error(
                 f"Failed to deserialize tag {vmn_tag}",
                 exc_info=True,
             )
 
             raise exc
 
 
@@ -476,15 +583,15 @@
         self.repo_path = repo_path
         self.active_branch = "none"
         self.remote_active_branch = "remote/none"
 
     def __del__(self):
         pass
 
-    def perform_cached_fetch(self, repo_path):
+    def perform_cached_fetch(self, force=False):
         return
 
     def get_first_reachable_version_info(
         self, app_name, root=False, type=RELATIVE_TO_GLOBAL_TYPE
     ):
         ver_infos = {
             "none": {
@@ -540,57 +647,60 @@
         ver_infos = {
             tag_name: {"ver_info": None, "tag_object": None, "commit_object": None}
         }
         try:
             with open(path, "r") as f:
                 ver_infos[tag_name]["ver_info"] = yaml.safe_load(f)
         except Exception as exc:
-            LOGGER.error("Logged Exception message:", exc_info=True)
+            VMN_LOGGER.error("Logged Exception message:", exc_info=True)
 
         return tag_name, ver_infos
 
 
 class GitBackend(VMNBackend):
+    @measure_runtime_decorator
     def __init__(self, repo_path, inherit_env=False):
         VMNBackend.__init__(self, VMN_BE_TYPE_GIT)
 
         self._be = GitBackend.initialize_git_backend(repo_path, inherit_env)
         self.add_git_user_cfg_if_missing()
 
-        # TODO:: make _selected_remote configurable.
+        # TODO:: make selected_remote configurable.
         # Currently just selecting the first one
-        self._selected_remote = self._be.remotes[0]
+        self.selected_remote = self._be.remotes[0]
         self.repo_path = repo_path
         self.active_branch = self.get_active_branch()
         self.remote_active_branch = self.get_remote_tracking_branch(self.active_branch)
         self.detached_head = self.in_detached_head()
 
-    def perform_cached_fetch(self):
+    @measure_runtime_decorator
+    def perform_cached_fetch(self, force=False):
         vmn_cache_path = os.path.join(self.repo_path, ".vmn", "vmn.cache")
-        if not os.path.exists(vmn_cache_path):
+        if not os.path.exists(vmn_cache_path) or force:
             pathlib.Path(os.path.join(self.repo_path, ".vmn")).mkdir(
                 parents=True, exist_ok=True
             )
             pathlib.Path(vmn_cache_path).touch()
 
             self._be.git.execute(["git", "fetch", "--tags"])
-        else:
+        elif os.path.exists(vmn_cache_path):
             minutes_ago = datetime.datetime.now() - datetime.timedelta(minutes=30)
             filemtime = datetime.datetime.fromtimestamp(
                 os.path.getmtime(vmn_cache_path)
             )
             # file is more than 30 minutes old
             if filemtime < minutes_ago:
                 pathlib.Path(vmn_cache_path).touch()
                 self._be.git.execute(["git", "fetch", "--tags"])
 
     def __del__(self):
         self._be.close()
 
     @staticmethod
+    @measure_runtime_decorator
     def initialize_git_backend(repo_path, inherit_env):
         be = git.Repo(repo_path, search_parent_directories=True)
 
         if inherit_env:
             current_git_env = {
                 k: os.environ[k] for k in os.environ if k.startswith("GIT_")
             }
@@ -603,121 +713,137 @@
                 }
             )
             be.git.update_environment(**current_git_env)
 
         return be
 
     @staticmethod
+    @measure_runtime_decorator
     def get_repo_details(path):
         try:
             client = git.Repo(path, search_parent_directories=True)
         except git.exc.InvalidGitRepositoryError as exc:
-            LOGGER.debug(f'Skipping "{path}" directory reason:\n', exc_info=True)
+            VMN_LOGGER.debug(f'Skipping "{path}" directory reason:\n', exc_info=True)
             return None
         except Exception as exc:
-            LOGGER.debug(f'Skipping "{path}" directory reason:\n', exc_info=True)
+            VMN_LOGGER.debug(f'Skipping "{path}" directory reason:\n', exc_info=True)
             return None
 
         try:
             hash = client.head.commit.hexsha
             remote = tuple(client.remotes[0].urls)[0]
             if os.path.isdir(remote):
                 remote = os.path.relpath(remote, client.working_dir)
         except Exception as exc:
-            LOGGER.debug(f'Skipping "{path}" directory reason:\n', exc_info=True)
+            VMN_LOGGER.debug(f'Skipping "{path}" directory reason:\n', exc_info=True)
             return None
         finally:
             client.close()
 
         return hash, remote, "git"
 
+    @measure_runtime_decorator
     def is_path_tracked(self, path):
         try:
             self._be.git.execute(["git", "ls-files", "--error-unmatch", path])
             return True
         except Exception as exc:
-            LOGGER.debug(f"Logged exception for path {path}: ", exc_info=True)
+            VMN_LOGGER.debug(f"Logged exception for path {path}: ", exc_info=True)
             return False
 
+    @measure_runtime_decorator
     def tag(self, tags, messages, ref="HEAD", push=False):
         if push and self.remote_active_branch is None:
             raise RuntimeError("Will not push remote branch does not exist")
 
         for tag, message in zip(tags, messages):
             # This is required in order to preserver chronological order when
             # listing tags since the taggerdate field is in seconds resolution
             time.sleep(1.1)
             self._be.create_tag(tag, ref=ref, message=message)
 
             if not push:
                 continue
 
             try:
-                self._selected_remote.push(refspec=f"refs/tags/{tag}", o="ci.skip")
+                self.selected_remote.push(refspec=f"refs/tags/{tag}", o="ci.skip")
             except Exception:
-                self._selected_remote.push(refspec=f"refs/tags/{tag}")
+                self.selected_remote.push(refspec=f"refs/tags/{tag}")
 
+    @measure_runtime_decorator
     def push(self, tags=()):
         if self.detached_head:
             raise RuntimeError("Will not push from detached head")
 
         if self.remote_active_branch is None:
             raise RuntimeError("Will not push remote branch does not exist")
 
+        remote_branch_name_no_remote_name = "".join(
+            self.remote_active_branch.split(f"{self.selected_remote.name}/")
+        )
+
         try:
-            ret = self._selected_remote.push(
-                refspec=f"refs/heads/{self.active_branch}:{self.remote_active_branch.split('/')[-1]}",
+            ret = self.selected_remote.push(
+                refspec=f"refs/heads/{self.active_branch}:{remote_branch_name_no_remote_name}",
                 o="ci.skip",
             )
         except Exception as exc:
-            ret = self._selected_remote.push(
-                refspec=f"refs/heads/{self.active_branch}:{self.remote_active_branch.split('/')[-1]}"
+            ret = self.selected_remote.push(
+                refspec=f"refs/heads/{self.active_branch}:{remote_branch_name_no_remote_name}"
             )
 
         if ret[0].old_commit is None:
             if "up to date" in ret[0].summary:
-                LOGGER.warning(
+                VMN_LOGGER.warning(
                     "GitPython library has failed to push because we are "
                     "up to date already. How can it be? "
                 )
             else:
-                LOGGER.error("Push has failed. Please verify that 'git push' works")
+                VMN_LOGGER.error("Push has failed. Please verify that 'git push' works")
                 raise Warning(
                     f"Push has failed because: {ret[0].summary}.\n"
                     "Please verify that 'git push' works"
                 )
 
         for tag in tags:
             try:
-                self._selected_remote.push(refspec=f"refs/tags/{tag}", o="ci.skip")
+                self.selected_remote.push(refspec=f"refs/tags/{tag}", o="ci.skip")
             except Exception:
-                self._selected_remote.push(refspec=f"refs/tags/{tag}")
+                self.selected_remote.push(refspec=f"refs/tags/{tag}")
 
+    @measure_runtime_decorator
     def pull(self):
-        self._selected_remote.pull()
+        if self.detached_head:
+            raise RuntimeError("Will not pull in detached head")
+
+        self.selected_remote.pull("--ff-only")
 
+    @measure_runtime_decorator
     def commit(self, message, user, include=None):
         if include is not None:
             for file in include:
                 self._be.index.add(file)
         author = git.Actor(user, user)
 
         self._be.index.commit(message=message, author=author)
 
+    @measure_runtime_decorator
     def root(self):
         return self._be.working_dir
 
+    @measure_runtime_decorator
     def status(self, tag):
         found_tag = self._be.tag(f"refs/tags/{tag}")
         try:
             return tuple(found_tag.commit.stats.files)
         except Exception as exc:
-            LOGGER.debug(f"Logged exception: ", exc_info=True)
+            VMN_LOGGER.debug(f"Logged exception: ", exc_info=True)
             return None
 
+    @measure_runtime_decorator
     def get_latest_stamp_tags(
         self, app_name, root_context, type=RELATIVE_TO_GLOBAL_TYPE
     ):
         if root_context:
             msg_filter = f"^{app_name}/.*: Stamped"
         else:
             msg_filter = f"^{app_name}: Stamped"
@@ -727,14 +853,16 @@
         elif type == RELATIVE_TO_CURRENT_VCS_POSITION_TYPE:
             cmd_suffix = "HEAD"
         else:
             cmd_suffix = f"--branches"
 
         shallow = os.path.exists(os.path.join(self._be.common_dir, "shallow"))
         if shallow:
+            # This is the only usecase where we must perform a remote operation
+            # because otherwise even show will not work
             self.perform_cached_fetch()
             (
                 tag_names,
                 cobj,
                 ver_infos,
             ) = self._get_shallow_first_reachable_vmn_stamp_tag_list(
                 app_name,
@@ -744,27 +872,28 @@
         else:
             tag_names, cobj, ver_infos = self._get_first_reachable_vmn_stamp_tag_list(
                 app_name, cmd_suffix, msg_filter
             )
 
         return tag_names, cobj, ver_infos
 
+    @measure_runtime_decorator
     def _get_first_reachable_vmn_stamp_tag_list(self, app_name, cmd_suffix, msg_filter):
         cobj, ver_infos = self._get_top_vmn_commit(app_name, cmd_suffix, msg_filter)
         bug_limit = 0
         while not ver_infos and bug_limit < 100:
             if cobj is None:
                 break
 
             cmd_suffix = f"{cobj.hexsha}~1"
             cobj, ver_infos = self._get_top_vmn_commit(app_name, cmd_suffix, msg_filter)
 
             bug_limit += 1
             if bug_limit == 100:
-                LOGGER.warning(
+                VMN_LOGGER.warning(
                     f"Probable bug: vmn failed to find "
                     f"vmn's commit after 100 interations."
                 )
                 ver_infos = {}
                 break
 
         tag_objects = []
@@ -778,14 +907,15 @@
         )
         tag_names = []
         for tag_object in tag_objects:
             tag_names.append(tag_object.name)
 
         return tag_names, cobj, ver_infos
 
+    @measure_runtime_decorator
     def _get_shallow_first_reachable_vmn_stamp_tag_list(
         self, app_name, cmd_suffix, msg_filter
     ):
         cobj, ver_infos = self._get_top_vmn_commit(app_name, cmd_suffix, msg_filter)
 
         if ver_infos:
             tag_objects = []
@@ -826,15 +956,15 @@
 
                 latest_tag = tname
                 break
 
         try:
             found_tag = self._be.tag(f"refs/tags/{latest_tag}")
         except Exception as exc:
-            LOGGER.error(f"Failed to get tag object from tag name: {latest_tag}")
+            VMN_LOGGER.error(f"Failed to get tag object from tag name: {latest_tag}")
             return [], cobj, ver_infos
 
         ver_infos = self.get_all_commit_tags(found_tag.commit.hexsha)
         tag_objects = []
 
         for k in ver_infos.keys():
             if ver_infos[k]["tag_object"]:
@@ -848,196 +978,221 @@
 
         final_list_of_tag_names = []
         for tag_object in tag_objects:
             final_list_of_tag_names.append(tag_object.name)
 
         return final_list_of_tag_names, found_tag.commit, ver_infos
 
+    @measure_runtime_decorator
     def _get_top_vmn_commit(self, app_name, cmd_suffix, msg_filter):
         cmd = [
             f"--grep={msg_filter}",
             f"-1",
             f"--author={VMN_USER_NAME}",
             "--pretty=%H,,,%D",
             "--decorate=short",
             cmd_suffix,
         ]
-        LOGGER.debug(f"Going to run: git log {' '.join(cmd)}")
         log_res = self._be.git.log(*cmd).split("\n")
         if len(log_res) == 1 and log_res[0] == "":
             log_res.pop(0)
 
         if not log_res:
             return None, {}
 
         items = log_res[0].split(",,,")
         tags = items[1].split(",")
+        if len(tags) == 1 and tags[0] == "":
+            tags.pop(0)
+
         commit_hex = items[0]
         ver_infos = self.get_all_commit_tags_log_impl(commit_hex, tags, app_name)
 
         cobj = self.get_commit_object_from_commit_hex(commit_hex)
 
         return cobj, ver_infos
 
+    @measure_runtime_decorator
     def get_latest_available_tag(self, tag_prefix_filter):
         cmd = ["--sort", "taggerdate", "--list", tag_prefix_filter]
         tag_names = self._be.git.tag(*cmd).split("\n")
 
         if len(tag_names) == 1 and tag_names[0] == "":
             return None
 
         return tag_names[-1]
 
+    @measure_runtime_decorator
     def get_commit_object_from_branch_name(self, bname):
         # TODO:: Unfortunately, need to spend o(N) here
         for branch in self._be.branches:
             if bname != branch.name:
                 continue
 
             # yay, we found the tag's commit object
             return branch.commit
 
         raise RuntimeError(
             f"Somehow did not find a branch commit object for branch: {bname}"
         )
 
+    @measure_runtime_decorator
     def get_tag_object_from_tag_name(self, tname):
         try:
             o = self._be.tag(f"refs/tags/{tname}")
         except Exception as exc:
-            LOGGER.debug(f"Logged exception: ", exc_info=True)
+            VMN_LOGGER.debug(f"Logged exception: ", exc_info=True)
             # Backward compatability code for vmn 0.3.9:
             try:
                 _tag_name = f"{tname}.0"
                 o = self._be.tag(f"refs/tags/{tname}")
                 tag_name = _tag_name
             except Exception as exc:
-                LOGGER.debug(f"Logged exception: ", exc_info=True)
+                VMN_LOGGER.debug(f"Logged exception: ", exc_info=True)
                 return tname, None
 
         try:
             if o.commit.author.name != "vmn":
                 return tname, None
         except Exception as exc:
-            LOGGER.debug("Exception info: ", exc_info=True)
+            VMN_LOGGER.debug("Exception info: ", exc_info=True)
             return tname, None
 
         if o.tag is None:
             return tname, None
 
         if o is None:
-            LOGGER.debug(f"Somehow did not find a tag object for tag: {tname}")
+            VMN_LOGGER.debug(f"Somehow did not find a tag object for tag: {tname}")
 
         return tname, o
 
+    @measure_runtime_decorator
     def get_all_commit_tags_log_impl(self, hexsha, tags, app_name):
-        ver_infos = {}
+        cleaned_tags = []
         for t in tags:
             if "tag:" not in t:
-                # Maybe rebase or tag was removed. Will handle the rebase case here
-                try:
-                    commit_obj = self.get_commit_object_from_commit_hex(hexsha)
-                    verstr = commit_obj.message.split(" version ")[1].strip()
-                    tagname = f"{app_name}_{verstr}"
-                    tagname, ver_info_c = self.parse_tag_message(tagname)
-                    if ver_info_c["tag_object"]:
-
-                        ver_infos[tagname] = ver_info_c
-                except Exception as exc:
-                    LOGGER.debug(f"Skipped on {hexsha} commit")
-
                 continue
 
             tname = t.split("tag:")[1].strip()
+            cleaned_tags.append(tname)
+
+        ver_infos = {}
+        if not cleaned_tags:
+            # Maybe rebase or tag was removed. Will handle the rebase case here
+            try:
+                commit_obj = self.get_commit_object_from_commit_hex(hexsha)
+                verstr = commit_obj.message.split(" version ")[1].strip()
+                tagname = f"{app_name}_{verstr}"
+                tagname, ver_info_c = self.parse_tag_message(tagname)
+                if ver_info_c["tag_object"]:
+                    ver_infos[tagname] = ver_info_c
+
+                    cleaned_tags = self.get_all_brother_tags(tagname)
+                    cleaned_tags.pop(tagname)
+                    cleaned_tags = cleaned_tags.keys()
+            except Exception as exc:
+                VMN_LOGGER.debug(f"Skipped on {hexsha} commit")
+
+        for tname in cleaned_tags:
             tname, ver_info_c = self.parse_tag_message(tname)
             if ver_info_c["ver_info"] is None:
-                LOGGER.debug(
+                VMN_LOGGER.debug(
                     f"Probably non-vmn tag - {tname} with tag msg: {ver_info_c['ver_info']}. Skipping ",
                     exc_info=True,
                 )
                 continue
 
             ver_infos[tname] = ver_info_c
 
         return ver_infos
 
+    @measure_runtime_decorator
     def get_all_commit_tags(self, hexsha="HEAD"):
         if hexsha is None:
             hexsha = "HEAD"
 
         cmd = ["--points-at", hexsha]
         tags = self._be.git.tag(*cmd).split("\n")
 
         if len(tags) == 1 and tags[0] == "":
             tags.pop(0)
 
         ver_infos = {}
         for t in tags:
             t, ver_info_c = self.parse_tag_message(t)
             if ver_info_c["ver_info"] is None:
-                LOGGER.debug(
+                VMN_LOGGER.debug(
                     f"Probably non-vmn tag - {t} with tag msg: {ver_info_c['ver_info']}. Skipping ",
                     exc_info=True,
                 )
                 continue
 
             ver_infos[t] = ver_info_c
 
         return ver_infos
 
+    @measure_runtime_decorator
     def get_all_brother_tags(self, tag_name):
         try:
             sha = self.changeset(tag=tag_name)
             ver_infos = self.get_all_commit_tags(sha)
         except Exception as exc:
-            LOGGER.debug(
+            VMN_LOGGER.debug(
                 f"Failed to get brother tags for tag: {tag_name}. "
                 f"Logged exception: ",
                 exc_info=True,
             )
             return []
 
         return ver_infos
 
     def in_detached_head(self):
         return self._be.head.is_detached
 
+    @measure_runtime_decorator
     def add_git_user_cfg_if_missing(self):
         try:
             self._be.config_reader().get_value("user", "name")
             self._be.config_reader().get_value("user", "email")
         except (configparser.NoSectionError, configparser.NoOptionError):
             # git user name or email configuration is missing, add default override
             self._be.git.set_persistent_git_options(
                 c=[f'user.name="{VMN_USER_NAME}"', f'user.email="{VMN_USER_NAME}"']
             )
 
+    @measure_runtime_decorator
     def check_for_pending_changes(self):
         if self._be.is_dirty():
             err = f"Pending changes in {self.root()}."
             return err
 
         return None
 
+    @measure_runtime_decorator
     def check_for_outgoing_changes(self):
         if self.in_detached_head():
             err = f"Detached head in {self.root()}."
             return err
 
         if self.remote_active_branch is None:
-            err = f"No remote branch found in {self.root()}."
+            err = (
+                f"No upstream branch found in {self.root()}. "
+                f"for local branch {self.active_branch}. "
+                f"Probably no upstream branch is set"
+            )
+
             return err
 
         branch_name = self.active_branch
         try:
             self._be.git.rev_parse("--verify", f"{self.remote_active_branch}")
         except Exception:
             err = (
-                f"Branch {self.remote_active_branch} does not exist. "
-                "Please push or set-upstream branch to "
+                f"Remote branch {self.remote_active_branch} does not exist. "
+                "Please set-upstream branch to "
                 f"{self.remote_active_branch} of branch {branch_name}"
             )
             return err
 
         outgoing = tuple(
             self._be.iter_commits(f"{self.remote_active_branch}..{branch_name}")
         )
@@ -1050,97 +1205,159 @@
                 f"The commits that are outgoing are: {outgoing}"
             )
 
             return err
 
         return None
 
+    @measure_runtime_decorator
     def checkout_branch(self, branch_name=None):
         try:
             if branch_name is None:
                 branch_name = self.active_branch
 
             self.checkout(branch=branch_name)
-        except Exception:
-            logging.info("Failed to get branch name. Trying to checkout to master")
-            LOGGER.debug("Exception info: ", exc_info=True)
-            # TODO:: change to some branch name that can be retreived from repo
-            try:
-                # TODO:: configure the default branchname
-                self.checkout(branch="master")
-            except Exception as exc:
-                self.checkout(branch="main")
+        except Exception as exc:
+            logging.error("Failed to get branch name")
+            VMN_LOGGER.debug("Exception info: ", exc_info=True)
+
+            return None
 
         return self._be.active_branch.commit.hexsha
 
+    @measure_runtime_decorator
     def get_remote_tracking_branch(self, local_branch_name):
         command = [
             "git",
             "rev-parse",
             "--abbrev-ref",
             "--symbolic-full-name",
             f"{local_branch_name}@{{u}}",
         ]
 
         try:
-            return self._be.git.execute(command)
+            ret = self._be.git.execute(command)
+
+            try:
+                assert ret.startswith(self.selected_remote.name)
+            except Exception as exc:
+                VMN_LOGGER.warning(
+                    f"Found remote branch {ret} however it belongs to a "
+                    f"different remote that vmn has selected to work with. "
+                    f"Will behave like no remote was found. The remote that vmn has "
+                    f"selected to work with is: {self.selected_remote.name}"
+                )
+
+                return None
+
+            return ret
         except Exception as exc:
             return None
 
+    @measure_runtime_decorator
+    def prepare_for_remote_operation(self):
+        if self.remote_active_branch is not None:
+            return 0
+
+        local_branch_name = self.active_branch
+
+        VMN_LOGGER.warning(
+            f"No remote branch for local branch: {local_branch_name} "
+            f"was found. Will try to set upstream for it"
+        )
+
+        out = self._be.git.branch("-r", "--contains", "HEAD")
+        out = out.split("\n")[0].strip()
+        if not out:
+            out = f"{self.selected_remote.name}/{local_branch_name}"
+
+        try:
+            self._be.git.execute(
+                [
+                    "git",
+                    "remote",
+                    "set-branches",
+                    "--add",
+                    self.selected_remote.name,
+                    local_branch_name,
+                ]
+            )
+            self._be.git.branch(f"--set-upstream-to={out}", local_branch_name)
+        except Exception as exc:
+            VMN_LOGGER.debug(
+                f"Failed to set upstream branch for {local_branch_name}:", exc_info=True
+            )
+            return 1
+
+        self.remote_active_branch = out
+
+        return 0
+
+    @measure_runtime_decorator
     def get_active_branch(self):
         # TODO:: return the full ref name: refs/heads/..
         if not self.in_detached_head():
             active_branch = self._be.active_branch.name
         else:
             active_branch = self.get_branch_from_changeset(self._be.head.commit.hexsha)
 
         return active_branch
 
+    @measure_runtime_decorator
     def get_branch_from_changeset(self, hexsha):
         out = self._be.git.branch("--contains", hexsha)
         out = out.split("\n")[1:]
         if not out:
             # TODO:: add debug print here
             out = self._be.git.branch().split("\n")[1:]
 
         active_branches = []
         for item in out:
             active_branches.append(item.strip())
         if len(active_branches) > 1:
-            LOGGER.info(
+            VMN_LOGGER.info(
                 f"{self._be.head.commit.hexsha} is "
                 f"related to multiple branches: {active_branches}. "
                 "Using the first one as the active branch"
             )
 
         if not active_branches:
             out = self._be.git.branch("-r", "--contains", hexsha)
             out = out.split("\n")[0].strip()
 
             if not out:
                 raise RuntimeError(f"Failed to find remote branch for hex: {hexsha}")
 
+            assert out.startswith(self.selected_remote.name)
+
             local_branch_name = (
                 f"vmn_tracking_remote__{out.replace('/', '_')}__from_{hexsha[:5]}"
             )
             self._be.git.branch(local_branch_name, out)
             self._be.git.branch(f"--set-upstream-to={out}", local_branch_name)
 
+            VMN_LOGGER.debug(
+                f"Setting local branch {local_branch_name} "
+                f"to track remote branch {out}"
+            )
+
             self.active_branch = local_branch_name
             self.remote_active_branch = out
 
             remote_branch_hexsha = self._be.refs[out].commit.hexsha
             if remote_branch_hexsha == hexsha:
-                self.checkout_branch()
+                ret = self.checkout_branch()
+                assert ret is not None
 
             active_branches.append(local_branch_name)
 
         active_branch = active_branches[0]
         return active_branch
 
+    @measure_runtime_decorator
     def checkout(self, rev=None, tag=None, branch=None):
         if tag is not None:
             # TODO:: maybe it issafer to
             rev = f"refs/tags/{tag}"
         elif branch is not None:
             # TODO:: : f"refs/heads/{branch}"
             rev = f"{branch}"
@@ -1148,14 +1365,15 @@
         assert rev is not None
 
         self._be.git.checkout(rev)
 
         self.detached_head = self.in_detached_head()
 
     @staticmethod
+    @measure_runtime_decorator
     def get_actual_deps_state(vmn_root_path, paths):
         actual_deps_state = {}
         for path in paths:
             full_path = os.path.join(vmn_root_path, path)
             details = GitBackend.get_repo_details(full_path)
             if details is None:
                 continue
@@ -1164,48 +1382,51 @@
                 "hash": details[0],
                 "remote": details[1],
                 "vcs_type": details[2],
             }
 
         return actual_deps_state
 
+    @measure_runtime_decorator
     def last_user_changeset(self):
         p = self._be.head.commit
         if p.author.name == VMN_USER_NAME:
             if p.message.startswith(INIT_COMMIT_MESSAGE):
                 return p.hexsha
 
             ver_infos = self.get_all_commit_tags(p.hexsha)
             if not ver_infos:
-                LOGGER.warning(
+                VMN_LOGGER.warning(
                     f"Somehow vmn's commit {p.hexsha} has no tags. "
                     f"Check your repo. Assuming this commit is a user commit"
                 )
                 return p.hexsha
 
             for t, v in ver_infos.items():
                 if "stamping" in v["ver_info"]:
                     return v["ver_info"]["stamping"]["app"]["changesets"]["."]["hash"]
 
-            LOGGER.warning(
+            VMN_LOGGER.warning(
                 f"Somehow vmn's commit {p.hexsha} has no tags that are parsable. "
                 f"Check your repo. Assuming this commit is a user commit"
             )
             return p.hexsha
 
         return p.hexsha
 
+    @measure_runtime_decorator
     def remote(self):
-        remote = tuple(self._selected_remote.urls)[0]
+        remote = tuple(self.selected_remote.urls)[0]
 
         if os.path.isdir(remote):
             remote = os.path.relpath(remote, self.root())
 
         return remote
 
+    @measure_runtime_decorator
     def changeset(self, tag=None, short=False):
         if tag is None:
             if short:
                 return self._be.head.commit.hexsha[:6]
 
             return self._be.head.commit.hexsha
 
@@ -1213,58 +1434,61 @@
 
         try:
             if short:
                 return found_tag.commit.hexsha[:6]
 
             return found_tag.commit.hexsha
         except Exception as exc:
-            LOGGER.debug(f"Logged exception: ", exc_info=True)
+            VMN_LOGGER.debug(f"Logged exception: ", exc_info=True)
             return None
 
+    @measure_runtime_decorator
     def revert_local_changes(self, files=[]):
         if files:
             try:
                 try:
                     for f in files:
                         self._be.git.reset(f)
                 except Exception as exc:
-                    LOGGER.debug(f"Failed to git reset files: {files}", exc_info=True)
+                    VMN_LOGGER.debug(f"Failed to git reset files: {files}", exc_info=True)
 
                 self._be.index.checkout(files, force=True)
             except Exception as exc:
-                LOGGER.debug(f"Failed to git checkout files: {files}", exc_info=True)
+                VMN_LOGGER.debug(f"Failed to git checkout files: {files}", exc_info=True)
 
+    @measure_runtime_decorator
     def revert_vmn_commit(self, prev_changeset, version_files, tags=[]):
         self.revert_local_changes(version_files)
 
         # TODO: also validate that the commit is
         #  currently worked on app name
         if self.changeset() == prev_changeset:
             return
 
         if self._be.active_branch.commit.author.name != VMN_USER_NAME:
-            LOGGER.error("BUG: Will not revert non-vmn commit.")
+            VMN_LOGGER.error("BUG: Will not revert non-vmn commit.")
             raise RuntimeError()
 
         self._be.git.reset("--hard", "HEAD~1")
         for tag in tags:
             try:
                 self._be.delete_tag(tag)
             except Exception:
-                LOGGER.info(f"Failed to remove tag {tag}")
-                LOGGER.debug("Exception info: ", exc_info=True)
+                VMN_LOGGER.info(f"Failed to remove tag {tag}")
+                VMN_LOGGER.debug("Exception info: ", exc_info=True)
 
                 continue
 
         try:
             self._be.git.fetch("--tags")
         except Exception:
-            LOGGER.info("Failed to fetch tags")
-            LOGGER.debug("Exception info: ", exc_info=True)
+            VMN_LOGGER.info("Failed to fetch tags")
+            VMN_LOGGER.debug("Exception info: ", exc_info=True)
 
+    @measure_runtime_decorator
     def get_first_reachable_version_info(
         self, app_name, root_context=False, type=RELATIVE_TO_GLOBAL_TYPE
     ):
         app_tags, cobj, ver_infos = self.get_latest_stamp_tags(
             app_name, root_context, type
         )
 
@@ -1291,49 +1515,54 @@
             cleaned_app_tag = tag
             break
 
         if cleaned_app_tag is None:
             return None, {}
 
         if cleaned_app_tag not in ver_infos:
-            LOGGER.debug(f"Somehow {cleaned_app_tag} not in ver_infos")
+            VMN_LOGGER.debug(f"Somehow {cleaned_app_tag} not in ver_infos")
             return None, {}
 
         VMNBackend.enhance_ver_info(ver_infos)
 
         return cleaned_app_tag, ver_infos
 
+    @measure_runtime_decorator
     def get_tag_version_info(self, tag_name):
         ver_infos = {}
         tag_name, commit_tag_obj = self.get_commit_object_from_tag_name(tag_name)
+        if commit_tag_obj is None:
+            VMN_LOGGER.debug(f"Tried to find {tag_name} but with no success")
+            return tag_name, ver_infos
 
-        if commit_tag_obj is None or commit_tag_obj.author.name != VMN_USER_NAME:
-            LOGGER.debug(f"Corrupted tag {tag_name}: author name is not vmn")
+        if commit_tag_obj.author.name != VMN_USER_NAME:
+            VMN_LOGGER.debug(f"Corrupted tag {tag_name}: author name is not vmn")
             return tag_name, ver_infos
 
         # "raw" ver_infos
         ver_infos = self.get_all_brother_tags(tag_name)
         if tag_name not in ver_infos:
-            LOGGER.debug(f"Could not find version info for {tag_name}")
+            VMN_LOGGER.debug(f"Could not find version info for {tag_name}")
             return tag_name, None
 
         VMNBackend.enhance_ver_info(ver_infos)
 
         return tag_name, ver_infos
 
+    @measure_runtime_decorator
     def parse_tag_message(self, tag_name):
         tag_name, tag_obj = self.get_tag_object_from_tag_name(tag_name)
 
         ret = {"ver_info": None, "tag_object": tag_obj, "commit_object": None}
         if not tag_obj:
             return tag_name, ret
 
         commit_tag_obj = tag_obj.commit
         if commit_tag_obj is None or commit_tag_obj.author.name != VMN_USER_NAME:
-            LOGGER.debug(f"Corrupted tag {tag_name}: author name is not vmn")
+            VMN_LOGGER.debug(f"Corrupted tag {tag_name}: author name is not vmn")
             return tag_name, ret
 
         ret["commit_object"] = commit_tag_obj
 
         # TODO:: Check API commit version
         # safe_load discards any text before the YAML document (if present)
         ver_info = yaml.safe_load(tag_obj.object.message)
@@ -1350,45 +1579,46 @@
                 commit_msg["stamping"]["app"]["prerelease_count"] = {}
 
             ver_info = commit_msg
             if ver_info is None:
                 return tag_name, ret
 
         if "vmn_info" not in ver_info:
-            LOGGER.debug(f"vmn_info key was not found in tag {tag_name}")
+            VMN_LOGGER.debug(f"vmn_info key was not found in tag {tag_name}")
             return tag_name, ret
 
         ret["ver_info"] = ver_info
 
         return tag_name, ret
 
+    @measure_runtime_decorator
     def get_commit_object_from_commit_hex(self, hex):
         return self._be.commit(hex)
 
+    @measure_runtime_decorator
     def get_commit_object_from_tag_name(self, tag_name):
         try:
             commit_tag_obj = self._be.commit(tag_name)
         except Exception as exc:
-            LOGGER.debug(f"Logged exception: ", exc_info=True)
             # Backward compatability code for vmn 0.3.9:
             try:
                 _tag_name = f"{tag_name}.0"
                 commit_tag_obj = self._be.commit(_tag_name)
                 tag_name = _tag_name
             except Exception as exc:
-                LOGGER.debug(f"Logged exception: ", exc_info=True)
                 return tag_name, None
 
         return tag_name, commit_tag_obj
 
     @staticmethod
     def clone(path, remote):
         git.Repo.clone_from(f"{remote}", f"{path}")
 
 
+@measure_runtime_decorator
 def get_client(root_path, be_type, inherit_env=False):
     if be_type == "local_file":
         be = LocalFileBackend(root_path)
         return be, None
 
     try:
         client = git.Repo(root_path, search_parent_directories=True)
```

## version_stamp/version.py

```diff
@@ -1,3 +1,3 @@
 name = "vmn"
-version = "0.8.0-rc8"
-_version = "0.8.0-rc8"
+version = "0.8.1"
+_version = "0.8.1"
```

## version_stamp/vmn.py

```diff
@@ -16,41 +16,47 @@
 import jinja2
 import tomlkit
 import yaml
 from filelock import FileLock
 from packaging import version as pversion
 
 CUR_PATH = "{0}/".format(os.path.dirname(__file__))
+sys.path.append(CUR_PATH)
+import version as version_mod
+import stamp_utils
+
+
+LOCK_FILE_ENV = "VMN_LOCK_FILE_PATH"
+
 VER_FILE_NAME = "last_known_app_version.yml"
 INIT_FILENAME = "conf.yml"
 LOCK_FILENAME = "vmn.lock"
 LOG_FILENAME = "vmn.log"
 CACHE_FILENAME = "vmn.cache"
 
-IGNORED_FILES = [LOCK_FILENAME, LOG_FILENAME, CACHE_FILENAME]
-VMN_ARGS = [
-    "init",
-    "init-app",
-    "show",
-    "stamp",
-    "goto",
-    "release",
-    "gen",
-    "add",
+IGNORED_FILES = [
+    LOCK_FILENAME,
+    LOG_FILENAME,
+    CACHE_FILENAME,
+    stamp_utils.GLOBAL_LOG_FILENAME,
 ]
+VMN_ARGS = {
+    "init": "remote",
+    "init-app": "remote",
+    "show": "local",
+    "stamp": "remote",
+    "goto": "local",
+    "release": "remote",
+    "gen": "local",
+    "add": "remote",
+}
 
-sys.path.append(CUR_PATH)
 
-import version as version_mod
-import stamp_utils
-
-LOGGER = None
-
-
-class VMNContextMAnager(object):
+class VMNContainer(object):
+    @stamp_utils.measure_runtime_decorator
     def __init__(self, args, root_path):
         self.args = args
         root = False
         if "root" in self.args:
             root = self.args.root
 
         initial_params = {"root": root, "name": None, "root_path": root_path}
@@ -58,42 +64,28 @@
         if "name" in self.args and self.args.name:
             validate_app_name(self.args)
             initial_params["name"] = self.args.name
 
             if "command" in self.args and "stamp" in self.args.command:
                 initial_params["extra_commit_message"] = self.args.extra_commit_message
 
-        vmn_path = os.path.join(root_path, ".vmn")
-        lock_file_path = os.path.join(vmn_path, LOCK_FILENAME)
-
-        self.lock = FileLock(lock_file_path)
         self.params = initial_params
         self.vcs = None
-        self.lock_file_path = lock_file_path
 
         # Currently this is used only for show and only for cargo situation
         # TODO:: think if this feature should exist at all
         self.params["be_type"] = stamp_utils.VMN_BE_TYPE_GIT
         if "from_file" in self.args and self.args.from_file:
             self.params["be_type"] = stamp_utils.VMN_BE_TYPE_LOCAL_FILE
 
         self.vcs = VersionControlStamper(self.params)
 
-    def __enter__(self):
-        self.lock.acquire()
-        return self
-
-    def __exit__(self, exc_type, exc_value, exc_traceback):
-        self.lock.release()
-
-        if os.path.exists(self.lock_file_path):
-            os.unlink(self.lock_file_path)
-
 
 class IVersionsStamper(object):
+    @stamp_utils.measure_runtime_decorator
     def __init__(self, arg_params):
         self.app_conf_path = None
         self.params: dict = arg_params
         self.vmn_root_path: str = arg_params["root_path"]
         self.repo_name: str = "."
         self.name: str = arg_params["name"]
         self.be_type = arg_params["be_type"]
@@ -101,16 +93,16 @@
         # Configuration defaults
         self.template: str = stamp_utils.VMN_DEFAULT_TEMPLATE
         self.extra_info = False
         self.create_verinfo_files = False
         self.hide_zero_hotfix = True
         self.version_backends = {}
         # This one will be filled with self dependency ('.') by default
-        self.raw_configured_deps = None
-        self.configured_deps = None
+        self.raw_configured_deps = {}
+        self.configured_deps = {}
         self.conf_file_exists = False
         self.root_conf_file_exists = False
 
         self.should_publish = True
         self.current_version_info = {
             "vmn_info": {
                 "description_message_version": "1.1",
@@ -125,15 +117,15 @@
         self.backend, err = stamp_utils.get_client(
             self.vmn_root_path,
             self.be_type,
             inherit_env=True,
         )
         if err:
             err_str = "Failed to create backend {0}. Exiting".format(err)
-            LOGGER.error(err_str)
+            stamp_utils.VMN_LOGGER.error(err_str)
             raise RuntimeError(err_str)
 
         if self.name is None:
             self.tracked = False
             return
 
         self.initialize_paths()
@@ -155,14 +147,15 @@
             }
 
         err = self.initialize_backend_attrs()
         if err:
             # TODO:: test this
             raise RuntimeError("Failed to initialize_backend_attrs")
 
+    @stamp_utils.measure_runtime_decorator
     def update_attrs_from_app_conf_file(self):
         # TODO:: handle deleted app with missing conf file
         if os.path.isfile(self.app_conf_path):
             self.conf_file_exists = True
 
             with open(self.app_conf_path, "r") as f:
                 data = yaml.safe_load(f)
@@ -186,14 +179,15 @@
         ):
             self.root_conf_file_exists = True
             with open(self.root_app_conf_path) as f:
                 data = yaml.safe_load(f)
                 if "external_services" in data["conf"]:
                     self.external_services = data["conf"]["external_services"]
 
+    @stamp_utils.measure_runtime_decorator
     def initialize_paths(self):
         self.app_dir_path = os.path.join(
             self.vmn_root_path, ".vmn", self.name.replace("/", os.sep)
         )
 
         self.version_file_path = os.path.join(self.app_dir_path, VER_FILE_NAME)
 
@@ -224,19 +218,18 @@
                 f"{self.backend.active_branch}_root_conf.yml",
             )
             if not os.path.isfile(self.root_app_conf_path):
                 self.root_app_conf_path = os.path.join(
                     self.root_app_dir_path, "root_conf.yml"
                 )
 
+    @stamp_utils.measure_runtime_decorator
     def initialize_configured_deps(self, self_base, self_dep):
-        if self.raw_configured_deps is not None:
+        if self.raw_configured_deps:
             self.configured_deps = self.raw_configured_deps
-        if self.configured_deps is None:
-            self.configured_deps = {}
 
         if os.path.join("../") not in self.configured_deps:
             self.configured_deps[os.path.join("../")] = {}
         if self_base not in self.configured_deps[os.path.join("../")]:
             self.configured_deps[os.path.join("../")][self_base] = {}
 
         self.configured_deps[os.path.join("../")][self_base] = self_dep
@@ -248,53 +241,59 @@
                     os.path.join(self.vmn_root_path, rel_path, repo),
                     self.vmn_root_path,
                 )
                 flat_deps[key] = v[repo]
 
         self.configured_deps = flat_deps
 
+    @stamp_utils.measure_runtime_decorator
     def get_version_info_from_verstr(self, verstr):
         tag_name = self.get_tag_name(verstr)
         if self.root_context:
             try:
                 int(verstr)
             except Exception:
-                LOGGER.error("wrong version specified: root version must be an integer")
+                stamp_utils.VMN_LOGGER.error(
+                    "wrong version specified: root version must be an integer"
+                )
 
                 return tag_name, {}
         else:
             try:
                 stamp_utils.VMNBackend.deserialize_vmn_tag_name(tag_name)
             except Exception as exc:
-                LOGGER.error(f"Wrong version specified: {verstr}")
-                LOGGER.debug(f"Logged exception: ", exc_info=True)
+                stamp_utils.VMN_LOGGER.error(f"Wrong version specified: {verstr}")
+                stamp_utils.VMN_LOGGER.debug(f"Logged exception: ", exc_info=True)
 
                 return tag_name, {}
 
-        try:
-            tag_name, ver_infos = self.backend.get_tag_version_info(tag_name)
-        except Exception:
-            LOGGER.error(f"Faield to get version info for tag: {tag_name}")
+        tag_name, ver_infos = self.backend.get_tag_version_info(tag_name)
+        if not ver_infos:
+            stamp_utils.VMN_LOGGER.error(
+                f"Failed to get version info for tag: {tag_name}"
+            )
 
             return tag_name, {}
 
         if tag_name not in ver_infos or ver_infos[tag_name]["ver_info"] is None:
             return tag_name, {}
 
         stamp_utils.VMNBackend.enhance_ver_info(ver_infos)
 
         return tag_name, ver_infos
 
+    @stamp_utils.measure_runtime_decorator
     def get_tag_name(self, verstr):
         tag_name = f'{self.name.replace("/", "-")}'
         assert verstr is not None
         tag_name = f"{tag_name}_{verstr}"
 
         return tag_name
 
+    @stamp_utils.measure_runtime_decorator
     def initialize_backend_attrs(self):
         self_base = os.path.basename(self.vmn_root_path)
         self_dep = {"remote": self.backend.remote(), "vcs_type": self.backend.type()}
 
         self.initialize_configured_deps(self_base, self_dep)
 
         if self.name is None:
@@ -313,22 +312,45 @@
             self.vmn_root_path,
             self.configured_deps,
         )
         self.actual_deps_state["."]["hash"] = self.last_user_changeset
         self.current_version_info["stamping"]["app"]["changesets"] = copy.deepcopy(
             self.actual_deps_state
         )
+
+        self.ver_infos_from_repo = {}
+        self.selected_tag = None
         (
-            self.selected_tag,
-            self.ver_infos_from_repo,
-        ) = self.backend.get_first_reachable_version_info(
-            self.name,
-            self.root_context,
-            type=stamp_utils.RELATIVE_TO_CURRENT_VCS_POSITION_TYPE,
-        )
+            initial_version,
+            prerelease,
+            prerelease_count,
+        ) = VersionControlStamper.get_version_number_from_file(self.version_file_path)
+        if initial_version is not None:
+            verstr = stamp_utils.VMNBackend.serialize_vmn_version(
+                initial_version, prerelease, prerelease_count, self.hide_zero_hotfix
+            )
+            (
+                self.selected_tag,
+                self.ver_infos_from_repo,
+            ) = self.get_version_info_from_verstr(verstr)
+            t = self.get_tag_name(initial_version)
+            if t != self.selected_tag and t in self.ver_infos_from_repo:
+                self.selected_tag = t
+
+        if not self.ver_infos_from_repo:
+            (
+                selected_tag,
+                self.ver_infos_from_repo,
+            ) = self.backend.get_first_reachable_version_info(
+                self.name,
+                self.root_context,
+                type=stamp_utils.RELATIVE_TO_CURRENT_VCS_POSITION_TYPE,
+            )
+            if selected_tag is not None and selected_tag != self.selected_tag:
+                self.selected_tag = selected_tag
 
         self.tracked = (
             self.selected_tag in self.ver_infos_from_repo
             and self.ver_infos_from_repo[self.selected_tag]["ver_info"] is not None
         )
         if self.tracked:
             for rel_path, dep in self.configured_deps.items():
@@ -353,15 +375,15 @@
         return 0
 
     def set_template(self, template):
         try:
             self.template = IVersionsStamper.parse_template(template)
             self.bad_format_template = False
         except Exception as exc:
-            LOGGER.debug("Logged exception: ", exc_info=True)
+            stamp_utils.VMN_LOGGER.debug("Logged exception: ", exc_info=True)
             self.template = IVersionsStamper.parse_template(
                 stamp_utils.VMN_DEFAULT_TEMPLATE
             )
             self.template_err_str = (
                 "Failed to parse template: "
                 f"{template}. "
                 f"Falling back to default one: "
@@ -400,19 +422,19 @@
     def _advance_prerelease(self, verstr, prerelease, prerelease_count):
         if prerelease is None:
             return None, {}
         if prerelease == "release":
             try:
                 raise RuntimeError()
             except RuntimeError:
-                LOGGER.error(
+                stamp_utils.VMN_LOGGER.error(
                     "prerelease equals to 'release' somehow. "
                     "Turn on debug mode to see traceback"
                 )
-                LOGGER.debug("Exception info: ", exc_info=True)
+                stamp_utils.VMN_LOGGER.debug("Exception info: ", exc_info=True)
 
             return None, {}
 
         prerelease_count = copy.deepcopy(prerelease_count)
         counter_key = f"{prerelease}"
         if counter_key not in prerelease_count:
             prerelease_count[counter_key] = 0
@@ -503,15 +525,15 @@
             hotfix,
         )
 
     def write_version_to_file(
         self, version_number: str, prerelease: str, prerelease_count: dict
     ) -> None:
         if self.dry_run:
-            LOGGER.info(
+            stamp_utils.VMN_LOGGER.info(
                 "Would have written to version file:\n"
                 f"version: {version_number}\n"
                 f"prerelease: {prerelease}\n"
                 f"prerelease count: {prerelease_count}"
             )
         else:
             self._write_version_to_vmn_version_file(
@@ -527,69 +549,89 @@
             prerelease_count,
             self.hide_zero_hotfix,
         )
         verstr = self.get_be_formatted_version(verstr)
         for backend in self.version_backends:
             try:
                 if backend == "vmn_version_file":
-                    LOGGER.warning(
+                    stamp_utils.VMN_LOGGER.warning(
                         "Remove vmn_version_file version backend from the configuration"
                     )
                     continue
 
                 handler = getattr(self, f"_write_version_to_{backend}")
                 if self.dry_run:
-                    LOGGER.info(
+                    stamp_utils.VMN_LOGGER.info(
                         "Would have written to a version backend file:\n"
                         f"backend: {backend}\n"
                         f"version: {verstr}"
                     )
                 else:
                     handler(verstr)
             except AttributeError:
-                LOGGER.warning(f"Unsupported version backend {backend}")
+                stamp_utils.VMN_LOGGER.warning(f"Unsupported version backend {backend}")
                 continue
 
     def _write_version_to_npm(self, verstr):
         backend_conf = self.version_backends["npm"]
         file_path = os.path.join(self.vmn_root_path, backend_conf["path"])
         try:
             with open(file_path, "r") as f:
                 data = json.load(f)
 
             data["version"] = verstr
             with open(file_path, "w") as f:
                 json.dump(data, f, indent=4, sort_keys=True)
         except IOError as e:
-            LOGGER.error(f"Error writing npm ver file: {file_path}\n")
-            LOGGER.debug("Exception info: ", exc_info=True)
+            stamp_utils.VMN_LOGGER.error(f"Error writing npm ver file: {file_path}\n")
+            stamp_utils.VMN_LOGGER.debug("Exception info: ", exc_info=True)
 
             raise IOError(e)
         except Exception as e:
-            LOGGER.debug(e, exc_info=True)
+            stamp_utils.VMN_LOGGER.debug(e, exc_info=True)
             raise RuntimeError(e)
 
     def _write_version_to_cargo(self, verstr):
         backend_conf = self.version_backends["cargo"]
         file_path = os.path.join(self.vmn_root_path, backend_conf["path"])
         try:
             with open(file_path, "r") as f:
                 data = tomlkit.loads(f.read())
 
             data["package"]["version"] = verstr
             with open(file_path, "w") as f:
                 data = tomlkit.dumps(data)
                 f.write(data)
         except IOError as e:
-            LOGGER.error(f"Error writing cargo ver file: {file_path}\n")
-            LOGGER.debug("Exception info: ", exc_info=True)
+            stamp_utils.VMN_LOGGER.error(f"Error writing cargo ver file: {file_path}\n")
+            stamp_utils.VMN_LOGGER.debug("Exception info: ", exc_info=True)
+
+            raise IOError(e)
+        except Exception as e:
+            stamp_utils.VMN_LOGGER.debug(e, exc_info=True)
+            raise RuntimeError(e)
+
+    def _write_version_to_poetry(self, verstr):
+        backend_conf = self.version_backends["poetry"]
+        file_path = os.path.join(self.vmn_root_path, backend_conf["path"])
+        try:
+            with open(file_path, "r") as f:
+                data = tomlkit.loads(f.read())
+
+            data["tool"]["poetry"]["version"] = verstr
+            with open(file_path, "w") as f:
+                data = tomlkit.dumps(data)
+                f.write(data)
+        except IOError as e:
+            stamp_utils.VMN_LOGGER.error(f"Error writing cargo ver file: {file_path}\n")
+            stamp_utils.VMN_LOGGER.debug("Exception info: ", exc_info=True)
 
             raise IOError(e)
         except Exception as e:
-            LOGGER.debug(e, exc_info=True)
+            stamp_utils.VMN_LOGGER.debug(e, exc_info=True)
             raise RuntimeError(e)
 
     def _write_version_to_vmn_version_file(
         self, prerelease, prerelease_count, version_number
     ):
         file_path = self.version_file_path
         if prerelease is None:
@@ -601,20 +643,20 @@
                 ver_dict = {
                     "version_to_stamp_from": version_number,
                     "prerelease": prerelease,
                     "prerelease_count": prerelease_count,
                 }
                 yaml.dump(ver_dict, fid)
         except IOError as e:
-            LOGGER.error(f"Error writing ver file: {file_path}\n")
-            LOGGER.debug("Exception info: ", exc_info=True)
+            stamp_utils.VMN_LOGGER.error(f"Error writing ver file: {file_path}\n")
+            stamp_utils.VMN_LOGGER.debug("Exception info: ", exc_info=True)
 
             raise IOError(e)
         except Exception as e:
-            LOGGER.debug(e, exc_info=True)
+            stamp_utils.VMN_LOGGER.debug(e, exc_info=True)
             raise RuntimeError(e)
 
     @staticmethod
     def parse_template(template: str) -> object:
         match = re.search(stamp_utils.VMN_TEMPLATE_REGEX, template)
 
         gdict = match.groupdict()
@@ -668,17 +710,19 @@
 
         with open(self.root_app_conf_path, "w+") as f:
             f.write("# Autogenerated by vmn\n")
             yaml.dump(ver_yml, f, sort_keys=True)
 
 
 class VersionControlStamper(IVersionsStamper):
+    @stamp_utils.measure_runtime_decorator
     def __init__(self, arg_params):
         IVersionsStamper.__init__(self, arg_params)
 
+    @stamp_utils.measure_runtime_decorator
     def find_matching_version(self, version, prerelease, prerelease_count):
         """
         Try to find any version of the application matching the
         user's repositories local state
         :param version:
         :param prerelease:
         :param prerelease_count:
@@ -701,28 +745,35 @@
         )
 
         if self.selected_tag != tag_formatted_app_name:
             # Get version info for tag
             tag_formatted_app_name, ver_infos = self.backend.get_tag_version_info(
                 tag_formatted_app_name
             )
+            if not ver_infos:
+                stamp_utils.VMN_LOGGER.error(
+                    f"Failed to get version info for tag: {tag_formatted_app_name}"
+                )
+                return None
         else:
             ver_infos = self.ver_infos_from_repo
 
+        # TODO:: just a sanity? May be removed?
         if (
             tag_formatted_app_name not in ver_infos
             or ver_infos[tag_formatted_app_name] is None
         ):
             return None
 
         # means we are trying to find a matching version that is in rc state
         if prerelease_count:
             # try to check if there is a release version on it
             for k, v in ver_infos.items():
                 if v is None:
+                    # TODO: WTF?
                     raise RuntimeError("Bug")
 
         tmp = ver_infos[tag_formatted_app_name]["ver_info"]
         if release_tag_formatted_app_name in ver_infos:
             tmp = ver_infos[release_tag_formatted_app_name]["ver_info"]
 
         # Can happen if app's name is a prefix of another app
@@ -751,14 +802,15 @@
 
         if found:
             return tmp
 
         return None
 
     @staticmethod
+    @stamp_utils.measure_runtime_decorator
     def get_version_number_from_file(version_file_path) -> str or None:
         if not os.path.exists(version_file_path):
             return (None, None, None)
 
         with open(version_file_path, "r") as fid:
             ver_dict = yaml.safe_load(fid)
             if "version_to_stamp_from" in ver_dict:
@@ -778,17 +830,18 @@
 
             return (
                 ver_dict["last_stamped_version"],
                 ver_dict["prerelease"],
                 ver_dict["prerelease_count"],
             )
 
+    @stamp_utils.measure_runtime_decorator
     def release_app_version(self, tag_name, ver_info):
         if ver_info is None:
-            LOGGER.error(
+            stamp_utils.VMN_LOGGER.error(
                 f"Tag {tag_name} doesn't seem to exist. Wrong version specified?"
             )
             raise RuntimeError()
 
         tmp = ver_info["stamping"]["app"]
         release_tag_name = stamp_utils.VMNBackend.serialize_vmn_tag_name(
             self.name,
@@ -814,19 +867,20 @@
             messages,
             ref=self.backend.changeset(tag=tag_name),
             push=True,
         )
 
         return props["version"]
 
+    @stamp_utils.measure_runtime_decorator
     def add_metadata_to_version(self, tag_name, ver_info):
         # TODO:: merge logic with release_app_version and
         #  publish and handle reverting this way
         if ver_info is None:
-            LOGGER.error(
+            stamp_utils.VMN_LOGGER.error(
                 f"Tag {tag_name} doesn't seem to exist. Wrong version specified?"
             )
             raise RuntimeError()
 
         tmp = ver_info["stamping"]["app"]
         res_ver = stamp_utils.VMNBackend.serialize_vmn_version(
             tmp["_version"],
@@ -864,17 +918,19 @@
             with open(path) as f:
                 ver_info["stamping"]["app"]["version_metadata"] = yaml.safe_load(f)
 
         (
             buildmetadata_tag_name,
             tag_ver_infos,
         ) = self.backend.get_tag_version_info(buildmetadata_tag_name)
-        if buildmetadata_tag_name in tag_ver_infos is not None:
+        if buildmetadata_tag_name in tag_ver_infos:
             if tag_ver_infos[buildmetadata_tag_name]["ver_info"] != ver_info:
-                LOGGER.error(f"Tried to add different metadata for the same version.")
+                stamp_utils.VMN_LOGGER.error(
+                    f"Tried to add different metadata for the same version."
+                )
                 raise RuntimeError()
 
             return res_ver
 
         messages = [yaml.dump(ver_info, sort_keys=True)]
 
         self.backend.tag(
@@ -882,19 +938,20 @@
             messages,
             ref=self.backend.changeset(tag=tag_name),
             push=True,
         )
 
         return res_ver
 
+    @stamp_utils.measure_runtime_decorator
     def stamp_app_version(
         self, initial_version, initialprerelease, initialprerelease_count
     ):
         if initialprerelease == "release" and self.release_mode is None:
-            LOGGER.error(
+            stamp_utils.VMN_LOGGER.error(
                 "When not in release candidate mode, "
                 "a release mode must be specified - use "
                 "-r/--release-mode with one of major/minor/patch/hotfix"
             )
             raise RuntimeError()
 
         if initialprerelease != "release" and self.release_mode is None:
@@ -908,15 +965,15 @@
                 ver_infos,
             ) = self.backend.get_tag_version_info(release_tag_formatted_app_name)
 
             if (
                 release_tag_formatted_app_name in ver_infos
                 and ver_infos[release_tag_formatted_app_name] is not None
             ):
-                LOGGER.error(
+                stamp_utils.VMN_LOGGER.error(
                     f"The version {initial_version} was already released. "
                     "Will refuse to stamp prerelease version "
                 )
                 raise RuntimeError()
 
         current_version, prerelease, prerelease_count = self.gen_advanced_version(
             initial_version, initialprerelease, initialprerelease_count
@@ -942,14 +999,15 @@
             prerelease,
             prerelease_count,
             release_mode,
         )
 
         return current_version, prerelease, prerelease_count
 
+    @stamp_utils.measure_runtime_decorator
     def update_stamping_info(
         self,
         info,
         initial_version,
         initialprerelease,
         initialprerelease_count,
         current_version,
@@ -979,31 +1037,34 @@
         self.current_version_info["stamping"]["app"][
             "stamped_on_remote_branch"
         ] = self.backend.remote_active_branch
         self.current_version_info["stamping"]["app"][
             "prerelease_count"
         ] = copy.deepcopy(prerelease_count)
 
+    @stamp_utils.measure_runtime_decorator
     def stamp_root_app_version(self, override_version=None):
         if self.root_app_name is None:
             return None
 
         tag_name, ver_infos = self.backend.get_first_reachable_version_info(
             self.root_app_name,
             root_context=True,
             type=stamp_utils.RELATIVE_TO_CURRENT_VCS_POSITION_TYPE,
         )
 
         if tag_name not in ver_infos or ver_infos[tag_name]["ver_info"] is None:
-            LOGGER.error(f"Version information for {self.root_app_name} was not found")
+            stamp_utils.VMN_LOGGER.error(
+                f"Version information for {self.root_app_name} was not found"
+            )
             raise RuntimeError()
 
         # TODO: think about this case
         if "version" not in ver_infos[tag_name]["ver_info"]["stamping"]["root_app"]:
-            LOGGER.error(
+            stamp_utils.VMN_LOGGER.error(
                 f"Root app name is {self.root_app_name} and app name is {self.name}. "
                 f"However no version information for root was found"
             )
             raise RuntimeError()
 
         old_version = int(
             ver_infos[tag_name]["ver_info"]["stamping"]["root_app"]["version"]
@@ -1040,14 +1101,15 @@
         version_files = []
         for path in paths:
             if path in changed or path in untracked:
                 version_files.append(path)
 
         return version_files
 
+    @stamp_utils.measure_runtime_decorator
     def publish_stamp(
         self, app_version, prerelease, prerelease_count, root_app_version
     ):
         verstr = stamp_utils.VMNBackend.serialize_vmn_version(
             app_version,
             prerelease,
             prerelease_count,
@@ -1106,141 +1168,144 @@
         self.current_version_info["stamping"]["msg"] = commit_msg
 
         prev_changeset = self.backend.changeset()
 
         try:
             self.publish_commit(version_files_to_add)
         except Exception as exc:
-            LOGGER.debug("Logged Exception message: ", exc_info=True)
-            LOGGER.info(f"Reverting vmn changes... ")
+            stamp_utils.VMN_LOGGER.debug("Logged Exception message: ", exc_info=True)
+            stamp_utils.VMN_LOGGER.info(f"Reverting vmn changes... ")
             if self.dry_run:
-                LOGGER.info(f"Would have tried to revert a vmn commit")
+                stamp_utils.VMN_LOGGER.info(f"Would have tried to revert a vmn commit")
             else:
                 self.backend.revert_vmn_commit(prev_changeset, self.version_files)
 
             # TODO:: turn to error codes. This one means - exit without retries
             return 3
 
         tag = f'{self.name.replace("/", "-")}_{verstr}'
         match = re.search(stamp_utils.VMN_TAG_REGEX, tag)
         if match is None:
-            LOGGER.error(
+            stamp_utils.VMN_LOGGER.error(
                 f"Tag {tag} doesn't comply to vmn version format"
                 f"Reverting vmn changes ..."
             )
             if self.dry_run:
-                LOGGER.info("Would have reverted vmn commit.")
+                stamp_utils.VMN_LOGGER.info("Would have reverted vmn commit.")
             else:
                 self.backend.revert_vmn_commit(prev_changeset, self.version_files)
 
             return 3
 
         tags = [tag]
         msgs = [app_msg]
 
         if self.root_app_name is not None:
             msgs.append(root_app_msg)
             tag = f"{self.root_app_name}_{root_app_version}"
             match = re.search(stamp_utils.VMN_ROOT_TAG_REGEX, tag)
             if match is None:
-                LOGGER.error(
+                stamp_utils.VMN_LOGGER.error(
                     f"Tag {tag} doesn't comply to vmn version format"
                     f"Reverting vmn changes ..."
                 )
                 if self.dry_run:
-                    LOGGER.info("Would have reverted vmn commit.")
+                    stamp_utils.VMN_LOGGER.info("Would have reverted vmn commit.")
                 else:
                     self.backend.revert_vmn_commit(prev_changeset, self.version_files)
 
                 return 3
 
             tags.append(tag)
 
         all_tags = []
         all_tags.extend(tags)
 
         try:
             for t, m in zip(tags, msgs):
                 if self.dry_run:
-                    LOGGER.info(
+                    stamp_utils.VMN_LOGGER.info(
                         "Would have created tag:\n"
                         f"{t}\n"
                         f"Tag content:\n{yaml.dump(m, sort_keys=True)}"
                     )
                 else:
                     self.backend.tag([t], [yaml.dump(m, sort_keys=True)])
         except Exception as exc:
-            LOGGER.debug("Logged Exception message:", exc_info=True)
-            LOGGER.info(f"Reverting vmn changes for tags: {tags} ... ")
+            stamp_utils.VMN_LOGGER.debug("Logged Exception message:", exc_info=True)
+            stamp_utils.VMN_LOGGER.info(f"Reverting vmn changes for tags: {tags} ... ")
             if self.dry_run:
-                LOGGER.info(
+                stamp_utils.VMN_LOGGER.info(
                     f"Would have reverted vmn commit and delete tags:\n{all_tags}"
                 )
             else:
                 self.backend.revert_vmn_commit(
                     prev_changeset, self.version_files, all_tags
                 )
 
             return 1
 
         try:
             if self.dry_run:
-                LOGGER.info("Would have pushed with tags.\n" f"tags: {all_tags} ")
+                stamp_utils.VMN_LOGGER.info(
+                    "Would have pushed with tags.\n" f"tags: {all_tags} "
+                )
             else:
                 self.backend.push(all_tags)
 
                 count = 0
                 res = self.backend.check_for_outgoing_changes()
                 while count < 5 and res:
                     count += 1
-                    LOGGER.error(
+                    stamp_utils.VMN_LOGGER.error(
                         f"BUG: Somehow we have outgoing changes right "
                         f"after publishing:\n{res}"
                     )
-                    time.sleep(count)
+                    time.sleep(60)
                     res = self.backend.check_for_outgoing_changes()
 
                 if count == 5 and res:
                     raise RuntimeError(
                         f"BUG: Somehow we have outgoing changes right "
                         f"after publishing:\n{res}"
                     )
         except Exception:
-            LOGGER.debug("Logged Exception message:", exc_info=True)
-            LOGGER.info(f"Reverting vmn changes for tags: {tags} ...")
+            stamp_utils.VMN_LOGGER.debug("Logged Exception message:", exc_info=True)
+            stamp_utils.VMN_LOGGER.info(f"Reverting vmn changes for tags: {tags} ...")
             if self.dry_run:
-                LOGGER.info(
+                stamp_utils.VMN_LOGGER.info(
                     f"Would have reverted vmn commit and delete tags:\n{all_tags}"
                 )
             else:
                 self.backend.revert_vmn_commit(
                     prev_changeset, self.version_files, all_tags
                 )
 
             return 2
 
         return 0
 
+    @stamp_utils.measure_runtime_decorator
     def publish_commit(self, version_files_to_add):
         cur_branch = self.backend.active_branch
         path = os.path.join(
             self.app_dir_path,
             f"*_conf.yml",
         )
         list_of_files = glob.glob(path)
         branch_conf_path = os.path.join(self.app_dir_path, f"{cur_branch}_conf.yml")
 
         if self.dry_run:
             if list_of_files:
-                LOGGER.info(
+                stamp_utils.VMN_LOGGER.info(
                     "Would have removed config files:\n"
                     f"{set(list_of_files) - set([branch_conf_path])}"
                 )
 
-            LOGGER.info(
+            stamp_utils.VMN_LOGGER.info(
                 "Would have created commit with message:\n"
                 f'{self.current_version_info["stamping"]["msg"]}'
             )
         else:
             for f in set(list_of_files) - set([branch_conf_path]):
                 try:
                     self.backend._be.index.remove([f], working_tree=True)
@@ -1255,61 +1320,66 @@
 
             self.backend.commit(
                 message=self.current_version_info["stamping"]["msg"],
                 user="vmn",
                 include=version_files_to_add,
             )
 
+    @stamp_utils.measure_runtime_decorator
     def create_verinfo_root_file(
         self, root_app_msg, root_app_version, version_files_to_add
     ):
         dir_path = os.path.join(self.root_app_dir_path, "root_verinfo")
 
         if self.dry_run:
-            LOGGER.info(
+            stamp_utils.VMN_LOGGER.info(
                 "Would have written to root verinfo file:\n"
                 f"path: {dir_path} version: {root_app_version}\n"
                 f"message: {root_app_msg}"
             )
         else:
             Path(dir_path).mkdir(parents=True, exist_ok=True)
             path = os.path.join(dir_path, f"{root_app_version}.yml")
             with open(path, "w") as f:
                 data = yaml.dump(root_app_msg, sort_keys=True)
                 f.write(data)
             version_files_to_add.append(path)
 
+    @stamp_utils.measure_runtime_decorator
     def create_verinfo_file(self, app_msg, version_files_to_add, verstr):
         dir_path = os.path.join(self.app_dir_path, "verinfo")
 
         if self.dry_run:
-            LOGGER.info(
+            stamp_utils.VMN_LOGGER.info(
                 "Would have written to verinfo file:\n"
                 f"path: {dir_path} version: {verstr}\n"
                 f"message: {app_msg}"
             )
         else:
             Path(dir_path).mkdir(parents=True, exist_ok=True)
             path = os.path.join(dir_path, f"{verstr}.yml")
             with open(path, "w") as f:
                 data = yaml.dump(app_msg, sort_keys=True)
                 f.write(data)
 
             version_files_to_add.append(path)
 
+    @stamp_utils.measure_runtime_decorator
     def retrieve_remote_changes(self):
         self.backend.pull()
 
 
+@stamp_utils.measure_runtime_decorator
 def handle_init(vmn_ctx):
     expected_status = {"repos_exist_locally"}
+    optional_status = {"deps_synced_with_conf"}
 
-    status = _get_repo_status(vmn_ctx.vcs, expected_status)
+    status = _get_repo_status(vmn_ctx.vcs, expected_status, optional_status)
     if status["error"]:
-        LOGGER.debug(
+        stamp_utils.VMN_LOGGER.debug(
             f"Error occured when getting the repo status: {status}", exc_info=True
         )
 
         return 1
 
     be = vmn_ctx.vcs.backend
 
@@ -1327,41 +1397,45 @@
     be.commit(
         message=stamp_utils.INIT_COMMIT_MESSAGE,
         user="vmn",
         include=[vmn_init_path, git_ignore_path],
     )
     be.push()
 
-    LOGGER.info(f"Initialized vmn tracking on {vmn_ctx.vcs.vmn_root_path}")
+    stamp_utils.VMN_LOGGER.info(
+        f"Initialized vmn tracking on {vmn_ctx.vcs.vmn_root_path}"
+    )
 
     return 0
 
 
+@stamp_utils.measure_runtime_decorator
 def handle_init_app(vmn_ctx):
     vmn_ctx.vcs.dry_run = vmn_ctx.args.dry
 
     # TODO: validate version number is of type major.minor.patch[.hotfix]
     err = _init_app(vmn_ctx.vcs, vmn_ctx.args.version)
     if err:
         return 1
 
     if vmn_ctx.vcs.dry_run:
-        LOGGER.info(
+        stamp_utils.VMN_LOGGER.info(
             "Would have initialized app tracking on {0}".format(
                 vmn_ctx.vcs.root_app_dir_path
             )
         )
     else:
-        LOGGER.info(
+        stamp_utils.VMN_LOGGER.info(
             "Initialized app tracking on {0}".format(vmn_ctx.vcs.root_app_dir_path)
         )
 
     return 0
 
 
+@stamp_utils.measure_runtime_decorator
 def handle_stamp(vmn_ctx):
     vmn_ctx.vcs.prerelease = vmn_ctx.args.pr
     vmn_ctx.vcs.buildmetadata = None
     vmn_ctx.vcs.release_mode = vmn_ctx.args.release_mode
     vmn_ctx.vcs.override_root_version = vmn_ctx.args.orv
     vmn_ctx.vcs.override_version = vmn_ctx.args.ov
     vmn_ctx.vcs.dry_run = vmn_ctx.args.dry
@@ -1378,48 +1452,56 @@
         ][
             "app"
         ][
             "release_mode"
         ]
 
     optional_status = {"modified", "detached"}
-    expected_status = {"repos_exist_locally", "repo_tracked", "app_tracked"}
+    expected_status = {
+        "repos_exist_locally",
+        "repo_tracked",
+        "app_tracked",
+        "deps_synced_with_conf",
+    }
 
     status = _get_repo_status(vmn_ctx.vcs, expected_status, optional_status)
     if status["error"]:
-        LOGGER.debug(
+        stamp_utils.VMN_LOGGER.debug(
             f"Error occured when getting the repo status: {status}", exc_info=True
         )
 
         return 1
 
     if status["matched_version_info"] is not None:
         # Good we have found an existing version matching
         # the actual_deps_state
         version = vmn_ctx.vcs.get_be_formatted_version(
             status["matched_version_info"]["stamping"]["app"]["_version"]
         )
 
-        LOGGER.info(version)
+        stamp_utils.VMN_LOGGER.info(version)
 
         return 0
 
     if "detached" in status["state"]:
-        LOGGER.error("In detached head. Will not stamp new version")
+        stamp_utils.VMN_LOGGER.error("In detached head. Will not stamp new version")
         return 1
 
     vmn_ctx.vcs.backend.perform_cached_fetch()
 
     # We didn't find any existing version
     if vmn_ctx.args.pull:
         try:
+            vmn_ctx.vcs.backend.perform_cached_fetch(force=True)
             vmn_ctx.vcs.retrieve_remote_changes()
         except Exception as exc:
-            LOGGER.error("Failed to pull, run with --debug for more details")
-            LOGGER.debug("Logged Exception message:", exc_info=True)
+            stamp_utils.VMN_LOGGER.error(
+                "Failed to pull, run with --debug for more details"
+            )
+            stamp_utils.VMN_LOGGER.debug("Logged Exception message:", exc_info=True)
 
             return 1
 
     (
         initial_version,
         prerelease,
         prerelease_count,
@@ -1436,60 +1518,61 @@
             vmn_ctx.args.pull,
             vmn_ctx.args.check_vmn_version,
             initial_version,
             prerelease,
             prerelease_count,
         )
     except Exception as exc:
-        LOGGER.debug("Logged Exception message:", exc_info=True)
+        stamp_utils.VMN_LOGGER.debug("Logged Exception message:", exc_info=True)
 
         return 1
 
     if vmn_ctx.vcs.dry_run:
-        LOGGER.info(f"Would have stamped {version}")
+        stamp_utils.VMN_LOGGER.info(f"Would have stamped {version}")
     else:
-        LOGGER.info(f"{version}")
+        stamp_utils.VMN_LOGGER.info(f"{version}")
 
     return 0
 
 
+@stamp_utils.measure_runtime_decorator
 def handle_release(vmn_ctx):
     expected_status = {"repos_exist_locally", "repo_tracked", "app_tracked"}
-    optional_status = {"detached", "modified", "dirty_deps"}
+    optional_status = {"detached", "modified", "dirty_deps", "deps_synced_with_conf"}
 
     status = _get_repo_status(vmn_ctx.vcs, expected_status, optional_status)
     if status["error"]:
-        LOGGER.debug(
+        stamp_utils.VMN_LOGGER.debug(
             f"Error occured when getting the repo status: {status}", exc_info=True
         )
 
         return 1
 
     ver = vmn_ctx.args.version
 
     if ver:
         # TODO:: extract method
         match = re.search(stamp_utils.VMN_REGEX, ver)
         res = match.groupdict()
         if res["buildmetadata"]:
-            LOGGER.error(
+            stamp_utils.VMN_LOGGER.error(
                 f"Failed to release {ver}. "
                 f"Releasing metadata versions is not supported"
             )
 
             return 1
 
     if ver is None and status["matched_version_info"] is not None:
         # Good we have found an existing version matching
         # the actual_deps_state
         ver = vmn_ctx.vcs.get_be_formatted_version(
             status["matched_version_info"]["stamping"]["app"]["_version"]
         )
     elif ver is None:
-        LOGGER.error(
+        stamp_utils.VMN_LOGGER.error(
             "When running vmn release and not on a version commit, "
             "you must specify a specific version using -v flag"
         )
 
         return 1
 
     try:
@@ -1507,182 +1590,196 @@
         tag_formatted_app_name = stamp_utils.VMNBackend.serialize_vmn_tag_name(
             vmn_ctx.vcs.name,
             base_ver,
             vmn_ctx.vcs.hide_zero_hotfix,
         )
 
         if tag_formatted_app_name in ver_infos:
-            LOGGER.info(base_ver)
+            stamp_utils.VMN_LOGGER.info(base_ver)
             return 0
 
-        LOGGER.info(vmn_ctx.vcs.release_app_version(tag_name, ver_info))
+        stamp_utils.VMN_LOGGER.info(vmn_ctx.vcs.release_app_version(tag_name, ver_info))
     except Exception as exc:
-        LOGGER.error(f"Failed to release {ver}")
-        LOGGER.debug("Logged Exception message:", exc_info=True)
+        stamp_utils.VMN_LOGGER.error(f"Failed to release {ver}")
+        stamp_utils.VMN_LOGGER.debug("Logged Exception message:", exc_info=True)
 
         return 1
 
     return 0
 
 
+@stamp_utils.measure_runtime_decorator
 def handle_add(vmn_ctx):
     vmn_ctx.params["buildmetadata"] = vmn_ctx.args.bm
     vmn_ctx.params["version_metadata_path"] = vmn_ctx.args.vmp
     vmn_ctx.params["version_metadata_url"] = vmn_ctx.args.vmu
 
     expected_status = {"repos_exist_locally", "repo_tracked", "app_tracked"}
-    optional_status = {"detached", "modified", "dirty_deps"}
+    optional_status = {"detached", "modified", "dirty_deps", "deps_synced_with_conf"}
 
     status = _get_repo_status(vmn_ctx.vcs, expected_status, optional_status)
     if status["error"]:
-        LOGGER.debug(
+        stamp_utils.VMN_LOGGER.debug(
             f"Error occured when getting the repo status: {status}", exc_info=True
         )
 
         return 1
 
     ver = vmn_ctx.args.version
 
     if ver:
         # TODO:: extract method
         match = re.search(stamp_utils.VMN_REGEX, ver)
         res = match.groupdict()
         if res["buildmetadata"]:
-            LOGGER.error(
+            stamp_utils.VMN_LOGGER.error(
                 f"Failed to add to {ver}. "
                 f"Adding metadata versions to metadata versions is not supported"
             )
 
             return 1
 
     if ver is None and status["matched_version_info"] is not None:
         # Good we have found an existing version matching
         # the actual_deps_state
         ver = vmn_ctx.vcs.get_be_formatted_version(
             status["matched_version_info"]["stamping"]["app"]["_version"]
         )
     elif ver is None:
-        LOGGER.error(
+        stamp_utils.VMN_LOGGER.error(
             "When running vmn add and not on a version commit, "
             "you must specify a specific version using -v flag"
         )
 
         return 1
 
     try:
         tag_name, ver_infos = vmn_ctx.vcs.get_version_info_from_verstr(ver)
         if tag_name not in ver_infos or ver_infos[tag_name]["ver_info"] is None:
             ver_info = None
         else:
             ver_info = ver_infos[tag_name]["ver_info"]
-        LOGGER.info(vmn_ctx.vcs.add_metadata_to_version(tag_name, ver_info))
+        stamp_utils.VMN_LOGGER.info(
+            vmn_ctx.vcs.add_metadata_to_version(tag_name, ver_info)
+        )
     except Exception as exc:
-        LOGGER.debug("Logged Exception message:", exc_info=True)
+        stamp_utils.VMN_LOGGER.debug("Logged Exception message:", exc_info=True)
 
         return 1
 
     return 0
 
 
+@stamp_utils.measure_runtime_decorator
 def handle_show(vmn_ctx):
     vmn_ctx.params["from_file"] = vmn_ctx.args.from_file
 
     # root app does not have raw version number
     if vmn_ctx.vcs.root_context:
         vmn_ctx.params["raw"] = False
     else:
         vmn_ctx.params["raw"] = vmn_ctx.args.raw
 
     vmn_ctx.params["ignore_dirty"] = vmn_ctx.args.ignore_dirty
 
     vmn_ctx.params["verbose"] = vmn_ctx.args.verbose
+    vmn_ctx.params["conf"] = vmn_ctx.args.conf
+
     if vmn_ctx.args.template is not None:
         vmn_ctx.vcs.set_template(vmn_ctx.args.template)
 
     vmn_ctx.params["display_unique_id"] = vmn_ctx.args.display_unique_id
     vmn_ctx.params["display_type"] = vmn_ctx.args.display_type
 
     try:
         out = show(vmn_ctx.vcs, vmn_ctx.params, vmn_ctx.args.version)
     except Exception as exc:
-        LOGGER.debug("Logged Exception message:", exc_info=True)
+        stamp_utils.VMN_LOGGER.debug("Logged Exception message:", exc_info=True)
         return 1
 
     return 0
 
 
+@stamp_utils.measure_runtime_decorator
 def handle_gen(vmn_ctx):
     vmn_ctx.params["jinja_template"] = vmn_ctx.args.template
     vmn_ctx.params["verify_version"] = vmn_ctx.args.verify_version
     vmn_ctx.params["output"] = vmn_ctx.args.output
     vmn_ctx.params["custom_values"] = vmn_ctx.args.custom_values
 
     try:
         out = gen(vmn_ctx.vcs, vmn_ctx.params, vmn_ctx.args.version)
     except Exception as exc:
-        LOGGER.error("Failed to gen, run with --debug for more details")
-        LOGGER.debug("Logged Exception message:", exc_info=True)
+        stamp_utils.VMN_LOGGER.error("Failed to gen, run with --debug for more details")
+        stamp_utils.VMN_LOGGER.debug("Logged Exception message:", exc_info=True)
         return 1
 
     return 0
 
 
+@stamp_utils.measure_runtime_decorator
 def handle_goto(vmn_ctx):
     expected_status = {"repo_tracked", "app_tracked"}
-    optional_status = {"detached", "repos_exist_locally", "modified"}
+    optional_status = {
+        "detached",
+        "repos_exist_locally",
+        "modified",
+        "deps_synced_with_conf",
+    }
 
     vmn_ctx.params["deps_only"] = vmn_ctx.args.deps_only
 
     status = _get_repo_status(vmn_ctx.vcs, expected_status, optional_status)
     if status["error"]:
-        LOGGER.debug(
+        stamp_utils.VMN_LOGGER.debug(
             f"Error occured when getting the repo status: {status}", exc_info=True
         )
 
         return 1
 
-    if vmn_ctx.args.pull:
-        try:
-            vmn_ctx.vcs.retrieve_remote_changes()
-        except Exception as exc:
-            LOGGER.error("Failed to pull, run with --debug for more details")
-            LOGGER.debug("Logged Exception message:", exc_info=True)
-
-            return 1
-
-    return goto_version(vmn_ctx.vcs, vmn_ctx.params, vmn_ctx.args.version)
+    return goto_version(
+        vmn_ctx.vcs, vmn_ctx.params, vmn_ctx.args.version, vmn_ctx.args.pull
+    )
 
 
+@stamp_utils.measure_runtime_decorator
 def _get_repo_status(vcs, expected_status, optional_status=set()):
     be = vcs.backend
     default_status = {
         "pending": False,
         "detached": False,
         "outgoing": False,
         "state": set(),
         "error": False,
     }
     status = copy.deepcopy(default_status)
     status.update(
         {
             "repos_exist_locally": True,
+            "deps_synced_with_conf": True,
+            "repo_tracked": True,
+            "app_tracked": True,
             # TODO: rename to on_stamped_version and turn to True
             "modified": False,
             "dirty_deps": False,
-            "repo_tracked": True,
-            "app_tracked": True,
             "err_msgs": {
                 "dirty_deps": "",
+                "deps_synced_with_conf": "",
                 "repo_tracked": "vmn repo tracking is already initialized",
                 "app_tracked": "vmn app tracking is already initialized",
             },
             "repos": {},
             "matched_version_info": None,
             # Assumed state
-            "state": {"repos_exist_locally", "repo_tracked", "app_tracked"},
+            "state": {
+                "repos_exist_locally",
+                "deps_synced_with_conf",
+                "repo_tracked",
+                "app_tracked",
+            },
             "local_repos_diff": set(),
         }
     )
 
     path = os.path.join(vcs.vmn_root_path, ".vmn")
     if not vcs.tracked:
         status["app_tracked"] = False
@@ -1730,36 +1827,43 @@
             status["state"].add("modified")
         else:
             status["matched_version_info"] = matched_version_info
 
         configured_repos = set(vcs.configured_deps.keys())
         local_repos = set(vcs.actual_deps_state.keys())
 
-        if configured_repos - local_repos:
+        missing_deps = configured_repos - local_repos
+        if missing_deps:
             paths = []
-            for path in configured_repos - local_repos:
+            for path in missing_deps:
                 paths.append(os.path.join(vcs.vmn_root_path, path))
 
             status["repos_exist_locally"] = False
             status["err_msgs"]["repos_exist_locally"] = (
                 f"Dependency repository were specified in conf.yml file. "
                 f"However repos: {paths} do not exist. Please clone and rerun"
             )
-            status["local_repos_diff"] = configured_repos - local_repos
+            status["local_repos_diff"] = missing_deps
             status["state"].remove("repos_exist_locally")
 
         err = 0
-        for repo in configured_repos & local_repos:
+        common_deps = configured_repos & local_repos
+        for repo in common_deps:
+            # Skip local repo
             if repo == ".":
                 continue
 
             status["repos"][repo] = copy.deepcopy(default_status)
             full_path = os.path.join(vcs.vmn_root_path, repo)
 
             dep_be, err = stamp_utils.get_client(full_path, vcs.be_type)
+            if err:
+                err_str = "Failed to create backend {0}. Exiting".format(err)
+                stamp_utils.VMN_LOGGER.error(err)
+                raise RuntimeError(err)
 
             err = dep_be.check_for_pending_changes()
             if err:
                 status["dirty_deps"] = True
                 status["err_msgs"][
                     "dirty_deps"
                 ] = f"{status['err_msgs']['dirty_deps']}\n{err}"
@@ -1773,55 +1877,61 @@
                     err_msg = (
                         f"{repo} repository is on a different branch: "
                         f"{branch_name} than what is required by the configuration: "
                         f"{vcs.configured_deps[repo]['branch']}"
                     )
                     assert branch_name == vcs.configured_deps[repo]["branch"]
                 except Exception as exc:
-                    status["dirty_deps"] = True
+                    status["deps_synced_with_conf"] = False
                     status["err_msgs"][
-                        "dirty_deps"
-                    ] = f"{status['err_msgs']['dirty_deps']}\n{err_msg}"
-                    status["state"].add("dirty_deps")
-                    status["repos"][repo]["branch_error"] = True
-                    status["repos"][repo]["state"].add("branch_error")
+                        "deps_synced_with_conf"
+                    ] = f"{status['err_msgs']['deps_synced_with_conf']}\n{err_msg}"
+                    if "deps_synced_with_conf" in status["state"]:
+                        status["state"].remove("deps_synced_with_conf")
+
+                    status["repos"][repo]["branch_synced_error"] = True
+                    status["repos"][repo]["state"].add("not_synced_with_conf")
 
             if "tag" in vcs.configured_deps[repo]:
                 try:
                     err_msg = (
                         f"Repository in not on the requested tag by the configuration "
                         f"for {repo}."
                     )
                     c1 = dep_be.changeset(tag=vcs.configured_deps[repo]["tag"])
                     c2 = dep_be.changeset()
                     assert c1 == c2
                 except Exception as exc:
-                    status["dirty_deps"] = True
+                    status["deps_synced_with_conf"] = False
                     status["err_msgs"][
-                        "dirty_deps"
-                    ] = f"{status['err_msgs']['dirty_deps']}\n{err_msg}"
-                    status["state"].add("dirty_deps")
-                    status["repos"][repo]["tag_error"] = True
-                    status["repos"][repo]["state"].add("tag_error")
+                        "deps_synced_with_conf"
+                    ] = f"{status['err_msgs']['deps_synced_with_conf']}\n{err_msg}"
+                    if "deps_synced_with_conf" in status["state"]:
+                        status["state"].remove("deps_synced_with_conf")
+
+                    status["repos"][repo]["tag_synced_error"] = True
+                    status["repos"][repo]["state"].add("not_synced_with_conf")
 
             if "hash" in vcs.configured_deps[repo]:
                 try:
                     err_msg = (
                         f"Repository in not on the requested hash by the configuration "
                         f"for {repo}."
                     )
                     assert vcs.configured_deps[repo]["hash"] == dep_be.changeset()
                 except Exception as exc:
-                    status["dirty_deps"] = True
+                    status["deps_synced_with_conf"] = False
                     status["err_msgs"][
-                        "dirty_deps"
-                    ] = f"{status['err_msgs']['dirty_deps']}\n{err_msg}"
-                    status["state"].add("dirty_deps")
-                    status["repos"][repo]["tag_error"] = True
-                    status["repos"][repo]["state"].add("tag_error")
+                        "deps_synced_with_conf"
+                    ] = f"{status['err_msgs']['deps_synced_with_conf']}\n{err_msg}"
+                    if "deps_synced_with_conf" in status["state"]:
+                        status["state"].remove("deps_synced_with_conf")
+
+                    status["repos"][repo]["hash_synced_error"] = True
+                    status["repos"][repo]["state"].add("not_synced_with_conf")
 
             if not dep_be.in_detached_head():
                 err = dep_be.check_for_outgoing_changes()
                 if err:
                     status["dirty_deps"] = True
                     status["err_msgs"][
                         "dirty_deps"
@@ -1832,45 +1942,46 @@
             else:
                 status["repos"][repo]["detached"] = True
                 status["repos"][repo]["state"].add("detached")
 
     if (expected_status & status["state"]) != expected_status:
         for msg in expected_status - status["state"]:
             if msg in status["err_msgs"] and status["err_msgs"][msg]:
-                LOGGER.error(status["err_msgs"][msg])
+                stamp_utils.VMN_LOGGER.error(status["err_msgs"][msg])
 
         status["error"] = True
 
         return status
 
     if ((optional_status | status["state"]) - expected_status) != optional_status:
         for msg in (optional_status | status["state"]) - expected_status:
             if msg in status["err_msgs"] and status["err_msgs"][msg]:
-                LOGGER.error(status["err_msgs"][msg])
+                stamp_utils.VMN_LOGGER.error(status["err_msgs"][msg])
 
-        LOGGER.error(
+        stamp_utils.VMN_LOGGER.error(
             f"Repository status is in unexpected state:\n"
             f"{((optional_status | status['state']) - expected_status)}\n"
             f"versus optional:\n{optional_status}"
         )
 
         status["error"] = True
 
         return status
 
     return status
 
 
+@stamp_utils.measure_runtime_decorator
 def _init_app(versions_be_ifc, starting_version):
     optional_status = {"modified", "detached"}
-    expected_status = {"repos_exist_locally", "repo_tracked"}
+    expected_status = {"repos_exist_locally", "repo_tracked", "deps_synced_with_conf"}
 
     status = _get_repo_status(versions_be_ifc, expected_status, optional_status)
     if status["error"]:
-        LOGGER.debug(
+        stamp_utils.VMN_LOGGER.debug(
             f"Error occured when getting the repo status: {status}", exc_info=True
         )
 
         return 1
 
     versions_be_ifc.create_config_files()
 
@@ -1909,25 +2020,26 @@
         msg_root_app["services"][versions_be_ifc.name] = msg_app["_version"]
 
     try:
         err = versions_be_ifc.publish_stamp(
             starting_version, "release", {}, root_app_version
         )
     except Exception as exc:
-        LOGGER.debug("Logged Exception message: ", exc_info=True)
+        stamp_utils.VMN_LOGGER.debug("Logged Exception message: ", exc_info=True)
         versions_be_ifc.backend.revert_local_changes(versions_be_ifc.version_files)
         err = -1
 
     if err:
-        LOGGER.error("Failed to init app")
+        stamp_utils.VMN_LOGGER.error("Failed to init app")
         raise RuntimeError()
 
     return 0
 
 
+@stamp_utils.measure_runtime_decorator
 def _stamp_version(
     versions_be_ifc,
     pull,
     check_vmn_version,
     initial_version,
     initialprerelease,
     initialprerelease_count,
@@ -1936,27 +2048,29 @@
     retries = 3
     override_initial_version = initial_version
     override_initialprerelease = initialprerelease
     override_initialprerelease_count = initialprerelease_count
     override_main_current_version = versions_be_ifc.override_root_version
 
     if check_vmn_version:
-        newer_stamping = version_mod.version != "dev" and (
+        newer_stamping = version_mod.version != "0.0.0" and (
             pversion.parse(
                 versions_be_ifc.current_version_info["vmn_info"]["vmn_version"]
             )
             > pversion.parse(version_mod.version)
         )
 
         if newer_stamping:
-            LOGGER.error("Refusing to stamp with old vmn. Please upgrade")
+            stamp_utils.VMN_LOGGER.error(
+                "Refusing to stamp with old vmn. Please upgrade"
+            )
             raise RuntimeError()
 
     if versions_be_ifc.bad_format_template:
-        LOGGER.warning(versions_be_ifc.template_err_str)
+        stamp_utils.VMN_LOGGER.warning(versions_be_ifc.template_err_str)
 
     while retries:
         retries -= 1
 
         (
             current_version,
             prerelease,
@@ -1969,32 +2083,32 @@
         main_ver = versions_be_ifc.stamp_root_app_version(override_main_current_version)
 
         try:
             err = versions_be_ifc.publish_stamp(
                 current_version, prerelease, prerelease_count, main_ver
             )
         except Exception as exc:
-            LOGGER.error(
+            stamp_utils.VMN_LOGGER.error(
                 f"Failed to publish. Will revert local changes {exc}\nFor more details use --debug"
             )
-            LOGGER.debug("Exception info: ", exc_info=True)
+            stamp_utils.VMN_LOGGER.debug("Exception info: ", exc_info=True)
             versions_be_ifc.backend.revert_local_changes(versions_be_ifc.version_files)
             err = -1
 
         if not err:
             stamped = True
             break
 
         if err == 1:
             override_initial_version = current_version
             override_initialprerelease = prerelease
             override_initialprerelease_count = prerelease_count
             override_main_current_version = main_ver
 
-            LOGGER.warning(
+            stamp_utils.VMN_LOGGER.warning(
                 "Failed to publish. Will try to auto-increase "
                 "from {0} to {1}".format(
                     current_version,
                     versions_be_ifc.gen_advanced_version(
                         override_initial_version,
                         override_initialprerelease,
                         override_initialprerelease_count,
@@ -2002,30 +2116,34 @@
                 )
             )
         elif err == 2:
             if not pull:
                 break
 
             time.sleep(random.randint(1, 5))
-            versions_be_ifc.retrieve_remote_changes()
+            try:
+                versions_be_ifc.retrieve_remote_changes()
+            except Exception as exc:
+                stamp_utils.VMN_LOGGER.error("Failed to pull", exc_info=True)
         else:
             break
 
     if not stamped:
         err = "Failed to stamp"
-        LOGGER.error(err)
+        stamp_utils.VMN_LOGGER.error(err)
         raise RuntimeError(err)
 
     verstr = stamp_utils.VMNBackend.serialize_vmn_version(
         current_version, prerelease, prerelease_count, versions_be_ifc.hide_zero_hotfix
     )
 
     return versions_be_ifc.get_be_formatted_version(verstr)
 
 
+@stamp_utils.measure_runtime_decorator
 def show(vcs, params, verstr=None):
     dirty_states = None
     ver_infos = vcs.ver_infos_from_repo
     tag_name = vcs.selected_tag
     if verstr:
         tag_name, ver_infos = vcs.get_version_info_from_verstr(verstr)
 
@@ -2034,50 +2152,68 @@
         optional_status = {
             "repos_exist_locally",
             "detached",
             "pending",
             "outgoing",
             "modified",
             "dirty_deps",
+            "deps_synced_with_conf",
         }
         status = _get_repo_status(vcs, expected_status, optional_status)
         if status["error"]:
-            LOGGER.error("Error occured when getting the repo status")
-            LOGGER.debug(status, exc_info=True)
+            stamp_utils.VMN_LOGGER.error("Error occured when getting the repo status")
+            stamp_utils.VMN_LOGGER.debug(status, exc_info=True)
 
             raise RuntimeError()
 
         if tag_name in ver_infos:
             dirty_states = list(get_dirty_states(optional_status, status))
 
             if params["ignore_dirty"]:
                 dirty_states = None
 
             vers = []
             for i in ver_infos.keys():
                 vers.append(i.split("_")[-1])
+
             ver_infos[tag_name]["ver_info"]["stamping"]["app"]["versions"] = []
             ver_infos[tag_name]["ver_info"]["stamping"]["app"]["versions"].extend(vers)
 
     if tag_name not in ver_infos:
         ver_info = None
     else:
         ver_info = ver_infos[tag_name]["ver_info"]
 
     if ver_info is None:
-        LOGGER.info("Version information was not found " "for {0}.".format(vcs.name))
+        stamp_utils.VMN_LOGGER.info(
+            "Version information was not found " "for {0}.".format(vcs.name)
+        )
 
         raise RuntimeError()
 
     data = {}
 
+    if params["conf"]:
+        data["conf"] = {
+            "raw_deps": copy.deepcopy(vcs.raw_configured_deps),
+            "deps": copy.deepcopy(vcs.configured_deps),
+            "template": vcs.template,
+            "hide_zero_hotfix": vcs.hide_zero_hotfix,
+            "version_backends": copy.deepcopy(vcs.version_backends),
+        }
+
+    if params.get("display_type"):
+        data["type"] = ver_info["stamping"]["app"]["prerelease"]
+
     if vcs.root_context:
         data.update(ver_info["stamping"]["root_app"])
         if not data:
-            LOGGER.info("App {0} does not have a root app ".format(vcs.name))
+            stamp_utils.VMN_LOGGER.info(
+                "App {0} does not have a root app ".format(vcs.name)
+            )
 
             raise RuntimeError()
 
         out = None
         if params.get("verbose"):
             out = yaml.dump(data)
         else:
@@ -2125,81 +2261,95 @@
             d_out.update(
                 {
                     "out": out,
                     "type": data["prerelease"],
                 }
             )
 
+        if params.get("conf"):
+            d_out.update(
+                {
+                    "out": out,
+                    "conf": data["conf"],
+                }
+            )
+
         if d_out:
             out = yaml.safe_dump(d_out)
 
     print(out)
 
     return out
 
 
+@stamp_utils.measure_runtime_decorator
 def gen(vcs, params, verstr=None):
     expected_status = {"repo_tracked", "app_tracked"}
     optional_status = {
         "repos_exist_locally",
         "detached",
         "pending",
         "outgoing",
         "modified",
         "dirty_deps",
+        "deps_synced_with_conf",
     }
     status = _get_repo_status(vcs, expected_status, optional_status)
     if status["error"]:
-        LOGGER.error("Error occured when getting the repo status")
-        LOGGER.debug(status, exc_info=True)
+        stamp_utils.VMN_LOGGER.error("Error occured when getting the repo status")
+        stamp_utils.VMN_LOGGER.debug(status, exc_info=True)
 
         raise RuntimeError()
 
     if verstr is None:
         ver_infos = vcs.ver_infos_from_repo
         tag_name = vcs.selected_tag
     else:
         tag_name, ver_infos = vcs.get_version_info_from_verstr(verstr)
 
     if tag_name not in ver_infos or ver_infos[tag_name]["ver_info"] is None:
-        LOGGER.error("Version information was not found " "for {0}.".format(vcs.name))
+        stamp_utils.VMN_LOGGER.error(
+            "Version information was not found " "for {0}.".format(vcs.name)
+        )
 
         raise RuntimeError()
 
     dirty_states = get_dirty_states(optional_status, status)
     if params["verify_version"]:
         # TODO: check here what will happen when using "hotfix" octa
         if dirty_states:
-            LOGGER.error(
+            stamp_utils.VMN_LOGGER.error(
                 f"The repository and maybe some of its dependencies are in dirty state."
                 f"Dirty states found: {dirty_states}.\nError messages collected for dependencies:\n"
                 f"{status['err_msgs']['dirty_deps']}\n"
                 f"Refusing to gen."
             )
             raise RuntimeError()
 
         if (
             status["matched_version_info"] is not None
             and verstr is not None
             and status["matched_version_info"]["stamping"]["app"]["_version"]
         ):
-            LOGGER.error(
+            stamp_utils.VMN_LOGGER.error(
                 f"The repository is not exactly at version: {verstr}. "
                 f"You can use `vmn goto` in order to jump to that version.\n"
                 f"Refusing to gen."
             )
             raise RuntimeError()
 
     data = ver_infos[tag_name]["ver_info"]["stamping"]["app"]
     if verstr is None:
         data["changesets"] = {}
 
         for k, v in vcs.configured_deps.items():
             if k not in vcs.actual_deps_state:
-                LOGGER.error(f"{k} doesn't exist locally. Use vmn goto and rerun")
+                stamp_utils.VMN_LOGGER.error(
+                    f"{k} doesn't exist locally. Use vmn goto and rerun"
+                )
                 raise RuntimeError()
 
             data["changesets"][k] = copy.deepcopy(vcs.actual_deps_state[k])
             data["changesets"][k]["state"] = {"clean"}
 
             if status["repos"] and vcs.repo_name != k:
                 data["changesets"][k]["state"] = status["repos"][k]["state"]
@@ -2224,15 +2374,15 @@
         with open(params["custom_values"], "r") as f:
             ret = yaml.safe_load(f)
             tmplt_value.update(ret)
 
     with open(params["jinja_template"]) as file_:
         template = jinja2.Template(file_.read())
 
-    LOGGER.debug(
+    stamp_utils.VMN_LOGGER.debug(
         f"Possible keywords for your Jinja template:\n" f"{pformat(tmplt_value)}"
     )
     out = template.render(tmplt_value)
 
     out_path = params["output"]
 
     if os.path.exists(out_path):
@@ -2248,61 +2398,120 @@
 
 
 def get_dirty_states(optional_status, status):
     dirty_states = (optional_status & status["state"]) | {
         "repos_exist_locally",
         "detached",
     }
-    dirty_states -= {"detached", "repos_exist_locally"}
+    dirty_states -= {"detached", "repos_exist_locally", "deps_synced_with_conf"}
 
     try:
         debug_msg = ""
         for k in status["err_msgs"].keys():
             if k in dirty_states:
                 debug_msg = f"{debug_msg}\n{status['err_msgs'][k]}"
 
         if debug_msg:
-            LOGGER.debug(f"Debug for dirty states call:\n{debug_msg}")
+            stamp_utils.VMN_LOGGER.debug(f"Debug for dirty states call:{debug_msg}")
     except Exception as exc:
-        LOGGER.debug("Logged Exception message: ", exc_info=True)
+        stamp_utils.VMN_LOGGER.debug("Logged Exception message: ", exc_info=True)
         pass
 
     return dirty_states
 
 
-def goto_version(vcs, params, version):
+@stamp_utils.measure_runtime_decorator
+def goto_version(vcs, params, version, pull):
     unique_id = None
     check_unique = False
-    if version is not None:
-        # check for unique id
-        res = version.split("+")
-        if len(res) > 1:
-            version, unique_id = res
-            check_unique = True
+    status_str = ""
 
     if version is None:
+        if not params["deps_only"]:
+            ret = vcs.backend.checkout_branch()
+            assert ret is not None
+
+            if pull:
+                try:
+                    vcs.retrieve_remote_changes()
+                except Exception as exc:
+                    stamp_utils.VMN_LOGGER.error(
+                        "Failed to pull, run with --debug for more details"
+                    )
+                    stamp_utils.VMN_LOGGER.debug(
+                        "Logged Exception message:", exc_info=True
+                    )
+
+                    return 1
+
+                ret = vcs.backend.checkout_branch()
+                assert ret is not None
+
+            del vcs
+            vcs = VersionControlStamper(params)
+
         tag_name, ver_infos = vcs.backend.get_first_reachable_version_info(
             vcs.name, vcs.root_context, stamp_utils.RELATIVE_TO_CURRENT_VCS_BRANCH_TYPE
         )
+        if tag_name not in ver_infos or ver_infos[tag_name]["ver_info"] is None:
+            stamp_utils.VMN_LOGGER.error(f"No such app: {vcs.name}")
+            return 1
+
+        data = ver_infos[tag_name]["ver_info"]["stamping"]["app"]
+        deps = copy.deepcopy(vcs.configured_deps)
+
+        if not params["deps_only"]:
+            if vcs.root_context:
+                verstr = ver_infos[tag_name]["ver_info"]["stamping"]["root_app"][
+                    "version"
+                ]
+                status_str = f"You are at the tip of the branch of version {verstr} for {vcs.name}"
+            else:
+                status_str = f"You are at the tip of the branch of version {data['_version']} for {vcs.name}"
     else:
-        tag_name, ver_infos = vcs.get_version_info_from_verstr(version)
+        # check for unique id
+        res = version.split("+")
+        if len(res) > 1:
+            version, unique_id = res
+            check_unique = True
 
-    if tag_name not in ver_infos or ver_infos[tag_name]["ver_info"] is None:
-        LOGGER.error(f"No such app: {vcs.name}")
-        return 1
+        if not params["deps_only"] and pull:
+            try:
+                vcs.retrieve_remote_changes()
+            except Exception as exc:
+                stamp_utils.VMN_LOGGER.error(
+                    "Failed to pull, run with --debug for more details"
+                )
+                stamp_utils.VMN_LOGGER.debug("Logged Exception message:", exc_info=True)
 
-    data = ver_infos[tag_name]["ver_info"]["stamping"]["app"]
-    if version is not None:
+                return 1
+
+        tag_name, ver_infos = vcs.get_version_info_from_verstr(version)
+        if tag_name not in ver_infos or ver_infos[tag_name]["ver_info"] is None:
+            stamp_utils.VMN_LOGGER.error(f"No such app: {vcs.name}")
+            return 1
+
+        data = ver_infos[tag_name]["ver_info"]["stamping"]["app"]
         deps = copy.deepcopy(data["changesets"])
-    else:
-        deps = copy.deepcopy(vcs.configured_deps)
+
+        if not params["deps_only"]:
+            try:
+                vcs.backend.checkout(tag=tag_name)
+                status_str = f"You are at version {version} of {vcs.name}"
+            except Exception:
+                stamp_utils.VMN_LOGGER.error(
+                    "App: {0} with version: {1} was "
+                    "not found".format(vcs.name, version)
+                )
+
+                return 1
 
     if check_unique:
         if not deps["."]["hash"].startswith(unique_id):
-            LOGGER.error(f"Wrong unique id")
+            stamp_utils.VMN_LOGGER.error(f"Wrong unique id")
             return 1
 
     deps.pop(".")
     if deps:
         if version is None:
             for rel_path, v in deps.items():
                 v["hash"] = None
@@ -2313,144 +2522,142 @@
                     v["branch"] = None
                     v["tag"] = vcs.configured_deps[rel_path]["tag"]
                 if "hash" in vcs.configured_deps[rel_path]:
                     v["branch"] = None
                     v["tag"] = None
                     v["hash"] = vcs.configured_deps[rel_path]["hash"]
         try:
-            _goto_version(deps, vcs.vmn_root_path)
+            _goto_version(deps, vcs.vmn_root_path, pull)
         except Exception as exc:
-            LOGGER.error(f"goto failed: {exc}")
-            LOGGER.debug(f"", exc_info=True)
+            stamp_utils.VMN_LOGGER.error(f"goto failed: {exc}")
+            stamp_utils.VMN_LOGGER.debug(f"", exc_info=True)
 
             return 1
 
-    if version is None and not params["deps_only"]:
-        vcs.backend.checkout_branch()
-
-        if vcs.root_context:
-            verstr = ver_infos[tag_name]["ver_info"]["stamping"]["root_app"]["version"]
-            LOGGER.info(
-                f"You are at the tip of the branch of version {verstr} for {vcs.name}"
-            )
-        else:
-            LOGGER.info(
-                f"You are at the tip of the branch of version {data['_version']} for {vcs.name}"
-            )
-    elif not params["deps_only"]:
-        try:
-            vcs.backend.checkout(tag=tag_name)
-            LOGGER.info(f"You are at version {version} of {vcs.name}")
-        except Exception:
-            LOGGER.error(
-                "App: {0} with version: {1} was " "not found".format(vcs.name, version)
-            )
-
-            return 1
+    if status_str:
+        stamp_utils.VMN_LOGGER.info(status_str)
 
     return 0
 
 
+@stamp_utils.measure_runtime_decorator
 def _update_repo(args):
-    global LOGGER
     root_path = stamp_utils.resolve_root_path()
     vmn_path = os.path.join(root_path, ".vmn")
 
-    LOGGER = stamp_utils.init_stamp_logger(os.path.join(vmn_path, LOG_FILENAME))
+    stamp_utils.init_stamp_logger(os.path.join(vmn_path, LOG_FILENAME))
 
-    path, rel_path, branch_name, tag, changeset = args
+    path, rel_path, branch_name, tag, changeset, pull = args
 
     client = None
     try:
         if path == root_path:
             client, err = stamp_utils.get_client(path, "git", inherit_env=True)
         else:
             client, err = stamp_utils.get_client(path, "git")
 
+        # TODO:: why this is not an error?
         if client is None:
             return {"repo": rel_path, "status": 0, "description": err}
     except Exception as exc:
-        LOGGER.exception(
+        stamp_utils.VMN_LOGGER.exception(
             "Unexpected behaviour:\nAborting update " f"operation in {path} Reason:\n"
         )
 
         return {"repo": rel_path, "status": 1, "description": None}
 
     try:
         err = client.check_for_pending_changes()
         if err:
-            LOGGER.info("{0}. Aborting update operation ".format(err))
+            stamp_utils.VMN_LOGGER.info("{0}. Aborting update operation ".format(err))
             return {"repo": rel_path, "status": 1, "description": err}
 
     except Exception as exc:
-        LOGGER.debug(f'Skipping "{path}"')
-        LOGGER.debug("Exception info: ", exc_info=True)
+        stamp_utils.VMN_LOGGER.debug(f'Skipping "{path}"')
+        stamp_utils.VMN_LOGGER.debug("Exception info: ", exc_info=True)
 
         return {"repo": rel_path, "status": 0, "description": None}
 
     cur_changeset = client.changeset()
     try:
         if not client.in_detached_head():
             err = client.check_for_outgoing_changes()
             if err:
-                LOGGER.info("{0}. Aborting update operation".format(err))
+                stamp_utils.VMN_LOGGER.info(
+                    "{0}. Aborting update operation".format(err)
+                )
                 return {"repo": rel_path, "status": 1, "description": err}
 
-        LOGGER.info("Updating {0}".format(rel_path))
-        if changeset is None:
-            if not client.in_detached_head():
+        stamp_utils.VMN_LOGGER.info("Updating {0}".format(rel_path))
+
+        if pull:
+            try:
+                client.checkout_branch()
                 client.pull()
+            except Exception as exc:
+                stamp_utils.VMN_LOGGER.exception("Failed to pull:", exc_info=True)
+                return {"repo": rel_path, "status": 1, "description": "Failed to pull"}
 
+        if changeset is None:
             if tag is not None:
                 client.checkout(tag=tag)
-                LOGGER.info("Updated {0} to tag {1}".format(rel_path, tag))
+                stamp_utils.VMN_LOGGER.info(
+                    "Updated {0} to tag {1}".format(rel_path, tag)
+                )
             else:
                 rev = client.checkout_branch(branch_name=branch_name)
+                if rev is None:
+                    raise RuntimeError(f"Failed to checkout to branch {branch_name}")
+
                 if branch_name is not None:
-                    LOGGER.info(
+                    stamp_utils.VMN_LOGGER.info(
                         "Updated {0} to branch {1}".format(rel_path, branch_name)
                     )
                 else:
-                    LOGGER.info("Updated {0} to changeset {1}".format(rel_path, rev))
+                    stamp_utils.VMN_LOGGER.info(
+                        "Updated {0} to changeset {1}".format(rel_path, rev)
+                    )
         else:
-            if not client.in_detached_head():
-                client.pull()
-
             client.checkout(rev=changeset)
 
-            LOGGER.info("Updated {0} to {1}".format(rel_path, changeset))
+            stamp_utils.VMN_LOGGER.info(
+                "Updated {0} to {1}".format(rel_path, changeset)
+            )
     except Exception as exc:
-        LOGGER.exception(
+        stamp_utils.VMN_LOGGER.exception(
             f"Unexpected behaviour:\n"
-            f"Aborting update operation in {path} "
-            "Reason:\n"
+            f"Trying to abort update operation in {path} "
+            "Reason:\n",
+            exc_info=True,
         )
 
         try:
             client.checkout(rev=cur_changeset)
-        except Exception:
-            LOGGER.exception("Unexpected behaviour:")
+        except Exception as exc:
+            stamp_utils.VMN_LOGGER.exception(
+                "Unexpected behaviour when tried to revert:", exc_info=True
+            )
 
         return {"repo": rel_path, "status": 1, "description": None}
 
     return {"repo": rel_path, "status": 0, "description": None}
 
 
+@stamp_utils.measure_runtime_decorator
 def _clone_repo(args):
-    global LOGGER
     root_path = stamp_utils.resolve_root_path()
     vmn_path = os.path.join(root_path, ".vmn")
 
-    LOGGER = stamp_utils.init_stamp_logger(os.path.join(vmn_path, LOG_FILENAME))
+    stamp_utils.init_stamp_logger(os.path.join(vmn_path, LOG_FILENAME))
 
     path, rel_path, remote, vcs_type = args
     if os.path.exists(path):
         return {"repo": rel_path, "status": 0, "description": None}
 
-    LOGGER.info("Cloning {0}..".format(rel_path))
+    stamp_utils.VMN_LOGGER.info("Cloning {0}..".format(rel_path))
     try:
         if vcs_type == "git":
             stamp_utils.GitBackend.clone(path, remote)
     except Exception as exc:
         try:
             str = "already exists and is not an empty directory."
             if str in exc.stderr:
@@ -2462,19 +2669,20 @@
             rel_path, exc.args
         )
         return {"repo": rel_path, "status": 1, "description": err}
 
     return {"repo": rel_path, "status": 0, "description": None}
 
 
-def _goto_version(deps, vmn_root_path):
+@stamp_utils.measure_runtime_decorator
+def _goto_version(deps, vmn_root_path, pull):
     args = []
     for rel_path, v in deps.items():
         if "remote" not in v or not v["remote"]:
-            LOGGER.error(
+            stamp_utils.VMN_LOGGER.error(
                 "Failed to find a remote for a configured repository. Failing goto"
             )
             raise RuntimeError()
 
         # In case the remote is a local dir
         if v["remote"].startswith("."):
             v["remote"] = os.path.join(vmn_root_path, v["remote"])
@@ -2486,165 +2694,228 @@
                 v["remote"],
                 v["vcs_type"],
             )
         )
     with Pool(min(len(args), 10)) as p:
         results = p.map(_clone_repo, args)
 
+    err = False
+    failed_repos = set()
     for res in results:
         if res["status"] == 1:
+            err = True
+
             if res["repo"] is None and res["description"] is None:
                 continue
 
             msg = "Failed to clone "
             if res["repo"] is not None:
+                failed_repos.add(res["repo"])
                 msg += "from {0} ".format(res["repo"])
             if res["description"] is not None:
                 msg += "because {0}".format(res["description"])
 
-            LOGGER.info(msg)
+            stamp_utils.VMN_LOGGER.info(msg)
 
     args = []
     for rel_path, v in deps.items():
+        if rel_path in failed_repos:
+            continue
+
         branch = None
         if "branch" in v and v["branch"] is not None:
             branch = v["branch"]
         tag = None
         if "tag" in v and v["tag"] is not None:
             tag = v["tag"]
 
         args.append(
             (
                 os.path.join(vmn_root_path, rel_path),
                 rel_path,
                 branch,
                 tag,
                 v["hash"],
+                pull,
             )
         )
 
     with Pool(min(len(args), 20)) as p:
         results = p.map(_update_repo, args)
 
-    err = False
     for res in results:
         if res["status"] == 1:
             err = True
             if res["repo"] is None and res["description"] is None:
                 continue
 
             msg = "Failed to update "
             if res["repo"] is not None:
                 msg += " {0} ".format(res["repo"])
             if res["description"] is not None:
                 msg += "because {0}".format(res["description"])
 
-            LOGGER.warning(msg)
+            stamp_utils.VMN_LOGGER.warning(msg)
 
     if err:
-        LOGGER.error(
+        stamp_utils.VMN_LOGGER.error(
             "Failed to update one or more " "of the required repos. See log above"
         )
         raise RuntimeError()
 
 
+@stamp_utils.measure_runtime_decorator
 def main(command_line=None):
     # Please KEEP this function exactly like this
     # The purpose of this function is to keep the return
     # value to be an integer
     res, _ = vmn_run(command_line)
+
     return res
 
 
+@stamp_utils.measure_runtime_decorator
 def vmn_run(command_line=None):
-    global LOGGER
     try:
-        LOGGER = stamp_utils.init_stamp_logger()
+        stamp_utils.init_stamp_logger()
         args = parse_user_commands(command_line)
     except Exception as exc:
-        LOGGER.debug("Logged exception: ", exc_info=True)
+        stamp_utils.VMN_LOGGER.debug("Logged exception: ", exc_info=True)
         return 1, None
 
     try:
-        LOGGER = stamp_utils.init_stamp_logger(debug=args.debug)
+        stamp_utils.init_stamp_logger(debug=args.debug)
 
         root_path = stamp_utils.resolve_root_path()
         vmn_path = os.path.join(root_path, ".vmn")
         pathlib.Path(vmn_path).mkdir(parents=True, exist_ok=True)
 
-        LOGGER = stamp_utils.init_stamp_logger(
-            os.path.join(vmn_path, LOG_FILENAME), args.debug
-        )
     except Exception as exc:
-        LOGGER.error(
+        stamp_utils.VMN_LOGGER.error(
             "Failed to init logger. "
             "Maybe you are running from a non-managed directory?"
         )
-        LOGGER.debug("Logged exception: ", exc_info=True)
+        stamp_utils.VMN_LOGGER.debug("Logged exception: ", exc_info=True)
 
         return 1, None
 
-    command_line = copy.deepcopy(command_line)
-
+    err = 0
+    vmnc = None
     try:
+        lock_file_path = os.path.join(vmn_path, LOCK_FILENAME)
+        if LOCK_FILE_ENV in os.environ:
+            lock_file_path = os.environ[LOCK_FILE_ENV]
+
+        lock = FileLock(lock_file_path)
+
+        # start of non-parallel code section
+        lock.acquire()
+
+        stamp_utils.init_stamp_logger(os.path.join(vmn_path, LOG_FILENAME), args.debug)
+        command_line = copy.deepcopy(command_line)
+
         if command_line is None or not command_line:
             command_line = sys.argv
             if command_line is None:
                 command_line = ["vmn"]
 
         if not command_line[0].endswith("vmn"):
             command_line.insert(0, "vmn")
 
         bold_char = "\033[1m"
         end_char = "\033[0m"
-        LOGGER.debug(f"\n{bold_char}Command line: {' '.join(command_line)}{end_char}")
+        stamp_utils.VMN_LOGGER.debug(
+            f"\n{bold_char}Command line: {' '.join(command_line)}{end_char}"
+        )
+
+        # Call the actual function
+        err, vmnc = _vmn_run(args, root_path)
+        # We only need it here. In other, Exception cases -
+        # the unlock will happen naturally because the process will exit
+        lock.release()
 
-        return _vmn_run(args, root_path)
     except Exception as exc:
-        LOGGER.error("vmn_run raised exception. Run vmn --debug for details")
-        LOGGER.debug("Exception info: ", exc_info=True)
+        stamp_utils.VMN_LOGGER.error(
+            "vmn_run raised exception. Run vmn --debug for details"
+        )
+        stamp_utils.VMN_LOGGER.debug("Exception info: ", exc_info=True)
 
-        return 1, None
+        err = 1
     except:
-        LOGGER.debug("Exception info: ", exc_info=True)
-        return 1, None
+        stamp_utils.VMN_LOGGER.debug("Exception info: ", exc_info=True)
+        err = 1
+
+    return err, vmnc
 
 
+@stamp_utils.measure_runtime_decorator
 def _vmn_run(args, root_path):
-    err = 0
-    vmn_ctx = VMNContextMAnager(args, root_path)
-    with vmn_ctx:
-        if vmn_ctx.args.command in VMN_ARGS:
-            cmd = vmn_ctx.args.command.replace("-", "_")
-            err = getattr(sys.modules[__name__], f"handle_{cmd}")(vmn_ctx)
-        else:
-            LOGGER.info("Run vmn -h for help")
+    vmnc = VMNContainer(args, root_path)
+    if vmnc.args.command not in VMN_ARGS:
+        stamp_utils.VMN_LOGGER.info("Run vmn -h for help")
+        return 1, vmnc
+
+    if VMN_ARGS[vmnc.args.command] == "remote" or (
+            "pull" in vmnc.args and vmnc.args.pull
+    ):
+        err = vmnc.vcs.backend.prepare_for_remote_operation()
+        if err:
+            stamp_utils.VMN_LOGGER.error(
+                "Failed to run prepare for remote operation.\n"
+                "Check the log. Aborting remote operation."
+            )
+            return err, vmnc
+
+        if vmnc.vcs.name is not None:
+            # If there is no remote branch set, it is impossible
+            # to understand if there are outgoing changes. Thus this is required for
+            # remote operations.
+            # TODO:: verify that this assumaption is correct
+            configured_repos = set(vmnc.vcs.configured_deps.keys())
+            local_repos = set(vmnc.vcs.actual_deps_state.keys())
+            common_deps = configured_repos & local_repos
+            common_deps.remove(".")
+
+            for repo in common_deps:
+                full_path = os.path.join(vmnc.vcs.vmn_root_path, repo)
+
+                dep_be, err = stamp_utils.get_client(full_path, vmnc.vcs.be_type)
+                if err:
+                    err_str = "Failed to create backend {0}. Exiting".format(err)
+                    stamp_utils.VMN_LOGGER.error(err)
+                    raise RuntimeError(err)
+
+                dep_be.prepare_for_remote_operation()
+                del dep_be
+
+    cmd = vmnc.args.command.replace("-", "_")
+    err = getattr(sys.modules[__name__], f"handle_{cmd}")(vmnc)
 
-    return err, vmn_ctx
+    return err, vmnc
 
 
 def validate_app_name(args):
     if args.name.startswith("/"):
-        LOGGER.error("App name cannot start with /")
+        stamp_utils.VMN_LOGGER.error("App name cannot start with /")
         raise RuntimeError()
     if "-" in args.name:
-        LOGGER.error("App name cannot include -")
+        stamp_utils.VMN_LOGGER.error("App name cannot include -")
         raise RuntimeError()
 
 
 def parse_user_commands(command_line):
     parser = argparse.ArgumentParser("vmn")
     parser.add_argument(
         "--version", "-v", action="version", version=version_mod.version
     )
     parser.add_argument("--debug", required=False, action="store_true")
     parser.set_defaults(debug=False)
     subprasers = parser.add_subparsers(dest="command")
 
-    for arg in VMN_ARGS:
+    for arg in VMN_ARGS.keys():
         arg = arg.replace("-", "_")
         getattr(sys.modules[__name__], f"add_arg_{arg}")(subprasers)
 
     args = parser.parse_args(command_line)
 
     verify_user_input_version(args, "version")
     verify_user_input_version(args, "ov")
@@ -2775,14 +3046,16 @@
     pshow.add_argument(
         "-t", "--template", default=None, help="The template to use in show"
     )
     pshow.add_argument("--root", dest="root", action="store_true")
     pshow.set_defaults(root=False)
     pshow.add_argument("--verbose", dest="verbose", action="store_true")
     pshow.set_defaults(verbose=False)
+    pshow.add_argument("--conf", dest="conf", action="store_true")
+    pshow.set_defaults(conf=False)
     pshow.add_argument("--raw", dest="raw", action="store_true")
     pshow.set_defaults(raw=False)
     pshow.add_argument("--from-file", dest="from_file", action="store_true")
     pshow.set_defaults(from_file=False)
     pshow.add_argument("--ignore-dirty", dest="ignore_dirty", action="store_true")
     pshow.set_defaults(ignore_dirty=False)
     pshow.add_argument("-u", "--unique", dest="display_unique_id", action="store_true")
@@ -2870,15 +3143,15 @@
 
     if match is None:
         if "root" not in args or not args.root:
             err = f"Version must be in format: {stamp_utils.VMN_VERSION_FORMAT}"
         else:
             err = f"Root version must be an integer"
 
-        LOGGER.error(err)
+        stamp_utils.VMN_LOGGER.error(err)
 
         raise RuntimeError(err)
 
 
 if __name__ == "__main__":
     ret_err = main()
     if ret_err:
```

## Comparing `vmn-0.8.0rc8.dist-info/LICENSE.txt` & `vmn-0.8.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

