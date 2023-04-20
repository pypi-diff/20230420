# Comparing `tmp/openchord-0.1.1.tar.gz` & `tmp/openchord-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openchord-0.1.1.tar", last modified: Thu Apr 20 16:29:50 2023, max compression
+gzip compressed data, was "openchord-0.1.2.tar", last modified: Thu Apr 20 16:58:00 2023, max compression
```

## Comparing `openchord-0.1.1.tar` & `openchord-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 16:29:50.523512 openchord-0.1.1/
--rw-rw-r--   0 kenny     (1000) kenny     (1000)    35149 2023-04-20 13:29:24.000000 openchord-0.1.1/LICENSE
--rw-rw-r--   0 kenny     (1000) kenny     (1000)     2253 2023-04-20 16:29:50.523512 openchord-0.1.1/PKG-INFO
--rw-rw-r--   0 kenny     (1000) kenny     (1000)     1736 2023-04-20 16:03:05.000000 openchord-0.1.1/README.md
--rw-rw-r--   0 kenny     (1000) kenny     (1000)      675 2023-04-20 16:29:42.000000 openchord-0.1.1/pyproject.toml
--rw-rw-r--   0 kenny     (1000) kenny     (1000)       38 2023-04-20 16:29:50.523512 openchord-0.1.1/setup.cfg
-drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 16:29:50.519512 openchord-0.1.1/src/
--rw-rw-r--   0 kenny     (1000) kenny     (1000)        0 2023-04-20 13:36:13.000000 openchord-0.1.1/src/__init__.py
-drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 16:29:50.523512 openchord-0.1.1/src/openchord.egg-info/
--rw-rw-r--   0 kenny     (1000) kenny     (1000)     2253 2023-04-20 16:29:50.000000 openchord-0.1.1/src/openchord.egg-info/PKG-INFO
--rw-rw-r--   0 kenny     (1000) kenny     (1000)      249 2023-04-20 16:29:50.000000 openchord-0.1.1/src/openchord.egg-info/SOURCES.txt
--rw-rw-r--   0 kenny     (1000) kenny     (1000)        1 2023-04-20 16:29:50.000000 openchord-0.1.1/src/openchord.egg-info/dependency_links.txt
--rw-rw-r--   0 kenny     (1000) kenny     (1000)       20 2023-04-20 16:29:50.000000 openchord-0.1.1/src/openchord.egg-info/requires.txt
--rw-rw-r--   0 kenny     (1000) kenny     (1000)       19 2023-04-20 16:29:50.000000 openchord-0.1.1/src/openchord.egg-info/top_level.txt
--rw-rw-r--   0 kenny     (1000) kenny     (1000)     6261 2023-04-20 13:29:24.000000 openchord-0.1.1/src/openchord.py
+drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 16:58:00.193435 openchord-0.1.2/
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)    35149 2023-04-20 13:29:24.000000 openchord-0.1.2/LICENSE
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)     2042 2023-04-20 16:58:00.193435 openchord-0.1.2/PKG-INFO
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)     1525 2023-04-20 16:54:19.000000 openchord-0.1.2/README.md
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)      685 2023-04-20 16:57:45.000000 openchord-0.1.2/pyproject.toml
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)       38 2023-04-20 16:58:00.193435 openchord-0.1.2/setup.cfg
+drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 16:58:00.193435 openchord-0.1.2/src/
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)        0 2023-04-20 13:36:13.000000 openchord-0.1.2/src/__init__.py
+drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 16:58:00.193435 openchord-0.1.2/src/openchord.egg-info/
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)     2042 2023-04-20 16:58:00.000000 openchord-0.1.2/src/openchord.egg-info/PKG-INFO
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)      249 2023-04-20 16:58:00.000000 openchord-0.1.2/src/openchord.egg-info/SOURCES.txt
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)        1 2023-04-20 16:58:00.000000 openchord-0.1.2/src/openchord.egg-info/dependency_links.txt
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)       30 2023-04-20 16:58:00.000000 openchord-0.1.2/src/openchord.egg-info/requires.txt
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)       19 2023-04-20 16:58:00.000000 openchord-0.1.2/src/openchord.egg-info/top_level.txt
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)     6261 2023-04-20 13:29:24.000000 openchord-0.1.2/src/openchord.py
```

### Comparing `openchord-0.1.1/LICENSE` & `openchord-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openchord-0.1.1/PKG-INFO` & `openchord-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openchord
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for ploting chord diagrams
 Author-email: Kenny Pang <pangkhangee@gmail.com>
 Project-URL: Homepage, https://github.com/pke1029/open-chord
 Keywords: plot,data science,Jupyter,network,graph
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -14,17 +14,17 @@
 
 # OpenChord
 
 OpenChord is a Python library I am developing to plot beautiful chord diagrams for visualising networks and graphs. OpenChord uses the `drawsvg` library and can display figures in a Jupyter notebook or Jupyter lab. Other libraries for drawing chord diagram includes [PlotAPI](https://plotapi.com/) (paid), [Bokeh](https://holoviews.org/reference/elements/bokeh/Chord.html) (visible moire artifact), and [Plotly](https://plotly.com/python/v3/filled-chord-diagram/) (tedious). 
 
 ## Installation
 
-I am working on hosting the library on PyPI.org. At the meantime, you can download the `openchord.py` file into your working directory/folder and use it that way. You will also need to install the `drawsvg` library (https://github.com/cduck/drawsvg) using the command
+OpenChord is now on PyPI.org! Install using the command
 ```
-python3 -m pip install "drawsvg[all]"
+python3 -m pip install openchord
 ```
 
 ## Usage
 
 Currently, the function only support symmetric adjacency matricies (i.e. weighted graph, non-directed)
 ```python
 import openchord as ocd
@@ -44,8 +44,8 @@
 fig.color_map = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
 fig.show()
 ```
 You can export the figure as an .svg file and open it in a vector graphics software such as [Inkscape](https://inkscape.org/)
 ```python
 fig.save_svg("figure.svg")
 ```
-![Chord diagram using OpenChord](https://github.com/pke1029/open-chord/blob/main/figure.png)
+![Chord diagram using OpenChord](https://github.com/pke1029/open-chord/blob/main/media/figure.png)
```

### Comparing `openchord-0.1.1/README.md` & `openchord-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # OpenChord
 
 OpenChord is a Python library I am developing to plot beautiful chord diagrams for visualising networks and graphs. OpenChord uses the `drawsvg` library and can display figures in a Jupyter notebook or Jupyter lab. Other libraries for drawing chord diagram includes [PlotAPI](https://plotapi.com/) (paid), [Bokeh](https://holoviews.org/reference/elements/bokeh/Chord.html) (visible moire artifact), and [Plotly](https://plotly.com/python/v3/filled-chord-diagram/) (tedious). 
 
 ## Installation
 
-I am working on hosting the library on PyPI.org. At the meantime, you can download the `openchord.py` file into your working directory/folder and use it that way. You will also need to install the `drawsvg` library (https://github.com/cduck/drawsvg) using the command
+OpenChord is now on PyPI.org! Install using the command
 ```
-python3 -m pip install "drawsvg[all]"
+python3 -m pip install openchord
 ```
 
 ## Usage
 
 Currently, the function only support symmetric adjacency matricies (i.e. weighted graph, non-directed)
 ```python
 import openchord as ocd
@@ -30,8 +30,8 @@
 fig.color_map = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
 fig.show()
 ```
 You can export the figure as an .svg file and open it in a vector graphics software such as [Inkscape](https://inkscape.org/)
 ```python
 fig.save_svg("figure.svg")
 ```
-![Chord diagram using OpenChord](https://github.com/pke1029/open-chord/blob/main/figure.png)
+![Chord diagram using OpenChord](https://github.com/pke1029/open-chord/blob/main/media/figure.png)
```

### Comparing `openchord-0.1.1/pyproject.toml` & `openchord-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openchord"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name = "Kenny Pang", email = "pangkhangee@gmail.com"},
 ]
 description = "A library for ploting chord diagrams"
 readme = "README.md"
 requires-python = ">=3.6"
 keywords = ["plot", "data science", "Jupyter", "network", "graph"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "drawsvg",
+    "drawsvg[all]~=2.0",
     "numpy ~= 1.16"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/pke1029/open-chord"
```

### Comparing `openchord-0.1.1/src/openchord.egg-info/PKG-INFO` & `openchord-0.1.2/src/openchord.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openchord
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for ploting chord diagrams
 Author-email: Kenny Pang <pangkhangee@gmail.com>
 Project-URL: Homepage, https://github.com/pke1029/open-chord
 Keywords: plot,data science,Jupyter,network,graph
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -14,17 +14,17 @@
 
 # OpenChord
 
 OpenChord is a Python library I am developing to plot beautiful chord diagrams for visualising networks and graphs. OpenChord uses the `drawsvg` library and can display figures in a Jupyter notebook or Jupyter lab. Other libraries for drawing chord diagram includes [PlotAPI](https://plotapi.com/) (paid), [Bokeh](https://holoviews.org/reference/elements/bokeh/Chord.html) (visible moire artifact), and [Plotly](https://plotly.com/python/v3/filled-chord-diagram/) (tedious). 
 
 ## Installation
 
-I am working on hosting the library on PyPI.org. At the meantime, you can download the `openchord.py` file into your working directory/folder and use it that way. You will also need to install the `drawsvg` library (https://github.com/cduck/drawsvg) using the command
+OpenChord is now on PyPI.org! Install using the command
 ```
-python3 -m pip install "drawsvg[all]"
+python3 -m pip install openchord
 ```
 
 ## Usage
 
 Currently, the function only support symmetric adjacency matricies (i.e. weighted graph, non-directed)
 ```python
 import openchord as ocd
@@ -44,8 +44,8 @@
 fig.color_map = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
 fig.show()
 ```
 You can export the figure as an .svg file and open it in a vector graphics software such as [Inkscape](https://inkscape.org/)
 ```python
 fig.save_svg("figure.svg")
 ```
-![Chord diagram using OpenChord](https://github.com/pke1029/open-chord/blob/main/figure.png)
+![Chord diagram using OpenChord](https://github.com/pke1029/open-chord/blob/main/media/figure.png)
```

### Comparing `openchord-0.1.1/src/openchord.py` & `openchord-0.1.2/src/openchord.py`

 * *Files identical despite different names*

