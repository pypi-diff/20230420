# Comparing `tmp/sqlstrings-0.0.6.tar.gz` & `tmp/sqlstrings-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlstrings-0.0.6.tar", last modified: Mon Apr 17 14:05:16 2023, max compression
+gzip compressed data, was "sqlstrings-0.0.7.tar", last modified: Thu Apr 20 10:13:15 2023, max compression
```

## Comparing `sqlstrings-0.0.6.tar` & `sqlstrings-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 14:05:16.941518 sqlstrings-0.0.6/
--rw-rw-rw-   0        0        0     1091 2023-04-17 07:54:03.000000 sqlstrings-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      874 2023-04-17 14:05:16.940345 sqlstrings-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-04-17 10:54:33.000000 sqlstrings-0.0.6/README.md
--rw-rw-rw-   0        0        0      576 2023-04-17 14:02:40.000000 sqlstrings-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 14:05:16.942525 sqlstrings-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 14:05:16.812056 sqlstrings-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 14:05:16.874405 sqlstrings-0.0.6/src/sqlstrings/
--rw-rw-rw-   0        0        0       67 2023-04-17 14:00:38.000000 sqlstrings-0.0.6/src/sqlstrings/__init__.py
--rw-rw-rw-   0        0        0     3583 2023-04-17 13:05:55.000000 sqlstrings-0.0.6/src/sqlstrings/csv_handling.py
--rw-rw-rw-   0        0        0     4543 2023-04-13 13:01:44.000000 sqlstrings-0.0.6/src/sqlstrings/postgre.py
--rw-rw-rw-   0        0        0     4190 2023-03-31 16:29:50.000000 sqlstrings-0.0.6/src/sqlstrings/transact.py
--rw-rw-rw-   0        0        0     2068 2023-04-14 09:05:58.000000 sqlstrings-0.0.6/src/sqlstrings/value_handling.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:05:16.920619 sqlstrings-0.0.6/src/sqlstrings.egg-info/
--rw-rw-rw-   0        0        0      874 2023-04-17 14:05:16.000000 sqlstrings-0.0.6/src/sqlstrings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-04-17 14:05:16.000000 sqlstrings-0.0.6/src/sqlstrings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 14:05:16.000000 sqlstrings-0.0.6/src/sqlstrings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-17 14:05:16.000000 sqlstrings-0.0.6/src/sqlstrings.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 14:05:16.936946 sqlstrings-0.0.6/tests/
--rw-rw-rw-   0        0        0       30 2023-03-31 16:34:51.000000 sqlstrings-0.0.6/tests/test_csv_handling.py
--rw-rw-rw-   0        0        0      162 2023-03-31 16:28:49.000000 sqlstrings-0.0.6/tests/test_main.py
--rw-rw-rw-   0        0        0     2472 2023-04-13 13:01:08.000000 sqlstrings-0.0.6/tests/test_postgre.py
--rw-rw-rw-   0        0        0     1984 2023-04-12 16:19:18.000000 sqlstrings-0.0.6/tests/test_transact.py
--rw-rw-rw-   0        0        0     1632 2023-04-12 16:19:28.000000 sqlstrings-0.0.6/tests/test_value_handling.py
+drwxrwxrwx   0        0        0        0 2023-04-20 10:13:15.902919 sqlstrings-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 15:39:37.000000 sqlstrings-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      509 2023-04-20 10:13:15.899948 sqlstrings-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-04-19 16:09:43.000000 sqlstrings-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 10:13:15.903938 sqlstrings-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      638 2023-04-20 10:12:30.000000 sqlstrings-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 10:13:15.853825 sqlstrings-0.0.7/sqlstrings/
+-rw-rw-rw-   0        0        0       67 2023-04-17 15:00:41.000000 sqlstrings-0.0.7/sqlstrings/__init__.py
+-rw-rw-rw-   0        0        0     3597 2023-04-20 10:08:31.000000 sqlstrings-0.0.7/sqlstrings/csv_handling.py
+-rw-rw-rw-   0        0        0     4542 2023-04-20 10:00:39.000000 sqlstrings-0.0.7/sqlstrings/postgre.py
+-rw-rw-rw-   0        0        0     4175 2023-04-20 09:59:55.000000 sqlstrings-0.0.7/sqlstrings/transact.py
+-rw-rw-rw-   0        0        0     2053 2023-04-20 08:23:09.000000 sqlstrings-0.0.7/sqlstrings/value_handling.py
+drwxrwxrwx   0        0        0        0 2023-04-20 10:13:15.882392 sqlstrings-0.0.7/sqlstrings.egg-info/
+-rw-rw-rw-   0        0        0      509 2023-04-20 10:13:15.000000 sqlstrings-0.0.7/sqlstrings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-04-20 10:13:15.000000 sqlstrings-0.0.7/sqlstrings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 10:13:15.000000 sqlstrings-0.0.7/sqlstrings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 10:13:15.000000 sqlstrings-0.0.7/sqlstrings.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 10:13:15.896923 sqlstrings-0.0.7/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-17 15:36:45.000000 sqlstrings-0.0.7/tests/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-03-31 16:34:51.000000 sqlstrings-0.0.7/tests/test_csv_handling.py
+-rw-rw-rw-   0        0        0      163 2023-04-17 15:38:11.000000 sqlstrings-0.0.7/tests/test_main.py
+-rw-rw-rw-   0        0        0     2474 2023-04-17 15:39:16.000000 sqlstrings-0.0.7/tests/test_postgre.py
+-rw-rw-rw-   0        0        0     1986 2023-04-17 15:38:37.000000 sqlstrings-0.0.7/tests/test_transact.py
+-rw-rw-rw-   0        0        0     1634 2023-04-17 15:38:35.000000 sqlstrings-0.0.7/tests/test_value_handling.py
```

### Comparing `sqlstrings-0.0.6/LICENSE` & `sqlstrings-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.6/src/sqlstrings/csv_handling.py` & `sqlstrings-0.0.7/sqlstrings/csv_handling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from value_handling import value_reader
+from sqlstrings.value_handling import read_val
 from typing import Callable, Any
 from pathlib import Path
 from csv import reader
-from transact import insertion, update
+from sqlstrings.transact import insertion, update
 import logging
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
 class CSVFile:
@@ -53,33 +53,33 @@
     mapping each header title to its respective value.
     :param header: The header of the csv file.
     :param row: The row of the csv file.
     :return: row_dict The dictionary representing that row.
     """
     row_dict = {}
     for idx, value in enumerate(row):
-        row_dict[header[idx]] = value_reader(value.lstrip().rstrip())
+        row_dict[header[idx]] = read_val(value.lstrip().rstrip())
     return row_dict
 
 
-def csv_as_inserts(path: str | Path, table_name: str, insertion_func: Callable = insertion):
+def csv_to_inserts(path: str | Path, table_name: str, insertion_func: Callable = insertion):
     """
     Converts a .csv file into a list of insert statement strings that can be executed in a SQL Database.
     :param path: The path of the file to convert.
     :param table_name: The name of the table in which to insert.
     :param insertion_func: The function to use to generate the insertion statements i.e. from postgre, or sql?
     :return: A list of insert strings.
     """
     with CSVFile(path) as f:
         for row in f.rows:
             # Create a dict with the names and values for insertion convertion
             yield insertion_func(table_name, __row_to_header_row_dict(f.header, row))
 
 
-def csv_as_updates(path: str | Path, table_name: str, update_func: Callable = update):
+def csv_to_updates(path: str | Path, table_name: str, update_func: Callable = update):
     """
     A generator yielding the rows of a given csv file as updatet statements.
     :param path: The path of the csv file to target.
     :param table_name: The name of the table in the update statement.
     :update_func: The name of the function used to construct the update statement (varying by dialect).
     """
     with CSVFile(path) as f:
@@ -87,11 +87,11 @@
             # Create a dict with the column names and update values.
             yield update_func(table_name, __row_to_header_row_dict(f.header, row))
 
 if __name__ == '__main__':
     # def csv_to_updates(path: str | Path, table_name: str, update_func: Callable = update):
     test_path = "C:/Users/AlistairKellaway/Downloads/snakes_count_100.csv"
 
-    print(list(csv_as_inserts(test_path, "table_name", insertion_func=insertion)))
-    print(up := list(csv_as_updates(test_path, "table_name", update_func=update)))
+    print(list(csv_to_inserts(test_path, "table_name", insertion_func=insertion)))
+    print(up := list(csv_to_updates(test_path, "table_name", update_func=update)))
     for u in up:
         print(u)
```

### Comparing `sqlstrings-0.0.6/src/sqlstrings/postgre.py` & `sqlstrings-0.0.7/sqlstrings/postgre.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from value_handling import value_writer
+from sqlstrings.value_handling import write_val
 import logging
 from typing import Any
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 def insertion(table_name: str, names_values: dict[str:str] | list[dict[str:str]]) -> str:
@@ -10,15 +10,15 @@
     Generates an insert statement for a postgre sql database.
     :param table_name: The name of the table to insert into.
     :param names_values: A dictionary or list of dictionaries with names of the columns and the values mapped to each column.
     :return: A string insert statement able to insert the given information.
     """
     outstr = f'INSERT INTO {table_name}\n'
     def args_serialise(value_dict): return ", ".join(
-        map(lambda v: f'{value_writer(v)}', value_dict.values()))
+        map(lambda v: f'{write_val(v)}', value_dict.values()))
     if isinstance(names_values, list):
         names = names_values[0].keys()
         values_str = ", \n\t".join(
             map(lambda d: f'({args_serialise(d)})', names_values))
     elif isinstance(names_values, dict):
         names = names_values.keys()
         values_str = f'({args_serialise(names_values)})'
@@ -34,15 +34,15 @@
     :param table_name: The name of the table to update.
     :param names_values: A dict mapping the names of the columns to update to the values to update them to.
     :param where: A string of conditionals which will be used to filter the tuples to update.
     :return: A string that can be used to update the table <table_name> with the values given in a postgre db.
     """
     outstr = f'UPDATE {table_name}\nSET '
     outstr += ",\n    ".join(
-        map(lambda kvp: f'{kvp[0]} = {value_writer(kvp[1])}', names_values.items()))
+        map(lambda kvp: f'{kvp[0]} = {write_val(kvp[1])}', names_values.items()))
     if where is not None:
         outstr += f'\nWHERE {where};'
     logger.debug(f'Created {__name__} update:\n{outstr}')
     return outstr
 
 
 def create_table(table_name: str, names_types: dict[str:str]) -> str:
@@ -60,15 +60,15 @@
 
 def procedure_call(proc_name: str, param_args: dict[str:Any]) -> str:
     """
     Generates a string that can be used to call a procedure of a given name with the given arguments when executed.
     :param proc_name: The name of the procedure to call.
     :param param_args: The names of the parameters mapped to their respective values.
     """
-    outstr = f'CALL {proc_name}({", ".join(map(lambda kvp: value_writer(kvp[1]), param_args.items()))});'
+    outstr = f'CALL {proc_name}({", ".join(map(lambda kvp: write_val(kvp[1]), param_args.items()))});'
     logging.debug(f'Created {__name__} proceduce call:\n{outstr}')
     return outstr
 
 
 def drop_table(table_names: str | list, if_exists: bool = False, cascade: bool = False, restrict: bool = False):
     """
     Generates a string that can be used to drop a table given its name (or multiple tables when given a list of names) when executed.
```

### Comparing `sqlstrings-0.0.6/src/sqlstrings/transact.py` & `sqlstrings-0.0.7/sqlstrings/transact.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 import logging
-from value_handling import value_reader, value_writer
+from sqlstrings.value_handling import write_val
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
 def insertion(table_name: str, names_values: dict[str:Any]) -> str:
     """
@@ -12,15 +12,15 @@
     to the values to insert.
     :param table_name: The name of the table to insert into.
     :param names_value: A dictionary mapping the names of the columns to the values to insert.
     :return: A string which can be used to insert the values given into a table of name table_name
     into a SQL database.
     """
     def f(collection): return ", ".join(
-        map(lambda n: f'{value_writer(n)}', collection))
+        map(lambda n: f'{write_val(n)}', collection))
     outstr = f'INSERT INTO {table_name} ({f(names_values.keys())})\n'
     outstr += f'VALUES ({f(names_values.values())});'
     logger.debug(f'Created {__name__} insert statement:\n{outstr}')
     return outstr
 
 
 def procedure_call(proc_name: str, names_vals: dict[str:Any]) -> str:
@@ -28,15 +28,15 @@
     Generates a string which can be used to execute a procedure of a given name with given parameters.
     :param proc_name: The name of the stored procedure to execute.
     :param names_vals: A dictionary mapping the parameter names to the argument values.
     :return: A string which can be used to call a stored procedure on a SQL database.
     """
     outstr = f'EXEC {proc_name} '
     outstr += ", ".join(
-        map(lambda kvp: f'@{kvp[0]} = {value_writer(kvp[1])}', names_vals.items())) + ";"
+        map(lambda kvp: f'@{kvp[0]} = {write_val(kvp[1])}', names_vals.items())) + ";"
             # kvp: keyvaluepair
     logger.debug(f'Created {__name__} proc call:\n{outstr}')
     return outstr
 
 
 def create_table(table_name: str, col_names_types: dict[str:str]) -> str:
     """
@@ -71,15 +71,15 @@
     :param table_name: A string containing the name of the table to update.
     :param names_values: A dictionary mapping the column names to update to the replacement values.
     :param where: A string containing the where condition logic.
     :return: A string which can be used to update a table in a SQL database.
     """
     outstr = f'UPDATE {table_name}\nSET '
     outstr += ", ".join(
-        map(lambda kvp: f'{kvp[0]} = {value_writer(kvp[1])}', names_values.items()))
+        map(lambda kvp: f'{kvp[0]} = {write_val(kvp[1])}', names_values.items()))
     # keyvaluepair
     outstr = outstr + (";" if where is None else f'\nWHERE {where};')
     logger.debug(f'Created {__name__} update statement:\n{outstr}')
     return outstr
 
 
 if __name__ == '__main__':
```

### Comparing `sqlstrings-0.0.6/src/sqlstrings/value_handling.py` & `sqlstrings-0.0.7/sqlstrings/value_handling.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import logging
 from typing import Any
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
-NULL_SET = ("NONE", "NULL")  # The set of strings that will be represented as None by Python.
+# The set of strings that will be represented as None by Python.
+NULL_SET = ("NONE", "NULL")
 NULL_TOK = "NULL"  # The string used as the null token in output strings.
 SPECIAL_CHAR_SET = ("\"")  # The list of special characters in the SQL dialect
 ESC_CHAR = "\\"  # The escape character used in the dialect.
 
-def value_writer(value: Any) -> str:
+
+def write_val(value: Any) -> str:
     """
     Takes an object and converts it into a string which a SQL compiler could interpret.
     :param value: A Python object which is to be converted into a string.
     :return: A string representation of an object which can be understood by a SQL compiler.
     """
     if value is None or value == NULL_TOK:
         return NULL_TOK
     if isinstance(value, str):
         return f'"{esc_special_chars(value)}"'
     if isinstance(value, int) or isinstance(value, float):
         return f'{value}'
     raise NotImplemented("Unable to handle input of type: " + str(type(value)))
 
 
-def value_reader(value: str) -> Any:
+def read_val(value: str) -> Any:
     """
     Aims to read strings from csv files and convert them into Python object for correct operation.
     :param value: The string to attempt to convert.
     :return: A python object representing the input value, if possible and supported.
     """
     if not isinstance(value, str):
         return value
@@ -49,12 +51,11 @@
     return esc_special_chars(value)
 
 
 def esc_special_chars(value: str) -> str:
     for c in SPECIAL_CHAR_SET:
         value = value.replace(f'{c}', f'{ESC_CHAR}{c}')
     return value
-    
 
 
 if __name__ == '__main__':
-    print(value_reader("\"NULL\""))
+    print(read_val("\"NULL\""))
```

### Comparing `sqlstrings-0.0.6/tests/test_postgre.py` & `sqlstrings-0.0.7/tests/test_postgre.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from sys import path
 
-path.append("sqltools")
+path.append("sqlstrings")
 
 import postgre
 
 class TestPostgre(unittest.TestCase):
 
     def test_insertion(self):
         names_values = {
```

### Comparing `sqlstrings-0.0.6/tests/test_transact.py` & `sqlstrings-0.0.7/tests/test_transact.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from sys import path
 
-path.append("sqltools")
+path.append("sqlstrings")
 
 import transact
 
 class TestTransact(unittest.TestCase):
 
     def test_insertion(self):
         names_values = {
```

### Comparing `sqlstrings-0.0.6/tests/test_value_handling.py` & `sqlstrings-0.0.7/tests/test_value_handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from sys import path
 
-path.append("sqltools")
+path.append("sqlstrings")
 
 import value_handling as vh
 
 class TestValueHandling(unittest.TestCase):
 
     # value writer tests
```

