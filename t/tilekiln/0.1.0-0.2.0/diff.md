# Comparing `tmp/tilekiln-0.1.0.tar.gz` & `tmp/tilekiln-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tilekiln-0.1.0.tar", last modified: Mon Oct 31 08:16:22 2022, max compression
+gzip compressed data, was "tilekiln-0.2.0.tar", last modified: Wed Apr 19 23:19:35 2023, max compression
```

## Comparing `tilekiln-0.1.0.tar` & `tilekiln-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,31 @@
-drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2022-10-31 08:16:22.845745 tilekiln-0.1.0/
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)    35147 2022-10-19 18:01:33.000000 tilekiln-0.1.0/LICENSE
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)     3408 2022-10-31 08:16:22.845745 tilekiln-0.1.0/PKG-INFO
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)     2584 2022-10-19 18:06:23.000000 tilekiln-0.1.0/README.md
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)       38 2022-10-31 08:16:22.845745 tilekiln-0.1.0/setup.cfg
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)     1546 2022-10-27 06:42:23.000000 tilekiln-0.1.0/setup.py
-drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2022-10-31 08:16:22.845745 tilekiln-0.1.0/tilekiln/
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)      440 2022-10-25 22:21:39.000000 tilekiln-0.1.0/tilekiln/__init__.py
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)     3639 2022-10-30 00:36:48.000000 tilekiln-0.1.0/tilekiln/config.py
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)     1952 2022-10-29 03:03:04.000000 tilekiln-0.1.0/tilekiln/definition.py
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)     1077 2022-10-29 03:20:10.000000 tilekiln-0.1.0/tilekiln/kiln.py
-drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2022-10-31 08:16:22.845745 tilekiln-0.1.0/tilekiln/scripts/
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)     2705 2022-10-29 03:21:09.000000 tilekiln-0.1.0/tilekiln/scripts/__init__.py
-drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2022-10-31 08:16:22.845745 tilekiln-0.1.0/tilekiln/server/
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)     1715 2022-10-29 03:42:47.000000 tilekiln-0.1.0/tilekiln/server/__init__.py
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)      493 2022-10-27 08:15:06.000000 tilekiln-0.1.0/tilekiln/tile.py
-drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2022-10-31 08:16:22.845745 tilekiln-0.1.0/tilekiln.egg-info/
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)     3408 2022-10-31 08:16:22.000000 tilekiln-0.1.0/tilekiln.egg-info/PKG-INFO
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)      374 2022-10-31 08:16:22.000000 tilekiln-0.1.0/tilekiln.egg-info/SOURCES.txt
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)        1 2022-10-31 08:16:22.000000 tilekiln-0.1.0/tilekiln.egg-info/dependency_links.txt
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)       50 2022-10-31 08:16:22.000000 tilekiln-0.1.0/tilekiln.egg-info/entry_points.txt
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)       54 2022-10-31 08:16:22.000000 tilekiln-0.1.0/tilekiln.egg-info/requires.txt
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)        9 2022-10-31 08:16:22.000000 tilekiln-0.1.0/tilekiln.egg-info/top_level.txt
+drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2023-04-19 23:19:35.225109 tilekiln-0.2.0/
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)    35147 2022-10-19 18:01:33.000000 tilekiln-0.2.0/LICENSE
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     3416 2023-04-19 23:19:35.225109 tilekiln-0.2.0/PKG-INFO
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     2589 2023-01-07 05:17:16.000000 tilekiln-0.2.0/README.md
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)       38 2023-04-19 23:19:35.225109 tilekiln-0.2.0/setup.cfg
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     1593 2023-04-19 23:15:47.000000 tilekiln-0.2.0/setup.py
+drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2023-04-19 23:19:35.221109 tilekiln-0.2.0/tests/
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     5431 2023-01-02 06:21:10.000000 tilekiln-0.2.0/tests/test_config.py
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     2746 2022-10-29 03:22:42.000000 tilekiln-0.2.0/tests/test_definition.py
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)       80 2023-01-03 00:21:38.000000 tilekiln-0.2.0/tests/test_storage.py
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)      469 2022-10-27 08:17:18.000000 tilekiln-0.2.0/tests/test_tile.py
+drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2023-04-19 23:19:35.221109 tilekiln-0.2.0/tilekiln/
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)      440 2022-10-25 22:21:39.000000 tilekiln-0.2.0/tilekiln/__init__.py
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     3658 2023-04-08 05:41:47.000000 tilekiln-0.2.0/tilekiln/config.py
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     1952 2023-04-08 05:41:31.000000 tilekiln-0.2.0/tilekiln/definition.py
+drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2023-04-19 23:19:35.221109 tilekiln-0.2.0/tilekiln/dev/
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     1715 2022-10-29 03:42:47.000000 tilekiln-0.2.0/tilekiln/dev/__init__.py
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     1077 2022-10-29 03:20:10.000000 tilekiln-0.2.0/tilekiln/kiln.py
+drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2023-04-19 23:19:35.225109 tilekiln-0.2.0/tilekiln/scripts/
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)    11237 2023-04-08 05:51:43.000000 tilekiln-0.2.0/tilekiln/scripts/__init__.py
+drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2023-04-19 23:19:35.225109 tilekiln-0.2.0/tilekiln/server/
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     4298 2023-04-10 04:56:21.000000 tilekiln-0.2.0/tilekiln/server/__init__.py
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     4153 2023-04-08 06:10:20.000000 tilekiln-0.2.0/tilekiln/storage.py
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)      734 2023-01-06 04:55:26.000000 tilekiln-0.2.0/tilekiln/tile.py
+drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2023-04-19 23:19:35.221109 tilekiln-0.2.0/tilekiln.egg-info/
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     3416 2023-04-19 23:19:35.000000 tilekiln-0.2.0/tilekiln.egg-info/PKG-INFO
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)      506 2023-04-19 23:19:35.000000 tilekiln-0.2.0/tilekiln.egg-info/SOURCES.txt
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)        1 2023-04-19 23:19:35.000000 tilekiln-0.2.0/tilekiln.egg-info/dependency_links.txt
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)       50 2023-04-19 23:19:35.000000 tilekiln-0.2.0/tilekiln.egg-info/entry_points.txt
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)       76 2023-04-19 23:19:35.000000 tilekiln-0.2.0/tilekiln.egg-info/requires.txt
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)        9 2023-04-19 23:19:35.000000 tilekiln-0.2.0/tilekiln.egg-info/top_level.txt
```

### Comparing `tilekiln-0.1.0/LICENSE` & `tilekiln-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tilekiln-0.1.0/PKG-INFO` & `tilekiln-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tilekiln
-Version: 0.1.0
+Version: 0.2.0
 Summary: A set of command-line utilities to generate and serve Mapbox Vector Tiles (MVTs)
 Home-page: https://github.com/pnorman/tilekiln
 Author: Paul Norman
 Author-email: osm@paulnorman.ca
 Project-URL: Bug Reports, https://github.com/pnorman/tilekiln/issues
-Project-URL: Source, https://github.com/pypa/tilekiln/
+Project-URL: Source, https://github.com/pnorman/tilekiln/
 Keywords: openstreetmap,mvt,osm
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: GIS
@@ -44,15 +44,15 @@
 
 The tilekiln configuration syntax is based on studies and experience with other vector tile and map generation configurations. In particular, it is heavily inspired by Tilezen's use of Jinja2 templates and TileJSON for necessary metadata.
 
 ## License
 
 ### Code
 
-Copyright © 2022 Paul Norman <osm@paulnorman.ca>
+Copyright © 2022-2023 Paul Norman <osm@paulnorman.ca>
 
 The code is licensed terms of the GNU General Public License as
 published by the Free Software Foundation, either version 3 of
 the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `tilekiln-0.1.0/README.md` & `tilekiln-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 The tilekiln configuration syntax is based on studies and experience with other vector tile and map generation configurations. In particular, it is heavily inspired by Tilezen's use of Jinja2 templates and TileJSON for necessary metadata.
 
 ## License
 
 ### Code
 
-Copyright © 2022 Paul Norman <osm@paulnorman.ca>
+Copyright © 2022-2023 Paul Norman <osm@paulnorman.ca>
 
 The code is licensed terms of the GNU General Public License as
 published by the Free Software Foundation, either version 3 of
 the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `tilekiln-0.1.0/setup.py` & `tilekiln-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 setup (
     name="tilekiln",
-    version="0.1.0",
+    version="0.2.0",
     description="A set of command-line utilities to generate and serve Mapbox Vector Tiles (MVTs)",
 
     # Use README.md as the long description
     long_description=(here / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/pnorman/tilekiln",
     author="Paul Norman",
@@ -30,21 +30,23 @@
     python_requires=">=3.9, <4",
     install_requires=[
         "Click",
         "pyyaml",
         "fs",
         "Jinja2",
         "fastapi",
-        "psycopg"
+        "psycopg",
+        "psycopg[pool]",
+        "uvicorn"
     ],
     extras_require={
         "test": ["pytest"]
     },
     setup_requires=["flake8"],
     entry_points={
         "console_scripts": ["tilekiln = tilekiln.scripts:cli"]
     },
     project_urls={
         "Bug Reports": "https://github.com/pnorman/tilekiln/issues",
-        "Source": "https://github.com/pypa/tilekiln/",
+        "Source": "https://github.com/pnorman/tilekiln/",
     }
 )
```

### Comparing `tilekiln-0.1.0/tilekiln/config.py` & `tilekiln-0.2.0/tilekiln/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 class Config:
     def __init__(self, yaml_string, filesystem):
         '''Create a config from a yaml string
            Creates a config from the yaml string. Any SQL files referenced must be in the
            filesystem.
         '''
         config = yaml.safe_load(yaml_string)
-        self.name = config.get("metadata").get("name")
-        self.description = config.get("metadata").get("description")
-        self.attribution = config.get("metadata").get("attribution")
-        self.version = config.get("metadata").get("version")
-        self.bounds = config.get("metadata").get("bounds")
-        self.center = config.get("metadata").get("center")
+        self.id = config["metadata"]["id"]
+        self.name = config["metadata"].get("name")
+        self.description = config["metadata"].get("description")
+        self.attribution = config["metadata"].get("attribution")
+        self.version = config["metadata"].get("version")
+        self.bounds = config["metadata"].get("bounds")
+        self.center = config["metadata"].get("center")
 
         # TODO: Make private and expose needed operations through proper functions
         self.layers = []
         for id, l in config.get("vector_layers", {}).items():
             self.layers.append(LayerConfig(id, l, filesystem))
 
         self.minzoom = None
```

### Comparing `tilekiln-0.1.0/tilekiln/definition.py` & `tilekiln-0.2.0/tilekiln/definition.py`

 * *Files identical despite different names*

### Comparing `tilekiln-0.1.0/tilekiln/kiln.py` & `tilekiln-0.2.0/tilekiln/kiln.py`

 * *Files identical despite different names*

### Comparing `tilekiln-0.1.0/tilekiln/server/__init__.py` & `tilekiln-0.2.0/tilekiln/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `tilekiln-0.1.0/tilekiln.egg-info/PKG-INFO` & `tilekiln-0.2.0/tilekiln.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tilekiln
-Version: 0.1.0
+Version: 0.2.0
 Summary: A set of command-line utilities to generate and serve Mapbox Vector Tiles (MVTs)
 Home-page: https://github.com/pnorman/tilekiln
 Author: Paul Norman
 Author-email: osm@paulnorman.ca
 Project-URL: Bug Reports, https://github.com/pnorman/tilekiln/issues
-Project-URL: Source, https://github.com/pypa/tilekiln/
+Project-URL: Source, https://github.com/pnorman/tilekiln/
 Keywords: openstreetmap,mvt,osm
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: GIS
@@ -44,15 +44,15 @@
 
 The tilekiln configuration syntax is based on studies and experience with other vector tile and map generation configurations. In particular, it is heavily inspired by Tilezen's use of Jinja2 templates and TileJSON for necessary metadata.
 
 ## License
 
 ### Code
 
-Copyright © 2022 Paul Norman <osm@paulnorman.ca>
+Copyright © 2022-2023 Paul Norman <osm@paulnorman.ca>
 
 The code is licensed terms of the GNU General Public License as
 published by the Free Software Foundation, either version 3 of
 the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
```

