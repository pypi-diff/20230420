# Comparing `tmp/qabot-0.3.3.tar.gz` & `tmp/qabot-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qabot-0.3.3.tar", max compression
+gzip compressed data, was "qabot-0.3.4.tar", max compression
```

## Comparing `qabot-0.3.3.tar` & `qabot-0.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-03-27 21:19:57.134744 qabot-0.3.3/LICENSE
--rw-r--r--   0        0        0     5039 2023-04-12 02:14:39.645321 qabot-0.3.3/README.md
--rw-r--r--   0        0        0      711 2023-04-12 02:30:40.274395 qabot-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      709 2023-04-12 01:11:09.111570 qabot-0.3.3/qabot/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 21:48:52.942092 qabot-0.3.3/qabot/agents/__init__.py
--rw-r--r--   0        0        0     4495 2023-04-12 02:30:40.262395 qabot-0.3.3/qabot/agents/agent.py
--rw-r--r--   0        0        0    10860 2023-04-12 02:00:21.625211 qabot-0.3.3/qabot/agents/data_query_chain.py
--rw-r--r--   0        0        0     1707 2023-03-27 21:19:57.138745 qabot-0.3.3/qabot/caching.py
--rw-r--r--   0        0        0     6471 2023-04-12 02:06:49.481090 qabot-0.3.3/qabot/cli.py
--rw-r--r--   0        0        0      390 2023-04-12 02:06:49.469090 qabot-0.3.3/qabot/config.py
--rw-r--r--   0        0        0     3378 2023-03-27 21:34:35.864207 qabot-0.3.3/qabot/duckdb_manual_data_loader.py
--rw-r--r--   0        0        0     1339 2023-04-12 02:28:36.278238 qabot-0.3.3/qabot/duckdb_query.py
--rw-r--r--   0        0        0     2555 2023-04-12 00:25:15.975882 qabot-0.3.3/qabot/progress_callback.py
--rw-r--r--   0        0        0        0 2023-03-06 20:20:33.902705 qabot-0.3.3/qabot/tools/__init__.py
--rw-r--r--   0        0        0      518 2023-03-27 21:19:57.138745 qabot-0.3.3/qabot/tools/describe_duckdb_table.py
--rw-r--r--   0        0        0     1027 2023-03-27 21:19:57.138745 qabot-0.3.3/qabot/tools/duckdb_execute_tool.py
--rw-r--r--   0        0        0     2681 2023-04-11 22:19:46.181702 qabot-0.3.3/qabot/tools/wikidata.py
--rw-r--r--   0        0        0     5790 1970-01-01 00:00:00.000000 qabot-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-27 21:19:57.134744 qabot-0.3.4/LICENSE
+-rw-r--r--   0        0        0     4973 2023-04-12 02:34:48.430716 qabot-0.3.4/README.md
+-rw-r--r--   0        0        0      711 2023-04-20 01:33:03.884435 qabot-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      709 2023-04-12 01:11:09.111570 qabot-0.3.4/qabot/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-08 21:48:52.942092 qabot-0.3.4/qabot/agents/__init__.py
+-rw-r--r--   0        0        0     4495 2023-04-12 02:30:40.262395 qabot-0.3.4/qabot/agents/agent.py
+-rw-r--r--   0        0        0    10860 2023-04-12 02:00:21.625211 qabot-0.3.4/qabot/agents/data_query_chain.py
+-rw-r--r--   0        0        0     1707 2023-03-27 21:19:57.138745 qabot-0.3.4/qabot/caching.py
+-rw-r--r--   0        0        0     6460 2023-04-20 01:20:40.603304 qabot-0.3.4/qabot/cli.py
+-rw-r--r--   0        0        0      382 2023-04-20 01:29:14.747387 qabot-0.3.4/qabot/config.py
+-rw-r--r--   0        0        0     3425 2023-04-20 01:21:13.183016 qabot-0.3.4/qabot/duckdb_manual_data_loader.py
+-rw-r--r--   0        0        0     1339 2023-04-12 02:28:36.278238 qabot-0.3.4/qabot/duckdb_query.py
+-rw-r--r--   0        0        0     2555 2023-04-12 00:25:15.975882 qabot-0.3.4/qabot/progress_callback.py
+-rw-r--r--   0        0        0        0 2023-03-06 20:20:33.902705 qabot-0.3.4/qabot/tools/__init__.py
+-rw-r--r--   0        0        0      518 2023-03-27 21:19:57.138745 qabot-0.3.4/qabot/tools/describe_duckdb_table.py
+-rw-r--r--   0        0        0     1027 2023-03-27 21:19:57.138745 qabot-0.3.4/qabot/tools/duckdb_execute_tool.py
+-rw-r--r--   0        0        0     2681 2023-04-11 22:19:46.181702 qabot-0.3.4/qabot/tools/wikidata.py
+-rw-r--r--   0        0        0     5724 1970-01-01 00:00:00.000000 qabot-0.3.4/PKG-INFO
```

### Comparing `qabot-0.3.3/LICENSE` & `qabot-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qabot-0.3.3/README.md` & `qabot-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,14 @@
 - [Agent docs to talk to arbitrary apis via OpenAPI/Swagger](https://langchain.readthedocs.io/en/latest/modules/agents/agent_toolkits/openapi.html)
 - [Agents/Tools to talk SQL](https://langchain.readthedocs.io/en/latest/modules/agents/agent_toolkits/sql_database.html)
 - [Typescript library](https://hwchase17.github.io/langchainjs/docs/overview/)
 
 
 ## Ideas
 
-- Decent Python Library API so can be used from other Python code
 - streaming mode to output results as they come in
 - token limits
 - Supervisor agent - assess whether a query is "safe" to run, could ask for user confirmation to run anything that gets flagged.
 - Often we can zero-shot the question and get a single query out - perhaps we try this before the MKL chain
 - test each zeroshot agent individually
 - Generate and pass back assumptions made to the user
 - Add an optional "clarify" tool to the chain that asks the user to clarify the question
```

### Comparing `qabot-0.3.3/pyproject.toml` & `qabot-0.3.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "qabot"
-version = "0.3.3"
+version = "0.3.4"
 license = "Apache-2.0"
 description = "Query local or remote data files with natural language queries powered by OpenAI and DuckDB."
 authors = ["Brian Thorne <brian@hardbyte.nz>"]
 readme = "README.md"
 packages = [{include = "qabot"}]
 
 [tool.poetry.scripts]
 qabot = "qabot.cli:run"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-langchain = "^0.0.137"
+langchain = "^0.0.144"
 openai = "^0.27.4"
 duckdb = "^0.7.1"
 typer = "^0.7.0"
 rich = "^13.3.3"
 httpx = "^0.24.0"
```

### Comparing `qabot-0.3.3/qabot/__init__.py` & `qabot-0.3.4/qabot/__init__.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.3/qabot/agents/agent.py` & `qabot-0.3.4/qabot/agents/agent.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.3/qabot/agents/data_query_chain.py` & `qabot-0.3.4/qabot/agents/data_query_chain.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.3/qabot/caching.py` & `qabot-0.3.4/qabot/caching.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.3/qabot/cli.py` & `qabot-0.3.4/qabot/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     executed_sql = ''
     # If files are given load data into local DuckDB
     database_engine = create_duckdb(database_uri)
 
     if len(file) > 0:
         if isinstance(file, str):
             file = [file]
-        print("[red]🦆[/red] [bold]Loading data from files...[/bold]")
+        print("[red]🦆[/red] [bold]Loading data...[/bold]")
         database_engine, executed_sql = import_into_duckdb_from_files(database_engine, file)
         executed_sql = '\n'.join(executed_sql)
     else:
         print("[red]🦆[/red]")
 
     with Progress(
         SpinnerColumn(),
```

### Comparing `qabot-0.3.3/qabot/duckdb_manual_data_loader.py` & `qabot-0.3.4/qabot/duckdb_manual_data_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,39 +21,36 @@
     # persistent storage
 
     duckdb_connection = duckdb.connect(duckdb_path)
     try:
         duckdb_connection.sql("INSTALL httpfs;")
         duckdb_connection.sql("LOAD httpfs;")
     except Exception:
-        print("Failed to install httpfs extension. Only loading from local files will be supported")
+        print("Failed to install httpfs extension. Loading remote files will not be supported")
+
+    try:
+        duckdb_connection.sql("INSTALL postgres_scanner;")
+        duckdb_connection.sql("LOAD postgres_scanner;")
+    except Exception:
+        print("Failed to install postgres_scanner extension. Loading directly from postgresql will not be supported")
 
     duckdb_connection.sql("create table if not exists qabot_queries(query VARCHAR, timestamp TIMESTAMP DEFAULT CURRENT_TIMESTAMP);")
 
     return duckdb_connection
 
 
 def import_into_duckdb_from_files(duckdb_connection: duckdb.DuckDBPyConnection, files: list[str]) -> Tuple[duckdb.DuckDBPyConnection, list[str]]:
 
     executed_sql = []
     for i, file_path in enumerate(files, 1):
 
-        executed_sql.append(load_external_data_into_db(duckdb_connection, file_path))
-
-        # Alternative is to allow user to pass in column types:
-        # conn.sql(f"""
-        # create table {table_name} as (
-        #     select * from read_csv_auto(
-        #         '%s',
-        #         delim='|',
-        #         header=True,
-        #         --types={'phone': 'VARCHAR'}
-        #     )
-        # )
-        # """ % file_path)
+        if file_path.startswith("postgresql://"):
+            duckdb_connection.execute(f"CALL postgres_attach('{file_path}')")
+        else:
+            executed_sql.append(load_external_data_into_db(duckdb_connection, file_path))
 
     return duckdb_connection, executed_sql
 
 
 def load_external_data_into_db(conn: duckdb.DuckDBPyConnection, file_path, allow_view=True):
     # Work out if the filepath is actually a url (e.g. s3://)
     is_url = uri_validator(file_path)
```

### Comparing `qabot-0.3.3/qabot/duckdb_query.py` & `qabot-0.3.4/qabot/duckdb_query.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.3/qabot/progress_callback.py` & `qabot-0.3.4/qabot/progress_callback.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.3/qabot/tools/describe_duckdb_table.py` & `qabot-0.3.4/qabot/tools/describe_duckdb_table.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.3/qabot/tools/duckdb_execute_tool.py` & `qabot-0.3.4/qabot/tools/duckdb_execute_tool.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.3/qabot/tools/wikidata.py` & `qabot-0.3.4/qabot/tools/wikidata.py`

 * *Files identical despite different names*

### Comparing `qabot-0.3.3/PKG-INFO` & `qabot-0.3.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: qabot
-Version: 0.3.3
+Version: 0.3.4
 Summary: Query local or remote data files with natural language queries powered by OpenAI and DuckDB.
 License: Apache-2.0
 Author: Brian Thorne
 Author-email: brian@hardbyte.nz
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: duckdb (>=0.7.1,<0.8.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
-Requires-Dist: langchain (>=0.0.137,<0.0.138)
+Requires-Dist: langchain (>=0.0.144,<0.0.145)
 Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # qabot
 
@@ -159,15 +159,14 @@
 - [Agent docs to talk to arbitrary apis via OpenAPI/Swagger](https://langchain.readthedocs.io/en/latest/modules/agents/agent_toolkits/openapi.html)
 - [Agents/Tools to talk SQL](https://langchain.readthedocs.io/en/latest/modules/agents/agent_toolkits/sql_database.html)
 - [Typescript library](https://hwchase17.github.io/langchainjs/docs/overview/)
 
 
 ## Ideas
 
-- Decent Python Library API so can be used from other Python code
 - streaming mode to output results as they come in
 - token limits
 - Supervisor agent - assess whether a query is "safe" to run, could ask for user confirmation to run anything that gets flagged.
 - Often we can zero-shot the question and get a single query out - perhaps we try this before the MKL chain
 - test each zeroshot agent individually
 - Generate and pass back assumptions made to the user
 - Add an optional "clarify" tool to the chain that asks the user to clarify the question
```

