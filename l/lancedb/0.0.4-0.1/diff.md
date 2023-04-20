# Comparing `tmp/lancedb-0.0.4.tar.gz` & `tmp/lancedb-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lancedb-0.0.4.tar", last modified: Tue Apr 18 16:23:07 2023, max compression
+gzip compressed data, was "lancedb-0.1.tar", last modified: Thu Apr 20 06:34:05 2023, max compression
```

## Comparing `lancedb-0.0.4.tar` & `lancedb-0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-18 16:23:07.529026 lancedb-0.0.4/
--rw-r--r--   0 changshe   (501) staff       (20)      996 2023-04-18 16:23:07.528901 lancedb-0.0.4/PKG-INFO
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-18 16:23:07.527813 lancedb-0.0.4/lancedb/
--rw-r--r--   0 changshe   (501) staff       (20)      922 2023-03-18 17:14:30.000000 lancedb-0.0.4/lancedb/__init__.py
--rw-r--r--   0 changshe   (501) staff       (20)      889 2023-03-22 23:02:41.000000 lancedb-0.0.4/lancedb/common.py
--rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-03-24 06:56:52.000000 lancedb-0.0.4/lancedb/context.py
--rw-r--r--   0 changshe   (501) staff       (20)     2756 2023-03-24 06:56:52.000000 lancedb-0.0.4/lancedb/db.py
--rw-r--r--   0 changshe   (501) staff       (20)     3644 2023-03-31 02:15:49.000000 lancedb-0.0.4/lancedb/embeddings.py
--rw-r--r--   0 changshe   (501) staff       (20)     3336 2023-03-24 06:56:52.000000 lancedb-0.0.4/lancedb/query.py
--rw-r--r--   0 changshe   (501) staff       (20)     6645 2023-04-18 16:20:06.000000 lancedb-0.0.4/lancedb/table.py
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-18 16:23:07.528343 lancedb-0.0.4/lancedb.egg-info/
--rw-r--r--   0 changshe   (501) staff       (20)      996 2023-04-18 16:23:07.000000 lancedb-0.0.4/lancedb.egg-info/PKG-INFO
--rw-r--r--   0 changshe   (501) staff       (20)      386 2023-04-18 16:23:07.000000 lancedb-0.0.4/lancedb.egg-info/SOURCES.txt
--rw-r--r--   0 changshe   (501) staff       (20)        1 2023-04-18 16:23:07.000000 lancedb-0.0.4/lancedb.egg-info/dependency_links.txt
--rw-r--r--   0 changshe   (501) staff       (20)      143 2023-04-18 16:23:07.000000 lancedb-0.0.4/lancedb.egg-info/requires.txt
--rw-r--r--   0 changshe   (501) staff       (20)        8 2023-04-18 16:23:07.000000 lancedb-0.0.4/lancedb.egg-info/top_level.txt
--rw-r--r--   0 changshe   (501) staff       (20)     1318 2023-04-18 16:20:39.000000 lancedb-0.0.4/pyproject.toml
--rw-r--r--   0 changshe   (501) staff       (20)       38 2023-04-18 16:23:07.529062 lancedb-0.0.4/setup.cfg
--rw-r--r--   0 changshe   (501) staff       (20)      660 2023-03-23 18:53:47.000000 lancedb-0.0.4/setup.py
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-18 16:23:07.528726 lancedb-0.0.4/tests/
--rw-r--r--   0 changshe   (501) staff       (20)     1346 2023-03-23 01:47:48.000000 lancedb-0.0.4/tests/test_db.py
--rw-r--r--   0 changshe   (501) staff       (20)     1527 2023-03-31 02:15:49.000000 lancedb-0.0.4/tests/test_embeddings.py
--rw-r--r--   0 changshe   (501) staff       (20)     1814 2023-03-23 01:47:48.000000 lancedb-0.0.4/tests/test_query.py
--rw-r--r--   0 changshe   (501) staff       (20)     3092 2023-04-18 16:20:06.000000 lancedb-0.0.4/tests/test_table.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-20 06:34:05.567274 lancedb-0.1/
+-rw-r--r--   0 changshe   (501) staff       (20)      994 2023-04-20 06:34:05.567124 lancedb-0.1/PKG-INFO
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-20 06:34:05.565726 lancedb-0.1/lancedb/
+-rw-r--r--   0 changshe   (501) staff       (20)      922 2023-03-18 17:14:30.000000 lancedb-0.1/lancedb/__init__.py
+-rw-r--r--   0 changshe   (501) staff       (20)      889 2023-03-22 23:02:41.000000 lancedb-0.1/lancedb/common.py
+-rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-03-24 06:56:52.000000 lancedb-0.1/lancedb/context.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3058 2023-04-20 04:26:50.000000 lancedb-0.1/lancedb/db.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3644 2023-04-20 04:26:39.000000 lancedb-0.1/lancedb/embeddings.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3336 2023-03-24 06:56:52.000000 lancedb-0.1/lancedb/query.py
+-rw-r--r--   0 changshe   (501) staff       (20)     7486 2023-04-20 04:26:50.000000 lancedb-0.1/lancedb/table.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-20 06:34:05.566264 lancedb-0.1/lancedb.egg-info/
+-rw-r--r--   0 changshe   (501) staff       (20)      994 2023-04-20 06:34:05.000000 lancedb-0.1/lancedb.egg-info/PKG-INFO
+-rw-r--r--   0 changshe   (501) staff       (20)      386 2023-04-20 06:34:05.000000 lancedb-0.1/lancedb.egg-info/SOURCES.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        1 2023-04-20 06:34:05.000000 lancedb-0.1/lancedb.egg-info/dependency_links.txt
+-rw-r--r--   0 changshe   (501) staff       (20)      150 2023-04-20 06:34:05.000000 lancedb-0.1/lancedb.egg-info/requires.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        8 2023-04-20 06:34:05.000000 lancedb-0.1/lancedb.egg-info/top_level.txt
+-rw-r--r--   0 changshe   (501) staff       (20)     1323 2023-04-20 06:25:59.000000 lancedb-0.1/pyproject.toml
+-rw-r--r--   0 changshe   (501) staff       (20)       38 2023-04-20 06:34:05.567312 lancedb-0.1/setup.cfg
+-rw-r--r--   0 changshe   (501) staff       (20)      660 2023-03-23 18:53:47.000000 lancedb-0.1/setup.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-20 06:34:05.566925 lancedb-0.1/tests/
+-rw-r--r--   0 changshe   (501) staff       (20)     2796 2023-04-20 04:26:50.000000 lancedb-0.1/tests/test_db.py
+-rw-r--r--   0 changshe   (501) staff       (20)     1527 2023-03-31 02:15:49.000000 lancedb-0.1/tests/test_embeddings.py
+-rw-r--r--   0 changshe   (501) staff       (20)     1814 2023-03-23 01:47:48.000000 lancedb-0.1/tests/test_query.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3763 2023-04-20 04:26:50.000000 lancedb-0.1/tests/test_table.py
```

### Comparing `lancedb-0.0.4/PKG-INFO` & `lancedb-0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.0.4
+Version: 0.1
 Summary: lancedb
 Author-email: Lance Devs <dev@eto.ai>
 Project-URL: repository, https://github.com/eto-ai/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.0.4/lancedb/__init__.py` & `lancedb-0.1/lancedb/__init__.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.4/lancedb/common.py` & `lancedb-0.1/lancedb/common.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.4/lancedb/context.py` & `lancedb-0.1/lancedb/context.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.4/lancedb/db.py` & `lancedb-0.1/lancedb/db.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,38 +51,46 @@
     def __contains__(self, name: str) -> bool:
         return name in self.table_names()
 
     def __getitem__(self, name: str) -> LanceTable:
         return self.open_table(name)
 
     def create_table(
-        self, name: str, data: DATA = None, schema: pa.Schema = None
+        self,
+        name: str,
+        data: DATA = None,
+        schema: pa.Schema = None,
+        mode: str = "create",
     ) -> LanceTable:
         """Create a table in the database.
 
         Parameters
         ----------
         name: str
             The name of the table.
         data: list, tuple, dict, pd.DataFrame; optional
             The data to insert into the table.
         schema: pyarrow.Schema; optional
             The schema of the table.
+        mode: str; default "create"
+            The mode to use when creating the table.
+            By default, if the table already exists, an exception is raised.
+            If you want to overwrite the table, use mode="overwrite".
 
         Note
         ----
         The vector index won't be created by default.
         To create the index, call the `create_index` method on the table.
 
         Returns
         -------
         A LanceTable object representing the table.
         """
         if data is not None:
-            tbl = LanceTable.create(self, name, data, schema)
+            tbl = LanceTable.create(self, name, data, schema, mode=mode)
         else:
             tbl = LanceTable(self, name)
         return tbl
 
     def open_table(self, name: str) -> LanceTable:
         """Open a table in the database.
```

### Comparing `lancedb-0.0.4/lancedb/embeddings.py` & `lancedb-0.1/lancedb/embeddings.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.4/lancedb/query.py` & `lancedb-0.1/lancedb/query.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.4/lancedb/table.py` & `lancedb-0.1/lancedb/table.py`

 * *Files 22% similar despite different names*

```diff
@@ -42,23 +42,49 @@
 
 
 class LanceTable:
     """
     A table in a LanceDB database.
     """
 
-    def __init__(self, connection: "lancedb.db.LanceDBConnection", name: str):
+    def __init__(
+        self, connection: "lancedb.db.LanceDBConnection", name: str, version: int = None
+    ):
         self._conn = connection
         self.name = name
+        self._version = version
+
+    def _reset_dataset(self):
+        try:
+            del self.__dict__["_dataset"]
+        except AttributeError:
+            pass
 
     @property
     def schema(self) -> pa.Schema:
         """Return the schema of the table."""
         return self._dataset.schema
 
+    def list_versions(self):
+        """List all versions of the table"""
+        return self._dataset.versions()
+
+    @property
+    def version(self):
+        """Get the current version of the table"""
+        return self._dataset.version
+
+    def checkout(self, version: int):
+        """Checkout a version of the table"""
+        max_ver = max([v["version"] for v in self._dataset.versions()])
+        if version < 1 or version > max_ver:
+            raise ValueError(f"Invalid version {version}")
+        self._version = version
+        self._reset_dataset()
+
     def __len__(self):
         return self._dataset.count_rows()
 
     def __repr__(self) -> str:
         return f"LanceTable({self.name})"
 
     def __str__(self) -> str:
@@ -88,24 +114,25 @@
         num_partitions: int
             The number of IVF partitions to use when creating the index.
             Default is 256.
         num_sub_vectors: int
             The number of PQ sub-vectors to use when creating the index.
             Default is 96.
         """
-        return self._dataset.create_index(
+        self._dataset.create_index(
             column=VECTOR_COLUMN_NAME,
             index_type="IVF_PQ",
             num_partitions=num_partitions,
             num_sub_vectors=num_sub_vectors,
         )
+        self._reset_dataset()
 
     @cached_property
     def _dataset(self) -> LanceDataset:
-        return lance.dataset(self._dataset_uri)
+        return lance.dataset(self._dataset_uri, version=self._version)
 
     def to_lance(self) -> LanceDataset:
         """Return the LanceDataset backing this table."""
         return self._dataset
 
     def add(self, data: DATA, mode: str = "append") -> int:
         """Add data to the table.
@@ -119,16 +146,17 @@
             "append" and "overwrite".
 
         Returns
         -------
         The number of vectors added to the table.
         """
         data = _sanitize_data(data, self.schema)
-        ds = lance.write_dataset(data, self._dataset_uri, mode=mode)
-        return ds.count_rows()
+        lance.write_dataset(data, self._dataset_uri, mode=mode)
+        self._reset_dataset()
+        return len(self)
 
     def search(self, query: VEC) -> LanceQueryBuilder:
         """Create a search query to find the nearest neighbors
         of the given query vector.
 
         Parameters
         ----------
@@ -144,18 +172,18 @@
         if isinstance(query, np.ndarray):
             query = query.astype(np.float32)
         else:
             raise TypeError(f"Unsupported query type: {type(query)}")
         return LanceQueryBuilder(self, query)
 
     @classmethod
-    def create(cls, db, name, data, schema=None):
+    def create(cls, db, name, data, schema=None, mode="create"):
         tbl = LanceTable(db, name)
         data = _sanitize_data(data, schema)
-        lance.write_dataset(data, tbl._dataset_uri, mode="create")
+        lance.write_dataset(data, tbl._dataset_uri, mode=mode)
         return tbl
 
 
 def _sanitize_schema(data: pa.Table, schema: pa.Schema = None) -> pa.Table:
     """Ensure that the table has the expected schema.
 
     Parameters
```

### Comparing `lancedb-0.0.4/lancedb.egg-info/PKG-INFO` & `lancedb-0.1/lancedb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.0.4
+Version: 0.1
 Summary: lancedb
 Author-email: Lance Devs <dev@eto.ai>
 Project-URL: repository, https://github.com/eto-ai/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.0.4/pyproject.toml` & `lancedb-0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "lancedb"
-version = "0.0.4"
-dependencies = ["pylance", "ratelimiter", "retry", "tqdm"]
+version = "0.1"
+dependencies = ["pylance>=0.4.3", "ratelimiter", "retry", "tqdm"]
 description = "lancedb"
 authors = [
     { name = "Lance Devs", email = "dev@eto.ai" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `lancedb-0.0.4/setup.py` & `lancedb-0.1/setup.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.4/tests/test_embeddings.py` & `lancedb-0.1/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.4/tests/test_query.py` & `lancedb-0.1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.4/tests/test_table.py` & `lancedb-0.1/tests/test_table.py`

 * *Files 22% similar despite different names*

```diff
@@ -95,18 +95,45 @@
     assert len(table) == 2
 
     count = table.add([{"vector": [6.3, 100.5], "item": "new", "price": 30.0}])
     assert count == 3
 
     expected = pa.Table.from_arrays(
         [
-            pa.FixedSizeListArray.from_arrays(pa.array([3.1, 4.1, 5.9, 26.5]), 2),
-            pa.array(["foo", "bar"]),
-            pa.array([10.0, 20.0]),
+            pa.FixedSizeListArray.from_arrays(
+                pa.array([3.1, 4.1, 5.9, 26.5, 6.3, 100.5]), 2
+            ),
+            pa.array(["foo", "bar", "new"]),
+            pa.array([10.0, 20.0, 30.0]),
         ],
-        schema=pa.schema([
-            pa.field("vector", pa.list_(pa.float32(), 2)),
-            pa.field("item", pa.string()),
-            pa.field("price", pa.float64()),
-        ]),
+        schema=pa.schema(
+            [
+                pa.field("vector", pa.list_(pa.float32(), 2)),
+                pa.field("item", pa.string()),
+                pa.field("price", pa.float64()),
+            ]
+        ),
     )
     assert expected == table.to_arrow()
+
+
+def test_versioning(db):
+    table = LanceTable.create(
+        db,
+        "test",
+        data=[
+            {"vector": [3.1, 4.1], "item": "foo", "price": 10.0},
+            {"vector": [5.9, 26.5], "item": "bar", "price": 20.0},
+        ],
+    )
+
+    assert len(table.list_versions()) == 1
+    assert table.version == 1
+
+    table.add([{"vector": [6.3, 100.5], "item": "new", "price": 30.0}])
+    assert len(table.list_versions()) == 2
+    assert table.version == 2
+    assert len(table) == 3
+
+    table.checkout(1)
+    assert table.version == 1
+    assert len(table) == 2
```

