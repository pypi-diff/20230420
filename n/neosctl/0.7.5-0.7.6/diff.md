# Comparing `tmp/neosctl-0.7.5.tar.gz` & `tmp/neosctl-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosctl-0.7.5.tar", max compression
+gzip compressed data, was "neosctl-0.7.6.tar", max compression
```

## Comparing `neosctl-0.7.5.tar` & `neosctl-0.7.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     2655 2023-04-10 08:51:16.732342 neosctl-0.7.5/README.md
--rw-r--r--   0        0        0       22 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/__init__.py
--rw-r--r--   0        0        0     4478 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/auth.py
--rw-r--r--   0        0        0     4526 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/cli.py
--rw-r--r--   0        0        0      224 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/constant.py
--rw-r--r--   0        0        0      723 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/consume.py
--rw-r--r--   0        0        0     3730 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/iam.py
--rw-r--r--   0        0        0     4989 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/kafka.py
--rw-r--r--   0        0        0    15038 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/metadata.py
--rw-r--r--   0        0        0     7010 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/product.py
--rw-r--r--   0        0        0     4420 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/profile.py
--rw-r--r--   0        0        0     3062 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/registry.py
--rw-r--r--   0        0        0     7189 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/schema.py
--rw-r--r--   0        0        0     5884 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/secret.py
--rw-r--r--   0        0        0    10601 2023-04-10 08:51:16.734342 neosctl-0.7.5/neosctl/source.py
--rw-r--r--   0        0        0    13142 2023-04-10 08:51:16.734342 neosctl-0.7.5/neosctl/spark.py
--rw-r--r--   0        0        0    12105 2023-04-10 08:51:16.734342 neosctl-0.7.5/neosctl/storage.py
--rw-r--r--   0        0        0     8339 2023-04-10 08:51:16.734342 neosctl-0.7.5/neosctl/util.py
--rw-r--r--   0        0        0     2712 2023-04-10 08:51:16.734342 neosctl-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     3552 1970-01-01 00:00:00.000000 neosctl-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     2655 2023-04-20 08:51:11.098121 neosctl-0.7.6/README.md
+-rw-r--r--   0        0        0       22 2023-04-20 08:51:11.098121 neosctl-0.7.6/neosctl/__init__.py
+-rw-r--r--   0        0        0     4478 2023-04-20 08:51:11.098121 neosctl-0.7.6/neosctl/auth.py
+-rw-r--r--   0        0        0     4613 2023-04-20 08:51:11.098121 neosctl-0.7.6/neosctl/cli.py
+-rw-r--r--   0        0        0      224 2023-04-20 08:51:11.098121 neosctl-0.7.6/neosctl/constant.py
+-rw-r--r--   0        0        0      723 2023-04-20 08:51:11.098121 neosctl-0.7.6/neosctl/consume.py
+-rw-r--r--   0        0        0     3730 2023-04-20 08:51:11.098121 neosctl-0.7.6/neosctl/iam.py
+-rw-r--r--   0        0        0     4989 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/kafka.py
+-rw-r--r--   0        0        0     2809 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/link.py
+-rw-r--r--   0        0        0    15038 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/metadata.py
+-rw-r--r--   0        0        0     8557 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/product.py
+-rw-r--r--   0        0        0     4420 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/profile.py
+-rw-r--r--   0        0        0     3062 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/registry.py
+-rw-r--r--   0        0        0     7596 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/schema.py
+-rw-r--r--   0        0        0     5884 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/secret.py
+-rw-r--r--   0        0        0    12329 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/source.py
+-rw-r--r--   0        0        0    13142 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/spark.py
+-rw-r--r--   0        0        0    12105 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/storage.py
+-rw-r--r--   0        0        0     8339 2023-04-20 08:51:11.100121 neosctl-0.7.6/neosctl/util.py
+-rw-r--r--   0        0        0     2712 2023-04-20 08:51:11.100121 neosctl-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     3552 1970-01-01 00:00:00.000000 neosctl-0.7.6/PKG-INFO
```

### Comparing `neosctl-0.7.5/README.md` & `neosctl-0.7.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Core CLI v0.7.5
+# Core CLI v0.7.6
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

### Comparing `neosctl-0.7.5/neosctl/auth.py` & `neosctl-0.7.6/neosctl/auth.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.5/neosctl/cli.py` & `neosctl-0.7.6/neosctl/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import neosctl
 from neosctl import (
     auth,
     constant,
     consume,
     iam,
     kafka,
+    link,
     metadata,
     product,
     profile,
     registry,
     schema,
     secret,
     source,
@@ -137,7 +138,8 @@
 app.add_typer(metadata.app, name="metadata", callback=_common, help="Manage and browse metadata.")
 app.add_typer(product.app, name="product", callback=_common, help="Manage data products.")
 app.add_typer(source.app, name="source", help="Manage sources.")
 app.add_typer(registry.app, name="registry", callback=_common, help="Manage cores and search data products.")
 app.add_typer(spark.app, name="spark", callback=_common, help="Manage data product spark jobs.")
 app.add_typer(secret.app, name="secret", callback=_common, help="Manage secrets.")
 app.add_typer(kafka.app, name="kafka", callback=_common, help="Manage data product kafka streaming.")
+app.add_typer(link.app, name="link", callback=_common, help="Manage links.")
```

### Comparing `neosctl-0.7.5/neosctl/consume.py` & `neosctl-0.7.6/neosctl/consume.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.5/neosctl/iam.py` & `neosctl-0.7.6/neosctl/iam.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.5/neosctl/kafka.py` & `neosctl-0.7.6/neosctl/kafka.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.5/neosctl/metadata.py` & `neosctl-0.7.6/neosctl/metadata.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.5/neosctl/product.py` & `neosctl-0.7.6/neosctl/product.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,34 +32,37 @@
         help="Data Product description",
         callback=util.sanitize,
     ),
     filepath: str = typer.Option(
         ...,
         "--filepath",
         "-f",
-        help="Filepath of the details json payload",
+        help="Filepath of the details and info json payload",
         callback=util.sanitize,
     ),
 ) -> None:
     """Create a data product."""
 
     @ensure_login
     def _request(ctx: typer.Context, dpc: schema.CreateDataProduct) -> httpx.Response:
         return util.post(
             ctx,
             f"{_product_url(ctx)}",
             json=dpc.dict(exclude_none=True, by_alias=True),
         )
 
     fp = util.get_file_location(filepath)
-    details = util.load_object_file(fp, "details")
+    content = util.load_object_file(fp, "details")
+    details = content["details"]
+    info = content["info"]
 
     dpc = schema.CreateDataProduct(
         name=name,
         description=description or "",
+        info=info,  # type: ignore[reportGeneralTypeIssues]
         details=details,  # type: ignore[reportGeneralTypeIssues]
     )
 
     r = _request(ctx, dpc)
     process_response(r)
 
 
@@ -90,14 +93,45 @@
 
     dps = schema.UpdateDataProductSchema(details=details)  # type: ignore[reportGeneralTypeIssues]
 
     r = _request(ctx, dps)
     process_response(r)
 
 
+@app.command(name="update-info")
+def update_info(
+    ctx: typer.Context,
+    product_identifier: str = typer.Argument(..., help="Data Product identifier", callback=util.sanitize),
+    filepath: str = typer.Option(
+        ...,
+        "--filepath",
+        "-f",
+        help="Filepath of the info json payload",
+        callback=util.sanitize,
+    ),
+) -> None:
+    """Update data product info."""
+
+    @ensure_login
+    def _request(ctx: typer.Context, dps: schema.UpdateDataProductInfo) -> httpx.Response:
+        return util.put(
+            ctx,
+            f"{_product_url(ctx)}/{product_identifier}/info",
+            json=dps.dict(exclude_none=True, by_alias=True),
+        )
+
+    fp = util.get_file_location(filepath)
+    info = util.load_object_file(fp, "info")
+
+    dps = schema.UpdateDataProductInfo(info=info)  # type: ignore[reportGeneralTypeIssues]
+
+    r = _request(ctx, dps)
+    process_response(r)
+
+
 @app.command(name="list")
 def list_products(
     ctx: typer.Context,
     filter_: typing.Optional[str] = typer.Option(
         None,
         "--filter",
         "-f",
@@ -241,14 +275,36 @@
             f"{_product_url(ctx)}/{product_identifier}",
         )
 
     r = _request(ctx)
     process_response(r)
 
 
+@app.command(name="get-links")
+def get_product_links(
+    ctx: typer.Context,
+    product_identifier: str = typer.Argument(
+        ...,
+        help="Data Product identifier",
+        callback=util.sanitize,
+    ),
+) -> None:
+    """Get data product links."""
+
+    @ensure_login
+    def _request(ctx: typer.Context) -> httpx.Response:
+        return util.get(
+            ctx,
+            f"{_product_url(ctx)}/{product_identifier}/link",
+        )
+
+    r = _request(ctx)
+    process_response(r)
+
+
 @app.command()
 def preview(
     ctx: typer.Context,
     product_identifier: str = typer.Argument(
         ...,
         help="Data Product identifier",
         callback=util.sanitize,
```

### Comparing `neosctl-0.7.5/neosctl/profile.py` & `neosctl-0.7.6/neosctl/profile.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.5/neosctl/registry.py` & `neosctl-0.7.6/neosctl/registry.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.5/neosctl/schema.py` & `neosctl-0.7.6/neosctl/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,17 +62,26 @@
 
 class CreateStoredDataProduct(pydantic.BaseModel):
     name: str
     description: str
     details: StoredSchemaBase
 
 
+class Info(pydantic.BaseModel):
+    label: str
+    owner: Union[str, None]
+    contact_ids: List[str]
+    links: List[str]
+    notes: Union[str, None]
+
+
 class CreateDataProduct(pydantic.BaseModel):
     name: str
     description: str
+    info: Info
     details: Union[StoredSchemaBase, CreateStreamingSchema, SubsetSchema] = pydantic.Field(..., discriminator="type")
 
 
 class StreamingDataProductSchema(StreamingSchemaBase):
     fields: List[FieldDefinition]
 
 
@@ -80,14 +89,18 @@
     fields: List[FieldDefinition]
 
 
 class UpdateDataProductSchema(pydantic.BaseModel):
     details: Union[StreamingDataProductSchema, StoredDataProductSchema] = pydantic.Field(..., discriminator="type")
 
 
+class UpdateDataProductInfo(pydantic.BaseModel):
+    info: Info
+
+
 class ExpectationItem(pydantic.BaseModel):
     expectation_type: str
     kwargs: dict
     meta: dict
 
 
 class ExpectationWeights(pydantic.BaseModel):
@@ -125,14 +138,24 @@
 class RemoveCore(BaseModel):
     urn: str
 
 
 class CreateSource(pydantic.BaseModel):
     name: str
     description: Union[str, None] = None
+    info: Info
+
+
+class UpdateSource(pydantic.BaseModel):
+    name: str
+    description: Union[str, None] = None
+
+
+class UpdateSourceInfo(pydantic.BaseModel):
+    info: Info
 
 
 class ExternalDatabaseConnectionDetails(pydantic.BaseModel):
     type: Literal["external_database"]  # noqa: A003
     engine: str
     schema_: str = pydantic.Field(..., alias="schema")
     host: str
```

### Comparing `neosctl-0.7.5/neosctl/secret.py` & `neosctl-0.7.6/neosctl/secret.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.5/neosctl/source.py` & `neosctl-0.7.6/neosctl/source.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,26 +28,39 @@
 
 
 @app.command()
 def create_source(
     ctx: typer.Context,
     name: str = typer.Option(..., "--name", "-n", help="Source name", callback=util.sanitize),
     description: str = typer.Option(..., "--description", "-d", help="Source description", callback=util.sanitize),
+    filepath: str = typer.Option(
+        ...,
+        "--filepath",
+        "-f",
+        help="Filepath of the info json payload",
+        callback=util.sanitize,
+    ),
 ) -> None:
     """Create a new source."""
 
     @ensure_login
     def _request(ctx: typer.Context, content: schema.CreateSource) -> httpx.Response:
         return util.post(
             ctx,
             url=_source_url(ctx),
             json=content.dict(exclude_none=True, by_alias=True),
         )
 
-    payload = schema.CreateSource(name=name, description=description)
+    fp = util.get_file_location(filepath)
+    info = util.load_object_file(fp, "info")
+    payload = schema.CreateSource(
+        name=name,
+        description=description,
+        info=info,  # type: ignore[reportGeneralTypeIssues]
+    )
     r = _request(ctx, payload)
     process_response(r)
 
 
 @app.command()
 def list_sources(
     ctx: typer.Context,
@@ -79,14 +92,32 @@
             url=f"{_source_url(ctx)}/{source_identifier}",
         )
 
     r = _request(ctx)
     process_response(r)
 
 
+@app.command(name="get-source-links")
+def get_source_links(
+    ctx: typer.Context,
+    source_identifier: int = typer.Argument(..., help="Source identifier", callback=util.sanitize),
+) -> None:
+    """Get source links."""
+
+    @ensure_login
+    def _request(ctx: typer.Context) -> httpx.Response:
+        return util.get(
+            ctx,
+            f"{_source_url(ctx)}/{source_identifier}/link",
+        )
+
+    r = _request(ctx)
+    process_response(r)
+
+
 @app.command()
 def update_source(
     ctx: typer.Context,
     source_identifier: int = typer.Argument(..., help="Source identifier", callback=util.sanitize),
     filepath: str = typer.Option(
         ...,
         "--filepath",
@@ -94,24 +125,53 @@
         help="Filepath of the source json payload",
         callback=util.sanitize,
     ),
 ) -> None:
     """Update a source."""
 
     @ensure_login
-    def _request(ctx: typer.Context, content: schema.CreateSource) -> httpx.Response:
+    def _request(ctx: typer.Context, content: schema.UpdateSource) -> httpx.Response:
         return util.put(
             ctx,
             url=f"{_source_url(ctx)}/{source_identifier}",
             json=content.dict(exclude_none=True, by_alias=True),
         )
 
     fp = util.get_file_location(filepath)
     file_content: dict = util.load_json_file(fp, "json")  # type: ignore[reportGeneralTypeIssues]
-    payload = schema.CreateSource(**file_content)
+    payload = schema.UpdateSource(**file_content)
+    r = _request(ctx, payload)
+    process_response(r)
+
+
+@app.command()
+def update_source_info(
+    ctx: typer.Context,
+    source_identifier: int = typer.Argument(..., help="Source identifier", callback=util.sanitize),
+    filepath: str = typer.Option(
+        ...,
+        "--filepath",
+        "-f",
+        help="Filepath of the source info json payload",
+        callback=util.sanitize,
+    ),
+) -> None:
+    """Update a source info."""
+
+    @ensure_login
+    def _request(ctx: typer.Context, content: schema.UpdateSourceInfo) -> httpx.Response:
+        return util.put(
+            ctx,
+            url=f"{_source_url(ctx)}/{source_identifier}/info",
+            json=content.dict(exclude_none=True, by_alias=True),
+        )
+
+    fp = util.get_file_location(filepath)
+    file_content: dict = util.load_json_file(fp, "info")  # type: ignore[reportGeneralTypeIssues]
+    payload = schema.UpdateSourceInfo(**file_content)
     r = _request(ctx, payload)
     process_response(r)
 
 
 @app.command()
 def delete_source(
     ctx: typer.Context,
```

### Comparing `neosctl-0.7.5/neosctl/spark.py` & `neosctl-0.7.6/neosctl/spark.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.5/neosctl/storage.py` & `neosctl-0.7.6/neosctl/storage.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.5/neosctl/util.py` & `neosctl-0.7.6/neosctl/util.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.5/pyproject.toml` & `neosctl-0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neosctl"
-version = "0.7.5"
+version = "0.7.6"
 description = "Nortal Core CLI"
 authors = []
 license = "closed"
 repository="https://github.com/NEOS-Critical/neos-platform-cli"
 homepage="https://github.com/NEOS-Critical/neos-platform-cli"
 readme = "README.md"
```

### Comparing `neosctl-0.7.5/PKG-INFO` & `neosctl-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosctl
-Version: 0.7.5
+Version: 0.7.6
 Summary: Nortal Core CLI
 Home-page: https://github.com/NEOS-Critical/neos-platform-cli
 License: closed
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -16,15 +16,15 @@
 Requires-Dist: jq (>=1.4.0,<2.0.0) ; sys_platform != "win32"
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Requires-Dist: typing_extensions (>=4.4.0,<5.0.0) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/NEOS-Critical/neos-platform-cli
 Description-Content-Type: text/markdown
 
-# Core CLI v0.7.5
+# Core CLI v0.7.6
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

