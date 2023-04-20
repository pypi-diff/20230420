# Comparing `tmp/rockalyzer-0.0.4.tar.gz` & `tmp/rockalyzer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockalyzer-0.0.4.tar", last modified: Thu Apr 20 16:22:36 2023, max compression
+gzip compressed data, was "rockalyzer-0.0.5.tar", last modified: Thu Apr 20 16:27:25 2023, max compression
```

## Comparing `rockalyzer-0.0.4.tar` & `rockalyzer-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 16:22:36.203300 rockalyzer-0.0.4/
--rw-rw-rw-   0        0        0     1089 2023-03-07 15:36:40.000000 rockalyzer-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2727 2023-04-20 16:22:36.202295 rockalyzer-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2146 2023-04-20 16:19:45.000000 rockalyzer-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 16:22:36.203300 rockalyzer-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-04-20 16:21:42.000000 rockalyzer-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:22:36.198294 rockalyzer-0.0.4/src/
--rw-rw-rw-   0        0        0    32560 2023-03-30 15:25:48.000000 rockalyzer-0.0.4/src/Action.py
--rw-rw-rw-   0        0        0    66093 2023-04-20 15:27:08.000000 rockalyzer-0.0.4/src/Game.py
--rw-rw-rw-   0        0        0      205 2023-03-27 18:56:29.000000 rockalyzer-0.0.4/src/console_colors.py
--rw-rw-rw-   0        0        0     4048 2023-04-20 08:11:58.000000 rockalyzer-0.0.4/src/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:22:36.202295 rockalyzer-0.0.4/src/rockalyzer.egg-info/
--rw-rw-rw-   0        0        0     2727 2023-04-20 16:22:36.000000 rockalyzer-0.0.4/src/rockalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-20 16:22:36.000000 rockalyzer-0.0.4/src/rockalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 16:22:36.000000 rockalyzer-0.0.4/src/rockalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-20 16:22:36.000000 rockalyzer-0.0.4/src/rockalyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       48 2023-04-20 16:22:36.000000 rockalyzer-0.0.4/src/rockalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4948 2023-04-20 08:08:30.000000 rockalyzer-0.0.4/src/rockalyzer.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:27:25.913489 rockalyzer-0.0.5/
+-rw-rw-rw-   0        0        0     1089 2023-03-07 15:36:40.000000 rockalyzer-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2894 2023-04-20 16:27:25.912489 rockalyzer-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2209 2023-04-20 16:25:18.000000 rockalyzer-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 16:27:25.913489 rockalyzer-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1110 2023-04-20 16:25:37.000000 rockalyzer-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:27:25.908394 rockalyzer-0.0.5/src/
+-rw-rw-rw-   0        0        0    32560 2023-03-30 15:25:48.000000 rockalyzer-0.0.5/src/Action.py
+-rw-rw-rw-   0        0        0    66093 2023-04-20 15:27:08.000000 rockalyzer-0.0.5/src/Game.py
+-rw-rw-rw-   0        0        0      205 2023-03-27 18:56:29.000000 rockalyzer-0.0.5/src/console_colors.py
+-rw-rw-rw-   0        0        0     4048 2023-04-20 08:11:58.000000 rockalyzer-0.0.5/src/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:27:25.911488 rockalyzer-0.0.5/src/rockalyzer.egg-info/
+-rw-rw-rw-   0        0        0     2894 2023-04-20 16:27:25.000000 rockalyzer-0.0.5/src/rockalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-04-20 16:27:25.000000 rockalyzer-0.0.5/src/rockalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 16:27:25.000000 rockalyzer-0.0.5/src/rockalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-20 16:27:25.000000 rockalyzer-0.0.5/src/rockalyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       48 2023-04-20 16:27:25.000000 rockalyzer-0.0.5/src/rockalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4948 2023-04-20 08:08:30.000000 rockalyzer-0.0.5/src/rockalyzer.py
```

### Comparing `rockalyzer-0.0.4/LICENSE` & `rockalyzer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rockalyzer-0.0.4/PKG-INFO` & `rockalyzer-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: rockalyzer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Rocket League Boxcars-Replay Analyzer
 Home-page: https://github.com/eliastheis/rockalyzer
 Author: Elias Theis
 Author-email: mail@eliastheis.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Rocket League Boxcars-Replay Analyzer
 
@@ -59,14 +61,14 @@
 
 # get stats
 stats = replayer.get_stats()
 ```
 
 ### Simple render
 If you set `render=True` when creating the `Replayer`-object, you get a simple (almost real-time) render of the game using [matplotlib](https://matplotlib.org/)
-![Screenshot of render](render_screenshot.png)
+![Screenshot of render](https://raw.githubusercontent.com/eliastheis/rockalyzer/master/render_screenshot.png)
 
 ## Build and upload package to PyPi
 ```python
 python ./setup bdist_wheel sdist
 python -m twine upload dist/*
 ```
```

### Comparing `rockalyzer-0.0.4/README.md` & `rockalyzer-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,14 @@
 
 # get stats
 stats = replayer.get_stats()
 ```
 
 ### Simple render
 If you set `render=True` when creating the `Replayer`-object, you get a simple (almost real-time) render of the game using [matplotlib](https://matplotlib.org/)
-![Screenshot of render](render_screenshot.png)
+![Screenshot of render](https://raw.githubusercontent.com/eliastheis/rockalyzer/master/render_screenshot.png)
 
 ## Build and upload package to PyPi
 ```python
 python ./setup bdist_wheel sdist
 python -m twine upload dist/*
 ```
```

### Comparing `rockalyzer-0.0.4/setup.py` & `rockalyzer-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # read the contents of your README file for the long description
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='rockalyzer',
-    version='0.0.4',
+    version='0.0.5',
     description='Rocket League Boxcars-Replay Analyzer',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/eliastheis/rockalyzer',
     author='Elias Theis',
     author_email='mail@eliastheis.de',
     py_modules=['rockalyzer', 'Game', 'Action', 'console_colors', 'constants'],
@@ -21,12 +21,14 @@
         'matplotlib',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 
 )
```

### Comparing `rockalyzer-0.0.4/src/Action.py` & `rockalyzer-0.0.5/src/Action.py`

 * *Files identical despite different names*

### Comparing `rockalyzer-0.0.4/src/Game.py` & `rockalyzer-0.0.5/src/Game.py`

 * *Files identical despite different names*

### Comparing `rockalyzer-0.0.4/src/constants.py` & `rockalyzer-0.0.5/src/constants.py`

 * *Files identical despite different names*

### Comparing `rockalyzer-0.0.4/src/rockalyzer.egg-info/PKG-INFO` & `rockalyzer-0.0.5/src/rockalyzer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: rockalyzer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Rocket League Boxcars-Replay Analyzer
 Home-page: https://github.com/eliastheis/rockalyzer
 Author: Elias Theis
 Author-email: mail@eliastheis.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Rocket League Boxcars-Replay Analyzer
 
@@ -59,14 +61,14 @@
 
 # get stats
 stats = replayer.get_stats()
 ```
 
 ### Simple render
 If you set `render=True` when creating the `Replayer`-object, you get a simple (almost real-time) render of the game using [matplotlib](https://matplotlib.org/)
-![Screenshot of render](render_screenshot.png)
+![Screenshot of render](https://raw.githubusercontent.com/eliastheis/rockalyzer/master/render_screenshot.png)
 
 ## Build and upload package to PyPi
 ```python
 python ./setup bdist_wheel sdist
 python -m twine upload dist/*
 ```
```

### Comparing `rockalyzer-0.0.4/src/rockalyzer.py` & `rockalyzer-0.0.5/src/rockalyzer.py`

 * *Files identical despite different names*

