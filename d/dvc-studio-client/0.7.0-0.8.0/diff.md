# Comparing `tmp/dvc-studio-client-0.7.0.tar.gz` & `tmp/dvc-studio-client-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-studio-client-0.7.0.tar", last modified: Tue Apr 18 08:23:19 2023, max compression
+gzip compressed data, was "dvc-studio-client-0.8.0.tar", last modified: Thu Apr 20 17:44:58 2023, max compression
```

## Comparing `dvc-studio-client-0.7.0.tar` & `dvc-studio-client-0.8.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.357617 dvc-studio-client-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.353617 dvc-studio-client-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.353617 dvc-studio-client-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.353617 dvc-studio-client-0.7.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-18 08:23:19.357617 dvc-studio-client-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.353617 dvc-studio-client-0.7.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.353617 dvc-studio-client-0.7.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-18 08:23:19.357617 dvc-studio-client-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.353617 dvc-studio-client-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.353617 dvc-studio-client-0.7.0/src/dvc_studio_client/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/src/dvc_studio_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/src/dvc_studio_client/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/src/dvc_studio_client/post_live_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/src/dvc_studio_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/src/dvc_studio_client/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.357617 dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-18 08:23:19.000000 dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-18 08:23:19.000000 dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:23:19.000000 dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:23:19.000000 dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-18 08:23:19.000000 dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 08:23:19.000000 dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:23:19.357617 dvc-studio-client-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-04-18 08:23:02.000000 dvc-studio-client-0.7.0/tests/test_post_live_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-20 17:44:58.971891 dvc-studio-client-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.963891 dvc-studio-client-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/src/dvc_studio_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/src/dvc_studio_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/src/dvc_studio_client/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/src/dvc_studio_client/post_live_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/src/dvc_studio_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/src/dvc_studio_client/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-20 17:44:58.000000 dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-20 17:44:58.000000 dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 17:44:58.000000 dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 17:44:58.000000 dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 17:44:58.000000 dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 17:44:58.000000 dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:44:58.967891 dvc-studio-client-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-04-20 17:44:44.000000 dvc-studio-client-0.8.0/tests/test_post_live_metrics.py
```

### Comparing `dvc-studio-client-0.7.0/.cruft.json` & `dvc-studio-client-0.8.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/.github/dependabot.yml` & `dvc-studio-client-0.8.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/.github/workflows/docs.yml` & `dvc-studio-client-0.8.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/.github/workflows/pre-commit.yml` & `dvc-studio-client-0.8.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/.github/workflows/release.yml` & `dvc-studio-client-0.8.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/.github/workflows/tests.yml` & `dvc-studio-client-0.8.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/.gitignore` & `dvc-studio-client-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/.pre-commit-config.yaml` & `dvc-studio-client-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/CODE_OF_CONDUCT.rst` & `dvc-studio-client-0.8.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/CONTRIBUTING.rst` & `dvc-studio-client-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/LICENSE` & `dvc-studio-client-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/PKG-INFO` & `dvc-studio-client-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-studio-client
-Version: 0.7.0
+Version: 0.8.0
 Summary: Small library to post data from DVC/DVCLive to Iterative Studio
 Home-page: https://github.com/iterative/DVC Studio Client
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-studio-client-0.7.0/README.rst` & `dvc-studio-client-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/docs/assets/logo.svg` & `dvc-studio-client-0.8.0/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/docs/gen_ref_pages.py` & `dvc-studio-client-0.8.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/mkdocs.yml` & `dvc-studio-client-0.8.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/pyproject.toml` & `dvc-studio-client-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/setup.cfg` & `dvc-studio-client-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/src/dvc_studio_client/post_live_metrics.py` & `dvc-studio-client-0.8.0/src/dvc_studio_client/post_live_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,39 +49,42 @@
             "Couldn't find a valid Studio Repo URL.\n"
             "You can try manually setting the environment variable `%s`.",
             STUDIO_REPO_URL,
         )
         return None
 
 
-def get_studio_token_and_repo_url():
-    studio_token = getenv(DVC_STUDIO_TOKEN) or getenv(STUDIO_TOKEN)
+def get_studio_token_and_repo_url(studio_token=None, studio_repo_url=None):
+    studio_token = studio_token or getenv(DVC_STUDIO_TOKEN) or getenv(STUDIO_TOKEN)
     if studio_token is None:
         logger.debug(
             f"{DVC_STUDIO_TOKEN} not found. Skipping `post_studio_live_metrics`"
         )
         return None, None
 
-    studio_repo_url = getenv(STUDIO_REPO_URL, None)
+    studio_repo_url = studio_repo_url or getenv(STUDIO_REPO_URL, None)
     if studio_repo_url is None:
         logger.debug(f"`{STUDIO_REPO_URL}` not found. Trying to automatically find it.")
         studio_repo_url = get_studio_repo_url()
     return studio_token, studio_repo_url
 
 
 def post_live_metrics(
     event_type: Literal["start", "data", "done"],
     baseline_sha: str,
     name: str,
     client: Literal["dvc", "dvclive"],
     experiment_rev: Optional[str] = None,
+    machine: Optional[Dict[str, Any]] = None,
     metrics: Optional[Dict[str, Any]] = None,
     params: Optional[Dict[str, Any]] = None,
     plots: Optional[Dict[str, Any]] = None,
     step: Optional[int] = None,
+    studio_token: Optional[str] = None,
+    studio_repo_url: Optional[str] = None,
 ) -> Optional[bool]:
     """Post `event_type` to Studio's `api/live`.
 
     Requires the environment variable `STUDIO_TOKEN` to be set.
     If the environment variable `STUDIO_REPO_URL` is not set, will attempt to
     infer it from `git ls-remote --get-url`.
 
@@ -92,14 +95,25 @@
             Automatically generated by DVC(Live) or manually passed by the user.
             (baseline_sha, name) is a unique identifier of the experiment.
         client (Literal["dvc", "dvclive"]): Name of the client.
         experiment_rev (Optional[str]): SHA of the revision created for
             the experiment.
             Only used when `event_type="done"`.
             Only used when
+        machine (Optional[Dict[str, Any]]): Information about the machine
+            running the experiment.
+            Defaults to `None`.
+            ```
+            machine={
+                "cpu": 0.94
+                "memory": 0.99
+                "cloud": "aws"
+                "instance": "t2.micro"
+            }
+            ```
         metrics (Optional[Dict[str, Any]]): Updates to DVC metric files.
             Defaults to `None`.
             Only used when `event_type="data"`.
             ```
             metrics={
                 "dvclive/metrics.json": {
                     "data": {
@@ -127,22 +141,26 @@
                 }
             }
             ```
         step: (Optional[int]): Current step of the training loop.
             Usually comes from DVCLive `Live.step` property.
             Required in when `event_type="data"`.
             Defaults to `None`.
-
+        studio_token (Optional[str]): Studio access token obtained from the UI.
+        studio_repo_url (Optional[str]): URL of the Git repository that has been
+            imported into Studio UI.
     Returns:
         Optional[bool]:
             `True` - if received status code 200 from Studio.
             `False` - if received other status code or RequestException raised.
             `None`- if prerequisites weren't met and the request was not sent.
     """
-    studio_token, studio_repo_url = get_studio_token_and_repo_url()
+    studio_token, studio_repo_url = get_studio_token_and_repo_url(
+        studio_token, studio_repo_url
+    )
 
     if any(x is None for x in (studio_token, studio_repo_url)):
         return None
 
     body = {
         "type": event_type,
         "repo_url": studio_repo_url,
@@ -153,14 +171,17 @@
 
     if params:
         body["params"] = params
 
     if metrics:
         body["metrics"] = metrics
 
+    if machine:
+        body["machine"] = machine
+
     if event_type == "data":
         if step is None:
             logger.warning("Missing `step` in `data` event.")
             return None
         body["step"] = step
         if plots:
             body["plots"] = plots
```

### Comparing `dvc-studio-client-0.7.0/src/dvc_studio_client/schema.py` & `dvc-studio-client-0.8.0/src/dvc_studio_client/schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         Required("baseline_sha"): Sha,
         "name": str,
         "env": dict,
         "client": str,
         "errors": [ERROR_SCHEMA],
         "params": {str: dict},
         "metrics": {str: {"data": dict, "error": ERROR_SCHEMA}},
+        "machine": dict,
         # Required("timestamp"): iso_datetime,  # TODO: decide if we need this
     }
 )
 SCHEMAS_BY_TYPE = {
     "start": BASE_SCHEMA,
     "data": BASE_SCHEMA.extend(
         {
```

### Comparing `dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/PKG-INFO` & `dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-studio-client
-Version: 0.7.0
+Version: 0.8.0
 Summary: Small library to post data from DVC/DVCLive to Iterative Studio
 Home-page: https://github.com/iterative/DVC Studio Client
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-studio-client-0.7.0/src/dvc_studio_client.egg-info/SOURCES.txt` & `dvc-studio-client-0.8.0/src/dvc_studio_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.7.0/tests/test_post_live_metrics.py` & `dvc-studio-client-0.8.0/tests/test_post_live_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,14 +106,49 @@
             "Authorization": "token FOO_TOKEN",
             "Content-type": "application/json",
         },
         timeout=5,
     )
 
 
+def test_post_live_metrics_start_event_machine(mocker, monkeypatch):
+    monkeypatch.setenv(DVC_STUDIO_URL, "https://0.0.0.0")
+    monkeypatch.setenv(STUDIO_TOKEN, "FOO_TOKEN")
+    monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
+
+    mocked_response = mocker.MagicMock()
+    mocked_response.status_code = 200
+    mocked_post = mocker.patch("requests.post", return_value=mocked_response)
+
+    assert post_live_metrics(
+        "start",
+        "f" * 40,
+        "fooname",
+        "fooclient",
+        machine={"cpu": 1, "gpu": 2},
+    )
+
+    mocked_post.assert_called_with(
+        "https://0.0.0.0/api/live",
+        json={
+            "type": "start",
+            "repo_url": "FOO_REPO_URL",
+            "baseline_sha": "f" * 40,
+            "name": "fooname",
+            "client": "fooclient",
+            "machine": {"cpu": 1, "gpu": 2},
+        },
+        headers={
+            "Authorization": "token FOO_TOKEN",
+            "Content-type": "application/json",
+        },
+        timeout=5,
+    )
+
+
 def test_post_live_metrics_data_skip_if_no_step(caplog, monkeypatch):
     monkeypatch.setenv(DVC_STUDIO_TOKEN, "FOO_TOKEN")
     monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
 
     assert post_live_metrics("data", "f" * 40, "fooname", "fooclient") is None
     assert caplog.records[0].message == ("Missing `step` in `data` event.")
 
@@ -306,7 +341,40 @@
 
 
 def test_get_studio_token_and_repo_url_skip_repo_url(monkeypatch):
     monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
     token, repo_url = get_studio_token_and_repo_url()
     assert token is None
     assert repo_url is None  # Skipped call to get_repo_url
+
+
+def test_post_live_metrics_token_and_repo_url_args(mocker, monkeypatch):
+    monkeypatch.setenv(DVC_STUDIO_URL, "https://0.0.0.0")
+
+    mocked_response = mocker.MagicMock()
+    mocked_response.status_code = 200
+    mocked_post = mocker.patch("requests.post", return_value=mocked_response)
+
+    assert post_live_metrics(
+        "start",
+        "f" * 40,
+        "fooname",
+        "fooclient",
+        studio_token="FOO_TOKEN",
+        studio_repo_url="FOO_REPO_URL",
+    )
+
+    mocked_post.assert_called_with(
+        "https://0.0.0.0/api/live",
+        json={
+            "type": "start",
+            "repo_url": "FOO_REPO_URL",
+            "baseline_sha": "f" * 40,
+            "name": "fooname",
+            "client": "fooclient",
+        },
+        headers={
+            "Authorization": "token FOO_TOKEN",
+            "Content-type": "application/json",
+        },
+        timeout=5,
+    )
```

