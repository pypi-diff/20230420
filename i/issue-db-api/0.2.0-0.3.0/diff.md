# Comparing `tmp/issue_db_api-0.2.0.tar.gz` & `tmp/issue_db_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.2.0.tar", last modified: Thu Apr 20 09:21:05 2023, max compression
+gzip compressed data, was "issue_db_api-0.3.0.tar", last modified: Thu Apr 20 10:16:32 2023, max compression
```

## Comparing `issue_db_api-0.2.0.tar` & `issue_db_api-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 09:21:05.632223 issue_db_api-0.2.0/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.2.0/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-20 09:21:05.632223 issue_db_api-0.2.0/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 09:21:05.628224 issue_db_api-0.2.0/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      469 2023-04-20 09:20:00.000000 issue_db_api-0.2.0/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     7188 2023-04-20 09:14:52.000000 issue_db_api-0.2.0/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 09:21:05.632223 issue_db_api-0.2.0/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    41427 2023-04-20 09:17:20.000000 issue_db_api-0.2.0/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3767 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    34087 2023-04-20 09:13:55.000000 issue_db_api-0.2.0/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10105 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3710 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5316 2023-04-20 09:13:55.000000 issue_db_api-0.2.0/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 09:21:05.632223 issue_db_api-0.2.0/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 09:21:05.628224 issue_db_api-0.2.0/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-20 09:21:05.000000 issue_db_api-0.2.0/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-04-20 09:21:05.000000 issue_db_api-0.2.0/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.2.0/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.2.0/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-04-20 09:21:05.000000 issue_db_api-0.2.0/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-04-20 09:20:00.000000 issue_db_api-0.2.0/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-04-20 09:21:05.632223 issue_db_api-0.2.0/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 10:16:32.495521 issue_db_api-0.3.0/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.3.0/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-20 10:16:32.495521 issue_db_api-0.3.0/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 10:16:32.491521 issue_db_api-0.3.0/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      469 2023-04-20 10:15:51.000000 issue_db_api-0.3.0/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     7670 2023-04-20 10:10:15.000000 issue_db_api-0.3.0/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 10:16:32.495521 issue_db_api-0.3.0/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    41427 2023-04-20 09:17:20.000000 issue_db_api-0.3.0/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3767 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    35234 2023-04-20 10:11:50.000000 issue_db_api-0.3.0/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-20 10:10:15.000000 issue_db_api-0.3.0/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3710 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5660 2023-04-20 09:58:42.000000 issue_db_api-0.3.0/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 10:16:32.495521 issue_db_api-0.3.0/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 10:16:32.495521 issue_db_api-0.3.0/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-20 10:16:32.000000 issue_db_api-0.3.0/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-04-20 10:16:32.000000 issue_db_api-0.3.0/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 10:16:32.000000 issue_db_api-0.3.0/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.3.0/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-04-20 10:16:32.000000 issue_db_api-0.3.0/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-04-20 10:15:51.000000 issue_db_api-0.3.0/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-04-20 10:16:32.495521 issue_db_api-0.3.0/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.3.0/setup.py
```

### Comparing `issue_db_api-0.2.0/LICENSE` & `issue_db_api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.2.0/PKG-INFO` & `issue_db_api-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.2.0
+Version: 0.3.0
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.2.0/issue_db_api/issue_api.pyi` & `issue_db_api-0.3.0/issue_db_api/issue_api.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     def find_issues_by_key(self, *args: tuple[str, str]) -> list[Issue]:
         ...
 
     @property
     def models(self) -> list[Model]:
         ...
 
+    def get_model_by_id(self, id: str) -> Model:
+        ...
+
     def add_model(self, name: str, config: dict[str, typing.Any]) -> Model:
         ...
 
 
 class Repo:
     def __repr__(self) -> str:
         ...
@@ -331,14 +334,18 @@
     def __eq__(self, other) -> bool:
         ...
 
     def __hash__(self) -> int:
         ...
 
     @property
+    def identifier(self) -> str:
+        ...
+
+    @property
     def name(self) -> str:
         ...
 
     @name.setter
     def name(self, name: str):
         ...
 
@@ -350,24 +357,30 @@
     def config(self, config: dict[str, typing.Any]):
         ...
 
     @property
     def versions(self) -> list[Version]:
         ...
 
+    def get_version_by_id(self, id: str) -> Version:
+        ...
+
     def add_version(self, path: str, description: str | None = None) -> Version:
         ...
 
     def remove_version(self, version: Version):
         ...
 
     @property
     def test_runs(self) -> list[TestRun]:
         ...
 
+    def get_run_by_id(self, id: str) -> TestRun:
+        ...
+
     def add_test_run(self,
                      data: list[typing.Any],
                      description: str | None = None) -> TestRun:
         ...
 
     def delete_test_run(self, run: TestRun):
         ...
@@ -377,14 +390,22 @@
 
     def __repr__(self) -> str:
         ...
 
     def __eq__(self, other) -> bool:
         ...
 
+    @property
+    def model_id(self) -> str:
+        ...
+
+    @property
+    def version_id(self) -> str:
+        ...
+
     def download(self, path: str):
         ...
 
     @property
     def predictions(self) -> dict[str, typing.Any]:
         ...
 
@@ -406,14 +427,22 @@
 
 class TestRun:
 
     def __repr__(self) -> str:
         ...
 
     @property
+    def model_id(self) -> str:
+        ...
+
+    @property
+    def run_id(self) -> str:
+        ...
+
+    @property
     def data(self) -> list[typing.Any]:
         ...
 
     @property
     def description(self) -> str:
         ...
```

### Comparing `issue_db_api-0.2.0/issue_db_api/src/api_core.rs` & `issue_db_api-0.3.0/issue_db_api/src/api_core.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.2.0/issue_db_api/src/comments.rs` & `issue_db_api-0.3.0/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.2.0/issue_db_api/src/config.rs` & `issue_db_api-0.3.0/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.2.0/issue_db_api/src/embedding.rs` & `issue_db_api-0.3.0/issue_db_api/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.2.0/issue_db_api/src/errors.rs` & `issue_db_api-0.3.0/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.2.0/issue_db_api/src/issues.rs` & `issue_db_api-0.3.0/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.2.0/issue_db_api/src/labels.rs` & `issue_db_api-0.3.0/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.2.0/issue_db_api/src/lib.rs` & `issue_db_api-0.3.0/issue_db_api/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     }
 
     #[pymethods]
     impl PyIssueRepository {
         #[new]
         #[pyo3(signature=(
             url, *,
-            credentials,
+            credentials=None,
             label_caching_policy="no_caching",
             config_handling_policy="read_fetch_write_fetch",
             allow_self_signed_certificates=false
         ))]
         fn __new__(url: String,
                    credentials: Option<(String, String)>,
                    label_caching_policy: &str,
@@ -278,14 +278,19 @@
             let result = api2py_error(self.repo.models())?
                 .into_iter()
                 .map(|m| PyModel{inner: m})
                 .collect();
             Ok(result)
         }
 
+        fn get_model_by_id(&self, id: String) -> PyResult<PyModel> {
+            let m = PyModel{inner: api2py_error(self.repo.get_model_by_id(id))?};
+            Ok(m)
+        }
+
         fn add_model(&self, name: String, config: HashMap<String, &PyAny>) -> PyResult<PyModel> {
             let mut converted = HashMap::with_capacity(config.len());
             for (k, v) in config {
                 converted.insert(k, py_to_json(v)?);
             }
             let model = api2py_error(self.repo.add_model(name, converted))?;
             Ok(PyModel{inner: model})
@@ -842,14 +847,19 @@
                 CompareOp::Eq => (self.inner == other.inner).into_py(py),
                 CompareOp::Ne => (self.inner != other.inner).into_py(py),
                 _ => py.NotImplemented(),
             }
         }
 
         #[getter]
+        fn identifier(&self) -> PyResult<String> {
+            Ok(self.inner.identifier())
+        }
+
+        #[getter]
         fn name(&self) -> PyResult<String> {
             api2py_error(self.inner.name())
         }
 
         #[setter]
         fn set_name(&mut self, name: String) -> PyResult<()> {
             api2py_error(self.inner.update_name(name))
@@ -880,14 +890,19 @@
             let result = api2py_error(self.inner.model_versions())?;
             let converted = result.into_iter()
                 .map(|v| PyVersion{inner: v})
                 .collect();
             Ok(converted)
         }
 
+        fn get_version_by_id(&self, id: String) -> PyResult<PyVersion> {
+            let v = PyVersion{inner: api2py_error(self.inner.get_version_by_id(id))?};
+            Ok(v)
+        }
+
         fn add_version(&self, path: String, description: Option<String>) -> PyResult<PyVersion> {
             let version = api2py_error(self.inner.upload_version(path, description))?;
             Ok(PyVersion{inner: version})
         }
 
         fn remove_version(&self, version: &PyVersion) -> PyResult<()> {
             api2py_error(self.inner.delete_version(version.inner.clone()))
@@ -898,14 +913,19 @@
             let result = api2py_error(self.inner.model_runs())?;
             let converted = result.into_iter()
                 .map(|r| PyPerformance{inner: r})
                 .collect();
             Ok(converted)
         }
 
+        fn get_run_by_id(&self, id: String) -> PyResult<PyPerformance> {
+            let r = PyPerformance{inner: api2py_error(self.inner.get_run_by_id(id))?};
+            Ok(r)
+        }
+
         fn add_test_run(&self, data: Vec<&PyAny>, description: Option<String>) -> PyResult<PyPerformance> {
             let mut converted = Vec::with_capacity(data.len());
             for obj in data {
                 converted.push(py_to_json(obj)?);
             }
             let run = api2py_error(self.inner.store_run(converted, description))?;
             Ok(PyPerformance{inner: run})
@@ -936,14 +956,24 @@
             match op {
                 CompareOp::Eq => (self.inner == other.inner).into_py(py),
                 CompareOp::Ne => (self.inner != other.inner).into_py(py),
                 _ => py.NotImplemented(),
             }
         }
 
+        #[getter]
+        fn model_id(&self) -> PyResult<String> {
+            Ok(self.inner.model_id())
+        }
+
+        #[getter]
+        fn version_id(&self) -> PyResult<String> {
+            Ok(self.inner.version_id())
+        }
+
         fn download(&self, path: String) -> PyResult<()> {
             api2py_error(self.inner.download(path))
         }
 
         #[getter]
         fn predictions(&self, py: Python<'_>) -> PyResult<PyObject> {
             let pred = api2py_error(self.inner.get_predictions(None))?;
@@ -990,14 +1020,24 @@
             let text = format!(
                 "<TestRun|model_id={}, id={}>", self.inner.model_id(), self.inner.run_id()
             );
             Ok(text)
         }
 
         #[getter]
+        fn model_id(&self) -> PyResult<String> {
+            Ok(self.inner.model_id())
+        }
+
+        #[getter]
+        fn run_id(&self) -> PyResult<String> {
+            Ok(self.inner.run_id())
+        }
+
+        #[getter]
         fn data(&self, py: Python<'_>) -> PyResult<Vec<PyObject>> {
             let result = api2py_error(self.inner.data())?;
             let mut converted = Vec::with_capacity(result.len());
             for fold in result {
                 converted.push(json_to_py(py, fold));
             }
             Ok(converted)
```

### Comparing `issue_db_api-0.2.0/issue_db_api/src/models.rs` & `issue_db_api-0.3.0/issue_db_api/src/models.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 use std::collections::HashMap;
 use std::hash::{Hash, Hasher};
 use std::sync::Arc;
 use serde_json::Value;
 use crate::api_core::IssueAPI;
 use crate::APIResult;
 use crate::config::ConfigHandlingPolicy;
+use crate::errors::APIError;
 use crate::util::CacheContainer;
 
 //////////////////////////////////////////////////////////////////////////////////////////////////
 //////////////////////////////////////////////////////////////////////////////////////////////////
 // Raw Models -- Used for Raw API responses
 //////////////////////////////////////////////////////////////////////////////////////////////////
 
@@ -107,16 +108,16 @@
             id,
             name,
             config: CacheContainer::new(config),
             data_policy: config_handling
         }
     }
 
-    pub(crate) fn identifier(&self) -> &String {
-        &self.id
+    pub fn identifier(&self) -> String {
+        self.id.clone()
     }
 
     pub fn name(&self) -> APIResult<String> {
         match self.data_policy {
             ConfigHandlingPolicy::ReadFetchWriteWithFetch => {
                 Ok(self.api.get_model_config(self.id.clone())?.model_name)
             },
@@ -203,14 +204,27 @@
         let converted = versions
             .into_iter()
             .map(|v| v.into_bound_model(self.api.clone()))
             .collect();
         Ok(converted)
     }
 
+    pub fn get_version_by_id(&self, id: String) -> APIResult<ModelVersion> {
+        let versions = self.model_versions()?;
+        let version = versions.into_iter()
+            .find(|v| v.version == id);
+        match version {
+            None => {
+                let text = format!("Could not find version with ID {id}");
+                Err(Box::new(APIError::new(text)))
+            },
+            Some(v) => Ok(v)
+        }
+    }
+
     pub fn model_runs(&self) -> APIResult<Vec<TestRun>> {
         let runs = self.api.get_performances_for_model(self.id.clone())?;
         let converted = runs
             .into_iter()
             .map(|r| r.into_bound_test_run(self.api.clone()))
             .collect();
         Ok(converted)
@@ -235,14 +249,27 @@
                 run: id,
                 description: String::new()
             }
         };
         Ok(run)
     }
 
+    pub fn get_run_by_id(&self, id: String) -> APIResult<TestRun> {
+        let runs = self.model_runs()?;
+        let run = runs.into_iter()
+            .find(|r| r.run == id);
+        match run {
+            None => {
+                let text = format!("Could not find test run with ID {id}");
+                Err(Box::new(APIError::new(text)))
+            },
+            Some(v) => Ok(v)
+        }
+    }
+
     pub fn delete_run(&self, run: TestRun) -> APIResult<()> {
         self.api.delete_performance_data(run.model, run.run)
     }
 }
 
 #[allow(unused)]
 #[derive(Debug, Clone)]
@@ -266,20 +293,20 @@
         self.version.hash(state);
         self.model.hash(state);
     }
 }
 
 #[allow(unused)]
 impl ModelVersion {
-    pub(crate) fn model_id(&self) -> &String {
-        &self.model
+    pub fn model_id(&self) -> String {
+        self.model.clone()
     }
 
-    pub(crate) fn version_id(&self) -> &String {
-        &self.version
+    pub fn version_id(&self) -> String {
+        self.version.clone()
     }
 
     pub fn description(&self) -> String {
         self.description.clone()
     }
 
     pub fn update_description(&mut self, description: String) -> APIResult<()> {
@@ -316,20 +343,20 @@
     model: String,
     run: String,
     description: String
 }
 
 #[allow(unused)]
 impl TestRun {
-    pub(crate) fn model_id(&self) -> &String {
-        &self.model
+    pub fn model_id(&self) -> String {
+        self.model.clone()
     }
 
-    pub(crate) fn run_id(&self) -> &String {
-        &self.run
+    pub fn run_id(&self) -> String {
+        self.run.clone()
     }
 
     pub fn data(&self) -> APIResult<Vec<Value>> {
         self.api.get_performance_data(self.model.clone(), self.run.clone())
     }
 
     pub fn description(&self) -> String {
```

### Comparing `issue_db_api-0.2.0/issue_db_api/src/query.rs` & `issue_db_api-0.3.0/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.2.0/issue_db_api/src/repository.rs` & `issue_db_api-0.3.0/issue_db_api/src/repository.rs`

 * *Files 10% similar despite different names*

```diff
@@ -135,14 +135,26 @@
                            m.model_id,
                            m.model_name,
                            None,
                            self.config_handling)
             ).collect();
         Ok(converted)
     }
+    
+    pub fn get_model_by_id(&self, id: String) -> APIResult<Model> {
+        let raw = self.api.get_model_config(id)?;
+        let model = Model::new(
+            self.api.clone(),
+            raw.model_id,
+            raw.model_name,
+            Some(raw.model_config),
+            self.config_handling
+        );
+        Ok(model)
+    }
 
     pub fn add_model(&self, name: String, config: HashMap<String, Value>) -> APIResult<Model> {
         let id = self.api.create_model_config(name.clone(), config.clone())?;
         let m = Model::new(
             self.api.clone(),
             id,
             name,
@@ -163,8 +175,8 @@
     pub fn name(&self) -> &String {
         &self.name 
     }
     
     pub fn projects(&self) -> APIResult<Vec<String>> {
         self.api.get_projects_for_repo(self.name.clone())
     }
-}
+}
```

### Comparing `issue_db_api-0.2.0/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.3.0/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.2.0/issue_db_api/src/tags.rs` & `issue_db_api-0.3.0/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.2.0/issue_db_api/src/util.rs` & `issue_db_api-0.3.0/issue_db_api/src/util.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.2.0/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.3.0/issue_db_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.2.0
+Version: 0.3.0
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.2.0/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.3.0/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.2.0/pyproject.toml` & `issue_db_api-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```

