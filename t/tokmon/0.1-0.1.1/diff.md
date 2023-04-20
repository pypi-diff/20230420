# Comparing `tmp/tokmon-0.1.tar.gz` & `tmp/tokmon-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokmon-0.1.tar", last modified: Thu Apr 20 15:16:07 2023, max compression
+gzip compressed data, was "tokmon-0.1.1.tar", last modified: Thu Apr 20 15:22:41 2023, max compression
```

## Comparing `tokmon-0.1.tar` & `tokmon-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 yb         (501) staff       (20)        0 2023-04-20 15:16:07.985330 tokmon-0.1/
--rw-r--r--   0 yb         (501) staff       (20)    11336 2023-04-20 14:46:39.000000 tokmon-0.1/LICENSE
--rw-r--r--   0 yb         (501) staff       (20)      151 2023-04-20 15:16:07.985174 tokmon-0.1/PKG-INFO
--rw-r--r--   0 yb         (501) staff       (20)     6766 2023-04-20 14:46:39.000000 tokmon-0.1/README.md
--rw-r--r--   0 yb         (501) staff       (20)       38 2023-04-20 15:16:07.985378 tokmon-0.1/setup.cfg
--rw-r--r--   0 yb         (501) staff       (20)      360 2023-04-13 02:57:04.000000 tokmon-0.1/setup.py
-drwxr-xr-x   0 yb         (501) staff       (20)        0 2023-04-20 15:16:07.984135 tokmon-0.1/tokmon/
--rw-r--r--   0 yb         (501) staff       (20)        0 2023-04-13 01:47:04.000000 tokmon-0.1/tokmon/__init__.py
--rwxr-xr-x   0 yb         (501) staff       (20)     4777 2023-04-20 14:46:37.000000 tokmon-0.1/tokmon/cli.py
--rw-r--r--   0 yb         (501) staff       (20)     3370 2023-04-13 22:54:00.000000 tokmon-0.1/tokmon/costcalculator.py
--rw-r--r--   0 yb         (501) staff       (20)     1021 2023-04-12 21:37:44.000000 tokmon-0.1/tokmon/pricing.json
--rwxr-xr-x   0 yb         (501) staff       (20)     9244 2023-04-14 19:59:32.000000 tokmon-0.1/tokmon/tokmon.py
-drwxr-xr-x   0 yb         (501) staff       (20)        0 2023-04-20 15:16:07.984984 tokmon-0.1/tokmon.egg-info/
--rw-r--r--   0 yb         (501) staff       (20)      151 2023-04-20 15:16:07.000000 tokmon-0.1/tokmon.egg-info/PKG-INFO
--rw-r--r--   0 yb         (501) staff       (20)      303 2023-04-20 15:16:07.000000 tokmon-0.1/tokmon.egg-info/SOURCES.txt
--rw-r--r--   0 yb         (501) staff       (20)        1 2023-04-20 15:16:07.000000 tokmon-0.1/tokmon.egg-info/dependency_links.txt
--rw-r--r--   0 yb         (501) staff       (20)       43 2023-04-20 15:16:07.000000 tokmon-0.1/tokmon.egg-info/entry_points.txt
--rw-r--r--   0 yb         (501) staff       (20)       19 2023-04-20 15:16:07.000000 tokmon-0.1/tokmon.egg-info/requires.txt
--rw-r--r--   0 yb         (501) staff       (20)        7 2023-04-20 15:16:07.000000 tokmon-0.1/tokmon.egg-info/top_level.txt
+drwxr-xr-x   0 yb         (501) staff       (20)        0 2023-04-20 15:22:41.680696 tokmon-0.1.1/
+-rw-r--r--   0 yb         (501) staff       (20)    11336 2023-04-20 14:46:39.000000 tokmon-0.1.1/LICENSE
+-rw-r--r--   0 yb         (501) staff       (20)     6936 2023-04-20 15:22:41.680565 tokmon-0.1.1/PKG-INFO
+-rw-r--r--   0 yb         (501) staff       (20)     6750 2023-04-20 15:21:13.000000 tokmon-0.1.1/README.md
+-rw-r--r--   0 yb         (501) staff       (20)       38 2023-04-20 15:22:41.680743 tokmon-0.1.1/setup.cfg
+-rw-r--r--   0 yb         (501) staff       (20)      624 2023-04-20 15:22:33.000000 tokmon-0.1.1/setup.py
+drwxr-xr-x   0 yb         (501) staff       (20)        0 2023-04-20 15:22:41.679505 tokmon-0.1.1/tokmon/
+-rw-r--r--   0 yb         (501) staff       (20)        0 2023-04-13 01:47:04.000000 tokmon-0.1.1/tokmon/__init__.py
+-rwxr-xr-x   0 yb         (501) staff       (20)     4777 2023-04-20 14:46:37.000000 tokmon-0.1.1/tokmon/cli.py
+-rw-r--r--   0 yb         (501) staff       (20)     3370 2023-04-13 22:54:00.000000 tokmon-0.1.1/tokmon/costcalculator.py
+-rw-r--r--   0 yb         (501) staff       (20)     1021 2023-04-12 21:37:44.000000 tokmon-0.1.1/tokmon/pricing.json
+-rwxr-xr-x   0 yb         (501) staff       (20)     9244 2023-04-14 19:59:32.000000 tokmon-0.1.1/tokmon/tokmon.py
+drwxr-xr-x   0 yb         (501) staff       (20)        0 2023-04-20 15:22:41.680385 tokmon-0.1.1/tokmon.egg-info/
+-rw-r--r--   0 yb         (501) staff       (20)     6936 2023-04-20 15:22:41.000000 tokmon-0.1.1/tokmon.egg-info/PKG-INFO
+-rw-r--r--   0 yb         (501) staff       (20)      303 2023-04-20 15:22:41.000000 tokmon-0.1.1/tokmon.egg-info/SOURCES.txt
+-rw-r--r--   0 yb         (501) staff       (20)        1 2023-04-20 15:22:41.000000 tokmon-0.1.1/tokmon.egg-info/dependency_links.txt
+-rw-r--r--   0 yb         (501) staff       (20)       43 2023-04-20 15:22:41.000000 tokmon-0.1.1/tokmon.egg-info/entry_points.txt
+-rw-r--r--   0 yb         (501) staff       (20)       19 2023-04-20 15:22:41.000000 tokmon-0.1.1/tokmon.egg-info/requires.txt
+-rw-r--r--   0 yb         (501) staff       (20)        7 2023-04-20 15:22:41.000000 tokmon-0.1.1/tokmon.egg-info/top_level.txt
```

### Comparing `tokmon-0.1/LICENSE` & `tokmon-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tokmon-0.1/README.md` & `tokmon-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,34 @@
+Metadata-Version: 2.1
+Name: tokmon
+Version: 0.1.1
+Summary: UNKNOWN
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # `tokmon` 🔤🧐 - CLI utility to monitor OpenAI token costs
 
 `tokmon` enables you to monitor your program's OpenAI API token usage.
 
 You use `tokmon` just like you would use the `time` utility, but instead of execution time you get token usage and cost.
 <p align="center">
     <img src="https://user-images.githubusercontent.com/3611042/231910274-3872e13f-d9e6-4752-bc89-44e5d334e21f.gif" />
 </p>
 
 ## Quick install
-Install using `pip` like so:
 ```
-$ pip install git+https://github.com/yagil/tokmon.git
-$ tokmon --help
+pip install tokmon
+```
+
+Make sure installation worked by running
+```
+tokmon --help
 ```
 
 To uninstall, run `pip uninstall tokmon`<br>
 Tip: make sure that the your python Library route is in your `PATH`.
 
 ## How to use `tokmon`
 
@@ -143,7 +156,9 @@
 4. Submit a pull request with a clear description of your changes and any relevant information.
 
 ## Warning
 1. `tokmon` comes without any warranty or guarantee whatsoever.
 2. `tokmon` was tested on macOS only. It might not work on other platforms.
 3. This tool may not work as intended, have unknown side effects, may output incorrect information, or not work at all.
 4. The pricing data in `pricing.json` may go out of date.
+
+
```

### Comparing `tokmon-0.1/tokmon/cli.py` & `tokmon-0.1.1/tokmon/cli.py`

 * *Files identical despite different names*

### Comparing `tokmon-0.1/tokmon/costcalculator.py` & `tokmon-0.1.1/tokmon/costcalculator.py`

 * *Files identical despite different names*

### Comparing `tokmon-0.1/tokmon/pricing.json` & `tokmon-0.1.1/tokmon/pricing.json`

 * *Files identical despite different names*

### Comparing `tokmon-0.1/tokmon/tokmon.py` & `tokmon-0.1.1/tokmon/tokmon.py`

 * *Files identical despite different names*

