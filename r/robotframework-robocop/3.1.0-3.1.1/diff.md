# Comparing `tmp/robotframework-robocop-3.1.0.tar.gz` & `tmp/robotframework-robocop-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robocop-3.1.0.tar", last modified: Tue Apr 18 11:05:52 2023, max compression
+gzip compressed data, was "robotframework-robocop-3.1.1.tar", last modified: Thu Apr 20 10:35:01 2023, max compression
```

## Comparing `robotframework-robocop-3.1.0.tar` & `robotframework-robocop-3.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:05:52.066964 robotframework-robocop-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-04-18 11:05:52.066964 robotframework-robocop-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:05:52.062965 robotframework-robocop-3.1.0/robocop/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:05:52.062965 robotframework-robocop-3.1.0/robocop/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17331 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/duplications.py
--rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    27365 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/lengths.py
--rw-r--r--   0 runner    (1001) docker     (123)    26679 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31744 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/naming.py
--rw-r--r--   0 runner    (1001) docker     (123)    33520 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    23822 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:05:52.066964 robotframework-robocop-3.1.0/robocop/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/utils/disablers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/utils/file_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/utils/run_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/utils/version_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:05:52.066964 robotframework-robocop-3.1.0/robotframework_robocop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-04-18 11:05:52.000000 robotframework-robocop-3.1.0/robotframework_robocop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-18 11:05:52.000000 robotframework-robocop-3.1.0/robotframework_robocop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:05:52.000000 robotframework-robocop-3.1.0/robotframework_robocop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 11:05:52.000000 robotframework-robocop-3.1.0/robotframework_robocop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-18 11:05:52.000000 robotframework-robocop-3.1.0/robotframework_robocop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 11:05:52.000000 robotframework-robocop-3.1.0/robotframework_robocop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 11:05:52.066964 robotframework-robocop-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:01.849020 robotframework-robocop-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-04-20 10:35:01.849020 robotframework-robocop-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:01.845019 robotframework-robocop-3.1.1/robocop/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:01.845019 robotframework-robocop-3.1.1/robocop/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17331 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/duplications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27365 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/lengths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26679 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33520 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23822 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:01.845019 robotframework-robocop-3.1.1/robocop/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/utils/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/utils/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/utils/run_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/utils/version_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:01.845019 robotframework-robocop-3.1.1/robotframework_robocop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-04-20 10:35:01.000000 robotframework-robocop-3.1.1/robotframework_robocop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-20 10:35:01.000000 robotframework-robocop-3.1.1/robotframework_robocop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:35:01.000000 robotframework-robocop-3.1.1/robotframework_robocop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 10:35:01.000000 robotframework-robocop-3.1.1/robotframework_robocop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-20 10:35:01.000000 robotframework-robocop-3.1.1/robotframework_robocop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 10:35:01.000000 robotframework-robocop-3.1.1/robotframework_robocop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:35:01.849020 robotframework-robocop-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/setup.py
```

### Comparing `robotframework-robocop-3.1.0/LICENSE` & `robotframework-robocop-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/PKG-INFO` & `robotframework-robocop-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 3.1.0
+Version: 3.1.1
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
```

### Comparing `robotframework-robocop-3.1.0/README.md` & `robotframework-robocop-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/checkers/__init__.py` & `robotframework-robocop-3.1.1/robocop/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/checkers/comments.py` & `robotframework-robocop-3.1.1/robocop/checkers/comments.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/checkers/documentation.py` & `robotframework-robocop-3.1.1/robocop/checkers/documentation.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/checkers/duplications.py` & `robotframework-robocop-3.1.1/robocop/checkers/duplications.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/checkers/errors.py` & `robotframework-robocop-3.1.1/robocop/checkers/errors.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/checkers/lengths.py` & `robotframework-robocop-3.1.1/robocop/checkers/lengths.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/checkers/misc.py` & `robotframework-robocop-3.1.1/robocop/checkers/misc.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/checkers/naming.py` & `robotframework-robocop-3.1.1/robocop/checkers/naming.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 """
 import re
 import string
 from collections import defaultdict
 from pathlib import Path
 
 from robot.api import Token
-from robot.parsing.model.blocks import Keyword
-from robot.parsing.model.statements import Arguments, KeywordCall
+from robot.errors import VariableError
+from robot.parsing.model.statements import Arguments
 from robot.variables.search import search_variable
 
 from robocop.checkers import VisitorChecker
 from robocop.rules import Rule, RuleParam, RuleSeverity
 from robocop.utils import (
     ROBOT_VERSION,
     find_robot_vars,
@@ -664,15 +664,18 @@
             "setsuitevariable",
             "setglobalvariable",
         }
         super().__init__()
 
     def visit_Variable(self, node):  # noqa
         token = node.data_tokens[0]
-        var_name = search_variable(token.value).base
+        try:
+            var_name = search_variable(token.value).base
+        except VariableError:
+            return  # TODO: Ignore for now, for example ${not  closed in variables will throw it
         if var_name is None:
             return  # in RF<=5, a continuation mark ` ...` is wrongly considered a variable
         # in Variables section, everything needs to be in uppercase
         # because even when the variable is nested, it needs to be global
         if not var_name.isupper():
             self.report(
                 "section-variable-not-uppercase",
@@ -697,15 +700,20 @@
             return
         if normalize_robot_name(node.keyword, remove_prefix="builtin.") in self.set_variable_variants:
             if len(node.data_tokens) < 2:
                 return
             token = node.data_tokens[1]
             if not token.value:
                 return
-            var_name = search_variable(token.value).base
+            try:
+                var_name = search_variable(token.value).base
+            except VariableError:
+                return  # TODO: Ignore for now, for example ${not  closed in variables will throw it
+            if var_name is None:  # possibly $escaped or \${escaped}, or invalid variable name
+                return
             normalized_var_name = remove_nested_variables(var_name)
             # a variable as a keyword argument can contain lowercase nested variable
             # because the actual value of it may be uppercase
             if not normalized_var_name.isupper():
                 self.report(
                     "non-local-variables-should-be-uppercase",
                     node=node,
```

### Comparing `robotframework-robocop-3.1.0/robocop/checkers/spacing.py` & `robotframework-robocop-3.1.1/robocop/checkers/spacing.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/checkers/tags.py` & `robotframework-robocop-3.1.1/robocop/checkers/tags.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/config.py` & `robotframework-robocop-3.1.1/robocop/config.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/exceptions.py` & `robotframework-robocop-3.1.1/robocop/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/files.py` & `robotframework-robocop-3.1.1/robocop/files.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/reports.py` & `robotframework-robocop-3.1.1/robocop/reports.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/rules.py` & `robotframework-robocop-3.1.1/robocop/rules.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/run.py` & `robotframework-robocop-3.1.1/robocop/run.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/utils/__init__.py` & `robotframework-robocop-3.1.1/robocop/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/utils/disablers.py` & `robotframework-robocop-3.1.1/robocop/utils/disablers.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/utils/file_types.py` & `robotframework-robocop-3.1.1/robocop/utils/file_types.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/utils/misc.py` & `robotframework-robocop-3.1.1/robocop/utils/misc.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/utils/run_keywords.py` & `robotframework-robocop-3.1.1/robocop/utils/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robocop/utils/version_matching.py` & `robotframework-robocop-3.1.1/robocop/utils/version_matching.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/robotframework_robocop.egg-info/PKG-INFO` & `robotframework-robocop-3.1.1/robotframework_robocop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 3.1.0
+Version: 3.1.1
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
```

### Comparing `robotframework-robocop-3.1.0/robotframework_robocop.egg-info/SOURCES.txt` & `robotframework-robocop-3.1.1/robotframework_robocop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.0/setup.py` & `robotframework-robocop-3.1.1/setup.py`

 * *Files identical despite different names*

