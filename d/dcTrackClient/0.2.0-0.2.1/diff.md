# Comparing `tmp/dctrackclient-0.2.0.tar.gz` & `tmp/dctrackclient-0.2.1.tar.gz`

## Comparing `dctrackclient-0.2.0.tar` & `dctrackclient-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/.github/workflows/doc.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/LICENSE
--rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 dctrackclient-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0      466 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/.github/workflows/doc.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/README.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/PKG-INFO
```

### Comparing `dctrackclient-0.2.0/.github/workflows/python-publish.yml` & `dctrackclient-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.2.0/src/dcTrackClient/__init__.py` & `dctrackclient-0.2.1/src/dcTrackClient/__init__.py`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.2.0/LICENSE` & `dctrackclient-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.2.0/README.md` & `dctrackclient-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 - This example shows the minimum attributes required to create an item
 - See [the official documentation](#official-dctrack-documentation) for a comprehensive list of attributes
 - This function returns the JSON object for the newly created item
 - If it fails, the function will return a JSON object containing the error message
 
 ```py
-api.createItem({'cmbLocation': 'CRT > 2ND > IT', 'tiName': 'NEW-ITEM', 'cmbMake': 'Generic', 'cmbModel': 'Generic^Rackable^01'})
+api.createItem({'cmbLocation': 'SAMPLE LOCATION', 'tiName': 'NEW-ITEM', 'cmbMake': 'Generic', 'cmbModel': 'Generic^Rackable^01'})
 ```
 
 ### Retrieve item details:
 
 ```py
 item = api.getItem(1234)
 ```
@@ -64,15 +64,15 @@
 ```
 
 ## Official DcTrack Documentation
 
 Visit this link for the official documentation on request bodies and attrribute names.
 
 https://www.sunbirddcim.com/help/dcTrack/v900/API/en/Default.htm
-## Documentation
+## Module Documentation
 ### class Client:
 ```py
 def __init__(self, baseUrl: str, username: str = '', password: str = '', apiToken: str = ''):
 ```
 > Provide either a username and password, or an API token to access the dcTrack database with Python.
 ```py
 def createItem(self, data: dict, returnDetails: bool = True):
```

### Comparing `dctrackclient-0.2.0/pyproject.toml` & `dctrackclient-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.2.0/PKG-INFO` & `dctrackclient-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.2.0
+Version: 0.2.1
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -42,15 +42,15 @@
 
 - This example shows the minimum attributes required to create an item
 - See [the official documentation](#official-dctrack-documentation) for a comprehensive list of attributes
 - This function returns the JSON object for the newly created item
 - If it fails, the function will return a JSON object containing the error message
 
 ```py
-api.createItem({'cmbLocation': 'CRT > 2ND > IT', 'tiName': 'NEW-ITEM', 'cmbMake': 'Generic', 'cmbModel': 'Generic^Rackable^01'})
+api.createItem({'cmbLocation': 'SAMPLE LOCATION', 'tiName': 'NEW-ITEM', 'cmbMake': 'Generic', 'cmbModel': 'Generic^Rackable^01'})
 ```
 
 ### Retrieve item details:
 
 ```py
 item = api.getItem(1234)
 ```
@@ -78,15 +78,15 @@
 ```
 
 ## Official DcTrack Documentation
 
 Visit this link for the official documentation on request bodies and attrribute names.
 
 https://www.sunbirddcim.com/help/dcTrack/v900/API/en/Default.htm
-## Documentation
+## Module Documentation
 ### class Client:
 ```py
 def __init__(self, baseUrl: str, username: str = '', password: str = '', apiToken: str = ''):
 ```
 > Provide either a username and password, or an API token to access the dcTrack database with Python.
 ```py
 def createItem(self, data: dict, returnDetails: bool = True):
```

