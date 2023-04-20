# Comparing `tmp/mkdocs-yaml-schema-plugin-0.1.3.tar.gz` & `tmp/mkdocs-yaml-schema-plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-yaml-schema-plugin-0.1.3.tar", last modified: Wed Apr 19 13:34:03 2023, max compression
+gzip compressed data, was "mkdocs-yaml-schema-plugin-0.2.0.tar", last modified: Thu Apr 20 09:48:38 2023, max compression
```

## Comparing `mkdocs-yaml-schema-plugin-0.1.3.tar` & `mkdocs-yaml-schema-plugin-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 patsm159  (1000) patsm159  (1000)        0 2023-04-19 13:34:03.660050 mkdocs-yaml-schema-plugin-0.1.3/
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)    34961 2023-04-19 11:50:13.000000 mkdocs-yaml-schema-plugin-0.1.3/LICENSE.md
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)     1238 2023-04-19 13:34:03.660050 mkdocs-yaml-schema-plugin-0.1.3/PKG-INFO
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)      540 2023-04-19 12:50:40.000000 mkdocs-yaml-schema-plugin-0.1.3/README.md
-drwxrwxr-x   0 patsm159  (1000) patsm159  (1000)        0 2023-04-19 13:34:03.660050 mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin/
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)       73 2023-04-19 11:50:13.000000 mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin/__init__.py
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)      497 2023-04-19 13:34:03.660050 mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin/_version.py
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)     2171 2023-04-18 14:08:50.000000 mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin/markdown.py
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)      529 2023-04-18 14:08:50.000000 mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin/plugin.py
-drwxrwxr-x   0 patsm159  (1000) patsm159  (1000)        0 2023-04-19 13:34:03.660050 mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin.egg-info/
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)     1238 2023-04-19 13:34:03.000000 mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)      499 2023-04-19 13:34:03.000000 mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)        1 2023-04-19 13:34:03.000000 mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)       76 2023-04-19 13:34:03.000000 mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)       14 2023-04-19 13:34:03.000000 mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin.egg-info/requires.txt
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)       26 2023-04-19 13:34:03.000000 mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin.egg-info/top_level.txt
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)      277 2023-04-19 13:34:03.660050 mkdocs-yaml-schema-plugin-0.1.3/setup.cfg
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)     1243 2023-04-19 13:28:02.000000 mkdocs-yaml-schema-plugin-0.1.3/setup.py
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)    83607 2023-04-19 12:50:40.000000 mkdocs-yaml-schema-plugin-0.1.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:48:38.574918 mkdocs-yaml-schema-plugin-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-04-20 09:48:28.000000 mkdocs-yaml-schema-plugin-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-20 09:48:38.574918 mkdocs-yaml-schema-plugin-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 09:48:28.000000 mkdocs-yaml-schema-plugin-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:48:38.574918 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 09:48:28.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 09:48:38.574918 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-20 09:48:28.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-20 09:48:28.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:48:38.574918 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-20 09:48:38.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-20 09:48:38.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:48:38.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 09:48:38.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 09:48:38.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 09:48:38.000000 mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-20 09:48:38.574918 mkdocs-yaml-schema-plugin-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-20 09:48:28.000000 mkdocs-yaml-schema-plugin-0.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-20 09:48:28.000000 mkdocs-yaml-schema-plugin-0.2.0/versioneer.py
```

### Comparing `mkdocs-yaml-schema-plugin-0.1.3/LICENSE.md` & `mkdocs-yaml-schema-plugin-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-yaml-schema-plugin-0.1.3/PKG-INFO` & `mkdocs-yaml-schema-plugin-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mkdocs-yaml-schema-plugin
-Version: 0.1.3
+Version: 0.2.0
 Summary: MkDocs Plugin to parse yaml schemas.
 Home-page: https://github.com/smeds/mkdocs-yaml-schema-plugin
 Author: Patrik Smeds
 Author-email: patrik.smeds@gmail.com
 License: MIT license
 Keywords: mkdocs,plugin,yaml,schema
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8, <4
@@ -40,9 +39,7 @@
         tag: "RESOURCESSCHEMA"
 ```
 
 In your target file, add a tag to be replaced
 ```
 #RESOURCESSCHEMA#
 ```
-
-
```

### Comparing `mkdocs-yaml-schema-plugin-0.1.3/README.md` & `mkdocs-yaml-schema-plugin-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin/markdown.py` & `mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin/markdown.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         return yaml_data
 
 
 class markdown_gen:
     schema_file = ''
     tag = ''
     indent_val = "    "
+    bold_keys = ["NOTE:", "RECOMMENDATION:"]
 
     def safe_get_value(self, data, key):
         if data is None:
             return None, False
         try:
             output = data[key]
             return output, True
@@ -31,25 +32,28 @@
                     self.yaml_config[index]['data'] = yaml.safe_load(yaml_file)
 
             for values in self.yaml_config:
                 for g in re.finditer(values['regex'], markdown):
                     parts = g.group()[1:-1].split("__")
                     new_markdown = self.markdown_for_items(parts[1],
                                                            extract_yaml_section(parts[1:],
-                                                                                values['data']['properties']))
+                                                           values['data']['properties']))
                     markdown = markdown.replace(g.group(), new_markdown)
 
             return markdown
 
     def markdown_for_items(self, section, items):
         markdown_data = "| Key | Type | Description |\n"
         markdown_data += "| --- | --- | --- |\n"
 
         for key, values in items['properties'].items():
-            markdown_data += f"| {key} | {values['type']} | {values['description']} |\n"
+            description = values['description'].replace("\n", "<br />")
+            for bold_key in bold_keys:
+                description = values['description'].replace(bold_key, f"**{bold_key}**")
+            markdown_data += f"| {key} | {values['type']} | {description} |\n"
 
         return markdown_data
 
     def set_config(self, config):
         self.yaml_config = []
         # CHeck why I need to fetch first object
         for f in self.safe_get_value(config, "yaml_files")[0]:
```

### Comparing `mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin/plugin.py` & `mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-yaml-schema-plugin-0.1.3/mkdocs_yaml_schema_plugin.egg-info/PKG-INFO` & `mkdocs-yaml-schema-plugin-0.2.0/mkdocs_yaml_schema_plugin.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mkdocs-yaml-schema-plugin
-Version: 0.1.3
+Version: 0.2.0
 Summary: MkDocs Plugin to parse yaml schemas.
 Home-page: https://github.com/smeds/mkdocs-yaml-schema-plugin
 Author: Patrik Smeds
 Author-email: patrik.smeds@gmail.com
 License: MIT license
 Keywords: mkdocs,plugin,yaml,schema
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8, <4
@@ -40,9 +39,7 @@
         tag: "RESOURCESSCHEMA"
 ```
 
 In your target file, add a tag to be replaced
 ```
 #RESOURCESSCHEMA#
 ```
-
-
```

### Comparing `mkdocs-yaml-schema-plugin-0.1.3/setup.py` & `mkdocs-yaml-schema-plugin-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `mkdocs-yaml-schema-plugin-0.1.3/versioneer.py` & `mkdocs-yaml-schema-plugin-0.2.0/versioneer.py`

 * *Files identical despite different names*

