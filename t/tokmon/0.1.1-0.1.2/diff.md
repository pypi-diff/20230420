# Comparing `tmp/tokmon-0.1.1.tar.gz` & `tmp/tokmon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokmon-0.1.1.tar", last modified: Thu Apr 20 15:22:41 2023, max compression
+gzip compressed data, was "tokmon-0.1.2.tar", last modified: Thu Apr 20 15:48:32 2023, max compression
```

## Comparing `tokmon-0.1.1.tar` & `tokmon-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 yb         (501) staff       (20)        0 2023-04-20 15:22:41.680696 tokmon-0.1.1/
--rw-r--r--   0 yb         (501) staff       (20)    11336 2023-04-20 14:46:39.000000 tokmon-0.1.1/LICENSE
--rw-r--r--   0 yb         (501) staff       (20)     6936 2023-04-20 15:22:41.680565 tokmon-0.1.1/PKG-INFO
--rw-r--r--   0 yb         (501) staff       (20)     6750 2023-04-20 15:21:13.000000 tokmon-0.1.1/README.md
--rw-r--r--   0 yb         (501) staff       (20)       38 2023-04-20 15:22:41.680743 tokmon-0.1.1/setup.cfg
--rw-r--r--   0 yb         (501) staff       (20)      624 2023-04-20 15:22:33.000000 tokmon-0.1.1/setup.py
-drwxr-xr-x   0 yb         (501) staff       (20)        0 2023-04-20 15:22:41.679505 tokmon-0.1.1/tokmon/
--rw-r--r--   0 yb         (501) staff       (20)        0 2023-04-13 01:47:04.000000 tokmon-0.1.1/tokmon/__init__.py
--rwxr-xr-x   0 yb         (501) staff       (20)     4777 2023-04-20 14:46:37.000000 tokmon-0.1.1/tokmon/cli.py
--rw-r--r--   0 yb         (501) staff       (20)     3370 2023-04-13 22:54:00.000000 tokmon-0.1.1/tokmon/costcalculator.py
--rw-r--r--   0 yb         (501) staff       (20)     1021 2023-04-12 21:37:44.000000 tokmon-0.1.1/tokmon/pricing.json
--rwxr-xr-x   0 yb         (501) staff       (20)     9244 2023-04-14 19:59:32.000000 tokmon-0.1.1/tokmon/tokmon.py
-drwxr-xr-x   0 yb         (501) staff       (20)        0 2023-04-20 15:22:41.680385 tokmon-0.1.1/tokmon.egg-info/
--rw-r--r--   0 yb         (501) staff       (20)     6936 2023-04-20 15:22:41.000000 tokmon-0.1.1/tokmon.egg-info/PKG-INFO
--rw-r--r--   0 yb         (501) staff       (20)      303 2023-04-20 15:22:41.000000 tokmon-0.1.1/tokmon.egg-info/SOURCES.txt
--rw-r--r--   0 yb         (501) staff       (20)        1 2023-04-20 15:22:41.000000 tokmon-0.1.1/tokmon.egg-info/dependency_links.txt
--rw-r--r--   0 yb         (501) staff       (20)       43 2023-04-20 15:22:41.000000 tokmon-0.1.1/tokmon.egg-info/entry_points.txt
--rw-r--r--   0 yb         (501) staff       (20)       19 2023-04-20 15:22:41.000000 tokmon-0.1.1/tokmon.egg-info/requires.txt
--rw-r--r--   0 yb         (501) staff       (20)        7 2023-04-20 15:22:41.000000 tokmon-0.1.1/tokmon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:48:32.731674 tokmon-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-04-20 15:48:22.000000 tokmon-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-20 15:48:32.731674 tokmon-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-20 15:48:22.000000 tokmon-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:48:32.731674 tokmon-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-20 15:48:32.000000 tokmon-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:48:32.731674 tokmon-0.1.2/tokmon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:48:22.000000 tokmon-0.1.2/tokmon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4777 2023-04-20 15:48:22.000000 tokmon-0.1.2/tokmon/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-20 15:48:22.000000 tokmon-0.1.2/tokmon/costcalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-20 15:48:22.000000 tokmon-0.1.2/tokmon/pricing.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9244 2023-04-20 15:48:22.000000 tokmon-0.1.2/tokmon/tokmon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:48:32.731674 tokmon-0.1.2/tokmon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-20 15:48:32.000000 tokmon-0.1.2/tokmon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-20 15:48:32.000000 tokmon-0.1.2/tokmon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:48:32.000000 tokmon-0.1.2/tokmon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 15:48:32.000000 tokmon-0.1.2/tokmon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 15:48:32.000000 tokmon-0.1.2/tokmon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 15:48:32.000000 tokmon-0.1.2/tokmon.egg-info/top_level.txt
```

### Comparing `tokmon-0.1.1/LICENSE` & `tokmon-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tokmon-0.1.1/PKG-INFO` & `tokmon-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 Metadata-Version: 2.1
 Name: tokmon
-Version: 0.1.1
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 0.1.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `tokmon` 🔤🧐 - CLI utility to monitor OpenAI token costs
 
 `tokmon` enables you to monitor your program's OpenAI API token usage.
 
@@ -24,15 +20,14 @@
 
 Make sure installation worked by running
 ```
 tokmon --help
 ```
 
 To uninstall, run `pip uninstall tokmon`<br>
-Tip: make sure that the your python Library route is in your `PATH`.
 
 ## How to use `tokmon`
 
 > **Warning**
 > This is a debugging tool. It is not intended to be used in any consequential setting. Use your best judgement, you're on your own!
 
 Prepend `tokmon` to your normal program invocation like so:
@@ -156,9 +151,7 @@
 4. Submit a pull request with a clear description of your changes and any relevant information.
 
 ## Warning
 1. `tokmon` comes without any warranty or guarantee whatsoever.
 2. `tokmon` was tested on macOS only. It might not work on other platforms.
 3. This tool may not work as intended, have unknown side effects, may output incorrect information, or not work at all.
 4. The pricing data in `pricing.json` may go out of date.
-
-
```

### Comparing `tokmon-0.1.1/README.md` & `tokmon-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 Make sure installation worked by running
 ```
 tokmon --help
 ```
 
 To uninstall, run `pip uninstall tokmon`<br>
-Tip: make sure that the your python Library route is in your `PATH`.
 
 ## How to use `tokmon`
 
 > **Warning**
 > This is a debugging tool. It is not intended to be used in any consequential setting. Use your best judgement, you're on your own!
 
 Prepend `tokmon` to your normal program invocation like so:
```

### Comparing `tokmon-0.1.1/setup.py` & `tokmon-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of the README.md file
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='tokmon',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'mitmproxy',
         'tiktoken',
     ],
     package_data={
         "tokmon": ["pricing.json"],
```

### Comparing `tokmon-0.1.1/tokmon/cli.py` & `tokmon-0.1.2/tokmon/cli.py`

 * *Files identical despite different names*

### Comparing `tokmon-0.1.1/tokmon/costcalculator.py` & `tokmon-0.1.2/tokmon/costcalculator.py`

 * *Files identical despite different names*

### Comparing `tokmon-0.1.1/tokmon/pricing.json` & `tokmon-0.1.2/tokmon/pricing.json`

 * *Files identical despite different names*

### Comparing `tokmon-0.1.1/tokmon/tokmon.py` & `tokmon-0.1.2/tokmon/tokmon.py`

 * *Files identical despite different names*

### Comparing `tokmon-0.1.1/tokmon.egg-info/PKG-INFO` & `tokmon-0.1.2/tokmon.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 Metadata-Version: 2.1
 Name: tokmon
-Version: 0.1.1
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 0.1.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `tokmon` 🔤🧐 - CLI utility to monitor OpenAI token costs
 
 `tokmon` enables you to monitor your program's OpenAI API token usage.
 
@@ -24,15 +20,14 @@
 
 Make sure installation worked by running
 ```
 tokmon --help
 ```
 
 To uninstall, run `pip uninstall tokmon`<br>
-Tip: make sure that the your python Library route is in your `PATH`.
 
 ## How to use `tokmon`
 
 > **Warning**
 > This is a debugging tool. It is not intended to be used in any consequential setting. Use your best judgement, you're on your own!
 
 Prepend `tokmon` to your normal program invocation like so:
@@ -156,9 +151,7 @@
 4. Submit a pull request with a clear description of your changes and any relevant information.
 
 ## Warning
 1. `tokmon` comes without any warranty or guarantee whatsoever.
 2. `tokmon` was tested on macOS only. It might not work on other platforms.
 3. This tool may not work as intended, have unknown side effects, may output incorrect information, or not work at all.
 4. The pricing data in `pricing.json` may go out of date.
-
-
```

