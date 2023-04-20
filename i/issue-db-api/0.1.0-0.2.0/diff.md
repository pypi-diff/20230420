# Comparing `tmp/issue_db_api-0.1.0.tar.gz` & `tmp/issue_db_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.1.0.tar", last modified: Wed Apr 19 13:30:33 2023, max compression
+gzip compressed data, was "issue_db_api-0.2.0.tar", last modified: Thu Apr 20 09:21:05 2023, max compression
```

## Comparing `issue_db_api-0.1.0.tar` & `issue_db_api-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 13:30:33.696788 issue_db_api-0.1.0/
--rw-rw-rw-   0        0        0       85 2023-04-19 13:01:57.000000 issue_db_api-0.1.0/.gitignore
--rw-rw-rw-   0        0        0     1087 2023-04-19 13:08:40.000000 issue_db_api-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      105 2023-04-18 10:26:56.000000 issue_db_api-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      567 2023-04-19 13:30:33.695788 issue_db_api-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-04-19 13:05:20.000000 issue_db_api-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 13:30:33.672793 issue_db_api-0.1.0/issue_db_api/
--rw-rw-rw-   0        0        0      469 2023-04-17 23:21:19.000000 issue_db_api-0.1.0/issue_db_api/Cargo.toml
--rw-rw-rw-   0        0        0       26 2023-04-18 10:17:02.000000 issue_db_api-0.1.0/issue_db_api/__init__.py
--rw-rw-rw-   0        0        0     7079 2023-04-19 12:57:15.000000 issue_db_api-0.1.0/issue_db_api/issue_api.pyi
-drwxrwxrwx   0        0        0        0 2023-04-19 13:30:33.693790 issue_db_api-0.1.0/issue_db_api/src/
--rw-rw-rw-   0        0        0    40325 2023-04-19 10:42:41.000000 issue_db_api-0.1.0/issue_db_api/src/api_core.rs
--rw-rw-rw-   0        0        0     1091 2023-04-17 16:51:29.000000 issue_db_api-0.1.0/issue_db_api/src/comments.rs
--rw-rw-rw-   0        0        0     5436 2023-04-18 23:34:45.000000 issue_db_api-0.1.0/issue_db_api/src/config.rs
--rw-rw-rw-   0        0        0     3893 2023-04-18 23:34:45.000000 issue_db_api-0.1.0/issue_db_api/src/embedding.rs
--rw-rw-rw-   0        0        0     1616 2023-04-18 18:21:49.000000 issue_db_api-0.1.0/issue_db_api/src/errors.rs
--rw-rw-rw-   0        0        0     8958 2023-04-18 16:39:25.000000 issue_db_api-0.1.0/issue_db_api/src/issues.rs
--rw-rw-rw-   0        0        0      600 2023-04-17 13:40:17.000000 issue_db_api-0.1.0/issue_db_api/src/labels.rs
--rw-rw-rw-   0        0        0    33092 2023-04-19 12:56:38.000000 issue_db_api-0.1.0/issue_db_api/src/lib.rs
--rw-rw-rw-   0        0        0     8434 2023-04-19 12:56:47.000000 issue_db_api-0.1.0/issue_db_api/src/models.rs
--rw-rw-rw-   0        0        0     3819 2023-04-16 15:57:56.000000 issue_db_api-0.1.0/issue_db_api/src/query.rs
--rw-rw-rw-   0        0        0     5330 2023-04-19 12:08:43.000000 issue_db_api-0.1.0/issue_db_api/src/repository.rs
-drwxrwxrwx   0        0        0        0 2023-04-19 13:30:33.694790 issue_db_api-0.1.0/issue_db_api/src/schemas/
--rw-rw-rw-   0        0        0     5182 2023-04-16 18:23:39.000000 issue_db_api-0.1.0/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-rw-   0        0        0       27 2023-04-11 16:23:13.000000 issue_db_api-0.1.0/issue_db_api/src/schemas.rs
--rw-rw-rw-   0        0        0     1693 2023-04-18 12:43:33.000000 issue_db_api-0.1.0/issue_db_api/src/tags.rs
--rw-rw-rw-   0        0        0     2552 2023-04-19 12:03:22.000000 issue_db_api-0.1.0/issue_db_api/src/util.rs
-drwxrwxrwx   0        0        0        0 2023-04-19 13:30:33.677790 issue_db_api-0.1.0/issue_db_api.egg-info/
--rw-rw-rw-   0        0        0      567 2023-04-19 13:30:33.000000 issue_db_api-0.1.0/issue_db_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      748 2023-04-19 13:30:33.000000 issue_db_api-0.1.0/issue_db_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 13:30:33.000000 issue_db_api-0.1.0/issue_db_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-18 10:19:03.000000 issue_db_api-0.1.0/issue_db_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-04-19 13:30:33.000000 issue_db_api-0.1.0/issue_db_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      549 2023-04-18 10:24:49.000000 issue_db_api-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 13:30:33.696788 issue_db_api-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      262 2023-04-18 12:36:23.000000 issue_db_api-0.1.0/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 09:21:05.632223 issue_db_api-0.2.0/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.2.0/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-20 09:21:05.632223 issue_db_api-0.2.0/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 09:21:05.628224 issue_db_api-0.2.0/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      469 2023-04-20 09:20:00.000000 issue_db_api-0.2.0/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     7188 2023-04-20 09:14:52.000000 issue_db_api-0.2.0/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 09:21:05.632223 issue_db_api-0.2.0/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    41427 2023-04-20 09:17:20.000000 issue_db_api-0.2.0/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3767 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    34087 2023-04-20 09:13:55.000000 issue_db_api-0.2.0/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10105 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3710 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5316 2023-04-20 09:13:55.000000 issue_db_api-0.2.0/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 09:21:05.632223 issue_db_api-0.2.0/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 09:21:05.628224 issue_db_api-0.2.0/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-20 09:21:05.000000 issue_db_api-0.2.0/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-04-20 09:21:05.000000 issue_db_api-0.2.0/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.2.0/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.2.0/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-04-20 09:21:05.000000 issue_db_api-0.2.0/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-04-20 09:20:00.000000 issue_db_api-0.2.0/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-04-20 09:21:05.632223 issue_db_api-0.2.0/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.2.0/setup.py
```

### Comparing `issue_db_api-0.1.0/LICENSE` & `issue_db_api-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2023 - Mining Design Decisions 
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2023 - Mining Design Decisions 
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `issue_db_api-0.1.0/PKG-INFO` & `issue_db_api-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
-Name: issue_db_api
-Version: 0.1.0
-Author: Jesse Maarleveld
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Issue DB API Client 
-
-This is an experimental work in progress auxiliary package for an ongoing research project. 
-
-More details will be added after the work is done, and all code will be published.
+Metadata-Version: 2.1
+Name: issue_db_api
+Version: 0.2.0
+Author: Jesse Maarleveld
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Issue DB API Client 
+
+This is an experimental work in progress auxiliary package for an ongoing research project. 
+
+More details will be added after the work is done, and all code will be published.
```

### Comparing `issue_db_api-0.1.0/issue_db_api/src/api_core.rs` & `issue_db_api-0.2.0/issue_db_api/src/api_core.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,1031 +1,1073 @@
-use std::collections::HashMap;
-
-#[cfg(feature = "blocking")]
-use reqwest::blocking::Client;
-use reqwest::blocking::multipart;
-
-use serde_json::{Map, Value};
-use lazy_init::Lazy;
-
-use crate::comments::UnboundComment;
-use crate::config::IssueAttribute;
-use crate::embedding::UnboundEmbedding;
-use crate::schemas::raw_issue_response::RawIssueData;
-use crate::query::Query;
-use crate::labels::Label;
-use crate::tags::UnboundTag;
-use crate::util::initialize_lazy_field;
-use crate::util::APIResult;
-use crate::errors::*;
-use crate::models::{ModelInfo, UnboundModelConfig, UnboundModelVersion, UnboundTestRun};
-
-//////////////////////////////////////////////////////////////////////////////////////////////////
-//////////////////////////////////////////////////////////////////////////////////////////////////
-// Core Structs
-//////////////////////////////////////////////////////////////////////////////////////////////////
-
-/// The IssueAPI struct provides a low-level wrapper around the issues API.
-/// This struct provides basics means of session management,
-/// and exposes all available endpoints through Rust functions.
-#[allow(unused)]
-#[derive(Debug, Clone)]
-pub struct IssueAPI {
-    url: String,
-    token: Option<String>,
-    client: Client
-}
-
-#[allow(unused)]
-#[derive(Debug, Clone)]
-pub struct IssueData {
-    ident: String,
-    key: Lazy<String>,
-    summary: Lazy<String>,
-    description: Lazy<String>,
-    comments: Lazy<Vec<String>>,
-    status: Lazy<String>,
-    priority: Lazy<String>,
-    resolution: Lazy<Option<String>>,
-    issue_type: Lazy<String>,
-    issue_links: Lazy<Vec<String>>,
-    parent: Lazy<Option<String>>,
-    subtasks: Lazy<Vec<String>>,
-    watches: Lazy<u64>,
-    votes: Lazy<u64>,
-    date_created: Lazy<String>,
-    date_updated: Lazy<String>,
-    date_resolved: Lazy<Option<String>>,
-    labels: Lazy<Vec<String>>,
-    components: Lazy<Vec<String>>,
-    affected_versions: Lazy<Vec<String>>,
-    fix_versions: Lazy<Vec<String>>
-}
-
-//////////////////////////////////////////////////////////////////////////////////////////////////
-//////////////////////////////////////////////////////////////////////////////////////////////////
-// Auxiliary structs and enums
-//////////////////////////////////////////////////////////////////////////////////////////////////
-
-#[allow(unused)]
-enum Verb {
-    Get,
-    Post,
-    Patch,
-    Delete
-}
-
-macro_rules! maybe_copy_attribute {
-    ($self:ident, $other:ident, $attr:ident) => {
-        {
-            if let Some(x) = $other.$attr.get() {
-                $self.$attr.get_or_create(|| x.clone());
-            }
-        }
-    }
-}
-
-macro_rules! load_lazy_attribute {
-    ($self:ident, $attr:ident, $e:expr, $api:expr) => {
-        {
-            if let Some(x) = $self.$attr.get() {
-                Ok(x)
-            } else {
-                let value = $api.get_issue_data(vec![$self.ident.clone()], vec![$e])?
-                    .get(&$self.ident)
-                    .expect("Issue data lookup failed")
-                    .$attr
-                    .get()
-                    .expect("Invalid missing data during lookup")
-                    .clone();
-                let x = $self.$attr.get_or_create(|| value);
-                Ok(x)
-            }
-        }
-    }
-}
-
-#[allow(unused)]
-impl IssueData {
-    pub(crate) fn new_empty(ident: String) -> Self {
-        Self::from_raw_data(ident, RawIssueData::default())
-    }
-
-    fn from_raw_data(ident: String, value: RawIssueData) -> Self {
-        Self {
-            ident,
-            key: initialize_lazy_field!(value.key),
-            summary: initialize_lazy_field!(value.summary),
-            description: initialize_lazy_field!(value.description),
-            comments: initialize_lazy_field!(
-                value.comments.map(|v| v.into_iter().map(|c| c.body).collect())
-            ),
-            status: initialize_lazy_field!(value.status.map(|x| x.name)),
-            resolution: initialize_lazy_field!(
-                value.resolution.map(|x| x.map(|y| y.name))
-            ),
-            priority: initialize_lazy_field!(value.priority.map(|x| x.name)),
-            issue_type: initialize_lazy_field!(value.issuetype.map(|x| x.name)),
-            issue_links: initialize_lazy_field!(Some(vec![])),
-            parent: initialize_lazy_field!(value.parent),
-            subtasks: initialize_lazy_field!(value.subtasks),
-            watches: initialize_lazy_field!(value.watches.map(|x| x.watch_count)),
-            votes: initialize_lazy_field!(value.votes.map(|x| x.votes)),
-            date_created: initialize_lazy_field!(value.created),
-            date_updated: initialize_lazy_field!(value.updated),
-            date_resolved: initialize_lazy_field!(value.resolutiondate),
-            labels: initialize_lazy_field!(value.labels),
-            components: initialize_lazy_field!(
-                value.components.map(|v| v.into_iter().map(|c| c.name).collect())
-            ),
-            affected_versions: initialize_lazy_field!(
-                value.versions.map(|v| v.into_iter().map(|c| c.name).collect())
-            ),
-            fix_versions: initialize_lazy_field!(
-                value.fix_versions.map(|v| v.into_iter().map(|c| c.name).collect())
-            )
-        }
-    }
-
-    pub(crate) fn update(&self, other: IssueData) {
-        maybe_copy_attribute!(self, other, key);
-        maybe_copy_attribute!(self, other, summary);
-        maybe_copy_attribute!(self, other, description);
-        maybe_copy_attribute!(self, other, comments);
-        maybe_copy_attribute!(self, other, parent);
-        maybe_copy_attribute!(self, other, subtasks);
-        maybe_copy_attribute!(self, other, issue_links);
-        maybe_copy_attribute!(self, other, status);
-        maybe_copy_attribute!(self, other, priority);
-        maybe_copy_attribute!(self, other, resolution);
-        maybe_copy_attribute!(self, other, issue_type);
-        maybe_copy_attribute!(self, other, watches);
-        maybe_copy_attribute!(self, other, votes);
-        maybe_copy_attribute!(self, other, date_created);
-        maybe_copy_attribute!(self, other, date_updated);
-        maybe_copy_attribute!(self, other, date_resolved);
-        maybe_copy_attribute!(self, other, labels);
-        maybe_copy_attribute!(self, other, components);
-        maybe_copy_attribute!(self, other, affected_versions);
-        maybe_copy_attribute!(self, other, fix_versions);
-    }
-
-    pub fn key(&self, api: &IssueAPI) -> APIResult<&String> {
-        load_lazy_attribute!(self, key, IssueAttribute::Key, api)
-    }
-
-    pub fn summary(&self, api: &IssueAPI) -> APIResult<&String> {
-        load_lazy_attribute!(self, summary, IssueAttribute::Summary, api)
-    }
-
-    pub fn description(&self, api: &IssueAPI) -> APIResult<&String> {
-        load_lazy_attribute!(self, description, IssueAttribute::Description, api)
-    }
-
-    pub fn comments(&self, api: &IssueAPI) -> APIResult<&Vec<String>> {
-        load_lazy_attribute!(self, comments, IssueAttribute::Comments, api)
-    }
-
-    pub fn parent(&self, api: &IssueAPI) -> APIResult<&Option<String>> {
-        load_lazy_attribute!(self, parent, IssueAttribute::Parent, api)
-    }
-
-    pub fn subtasks(&self, api: &IssueAPI) -> APIResult<&Vec<String>> {
-        load_lazy_attribute!(self, subtasks, IssueAttribute::Subtasks, api)
-    }
-
-    pub fn issue_links(&self, api: &IssueAPI) -> APIResult<&Vec<String>> {
-        load_lazy_attribute!(self, issue_links, IssueAttribute::IssueLinks, api)
-    }
-
-    pub fn status(&self, api: &IssueAPI) -> APIResult<&String> {
-        load_lazy_attribute!(self, status, IssueAttribute::Status, api)
-    }
-
-    pub fn priority(&self, api: &IssueAPI) -> APIResult<&String> {
-        load_lazy_attribute!(self, priority, IssueAttribute::Priority, api)
-    }
-
-    pub fn resolution(&self, api: &IssueAPI) -> APIResult<&Option<String>> {
-        load_lazy_attribute!(self, resolution, IssueAttribute::Resolution, api)
-    }
-
-    pub fn issue_type(&self, api: &IssueAPI) -> APIResult<&String> {
-        load_lazy_attribute!(self, issue_type, IssueAttribute::IssueType, api)
-    }
-
-    pub fn watches(&self, api: &IssueAPI) -> APIResult<u64> {
-        load_lazy_attribute!(self, watches, IssueAttribute::Watches, api).map(|x| *x)
-    }
-
-    pub fn votes(&self, api: &IssueAPI) -> APIResult<u64> {
-        load_lazy_attribute!(self, votes, IssueAttribute::Votes, api).map(|x| *x)
-    }
-
-    pub fn date_created(&self, api: &IssueAPI) -> APIResult<&String> {
-        load_lazy_attribute!(self, date_created, IssueAttribute::DateCreated, api)
-    }
-
-    pub fn date_updated(&self, api: &IssueAPI) -> APIResult<&String> {
-        load_lazy_attribute!(self, date_updated, IssueAttribute::DateUpdated, api)
-    }
-
-    pub fn date_resolved(&self, api: &IssueAPI) -> APIResult<&Option<String>> {
-        load_lazy_attribute!(self, date_resolved, IssueAttribute::DateResolved, api)
-    }
-
-    pub fn labels(&self, api: &IssueAPI) -> APIResult<&Vec<String>> {
-        load_lazy_attribute!(self, labels, IssueAttribute::Labels, api)
-    }
-
-    pub fn components(&self, api: &IssueAPI) -> APIResult<&Vec<String>> {
-        load_lazy_attribute!(self, components, IssueAttribute::Components, api)
-    }
-
-    pub fn affected_versions(&self, api: &IssueAPI) -> APIResult<&Vec<String>> {
-        load_lazy_attribute!(self, affected_versions, IssueAttribute::AffectedVersions, api)
-    }
-
-    pub fn fix_versions(&self, api: &IssueAPI) -> APIResult<&Vec<String>> {
-        load_lazy_attribute!(self, fix_versions, IssueAttribute::FixVersions, api)
-    }
-}
-
-
-//////////////////////////////////////////////////////////////////////////////////////////////////
-//////////////////////////////////////////////////////////////////////////////////////////////////
-// Blocking implementation
-//////////////////////////////////////////////////////////////////////////////////////////////////
-
-#[allow(unused)]
-#[cfg(feature = "blocking")]
-impl IssueAPI {
-    pub(crate) fn new(url: String, username: String, password: String) -> APIResult<Self> {
-        let mut read_only_api = Self::new_read_only(url);
-        read_only_api.login(username, password)?;
-        Ok(read_only_api)
-    }
-
-    pub(crate) fn new_read_only(url: String) -> Self {
-        IssueAPI{url, token: None, client: Client::new()}
-    }
-
-    fn login(&mut self, username: String, password: String) -> APIResult<()> {
-        #[derive(serde::Deserialize)]
-        struct TokenResponse {
-            access_token: String,
-            #[allow(dead_code)] token_type: String
-        }
-        let mut form = HashMap::new();
-        form.insert("username", username);
-        form.insert("password", password);
-        let token = self.client
-            .post(self.get_endpoint("token"))
-            .form(&form)
-            .send()?
-            .error_for_status()?
-            .json::<TokenResponse>()
-            .expect("Received invalid token payload from server")
-            .access_token;
-        self.token = Some(token);
-        Ok(())
-    }
-
-    /***************************************************************************
-     * Shared Networking Code
-     */
-
-    fn get_endpoint(&self, suffix: &str) -> String {
-        self.url.clone() + "/" + suffix
-    }
-
-    fn get_auth(&self) -> APIResult<String> {
-        if self.token.is_none() {
-            Err(Box::try_from(AuthenticationError {}).unwrap())
-        } else {
-            Ok("Bearer ".to_string() + self.token.clone().unwrap().as_str())
-        }
-    }
-
-    fn call_endpoint_json<I, O>(&self,
-                                suffix: &str,
-                                verb: Verb,
-                                payload: I) -> APIResult<O>
-    where
-        I: serde::Serialize,
-        O: for <'de> serde::Deserialize<'de>,
-    {
-        //println!("{}", serde_json::to_string_pretty(&payload).unwrap());
-        match verb {
-            Verb::Get => {
-                let result = self.client.get(self.get_endpoint(suffix))
-                    .json(&payload)
-                    .send()?
-                    .error_for_status()?
-                    .json::<O>()
-                    .expect("Received invalid response from server.");
-                Ok(result)
-            }
-            Verb::Post => {
-                let result: O = self.client.post(self.get_endpoint(suffix))
-                    .json(&payload)
-                    .header("Authorization", self.get_auth()?)
-                    .send()?
-                    .error_for_status()?
-                    .json::<O>()
-                    .expect("Received invalid response from server.");
-                Ok(result)
-            }
-            Verb::Patch => {
-                let result: O = self.client.patch(self.get_endpoint(suffix))
-                    .json(&payload)
-                    .header("Authorization", self.get_auth()?)
-                    .send()?
-                    .error_for_status()?
-                    .json::<O>()
-                    .expect("Received invalid response from server.");
-                Ok(result)
-            }
-            Verb::Delete => {
-                let result: O = self.client.delete(self.get_endpoint(suffix))
-                    .json(&payload)
-                    .header("Authorization", self.get_auth()?)
-                    .send()?
-                    .error_for_status()?
-                    .json::<O>()
-                    .expect("Received invalid response from server.");
-                Ok(result)
-            }
-        }
-    }
-
-    /***************************************************************************
-     * Issue-related endpoints
-     */
-
-    pub(crate) fn search(&self, query: Query) -> APIResult<Vec<String>> {
-        let mut map = Map::new();
-        map.insert("filter".to_string(), query.into_json());
-        #[derive(serde::Deserialize)]
-        struct SearchResponse {
-            issue_ids: Vec<String>
-        }
-        let result = self.call_endpoint_json::<_, SearchResponse>(
-            "issue-ids",
-            Verb::Get,
-            Value::Object(map)
-        )?;
-        Ok(result.issue_ids)
-    }
-
-    pub(crate) fn find_issue_id_by_key(&self, project: String, key: String) -> APIResult<String> {
-        #[derive(serde::Deserialize)]
-        struct IdResponse {
-            issue_id: String
-        }
-        let endpoint = format!("issue-ids/{}/{}", project, key);
-        let result = self.call_endpoint_json::<_, IdResponse>(
-            endpoint.as_str(),
-            Verb::Get,
-            Value::Object(Map::new())
-        )?;
-        Ok(result.issue_id)
-    }
-
-    pub(crate) fn find_issue_ids_by_keys(&self, ids: Vec<(String, String)>) -> APIResult<Vec<String>> {
-        #[derive(serde::Deserialize)]
-        struct IdsResponse {
-            issue_ids: HashMap<String, String>
-        }
-        let keys = ids.into_iter()
-            .map(|(project, key)| format!("{}-{}", project, key))
-            .collect::<Vec<_>>();
-        let mut map = Map::new();
-        map.insert(
-            "issue_keys".to_string(),
-            Value::Array(keys.iter().cloned().map(Value::String).collect())
-        );
-        let result = self.call_endpoint_json::<_, IdsResponse>(
-            "bulk/get-issue-ids-from-keys",
-            Verb::Get,
-            Value::Object(map)
-        )?;
-        let mut ids: Vec<String> = Vec::with_capacity(keys.len());
-        for key in keys {
-            match result.issue_ids.get(&key) {
-                None => {
-                    let msg = format!("No ID found for key \"{}\"", key);
-                    return Err(Box::new(APIError::new(msg)));
-                },
-                Some(id) => ids.push(id.clone())
-            }
-        }
-        Ok(ids)
-    }
-
-    pub(crate) fn get_issue_data(&self,
-                          issues: Vec<String>,
-                          attributes: Vec<IssueAttribute>) -> APIResult<HashMap<String, IssueData>> {
-        let mut map = Map::new();
-        map.insert(
-            "issue_ids".to_string(),
-            Value::Array(issues.into_iter().map(Value::String).collect())
-        );
-        map.insert(
-            "attributes".to_string(),
-            Value::Array(attributes.into_iter().map(|s| Value::String(s.to_string())).collect())
-        );
-        #[derive(Debug, serde::Deserialize)]
-        struct IssueDataResponse {
-            data: HashMap<String, RawIssueData>
-        }
-        let response = self.call_endpoint_json::<_, IssueDataResponse>(
-            "issue-data", Verb::Get, Value::Object(map)
-        )?.data;
-        let result = response
-            .into_iter()
-            .map(|(ident, data)| (
-                ident.clone(),
-                IssueData::from_raw_data(ident, data)
-            ))
-            .collect();
-        Ok(result)
-    }
-
-    /***************************************************************************
-     * Tag-related endpoints
-     */
-
-    pub(crate) fn get_all_tags(&self) -> APIResult<Vec<UnboundTag>> {
-        #[derive(Debug, serde::Deserialize)]
-        struct TagListResponse {
-            tags: Vec<UnboundTag>
-        }
-        let result = self.call_endpoint_json::<_, TagListResponse>(
-            "tags", Verb::Get, Value::Object(Map::new())
-        )?;
-        Ok(result.tags)
-    }
-
-    pub(crate) fn register_new_tag(&self, name: String, description: String) -> APIResult<()> {
-        let mut map = Map::new();
-        map.insert("tag".to_string(), Value::String(name));
-        map.insert("description".to_string(), Value::String(description));
-        self.call_endpoint_json("tags", Verb::Post, Value::Object(map))?;
-        Ok(())
-    }
-
-    pub(crate) fn get_tag_info(&self, tag: String) -> APIResult<UnboundTag> {
-        #[derive(Debug, serde::Deserialize)]
-        struct TagInfoResponse {
-            tag: UnboundTag
-        }
-        let endpoint = format!("tags/{}", tag);
-        let result = self.call_endpoint_json::<_, TagInfoResponse>(
-            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
-        )?;
-        Ok(result.tag)
-    }
-
-    pub(crate) fn update_tag(&self, tag: String, new_description: String) -> APIResult<()> {
-        let mut map = Map::new();
-        map.insert("description".to_string(), Value::String(new_description));
-        let endpoint = format!("tags/{}", tag);
-        self.call_endpoint_json(
-            endpoint.as_str(), Verb::Post, Value::Object(map)
-        )?;
-        Ok(())
-    }
-
-    pub(crate) fn delete_tag(&self, tag: String) -> APIResult<()> {
-        let endpoint = format!("tags/{}", tag);
-        self.call_endpoint_json(
-            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
-        )?;
-        Ok(())
-    }
-
-    /***************************************************************************
-     * Tag + Issue endpoints
-     */
-
-    pub(crate) fn start_issue_review(&self, issue_id: String) -> APIResult<()> {
-        let endpoint = format!("issues/{}/mark-review", issue_id);
-        self.call_endpoint_json(
-            endpoint.as_str(), Verb::Post, Value::Object(Map::new())
-        )?;
-        Ok(())
-    }
-
-    pub(crate) fn finish_issue_review(&self, issue_id: String) -> APIResult<()> {
-        let endpoint = format!("issues/{}/finish-review", issue_id);
-        self.call_endpoint_json(
-            endpoint.as_str(), Verb::Post, Value::Object(Map::new())
-        )?;
-        Ok(())
-    }
-
-    pub(crate) fn get_tags_for_issue(&self, issue_id: String) -> APIResult<Vec<String>> {
-        #[derive(Debug, serde::Deserialize)]
-        struct TagsResponse {
-            tags: Vec<String>
-        }
-        let endpoint = format!("issues/{}/tags", issue_id);
-        let result = self.call_endpoint_json::<_, TagsResponse>(
-            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
-        )?;
-        Ok(result.tags)
-    }
-
-    pub(crate) fn add_tag_to_issue(&self, issue_id: String, tag: String) -> APIResult<()> {
-        let endpoint = format!("issues/{}/tags", issue_id);
-        let mut map = Map::new();
-        map.insert("tag".to_string(), Value::String(tag));
-        self.call_endpoint_json(
-            endpoint.as_str(), Verb::Post, map
-        )?;
-        Ok(())
-    }
-
-    pub(crate) fn remove_tag_from_issue(&self, issue_id: String, tag: String) -> APIResult<()> {
-        let endpoint = format!("issues/{}/tags/{}", issue_id, tag);
-        self.call_endpoint_json(
-            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
-        )?;
-        Ok(())
-    }
-
-    pub(crate) fn bulk_add_tags(&self, issues_and_tags: HashMap<String, Vec<String>>) -> APIResult<()> {
-        let maps = issues_and_tags
-            .into_iter()
-            .map(|(key, value)| {
-                let mut map = Map::new();
-                map.insert("issue_id".to_string(), Value::String(key));
-                let tags = value.into_iter().map(Value::String).collect();
-                map.insert("tags".to_string(), Value::Array(tags));
-                Value::Object(map)
-            }).collect::<Vec<_>>();
-        let mut map = Map::new();
-        map.insert("data".to_string(), Value::Array(maps));
-        self.call_endpoint_json(
-            "/bulk/add-tags", Verb::Post, Value::Object(map)
-        )
-    }
-
-    /***************************************************************************
-     * Labeling endpoints
-     */
-
-    pub(crate) fn get_labeling_comments_for_issue(&self, issue_id: String) -> APIResult<Vec<UnboundComment>> {
-        #[derive(Debug, serde::Deserialize)]
-        struct RawComment {
-            author: String,
-            comment: String
-        }
-        #[derive(Debug, serde::Deserialize)]
-        struct CommentsResponse {
-            comments: HashMap<String, RawComment>
-        }
-        let endpoint = format!("manual-labels/{}/comments", issue_id);
-        let result = self.call_endpoint_json::<_, CommentsResponse>(
-            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
-        )?;
-        // collect converted comments
-        let converted: Vec<UnboundComment> = result.comments.into_iter()
-            .map(|(id, raw)| UnboundComment{id, author: raw.author, text: raw.comment})
-            .collect();
-        // Get object IDS in order to restore comment order
-        let mut object_ids: Vec<u128> = Vec::with_capacity(converted.len());
-        for c in converted.iter() {
-            let id = c.id
-                .parse::<u128>()
-                .map_err(|e| IDParsingError{msg: e.to_string()})?;
-            object_ids.push(id);
-        }
-        // Sort comments
-        let mut pairs = object_ids.into_iter()
-            .zip(converted.into_iter()).collect::<Vec<_>>();
-        pairs.sort_by_key(|p| p.0);
-        // Extract comments without ids
-        let (_, comments): (Vec<u128>, Vec<UnboundComment>) = pairs.into_iter().unzip();
-        Ok(comments)
-    }
-
-    pub(crate) fn add_labeling_comment_to_issue(&self, issue_id: String, text: String) -> APIResult<String> {
-        #[derive(Debug, serde::Deserialize)]
-        struct NewCommentResponse {
-            comment_id: String
-        }
-        let endpoint = format!("manual-labels/{}/comments", issue_id);
-        let mut map = Map::new();
-        map.insert("comment".to_string(), Value::String(text));
-        let result = self.call_endpoint_json::<_, NewCommentResponse>(
-            endpoint.as_str(), Verb::Post, Value::Object(map)
-        )?;
-        Ok(result.comment_id)
-    }
-
-    pub(crate) fn update_labeling_comment(&self,
-                                   issue_id: String,
-                                   comment_id: String,
-                                   new_text: String) -> APIResult<()> {
-        let endpoint = format!("manual-labels/{}/comments/{}", issue_id, comment_id);
-        let mut map = Map::new();
-        map.insert("comment".to_string(), Value::String(new_text));
-        self.call_endpoint_json(
-            endpoint.as_str(), Verb::Patch, Value::Object(map)
-        )?;
-        Ok(())
-    }
-
-    pub(crate) fn delete_labeling_comment(&self,
-                                   issue_id: String,
-                                   comment_id: String) -> APIResult<()> {
-        let endpoint = format!("manual-labels/{}/comments/{}", issue_id, comment_id);
-        self.call_endpoint_json(
-            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
-        )?;
-        Ok(())
-    }
-
-    pub(crate) fn get_manual_labels(&self, issues: Vec<String>) -> APIResult<HashMap<String, Label>> {
-        #[derive(Debug, serde::Deserialize)]
-        struct LabelsResponse {
-            manual_labels: HashMap<String, Label>
-        }
-        let mut map = Map::new();
-        map.insert("issue_ids".to_string(),
-                   Value::Array(issues.into_iter().map(Value::String).collect()));
-        let result = self.call_endpoint_json::<_, LabelsResponse>(
-            "manual-labels", Verb::Get, map
-        )?;
-        Ok(result.manual_labels)
-    }
-
-    pub(crate) fn update_manual_label_for_issue(&self, issue_id: String, label: Label) -> APIResult<()> {
-        let endpoint = format!("manual-labels/{}", issue_id);
-        self.call_endpoint_json(endpoint.as_str(), Verb::Post, label)?;
-        Ok(())
-    }
-
-    /***************************************************************************
-     * Embedding-related endpoints
-     */
-
-    pub(crate) fn get_all_embeddings(&self) -> APIResult<Vec<UnboundEmbedding>> {
-        #[derive(Debug, serde::Deserialize)]
-        struct EmbeddingsResponse {
-            embeddings: Vec<UnboundEmbedding>
-        }
-        let result = self.call_endpoint_json::<_, EmbeddingsResponse>(
-            "embeddings", Verb::Get, Value::Object(Map::new())
-        )?;
-        Ok(result.embeddings)
-    }
-
-    pub(crate) fn create_embedding(&self,
-                            name: String,
-                            config: HashMap<String, Value>) -> APIResult<String> {
-        let mut map = Map::new();
-        map.insert("name".to_string(), Value::String(name));
-        map.insert("config".to_string(),
-                   Value::Object(Map::from_iter(config.into_iter())));
-        let result = self.call_endpoint_json::<_, String>(
-            "embeddings", Verb::Post, Value::Object(map)
-        )?;
-        Ok(result)
-    }
-
-    pub(crate) fn get_embedding(&self, id: String) -> APIResult<UnboundEmbedding> {
-        let endpoint = format!("embeddings/{}", id);
-        self.call_endpoint_json::<_, UnboundEmbedding>(
-            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
-        )
-    }
-
-    pub(crate) fn update_embedding(&self,
-                            id: String,
-                            name: String,
-                            config: HashMap<String, Value>) -> APIResult<()> {
-        let mut map = Map::new();
-        map.insert("name".to_string(), Value::String(name));
-        map.insert("config".to_string(),
-                   Value::Object(Map::from_iter(config.into_iter())));
-        let endpoint = format!("embeddings/{}", id);
-        self.call_endpoint_json(endpoint.as_str(), Verb::Post, map)?;
-        Ok(())
-    }
-
-
-    pub(crate) fn delete_embedding(&self, id: String) -> APIResult<()> {
-        let endpoint = format!("embeddings/{}", id);
-        self.call_endpoint_json(
-            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
-        )?;
-        Ok(())
-    }
-
-    pub(crate) fn upload_embedding_binary(&self, id: String, filename: String) -> APIResult<()> {
-        let form = multipart::Form::new().file("file", filename)?;
-        let endpoint = format!("embeddings/{}/file", id);
-        self.client
-            .post(self.get_endpoint(endpoint.as_str()))
-            .multipart(form)
-            .header("Authorization", self.get_auth()?)
-            .send()?
-            .error_for_status()?;
-        Ok(())
-    }
-
-    pub(crate) fn download_embedding_binary(&self, id: String, filename: String) -> APIResult<()> {
-        let endpoint = format!("embeddings/{}/file", id);
-        let data = self.client
-            .get(self.get_endpoint(endpoint.as_str()))
-            .send()?
-            .error_for_status()?
-            .bytes()?;
-        let mut cursor = std::io::Cursor::new(data);
-        let mut file = std::fs::File::create(filename)?;
-        std::io::copy(&mut cursor, &mut file)?;
-        Ok(())
-    }
-
-    pub(crate) fn delete_embedding_binary(&self, id: String) -> APIResult<()> {
-        let endpoint = format!("embeddings/{}/file", id);
-        self.call_endpoint_json(
-            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
-        )?;
-        Ok(())
-    }
-
-    /***************************************************************************
-     * Repos and Project endpoints
-     */
-
-    pub(crate) fn get_all_repos(&self) -> APIResult<Vec<String>> {
-        #[derive(Debug, serde::Deserialize)]
-        struct ReposResponse {
-            repos: Vec<String>
-        }
-        let result = self.call_endpoint_json::<_, ReposResponse>(
-            "repos", Verb::Get, Value::Object(Map::new())
-        )?;
-        Ok(result.repos)
-    }
-
-    pub(crate) fn get_projects_for_repo(&self, repo: String) -> APIResult<Vec<String>> {
-        #[derive(Debug, serde::Deserialize)]
-        struct ProjectsResponse {
-            projects: Vec<String>
-        }
-        let endpoint = format!("repos/{}/projects", repo);
-        let result = self.call_endpoint_json::<_, ProjectsResponse>(
-            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
-        )?;
-        Ok(result.projects)
-    }
-
-    /***************************************************************************
-     * Model Config Endpoints
-     */
-
-    pub(crate) fn get_all_models(&self) -> APIResult<Vec<ModelInfo>> {
-        #[derive(Debug, serde::Deserialize)]
-        struct ModelsResponse {
-            models: Vec<ModelInfo>
-        }
-        let result = self.call_endpoint_json::<_, ModelsResponse>(
-            "models", Verb::Get, Value::Object(Map::new())
-        )?;
-        Ok(result.models)
-    }
-
-    pub(crate) fn create_model_config(&self,
-                                      name: String,
-                                      config: HashMap<String, Value>) -> APIResult<String> {
-        #[derive(Debug, serde::Deserialize)]
-        struct NewModelResponse {
-            model_id: String
-        }
-        let mut map = Map::new();
-        map.insert("model_name".to_string(), Value::String(name));
-        map.insert(
-            "model_config".to_string(),
-            Value::Object(Map::from_iter(config.into_iter()))
-        );
-        let result = self.call_endpoint_json::<_, NewModelResponse>(
-            "models", Verb::Post, Value::Object(map)
-        )?;
-        Ok(result.model_id)
-    }
-
-    pub(crate) fn get_model_config(&self, id: String) -> APIResult<UnboundModelConfig> {
-        let endpoint = format!("models/{}", id);
-        self.call_endpoint_json::<_, UnboundModelConfig>(
-            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
-        )
-    }
-
-    pub(crate) fn update_model_config(&self,
-                                      id: String,
-                                      name: String,
-                                      config: HashMap<String, Value>) -> APIResult<()> {
-        let endpoint = format!("models/{}", id);
-        let mut map = Map::new();
-        map.insert("model_name".to_string(), Value::String(name));
-        map.insert("model_config".to_string(),
-                   Value::Object(Map::from_iter(config.into_iter())));
-        self.call_endpoint_json(endpoint.as_str(), Verb::Post, Value::Object(map))
-    }
-
-    pub(crate) fn delete_model_config(&self, id: String) -> APIResult<()> {
-        let endpoint = format!("models/{}", id);
-        self.call_endpoint_json(
-            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
-        )
-    }
-
-    /***************************************************************************
-     * Model Versions
-     */
-
-    pub(crate) fn get_versions_for_model(&self,
-                                         model_id: String) -> APIResult<Vec<UnboundModelVersion>> {
-        let endpoint = format!("models/{}/versions", model_id.as_str());
-        #[derive(Debug, serde::Deserialize)]
-        struct RawVersionInfo {
-            version_id: String,
-            time: String
-        }
-        #[derive(Debug, serde::Deserialize)]
-        struct VersionsResponse {
-            versions: Vec<RawVersionInfo>
-        }
-        let result = self.call_endpoint_json::<_, VersionsResponse>(
-            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
-        )?;
-        let converted = result.versions
-            .into_iter()
-            .map(|v|
-                UnboundModelVersion{
-                    model_id: model_id.clone(),
-                    version_id: v.version_id,
-                    time: v.time
-                }
-            )
-            .collect();
-        Ok(converted)
-    }
-
-    pub(crate) fn upload_model_version(&self,
-                                       model_id: String,
-                                       time: String,
-                                       file: String) -> APIResult<String> {
-        #[derive(Debug, serde::Deserialize)]
-        struct NewVersionResponse {
-            version_id: String
-        }
-        let form = multipart::Form::new()
-            .file("file", file)?
-            .text("time", time);
-        let endpoint = format!("models/{}/versions", model_id);
-        let result = self.client
-            .post(self.get_endpoint(endpoint.as_str()))
-            .multipart(form)
-            .header("Authorization", self.get_auth()?)
-            .send()?
-            .error_for_status()?
-            .json::<NewVersionResponse>()
-            .expect("Received invalid response from server");
-        Ok(result.version_id)
-    }
-
-    pub(crate) fn download_model_version(&self,
-                                         model_id: String,
-                                         version_id: String,
-                                         file: String) -> APIResult<()> {
-        let endpoint = format!("models/{}/versions/{}", model_id, version_id);
-        let data = self.client
-            .get(self.get_endpoint(endpoint.as_str()))
-            .send()?
-            .error_for_status()?
-            .bytes()?;
-        let mut cursor = std::io::Cursor::new(data);
-        let mut file = std::fs::File::create(file)?;
-        std::io::copy(&mut cursor, &mut file)?;
-        Ok(())
-    }
-
-    pub(crate) fn delete_model_version(&self,
-                                       model_id: String,
-                                       version_id: String) -> APIResult<()> {
-        let endpoint = format!("models/{}/versions/{}", model_id, version_id);
-        self.call_endpoint_json(
-            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
-        )
-    }
-
-    /***************************************************************************
-    * Model Predictions
-    */
-
-    pub(crate) fn get_predictions(&self,
-                                  model_id: String,
-                                  version_id: String,
-                                  issues: Option<Vec<String>>) -> APIResult<HashMap<String, Value>> {
-        let endpoint = format!("models/{}/versions/{}/predictions", model_id, version_id);
-        let mut map = Map::new();
-        let payload = match issues {
-            None => Value::Null,
-            Some(ids) => Value::Array(ids.into_iter().map(Value::String).collect())
-        };
-        map.insert("issue_ids".to_string(), payload);
-        #[derive(Debug, serde::Deserialize)]
-        struct PredictionsResponse {
-            predictions: HashMap<String, Value>
-        }
-        let result = self.call_endpoint_json::<_, PredictionsResponse>(
-            endpoint.as_str(), Verb::Get, Value::Object(map)
-        )?;
-        Ok(result.predictions)
-    }
-
-    pub(crate) fn store_predictions(&self,
-                                    model_id: String,
-                                    version_id: String,
-                                    predictions: HashMap<String, Value>) -> APIResult<()> {
-        let endpoint = format!("models/{}/versions/{}/predictions", model_id, version_id);
-        let mut map = Map::new();
-        map.insert("predictions".to_string(),
-                   Value::Object(Map::from_iter(predictions.into_iter())));
-        self.call_endpoint_json(endpoint.as_str(), Verb::Post, Value::Object(map))
-    }
-
-    pub(crate) fn delete_predictions(&self,
-                                     model_id: String,
-                                     version_id: String) -> APIResult<()> {
-        let endpoint = format!("models/{}/versions/{}/predictions", model_id, version_id);
-        self.call_endpoint_json(
-            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
-        )
-    }
-
-    /***************************************************************************
-     * Model Performance
-     */
-
-    pub(crate) fn get_performances_for_model(&self, model_id: String) -> APIResult<Vec<UnboundTestRun>> {
-        #[derive(Debug, serde::Deserialize)]
-        struct PerformancesResponse {
-            performances: Vec<String>
-        }
-        let endpoint = format!("models/{}/performances", model_id.as_str());
-        let result = self.call_endpoint_json::<_, PerformancesResponse>(
-            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
-        )?;
-        let converted = result.performances
-            .into_iter()
-            .map(|r| UnboundTestRun{model_id: model_id.clone(), performance_id: r})
-            .collect();
-        Ok(converted)
-    }
-
-    pub(crate) fn store_model_performance(&self,
-                                          model_id: String,
-                                          data: Vec<Value>) -> APIResult<String> {
-        #[derive(Debug, serde::Deserialize)]
-        struct NewPerformanceResponse {
-            performance_id: String
-        }
-        let mut map = Map::new();
-        map.insert("performance".to_string(), Value::Array(data));
-        let endpoint = format!("models/{}/performances", model_id);
-        let result = self.call_endpoint_json::<_, NewPerformanceResponse>(
-            endpoint.as_str(), Verb::Post, Value::Object(map)
-        )?;
-        Ok(result.performance_id)
-    }
-
-    pub(crate) fn get_performance_data(&self,
-                                       model_id: String,
-                                       performance_id: String) -> APIResult<Vec<Value>> {
-        #[derive(Debug, serde::Deserialize)]
-        struct PerformanceDataResponse {
-            performance_id: String,
-            performance: Vec<Value>
-        }
-        let endpoint = format!("models/{}/performances/{}", model_id, performance_id);
-        let result = self.call_endpoint_json::<_, PerformanceDataResponse>(
-            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
-        )?;
-        Ok(result.performance)
-    }
-
-    pub(crate) fn delete_performance_data(&self,
-                                          model_id: String,
-                                          performance_id: String) -> APIResult<()> {
-        let endpoint = format!("models/{}/performances/{}", model_id, performance_id);
-        self.call_endpoint_json(
-            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
-        )
-    }
-}
+use std::collections::HashMap;
+
+#[cfg(feature = "blocking")]
+use reqwest::blocking::Client;
+use reqwest::blocking::{ClientBuilder, multipart};
+
+use serde_json::{Map, Value};
+use lazy_init::Lazy;
+
+use crate::comments::UnboundComment;
+use crate::config::IssueAttribute;
+use crate::embedding::UnboundEmbedding;
+use crate::schemas::raw_issue_response::RawIssueData;
+use crate::query::Query;
+use crate::labels::Label;
+use crate::tags::UnboundTag;
+use crate::util::initialize_lazy_field;
+use crate::util::APIResult;
+use crate::errors::*;
+use crate::models::{ModelInfo, UnboundModelConfig, UnboundModelVersion, UnboundTestRun};
+
+//////////////////////////////////////////////////////////////////////////////////////////////////
+//////////////////////////////////////////////////////////////////////////////////////////////////
+// Core Structs
+//////////////////////////////////////////////////////////////////////////////////////////////////
+
+/// The IssueAPI struct provides a low-level wrapper around the issues API.
+/// This struct provides basics means of session management,
+/// and exposes all available endpoints through Rust functions.
+#[allow(unused)]
+#[derive(Debug, Clone)]
+pub struct IssueAPI {
+    url: String,
+    token: Option<String>,
+    client: Client
+}
+
+#[allow(unused)]
+#[derive(Debug, Clone)]
+pub struct IssueData {
+    ident: String,
+    key: Lazy<String>,
+    summary: Lazy<String>,
+    description: Lazy<String>,
+    comments: Lazy<Vec<String>>,
+    status: Lazy<String>,
+    priority: Lazy<String>,
+    resolution: Lazy<Option<String>>,
+    issue_type: Lazy<String>,
+    issue_links: Lazy<Vec<String>>,
+    parent: Lazy<Option<String>>,
+    subtasks: Lazy<Vec<String>>,
+    watches: Lazy<u64>,
+    votes: Lazy<u64>,
+    date_created: Lazy<String>,
+    date_updated: Lazy<String>,
+    date_resolved: Lazy<Option<String>>,
+    labels: Lazy<Vec<String>>,
+    components: Lazy<Vec<String>>,
+    affected_versions: Lazy<Vec<String>>,
+    fix_versions: Lazy<Vec<String>>
+}
+
+//////////////////////////////////////////////////////////////////////////////////////////////////
+//////////////////////////////////////////////////////////////////////////////////////////////////
+// Auxiliary structs and enums
+//////////////////////////////////////////////////////////////////////////////////////////////////
+
+#[allow(unused)]
+enum Verb {
+    Get,
+    Post,
+    Patch,
+    Put,
+    Delete
+}
+
+macro_rules! maybe_copy_attribute {
+    ($self:ident, $other:ident, $attr:ident) => {
+        {
+            if let Some(x) = $other.$attr.get() {
+                $self.$attr.get_or_create(|| x.clone());
+            }
+        }
+    }
+}
+
+macro_rules! load_lazy_attribute {
+    ($self:ident, $attr:ident, $e:expr, $api:expr) => {
+        {
+            if let Some(x) = $self.$attr.get() {
+                Ok(x)
+            } else {
+                let value = $api.get_issue_data(vec![$self.ident.clone()], vec![$e])?
+                    .get(&$self.ident)
+                    .expect("Issue data lookup failed")
+                    .$attr
+                    .get()
+                    .expect("Invalid missing data during lookup")
+                    .clone();
+                let x = $self.$attr.get_or_create(|| value);
+                Ok(x)
+            }
+        }
+    }
+}
+
+#[allow(unused)]
+impl IssueData {
+    pub(crate) fn new_empty(ident: String) -> Self {
+        Self::from_raw_data(ident, RawIssueData::default())
+    }
+
+    fn from_raw_data(ident: String, value: RawIssueData) -> Self {
+        Self {
+            ident,
+            key: initialize_lazy_field!(value.key),
+            summary: initialize_lazy_field!(value.summary),
+            description: initialize_lazy_field!(value.description),
+            comments: initialize_lazy_field!(
+                value.comments.map(|v| v.into_iter().map(|c| c.body).collect())
+            ),
+            status: initialize_lazy_field!(value.status.map(|x| x.name)),
+            resolution: initialize_lazy_field!(
+                value.resolution.map(|x| x.map(|y| y.name))
+            ),
+            priority: initialize_lazy_field!(value.priority.map(|x| x.name)),
+            issue_type: initialize_lazy_field!(value.issuetype.map(|x| x.name)),
+            issue_links: initialize_lazy_field!(Some(vec![])),
+            parent: initialize_lazy_field!(value.parent),
+            subtasks: initialize_lazy_field!(value.subtasks),
+            watches: initialize_lazy_field!(value.watches.map(|x| x.watch_count)),
+            votes: initialize_lazy_field!(value.votes.map(|x| x.votes)),
+            date_created: initialize_lazy_field!(value.created),
+            date_updated: initialize_lazy_field!(value.updated),
+            date_resolved: initialize_lazy_field!(value.resolutiondate),
+            labels: initialize_lazy_field!(value.labels),
+            components: initialize_lazy_field!(
+                value.components.map(|v| v.into_iter().map(|c| c.name).collect())
+            ),
+            affected_versions: initialize_lazy_field!(
+                value.versions.map(|v| v.into_iter().map(|c| c.name).collect())
+            ),
+            fix_versions: initialize_lazy_field!(
+                value.fix_versions.map(|v| v.into_iter().map(|c| c.name).collect())
+            )
+        }
+    }
+
+    pub(crate) fn update(&self, other: IssueData) {
+        maybe_copy_attribute!(self, other, key);
+        maybe_copy_attribute!(self, other, summary);
+        maybe_copy_attribute!(self, other, description);
+        maybe_copy_attribute!(self, other, comments);
+        maybe_copy_attribute!(self, other, parent);
+        maybe_copy_attribute!(self, other, subtasks);
+        maybe_copy_attribute!(self, other, issue_links);
+        maybe_copy_attribute!(self, other, status);
+        maybe_copy_attribute!(self, other, priority);
+        maybe_copy_attribute!(self, other, resolution);
+        maybe_copy_attribute!(self, other, issue_type);
+        maybe_copy_attribute!(self, other, watches);
+        maybe_copy_attribute!(self, other, votes);
+        maybe_copy_attribute!(self, other, date_created);
+        maybe_copy_attribute!(self, other, date_updated);
+        maybe_copy_attribute!(self, other, date_resolved);
+        maybe_copy_attribute!(self, other, labels);
+        maybe_copy_attribute!(self, other, components);
+        maybe_copy_attribute!(self, other, affected_versions);
+        maybe_copy_attribute!(self, other, fix_versions);
+    }
+
+    pub fn key(&self, api: &IssueAPI) -> APIResult<&String> {
+        load_lazy_attribute!(self, key, IssueAttribute::Key, api)
+    }
+
+    pub fn summary(&self, api: &IssueAPI) -> APIResult<&String> {
+        load_lazy_attribute!(self, summary, IssueAttribute::Summary, api)
+    }
+
+    pub fn description(&self, api: &IssueAPI) -> APIResult<&String> {
+        load_lazy_attribute!(self, description, IssueAttribute::Description, api)
+    }
+
+    pub fn comments(&self, api: &IssueAPI) -> APIResult<&Vec<String>> {
+        load_lazy_attribute!(self, comments, IssueAttribute::Comments, api)
+    }
+
+    pub fn parent(&self, api: &IssueAPI) -> APIResult<&Option<String>> {
+        load_lazy_attribute!(self, parent, IssueAttribute::Parent, api)
+    }
+
+    pub fn subtasks(&self, api: &IssueAPI) -> APIResult<&Vec<String>> {
+        load_lazy_attribute!(self, subtasks, IssueAttribute::Subtasks, api)
+    }
+
+    pub fn issue_links(&self, api: &IssueAPI) -> APIResult<&Vec<String>> {
+        load_lazy_attribute!(self, issue_links, IssueAttribute::IssueLinks, api)
+    }
+
+    pub fn status(&self, api: &IssueAPI) -> APIResult<&String> {
+        load_lazy_attribute!(self, status, IssueAttribute::Status, api)
+    }
+
+    pub fn priority(&self, api: &IssueAPI) -> APIResult<&String> {
+        load_lazy_attribute!(self, priority, IssueAttribute::Priority, api)
+    }
+
+    pub fn resolution(&self, api: &IssueAPI) -> APIResult<&Option<String>> {
+        load_lazy_attribute!(self, resolution, IssueAttribute::Resolution, api)
+    }
+
+    pub fn issue_type(&self, api: &IssueAPI) -> APIResult<&String> {
+        load_lazy_attribute!(self, issue_type, IssueAttribute::IssueType, api)
+    }
+
+    pub fn watches(&self, api: &IssueAPI) -> APIResult<u64> {
+        load_lazy_attribute!(self, watches, IssueAttribute::Watches, api).map(|x| *x)
+    }
+
+    pub fn votes(&self, api: &IssueAPI) -> APIResult<u64> {
+        load_lazy_attribute!(self, votes, IssueAttribute::Votes, api).map(|x| *x)
+    }
+
+    pub fn date_created(&self, api: &IssueAPI) -> APIResult<&String> {
+        load_lazy_attribute!(self, date_created, IssueAttribute::DateCreated, api)
+    }
+
+    pub fn date_updated(&self, api: &IssueAPI) -> APIResult<&String> {
+        load_lazy_attribute!(self, date_updated, IssueAttribute::DateUpdated, api)
+    }
+
+    pub fn date_resolved(&self, api: &IssueAPI) -> APIResult<&Option<String>> {
+        load_lazy_attribute!(self, date_resolved, IssueAttribute::DateResolved, api)
+    }
+
+    pub fn labels(&self, api: &IssueAPI) -> APIResult<&Vec<String>> {
+        load_lazy_attribute!(self, labels, IssueAttribute::Labels, api)
+    }
+
+    pub fn components(&self, api: &IssueAPI) -> APIResult<&Vec<String>> {
+        load_lazy_attribute!(self, components, IssueAttribute::Components, api)
+    }
+
+    pub fn affected_versions(&self, api: &IssueAPI) -> APIResult<&Vec<String>> {
+        load_lazy_attribute!(self, affected_versions, IssueAttribute::AffectedVersions, api)
+    }
+
+    pub fn fix_versions(&self, api: &IssueAPI) -> APIResult<&Vec<String>> {
+        load_lazy_attribute!(self, fix_versions, IssueAttribute::FixVersions, api)
+    }
+}
+
+
+//////////////////////////////////////////////////////////////////////////////////////////////////
+//////////////////////////////////////////////////////////////////////////////////////////////////
+// Blocking implementation
+//////////////////////////////////////////////////////////////////////////////////////////////////
+
+#[allow(unused)]
+#[cfg(feature = "blocking")]
+impl IssueAPI {
+    pub(crate) fn new(url: String,
+                      username: String,
+                      password: String,
+                      allow_self_signed: bool) -> APIResult<Self> {
+        let mut read_only_api = Self::new_read_only(url, allow_self_signed)?;
+        read_only_api.login(username, password)?;
+        Ok(read_only_api)
+    }
+
+    pub(crate) fn new_read_only(url: String, allow_self_signed: bool) -> APIResult<Self> {
+        let client = ClientBuilder::new()
+            .danger_accept_invalid_certs(allow_self_signed)
+            .build()?;
+        Ok(IssueAPI{url, token: None, client})
+    }
+
+    fn login(&mut self, username: String, password: String) -> APIResult<()> {
+        #[derive(serde::Deserialize)]
+        struct TokenResponse {
+            access_token: String,
+            #[allow(dead_code)] token_type: String
+        }
+        let mut form = HashMap::new();
+        form.insert("username", username);
+        form.insert("password", password);
+        let token = self.client
+            .post(self.get_endpoint("token"))
+            .form(&form)
+            .send()?
+            .error_for_status()?
+            .json::<TokenResponse>()
+            .expect("Received invalid token payload from server")
+            .access_token;
+        self.token = Some(token);
+        Ok(())
+    }
+
+    /***************************************************************************
+     * Shared Networking Code
+     */
+
+    fn get_endpoint(&self, suffix: &str) -> String {
+        self.url.clone() + "/" + suffix
+    }
+
+    fn get_auth(&self) -> APIResult<String> {
+        if self.token.is_none() {
+            Err(Box::try_from(AuthenticationError {}).unwrap())
+        } else {
+            Ok(self.token.clone().unwrap())
+        }
+    }
+
+    fn build_request_base(&self, suffix: &str, verb: Verb) -> APIResult<reqwest::blocking::RequestBuilder> {
+        let url = self.get_endpoint(suffix);
+        let request_base = match verb {
+            Verb::Get => self.client.get(url),
+            Verb::Post => self.client.post(url).bearer_auth(self.get_auth()?),
+            Verb::Patch => self.client.patch(url).bearer_auth(self.get_auth()?),
+            Verb::Put => self.client.put(url).bearer_auth(self.get_auth()?),
+            Verb::Delete => self.client.delete(url).bearer_auth(self.get_auth()?)
+        };
+        Ok(request_base)
+    }
+
+    fn handle_error_status(&self,
+                           response: reqwest::blocking::Response) -> APIResult<reqwest::blocking::Response> {
+        Ok(response.error_for_status()?)
+    }
+
+    fn unpack_response<O>(&self, response: reqwest::blocking::Response) -> APIResult<O>
+    where
+        O: for <'de> serde::Deserialize<'de>
+    {
+        let result = self.handle_error_status(response)?
+            .json::<O>()
+            .expect("Received invalid response from server.");
+        Ok(result)
+    }
+
+    fn call_endpoint_json<I, O>(&self,
+                                suffix: &str,
+                                verb: Verb,
+                                payload: I) -> APIResult<O>
+    where
+        I: serde::Serialize,
+        O: for <'de> serde::Deserialize<'de>,
+    {
+        let response = self.build_request_base(suffix, verb)?.json(&payload).send()?;
+        let result = self.unpack_response(response)?;
+        Ok(result)
+    }
+
+    fn call_endpoint_form<I, O>(&self,
+                                suffix: &str,
+                                verb: Verb,
+                                payload: &I) -> APIResult<O>
+        where
+            I: serde::Serialize + ?Sized,
+            O: for <'de> serde::Deserialize<'de>,
+    {
+        let response = self.build_request_base(suffix, verb)?.form(payload).send()?;
+        let result = self.unpack_response(response)?;
+        Ok(result)
+    }
+
+    fn call_endpoint_multipart<O>(&self,
+                                  suffix: &str,
+                                  verb: Verb,
+                                  payload: multipart::Form) -> APIResult<O>
+        where
+            O: for <'de> serde::Deserialize<'de>,
+    {
+        let response = self.build_request_base(suffix, verb)?.multipart(payload).send()?;
+        let result = self.unpack_response(response)?;
+        Ok(result)
+    }
+
+    fn call_endpoint_download<I>(&self,
+                                 suffix: &str,
+                                 verb: Verb,
+                                 payload: I,
+                                 target_path: String) -> APIResult<()>
+        where
+            I: serde::Serialize,
+    {
+        let response = self.build_request_base(suffix, verb)?.json(&payload).send()?;
+        let data = self.handle_error_status(response)?.bytes()?;
+        let mut cursor = std::io::Cursor::new(data);
+        let mut file = std::fs::File::create(target_path)?;
+        std::io::copy(&mut cursor, &mut file)?;
+        Ok(())
+    }
+
+    /***************************************************************************
+     * Issue-related endpoints
+     */
+
+    pub(crate) fn search(&self, query: Query) -> APIResult<Vec<String>> {
+        let mut map = Map::new();
+        map.insert("filter".to_string(), query.into_json());
+        #[derive(serde::Deserialize)]
+        struct SearchResponse {
+            issue_ids: Vec<String>
+        }
+        let result = self.call_endpoint_json::<_, SearchResponse>(
+            "issue-ids",
+            Verb::Get,
+            Value::Object(map)
+        )?;
+        Ok(result.issue_ids)
+    }
+
+    pub(crate) fn find_issue_id_by_key(&self, project: String, key: String) -> APIResult<String> {
+        #[derive(serde::Deserialize)]
+        struct IdResponse {
+            issue_id: String
+        }
+        let endpoint = format!("issue-ids/{}/{}", project, key);
+        let result = self.call_endpoint_json::<_, IdResponse>(
+            endpoint.as_str(),
+            Verb::Get,
+            Value::Object(Map::new())
+        )?;
+        Ok(result.issue_id)
+    }
+
+    pub(crate) fn find_issue_ids_by_keys(&self, ids: Vec<(String, String)>) -> APIResult<Vec<String>> {
+        #[derive(serde::Deserialize)]
+        struct IdsResponse {
+            issue_ids: HashMap<String, String>
+        }
+        let keys = ids.into_iter()
+            .map(|(project, key)| format!("{}-{}", project, key))
+            .collect::<Vec<_>>();
+        let mut map = Map::new();
+        map.insert(
+            "issue_keys".to_string(),
+            Value::Array(keys.iter().cloned().map(Value::String).collect())
+        );
+        let result = self.call_endpoint_json::<_, IdsResponse>(
+            "bulk/get-issue-ids-from-keys",
+            Verb::Get,
+            Value::Object(map)
+        )?;
+        let mut ids: Vec<String> = Vec::with_capacity(keys.len());
+        for key in keys {
+            match result.issue_ids.get(&key) {
+                None => {
+                    let msg = format!("No ID found for key \"{}\"", key);
+                    return Err(Box::new(APIError::new(msg)));
+                },
+                Some(id) => ids.push(id.clone())
+            }
+        }
+        Ok(ids)
+    }
+
+    pub(crate) fn get_issue_data(&self,
+                          issues: Vec<String>,
+                          attributes: Vec<IssueAttribute>) -> APIResult<HashMap<String, IssueData>> {
+        let mut map = Map::new();
+        map.insert(
+            "issue_ids".to_string(),
+            Value::Array(issues.into_iter().map(Value::String).collect())
+        );
+        map.insert(
+            "attributes".to_string(),
+            Value::Array(attributes.into_iter().map(|s| Value::String(s.to_string())).collect())
+        );
+        #[derive(Debug, serde::Deserialize)]
+        struct IssueDataResponse {
+            data: HashMap<String, RawIssueData>
+        }
+        let response = self.call_endpoint_json::<_, IssueDataResponse>(
+            "issue-data", Verb::Get, Value::Object(map)
+        )?.data;
+        let result = response
+            .into_iter()
+            .map(|(ident, data)| (
+                ident.clone(),
+                IssueData::from_raw_data(ident, data)
+            ))
+            .collect();
+        Ok(result)
+    }
+
+    /***************************************************************************
+     * Tag-related endpoints
+     */
+
+    pub(crate) fn get_all_tags(&self) -> APIResult<Vec<UnboundTag>> {
+        #[derive(Debug, serde::Deserialize)]
+        struct TagListResponse {
+            tags: Vec<UnboundTag>
+        }
+        let result = self.call_endpoint_json::<_, TagListResponse>(
+            "tags", Verb::Get, Value::Object(Map::new())
+        )?;
+        Ok(result.tags)
+    }
+
+    pub(crate) fn register_new_tag(&self, name: String, description: String) -> APIResult<()> {
+        let mut map = Map::new();
+        map.insert("tag".to_string(), Value::String(name));
+        map.insert("description".to_string(), Value::String(description));
+        self.call_endpoint_json("tags", Verb::Post, Value::Object(map))?;
+        Ok(())
+    }
+
+    pub(crate) fn get_tag_info(&self, tag: String) -> APIResult<UnboundTag> {
+        #[derive(Debug, serde::Deserialize)]
+        struct TagInfoResponse {
+            tag: UnboundTag
+        }
+        let endpoint = format!("tags/{}", tag);
+        let result = self.call_endpoint_json::<_, TagInfoResponse>(
+            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
+        )?;
+        Ok(result.tag)
+    }
+
+    pub(crate) fn update_tag(&self, tag: String, new_description: String) -> APIResult<()> {
+        let mut map = Map::new();
+        map.insert("description".to_string(), Value::String(new_description));
+        let endpoint = format!("tags/{}", tag);
+        self.call_endpoint_json(
+            endpoint.as_str(), Verb::Post, Value::Object(map)
+        )?;
+        Ok(())
+    }
+
+    pub(crate) fn delete_tag(&self, tag: String) -> APIResult<()> {
+        let endpoint = format!("tags/{}", tag);
+        self.call_endpoint_json(
+            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
+        )?;
+        Ok(())
+    }
+
+    /***************************************************************************
+     * Tag + Issue endpoints
+     */
+
+    pub(crate) fn start_issue_review(&self, issue_id: String) -> APIResult<()> {
+        let endpoint = format!("issues/{}/mark-review", issue_id);
+        self.call_endpoint_json(
+            endpoint.as_str(), Verb::Post, Value::Object(Map::new())
+        )?;
+        Ok(())
+    }
+
+    pub(crate) fn finish_issue_review(&self, issue_id: String) -> APIResult<()> {
+        let endpoint = format!("issues/{}/finish-review", issue_id);
+        self.call_endpoint_json(
+            endpoint.as_str(), Verb::Post, Value::Object(Map::new())
+        )?;
+        Ok(())
+    }
+
+    pub(crate) fn get_tags_for_issue(&self, issue_id: String) -> APIResult<Vec<String>> {
+        #[derive(Debug, serde::Deserialize)]
+        struct TagsResponse {
+            tags: Vec<String>
+        }
+        let endpoint = format!("issues/{}/tags", issue_id);
+        let result = self.call_endpoint_json::<_, TagsResponse>(
+            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
+        )?;
+        Ok(result.tags)
+    }
+
+    pub(crate) fn add_tag_to_issue(&self, issue_id: String, tag: String) -> APIResult<()> {
+        let endpoint = format!("issues/{}/tags", issue_id);
+        let mut map = Map::new();
+        map.insert("tag".to_string(), Value::String(tag));
+        self.call_endpoint_json(
+            endpoint.as_str(), Verb::Post, map
+        )?;
+        Ok(())
+    }
+
+    pub(crate) fn remove_tag_from_issue(&self, issue_id: String, tag: String) -> APIResult<()> {
+        let endpoint = format!("issues/{}/tags/{}", issue_id, tag);
+        self.call_endpoint_json(
+            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
+        )?;
+        Ok(())
+    }
+
+    pub(crate) fn bulk_add_tags(&self, issues_and_tags: HashMap<String, Vec<String>>) -> APIResult<()> {
+        let maps = issues_and_tags
+            .into_iter()
+            .map(|(key, value)| {
+                let mut map = Map::new();
+                map.insert("issue_id".to_string(), Value::String(key));
+                let tags = value.into_iter().map(Value::String).collect();
+                map.insert("tags".to_string(), Value::Array(tags));
+                Value::Object(map)
+            }).collect::<Vec<_>>();
+        let mut map = Map::new();
+        map.insert("data".to_string(), Value::Array(maps));
+        self.call_endpoint_json(
+            "/bulk/add-tags", Verb::Post, Value::Object(map)
+        )
+    }
+
+    /***************************************************************************
+     * Labeling endpoints
+     */
+
+    pub(crate) fn get_labeling_comments_for_issue(&self, issue_id: String) -> APIResult<Vec<UnboundComment>> {
+        #[derive(Debug, serde::Deserialize)]
+        struct RawComment {
+            author: String,
+            comment: String
+        }
+        #[derive(Debug, serde::Deserialize)]
+        struct CommentsResponse {
+            comments: HashMap<String, RawComment>
+        }
+        let endpoint = format!("manual-labels/{}/comments", issue_id);
+        let result = self.call_endpoint_json::<_, CommentsResponse>(
+            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
+        )?;
+        // collect converted comments
+        let converted: Vec<UnboundComment> = result.comments.into_iter()
+            .map(|(id, raw)| UnboundComment{id, author: raw.author, text: raw.comment})
+            .collect();
+        // Get object IDS in order to restore comment order
+        let mut object_ids: Vec<u128> = Vec::with_capacity(converted.len());
+        for c in converted.iter() {
+            let id = c.id
+                .parse::<u128>()
+                .map_err(|e| IDParsingError{msg: e.to_string()})?;
+            object_ids.push(id);
+        }
+        // Sort comments
+        let mut pairs = object_ids.into_iter()
+            .zip(converted.into_iter()).collect::<Vec<_>>();
+        pairs.sort_by_key(|p| p.0);
+        // Extract comments without ids
+        let (_, comments): (Vec<u128>, Vec<UnboundComment>) = pairs.into_iter().unzip();
+        Ok(comments)
+    }
+
+    pub(crate) fn add_labeling_comment_to_issue(&self, issue_id: String, text: String) -> APIResult<String> {
+        #[derive(Debug, serde::Deserialize)]
+        struct NewCommentResponse {
+            comment_id: String
+        }
+        let endpoint = format!("manual-labels/{}/comments", issue_id);
+        let mut map = Map::new();
+        map.insert("comment".to_string(), Value::String(text));
+        let result = self.call_endpoint_json::<_, NewCommentResponse>(
+            endpoint.as_str(), Verb::Post, Value::Object(map)
+        )?;
+        Ok(result.comment_id)
+    }
+
+    pub(crate) fn update_labeling_comment(&self,
+                                   issue_id: String,
+                                   comment_id: String,
+                                   new_text: String) -> APIResult<()> {
+        let endpoint = format!("manual-labels/{}/comments/{}", issue_id, comment_id);
+        let mut map = Map::new();
+        map.insert("comment".to_string(), Value::String(new_text));
+        self.call_endpoint_json(
+            endpoint.as_str(), Verb::Patch, Value::Object(map)
+        )?;
+        Ok(())
+    }
+
+    pub(crate) fn delete_labeling_comment(&self,
+                                   issue_id: String,
+                                   comment_id: String) -> APIResult<()> {
+        let endpoint = format!("manual-labels/{}/comments/{}", issue_id, comment_id);
+        self.call_endpoint_json(
+            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
+        )?;
+        Ok(())
+    }
+
+    pub(crate) fn get_manual_labels(&self, issues: Vec<String>) -> APIResult<HashMap<String, Label>> {
+        #[derive(Debug, serde::Deserialize)]
+        struct LabelsResponse {
+            manual_labels: HashMap<String, Label>
+        }
+        let mut map = Map::new();
+        map.insert("issue_ids".to_string(),
+                   Value::Array(issues.into_iter().map(Value::String).collect()));
+        let result = self.call_endpoint_json::<_, LabelsResponse>(
+            "manual-labels", Verb::Get, map
+        )?;
+        Ok(result.manual_labels)
+    }
+
+    pub(crate) fn update_manual_label_for_issue(&self, issue_id: String, label: Label) -> APIResult<()> {
+        let endpoint = format!("manual-labels/{}", issue_id);
+        self.call_endpoint_json(endpoint.as_str(), Verb::Post, label)?;
+        Ok(())
+    }
+
+    /***************************************************************************
+     * Embedding-related endpoints
+     */
+
+    pub(crate) fn get_all_embeddings(&self) -> APIResult<Vec<UnboundEmbedding>> {
+        #[derive(Debug, serde::Deserialize)]
+        struct EmbeddingsResponse {
+            embeddings: Vec<UnboundEmbedding>
+        }
+        let result = self.call_endpoint_json::<_, EmbeddingsResponse>(
+            "embeddings", Verb::Get, Value::Object(Map::new())
+        )?;
+        Ok(result.embeddings)
+    }
+
+    pub(crate) fn create_embedding(&self,
+                            name: String,
+                            config: HashMap<String, Value>) -> APIResult<String> {
+        let mut map = Map::new();
+        map.insert("name".to_string(), Value::String(name));
+        map.insert("config".to_string(),
+                   Value::Object(Map::from_iter(config.into_iter())));
+        let result = self.call_endpoint_json::<_, String>(
+            "embeddings", Verb::Post, Value::Object(map)
+        )?;
+        Ok(result)
+    }
+
+    pub(crate) fn get_embedding(&self, id: String) -> APIResult<UnboundEmbedding> {
+        let endpoint = format!("embeddings/{}", id);
+        self.call_endpoint_json::<_, UnboundEmbedding>(
+            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
+        )
+    }
+
+    pub(crate) fn update_embedding(&self,
+                            id: String,
+                            name: String,
+                            config: HashMap<String, Value>) -> APIResult<()> {
+        let mut map = Map::new();
+        map.insert("name".to_string(), Value::String(name));
+        map.insert("config".to_string(),
+                   Value::Object(Map::from_iter(config.into_iter())));
+        let endpoint = format!("embeddings/{}", id);
+        self.call_endpoint_json(endpoint.as_str(), Verb::Post, map)?;
+        Ok(())
+    }
+
+
+    pub(crate) fn delete_embedding(&self, id: String) -> APIResult<()> {
+        let endpoint = format!("embeddings/{}", id);
+        self.call_endpoint_json(
+            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
+        )?;
+        Ok(())
+    }
+
+    pub(crate) fn upload_embedding_binary(&self, id: String, filename: String) -> APIResult<()> {
+        let form = multipart::Form::new().file("file", filename)?;
+        let endpoint = format!("embeddings/{}/file", id);
+        self.call_endpoint_multipart(endpoint.as_str(), Verb::Post, form)
+    }
+
+    pub(crate) fn download_embedding_binary(&self, id: String, filename: String) -> APIResult<()> {
+        let endpoint = format!("embeddings/{}/file", id);
+        self.call_endpoint_download(endpoint.as_str(),
+                                    Verb::Get,
+                                    Value::Object(Map::new()),
+                                    filename)
+    }
+
+    pub(crate) fn delete_embedding_binary(&self, id: String) -> APIResult<()> {
+        let endpoint = format!("embeddings/{}/file", id);
+        self.call_endpoint_json(
+            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
+        )?;
+        Ok(())
+    }
+
+    /***************************************************************************
+     * Repos and Project endpoints
+     */
+
+    pub(crate) fn get_all_repos(&self) -> APIResult<Vec<String>> {
+        #[derive(Debug, serde::Deserialize)]
+        struct ReposResponse {
+            repos: Vec<String>
+        }
+        let result = self.call_endpoint_json::<_, ReposResponse>(
+            "repos", Verb::Get, Value::Object(Map::new())
+        )?;
+        Ok(result.repos)
+    }
+
+    pub(crate) fn get_projects_for_repo(&self, repo: String) -> APIResult<Vec<String>> {
+        #[derive(Debug, serde::Deserialize)]
+        struct ProjectsResponse {
+            projects: Vec<String>
+        }
+        let endpoint = format!("repos/{}/projects", repo);
+        let result = self.call_endpoint_json::<_, ProjectsResponse>(
+            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
+        )?;
+        Ok(result.projects)
+    }
+
+    /***************************************************************************
+     * Model Config Endpoints
+     */
+
+    pub(crate) fn get_all_models(&self) -> APIResult<Vec<ModelInfo>> {
+        #[derive(Debug, serde::Deserialize)]
+        struct ModelsResponse {
+            models: Vec<ModelInfo>
+        }
+        let result = self.call_endpoint_json::<_, ModelsResponse>(
+            "models", Verb::Get, Value::Object(Map::new())
+        )?;
+        Ok(result.models)
+    }
+
+    pub(crate) fn create_model_config(&self,
+                                      name: String,
+                                      config: HashMap<String, Value>) -> APIResult<String> {
+        #[derive(Debug, serde::Deserialize)]
+        struct NewModelResponse {
+            model_id: String
+        }
+        let mut map = Map::new();
+        map.insert("model_name".to_string(), Value::String(name));
+        map.insert(
+            "model_config".to_string(),
+            Value::Object(Map::from_iter(config.into_iter()))
+        );
+        let result = self.call_endpoint_json::<_, NewModelResponse>(
+            "models", Verb::Post, Value::Object(map)
+        )?;
+        Ok(result.model_id)
+    }
+
+    pub(crate) fn get_model_config(&self, id: String) -> APIResult<UnboundModelConfig> {
+        let endpoint = format!("models/{}", id);
+        self.call_endpoint_json::<_, UnboundModelConfig>(
+            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
+        )
+    }
+
+    pub(crate) fn update_model_config(&self,
+                                      id: String,
+                                      name: String,
+                                      config: HashMap<String, Value>) -> APIResult<()> {
+        let endpoint = format!("models/{}", id);
+        let mut map = Map::new();
+        map.insert("model_name".to_string(), Value::String(name));
+        map.insert("model_config".to_string(),
+                   Value::Object(Map::from_iter(config.into_iter())));
+        self.call_endpoint_json(endpoint.as_str(), Verb::Post, Value::Object(map))
+    }
+
+    pub(crate) fn delete_model_config(&self, id: String) -> APIResult<()> {
+        let endpoint = format!("models/{}", id);
+        self.call_endpoint_json(
+            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
+        )
+    }
+
+    /***************************************************************************
+     * Model Versions
+     */
+
+    pub(crate) fn get_versions_for_model(&self,
+                                         model_id: String) -> APIResult<Vec<UnboundModelVersion>> {
+        let endpoint = format!("models/{}/versions", model_id.as_str());
+        #[derive(Debug, serde::Deserialize)]
+        struct RawVersionInfo {
+            version_id: String,
+            description: String
+        }
+        #[derive(Debug, serde::Deserialize)]
+        struct VersionsResponse {
+            versions: Vec<RawVersionInfo>
+        }
+        let result = self.call_endpoint_json::<_, VersionsResponse>(
+            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
+        )?;
+        let converted = result.versions
+            .into_iter()
+            .map(|v|
+                UnboundModelVersion{
+                    model_id: model_id.clone(),
+                    version_id: v.version_id,
+                    description: v.description
+                }
+            )
+            .collect();
+        Ok(converted)
+    }
+
+    pub(crate) fn upload_model_version(&self,
+                                       model_id: String,
+                                       file: String) -> APIResult<String> {
+        #[derive(Debug, serde::Deserialize)]
+        struct NewVersionResponse {
+            version_id: String
+        }
+        let form = multipart::Form::new()
+            .file("file", file)?;
+        let endpoint = format!("models/{}/versions", model_id);
+        let result = self.call_endpoint_multipart::<NewVersionResponse>(
+            endpoint.as_str(), Verb::Post, form
+        )?;
+        Ok(result.version_id)
+    }
+
+    pub(crate) fn download_model_version(&self,
+                                         model_id: String,
+                                         version_id: String,
+                                         filename: String) -> APIResult<()> {
+        let endpoint = format!("models/{}/versions/{}", model_id, version_id);
+        self.call_endpoint_download(endpoint.as_str(),
+                                    Verb::Get,
+                                    Value::Object(Map::new()),
+                                    filename)
+    }
+
+    pub(crate) fn delete_model_version(&self,
+                                       model_id: String,
+                                       version_id: String) -> APIResult<()> {
+        let endpoint = format!("models/{}/versions/{}", model_id, version_id);
+        self.call_endpoint_json(
+            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
+        )
+    }
+
+    pub(crate) fn update_version_description(&self,
+                                             model_id: String,
+                                             version_id: String,
+                                             description: String) -> APIResult<()> {
+        let endpoint = format!("models/{}/versions/{}/description", model_id, version_id);
+        let mut map = Map::new();
+        map.insert("description".to_string(), Value::String(description));
+        self.call_endpoint_json(endpoint.as_str(), Verb::Put, Value::Object(map))
+    }
+
+    /***************************************************************************
+    * Model Predictions
+    */
+
+    pub(crate) fn get_predictions(&self,
+                                  model_id: String,
+                                  version_id: String,
+                                  issues: Option<Vec<String>>) -> APIResult<HashMap<String, Value>> {
+        let endpoint = format!("models/{}/versions/{}/predictions", model_id, version_id);
+        let mut map = Map::new();
+        let payload = match issues {
+            None => Value::Null,
+            Some(ids) => Value::Array(ids.into_iter().map(Value::String).collect())
+        };
+        map.insert("issue_ids".to_string(), payload);
+        #[derive(Debug, serde::Deserialize)]
+        struct PredictionsResponse {
+            predictions: HashMap<String, Value>
+        }
+        let result = self.call_endpoint_json::<_, PredictionsResponse>(
+            endpoint.as_str(), Verb::Get, Value::Object(map)
+        )?;
+        Ok(result.predictions)
+    }
+
+    pub(crate) fn store_predictions(&self,
+                                    model_id: String,
+                                    version_id: String,
+                                    predictions: HashMap<String, Value>) -> APIResult<()> {
+        let endpoint = format!("models/{}/versions/{}/predictions", model_id, version_id);
+        let mut map = Map::new();
+        map.insert("predictions".to_string(),
+                   Value::Object(Map::from_iter(predictions.into_iter())));
+        self.call_endpoint_json(endpoint.as_str(), Verb::Post, Value::Object(map))
+    }
+
+    pub(crate) fn delete_predictions(&self,
+                                     model_id: String,
+                                     version_id: String) -> APIResult<()> {
+        let endpoint = format!("models/{}/versions/{}/predictions", model_id, version_id);
+        self.call_endpoint_json(
+            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
+        )
+    }
+
+    /***************************************************************************
+     * Model Performance
+     */
+
+    pub(crate) fn get_performances_for_model(&self, model_id: String) -> APIResult<Vec<UnboundTestRun>> {
+        #[derive(Debug, serde::Deserialize)]
+        struct PerformancesInfo {
+            performance_id: String,
+            description: String
+        }
+        #[derive(Debug, serde::Deserialize)]
+        struct PerformancesResponse {
+            performances: Vec<PerformancesInfo>
+        }
+        let endpoint = format!("models/{}/performances", model_id.as_str());
+        let result = self.call_endpoint_json::<_, PerformancesResponse>(
+            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
+        )?;
+        let converted = result.performances
+            .into_iter()
+            .map(|r| UnboundTestRun{
+                model_id: model_id.clone(),
+                performance_id: r.performance_id,
+                description: r.description
+            }).collect();
+        Ok(converted)
+    }
+
+    pub(crate) fn store_model_performance(&self,
+                                          model_id: String,
+                                          data: Vec<Value>) -> APIResult<String> {
+        #[derive(Debug, serde::Deserialize)]
+        struct NewPerformanceResponse {
+            performance_id: String
+        }
+        let mut map = Map::new();
+        map.insert("performance".to_string(), Value::Array(data));
+        let endpoint = format!("models/{}/performances", model_id);
+        let result = self.call_endpoint_json::<_, NewPerformanceResponse>(
+            endpoint.as_str(), Verb::Post, Value::Object(map)
+        )?;
+        Ok(result.performance_id)
+    }
+
+    pub(crate) fn get_performance_data(&self,
+                                       model_id: String,
+                                       performance_id: String) -> APIResult<Vec<Value>> {
+        #[derive(Debug, serde::Deserialize)]
+        struct PerformanceDataResponse {
+            performance_id: String,
+            description: String,
+            performance: Vec<Value>
+        }
+        let endpoint = format!("models/{}/performances/{}", model_id, performance_id);
+        let result = self.call_endpoint_json::<_, PerformanceDataResponse>(
+            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
+        )?;
+        Ok(result.performance)
+    }
+
+    pub(crate) fn delete_performance_data(&self,
+                                          model_id: String,
+                                          performance_id: String) -> APIResult<()> {
+        let endpoint = format!("models/{}/performances/{}", model_id, performance_id);
+        self.call_endpoint_json(
+            endpoint.as_str(), Verb::Delete, Value::Object(Map::new())
+        )
+    }
+
+    pub(crate) fn update_performance_description(&self,
+                                                 model_id: String,
+                                                 performance_id: String,
+                                                 description: String) -> APIResult<()> {
+        let endpoint = format!("models/{}/performances/{}/description", model_id, performance_id);
+        let mut map = Map::new();
+        map.insert("description".to_string(), Value::String(description));
+        self.call_endpoint_json(endpoint.as_str(), Verb::Put, Value::Object(map))
+    }
+}
```

### Comparing `issue_db_api-0.1.0/issue_db_api/src/comments.rs` & `issue_db_api-0.2.0/issue_db_api/src/comments.rs`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-use std::sync::Arc;
-use crate::api_core::IssueAPI;
-use crate::APIResult;
-
-#[allow(unused)]
-#[derive(Debug)]
-pub struct UnboundComment {
-    pub(crate) id: String,
-    pub(crate) author: String,
-    pub(crate) text: String
-}
-
-impl UnboundComment {
-    pub fn into_comment(self, api: Arc<IssueAPI>, parent: String) -> Comment {
-        Comment{api, parent, id: self.id, author: self.author, text: self.text}
-    }
-}
-
-
-#[allow(unused)]
-#[derive(Debug, Clone)]
-pub struct Comment {
-    api: Arc<IssueAPI>,
-    parent: String,
-    id: String,
-    author: String,
-    text: String
-}
-
-impl Comment {
-    pub(crate) fn identifier(&self) -> &String {
-        &self.id
-    }
-
-    pub fn author(&self) -> &String {
-        &self.author
-    }
-
-    pub fn text(&self) -> &String {
-        &self.text
-    }
-
-    pub fn update_text(&mut self, text: String) -> APIResult<()> {
-        self.api.update_labeling_comment(
-            self.parent.clone(),
-            self.id.clone(),
-            text.clone())?;
-        self.text = text;
-        Ok(())
-    }
+use std::sync::Arc;
+use crate::api_core::IssueAPI;
+use crate::APIResult;
+
+#[allow(unused)]
+#[derive(Debug)]
+pub struct UnboundComment {
+    pub(crate) id: String,
+    pub(crate) author: String,
+    pub(crate) text: String
+}
+
+impl UnboundComment {
+    pub fn into_comment(self, api: Arc<IssueAPI>, parent: String) -> Comment {
+        Comment{api, parent, id: self.id, author: self.author, text: self.text}
+    }
+}
+
+
+#[allow(unused)]
+#[derive(Debug, Clone)]
+pub struct Comment {
+    api: Arc<IssueAPI>,
+    parent: String,
+    id: String,
+    author: String,
+    text: String
+}
+
+impl Comment {
+    pub(crate) fn identifier(&self) -> &String {
+        &self.id
+    }
+
+    pub fn author(&self) -> &String {
+        &self.author
+    }
+
+    pub fn text(&self) -> &String {
+        &self.text
+    }
+
+    pub fn update_text(&mut self, text: String) -> APIResult<()> {
+        self.api.update_labeling_comment(
+            self.parent.clone(),
+            self.id.clone(),
+            text.clone())?;
+        self.text = text;
+        Ok(())
+    }
 }
```

### Comparing `issue_db_api-0.1.0/issue_db_api/src/config.rs` & `issue_db_api-0.2.0/issue_db_api/src/config.rs`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-use std::collections::HashMap;
-use std::error::Error;
-use std::sync::Arc;
-use crate::api_core::IssueAPI;
-use crate::{APIResult, Query, QueryCMP};
-use crate::errors::APIError;
-use crate::issues::Issue;
-
-#[allow(unused)]
-#[derive(Debug, Copy, Clone, PartialEq, Eq)]
-pub enum ConfigHandlingPolicy {
-    ReadLocalWriteNoFetch,
-    ReadLocalWriteWithFetch,
-    ReadFetchWriteWithFetch
-}
-
-
-#[allow(unused)]
-#[derive(Debug, Copy, Clone, PartialEq, Eq)]
-pub enum CachingPolicy {
-    NoCaching,
-    UseLocalAfterLoad
-}
-
-
-#[allow(unused)]
-#[derive(Debug, Copy, Clone)]
-pub enum IssueAttribute {
-    Key,
-    Summary, Description, Comments,
-    Parent, Subtasks, IssueLinks,
-    Status, Priority, Resolution, IssueType,
-    Watches, Votes,
-    DateCreated, DateUpdated, DateResolved,
-    Labels, Components,
-    AffectedVersions, FixVersions
-}
-
-impl std::fmt::Display for IssueAttribute {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        let text = match self {
-            IssueAttribute::Key => "key",
-            IssueAttribute::Summary => "summary",
-            IssueAttribute::Description => "description",
-            IssueAttribute::Comments => "comments",
-            IssueAttribute::Parent => "parent",
-            IssueAttribute::Subtasks => "subtasks",
-            IssueAttribute::IssueLinks => "issuelinks",
-            IssueAttribute::Status => "status",
-            IssueAttribute::Priority => "priority",
-            IssueAttribute::Resolution => "resolution",
-            IssueAttribute::IssueType => "issuetype",
-            IssueAttribute::Watches => "watches",
-            IssueAttribute::Votes => "votes",
-            IssueAttribute::DateCreated => "created",
-            IssueAttribute::DateUpdated => "updated",
-            IssueAttribute::DateResolved => "resolutiondate",
-            IssueAttribute::Labels => "labels",
-            IssueAttribute::Components => "components",
-            IssueAttribute::AffectedVersions => "versions",
-            IssueAttribute::FixVersions => "fixVersions"
-        };
-        write!(f, "{}", text)
-    }
-}
-
-impl TryFrom<String> for IssueAttribute {
-    type Error = Box<dyn Error>;
-
-    fn try_from(value: String) -> Result<Self, Self::Error> {
-        let attr = match value.as_str() {
-            "key" => IssueAttribute::Key,
-            "summary" => IssueAttribute::Summary,
-            "description" => IssueAttribute::Description,
-            "comments" => IssueAttribute::Comments,
-            "parent" => IssueAttribute::Parent,
-            "subtasks" => IssueAttribute::Subtasks,
-            "issue_links" => IssueAttribute::IssueLinks,
-            "status" => IssueAttribute::Status,
-            "priority" => IssueAttribute::Priority,
-            "resolution" => IssueAttribute::Resolution,
-            "issue_type" => IssueAttribute::IssueType,
-            "watches" => IssueAttribute::Watches,
-            "votes" => IssueAttribute::Votes,
-            "date_created" => IssueAttribute::DateCreated,
-            "date_updated" => IssueAttribute::DateUpdated,
-            "date_resolved" => IssueAttribute::DateResolved,
-            "labels" => IssueAttribute::Labels,
-            "components" => IssueAttribute::Components,
-            "affected+versions" => IssueAttribute::AffectedVersions,
-            "fix_versions" => IssueAttribute::FixVersions,
-            _ => {
-                let msg = format!("\"{}\" is an invalid issue attribute", value);
-                return Err(Box::new(APIError::new(msg)));
-            }
-        };
-        Ok(attr)
-    }
-}
-
-
-#[allow(unused)]
-#[derive(Debug, Clone, Default)]
-pub struct IssueLoadingSettings {
-    attributes: Vec<IssueAttribute>,
-    preload_labels: bool,
-}
-
-
-#[allow(unused)]
-impl IssueLoadingSettings {
-    pub fn new(attributes: Vec<IssueAttribute>,
-               preload_labels: bool) -> Self {
-        Self{attributes, preload_labels}
-    }
-
-    pub fn load_issues(self,
-                       api: Arc<IssueAPI>,
-                       ids: Vec<String>,
-                       label_caching_policy: CachingPolicy) -> APIResult<Vec<Issue>> {
-        let labels = if self.preload_labels {
-            let query = Query::And(vec![
-                Query::Tag(QueryCMP::Eq, "has-label".to_string()),
-                Query::Or(ids.iter().cloned().map(Query::Identifier).collect())
-            ]);
-            let ids_with_label = api.search(query)?;
-            api.get_manual_labels(ids_with_label)?
-        } else {
-            HashMap::new()
-        };
-        let data = api.get_issue_data(
-            ids.clone(), self.attributes
-        )?;
-        let issues = ids.into_iter()
-            .map(|id| Issue::new(
-                api.clone(),
-                id.clone(),
-                data.get(&id).unwrap().clone(),
-                label_caching_policy,
-                labels.get(&id).cloned()))
-            .collect();
-        Ok(issues)
-    }
-
-    pub fn load_issue(self,
-                      api: Arc<IssueAPI>,
-                      id: String,
-                      label_caching_policy: CachingPolicy) -> APIResult<Issue> {
-        let issue = self.load_issues(api, vec![id], label_caching_policy)?
-            .into_iter()
-            .last()
-            .expect("Failed to load issue");
-        Ok(issue)
-    }
-}
-
+use std::collections::HashMap;
+use std::error::Error;
+use std::sync::Arc;
+use crate::api_core::IssueAPI;
+use crate::{APIResult, Query, QueryCMP};
+use crate::errors::APIError;
+use crate::issues::Issue;
+
+#[allow(unused)]
+#[derive(Debug, Copy, Clone, PartialEq, Eq)]
+pub enum ConfigHandlingPolicy {
+    ReadLocalWriteNoFetch,
+    ReadLocalWriteWithFetch,
+    ReadFetchWriteWithFetch
+}
+
+
+#[allow(unused)]
+#[derive(Debug, Copy, Clone, PartialEq, Eq)]
+pub enum CachingPolicy {
+    NoCaching,
+    UseLocalAfterLoad
+}
+
+
+#[allow(unused)]
+#[derive(Debug, Copy, Clone)]
+pub enum IssueAttribute {
+    Key,
+    Summary, Description, Comments,
+    Parent, Subtasks, IssueLinks,
+    Status, Priority, Resolution, IssueType,
+    Watches, Votes,
+    DateCreated, DateUpdated, DateResolved,
+    Labels, Components,
+    AffectedVersions, FixVersions
+}
+
+impl std::fmt::Display for IssueAttribute {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        let text = match self {
+            IssueAttribute::Key => "key",
+            IssueAttribute::Summary => "summary",
+            IssueAttribute::Description => "description",
+            IssueAttribute::Comments => "comments",
+            IssueAttribute::Parent => "parent",
+            IssueAttribute::Subtasks => "subtasks",
+            IssueAttribute::IssueLinks => "issuelinks",
+            IssueAttribute::Status => "status",
+            IssueAttribute::Priority => "priority",
+            IssueAttribute::Resolution => "resolution",
+            IssueAttribute::IssueType => "issuetype",
+            IssueAttribute::Watches => "watches",
+            IssueAttribute::Votes => "votes",
+            IssueAttribute::DateCreated => "created",
+            IssueAttribute::DateUpdated => "updated",
+            IssueAttribute::DateResolved => "resolutiondate",
+            IssueAttribute::Labels => "labels",
+            IssueAttribute::Components => "components",
+            IssueAttribute::AffectedVersions => "versions",
+            IssueAttribute::FixVersions => "fixVersions"
+        };
+        write!(f, "{}", text)
+    }
+}
+
+impl TryFrom<String> for IssueAttribute {
+    type Error = Box<dyn Error>;
+
+    fn try_from(value: String) -> Result<Self, Self::Error> {
+        let attr = match value.as_str() {
+            "key" => IssueAttribute::Key,
+            "summary" => IssueAttribute::Summary,
+            "description" => IssueAttribute::Description,
+            "comments" => IssueAttribute::Comments,
+            "parent" => IssueAttribute::Parent,
+            "subtasks" => IssueAttribute::Subtasks,
+            "issue_links" => IssueAttribute::IssueLinks,
+            "status" => IssueAttribute::Status,
+            "priority" => IssueAttribute::Priority,
+            "resolution" => IssueAttribute::Resolution,
+            "issue_type" => IssueAttribute::IssueType,
+            "watches" => IssueAttribute::Watches,
+            "votes" => IssueAttribute::Votes,
+            "date_created" => IssueAttribute::DateCreated,
+            "date_updated" => IssueAttribute::DateUpdated,
+            "date_resolved" => IssueAttribute::DateResolved,
+            "labels" => IssueAttribute::Labels,
+            "components" => IssueAttribute::Components,
+            "affected+versions" => IssueAttribute::AffectedVersions,
+            "fix_versions" => IssueAttribute::FixVersions,
+            _ => {
+                let msg = format!("\"{}\" is an invalid issue attribute", value);
+                return Err(Box::new(APIError::new(msg)));
+            }
+        };
+        Ok(attr)
+    }
+}
+
+
+#[allow(unused)]
+#[derive(Debug, Clone, Default)]
+pub struct IssueLoadingSettings {
+    attributes: Vec<IssueAttribute>,
+    preload_labels: bool,
+}
+
+
+#[allow(unused)]
+impl IssueLoadingSettings {
+    pub fn new(attributes: Vec<IssueAttribute>,
+               preload_labels: bool) -> Self {
+        Self{attributes, preload_labels}
+    }
+
+    pub fn load_issues(self,
+                       api: Arc<IssueAPI>,
+                       ids: Vec<String>,
+                       label_caching_policy: CachingPolicy) -> APIResult<Vec<Issue>> {
+        let labels = if self.preload_labels {
+            let query = Query::And(vec![
+                Query::Tag(QueryCMP::Eq, "has-label".to_string()),
+                Query::Or(ids.iter().cloned().map(Query::Identifier).collect())
+            ]);
+            let ids_with_label = api.search(query)?;
+            api.get_manual_labels(ids_with_label)?
+        } else {
+            HashMap::new()
+        };
+        let data = api.get_issue_data(
+            ids.clone(), self.attributes
+        )?;
+        let issues = ids.into_iter()
+            .map(|id| Issue::new(
+                api.clone(),
+                id.clone(),
+                data.get(&id).unwrap().clone(),
+                label_caching_policy,
+                labels.get(&id).cloned()))
+            .collect();
+        Ok(issues)
+    }
+
+    pub fn load_issue(self,
+                      api: Arc<IssueAPI>,
+                      id: String,
+                      label_caching_policy: CachingPolicy) -> APIResult<Issue> {
+        let issue = self.load_issues(api, vec![id], label_caching_policy)?
+            .into_iter()
+            .last()
+            .expect("Failed to load issue");
+        Ok(issue)
+    }
+}
+
```

### Comparing `issue_db_api-0.1.0/issue_db_api/src/embedding.rs` & `issue_db_api-0.2.0/issue_db_api/src/embedding.rs`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-use std::collections::HashMap;
-use std::hash::{Hash, Hasher};
-use std::sync::Arc;
-use serde_json::Value;
-use crate::api_core::IssueAPI;
-use crate::APIResult;
-use crate::config::ConfigHandlingPolicy;
-
-#[allow(unused)]
-#[derive(Debug, serde::Deserialize)]
-pub(crate) struct UnboundEmbedding {
-    pub(crate) embedding_id: String,
-    pub(crate) name: String,
-    pub(crate) config: HashMap<String, Value>,
-    pub(crate) has_file: bool
-}
-
-impl UnboundEmbedding {
-    pub(crate) fn into_bound_embedding(self,
-                                       api: Arc<IssueAPI>,
-                                       config_handling: ConfigHandlingPolicy) -> Embedding {
-        Embedding{
-            api,
-            name: self.name,
-            id: self.embedding_id,
-            config: self.config,
-            has_file: self.has_file,
-            update_policy: config_handling
-        }
-    }
-}
-
-#[allow(unused)]
-#[derive(Debug)]
-pub struct Embedding {
-    api: Arc<IssueAPI>,
-    id: String,
-    name: String ,
-    config: HashMap<String, Value>,
-    has_file: bool,
-    update_policy: ConfigHandlingPolicy
-}
-
-impl PartialEq for Embedding {
-    fn eq(&self, other: &Self) -> bool {
-        self.id == other.id
-    }
-}
-
-impl Eq for Embedding {}
-
-impl Hash for Embedding {
-    fn hash<H: Hasher>(&self, state: &mut H) {
-        self.id.hash(state)
-    }
-}
-
-impl Embedding {
-    pub(crate) fn new(api: Arc<IssueAPI>,
-                      id: String,
-                      name: String,
-                      config: HashMap<String, Value>,
-                      has_file: bool,
-                      update_policy: ConfigHandlingPolicy) -> Self {
-        Embedding{api, id, name, config, has_file, update_policy}
-    }
-
-    pub fn identifier(&self) -> &String {
-        &self.id
-    }
-
-    pub fn name(&self) -> APIResult<String> {
-        match self.update_policy {
-            ConfigHandlingPolicy::ReadFetchWriteWithFetch => {
-                let name = self.api.get_embedding(self.id.clone())?.name;
-                Ok(name)
-            },
-            _ => Ok(self.name.clone())
-        }
-    }
-
-    pub fn update_name(&mut self, name: String) -> APIResult<()> {
-        let config = match self.update_policy {
-            ConfigHandlingPolicy::ReadLocalWriteNoFetch => self.config.clone(),
-            _ => self.api.get_embedding(self.id.clone())?.config
-        };
-        self.api.update_embedding(self.id.clone(),
-                                  name.clone(),
-                                  config)?;
-        self.name = name;
-        Ok(())
-    }
-
-    pub fn config(&self) -> APIResult<HashMap<String, Value>> {
-        match self.update_policy {
-            ConfigHandlingPolicy::ReadFetchWriteWithFetch => {
-                let config = self.api.get_embedding(self.id.clone())?.config;
-                Ok(config)
-            },
-            _ => Ok(self.config.clone())
-        }
-    }
-
-    pub fn update_config(&mut self, config: HashMap<String, Value>) -> APIResult<()> {
-        let name = match self.update_policy {
-            ConfigHandlingPolicy::ReadLocalWriteNoFetch => self.name.clone(),
-            _ => self.api.get_embedding(self.id.clone())?.name
-        };
-        self.api.update_embedding(self.id.clone(),
-                                  name,
-                                  config.clone())?;
-        self.config = config;
-        Ok(())
-    }
-
-    pub fn download_binary(&self, path: String) -> APIResult<()> {
-        self.api.download_embedding_binary(self.id.clone(), path)
-    }
-
-    pub fn upload_binary(&self, path: String) -> APIResult<()> {
-        self.api.upload_embedding_binary(self.id.clone(), path)
-    }
-
-    pub fn delete_binary(&self) -> APIResult<()> {
-        self.api.delete_embedding_binary(self.id.clone())
-    }
+use std::collections::HashMap;
+use std::hash::{Hash, Hasher};
+use std::sync::Arc;
+use serde_json::Value;
+use crate::api_core::IssueAPI;
+use crate::APIResult;
+use crate::config::ConfigHandlingPolicy;
+
+#[allow(unused)]
+#[derive(Debug, serde::Deserialize)]
+pub(crate) struct UnboundEmbedding {
+    pub(crate) embedding_id: String,
+    pub(crate) name: String,
+    pub(crate) config: HashMap<String, Value>,
+    pub(crate) has_file: bool
+}
+
+impl UnboundEmbedding {
+    pub(crate) fn into_bound_embedding(self,
+                                       api: Arc<IssueAPI>,
+                                       config_handling: ConfigHandlingPolicy) -> Embedding {
+        Embedding{
+            api,
+            name: self.name,
+            id: self.embedding_id,
+            config: self.config,
+            has_file: self.has_file,
+            update_policy: config_handling
+        }
+    }
+}
+
+#[allow(unused)]
+#[derive(Debug)]
+pub struct Embedding {
+    api: Arc<IssueAPI>,
+    id: String,
+    name: String ,
+    config: HashMap<String, Value>,
+    has_file: bool,
+    update_policy: ConfigHandlingPolicy
+}
+
+impl PartialEq for Embedding {
+    fn eq(&self, other: &Self) -> bool {
+        self.id == other.id
+    }
+}
+
+impl Eq for Embedding {}
+
+impl Hash for Embedding {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.id.hash(state)
+    }
+}
+
+impl Embedding {
+    pub(crate) fn new(api: Arc<IssueAPI>,
+                      id: String,
+                      name: String,
+                      config: HashMap<String, Value>,
+                      has_file: bool,
+                      update_policy: ConfigHandlingPolicy) -> Self {
+        Embedding{api, id, name, config, has_file, update_policy}
+    }
+
+    pub fn identifier(&self) -> &String {
+        &self.id
+    }
+
+    pub fn name(&self) -> APIResult<String> {
+        match self.update_policy {
+            ConfigHandlingPolicy::ReadFetchWriteWithFetch => {
+                let name = self.api.get_embedding(self.id.clone())?.name;
+                Ok(name)
+            },
+            _ => Ok(self.name.clone())
+        }
+    }
+
+    pub fn update_name(&mut self, name: String) -> APIResult<()> {
+        let config = match self.update_policy {
+            ConfigHandlingPolicy::ReadLocalWriteNoFetch => self.config.clone(),
+            _ => self.api.get_embedding(self.id.clone())?.config
+        };
+        self.api.update_embedding(self.id.clone(),
+                                  name.clone(),
+                                  config)?;
+        self.name = name;
+        Ok(())
+    }
+
+    pub fn config(&self) -> APIResult<HashMap<String, Value>> {
+        match self.update_policy {
+            ConfigHandlingPolicy::ReadFetchWriteWithFetch => {
+                let config = self.api.get_embedding(self.id.clone())?.config;
+                Ok(config)
+            },
+            _ => Ok(self.config.clone())
+        }
+    }
+
+    pub fn update_config(&mut self, config: HashMap<String, Value>) -> APIResult<()> {
+        let name = match self.update_policy {
+            ConfigHandlingPolicy::ReadLocalWriteNoFetch => self.name.clone(),
+            _ => self.api.get_embedding(self.id.clone())?.name
+        };
+        self.api.update_embedding(self.id.clone(),
+                                  name,
+                                  config.clone())?;
+        self.config = config;
+        Ok(())
+    }
+
+    pub fn download_binary(&self, path: String) -> APIResult<()> {
+        self.api.download_embedding_binary(self.id.clone(), path)
+    }
+
+    pub fn upload_binary(&self, path: String) -> APIResult<()> {
+        self.api.upload_embedding_binary(self.id.clone(), path)
+    }
+
+    pub fn delete_binary(&self) -> APIResult<()> {
+        self.api.delete_embedding_binary(self.id.clone())
+    }
 }
```

### Comparing `issue_db_api-0.1.0/issue_db_api/src/issues.rs` & `issue_db_api-0.2.0/issue_db_api/src/issues.rs`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,282 +1,282 @@
-use std::hash::{Hash, Hasher};
-use std::sync::{Arc, RwLock};
-use std::sync::atomic::{AtomicBool, Ordering};
-use crate::api_core::{IssueAPI, IssueData};
-use crate::comments::Comment;
-use crate::config::{CachingPolicy, IssueLoadingSettings};
-use crate::labels::Label;
-use crate::util::APIResult;
-
-#[allow(unused)]
-#[derive(Debug)]
-pub struct Issue {
-    api: Arc<IssueAPI>,
-    ident: String,
-    data: IssueData,
-    caching_policy: CachingPolicy,
-    label: RwLock<Option<Label>>,
-    dirty: AtomicBool
-}
-
-impl Hash for Issue {
-    fn hash<H: Hasher>(&self, state: &mut H) {
-        self.ident.hash(state);
-    }
-}
-
-impl PartialEq for Issue {
-    fn eq(&self, other: &Self) -> bool {
-        self.ident == other.ident
-    }
-}
-
-impl Eq for Issue {}
-
-#[allow(unused)]
-impl Issue {
-    pub(crate) fn new(api: Arc<IssueAPI>,
-                      ident: String,
-                      data: IssueData,
-                      caching: CachingPolicy,
-                      label: Option<Label>) -> Self {
-         Self{
-             api, ident, data,
-             caching_policy: caching,
-             label: RwLock::new(label),
-             dirty: AtomicBool::new(false)
-        }
-    }
-
-    #[inline(always)]
-    pub fn ident(&self) -> &String {
-        &self.ident
-    }
-
-    pub fn get_manual_label(&self) -> APIResult<Option<Label>> {
-        match self.caching_policy {
-            CachingPolicy::NoCaching => {
-                self.load_label()
-            }
-            CachingPolicy::UseLocalAfterLoad => {
-                let label = self.label
-                    .read()
-                    .expect("RwLock has been poisoned. Cannot recover");
-                if label.is_some() && !self.dirty.load(Ordering::Acquire) {
-                    Ok(Some(label.unwrap()))
-                } else {
-                    // First, acquire the write lock
-                    std::mem::drop(label);
-                    let mut label = self.label
-                        .write()
-                        .expect("RwLock has been poisoned. Cannot recover");
-                    // With the write lock in hand, check if another thread
-                    // updated the label in the meantime.
-                    if self.dirty.load(Ordering::Relaxed) && label.is_none() {
-                        // The label is definitely dirty; update it
-                        if let Some(inner) = self.load_label()? {
-                            label.insert(inner);
-                            self.dirty.store(false, Ordering::Release);
-                            Ok(Some(inner))
-                        } else {
-                            label.take();
-                            self.dirty.store(false, Ordering::Release);
-                            Ok(None)
-                        }
-                    } else {
-                        // Another thread updated the label; use a recursive
-                        // call to fetch the label.
-                        self.get_manual_label()
-                    }
-                }
-            }
-        }
-    }
-
-    fn load_label(&self) -> APIResult<Option<Label>> {
-        let labels = self.api.get_manual_labels(
-            vec![self.ident.clone()]
-        )?;
-        Ok(labels.get(&self.ident).copied())
-    }
-
-    pub fn set_manual_label(&self, label: Label) -> APIResult<()> {
-        self.api.update_manual_label_for_issue(self.ident.clone(), label)?;
-        if self.caching_policy == CachingPolicy::UseLocalAfterLoad {
-            let mut label = self.label
-                .write()
-                .expect("RwLock has been poisoned. Cannot recover");
-            if let Some(inner) = self.load_label()? {
-                label.insert(inner);
-            } else {
-                label.take();
-            }
-        }
-        Ok(())
-    }
-
-    pub fn invalidate_cached_label(&self) {
-        self.dirty.store(true, Ordering::Release);
-    }
-
-    pub fn get_tags(&self) -> APIResult<Vec<String>> {
-        self.api.get_tags_for_issue(self.ident.clone())
-    }
-
-    pub fn add_tag(&self, name: String) -> APIResult<()> {
-        self.api.add_tag_to_issue(self.ident.clone(), name)
-    }
-
-    pub fn remove_tag(&self, name: String) -> APIResult<()> {
-        self.api.remove_tag_from_issue(self.ident.clone(), name)
-    }
-
-    pub fn start_review(&self) -> APIResult<()> {
-        self.api.start_issue_review(self.ident.clone())
-    }
-
-    pub fn finish_review(&self) -> APIResult<()> {
-        self.api.finish_issue_review(self.ident.clone())
-    }
-
-    pub fn in_review(&self) -> APIResult<bool> {
-        Ok(self.get_tags()?.contains(&"needs-review".to_string()))
-    }
-
-    pub fn get_labelling_comments(&self) -> APIResult<Vec<Comment>> {
-        let comments = self.api
-            .get_labeling_comments_for_issue(self.ident.clone())?
-            .into_iter()
-            .map(|r| r.into_comment(self.api.clone(), self.ident.clone()))
-            .collect();
-        Ok(comments)
-    }
-
-    pub fn add_labelling_comment(&self, text: String) -> APIResult<()> {
-        let _ = self.api.add_labeling_comment_to_issue(self.ident.clone(), text)?;
-        Ok(())
-    }
-
-    pub fn remove_labelling_comment(&self, comment: Comment) -> APIResult<()> {
-        self.api.delete_labeling_comment(self.ident.clone(), comment.identifier().clone())
-    }
-
-    #[inline(always)]
-    pub fn key(&self) -> APIResult<&String> {
-        self.data.key(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn summary(&self) -> APIResult<&String> {
-        self.data.summary(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn description(&self) -> APIResult<&String> {
-        self.data.description(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn comments(&self) -> APIResult<&Vec<String>> {
-        self.data.comments(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn status(&self) -> APIResult<&String> {
-        self.data.status(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn priority(&self) -> APIResult<&String> {
-        self.data.priority(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn resolution(&self) -> APIResult<&Option<String>> {
-        self.data.resolution(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn issue_type(&self) -> APIResult<&String> {
-        self.data.issue_type(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn issue_links(&self, loading_settings: IssueLoadingSettings) -> APIResult<Vec<Issue>> {
-        let ids = self.data.issue_links(&self.api)?;
-        let issues = loading_settings.load_issues(
-            self.api.clone(), ids.clone(), self.caching_policy
-        )?;
-        assert_eq!(issues.len(), ids.len(), "Failed to retrieve all linked issues");
-        Ok(issues)
-    }
-
-    #[inline(always)]
-    pub fn parent(&self, loading_settings: IssueLoadingSettings) -> APIResult<Option<Issue>> {
-        if let Some(id) = self.data.parent(&self.api)? {
-            Ok(
-                Some(
-                    loading_settings.load_issue(self.api.clone(),
-                                                id.clone(),
-                                                self.caching_policy)?
-                )
-            )
-        } else {
-            Ok(None)
-        }
-    }
-
-    #[inline(always)]
-    pub fn subtasks(&self, loading_settings: IssueLoadingSettings) -> APIResult<Vec<Issue>> {
-        let ids = self.data.subtasks(&self.api)?;
-        let issues = loading_settings.load_issues(
-            self.api.clone(), ids.clone(), self.caching_policy
-        )?;
-        assert_eq!(issues.len(), ids.len(), "Failed to retrieve all subtasks");
-        Ok(issues)
-    }
-
-    #[inline(always)]
-    pub fn watches(&self) -> APIResult<u64> {
-        self.data.watches(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn votes(&self) -> APIResult<u64> {
-        self.data.votes(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn date_created(&self) -> APIResult<&String> {
-        self.data.date_created(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn date_updated(&self) -> APIResult<&String> {
-        self.data.date_updated(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn date_resolved(&self) -> APIResult<&Option<String>> {
-        self.data.date_resolved(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn labels(&self) -> APIResult<&Vec<String>> {
-        self.data.labels(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn components(&self) -> APIResult<&Vec<String>> {
-        self.data.components(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn affected_versions(&self) -> APIResult<&Vec<String>> {
-        self.data.affected_versions(&self.api)
-    }
-
-    #[inline(always)]
-    pub fn fix_versions(&self) -> APIResult<&Vec<String>> {
-        self.data.fix_versions(&self.api)
-    }
-}
+use std::hash::{Hash, Hasher};
+use std::sync::{Arc, RwLock};
+use std::sync::atomic::{AtomicBool, Ordering};
+use crate::api_core::{IssueAPI, IssueData};
+use crate::comments::Comment;
+use crate::config::{CachingPolicy, IssueLoadingSettings};
+use crate::labels::Label;
+use crate::util::APIResult;
+
+#[allow(unused)]
+#[derive(Debug)]
+pub struct Issue {
+    api: Arc<IssueAPI>,
+    ident: String,
+    data: IssueData,
+    caching_policy: CachingPolicy,
+    label: RwLock<Option<Label>>,
+    dirty: AtomicBool
+}
+
+impl Hash for Issue {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.ident.hash(state);
+    }
+}
+
+impl PartialEq for Issue {
+    fn eq(&self, other: &Self) -> bool {
+        self.ident == other.ident
+    }
+}
+
+impl Eq for Issue {}
+
+#[allow(unused)]
+impl Issue {
+    pub(crate) fn new(api: Arc<IssueAPI>,
+                      ident: String,
+                      data: IssueData,
+                      caching: CachingPolicy,
+                      label: Option<Label>) -> Self {
+         Self{
+             api, ident, data,
+             caching_policy: caching,
+             label: RwLock::new(label),
+             dirty: AtomicBool::new(false)
+        }
+    }
+
+    #[inline(always)]
+    pub fn ident(&self) -> &String {
+        &self.ident
+    }
+
+    pub fn get_manual_label(&self) -> APIResult<Option<Label>> {
+        match self.caching_policy {
+            CachingPolicy::NoCaching => {
+                self.load_label()
+            }
+            CachingPolicy::UseLocalAfterLoad => {
+                let label = self.label
+                    .read()
+                    .expect("RwLock has been poisoned. Cannot recover");
+                if label.is_some() && !self.dirty.load(Ordering::Acquire) {
+                    Ok(Some(label.unwrap()))
+                } else {
+                    // First, acquire the write lock
+                    std::mem::drop(label);
+                    let mut label = self.label
+                        .write()
+                        .expect("RwLock has been poisoned. Cannot recover");
+                    // With the write lock in hand, check if another thread
+                    // updated the label in the meantime.
+                    if self.dirty.load(Ordering::Relaxed) && label.is_none() {
+                        // The label is definitely dirty; update it
+                        if let Some(inner) = self.load_label()? {
+                            label.insert(inner);
+                            self.dirty.store(false, Ordering::Release);
+                            Ok(Some(inner))
+                        } else {
+                            label.take();
+                            self.dirty.store(false, Ordering::Release);
+                            Ok(None)
+                        }
+                    } else {
+                        // Another thread updated the label; use a recursive
+                        // call to fetch the label.
+                        self.get_manual_label()
+                    }
+                }
+            }
+        }
+    }
+
+    fn load_label(&self) -> APIResult<Option<Label>> {
+        let labels = self.api.get_manual_labels(
+            vec![self.ident.clone()]
+        )?;
+        Ok(labels.get(&self.ident).copied())
+    }
+
+    pub fn set_manual_label(&self, label: Label) -> APIResult<()> {
+        self.api.update_manual_label_for_issue(self.ident.clone(), label)?;
+        if self.caching_policy == CachingPolicy::UseLocalAfterLoad {
+            let mut label = self.label
+                .write()
+                .expect("RwLock has been poisoned. Cannot recover");
+            if let Some(inner) = self.load_label()? {
+                label.insert(inner);
+            } else {
+                label.take();
+            }
+        }
+        Ok(())
+    }
+
+    pub fn invalidate_cached_label(&self) {
+        self.dirty.store(true, Ordering::Release);
+    }
+
+    pub fn get_tags(&self) -> APIResult<Vec<String>> {
+        self.api.get_tags_for_issue(self.ident.clone())
+    }
+
+    pub fn add_tag(&self, name: String) -> APIResult<()> {
+        self.api.add_tag_to_issue(self.ident.clone(), name)
+    }
+
+    pub fn remove_tag(&self, name: String) -> APIResult<()> {
+        self.api.remove_tag_from_issue(self.ident.clone(), name)
+    }
+
+    pub fn start_review(&self) -> APIResult<()> {
+        self.api.start_issue_review(self.ident.clone())
+    }
+
+    pub fn finish_review(&self) -> APIResult<()> {
+        self.api.finish_issue_review(self.ident.clone())
+    }
+
+    pub fn in_review(&self) -> APIResult<bool> {
+        Ok(self.get_tags()?.contains(&"needs-review".to_string()))
+    }
+
+    pub fn get_labelling_comments(&self) -> APIResult<Vec<Comment>> {
+        let comments = self.api
+            .get_labeling_comments_for_issue(self.ident.clone())?
+            .into_iter()
+            .map(|r| r.into_comment(self.api.clone(), self.ident.clone()))
+            .collect();
+        Ok(comments)
+    }
+
+    pub fn add_labelling_comment(&self, text: String) -> APIResult<()> {
+        let _ = self.api.add_labeling_comment_to_issue(self.ident.clone(), text)?;
+        Ok(())
+    }
+
+    pub fn remove_labelling_comment(&self, comment: Comment) -> APIResult<()> {
+        self.api.delete_labeling_comment(self.ident.clone(), comment.identifier().clone())
+    }
+
+    #[inline(always)]
+    pub fn key(&self) -> APIResult<&String> {
+        self.data.key(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn summary(&self) -> APIResult<&String> {
+        self.data.summary(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn description(&self) -> APIResult<&String> {
+        self.data.description(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn comments(&self) -> APIResult<&Vec<String>> {
+        self.data.comments(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn status(&self) -> APIResult<&String> {
+        self.data.status(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn priority(&self) -> APIResult<&String> {
+        self.data.priority(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn resolution(&self) -> APIResult<&Option<String>> {
+        self.data.resolution(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn issue_type(&self) -> APIResult<&String> {
+        self.data.issue_type(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn issue_links(&self, loading_settings: IssueLoadingSettings) -> APIResult<Vec<Issue>> {
+        let ids = self.data.issue_links(&self.api)?;
+        let issues = loading_settings.load_issues(
+            self.api.clone(), ids.clone(), self.caching_policy
+        )?;
+        assert_eq!(issues.len(), ids.len(), "Failed to retrieve all linked issues");
+        Ok(issues)
+    }
+
+    #[inline(always)]
+    pub fn parent(&self, loading_settings: IssueLoadingSettings) -> APIResult<Option<Issue>> {
+        if let Some(id) = self.data.parent(&self.api)? {
+            Ok(
+                Some(
+                    loading_settings.load_issue(self.api.clone(),
+                                                id.clone(),
+                                                self.caching_policy)?
+                )
+            )
+        } else {
+            Ok(None)
+        }
+    }
+
+    #[inline(always)]
+    pub fn subtasks(&self, loading_settings: IssueLoadingSettings) -> APIResult<Vec<Issue>> {
+        let ids = self.data.subtasks(&self.api)?;
+        let issues = loading_settings.load_issues(
+            self.api.clone(), ids.clone(), self.caching_policy
+        )?;
+        assert_eq!(issues.len(), ids.len(), "Failed to retrieve all subtasks");
+        Ok(issues)
+    }
+
+    #[inline(always)]
+    pub fn watches(&self) -> APIResult<u64> {
+        self.data.watches(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn votes(&self) -> APIResult<u64> {
+        self.data.votes(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn date_created(&self) -> APIResult<&String> {
+        self.data.date_created(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn date_updated(&self) -> APIResult<&String> {
+        self.data.date_updated(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn date_resolved(&self) -> APIResult<&Option<String>> {
+        self.data.date_resolved(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn labels(&self) -> APIResult<&Vec<String>> {
+        self.data.labels(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn components(&self) -> APIResult<&Vec<String>> {
+        self.data.components(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn affected_versions(&self) -> APIResult<&Vec<String>> {
+        self.data.affected_versions(&self.api)
+    }
+
+    #[inline(always)]
+    pub fn fix_versions(&self) -> APIResult<&Vec<String>> {
+        self.data.fix_versions(&self.api)
+    }
+}
```

### Comparing `issue_db_api-0.1.0/issue_db_api/src/labels.rs` & `issue_db_api-0.2.0/issue_db_api/src/labels.rs`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-#[allow(unused)]
-#[derive(Debug, Copy, Clone)]
-#[derive(Eq, PartialEq, Hash)]
-#[derive(serde::Serialize, serde::Deserialize)]
-pub struct Label {
-    executive: bool,
-    existence: bool,
-    property: bool
-}
-
-
-#[allow(unused)]
-impl Label {
-    pub fn new(existence: bool, executive: bool, property: bool) -> Self {
-        Label{existence, executive, property}
-    }
-
-    pub fn existence(&self) -> bool {
-        self.existence
-    }
-
-    pub fn executive(&self) -> bool {
-        self.executive
-    }
-
-    pub fn property(&self) -> bool {
-        self.property
-    }
-}
+#[allow(unused)]
+#[derive(Debug, Copy, Clone)]
+#[derive(Eq, PartialEq, Hash)]
+#[derive(serde::Serialize, serde::Deserialize)]
+pub struct Label {
+    executive: bool,
+    existence: bool,
+    property: bool
+}
+
+
+#[allow(unused)]
+impl Label {
+    pub fn new(existence: bool, executive: bool, property: bool) -> Self {
+        Label{existence, executive, property}
+    }
+
+    pub fn existence(&self) -> bool {
+        self.existence
+    }
+
+    pub fn executive(&self) -> bool {
+        self.executive
+    }
+
+    pub fn property(&self) -> bool {
+        self.property
+    }
+}
```

### Comparing `issue_db_api-0.1.0/issue_db_api/src/lib.rs` & `issue_db_api-0.2.0/issue_db_api/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -136,19 +136,26 @@
         authenticated: bool,
         repo: IssueRepository
     }
 
     #[pymethods]
     impl PyIssueRepository {
         #[new]
-        #[pyo3(signature=(url, *, credentials, label_caching_policy="no_caching", config_handling_policy="read_fetch_write_fetch"))]
+        #[pyo3(signature=(
+            url, *,
+            credentials,
+            label_caching_policy="no_caching",
+            config_handling_policy="read_fetch_write_fetch",
+            allow_self_signed_certificates=false
+        ))]
         fn __new__(url: String,
                    credentials: Option<(String, String)>,
                    label_caching_policy: &str,
-                   config_handling_policy: &str) -> PyResult<Self> {
+                   config_handling_policy: &str,
+                   allow_self_signed_certificates: bool) -> PyResult<Self> {
             let caching = match label_caching_policy {
                 "no_caching" => CachingPolicy::NoCaching,
                 "use_local_after_load" => CachingPolicy::UseLocalAfterLoad,
                 _ => {
                     let text = format!("Invalid caching policy: {}", label_caching_policy);
                     return Err(IssueAPIError::new_err(text));
                 }
@@ -164,22 +171,24 @@
             };
             let (repo, auth) = if let Some((username, password)) = credentials {
                 (
                     IssueRepository::new(url.clone(),
                                          username,
                                          password,
                                          caching,
-                                         config_handling),
+                                         config_handling,
+                                         allow_self_signed_certificates),
                     true
                 )
             } else {
                 (
                     IssueRepository::new_read_only(url.clone(),
                                                    caching,
-                                                   config_handling),
+                                                   config_handling,
+                                                   allow_self_signed_certificates),
                     false
                 )
             };
             Ok(Self{url, authenticated: auth, repo: api2py_error(repo)?})
         }
 
         fn __repr__(&self) -> PyResult<String> {
@@ -871,16 +880,16 @@
             let result = api2py_error(self.inner.model_versions())?;
             let converted = result.into_iter()
                 .map(|v| PyVersion{inner: v})
                 .collect();
             Ok(converted)
         }
 
-        fn add_version(&self, time: String, path: String) -> PyResult<PyVersion> {
-            let version = api2py_error(self.inner.upload_version(time, path))?;
+        fn add_version(&self, path: String, description: Option<String>) -> PyResult<PyVersion> {
+            let version = api2py_error(self.inner.upload_version(path, description))?;
             Ok(PyVersion{inner: version})
         }
 
         fn remove_version(&self, version: &PyVersion) -> PyResult<()> {
             api2py_error(self.inner.delete_version(version.inner.clone()))
         }
 
@@ -889,20 +898,20 @@
             let result = api2py_error(self.inner.model_runs())?;
             let converted = result.into_iter()
                 .map(|r| PyPerformance{inner: r})
                 .collect();
             Ok(converted)
         }
 
-        fn add_test_run(&self, data: Vec<&PyAny>) -> PyResult<PyPerformance> {
+        fn add_test_run(&self, data: Vec<&PyAny>, description: Option<String>) -> PyResult<PyPerformance> {
             let mut converted = Vec::with_capacity(data.len());
             for obj in data {
                 converted.push(py_to_json(obj)?);
             }
-            let run = api2py_error(self.inner.store_run(converted))?;
+            let run = api2py_error(self.inner.store_run(converted, description))?;
             Ok(PyPerformance{inner: run})
         }
 
         fn delete_test_run(&self, run: &PyPerformance) -> PyResult<()> {
             api2py_error(self.inner.delete_run(run.inner.clone()))
         }
     }
@@ -953,14 +962,24 @@
             }
             api2py_error(self.inner.store_predictions(converted))
         }
 
         fn delete_predictions(&self) -> PyResult<()> {
             api2py_error(self.inner.delete_predictions())
         }
+
+        #[getter]
+        pub fn description(&self) -> PyResult<String> {
+            Ok(self.inner.description())
+        }
+
+        #[setter]
+        pub fn set_description(&mut self, description: String) -> PyResult<()> {
+            api2py_error(self.inner.update_description(description))
+        }
     }
 
     #[pyclass(name="TestRun")]
     #[allow(unused)]
     struct PyPerformance {
         inner: TestRun
     }
@@ -979,14 +998,24 @@
             let result = api2py_error(self.inner.data())?;
             let mut converted = Vec::with_capacity(result.len());
             for fold in result {
                 converted.push(json_to_py(py, fold));
             }
             Ok(converted)
         }
+
+        #[getter]
+        pub fn description(&self) -> PyResult<String> {
+            Ok(self.inner.description())
+        }
+
+        #[setter]
+        pub fn set_description(&mut self, description: String) -> PyResult<()> {
+            api2py_error(self.inner.update_description(description))
+        }
     }
 
     #[pymodule]
     fn issue_api(py: Python<'_>, m: &PyModule) -> PyResult<()> {
         m.add("IssueAPIError", py.get_type::<IssueAPIError>())?;
         m.add_class::<PyIssueRepository>()?;
         m.add_class::<PyIssue>()?;
```

### Comparing `issue_db_api-0.1.0/issue_db_api/src/repository.rs` & `issue_db_api-0.2.0/issue_db_api/src/repository.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,168 +1,170 @@
-use std::collections::HashMap;
-use std::sync::Arc;
-use serde_json::Value;
-
-use crate::api_core::IssueAPI;
-use crate::config::{CachingPolicy, IssueLoadingSettings, ConfigHandlingPolicy};
-use crate::embedding::Embedding;
-use crate::issues::Issue;
-use crate::models::Model;
-use crate::query::Query;
-use crate::tags::Tag;
-use crate::util::APIResult;
-
-
-#[allow(unused)]
-#[derive(Debug)]
-pub struct IssueRepository {
-    label_caching: CachingPolicy,
-    config_handling: ConfigHandlingPolicy,
-    api: Arc<IssueAPI>
-}
-
-
-#[allow(unused)]
-impl IssueRepository {
-    pub fn new_read_only(url: String,
-                         label_caching_policy: CachingPolicy,
-                         config_handling_policy: ConfigHandlingPolicy) -> APIResult<Self> {
-        Ok(
-            Self{
-                api: Arc::new(IssueAPI::new_read_only(url)),
-                label_caching: label_caching_policy,
-                config_handling: config_handling_policy
-            }
-        )
-    }
-
-    pub fn new(url: String,
-               username: String,
-               password: String,
-               label_caching_policy: CachingPolicy,
-               config_handling_policy: ConfigHandlingPolicy) -> APIResult<Self> {
-        let api = Arc::new(IssueAPI::new(url, username, password)?);
-        Ok(
-            Self{
-                api,
-                label_caching: label_caching_policy,
-                config_handling: config_handling_policy
-            }
-        )
-    }
-
-    pub fn search(&self,
-                  query: Query,
-                  issue_loading_settings: IssueLoadingSettings) -> APIResult<Vec<Issue>> {
-        let ids = self.api.search(query)?;
-        issue_loading_settings.load_issues(self.api.clone(),
-                                           ids,
-                                           self.label_caching)
-    }
-
-    pub fn find_issue_by_key(&self,
-                             project: String,
-                             name: String,
-                             loading: IssueLoadingSettings) -> APIResult<Issue> {
-        let id = self.api.find_issue_id_by_key(project, name)?;
-        loading.load_issue(self.api.clone(), id, self.label_caching)
-    }
-
-    pub fn find_issues_by_key(&self,
-                              issues: Vec<(String, String)>,
-                              loading: IssueLoadingSettings) -> APIResult<Vec<Issue>> {
-        let ids = self.api.find_issue_ids_by_keys(issues)?;
-        loading.load_issues(self.api.clone(), ids, self.label_caching)
-    }
-
-    pub fn repos(&self) -> APIResult<Vec<IssueRepo>> {
-        let repos = self.api.get_all_repos()?
-            .into_iter()
-            .map(|name| IssueRepo{name, api: self.api.clone()})
-            .collect();
-        Ok(repos)
-    }
-
-    pub fn tags(&self) -> APIResult<Vec<Tag>> {
-        let tags = self.api.get_all_tags()?
-            .into_iter()
-            .map(|t| t.into_bound_tag(self.api.clone()))
-            .collect();
-        Ok(tags)
-    }
-
-    pub fn add_new_tag(&self, name: String, description: String) -> APIResult<()> {
-        self.api.register_new_tag(name, description)
-    }
-
-    pub fn bulk_add_tags(&self, tags: HashMap<&Issue, Vec<String>>) -> APIResult<()> {
-        let payload = tags.into_iter()
-            .map(|(k, v)| (k.ident().clone(), v))
-            .collect();
-        self.api.bulk_add_tags(payload)
-    }
-
-    pub fn embeddings(&self) -> APIResult<Vec<Embedding>> {
-        let embeddings = self.api.get_all_embeddings()?
-            .into_iter()
-            .map(|e| e.into_bound_embedding(self.api.clone(), self.config_handling))
-            .collect();
-        Ok(embeddings)
-    }
-
-    pub fn create_embedding(&self,
-                            name: String,
-                            config: HashMap<String, Value>) -> APIResult<Embedding> {
-        let id = self.api.create_embedding(name.clone(), config.clone())?;
-        let embedding = Embedding::new(
-            self.api.clone(),
-            id,
-            name,
-            config,
-            false,
-            self.config_handling
-        );
-        Ok(embedding)
-    }
-
-    pub fn models(&self) -> APIResult<Vec<Model>> {
-        let models = self.api.get_all_models()?;
-        let converted = models
-            .into_iter()
-            .map(|m|
-                Model::new(self.api.clone(),
-                           m.model_id,
-                           m.model_name,
-                           None,
-                           self.config_handling)
-            ).collect();
-        Ok(converted)
-    }
-
-    pub fn add_model(&self, name: String, config: HashMap<String, Value>) -> APIResult<Model> {
-        let id = self.api.create_model_config(name.clone(), config.clone())?;
-        let m = Model::new(
-            self.api.clone(),
-            id,
-            name,
-            Some(config),
-            self.config_handling
-        );
-        Ok(m)
-    }
-}
-
-
-pub struct IssueRepo {
-    name: String,
-    api: Arc<IssueAPI>
-}
-
-impl IssueRepo {
-    pub fn name(&self) -> &String {
-        &self.name 
-    }
-    
-    pub fn projects(&self) -> APIResult<Vec<String>> {
-        self.api.get_projects_for_repo(self.name.clone())
-    }
+use std::collections::HashMap;
+use std::sync::Arc;
+use serde_json::Value;
+
+use crate::api_core::IssueAPI;
+use crate::config::{CachingPolicy, IssueLoadingSettings, ConfigHandlingPolicy};
+use crate::embedding::Embedding;
+use crate::issues::Issue;
+use crate::models::Model;
+use crate::query::Query;
+use crate::tags::Tag;
+use crate::util::APIResult;
+
+
+#[allow(unused)]
+#[derive(Debug)]
+pub struct IssueRepository {
+    label_caching: CachingPolicy,
+    config_handling: ConfigHandlingPolicy,
+    api: Arc<IssueAPI>
+}
+
+
+#[allow(unused)]
+impl IssueRepository {
+    pub fn new_read_only(url: String,
+                         label_caching_policy: CachingPolicy,
+                         config_handling_policy: ConfigHandlingPolicy,
+                         allow_self_signed_certs: bool) -> APIResult<Self> {
+        Ok(
+            Self{
+                api: Arc::new(IssueAPI::new_read_only(url, allow_self_signed_certs)?),
+                label_caching: label_caching_policy,
+                config_handling: config_handling_policy
+            }
+        )
+    }
+
+    pub fn new(url: String,
+               username: String,
+               password: String,
+               label_caching_policy: CachingPolicy,
+               config_handling_policy: ConfigHandlingPolicy,
+               allow_self_signed_certs: bool) -> APIResult<Self> {
+        let api = Arc::new(IssueAPI::new(url, username, password, allow_self_signed_certs)?);
+        Ok(
+            Self{
+                api,
+                label_caching: label_caching_policy,
+                config_handling: config_handling_policy
+            }
+        )
+    }
+
+    pub fn search(&self,
+                  query: Query,
+                  issue_loading_settings: IssueLoadingSettings) -> APIResult<Vec<Issue>> {
+        let ids = self.api.search(query)?;
+        issue_loading_settings.load_issues(self.api.clone(),
+                                           ids,
+                                           self.label_caching)
+    }
+
+    pub fn find_issue_by_key(&self,
+                             project: String,
+                             name: String,
+                             loading: IssueLoadingSettings) -> APIResult<Issue> {
+        let id = self.api.find_issue_id_by_key(project, name)?;
+        loading.load_issue(self.api.clone(), id, self.label_caching)
+    }
+
+    pub fn find_issues_by_key(&self,
+                              issues: Vec<(String, String)>,
+                              loading: IssueLoadingSettings) -> APIResult<Vec<Issue>> {
+        let ids = self.api.find_issue_ids_by_keys(issues)?;
+        loading.load_issues(self.api.clone(), ids, self.label_caching)
+    }
+
+    pub fn repos(&self) -> APIResult<Vec<IssueRepo>> {
+        let repos = self.api.get_all_repos()?
+            .into_iter()
+            .map(|name| IssueRepo{name, api: self.api.clone()})
+            .collect();
+        Ok(repos)
+    }
+
+    pub fn tags(&self) -> APIResult<Vec<Tag>> {
+        let tags = self.api.get_all_tags()?
+            .into_iter()
+            .map(|t| t.into_bound_tag(self.api.clone()))
+            .collect();
+        Ok(tags)
+    }
+
+    pub fn add_new_tag(&self, name: String, description: String) -> APIResult<()> {
+        self.api.register_new_tag(name, description)
+    }
+
+    pub fn bulk_add_tags(&self, tags: HashMap<&Issue, Vec<String>>) -> APIResult<()> {
+        let payload = tags.into_iter()
+            .map(|(k, v)| (k.ident().clone(), v))
+            .collect();
+        self.api.bulk_add_tags(payload)
+    }
+
+    pub fn embeddings(&self) -> APIResult<Vec<Embedding>> {
+        let embeddings = self.api.get_all_embeddings()?
+            .into_iter()
+            .map(|e| e.into_bound_embedding(self.api.clone(), self.config_handling))
+            .collect();
+        Ok(embeddings)
+    }
+
+    pub fn create_embedding(&self,
+                            name: String,
+                            config: HashMap<String, Value>) -> APIResult<Embedding> {
+        let id = self.api.create_embedding(name.clone(), config.clone())?;
+        let embedding = Embedding::new(
+            self.api.clone(),
+            id,
+            name,
+            config,
+            false,
+            self.config_handling
+        );
+        Ok(embedding)
+    }
+
+    pub fn models(&self) -> APIResult<Vec<Model>> {
+        let models = self.api.get_all_models()?;
+        let converted = models
+            .into_iter()
+            .map(|m|
+                Model::new(self.api.clone(),
+                           m.model_id,
+                           m.model_name,
+                           None,
+                           self.config_handling)
+            ).collect();
+        Ok(converted)
+    }
+
+    pub fn add_model(&self, name: String, config: HashMap<String, Value>) -> APIResult<Model> {
+        let id = self.api.create_model_config(name.clone(), config.clone())?;
+        let m = Model::new(
+            self.api.clone(),
+            id,
+            name,
+            Some(config),
+            self.config_handling
+        );
+        Ok(m)
+    }
+}
+
+
+pub struct IssueRepo {
+    name: String,
+    api: Arc<IssueAPI>
+}
+
+impl IssueRepo {
+    pub fn name(&self) -> &String {
+        &self.name 
+    }
+    
+    pub fn projects(&self) -> APIResult<Vec<String>> {
+        self.api.get_projects_for_repo(self.name.clone())
+    }
 }
```

### Comparing `issue_db_api-0.1.0/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.2.0/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-use serde_json::Value;
-
-fn deserialize_some<'de, T, D>(deserializer: D) -> Result<Option<T>, D::Error>
-    where T: serde::Deserialize<'de>,
-          D: serde::Deserializer<'de>
-{
-    serde::Deserialize::deserialize(deserializer).map(Some)
-}
-
-
-
-#[allow(unused)]
-#[derive(Debug, serde::Deserialize)]
-pub struct RawPriority {
-    #[serde(rename(deserialize = "self"))] pub self_: String,
-    #[serde(rename(deserialize = "iconUrl"))] pub icon_url: String,
-    pub name: String,
-    pub id: String
-}
-
-#[allow(unused)]
-#[derive(Debug, serde::Deserialize)]
-pub struct RawVersion {
-    #[serde(rename(deserialize = "self"))] pub self_: String,
-    pub name: String,
-    pub id: String,
-    pub archived: bool,
-    pub released: bool,
-    #[serde(rename(deserialize = "releaseDate"))] pub release_date: String
-}
-
-#[allow(unused)]
-#[derive(Debug, serde::Deserialize)]
-pub struct RawStatus {
-    #[serde(rename(deserialize = "self"))] pub self_: String,
-    #[serde(rename(deserialize = "iconUrl"))] pub icon_url: String,
-    pub description: String,
-    pub name: String,
-    pub id: String,
-    #[serde(rename(deserialize = "statusCategory"))] pub category: Value
-}
-
-#[allow(unused)]
-#[derive(Debug, serde::Deserialize)]
-pub struct RawComponent {
-    #[serde(rename(deserialize = "self"))] pub self_: String,
-    pub id: String,
-    pub name: String,
-}
-
-#[allow(unused)]
-#[derive(Debug, serde::Deserialize)]
-pub struct RawVotes {
-    #[serde(rename(deserialize = "self"))] pub self_: String,
-    pub votes: u64,
-    #[serde(rename(deserialize = "hasVoted"))] pub has_voted: bool
-}
-
-#[allow(unused)]
-#[derive(Debug, serde::Deserialize)]
-pub struct RawIssueType {
-    #[serde(rename(deserialize = "self"))] pub self_: String,
-    pub id: String,
-    pub description: String,
-    #[serde(rename(deserialize = "iconUrl"))] pub icon_url: String,
-    pub name: String,
-    pub subtask: bool,
-    #[serde(rename(deserialize = "avatarId"))] pub avatar_id: u64
-}
-
-#[allow(unused)]
-#[derive(Debug, serde::Deserialize)]
-pub struct RawWatches {
-    #[serde(rename(deserialize = "self"))] pub self_: String,
-    #[serde(rename(deserialize = "watchCount"))] pub watch_count: u64,
-    #[serde(rename(deserialize = "isWatching"))] pub is_watching: bool
-}
-
-#[allow(unused)]
-#[derive(Debug, serde::Deserialize)]
-pub struct RawResolution {
-    #[serde(rename(deserialize = "self"))] pub self_: String,
-    pub id: String,
-    pub description: String,
-    pub name: String
-}
-
-#[allow(unused)]
-#[derive(Debug, serde::Deserialize)]
-pub struct RawIssueLinkDescription {
-    pub id: String,
-    pub name: String,
-    pub inward: String,
-    pub outward: String,
-    #[serde(rename(deserialize = "self"))] pub self_: String,
-}
-
-#[allow(unused)]
-#[derive(Debug, serde::Deserialize)]
-pub struct RawComment {
-    #[serde(rename(deserialize = "self"))] pub self_: String,
-    pub id: String,
-    pub author: Value,
-    #[serde(rename(deserialize = "updateAuthor"))] pub update_author: Value,
-    pub created: String,
-    pub updated: String,
-    pub body: String
-}
-
-#[allow(unused)]
-#[derive(Debug, serde::Deserialize)]
-pub enum RawIssueLink {
-    InwardIssue{
-        #[serde(rename(deserialize = "self"))] self_: String,
-        id: String,
-        #[serde(rename(deserialize = "type"))] type_: RawIssueLinkDescription,
-        #[serde(rename(deserialize = "inwardIssue"))] inward_issue: String
-    },
-    OutWardIssue{
-        #[serde(rename(deserialize = "self"))] self_: String,
-        id: String,
-        #[serde(rename(deserialize = "type"))] type_: RawIssueLinkDescription,
-        #[serde(rename(deserialize = "outwardIssue"))] outward_issue: String
-    }
-}
-
-
-#[allow(unused)]
-#[derive(Debug, serde::Deserialize, Default)]
-pub struct RawIssueData {
-    #[serde(default)] pub key: Option<String>,
-    #[serde(default)] pub summary: Option<String>,
-    #[serde(default)] pub description: Option<String>,
-    #[serde(default)] pub comments: Option<Vec<RawComment>>,
-    #[serde(default)] pub status: Option<RawStatus>,
-    #[serde(default)] pub priority: Option<RawPriority>,
-    #[serde(default, deserialize_with = "deserialize_some")] pub resolution: Option<Option<RawResolution>>,
-    #[serde(default)] pub issuetype: Option<RawIssueType>,
-    #[serde(default)] pub issuelinks: Option<Vec<RawIssueLink>>,
-    #[serde(default, deserialize_with = "deserialize_some")] pub parent: Option<Option<String>>,
-    #[serde(default)] pub subtasks: Option<Vec<String>>,
-    #[serde(default)] pub watches: Option<RawWatches>,
-    #[serde(default)] pub votes: Option<RawVotes>,
-    #[serde(default)] pub created: Option<String>,
-    #[serde(default)] pub updated: Option<String>,
-    #[serde(default, deserialize_with = "deserialize_some")] pub resolutiondate: Option<Option<String>>,
-    #[serde(default)] pub labels: Option<Vec<String>>,
-    #[serde(default)] pub components: Option<Vec<RawComponent>>,
-    #[serde(default)] pub versions: Option<Vec<RawVersion>>,
-    #[serde(default, rename(deserialize = "fixVersions"))] pub fix_versions: Option<Vec<RawVersion>>
-}
+use serde_json::Value;
+
+fn deserialize_some<'de, T, D>(deserializer: D) -> Result<Option<T>, D::Error>
+    where T: serde::Deserialize<'de>,
+          D: serde::Deserializer<'de>
+{
+    serde::Deserialize::deserialize(deserializer).map(Some)
+}
+
+
+
+#[allow(unused)]
+#[derive(Debug, serde::Deserialize)]
+pub struct RawPriority {
+    #[serde(rename(deserialize = "self"))] pub self_: String,
+    #[serde(rename(deserialize = "iconUrl"))] pub icon_url: String,
+    pub name: String,
+    pub id: String
+}
+
+#[allow(unused)]
+#[derive(Debug, serde::Deserialize)]
+pub struct RawVersion {
+    #[serde(rename(deserialize = "self"))] pub self_: String,
+    pub name: String,
+    pub id: String,
+    pub archived: bool,
+    pub released: bool,
+    #[serde(rename(deserialize = "releaseDate"))] pub release_date: String
+}
+
+#[allow(unused)]
+#[derive(Debug, serde::Deserialize)]
+pub struct RawStatus {
+    #[serde(rename(deserialize = "self"))] pub self_: String,
+    #[serde(rename(deserialize = "iconUrl"))] pub icon_url: String,
+    pub description: String,
+    pub name: String,
+    pub id: String,
+    #[serde(rename(deserialize = "statusCategory"))] pub category: Value
+}
+
+#[allow(unused)]
+#[derive(Debug, serde::Deserialize)]
+pub struct RawComponent {
+    #[serde(rename(deserialize = "self"))] pub self_: String,
+    pub id: String,
+    pub name: String,
+}
+
+#[allow(unused)]
+#[derive(Debug, serde::Deserialize)]
+pub struct RawVotes {
+    #[serde(rename(deserialize = "self"))] pub self_: String,
+    pub votes: u64,
+    #[serde(rename(deserialize = "hasVoted"))] pub has_voted: bool
+}
+
+#[allow(unused)]
+#[derive(Debug, serde::Deserialize)]
+pub struct RawIssueType {
+    #[serde(rename(deserialize = "self"))] pub self_: String,
+    pub id: String,
+    pub description: String,
+    #[serde(rename(deserialize = "iconUrl"))] pub icon_url: String,
+    pub name: String,
+    pub subtask: bool,
+    #[serde(rename(deserialize = "avatarId"))] pub avatar_id: u64
+}
+
+#[allow(unused)]
+#[derive(Debug, serde::Deserialize)]
+pub struct RawWatches {
+    #[serde(rename(deserialize = "self"))] pub self_: String,
+    #[serde(rename(deserialize = "watchCount"))] pub watch_count: u64,
+    #[serde(rename(deserialize = "isWatching"))] pub is_watching: bool
+}
+
+#[allow(unused)]
+#[derive(Debug, serde::Deserialize)]
+pub struct RawResolution {
+    #[serde(rename(deserialize = "self"))] pub self_: String,
+    pub id: String,
+    pub description: String,
+    pub name: String
+}
+
+#[allow(unused)]
+#[derive(Debug, serde::Deserialize)]
+pub struct RawIssueLinkDescription {
+    pub id: String,
+    pub name: String,
+    pub inward: String,
+    pub outward: String,
+    #[serde(rename(deserialize = "self"))] pub self_: String,
+}
+
+#[allow(unused)]
+#[derive(Debug, serde::Deserialize)]
+pub struct RawComment {
+    #[serde(rename(deserialize = "self"))] pub self_: String,
+    pub id: String,
+    pub author: Value,
+    #[serde(rename(deserialize = "updateAuthor"))] pub update_author: Value,
+    pub created: String,
+    pub updated: String,
+    pub body: String
+}
+
+#[allow(unused)]
+#[derive(Debug, serde::Deserialize)]
+pub enum RawIssueLink {
+    InwardIssue{
+        #[serde(rename(deserialize = "self"))] self_: String,
+        id: String,
+        #[serde(rename(deserialize = "type"))] type_: RawIssueLinkDescription,
+        #[serde(rename(deserialize = "inwardIssue"))] inward_issue: String
+    },
+    OutWardIssue{
+        #[serde(rename(deserialize = "self"))] self_: String,
+        id: String,
+        #[serde(rename(deserialize = "type"))] type_: RawIssueLinkDescription,
+        #[serde(rename(deserialize = "outwardIssue"))] outward_issue: String
+    }
+}
+
+
+#[allow(unused)]
+#[derive(Debug, serde::Deserialize, Default)]
+pub struct RawIssueData {
+    #[serde(default)] pub key: Option<String>,
+    #[serde(default)] pub summary: Option<String>,
+    #[serde(default)] pub description: Option<String>,
+    #[serde(default)] pub comments: Option<Vec<RawComment>>,
+    #[serde(default)] pub status: Option<RawStatus>,
+    #[serde(default)] pub priority: Option<RawPriority>,
+    #[serde(default, deserialize_with = "deserialize_some")] pub resolution: Option<Option<RawResolution>>,
+    #[serde(default)] pub issuetype: Option<RawIssueType>,
+    #[serde(default)] pub issuelinks: Option<Vec<RawIssueLink>>,
+    #[serde(default, deserialize_with = "deserialize_some")] pub parent: Option<Option<String>>,
+    #[serde(default)] pub subtasks: Option<Vec<String>>,
+    #[serde(default)] pub watches: Option<RawWatches>,
+    #[serde(default)] pub votes: Option<RawVotes>,
+    #[serde(default)] pub created: Option<String>,
+    #[serde(default)] pub updated: Option<String>,
+    #[serde(default, deserialize_with = "deserialize_some")] pub resolutiondate: Option<Option<String>>,
+    #[serde(default)] pub labels: Option<Vec<String>>,
+    #[serde(default)] pub components: Option<Vec<RawComponent>>,
+    #[serde(default)] pub versions: Option<Vec<RawVersion>>,
+    #[serde(default, rename(deserialize = "fixVersions"))] pub fix_versions: Option<Vec<RawVersion>>
+}
```

### Comparing `issue_db_api-0.1.0/issue_db_api/src/tags.rs` & `issue_db_api-0.2.0/issue_db_api/src/tags.rs`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-use std::hash::{Hash, Hasher};
-use std::sync::Arc;
-use crate::api_core::IssueAPI;
-use crate::APIResult;
-
-#[allow(unused)]
-#[derive(Debug, Clone, Copy, serde::Deserialize)]
-pub enum TagType {
-    #[serde(rename="author")] Author,
-    #[serde(rename="project")] Project,
-    #[serde(rename="manual-tag")] Custom
-}
-
-#[allow(unused)]
-#[derive(Debug, Clone, serde::Deserialize)]
-pub(crate) struct UnboundTag {
-    pub(crate) name: String,
-    pub(crate) description: String,
-    #[serde(rename(deserialize="type"))] pub(crate) tag_type: TagType
-}
-
-impl UnboundTag {
-    pub(crate) fn into_bound_tag(self, api: Arc<IssueAPI>) -> Tag {
-        Tag{
-            api,
-            name: self.name,
-            description: self.description,
-            tag_type: self.tag_type
-        }
-    }
-}
-
-#[allow(unused)]
-#[derive(Debug, Clone)]
-pub struct Tag {
-    api: Arc<IssueAPI>,
-    name: String,
-    description: String,
-    tag_type: TagType
-}
-
-impl PartialEq for Tag {
-    fn eq(&self, other: &Self) -> bool {
-        self.name == other.name
-    }
-}
-
-impl Eq for Tag {}
-
-impl Hash for Tag {
-    fn hash<H: Hasher>(&self, state: &mut H) {
-        self.name.hash(state)
-    }
-}
-
-#[allow(unused)]
-impl Tag {
-    pub fn name(&self) -> &String {
-        &self.name
-    }
-
-    pub fn description(&self) -> &String {
-        &self.description
-    }
-
-    pub fn update_description(&mut self, description: String) -> APIResult<()> {
-        self.api.update_tag(self.name.clone(), description.clone())?;
-        self.description = description;
-        Ok(())
-    }
-
-    pub fn tag_type(&self) -> TagType {
-        self.tag_type
-    }
-}
+use std::hash::{Hash, Hasher};
+use std::sync::Arc;
+use crate::api_core::IssueAPI;
+use crate::APIResult;
+
+#[allow(unused)]
+#[derive(Debug, Clone, Copy, serde::Deserialize)]
+pub enum TagType {
+    #[serde(rename="author")] Author,
+    #[serde(rename="project")] Project,
+    #[serde(rename="manual-tag")] Custom
+}
+
+#[allow(unused)]
+#[derive(Debug, Clone, serde::Deserialize)]
+pub(crate) struct UnboundTag {
+    pub(crate) name: String,
+    pub(crate) description: String,
+    #[serde(rename(deserialize="type"))] pub(crate) tag_type: TagType
+}
+
+impl UnboundTag {
+    pub(crate) fn into_bound_tag(self, api: Arc<IssueAPI>) -> Tag {
+        Tag{
+            api,
+            name: self.name,
+            description: self.description,
+            tag_type: self.tag_type
+        }
+    }
+}
+
+#[allow(unused)]
+#[derive(Debug, Clone)]
+pub struct Tag {
+    api: Arc<IssueAPI>,
+    name: String,
+    description: String,
+    tag_type: TagType
+}
+
+impl PartialEq for Tag {
+    fn eq(&self, other: &Self) -> bool {
+        self.name == other.name
+    }
+}
+
+impl Eq for Tag {}
+
+impl Hash for Tag {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.name.hash(state)
+    }
+}
+
+#[allow(unused)]
+impl Tag {
+    pub fn name(&self) -> &String {
+        &self.name
+    }
+
+    pub fn description(&self) -> &String {
+        &self.description
+    }
+
+    pub fn update_description(&mut self, description: String) -> APIResult<()> {
+        self.api.update_tag(self.name.clone(), description.clone())?;
+        self.description = description;
+        Ok(())
+    }
+
+    pub fn tag_type(&self) -> TagType {
+        self.tag_type
+    }
+}
```

### Comparing `issue_db_api-0.1.0/issue_db_api/src/util.rs` & `issue_db_api-0.2.0/issue_db_api/src/util.rs`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-use std::sync::atomic::{AtomicBool, Ordering};
-use std::sync::{RwLock};
-
-pub type APIResult<T> = Result<T, Box<dyn std::error::Error>>;
-
-
-macro_rules! initialize_lazy_field {
-    ($e:expr) => {
-        {
-            let value: Option<_> = $e;
-            let lazy = lazy_init::Lazy::new();
-            if let Some(x) = value {
-                let _ = lazy.get_or_create(|| x);
-            }
-            lazy
-        }
-    }
-}
-
-
-pub(crate) use initialize_lazy_field;
-
-
-#[allow(unused)]
-#[derive(Debug)]
-struct CacheLockError {}
-
-impl std::fmt::Display for CacheLockError {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        write!(f, "Poisoned lock in cache. Cannot recover.")
-    }
-}
-
-impl std::error::Error for CacheLockError {
-    fn source(&self) -> Option<&(dyn std::error::Error + 'static)> {
-        None
-    }
-}
-
-
-#[derive(Debug)]
-pub struct CacheContainer<T: Clone> {
-    value: RwLock<Option<T>>,
-    dirty: AtomicBool
-}
-
-
-impl<T: Clone> CacheContainer<T> {
-    pub fn new(initial: Option<T>) -> Self {
-        CacheContainer{
-            value: RwLock::new(initial),
-            dirty: AtomicBool::new(true)
-        }
-    }
-
-    pub fn get<F: FnOnce() -> APIResult<T>>(&self, f: F) -> APIResult<T> {
-        let obj = self.value
-            .read()
-            .map_err(|_| Box::new(CacheLockError{}))?;
-        if obj.is_some() && !self.dirty.load(Ordering::Acquire) {
-            Ok(obj.clone().unwrap())
-        } else {
-            drop(obj);    // unlock
-            // First, acquire the write lock
-            let mut obj = self.value
-                .write()
-                .map_err(|_| Box::new(CacheLockError{}))?;
-            // With the write lock in hand, check if another thread
-            // updated the object in the meantime.
-            if self.dirty.load(Ordering::Relaxed) && obj.is_none() {
-                let inner = (f)()?;
-                let _ = obj.insert(inner.clone());
-                Ok(inner)
-            } else {
-                // Another thread updated the object; use a recursive
-                // call to fetch it.
-                self.get(f)
-            }
-        }
-    }
-
-    pub fn set(&self, value: T) -> APIResult<()> {
-        let mut obj = self.value
-            .write()
-            .map_err(|_| Box::new(CacheLockError{}))?;
-        let _ = obj.insert(value);
-        Ok(())
-    }
-
-    pub fn invalidate(&self) {
-        self.dirty.store(true, Ordering::Release);
-    }
+use std::sync::atomic::{AtomicBool, Ordering};
+use std::sync::{RwLock};
+
+pub type APIResult<T> = Result<T, Box<dyn std::error::Error>>;
+
+
+macro_rules! initialize_lazy_field {
+    ($e:expr) => {
+        {
+            let value: Option<_> = $e;
+            let lazy = lazy_init::Lazy::new();
+            if let Some(x) = value {
+                let _ = lazy.get_or_create(|| x);
+            }
+            lazy
+        }
+    }
+}
+
+
+pub(crate) use initialize_lazy_field;
+
+
+#[allow(unused)]
+#[derive(Debug)]
+struct CacheLockError {}
+
+impl std::fmt::Display for CacheLockError {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        write!(f, "Poisoned lock in cache. Cannot recover.")
+    }
+}
+
+impl std::error::Error for CacheLockError {
+    fn source(&self) -> Option<&(dyn std::error::Error + 'static)> {
+        None
+    }
+}
+
+
+#[derive(Debug)]
+pub struct CacheContainer<T: Clone> {
+    value: RwLock<Option<T>>,
+    dirty: AtomicBool
+}
+
+
+impl<T: Clone> CacheContainer<T> {
+    pub fn new(initial: Option<T>) -> Self {
+        CacheContainer{
+            value: RwLock::new(initial),
+            dirty: AtomicBool::new(true)
+        }
+    }
+
+    pub fn get<F: FnOnce() -> APIResult<T>>(&self, f: F) -> APIResult<T> {
+        let obj = self.value
+            .read()
+            .map_err(|_| Box::new(CacheLockError{}))?;
+        if obj.is_some() && !self.dirty.load(Ordering::Acquire) {
+            Ok(obj.clone().unwrap())
+        } else {
+            drop(obj);    // unlock
+            // First, acquire the write lock
+            let mut obj = self.value
+                .write()
+                .map_err(|_| Box::new(CacheLockError{}))?;
+            // With the write lock in hand, check if another thread
+            // updated the object in the meantime.
+            if self.dirty.load(Ordering::Relaxed) && obj.is_none() {
+                let inner = (f)()?;
+                let _ = obj.insert(inner.clone());
+                Ok(inner)
+            } else {
+                // Another thread updated the object; use a recursive
+                // call to fetch it.
+                self.get(f)
+            }
+        }
+    }
+
+    pub fn set(&self, value: T) -> APIResult<()> {
+        let mut obj = self.value
+            .write()
+            .map_err(|_| Box::new(CacheLockError{}))?;
+        let _ = obj.insert(value);
+        Ok(())
+    }
+
+    pub fn invalidate(&self) {
+        self.dirty.store(true, Ordering::Release);
+    }
 }
```

### Comparing `issue_db_api-0.1.0/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.2.0/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.1.0/pyproject.toml` & `issue_db_api-0.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-[build-system]
-requires = ["setuptools", "setuptools-scm", "wheel", "setuptools-rust"]
-build-backend = "setuptools.build_meta"
-
-[tool.setuptools.packages.find]
-where=["."]
-include = ["issue_db_api"]
-
-[project]
-name = "issue_db_api"
-version = "0.1.0"
-authors = [
-    {name = "Jesse Maarleveld"},
-]
-readme = "README.md"
-requires-python = ">=3.10"
-classifiers = [
-    "Programming Language :: Rust",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
+[build-system]
+requires = ["setuptools", "setuptools-scm", "wheel", "setuptools-rust"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.packages.find]
+where=["."]
+include = ["issue_db_api"]
+
+[project]
+name = "issue_db_api"
+version = "0.2.0"
+authors = [
+    {name = "Jesse Maarleveld"},
+]
+readme = "README.md"
+requires-python = ">=3.10"
+classifiers = [
+    "Programming Language :: Rust",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
 ]
```

