# Comparing `tmp/esprepomanager-1.0.0.tar.gz` & `tmp/esprepomanager-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esprepomanager-1.0.0.tar", last modified: Fri Apr 14 20:28:18 2023, max compression
+gzip compressed data, was "esprepomanager-1.1.0.tar", last modified: Thu Apr 20 15:27:27 2023, max compression
```

## Comparing `esprepomanager-1.0.0.tar` & `esprepomanager-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-14 20:28:18.794424 esprepomanager-1.0.0/
--rw-r--r--   0 tobias    (1012) familie    (155)    35149 2023-04-11 14:23:15.000000 esprepomanager-1.0.0/LICENSE
--rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-14 20:28:18.794424 esprepomanager-1.0.0/PKG-INFO
--rw-r--r--   0 tobias    (1012) familie    (155)      127 2023-04-14 20:13:12.000000 esprepomanager-1.0.0/README.md
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-14 20:28:18.794424 esprepomanager-1.0.0/esprepomanager/
--rw-rw-r--   0 tobias    (1012) familie    (155)    13625 2023-04-14 19:59:45.000000 esprepomanager-1.0.0/esprepomanager/__init__.py
--rw-r--r--   0 tobias    (1012) familie    (155)      146 2023-04-11 14:32:23.000000 esprepomanager-1.0.0/esprepomanager/__main__.py
--rw-r--r--   0 tobias    (1012) familie    (155)    10644 2023-04-14 17:25:28.000000 esprepomanager-1.0.0/esprepomanager/config.py
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-14 20:28:18.794424 esprepomanager-1.0.0/esprepomanager/gitlab/
--rw-r--r--   0 tobias    (1012) familie    (155)     6496 2023-04-14 20:16:08.000000 esprepomanager-1.0.0/esprepomanager/gitlab/__init__.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1915 2023-04-14 16:46:47.000000 esprepomanager-1.0.0/esprepomanager/gitlab/group.py
--rw-r--r--   0 tobias    (1012) familie    (155)     6442 2023-04-14 20:17:05.000000 esprepomanager-1.0.0/esprepomanager/gitlab/project.py
--rw-r--r--   0 tobias    (1012) familie    (155)      439 2023-04-13 01:24:15.000000 esprepomanager-1.0.0/esprepomanager/gitlab/user.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1850 2023-04-13 22:10:58.000000 esprepomanager-1.0.0/esprepomanager/person.py
--rw-r--r--   0 tobias    (1012) familie    (155)      678 2023-04-12 20:47:34.000000 esprepomanager-1.0.0/esprepomanager/repo.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1594 2023-04-14 15:42:33.000000 esprepomanager-1.0.0/esprepomanager/team.py
--rw-r--r--   0 tobias    (1012) familie    (155)     3887 2023-04-14 18:31:34.000000 esprepomanager-1.0.0/esprepomanager/utils.py
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-14 20:28:18.794424 esprepomanager-1.0.0/esprepomanager.egg-info/
--rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-14 20:28:18.000000 esprepomanager-1.0.0/esprepomanager.egg-info/PKG-INFO
--rw-rw-r--   0 tobias    (1012) familie    (155)      558 2023-04-14 20:28:18.000000 esprepomanager-1.0.0/esprepomanager.egg-info/SOURCES.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)        1 2023-04-14 20:28:18.000000 esprepomanager-1.0.0/esprepomanager.egg-info/dependency_links.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       55 2023-04-14 20:28:18.000000 esprepomanager-1.0.0/esprepomanager.egg-info/entry_points.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       14 2023-04-14 20:28:18.000000 esprepomanager-1.0.0/esprepomanager.egg-info/requires.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       15 2023-04-14 20:28:18.000000 esprepomanager-1.0.0/esprepomanager.egg-info/top_level.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       38 2023-04-14 20:28:18.794424 esprepomanager-1.0.0/setup.cfg
--rw-rw-r--   0 tobias    (1012) familie    (155)      768 2023-04-14 20:26:20.000000 esprepomanager-1.0.0/setup.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-20 15:27:27.645192 esprepomanager-1.1.0/
+-rw-r--r--   0 tobias    (1012) familie    (155)    35149 2023-04-11 14:23:15.000000 esprepomanager-1.1.0/LICENSE
+-rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-20 15:27:27.641192 esprepomanager-1.1.0/PKG-INFO
+-rw-r--r--   0 tobias    (1012) familie    (155)      127 2023-04-14 20:13:12.000000 esprepomanager-1.1.0/README.md
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-20 15:27:27.641192 esprepomanager-1.1.0/esprepomanager/
+-rw-rw-r--   0 tobias    (1012) familie    (155)    13625 2023-04-20 15:25:44.000000 esprepomanager-1.1.0/esprepomanager/__init__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      146 2023-04-11 14:32:23.000000 esprepomanager-1.1.0/esprepomanager/__main__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)    10644 2023-04-14 17:25:28.000000 esprepomanager-1.1.0/esprepomanager/config.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-20 15:27:27.641192 esprepomanager-1.1.0/esprepomanager/gitlab/
+-rw-r--r--   0 tobias    (1012) familie    (155)     6496 2023-04-14 20:16:08.000000 esprepomanager-1.1.0/esprepomanager/gitlab/__init__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1915 2023-04-14 16:46:47.000000 esprepomanager-1.1.0/esprepomanager/gitlab/group.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     7260 2023-04-20 15:25:33.000000 esprepomanager-1.1.0/esprepomanager/gitlab/project.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      439 2023-04-13 01:24:15.000000 esprepomanager-1.1.0/esprepomanager/gitlab/user.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1850 2023-04-13 22:10:58.000000 esprepomanager-1.1.0/esprepomanager/person.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      678 2023-04-12 20:47:34.000000 esprepomanager-1.1.0/esprepomanager/repo.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1594 2023-04-14 15:42:33.000000 esprepomanager-1.1.0/esprepomanager/team.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     3887 2023-04-14 18:31:34.000000 esprepomanager-1.1.0/esprepomanager/utils.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-20 15:27:27.641192 esprepomanager-1.1.0/esprepomanager.egg-info/
+-rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-20 15:27:27.000000 esprepomanager-1.1.0/esprepomanager.egg-info/PKG-INFO
+-rw-rw-r--   0 tobias    (1012) familie    (155)      558 2023-04-20 15:27:27.000000 esprepomanager-1.1.0/esprepomanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)        1 2023-04-20 15:27:27.000000 esprepomanager-1.1.0/esprepomanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       55 2023-04-20 15:27:27.000000 esprepomanager-1.1.0/esprepomanager.egg-info/entry_points.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       14 2023-04-20 15:27:27.000000 esprepomanager-1.1.0/esprepomanager.egg-info/requires.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       15 2023-04-20 15:27:27.000000 esprepomanager-1.1.0/esprepomanager.egg-info/top_level.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       38 2023-04-20 15:27:27.645192 esprepomanager-1.1.0/setup.cfg
+-rw-rw-r--   0 tobias    (1012) familie    (155)      768 2023-04-20 14:32:14.000000 esprepomanager-1.1.0/setup.py
```

### Comparing `esprepomanager-1.0.0/LICENSE` & `esprepomanager-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.0.0/PKG-INFO` & `esprepomanager-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esprepomanager
-Version: 1.0.0
+Version: 1.1.0
 Summary: manager for git repos
 Home-page: https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager
 Author: Teichi
 Author-email: tobias@teichmann.top
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `esprepomanager-1.0.0/esprepomanager/__init__.py` & `esprepomanager-1.1.0/esprepomanager/__init__.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.0.0/esprepomanager/config.py` & `esprepomanager-1.1.0/esprepomanager/config.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.0.0/esprepomanager/gitlab/__init__.py` & `esprepomanager-1.1.0/esprepomanager/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.0.0/esprepomanager/gitlab/group.py` & `esprepomanager-1.1.0/esprepomanager/gitlab/group.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.0.0/esprepomanager/gitlab/project.py` & `esprepomanager-1.1.0/esprepomanager/gitlab/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,14 +96,31 @@
     def members(self) -> List[User]:
         resp = self.send_request("GET", "members", params_={"per_page": "100"})
         if not resp.ok:
             log.debug(resp.json())
             return []
         return [User.from_json(x) for x in resp.json()]
 
+    def set_protected_branch(self, branch: str, access: int, allow_force: bool = False) -> bool:
+        resp = self.send_request("POST", "protected_branches", params_={
+            "name": branch,
+            "allow_force_push": "true" if allow_force else "false",
+            "push_access_level": str(access),
+            "merge_access_level": str(access)
+        })
+        if not resp.ok:
+            log.debug(resp.json())
+        return resp.ok
+
+    def unprotect_branch(self, branch: str) -> bool:
+        resp = self.send_request("DELETE", f"protected_branches/{branch}")
+        if not resp.ok:
+            log.debug(resp.json())
+        return resp.ok
+
     def fork(
         self, name: str, namespace_id: int, tree: Optional[List[str]],
         visibility_: visibility = "private", members: 'Optional[List[Person]]' = None,
         max_tries: int = 3
     ) -> 'Literal[False] | Tuple[str, int]':
         if self.id == -1:
             return self.create(name, namespace_id, members, max_tries)
@@ -123,14 +140,17 @@
                     break
                 self.gitlab.project(pid).delete(max_tries)
             log.debug(resp.json())
             time.sleep(1)
         else:
             return False
 
+        self.gitlab.project(pid).unprotect_branch("main")
+        self.gitlab.project(pid).set_protected_branch("main", access_level["developer"], False)
+
         if members:
             ret = self.gitlab.project(pid).add_members(members, access_level["developer"], max_tries)
             return (web_url, pid) if ret else False
         return (web_url, pid)
 
     def add_members(self, persons: 'List[Person]', access_level_: int, max_tries: int = 3) -> bool:
         ids = ",".join(x.gitlab_id for x in persons if x.gitlab_id)
```

### Comparing `esprepomanager-1.0.0/esprepomanager/person.py` & `esprepomanager-1.1.0/esprepomanager/person.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.0.0/esprepomanager/repo.py` & `esprepomanager-1.1.0/esprepomanager/repo.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.0.0/esprepomanager/team.py` & `esprepomanager-1.1.0/esprepomanager/team.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.0.0/esprepomanager/utils.py` & `esprepomanager-1.1.0/esprepomanager/utils.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.0.0/esprepomanager.egg-info/PKG-INFO` & `esprepomanager-1.1.0/esprepomanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esprepomanager
-Version: 1.0.0
+Version: 1.1.0
 Summary: manager for git repos
 Home-page: https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager
 Author: Teichi
 Author-email: tobias@teichmann.top
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `esprepomanager-1.0.0/esprepomanager.egg-info/SOURCES.txt` & `esprepomanager-1.1.0/esprepomanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.0.0/setup.py` & `esprepomanager-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="esprepomanager",
-    version="1.0.0",
+    version="1.1.0",
     author="Teichi",
     author_email="tobias@teichmann.top",
     description="manager for git repos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager",
     packages=setuptools.find_packages(),
```

