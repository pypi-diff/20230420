# Comparing `tmp/wafermap-0.2.2.tar.gz` & `tmp/wafermap-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-0.2.2.tar", max compression
+gzip compressed data, was "wafermap-0.2.3.tar", max compression
```

## Comparing `wafermap-0.2.2.tar` & `wafermap-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1093 2023-04-15 15:10:24.839496 wafermap-0.2.2/LICENSE
--rw-r--r--   0        0        0      897 2023-04-19 14:06:18.046113 wafermap-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     7982 2023-04-19 13:29:46.122469 wafermap-0.2.2/README.md
--rw-r--r--   0        0        0      171 2023-04-19 10:42:08.837188 wafermap-0.2.2/wafermap/__init__.py
--rw-r--r--   0        0        0     3033 2023-04-17 22:16:54.410477 wafermap-0.2.2/wafermap/utils.py
--rw-r--r--   0        0        0    26339 2023-04-19 13:53:53.176550 wafermap-0.2.2/wafermap/wafermap.py
--rw-r--r--   0        0        0     8633 1970-01-01 00:00:00.000000 wafermap-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-15 15:10:24.839496 wafermap-0.2.3/LICENSE
+-rw-r--r--   0        0        0      897 2023-04-20 07:24:42.616048 wafermap-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7982 2023-04-19 13:29:46.122469 wafermap-0.2.3/README.md
+-rw-r--r--   0        0        0      171 2023-04-19 10:42:08.837188 wafermap-0.2.3/wafermap/__init__.py
+-rw-r--r--   0        0        0     3033 2023-04-17 22:16:54.410477 wafermap-0.2.3/wafermap/utils.py
+-rw-r--r--   0        0        0    26571 2023-04-20 07:18:47.386306 wafermap-0.2.3/wafermap/wafermap.py
+-rw-r--r--   0        0        0     8633 1970-01-01 00:00:00.000000 wafermap-0.2.3/PKG-INFO
```

### Comparing `wafermap-0.2.2/LICENSE` & `wafermap-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wafermap-0.2.2/pyproject.toml` & `wafermap-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wafermap"
-version = "0.2.2"
+version = "0.2.3"
 description = "A python package to plot maps of semiconductor wafers."
 authors = ["Sotiris Thomas <sothomas88@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/cap1tan/wafermap"
 keywords = ["semiconductor", "wafer", "layout", "plot"]
```

### Comparing `wafermap-0.2.2/README.md` & `wafermap-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `wafermap-0.2.2/wafermap/utils.py` & `wafermap-0.2.3/wafermap/utils.py`

 * *Files identical despite different names*

### Comparing `wafermap-0.2.2/wafermap/wafermap.py` & `wafermap-0.2.3/wafermap/wafermap.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import math
 import os
 from io import BytesIO
 from typing import List, Tuple, Union
 
 import branca
 import folium
-from folium import IFrame, plugins
+from folium import Element, IFrame, plugins
 from PIL import Image
 
 from wafermap import utils
 
 try:
     import selenium
     from selenium import webdriver
@@ -26,15 +26,18 @@
     exclusion, cells and several types of markers (points, vectors, images)."""
 
     NOTCH_HEIGHT = 1
     NOTCH_WIDTH = 2.8284
     DEFAULT_MARKER_STYLE = {"color": "#ff0000", "fill": True}
     DEFAULT_VECTOR_STYLE = {"color": "#009900", "weight": 1}
     DEFAULT_POINT_STYLE = {"radius": 0.5, "fill": True}
-    DEFAULT_LABEL_HTML_STYLE = "font-size: 8pt; color: black; text-align: center;"
+    DEFAULT_LABEL_FONT_SIZE = 8
+    DEFAULT_LABEL_HTML_STYLE = (
+        f"font-size: {DEFAULT_LABEL_FONT_SIZE}pt; color: black; text-align: center;"
+    )
     IMAGE_SIZE_IN_POPUP = (400, 400)
     IMAGE_FOLDER = "\\_images\\"
     MAP_PADDING = (100, 100)  # in pixels (x, y)
 
     def __init__(
         self,
         wafer_radius: float,
@@ -101,28 +104,27 @@
             control_scale=False,
             zoom_control=False,
             zoom_start=1,
             min_zoom=0.1,
             max_zoom=1000,
             zoomSnap=0,
             zoomDelta=0.1,
+            png_enabled=True,
         )
 
         # Add the base layer
         # Create a white image of 4 pixels, and embed it in an url.
-        white_tile = branca.utilities.image_to_url(
-            [[bg_color, bg_color], [bg_color, bg_color]]
-        )
+        white_tile = branca.utilities.image_to_url([[bg_color] * 2, [bg_color] * 2])
         # create base TileLayer (white background)
-        base = folium.raster_layers.TileLayer(
+        self._tile_layer = folium.raster_layers.TileLayer(
             tiles=white_tile,
             name="base",
             attr="white tile",
         )
-        base.add_to(folium_map)
+        self._tile_layer.add_to(folium_map)
 
         # Init rest of layers
         self._grid_layer = folium.map.FeatureGroup(name="grid")
         self._cell_labels_layer = folium.map.FeatureGroup(
             name="cell labels", show=False
         )
         self._labels_layer = folium.map.FeatureGroup(name="labels", show=False)
@@ -246,28 +248,37 @@
                     # print labels
                     folium.map.Marker(
                         [
                             lower_left[0] + (0.5 * self.cell_size_y),
                             lower_left[1] + (0.5 * self.cell_size_x),
                         ],
                         icon=folium.features.DivIcon(
-                            icon_size=(40, 10),
-                            icon_anchor=(0, 0),
-                            html=f'<div style="font-size: 8pt; color: black; '
+                            icon_size=(50, 20),
+                            icon_anchor=(25, 10),
+                            html=f'<div style="font-size: 8pt; color: black;'
                             f'text-align: center">{str(cell_label)}</div>',
                         ),
                     ).add_to(self._cell_labels_layer)
 
         self._grid_layer.add_to(folium_map)
         self._cell_labels_layer.add_to(folium_map)
         self._labels_layer.add_to(folium_map)
         self._edge_exclusion_layer.add_to(folium_map)
         self._images_layer.add_to(folium_map)
         self._markers_layer.add_to(folium_map)
         self._vectors_layer.add_to(folium_map)
+        # add extra controls
+        plugins.MousePosition(
+            position="topright",
+            separator=" | ",
+            empty_string="NaN",
+            lng_first=True,
+            prefix="Wafer Coordinates:",
+        ).add_to(folium_map)
+        folium.LayerControl().add_to(folium_map)
 
         self.map = folium_map
 
         # default zoom
         self.map.fit_bounds(
             [
                 (-self.wafer_radius, -self.wafer_radius),
@@ -296,23 +307,14 @@
     def save_html(self, output_file="wafermap.html") -> str:
         """Save current Folium Map to HTML."""
         assert os.path.splitext(output_file)[1].lower() == ".html"
         # turn on/off relevant layers/controls
         self._cell_labels_layer.show = False
         self._labels_layer.show = False
         self.map.options["zoomControl"] = True
-        # add extra controls to the html map
-        plugins.MousePosition(
-            position="topright",
-            separator=" | ",
-            empty_string="NaN",
-            lng_first=True,
-            prefix="Wafer Coordinates:",
-        ).add_to(self.map)
-        folium.LayerControl().add_to(self.map)
         self.map.save(output_file)
         return output_file
 
     def save_png(self, output_file="wafermap.png") -> Union[str, None]:
         """Save current Folium Map to a PNG image. Selenium is required."""
         if webdriver is None or selenium is None:
             raise EnvironmentError(
@@ -638,17 +640,22 @@
                 raise ValueError(f"{str(cell)} does not exist in wafermap.")
         else:
             # offset is wafer coordinates. Origin is the center
             label_origin = (
                 offset[0],
                 offset[1],
             )
-        # we multiply by 5 so that we have some scaling the label size with the
-        # cell size but still, it is not 1-1 conversion to pixel size.
-        label_size_px = (self.cell_size_x * 4, self.cell_size_y * 3)
+        # we multiply so that we have some scaling the label size with the
+        # label size
+        # 1pt is 1.333px
+        label_size_px = (
+            min(len(label_text) * WaferMap.DEFAULT_LABEL_FONT_SIZE * 1.333, 100),
+            min(WaferMap.DEFAULT_LABEL_FONT_SIZE * 1.333, 100),
+        )
+        # put the label anchor at the center of the label
         label_anchor_px = (label_size_px[0] / 2, label_size_px[1] / 2)
         folium.map.Marker(
             location=label_origin,
             icon=folium.features.DivIcon(
                 icon_size=label_size_px,
                 icon_anchor=label_anchor_px,
                 html=f'<div style="{label_html_style}">{label_text}</div>',
```

### Comparing `wafermap-0.2.2/PKG-INFO` & `wafermap-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wafermap
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python package to plot maps of semiconductor wafers.
 Home-page: https://github.com/cap1tan/wafermap
 License: MIT
 Keywords: semiconductor,wafer,layout,plot
 Author: Sotiris Thomas
 Author-email: sothomas88@gmail.com
 Requires-Python: >=3.8,<4.0
```

