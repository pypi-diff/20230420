# Comparing `tmp/multi_repo_automation-0.2.0.tar.gz` & `tmp/multi_repo_automation-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_repo_automation-0.2.0.tar", max compression
+gzip compressed data, was "multi_repo_automation-0.3.0.tar", max compression
```

## Comparing `multi_repo_automation-0.2.0.tar` & `multi_repo_automation-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1284 2023-02-22 15:16:53.507914 multi_repo_automation-0.2.0/LICENSE
--rw-r--r--   0        0        0     2417 2023-02-22 15:16:53.507914 multi_repo_automation-0.2.0/README.md
--rw-r--r--   0        0        0    27568 2023-02-22 15:16:53.511914 multi_repo_automation-0.2.0/multi_repo_automation/__init__.py
--rw-r--r--   0        0        0     2126 2023-02-22 15:17:15.556100 multi_repo_automation-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3391 1970-01-01 00:00:00.000000 multi_repo_automation-0.2.0/setup.py
--rw-r--r--   0        0        0     3785 1970-01-01 00:00:00.000000 multi_repo_automation-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1284 2023-04-20 16:16:18.487034 multi_repo_automation-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2516 2023-04-20 16:16:18.487034 multi_repo_automation-0.3.0/README.md
+-rw-r--r--   0        0        0    26172 2023-04-20 16:16:18.487034 multi_repo_automation-0.3.0/multi_repo_automation/__init__.py
+-rw-r--r--   0        0        0    19015 2023-04-20 16:16:18.487034 multi_repo_automation-0.3.0/multi_repo_automation/editor.py
+-rw-r--r--   0        0        0     4901 2023-04-20 16:16:18.487034 multi_repo_automation-0.3.0/multi_repo_automation/tools.py
+-rw-r--r--   0        0        0     2249 2023-04-20 16:16:46.695219 multi_repo_automation-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3936 1970-01-01 00:00:00.000000 multi_repo_automation-0.3.0/PKG-INFO
```

### Comparing `multi_repo_automation-0.2.0/LICENSE` & `multi_repo_automation-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multi_repo_automation-0.2.0/README.md` & `multi_repo_automation-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,99 @@
 # Multi repo automation
 
-## Config
+## Configuration
 
-Create a file with something like this:
+To be able to apply your changes on multiple repository you should create a file with something like this:
 
 ```yaml
-- dir: /home/user/src/myrepo
-  name: user/myrepo
+- dir: /home/user/src/my-repo
+  name: user/my-repo
   types: ['javascript', 'python', 'docker']
   master_branch: master
   stabilization_branches: [1.0, 1.1]
   folders_to_clean: []
 ```
 
+The main configuration is a YAML file `~/.config/multi-repo-automation.yaml` with the following options:
+
+`repos_filename`: the filename of the files with the repositories definitions create above, default is `repos.yaml`.
+`browser`: the browser to use to open the pull requests, default is `xdg-open`.
+`editor`: the editor to use to edit files, default is `xdg-open`.
+
+## Migration script base
+
+```python
+#!/usr/bin/env python3
+
+import multi_repo_automation as mra
+
+def _do() -> None:
+    # Your actions
+
+if __name__ == "__main__":
+    mra.main(
+        _do,
+        config={
+        # pull_request_on_stabilization_branches: To apply the action on all stabilization (including master) branches.
+        # pull_request_title: The pull request title.
+        # pull_request_body: The pull request body.
+        # branch: The created branch branch name.
+        # pull_request_branch_prefix: The created branch prefix (used when we run it on all the stabilization branches).
+        },
+    )
+```
+
+Use the `--help` option to see the available options.
+
 ## Utilities
 
 ```python
 import multi_repo_automation as mra
 
 # Test if a file exists
 if mra.run(["git", "ls-files", "**/*.txt"], stdout=subprocess.PIPE).stdout.strip() != "":
   print("Found")
 # Get all YAML files:
 mra.all_filenames_identify("yaml")
 # Test if a file exists and contains a text
 if mra.git_grep(file, r"\<text\>"]):
   print("Found")
-# Edit a file in vscode
-mra.edit("file")
+# Edit a files manually
+mra.edit(["file"])
 ```
 
-## Genenric run
+### Edit file programmatically
 
 ```python
-#!/usr/bin/env python3
-import multi_repo_automation as mra
-
-
-def _do() -> None:
-    # Do something
-    pass
-
-if __name__ == "__main__":
-    mra.main(_do)
+   with mra.Edit('my-file.txt') as edit:
+      edit.content = edit.content.replace('<from>', '<to>')
 ```
 
-In the \_do function do the changes you want in your repo.
-
-Use the `--help` option to see the available options.
-
-## To update all the master branches write a script like
+### Edit YAML file programmatically
 
 ```python
-#!/usr/bin/env python3
-import multi_repo_automation as mra
-
-def _do() -> None:
-    # Do something
-    pass
-
-if __name__ == "__main__":
-    mra.main(
-        _do,
-        os.path.join(os.path.dirname(__file__), "repo.yaml"),
-        "/home/sbrunner/bin/firefox/firefox",
-        config={
-            "pull_request_branch": "branch_name",
-            "pull_request_title": "Commit/Pull request message",
-            "pull_request_body": "Optional body",
-        },
-    )
+   with mra.EditYAML('my-file.yaml') as edit:
+      edit.setdefault('dict', {})['prop'] = 'value'
 ```
 
-## To update all the stabilization branches write a script like
+### Edit TOML file programmatically
 
 ```python
-#!/usr/bin/env python3
-import multi_repo_automation as mra
+   with mra.EditTOML('my-file.toml') as edit:
+      edit.setdefault('dict', {})['prop'] = 'value'
+```
 
-def _do() -> None:
-    # Do something
-    pass
+### Edit Config file programmatically
 
-if __name__ == "__main__":
-    mra.main(
-        _do,
-        os.path.join(os.path.dirname(__file__), "repo.yaml"),
-        "/home/sbrunner/bin/firefox/firefox",
-        config={
-            "pull_request_on_stabilization_branches": True,
-            "pull_request_branch_prefix": "prefix",
-            "pull_request_title": "Commit/Pull request message",
-            "pull_request_body": "Optional body",
-        },
-    )
+```python
+   with mra.EditConfigL('my-file.ini') as edit:
+      edit.setdefault('dict', {})['prop'] = 'value'
 ```
 
-## Configuration
+## Contributing
 
-The configuration is a YAML file `~/.config/multi-repo-automation.yaml` with the following options:
+Install the pre-commit hooks:
 
-`repos_filename`: the filename of the files with the repositories definitions, default is `repos.yaml`.
-`browser`: the browser to use to open the pull requests, default is `xdg-open`.
+```bash
+pip install pre-commit
+pre-commit install --allow-missing-config
+```
```

### Comparing `multi_repo_automation-0.2.0/multi_repo_automation/__init__.py` & `multi_repo_automation-0.3.0/multi_repo_automation/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,59 +1,66 @@
 """Tools to automated changes on multiple repositories."""
 
 import argparse
-import io
 import os
 import re
-import shlex
 import shutil
 import subprocess  # nosec
-import sys
 import tempfile
-from types import TracebackType
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Iterator,
-    List,
-    Literal,
-    Optional,
-    Set,
-    Tuple,
-    Type,
-    TypedDict,
+import traceback
+from distutils.version import (  # pylint: disable=deprecated-module,useless-suppression
+    LooseVersion,
 )
+from types import TracebackType
+from typing import Any, Callable, Dict, List, Literal, Optional, Set, Tuple, Type, cast
 
 import requests
 import yaml
 from identify import identify
-from ruamel.yaml import YAML
+
+import multi_repo_automation.tools
+from multi_repo_automation.editor import (  # noqa
+    Edit,
+    EditConfig,
+    EditPreCommitConfig,
+    EditRenovateConfig,
+    EditTOML,
+    EditYAML,
+)
+from multi_repo_automation.tools import (  # noqa
+    Repo,
+    edit,
+    get_browser,
+    get_editor,
+    get_repo_config,
+    gh,
+    gh_json,
+    run,
+)
 
 CONFIG_FILENAME = "multi-repo-automation.yaml"
 
 if "APPDATA" in os.environ:
     CONFIG_FOLDER = os.environ["APPDATA"]
 elif "XDG_CONFIG_HOME" in os.environ:
     CONFIG_FOLDER = os.environ["XDG_CONFIG_HOME"]
 else:
     CONFIG_FOLDER = os.path.expanduser("~/.config")
 
 CONFIG_PATH = os.path.join(CONFIG_FOLDER, CONFIG_FILENAME)
 
 
-class Repo(TypedDict, total=False):
-    """The repository description."""
+_ARGUMENTS: Optional[argparse.Namespace] = None
+
 
-    dir: str
-    name: str
-    master_branch: str
-    stabilization_branches: List[str]
-    folders_to_clean: List[str]
-    clean: bool
+def get_arguments() -> argparse.Namespace:
+    """Get the global arguments."""
+
+    assert _ARGUMENTS is not None
+    return _ARGUMENTS
 
 
 def all_filenames(repo: Optional[Repo] = None) -> List[str]:
     """Get all the filenames of the repository."""
     cmd = ["git", "ls-files"]
     result = (
         run(cmd, stdout=subprocess.PIPE)
@@ -76,29 +83,14 @@
     result = []
     for filename in all_filenames(repo):
         if type_ in identify.tags_from_path(filename):
             result.append(filename)
     return result
 
 
-def run(cmd: List[str], exit_on_error: bool = True, **kwargs: Any) -> subprocess.CompletedProcess[str]:
-    """Run a command."""
-    print(shlex.join(cmd))
-    sys.stdout.flush()
-    if "stdout" in kwargs and kwargs["stdout"] == subprocess.PIPE and "encoding" not in kwargs:
-        kwargs["encoding"] = "utf-8"
-    process = subprocess.run(cmd, **kwargs)  # pylint: disable=subprocess-run-check # nosec
-
-    if process.returncode != 0:
-        print(f"Error on running: {shlex.join(cmd)}")
-        if exit_on_error:
-            sys.exit(process.returncode)
-    return process
-
-
 class Cwd:
     """
     Change the cwd in a with instruction.
 
     ```python with Cwd(repo):     # Do something in the repo ```
     """
 
@@ -114,14 +106,23 @@
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> Literal[False]:
         """Restore the cwd."""
+        del exc_tb
+
+        if exc_type is not None:
+            print("=" * 30)
+            print(type(self).__name__)
+            print(exc_type.__name__)
+            print(exc_val)
+            traceback.print_exc()
+
         os.chdir(self.cwd)
         return False
 
 
 class CreateBranch:
     """
     Create a branch in a with instruction.
@@ -149,122 +150,122 @@
     def __init__(
         self,
         repo: Repo,
         new_branch_name: str,
         commit_message: Optional[str] = None,
         force: bool = True,
         base_branch: Optional[str] = None,
-        pr_body: Optional[str] = None,
+        pull_request_body: Optional[str] = None,
     ) -> None:
         """Initialize."""
         self.repo = repo
         if base_branch is None:
             base_branch = repo.get("master_branch", "master")
         self.base_branch = base_branch
         self.new_branch_name = new_branch_name
         self.commit_message = commit_message
-        self.pr_body = pr_body
+        self.pull_request_body = pull_request_body
         self.force = force
         self.has_stashed = False
         self.pull_request_created = False
         self.old_branch_name = run(
             ["git", "rev-parse", "--abbrev-ref", "HEAD"],
             stdout=subprocess.PIPE,
         ).stdout.strip()
 
     def __enter__(self, *_: Any) -> None:
         """Create the branch."""
-        run(
-            [
-                "docker",
-                "run",
-                "--rm",
-                f"--volume={os.getcwd()}:/src",
-                "sbrunner/vim",
-                "chown",
-                f"{run(['id', '-u'], stdout=subprocess.PIPE).stdout.strip()}:"
-                f"{run(['id', '-g'], stdout=subprocess.PIPE).stdout.strip()}",
-                "-R",
-                ".",
-            ],
-        )
+        repo = self.repo.get("remote", "origin")
+        assert isinstance(repo, str)
+
         for folder in self.repo.get("folders_to_clean") or []:
             shutil.rmtree(folder, ignore_errors=True)
         if self.repo.get("clean", True):
-            run(["git", "clean", "-dfX"])
-            proc = run(["git", "stash", "--all"], stdout=subprocess.PIPE, encoding="utf-8", env={})
+            run(["git", "clean", "-dfX"], auto_fix_owner=True)
+            proc = run(
+                ["git", "stash", "--all", "--message=Stashed by multi repo automation"],
+                stdout=subprocess.PIPE,
+                exit_on_error=False,
+            )
             self.has_stashed = proc.stdout.strip() != "No local changes to save"
         else:
             proc = run(["git", "stash"], stdout=subprocess.PIPE, encoding="utf-8", env={})
             self.has_stashed = proc.stdout.strip() != "No local changes to save"
-        run(["git", "fetch"])
-        run(["git", "checkout", self.repo.get("master_branch") or "master"])
+        run(["git", "fetch", repo])
         if self.new_branch_name == self.old_branch_name:
-            run(["git", "reset", "--hard", f"origin/{self.new_branch_name}", "--"])
+            run(["git", "reset", "--hard", f"{repo}/{self.base_branch}", "--"])
         else:
-            run(["git", "branch", "--delete", "--force", self.new_branch_name], False)
+            run(["git", "branch", "--delete", "--force", self.new_branch_name], exit_on_error=False)
             run(
                 [
                     "git",
                     "checkout",
                     "-b",
                     self.new_branch_name,
-                    f"origin/{self.base_branch}",
+                    f"{repo}/{self.base_branch}",
                 ],
+                auto_fix_owner=True,
             )
         run(["git", "status"])
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> Literal[False]:
         """Create the pull request."""
-        del exc_val, exc_tb
+        del exc_tb
+
+        if exc_type is not None:
+            print("=" * 30)
+            print(type(self).__name__)
+            print(exc_type.__name__)
+            print(exc_val)
+            traceback.print_exc()
 
         if self.commit_message and exc_type is None:
             self.pull_request_created, self.message = create_pull_request(
                 self.repo,
                 self.commit_message,
                 force=self.force,
                 base_branch=self.base_branch,
-                body=self.pr_body,
+                body=self.pull_request_body,
             )
         if self.new_branch_name != self.old_branch_name:
             run(["git", "checkout", self.old_branch_name, "--"])
         if self.has_stashed:
             if run(["git", "stash", "pop"], False).returncode != 0:
                 run(["git", "reset", "--hard"])
         return False
 
 
 def create_pull_request(
     repo: Repo,
     title: Optional[str] = None,
     commit: bool = True,
-    label: str = "chore",
+    label: Optional[str] = None,
     body: Optional[str] = None,
     force: bool = True,
     base_branch: Optional[str] = None,
 ) -> Tuple[bool, str]:
     """Create a pull request."""
     run(["git", "status", "--short"])
     if not run(["git", "status", "--short"], stdout=subprocess.PIPE).stdout.strip():
         return False, ""
     if base_branch is None:
         base_branch = repo.get("master_branch", "master")
     cmd = [
         "gh",
         "pr",
         "create",
-        "--fill",
-        f"--label={label}",
         f"--base={base_branch}",
     ]
+    if label:
+        cmd.append(f"--label={label}")
     if commit:
         run(["git", "add", "--all"])
         assert title is not None  # nosec
         with tempfile.NamedTemporaryFile() as message_file:
             message_file.write(f"{title}\n".encode())
             if body is not None:
                 message_file.write(f"\n{body}\n".encode())
@@ -275,18 +276,29 @@
 
     if title is not None:
         cmd.extend(["--title", title])
         cmd.extend(["--body", body if body is not None else ""])
     else:
         cmd.append("--fill")
 
+    remote = repo.get("remote", "origin")
+    assert isinstance(remote, str)
+    branch_name = run(["git", "rev-parse", "--abbrev-ref", "HEAD"], stdout=subprocess.PIPE).stdout.strip()
     if force:
-        run(["git", "push", "--force"])
+        run(["git", "push", "--force", remote, f"HEAD:{branch_name}"])
     else:
-        run(["git", "push"])
+        run(["git", "push", remote, f"HEAD:{branch_name}"])
+    run(
+        [
+            "git",
+            "branch",
+            f"--set-upstream-to={remote}/{branch_name}",
+            branch_name,
+        ],
+    )
 
     url_proc = run(cmd, False, stdout=subprocess.PIPE)
     url = url_proc.stdout.strip()
     if url_proc.returncode != 0 or not url:
         url = f"https://github.com/{repo['name']}/pulls"
     elif re.match(r"https://github.com/camptocamp/tilecloud/pull/[0-9]+", url):
         url = f"{url}/tiles"
@@ -310,52 +322,53 @@
         self.old_branch_name = run(
             ["git", "rev-parse", "--abbrev-ref", "HEAD"],
             stdout=subprocess.PIPE,
         ).stdout.strip()
 
     def __enter__(self, *_: Any) -> None:
         """Create a new branch."""
-        run(
-            [
-                "docker",
-                "run",
-                "--rm",
-                f"--volume={os.getcwd()}:/src",
-                "sbrunner/vim",
-                "chown",
-                f"{run(['id', '-u'], stdout=subprocess.PIPE).stdout.strip()}:"
-                f"{run(['id', '-g'], stdout=subprocess.PIPE).stdout.strip()}",
-                "-R",
-                ".",
-            ],
-        )
         for folder in self.repo.get("folders_to_clean") or []:
             shutil.rmtree(folder, ignore_errors=True)
         if self.repo.get("clean", True):
             run(["git", "clean", "-dfX"])
             self.has_stashed = run(["git", "stash", "--all"], False).returncode == 0
         else:
             self.has_stashed = run(["git", "stash"], False).returncode == 0
 
         if self.old_branch_name != self.branch_name:
             run(["git", "branch", "--delete", "--force", self.branch_name], False)
             run(
-                ["git", "checkout", "-b", self.branch_name, "--track", f"origin/{self.branch_name}"],
+                [
+                    "git",
+                    "checkout",
+                    "-b",
+                    self.branch_name,
+                    f"{self.repo.get('remote', 'origin')}/{self.repo.get('master_branch', 'branch')}",
+                    "--track",
+                    f"{self.repo.get('remote', 'origin')}/{self.branch_name}",
+                ],
             )
         else:
-            run(["git", "pull", "--rebase"])
+            run(["git", "pull", self.repo.get("remote", "origin"), "--rebase"])
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> Literal[False]:
         """Exit."""
-        del exc_val, exc_tb
+        del exc_tb
+
+        if exc_type is not None:
+            print("=" * 30)
+            print(type(self).__name__)
+            print(exc_type.__name__)
+            print(exc_val)
+            traceback.print_exc()
 
         if exc_type is None and self.push:
             if self.force:
                 run(["git", "push", "--force"])
             else:
                 run(["git", "push"])
 
@@ -385,174 +398,53 @@
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> Literal[False]:
         """Commit the changes."""
-        del exc_val, exc_tb
+        del exc_tb
+
+        if exc_type is not None:
+            print("=" * 30)
+            print(type(self).__name__)
+            print(exc_type.__name__)
+            print(exc_val)
+            traceback.print_exc()
 
         if exc_type is None:
             if not run(["git", "status", "--short"], stdout=subprocess.PIPE).stdout.strip():
                 return False
             run(["git", "add", "--all"])
             with tempfile.NamedTemporaryFile() as message_file:
                 message_file.write(f"{self.commit_message}\n".encode())
                 message_file.flush()
                 if run(["git", "commit", f"--file={message_file.name}"], False).returncode != 0:
                     run(["git", "add", "--all"])
                     run(["git", "commit", "--no-verify", f"--file={message_file.name}"])
         return False
 
 
-class Edit:
-    r"""
-    Edit a file.
-
-    Usage:
-
-    ```python
-    with Edit("file.txt") as file:
-        file.content = "Header\n" + file.content
-    ```
-    """
-
-    def __init__(self, filename: str) -> None:
-        """Initialize."""
-        self.filename = filename
-        self.exists = os.path.exists(filename)
-        if not self.exists:
-            with open(filename, "w", encoding="utf-8") as opened_file:
-                pass
-        with open(self.filename, encoding="utf-8") as opened_file:
-            self.content = opened_file.read()
-
-    def __enter__(self) -> "Edit":
-        return self
-
-    def __exit__(
-        self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Literal[False]:
-        if not self.exists and not self.content:
-            os.remove(self.filename)
-            return False
-
-        with open(self.filename, "w", encoding="utf-8") as opened_file:
-            opened_file.write(self.content)
-
-        if os.path.exists(".pre-commit-config.yaml"):
-            run(["pre-commit", "run", "--files", self.filename], False)
-        return False
-
-
-class EditYAML:
-    """
-    Edit a YAML file by keeping the comments, in a with instruction.
-
-    ```python
-    with EditYAML("file.yaml") as yaml:
-        yaml["key"] = "value"
-    ```
-    """
-
-    original_data: Optional[str]
-
-    def __init__(
-        self, filename: str, width: int = 110, default_flow_style: bool = False, force: bool = False
-    ):
-        """Initialize the object."""
-        self.filename = filename
-        self.data: Dict[str, Any] = {}
-        self.yaml = YAML()
-        self.yaml.default_flow_style = default_flow_style
-        self.yaml.width = width  # type: ignore
-        self.force = force
-        self.exists = os.path.exists(filename)
-
-    def __enter__(self) -> "EditYAML":
-        """Load the file."""
-        if not self.exists:
-            with open(self.filename, encoding="utf-8") as file:
-                self.data = self.yaml.load(file)  # nosec
-        out = io.StringIO()
-        self.yaml.dump(self.data, out)
-        self.original_data = out.getvalue()
-        return self
-
-    def __exit__(
-        self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Literal[False]:
-        """Save the file if the data has changed."""
-        del exc_val, exc_tb
-        if exc_type is None:
-            if not self.exists and not self.data:
-                os.remove(self.filename)
-                return False
-
-            out = io.StringIO()
-            self.yaml.dump(self.data, out)
-            new_data = out.getvalue()
-            if self.force or new_data != self.original_data:
-                with open(self.filename, "w", encoding="utf-8") as file_:
-                    file_.write(new_data)
-                if os.path.exists(".pre-commit-config.yaml"):
-                    run(["pre-commit", "run", "--files", self.filename], False)
-        return False
-
-    def __getitem__(self, key: str) -> Any:
-        """Get the value for the key."""
-        return self.data[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        """Set the value for the key."""
-        self.data[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        """Delete the key."""
-        del self.data[key]
-
-    def __contains__(self, key: str) -> bool:
-        """Check if the key is in the data."""
-        return key in self.data
-
-    def __iter__(self) -> Iterator[str]:
-        """Iterate over the keys."""
-        return iter(self.data)
-
-    def __len__(self) -> int:
-        """Return the number of keys."""
-        return len(self.data)
-
-    def get(self, key: str, default: Any = None) -> Any:
-        """Get the value for the key."""
-        return self.data.get(key, default)
-
-    def setdefault(self, key: str, default: Any = None) -> Any:
-        """Set the default value for the key."""
-        return self.data.setdefault(key, default)
-
-
 def copy_file(from_: str, to_: str, only_if_already_exists: bool = True) -> None:
     """Copy a file."""
     if os.path.exists(to_):
         os.remove(to_)
         shutil.copyfile(from_, to_)
     elif not only_if_already_exists:
         shutil.copyfile(from_, to_)
 
 
 def git_grep(text: str, args: Optional[List[str]] = None) -> Set[str]:
     """Grep the code against the text."""
-    proc = run(["git", "grep", *(args or []), "--", text], stdout=subprocess.PIPE, encoding="utf-8")
+    proc = run(
+        ["git", "grep", *(args or []), "--", text],
+        exit_on_error=False,
+        stdout=subprocess.PIPE,
+        encoding="utf-8",
+    )
     files = set()
     for line in proc.stdout.split("\n"):
         if line and not line.startswith("Binary file "):
             print(f"{os.getcwd()}/{line}")
             files.add(line.split(":")[0])
     return files
 
@@ -562,70 +454,78 @@
     with open(filename, encoding="utf-8") as file_:
         content = file_.read()
     content = re.sub(search_text, replace_text, content)
     with open(filename, "w", encoding="utf-8") as file_:
         file_.write(content)
 
 
-def edit(files: List[str]) -> None:
-    """Edit the files in VSCode."""
-    for file in files:
-        print(os.path.abspath(file))
-        with open(file, "a", encoding="utf-8"):
-            pass
-        run(["code", file])
-        print("Press enter to continue")
-        input()
-        # Remove the file if he is empty
-        if os.stat(file).st_size == 0:
-            os.remove(file)
-
-
-def update_stabilization_branches(repo: Repo) -> None:
+def get_stabilization_versions(repo: Repo) -> List[str]:
     """
     Update the list of stabilization branches in the repo.
 
-    From the     `SECURITY.md` file.
+    From the `SECURITY.md` file.
     """
     import c2cciutils.security  # pylint: disable=import-outside-toplevel
 
+    stabilization_versions = []
     security_response = requests.get(
         f"https://raw.githubusercontent.com/{repo['name']}/{repo.get('master_branch', 'master')}/SECURITY.md",
         headers=c2cciutils.add_authorization_header({}),
-        timeout=int(os.environ.get("C2CCIUTILS_TIMEOUT", "30")),
+        timeout=30,
     )
     if security_response.ok:
         security = c2cciutils.security.Security(security_response.text)
 
         version_index = security.headers.index("Version")
         support_index = security.headers.index("Supported Until")
         versions = set()
         for data in security.data:
             if data[support_index] != "Unsupported" and data[version_index] != repo.get(
                 "master_branch", "master"
             ):
                 versions.add(data[version_index])
         if versions:
-            repo["stabilization_branches"] = list(versions)
+            stabilization_versions = list(versions)
+            stabilization_versions.sort(key=LooseVersion)
+    return stabilization_versions
 
-    for branch_name in repo.get("stabilization_branches") or []:
-        with Branch(repo, branch_name, push=False):
-            pass
+
+def get_stabilization_branches(repo: Repo) -> List[str]:
+    """
+    Update the list of stabilization branches in the repo.
+
+    From the     `SECURITY.md` file.
+    """
+
+    stabilization_versions = get_stabilization_versions(repo)
+    stabilization_version_to_branch: Dict[str, str] = repo.get("stabilization_version_to_branch", {})
+    return [stabilization_version_to_branch.get(v, v) for v in stabilization_versions]
+
+
+def update_stabilization_branches(repo: Repo) -> None:
+    """
+    Update the list of stabilization branches in the repo.
+
+    From the     `SECURITY.md` file.
+    """
+    stabilization_branches = get_stabilization_branches(repo)
+    if stabilization_branches:
+        repo["stabilization_branches"] = stabilization_branches
 
 
 def do_on_base_branches(
     repo: Repo, branch_prefix: str, func: Callable[[Repo], Optional[List[str]]]
 ) -> List[str]:
     """Do the func action on all the base branches of the repo."""
     result = set()
     branches = [*(repo.get("stabilization_branches") or []), repo.get("master_branch", "master")]
     for branch in branches:
         create_branch = CreateBranch(
             repo,
-            f"{branch_prefix}-{branch}",
+            f"{branch_prefix.rstrip('-')}-{branch}",
             "Fix pull requests check workflow, use our CI token",
             base_branch=branch,
         )
         with create_branch:
             func(repo)
         if create_branch.pull_request_created:
             if create_branch.message:
@@ -642,69 +542,71 @@
 
     To apply the conversion on all the repositories.
     """
 
     do_pr = False
     do_pr_on_stabilization_branches = False
     branch_prefix: Optional[str] = None
-    args: Any = None
     kwargs: Any = None
     local = False
     one = False
     repository_prefix: Optional[str] = None
 
     def __init__(self, repos: List[Repo], action: Callable[[], None], browser: str = "firefox") -> None:
         self.repos = repos
         self.action = action
         self.browser = browser
 
-    def init_pr(self, *args: Any, **kwargs: Any) -> None:
+    def init_pr(self, **kwargs: Any) -> None:
         """
         Configure to do create an pull request.
 
         On the master branch od all the repositories.
         """
         self.do_pr = True
-        self.args = args
         self.kwargs = kwargs
 
-    def init_pr_on_stabilization_branches(self, branch_prefix: str, *args: Any, **kwargs: Any) -> None:
+    def init_pr_on_stabilization_branches(self, branch_prefix: str, **kwargs: Any) -> None:
         """
         Configure to do create an pull request.
 
         On all the stabilization branches of all the repositories.
         """
         self.do_pr = True
         self.do_pr_on_stabilization_branches = True
         self.branch_prefix = branch_prefix
-        self.args = args
         self.kwargs = kwargs
 
     def run(self) -> None:
         """Run the conversion."""
+
         if self.local:
             self.action()
             return
         url_to_open = []
         try:
             for repo in self.repos:
+                multi_repo_automation.tools.set_repo_config(repo)
                 if self.repository_prefix is None or repo["name"].startswith(self.repository_prefix):
                     try:
                         print(f"=== {repo['name']} ===")
                         with Cwd(repo):
                             if self.do_pr:
                                 base_branches: Set[str] = {repo.get("master_branch", "master")}
                                 if self.do_pr_on_stabilization_branches:
                                     base_branches.update(repo.get("stabilization_branches") or [])
 
                                 for base_branch in base_branches:
                                     self.kwargs["base_branch"] = base_branch
                                     if self.do_pr_on_stabilization_branches:
-                                        self.kwargs["branch"] = f"{self.branch_prefix}-{base_branch}"
-                                    create_branch = CreateBranch(repo, *self.args, **self.kwargs)
+                                        assert self.branch_prefix is not None
+                                        self.kwargs[
+                                            "new_branch_name"
+                                        ] = f"{self.branch_prefix.rstrip('-')}-{base_branch}"
+                                    create_branch = CreateBranch(repo, **self.kwargs)
                                     with create_branch:
                                         self.action()
                                     if create_branch.pull_request_created:
                                         if create_branch.message:
                                             url_to_open.append(create_branch.message)
                                         else:
                                             url_to_open.append(f"https://github.com/{repo['name']}/pulls")
@@ -724,91 +626,136 @@
                 print(url)
 
 
 def main(
     action: Optional[Callable[[], None]] = None,
     description: str = "Apply an action on all the pre-configured repositories.",
     config: Optional[Dict[str, str]] = None,
+    add_arguments: Optional[Callable[[argparse.ArgumentParser], None]] = None,
 ) -> None:
     """Apply an action on all the repos."""
 
+    config = config or {}
     user_config = {}
     if os.path.exists(CONFIG_PATH):
         with open(CONFIG_PATH, encoding="utf-8") as config_file:
             user_config = yaml.load(config_file, Loader=yaml.SafeLoader)
     repos_filename: str = user_config.get("repos_filename", "repos.yaml")
-    browser: str = user_config.get("browser", "xdg-open")
 
     args_parser = argparse.ArgumentParser(description=description)
     args_parser_local = args_parser.add_argument_group("local", "To apply the action locally.")
     args_parser_local.add_argument("--local", action="store_true", help="Enable it.")
 
     args_parser_repos = args_parser.add_argument_group(
         "repos", "Option used to browse all the repositories, and create pull request with the result."
     )
     args_parser_repos.add_argument(
         "--repositories", default=repos_filename, help="A YAML file that contains the repositories."
     )
     args_parser_repos.add_argument("--repository-prefix", help="Apply on repository with prefix.")
     args_parser_repos.add_argument("--one", action="store_true", help="Open only one pull request.")
-    if config is None:
-        args_parser_repos.add_argument("--pull-request-title", help="The pull request title.")
-        args_parser_repos.add_argument("--pull-request-body", help="The pull request body.")
-        args_parser_master = args_parser.add_argument_group(
-            "master", "To apply the action on all master branches."
-        )
-        args_parser_master.add_argument("--branch", help="The created branch branch name.")
-        args_parser_stabilization = args_parser.add_argument_group(
-            "stabilization", "To apply the action on all stabilization (including master) branches."
-        )
+    args_parser_repos.add_argument(
+        "--pull-request-title", help="The pull request title.", default=config.get("pull_request_title", None)
+    )
+    args_parser_repos.add_argument(
+        "--pull-request-body", help="The pull request body.", default=config.get("pull_request_body", None)
+    )
+    args_parser_master = args_parser.add_argument_group(
+        "master", "To apply the action on all master branches."
+    )
+    args_parser_master.add_argument(
+        "--branch", help="The created branch branch name.", default=config.get("branch", None)
+    )
+    args_parser_stabilization = args_parser.add_argument_group(
+        "stabilization", "To apply the action on all stabilization (including master) branches."
+    )
+    if "pull_request_on_stabilization_branches" not in config:
         args_parser_stabilization.add_argument(
             "--on-stabilization-branches",
             action="store_true",
             help="Enable it.",
         )
-        args_parser_stabilization.add_argument("--branch-prefix", help="The created branch prefix.")
+    args_parser_stabilization.add_argument(
+        "--branch-prefix",
+        help="The created branch prefix.",
+        default=config.get("pull_request_branch_prefix", None),
+    )
     args_parser_repos.add_argument(
-        "--browser", default=browser, help="The browser used to open the created pull requests"
+        "--browser",
+        default=user_config.get("browser", "xdg-open"),
+        help="The browser used to open the created pull requests",
+    )
+    args_parser_repos.add_argument(
+        "--editor", default=user_config.get("editor", "xdg-open"), help="The editor used to open the files"
     )
     if action is None:
         args_parser.add_argument("command", help="The command to run.")
+
+    if add_arguments is not None:
+        add_arguments(args_parser)
+
     args = args_parser.parse_args()
+    global _ARGUMENTS  # pylint: disable=global-statement
+    _ARGUMENTS = args
 
-    if config is None:
-        pull_request_on_stabilization_branches = args.on_stabilization_branches
-        pull_request_title = args.pull_request_title
-        pull_request_body = args.pull_request_body
-        pull_request_branch = args.branch
-        pull_request_branch_prefix = args.branch_prefix
-    else:
-        pull_request_on_stabilization_branches = config.get("pull_request_on_stabilization_branches", False)
-        pull_request_title = config.get("pull_request_title", None)
-        pull_request_body = config.get("pull_request_body", None)
-        pull_request_branch = config.get("branch", None)
-        pull_request_branch_prefix = config.get("pull_request_branch_prefix", None)
+    pull_request_on_stabilization_branches = (
+        config["pull_request_on_stabilization_branches"]
+        if "pull_request_on_stabilization_branches" in config
+        else args.on_stabilization_branches
+    )
+    pull_request_title = args.pull_request_title
+    pull_request_body = args.pull_request_body
+    pull_request_branch = args.branch
+    pull_request_branch_prefix = args.branch_prefix
 
     repos = []
     if not args.local:
         with open(args.repositories, encoding="utf-8") as opened_file:
             repos = yaml.load(opened_file.read(), Loader=yaml.SafeLoader)
 
     if action is None:
 
         def action() -> None:
             run([args.command])
 
+    multi_repo_automation.tools.set_browser(args.browser)
+    multi_repo_automation.tools.set_editor(args.editor)
+
     app = App(repos, action, browser=args.browser)
     app.one = args.one
     app.repository_prefix = args.repository_prefix
     if args.local:
         app.local = True
     elif pull_request_on_stabilization_branches:
         app.init_pr_on_stabilization_branches(
-            pull_request_branch_prefix, pull_request_title, pull_request_body
+            branch_prefix=pull_request_branch_prefix,
+            commit_message=pull_request_title,
+            pull_request_body=pull_request_body,
         )
     elif pull_request_branch:
-        app.init_pr(pull_request_branch, pull_request_title, pull_request_body)
+        app.init_pr(
+            new_branch_name=pull_request_branch,
+            commit_message=pull_request_title,
+            pull_request_body=pull_request_body,
+        )
     app.run()
 
 
-if __name__ == "__main__":
-    main()
+def update_stabilization_branches_main() -> None:
+    """Update the stabilization branches."""
+    user_config = {}
+    if os.path.exists(CONFIG_PATH):
+        with open(CONFIG_PATH, encoding="utf-8") as config_file:
+            user_config = yaml.load(config_file, Loader=yaml.SafeLoader)
+    repos_filename: str = user_config.get("repos_filename", "repos.yaml")
+
+    args_parser = argparse.ArgumentParser(description="Update the stabilization branches.")
+    args_parser.add_argument(
+        "--repositories", default=repos_filename, help="A YAML file that contains the repositories."
+    )
+    args_parser.add_argument("--diff", action="store_true", help="Only show the diff")
+    args = args_parser.parse_args()
+
+    with EditYAML(args.repositories, diff=args.diff, run_pre_commit=False) as repos:
+        assert isinstance(repos, EditYAML)
+        for repo in repos:
+            update_stabilization_branches(cast(Repo, repo))
```

### Comparing `multi_repo_automation-0.2.0/pyproject.toml` & `multi_repo_automation-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 [tool.mypy]
 python_version = 3.8
 ignore_missing_imports = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 strict = true
-plugins = ["numpy.typing.mypy_plugin"]
 
 [tool.poetry]
 name = "multi-repo-automation"
-version = "0.2.0"
+version = "0.3.0"
 description = "Library for automation updates on multiple repositories."
 readme = "README.md"
 keywords = ["pre-commit"]
 license = "BSD-2-Clause"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
@@ -37,24 +36,29 @@
 repository = "https://github.com/sbrunner/multi-repo-automation"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 PyYAML = "6.0"
 requests = "2.28.2"
 "ruamel.yaml" = "0.17.21"
-identify = "2.5.17"
-c2cciutils = { version = "1.4.7", optional = true }
+identify = "2.5.22"
+c2cciutils = { version = "1.5.2", optional = true }
+tomlkit = "0.11.7"
+configupdater = "3.1.1"
 
 [tool.poetry.extras]
 update_stabilization_branches = ["c2cciutils"]
 
 [tool.poetry.group.dev.dependencies]
-prospector = { extras = ["with_bandit", "with_mypy", "with_pyroma"], version = "1.8.4" }
-types-PyYAML = "6.0.12.3"
-types-requests = "2.28.11.8"
+prospector = { extras = ["with_bandit", "with_mypy", "with_pyroma"], version = "1.9.0" }
+types-PyYAML = "6.0.12.9"
+types-requests = "2.28.11.17"
+
+[tool.poetry.scripts]
+mra-update-stabilization-branches = 'multi_repo_automation:update_stabilization_branches_main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "poetry-plugin-tweak-dependencies-version"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `multi_repo_automation-0.2.0/PKG-INFO` & `multi_repo_automation-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-repo-automation
-Version: 0.2.0
+Version: 0.3.0
 Summary: Library for automation updates on multiple repositories.
 Home-page: https://github.com/sbrunner/multi-repo-automation
 License: BSD-2-Clause
 Keywords: pre-commit
 Author: Stéphane Brunner
 Author-email: stephane.brunner@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -22,118 +22,115 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Provides-Extra: update-stabilization-branches
 Requires-Dist: PyYAML
 Requires-Dist: c2cciutils ; extra == "update-stabilization-branches"
+Requires-Dist: configupdater
 Requires-Dist: identify
 Requires-Dist: requests
 Requires-Dist: ruamel.yaml
+Requires-Dist: tomlkit
 Project-URL: Repository, https://github.com/sbrunner/multi-repo-automation
 Description-Content-Type: text/markdown
 
 # Multi repo automation
 
-## Config
+## Configuration
 
-Create a file with something like this:
+To be able to apply your changes on multiple repository you should create a file with something like this:
 
 ```yaml
-- dir: /home/user/src/myrepo
-  name: user/myrepo
+- dir: /home/user/src/my-repo
+  name: user/my-repo
   types: ['javascript', 'python', 'docker']
   master_branch: master
   stabilization_branches: [1.0, 1.1]
   folders_to_clean: []
 ```
 
+The main configuration is a YAML file `~/.config/multi-repo-automation.yaml` with the following options:
+
+`repos_filename`: the filename of the files with the repositories definitions create above, default is `repos.yaml`.
+`browser`: the browser to use to open the pull requests, default is `xdg-open`.
+`editor`: the editor to use to edit files, default is `xdg-open`.
+
+## Migration script base
+
+```python
+#!/usr/bin/env python3
+
+import multi_repo_automation as mra
+
+def _do() -> None:
+    # Your actions
+
+if __name__ == "__main__":
+    mra.main(
+        _do,
+        config={
+        # pull_request_on_stabilization_branches: To apply the action on all stabilization (including master) branches.
+        # pull_request_title: The pull request title.
+        # pull_request_body: The pull request body.
+        # branch: The created branch branch name.
+        # pull_request_branch_prefix: The created branch prefix (used when we run it on all the stabilization branches).
+        },
+    )
+```
+
+Use the `--help` option to see the available options.
+
 ## Utilities
 
 ```python
 import multi_repo_automation as mra
 
 # Test if a file exists
 if mra.run(["git", "ls-files", "**/*.txt"], stdout=subprocess.PIPE).stdout.strip() != "":
   print("Found")
 # Get all YAML files:
 mra.all_filenames_identify("yaml")
 # Test if a file exists and contains a text
 if mra.git_grep(file, r"\<text\>"]):
   print("Found")
-# Edit a file in vscode
-mra.edit("file")
+# Edit a files manually
+mra.edit(["file"])
 ```
 
-## Genenric run
+### Edit file programmatically
 
 ```python
-#!/usr/bin/env python3
-import multi_repo_automation as mra
-
-
-def _do() -> None:
-    # Do something
-    pass
-
-if __name__ == "__main__":
-    mra.main(_do)
+   with mra.Edit('my-file.txt') as edit:
+      edit.content = edit.content.replace('<from>', '<to>')
 ```
 
-In the \_do function do the changes you want in your repo.
-
-Use the `--help` option to see the available options.
-
-## To update all the master branches write a script like
+### Edit YAML file programmatically
 
 ```python
-#!/usr/bin/env python3
-import multi_repo_automation as mra
-
-def _do() -> None:
-    # Do something
-    pass
-
-if __name__ == "__main__":
-    mra.main(
-        _do,
-        os.path.join(os.path.dirname(__file__), "repo.yaml"),
-        "/home/sbrunner/bin/firefox/firefox",
-        config={
-            "pull_request_branch": "branch_name",
-            "pull_request_title": "Commit/Pull request message",
-            "pull_request_body": "Optional body",
-        },
-    )
+   with mra.EditYAML('my-file.yaml') as edit:
+      edit.setdefault('dict', {})['prop'] = 'value'
 ```
 
-## To update all the stabilization branches write a script like
+### Edit TOML file programmatically
 
 ```python
-#!/usr/bin/env python3
-import multi_repo_automation as mra
+   with mra.EditTOML('my-file.toml') as edit:
+      edit.setdefault('dict', {})['prop'] = 'value'
+```
 
-def _do() -> None:
-    # Do something
-    pass
+### Edit Config file programmatically
 
-if __name__ == "__main__":
-    mra.main(
-        _do,
-        os.path.join(os.path.dirname(__file__), "repo.yaml"),
-        "/home/sbrunner/bin/firefox/firefox",
-        config={
-            "pull_request_on_stabilization_branches": True,
-            "pull_request_branch_prefix": "prefix",
-            "pull_request_title": "Commit/Pull request message",
-            "pull_request_body": "Optional body",
-        },
-    )
+```python
+   with mra.EditConfigL('my-file.ini') as edit:
+      edit.setdefault('dict', {})['prop'] = 'value'
 ```
 
-## Configuration
+## Contributing
 
-The configuration is a YAML file `~/.config/multi-repo-automation.yaml` with the following options:
+Install the pre-commit hooks:
 
-`repos_filename`: the filename of the files with the repositories definitions, default is `repos.yaml`.
-`browser`: the browser to use to open the pull requests, default is `xdg-open`.
+```bash
+pip install pre-commit
+pre-commit install --allow-missing-config
+```
```

