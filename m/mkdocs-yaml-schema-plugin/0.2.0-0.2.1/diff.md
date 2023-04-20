# Comparing `tmp/mkdocs-yaml-schema-plugin-0.2.0.tar.gz` & `tmp/mkdocs-yaml-schema-plugin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-yaml-schema-plugin-0.2.0.tar", last modified: Thu Apr 20 09:48:38 2023, max compression
+gzip compressed data, was "mkdocs-yaml-schema-plugin-0.2.1.tar", last modified: Thu Apr 20 09:56:02 2023, max compression
```

## Comparing `mkdocs-yaml-schema-plugin-0.2.0.tar` & `mkdocs-yaml-schema-plugin-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:48:38.574918 mkdocs-yaml-schema-plugin-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-04-20 09:48:28.000000 mkdocs-yaml-schema-plugin-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-20 09:48:38.574918 mkdocs-yaml-schema-plugin-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 09:48:28.000000 mkdocs-yaml-schema-plugin-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:48:38.574918 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 09:48:28.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 09:48:38.574918 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-20 09:48:28.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-20 09:48:28.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:48:38.574918 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-20 09:48:38.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-20 09:48:38.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:48:38.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 09:48:38.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 09:48:38.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 09:48:38.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-20 09:48:38.574918 mkdocs-yaml-schema-plugin-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-20 09:48:28.000000 mkdocs-yaml-schema-plugin-0.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-20 09:48:28.000000 mkdocs-yaml-schema-plugin-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:56:02.724055 mkdocs-yaml-schema-plugin-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-04-20 09:55:46.000000 mkdocs-yaml-schema-plugin-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-20 09:56:02.724055 mkdocs-yaml-schema-plugin-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 09:55:46.000000 mkdocs-yaml-schema-plugin-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:56:02.724055 mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 09:55:46.000000 mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 09:56:02.724055 mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 09:55:46.000000 mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-20 09:55:46.000000 mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:56:02.724055 mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-20 09:56:02.000000 mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-20 09:56:02.000000 mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:56:02.000000 mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 09:56:02.000000 mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 09:56:02.000000 mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 09:56:02.000000 mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-20 09:56:02.724055 mkdocs-yaml-schema-plugin-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-20 09:55:46.000000 mkdocs-yaml-schema-plugin-0.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-20 09:55:46.000000 mkdocs-yaml-schema-plugin-0.2.1/versioneer.py
```

### Comparing `mkdocs-yaml-schema-plugin-0.2.0/LICENSE.md` & `mkdocs-yaml-schema-plugin-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-yaml-schema-plugin-0.2.0/PKG-INFO` & `mkdocs-yaml-schema-plugin-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-yaml-schema-plugin
-Version: 0.2.0
+Version: 0.2.1
 Summary: MkDocs Plugin to parse yaml schemas.
 Home-page: https://github.com/smeds/mkdocs-yaml-schema-plugin
 Author: Patrik Smeds
 Author-email: patrik.smeds@gmail.com
 License: MIT license
 Keywords: mkdocs,plugin,yaml,schema
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-yaml-schema-plugin-0.2.0/README.md` & `mkdocs-yaml-schema-plugin-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin/markdown.py` & `mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin/markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     def markdown_for_items(self, section, items):
         markdown_data = "| Key | Type | Description |\n"
         markdown_data += "| --- | --- | --- |\n"
 
         for key, values in items['properties'].items():
             description = values['description'].replace("\n", "<br />")
-            for bold_key in bold_keys:
+            for bold_key in self.bold_keys:
                 description = values['description'].replace(bold_key, f"**{bold_key}**")
             markdown_data += f"| {key} | {values['type']} | {description} |\n"
 
         return markdown_data
 
     def set_config(self, config):
         self.yaml_config = []
```

### Comparing `mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin/plugin.py` & `mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/PKG-INFO` & `mkdocs-yaml-schema-plugin-0.2.1/mkdocs_yaml_schema_plugin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-yaml-schema-plugin
-Version: 0.2.0
+Version: 0.2.1
 Summary: MkDocs Plugin to parse yaml schemas.
 Home-page: https://github.com/smeds/mkdocs-yaml-schema-plugin
 Author: Patrik Smeds
 Author-email: patrik.smeds@gmail.com
 License: MIT license
 Keywords: mkdocs,plugin,yaml,schema
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-yaml-schema-plugin-0.2.0/setup.py` & `mkdocs-yaml-schema-plugin-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `mkdocs-yaml-schema-plugin-0.2.0/versioneer.py` & `mkdocs-yaml-schema-plugin-0.2.1/versioneer.py`

 * *Files identical despite different names*

