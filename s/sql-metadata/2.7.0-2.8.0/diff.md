# Comparing `tmp/sql_metadata-2.7.0.tar.gz` & `tmp/sql_metadata-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_metadata-2.7.0.tar", max compression
+gzip compressed data, was "sql_metadata-2.8.0.tar", max compression
```

## Comparing `sql_metadata-2.7.0.tar` & `sql_metadata-2.8.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-03-23 19:40:24.712773 sql_metadata-2.7.0/LICENSE
--rw-r--r--   0        0        0     9003 2023-03-23 19:40:24.712773 sql_metadata-2.7.0/README.md
--rw-r--r--   0        0        0      895 2023-03-23 19:40:24.712773 sql_metadata-2.7.0/pyproject.toml
--rw-r--r--   0        0        0      264 2023-03-23 19:40:24.712773 sql_metadata-2.7.0/sql_metadata/__init__.py
--rw-r--r--   0        0        0     1311 2023-03-23 19:40:24.712773 sql_metadata-2.7.0/sql_metadata/compat.py
--rw-r--r--   0        0        0     2446 2023-03-23 19:40:24.712773 sql_metadata-2.7.0/sql_metadata/generalizator.py
--rw-r--r--   0        0        0     2498 2023-03-23 19:40:24.712773 sql_metadata-2.7.0/sql_metadata/keywords_lists.py
--rw-r--r--   0        0        0    41602 2023-03-23 19:40:24.712773 sql_metadata-2.7.0/sql_metadata/parser.py
--rw-r--r--   0        0        0    19115 2023-03-23 19:40:24.712773 sql_metadata-2.7.0/sql_metadata/token.py
--rw-r--r--   0        0        0      778 2023-03-23 19:40:24.712773 sql_metadata-2.7.0/sql_metadata/utils.py
--rw-r--r--   0        0        0     9749 1970-01-01 00:00:00.000000 sql_metadata-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/LICENSE
+-rw-r--r--   0        0        0     9003 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/README.md
+-rw-r--r--   0        0        0      895 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0      264 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/sql_metadata/__init__.py
+-rw-r--r--   0        0        0     1311 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/sql_metadata/compat.py
+-rw-r--r--   0        0        0     2446 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/sql_metadata/generalizator.py
+-rw-r--r--   0        0        0     2498 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/sql_metadata/keywords_lists.py
+-rw-r--r--   0        0        0    42049 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/sql_metadata/parser.py
+-rw-r--r--   0        0        0    19115 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/sql_metadata/token.py
+-rw-r--r--   0        0        0      778 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/sql_metadata/utils.py
+-rw-r--r--   0        0        0     9749 1970-01-01 00:00:00.000000 sql_metadata-2.8.0/PKG-INFO
```

### Comparing `sql_metadata-2.7.0/LICENSE` & `sql_metadata-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_metadata-2.7.0/README.md` & `sql_metadata-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `sql_metadata-2.7.0/pyproject.toml` & `sql_metadata-2.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql_metadata"
-version = "2.7.0"
+version = "2.8.0"
 license="MIT"
 description = "Uses tokenized query returned by python-sqlparse and generates query metadata"
 authors = ["Maciej Brencz <maciej.brencz@gmail.com>", "Radosław Drążkiewicz <collerek@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/macbre/sql-metadata"
 repository = "https://github.com/macbre/sql-metadata"
 
@@ -13,18 +13,18 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
 sqlparse = "^0.4.1"
 
 [tool.poetry.dev-dependencies]
-black = "^23.1"
+black = "^23.3"
 coverage = {extras = ["toml"], version = "^6.5"}
-pylint = "^2.17.1"
-pytest = "^7.2.2"
+pylint = "^2.17.2"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 coveralls = "^3.3.1"
 flake8 = "^5.0.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sql_metadata-2.7.0/sql_metadata/compat.py` & `sql_metadata-2.8.0/sql_metadata/compat.py`

 * *Files identical despite different names*

### Comparing `sql_metadata-2.7.0/sql_metadata/generalizator.py` & `sql_metadata-2.8.0/sql_metadata/generalizator.py`

 * *Files identical despite different names*

### Comparing `sql_metadata-2.7.0/sql_metadata/keywords_lists.py` & `sql_metadata-2.8.0/sql_metadata/keywords_lists.py`

 * *Files identical despite different names*

### Comparing `sql_metadata-2.7.0/sql_metadata/parser.py` & `sql_metadata-2.8.0/sql_metadata/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,14 +353,22 @@
                         query_type=self.query_type
                     )
                     or token.is_columns_alias_of_with_query_or_column_in_insert_query(
                         with_names=with_names
                     )
                 ):
                     continue
+
+                # handle INSERT INTO ON DUPLICATE KEY UPDATE queries
+                if (
+                    token.last_keyword_normalized == "UPDATE"
+                    and self.query_type == "INSERT"
+                ):
+                    continue
+
                 table_name = str(token.value.strip("`"))
                 token.token_type = TokenType.TABLE
                 tables.append(table_name)
 
         self._tables = tables - with_names
         return self._tables
 
@@ -378,16 +386,20 @@
             if token.is_integer:
                 if token.last_keyword_normalized == "LIMIT" and not limit:
                     # LIMIT <limit>
                     limit = int(token.value)
                 elif token.last_keyword_normalized == "OFFSET":
                     # OFFSET <offset>
                     offset = int(token.value)
-                elif token.previous_token.is_punctuation:
+                elif (
+                    token.previous_token.is_punctuation
+                    and token.last_keyword_normalized == "LIMIT"
+                ):
                     # LIMIT <offset>,<limit>
+                    #  enter this condition only when the limit has already been parsed
                     offset = limit
                     limit = int(token.value)
 
         if limit is None:
             return None
 
         self._limit_and_offset = limit, offset or 0
```

### Comparing `sql_metadata-2.7.0/sql_metadata/token.py` & `sql_metadata-2.8.0/sql_metadata/token.py`

 * *Files identical despite different names*

### Comparing `sql_metadata-2.7.0/sql_metadata/utils.py` & `sql_metadata-2.8.0/sql_metadata/utils.py`

 * *Files identical despite different names*

### Comparing `sql_metadata-2.7.0/PKG-INFO` & `sql_metadata-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-metadata
-Version: 2.7.0
+Version: 2.8.0
 Summary: Uses tokenized query returned by python-sqlparse and generates query metadata
 Home-page: https://github.com/macbre/sql-metadata
 License: MIT
 Author: Maciej Brencz
 Author-email: maciej.brencz@gmail.com
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sql-metadata Version: 2.7.0 Summary: Uses tokenized
+Metadata-Version: 2.1 Name: sql-metadata Version: 2.8.0 Summary: Uses tokenized
 query returned by python-sqlparse and generates query metadata Home-page:
 https://github.com/macbre/sql-metadata License: MIT Author: Maciej Brencz
 Author-email: maciej.brencz@gmail.com Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

