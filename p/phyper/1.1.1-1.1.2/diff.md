# Comparing `tmp/phyper-1.1.1-py3-none-any.whl.zip` & `tmp/phyper-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 28823 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat      702 b- defN 23-Apr-20 10:25 phyper/__init__.py
--rw-rw-rw-  2.0 fat      306 b- defN 23-Apr-20 10:25 phyper/chemometrics/__init__.py
--rw-rw-rw-  2.0 fat     9908 b- defN 23-Apr-20 10:25 phyper/chemometrics/_gui.py
--rw-rw-rw-  2.0 fat    13557 b- defN 23-Apr-20 10:25 phyper/chemometrics/analysis.py
--rw-rw-rw-  2.0 fat    49010 b- defN 23-Apr-20 10:25 phyper/chemometrics/dataset.py
--rw-rw-rw-  2.0 fat     2812 b- defN 23-Apr-20 10:25 phyper/chemometrics/preprocessing.py
--rw-rw-rw-  2.0 fat     2367 b- defN 23-Apr-20 10:25 phyper/chemometrics/sampling.py
--rw-rw-rw-  2.0 fat      125 b- defN 23-Apr-20 10:25 phyper/lab/__init__.py
--rw-rw-rw-  2.0 fat      837 b- defN 23-Apr-20 10:25 phyper/lab/_misc.py
--rw-rw-rw-  2.0 fat    15674 b- defN 23-Apr-20 10:25 phyper/lab/measurement.py
--rw-rw-rw-  2.0 fat     1096 b- defN 23-Apr-20 10:28 phyper-1.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2246 b- defN 23-Apr-20 10:28 phyper-1.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 10:28 phyper-1.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-20 10:28 phyper-1.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1219 b- defN 23-Apr-20 10:28 phyper-1.1.1.dist-info/RECORD
-15 files, 99958 bytes uncompressed, 26813 bytes compressed:  73.2%
+Zip file size: 28806 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      685 b- defN 23-Apr-20 10:38 phyper/__init__.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Apr-20 12:42 phyper/chemometrics/__init__.py
+-rw-r--r--  2.0 unx     9505 b- defN 23-Apr-20 13:00 phyper/chemometrics/_gui.py
+-rw-r--r--  2.0 unx    13252 b- defN 23-Apr-20 10:38 phyper/chemometrics/analysis.py
+-rw-r--r--  2.0 unx    48428 b- defN 23-Apr-20 12:55 phyper/chemometrics/dataset.py
+-rw-r--r--  2.0 unx     2713 b- defN 23-Apr-20 10:38 phyper/chemometrics/preprocessing.py
+-rw-r--r--  2.0 unx     2298 b- defN 23-Apr-20 10:38 phyper/chemometrics/sampling.py
+-rw-r--r--  2.0 unx      121 b- defN 23-Apr-20 10:38 phyper/lab/__init__.py
+-rw-r--r--  2.0 unx      802 b- defN 23-Apr-20 10:38 phyper/lab/_misc.py
+-rw-r--r--  2.0 unx    15275 b- defN 23-Apr-20 10:38 phyper/lab/measurement.py
+-rwxrwxrwx  2.0 unx     1075 b- defN 23-Apr-20 13:03 phyper-1.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2231 b- defN 23-Apr-20 13:03 phyper-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 13:03 phyper-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-20 13:03 phyper-1.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1219 b- defN 23-Apr-20 13:03 phyper-1.1.2.dist-info/RECORD
+15 files, 97995 bytes uncompressed, 26796 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: phyper/lab/_misc.py
 Comment: 
 
 Filename: phyper/lab/measurement.py
 Comment: 
 
-Filename: phyper-1.1.1.dist-info/LICENSE
+Filename: phyper-1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: phyper-1.1.1.dist-info/METADATA
+Filename: phyper-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: phyper-1.1.1.dist-info/WHEEL
+Filename: phyper-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: phyper-1.1.1.dist-info/top_level.txt
+Filename: phyper-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: phyper-1.1.1.dist-info/RECORD
+Filename: phyper-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## phyper/__init__.py

 * *Ordering differences only*

```diff
@@ -1,18 +1,18 @@
-""" This is a Python toolbox for hYPERspectral data. This toolbox includes methods for reading hyperspectral images and provides an interface for basic machine learning algorithms like decomposition and clustering.
-
-A demo file can be found in the 'main.py' file.
-
-This toolbox is devided into two packages
-
-- chemometrics
-    Package for creating datasets and preforming basic chemometrics analysises on them
-- lab
-    Package for managing data collected with the lab equiment and file structures from MeBioS.
-
-Written by Remi Van Belleghem. Based on Matlab toolbox from Niels Wouters.
-
-"""
-
-# wavelength unit to be used in the entire package
-WL_UNIT = 'nm'
+""" This is a Python toolbox for hYPERspectral data. This toolbox includes methods for reading hyperspectral images and provides an interface for basic machine learning algorithms like decomposition and clustering.
+
+A demo file can be found in the 'main.py' file.
+
+This toolbox is devided into two packages
+
+- chemometrics
+    Package for creating datasets and preforming basic chemometrics analysises on them
+- lab
+    Package for managing data collected with the lab equiment and file structures from MeBioS.
+
+Written by Remi Van Belleghem. Based on Matlab toolbox from Niels Wouters.
+
+"""
+
+# wavelength unit to be used in the entire package
+WL_UNIT = 'nm'
 WL_UNIT_LONG = 'nanometer'
```

## phyper/chemometrics/__init__.py

 * *Ordering differences only*

```diff
@@ -1,14 +1,14 @@
-""" Chemometrics package from Pyper toolbox
-
-Contains methods and classes for
-
-- (hyperspectral)dataset creation
-    datasets
-- classification, clustering and decompostion
-    cluster
-    classif
-    decomposition
-- utilities for preprocessing and sampling
-    preprocessing
-    sampling
-"""
+""" Chemometrics package from Pyper toolbox
+
+Contains methods and classes for
+
+- (hyperspectral)dataset creation
+    datasets
+- classification, clustering and decompostion
+    cluster
+    classif
+    decomposition
+- utilities for preprocessing and sampling
+    preprocessing
+    sampling
+"""
```

## phyper/chemometrics/_gui.py

```diff
@@ -1,260 +1,257 @@
-from matplotlib import pyplot
-from matplotlib.path import Path
-from matplotlib.widgets import PolygonSelector, LassoSelector
-import numpy as np
-
-from .. import WL_UNIT, WL_UNIT_LONG
-
-class Gui(object):
-    """ Helper class for managing a gui for exploring an HyperSpectralDataset object """
-
-    def __init__(self, HSD):
-        self.HSD = HSD
-
-        self.wl_idx = 0
-        included_image = self.HSD.get_included_image()
-        row_idx, col_idx = np.nonzero(included_image)
-        # list of type SpectrumPoint. Initialise with some point inside included data
-        self.spectra = [self.SpectrumPoint(col_idx[0], row_idx[0], 0)]
-
-        self.selected_point = None
-        self.selected_line = None
-
-        self.vline_artist = None
-
-        self.fig, [self.image_ax, self.spectral_ax] = pyplot.subplots(1, 2)
-
-        self.fig.canvas.mpl_connect('pick_event', self.on_pick)
-        self.fig.canvas.mpl_connect('button_press_event', self.on_press)
-        self.fig.canvas.mpl_connect('button_release_event', self.on_release)
-        self.fig.canvas.mpl_connect('key_press_event', self.on_key)
-        self.fig.canvas.mpl_connect('motion_notify_event', self.on_motion)
-
-    def on_press(self, event):
-        if self.selected_point is not None or self.selected_line is not None:
-            return
-        if not event.dblclick:
-            # TODO: make sure only add spectrum when press event is in image axis.
-            # Watch out with notebook!! -> event.isaxis == self.image_ax doesn't work.
-            return
-        # add new SpectrumPoint to list of spectra
-        self.spectra.append(self.SpectrumPoint(round(event.xdata), round(event.ydata), len(self.spectra) + 1))
-
-        self.update_axes()
-
-    def on_key(self, event):
-        if event.key == 'left':
-            self.wl_idx = max([0, self.wl_idx - 1])
-            self.update_axes()
-        elif event.key == 'right':
-            self.wl_idx = min([self.HSD.get_dimL(), self.wl_idx + 1])
-            self.update_axes()
-
-    def on_pick(self, event):
-        if event.mouseevent.button == 3:
-            # remove point if right-clicked
-            self.spectra.remove(event.artist.obj)
-            self.update_axes()
-        elif event.mouseevent.button == 1:
-            if hasattr(event.artist, 'obj'):
-                self.selected_point = event.artist
-            elif self.vline_artist == event.artist:
-                self.selected_line = event.artist
-
-    def on_motion(self, event):
-        if self.selected_line is None and self.selected_point is None:
-            return
-        elif self.selected_point is not None and event.xdata is not None:
-            self.selected_point.obj.x = round(event.xdata)
-            self.selected_point.obj.y = round(event.ydata)
-            self.update_axes()
-        elif self.selected_line is not None and event.xdata is not None:
-            request_wl = np.clip(round(event.xdata), min(self.HSD.get_wl()), max(self.HSD.get_wl()))
-            self.wl_idx = self.HSD.get_wl_idx(request_wl)
-            self.update_axes()
-
-    def on_release(self, event):
-        self.selected_line = None
-        self.selected_point = None
-
-    def update_axes(self):
-
-        # save x/y limits of axes to retain zoom ratio when updating window
-        old_xlim_image = self.image_ax.get_xlim()
-        old_ylim_image = self.image_ax.get_ylim()
-
-        old_xlim_spectral = self.spectral_ax.get_xlim()
-
-        # clear axes
-        self.image_ax.clear()
-        self.spectral_ax.clear()
-
-        # show band image in image axis
-        self.image_ax.imshow(self.HSD.get_band_image(self.wl_idx))
-
-        # indicate wavelength
-        self.vline_artist = self.spectral_ax.axvline(x=self.HSD.get_wl()[self.wl_idx], color='k', picker=True,
-                                                     pickradius=20)
-
-        # plot points and spectra for each spectrum in list with SpectrumPoints
-        for spectrum in self.spectra:
-            # draw point in image axis
-            spectrum.draw_point(self.image_ax)
-
-            # draw spectrum in spectral axis
-            spectrum.draw_spectrum(self.spectral_ax, self.HSD.get_wl(),
-                                   self.HSD.get_spectrum_at(spectrum.y, spectrum.x))
-
-        # format axes titles and labels
-        self.image_ax.set_title('Wavelenght = {0:.1f} [{1}]'.format(self.HSD.get_wl()[self.wl_idx], WL_UNIT))
-        if old_xlim_image != (0, 1):
-            self.image_ax.set_xlim(old_xlim_image)
-            self.image_ax.set_ylim(old_ylim_image)
-
-        self.spectral_ax.set_xlabel(f'Wavelength [{WL_UNIT}]')
-        self.spectral_ax.set_ylabel('Reflectance [-]')
-        if old_xlim_spectral != (0, 1):
-            self.spectral_ax.set_xlim(old_xlim_spectral)
-
-        # draw new canvas
-        self.fig.canvas.draw()
-
-    class SpectrumPoint:
-        """ Helper class to manage points for which the spectrum is requested """
-        colors = ['#006BA4', '#FF800E', '#ABABAB', '#595959', '#5F9ED1', '#C85200', '#898989', '#A2C8EC', '#FFBC79',
-                  '#CFCFCF']
-        picker_tolerance = 5
-        marker = 'o'
-        marker_size = 10
-
-        def __init__(self, Xpos, Ypos, unique_id):
-            self.x = Xpos
-            self.y = Ypos
-            self.id = unique_id
-            self.color = self.colors[self.id % len(self.colors)]
-            self.point_artist = None  # initialize artist in image axis to None untill first draw
-            self.line_artist = None  # initialize artist in spectral axis to None untill first draw
-
-        def draw_point(self, axis):
-            self.point_artist = axis.plot(self.x, self.y, color=self.color, marker=self.marker, picker=True,
-                                          pickradius=self.picker_tolerance)[0]
-            self.point_artist.obj = self
-
-        def draw_spectrum(self, axis, wl, spectrum):
-            axis.plot(wl, spectrum, color=self.color)
-
-class MaskCreator(object):
-    """Draw mask using selector
-    """
-    def __init__(self, ax, selector = 'polygon'):
-        ''' Selector can be 'lasso' or 'polygon' or 'points'
-        '''
-        if selector == 'lasso':
-            self.selector = LassoSelector(ax,
-                                          self.onselect,
-                                          lineprops={'color':'r','linewidth':5})
-        elif selector == 'polygon':
-            self.selector = PolygonSelector(ax,
-                                            self.onselect,
-                                            useblit=True,
-                                            lineprops={'color':'r'},
-                                            markerprops={'color':'r'})
-        else:
-            raise ValueError(f'Unknown selector value "{selector}" ')
-        
-        self.path = None
-
-    def get_mask(self, shape):
-        """Return image mask given by mask creator"""
-        if self.path is None:
-            return np.zeros(shape,dtype=bool)
-        h, w = shape
-        y, x = np.mgrid[:h, :w]
-        points = np.transpose((x.ravel(), y.ravel()))
-        grid = self.path.contains_points(points)  # now you have a mask with points inside a polygon
-        return grid.reshape(h, w)
-
-    def onselect(self, verts):
-        self.path = Path(verts)
-
-class PointsCreator(object):
-    def __init__(self, ax):
-        self.fig = ax.get_figure()
-        self.fig.canvas.mpl_connect('button_press_event', self.on_press)
-        self.fig.canvas.mpl_connect('pick_event', self.on_pick)
-        self.ax = ax
-
-        self.marker = 'o'
-        self.picker_tolerance = 5
-        self.color = 'red'
-
-        self.points = list()
-
-    def on_press(self, event):
-        if not event.dblclick:
-            #only select with double click, protects you against points when using tools or when removing point
-            return
-        x= round(event.xdata)
-        y = round(event.ydata)
-        point = (x,y)
-        self.points.append(point)
-        point_artist = self.ax.plot(x, y, color=self.color, marker=self.marker, picker=True, pickradius=self.picker_tolerance)[0]
-        point_artist.obj = point #link point to artist 
-        print(self.points)
-        self.update()
-
-    def update(self):
-         # save x/y limits of axes to retain zoom ratio when updating window
-        old_xlim_image = self.ax.get_xlim()
-        old_ylim_image = self.ax.get_ylim()
-
-        self.fig.canvas.draw()
-
-        if old_xlim_image != (0, 1):
-            self.ax.set_xlim(old_xlim_image)
-            self.ax.set_ylim(old_ylim_image)
-
-    def on_pick(self, event):
-        if event.mouseevent.button == 3:
-            print(event.artist)
-            # remove point if right-clicked
-            self.points.remove(event.artist.obj)
-            event.artist.remove()
-        self.update()
-
-    def get_mask(self, shape):
-        """Return image mask given by mask creator"""
-        mask =  np.zeros(shape,dtype=bool)
-        for x,y in self.points:
-            mask[y,x] = True
-        return mask
-    
-def mask_creator_demo():
-    img = np.random.uniform(0, 255, size=(100, 100))
-    ax = pyplot.subplot(111)
-    ax.imshow(img)
-
-    mc = MaskCreator(ax, 'lasso')
-    pyplot.show()
-
-    mask = mc.get_mask(img.shape)
-    img[~mask] = np.uint8(np.clip(img[~mask] - 100., 0, 255))
-    pyplot.imshow(img)
-    pyplot.title('Region outside of mask is darkened')
-    pyplot.show()
-
-def points_creator_demo():
-    img = np.random.uniform(0, 255, size=(100, 100))
-    ax = pyplot.subplot(111)
-    ax.imshow(img)
-
-    mc = PointsCreator(ax)
-    pyplot.show()
-
-    mask = mc.get_mask(img.shape)
-    pyplot.imshow(mask)
-    pyplot.show()
-
-if __name__ == '__main__':
-    points_creator_demo()
+from matplotlib import pyplot
+from matplotlib.path import Path
+from matplotlib.widgets import PolygonSelector, LassoSelector
+import numpy as np
+
+from .. import WL_UNIT, WL_UNIT_LONG
+
+class Gui(object):
+    """ Helper class for managing a gui for exploring an HyperSpectralDataset object """
+
+    def __init__(self, HSD):
+        self.HSD = HSD
+
+        self.wl_idx = 0
+        included_image = self.HSD.get_included_image()
+        row_idx, col_idx = np.nonzero(included_image)
+        # list of type SpectrumPoint. Initialise with some point inside included data
+        self.spectra = [self.SpectrumPoint(col_idx[0], row_idx[0], 0)]
+
+        self.selected_point = None
+        self.selected_line = None
+
+        self.vline_artist = None
+
+        self.fig, [self.image_ax, self.spectral_ax] = pyplot.subplots(1, 2)
+
+        self.fig.canvas.mpl_connect('pick_event', self.on_pick)
+        self.fig.canvas.mpl_connect('button_press_event', self.on_press)
+        self.fig.canvas.mpl_connect('button_release_event', self.on_release)
+        self.fig.canvas.mpl_connect('key_press_event', self.on_key)
+        self.fig.canvas.mpl_connect('motion_notify_event', self.on_motion)
+
+    def on_press(self, event):
+        if self.selected_point is not None or self.selected_line is not None:
+            return
+        if not event.dblclick:
+            # TODO: make sure only add spectrum when press event is in image axis.
+            # Watch out with notebook!! -> event.isaxis == self.image_ax doesn't work.
+            return
+        # add new SpectrumPoint to list of spectra
+        self.spectra.append(self.SpectrumPoint(round(event.xdata), round(event.ydata), len(self.spectra) + 1))
+
+        self.update_axes()
+
+    def on_key(self, event):
+        if event.key == 'left':
+            self.wl_idx = max([0, self.wl_idx - 1])
+            self.update_axes()
+        elif event.key == 'right':
+            self.wl_idx = min([self.HSD.get_dimL(), self.wl_idx + 1])
+            self.update_axes()
+
+    def on_pick(self, event):
+        if event.mouseevent.button == 3:
+            # remove point if right-clicked
+            self.spectra.remove(event.artist.obj)
+            self.update_axes()
+        elif event.mouseevent.button == 1:
+            if hasattr(event.artist, 'obj'):
+                self.selected_point = event.artist
+            elif self.vline_artist == event.artist:
+                self.selected_line = event.artist
+
+    def on_motion(self, event):
+        if self.selected_line is None and self.selected_point is None:
+            return
+        elif self.selected_point is not None and event.xdata is not None:
+            self.selected_point.obj.x = round(event.xdata)
+            self.selected_point.obj.y = round(event.ydata)
+            self.update_axes()
+        elif self.selected_line is not None and event.xdata is not None:
+            request_wl = np.clip(round(event.xdata), min(self.HSD.get_wl()), max(self.HSD.get_wl()))
+            self.wl_idx = self.HSD.get_wl_idx(request_wl)
+            self.update_axes()
+
+    def on_release(self, event):
+        self.selected_line = None
+        self.selected_point = None
+
+    def update_axes(self):
+
+        # save x/y limits of axes to retain zoom ratio when updating window
+        old_xlim_image = self.image_ax.get_xlim()
+        old_ylim_image = self.image_ax.get_ylim()
+
+        old_xlim_spectral = self.spectral_ax.get_xlim()
+
+        # clear axes
+        self.image_ax.clear()
+        self.spectral_ax.clear()
+
+        # show band image in image axis
+        self.image_ax.imshow(self.HSD.get_band_image(self.wl_idx))
+
+        # indicate wavelength
+        self.vline_artist = self.spectral_ax.axvline(x=self.HSD.get_wl()[self.wl_idx], color='k', picker=True,
+                                                     pickradius=20)
+
+        # plot points and spectra for each spectrum in list with SpectrumPoints
+        for spectrum in self.spectra:
+            # draw point in image axis
+            spectrum.draw_point(self.image_ax)
+
+            # draw spectrum in spectral axis
+            spectrum.draw_spectrum(self.spectral_ax, self.HSD.get_wl(),
+                                   self.HSD.get_spectrum_at(spectrum.y, spectrum.x))
+
+        # format axes titles and labels
+        self.image_ax.set_title('Wavelenght = {0:.1f} [{1}]'.format(self.HSD.get_wl()[self.wl_idx], WL_UNIT))
+        if old_xlim_image != (0, 1):
+            self.image_ax.set_xlim(old_xlim_image)
+            self.image_ax.set_ylim(old_ylim_image)
+
+        self.spectral_ax.set_xlabel(f'Wavelength [{WL_UNIT}]')
+        self.spectral_ax.set_ylabel('Reflectance [-]')
+        if old_xlim_spectral != (0, 1):
+            self.spectral_ax.set_xlim(old_xlim_spectral)
+
+        # draw new canvas
+        self.fig.canvas.draw()
+
+    class SpectrumPoint:
+        """ Helper class to manage points for which the spectrum is requested """
+        colors = ['#006BA4', '#FF800E', '#ABABAB', '#595959', '#5F9ED1', '#C85200', '#898989', '#A2C8EC', '#FFBC79',
+                  '#CFCFCF']
+        picker_tolerance = 5
+        marker = 'o'
+        marker_size = 10
+
+        def __init__(self, Xpos, Ypos, unique_id):
+            self.x = Xpos
+            self.y = Ypos
+            self.id = unique_id
+            self.color = self.colors[self.id % len(self.colors)]
+            self.point_artist = None  # initialize artist in image axis to None untill first draw
+            self.line_artist = None  # initialize artist in spectral axis to None untill first draw
+
+        def draw_point(self, axis):
+            self.point_artist = axis.plot(self.x, self.y, color=self.color, marker=self.marker, picker=True,
+                                          pickradius=self.picker_tolerance)[0]
+            self.point_artist.obj = self
+
+        def draw_spectrum(self, axis, wl, spectrum):
+            axis.plot(wl, spectrum, color=self.color)
+
+class MaskCreator(object):
+    """Draw mask using selector
+    """
+    def __init__(self, ax, selector = 'polygon'):
+        ''' Selector can be 'lasso' or 'polygon' or 'points'
+        '''
+        if selector == 'lasso':
+            self.selector = LassoSelector(ax,
+                                          self.onselect,
+                                          props=dict(color='red'))
+        elif selector == 'polygon':
+            self.selector = PolygonSelector(ax,
+                                            self.onselect,
+                                            useblit=True,
+                                            props=dict(color='red'))
+        else:
+            raise ValueError(f'Unknown selector value "{selector}" ')
+        
+        self.path = None
+
+    def get_mask(self, shape):
+        """Return image mask given by mask creator"""
+        if self.path is None:
+            return np.zeros(shape,dtype=bool)
+        h, w = shape
+        y, x = np.mgrid[:h, :w]
+        points = np.transpose((x.ravel(), y.ravel()))
+        grid = self.path.contains_points(points)  # now you have a mask with points inside a polygon
+        return grid.reshape(h, w)
+
+    def onselect(self, verts):
+        self.path = Path(verts)
+
+class PointsCreator(object):
+    def __init__(self, ax):
+        self.fig = ax.get_figure()
+        self.fig.canvas.mpl_connect('button_press_event', self.on_press)
+        self.fig.canvas.mpl_connect('pick_event', self.on_pick)
+        self.ax = ax
+
+        self.marker = 'o'
+        self.picker_tolerance = 5
+        self.color = 'red'
+
+        self.points = list()
+
+    def on_press(self, event):
+        if not event.dblclick:
+            #only select with double click, protects you against points when using tools or when removing point
+            return
+        x= round(event.xdata)
+        y = round(event.ydata)
+        point = (x,y)
+        self.points.append(point)
+        point_artist = self.ax.plot(x, y, color=self.color, marker=self.marker, picker=True, pickradius=self.picker_tolerance)[0]
+        point_artist.obj = point #link point to artist 
+        self.update()
+
+    def update(self):
+         # save x/y limits of axes to retain zoom ratio when updating window
+        old_xlim_image = self.ax.get_xlim()
+        old_ylim_image = self.ax.get_ylim()
+
+        self.fig.canvas.draw()
+
+        if old_xlim_image != (0, 1):
+            self.ax.set_xlim(old_xlim_image)
+            self.ax.set_ylim(old_ylim_image)
+
+    def on_pick(self, event):
+        if event.mouseevent.button == 3:
+            # remove point if right-clicked
+            self.points.remove(event.artist.obj)
+            event.artist.remove()
+        self.update()
+
+    def get_mask(self, shape):
+        """Return image mask given by mask creator"""
+        mask =  np.zeros(shape,dtype=bool)
+        for x,y in self.points:
+            mask[y,x] = True
+        return mask
+    
+def mask_creator_demo():
+    img = np.random.uniform(0, 255, size=(100, 100))
+    ax = pyplot.subplot(111)
+    ax.imshow(img)
+
+    mc = MaskCreator(ax, 'lasso')
+    pyplot.show()
+
+    mask = mc.get_mask(img.shape)
+    img[~mask] = np.uint8(np.clip(img[~mask] - 100., 0, 255))
+    pyplot.imshow(img)
+    pyplot.title('Region outside of mask is darkened')
+    pyplot.show()
+
+def points_creator_demo():
+    img = np.random.uniform(0, 255, size=(100, 100))
+    ax = pyplot.subplot(111)
+    ax.imshow(img)
+
+    mc = PointsCreator(ax)
+    pyplot.show()
+
+    mask = mc.get_mask(img.shape)
+    pyplot.imshow(mask)
+    pyplot.show()
+
+if __name__ == '__main__':
+    points_creator_demo()
     mask_creator_demo()
```

## phyper/chemometrics/analysis.py

```diff
@@ -1,358 +1,359 @@
-from abc import ABC, abstractmethod
-import numpy as np
-from copy import deepcopy
-
-from .dataset import Dataset, SpectralDataset, HyperSpectralDataset
-from .preprocessing import MeanCenter
-
-from sklearn import cross_decomposition, svm, decomposition, cluster
-from skimage import segmentation
-from scipy import interpolate
-
-class Analysis(ABC):
-
-    def __init__(self):
-        super().__init__()
-        self.X_cal = None
-        self.Y_cal = None
-        self.preprocessing_list = None
-        self.model = None
-
-    def set_calibration_data(self, X_cal=None, Y_cal=None, copy=True):
-        if isinstance(X_cal, Dataset):
-            self.preprocessing_list = deepcopy(X_cal.preprocess_list)
-            is_mean_centered = False
-            for preprocess in self.preprocessing_list:
-             if isinstance(preprocess, MeanCenter):
-                is_mean_centered = True
-            if not is_mean_centered:
-                print('WARNING: Preprocessing does not contain mean-centering. Mean centering is often required for optimal algorithm performance!')
-        if copy:
-            self.X_cal = deepcopy(X_cal)
-            self.Y_cal = deepcopy(Y_cal)
-        else:
-            self.X_cal = X_cal
-            self.Y_cal = Y_cal
-
-    def has_preprocessing(self):
-        return bool(self.preprocessing_list)
-
-    def get_calibration_data(self):
-        """ Get shallow copy of X_cal and Y_cal"""
-        return self.X_cal, self.Y_cal
-    
-    def get_X_cal(self):
-        return self.get_calibration_data()[0]
-
-    def get_Y_cal(self):
-        if self.get_calibration_data()[1] is None:
-            if isinstance(self.get_X_cal(), Dataset) and self.get_X_cal().get_labels() is not None:
-                return self.get_X_cal().get_labels()
-            else:
-                return None
-        else:
-            return self.get_calibration_data()[1]
-
-    def return_as(self, result, input_data):
-        if isinstance(input_data, HyperSpectralDataset):
-            return np.reshape(result, input_data.get_image_size())
-        else:
-            return result
-
-# ----------------- Classification -----------------
-
-class Classification(Analysis):
-    """ Wrapper class for all classification classes (e.g. PLSDA/LDA/QDA/SVM...) """
-
-    def __init__(self):
-        super(Classification, self).__init__()
-
-    def calibrate(self, X_cal=None, Y_cal=None):
-        self.set_calibration_data(X_cal, Y_cal)
-
-        if self.get_X_cal() is None or self.get_Y_cal() is None:
-            raise ValueError('Can not calibrate with X_cal or Y_cal missing.')
-
-        self.model.fit(np.asarray(self.get_X_cal()), np.asarray(self.get_Y_cal()))
-
-    def predict(self, X_test):
-        X_test = deepcopy(X_test)
-        if isinstance(X_test, Dataset) and isinstance(self.get_X_cal(), Dataset):
-            X_test.copy_preprocess(self.get_X_cal())
-        class_labels = self.model.predict(X_test)
-        if isinstance(X_test, HyperSpectralDataset):
-            X_test.assign_labels(class_labels)
-            return X_test.get_label_image()
-        elif isinstance(X_test, Dataset):
-            X_test.assign_labels(class_labels)
-            return X_test.get_labels()
-        else:
-            return class_labels
-
-    def accuracy(self):
-        return sum(np.equal(self.predict(self.get_X_cal()), self.get_Y_cal())) / self.get_Y_cal().size
-
-class PLSDA(Classification):
-
-    def __init__(self, nb_latent_variables=2):
-        super(PLSDA, self).__init__()
-        self.nb_latent_variables = nb_latent_variables
-        self.model = cross_decomposition.PLSRegression(n_components=self.nb_latent_variables, scale=False)
-
-    def calibrate(self, X_cal=None, Y_cal=None):
-        self.set_calibration_data(X_cal, Y_cal)
-
-        if self.get_X_cal() is None:
-            raise ValueError('Can not calibrate PLSDA with X_cal missing.')
-        if self.get_Y_cal() is None:
-            raise ValueError('Can not calibrate PLSDA with Y_cal missing.')
-
-        Y_regression = self.class_to_regression(self.get_Y_cal())
-        print(np.asarray(X_cal).shape, np.asarray(Y_regression).shape)
-        self.model.fit(np.asarray(X_cal), np.asarray(Y_regression))
-
-    def predict(self, X_test, decision_rule=0.5):
-        X_test = deepcopy(X_test)
-        if isinstance(X_test, Dataset) and isinstance(self.get_X_cal(), Dataset):
-            if self.has_preprocessing():
-                X_test.preprocess_list = self.preprocessing_list
-                X_test.apply_preprocess()
-        Y_regression = self.model.predict(np.asarray(X_test))
-        class_labels = self.regression_to_class(Y_regression, decision_rule=decision_rule)
-        if isinstance(X_test, HyperSpectralDataset):
-            X_test.assign_labels(class_labels)
-            return X_test.get_label_image()
-        elif isinstance(X_test, Dataset):
-            X_test.assign_labels(class_labels)
-            return X_test.get_labels()
-        else:
-            return class_labels
-
-    def get_class_ids(self):
-        if self.get_Y_cal() is not None:
-            return np.unique(self.get_Y_cal())
-        else:
-            raise AttributeError('Please provide Y calibration data before requesting class ids')
-
-    def get_nb_classes(self):
-        """ TODO: make independed of changes in calibration data (because atm shallow copy)."""
-        return self.get_class_ids().size
-
-    def class_to_regression(self, Y_class):
-        nb_samples = Y_class.shape[0]
-        nb_classes = self.get_nb_classes()
-        class_ids = self.get_class_ids()
-
-        Y_reg = np.zeros((nb_samples, nb_classes), dtype=int)
-        for i in range(nb_classes):
-            Y_reg[:, i] = Y_class == class_ids[i]
-
-        return Y_reg
-
-    def regression_to_class(self, Y_regression, decision_rule=0.5):
-        """ decision rule options: 'most_probable' or float percentage (e.g. 0.5).
-        Uncertain values are returned as -1
-        """
-        assert self.get_nb_classes() == Y_regression.shape[1]
-
-        nb_samples, nb_classes = Y_regression.shape
-        class_ids = self.get_class_ids()
-
-        if isinstance(decision_rule, float):
-            binary_matrix = Y_regression > decision_rule
-
-        elif decision_rule == 'most_probable':
-            max_prop = np.amax(Y_regression, axis=1)
-            binary_matrix = np.equal(Y_regression.transpose(), max_prop).transpose()
-        else:
-            raise ValueError('Unknown decision rule {0}'.format(decision_rule))
-
-        Y_class = np.full([nb_samples, ], -1, dtype=int)
-
-        for i in range(nb_classes):
-            Y_class[binary_matrix[:, i]] = class_ids[i]
-        return Y_class
-
-    def get_coeffs(self):
-        return self.model.coef_
-
-    def get_vips(self):
-        if self.model is not None:
-            t = self.model.x_scores_
-            w = self.model.x_weights_
-            q = self.model.y_loadings_
-            p, h = w.shape
-            vips = np.zeros((p,))
-            s = np.diag(t.T @ t @ q.T @ q).reshape(h, -1)
-            total_s = np.sum(s)
-            for i in range(p):
-                weight = np.array([(w[i, j] / np.linalg.norm(w[:, j])) ** 2 for j in range(h)])
-                vips[i] = np.sqrt(p * (s.T @ weight) / total_s)
-            return vips
-
-class SVM(Classification):
-
-    def __init__(self):
-        super(SVM, self).__init__()
-        self.model = svm.LinearSVC()
-# ----------------- Decomposition -----------------
-
-class Decomposition(Analysis):
-
-    def __init__(self):
-        super().__init__()
-
-    def calibrate(self, X_cal=None):
-        if X_cal is not None:
-            self.set_calibration_data(X_cal)
-
-        if self.get_X_cal() is None:
-            raise ValueError('Can not calibrate because no calibration data (X_cal) was provided')
-        else:
-            self.model.fit(self.get_X_cal())
-
-
-class PCA(Decomposition):
-
-    def __init__(self, number_of_components='mle'):
-        """ Create PCA model.
-            number_of_components: (int, float, 'mle', None)
-                - int: fixed number of components
-                - float: number between 0 and 1: find number of components that explains this percentage of variance
-                - 'mle' {default}: automaticaly find number of components based on max likelihood estimation
-                - None: take maximal number of components (based on nb_variables and nb_samples)"""
-
-        super().__init__()
-        self.model = decomposition.PCA(n_components=number_of_components)
-
-    def scores_plot(self, score_1, score_2):
-        scores_matrix = self.get_scores()
-        plt.scatter(scores_matrix[:, score_1], scores_matrix[:, score_2])
-        plt.show()
-
-    def plot_loadings(self):
-        plt.plot(self.get_loadings())
-        plt.show()
-
-    def get_scores(self):
-        return self.apply(self.get_X_cal())
-
-    def apply(self, X):
-        if self.model is None:
-            raise Exception('Please calibrate model before applying to test data')
-        else:
-            scores = self.model.transform(X)
-            if isinstance(X, HyperSpectralDataset):
-                return HyperSpectralDataset(
-                    hypercube=np.reshape(scores, [X.get_dimY(), X.get_dimX(), self.get_nb_components()]))
-            elif isinstance(X, Dataset):
-                return Dataset(scores)
-            else:
-                return scores
-
-    def get_loadings(self):
-        if self.model is None:
-            raise Exception('Please calibrate model before getting score')
-        else:
-            return self.model.components_
-
-    def get_nb_components(self):
-        if self.model is None:
-            raise Exception('Please calibrate model before getting score')
-        else:
-            return self.model.n_components_
-
-
-class Spline(Analysis):
-    """ good website with information on splines: https://observablehq.com/@herbps10/b-splines"""
-
-    def __init__(self, nb_splines, spline_degree=2):
-        """ Default: cubic spline (degree 2)"""
-        super().__init__()
-        self.nb_splines = nb_splines
-        self.spline_degree = spline_degree
-
-    def apply(self, X):
-        data_array = np.asarray(X)
-        nb_samples = data_array.shape[0]
-        spline_coeff_array = np.zeros((nb_samples, self.nb_splines))
-        predicted_data = np.zeros(data_array.shape)
-
-        # work with wavelengths as x for Spectral data
-        if isinstance(X, SpectralDataset):
-            x = X.get_wl()
-        else:
-            x = np.linspace(0, data_array.shape[1])
-
-        # iterate over all samples. Fit least squares spline estimation for each sample
-        for i in range(nb_samples):
-            nb_knots = self.nb_splines - 2 * self.spline_degree
-            knots = np.linspace(x[0], x[-1], nb_knots)
-            knots = knots[1:-1]
-            y = data_array[i]
-
-            t, c, k = interpolate.splrep(x=x, y=y, k=self.spline_degree, t=knots)
-
-            spline_coeff_array[i] = c
-            # predicted_data[i] = sp_interp.splev(x,(t,c,k))
-
-        if isinstance(X, HyperSpectralDataset):
-            return HyperSpectralDataset(
-                hypercube=np.reshape(spline_coeff_array, [X.get_dimY(), X.get_dimX(), self.nb_splines]), wavelength=t)
-        if isinstance(X, SpectralDataset):
-            return SpectralDataset(spline_coeff_array, t)
-        elif isinstance(X, Dataset):
-            return Dataset(spline_coeff_array)
-        else:
-            return spline_coeff_array
-
-# ----------------- Clustering -----------------
-
-class Cluster(Analysis):
-
-    def __init__(self):
-        super().__init__()
-
-
-class KMeans(Cluster):
-
-    def __init__(self, n_clusters=8):
-        super().__init__()
-        self.model = cluster.MiniBatchKMeans(n_clusters=n_clusters)
-
-    def apply(self, X):
-        self.set_calibration_data(X_cal=X)
-        return self.return_as(self.model.fit_predict(X=X), X)
-
-class SlicKMeans(Cluster):
-    """ Class for fast clustering of Hyperspectral Images.
-
-    First a SLIC will be performed on the fake RGB image. In a second step, the mean spectrum from each superpixel will be clustered.
-    """
-
-    def __init__(self, n_clusters=8, n_pixels=1000):
-        super().__init__()
-        self.n_clusters = n_clusters
-        self.n_pixels = n_pixels
-
-    def apply(self, X):
-        if not isinstance(X, HyperSpectralDataset):
-            raise ValueError('SlicKMeans algorithm can only be applied to objects of class "HypespectralDataset"')
-        else:
-            self.set_calibration_data(X_cal=X)
-
-            #determine superpixels and extract mean spectra
-            slic_seg = segmentation.slic(self.get_X_cal().get_rgb(), n_segments=self.n_pixels, start_label=1)
-            self.get_X_cal().assign_label_image(slic_seg)
-            data, labels = self.get_X_cal()._get_mean_data()
-
-            #cluster mean spectra
-            cluster_labels = cluster.MiniBatchKMeans(n_clusters=self.n_clusters).fit_predict(data)
-
-            #reconstruct label image with cluster output
-            #TODO: make fool proof is nuber of clusters is creater than 255
-            label_image = np.full(self.get_X_cal().get_image_size(), fill_value=0, dtype=np.uint8)
-            for i in range(len(labels)):
-                label_image[slic_seg == labels[i]] = cluster_labels[i]
-            return label_image
-
+from abc import ABC, abstractmethod
+import numpy as np
+from copy import deepcopy
+
+from .dataset import Dataset, SpectralDataset, HyperSpectralDataset
+from .preprocessing import MeanCenter
+
+from sklearn import cross_decomposition, svm, decomposition, cluster
+from skimage import segmentation
+from scipy import interpolate
+
+class Analysis(ABC):
+
+    def __init__(self):
+        super().__init__()
+        self.X_cal = None
+        self.Y_cal = None
+        self.preprocessing_list = None
+        self.model = None
+
+    def set_calibration_data(self, X_cal=None, Y_cal=None, copy=True):
+        if isinstance(X_cal, Dataset):
+            self.preprocessing_list = deepcopy(X_cal.preprocess_list)
+            is_mean_centered = False
+            for preprocess in self.preprocessing_list:
+             if isinstance(preprocess, MeanCenter):
+                is_mean_centered = True
+            if not is_mean_centered:
+                print('WARNING: Preprocessing does not contain mean-centering. Mean centering is often required for optimal algorithm performance!')
+        if copy:
+            self.X_cal = deepcopy(X_cal)
+            self.Y_cal = deepcopy(Y_cal)
+        else:
+            self.X_cal = X_cal
+            self.Y_cal = Y_cal
+
+    def has_preprocessing(self):
+        return bool(self.preprocessing_list)
+
+    def get_calibration_data(self):
+        """ Get shallow copy of X_cal and Y_cal"""
+        return self.X_cal, self.Y_cal
+    
+    def get_X_cal(self):
+        return self.get_calibration_data()[0]
+
+    def get_Y_cal(self):
+        if self.get_calibration_data()[1] is None:
+            if isinstance(self.get_X_cal(), Dataset) and self.get_X_cal().get_labels() is not None:
+                return self.get_X_cal().get_labels()
+            else:
+                return None
+        else:
+            return self.get_calibration_data()[1]
+
+    def return_as(self, result, input_data):
+        if isinstance(input_data, HyperSpectralDataset):
+            return np.reshape(result, input_data.get_image_size())
+        else:
+            return result
+
+# ----------------- Classification -----------------
+
+class Classification(Analysis):
+    """ Wrapper class for all classification classes (e.g. PLSDA/LDA/QDA/SVM...) """
+
+    def __init__(self):
+        super(Classification, self).__init__()
+
+    def calibrate(self, X_cal=None, Y_cal=None):
+        self.set_calibration_data(X_cal, Y_cal)
+
+        if self.get_X_cal() is None or self.get_Y_cal() is None:
+            raise ValueError('Can not calibrate with X_cal or Y_cal missing.')
+
+        self.model.fit(np.asarray(self.get_X_cal()), np.asarray(self.get_Y_cal()))
+
+    def predict(self, X_test):
+        X_test = deepcopy(X_test)
+        if isinstance(X_test, Dataset) and isinstance(self.get_X_cal(), Dataset):
+            X_test.copy_preprocess(self.get_X_cal())
+        class_labels = self.model.predict(X_test)
+        if isinstance(X_test, HyperSpectralDataset):
+            X_test.assign_labels(class_labels)
+            return X_test.get_label_image()
+        elif isinstance(X_test, Dataset):
+            X_test.assign_labels(class_labels)
+            return X_test.get_labels()
+        else:
+            return class_labels
+
+    def accuracy(self):
+        return sum(np.equal(self.predict(self.get_X_cal()), self.get_Y_cal())) / self.get_Y_cal().size
+
+class PLSDA(Classification):
+
+    def __init__(self, nb_latent_variables=2):
+        super(PLSDA, self).__init__()
+        self.nb_latent_variables = nb_latent_variables
+        self.model = cross_decomposition.PLSRegression(n_components=self.nb_latent_variables, scale=False)
+
+    def calibrate(self, X_cal=None, Y_cal=None):
+        self.set_calibration_data(X_cal, Y_cal)
+
+        if self.get_X_cal() is None:
+            raise ValueError('Can not calibrate PLSDA with X_cal missing.')
+        if self.get_Y_cal() is None:
+            raise ValueError('Can not calibrate PLSDA with Y_cal missing.')
+
+        Y_regression = self.class_to_regression(self.get_Y_cal())
+        print(np.asarray(X_cal).shape, np.asarray(Y_regression).shape)
+        self.model.fit(np.asarray(X_cal), np.asarray(Y_regression))
+
+    def predict(self, X_test, decision_rule=0.5):
+        X_test = deepcopy(X_test)
+        if isinstance(X_test, Dataset) and isinstance(self.get_X_cal(), Dataset):
+            if self.has_preprocessing():
+                X_test.preprocess_list = self.preprocessing_list
+                X_test.apply_preprocess()
+        Y_regression = self.model.predict(np.asarray(X_test))
+        class_labels = self.regression_to_class(Y_regression, decision_rule=decision_rule)
+        if isinstance(X_test, HyperSpectralDataset):
+            X_test.assign_labels(class_labels)
+            return X_test.get_label_image()
+        elif isinstance(X_test, Dataset):
+            X_test.assign_labels(class_labels)
+            return X_test.get_labels()
+        else:
+            return class_labels
+
+    def get_class_ids(self):
+        if self.get_Y_cal() is not None:
+            return np.unique(self.get_Y_cal())
+        else:
+            raise AttributeError('Please provide Y calibration data before requesting class ids')
+
+    def get_nb_classes(self):
+        """ TODO: make independed of changes in calibration data (because atm shallow copy)."""
+        return self.get_class_ids().size
+
+    def class_to_regression(self, Y_class):
+        nb_samples = Y_class.shape[0]
+        nb_classes = self.get_nb_classes()
+        class_ids = self.get_class_ids()
+
+        Y_reg = np.zeros((nb_samples, nb_classes), dtype=int)
+        for i in range(nb_classes):
+            Y_reg[:, i] = Y_class == class_ids[i]
+
+        return Y_reg
+
+    def regression_to_class(self, Y_regression, decision_rule=0.5):
+        """ decision rule options: 'most_probable' or float percentage (e.g. 0.5).
+        Uncertain values are returned as -1
+        """
+        assert self.get_nb_classes() == Y_regression.shape[1]
+
+        nb_samples, nb_classes = Y_regression.shape
+        class_ids = self.get_class_ids()
+
+        if isinstance(decision_rule, float):
+            binary_matrix = Y_regression > decision_rule
+
+        elif decision_rule == 'most_probable':
+            max_prop = np.amax(Y_regression, axis=1)
+            binary_matrix = np.equal(Y_regression.transpose(), max_prop).transpose()
+        else:
+            raise ValueError('Unknown decision rule {0}'.format(decision_rule))
+
+        Y_class = np.full([nb_samples, ], -1, dtype=int)
+
+        for i in range(nb_classes):
+            Y_class[binary_matrix[:, i]] = class_ids[i]
+        return Y_class
+
+    def get_coeffs(self):
+        return self.model.coef_
+
+    def get_vips(self):
+        if self.model is not None:
+            t = self.model.x_scores_
+            w = self.model.x_weights_
+            q = self.model.y_loadings_
+            p, h = w.shape
+            vips = np.zeros((p,))
+            s = np.diag(t.T @ t @ q.T @ q).reshape(h, -1)
+            total_s = np.sum(s)
+            for i in range(p):
+                weight = np.array([(w[i, j] / np.linalg.norm(w[:, j])) ** 2 for j in range(h)])
+                vips[i] = np.sqrt(p * (s.T @ weight) / total_s)
+            return vips
+
+class SVM(Classification):
+
+    def __init__(self):
+        super(SVM, self).__init__()
+        self.model = svm.LinearSVC()
+# ----------------- Decomposition -----------------
+
+class Decomposition(Analysis):
+
+    def __init__(self):
+        super().__init__()
+
+    def calibrate(self, X_cal=None):
+        if X_cal is not None:
+            self.set_calibration_data(X_cal)
+
+        if self.get_X_cal() is None:
+            raise ValueError('Can not calibrate because no calibration data (X_cal) was provided')
+        else:
+            self.model.fit(self.get_X_cal())
+
+
+class PCA(Decomposition):
+
+    def __init__(self, number_of_components='mle'):
+        """ Create PCA model.
+            number_of_components: (int, float, 'mle', None)
+                - int: fixed number of components
+                - float: number between 0 and 1: find number of components that explains this percentage of variance
+                - 'mle' {default}: automaticaly find number of components based on max likelihood estimation
+                - None: take maximal number of components (based on nb_variables and nb_samples)"""
+
+        super().__init__()
+        self.model = decomposition.PCA(n_components=number_of_components)
+
+    def scores_plot(self, score_1, score_2):
+        scores_matrix = self.get_scores()
+        plt.scatter(scores_matrix[:, score_1], scores_matrix[:, score_2])
+        plt.show()
+
+    def plot_loadings(self):
+        plt.plot(self.get_loadings())
+        plt.show()
+
+    def get_scores(self):
+        return self.apply(self.get_X_cal())
+
+    def apply(self, X):
+        if self.model is None:
+            raise Exception('Please calibrate model before applying to test data')
+        else:
+            scores = self.model.transform(X)
+            scores = scores.astype(X.get_HC().dtype)
+            if isinstance(X, HyperSpectralDataset):
+                return HyperSpectralDataset(
+                    hypercube=np.reshape(scores, [X.get_dimY(), X.get_dimX(), self.get_nb_components()]))
+            elif isinstance(X, Dataset):
+                return Dataset(scores)
+            else:
+                return scores
+
+    def get_loadings(self):
+        if self.model is None:
+            raise Exception('Please calibrate model before getting score')
+        else:
+            return self.model.components_
+
+    def get_nb_components(self):
+        if self.model is None:
+            raise Exception('Please calibrate model before getting score')
+        else:
+            return self.model.n_components_
+
+
+class Spline(Analysis):
+    """ good website with information on splines: https://observablehq.com/@herbps10/b-splines"""
+
+    def __init__(self, nb_splines, spline_degree=2):
+        """ Default: cubic spline (degree 2)"""
+        super().__init__()
+        self.nb_splines = nb_splines
+        self.spline_degree = spline_degree
+
+    def apply(self, X):
+        data_array = np.asarray(X)
+        nb_samples = data_array.shape[0]
+        spline_coeff_array = np.zeros((nb_samples, self.nb_splines))
+        predicted_data = np.zeros(data_array.shape)
+
+        # work with wavelengths as x for Spectral data
+        if isinstance(X, SpectralDataset):
+            x = X.get_wl()
+        else:
+            x = np.linspace(0, data_array.shape[1])
+
+        # iterate over all samples. Fit least squares spline estimation for each sample
+        for i in range(nb_samples):
+            nb_knots = self.nb_splines - 2 * self.spline_degree
+            knots = np.linspace(x[0], x[-1], nb_knots)
+            knots = knots[1:-1]
+            y = data_array[i]
+
+            t, c, k = interpolate.splrep(x=x, y=y, k=self.spline_degree, t=knots)
+
+            spline_coeff_array[i] = c
+            # predicted_data[i] = sp_interp.splev(x,(t,c,k))
+
+        if isinstance(X, HyperSpectralDataset):
+            return HyperSpectralDataset(
+                hypercube=np.reshape(spline_coeff_array, [X.get_dimY(), X.get_dimX(), self.nb_splines]), wavelength=t)
+        if isinstance(X, SpectralDataset):
+            return SpectralDataset(spline_coeff_array, t)
+        elif isinstance(X, Dataset):
+            return Dataset(spline_coeff_array)
+        else:
+            return spline_coeff_array
+
+# ----------------- Clustering -----------------
+
+class Cluster(Analysis):
+
+    def __init__(self):
+        super().__init__()
+
+
+class KMeans(Cluster):
+
+    def __init__(self, n_clusters=8):
+        super().__init__()
+        self.model = cluster.MiniBatchKMeans(n_clusters=n_clusters)
+
+    def apply(self, X):
+        self.set_calibration_data(X_cal=X)
+        return self.return_as(self.model.fit_predict(X=X), X)
+
+class SlicKMeans(Cluster):
+    """ Class for fast clustering of Hyperspectral Images.
+
+    First a SLIC will be performed on the fake RGB image. In a second step, the mean spectrum from each superpixel will be clustered.
+    """
+
+    def __init__(self, n_clusters=8, n_pixels=1000):
+        super().__init__()
+        self.n_clusters = n_clusters
+        self.n_pixels = n_pixels
+
+    def apply(self, X):
+        if not isinstance(X, HyperSpectralDataset):
+            raise ValueError('SlicKMeans algorithm can only be applied to objects of class "HypespectralDataset"')
+        else:
+            self.set_calibration_data(X_cal=X)
+
+            #determine superpixels and extract mean spectra
+            slic_seg = segmentation.slic(self.get_X_cal().get_rgb(), n_segments=self.n_pixels, start_label=1)
+            self.get_X_cal().assign_label_image(slic_seg)
+            data, labels = self.get_X_cal()._get_mean_data()
+
+            #cluster mean spectra
+            cluster_labels = cluster.MiniBatchKMeans(n_clusters=self.n_clusters).fit_predict(data)
+
+            #reconstruct label image with cluster output
+            #TODO: make fool proof is nuber of clusters is creater than 255
+            label_image = np.full(self.get_X_cal().get_image_size(), fill_value=0, dtype=np.uint8)
+            for i in range(len(labels)):
+                label_image[slic_seg == labels[i]] = cluster_labels[i]
+            return label_image
+
```

## phyper/chemometrics/dataset.py

```diff
@@ -1,1234 +1,1246 @@
-import os
-from tracemalloc import start
-import numpy as np
-import h5py
-from matplotlib import pyplot
-from pytz import NonExistentTimeError
-from skimage.color import label2rgb
-from skimage import transform
-from typing import Optional, Union
-
-from .preprocessing import _Preprocess
-from ._gui import Gui, MaskCreator
-from .. import WL_UNIT, WL_UNIT_LONG
-from copy import deepcopy
-from spectral import open_image
-from scipy.signal import medfilt
-
-def _docstring_parameter(*sub):
-    def dec(obj):
-        obj.__doc__ = obj.__doc__.format(*sub)
-        return obj
-    return dec
-
-class Dataset(object):
-    """
-    Class for creating a simple dataset with N samples and M variables
-    """
-
-    def __init__(self, data, labels=None, label_table = []):
-        """ Create a Dataset from the N-by-M numpy array with N samples and M variables.
-
-        Parameters
-        ----------
-        data : ndarray
-            A 2-D array of shape (N, M) with N the number of samples and M the number of variables.
-        labels : ndarray, optional
-            A 1-D array of shape (N,) with label ID's for every sample. Label ID's should be integers that can be found in `label_table`.
-            If the integer can not be found in the label_table, or no label table is provided, a default label tabel will be generated.
-        label_table : list of tuples, optional
-            A list of tuples, where every tuple has the format (label_id, label_name). E.g. label_table = [(1, "good"),(2, "bad")].
-        """
-
-        # initialise empty preprocessing list
-        self.preprocess_list = []
-        self.catched_preprocess_list = []
-
-        # initialise data and data_pre
-        # data_pre is a cache for the data that has been preprocessed based on the preprocessing list.
-        self.data = None
-        self.catched_data_preproc = None
-        # initialize data by setting the data to the given data
-        self._set_data(data)
-
-        #assign labels
-        self.labels = labels
-        self.label_table = label_table
-        self._fill_label_table()
-
-    def __array__(self, dtype=None):
-        return self.get_data().copy()
-
-    def __len__(self):
-        return self.get_nb_samples()
-
-    def __repr__(self):
-        return ('A Dataset with size {0}x{1} and preprocessing {2}. {3} samples are included.'.format(self.get_nb_samples(),
-                                                                                                      self.get_nb_variables(),
-                                                                                                      self.preprocess_list,
-                                                                                                      self.get_nb_samples(original=True)))
-
-    @property
-    def shape(self):
-        """ Return the shape (N,M) of the dataset.
-
-        N is the number of samples and M is the number of variables.
-        """
-
-        return (self.get_nb_samples(), self.get_nb_variables)
-
-    def get_nb_samples(self, original=False) -> int:
-        if original:
-            return self.get_original_data().shape[0]
-        else:
-            return self.get_data().shape[0]
-
-    def get_nb_variables(self) -> int:
-        return self.get_data().shape[1]
-
-    def include_only_variables(self, variables_idx):
-        """ Make a selected of which variables to retrain in the dataset."""
-        self.data = self.data[:, variables_idx]
-        self.catched_data_preproc = None
-
-    def include_variables_from(self, start_idx, end_idx):
-        self.data = self.data[:, start_idx:end_idx]
-        self.catched_data_preproc = None
-    ############################# Data Handling #############################
-
-    def _set_data(self, data, included_samples=None, labels=None):
-        """ Set new data. RESTRICTED USE
-
-        This function allows to change data for this dataset.
-        As a result al labels and included samples will be reset or set to the given values.
-        """
-        assert(self._is_valid_data(data))
-        if included_samples is None:
-            self.included_samples = np.ones(data.shape[0], dtype=bool)
-        self.labels = labels
-        self.data = data
-
-        self.catched_data_preproc = None
-
-    @staticmethod
-    def _is_valid_data(data) -> bool:
-        """ Check if the given `data` has the correct format.
-
-        Data should be an numpy ndarray with a shape of the format (N,M).
-        """
-        if isinstance(data, np.ndarray):
-            return len(data.shape) == 2
-        else:
-            return False
-
-    def get_original_data(self):
-        """ Return the original data.
-
-        Original data means the data as intialy provided, without preprocessing and with all samples included.
-        """
-
-        return self.data
-
-    def get_data(self, preproc=True, fill_nans=False) -> np.ndarray:
-        """ Return the data as a numpy array.
-
-        Parameters
-        ----------
-        preproc : bool, default=True
-            If preprocessing is selected (default), the preprocessed data will be returned. Otherwise the raw data will be returned.
-        fill_nans : bool, default=False
-            By default only the included samples are given. If `fill_nans` is set to True however, the returned dataset will have the same shape as the original dataset, with excluded samples having NaN as value for all variables.
-
-        Returns
-        -------
-        data: ndarray
-            2D dimensional array of shape (K,M) where K is the number of included samples. If `fill_nans`, K is the total number of samples.
-
-        See Also
-        --------
-        get_original_data : Return the original data, without preprocessing and with the actual values for the excluded samples.
-        """
-        #check if preprocessed data is asked, and if so, check if catched preprocessing is still valid
-        if preproc and not self._is_valid_catch():
-            self.apply_preprocess()
-        
-        #check if asked to return filled, original or preprocessed data
-        if self.has_excluded_samples() and fill_nans:
-            data = np.full(self.data.shape, np.nan, dtype=self.data.dtype)
-            data[self.included_samples, :] = self.get_data(preproc=preproc, fill_nans=False)
-            return np.squeeze(data)
-        elif (self.catched_data_preproc is not None) and preproc:
-            data = self.catched_data_preproc
-        else:
-            data = self.get_original_data()
-
-        # indexing takes a lot more time so check if this is needed.
-        if self.has_excluded_samples():
-            return np.squeeze(data[self.included_samples, :])
-        else:
-            return data
-
-    ############################# Sample inclusion/exclusion #############################
-
-    def include(self, bool_inclusion):
-        """ Include only part of the samples based on a boolean array of shape (N,).
-
-        Parameters
-        ----------
-        bool_inclusion : ndarray
-            1-D boolean array of shape (N,) where N is the total number of samples.
-            Only samples that were already in the included samples can be included.
-
-        See Also
-        --------
-        include_all
-        """
-
-        self.included_samples = np.logical_and(self.included_samples, bool_inclusion)
-
-    def include_all(self):
-        """ Include all samples that were in the original dataset. Remove any exclusions.
-
-        See Also
-        --------
-        include
-        exclude_label
-        """
-
-        self.included_samples = np.ones(self.data.shape[0], dtype=bool)
-        #TODO: also check all labels are in label table
-
-    def has_excluded_samples(self) -> bool:
-        """ Check if any of the original datasamples has been excluded.
-        """
-
-        return np.any(np.logical_not(self.included_samples))
-
-    def exclude_label(self, label_id: int):
-        """ Exclude all samples with a given `label_id`.
-
-        Parameters
-        ----------
-        label_id : int
-            `label_id` should correspond to one of the labels_id - label_name pairs in the label_table.
-
-        See Also
-        --------
-        _has_label_id : Check if certain `label_id` is in the label_table.
-        """
-
-        if self.labels is not None:
-            if np.any(self.get_labels() == label_id):
-                self.include(self.labels != label_id)
-                if self._has_label_id(label_id=label_id):
-                    self.label_table.remove((label_id, self.get_label_name(label_id)))
-            else:
-                print('WARNING: Not able to exclude label {0} because it was not found in labels'.format(label_id))
-        else:
-            print('WARNING: Not able to exclude label {0} because not labels were found'.format(label_id))
-
-    ############################# Preprocessing #############################
-
-    def apply(func):
-        """ Decorator. Apply preprocessing after method that changes preprocessing list. """
-        def wrapper(self, *args):
-            func(self, *args)
-            self.apply_preprocess()
-
-        return wrapper
-
-    @apply
-    def add_preprocess(self, preprocess: _Preprocess, position=None, allow_double=False) -> None:
-        """ Add a preprocessing step to the preprocessing list.
-
-        This method allows to add a new preprocessing step to the preprocessing list.
-        This list of preprocessing steps will be applied to the data from index 0 to -1.
-
-        Parameters
-        ----------
-        preprocess : _Preprocess
-            Preprocessing object to be added to the preprocessing list.
-        position : int, optional
-            Position at which to add the new `preprocess` within the preprocessing list. If no position is given, the `preprocess` is added at the end of the list (default).
-        allow_double : bool, default=False
-            Normally the same type of preprocessing can not be added twice, unless `allow_double` is set to True.
-        """
-
-        assert(isinstance(preprocess, _Preprocess))
-        if preprocess in self.preprocess_list and not allow_double:
-            print("WARNING: \n New preprocess ({0}) was already in preprocessing list ({1}). \n If this is what you want, use allow_double=True".format(preprocess, self.preprocess_list))
-        else:
-            if position is None:
-                self.preprocess_list.append(preprocess)
-            else:
-                self.preprocess_list.insert(position, preprocess)
-
-    @apply
-    def remove_preprocess(self, position:int) -> None:
-        """ Remove a preprocessing step at a certain `position` from the prepocessing list.
-
-        Parameters
-        ----------
-        position: int
-            Index in preprocessing list.
-
-        See Also 
-        --------
-        print_preprocessing_list()
-        """
-
-        self.preprocess_list.pop(position)
-
-    def has_preprocessing(self) -> bool:
-        """ Check if there are preprocessing steps in the preprocessing list."""
-        return bool(self.preprocess_list)
-
-    @apply
-    def clear_preprocess(self):
-        """ Clear the preprocessing list. No preprocessing will be performed anymore.
-
-        See Also
-        --------
-        get_original_data : directly get the original data on which the preprocessing is being applied.
-        """
-        self.preprocess_list = []
-
-    @apply
-    def copy_preprocess(self, other: 'Dataset'):
-        """ Copy the preprocessing steps from an other Dataset (`other`).
-
-        This method allows to copy the preprocessing that has been performed on an other Dataset `other`, to your dataset.
-        This copying also includes any calibration data from the preprocessing that has been performed on `other` (e.g. mean centering).
-
-        Parameters
-        ---------
-        other: Dataset
-            Dataset from which to copy the list of preprocessing
-
-        Note
-        ----
-        When invocking this method, the new preprocessing list will directly be applied to the dataset. 
-        The original data are stored in parallel and can be accesed using get_original_data() or by using clear_preprocess().
-        """
-
-        assert isinstance(other, Dataset)
-        self.preprocess_list = deepcopy(other.preprocess_list)
-
-    def print_preprocessing_list(self):
-        """Print entire preprocessing list.
-        """
-
-        for idx, preproc in enumerate(self.preprocess_list):
-            print(f'[{idx}] {preproc}')
-
-    def _is_valid_catch(self):
-        """ Check if the catched preprocessing data is still valid (preprocessing not changed since last time applying preprocessing)
-        """
-
-        return self.preprocess_list == self.catched_preprocess_list
-
-    def apply_preprocess(self):
-        """ Apply all preprocessing steps in the preprocessing list, starting from `preprocess_list[0]`.
-
-        Normally these function does not have to be called explicitly, as it is called automaticly after every method that makes changes to the preprocessing list.
-
-        Note
-        ----
-        If the preprocessing list has not changed since the last time this method was invoced, the cached prepropressing data will be used.
-        """
-        if self._is_valid_catch():
-            return self.catched_data_preproc
-        elif self.preprocess_list:
-            self.catched_data_preproc = self.get_original_data().copy()
-            for preproc in self.preprocess_list:
-                self.catched_data_preproc = preproc.apply(self.catched_data_preproc)
-        else:
-            self.catched_data_preproc = None
-        self.catched_preprocess_list = self.preprocess_list
-
-    ############################# Labels #############################
-
-    def get_label_data(self, label_id):
-        """ Get the data belonging to samples with a certain `label_id`.
-
-        If no label data is available for this Dataset, all included samples are included in the returned array.
-
-        Parameters
-        ----------
-        label_id : int
-            The `label_id` should be one from the label_ids listed in the label table.
-
-        Return
-        ------
-        Numpy ndarray of shape (L,M) with L the number of samples for with as label id the given `label_id`.
-        If the `label_id` can not be found in the label table, None will be returned.
-
-        See Also
-        --------
-        get_label_table
-
-        """
-
-        if not self._has_labels():
-            print('No lables were found, returning all data')
-            return self.get_data()
-        else:
-            if self._has_label_id(label_id):
-                class_idx = self.get_labels() == label_id
-                return self.get_data()[class_idx, :]
-            else:
-                print('Label id ({0}) was not found in label table {1}'.format(label_id, str(self.label_table)))
-                return None
-
-    def assign_labels(self, labels, label_table=None):
-        """ Assign labels to the samples in the dataset.
-
-        Parameters
-        ----------
-        labels : ndarray
-            1-D array of shape (N,) with N the number of included samples
-        label_table : list[], optional
-            List of tuples where each tuple corresponds to a lable_id, label_name pair. E.g. label_table = [(0, "good"),(1,"bad")].
-            If no `label_table` is provided, a default label table will be created.
-        """
-        assert(labels.shape == (self.get_nb_samples(),))
-        self.labels = np.full(self.data.shape[0], 0, dtype=np.int)
-        self.labels[self.included_samples] = np.asarray(labels, dtype=int)
-        if label_table is not None:
-            for label in label_table:
-                label_id, label_name = label
-                self.add_label_id(label_id, label_name)
-        self._fill_label_table()
-
-    def _fill_label_table(self):
-        """ Check if there are any label_ids in the labels that are not in the label_table, and add these label_ids to the label_table with a defautl label_name ('ClassX')
-        """
-        if self._has_labels():
-            for x in np.unique(self.labels):
-                if not self._has_label_id(x):
-                    self.add_label_id(x, "Class_{}".format(x))
-
-    def get_labels(self, fill=False):
-        """ Get the labels belong to the samples of this dataset.
-
-
-        Parameters
-        ----------
-        fill : bool, default=False
-            By default only the labels for the included samples are given.
-            If `fill` is set to True, the excluded samples get -1 as label.
-
-        Returns
-        -------
-        labels: ndarrray or None
-            1-D array with shape (N,) where N is the number of included samples.
-            If `fill_nans` is set to True, N will be the total number of samples.
-            If the `label_id` was not found in the dataset, None will be returned.
-        """
-
-        if self.labels is not None:
-            if fill:
-                labels = np.full(self.labels.shape, -1, dtype=int)
-                labels[self.included_samples] = self.get_labels(fill=False)
-                return np.squeeze(labels).astype(int)
-            else:
-                return np.squeeze(self.labels[self.included_samples]).astype(int)
-        else:
-            return None
-
-    def _has_labels(self):
-        """ Check if labels are available for the samples."""
-        return self.get_labels() is not None
-
-    def _has_label_id(self, label_id):
-        for label_tuple in self.label_table:
-            if label_tuple[0] == label_id:
-                return True
-        return False
-
-    def add_label_id(self, label_id, label_name):
-        """ Add a label with a certain `label_id` and `label_name` to the label_table.
-        
-        Parameters
-        ----------
-        label_id : int
-            Unique id for the label. `label_id` should be different from the other label id's already present in the label_table.
-        label_name : str
-            Name for the label.
-        
-        See Also
-        --------
-        get_label_table
-        get_labels
-        """
-
-        if not self._has_label_id(label_id):
-            self.label_table.append((label_id, label_name))
-        else:
-            print('Label {0} was already in labeltabel with name {1} (instead of given name {2})'.format(label_id, self.get_label_name(label_id), label_name))
-
-    def get_label_name(self, label_id) -> Optional[str]:
-        """ Get the label name beloging to the `label_id`.
-        
-        Parameters
-        ---------
-        label_id : int
-            Label_id as can be found in the labels from this dataset.
-        
-        Returns
-        -------
-        name : str
-            Name for the given `label_id`. If the `label_id` was not found in the label_table, the method will return None.
-        
-        See Also
-        --------
-        get_labels
-        get_label_table
-        """
-
-        for label in self.label_table:
-            id, name = label
-            if label_id == id:
-                return name
-        return None
-
-    def get_nb_classes(self):
-        """ 
-        .. deprecated:: 0.0
-          `get_nb_classes` will be removed. Use get_nb_labels instead.
-        """
-
-        return self.get_nb_labels()
-
-    def get_nb_labels(self):
-        """ Get the total number of unique labels for all"""
-        if self.get_labels() is None:
-            return 0
-        else:
-            return np.unique(self.get_labels()).size
-
-    def get_label_table(self, include_quantity = False):
-        """ Get overview of labels as list of tuples with label tuples as (label_id,label_name) or (label_id,label_name,nb_of_labels) if include_quantity
-        """
-
-        if not include_quantity:
-            return deepcopy(self.label_table)
-        else:
-            label_table = list()
-            for label in self.label_table:
-                label_id, label_name = label
-                label_quantity = sum(self.get_labels()==label_id)
-                label_table.append((label_id, label_name,label_quantity))
-            return label_table
-
-    ############################# Utils #############################
-    def _get_mean_data(self, by_label=True) -> Union[tuple, np.ndarray]:
-        """ Get data mean. If labels are given, the mean for each label will be returned.
-        
-        Parameters
-        ----------
-        by_label : bool, optional
-            Indicate if needed to calculate the mean for each label seperatly. If not, the total mean of the data will be returned.
-        
-        Returns
-        -------
-        mean_data
-            If no labels are given or `by_label` is set to False, a 1-D array will be returned. 
-            Otherwise, a 2-D array will be returned with diffent rows corresponding to the mean of different lables.
-        labels_ids
-            If the mean is calcuted for the different labels, the `labels_ids` corresponding to the different rows are given.
-        """
-        if (self.get_nb_classes() == 0) or not by_label:
-            return np.mean(self.get_data(), axis=0)
-        else:
-            mean_data = np.full([self.get_nb_classes(), self.get_nb_variables()], fill_value=0, dtype=self.get_data().dtype)
-            label_ids = np.full([self.get_nb_classes(),], fill_value=0, dtype=self.get_labels().dtype)
-            i = 0
-            for label_id, labelname in self.get_label_table():
-                mean_data[i, :] = np.mean(self.get_label_data(label_id), axis=0)
-                label_ids[i] = label_id
-                i += 1
-            return mean_data, label_ids
-
-    def add(self, ds) -> None:
-        """ 
-        .. deprecated:: 0.0
-          `add` will be removed. Use merge instead.
-        """
-        print('WARNING: DEPRECATED : Please use merge instead')
-        new_data = np.concatenate((self.get_data(), ds.get_data()), axis=0)
-        if self._has_labels() and ds._has_labels():
-            new_labels = np.concatenate((self.get_labels(), ds.get_labels()), axis=0)
-        else:
-            new_labels = None
-        self._set_data(data=new_data, labels=new_labels)
-
-        #fix missing lables
-        for label_id, label_name in ds.label_table:
-            self.add_label_id(label_id, label_name)
-
-    def merge(self, ds : 'Dataset or SpectralDataset') -> 'Dataset or SpectralDataset':
-        """ Create a new Dataset by merging the current dataset with a new dataset `ds`.
-        
-        Parameters
-        ----------
-        ds : Dataset
-            New dataset to merge with the current dataset.
-        
-        Returns
-        -------
-        ds : Dataset
-            Merged dataset from the current dataset and `ds`.
-        """
-    
-        new_data = np.concatenate((self.get_data(), ds.get_data()), axis=0)
-        if self._has_labels() and ds._has_labels():
-            new_labels = np.concatenate((self.get_labels(), ds.get_labels()), axis=0)
-        else:
-            new_labels = None
-        if isinstance(ds, SpectralDataset):
-            ds = SpectralDataset(data=new_data, wavelength=ds.get_wl(), labels=new_labels, label_table=self.get_label_table())
-        else:
-            ds = Dataset(data=new_data, labels=new_labels, label_table=self.get_label_table())
-
-        #fix missing lables
-        for label_id, label_name in ds.label_table:
-            ds.add_label_id(label_id, label_name)
-        return ds
-
-    def plot(self, nb_samples=100, labels=True, label_ids = [], ax=None, show=True):
-        """ Visualise the dataset by plotting some samples.
-        
-        Parameters
-        ----------
-        nb_samples : int, default=100
-            Maximal number of samples to visualize on the plot. 
-            If the number of samples in the dataset is higher than `nb_samples`, random samples will be selected.
-        labels : bool, default=True
-            If True, plot the mean value and standard deviation for all samples with the same label_id.
-        label_ids : list[int], optional
-            If `labels`, `labels_ids` allows to define for which labels the mean and standard deviation should be plotted.
-            By default all labels are included in the list.
-        ax : matplotlib.axes.Axes, optional
-            Axis on which to plot the samples. By default a new figure with a new axis is generated.
-        show : bool, default = True
-            Automatically call pyplot.show() at the end of the method
-        
-        Returns
-        -------
-        ax : matplotlib.axes.Axes
-            Axis on which the samples were plotted.
-        """
-
-        #TODO: you can not use 'get_wl() for dataset, but you need an x variable to plot against, you can not simply change the axis labels afterwards.'
-        if ax is None:
-            ax = pyplot.subplot(111)
-        if isinstance(self,SpectralDataset):
-            wl = self.get_wl()
-        else:
-            wl = np.arange(self.get_nb_variables())
-        if labels and self._has_labels():
-            for label_id, label_name in self.label_table:
-                if not label_ids or label_id in label_ids:
-                    data = self.get_label_data(label_id)
-                    if data is not None and data.size > 0:
-                        data_mean = np.mean(data, axis=0)
-                        data_std = np.std(data, axis=0)
-                        ax.plot(wl, data_mean, '-', label=label_name)
-                        ax.fill_between(wl, data_mean - data_std, data_mean + data_std, alpha=0.2)
-                        ax.legend()
-        else:
-            if self.get_nb_samples() > nb_samples:
-                rng = np.random.default_rng(2021)
-                sample_indices = rng.choice(self.get_nb_samples(), nb_samples, replace=False)
-                ax.plot(wl, np.transpose(self.get_data()[sample_indices, :]))
-            else:
-                ax.plot(wl, np.transpose(self.get_data()))
-        if show:
-            pyplot.show()
-        return ax
-        
-class SpectralDataset(Dataset):
-    """
-    Class for managing a hyperspectral dataset with N samples and M wavelengths
-    """
-    def __init__(self, data, wavelength, **kwargs):
-        """ Create SpectralDataset using measurment data (N-by-M) with N samples and M wavelengths.
-
-        This method extends the constructor from Dataset.
-        
-        Parameters
-        ----------
-        data : ndarray
-            A 2-D array of shape (N, M) with N the number of samples and M the number of wavelengths.
-        wavelenghts : ndarray
-            A 1-D array of shape (M,) with M the number of wavelenghts.
-        **kwargs: 
-            See Dataset.__init__
-        """
-
-        super().__init__(data, **kwargs)
-        self.set_wl(wavelength)
-    
-    def set_wl(self, wavelength):
-        """ Set the wavelengths to the given `wavelength`.
-        
-        Parameters
-        ----------
-        wavelengths : ndarray
-            A 1-D array of shape (M,) with M the number of wavelengths.
-        """
-        
-        assert (self._are_valid_wavelengths(wavelength))
-        self.wl = deepcopy(wavelength)
-
-    def get_wl(self):
-        """ Get wavelenghts as numpy array.
-        
-        Returns
-        -------
-        wavelengths: ndarray
-            A 1-D array of shape (M,) with M the number of wavelengths.
-        """
-        return np.asarray(self.wl)
-
-    @_docstring_parameter(WL_UNIT)
-    def include_wavelengths(self, start_wl, end_wl):
-        """ Include only the spectral region between `start_wl` and `end_wl`.
-
-        Parameters
-        ----------
-        start_wl: float
-            Start wavelength [{0}]
-        end_wl: float
-            End wavelength [{0}] 
-        """
-        start_idx = self.get_wl_idx(start_wl)
-        end_idx = self.get_wl_idx(end_wl)
-        self._set_data(self.data[:,start_idx:end_idx])
-        self.set_wl(self.get_wl()[start_idx:end_idx])
-
-    @_docstring_parameter(WL_UNIT)
-    def _is_valid_wavelength(self, wavelength):
-        """ Check if a certain `wavelength` is valid for this SpectralDataset with given wavelengths.
-        
-        Parameters
-        ----------
-        wavelength: float
-            Wavelength [{0}] to check
-        
-        See Also
-        --------
-        get_wl: get entire array of wavelengths
-        """
-
-        if self.get_wl() is None:
-            print('No wavelength variables were given to the SpectralDataset. So could not check wavelength of {0}{1}'.format(wavelength, WL_UNIT))
-            return False
-        elif wavelength < min(self.get_wl()):
-            print('Given wavelength ({0}{2}) should be greater then {1}{2}'.format(wavelength, min(self.get_wl()), WL_UNIT))
-            return False
-        elif wavelength > max(self.get_wl()):
-            print('Given wavelength ({0}{2}) should be smaller then {1}{2}'.format(wavelength, max(self.get_wl()), WL_UNIT))
-            return False
-        else:
-            return True
-
-    @_docstring_parameter(WL_UNIT_LONG)
-    def _are_valid_wavelengths(self, wavelengths):
-        """ Check if the given array of wavelenghts `wavelengths` matches the data structure already present. 
-        First assign data before assigning wavelengths.
-
-        Parameters
-        ----------
-        wavelengths: ndarray
-            A 1-D array of shape (M,) with M the number of wavelengths. Wavelengths should be given in {0}.
-        """
-        assert(isinstance(wavelengths, np.ndarray))
-
-        if wavelengths.shape == (self.get_nb_variables(),):
-            return True
-        else:
-            print('Wavelength was shape {0}, while number of variables was {1}'.format(wavelengths.shape, self.get_nb_variables()))
-            return False
-    
-    @_docstring_parameter(WL_UNIT)
-    def get_wl_idx(self, wavelength):
-        """ Get index closes to a certain `wavelength` [{0}].
-
-        Parameters
-        ----------
-        wavelength: float
-            Wavelength [{0}]. Wavelength should be in valid range of given wavelengths.
-
-        Returns
-        -------
-        idx: int
-            Index along the spectral dimensions for which get_wl()[idx] is the closest to `wavelength`.
-        
-        Raises
-        ------
-        ValueError
-            If the given wavelength is outside the wavelength range for this SpectralDataset.
-        """
-
-        if not self._is_valid_wavelength(wavelength):
-            raise ValueError('Invalid wavelength {0}{1}.'.format(wavelength, WL_UNIT))
-
-        diff = (np.abs(self.get_wl() - wavelength))
-
-        idx = diff.argmin()
-        return idx
-
-    def plot(self, nb_spectra=100, labels=True, ax=None, class_ids = [], show=True):
-        """ See Dataset.plot """
-        if ax is None:
-            ax = pyplot.subplot(111)
-        ax.set_xlabel('Wavelength [{0}]'.format(WL_UNIT))
-        ax.set_ylabel('Reflectance [-]')
-        super(SpectralDataset, self).plot(nb_samples=nb_spectra, labels=labels, ax=ax, label_ids=class_ids, show=show)
-
-class HyperSpectralDataset(SpectralDataset):
-    """
-    Class for handeling HyperSpectralDataset objects.
-    """
-
-    def __init__(self, hypercube, wavelength=None, labels=None):
-        """
-        Create a HyperSpectralDataset.
-
-        Parameters
-        ----------
-        hypercube: ndarray
-            A 3-dimensional array with shape (Y,X,L) where Y and X are the spatial dimension and L is the spectral dimension.
-        wavelength: ndarray or list, optional
-            A 1-dimensional list or array with shape (L,). If no wavelengths are provided, the spectral indices are used as wavelengths.
-        labels: ndarray of ints, optional
-            If given, a 1-dimensional array with shape (X*Y,) that contains a label for every spatial position in the X-Y plane.
-        
-        See Also
-        --------
-        SpectralDataset
-        Dataset
-        """
-        
-        dimY, dimX, dimL = hypercube.shape
-
-        self.image_size = (dimY, dimX)
-
-        if wavelength is None:
-            wavelength = range(dimL)
-        
-        #convert wavelength lists to arrays
-        wavelength = np.asarray(wavelength)
-        
-        self.gui = None
-
-        # first try to reshape inplace to save memory footprint
-        try:
-            hypercube.shape = (dimY*dimX, dimL)
-        except AttributeError:
-            hypercube = hypercube.reshape(dimY*dimX, dimL)
-
-        super().__init__(hypercube, wavelength, labels=labels)
-
-    def __getitem__(self, val):
-        """ Index a hyperspectral dataset as if it would be a numpy array.
-        
-        Returns:
-        other: HyperSpectralDataset
-            New hyperspectral dataset with indexed selection
-        """
-
-        #TODO: also allow transfer of labels and included pixels
-        HC = self.get_HC(preprocessed=False).__getitem__(val)
-
-        if isinstance(val, tuple) and len(val)==3:
-            wl = self.get_wl().__getitem__(val[2])
-        else:
-            wl = self.get_wl()
-        
-        return HyperSpectralDataset(hypercube=HC, wavelength=wl)
-    
-    def __truediv__(self, other) -> None:
-        """ Divide this hyperspectral dataset with an other as if they were 3-D numpy arrays."""
-        self._as_numpy_function(other, np.divide)
-    
-    def __sub__(self, other) -> None:
-        """ Substract an other hyperspectral dataset with this one as if they were 3D numpy arrays."""
-        self._as_numpy_function(other, np.subtract)
-
-    def __add__(self, other) -> None:
-        """ Add an other hyperspectral dataset to this one as if they were 3D numpy arrays."""
-        self._as_numpy_function(other, np.add)
-
-    def _as_numpy_function(self, other, np_func)-> None:
-        """ Helper function to apply numpy mathematical operations on the hypercube. Operations happen inplace.
-        
-        Parameters
-        ----------
-        other: HyperSpectralDataset or ndarray
-            Argument required for the `np_func`supplied
-        np_func: numpy method
-            Mathematical method form the numpy library. e.g. np.divide
-        """
-        HC = self.get_HC()
-        if isinstance(other, HyperSpectralDataset):
-            HC = np_func(HC, other.get_HC(), out=HC)
-        elif isinstance(other, np.ndarray):
-            HC = np_func(HC, other, out=HC)
-        else:
-            raise AttributeError(f'{np_func} on HyperSpectralDataset is not possible with {other.type}')
-        self.set_HC(HC)
-
-    def median_filter(self, kernel_size=[3, 3, 3]):
-        HC = self.get_HC()
-        HC = medfilt(HC, kernel_size=kernel_size)
-        self.set_HC(HC)
-
-    @property
-    def shape(self):
-        return (self.get_dimY(), self.get_dimX(), self.get_dimL())
-
-    def get_label_image(self):
-        return self.get_labels(fill=True).reshape((self.get_dimY(), self.get_dimX()))
-
-    def get_band_image(self, band_idx, labeloverlay=False):
-        """
-        Get image of certain band as Y-by-X ndarray.
-
-        If labeloverlay is true and the HyperSpectralDataset has labels assigend, then an fake RGB image is given with labels overlayed.
-        """
-        im = np.squeeze(self.get_HC()[:, :, band_idx])
-        if labeloverlay and self._has_labels():
-            return label2rgb(self.get_label_image(), image=im)
-        else:
-            return im
-
-    def get_band_ratio_image(self, band1_idx, band2_idx):
-        """ Return ratio image of (Band1-Band2)/(Band1+Band2).
-        """
-        im1 = self.get_band_image(band1_idx)
-        im2 = self.get_band_image(band2_idx)
-        return (im1-im2)/(im1+im2)
-
-    @_docstring_parameter(WL_UNIT_LONG)
-    def get_wl_image(self, wavelength):
-        """ Get image at certain wavelength, given in {0}.
-        """
-        assert self._is_valid_wavelength(wavelength)
-        return self.get_band_image(self.get_wl_idx(wavelength))
-
-    def get_wl_ratio_image(self, wavelength1, wavelength2):
-        """ Get ratio image between two wavelengths.
-        
-        Parameters
-        ----------
-        wavelength1: float
-            Wavelength of band 1 [{0}]
-        wavelength2: flaot
-            Wavelength of band 2 [{0}]
-        
-        Returns
-        -------
-        ratio_image: ndarray
-            A 2-dimensional array with shape Y by X.
-        """
-        assert self._is_valid_wavelength(wavelength1) and self._is_valid_wavelength(wavelength2)
-        return self.get_band_ratio_image(self.get_wl_idx(wavelength1), self.get_wl_idx(wavelength2))
-
-    def get_spectrum_at(self, posY, posX):
-        """ Get spectrum at a certain pixel position Y-X
-        """
-        spectrum_idx = np.ravel_multi_index((posY, posX), self.get_image_size())
-        return np.squeeze(self.get_data(preproc=True, fill_nans=True)[spectrum_idx, :])
-
-    def get_HC(self, preprocessed=True):
-        """Get HyperSpectralDataset as ndarray with dimensions dimY-by-dimX-by-dimL.
-        By default preprocessed data are given based on self.preprocess_list.
-        """
-        return self.get_data(preproc=preprocessed, fill_nans=True).reshape((self.get_dimY(), self.get_dimX(), self.get_dimL()))
-
-    def set_HC(self, HC):
-        dimY, dimX, dimL = HC.shape
-
-        self.image_size = (dimY, dimX)
-        self._set_data(HC.reshape(dimY * dimX, dimL))
-
-    def crop(self, mask):
-        assert mask.shape == self.get_image_size()
-        rows, cols = np.where(mask)
-        return self.get_roi(min_row = min(rows),
-                            min_col = min(cols),
-                            max_row = max(rows),
-                            max_col = max(cols))
-
-    def get_roi(self, min_row=0, min_col=0, max_row=-1, max_col=-1):
-        """ Select a Region Of Interest (ROI) for the HyperSpectralDataset. 
-
-        ROI should be defined as a rectangular area defined from a min_row to max_row, and min_col to max_col.
-        TODO: can possible be removed with fancy indexing now with __getitem__
-        """
-        #TODO: make returning copy of self more elegent, maybe use deep copy and change only certain parameters
-        if ((min_row >= 0 and min_col >= 0) and (max_row <= self.get_dimY() and max_col <= self.get_dimX())):
-            roiHSD = deepcopy(self)
-            roiHSD.set_HC(self.get_HC()[round(min_row):round(max_row),round(min_col):round(max_col),:])
-            return roiHSD
-        else:
-            print('ROI does not agree with hypercube dimensions ({0},{1})'.format(self.get_dimY(),self.get_dimX()))
-            return None
-
-    def get_rgb(self, preprocessed=False, labeloverlay=True, raw=False):
-
-        try:
-            red_idx = self.get_wl_idx(570)
-            green_idx = self.get_wl_idx(540)
-            blue_idx = self.get_wl_idx(500)
-        except:
-            red_idx = self.get_wl_idx(1100)
-            green_idx = self.get_wl_idx(1300)
-            blue_idx = self.get_wl_idx(1600)
-
-        reflectance_im = self.get_HC(preprocessed=preprocessed)[:, :, [red_idx, green_idx, blue_idx]]
-
-        #scale raw images to max bit value
-        if raw:
-            #TODO: make valid for all kinds of bit depth images. Mabye store type
-            reflectance_im = reflectance_im/(2**12-1)
-        
-        #convert to 8bit RGB
-        reflectance_im = np.clip(reflectance_im, 0, 1)
-
-        im = np.multiply(reflectance_im, 255).astype(np.uint8)
-        if labeloverlay and self._has_labels():
-            return label2rgb(self.get_label_image(), image=im, bg_label=0)
-        else:
-            return im
-
-    def get_dimY(self):
-        """
-        Get dimension along scanning direction (Y)
-        """
-        return self.get_image_size()[0]
-
-    def get_dimX(self):
-        """
-        Get dimension along spatial direction (X)
-        """
-        return self.get_image_size()[1]
-
-    def get_dimL(self):
-        """
-        Get dimension along spectral direction (L)
-        """
-        return self.get_data().shape[1]
-
-    def get_image_size(self):
-        """ Get spatial image size as Y-by-X.
-        """
-        return self.image_size
-
-    def explore(self):
-        """ Interactive gui for exploring the hypercube.
-        
-        Note
-        ----
-        Explore functionality is not gauranteed to work in an interactive Python environment like Jupyter Notebook. Use `%matplolib qt5` magic to activate Qt5 backend.
-        """
-
-        self.gui = Gui(self)
-        self.gui.update_axes()
-        pyplot.show()
-
-    @classmethod
-    def load(cls, path, **kwargs):
-        """ Load HyperSpectralDataset from file. 
-        
-        File can be either custom hdf5 format or standard remote sensing format like ENVI, Erdas or Aviris.
-
-        Parameters
-        ----------
-        path: str
-            Relative or absolute path to the datafile. For ENVI files, the path to the .hdr file should be given.
-        Y_bin: int (optional)
-            Binning to be applied along Y dimension before loading
-        X_bin: int (optional)
-            Binning to be applied along X dimension before loading
-        L_bin: int (optional)
-            Binning to be applied along L dimension before loading   
-        
-        Returns
-        -------
-        hyperspectraldatset: HyperSpectralDataset
-            Hyperspectral dataset object from file
-        
-        See Also
-        --------
-        _read_from_remote_sensing_format
-        _read_from_hdf5
-        """
-        root, ext = os.path.splitext(path)
-        if ext in ['.hdf5','.h5']:
-            HC, wavelength, labels = HyperSpectralDataset._read_from_hdf5(path, **kwargs)
-        else:
-            HC, wavelength = HyperSpectralDataset._read_from_remote_sensing_format(path, **kwargs)
-            labels = None
-        
-        return cls(HC, wavelength, labels)
-
-    def _read_from_remote_sensing_format(path, Y_bin=1, X_bin=1, L_bin=1):
-        """ Use the `spectral` library to open ENVI (.hdr), Erdas (.lan) or Aviris (.rfl/.spc) files.
-        
-        Parameters
-        ----------
-        path: str
-            Relative or absolute path to the datafile. For ENVI files, the path to the .hdr file should be given.
-        Y_bin: int (optional)
-            Binning to be applied along Y dimension before loading
-        X_bin: int (optional)
-            Binning to be applied along X dimension before loading
-        L_bin: int (optional)
-            Binning to be applied along L dimension before loading   
-        Returns
-        -------
-        HC
-        wl
-        """
-        spyfile = open_image(path)
-        image_array = spyfile[::Y_bin, ::X_bin, ::L_bin]
-        HC = np.asarray(image_array)
-        if spyfile.bands.centers is not None:
-            wl = spyfile.bands.centers
-        else: 
-            wl = np.arange(spyfile.nbands)
-        wl = wl[::L_bin]
-        return HC, wl
-
-    @staticmethod
-    def _read_from_hdf5(path, Y_bin=1, X_bin=1, L_bin=1):
-        """ Read HyperSpectralDataset object from custom hdf5 format.
-        
-        See Also
-        --------
-        save_to_hdf5
-        """
-
-        with h5py.File(path, 'r') as hf:
-            HC = hf['Hypercube'][::Y_bin,::X_bin,::L_bin]
-            wavelength = hf['Wavelengths'][::L_bin]
-            labels = None
-
-            if 'Labels' in hf.keys():
-                # TODO: include label tablelabel_table=hf['Labels'].attrs['Label_table']
-                labels = labels=hf['Labels'][::Y_bin,::X_bin,::L_bin]
-
-        return HC, wavelength, labels
-
-    def save_to_hdf5(self, path, overwrite=False, preprocessed=False):
-        #TODO: allow saving preprocessed
-        #TODO: make more elegant and future proof using dict (cfr vars(object) -> {'HC': numpy.ndarray, ...}
-        if not os.path.isfile(path) or overwrite:
-            with h5py.File(path, 'w') as hf:
-                #TODO also include inclusion
-                self.include_all()
-                hf.create_dataset('Hypercube', data=self.get_HC(preprocessed=preprocessed))
-                hf.create_dataset('Wavelengths', data=self.get_wl())
-                # TODO include preprocessing list. Problem is that preprocessing objects can be not saved to a HDF5 dataset.
-                #  Maybe use String representation for preprocessing or never save preprocessing or save preprocessed data.
-
-                if self.labels is not None:
-                    label_dataset = hf.create_dataset('Labels', data=self.get_labels())
-                    # TODO include label table
-                    #label_dataset.attrs['Label_table'] = np.asarray(self.label_table)
-        else:
-            print('File {0} already exists. Use overwrite=True to overwrite file'.format(path))
-            return
-
-    def _is_valid_reference(self, refHSD) -> bool:
-        """ Check if a dark or white reference is the correct format"""
-        return refHSD.get_dimL() == self.get_dimL()
-
-    def assign_label_image(self, label_image, label_table=None):
-        self.assign_labels(label_image.reshape(self.get_dimY()*self.get_dimX(),), label_table=label_table)
-
-    def draw_mask(self, title='Please draw mask'):
-        """ Helper function for drawing mask on RGB image from hyperspectraldataset."""
-        img = self.get_rgb()
-        fig, ax = pyplot.subplots(1, 1)
-        fig.suptitle(title, fontsize=16)
-        ax.imshow(img)
-
-        mc = MaskCreator(ax)
-        pyplot.show()
-
-        mask = mc.get_mask(self.get_image_size())
-
-        return mask
-
-    def draw_labels(self, label_table)->None:
-        """ Interactive tool to draw labels on an image. 
-        
-        Allows you to draw a polygon area for every label in the label_table. Labels are saved inplace at the end.
-
-        Parameters
-        ----------
-        label_table : list of tuples, optional
-            A list of tuples, where every tuple has the format (label_id, label_name). E.g. label_table = [(1, "good"),(2, "bad")].
-        """
-
-        label_image = np.zeros(self.get_image_size())
-
-        for label_id, label_name in label_table:
-            mask = self.draw_mask('Please select {0}'.format(label_name))
-            label_image[mask] = label_id
-
-        self.assign_label_image(label_image, label_table=label_table)
-
-    def get_included_image(self):
-        """Get binary image for pixels that are included.
-        
-        Returns
-        -------
-        mask: ndarray of booleans
-            A Y-by-X boolean array
-        
-        See Also
-        --------
-        include
-        """
-        return self.included_samples.reshape(self.get_dimY(), self.get_dimX())
-    
-    def include(self, mask):
-        """ Include only the pixels from the mask.
-        
-        See Also
-        --------
-        Dataset.include
-        """
-        assert((mask.shape == self.get_image_size()) or (mask.shape == (np.prod(self.get_image_size()))) )
-        super(HyperSpectralDataset, self).include(np.ravel(mask))
-
-    def rotate(self, angle, center=None, resize=False):
-        """ Return a rotated HyperSpectralDataset. Based on skimage.transform.rotate
-
-        angle: float
-            Rotation angle in degrees in counter-clockwise direction.
-        center: iterable of length 2, optional: Default None
-            The rotation center. If center = None, the hypercube is rotated around its image center, i.e. center = self.get_image_size()/2
-        resize: bool, optional: default False
-            Determine whether the shape of the input image will be automatically calculated, so the complete rotated image exaclty fits.
-        """
-        #TODO also include labels and inclusion in rotation
-        return HyperSpectralDataset(hypercube=transform.rotate(self.get_HC(), angle, center=center, resize=resize),
-                                    wavelength= self.get_wl())
-
-    def __deepcopy__(self, memodict={}):
-        self.gui = None
-        cls = self.__class__  # Extract the class of the object
-        result = cls.__new__(cls)  # Create a new instance of the object based on extracted class
-        memodict[id(self)] = result
-        for k, v in self.__dict__.items():
-            setattr(result, k, deepcopy(v,memodict))  # Copy over attributes by copying directly or in case of complex objects like lists for exaample calling the `__deepcopy()__` method defined by them. Thus recursively copying the whole tree of objects.
-        return result
-
-
+import os
+from tracemalloc import start
+import numpy as np
+import h5py
+from matplotlib import pyplot
+from pytz import NonExistentTimeError
+from skimage.color import label2rgb
+from skimage import transform
+from typing import Optional, Union
+
+from .preprocessing import _Preprocess
+from ._gui import Gui, MaskCreator, PointsCreator
+from .. import WL_UNIT, WL_UNIT_LONG
+from copy import deepcopy
+from spectral import open_image
+from scipy.signal import medfilt
+
+def _docstring_parameter(*sub):
+    def dec(obj):
+        obj.__doc__ = obj.__doc__.format(*sub)
+        return obj
+    return dec
+
+class Dataset(object):
+    """
+    Class for creating a simple dataset with N samples and M variables
+    """
+
+    def __init__(self, data, labels=None, label_table = []):
+        """ Create a Dataset from the N-by-M numpy array with N samples and M variables.
+
+        Parameters
+        ----------
+        data : ndarray
+            A 2-D array of shape (N, M) with N the number of samples and M the number of variables.
+        labels : ndarray, optional
+            A 1-D array of shape (N,) with label ID's for every sample. Label ID's should be integers that can be found in `label_table`.
+            If the integer can not be found in the label_table, or no label table is provided, a default label tabel will be generated.
+        label_table : list of tuples, optional
+            A list of tuples, where every tuple has the format (label_id, label_name). E.g. label_table = [(1, "good"),(2, "bad")].
+        """
+
+        # initialise empty preprocessing list
+        self.preprocess_list = []
+        self.catched_preprocess_list = []
+
+        # initialise data and data_pre
+        # data_pre is a cache for the data that has been preprocessed based on the preprocessing list.
+        self.data = None
+        self.catched_data_preproc = None
+        # initialize data by setting the data to the given data
+        self._set_data(data)
+
+        #assign labels
+        self.labels = labels
+        self.label_table = label_table
+        self._fill_label_table()
+
+    def __array__(self, dtype=None):
+        return self.get_data().copy()
+
+    def __len__(self):
+        return self.get_nb_samples()
+
+    def __repr__(self):
+        return ('A Dataset with size {0}x{1} and preprocessing {2}. {3} samples are included.'.format(self.get_nb_samples(),
+                                                                                                      self.get_nb_variables(),
+                                                                                                      self.preprocess_list,
+                                                                                                      self.get_nb_samples(original=True)))
+
+    @property
+    def shape(self):
+        """ Return the shape (N,M) of the dataset.
+
+        N is the number of samples and M is the number of variables.
+        """
+
+        return (self.get_nb_samples(), self.get_nb_variables)
+
+    def get_nb_samples(self, original=False) -> int:
+        if original:
+            return self.get_original_data().shape[0]
+        else:
+            return self.get_data().shape[0]
+
+    def get_nb_variables(self) -> int:
+        return self.get_data().shape[1]
+
+    def include_only_variables(self, variables_idx):
+        """ Make a selected of which variables to retrain in the dataset."""
+        self.data = self.data[:, variables_idx]
+        self.catched_data_preproc = None
+
+    def include_variables_from(self, start_idx, end_idx):
+        self.data = self.data[:, start_idx:end_idx]
+        self.catched_data_preproc = None
+    ############################# Data Handling #############################
+
+    def _set_data(self, data, included_samples=None, labels=None):
+        """ Set new data. RESTRICTED USE
+
+        This function allows to change data for this dataset.
+        As a result al labels and included samples will be reset or set to the given values.
+        """
+        assert(self._is_valid_data(data))
+        if included_samples is None:
+            self.included_samples = np.ones(data.shape[0], dtype=bool)
+        self.labels = labels
+        self.data = data
+
+        self.catched_data_preproc = None
+
+    @staticmethod
+    def _is_valid_data(data) -> bool:
+        """ Check if the given `data` has the correct format.
+
+        Data should be an numpy ndarray with a shape of the format (N,M).
+        """
+        if isinstance(data, np.ndarray):
+            return len(data.shape) == 2
+        else:
+            return False
+
+    def get_original_data(self):
+        """ Return the original data.
+
+        Original data means the data as intialy provided, without preprocessing and with all samples included.
+        """
+
+        return self.data
+
+    def get_data(self, preproc=True, fill_nans=False) -> np.ndarray:
+        """ Return the data as a numpy array.
+
+        Parameters
+        ----------
+        preproc : bool, default=True
+            If preprocessing is selected (default), the preprocessed data will be returned. Otherwise the raw data will be returned.
+        fill_nans : bool, default=False
+            By default only the included samples are given. If `fill_nans` is set to True however, the returned dataset will have the same shape as the original dataset, with excluded samples having NaN as value for all variables.
+
+        Returns
+        -------
+        data: ndarray
+            2D dimensional array of shape (K,M) where K is the number of included samples. If `fill_nans`, K is the total number of samples.
+
+        See Also
+        --------
+        get_original_data : Return the original data, without preprocessing and with the actual values for the excluded samples.
+        """
+        #check if preprocessed data is asked, and if so, check if catched preprocessing is still valid
+        if preproc and not self._is_valid_catch():
+            self.apply_preprocess()
+        
+        #check if asked to return filled, original or preprocessed data
+        if self.has_excluded_samples() and fill_nans:
+            data = np.full(self.data.shape, np.nan, dtype=self.data.dtype)
+            data[self.included_samples, :] = self.get_data(preproc=preproc, fill_nans=False)
+            return np.squeeze(data)
+        elif (self.catched_data_preproc is not None) and preproc:
+            data = self.catched_data_preproc
+        else:
+            data = self.get_original_data()
+
+        # indexing takes a lot more time so check if this is needed.
+        if self.has_excluded_samples():
+            return np.squeeze(data[self.included_samples, :])
+        else:
+            return data
+
+    ############################# Sample inclusion/exclusion #############################
+
+    def include(self, bool_inclusion):
+        """ Include only part of the samples based on a boolean array of shape (N,).
+
+        Parameters
+        ----------
+        bool_inclusion : ndarray
+            1-D boolean array of shape (N,) where N is the total number of samples.
+            Only samples that were already in the included samples can be included.
+
+        See Also
+        --------
+        include_all
+        """
+
+        self.included_samples = np.logical_and(self.included_samples, bool_inclusion)
+
+    def include_all(self):
+        """ Include all samples that were in the original dataset. Remove any exclusions.
+
+        See Also
+        --------
+        include
+        exclude_label
+        """
+
+        self.included_samples = np.ones(self.data.shape[0], dtype=bool)
+        #TODO: also check all labels are in label table
+
+    def has_excluded_samples(self) -> bool:
+        """ Check if any of the original datasamples has been excluded.
+        """
+
+        return np.any(np.logical_not(self.included_samples))
+
+    def exclude_label(self, label_id: int):
+        """ Exclude all samples with a given `label_id`.
+
+        Parameters
+        ----------
+        label_id : int
+            `label_id` should correspond to one of the labels_id - label_name pairs in the label_table.
+
+        See Also
+        --------
+        _has_label_id : Check if certain `label_id` is in the label_table.
+        """
+
+        if self.labels is not None:
+            if np.any(self.get_labels() == label_id):
+                self.include(self.labels != label_id)
+                if self._has_label_id(label_id=label_id):
+                    self.label_table.remove((label_id, self.get_label_name(label_id)))
+            else:
+                print('WARNING: Not able to exclude label {0} because it was not found in labels'.format(label_id))
+        else:
+            print('WARNING: Not able to exclude label {0} because not labels were found'.format(label_id))
+
+    ############################# Preprocessing #############################
+
+    def apply(func):
+        """ Decorator. Apply preprocessing after method that changes preprocessing list. """
+        def wrapper(self, *args):
+            func(self, *args)
+            self.apply_preprocess()
+
+        return wrapper
+
+    @apply
+    def add_preprocess(self, preprocess: _Preprocess, position=None, allow_double=False) -> None:
+        """ Add a preprocessing step to the preprocessing list.
+
+        This method allows to add a new preprocessing step to the preprocessing list.
+        This list of preprocessing steps will be applied to the data from index 0 to -1.
+
+        Parameters
+        ----------
+        preprocess : _Preprocess
+            Preprocessing object to be added to the preprocessing list.
+        position : int, optional
+            Position at which to add the new `preprocess` within the preprocessing list. If no position is given, the `preprocess` is added at the end of the list (default).
+        allow_double : bool, default=False
+            Normally the same type of preprocessing can not be added twice, unless `allow_double` is set to True.
+        """
+
+        assert(isinstance(preprocess, _Preprocess))
+        if preprocess in self.preprocess_list and not allow_double:
+            print("WARNING: \n New preprocess ({0}) was already in preprocessing list ({1}). \n If this is what you want, use allow_double=True".format(preprocess, self.preprocess_list))
+        else:
+            if position is None:
+                self.preprocess_list.append(preprocess)
+            else:
+                self.preprocess_list.insert(position, preprocess)
+
+    @apply
+    def remove_preprocess(self, position:int) -> None:
+        """ Remove a preprocessing step at a certain `position` from the prepocessing list.
+
+        Parameters
+        ----------
+        position: int
+            Index in preprocessing list.
+
+        See Also 
+        --------
+        print_preprocessing_list()
+        """
+
+        self.preprocess_list.pop(position)
+
+    def has_preprocessing(self) -> bool:
+        """ Check if there are preprocessing steps in the preprocessing list."""
+        return bool(self.preprocess_list)
+
+    @apply
+    def clear_preprocess(self):
+        """ Clear the preprocessing list. No preprocessing will be performed anymore.
+
+        See Also
+        --------
+        get_original_data : directly get the original data on which the preprocessing is being applied.
+        """
+        self.preprocess_list = []
+
+    @apply
+    def copy_preprocess(self, other: 'Dataset'):
+        """ Copy the preprocessing steps from an other Dataset (`other`).
+
+        This method allows to copy the preprocessing that has been performed on an other Dataset `other`, to your dataset.
+        This copying also includes any calibration data from the preprocessing that has been performed on `other` (e.g. mean centering).
+
+        Parameters
+        ---------
+        other: Dataset
+            Dataset from which to copy the list of preprocessing
+
+        Note
+        ----
+        When invocking this method, the new preprocessing list will directly be applied to the dataset. 
+        The original data are stored in parallel and can be accesed using get_original_data() or by using clear_preprocess().
+        """
+
+        assert isinstance(other, Dataset)
+        self.preprocess_list = deepcopy(other.preprocess_list)
+
+    def print_preprocessing_list(self):
+        """Print entire preprocessing list.
+        """
+
+        for idx, preproc in enumerate(self.preprocess_list):
+            print(f'[{idx}] {preproc}')
+
+    def _is_valid_catch(self):
+        """ Check if the catched preprocessing data is still valid (preprocessing not changed since last time applying preprocessing)
+        """
+
+        return self.preprocess_list == self.catched_preprocess_list
+
+    def apply_preprocess(self):
+        """ Apply all preprocessing steps in the preprocessing list, starting from `preprocess_list[0]`.
+
+        Normally these function does not have to be called explicitly, as it is called automaticly after every method that makes changes to the preprocessing list.
+
+        Note
+        ----
+        If the preprocessing list has not changed since the last time this method was invoced, the cached prepropressing data will be used.
+        """
+        if self._is_valid_catch():
+            return self.catched_data_preproc
+        elif self.preprocess_list:
+            self.catched_data_preproc = self.get_original_data().copy()
+            for preproc in self.preprocess_list:
+                self.catched_data_preproc = preproc.apply(self.catched_data_preproc)
+        else:
+            self.catched_data_preproc = None
+        self.catched_preprocess_list = self.preprocess_list
+
+    ############################# Labels #############################
+
+    def get_label_data(self, label_id):
+        """ Get the data belonging to samples with a certain `label_id`.
+
+        If no label data is available for this Dataset, all included samples are included in the returned array.
+
+        Parameters
+        ----------
+        label_id : int
+            The `label_id` should be one from the label_ids listed in the label table.
+
+        Return
+        ------
+        Numpy ndarray of shape (L,M) with L the number of samples for with as label id the given `label_id`.
+        If the `label_id` can not be found in the label table, None will be returned.
+
+        See Also
+        --------
+        get_label_table
+
+        """
+
+        if not self._has_labels():
+            print('No lables were found, returning all data')
+            return self.get_data()
+        else:
+            if self._has_label_id(label_id):
+                class_idx = self.get_labels() == label_id
+                return self.get_data()[class_idx, :]
+            else:
+                print('Label id ({0}) was not found in label table {1}'.format(label_id, str(self.label_table)))
+                return None
+
+    def assign_labels(self, labels, label_table=None):
+        """ Assign labels to the samples in the dataset.
+
+        Parameters
+        ----------
+        labels : ndarray
+            1-D array of shape (N,) with N the number of included samples
+        label_table : list[], optional
+            List of tuples where each tuple corresponds to a lable_id, label_name pair. E.g. label_table = [(0, "good"),(1,"bad")].
+            If no `label_table` is provided, a default label table will be created.
+        """
+        assert(labels.shape == (self.get_nb_samples(),))
+        self.labels = np.full(self.data.shape[0], 0, dtype=int)
+        self.labels[self.included_samples] = np.asarray(labels, dtype=int)
+        if label_table is not None:
+            for label in label_table:
+                label_id, label_name = label
+                self.add_label_id(label_id, label_name)
+        self._fill_label_table()
+
+    def _fill_label_table(self):
+        """ Check if there are any label_ids in the labels that are not in the label_table, and add these label_ids to the label_table with a defautl label_name ('ClassX')
+        """
+        if self._has_labels():
+            for x in np.unique(self.labels):
+                if not self._has_label_id(x):
+                    self.add_label_id(x, "Class_{}".format(x))
+
+    def get_labels(self, fill=False):
+        """ Get the labels belong to the samples of this dataset.
+
+
+        Parameters
+        ----------
+        fill : bool, default=False
+            By default only the labels for the included samples are given.
+            If `fill` is set to True, the excluded samples get -1 as label.
+
+        Returns
+        -------
+        labels: ndarrray or None
+            1-D array with shape (N,) where N is the number of included samples.
+            If `fill_nans` is set to True, N will be the total number of samples.
+            If the `label_id` was not found in the dataset, None will be returned.
+        """
+
+        if self.labels is not None:
+            if fill:
+                labels = np.full(self.labels.shape, -1, dtype=int)
+                labels[self.included_samples] = self.get_labels(fill=False)
+                return np.squeeze(labels).astype(int)
+            else:
+                return np.squeeze(self.labels[self.included_samples]).astype(int)
+        else:
+            return None
+
+    def _has_labels(self):
+        """ Check if labels are available for the samples."""
+        return self.get_labels() is not None
+
+    def _has_label_id(self, label_id):
+        for label_tuple in self.label_table:
+            if label_tuple[0] == label_id:
+                return True
+        return False
+
+    def add_label_id(self, label_id, label_name):
+        """ Add a label with a certain `label_id` and `label_name` to the label_table.
+        
+        Parameters
+        ----------
+        label_id : int
+            Unique id for the label. `label_id` should be different from the other label id's already present in the label_table.
+        label_name : str
+            Name for the label.
+        
+        See Also
+        --------
+        get_label_table
+        get_labels
+        """
+
+        if not self._has_label_id(label_id):
+            self.label_table.append((label_id, label_name))
+        else:
+            print('Label {0} was already in labeltabel with name {1} (instead of given name {2})'.format(label_id, self.get_label_name(label_id), label_name))
+
+    def get_label_name(self, label_id) -> Optional[str]:
+        """ Get the label name beloging to the `label_id`.
+        
+        Parameters
+        ---------
+        label_id : int
+            Label_id as can be found in the labels from this dataset.
+        
+        Returns
+        -------
+        name : str
+            Name for the given `label_id`. If the `label_id` was not found in the label_table, the method will return None.
+        
+        See Also
+        --------
+        get_labels
+        get_label_table
+        """
+
+        for label in self.label_table:
+            id, name = label
+            if label_id == id:
+                return name
+        return None
+
+    def get_nb_classes(self):
+        """ 
+        .. deprecated:: 0.0
+          `get_nb_classes` will be removed. Use get_nb_labels instead.
+        """
+
+        return self.get_nb_labels()
+
+    def get_nb_labels(self):
+        """ Get the total number of unique labels for all"""
+        if self.get_labels() is None:
+            return 0
+        else:
+            return np.unique(self.get_labels()).size
+
+    def get_label_table(self, include_quantity = False):
+        """ Get overview of labels as list of tuples with label tuples as (label_id,label_name) or (label_id,label_name,nb_of_labels) if include_quantity
+        """
+
+        if not include_quantity:
+            return deepcopy(self.label_table)
+        else:
+            label_table = list()
+            for label in self.label_table:
+                label_id, label_name = label
+                label_quantity = sum(self.get_labels()==label_id)
+                label_table.append((label_id, label_name,label_quantity))
+            return label_table
+
+    ############################# Utils #############################
+    def _get_mean_data(self, by_label=True) -> Union[tuple, np.ndarray]:
+        """ Get data mean. If labels are given, the mean for each label will be returned.
+        
+        Parameters
+        ----------
+        by_label : bool, optional
+            Indicate if needed to calculate the mean for each label seperatly. If not, the total mean of the data will be returned.
+        
+        Returns
+        -------
+        mean_data
+            If no labels are given or `by_label` is set to False, a 1-D array will be returned. 
+            Otherwise, a 2-D array will be returned with diffent rows corresponding to the mean of different lables.
+        labels_ids
+            If the mean is calcuted for the different labels, the `labels_ids` corresponding to the different rows are given.
+        """
+        if (self.get_nb_classes() == 0) or not by_label:
+            return np.mean(self.get_data(), axis=0)
+        else:
+            mean_data = np.full([self.get_nb_classes(), self.get_nb_variables()], fill_value=0, dtype=self.get_data().dtype)
+            label_ids = np.full([self.get_nb_classes(),], fill_value=0, dtype=self.get_labels().dtype)
+            i = 0
+            for label_id, labelname in self.get_label_table():
+                mean_data[i, :] = np.mean(self.get_label_data(label_id), axis=0)
+                label_ids[i] = label_id
+                i += 1
+            return mean_data, label_ids
+
+    def add(self, ds) -> None:
+        """ 
+        .. deprecated:: 0.0
+          `add` will be removed. Use merge instead.
+        """
+        print('WARNING: DEPRECATED : Please use merge instead')
+        new_data = np.concatenate((self.get_data(), ds.get_data()), axis=0)
+        if self._has_labels() and ds._has_labels():
+            new_labels = np.concatenate((self.get_labels(), ds.get_labels()), axis=0)
+        else:
+            new_labels = None
+        self._set_data(data=new_data, labels=new_labels)
+
+        #fix missing lables
+        for label_id, label_name in ds.label_table:
+            self.add_label_id(label_id, label_name)
+
+    def merge(self, ds : 'Dataset or SpectralDataset') -> 'Dataset or SpectralDataset':
+        """ Create a new Dataset by merging the current dataset with a new dataset `ds`.
+        
+        Parameters
+        ----------
+        ds : Dataset
+            New dataset to merge with the current dataset.
+        
+        Returns
+        -------
+        ds : Dataset
+            Merged dataset from the current dataset and `ds`.
+        """
+    
+        new_data = np.concatenate((self.get_data(), ds.get_data()), axis=0)
+        if self._has_labels() and ds._has_labels():
+            new_labels = np.concatenate((self.get_labels(), ds.get_labels()), axis=0)
+        else:
+            new_labels = None
+        if isinstance(ds, SpectralDataset):
+            ds = SpectralDataset(data=new_data, wavelength=ds.get_wl(), labels=new_labels, label_table=self.get_label_table())
+        else:
+            ds = Dataset(data=new_data, labels=new_labels, label_table=self.get_label_table())
+
+        #fix missing lables
+        for label_id, label_name in ds.label_table:
+            ds.add_label_id(label_id, label_name)
+        return ds
+
+    def plot(self, nb_samples=100, labels=True, label_ids = [], ax=None, show=True):
+        """ Visualise the dataset by plotting some samples.
+        
+        Parameters
+        ----------
+        nb_samples : int, default=100
+            Maximal number of samples to visualize on the plot. 
+            If the number of samples in the dataset is higher than `nb_samples`, random samples will be selected.
+        labels : bool, default=True
+            If True, plot the mean value and standard deviation for all samples with the same label_id.
+        label_ids : list[int], optional
+            If `labels`, `labels_ids` allows to define for which labels the mean and standard deviation should be plotted.
+            By default all labels are included in the list.
+        ax : matplotlib.axes.Axes, optional
+            Axis on which to plot the samples. By default a new figure with a new axis is generated.
+        show : bool, default = True
+            Automatically call pyplot.show() at the end of the method
+        
+        Returns
+        -------
+        ax : matplotlib.axes.Axes
+            Axis on which the samples were plotted.
+        """
+
+        #TODO: you can not use 'get_wl() for dataset, but you need an x variable to plot against, you can not simply change the axis labels afterwards.'
+        if ax is None:
+            ax = pyplot.subplot(111)
+        if isinstance(self,SpectralDataset):
+            wl = self.get_wl()
+        else:
+            wl = np.arange(self.get_nb_variables())
+        if labels and self._has_labels():
+            for label_id, label_name in self.label_table:
+                if not label_ids or label_id in label_ids:
+                    data = self.get_label_data(label_id)
+                    if data is not None and data.size > 0:
+                        data_mean = np.mean(data, axis=0)
+                        data_std = np.std(data, axis=0)
+                        ax.plot(wl, data_mean, '-', label=label_name)
+                        ax.fill_between(wl, data_mean - data_std, data_mean + data_std, alpha=0.2)
+                        ax.legend()
+        else:
+            if self.get_nb_samples() > nb_samples:
+                rng = np.random.default_rng(2021)
+                sample_indices = rng.choice(self.get_nb_samples(), nb_samples, replace=False)
+                ax.plot(wl, np.transpose(self.get_data()[sample_indices, :]))
+            else:
+                ax.plot(wl, np.transpose(self.get_data()))
+        if show:
+            pyplot.show()
+        return ax
+        
+class SpectralDataset(Dataset):
+    """
+    Class for managing a hyperspectral dataset with N samples and M wavelengths
+    """
+    def __init__(self, data, wavelength, **kwargs):
+        """ Create SpectralDataset using measurment data (N-by-M) with N samples and M wavelengths.
+
+        This method extends the constructor from Dataset.
+        
+        Parameters
+        ----------
+        data : ndarray
+            A 2-D array of shape (N, M) with N the number of samples and M the number of wavelengths.
+        wavelenghts : ndarray
+            A 1-D array of shape (M,) with M the number of wavelenghts.
+        **kwargs: 
+            See Dataset.__init__
+        """
+
+        super().__init__(data, **kwargs)
+        self.set_wl(wavelength)
+    
+    def set_wl(self, wavelength):
+        """ Set the wavelengths to the given `wavelength`.
+        
+        Parameters
+        ----------
+        wavelengths : ndarray
+            A 1-D array of shape (M,) with M the number of wavelengths.
+        """
+        
+        assert (self._are_valid_wavelengths(wavelength))
+        self.wl = deepcopy(wavelength)
+
+    def get_wl(self):
+        """ Get wavelenghts as numpy array.
+        
+        Returns
+        -------
+        wavelengths: ndarray
+            A 1-D array of shape (M,) with M the number of wavelengths.
+        """
+        return np.asarray(self.wl)
+
+    @_docstring_parameter(WL_UNIT)
+    def include_wavelengths(self, start_wl, end_wl):
+        """ Include only the spectral region between `start_wl` and `end_wl`.
+
+        Parameters
+        ----------
+        start_wl: float
+            Start wavelength [{0}]
+        end_wl: float
+            End wavelength [{0}] 
+        """
+        start_idx = self.get_wl_idx(start_wl)
+        end_idx = self.get_wl_idx(end_wl)
+        self._set_data(self.data[:,start_idx:end_idx])
+        self.set_wl(self.get_wl()[start_idx:end_idx])
+
+    @_docstring_parameter(WL_UNIT)
+    def _is_valid_wavelength(self, wavelength):
+        """ Check if a certain `wavelength` is valid for this SpectralDataset with given wavelengths.
+        
+        Parameters
+        ----------
+        wavelength: float
+            Wavelength [{0}] to check
+        
+        See Also
+        --------
+        get_wl: get entire array of wavelengths
+        """
+
+        if self.get_wl() is None:
+            print('No wavelength variables were given to the SpectralDataset. So could not check wavelength of {0}{1}'.format(wavelength, WL_UNIT))
+            return False
+        elif wavelength < min(self.get_wl()):
+            print('Given wavelength ({0}{2}) should be greater then {1}{2}'.format(wavelength, min(self.get_wl()), WL_UNIT))
+            return False
+        elif wavelength > max(self.get_wl()):
+            print('Given wavelength ({0}{2}) should be smaller then {1}{2}'.format(wavelength, max(self.get_wl()), WL_UNIT))
+            return False
+        else:
+            return True
+
+    @_docstring_parameter(WL_UNIT_LONG)
+    def _are_valid_wavelengths(self, wavelengths):
+        """ Check if the given array of wavelenghts `wavelengths` matches the data structure already present. 
+        First assign data before assigning wavelengths.
+
+        Parameters
+        ----------
+        wavelengths: ndarray
+            A 1-D array of shape (M,) with M the number of wavelengths. Wavelengths should be given in {0}.
+        """
+        assert(isinstance(wavelengths, np.ndarray))
+
+        if wavelengths.shape == (self.get_nb_variables(),):
+            return True
+        else:
+            print('Wavelength was shape {0}, while number of variables was {1}'.format(wavelengths.shape, self.get_nb_variables()))
+            return False
+    
+    @_docstring_parameter(WL_UNIT)
+    def get_wl_idx(self, wavelength):
+        """ Get index closes to a certain `wavelength` [{0}].
+
+        Parameters
+        ----------
+        wavelength: float
+            Wavelength [{0}]. Wavelength should be in valid range of given wavelengths.
+
+        Returns
+        -------
+        idx: int
+            Index along the spectral dimensions for which get_wl()[idx] is the closest to `wavelength`.
+        
+        Raises
+        ------
+        ValueError
+            If the given wavelength is outside the wavelength range for this SpectralDataset.
+        """
+
+        if not self._is_valid_wavelength(wavelength):
+            raise ValueError('Invalid wavelength {0}{1}.'.format(wavelength, WL_UNIT))
+
+        diff = (np.abs(self.get_wl() - wavelength))
+
+        idx = diff.argmin()
+        return idx
+
+    def plot(self, nb_spectra=100, labels=True, ax=None, class_ids = [], show=True):
+        """ See Dataset.plot """
+        if ax is None:
+            ax = pyplot.subplot(111)
+        ax.set_xlabel('Wavelength [{0}]'.format(WL_UNIT))
+        ax.set_ylabel('Reflectance [-]')
+        super(SpectralDataset, self).plot(nb_samples=nb_spectra, labels=labels, ax=ax, label_ids=class_ids, show=show)
+
+class HyperSpectralDataset(SpectralDataset):
+    """
+    Class for handeling HyperSpectralDataset objects.
+    """
+
+    def __init__(self, hypercube, wavelength=None, labels=None):
+        """
+        Create a HyperSpectralDataset.
+
+        Parameters
+        ----------
+        hypercube: ndarray
+            A 3-dimensional array with shape (Y,X,L) where Y and X are the spatial dimension and L is the spectral dimension.
+        wavelength: ndarray or list, optional
+            A 1-dimensional list or array with shape (L,). If no wavelengths are provided, the spectral indices are used as wavelengths.
+        labels: ndarray of ints, optional
+            If given, a 1-dimensional array with shape (X*Y,) that contains a label for every spatial position in the X-Y plane.
+        
+        See Also
+        --------
+        SpectralDataset
+        Dataset
+        """
+        
+        dimY, dimX, dimL = hypercube.shape
+
+        self.image_size = (dimY, dimX)
+
+        if wavelength is None:
+            wavelength = range(dimL)
+        
+        #convert wavelength lists to arrays
+        wavelength = np.asarray(wavelength)
+        
+        self.gui = None
+
+        # first try to reshape inplace to save memory footprint
+        try:
+            hypercube.shape = (dimY*dimX, dimL)
+        except AttributeError:
+            hypercube = hypercube.reshape(dimY*dimX, dimL)
+
+        super().__init__(hypercube, wavelength, labels=labels)
+
+    def __getitem__(self, val):
+        """ Index a hyperspectral dataset as if it would be a numpy array.
+        
+        Returns:
+        other: HyperSpectralDataset
+            New hyperspectral dataset with indexed selection
+        """
+
+        #TODO: also allow transfer of labels and included pixels
+        HC = self.get_HC(preprocessed=False).__getitem__(val)
+
+        if isinstance(val, tuple) and len(val)==3:
+            wl = self.get_wl().__getitem__(val[2])
+        else:
+            wl = self.get_wl()
+        
+        return HyperSpectralDataset(hypercube=HC, wavelength=wl)
+    
+    def __truediv__(self, other) -> None:
+        """ Divide this hyperspectral dataset with an other as if they were 3-D numpy arrays."""
+        self._as_numpy_function(other, np.divide)
+    
+    def __sub__(self, other) -> None:
+        """ Substract an other hyperspectral dataset with this one as if they were 3D numpy arrays."""
+        self._as_numpy_function(other, np.subtract)
+
+    def __add__(self, other) -> None:
+        """ Add an other hyperspectral dataset to this one as if they were 3D numpy arrays."""
+        self._as_numpy_function(other, np.add)
+
+    def _as_numpy_function(self, other, np_func)-> None:
+        """ Helper function to apply numpy mathematical operations on the hypercube. Operations happen inplace.
+        
+        Parameters
+        ----------
+        other: HyperSpectralDataset or ndarray
+            Argument required for the `np_func`supplied
+        np_func: numpy method
+            Mathematical method form the numpy library. e.g. np.divide
+        """
+        HC = self.get_HC()
+        if isinstance(other, HyperSpectralDataset):
+            HC = np_func(HC, other.get_HC(), out=HC)
+        elif isinstance(other, np.ndarray):
+            HC = np_func(HC, other, out=HC)
+        else:
+            raise AttributeError(f'{np_func} on HyperSpectralDataset is not possible with {other.type}')
+        self.set_HC(HC)
+
+    def median_filter(self, kernel_size=[3, 3, 3]):
+        HC = self.get_HC()
+        HC = medfilt(HC, kernel_size=kernel_size)
+        self.set_HC(HC)
+
+    @property
+    def shape(self):
+        return (self.get_dimY(), self.get_dimX(), self.get_dimL())
+
+    def get_label_image(self):
+        return self.get_labels(fill=True).reshape((self.get_dimY(), self.get_dimX()))
+
+    def get_band_image(self, band_idx, labeloverlay=False):
+        """
+        Get image of certain band as Y-by-X ndarray.
+
+        If labeloverlay is true and the HyperSpectralDataset has labels assigend, then an fake RGB image is given with labels overlayed.
+        """
+        im = np.squeeze(self.get_HC()[:, :, band_idx])
+        if labeloverlay and self._has_labels():
+            return label2rgb(self.get_label_image(), image=im)
+        else:
+            return im
+
+    def get_band_ratio_image(self, band1_idx, band2_idx):
+        """ Return ratio image of (Band1-Band2)/(Band1+Band2).
+        """
+        im1 = self.get_band_image(band1_idx)
+        im2 = self.get_band_image(band2_idx)
+        return (im1-im2)/(im1+im2)
+
+    @_docstring_parameter(WL_UNIT_LONG)
+    def get_wl_image(self, wavelength):
+        """ Get image at certain wavelength, given in {0}.
+        """
+        assert self._is_valid_wavelength(wavelength)
+        return self.get_band_image(self.get_wl_idx(wavelength))
+
+    def get_wl_ratio_image(self, wavelength1, wavelength2):
+        """ Get ratio image between two wavelengths.
+        
+        Parameters
+        ----------
+        wavelength1: float
+            Wavelength of band 1 [{0}]
+        wavelength2: flaot
+            Wavelength of band 2 [{0}]
+        
+        Returns
+        -------
+        ratio_image: ndarray
+            A 2-dimensional array with shape Y by X.
+        """
+        assert self._is_valid_wavelength(wavelength1) and self._is_valid_wavelength(wavelength2)
+        return self.get_band_ratio_image(self.get_wl_idx(wavelength1), self.get_wl_idx(wavelength2))
+
+    def get_spectrum_at(self, posY, posX):
+        """ Get spectrum at a certain pixel position Y-X
+        """
+        spectrum_idx = np.ravel_multi_index((posY, posX), self.get_image_size())
+        return np.squeeze(self.get_data(preproc=True, fill_nans=True)[spectrum_idx, :])
+
+    def get_HC(self, preprocessed=True):
+        """Get HyperSpectralDataset as ndarray with dimensions dimY-by-dimX-by-dimL.
+        By default preprocessed data are given based on self.preprocess_list.
+        """
+        return self.get_data(preproc=preprocessed, fill_nans=True).reshape((self.get_dimY(), self.get_dimX(), self.get_dimL()))
+
+    def set_HC(self, HC):
+        dimY, dimX, dimL = HC.shape
+
+        self.image_size = (dimY, dimX)
+        self._set_data(HC.reshape(dimY * dimX, dimL))
+
+    def crop(self, mask):
+        assert mask.shape == self.get_image_size()
+        rows, cols = np.where(mask)
+        return self.get_roi(min_row = min(rows),
+                            min_col = min(cols),
+                            max_row = max(rows),
+                            max_col = max(cols))
+
+    def get_roi(self, min_row=0, min_col=0, max_row=-1, max_col=-1):
+        """ Select a Region Of Interest (ROI) for the HyperSpectralDataset. 
+
+        ROI should be defined as a rectangular area defined from a min_row to max_row, and min_col to max_col.
+        TODO: can possible be removed with fancy indexing now with __getitem__
+        """
+        #TODO: make returning copy of self more elegent, maybe use deep copy and change only certain parameters
+        if ((min_row >= 0 and min_col >= 0) and (max_row <= self.get_dimY() and max_col <= self.get_dimX())):
+            roiHSD = deepcopy(self)
+            roiHSD.set_HC(self.get_HC()[round(min_row):round(max_row),round(min_col):round(max_col),:])
+            return roiHSD
+        else:
+            print('ROI does not agree with hypercube dimensions ({0},{1})'.format(self.get_dimY(),self.get_dimX()))
+            return None
+
+    def get_rgb(self, preprocessed=False, labeloverlay=True, raw=False, channels=[]):
+        
+        if not channels:
+            try:
+                red_idx = self.get_wl_idx(570)
+                green_idx = self.get_wl_idx(540)
+                blue_idx = self.get_wl_idx(500)
+            except:
+                red_idx = self.get_wl_idx(1100)
+                green_idx = self.get_wl_idx(1300)
+                blue_idx = self.get_wl_idx(1600)
+        else:
+            red_idx, green_idx, blue_idx = [self.get_wl_idx(wl) for wl in channels]
+
+        reflectance_im = self.get_HC(preprocessed=preprocessed)[:, :, [red_idx, green_idx, blue_idx]]
+
+        #scale raw images to max bit value
+        if raw:
+            #TODO: make valid for all kinds of bit depth images. Mabye store type
+            reflectance_im = reflectance_im/(2**12-1)
+        
+        #convert to 8bit RGB
+        reflectance_im = np.clip(reflectance_im, 0, 1)
+
+        im = np.multiply(reflectance_im, 255).astype(np.uint8)
+        if labeloverlay and self._has_labels():
+            return label2rgb(self.get_label_image(), image=im, bg_label=0)
+        else:
+            return im
+
+    def get_dimY(self):
+        """
+        Get dimension along scanning direction (Y)
+        """
+        return self.get_image_size()[0]
+
+    def get_dimX(self):
+        """
+        Get dimension along spatial direction (X)
+        """
+        return self.get_image_size()[1]
+
+    def get_dimL(self):
+        """
+        Get dimension along spectral direction (L)
+        """
+        return self.get_data().shape[1]
+
+    def get_image_size(self):
+        """ Get spatial image size as Y-by-X.
+        """
+        return self.image_size
+
+    def explore(self):
+        """ Interactive gui for exploring the hypercube.
+        
+        Note
+        ----
+        Explore functionality is not gauranteed to work in an interactive Python environment like Jupyter Notebook. Use `%matplolib qt5` magic to activate Qt5 backend.
+        """
+
+        self.gui = Gui(self)
+        self.gui.update_axes()
+        pyplot.show()
+
+    @classmethod
+    def load(cls, path, **kwargs):
+        """ Load HyperSpectralDataset from file. 
+        
+        File can be either custom hdf5 format or standard remote sensing format like ENVI, Erdas or Aviris.
+
+        Parameters
+        ----------
+        path: str
+            Relative or absolute path to the datafile. For ENVI files, the path to the .hdr file should be given.
+        Y_bin: int (optional)
+            Binning to be applied along Y dimension before loading
+        X_bin: int (optional)
+            Binning to be applied along X dimension before loading
+        L_bin: int (optional)
+            Binning to be applied along L dimension before loading   
+        
+        Returns
+        -------
+        hyperspectraldatset: HyperSpectralDataset
+            Hyperspectral dataset object from file
+        
+        See Also
+        --------
+        _read_from_remote_sensing_format
+        _read_from_hdf5
+        """
+        root, ext = os.path.splitext(path)
+        if ext in ['.hdf5','.h5']:
+            HC, wavelength, labels = HyperSpectralDataset._read_from_hdf5(path, **kwargs)
+        else:
+            HC, wavelength = HyperSpectralDataset._read_from_remote_sensing_format(path, **kwargs)
+            labels = None
+        
+        return cls(HC, wavelength, labels)
+
+    def _read_from_remote_sensing_format(path, Y_bin=1, X_bin=1, L_bin=1):
+        """ Use the `spectral` library to open ENVI (.hdr), Erdas (.lan) or Aviris (.rfl/.spc) files.
+        
+        Parameters
+        ----------
+        path: str
+            Relative or absolute path to the datafile. For ENVI files, the path to the .hdr file should be given.
+        Y_bin: int (optional)
+            Binning to be applied along Y dimension before loading
+        X_bin: int (optional)
+            Binning to be applied along X dimension before loading
+        L_bin: int (optional)
+            Binning to be applied along L dimension before loading   
+        Returns
+        -------
+        HC
+        wl
+        """
+        spyfile = open_image(path)
+        image_array = spyfile[::Y_bin, ::X_bin, ::L_bin]
+        HC = np.asarray(image_array)
+        if spyfile.bands.centers is not None:
+            wl = spyfile.bands.centers
+        else: 
+            wl = np.arange(spyfile.nbands)
+        wl = wl[::L_bin]
+        return HC, wl
+
+    @staticmethod
+    def _read_from_hdf5(path, Y_bin=1, X_bin=1, L_bin=1):
+        """ Read HyperSpectralDataset object from custom hdf5 format.
+        
+        See Also
+        --------
+        save_to_hdf5
+        """
+
+        with h5py.File(path, 'r') as hf:
+            if Y_bin != 1 or X_bin != 1 or L_bin!=1:
+                HC = hf['Hypercube'][::Y_bin,::X_bin,::L_bin]
+            else:
+                HC = hf['Hypercube'][:]
+            wavelength = hf['Wavelengths'][::L_bin]
+            labels = None
+
+            if 'Labels' in hf.keys():
+                # TODO: include label tablelabel_table=hf['Labels'].attrs['Label_table']
+                labels = labels=hf['Labels'][::Y_bin,::X_bin,::L_bin]
+
+        return HC, wavelength, labels
+
+    def save_to_hdf5(self, path, overwrite=False, preprocessed=False):
+        #TODO: allow saving preprocessed
+        #TODO: make more elegant and future proof using dict (cfr vars(object) -> {'HC': numpy.ndarray, ...}
+        if not os.path.isfile(path) or overwrite:
+            with h5py.File(path, 'w') as hf:
+                #TODO also include inclusion
+                self.include_all()
+                hf.create_dataset('Hypercube', data=self.get_HC(preprocessed=preprocessed))
+                hf.create_dataset('Wavelengths', data=self.get_wl())
+                # TODO include preprocessing list. Problem is that preprocessing objects can be not saved to a HDF5 dataset.
+                #  Maybe use String representation for preprocessing or never save preprocessing or save preprocessed data.
+
+                if self.labels is not None:
+                    label_dataset = hf.create_dataset('Labels', data=self.get_labels())
+                    # TODO include label table
+                    #label_dataset.attrs['Label_table'] = np.asarray(self.label_table)
+        else:
+            print('File {0} already exists. Use overwrite=True to overwrite file'.format(path))
+            return
+
+    def _is_valid_reference(self, refHSD) -> bool:
+        """ Check if a dark or white reference is the correct format"""
+        return refHSD.get_dimL() == self.get_dimL()
+
+    def assign_label_image(self, label_image, label_table=None):
+        self.assign_labels(label_image.reshape(self.get_dimY()*self.get_dimX(),), label_table=label_table)
+
+    def draw_mask(self, title='Please draw mask. Close figure when ready', tool='points'):
+        """ Helper function for drawing mask on RGB image from hyperspectraldataset."""
+        img = self.get_rgb()
+        fig, ax = pyplot.subplots(1, 1)
+        fig.suptitle(title, fontsize=16)
+        ax.imshow(img)
+
+        if tool == 'points':
+            mc = PointsCreator(ax)
+        else:
+            mc = MaskCreator(ax, selector=tool)
+
+        pyplot.show() #wait for figure to close to get mask 
+
+        mask = mc.get_mask(self.get_image_size())
+
+        return mask
+
+    def draw_labels(self, label_table, tool='points')->None:
+        """ Interactive tool to draw labels on an image. 
+        
+        Allows you to draw a polygon area for every label in the label_table. Labels are saved inplace at the end.
+
+        Parameters
+        ----------
+        label_table : list of tuples, optional
+            A list of tuples, where every tuple has the format (label_id, label_name). E.g. label_table = [(1, "good"),(2, "bad")].
+        tool: str, option
+            Select a tool to use, this can be either 'points' (default), 'polygon' or 'lasso'
+        """
+
+        label_image = np.zeros(self.get_image_size())
+
+        for label_id, label_name in label_table:
+            mask = self.draw_mask('Please select {0}. Close figure when ready.'.format(label_name), tool=tool)
+            label_image[mask] = label_id
+
+        self.assign_label_image(label_image, label_table=label_table)
+
+    def get_included_image(self):
+        """Get binary image for pixels that are included.
+        
+        Returns
+        -------
+        mask: ndarray of booleans
+            A Y-by-X boolean array
+        
+        See Also
+        --------
+        include
+        """
+        return self.included_samples.reshape(self.get_dimY(), self.get_dimX())
+    
+    def include(self, mask):
+        """ Include only the pixels from the mask.
+        
+        See Also
+        --------
+        Dataset.include
+        """
+        assert((mask.shape == self.get_image_size()) or (mask.shape == (np.prod(self.get_image_size()))) )
+        super(HyperSpectralDataset, self).include(np.ravel(mask))
+
+    def rotate(self, angle, center=None, resize=False):
+        """ Return a rotated HyperSpectralDataset. Based on skimage.transform.rotate
+
+        angle: float
+            Rotation angle in degrees in counter-clockwise direction.
+        center: iterable of length 2, optional: Default None
+            The rotation center. If center = None, the hypercube is rotated around its image center, i.e. center = self.get_image_size()/2
+        resize: bool, optional: default False
+            Determine whether the shape of the input image will be automatically calculated, so the complete rotated image exaclty fits.
+        """
+        #TODO also include labels and inclusion in rotation
+        return HyperSpectralDataset(hypercube=transform.rotate(self.get_HC(), angle, center=center, resize=resize),
+                                    wavelength= self.get_wl())
+
+    def __deepcopy__(self, memodict={}):
+        self.gui = None
+        cls = self.__class__  # Extract the class of the object
+        result = cls.__new__(cls)  # Create a new instance of the object based on extracted class
+        memodict[id(self)] = result
+        for k, v in self.__dict__.items():
+            setattr(result, k, deepcopy(v,memodict))  # Copy over attributes by copying directly or in case of complex objects like lists for exaample calling the `__deepcopy()__` method defined by them. Thus recursively copying the whole tree of objects.
+        return result
+
+
```

## phyper/chemometrics/preprocessing.py

 * *Ordering differences only*

```diff
@@ -1,100 +1,100 @@
-from abc import ABC, abstractmethod
-import numpy as np
-import scipy.signal as sp_signal
-
-class _Preprocess(ABC):
-    def __init__(self):
-        self.calibration_data = None
-    
-    def is_calibrated(self):
-        return self.calibration_data is None
-
-    @abstractmethod
-    def apply(self, data):
-        return data
-
-    @abstractmethod
-    def __str__(self):
-        return 'Default preprocessing'
-
-    def calibrate(self, data):
-        pass
-
-    def __repr__(self):
-        return str(self)
-
-    def __eq__(self, other):
-        #combare preprocessings based on their discription string
-        return str(self) == str(other)
-
-class MeanCenter(_Preprocess):
-
-    def __init__(self):
-        super().__init__()
-        self.mean = None
-        
-
-    def apply(self, data):
-        if self.mean is None:
-            self.calibrate(data)
-        return data - self.mean
-
-    def calibrate(self, data):
-        self.calibration_data = data
-        self.mean = np.mean(data, axis=0)
-    
-    def __str__(self):
-        return f'Mean Center with mean {self.mean}'
-    
-class Normalize(_Preprocess):
-    
-    def apply(self, data):
-        return np.divide(data.transpose(), np.sum(data, axis=1)).transpose()
-
-    def __str__(self):
-        return 'Normalize (Area 1)'
-    
-class SavGol(_Preprocess):
-
-    def __init__(self, window_width = 15, polynomial_order = 2, derivative = 1 ):
-        super().__init__()
-        self.window_length = window_width
-        self.polynomial_order = polynomial_order
-        self.derivative = derivative
-
-    def apply(self, data):
-        return  sp_signal.savgol_filter(data, window_length = self.window_length, polyorder = self.polynomial_order, deriv = self.derivative)
-
-    def __str__(self):
-
-        if self.derivative == 0:
-            derivative_str = 'SavGol smoothing'
-        elif self.derivative == 1: 
-            derivative_str = 'SavGol first derivate'
-        elif self.derivative == 2:
-            derivative_str = 'SavGol second derivative'
-        else:
-            derivative_str = 'SavGol {0}\'th'.format(self.derivative)
-
-        return derivative_str + ' with window width {0} and polynomial order {1}'.format(self.window_length,self.polynomial_order)
-
-class SNV(_Preprocess):
-
-    def apply(self, data): 
-        x_t = data.T
-        return ((x_t - x_t.mean(axis=0))/x_t.std(axis=0)).T
-    
-    def __str__(self):
-        return 'Standard Normal Variate (SNV)'
-
-class Binning(_Preprocess):
-    """ Simple binning class""" 
-    def __init__(self,binning=2):
-        super().__init__()
-        self.binning=binning
-
-    def apply(self,data):
-        return data[:,::self.binning] 
-
-    def __str__(self):
+from abc import ABC, abstractmethod
+import numpy as np
+import scipy.signal as sp_signal
+
+class _Preprocess(ABC):
+    def __init__(self):
+        self.calibration_data = None
+    
+    def is_calibrated(self):
+        return self.calibration_data is None
+
+    @abstractmethod
+    def apply(self, data):
+        return data
+
+    @abstractmethod
+    def __str__(self):
+        return 'Default preprocessing'
+
+    def calibrate(self, data):
+        pass
+
+    def __repr__(self):
+        return str(self)
+
+    def __eq__(self, other):
+        #combare preprocessings based on their discription string
+        return str(self) == str(other)
+
+class MeanCenter(_Preprocess):
+
+    def __init__(self):
+        super().__init__()
+        self.mean = None
+        
+
+    def apply(self, data):
+        if self.mean is None:
+            self.calibrate(data)
+        return data - self.mean
+
+    def calibrate(self, data):
+        self.calibration_data = data
+        self.mean = np.mean(data, axis=0)
+    
+    def __str__(self):
+        return f'Mean Center with mean {self.mean}'
+    
+class Normalize(_Preprocess):
+    
+    def apply(self, data):
+        return np.divide(data.transpose(), np.sum(data, axis=1)).transpose()
+
+    def __str__(self):
+        return 'Normalize (Area 1)'
+    
+class SavGol(_Preprocess):
+
+    def __init__(self, window_width = 15, polynomial_order = 2, derivative = 1 ):
+        super().__init__()
+        self.window_length = window_width
+        self.polynomial_order = polynomial_order
+        self.derivative = derivative
+
+    def apply(self, data):
+        return  sp_signal.savgol_filter(data, window_length = self.window_length, polyorder = self.polynomial_order, deriv = self.derivative)
+
+    def __str__(self):
+
+        if self.derivative == 0:
+            derivative_str = 'SavGol smoothing'
+        elif self.derivative == 1: 
+            derivative_str = 'SavGol first derivate'
+        elif self.derivative == 2:
+            derivative_str = 'SavGol second derivative'
+        else:
+            derivative_str = 'SavGol {0}\'th'.format(self.derivative)
+
+        return derivative_str + ' with window width {0} and polynomial order {1}'.format(self.window_length,self.polynomial_order)
+
+class SNV(_Preprocess):
+
+    def apply(self, data): 
+        x_t = data.T
+        return ((x_t - x_t.mean(axis=0))/x_t.std(axis=0)).T
+    
+    def __str__(self):
+        return 'Standard Normal Variate (SNV)'
+
+class Binning(_Preprocess):
+    """ Simple binning class""" 
+    def __init__(self,binning=2):
+        super().__init__()
+        self.binning=binning
+
+    def apply(self,data):
+        return data[:,::self.binning] 
+
+    def __str__(self):
         return f'Binning with bin {self.binning}'
```

## phyper/chemometrics/sampling.py

 * *Ordering differences only*

```diff
@@ -1,69 +1,69 @@
-from .dataset import Dataset
-import numpy as np
-
-def sample_by_class(ds: Dataset, nb_samples_per_class, seed=2021):
-    #set fixed seed for rng
-    rng = np.random.default_rng(seed=seed)
-
-    all_labels = ds.get_labels(fill=True)
-
-    boolean_samples = np.zeros(ds.included_samples.size, dtype=bool)
-
-    #iterate over labels in dataset
-    for label_id, label in ds.get_label_table():
-
-        label_bools = all_labels == label_id
-
-        nb_label_samples = label_bools.sum()
-
-        if nb_label_samples > nb_samples_per_class:
-            t_mask = np.zeros(nb_label_samples, dtype=bool)
-            t_mask[rng.choice(nb_label_samples, nb_samples_per_class, replace=False)] = True
-            label_bools[label_bools] = t_mask
-
-        boolean_samples[label_bools] = True
-
-    ds.included_samples = boolean_samples
-
-    return ds
-
-def sample_from_list(dataset_list, nb_samples_per_dataset=None, total_nb_samples=None):
-    merged_dataset = None
-
-    number_of_samples = [ds.get_nb_samples() for ds in dataset_list]
-    max_nb_samples = sum(number_of_samples)
-
-    if total_nb_samples is None:
-        total_nb_samples = max_nb_samples
-    if total_nb_samples > max_nb_samples:
-        print('WARNING: requested total number of samples ({0}) was greather then sum of all samples in dataset list ({1}).'
-              ' \n Returning combination of all dataset.'.format(total_nb_samples, max_nb_samples))
-
-    for ds in dataset_list:
-        if nb_samples_per_dataset is None:
-            percentage = total_nb_samples/max_nb_samples
-            nb_samples_per_dataset = np.floor(dataset.get_nb_samples()*percentage)
-        sample_random(ds, nb_samples_per_dataset)
-        if merged_dataset is None:
-            merged_dataset = ds
-        else:
-            merged_dataset.add(ds)
-
-    return merged_dataset
-
-def sample_random(dataset, nb_points, seed=2021):
-    assert dataset.included_samples.dtype == np.bool
-
-    # set fixed seed for rng
-    rng = np.random.default_rng(seed=seed)
-
-    incluced_bool = dataset.included_samples
-    nb_included = np.sum(incluced_bool)
-
-    t_mask = np.zeros(nb_included, dtype=bool)
-    t_mask[rng.choice(nb_included, nb_points, replace=False)] = True
-    incluced_bool[incluced_bool] = t_mask
-
-    dataset.included_samples = incluced_bool
-
-    return dataset
+from .dataset import Dataset
+import numpy as np
+
+def sample_by_class(ds: Dataset, nb_samples_per_class, seed=2021):
+    #set fixed seed for rng
+    rng = np.random.default_rng(seed=seed)
+
+    all_labels = ds.get_labels(fill=True)
+
+    boolean_samples = np.zeros(ds.included_samples.size, dtype=bool)
+
+    #iterate over labels in dataset
+    for label_id, label in ds.get_label_table():
+
+        label_bools = all_labels == label_id
+
+        nb_label_samples = label_bools.sum()
+
+        if nb_label_samples > nb_samples_per_class:
+            t_mask = np.zeros(nb_label_samples, dtype=bool)
+            t_mask[rng.choice(nb_label_samples, nb_samples_per_class, replace=False)] = True
+            label_bools[label_bools] = t_mask
+
+        boolean_samples[label_bools] = True
+
+    ds.included_samples = boolean_samples
+
+    return ds
+
+def sample_from_list(dataset_list, nb_samples_per_dataset=None, total_nb_samples=None):
+    merged_dataset = None
+
+    number_of_samples = [ds.get_nb_samples() for ds in dataset_list]
+    max_nb_samples = sum(number_of_samples)
+
+    if total_nb_samples is None:
+        total_nb_samples = max_nb_samples
+    if total_nb_samples > max_nb_samples:
+        print('WARNING: requested total number of samples ({0}) was greather then sum of all samples in dataset list ({1}).'
+              ' \n Returning combination of all dataset.'.format(total_nb_samples, max_nb_samples))
+
+    for ds in dataset_list:
+        if nb_samples_per_dataset is None:
+            percentage = total_nb_samples/max_nb_samples
+            nb_samples_per_dataset = np.floor(dataset.get_nb_samples()*percentage)
+        sample_random(ds, nb_samples_per_dataset)
+        if merged_dataset is None:
+            merged_dataset = ds
+        else:
+            merged_dataset.add(ds)
+
+    return merged_dataset
+
+def sample_random(dataset, nb_points, seed=2021):
+    assert dataset.included_samples.dtype == np.bool
+
+    # set fixed seed for rng
+    rng = np.random.default_rng(seed=seed)
+
+    incluced_bool = dataset.included_samples
+    nb_included = np.sum(incluced_bool)
+
+    t_mask = np.zeros(nb_included, dtype=bool)
+    t_mask[rng.choice(nb_included, nb_points, replace=False)] = True
+    incluced_bool[incluced_bool] = t_mask
+
+    dataset.included_samples = incluced_bool
+
+    return dataset
```

## phyper/lab/__init__.py

 * *Ordering differences only*

```diff
@@ -1,5 +1,5 @@
-""" Lab package from Pyper toolbox
-
-Helper package for managing measurements performed with lab equipment at MeBioS.
-
+""" Lab package from Pyper toolbox
+
+Helper package for managing measurements performed with lab equipment at MeBioS.
+
 """
```

## phyper/lab/_misc.py

 * *Ordering differences only*

```diff
@@ -1,36 +1,36 @@
-#misc functions 
-import re
-import cv2
-import png
-import numpy as np
-import os
-
-import tifffile
-
-
-def atoi(text):
-    return int(text) if text.isdigit() else text
-
-def natural_keys(text):
-    return [ atoi(c) for c in re.split(r'(\d+)', text) ]
-
-def read_png(path):
-    #read image using openCV
-    im = cv2.imread(path, cv2.IMREAD_ANYDEPTH)
-
-    #check image metadata using png reader
-    meta = png.Reader(path)
-    meta.preamble()
-    significant_bits = ord(meta.sbit)
-    
-    im = np.right_shift(im,16-significant_bits)
-    return im
-
-def imread(path):
-    _, file_extension = os.path.splitext(path)
-    if file_extension == '.png':
-        return read_png(path)
-    elif file_extension == '.tiff':
-        return tifffile.imread(path)
-    else:
+#misc functions 
+import re
+import cv2
+import png
+import numpy as np
+import os
+
+import tifffile
+
+
+def atoi(text):
+    return int(text) if text.isdigit() else text
+
+def natural_keys(text):
+    return [ atoi(c) for c in re.split(r'(\d+)', text) ]
+
+def read_png(path):
+    #read image using openCV
+    im = cv2.imread(path, cv2.IMREAD_ANYDEPTH)
+
+    #check image metadata using png reader
+    meta = png.Reader(path)
+    meta.preamble()
+    significant_bits = ord(meta.sbit)
+    
+    im = np.right_shift(im,16-significant_bits)
+    return im
+
+def imread(path):
+    _, file_extension = os.path.splitext(path)
+    if file_extension == '.png':
+        return read_png(path)
+    elif file_extension == '.tiff':
+        return tifffile.imread(path)
+    else:
         return cv2.imread(path, cv2.IMREAD_ANYDEPTH)
```

## phyper/lab/measurement.py

 * *Ordering differences only*

```diff
@@ -1,400 +1,400 @@
-import glob
-import enum
-from tkinter import Tk, filedialog
-import os
-import numpy as np
-import re
-from matplotlib import pyplot
-from copy import deepcopy
-from datetime import datetime
-from tqdm import tqdm
-from xml.etree import ElementTree as ET
-
-from ._misc import natural_keys
-from . import _misc
-from ..chemometrics.dataset import Dataset, SpectralDataset, HyperSpectralDataset
-
-IMAGE_EXT = ['.tiff','.tif','.png']
-
-def build_HC_from_folder(folder_dir=None, Y_start=0, Y_end=-1, Y_bin = 1, X_bin = 1, L_bin = 1, silent=False, dtype=np.float32) -> np.ndarray :
-    """
-    Build HyperSpectralDataset from folder containing png images
-    """
-    if folder_dir is None:
-        Tk().withdraw()
-        folder_dir = filedialog.askdirectory(title="Please select folder containing the linescan images")
-    
-    all_file_names = os.listdir(folder_dir)
-    file_names = list()
-    parameter_dict = dict()
-    for file_name in all_file_names:
-        [name,ext] = os.path.splitext(file_name)
-        if ext in IMAGE_EXT:
-            file_names.append(file_name)
-        elif ext == '.xml':
-            parameter_dict.update(read_xml_to_dict(os.path.join(folder_dir,file_name)))
-        else:
-            Warning("file: {0} was not included in HyperSpectralDataset because of invalid extention {1}".format(file_name,ext))
-    
-    file_names.sort(key=_misc.natural_keys)
-
-    dimY = len(file_names)
-    [dimL, dimX] = _misc.imread(os.path.join(folder_dir, file_names[0]))[::L_bin, ::X_bin].shape
-
-    if Y_end == -1:
-                Y_end = dimY
-
-    HC = np.empty([len(range(Y_start, Y_end, Y_bin)), dimX, dimL], dtype=dtype)
-    j = 0
-    parameter_dict['Time'] = datetime.fromtimestamp(os.path.getmtime(os.path.join(folder_dir, file_names[Y_start])))
-    for i in tqdm(range(Y_start, Y_end, Y_bin),desc="Building HyperSpectralDataset...",disable=silent):
-        HC[j, :, :] = np.swapaxes(_misc.imread(os.path.join(folder_dir, file_names[i]))[::L_bin, ::X_bin], 0, 1)
-        j = j+1
-    return HC, parameter_dict
-
-def read_xml_to_dict(path):
-    file_name, ext = os.path.splitext(path)
-    assert ext == ".xml"
-
-    xml = ET.parse(path)
-
-    root_element = xml.getroot()
-
-    parameter_dict = dict()
-    for child in root_element:
-        type = child.tag
-        value = child.find('Val')
-        name = child.find('Name')
-        if value is not None:
-            if type == 'Boolean':
-                parameter_dict[name.text] = value.text == '1'
-            if type == 'String':
-                parameter_dict[name.text] = value.text
-            else:
-                parameter_dict[name.text] = float(value.text)
-
-    return parameter_dict
-
-class Measurement(HyperSpectralDataset):
-    """ Class to manage measurement taken with certain hyperspectral imaging setup."""
-    
-    def __init__(self, basepath=None, folder=None, measurement=None, camera_name=None, spectral_calib = True, reference_correction=True, **kwargs):
-        """ Create measurement from folder with images
-
-        Parameters
-        ----------
-        basepath: str
-            Basepath where all folders are located (e.g. 'C:\myData' )
-        folder: str
-            A larger folder within the basepath that contains multiple measurements (e.g. 'DAY_1')
-        measurement: str
-            Folder containing the actual images ('e.g. 'Sample_1'),
-        camera_name:
-            Camera that was used for the measurements. For the Measurement class this can be either 'FX10' or 'FX17' (or 'FX35').
-        kwargs:
-            see pyper.chemometric.HyperSpectralDataset"""
-            
-        if measurement is None:
-            Tk().withdraw()
-            if basepath is not None and os.path.isdir(basepath):
-                initialdir = basepath
-            else:
-                initialdir = None
-            path = filedialog.askdirectory(initialdir=initialdir, title="Please select the folder that contains the RAW images")
-            self.bp, self.folder, self.measurement, self.camera_name = self.split_path(path)
-        else:
-            if camera_name is None:
-                raise ValueError('Please provide camera_name!')
-            self.bp = basepath
-            self.folder = folder
-            self.measurement = measurement
-            self.camera_name = camera_name
-
-        # get camera from camera name
-        self.camera: Camera = self.get_camera_from_name(self.camera_name)
-
-        # get wavelengths from camera
-        wavelength = self.camera.get_wl_full()
-        if 'L_bin' in kwargs:
-            L_bin = kwargs['L_bin']
-            wavelength = wavelength[::L_bin]
-
-        # RAW
-        rawHC, parameter_dict = build_HC_from_folder(self._get_data_path(), **kwargs)
-        super().__init__(hypercube=rawHC, wavelength=wavelength)
-        
-        self.parameter_dict = parameter_dict
-        
-        ## correct for white and dark reference ##
-
-        #remove Y parameters from argument list for reference measurements.
-        reference_kwargs = deepcopy(kwargs)
-        reference_kwargs.pop('Y_bin', None)
-        reference_kwargs.pop('Y_start', None)
-        reference_kwargs.pop('Y_end', None)
-
-        #initialze withouth reference correction
-        self.isWhiteCorrected = False
-        self.isDarkCorrected = False
-
-        # WhiteRef
-        if reference_correction and self._get_path_WhiteRef() is not None:
-            HC, _ = build_HC_from_folder(self._get_path_WhiteRef(), **reference_kwargs)
-            self.whiteHC = HyperSpectralDataset(hypercube=HC, wavelength=wavelength)
-        else:
-            self.whiteHC = None
-
-        # DarkRef
-        if reference_correction and self._get_path_DarkRef() is not None:
-            HC, _ = build_HC_from_folder(self._get_path_DarkRef(), **reference_kwargs)
-            self.darkHC = HyperSpectralDataset(hypercube=HC, wavelength=wavelength)
-        else:
-            self.darkHC = None        
-
-        # perform reference correction either with true hypercubes or with None
-        self.referenceCorrection(self.whiteHC, self.darkHC)
-
-        if spectral_calib:
-            #check Signal to Noise (SNR)
-            if self.isWhiteCorrected and self.isDarkCorrected:
-                try:
-                    s2n, (start_idx, end_idx) = self.get_s2n()
-                    #TODO: make shorter, wrap in warning printer or make more general, not 2x the same
-                    if ( self.get_wl()[start_idx] > self.camera.get_start_wl_s2n() ) or ( self.get_wl()[end_idx] < self.camera.get_end_wl_s2n() ):
-                        print(
-                            'WARNING: The normal wavelength range for {0} was [{1:.1f}nm - {2:.1f}nm], while the SNR suggests a wavelenght range [{3:.1f}nm - {4:.1f}nm].'.format(
-                                self.camera,
-                                self.camera.get_start_wl_s2n(),
-                                self.camera.get_end_wl_s2n(),
-                                self.get_wl()[start_idx],
-                                self.get_wl()[end_idx])
-                                )
-                except ValueError as e:
-                    print(str(e))
-            else:
-                print('WARNING: Data was not white and dark corrected')
-
-            #include only high SNR range from spectrum
-            self.include_wavelengths(self.camera.get_start_wl_s2n(), self.camera.get_end_wl_s2n())
-
-    def referenceCorrection(self, whiteRefHSD = None, darkRefHSD = None):
-
-        # construct references based on given whiteRefHSD and darkRefHSD
-        if darkRefHSD is not None:
-            assert self._is_valid_reference(darkRefHSD)
-            self.isDarkCorrected = True
-            dark_ref = np.mean(darkRefHSD.get_HC(), axis=0)
-        else:
-            dark_ref = 0
-
-        if whiteRefHSD is not None:
-            assert self._is_valid_reference(whiteRefHSD)
-            self.isWhiteCorrected = True
-            white_ref = np.mean(whiteRefHSD.get_HC(), axis=0)
-
-        else:
-            white_ref = 1
-    
-        #perform reference correction
-        HC = self.get_HC()
-
-        HC = np.subtract(HC, dark_ref, out=HC)
-        if self.isWhiteCorrected:
-            white_ref = np.subtract(white_ref, dark_ref, out=white_ref)
-            HC = np.divide(HC, white_ref, out=HC)
-            
-        self.set_HC(HC)
-    
-    @staticmethod
-    def get_camera_from_name(name):
-        if name == 'VISNIR':
-            return Camera.BAUMER
-        elif name == 'SWIR':
-            return Camera.HEADWALL
-        else:
-            ValueError('Unknow Camera name: {0}'.format(name))
-            return None
-
-    def _get_data_path(self):
-        return os.path.join(self.bp, self.folder, self.measurement, self.camera_name)
-
-    def _get_path_WhiteRef(self):
-        return self._get_path('WhRef')
-
-    def _get_path_DarkRef(self):
-        return self._get_path('DarkRef')
-
-    def _construct_searchpath(self, RefType):
-        return os.path.join(self.bp,self.folder,'{0}_{1}*'.format(RefType,self.camera_name))
-
-    def _get_path(self, RefType):
-        """ Get path from a certrain reference type ('DarkRef' or 'WhRef') """
-        search_path = self._construct_searchpath(RefType)
-        folder_list = glob.glob(search_path)
-        
-        #TODO: check with old measurments that have multiple white references, they should take the last one but not compatible with looking at time
-        def sort_key_references(folder_path):
-            if self.parameter_dict and 'Time' in self.parameter_dict:
-                
-                measurement_time = self.parameter_dict['Time']
-                
-                reference_image_path = os.path.join(folder_path, os.listdir(folder_path)[0])
-                reference_time = datetime.fromtimestamp(os.path.getmtime(reference_image_path))
-                return -abs(measurement_time - reference_time)
-            else:
-                return natural_keys(folder_path)
-            
-        folder_list.sort(key= sort_key_references)
-        
-        if len(folder_list) == 0:
-            print('WARNING: No {0} \'s was found, continuing without'.format(RefType))
-            return None
-        elif len(folder_list) > 1:
-            path = folder_list[-1]
-            print('WARNING: Multiple {0} \'s were found, using the last one: {1}'.format(RefType, os.path.split(path)[1]))
-            return path
-        else:
-            return folder_list[0]
-
-    def get_s2n(self, plot=False, s2n_threshold=3):
-        """ Return signal to noise ratio for measurement based on white reference and dark reference.
-
-        plot=True gives an illustrative figure with mean white and dark reference spectra.
-
-        Returns:
-            s2n vector (1-by-nb_wavelengths)
-            tuple of start index and end idx where s2n is greater then s2n_threshold. """
-
-        mean_white_spectrum = self.whiteHC._get_mean_data()
-        mean_dark_spectrum = self.darkHC._get_mean_data()
-        s2n = mean_white_spectrum / mean_dark_spectrum
-
-        if not any(s2n>s2n_threshold):
-            raise ValueError('Not a single wavelength had a signal to noise ration higher then the s2n threshold ({0}). Highest SNR value was {1}.'.format(s2n_threshold, np.amax(s2n)))
-        else:
-            start_idx = np.nonzero(s2n>s2n_threshold)[0][0]
-            end_idx = np.nonzero(s2n>s2n_threshold)[0][-1]
-
-        if plot:
-            fig, (ax1, ax2) = pyplot.subplots(1, 2, figsize=(10, 5))
-
-            wavelength = self.whiteHC.get_wl()
-            ax1.plot(wavelength, mean_white_spectrum, '-m', label= 'Mean Spectrum White Ref')
-            ax1.plot(wavelength, mean_dark_spectrum, '-g', label='Mean Spectrum Dark Ref')
-            ax1.axvline(x=wavelength[start_idx], color='b')
-            ax1.axvline(x=wavelength[end_idx], color='b')
-            ax1.legend()
-
-
-            ax2.plot(s2n, color='k')
-            ax2.axhline(y=s2n_threshold, color='r')
-            ax2.axvline(x=start_idx, color='b')
-            ax2.axvline(x=end_idx, color='b')
-            ax2.set_title('Signal to Noise Ratio')
-
-            pyplot.show()
-        return s2n, (start_idx, end_idx)
-
-    @staticmethod
-    def split_path(path):
-        """ Split the given path that contains the RAW images into a basepath, folder, measurement and camera."""
-        path, camera = os.path.split(path)
-        path, measurement = os.path.split(path)
-        basepath, folder = os.path.split(path)
-        return basepath, folder, measurement, camera
-
-    
-    def isVISNIR(self):
-        return (max(self.get_wl()) < 1100) and (min(self.get_wl()) < 500)
-
-    def isSWIR(self):
-        return (max(self.get_wl()) > 1500) and (min(self.get_wl()) > 900)
-        
-class FxMeasurement(Measurement):
-
-    def __init__(self, basepath=None, folder=None, measurement=None, camera_name=None, **kwargs):
-        super().__init__(basepath=basepath,
-                         folder=folder,
-                         measurement=measurement,
-                         camera_name=camera_name,
-                         **kwargs)
-
-    @staticmethod
-    def get_camera_from_name(name):
-        if name == 'FX10':
-            return Camera.SPECIM_FX10
-        elif name in ['FX17','FX35', 'FX35']:
-            return Camera.SPECIM_FX17
-        else:
-            ValueError('Unknow Camera name: {0}'.format(name))
-            return None
-
-    @staticmethod
-    def split_path(path):
-        path, measurement = os.path.spit(path)
-        path, camera_name = os.path.split(path)
-        basepath, folder = os.path.split(path)
-        return (basepath, folder, measurement, camera_name)
-
-    def _get_data_path(self):
-        return os.path.join(self.bp,self.folder,self.camera_name,self.measurement)
-
-    def _get_path_WhiteRef(self):
-        return self._get_path('WhiteRef')
-    
-    def _construct_searchpath(self, RefType):
-        return os.path.join(self.bp,self.folder,self.camera_name,'{0}*'.format(RefType))
-
-
-class Camera(enum.Enum):
-    BAUMER = ('VISNIR',
-        (3.167478045363729e+02, 1.015349419043834e+03),
-        520,
-        (64, 519))
-
-    HEADWALL = ('SWIR', 
-        (859, 2748),
-        256,
-        (22, 213))
-
-    SPECIM_FX10 = ('VISNIR',
-        (397.66, 1003.81),
-        224,
-        (12, 223))
-
-    SPECIM_FX17 = ('SWIR',
-        (935.61, 1720.23),
-        224,
-        (4, 212))
-    
-    def __init__(self, spectral_name, spectral_range_nm, nb_wl_channels, signal_2_noise_indices):
-        self.spectral_name = spectral_name
-        self.spectral_range_nm = spectral_range_nm
-        self.nb_wl_channels = nb_wl_channels
-        self.signal_2_noise_indices = signal_2_noise_indices
-    
-    def get_wl_full(self):
-        return np.linspace(self.spectral_range_nm[0],self.spectral_range_nm[1],self.nb_wl_channels)
-
-    def get_wl(self):
-        return self.get_wl_full()[self.signal_2_noise_indices[0] : self.signal_2_noise_indices[1]]
-
-    def get_start_idx_s2n(self):
-        return self.signal_2_noise_indices[0]
-
-    def get_start_wl_s2n(self):
-        return self.get_wl_full()[self.get_start_idx_s2n()]
-    
-    def get_end_idx_s2n(self):
-        return self.signal_2_noise_indices[1]
-    
-    def get_end_wl_s2n(self):
-        return self.get_wl_full()[self.get_end_idx_s2n()]
-
-def atoi(text):
-    return int(text) if text.isdigit() else text
-
-def natural_keys(text):
-    return [ atoi(c) for c in re.split(r'(\d+)', text) ]
-
+import glob
+import enum
+from tkinter import Tk, filedialog
+import os
+import numpy as np
+import re
+from matplotlib import pyplot
+from copy import deepcopy
+from datetime import datetime
+from tqdm import tqdm
+from xml.etree import ElementTree as ET
+
+from ._misc import natural_keys
+from . import _misc
+from ..chemometrics.dataset import Dataset, SpectralDataset, HyperSpectralDataset
+
+IMAGE_EXT = ['.tiff','.tif','.png']
+
+def build_HC_from_folder(folder_dir=None, Y_start=0, Y_end=-1, Y_bin = 1, X_bin = 1, L_bin = 1, silent=False, dtype=np.float32) -> np.ndarray :
+    """
+    Build HyperSpectralDataset from folder containing png images
+    """
+    if folder_dir is None:
+        Tk().withdraw()
+        folder_dir = filedialog.askdirectory(title="Please select folder containing the linescan images")
+    
+    all_file_names = os.listdir(folder_dir)
+    file_names = list()
+    parameter_dict = dict()
+    for file_name in all_file_names:
+        [name,ext] = os.path.splitext(file_name)
+        if ext in IMAGE_EXT:
+            file_names.append(file_name)
+        elif ext == '.xml':
+            parameter_dict.update(read_xml_to_dict(os.path.join(folder_dir,file_name)))
+        else:
+            Warning("file: {0} was not included in HyperSpectralDataset because of invalid extention {1}".format(file_name,ext))
+    
+    file_names.sort(key=_misc.natural_keys)
+
+    dimY = len(file_names)
+    [dimL, dimX] = _misc.imread(os.path.join(folder_dir, file_names[0]))[::L_bin, ::X_bin].shape
+
+    if Y_end == -1:
+                Y_end = dimY
+
+    HC = np.empty([len(range(Y_start, Y_end, Y_bin)), dimX, dimL], dtype=dtype)
+    j = 0
+    parameter_dict['Time'] = datetime.fromtimestamp(os.path.getmtime(os.path.join(folder_dir, file_names[Y_start])))
+    for i in tqdm(range(Y_start, Y_end, Y_bin),desc="Building HyperSpectralDataset...",disable=silent):
+        HC[j, :, :] = np.swapaxes(_misc.imread(os.path.join(folder_dir, file_names[i]))[::L_bin, ::X_bin], 0, 1)
+        j = j+1
+    return HC, parameter_dict
+
+def read_xml_to_dict(path):
+    file_name, ext = os.path.splitext(path)
+    assert ext == ".xml"
+
+    xml = ET.parse(path)
+
+    root_element = xml.getroot()
+
+    parameter_dict = dict()
+    for child in root_element:
+        type = child.tag
+        value = child.find('Val')
+        name = child.find('Name')
+        if value is not None:
+            if type == 'Boolean':
+                parameter_dict[name.text] = value.text == '1'
+            if type == 'String':
+                parameter_dict[name.text] = value.text
+            else:
+                parameter_dict[name.text] = float(value.text)
+
+    return parameter_dict
+
+class Measurement(HyperSpectralDataset):
+    """ Class to manage measurement taken with certain hyperspectral imaging setup."""
+    
+    def __init__(self, basepath=None, folder=None, measurement=None, camera_name=None, spectral_calib = True, reference_correction=True, **kwargs):
+        """ Create measurement from folder with images
+
+        Parameters
+        ----------
+        basepath: str
+            Basepath where all folders are located (e.g. 'C:\myData' )
+        folder: str
+            A larger folder within the basepath that contains multiple measurements (e.g. 'DAY_1')
+        measurement: str
+            Folder containing the actual images ('e.g. 'Sample_1'),
+        camera_name:
+            Camera that was used for the measurements. For the Measurement class this can be either 'FX10' or 'FX17' (or 'FX35').
+        kwargs:
+            see pyper.chemometric.HyperSpectralDataset"""
+            
+        if measurement is None:
+            Tk().withdraw()
+            if basepath is not None and os.path.isdir(basepath):
+                initialdir = basepath
+            else:
+                initialdir = None
+            path = filedialog.askdirectory(initialdir=initialdir, title="Please select the folder that contains the RAW images")
+            self.bp, self.folder, self.measurement, self.camera_name = self.split_path(path)
+        else:
+            if camera_name is None:
+                raise ValueError('Please provide camera_name!')
+            self.bp = basepath
+            self.folder = folder
+            self.measurement = measurement
+            self.camera_name = camera_name
+
+        # get camera from camera name
+        self.camera: Camera = self.get_camera_from_name(self.camera_name)
+
+        # get wavelengths from camera
+        wavelength = self.camera.get_wl_full()
+        if 'L_bin' in kwargs:
+            L_bin = kwargs['L_bin']
+            wavelength = wavelength[::L_bin]
+
+        # RAW
+        rawHC, parameter_dict = build_HC_from_folder(self._get_data_path(), **kwargs)
+        super().__init__(hypercube=rawHC, wavelength=wavelength)
+        
+        self.parameter_dict = parameter_dict
+        
+        ## correct for white and dark reference ##
+
+        #remove Y parameters from argument list for reference measurements.
+        reference_kwargs = deepcopy(kwargs)
+        reference_kwargs.pop('Y_bin', None)
+        reference_kwargs.pop('Y_start', None)
+        reference_kwargs.pop('Y_end', None)
+
+        #initialze withouth reference correction
+        self.isWhiteCorrected = False
+        self.isDarkCorrected = False
+
+        # WhiteRef
+        if reference_correction and self._get_path_WhiteRef() is not None:
+            HC, _ = build_HC_from_folder(self._get_path_WhiteRef(), **reference_kwargs)
+            self.whiteHC = HyperSpectralDataset(hypercube=HC, wavelength=wavelength)
+        else:
+            self.whiteHC = None
+
+        # DarkRef
+        if reference_correction and self._get_path_DarkRef() is not None:
+            HC, _ = build_HC_from_folder(self._get_path_DarkRef(), **reference_kwargs)
+            self.darkHC = HyperSpectralDataset(hypercube=HC, wavelength=wavelength)
+        else:
+            self.darkHC = None        
+
+        # perform reference correction either with true hypercubes or with None
+        self.referenceCorrection(self.whiteHC, self.darkHC)
+
+        if spectral_calib:
+            #check Signal to Noise (SNR)
+            if self.isWhiteCorrected and self.isDarkCorrected:
+                try:
+                    s2n, (start_idx, end_idx) = self.get_s2n()
+                    #TODO: make shorter, wrap in warning printer or make more general, not 2x the same
+                    if ( self.get_wl()[start_idx] > self.camera.get_start_wl_s2n() ) or ( self.get_wl()[end_idx] < self.camera.get_end_wl_s2n() ):
+                        print(
+                            'WARNING: The normal wavelength range for {0} was [{1:.1f}nm - {2:.1f}nm], while the SNR suggests a wavelenght range [{3:.1f}nm - {4:.1f}nm].'.format(
+                                self.camera,
+                                self.camera.get_start_wl_s2n(),
+                                self.camera.get_end_wl_s2n(),
+                                self.get_wl()[start_idx],
+                                self.get_wl()[end_idx])
+                                )
+                except ValueError as e:
+                    print(str(e))
+            else:
+                print('WARNING: Data was not white and dark corrected')
+
+            #include only high SNR range from spectrum
+            self.include_wavelengths(self.camera.get_start_wl_s2n(), self.camera.get_end_wl_s2n())
+
+    def referenceCorrection(self, whiteRefHSD = None, darkRefHSD = None):
+
+        # construct references based on given whiteRefHSD and darkRefHSD
+        if darkRefHSD is not None:
+            assert self._is_valid_reference(darkRefHSD)
+            self.isDarkCorrected = True
+            dark_ref = np.mean(darkRefHSD.get_HC(), axis=0)
+        else:
+            dark_ref = 0
+
+        if whiteRefHSD is not None:
+            assert self._is_valid_reference(whiteRefHSD)
+            self.isWhiteCorrected = True
+            white_ref = np.mean(whiteRefHSD.get_HC(), axis=0)
+
+        else:
+            white_ref = 1
+    
+        #perform reference correction
+        HC = self.get_HC()
+
+        HC = np.subtract(HC, dark_ref, out=HC)
+        if self.isWhiteCorrected:
+            white_ref = np.subtract(white_ref, dark_ref, out=white_ref)
+            HC = np.divide(HC, white_ref, out=HC)
+            
+        self.set_HC(HC)
+    
+    @staticmethod
+    def get_camera_from_name(name):
+        if name == 'VISNIR':
+            return Camera.BAUMER
+        elif name == 'SWIR':
+            return Camera.HEADWALL
+        else:
+            ValueError('Unknow Camera name: {0}'.format(name))
+            return None
+
+    def _get_data_path(self):
+        return os.path.join(self.bp, self.folder, self.measurement, self.camera_name)
+
+    def _get_path_WhiteRef(self):
+        return self._get_path('WhRef')
+
+    def _get_path_DarkRef(self):
+        return self._get_path('DarkRef')
+
+    def _construct_searchpath(self, RefType):
+        return os.path.join(self.bp,self.folder,'{0}_{1}*'.format(RefType,self.camera_name))
+
+    def _get_path(self, RefType):
+        """ Get path from a certrain reference type ('DarkRef' or 'WhRef') """
+        search_path = self._construct_searchpath(RefType)
+        folder_list = glob.glob(search_path)
+        
+        #TODO: check with old measurments that have multiple white references, they should take the last one but not compatible with looking at time
+        def sort_key_references(folder_path):
+            if self.parameter_dict and 'Time' in self.parameter_dict:
+                
+                measurement_time = self.parameter_dict['Time']
+                
+                reference_image_path = os.path.join(folder_path, os.listdir(folder_path)[0])
+                reference_time = datetime.fromtimestamp(os.path.getmtime(reference_image_path))
+                return -abs(measurement_time - reference_time)
+            else:
+                return natural_keys(folder_path)
+            
+        folder_list.sort(key= sort_key_references)
+        
+        if len(folder_list) == 0:
+            print('WARNING: No {0} \'s was found, continuing without'.format(RefType))
+            return None
+        elif len(folder_list) > 1:
+            path = folder_list[-1]
+            print('WARNING: Multiple {0} \'s were found, using the last one: {1}'.format(RefType, os.path.split(path)[1]))
+            return path
+        else:
+            return folder_list[0]
+
+    def get_s2n(self, plot=False, s2n_threshold=3):
+        """ Return signal to noise ratio for measurement based on white reference and dark reference.
+
+        plot=True gives an illustrative figure with mean white and dark reference spectra.
+
+        Returns:
+            s2n vector (1-by-nb_wavelengths)
+            tuple of start index and end idx where s2n is greater then s2n_threshold. """
+
+        mean_white_spectrum = self.whiteHC._get_mean_data()
+        mean_dark_spectrum = self.darkHC._get_mean_data()
+        s2n = mean_white_spectrum / mean_dark_spectrum
+
+        if not any(s2n>s2n_threshold):
+            raise ValueError('Not a single wavelength had a signal to noise ration higher then the s2n threshold ({0}). Highest SNR value was {1}.'.format(s2n_threshold, np.amax(s2n)))
+        else:
+            start_idx = np.nonzero(s2n>s2n_threshold)[0][0]
+            end_idx = np.nonzero(s2n>s2n_threshold)[0][-1]
+
+        if plot:
+            fig, (ax1, ax2) = pyplot.subplots(1, 2, figsize=(10, 5))
+
+            wavelength = self.whiteHC.get_wl()
+            ax1.plot(wavelength, mean_white_spectrum, '-m', label= 'Mean Spectrum White Ref')
+            ax1.plot(wavelength, mean_dark_spectrum, '-g', label='Mean Spectrum Dark Ref')
+            ax1.axvline(x=wavelength[start_idx], color='b')
+            ax1.axvline(x=wavelength[end_idx], color='b')
+            ax1.legend()
+
+
+            ax2.plot(s2n, color='k')
+            ax2.axhline(y=s2n_threshold, color='r')
+            ax2.axvline(x=start_idx, color='b')
+            ax2.axvline(x=end_idx, color='b')
+            ax2.set_title('Signal to Noise Ratio')
+
+            pyplot.show()
+        return s2n, (start_idx, end_idx)
+
+    @staticmethod
+    def split_path(path):
+        """ Split the given path that contains the RAW images into a basepath, folder, measurement and camera."""
+        path, camera = os.path.split(path)
+        path, measurement = os.path.split(path)
+        basepath, folder = os.path.split(path)
+        return basepath, folder, measurement, camera
+
+    
+    def isVISNIR(self):
+        return (max(self.get_wl()) < 1100) and (min(self.get_wl()) < 500)
+
+    def isSWIR(self):
+        return (max(self.get_wl()) > 1500) and (min(self.get_wl()) > 900)
+        
+class FxMeasurement(Measurement):
+
+    def __init__(self, basepath=None, folder=None, measurement=None, camera_name=None, **kwargs):
+        super().__init__(basepath=basepath,
+                         folder=folder,
+                         measurement=measurement,
+                         camera_name=camera_name,
+                         **kwargs)
+
+    @staticmethod
+    def get_camera_from_name(name):
+        if name == 'FX10':
+            return Camera.SPECIM_FX10
+        elif name in ['FX17','FX35', 'FX35']:
+            return Camera.SPECIM_FX17
+        else:
+            ValueError('Unknow Camera name: {0}'.format(name))
+            return None
+
+    @staticmethod
+    def split_path(path):
+        path, measurement = os.path.spit(path)
+        path, camera_name = os.path.split(path)
+        basepath, folder = os.path.split(path)
+        return (basepath, folder, measurement, camera_name)
+
+    def _get_data_path(self):
+        return os.path.join(self.bp,self.folder,self.camera_name,self.measurement)
+
+    def _get_path_WhiteRef(self):
+        return self._get_path('WhiteRef')
+    
+    def _construct_searchpath(self, RefType):
+        return os.path.join(self.bp,self.folder,self.camera_name,'{0}*'.format(RefType))
+
+
+class Camera(enum.Enum):
+    BAUMER = ('VISNIR',
+        (3.167478045363729e+02, 1.015349419043834e+03),
+        520,
+        (64, 519))
+
+    HEADWALL = ('SWIR', 
+        (859, 2748),
+        256,
+        (22, 213))
+
+    SPECIM_FX10 = ('VISNIR',
+        (397.66, 1003.81),
+        224,
+        (12, 223))
+
+    SPECIM_FX17 = ('SWIR',
+        (935.61, 1720.23),
+        224,
+        (4, 212))
+    
+    def __init__(self, spectral_name, spectral_range_nm, nb_wl_channels, signal_2_noise_indices):
+        self.spectral_name = spectral_name
+        self.spectral_range_nm = spectral_range_nm
+        self.nb_wl_channels = nb_wl_channels
+        self.signal_2_noise_indices = signal_2_noise_indices
+    
+    def get_wl_full(self):
+        return np.linspace(self.spectral_range_nm[0],self.spectral_range_nm[1],self.nb_wl_channels)
+
+    def get_wl(self):
+        return self.get_wl_full()[self.signal_2_noise_indices[0] : self.signal_2_noise_indices[1]]
+
+    def get_start_idx_s2n(self):
+        return self.signal_2_noise_indices[0]
+
+    def get_start_wl_s2n(self):
+        return self.get_wl_full()[self.get_start_idx_s2n()]
+    
+    def get_end_idx_s2n(self):
+        return self.signal_2_noise_indices[1]
+    
+    def get_end_wl_s2n(self):
+        return self.get_wl_full()[self.get_end_idx_s2n()]
+
+def atoi(text):
+    return int(text) if text.isdigit() else text
+
+def natural_keys(text):
+    return [ atoi(c) for c in re.split(r'(\d+)', text) ]
+
```

## Comparing `phyper-1.1.1.dist-info/LICENSE` & `phyper-1.1.2.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Remi Van Belleghem
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Remi Van Belleghem
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

## Comparing `phyper-1.1.1.dist-info/METADATA` & `phyper-1.1.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: phyper
-Version: 1.1.1
+Version: 1.1.2
 Summary: Package for managing (hyper)spectral datasets
 Home-page: https://gitlab.kuleuven.be/u0123403/pyper
 Author: Remi Van Belleghem
 Author-email: remi.vanbelleghem@kuleuven.be
 Maintainer: MeBios - KULeuven
 Maintainer-email: wouter.saeys@kuleuven.be
-License: UNKNOWN
 Keywords: hyperspectral,chemometrics
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6,<4.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 Requires-Dist: numpy
 Requires-Dist: scikit-image
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: h5py
@@ -64,9 +63,7 @@
 2. Use pip to install the package in editable format  
 `pip install -e .`
 
 
 ## Acknowledgements
 
 Written by Remi Van Belleghem. Based on Matlab toolbox from Niels Wouters.
-
-
```

## Comparing `phyper-1.1.1.dist-info/RECORD` & `phyper-1.1.2.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-phyper/__init__.py,sha256=rMnnYTKywiNcd7S6oPtxYBT4QEV8eI0iEo8qODIE7NE,702
-phyper/chemometrics/__init__.py,sha256=qVRqkzJvD4R_HUW0YQQX_ZnBs0m0p8VRyZR-QeBTFRE,306
-phyper/chemometrics/_gui.py,sha256=EnzCiq8Qoicyzlkc3Y_x2e8sGeqOEaBaFebk_AG1cqY,9908
-phyper/chemometrics/analysis.py,sha256=_JMSybKDLtsCa_XdzZP2xSRGWOekIyJrf86j0i66naM,13557
-phyper/chemometrics/dataset.py,sha256=Y80Frsee_7bPLn1Ou2QFHY_kp5_ERJ3Bx44mu9HyOa4,49010
-phyper/chemometrics/preprocessing.py,sha256=PGAKLEt9MZ8zf-e-3dlHorm6Z08Kq3S14eENWH6U__g,2812
-phyper/chemometrics/sampling.py,sha256=06c2PBQAiKWISs9XB58KZM3GdQ6auyPhtAGW-qIAhd0,2367
-phyper/lab/__init__.py,sha256=W0eCkr3D_9dfJAtpdQUqP0TdcFhawvgtYhFzjJJACSE,125
-phyper/lab/_misc.py,sha256=KTk0YJ-7xZD5KHvWFpUvQ1tlknScsmyKwsQBBU4gi-A,837
-phyper/lab/measurement.py,sha256=u0jMaFvN8Vg2jQWZlNpRGjxeHaLyn1pIKyBc0HQWkPM,15674
-phyper-1.1.1.dist-info/LICENSE,sha256=T4LpDPD8asb3PVqM4EeapjKLmfOIFDoGstaL4g-Bzpc,1096
-phyper-1.1.1.dist-info/METADATA,sha256=IqRGd8gtMA-s4uPxep1Fvc5B6HxYxRJA-6hgBXtP0KA,2246
-phyper-1.1.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-phyper-1.1.1.dist-info/top_level.txt,sha256=1CRpBqxQW0H4uxZ6GzjiIKUq4FJksW5pai8komowTII,7
-phyper-1.1.1.dist-info/RECORD,,
+phyper/__init__.py,sha256=4hYB58cealu01B6FLn3lhRnI0JAPY6Va107e65WXTcs,685
+phyper/chemometrics/__init__.py,sha256=5y7WaXHDvt1RbplvdekletkldO9cMdvYHRFzJkE1ziE,292
+phyper/chemometrics/_gui.py,sha256=3h4jW2pVt-14QTx3g-wFnMzaQTq8SZC2BBabRBZ9bpA,9505
+phyper/chemometrics/analysis.py,sha256=903ZGNPjkmJL_z0CeeorcQkoiCMZLeOYK3_q18CmBnc,13252
+phyper/chemometrics/dataset.py,sha256=cb4A3edpXYI0IEQ-QaCP7o8diph15cNHgF4LkffKsyg,48428
+phyper/chemometrics/preprocessing.py,sha256=lKoB64-a4IdM82pC1OAh9cCy-LXKLOcFbygVYnQCBcM,2713
+phyper/chemometrics/sampling.py,sha256=H-xl0PrAwRoaxwah8DqVSlRJ1gPl9Qm806Zh7MPuu2U,2298
+phyper/lab/__init__.py,sha256=p1f53MLglxawnDhRGT4O1NI5CpL2Rvski2XEyg9ErM8,121
+phyper/lab/_misc.py,sha256=irgAaObHkaIBESTdw-o0e0Eb-z2pUm9Kdc9ujZq8pg8,802
+phyper/lab/measurement.py,sha256=YCQX5YkgWDmwesoELt14JgdWcVYc2vq8cqnjIbxHfSM,15275
+phyper-1.1.2.dist-info/LICENSE,sha256=i-l_fDhG098wzA_kHlskLIwp3UKEjHzNP1PVuIu2wuQ,1075
+phyper-1.1.2.dist-info/METADATA,sha256=rsaJ8dFhjWDd87IaeJPwJdq1crlJsJvs_sCKnLjAFtU,2231
+phyper-1.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+phyper-1.1.2.dist-info/top_level.txt,sha256=1CRpBqxQW0H4uxZ6GzjiIKUq4FJksW5pai8komowTII,7
+phyper-1.1.2.dist-info/RECORD,,
```

