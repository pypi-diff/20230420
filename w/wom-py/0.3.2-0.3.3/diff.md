# Comparing `tmp/wom_py-0.3.2.tar.gz` & `tmp/wom_py-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wom_py-0.3.2.tar", max compression
+gzip compressed data, was "wom_py-0.3.3.tar", max compression
```

## Comparing `wom_py-0.3.2.tar` & `wom_py-0.3.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1074 2023-04-14 20:14:27.072223 wom_py-0.3.2/LICENSE
--rw-r--r--   0        0        0     1942 2023-04-14 20:14:27.072223 wom_py-0.3.2/README.md
--rw-r--r--   0        0        0     2138 2023-04-14 20:14:27.076223 wom_py-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4295 2023-04-14 20:14:27.184223 wom_py-0.3.2/wom/__init__.py
--rw-r--r--   0        0        0     1324 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/__main__.py
--rw-r--r--   0        0        0     1808 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/_cli.py
--rw-r--r--   0        0        0     8494 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/client.py
--rw-r--r--   0        0        0     1447 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/constants.py
--rw-r--r--   0        0        0     7212 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/enums.py
--rw-r--r--   0        0        0     1729 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/errors.py
--rw-r--r--   0        0        0     3138 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/__init__.py
--rw-r--r--   0        0        0     1555 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/base.py
--rw-r--r--   0        0        0     1673 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/competitions/__init__.py
--rw-r--r--   0        0        0     1591 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/competitions/enums.py
--rw-r--r--   0        0        0     7364 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/competitions/models.py
--rw-r--r--   0        0        0     1289 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/deltas/__init__.py
--rw-r--r--   0        0        0     1824 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/deltas/models.py
--rw-r--r--   0        0        0     1716 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/groups/__init__.py
--rw-r--r--   0        0        0     7780 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/groups/enums.py
--rw-r--r--   0        0        0     9075 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/groups/models.py
--rw-r--r--   0        0        0     1738 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/http.py
--rw-r--r--   0        0        0     1381 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/names/__init__.py
--rw-r--r--   0        0        0     1413 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/models/names/enums.py
--rw-r--r--   0        0        0     3778 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/models/names/models.py
--rw-r--r--   0        0        0     1754 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/models/players/__init__.py
--rw-r--r--   0        0        0     5664 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/models/players/enums.py
--rw-r--r--   0        0        0    11832 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/models/players/models.py
--rw-r--r--   0        0        0     1300 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/models/records/__init__.py
--rw-r--r--   0        0        0     2217 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/models/records/models.py
--rw-r--r--   0        0        0        0 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/py.typed
--rw-r--r--   0        0        0     5561 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/result.py
--rw-r--r--   0        0        0     6420 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/routes.py
--rw-r--r--   0        0        0    33973 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/serializer.py
--rw-r--r--   0        0        0     1709 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/__init__.py
--rw-r--r--   0        0        0     2042 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/base.py
--rw-r--r--   0        0        0    21066 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/competitions.py
--rw-r--r--   0        0        0     3511 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/deltas.py
--rw-r--r--   0        0        0     3671 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/efficiency.py
--rw-r--r--   0        0        0    23928 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/groups.py
--rw-r--r--   0        0        0     5750 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/http.py
--rw-r--r--   0        0        0     4824 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/names.py
--rw-r--r--   0        0        0    17995 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/players.py
--rw-r--r--   0        0        0     3489 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/records.py
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 wom_py-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-20 02:53:58.701105 wom_py-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1942 2023-04-20 02:53:58.701105 wom_py-0.3.3/README.md
+-rw-r--r--   0        0        0     2138 2023-04-20 02:53:58.701105 wom_py-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4295 2023-04-20 02:53:58.781106 wom_py-0.3.3/wom/__init__.py
+-rw-r--r--   0        0        0     1324 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/__main__.py
+-rw-r--r--   0        0        0     1808 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/_cli.py
+-rw-r--r--   0        0        0     8494 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/client.py
+-rw-r--r--   0        0        0     1447 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/constants.py
+-rw-r--r--   0        0        0     7212 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/enums.py
+-rw-r--r--   0        0        0     1729 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/errors.py
+-rw-r--r--   0        0        0     3138 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/__init__.py
+-rw-r--r--   0        0        0     1555 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/base.py
+-rw-r--r--   0        0        0     1673 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/competitions/__init__.py
+-rw-r--r--   0        0        0     1591 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/competitions/enums.py
+-rw-r--r--   0        0        0     7364 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/competitions/models.py
+-rw-r--r--   0        0        0     1289 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/deltas/__init__.py
+-rw-r--r--   0        0        0     1824 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/deltas/models.py
+-rw-r--r--   0        0        0     1716 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/groups/__init__.py
+-rw-r--r--   0        0        0     7780 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/groups/enums.py
+-rw-r--r--   0        0        0     9075 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/groups/models.py
+-rw-r--r--   0        0        0     1738 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/http.py
+-rw-r--r--   0        0        0     1381 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/names/__init__.py
+-rw-r--r--   0        0        0     1413 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/names/enums.py
+-rw-r--r--   0        0        0     3778 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/names/models.py
+-rw-r--r--   0        0        0     1754 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/players/__init__.py
+-rw-r--r--   0        0        0     5664 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/players/enums.py
+-rw-r--r--   0        0        0    11832 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/players/models.py
+-rw-r--r--   0        0        0     1300 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/records/__init__.py
+-rw-r--r--   0        0        0     2217 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/records/models.py
+-rw-r--r--   0        0        0        0 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/py.typed
+-rw-r--r--   0        0        0     5561 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/result.py
+-rw-r--r--   0        0        0     6539 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/routes.py
+-rw-r--r--   0        0        0    33973 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/serializer.py
+-rw-r--r--   0        0        0     1709 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/__init__.py
+-rw-r--r--   0        0        0     2042 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/base.py
+-rw-r--r--   0        0        0    21066 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/competitions.py
+-rw-r--r--   0        0        0     3511 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/deltas.py
+-rw-r--r--   0        0        0     3671 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/efficiency.py
+-rw-r--r--   0        0        0    23928 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/groups.py
+-rw-r--r--   0        0        0     5750 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/http.py
+-rw-r--r--   0        0        0     4824 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/names.py
+-rw-r--r--   0        0        0    17995 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/players.py
+-rw-r--r--   0        0        0     3489 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/records.py
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 wom_py-0.3.3/PKG-INFO
```

### Comparing `wom_py-0.3.2/LICENSE` & `wom_py-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/README.md` & `wom_py-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/pyproject.toml` & `wom_py-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wom.py"
-version = "0.3.2"
+version = "0.3.3"
 description = "An asynchronous wrapper for the Wise Old Man API."
 authors = ["Jonxslays"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jonxslays/wom.py"
 repository = "https://github.com/Jonxslays/wom.py"
 documentation = "https://jonxslays.github.io/wom.py"
```

### Comparing `wom_py-0.3.2/wom/__init__.py` & `wom_py-0.3.3/wom/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,23 +130,23 @@
     "Team",
     "Top5ProgressResult",
     "UnwrapError",
     "WomError",
 )
 
 __packagename__: Final[str] = "wom.py"
-__version__: Final[str] = "0.3.2"
+__version__: Final[str] = "0.3.3"
 __author__: Final[str] = "Jonxslays"
 __copyright__: Final[str] = "2023-present Jonxslays"
 __description__: Final[str] = "An asynchronous wrapper for the Wise Old Man API."
 __url__: Final[str] = "https://github.com/Jonxslays/wom.py"
 __docs__: Final[str] = "https://jonxslays.github.io/wom.py"
 __repository__: Final[str] = __url__
 __license__: Final[str] = "MIT"
-__git_sha__: Final[str] = "[d9d3e5e]"
+__git_sha__: Final[str] = "[57608ca]"
 
 from . import client
 from . import constants
 from . import enums
 from . import errors
 from . import models
 from . import result
```

### Comparing `wom_py-0.3.2/wom/__main__.py` & `wom_py-0.3.3/wom/__main__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/_cli.py` & `wom_py-0.3.3/wom/_cli.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/client.py` & `wom_py-0.3.3/wom/client.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/constants.py` & `wom_py-0.3.3/wom/constants.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/enums.py` & `wom_py-0.3.3/wom/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/errors.py` & `wom_py-0.3.3/wom/errors.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/__init__.py` & `wom_py-0.3.3/wom/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/base.py` & `wom_py-0.3.3/wom/models/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/competitions/__init__.py` & `wom_py-0.3.3/wom/models/competitions/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/competitions/enums.py` & `wom_py-0.3.3/wom/models/competitions/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/competitions/models.py` & `wom_py-0.3.3/wom/models/competitions/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/deltas/__init__.py` & `wom_py-0.3.3/wom/models/deltas/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/deltas/models.py` & `wom_py-0.3.3/wom/models/deltas/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/groups/__init__.py` & `wom_py-0.3.3/wom/models/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/groups/enums.py` & `wom_py-0.3.3/wom/models/groups/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/groups/models.py` & `wom_py-0.3.3/wom/models/groups/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/http.py` & `wom_py-0.3.3/wom/models/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/names/__init__.py` & `wom_py-0.3.3/wom/models/names/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/names/enums.py` & `wom_py-0.3.3/wom/models/names/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/names/models.py` & `wom_py-0.3.3/wom/models/names/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/players/__init__.py` & `wom_py-0.3.3/wom/models/players/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/players/enums.py` & `wom_py-0.3.3/wom/models/players/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/players/models.py` & `wom_py-0.3.3/wom/models/players/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/records/__init__.py` & `wom_py-0.3.3/wom/models/records/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/models/records/models.py` & `wom_py-0.3.3/wom/models/records/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/result.py` & `wom_py-0.3.3/wom/result.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/routes.py` & `wom_py-0.3.3/wom/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,29 +33,34 @@
 class CompiledRoute:
     """A route that has been compiled to include uri variables.
 
     Args:
         route: The route to compile.
     """
 
-    __slots__ = ("_route", "_params")
+    __slots__ = ("_route", "_uri", "_params")
 
-    def __init__(self, route: Route) -> None:
+    def __init__(self, route: Route, uri: str) -> None:
+        self._uri = uri
         self._route = route
         self._params: dict[str, str | int] = {}
 
     @property
     def route(self) -> Route:
         """The route itself."""
         return self._route
 
     @property
     def uri(self) -> str:
         """The routes uri endpoint."""
-        return self.route.uri
+        return self._uri
+
+    @uri.setter
+    def uri(self, uri: str) -> None:
+        self._uri = uri
 
     @property
     def method(self) -> str:
         """The routes method, i.e. GET, POST..."""
         return self.route.method
 
     @property
@@ -92,18 +97,18 @@
 
         Args:
             *args: The arguments to insert into the uri.
 
         Returns:
             The compiled route.
         """
-        compiled = CompiledRoute(self)
+        compiled = CompiledRoute(self, self.uri)
 
         for arg in args:
-            compiled.route.uri = compiled.uri.replace(r"{}", str(arg), 1)
+            compiled.uri = compiled.uri.replace(r"{}", str(arg), 1)
 
         return compiled
 
 
 SEARCH_PLAYERS: t.Final[Route] = Route("GET", "/players/search")
 UPDATE_PLAYER: t.Final[Route] = Route("POST", "/players/{}")
 ASSERT_PLAYER_TYPE: t.Final[Route] = Route("POST", "/players/{}/assert-type")
```

### Comparing `wom_py-0.3.2/wom/serializer.py` & `wom_py-0.3.3/wom/serializer.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/services/__init__.py` & `wom_py-0.3.3/wom/services/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/services/base.py` & `wom_py-0.3.3/wom/services/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/services/competitions.py` & `wom_py-0.3.3/wom/services/competitions.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/services/deltas.py` & `wom_py-0.3.3/wom/services/deltas.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/services/efficiency.py` & `wom_py-0.3.3/wom/services/efficiency.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/services/groups.py` & `wom_py-0.3.3/wom/services/groups.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/services/http.py` & `wom_py-0.3.3/wom/services/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/services/names.py` & `wom_py-0.3.3/wom/services/names.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/services/players.py` & `wom_py-0.3.3/wom/services/players.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/wom/services/records.py` & `wom_py-0.3.3/wom/services/records.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.2/PKG-INFO` & `wom_py-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wom-py
-Version: 0.3.2
+Version: 0.3.3
 Summary: An asynchronous wrapper for the Wise Old Man API.
 Home-page: https://github.com/Jonxslays/wom.py
 License: MIT
 Author: Jonxslays
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

