# Comparing `tmp/skye-0.0.1.tar.gz` & `tmp/skye-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skye-0.0.1.tar", last modified: Thu Apr 20 04:49:40 2023, max compression
+gzip compressed data, was "skye-0.0.2.tar", last modified: Thu Apr 20 06:46:09 2023, max compression
```

## Comparing `skye-0.0.1.tar` & `skye-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-20 04:49:40.623378 skye-0.0.1/
--rw-r--r--   0 iosefa     (501) staff       (20)     1072 2023-04-20 02:33:45.000000 skye-0.0.1/LICENSE
--rw-r--r--   0 iosefa     (501) staff       (20)      783 2023-04-20 04:49:40.623142 skye-0.0.1/PKG-INFO
--rw-r--r--   0 iosefa     (501) staff       (20)      285 2023-04-20 02:33:45.000000 skye-0.0.1/README.md
--rw-r--r--   0 iosefa     (501) staff       (20)       38 2023-04-20 04:49:40.623451 skye-0.0.1/setup.cfg
--rw-r--r--   0 iosefa     (501) staff       (20)      756 2023-04-20 03:42:43.000000 skye-0.0.1/setup.py
-drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-20 04:49:40.621121 skye-0.0.1/skye/
--rw-r--r--   0 iosefa     (501) staff       (20)        0 2023-04-20 02:33:45.000000 skye-0.0.1/skye/__init__.py
--rw-r--r--   0 iosefa     (501) staff       (20)     9886 2023-04-20 04:46:13.000000 skye-0.0.1/skye/core.py
--rw-r--r--   0 iosefa     (501) staff       (20)      876 2023-04-20 02:33:45.000000 skye-0.0.1/skye/utils.py
-drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-20 04:49:40.622804 skye-0.0.1/skye.egg-info/
--rw-r--r--   0 iosefa     (501) staff       (20)      783 2023-04-20 04:49:40.000000 skye-0.0.1/skye.egg-info/PKG-INFO
--rw-r--r--   0 iosefa     (501) staff       (20)      182 2023-04-20 04:49:40.000000 skye-0.0.1/skye.egg-info/SOURCES.txt
--rw-r--r--   0 iosefa     (501) staff       (20)        1 2023-04-20 04:49:40.000000 skye-0.0.1/skye.egg-info/dependency_links.txt
--rw-r--r--   0 iosefa     (501) staff       (20)        5 2023-04-20 04:49:40.000000 skye-0.0.1/skye.egg-info/top_level.txt
+drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-20 06:46:09.317968 skye-0.0.2/
+-rw-r--r--   0 iosefa     (501) staff       (20)     1072 2023-04-20 02:33:45.000000 skye-0.0.2/LICENSE
+-rw-r--r--   0 iosefa     (501) staff       (20)      858 2023-04-20 06:46:09.317641 skye-0.0.2/PKG-INFO
+-rw-r--r--   0 iosefa     (501) staff       (20)      360 2023-04-20 04:54:09.000000 skye-0.0.2/README.md
+-rw-r--r--   0 iosefa     (501) staff       (20)       38 2023-04-20 06:46:09.318059 skye-0.0.2/setup.cfg
+-rw-r--r--   0 iosefa     (501) staff       (20)      756 2023-04-20 06:44:05.000000 skye-0.0.2/setup.py
+drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-20 06:46:09.316039 skye-0.0.2/skye/
+-rw-r--r--   0 iosefa     (501) staff       (20)        0 2023-04-20 02:33:45.000000 skye-0.0.2/skye/__init__.py
+-rw-r--r--   0 iosefa     (501) staff       (20)     9442 2023-04-20 06:22:51.000000 skye-0.0.2/skye/core.py
+-rw-r--r--   0 iosefa     (501) staff       (20)      876 2023-04-20 02:33:45.000000 skye-0.0.2/skye/utils.py
+drwxr-xr-x   0 iosefa     (501) staff       (20)        0 2023-04-20 06:46:09.317310 skye-0.0.2/skye.egg-info/
+-rw-r--r--   0 iosefa     (501) staff       (20)      858 2023-04-20 06:46:09.000000 skye-0.0.2/skye.egg-info/PKG-INFO
+-rw-r--r--   0 iosefa     (501) staff       (20)      182 2023-04-20 06:46:09.000000 skye-0.0.2/skye.egg-info/SOURCES.txt
+-rw-r--r--   0 iosefa     (501) staff       (20)        1 2023-04-20 06:46:09.000000 skye-0.0.2/skye.egg-info/dependency_links.txt
+-rw-r--r--   0 iosefa     (501) staff       (20)        5 2023-04-20 06:46:09.000000 skye-0.0.2/skye.egg-info/top_level.txt
```

### Comparing `skye-0.0.1/LICENSE` & `skye-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skye-0.0.1/PKG-INFO` & `skye-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skye
-Version: 0.0.1
+Version: 0.0.2
 Summary: 360-degree image analysis for forest ecology
 Home-page: https://github.com/iosefa/skye
 Author: Iosefa Percival
 Author-email: ipercival@gmail.com
 Project-URL: Bug Tracker, https://github.com/iosefa/skye/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,9 +13,12 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SKYE
 
 Skye is a simple python library for working with 360-degree photos for analysis in forest ecology.
 
+_This library is currently experimental and is under heavy development_.
+
 Current features include the ability to create hemispherical photographs from 3-band (RGB) 360-degree photos, 
 sky object detection, and the calculation of the sky view factor.
+
```

### Comparing `skye-0.0.1/setup.py` & `skye-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="skye",
-    version="0.0.1",
+    version="0.0.2",
     author="Iosefa Percival",
     author_email="ipercival@gmail.com",
     description="360-degree image analysis for forest ecology",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iosefa/skye",
     project_urls={
```

### Comparing `skye-0.0.1/skye/core.py` & `skye-0.0.2/skye/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         image = io.imread(img)
         return image
     except Exception as e:
         raise Exception(f'Could not import image. Original exception: {e}')
 
 
 def segment_image(img, ratio=0.85, sigma=0):
+    img = np.array(img)
     img = img_as_float(img)
     segments = quickshift(img, ratio=ratio, sigma=sigma)
     return segments
 
 
 def summary_statistics(segment_pixels):
     """
@@ -50,14 +51,15 @@
     return features
 
 
 def create_objects(img, segments):
     """
     Creates objects based on a given segmentation algorithm
     """
+    img = np.array(img)
     image = img_as_float(img)
     segment_ids = np.unique(segments)
 
     objects = []
     for segment_id in tqdm(segment_ids, bar_format='{l_bar}{bar}', desc="Creating Objects"):
         segment_pixels = image[segments == segment_id]
         segment_stats = summary_statistics(segment_pixels)
@@ -107,15 +109,16 @@
     im_b = np.concatenate((img_h2[:dim2], img_h2[dim2 + 2:]), axis=0)
     im_bb = np.concatenate((im_b[:, :dim2], im_b[:, dim2 + 2:]), axis=1)
     img = Image.fromarray(im_bb.astype(np.uint8))
     return img
 
 
 def calculate_svf(img, bi_img):
-    img = img_as_float(img)
+    img = np.array(img)
+    bi_img = np.array(bi_img)
     total_pixels = img.shape[0] * img.shape[0]
     hemisphere_pixels = pi * ((img.shape[0] / 2) ** 2)
     outside_pixels = total_pixels - hemisphere_pixels
 
     black_pixels = total_pixels - np.sum(bi_img / 255) - outside_pixels
     svf = (hemisphere_pixels - black_pixels) / hemisphere_pixels
     return svf
@@ -126,30 +129,28 @@
         self,
         image_path: str,
         threshold=0.5
     ):
         self.image_path = image_path
         self.img = create_hemispherical(image_path)
         self.threshold = threshold * 255
-        self.gray_img = cv2.cvtColor(self.img, cv2.COLOR_RGB2GRAY)
+        self.gray_img = cv2.cvtColor(np.array(self.img), cv2.COLOR_RGB2GRAY)
         self.binary_img = self.create_binary()
         self.sky_view_factor = calculate_svf(self.img, self.binary_img)
 
     def create_binary(self):
         binary_img = self.gray_img.copy()
         binary_img[binary_img >= self.threshold] = 255
         binary_img[binary_img < self.threshold] = 0
-        return binary_img
+        im = Image.fromarray(binary_img.astype(np.uint8))
+        return im
 
-    def plot_binary(self):
-        im = Image.fromarray(self.binary_img.astype(np.uint8))
-        fig = plt.figure("Binary Threshold Image", figsize=(14, 14))
-        ax = fig.add_subplot(1, 1, 1)
-        ax.imshow(im)
-        plt.axis("off")
+    def plot_binary(self, ax):
+        out = ax.imshow(self.binary_img)
+        return out
 
 
 class SkyViewClassified:
     def __init__(
         self,
         image_path: str,
         training_data_path=None
@@ -186,29 +187,30 @@
             logging.warning('You must create or import training data in order to calculate the sky view factor')
 
     def plot_rgb(self, ax):
         out = ax.imshow(self.img)
         return out
 
     def plot_segments(self, ax):
-        img = img_as_float(self.img)
+        img = np.array(self.img)
         boundaries = mark_boundaries(img, self.segments)
         out = ax.imshow(boundaries)
         return out
 
     def plot_classified(self, ax):
         if self.classified_img is None:
             logging.warning('Image has not yet been classified. Aborting.')
             return
         out = ax.imshow(self.classified_img)
         return out
 
     def create_training_data(self, n_samples=500, notebook=False):
         sample = random.sample(list(self.objects_df_clean['segment_id'].values), n_samples)
-        img = img_as_float(self.img)
+        img = np.array(self.img)
+        img = img_as_float(img)
         for j, i in enumerate(sample):
             print(f'working on segment {i} ({j}/500)')
             mask = np.ma.masked_where(self.segments != i, self.segments)
             valid_pixels = np.argwhere(~np.isnan(mask))
             y_min, x_min = tuple(np.min(valid_pixels, axis=0))
             y_max, x_max = tuple(np.max(valid_pixels, axis=0))
 
@@ -246,26 +248,15 @@
         x_train = self.training_classes.drop(['class'], axis=1)
         y_train = self.training_classes['class']
         x_test = self.objects_df.drop(['segment_id'], axis=1).dropna()
         rf = RandomForestClassifier()
         rf.fit(x_train, y_train)
         y_pred = rf.predict(x_test)
         segment_ids = list(self.objects_df_clean['segment_id'].values)
-        classified_img = img_as_float(self.img).copy()
+        classified_img = img_as_float(np.array(self.img)).copy()
         for i, segment_id in enumerate(segment_ids):
             idx = np.argwhere(self.segments == segment_id)
             for j in idx:
                 classified_img[j[0], j[1], 0] = y_pred[i]
-
-        return classified_img[:, :, 0]
-
-    # def calculate_svf(self):
-    #     if not self.classified_img:
-    #         print('Image has not yet been classified.')
-    #         return
-    #     total_pixels = self.img.shape[0] * self.img.shape[0]
-    #     hemisphere_pixels = pi * ((self.img.shape[0] / 2) ** 2)
-    #     outside_pixels = total_pixels - hemisphere_pixels
-    #
-    #     black_pixels = total_pixels - np.sum(self.classified_img / 255) - outside_pixels
-    #     svf = (hemisphere_pixels - black_pixels) / hemisphere_pixels
-    #     return svf
+        clf = classified_img[:, :, 0]
+        im = Image.fromarray(clf.astype(np.uint8))
+        return im
```

### Comparing `skye-0.0.1/skye/utils.py` & `skye-0.0.2/skye/utils.py`

 * *Files identical despite different names*

### Comparing `skye-0.0.1/skye.egg-info/PKG-INFO` & `skye-0.0.2/skye.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skye
-Version: 0.0.1
+Version: 0.0.2
 Summary: 360-degree image analysis for forest ecology
 Home-page: https://github.com/iosefa/skye
 Author: Iosefa Percival
 Author-email: ipercival@gmail.com
 Project-URL: Bug Tracker, https://github.com/iosefa/skye/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,9 +13,12 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SKYE
 
 Skye is a simple python library for working with 360-degree photos for analysis in forest ecology.
 
+_This library is currently experimental and is under heavy development_.
+
 Current features include the ability to create hemispherical photographs from 3-band (RGB) 360-degree photos, 
 sky object detection, and the calculation of the sky view factor.
+
```

