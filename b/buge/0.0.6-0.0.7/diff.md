# Comparing `tmp/buge-0.0.6.tar.gz` & `tmp/buge-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buge-0.0.6.tar", last modified: Wed Apr 19 23:36:55 2023, max compression
+gzip compressed data, was "buge-0.0.7.tar", last modified: Thu Apr 20 00:51:24 2023, max compression
```

## Comparing `buge-0.0.6.tar` & `buge-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-19 23:36:55.544543 buge-0.0.6/
--rw-r--r--   0 damonpickett   (501) staff       (20)     1073 2023-04-14 22:43:18.000000 buge-0.0.6/LICENSE
--rw-r--r--   0 damonpickett   (501) staff       (20)       25 2023-04-14 22:43:29.000000 buge-0.0.6/MANIFEST.in
--rw-r--r--   0 damonpickett   (501) staff       (20)     4912 2023-04-19 23:36:55.544591 buge-0.0.6/PKG-INFO
--rw-r--r--   0 damonpickett   (501) staff       (20)     4708 2023-04-19 20:52:30.000000 buge-0.0.6/README.md
-drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-19 23:36:55.543607 buge-0.0.6/buge/
--rw-r--r--   0 damonpickett   (501) staff       (20)     2734 2023-04-19 20:01:30.000000 buge-0.0.6/buge/main.py
-drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-19 23:36:55.544414 buge-0.0.6/buge.egg-info/
--rw-r--r--   0 damonpickett   (501) staff       (20)     4912 2023-04-19 23:36:55.000000 buge-0.0.6/buge.egg-info/PKG-INFO
--rw-r--r--   0 damonpickett   (501) staff       (20)      260 2023-04-19 23:36:55.000000 buge-0.0.6/buge.egg-info/SOURCES.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)        1 2023-04-19 23:36:55.000000 buge-0.0.6/buge.egg-info/dependency_links.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)       40 2023-04-19 23:36:55.000000 buge-0.0.6/buge.egg-info/entry_points.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)       26 2023-04-19 23:36:55.000000 buge-0.0.6/buge.egg-info/requires.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)        5 2023-04-19 23:36:55.000000 buge-0.0.6/buge.egg-info/top_level.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)     4273 2023-04-19 23:36:27.000000 buge-0.0.6/pypiREADME.md
--rw-r--r--   0 damonpickett   (501) staff       (20)      648 2023-04-19 23:36:27.000000 buge-0.0.6/pyproject.toml
--rw-r--r--   0 damonpickett   (501) staff       (20)      784 2023-04-19 23:36:55.544815 buge-0.0.6/setup.cfg
--rw-r--r--   0 damonpickett   (501) staff       (20)       37 2023-04-13 22:46:26.000000 buge-0.0.6/setup.py
+drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-20 00:51:24.363875 buge-0.0.7/
+-rw-r--r--   0 damonpickett   (501) staff       (20)     1073 2023-04-14 22:43:18.000000 buge-0.0.7/LICENSE
+-rw-r--r--   0 damonpickett   (501) staff       (20)       25 2023-04-14 22:43:29.000000 buge-0.0.7/MANIFEST.in
+-rw-r--r--   0 damonpickett   (501) staff       (20)     4912 2023-04-20 00:51:24.363923 buge-0.0.7/PKG-INFO
+-rw-r--r--   0 damonpickett   (501) staff       (20)     4708 2023-04-19 20:52:30.000000 buge-0.0.7/README.md
+drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-20 00:51:24.363014 buge-0.0.7/buge/
+-rw-r--r--   0 damonpickett   (501) staff       (20)     2728 2023-04-20 00:50:30.000000 buge-0.0.7/buge/main.py
+drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-20 00:51:24.363754 buge-0.0.7/buge.egg-info/
+-rw-r--r--   0 damonpickett   (501) staff       (20)     4912 2023-04-20 00:51:24.000000 buge-0.0.7/buge.egg-info/PKG-INFO
+-rw-r--r--   0 damonpickett   (501) staff       (20)      260 2023-04-20 00:51:24.000000 buge-0.0.7/buge.egg-info/SOURCES.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)        1 2023-04-20 00:51:24.000000 buge-0.0.7/buge.egg-info/dependency_links.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)       40 2023-04-20 00:51:24.000000 buge-0.0.7/buge.egg-info/entry_points.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)       26 2023-04-20 00:51:24.000000 buge-0.0.7/buge.egg-info/requires.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)        5 2023-04-20 00:51:24.000000 buge-0.0.7/buge.egg-info/top_level.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)     4273 2023-04-19 23:36:27.000000 buge-0.0.7/pypiREADME.md
+-rw-r--r--   0 damonpickett   (501) staff       (20)      648 2023-04-20 00:50:55.000000 buge-0.0.7/pyproject.toml
+-rw-r--r--   0 damonpickett   (501) staff       (20)      784 2023-04-20 00:51:24.364150 buge-0.0.7/setup.cfg
+-rw-r--r--   0 damonpickett   (501) staff       (20)       37 2023-04-13 22:46:26.000000 buge-0.0.7/setup.py
```

### Comparing `buge-0.0.6/LICENSE` & `buge-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `buge-0.0.6/PKG-INFO` & `buge-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buge
-Version: 0.0.6
+Version: 0.0.7
 Summary: buge is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 Home-page: https://github.com/damonpickett/buge
 Author: Damon Pickett
 Author-email: Damon Pickett <damon.pickett@gmail.com>
 Project-URL: Homepage, https://github.com/damonpickett/buge
 Project-URL: Bug Tracker, https://github.com/damonpickett/buge/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: buge Version: 0.0.6 Summary: buge is a command-line
+Metadata-Version: 2.1 Name: buge Version: 0.0.7 Summary: buge is a command-line
 application that uses the OpenAI API to diagnose bugs when programming. Home-
 page: https://github.com/damonpickett/buge Author: Damon Pickett Author-email:
 Damon Pickett
 pickett@gmail.com> Project-URL: Homepage, https://github.com/damonpickett/buge
 Project-URL: Bug Tracker, https://github.com/damonpickett/buge/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
```

### Comparing `buge-0.0.6/README.md` & `buge-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `buge-0.0.6/buge/main.py` & `buge-0.0.7/buge/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,21 +63,21 @@
         )
         third_response_text = third_response.choices[0].text.strip()
 
         print("")
         console.print('[bold]--------------------[/bold]')
         print("")
         console.print("[bold cyan]Meaning:[/bold cyan]")
-        console.print(f"[green]`{base_response_text}`[green]")
+        console.print(f"[green]{base_response_text}[green]")
         print("")
         console.print("[bold cyan]Possible Causes:[/bold cyan]")
-        console.print(f"[green]`{secondary_response_text}`[green]")
+        console.print(f"[green]{secondary_response_text}[green]")
         print("")
         console.print("[bold cyan]Possible Solutions:[/bold cyan]")
-        console.print(f"[green]`{third_response_text}`[green]")
+        console.print(f"[green]{third_response_text}[green]")
         print("")
         console.print('[bold]--------------------[/bold]')
         print("")
 
     get_error_explanation(error_message)
 
 if __name__ == '__main__':
```

### Comparing `buge-0.0.6/buge.egg-info/PKG-INFO` & `buge-0.0.7/buge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buge
-Version: 0.0.6
+Version: 0.0.7
 Summary: buge is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 Home-page: https://github.com/damonpickett/buge
 Author: Damon Pickett
 Author-email: Damon Pickett <damon.pickett@gmail.com>
 Project-URL: Homepage, https://github.com/damonpickett/buge
 Project-URL: Bug Tracker, https://github.com/damonpickett/buge/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: buge Version: 0.0.6 Summary: buge is a command-line
+Metadata-Version: 2.1 Name: buge Version: 0.0.7 Summary: buge is a command-line
 application that uses the OpenAI API to diagnose bugs when programming. Home-
 page: https://github.com/damonpickett/buge Author: Damon Pickett Author-email:
 Damon Pickett
 pickett@gmail.com> Project-URL: Homepage, https://github.com/damonpickett/buge
 Project-URL: Bug Tracker, https://github.com/damonpickett/buge/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
```

### Comparing `buge-0.0.6/pypiREADME.md` & `buge-0.0.7/pypiREADME.md`

 * *Files identical despite different names*

### Comparing `buge-0.0.6/pyproject.toml` & `buge-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "buge"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Damon Pickett", email="damon.pickett@gmail.com" },
 ]
 description = "buge is a command-line application that uses the OpenAI API to diagnose bugs when programming."
 readme = "pypiREADME.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `buge-0.0.6/setup.cfg` & `buge-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = buge
-version = 0.0.6
+version = 0.0.7
 author = Damon Pickett
 author_email = damon.pickett@gmail.com
 description = buge is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/damonpickett/buge
 classifiers =
```

