# Comparing `tmp/pygitguardian-1.5.1.tar.gz` & `tmp/pygitguardian-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygitguardian-1.5.1.tar", last modified: Wed Mar 29 09:12:49 2023, max compression
+gzip compressed data, was "pygitguardian-1.6.0.tar", last modified: Thu Apr 20 08:43:43 2023, max compression
```

## Comparing `pygitguardian-1.5.1.tar` & `pygitguardian-1.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:12:49.551272 pygitguardian-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-29 09:12:41.000000 pygitguardian-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-29 09:12:41.000000 pygitguardian-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-03-29 09:12:49.551272 pygitguardian-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-03-29 09:12:41.000000 pygitguardian-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:12:49.547272 pygitguardian-1.5.1/pygitguardian/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-29 09:12:41.000000 pygitguardian-1.5.1/pygitguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-03-29 09:12:41.000000 pygitguardian-1.5.1/pygitguardian/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-29 09:12:41.000000 pygitguardian-1.5.1/pygitguardian/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-29 09:12:41.000000 pygitguardian-1.5.1/pygitguardian/iac_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-03-29 09:12:41.000000 pygitguardian-1.5.1/pygitguardian/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:12:49.547272 pygitguardian-1.5.1/pygitguardian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-03-29 09:12:49.000000 pygitguardian-1.5.1/pygitguardian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-29 09:12:49.000000 pygitguardian-1.5.1/pygitguardian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 09:12:49.000000 pygitguardian-1.5.1/pygitguardian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-29 09:12:49.000000 pygitguardian-1.5.1/pygitguardian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-29 09:12:49.000000 pygitguardian-1.5.1/pygitguardian.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 09:12:49.000000 pygitguardian-1.5.1/pygitguardian.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-29 09:12:41.000000 pygitguardian-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-29 09:12:49.551272 pygitguardian-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-29 09:12:41.000000 pygitguardian-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:12:49.551272 pygitguardian-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-03-29 09:12:41.000000 pygitguardian-1.5.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-03-29 09:12:41.000000 pygitguardian-1.5.1/tests/test_iac_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-03-29 09:12:41.000000 pygitguardian-1.5.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-03-29 09:12:41.000000 pygitguardian-1.5.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:43:43.045639 pygitguardian-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-04-20 08:43:43.045639 pygitguardian-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:43:43.041639 pygitguardian-1.6.0/pygitguardian/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/pygitguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/pygitguardian/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/pygitguardian/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/pygitguardian/iac_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/pygitguardian/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:43:43.045639 pygitguardian-1.6.0/pygitguardian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-04-20 08:43:43.000000 pygitguardian-1.6.0/pygitguardian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-20 08:43:43.000000 pygitguardian-1.6.0/pygitguardian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 08:43:43.000000 pygitguardian-1.6.0/pygitguardian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 08:43:43.000000 pygitguardian-1.6.0/pygitguardian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 08:43:43.000000 pygitguardian-1.6.0/pygitguardian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 08:43:43.000000 pygitguardian-1.6.0/pygitguardian.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-20 08:43:43.045639 pygitguardian-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:43:43.045639 pygitguardian-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/tests/test_iac_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/tests/test_utils.py
```

### Comparing `pygitguardian-1.5.1/LICENSE` & `pygitguardian-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.5.1/PKG-INFO` & `pygitguardian-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygitguardian
-Version: 1.5.1
+Version: 1.6.0
 Summary: Python Wrapper for GitGuardian's API -- Scan security policy breaks everywhere
 Home-page: https://github.com/GitGuardian/py-gitguardian
 Author: GitGuardian
 Author-email: support@gitguardian.com
 Maintainer: GitGuardian
 License: MIT
 Keywords: api-client devsecops secrets-detection security-tools library gitguardian
```

### Comparing `pygitguardian-1.5.1/README.md` & `pygitguardian-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.5.1/pygitguardian/client.py` & `pygitguardian-1.6.0/pygitguardian/client.py`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.5.1/pygitguardian/iac_models.py` & `pygitguardian-1.6.0/pygitguardian/iac_models.py`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.5.1/pygitguardian/models.py` & `pygitguardian-1.6.0/pygitguardian/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,15 @@
 
 
 class PolicyBreakSchema(BaseSchema):
     break_type = fields.String(data_key="type", required=True)
     policy = fields.String(required=True)
     validity = fields.String(required=False, load_default=None, dump_default=None)
     known_secret = fields.Boolean(required=False, load_default=False, dump_default=None)
+    incident_url = fields.String(required=False, load_default=False, dump_default=None)
     matches = fields.List(fields.Nested(MatchSchema), required=True)
 
     @post_load
     def make_policy_break(self, data: Dict[str, Any], **kwargs: Any) -> "PolicyBreak":
         return PolicyBreak(**data)
 
 
@@ -226,21 +227,23 @@
     def __init__(
         self,
         break_type: str,
         policy: str,
         validity: str,
         matches: List[Match],
         known_secret: bool = False,
+        incident_url: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         super().__init__()
         self.break_type = break_type
         self.policy = policy
         self.validity = validity
         self.known_secret = known_secret
+        self.incident_url = incident_url
         self.matches = matches
 
     @property
     def is_secret(self) -> bool:
         return self.policy == "Secrets detection"
 
     def __repr__(self) -> str:
```

### Comparing `pygitguardian-1.5.1/pygitguardian.egg-info/PKG-INFO` & `pygitguardian-1.6.0/pygitguardian.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygitguardian
-Version: 1.5.1
+Version: 1.6.0
 Summary: Python Wrapper for GitGuardian's API -- Scan security policy breaks everywhere
 Home-page: https://github.com/GitGuardian/py-gitguardian
 Author: GitGuardian
 Author-email: support@gitguardian.com
 Maintainer: GitGuardian
 License: MIT
 Keywords: api-client devsecops secrets-detection security-tools library gitguardian
```

### Comparing `pygitguardian-1.5.1/pyproject.toml` & `pygitguardian-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.5.1/setup.py` & `pygitguardian-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.5.1/tests/test_client.py` & `pygitguardian-1.6.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.5.1/tests/test_iac_models.py` & `pygitguardian-1.6.0/tests/test_iac_models.py`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.5.1/tests/test_models.py` & `pygitguardian-1.6.0/tests/test_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -88,14 +88,26 @@
                     "type": "hello",
                     "policy": "hello",
                     "validity": "hey",
                     "matches": [{"match": "hello", "type": "hello"}],
                 },
             ),
             (
+                PolicyBreakSchema,
+                PolicyBreak,
+                {
+                    "type": "hello",
+                    "policy": "hello",
+                    "validity": "hey",
+                    "known_secret": True,
+                    "incident_url": "https://api.gitguardian.com/workspace/2/incidents/3",
+                    "matches": [{"match": "hello", "type": "hello"}],
+                },
+            ),
+            (
                 QuotaSchema,
                 Quota,
                 {
                     "count": 1,
                     "limit": 1,
                     "remaining": 1,
                     "since": "2021-04-18",
```

### Comparing `pygitguardian-1.5.1/tests/test_utils.py` & `pygitguardian-1.6.0/tests/test_utils.py`

 * *Files identical despite different names*

