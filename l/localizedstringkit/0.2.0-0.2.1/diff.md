# Comparing `tmp/localizedstringkit-0.2.0.tar.gz` & `tmp/localizedstringkit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localizedstringkit-0.2.0.tar", max compression
+gzip compressed data, was "localizedstringkit-0.2.1.tar", max compression
```

## Comparing `localizedstringkit-0.2.0.tar` & `localizedstringkit-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0        0 2022-11-29 03:40:30.643858 localizedstringkit-0.2.0/README.md
--rwxr-xr-x   0        0        0    12803 2022-12-01 01:59:40.023140 localizedstringkit-0.2.0/localizedstringkit/__init__.py
--rwxr-xr-x   0        0        0     4735 2022-12-01 01:59:40.024067 localizedstringkit-0.2.0/localizedstringkit/command_line.py
--rwxr-xr-x   0        0        0    10268 2022-12-01 01:59:40.025225 localizedstringkit-0.2.0/localizedstringkit/detection.py
--rwxr-xr-x   0        0        0      140 2022-11-29 03:40:30.653603 localizedstringkit-0.2.0/localizedstringkit/exceptions.py
--rwxr-xr-x   0        0        0     3114 2022-12-01 01:59:40.025985 localizedstringkit-0.2.0/localizedstringkit/files.py
--rw-r--r--   0        0        0      731 2022-11-29 03:40:30.654158 localizedstringkit-0.2.0/localizedstringkit/logger.py
--rw-r--r--   0        0        0     1122 2022-12-01 01:59:40.029009 localizedstringkit-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 localizedstringkit-0.2.0/setup.py
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 localizedstringkit-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-17 13:40:18.279120 localizedstringkit-0.2.1/README.md
+-rwxr-xr-x   0        0        0    12829 2023-04-20 06:27:01.562832 localizedstringkit-0.2.1/localizedstringkit/__init__.py
+-rwxr-xr-x   0        0        0     4735 2023-04-17 13:40:18.285642 localizedstringkit-0.2.1/localizedstringkit/command_line.py
+-rwxr-xr-x   0        0        0    10293 2023-04-20 06:27:01.567959 localizedstringkit-0.2.1/localizedstringkit/detection.py
+-rwxr-xr-x   0        0        0      140 2023-04-17 13:40:18.285992 localizedstringkit-0.2.1/localizedstringkit/exceptions.py
+-rwxr-xr-x   0        0        0     3193 2023-04-20 06:27:01.569999 localizedstringkit-0.2.1/localizedstringkit/files.py
+-rw-r--r--   0        0        0      731 2023-04-17 13:40:18.290979 localizedstringkit-0.2.1/localizedstringkit/logger.py
+-rw-r--r--   0        0        0     1374 2023-04-20 06:27:01.575689 localizedstringkit-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 localizedstringkit-0.2.1/PKG-INFO
```

### Comparing `localizedstringkit-0.2.0/localizedstringkit/__init__.py` & `localizedstringkit-0.2.1/localizedstringkit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,18 @@
         results[entry.key] = entry.stringsdict_format()
 
     with open(existing_stringsdict_path, "wb") as stringsdict_file:
         plistlib.dump(results, stringsdict_file, sort_keys=True)
 
 
 def generate_files(
-    *, code_files: List[str], localized_string_kit_path: str, generate_stringsdict_files: bool
+    *,
+    code_files: List[str],
+    localized_string_kit_path: str,
+    generate_stringsdict_files: bool,
 ) -> None:
     """Run the localization substitution process.
 
     :param List[str] code_files: The list of file paths to generate the .strings
                                   and .stringsdict for.
     :param str localized_string_kit_path: Path to the LocalizedStringsKit
                                            folder which contains the strings
@@ -276,15 +279,18 @@
         if keys_and_variable_names_from_code != keys_and_variable_names_from_file:
             return True
 
     return False
 
 
 def has_changes(
-    *, localized_string_kit_path: str, code_files: List[str], including_stringsdict_files=False
+    *,
+    localized_string_kit_path: str,
+    code_files: List[str],
+    including_stringsdict_files=False,
 ) -> bool:
     """Check if there are outstanding LocalizedStringKit changes.
 
     :param str localized_string_kit_path: Path to the LocalizedStringsKit
                                           folder which contains the strings
                                           bundle and other library data.
     :param List[str] code_files: The list of file paths to check for changes to.
```

### Comparing `localizedstringkit-0.2.0/localizedstringkit/command_line.py` & `localizedstringkit-0.2.1/localizedstringkit/command_line.py`

 * *Files identical despite different names*

### Comparing `localizedstringkit-0.2.0/localizedstringkit/detection.py` & `localizedstringkit-0.2.1/localizedstringkit/detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,16 @@
         results = []
 
         for found_match in matches_in_buffer:
             match: List = []
             for i in range(len(found_match) - 1):
                 match.append(
                     found_match[i].replace(
-                        Detector.TEMPORARY_ESCAPE_SEQUENCE, Detector.QUOTE_ESCAPE_SEQUENCE
+                        Detector.TEMPORARY_ESCAPE_SEQUENCE,
+                        Detector.QUOTE_ESCAPE_SEQUENCE,
                     ),
                 )
 
             match.append(found_match[-1])
 
             # Subtract 1 for length since we append the deriving Pattern to the tuple
             length: int = len(match) - 1
```

### Comparing `localizedstringkit-0.2.0/localizedstringkit/files.py` & `localizedstringkit-0.2.1/localizedstringkit/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,25 @@
     excluded_folders = [os.path.join(root_path, folder) for folder in excluded_folders]
 
     log.debug("Fetching localizable files")
 
     results = []
 
     # Execute find commands
-    find_cmd = ["find", root_path, "-type", "f", "-name", "*.swift", "-o", "-name", "*.m"]
+    find_cmd = [
+        "find",
+        root_path,
+        "-type",
+        "f",
+        "-name",
+        "*.swift",
+        "-o",
+        "-name",
+        "*.m",
+    ]
 
     log.debug(f"Running find command: {find_cmd}")
 
     find_result = subprocess.run(
         find_cmd, universal_newlines=True, check=True, stdout=subprocess.PIPE
     ).stdout
```

### Comparing `localizedstringkit-0.2.0/localizedstringkit/logger.py` & `localizedstringkit-0.2.1/localizedstringkit/logger.py`

 * *Files identical despite different names*

### Comparing `localizedstringkit-0.2.0/pyproject.toml` & `localizedstringkit-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "localizedstringkit"
-version = "0.2.0"
+version = "0.2.1"
 description = "Generate .strings files directly from your code"
 authors = ["Dale Myers <dalemy@microsoft.com>"]
 license = "MIT"
 readme = 'README.md'
 
 repository = "https://github.com/microsoft/LocalizedStringKit"
 homepage = "https://github.com/microsoft/LocalizedStringKit"
@@ -12,31 +12,41 @@
 keywords = ['localization', 'strings', 'generation']
 
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Software Development',
     'Topic :: Software Development :: Internationalization',
     'Topic :: Utilities'
 ]
 
 [tool.poetry.scripts]
 localizedstringkit = 'localizedstringkit:command_line.run'
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
+python = "^3.8"
 dotstrings = "^1.1.3"
-deserialize = "^1.5.0"
+deserialize = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
-black = "=22.10.0"
-mypy = "=0.991"
-pylint = "=2.15.6"
-pytest = "=7.2.0"
-pytest-cov = "=4.0.0"
+black = "^23.3.0"
+mypy = "^1.2.0"
+pylint = "^2.17.2"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+
+[[tool.mypy.overrides]]
+module = [
+    "dotstrings",
+    "dotstrings.genstrings"
+]
+ignore_missing_imports = true
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `localizedstringkit-0.2.0/PKG-INFO` & `localizedstringkit-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: localizedstringkit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generate .strings files directly from your code
 Home-page: https://github.com/microsoft/LocalizedStringKit
 License: MIT
 Keywords: localization,strings,generation
 Author: Dale Myers
 Author-email: dalemy@microsoft.com
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Utilities
-Requires-Dist: deserialize (>=1.5.0,<2.0.0)
+Requires-Dist: deserialize (>=2.0.1,<3.0.0)
 Requires-Dist: dotstrings (>=1.1.3,<2.0.0)
 Project-URL: Repository, https://github.com/microsoft/LocalizedStringKit
 Description-Content-Type: text/markdown
```

