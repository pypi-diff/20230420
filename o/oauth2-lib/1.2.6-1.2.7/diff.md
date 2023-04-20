# Comparing `tmp/oauth2-lib-1.2.6.tar.gz` & `tmp/oauth2-lib-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauth2-lib-1.2.6.tar", last modified: Tue Mar 28 08:00:37 2023, max compression
+gzip compressed data, was "oauth2-lib-1.2.7.tar", last modified: Thu Apr 20 12:49:38 2023, max compression
```

## Comparing `oauth2-lib-1.2.6.tar` & `oauth2-lib-1.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      363 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/.bumpversion.cfg
--rw-r--r--   0        0        0      550 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0      389 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/.github/workflows/pull-request.yml
--rw-r--r--   0        0        0     1894 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1518 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/.github/workflows/test-package.yml
--rw-r--r--   0        0        0     1103 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/.gitignore
--rw-r--r--   0        0        0     2066 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/LICENSE
--rw-r--r--   0        0        0     1051 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/README.md
--rwxr-xr-x   0        0        0      150 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/fmt_code.sh
--rw-r--r--   0        0        0      671 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/oauth2_lib/__init__.py
--rw-r--r--   0        0        0     5433 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/oauth2_lib/async_api_client.py
--rw-r--r--   0        0        0    15285 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/oauth2_lib/fastapi.py
--rw-r--r--   0        0        0        0 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/oauth2_lib/py.typed
--rw-r--r--   0        0        0     2392 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     1151 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/setup.cfg
--rw-r--r--   0        0        0        0 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/tests/__init__.py
--rw-r--r--   0        0        0      758 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/tests/conftest.py
--rw-r--r--   0        0        0    13749 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/tests/test_fastapi.py
--rw-r--r--   0        0        0     6570 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/tests/test_opa_decision.py
--rw-r--r--   0        0        0      474 2023-03-28 08:00:29.160975 oauth2-lib-1.2.6/tests/test_opa_graphql_decision.py
--rw-r--r--   0        0        0     3710 1970-01-01 00:00:00.000000 oauth2-lib-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0      363 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/.bumpversion.cfg
+-rw-r--r--   0        0        0      550 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0      389 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/.github/workflows/pull-request.yml
+-rw-r--r--   0        0        0     1894 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1518 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/.github/workflows/test-package.yml
+-rw-r--r--   0        0        0     1103 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/.gitignore
+-rw-r--r--   0        0        0     2066 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/LICENSE
+-rw-r--r--   0        0        0     1051 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/README.md
+-rwxr-xr-x   0        0        0      150 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/fmt_code.sh
+-rw-r--r--   0        0        0      671 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/oauth2_lib/__init__.py
+-rw-r--r--   0        0        0     7652 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/oauth2_lib/async_api_client.py
+-rw-r--r--   0        0        0    15285 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/oauth2_lib/fastapi.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/oauth2_lib/py.typed
+-rw-r--r--   0        0        0     2420 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1151 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/setup.cfg
+-rw-r--r--   0        0        0        0 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/tests/__init__.py
+-rw-r--r--   0        0        0      758 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/tests/conftest.py
+-rw-r--r--   0        0        0    13749 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/tests/test_fastapi.py
+-rw-r--r--   0        0        0     6570 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/tests/test_opa_decision.py
+-rw-r--r--   0        0        0      474 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/tests/test_opa_graphql_decision.py
+-rw-r--r--   0        0        0     3746 1970-01-01 00:00:00.000000 oauth2-lib-1.2.7/PKG-INFO
```

### Comparing `oauth2-lib-1.2.6/.github/workflows/publish-release.yml` & `oauth2-lib-1.2.7/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.6/.github/workflows/scheduled-build.yml` & `oauth2-lib-1.2.7/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.6/.github/workflows/test-package.yml` & `oauth2-lib-1.2.7/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.6/.gitignore` & `oauth2-lib-1.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.6/.pre-commit-config.yaml` & `oauth2-lib-1.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.6/LICENSE` & `oauth2-lib-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.6/README.md` & `oauth2-lib-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.6/oauth2_lib/__init__.py` & `oauth2-lib-1.2.7/oauth2_lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the SURF Oauth2 module that interfaces with the oauth2 setup."""
 
-__version__ = "1.2.6"
+__version__ = "1.2.7"
```

### Comparing `oauth2-lib-1.2.6/oauth2_lib/fastapi.py` & `oauth2-lib-1.2.7/oauth2_lib/fastapi.py`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.6/pyproject.toml` & `oauth2-lib-1.2.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "Programming Language :: Python :: 3.10",
 ]
 requires = [
     "requests>=2.19.0",
     "ruamel.yaml~=0.16.10",
     "structlog>=20.2.0",
     "fastapi>=0.90.1",
+    "opentelemetry-distro",
     "httpx[http2]==0.23.0",
     "authlib==1.0.1",
     "pydantic>=1.8.0",
 ]
 description-file = "README.md"
 requires-python = ">3.8"
```

### Comparing `oauth2-lib-1.2.6/setup.cfg` & `oauth2-lib-1.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.6/tests/conftest.py` & `oauth2-lib-1.2.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.6/tests/test_fastapi.py` & `oauth2-lib-1.2.7/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.6/tests/test_opa_decision.py` & `oauth2-lib-1.2.7/tests/test_opa_decision.py`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.6/PKG-INFO` & `oauth2-lib-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2-lib
-Version: 1.2.6
+Version: 1.2.7
 Summary: This is the SURF Oauth2 module that interfaces with the oauth2 setup.
 Home-page: https://github.com/workfloworchestrator/oauth2-lib
 Author: SURF
 Author-email: automation-beheer@surf.nl
 Requires-Python: >3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -25,14 +25,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: requests>=2.19.0
 Requires-Dist: ruamel.yaml~=0.16.10
 Requires-Dist: structlog>=20.2.0
 Requires-Dist: fastapi>=0.90.1
+Requires-Dist: opentelemetry-distro
 Requires-Dist: httpx[http2]==0.23.0
 Requires-Dist: authlib==1.0.1
 Requires-Dist: pydantic>=1.8.0
 Requires-Dist: bumpversion ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: apache-license-check ; extra == "test"
 Requires-Dist: black ; extra == "test"
```

