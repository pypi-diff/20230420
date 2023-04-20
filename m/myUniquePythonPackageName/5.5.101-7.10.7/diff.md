# Comparing `tmp/myUniquePythonPackageName-5.5.101.tar.gz` & `tmp/myUniquePythonPackageName-7.10.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myUniquePythonPackageName-5.5.101.tar", last modified: Thu Apr 20 07:31:46 2023, max compression
+gzip compressed data, was "myUniquePythonPackageName-7.10.7.tar", last modified: Fri Mar 31 12:05:44 2023, max compression
```

## Comparing `myUniquePythonPackageName-5.5.101.tar` & `myUniquePythonPackageName-7.10.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:31:46.772384 myUniquePythonPackageName-5.5.101/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      245 2023-04-20 07:31:46.772384 myUniquePythonPackageName-5.5.101/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2858 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:31:46.756384 myUniquePythonPackageName-5.5.101/apimaticcalculator/
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      561 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/apimaticcalculator_client.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:31:46.761384 myUniquePythonPackageName-5.5.101/apimaticcalculator/controllers/
--rw-r--r--   0 root         (0) root         (0)       75 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/controllers/simple_calculator_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:31:46.762384 myUniquePythonPackageName-5.5.101/apimaticcalculator/exceptions/
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:31:46.766384 myUniquePythonPackageName-5.5.101/apimaticcalculator/http/
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      480 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      487 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:31:46.768384 myUniquePythonPackageName-5.5.101/apimaticcalculator/models/
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/models/operation_type_enum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:31:46.769384 myUniquePythonPackageName-5.5.101/apimaticcalculator/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/apimaticcalculator/utilities/file_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:31:46.772384 myUniquePythonPackageName-5.5.101/myUniquePythonPackageName.egg-info/
--rw-r--r--   0 root         (0) root         (0)      245 2023-04-20 07:31:46.000000 myUniquePythonPackageName-5.5.101/myUniquePythonPackageName.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-20 07:31:46.000000 myUniquePythonPackageName-5.5.101/myUniquePythonPackageName.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 07:31:46.000000 myUniquePythonPackageName-5.5.101/myUniquePythonPackageName.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-04-20 07:31:46.000000 myUniquePythonPackageName-5.5.101/myUniquePythonPackageName.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-20 07:31:46.000000 myUniquePythonPackageName-5.5.101/myUniquePythonPackageName.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      593 2023-04-20 07:31:09.000000 myUniquePythonPackageName-5.5.101/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-20 07:31:46.773383 myUniquePythonPackageName-5.5.101/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.125621 myUniquePythonPackageName-7.10.7/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      244 2023-03-31 12:05:44.126621 myUniquePythonPackageName-7.10.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2602 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.102621 myUniquePythonPackageName-7.10.7/apimaticcalculator/
+-rw-r--r--   0 root         (0) root         (0)      156 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      561 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/apimaticcalculator_client.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.108621 myUniquePythonPackageName-7.10.7/apimaticcalculator/controllers/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/controllers/simple_calculator_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.111621 myUniquePythonPackageName-7.10.7/apimaticcalculator/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.115621 myUniquePythonPackageName-7.10.7/apimaticcalculator/http/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      480 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      487 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.117621 myUniquePythonPackageName-7.10.7/apimaticcalculator/models/
+-rw-r--r--   0 root         (0) root         (0)       42 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/models/operation_type_enum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.120621 myUniquePythonPackageName-7.10.7/apimaticcalculator/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.125621 myUniquePythonPackageName-7.10.7/myUniquePythonPackageName.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-03-31 12:05:44.000000 myUniquePythonPackageName-7.10.7/myUniquePythonPackageName.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-03-31 12:05:44.000000 myUniquePythonPackageName-7.10.7/myUniquePythonPackageName.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 12:05:44.000000 myUniquePythonPackageName-7.10.7/myUniquePythonPackageName.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2023-03-31 12:05:44.000000 myUniquePythonPackageName-7.10.7/myUniquePythonPackageName.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-03-31 12:05:44.000000 myUniquePythonPackageName-7.10.7/myUniquePythonPackageName.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      592 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-03-31 12:05:44.127621 myUniquePythonPackageName-7.10.7/setup.cfg
```

### Comparing `myUniquePythonPackageName-5.5.101/LICENSE` & `myUniquePythonPackageName-7.10.7/LICENSE`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.101/README.md` & `myUniquePythonPackageName-7.10.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 
 ## Introduction
 
 Simple calculator API hosted on APIMATIC
 
 ## Install the Package
 
-The package is compatible with Python versions `3 >=3.7, <= 3.11`.
+The package is compatible with Python versions `3 >=3.7, <= 3.10`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install myUniquePythonPackageName==5.5.101
+pip install myUniquePythonPackageName==7.10.7
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/myUniquePythonPackageName/5.5.101
+https://pypi.python.org/pypi/myUniquePythonPackageName/7.10.7
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
 ```
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://github.com/git-fudge/cSharpSourceCode/blob/5.5.101/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
@@ -46,22 +46,23 @@
 | `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
 | `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
 
 The API client can be initialized as follows:
 
 ```python
 from apimaticcalculator.apimaticcalculator_client import ApimaticcalculatorClient
-from apimaticcalculator.configuration import Environment
+from apimaticcalculator.configuration import Environment
 
-client = ApimaticcalculatorClient()
+client = ApimaticcalculatorClient(
+    environment=Environment.PRODUCTION,)
 ```
 
 ## List of APIs
 
-* [Simple Calculator](https://github.com/git-fudge/cSharpSourceCode/blob/5.5.101/doc/controllers/simple-calculator.md)
+* [Simple Calculator](doc/controllers/simple-calculator.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://github.com/git-fudge/cSharpSourceCode/blob/5.5.101/doc/utility-classes.md)
-* [HttpResponse](https://github.com/git-fudge/cSharpSourceCode/blob/5.5.101/doc/http-response.md)
-* [HttpRequest](https://github.com/git-fudge/cSharpSourceCode/blob/5.5.101/doc/http-request.md)
+* [Utility Classes](doc/utility-classes.md)
+* [HttpResponse](doc/http-response.md)
+* [HttpRequest](doc/http-request.md)
```

### Comparing `myUniquePythonPackageName-5.5.101/apimaticcalculator/api_helper.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/api_helper.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.101/apimaticcalculator/apimaticcalculator_client.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/apimaticcalculator_client.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.101/apimaticcalculator/configuration.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/configuration.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.101/apimaticcalculator/controllers/base_controller.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.101/apimaticcalculator/controllers/simple_calculator_controller.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/controllers/simple_calculator_controller.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.101/apimaticcalculator/exceptions/api_exception.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.101/apimaticcalculator/http/http_request.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/http/http_request.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.101/apimaticcalculator/http/http_response.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/http/http_response.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.101/apimaticcalculator/models/operation_type_enum.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/models/operation_type_enum.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.101/myUniquePythonPackageName.egg-info/SOURCES.txt` & `myUniquePythonPackageName-7.10.7/myUniquePythonPackageName.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.101/pyproject.toml` & `myUniquePythonPackageName-7.10.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "myUniquePythonPackageName"
 description = "Simple calculator API hosted on APIMATIC"
-version = "5.5.101"
+version = "7.10.7"
 requires-python = ">=3.7"
 keywords = []
 authors = [{name = "RandomPerson", email = "randomEmail@testing.com"}]
 urls = {}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10"]
 classifiers = []
 [project.optional-dependencies]
-testutils = ["pytest>=7.2.2"]
+testutils = ["pytest>=7.1.3"]
```

