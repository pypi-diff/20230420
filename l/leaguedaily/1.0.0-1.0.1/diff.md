# Comparing `tmp/leaguedaily-1.0.0.tar.gz` & `tmp/leaguedaily-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leaguedaily-1.0.0.tar", max compression
+gzip compressed data, was "leaguedaily-1.0.1.tar", max compression
```

## Comparing `leaguedaily-1.0.0.tar` & `leaguedaily-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-03-17 22:02:03.580299 leaguedaily-1.0.0/LICENSE
--rw-r--r--   0        0        0     1837 2023-04-20 14:48:45.823642 leaguedaily-1.0.0/README.md
--rw-r--r--   0        0        0      827 2023-04-20 14:49:23.548019 leaguedaily-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-24 17:34:16.118879 leaguedaily-1.0.0/src/__init__.py
--rw-r--r--   0        0        0     5925 2023-04-20 14:11:39.837378 leaguedaily-1.0.0/src/daily_update.py
--rw-r--r--   0        0        0     4407 2023-04-07 23:07:09.100211 leaguedaily-1.0.0/src/display.py
--rw-r--r--   0        0        0     3208 2023-04-20 14:11:49.405474 leaguedaily-1.0.0/src/main.py
--rw-r--r--   0        0        0     1055 2023-04-07 23:11:08.974744 leaguedaily-1.0.0/src/match.py
--rw-r--r--   0        0        0      672 2023-04-07 18:15:32.361055 leaguedaily-1.0.0/src/result.py
--rw-r--r--   0        0        0     2110 2023-04-20 14:11:54.537525 leaguedaily-1.0.0/src/team.py
--rw-r--r--   0        0        0     1747 2023-04-07 22:52:10.094716 leaguedaily-1.0.0/src/util.py
--rw-r--r--   0        0        0     2944 1970-01-01 00:00:00.000000 leaguedaily-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-17 22:02:03.580299 leaguedaily-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1837 2023-04-20 14:48:45.823642 leaguedaily-1.0.1/README.md
+-rw-r--r--   0        0        0      827 2023-04-20 14:55:58.171966 leaguedaily-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-24 17:34:16.118879 leaguedaily-1.0.1/src/__init__.py
+-rw-r--r--   0        0        0     5925 2023-04-20 14:11:39.837378 leaguedaily-1.0.1/src/daily_update.py
+-rw-r--r--   0        0        0     4407 2023-04-07 23:07:09.100211 leaguedaily-1.0.1/src/display.py
+-rw-r--r--   0        0        0     3208 2023-04-20 14:11:49.405474 leaguedaily-1.0.1/src/main.py
+-rw-r--r--   0        0        0     1055 2023-04-07 23:11:08.974744 leaguedaily-1.0.1/src/match.py
+-rw-r--r--   0        0        0      672 2023-04-07 18:15:32.361055 leaguedaily-1.0.1/src/result.py
+-rw-r--r--   0        0        0     2110 2023-04-20 14:11:54.537525 leaguedaily-1.0.1/src/team.py
+-rw-r--r--   0        0        0     1747 2023-04-07 22:52:10.094716 leaguedaily-1.0.1/src/util.py
+-rw-r--r--   0        0        0     2944 1970-01-01 00:00:00.000000 leaguedaily-1.0.1/PKG-INFO
```

### Comparing `leaguedaily-1.0.0/LICENSE` & `leaguedaily-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `leaguedaily-1.0.0/README.md` & `leaguedaily-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `leaguedaily-1.0.0/pyproject.toml` & `leaguedaily-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "leaguedaily"
-version = "1.0.0"
+version = "1.0.1"
 description = "League of Legends Esports results from your terminal!"
-authors = ["Hieu Vuong <tvuong5@dons.usfca.edu>"]
+authors = ["Hieu Vuong <hieuvuong.cs@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "src"}
 ]
 
 [tool.poetry.scripts]
 leaguedaily = "src.main:app"
```

### Comparing `leaguedaily-1.0.0/src/daily_update.py` & `leaguedaily-1.0.1/src/daily_update.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-1.0.0/src/display.py` & `leaguedaily-1.0.1/src/display.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-1.0.0/src/main.py` & `leaguedaily-1.0.1/src/main.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-1.0.0/src/match.py` & `leaguedaily-1.0.1/src/match.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-1.0.0/src/result.py` & `leaguedaily-1.0.1/src/result.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-1.0.0/src/team.py` & `leaguedaily-1.0.1/src/team.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-1.0.0/src/util.py` & `leaguedaily-1.0.1/src/util.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-1.0.0/PKG-INFO` & `leaguedaily-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: leaguedaily
-Version: 1.0.0
+Version: 1.0.1
 Summary: League of Legends Esports results from your terminal!
 Author: Hieu Vuong
-Author-email: tvuong5@dons.usfca.edu
+Author-email: hieuvuong.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certifi (==2022.12.7)
 Requires-Dist: charset-normalizer (==3.1.0)
 Requires-Dist: click (==8.1.3)
```

