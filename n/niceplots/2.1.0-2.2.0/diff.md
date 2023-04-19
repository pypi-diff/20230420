# Comparing `tmp/niceplots-2.1.0-py3-none-any.whl.zip` & `tmp/niceplots-2.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16073 bytes, number of entries: 11
--rw-r--r--  2.0 unx       66 b- defN 23-Jan-31 16:17 niceplots/__init__.py
--rw-r--r--  2.0 unx     3452 b- defN 23-Jan-31 16:17 niceplots/parula.py
--rw-r--r--  2.0 unx    30725 b- defN 23-Jan-31 16:17 niceplots/utils.py
--rw-r--r--  2.0 unx     1146 b- defN 23-Jan-31 16:17 niceplots/styles/doumont-dark.mplstyle
--rw-r--r--  2.0 unx     1112 b- defN 23-Jan-31 16:17 niceplots/styles/doumont-light.mplstyle
--rw-r--r--  2.0 unx      857 b- defN 23-Jan-31 16:17 niceplots/styles/james-dark.mplstyle
--rw-r--r--  2.0 unx      852 b- defN 23-Jan-31 16:17 niceplots/styles/james-light.mplstyle
--rw-r--r--  2.0 unx     4456 b- defN 23-Jan-31 16:17 niceplots-2.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-31 16:17 niceplots-2.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jan-31 16:17 niceplots-2.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      910 b- defN 23-Jan-31 16:17 niceplots-2.1.0.dist-info/RECORD
-11 files, 43678 bytes uncompressed, 14527 bytes compressed:  66.7%
+Zip file size: 16773 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       66 b- defN 23-Apr-19 23:28 niceplots/__init__.py
+-rw-r--r--  2.0 unx     3452 b- defN 23-Apr-19 23:28 niceplots/parula.py
+-rw-r--r--  2.0 unx    33254 b- defN 23-Apr-19 23:28 niceplots/utils.py
+-rw-r--r--  2.0 unx     1146 b- defN 23-Apr-19 23:28 niceplots/styles/doumont-dark.mplstyle
+-rw-r--r--  2.0 unx     1112 b- defN 23-Apr-19 23:28 niceplots/styles/doumont-light.mplstyle
+-rw-r--r--  2.0 unx      909 b- defN 23-Apr-19 23:28 niceplots/styles/james-dark.mplstyle
+-rw-r--r--  2.0 unx      904 b- defN 23-Apr-19 23:28 niceplots/styles/james-light.mplstyle
+-rw-r--r--  2.0 unx     4485 b- defN 23-Apr-19 23:28 niceplots-2.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 23:28 niceplots-2.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-19 23:28 niceplots-2.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      910 b- defN 23-Apr-19 23:28 niceplots-2.2.0.dist-info/RECORD
+11 files, 46340 bytes uncompressed, 15227 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: niceplots/styles/james-dark.mplstyle
 Comment: 
 
 Filename: niceplots/styles/james-light.mplstyle
 Comment: 
 
-Filename: niceplots-2.1.0.dist-info/METADATA
+Filename: niceplots-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: niceplots-2.1.0.dist-info/WHEEL
+Filename: niceplots-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: niceplots-2.1.0.dist-info/top_level.txt
+Filename: niceplots-2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: niceplots-2.1.0.dist-info/RECORD
+Filename: niceplots-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## niceplots/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = "2.1.0"
+__version__ = "2.2.0"
 
 from .utils import *
 from .parula import *
```

## niceplots/utils.py

```diff
@@ -1,9 +1,10 @@
 import matplotlib.pyplot as plt
 import numpy as np
+from scipy.interpolate import make_interp_spline, Akima1DInterpolator
 from collections import OrderedDict
 from .parula import parula_map
 from matplotlib import patheffects
 from matplotlib.collections import LineCollection
 import matplotlib.colors as mcolor
 import warnings
 import os
@@ -176,15 +177,14 @@
     xs, ys = np.meshgrid(lins, lins)
     xs = xs.reshape(-1)
     ys = ys.reshape(-1)
     coords = np.zeros(2)
 
     # Loop over each line in the plot and create a label
     for idx, line in enumerate(axis.lines):
-
         # Set the starting coordinates of the label
         coords[0] = xs[idx]
         coords[1] = ys[idx]
         label = line.get_label()
 
         # Get the color of each line to set the label color as the same
         if color_on:
@@ -215,15 +215,15 @@
     colors : single or list of colors, optional
         Color(s) to use for each line, can be a single color for all lines or a list containing an entry for each line,
         by default uses each line's color
     x_offset_pts : int, float, optional
         Horizontal offset of label from the right end of the line, in points, by default 6
     y_offset_pts : int, float, optional
         Vertical offset of label from the right end of the line, in points, by default 0
-    **kwargs :
+    kwargs
         Any valid keywords for matplotlib's annotate function, except ``xy``, ``xytext``, ``color``, ``textcoords``,
         ``va``
 
     Returns
     -------
     list of matplotlib annotation objects
         The annotations created
@@ -312,15 +312,14 @@
     for t in times:
         tm = len(str(int(t)))
         if tm > t_max_digits:
             t_max_digits = tm
 
     # Actual loop that draws each bar
     for j, (l, t, ax) in enumerate(zip(labels, times, axarr)):
-
         # Draw the gray line and singular yellow dot
         ax.axhline(y=1, c=line_color, lw=3, zorder=0, alpha=0.5)
         ax.scatter([t], [1], c=color, lw=0, s=100, zorder=1, clip_on=False)
 
         # Set chart properties
         ax.set_ylim(0.99, 1.01)
         ax.set_xlim(0, t_max * 1.05)
@@ -364,15 +363,14 @@
     cushion=0.1,
     colors=None,
     lines_only=False,
     line_scaler=1.0,
     xlim=None,
     dpi=200,
 ):
-
     # If it's a dictionary, make it into a list so we can generically loop over it
     if isinstance(data_dict_list, dict):
         data_dict_list = [data_dict_list]
 
     if colors is None:
         colors = get_colors_list()
 
@@ -524,15 +522,16 @@
 
     # --- Check if user has a recent enough version of matplotlib to use hashed boundaries ---
     if conStyle.lower() == "hashed":
         try:
             patheffects.withTickedStroke
         except AttributeError:
             warnings.warn(
-                "matplotlib >= 3.4 is required for hashed inequality constrain boundaries, switching to shaded inequality constraint style"
+                "matplotlib >= 3.4 is required for hashed inequality constrain boundaries, switching to shaded inequality constraint style",
+                stacklevel=2,
             )
             conStyle = "shaded"
 
     # --- Define some default values if the user didn't provide them ---
     if cmap is None:
         cmap = parula_map
 
@@ -861,12 +860,77 @@
 
     if returnFig:
         return pieObjects, fig, ax
     else:
         return pieObjects
 
 
+def plot_spline(x, y, ax=None, spline_type="non-overshoot", num_interp_pts=100, spline_options={}, **plot_kwargs):
+    """
+    Fits a spline to the data points and plots the spline.
+
+    Parameters
+    ----------
+    x : array-like
+        X-coordinates of points to interpolate and plot
+    y : array-like
+        X-coordinates of points to interpolate and plot
+    ax : matplotlib Axis object, optional
+        Axes on which to plot, by default creates and returns new figure and axis
+    spline_type : str, optional
+        Type of spline from the following list of options (by default non-overshoot):
+
+            - "non-overshoot": Cubic spline that does not overshoot data (SciPy's Akima1DInterpolator)
+            - "b-spline": B-spline (SciPy's make_interp_spline)
+
+    num_interp_pts : int, optional
+        Number of points at which to evaluate the spline (linearly spaced between
+        min and max x values), by default 100
+    spline_options : dict, optional
+        Options to pass to the spline, by default none if spline_type is non-overshoot or sets the
+        spline order to the minimum of 3 and one less than the length of x if b-spline. The available
+        options can be found here:
+
+            - "non-overshoot": https://docs.scipy.org/doc/scipy/reference/generated/scipy.interpolate.Akima1DInterpolator.html
+            - "b-spline": https://docs.scipy.org/doc/scipy/reference/generated/scipy.interpolate.make_interp_spline.html
+
+    plot_kwargs
+        Keyword arguments to pass to matplotlib's plot function
+
+    Returns
+    -------
+    fig, ax
+        If ax is not provided, generates and returns new matplotlib figure and axis
+    """
+    return_fig = False
+    if ax is None:
+        fig, ax = plt.subplots()
+        return_fig = True
+
+    # Make the spline
+    if spline_type == "b-spline":
+        spline_option_defaults = {"k": min(len(x) - 1, 3)}
+    else:
+        spline_option_defaults = {}
+
+    options = spline_option_defaults | spline_options
+
+    if spline_type == "non-overshoot":
+        spline = Akima1DInterpolator(x, y, **options)
+    elif spline_type == "b-spline":
+        spline = make_interp_spline(x, y, **options)
+    else:
+        raise ValueError(f"Unknown spline_type {spline_type}")
+
+    # Interpolate and plot
+    x_interp = np.linspace(np.min(x), np.max(x), num_interp_pts)
+    ax.plot(x_interp, spline(x_interp), **plot_kwargs)
+
+    if return_fig:
+        return fig, ax
+
+
 def All():
     """Runs commonly called functions provided in this module."""
     adjust_spines()
     draggable_legend()
     plt.gcf().canvas.mpl_connect("close_event", handle_close)
```

## niceplots/styles/james-dark.mplstyle

```diff
@@ -17,19 +17,21 @@
 
 axes.prop_cycle : cycler('color', ['52a1fa', 'f26f6f', 'd6d6d6', 'c678fa', '78b865', 'e6ad53'])
 
 # Use this parameter, which (hopefully) nobody will ever use,
 # to store text the names of the colors in the color cycle
 keymap.help : Blue, Red, White, Purple, Green, Orange
 
-axes.edgecolor : bfd0e3
+axes.edgecolor : 6f8bab
 text.color : f5f5f5
 axes.labelcolor : f5f5f5
 axes.labelweight : 500
-xtick.color : bfd0e3
-ytick.color : bfd0e3
+xtick.color : 6f8bab
+ytick.color : 6f8bab
 xtick.labelsize : small
 ytick.labelsize : small
+xtick.labelcolor : bfd0e3
+ytick.labelcolor : bfd0e3
 axes.facecolor : 011d3b
 figure.facecolor : 011d3b
 
 pgf.rcfonts : True
```

## niceplots/styles/james-light.mplstyle

```diff
@@ -17,19 +17,21 @@
 
 axes.prop_cycle : cycler('color', ['52a1fa', 'f26f6f', '485263', 'ae66de', '3eb051', 'faaa48'])
 
 # Use this parameter, which (hopefully) nobody will ever use,
 # to store text the names of the colors in the color cycle
 keymap.help : Blue, Red, Navy, Purple, Green, Orange
 
-axes.edgecolor : 3b4c66
+axes.edgecolor : bababa
 text.color : 273345
 axes.labelcolor : 273345
 axes.labelweight : 500
-xtick.color : 3b4c66
-ytick.color : 3b4c66
+xtick.color : bababa
+ytick.color : bababa
 xtick.labelsize : small
 ytick.labelsize : small
+xtick.labelcolor : 273345
+ytick.labelcolor : 273345
 axes.facecolor : none
 figure.facecolor : none
 
 pgf.rcfonts : True
```

## Comparing `niceplots-2.1.0.dist-info/METADATA` & `niceplots-2.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: niceplots
-Version: 2.1.0
+Version: 2.2.0
 Summary: Plotting utilities for matplotlib in python
 Home-page: https://github.com/mdolab/niceplots
 Author: 
 Author-email: 
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: numpy (>=1.16)
 Requires-Dist: matplotlib (>=2.2)
+Requires-Dist: scipy (>=1.7)
 
 # NicePlots
 ## A collection of small tweaks to improve Python / plotting
 
 ![Build Status](https://github.com/mdolab/niceplots/workflows/niceplots/badge.svg)
 [![Documentation Status](https://readthedocs.com/projects/mdolab-niceplots/badge/?version=latest)](https://mdolab-niceplots.readthedocs-hosted.com/en/latest)
 [![PyPI](https://img.shields.io/pypi/v/niceplots)](https://pypi.org/project/niceplots/)
```

