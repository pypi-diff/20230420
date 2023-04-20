# Comparing `tmp/leaguedaily-0.2.0.tar.gz` & `tmp/leaguedaily-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leaguedaily-0.2.0.tar", max compression
+gzip compressed data, was "leaguedaily-0.2.1.tar", max compression
```

## Comparing `leaguedaily-0.2.0.tar` & `leaguedaily-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-03-17 22:02:03.580299 leaguedaily-0.2.0/LICENSE
--rw-r--r--   0        0        0     2111 2023-04-20 14:15:46.411844 leaguedaily-0.2.0/README.md
--rw-r--r--   0        0        0      828 2023-04-20 14:17:28.236863 leaguedaily-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-24 17:34:16.118879 leaguedaily-0.2.0/src/__init__.py
--rw-r--r--   0        0        0     5925 2023-04-20 14:11:39.837378 leaguedaily-0.2.0/src/daily_update.py
--rw-r--r--   0        0        0     4407 2023-04-07 23:07:09.100211 leaguedaily-0.2.0/src/display.py
--rw-r--r--   0        0        0     3208 2023-04-20 14:11:49.405474 leaguedaily-0.2.0/src/main.py
--rw-r--r--   0        0        0     1055 2023-04-07 23:11:08.974744 leaguedaily-0.2.0/src/match.py
--rw-r--r--   0        0        0      672 2023-04-07 18:15:32.361055 leaguedaily-0.2.0/src/result.py
--rw-r--r--   0        0        0     2110 2023-04-20 14:11:54.537525 leaguedaily-0.2.0/src/team.py
--rw-r--r--   0        0        0     1747 2023-04-07 22:52:10.094716 leaguedaily-0.2.0/src/util.py
--rw-r--r--   0        0        0     3218 1970-01-01 00:00:00.000000 leaguedaily-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-17 22:02:03.580299 leaguedaily-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2112 2023-04-20 14:32:46.302045 leaguedaily-0.2.1/README.md
+-rw-r--r--   0        0        0      827 2023-04-20 14:33:47.714659 leaguedaily-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-24 17:34:16.118879 leaguedaily-0.2.1/src/__init__.py
+-rw-r--r--   0        0        0     5925 2023-04-20 14:11:39.837378 leaguedaily-0.2.1/src/daily_update.py
+-rw-r--r--   0        0        0     4407 2023-04-07 23:07:09.100211 leaguedaily-0.2.1/src/display.py
+-rw-r--r--   0        0        0     3208 2023-04-20 14:11:49.405474 leaguedaily-0.2.1/src/main.py
+-rw-r--r--   0        0        0     1055 2023-04-07 23:11:08.974744 leaguedaily-0.2.1/src/match.py
+-rw-r--r--   0        0        0      672 2023-04-07 18:15:32.361055 leaguedaily-0.2.1/src/result.py
+-rw-r--r--   0        0        0     2110 2023-04-20 14:11:54.537525 leaguedaily-0.2.1/src/team.py
+-rw-r--r--   0        0        0     1747 2023-04-07 22:52:10.094716 leaguedaily-0.2.1/src/util.py
+-rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 leaguedaily-0.2.1/PKG-INFO
```

### Comparing `leaguedaily-0.2.0/LICENSE` & `leaguedaily-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.0/README.md` & `leaguedaily-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 requirement: `python3 >= 3.10`
 
 
 `pip install leaguedaily`
 
 # Usage
 
-By default, `league-daily` without any arguments will show League of Legends Esports result from the previous day.
+By default, `leaguedaily` without any arguments will show League of Legends Esports result from the previous day.
 
 <img width="638" alt="Screenshot 2023-04-19 at 8 00 06 PM" src="https://user-images.githubusercontent.com/60205090/233247146-f660c989-8cae-41a2-9360-0c60b13ee694.png">
 
 You can also specify dates in the format of `YYYY-MM-DD` as an argument to the program.
 
 <img width="878" alt="Screenshot 2023-04-19 at 8 05 28 PM" src="https://user-images.githubusercontent.com/60205090/233247879-074f620d-b2fd-4a26-a836-3d853a5ad27b.png">
 
@@ -33,9 +33,9 @@
 
 # Known problems
 
 1. Data is pulled from leaguepedia, so there is a limit as to how much data a normal user can pull. As a result, given a too-far-away-from-present date, program's result could be truncated or incorrect.
 2. A BO3 series could be in the same day in local time, but in UTC (default time when pulled from API), 2 matches are on the same day and 1 match is on the next day (past midnight UTC time, but still the same day local time). 
 
 Given the goal of this project (daily update for some busy fans), I decide not to address these problems. The program works consistently enough for what it is created for.
-
+SS
 Cheers! 🎆
```

### Comparing `leaguedaily-0.2.0/pyproject.toml` & `leaguedaily-0.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "leaguedaily"
-version = "0.2.0"
+version = "0.2.1"
 description = "League of Legends Esports results from your terminal!"
 authors = ["Hieu Vuong <tvuong5@dons.usfca.edu>"]
 readme = "README.md"
 packages = [
     {include = "src"}
 ]
 
 [tool.poetry.scripts]
-league-daily = "src.main:app"
+leaguedaily = "src.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = "0.7.0"
 certifi = "2022.12.7"
 charset-normalizer = "3.1.0"
 click = "8.1.3"
```

### Comparing `leaguedaily-0.2.0/src/daily_update.py` & `leaguedaily-0.2.1/src/daily_update.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.0/src/display.py` & `leaguedaily-0.2.1/src/display.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.0/src/main.py` & `leaguedaily-0.2.1/src/main.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.0/src/match.py` & `leaguedaily-0.2.1/src/match.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.0/src/result.py` & `leaguedaily-0.2.1/src/result.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.0/src/team.py` & `leaguedaily-0.2.1/src/team.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.0/src/util.py` & `leaguedaily-0.2.1/src/util.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.0/PKG-INFO` & `leaguedaily-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leaguedaily
-Version: 0.2.0
+Version: 0.2.1
 Summary: League of Legends Esports results from your terminal!
 Author: Hieu Vuong
 Author-email: tvuong5@dons.usfca.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -40,15 +40,15 @@
 requirement: `python3 >= 3.10`
 
 
 `pip install leaguedaily`
 
 # Usage
 
-By default, `league-daily` without any arguments will show League of Legends Esports result from the previous day.
+By default, `leaguedaily` without any arguments will show League of Legends Esports result from the previous day.
 
 <img width="638" alt="Screenshot 2023-04-19 at 8 00 06 PM" src="https://user-images.githubusercontent.com/60205090/233247146-f660c989-8cae-41a2-9360-0c60b13ee694.png">
 
 You can also specify dates in the format of `YYYY-MM-DD` as an argument to the program.
 
 <img width="878" alt="Screenshot 2023-04-19 at 8 05 28 PM" src="https://user-images.githubusercontent.com/60205090/233247879-074f620d-b2fd-4a26-a836-3d853a5ad27b.png">
 
@@ -65,10 +65,10 @@
 
 # Known problems
 
 1. Data is pulled from leaguepedia, so there is a limit as to how much data a normal user can pull. As a result, given a too-far-away-from-present date, program's result could be truncated or incorrect.
 2. A BO3 series could be in the same day in local time, but in UTC (default time when pulled from API), 2 matches are on the same day and 1 match is on the next day (past midnight UTC time, but still the same day local time). 
 
 Given the goal of this project (daily update for some busy fans), I decide not to address these problems. The program works consistently enough for what it is created for.
-
+SS
 Cheers! 🎆
```

