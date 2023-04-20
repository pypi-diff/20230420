# Comparing `tmp/leaguedaily-0.2.1.tar.gz` & `tmp/leaguedaily-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leaguedaily-0.2.1.tar", max compression
+gzip compressed data, was "leaguedaily-1.0.0.tar", max compression
```

## Comparing `leaguedaily-0.2.1.tar` & `leaguedaily-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-03-17 22:02:03.580299 leaguedaily-0.2.1/LICENSE
--rw-r--r--   0        0        0     2112 2023-04-20 14:32:46.302045 leaguedaily-0.2.1/README.md
--rw-r--r--   0        0        0      827 2023-04-20 14:33:47.714659 leaguedaily-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-24 17:34:16.118879 leaguedaily-0.2.1/src/__init__.py
--rw-r--r--   0        0        0     5925 2023-04-20 14:11:39.837378 leaguedaily-0.2.1/src/daily_update.py
--rw-r--r--   0        0        0     4407 2023-04-07 23:07:09.100211 leaguedaily-0.2.1/src/display.py
--rw-r--r--   0        0        0     3208 2023-04-20 14:11:49.405474 leaguedaily-0.2.1/src/main.py
--rw-r--r--   0        0        0     1055 2023-04-07 23:11:08.974744 leaguedaily-0.2.1/src/match.py
--rw-r--r--   0        0        0      672 2023-04-07 18:15:32.361055 leaguedaily-0.2.1/src/result.py
--rw-r--r--   0        0        0     2110 2023-04-20 14:11:54.537525 leaguedaily-0.2.1/src/team.py
--rw-r--r--   0        0        0     1747 2023-04-07 22:52:10.094716 leaguedaily-0.2.1/src/util.py
--rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 leaguedaily-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-17 22:02:03.580299 leaguedaily-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1837 2023-04-20 14:48:45.823642 leaguedaily-1.0.0/README.md
+-rw-r--r--   0        0        0      827 2023-04-20 14:49:23.548019 leaguedaily-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-24 17:34:16.118879 leaguedaily-1.0.0/src/__init__.py
+-rw-r--r--   0        0        0     5925 2023-04-20 14:11:39.837378 leaguedaily-1.0.0/src/daily_update.py
+-rw-r--r--   0        0        0     4407 2023-04-07 23:07:09.100211 leaguedaily-1.0.0/src/display.py
+-rw-r--r--   0        0        0     3208 2023-04-20 14:11:49.405474 leaguedaily-1.0.0/src/main.py
+-rw-r--r--   0        0        0     1055 2023-04-07 23:11:08.974744 leaguedaily-1.0.0/src/match.py
+-rw-r--r--   0        0        0      672 2023-04-07 18:15:32.361055 leaguedaily-1.0.0/src/result.py
+-rw-r--r--   0        0        0     2110 2023-04-20 14:11:54.537525 leaguedaily-1.0.0/src/team.py
+-rw-r--r--   0        0        0     1747 2023-04-07 22:52:10.094716 leaguedaily-1.0.0/src/util.py
+-rw-r--r--   0        0        0     2944 1970-01-01 00:00:00.000000 leaguedaily-1.0.0/PKG-INFO
```

### Comparing `leaguedaily-0.2.1/LICENSE` & `leaguedaily-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.1/README.md` & `leaguedaily-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# league-daily
+# LeagueDaily
 
 Leauge of Legends Esports update straight from the terminal!
 
 Now you can stay up-to-date with your favorite LoL teams/leagues despite your busy schedule.
 # Install
 
 requirement: `python3 >= 3.10`
@@ -10,32 +10,31 @@
 
 `pip install leaguedaily`
 
 # Usage
 
 By default, `leaguedaily` without any arguments will show League of Legends Esports result from the previous day.
 
-<img width="638" alt="Screenshot 2023-04-19 at 8 00 06 PM" src="https://user-images.githubusercontent.com/60205090/233247146-f660c989-8cae-41a2-9360-0c60b13ee694.png">
+![Screenshot from 2023-04-20 07-43-17](https://user-images.githubusercontent.com/60205090/233401825-ff74f03d-7e29-4fc0-ad0c-9f1fb5639e72.png)
 
 You can also specify dates in the format of `YYYY-MM-DD` as an argument to the program.
 
-<img width="878" alt="Screenshot 2023-04-19 at 8 05 28 PM" src="https://user-images.githubusercontent.com/60205090/233247879-074f620d-b2fd-4a26-a836-3d853a5ad27b.png">
+![Screenshot from 2023-04-20 07-41-48](https://user-images.githubusercontent.com/60205090/233401471-2f539f98-7a97-4dcc-a5a1-5a292ff9d77d.png)
 
 
 `--team` flag can be used to specify one or more teams in addition to the given date argument.
 
-<img width="574" alt="Screenshot 2023-04-19 at 8 08 03 PM" src="https://user-images.githubusercontent.com/60205090/233248250-c9a32b79-53be-4f7c-9415-c57f6e85ade5.png">
-<img width="730" alt="Screenshot 2023-04-19 at 8 08 51 PM" src="https://user-images.githubusercontent.com/60205090/233248406-3f666713-be6b-4128-aaa3-855db1ef6a4d.png">
+![Screenshot from 2023-04-20 07-45-08](https://user-images.githubusercontent.com/60205090/233402355-e9d1c5ce-2a57-47a3-bfcd-23bf0bb4cf02.png)
 
-`--league` flag can be used to limit the results to only the given leagues.
 
-<img width="859" alt="Screenshot 2023-04-19 at 8 12 15 PM" src="https://user-images.githubusercontent.com/60205090/233248886-ce80d938-f530-43ad-b078-dc7331f52614.png">
+`--league` flag can be used to limit the results to only the given leagues.
 
+![Screenshot from 2023-04-20 07-46-33](https://user-images.githubusercontent.com/60205090/233402764-f5ec7044-8899-4bc1-a7c6-2b442acddb5d.png)
 
 # Known problems
 
 1. Data is pulled from leaguepedia, so there is a limit as to how much data a normal user can pull. As a result, given a too-far-away-from-present date, program's result could be truncated or incorrect.
 2. A BO3 series could be in the same day in local time, but in UTC (default time when pulled from API), 2 matches are on the same day and 1 match is on the next day (past midnight UTC time, but still the same day local time). 
 
 Given the goal of this project (daily update for some busy fans), I decide not to address these problems. The program works consistently enough for what it is created for.
-SS
+
 Cheers! 🎆
```

### Comparing `leaguedaily-0.2.1/pyproject.toml` & `leaguedaily-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leaguedaily"
-version = "0.2.1"
+version = "1.0.0"
 description = "League of Legends Esports results from your terminal!"
 authors = ["Hieu Vuong <tvuong5@dons.usfca.edu>"]
 readme = "README.md"
 packages = [
     {include = "src"}
 ]
```

### Comparing `leaguedaily-0.2.1/src/daily_update.py` & `leaguedaily-1.0.0/src/daily_update.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.1/src/display.py` & `leaguedaily-1.0.0/src/display.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.1/src/main.py` & `leaguedaily-1.0.0/src/main.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.1/src/match.py` & `leaguedaily-1.0.0/src/match.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.1/src/result.py` & `leaguedaily-1.0.0/src/result.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.1/src/team.py` & `leaguedaily-1.0.0/src/team.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.1/src/util.py` & `leaguedaily-1.0.0/src/util.py`

 * *Files identical despite different names*

### Comparing `leaguedaily-0.2.1/PKG-INFO` & `leaguedaily-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leaguedaily
-Version: 0.2.1
+Version: 1.0.0
 Summary: League of Legends Esports results from your terminal!
 Author: Hieu Vuong
 Author-email: tvuong5@dons.usfca.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -26,15 +26,15 @@
 Requires-Dist: six (==1.16.0)
 Requires-Dist: typer (==0.7.0)
 Requires-Dist: tzdata (==2022.7)
 Requires-Dist: tzlocal (==4.2)
 Requires-Dist: urllib3 (==1.26.15)
 Description-Content-Type: text/markdown
 
-# league-daily
+# LeagueDaily
 
 Leauge of Legends Esports update straight from the terminal!
 
 Now you can stay up-to-date with your favorite LoL teams/leagues despite your busy schedule.
 # Install
 
 requirement: `python3 >= 3.10`
@@ -42,33 +42,32 @@
 
 `pip install leaguedaily`
 
 # Usage
 
 By default, `leaguedaily` without any arguments will show League of Legends Esports result from the previous day.
 
-<img width="638" alt="Screenshot 2023-04-19 at 8 00 06 PM" src="https://user-images.githubusercontent.com/60205090/233247146-f660c989-8cae-41a2-9360-0c60b13ee694.png">
+![Screenshot from 2023-04-20 07-43-17](https://user-images.githubusercontent.com/60205090/233401825-ff74f03d-7e29-4fc0-ad0c-9f1fb5639e72.png)
 
 You can also specify dates in the format of `YYYY-MM-DD` as an argument to the program.
 
-<img width="878" alt="Screenshot 2023-04-19 at 8 05 28 PM" src="https://user-images.githubusercontent.com/60205090/233247879-074f620d-b2fd-4a26-a836-3d853a5ad27b.png">
+![Screenshot from 2023-04-20 07-41-48](https://user-images.githubusercontent.com/60205090/233401471-2f539f98-7a97-4dcc-a5a1-5a292ff9d77d.png)
 
 
 `--team` flag can be used to specify one or more teams in addition to the given date argument.
 
-<img width="574" alt="Screenshot 2023-04-19 at 8 08 03 PM" src="https://user-images.githubusercontent.com/60205090/233248250-c9a32b79-53be-4f7c-9415-c57f6e85ade5.png">
-<img width="730" alt="Screenshot 2023-04-19 at 8 08 51 PM" src="https://user-images.githubusercontent.com/60205090/233248406-3f666713-be6b-4128-aaa3-855db1ef6a4d.png">
+![Screenshot from 2023-04-20 07-45-08](https://user-images.githubusercontent.com/60205090/233402355-e9d1c5ce-2a57-47a3-bfcd-23bf0bb4cf02.png)
 
-`--league` flag can be used to limit the results to only the given leagues.
 
-<img width="859" alt="Screenshot 2023-04-19 at 8 12 15 PM" src="https://user-images.githubusercontent.com/60205090/233248886-ce80d938-f530-43ad-b078-dc7331f52614.png">
+`--league` flag can be used to limit the results to only the given leagues.
 
+![Screenshot from 2023-04-20 07-46-33](https://user-images.githubusercontent.com/60205090/233402764-f5ec7044-8899-4bc1-a7c6-2b442acddb5d.png)
 
 # Known problems
 
 1. Data is pulled from leaguepedia, so there is a limit as to how much data a normal user can pull. As a result, given a too-far-away-from-present date, program's result could be truncated or incorrect.
 2. A BO3 series could be in the same day in local time, but in UTC (default time when pulled from API), 2 matches are on the same day and 1 match is on the next day (past midnight UTC time, but still the same day local time). 
 
 Given the goal of this project (daily update for some busy fans), I decide not to address these problems. The program works consistently enough for what it is created for.
-SS
+
 Cheers! 🎆
```

