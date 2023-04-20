# Comparing `tmp/auto_gpt_plugin_template-0.0.1.tar.gz` & `tmp/auto_gpt_plugin_template-0.0.2.tar.gz`

## Comparing `auto_gpt_plugin_template-0.0.1.tar` & `auto_gpt_plugin_template-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/.coveragerc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/.editorconfig
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/.flake8
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/.isort.cfg
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/.sourcery.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/clean_all.sh
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/pylintrc
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/qa.bat
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/qa.sh
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/requirements.txt
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/run_pylint.py
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/style.bat
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/style.sh
--rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/src/auto_gpt_plugin_template/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/LICENSE
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/README.md
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/.coveragerc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/.editorconfig
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/.flake8
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/.isort.cfg
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/.sourcery.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/clean_all.sh
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/pylintrc
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/qa.bat
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/qa.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/run_pylint.py
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/style.bat
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/style.sh
+-rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/src/auto_gpt_plugin_template/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/LICENSE
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/README.md
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/PKG-INFO
```

### Comparing `auto_gpt_plugin_template-0.0.1/.coveragerc` & `auto_gpt_plugin_template-0.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `auto_gpt_plugin_template-0.0.1/.pre-commit-config.yaml` & `auto_gpt_plugin_template-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `auto_gpt_plugin_template-0.0.1/.sourcery.yaml` & `auto_gpt_plugin_template-0.0.2/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `auto_gpt_plugin_template-0.0.1/pylintrc` & `auto_gpt_plugin_template-0.0.2/pylintrc`

 * *Files identical despite different names*

### Comparing `auto_gpt_plugin_template-0.0.1/src/auto_gpt_plugin_template/__init__.py` & `auto_gpt_plugin_template-0.0.2/src/auto_gpt_plugin_template/__init__.py`

 * *Files identical despite different names*

### Comparing `auto_gpt_plugin_template-0.0.1/.gitignore` & `auto_gpt_plugin_template-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `auto_gpt_plugin_template-0.0.1/LICENSE` & `auto_gpt_plugin_template-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_gpt_plugin_template-0.0.1/pyproject.toml` & `auto_gpt_plugin_template-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "auto_gpt_plugin_template"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
-  { name="Bill Schumacher", email="34168009+BillSchumacher@users.noreply.github.com" },
+  { name="Torantulino", email="34168009+BillSchumacher@users.noreply.github.com" },
 ]
 description = "The template plugin for Auto-GPT."
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = ["abstract-singleton"]
 
 [project.urls]
-"Homepage" = "https://github.com/Torantulino/Auto-GPT-Plugin-Template"
-"Bug Tracker" = "https://github.com/Torantulino/Auto-GPT-Plugin-Template/issues"
+"Homepage" = "https://github.com/Torantulino/Auto-GPT"
+"Bug Tracker" = "https://github.com/Torantulino/Auto-GPT"
 
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

### Comparing `auto_gpt_plugin_template-0.0.1/PKG-INFO` & `auto_gpt_plugin_template-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: auto_gpt_plugin_template
-Version: 0.0.1
+Version: 0.0.2
 Summary: The template plugin for Auto-GPT.
-Project-URL: Homepage, https://github.com/Torantulino/Auto-GPT-Plugin-Template
-Project-URL: Bug Tracker, https://github.com/Torantulino/Auto-GPT-Plugin-Template/issues
-Author-email: Bill Schumacher <34168009+BillSchumacher@users.noreply.github.com>
+Project-URL: Homepage, https://github.com/Torantulino/Auto-GPT
+Project-URL: Bug Tracker, https://github.com/Torantulino/Auto-GPT
+Author-email: Torantulino <34168009+BillSchumacher@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Requires-Dist: abstract-singleton
 Description-Content-Type: text/markdown
 
 # (Coming Soon) Auto-GPT-Plugin-Template
 A starting point for developing your own plug-in for Auto-GPT
```

