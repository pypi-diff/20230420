# Comparing `tmp/servir-0.0.4.tar.gz` & `tmp/servir-0.0.5.tar.gz`

## Comparing `servir-0.0.4.tar` & `servir-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 servir-0.0.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 servir-0.0.4/.github/workflows/release.yml
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 servir-0.0.4/src/servir/__init__.py
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 servir-0.0.4/src/servir/_background_server.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 servir-0.0.4/src/servir/_protocols.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 servir-0.0.4/src/servir/_provide.py
--rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 servir-0.0.4/src/servir/_resources.py
--rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 servir-0.0.4/src/servir/_tilesets.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 servir-0.0.4/src/servir/_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 servir-0.0.4/src/servir/py.typed
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 servir-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 servir-0.0.4/tests/test_provider.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 servir-0.0.4/tests/test_servir.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 servir-0.0.4/tests/test_tilesets.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 servir-0.0.4/tests/test_util.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 servir-0.0.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 servir-0.0.4/LICENSE
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 servir-0.0.4/README.md
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 servir-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 servir-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 servir-0.0.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 servir-0.0.5/.github/workflows/release.yml
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/__init__.py
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/_background_server.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/_protocols.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/_provide.py
+-rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/_resources.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/_tilesets.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/py.typed
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 servir-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 servir-0.0.5/tests/test_provider.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 servir-0.0.5/tests/test_servir.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 servir-0.0.5/tests/test_tilesets.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 servir-0.0.5/tests/test_util.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 servir-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 servir-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 servir-0.0.5/README.md
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 servir-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 servir-0.0.5/PKG-INFO
```

### Comparing `servir-0.0.4/.github/workflows/ci.yml` & `servir-0.0.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `servir-0.0.4/.github/workflows/release.yml` & `servir-0.0.5/.github/workflows/release.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 name: Release
 
 on:
   push:
-    branches:
-      - main
     tags:
       - "v*"
-  workflow_dispatch:
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
 
@@ -26,9 +23,7 @@
           python -m pip install --upgrade pip
           pip install build
           python -m build
       - name: Publish distribution 📦 to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
-      - name: Release
-        uses: softprops/action-gh-release@v1
```

### Comparing `servir-0.0.4/src/servir/_background_server.py` & `servir-0.0.5/src/servir/_background_server.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.4/src/servir/_protocols.py` & `servir-0.0.5/src/servir/_protocols.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,19 @@
         """The URL for this provider."""
         ...
 
 
 class TilesetProtocol(typing.Protocol):
     """Represents a HiGlass Tileset."""
 
+    @property
+    def uid(self) -> str:
+        """The unique identifier for this tileset."""
+        ...
+
     def tiles(self, tile_ids: typing.Sequence[str]) -> list[typing.Any]:
         """Get the tiles for the given tile IDs.
 
         Parameters
         ----------
         tile_ids : list[str]
             The tile IDs to get.
```

### Comparing `servir-0.0.4/src/servir/_provide.py` & `servir-0.0.5/src/servir/_provide.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 from servir._background_server import BackgroundServer
 from servir._protocols import TilesetProtocol
 from servir._resources import (
     Resource,
     create_resource,
     create_resource_route,
 )
-from servir._tilesets import TilesetResource, create_tileset_route
+from servir._tilesets import TilesetResource, TilesetType, create_tileset_route
 
 
 class Provider(BackgroundServer):
     """A server that provides resources to a client."""
 
     _resources: typing.MutableMapping[str, Resource]
-    _tilesets: typing.MutableMapping[str, TilesetResource]
+    _tilesets: typing.MutableMapping[str, TilesetResource[TilesetProtocol]]
 
     def __init__(self, proxy: bool = False):
         """Create a new Provider.
 
         Parameters
         ----------
         proxy : bool, optional
@@ -79,39 +79,39 @@
 
     @typing.overload
     def create(self, path: pathlib.Path | str, /, **kwargs: typing.Any) -> Resource:
         ...
 
     @typing.overload
     def create(
-        self, tileset: TilesetProtocol, /, **kwargs: typing.Any
-    ) -> TilesetResource:
+        self, tileset: TilesetType, /, **kwargs: typing.Any
+    ) -> TilesetResource[TilesetType]:
         ...
 
     def create(
-        self, x: pathlib.Path | str | TilesetProtocol, /, **kwargs: typing.Any
-    ) -> Resource | TilesetResource:
+        self, x: pathlib.Path | str | TilesetType, /, **kwargs: typing.Any
+    ) -> Resource | TilesetResource[TilesetType]:
         """Create a resource from a path or tileset.
 
         Parameters
         ----------
         x : pathlib.Path | str | TilesetProtocol
             The path or tileset to create a resource from.
         **kwargs
             Additional keyword arguments to pass to the resource constructor.
 
         Returns
         -------
         Resource | TilesetResource
             The resource.
         """
-        resource: Resource | TilesetResource
+        resource: Resource | TilesetResource[TilesetProtocol]
 
         if not isinstance(x, (pathlib.Path, str)):
             resource = TilesetResource(x, provider=self, **kwargs)
             self._tilesets[resource.uid] = resource
         else:
             resource = create_resource(x, provider=self, **kwargs)
             self._resources[resource.guid] = resource
 
         self.start()
-        return resource
+        return typing.cast(TilesetResource[TilesetType], resource)
```

### Comparing `servir-0.0.4/src/servir/_resources.py` & `servir-0.0.5/src/servir/_resources.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.4/src/servir/_tilesets.py` & `servir-0.0.5/src/servir/_tilesets.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,46 +12,42 @@
 from servir._protocols import ProviderProtocol, TilesetProtocol
 
 # HiGlass
 
 
 _MOUNT_PATH = "/tilesets/api/v1/"
 
+TilesetType = typing.TypeVar("TilesetType", bound=TilesetProtocol)
 
-class TilesetResource:
+
+class TilesetResource(typing.Generic[TilesetType]):
     """A tileset resource."""
 
-    def __init__(
-        self, tileset: TilesetProtocol, provider: ProviderProtocol, uid: None | str = None
-    ):
+    def __init__(self, tileset: TilesetType, provider: ProviderProtocol):
         """Initialize a tileset resource.
 
         Parameters
         ----------
         tileset : TilesetProtocol
             The tileset.
         provider : ProviderProtocol
             The server provider.
-        uid : None | str, optional
-            The unique identifier for the tileset, by default None. If None, the
-            object id of the tileset instance will be used.
         """
         self._tileset = tileset
         self._provider = provider
-        self._uid = uid or str(id(tileset))
 
     @property
-    def tileset(self) -> TilesetProtocol:
+    def tileset(self) -> TilesetType:
         """The tileset."""
         return self._tileset
 
     @property
     def uid(self) -> str:
         """The unique identifier for the tileset."""
-        return self._uid
+        return self._tileset.uid
 
     @property
     def server(self) -> str:
         """The server url."""
         return f"{self._provider.url}{_MOUNT_PATH}"
 
 
@@ -71,15 +67,15 @@
         The list of values for the given field. For example, ['id1', 'id2', 'id3'].
     """
     kv_tuples = [x.split("=") for x in query.split("&")]
     return [v for k, v in kv_tuples if k == field]
 
 
 def tileset_info(
-    request: Request, tilesets: typing.Mapping[str, TilesetResource]
+    request: Request, tilesets: typing.Mapping[str, TilesetResource[TilesetProtocol]]
 ) -> JSONResponse:
     """Request handler for the tileset_info/ endpoint.
 
     Parameters
     ----------
     request : Request
         The request.
@@ -98,15 +94,15 @@
         else {"error": f"No such tileset with uid: {uid}"}
         for uid in uids
     }
     return JSONResponse(info)
 
 
 def tiles(
-    request: Request, tilesets: typing.Mapping[str, TilesetResource]
+    request: Request, tilesets: typing.Mapping[str, TilesetResource[TilesetProtocol]]
 ) -> JSONResponse:
     """Request handler for the tiles/ endpoint.
 
     Parameters
     ----------
     request : Request
         The request.
@@ -133,15 +129,15 @@
             )
         tiles.extend(tileset_resource.tileset.tiles(list(tids)))
     data = {tid: tval for tid, tval in tiles}
     return JSONResponse(data)
 
 
 def chromsizes(
-    request: Request, tilesets: typing.Mapping[str, TilesetResource]
+    request: Request, tilesets: typing.Mapping[str, TilesetResource[TilesetProtocol]]
 ) -> PlainTextResponse | JSONResponse:
     """Request handler for the chrom-sizes/ endpoint.
 
     Chromsizes are returned as a plain text response, as a TSV:
 
         chr1    249250621
         chr2    243199373
@@ -168,20 +164,20 @@
     assert "chromsizes" in info, "No chromsizes in tileset info"
     return PlainTextResponse(
         "\n".join(f"{chrom}\t{size}" for chrom, size in info["chromsizes"])
     )
 
 
 TilesetEndpoint = typing.Callable[
-    [Request, typing.Mapping[str, TilesetResource]], Response
+    [Request, typing.Mapping[str, TilesetResource[TilesetProtocol]]], Response
 ]
 
 
 def create_tileset_route(
-    tileset_resources: typing.Mapping[str, TilesetResource],
+    tileset_resources: typing.Mapping[str, TilesetResource[TilesetProtocol]],
     scope_id: str = "tilesets",
 ) -> Mount:
     """Create a route for tileset endpoints.
 
     Parameters
     ----------
     tileset_resources : typing.Mapping[str, TilesetResource]
```

### Comparing `servir-0.0.4/src/servir/_util.py` & `servir-0.0.5/src/servir/_util.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.4/tests/test_provider.py` & `servir-0.0.5/tests/test_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,14 +87,18 @@
 
     response = requests.get(server_resource.url + "/nested_dir/foo.txt")
     assert response.text == "foo"
 
 
 def test_tileset_resource(provider: Provider) -> None:
     class Tileset:
+        @property
+        def uid(self) -> str:
+            return "aaaaaaaaaa"
+
         def tiles(self, tile_ids: typing.Sequence[str]) -> list[typing.Any]:
             return [(tid, None) for tid in tile_ids]
 
         def info(self) -> typing.Any:
             return "tile_info"
 
     tileset = Tileset()
```

### Comparing `servir-0.0.4/tests/test_util.py` & `servir-0.0.5/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.4/LICENSE` & `servir-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `servir-0.0.4/README.md` & `servir-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `servir-0.0.4/pyproject.toml` & `servir-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `servir-0.0.4/PKG-INFO` & `servir-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servir
-Version: 0.0.4
+Version: 0.0.5
 Summary: an extensible async background server
 Project-URL: Documentation, https://github.com/unknown/servir#readme
 Project-URL: Issues, https://github.com/unknown/servir/issues
 Project-URL: Source, https://github.com/unknown/servir
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
```

