# Comparing `tmp/package_kpengz-1.0.1.tar.gz` & `tmp/package_kpengz-1.0.2.tar.gz`

## Comparing `package_kpengz-1.0.1.tar` & `package_kpengz-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/.idea/mysql-functions.iml
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/src/package_kpengz/__init__.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/src/package_kpengz/constants.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/src/package_kpengz/functions.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/LICENSE
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/README.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 package_kpengz-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/.idea/mysql-functions.iml
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/src/package_kpengz/__init__.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/src/package_kpengz/constants.py
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/src/package_kpengz/functions.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/LICENSE
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/README.md
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 package_kpengz-1.0.2/PKG-INFO
```

### Comparing `package_kpengz-1.0.1/.idea/workspace.xml` & `package_kpengz-1.0.2/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `package_kpengz-1.0.1/src/package_kpengz/functions.py` & `package_kpengz-1.0.2/src/package_kpengz/functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,30 +6,34 @@
 logger = logging.getLogger()
 lambda_environment = os.environ.get('ENVIRONMENT', "DEV")
 logging_level = "INFO" if lambda_environment == "DEV" else "WARN"
 print("logging_level :" + logging_level)
 logger.setLevel(logging_level)
 logging.info("Initializing the  environment variables for the connection pool")
 
-db_name = os.environ.get(constants.ENVIRONMENT_VARIABLE_DB_NAME)
-db_port = os.environ.get(constants.ENVIRONMENT_VARIABLE_DB_PORT)
-db_username = os.environ.get(constants.ENVIRONMENT_VARIABLE_DB_USERNAME)
-db_password = os.environ.get(constants.ENVIRONMENT_VARIABLE_DB_PASSWORD)
-rds_proxy_endpoint = os.environ.get(constants.ENVIRONMENT_VARIABLE_DB_PROXY_ENDPOINT)
+db_name = os.environ.get(constants.ENVIRONMENT_VARIABLE_DB_NAME,None)
+db_port = os.environ.get(constants.ENVIRONMENT_VARIABLE_DB_PORT, None)
+db_username = os.environ.get(constants.ENVIRONMENT_VARIABLE_DB_USERNAME, None)
+db_password = os.environ.get(constants.ENVIRONMENT_VARIABLE_DB_PASSWORD, None)
+rds_proxy_endpoint = os.environ.get(constants.ENVIRONMENT_VARIABLE_DB_PROXY_ENDPOINT, None)
 
 
-def get_environment_variable(variable_name, default_value):
+def get_environment_variable(variable_name: object, default_value: object) -> object:
     return os.environ.get(variable_name, default_value)
 
 
 def validate_parameter(parameter_name, parameter_value):
     if parameter_value is None or len(str(parameter_value)):
         raise ValueError(f"{parameter_name} must be defined")
 
 
+def test_version():
+    logging.info("Executing the version of this library ......................")
+
+
 def delete_order(order_id):
     logging.info("Executing the delete_order(order_id) .........................")
     database_name = get_environment_variable(constants.ENVIRONMENT_VARIABLE_DB_NAME, None)
     validate_parameter("db name", database_name)
     database_port = get_environment_variable(constants.ENVIRONMENT_VARIABLE_DB_PORT, None)
     validate_parameter("db port", database_port)
     database_username = get_environment_variable(constants.ENVIRONMENT_VARIABLE_DB_USERNAME, None)
```

### Comparing `package_kpengz-1.0.1/LICENSE` & `package_kpengz-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `package_kpengz-1.0.1/pyproject.toml` & `package_kpengz-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "package_kpengz"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Kolitha Perera", email="kolitha.perera@scania.com"},
 ]
 description = "Python package for mysql functions"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `package_kpengz-1.0.1/PKG-INFO` & `package_kpengz-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: package_kpengz
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python package for mysql functions
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Kolitha Perera <kolitha.perera@scania.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

