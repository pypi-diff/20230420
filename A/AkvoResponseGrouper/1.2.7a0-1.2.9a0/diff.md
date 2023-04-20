# Comparing `tmp/AkvoResponseGrouper-1.2.7a0.tar.gz` & `tmp/AkvoResponseGrouper-1.2.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AkvoResponseGrouper-1.2.7a0.tar", last modified: Tue Mar 28 06:40:35 2023, max compression
+gzip compressed data, was "AkvoResponseGrouper-1.2.9a0.tar", last modified: Thu Apr 20 05:41:51 2023, max compression
```

## Comparing `AkvoResponseGrouper-1.2.7a0.tar` & `AkvoResponseGrouper-1.2.9a0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 06:40:35.947797 AkvoResponseGrouper-1.2.7a0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-03-28 06:40:35.947797 AkvoResponseGrouper-1.2.7a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-28 06:40:35.947797 AkvoResponseGrouper-1.2.7a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 06:40:35.943797 AkvoResponseGrouper-1.2.7a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 06:40:35.943797 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 06:40:35.947797 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/cli/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/cli/checker_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/cli/generate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/response_grouper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 06:40:35.947797 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 06:40:35.943797 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-03-28 06:40:35.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-28 06:40:35.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 06:40:35.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-28 06:40:35.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-28 06:40:35.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-28 06:40:35.000000 AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 06:40:35.947797 AkvoResponseGrouper-1.2.7a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/tests/test_category_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-28 06:40:20.000000 AkvoResponseGrouper-1.2.7a0/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:51.565846 AkvoResponseGrouper-1.2.9a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/checker_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/generate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/response_grouper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-20 05:41:51.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 05:41:51.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 05:41:51.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 05:41:51.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 05:41:51.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 05:41:51.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/tests/test_category_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/tests/test_category_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/tests/test_example.py
```

### Comparing `AkvoResponseGrouper-1.2.7a0/LICENSE` & `AkvoResponseGrouper-1.2.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.7a0/PKG-INFO` & `AkvoResponseGrouper-1.2.9a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoResponseGrouper
-Version: 1.2.7a0
+Version: 1.2.9a0
 Summary: Fast-API Response catalog for pre-computed query
 Home-page: https://github.com/akvo/Akvo-ResponseGrouper
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-ResponseGrouper
 Project-URL: Bug Reports, https://github.com/akvo/Akvo-ResponseGrouper/issues
 Project-URL: Source Code, https://github.com/akvo/Akvo-ResponseGrouper
```

### Comparing `AkvoResponseGrouper-1.2.7a0/README.md` & `AkvoResponseGrouper-1.2.9a0/README.md`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.7a0/setup.py` & `AkvoResponseGrouper-1.2.9a0/setup.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/cli/checker.py` & `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/checker.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/cli/checker_db.py` & `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/checker_db.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/cli/generate_schema.py` & `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/generate_schema.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/cli/migrate.py` & `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/db.py` & `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/db.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/models.py` & `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/models.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/routes.py` & `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/routes.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/tests/conftest.py` & `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py` & `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py` & `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
+import pandas as pd
 from ..utils import (
     group_by_category_output,
     get_intersection,
     generate_data_as_json_file,
     get_valid_list,
     flatten_list,
     validate_number,
+    get_counted_category,
 )
 
 """
 A test case for utils with pytest
 """
 
 
@@ -58,33 +60,48 @@
     c = {
         "name": "Basic",
         "questions": [
             {
                 "id": 567820002,
                 "name": "Toilet Available?",
                 "options": ["Yes"],
-                "else": {"name": "No Service"},
+                "else": {
+                    "name": "No Service",
+                    "ignore": [567800083, 578820191],
+                },
             },
             {
                 "id": 567800083,
                 "name": "Share with outside member?",
                 "options": ["No"],
                 "else": {"name": "Limited"},
             },
             {
-                "id": 567800083,
+                "id": 578820191,
                 "name": "A",
                 "options": ["Boys n Girls"],
-                "else": {"name": "Limited"},
+                "other": [
+                    {
+                        "name": "Limited",
+                        "options": ["Girls Only", "Boys Only"],
+                        "questions": [],
+                    }
+                ],
+                "else": {"name": "No facility"},
             },
         ],
     }
     category = False
     _category = get_valid_list(opt, c, category)
     assert _category == "Limited"
+    opt2 = {
+        "567820002": ["No"],
+    }
+    _category2 = get_valid_list(opt2, c, category)
+    assert _category2 == "Basic"
 
 
 def test_get_flatten_list():
     list = [[1, 2, 3], [4, 5, 6]]
     results = flatten_list(ld=list)
     assert results == [1, 2, 3, 4, 5, 6]
 
@@ -106,7 +123,32 @@
     opt4 = {"number": {"greater_than_equal": 10}}
     res4 = validate_number(q=opt4, answer=answer)
     assert res4 is True
 
     opt5 = {"number": {"less_than_equal": 10}}
     res5 = validate_number(q=opt5, answer=answer)
     assert res5 is True
+
+
+def test_get_counted_category():
+    categories = [
+        {
+            "id": 1,
+            "data": 1,
+            "form": 1,
+            "name": "Water",
+            "category": "Limited",
+        },
+        {
+            "id": 1,
+            "data": 2,
+            "form": 1,
+            "name": "Water",
+            "category": "Basic",
+        },
+    ]
+    df = pd.DataFrame(categories)
+    grouped = get_counted_category(df=df)
+    assert grouped == [
+        {"category": "Basic", "count": 1, "form": 1, "name": "Water"},
+        {"category": "Limited", "count": 1, "form": 1, "name": "Water"},
+    ]
```

### Comparing `AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper.egg-info/PKG-INFO` & `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoResponseGrouper
-Version: 1.2.7a0
+Version: 1.2.9a0
 Summary: Fast-API Response catalog for pre-computed query
 Home-page: https://github.com/akvo/Akvo-ResponseGrouper
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-ResponseGrouper
 Project-URL: Bug Reports, https://github.com/akvo/Akvo-ResponseGrouper/issues
 Project-URL: Source Code, https://github.com/akvo/Akvo-ResponseGrouper
```

### Comparing `AkvoResponseGrouper-1.2.7a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt` & `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 src/AkvoResponseGrouper/cli/generate_schema.py
 src/AkvoResponseGrouper/cli/migrate.py
 src/AkvoResponseGrouper/tests/__init__.py
 src/AkvoResponseGrouper/tests/conftest.py
 src/AkvoResponseGrouper/tests/test_lib_01_route.py
 src/AkvoResponseGrouper/tests/test_lib_02_utils.py
 tests/test_category_checker.py
+tests/test_category_data_frame.py
 tests/test_example.py
```

### Comparing `AkvoResponseGrouper-1.2.7a0/tests/test_category_checker.py` & `AkvoResponseGrouper-1.2.9a0/tests/test_category_checker.py`

 * *Files identical despite different names*

