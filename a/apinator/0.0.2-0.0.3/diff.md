# Comparing `tmp/apinator-0.0.2.tar.gz` & `tmp/apinator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apinator-0.0.2.tar", last modified: Wed Apr 19 19:51:20 2023, max compression
+gzip compressed data, was "apinator-0.0.3.tar", last modified: Wed Apr 19 23:54:48 2023, max compression
```

## Comparing `apinator-0.0.2.tar` & `apinator-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0      177 2023-04-19 19:51:13.060293 apinator-0.0.2/.bumpversion.cfg
--rw-r--r--   0        0        0     2162 2022-07-05 17:25:03.902436 apinator-0.0.2/.gitignore
--rw-r--r--   0        0        0      720 2023-04-17 21:14:01.448694 apinator-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1095 2023-04-18 23:01:35.135695 apinator-0.0.2/.ruff.toml
--rw-r--r--   0        0        0    11558 2023-04-19 17:16:02.873453 apinator-0.0.2/LICENSE
--rw-r--r--   0        0        0     4264 2023-04-19 19:45:36.072300 apinator-0.0.2/README.md
--rw-r--r--   0        0        0      325 2023-04-19 19:51:13.058721 apinator-0.0.2/apinator/__init__.py
--rw-r--r--   0        0        0     1857 2023-04-18 23:40:26.561130 apinator-0.0.2/apinator/api.py
--rw-r--r--   0        0        0     3191 2023-04-18 23:40:26.623119 apinator-0.0.2/apinator/common.py
--rw-r--r--   0        0        0     9420 2023-04-19 18:29:57.123120 apinator-0.0.2/apinator/endpoint.py
--rw-r--r--   0        0        0      634 2023-04-19 17:16:03.453979 apinator-0.0.2/docs/Makefile
--rw-r--r--   0        0        0      132 2023-04-19 19:40:15.190935 apinator-0.0.2/docs/api/apinator.api.md
--rw-r--r--   0        0        0      138 2023-04-19 19:40:15.208048 apinator-0.0.2/docs/api/apinator.common.md
--rw-r--r--   0        0        0      142 2023-04-19 19:40:15.225072 apinator-0.0.2/docs/api/apinator.endpoint.md
--rw-r--r--   0        0        0      244 2023-04-19 19:41:40.182895 apinator-0.0.2/docs/api/apinator.md
--rw-r--r--   0        0        0     1247 2023-04-19 19:51:13.059773 apinator-0.0.2/docs/conf.py
--rw-r--r--   0        0        0     6811 2023-04-19 19:44:22.793594 apinator-0.0.2/docs/getting_started.md
--rw-r--r--   0        0        0     2809 2023-04-19 19:41:01.048308 apinator-0.0.2/docs/index.md
--rwxr-xr-x   0        0        0      765 2023-04-19 17:16:03.486524 apinator-0.0.2/docs/make.bat
--rw-r--r--   0        0        0     3151 2023-04-19 17:16:03.517149 apinator-0.0.2/docs/overview.md
--rw-r--r--   0        0        0       57 2023-04-19 19:49:31.416910 apinator-0.0.2/docs/requirements.txt
--rw-r--r--   0        0        0      627 2023-04-19 17:16:03.446049 apinator-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      696 2023-04-19 19:51:13.058195 apinator-0.0.2/setup.cfg
--rw-r--r--   0        0        0     4355 2023-04-18 23:40:26.979864 apinator-0.0.2/tests/test_basic.py
--rw-r--r--   0        0        0      485 2023-04-18 23:40:26.536764 apinator-0.0.2/tests/test_pathstr.py
--rw-r--r--   0        0        0      292 2023-04-18 23:40:26.527854 apinator-0.0.2/tests/test_request.py
--rw-r--r--   0        0        0     5001 1970-01-01 00:00:00.000000 apinator-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      177 2023-04-19 23:54:38.971658 apinator-0.0.3/.bumpversion.cfg
+-rw-r--r--   0        0        0      584 2023-04-19 20:33:39.872507 apinator-0.0.3/.github/workflows/dagger.yml
+-rw-r--r--   0        0        0     2162 2022-07-05 17:25:03.902436 apinator-0.0.3/.gitignore
+-rw-r--r--   0        0        0      720 2023-04-17 21:14:01.448694 apinator-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1095 2023-04-18 23:01:35.135695 apinator-0.0.3/.ruff.toml
+-rw-r--r--   0        0        0    11558 2023-04-19 17:16:02.873453 apinator-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4264 2023-04-19 19:45:36.072300 apinator-0.0.3/README.md
+-rw-r--r--   0        0        0      325 2023-04-19 23:54:38.970597 apinator-0.0.3/apinator/__init__.py
+-rw-r--r--   0        0        0     1857 2023-04-18 23:40:26.561130 apinator-0.0.3/apinator/api.py
+-rw-r--r--   0        0        0     3191 2023-04-18 23:40:26.623119 apinator-0.0.3/apinator/common.py
+-rw-r--r--   0        0        0     9456 2023-04-19 23:54:25.315535 apinator-0.0.3/apinator/endpoint.py
+-rw-r--r--   0        0        0      895 2023-04-19 20:28:33.161296 apinator-0.0.3/ci/main.py
+-rw-r--r--   0        0        0      634 2023-04-19 17:16:03.453979 apinator-0.0.3/docs/Makefile
+-rw-r--r--   0        0        0      132 2023-04-19 19:40:15.190935 apinator-0.0.3/docs/api/apinator.api.md
+-rw-r--r--   0        0        0      138 2023-04-19 19:40:15.208048 apinator-0.0.3/docs/api/apinator.common.md
+-rw-r--r--   0        0        0      142 2023-04-19 19:40:15.225072 apinator-0.0.3/docs/api/apinator.endpoint.md
+-rw-r--r--   0        0        0      244 2023-04-19 19:41:40.182895 apinator-0.0.3/docs/api/apinator.md
+-rw-r--r--   0        0        0     1247 2023-04-19 23:54:38.971658 apinator-0.0.3/docs/conf.py
+-rw-r--r--   0        0        0     6811 2023-04-19 19:44:22.793594 apinator-0.0.3/docs/getting_started.md
+-rw-r--r--   0        0        0     2809 2023-04-19 19:41:01.048308 apinator-0.0.3/docs/index.md
+-rwxr-xr-x   0        0        0      765 2023-04-19 17:16:03.486524 apinator-0.0.3/docs/make.bat
+-rw-r--r--   0        0        0     3151 2023-04-19 17:16:03.517149 apinator-0.0.3/docs/overview.md
+-rw-r--r--   0        0        0       57 2023-04-19 19:49:31.416910 apinator-0.0.3/docs/requirements.txt
+-rw-r--r--   0        0        0      627 2023-04-19 17:16:03.446049 apinator-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      696 2023-04-19 23:54:38.970070 apinator-0.0.3/setup.cfg
+-rw-r--r--   0        0        0     4355 2023-04-19 20:33:27.606781 apinator-0.0.3/tests/test_basic.py
+-rw-r--r--   0        0        0      485 2023-04-18 23:40:26.536764 apinator-0.0.3/tests/test_pathstr.py
+-rw-r--r--   0        0        0      292 2023-04-18 23:40:26.527854 apinator-0.0.3/tests/test_request.py
+-rw-r--r--   0        0        0     5001 1970-01-01 00:00:00.000000 apinator-0.0.3/PKG-INFO
```

### Comparing `apinator-0.0.2/.gitignore` & `apinator-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `apinator-0.0.2/.pre-commit-config.yaml` & `apinator-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `apinator-0.0.2/.ruff.toml` & `apinator-0.0.3/.ruff.toml`

 * *Files identical despite different names*

### Comparing `apinator-0.0.2/LICENSE` & `apinator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apinator-0.0.2/README.md` & `apinator-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `apinator-0.0.2/apinator/api.py` & `apinator-0.0.3/apinator/api.py`

 * *Files identical despite different names*

### Comparing `apinator-0.0.2/apinator/common.py` & `apinator-0.0.3/apinator/common.py`

 * *Files identical despite different names*

### Comparing `apinator-0.0.2/apinator/endpoint.py` & `apinator-0.0.3/apinator/endpoint.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
+from functools import partial
 from typing import Dict, Generic, Iterable, List, Optional, Type, TypeVar, Union
 
-from pydantic import BaseModel, PrivateAttr, validate_arguments
+from pydantic import BaseModel, validate_arguments
 from typing_extensions import Self
 
 from apinator.api import ApiBase
 from apinator.common import HttpMethod, PathStr, Request
 
 R = TypeVar("R", bound=BaseModel)
 M = TypeVar("M", bound=BaseModel)
@@ -178,14 +179,15 @@
         return cls(
             action_name="destroy",
             method=HttpMethod.DELETE,
             **kwargs,
         )
 
 
+# TODO: This should probably be a metaclass? Like `pydantic.Field`, this is really more of a descriptor than a real object
 class EndpointGroup:
     """A quick, OOP approach to creating a group of related endpoints.
 
     Consider the following API:
 
     ```
     class MyApi(JsonApiBase):
@@ -249,36 +251,29 @@
         else:
             assert self.name is not None
             bound_group = BoundEndpointGroup(api=instance, group=self)
             instance.__dict__[self.name] = bound_group
             return bound_group
 
 
-class BoundEndpointGroup(BaseModel):
-    api: ApiBase
-    group: EndpointGroup
-
-    _endpoints: Dict[str, Endpoint] = PrivateAttr(default_factory=dict)
-
-    class Config:
-        arbitrary_types_allowed = True
-        frozen = True
+class BoundEndpointGroup:
+    def __init__(self, api: ApiBase, group: EndpointGroup):
+        self._group = group
+        self._endpoints = {
+            action_name: action.create_endpoint(api, group.url, group.arg_names)
+            for action_name, action in group.actions.items()
+        }
 
     def __getattr__(self, item):
-        if item not in self._endpoints:
-            try:
-                action = self.group.actions[item]
-            except KeyError:
-                return getattr(super(), item)
-            else:
-                self._endpoints[item] = action.create_endpoint(
-                    self.api, self.group.url, self.group.arg_names
-                )
+        if item in self._endpoints:
+            return self._endpoints[item]
 
-        return self._endpoints[item]
+        # TODO: This is a mess
+        setattr(self, item, partial(getattr(type(self._group), item), self))
+        return getattr(self, item)
 
 
 class DeclarativeEndpoint(EndpointDefinition[R, M]):
     def _make_variant(self, **kwargs) -> Self:
         d = self.dict().copy()
         d.update(kwargs)
         return self.parse_obj(d)
```

### Comparing `apinator-0.0.2/docs/Makefile` & `apinator-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `apinator-0.0.2/docs/conf.py` & `apinator-0.0.3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "APInator"
 copyright = "2023, Rearc Data"
 author = "Rearc Data"
-release = "0.0.2"
+release = "0.0.3"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "myst_parser",
     "sphinx.ext.coverage",
```

### Comparing `apinator-0.0.2/docs/getting_started.md` & `apinator-0.0.3/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `apinator-0.0.2/docs/index.md` & `apinator-0.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `apinator-0.0.2/docs/make.bat` & `apinator-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `apinator-0.0.2/docs/overview.md` & `apinator-0.0.3/docs/overview.md`

 * *Files identical despite different names*

### Comparing `apinator-0.0.2/pyproject.toml` & `apinator-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apinator-0.0.2/setup.cfg` & `apinator-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 7665 7273  [metadata]..vers
-00000010: 696f 6e20 3d20 302e 302e 320d 0a6e 616d  ion = 0.0.2..nam
+00000010: 696f 6e20 3d20 302e 302e 330d 0a6e 616d  ion = 0.0.3..nam
 00000020: 6520 3d20 6170 696e 6174 6f72 0d0a 6465  e = apinator..de
 00000030: 7363 7269 7074 696f 6e20 3d20 546f 6f6c  scription = Tool
 00000040: 696e 6720 746f 2062 7569 6c64 2063 6f6e  ing to build con
 00000050: 7369 7374 656e 742c 2073 656c 662d 7661  sistent, self-va
 00000060: 6c69 6461 7469 6e67 2062 696e 6469 6e67  lidating binding
 00000070: 7320 746f 2065 7874 6572 6e61 6c20 4150  s to external AP
 00000080: 4927 730d 0a61 7574 686f 7220 3d20 5265  I's..author = Re
```

### Comparing `apinator-0.0.2/tests/test_basic.py` & `apinator-0.0.3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `apinator-0.0.2/PKG-INFO` & `apinator-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apinator
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for building type-checked bindings to external REST APIs
 Author-email: Rearc Data <data@rearc.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: typing_extensions>=4
 Requires-Dist: pydantic>=1,<2
 Requires-Dist: requests
```

