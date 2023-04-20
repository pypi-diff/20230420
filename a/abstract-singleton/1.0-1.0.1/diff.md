# Comparing `tmp/abstract_singleton-1.0.tar.gz` & `tmp/abstract_singleton-1.0.1.tar.gz`

## Comparing `abstract_singleton-1.0.tar` & `abstract_singleton-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 abstract_singleton-1.0/.coveragerc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 abstract_singleton-1.0/.editorconfig
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 abstract_singleton-1.0/.flake8
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 abstract_singleton-1.0/.isort.cfg
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 abstract_singleton-1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 abstract_singleton-1.0/.sourcery.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 abstract_singleton-1.0/clean_all.sh
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 abstract_singleton-1.0/pylintrc
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 abstract_singleton-1.0/qa.bat
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 abstract_singleton-1.0/qa.sh
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 abstract_singleton-1.0/requirements.txt
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 abstract_singleton-1.0/run_pylint.py
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 abstract_singleton-1.0/style.bat
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 abstract_singleton-1.0/style.sh
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 abstract_singleton-1.0/src/abstract_singleton/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 abstract_singleton-1.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 abstract_singleton-1.0/LICENSE
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 abstract_singleton-1.0/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 abstract_singleton-1.0/pyproject.toml
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 abstract_singleton-1.0/PKG-INFO
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/.coveragerc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/.editorconfig
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/.flake8
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/.isort.cfg
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/.sourcery.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/clean_all.sh
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/pylintrc
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/qa.bat
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/qa.sh
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/requirements.txt
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/run_pylint.py
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/style.bat
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/style.sh
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/src/abstract_singleton/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/LICENSE
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/README.md
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 abstract_singleton-1.0.1/PKG-INFO
```

### Comparing `abstract_singleton-1.0/.coveragerc` & `abstract_singleton-1.0.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `abstract_singleton-1.0/.pre-commit-config.yaml` & `abstract_singleton-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `abstract_singleton-1.0/.sourcery.yaml` & `abstract_singleton-1.0.1/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `abstract_singleton-1.0/pylintrc` & `abstract_singleton-1.0.1/pylintrc`

 * *Files identical despite different names*

### Comparing `abstract_singleton-1.0/src/abstract_singleton/__init__.py` & `abstract_singleton-1.0.1/src/abstract_singleton/__init__.py`

 * *Files identical despite different names*

### Comparing `abstract_singleton-1.0/.gitignore` & `abstract_singleton-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `abstract_singleton-1.0/LICENSE` & `abstract_singleton-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `abstract_singleton-1.0/pyproject.toml` & `abstract_singleton-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "abstract_singleton"
-version = "1.0"
+version = "1.0.1"
 authors = [
   { name="Bill Schumacher", email="34168009+BillSchumacher@users.noreply.github.com" },
 ]
 description = "An abstract singleton class."
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = []
 
 [project.urls]
 "Homepage" = "https://github.com/BillSchumacher/Abstract-Singleton"
 "Bug Tracker" = "https://github.com/BillSchumacher/Abstract-Singleton/issues"
 
 [tool.black]
 line-length = 88
-target-version = ['py310']
+target-version = ['py38']
 include = '\.pyi?$'
 extend-exclude = ""
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.messages_control]
```

### Comparing `abstract_singleton-1.0/PKG-INFO` & `abstract_singleton-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: abstract_singleton
-Version: 1.0
+Version: 1.0.1
 Summary: An abstract singleton class.
 Project-URL: Homepage, https://github.com/BillSchumacher/Abstract-Singleton
 Project-URL: Bug Tracker, https://github.com/BillSchumacher/Abstract-Singleton/issues
 Author-email: Bill Schumacher <34168009+BillSchumacher@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Abstract-Singleton
 
 A Singleton that also enforces abstract methods are implemented.
```

