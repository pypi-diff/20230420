# Comparing `tmp/phyper-1.0.0-py3-none-any.whl.zip` & `tmp/phyper-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 28419 bytes, number of entries: 15
+Zip file size: 28827 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat      702 b- defN 22-Jul-29 10:10 phyper/__init__.py
 -rw-rw-rw-  2.0 fat      306 b- defN 22-Feb-21 09:50 phyper/chemometrics/__init__.py
--rw-rw-rw-  2.0 fat     7709 b- defN 22-Jul-29 10:10 phyper/chemometrics/_gui.py
+-rw-rw-rw-  2.0 fat     9908 b- defN 23-Apr-20 07:56 phyper/chemometrics/_gui.py
 -rw-rw-rw-  2.0 fat    13557 b- defN 22-Oct-20 15:23 phyper/chemometrics/analysis.py
 -rw-rw-rw-  2.0 fat    49010 b- defN 22-Oct-20 15:23 phyper/chemometrics/dataset.py
 -rw-rw-rw-  2.0 fat     2812 b- defN 22-Oct-20 15:23 phyper/chemometrics/preprocessing.py
 -rw-rw-rw-  2.0 fat     2367 b- defN 22-Feb-21 09:50 phyper/chemometrics/sampling.py
 -rw-rw-rw-  2.0 fat      125 b- defN 22-Feb-21 09:50 phyper/lab/__init__.py
 -rw-rw-rw-  2.0 fat      837 b- defN 22-Oct-20 15:23 phyper/lab/_misc.py
--rw-rw-rw-  2.0 fat    15674 b- defN 22-Oct-20 15:23 phyper/lab/measurement.py
--rw-rw-rw-  2.0 fat     1096 b- defN 23-Feb-01 10:32 phyper-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2134 b- defN 23-Feb-01 10:32 phyper-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-01 10:32 phyper-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Feb-01 10:32 phyper-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1219 b- defN 23-Feb-01 10:32 phyper-1.0.0.dist-info/RECORD
-15 files, 97647 bytes uncompressed, 26409 bytes compressed:  73.0%
+-rw-rw-rw-  2.0 fat    15674 b- defN 23-Mar-28 09:11 phyper/lab/measurement.py
+-rw-rw-rw-  2.0 fat     1096 b- defN 23-Apr-20 10:22 phyper-1.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-Apr-20 10:22 phyper-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 10:22 phyper-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-20 10:22 phyper-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1219 b- defN 23-Apr-20 10:22 phyper-1.1.0.dist-info/RECORD
+15 files, 99958 bytes uncompressed, 26817 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: phyper/lab/_misc.py
 Comment: 
 
 Filename: phyper/lab/measurement.py
 Comment: 
 
-Filename: phyper-1.0.0.dist-info/LICENSE
+Filename: phyper-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: phyper-1.0.0.dist-info/METADATA
+Filename: phyper-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: phyper-1.0.0.dist-info/WHEEL
+Filename: phyper-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: phyper-1.0.0.dist-info/top_level.txt
+Filename: phyper-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: phyper-1.0.0.dist-info/RECORD
+Filename: phyper-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## phyper/chemometrics/_gui.py

```diff
@@ -143,26 +143,29 @@
         def draw_spectrum(self, axis, wl, spectrum):
             axis.plot(wl, spectrum, color=self.color)
 
 class MaskCreator(object):
     """Draw mask using selector
     """
     def __init__(self, ax, selector = 'polygon'):
-        ''' Selector can be 'lasso' or 'polygon'
+        ''' Selector can be 'lasso' or 'polygon' or 'points'
         '''
         if selector == 'lasso':
             self.selector = LassoSelector(ax,
                                           self.onselect,
                                           lineprops={'color':'r','linewidth':5})
-        else:
+        elif selector == 'polygon':
             self.selector = PolygonSelector(ax,
                                             self.onselect,
                                             useblit=True,
                                             lineprops={'color':'r'},
                                             markerprops={'color':'r'})
+        else:
+            raise ValueError(f'Unknown selector value "{selector}" ')
+        
         self.path = None
 
     def get_mask(self, shape):
         """Return image mask given by mask creator"""
         if self.path is None:
             return np.zeros(shape,dtype=bool)
         h, w = shape
@@ -170,25 +173,88 @@
         points = np.transpose((x.ravel(), y.ravel()))
         grid = self.path.contains_points(points)  # now you have a mask with points inside a polygon
         return grid.reshape(h, w)
 
     def onselect(self, verts):
         self.path = Path(verts)
 
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
+        print(self.points)
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
+            print(event.artist)
+            # remove point if right-clicked
+            self.points.remove(event.artist.obj)
+            event.artist.remove()
+        self.update()
 
+    def get_mask(self, shape):
+        """Return image mask given by mask creator"""
+        mask =  np.zeros(shape,dtype=bool)
+        for x,y in self.points:
+            mask[y,x] = True
+        return mask
+    
 def mask_creator_demo():
     img = np.random.uniform(0, 255, size=(100, 100))
     ax = pyplot.subplot(111)
     ax.imshow(img)
 
     mc = MaskCreator(ax, 'lasso')
     pyplot.show()
 
     mask = mc.get_mask(img.shape)
     img[~mask] = np.uint8(np.clip(img[~mask] - 100., 0, 255))
     pyplot.imshow(img)
     pyplot.title('Region outside of mask is darkened')
     pyplot.show()
 
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
 
 if __name__ == '__main__':
+    points_creator_demo()
     mask_creator_demo()
```

## Comparing `phyper-1.0.0.dist-info/LICENSE` & `phyper-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `phyper-1.0.0.dist-info/METADATA` & `phyper-1.1.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phyper
-Version: 1.0.0
+Version: 1.1.0
 Summary: Package for managing (hyper)spectral datasets
 Home-page: https://gitlab.kuleuven.be/u0123403/pyper
 Author: Remi Van Belleghem
 Author-email: remi.vanbelleghem@kuleuven.be
 Maintainer: MeBios - KULeuven
 Maintainer-email: wouter.saeys@kuleuven.be
 License: UNKNOWN
@@ -37,15 +37,20 @@
 
 ### Non-editable installation
 
 0. (Optional) create virtual environment  
 `conda create -n my_env python=3.8`  
 `conda activate my_env`
 
-1. Directly intall from gitlab repostiory  
+1.a Directly install from PyPi directory where pyper is saved as 'phyper' (WITH h!)
+`pip install phyper`
+
+OR  
+
+1.b Directly intall from gitlab repostiory
 `pip install git+https://gitlab.kuleuven.be/u0123403/pyper.git`
 
 ### Editable installation 
 
 Use this installation if you want to make changes to the code yourself.
 
 0. (Optional) create virtual environment   
@@ -60,7 +65,8 @@
 `pip install -e .`
 
 
 ## Acknowledgements
 
 Written by Remi Van Belleghem. Based on Matlab toolbox from Niels Wouters.
 
+
```

## Comparing `phyper-1.0.0.dist-info/RECORD` & `phyper-1.1.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 phyper/__init__.py,sha256=rMnnYTKywiNcd7S6oPtxYBT4QEV8eI0iEo8qODIE7NE,702
 phyper/chemometrics/__init__.py,sha256=qVRqkzJvD4R_HUW0YQQX_ZnBs0m0p8VRyZR-QeBTFRE,306
-phyper/chemometrics/_gui.py,sha256=dWxz4y2vqxfCRq9jWhNtz0wQ6jzvGElBXy0Ce_-mcDc,7709
+phyper/chemometrics/_gui.py,sha256=EnzCiq8Qoicyzlkc3Y_x2e8sGeqOEaBaFebk_AG1cqY,9908
 phyper/chemometrics/analysis.py,sha256=_JMSybKDLtsCa_XdzZP2xSRGWOekIyJrf86j0i66naM,13557
 phyper/chemometrics/dataset.py,sha256=Y80Frsee_7bPLn1Ou2QFHY_kp5_ERJ3Bx44mu9HyOa4,49010
 phyper/chemometrics/preprocessing.py,sha256=PGAKLEt9MZ8zf-e-3dlHorm6Z08Kq3S14eENWH6U__g,2812
 phyper/chemometrics/sampling.py,sha256=06c2PBQAiKWISs9XB58KZM3GdQ6auyPhtAGW-qIAhd0,2367
 phyper/lab/__init__.py,sha256=W0eCkr3D_9dfJAtpdQUqP0TdcFhawvgtYhFzjJJACSE,125
 phyper/lab/_misc.py,sha256=KTk0YJ-7xZD5KHvWFpUvQ1tlknScsmyKwsQBBU4gi-A,837
 phyper/lab/measurement.py,sha256=u0jMaFvN8Vg2jQWZlNpRGjxeHaLyn1pIKyBc0HQWkPM,15674
-phyper-1.0.0.dist-info/LICENSE,sha256=T4LpDPD8asb3PVqM4EeapjKLmfOIFDoGstaL4g-Bzpc,1096
-phyper-1.0.0.dist-info/METADATA,sha256=zbt2aXhMLl3AaTLGgH8XLAZiEdMGdqgrHYwJu62KY54,2134
-phyper-1.0.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-phyper-1.0.0.dist-info/top_level.txt,sha256=1CRpBqxQW0H4uxZ6GzjiIKUq4FJksW5pai8komowTII,7
-phyper-1.0.0.dist-info/RECORD,,
+phyper-1.1.0.dist-info/LICENSE,sha256=T4LpDPD8asb3PVqM4EeapjKLmfOIFDoGstaL4g-Bzpc,1096
+phyper-1.1.0.dist-info/METADATA,sha256=Rq3M0yE3wF4Yw5_sJgPLVERhpGMRdIHkBS5M1McEHCc,2246
+phyper-1.1.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+phyper-1.1.0.dist-info/top_level.txt,sha256=1CRpBqxQW0H4uxZ6GzjiIKUq4FJksW5pai8komowTII,7
+phyper-1.1.0.dist-info/RECORD,,
```

