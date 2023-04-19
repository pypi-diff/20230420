# Comparing `tmp/dreifus-0.0.5.tar.gz` & `tmp/dreifus-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/dreifus/dist/.tmp-36f1wxmx/dreifus-0.0.5.tar", last modified: Tue Apr 11 22:04:55 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/dreifus/dist/.tmp-9t5ppmgm/dreifus-0.0.6.tar", last modified: Wed Apr 19 23:40:52 2023, max compression
```

## Comparing `dreifus-0.0.5.tar` & `dreifus-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:55.000000 dreifus-0.0.5/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-04-11 22:04:55.000000 dreifus-0.0.5/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       10 2023-02-13 11:32:40.000000 dreifus-0.0.5/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1087 2023-04-11 22:01:51.000000 dreifus-0.0.5/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       38 2023-04-11 22:04:55.000000 dreifus-0.0.5/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      151 2023-02-13 09:12:52.000000 dreifus-0.0.5/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:54.000000 dreifus-0.0.5/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:54.000000 dreifus-0.0.5/src/dreifus/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 08:09:12.000000 dreifus-0.0.5/src/dreifus/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5520 2023-04-11 17:10:32.000000 dreifus-0.0.5/src/dreifus/camera.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5078 2023-04-11 17:41:05.000000 dreifus-0.0.5/src/dreifus/camera_bundle.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1483 2023-02-24 11:10:52.000000 dreifus-0.0.5/src/dreifus/graphics.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:55.000000 dreifus-0.0.5/src/dreifus/matrix/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      251 2023-04-11 16:52:12.000000 dreifus-0.0.5/src/dreifus/matrix/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5852 2023-02-23 11:03:29.000000 dreifus-0.0.5/src/dreifus/matrix/intrinsics_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3655 2023-02-13 10:22:40.000000 dreifus-0.0.5/src/dreifus/matrix/intrinsics_torch.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1315 2023-02-13 11:10:42.000000 dreifus-0.0.5/src/dreifus/matrix/pose_base.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    17272 2023-04-11 17:19:43.000000 dreifus-0.0.5/src/dreifus/matrix/pose_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13757 2023-02-13 11:30:59.000000 dreifus-0.0.5/src/dreifus/matrix/pose_torch.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1329 2023-03-08 15:24:39.000000 dreifus-0.0.5/src/dreifus/matrix/transform_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     9337 2023-04-11 17:36:08.000000 dreifus-0.0.5/src/dreifus/pyvista.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3367 2023-02-24 12:49:30.000000 dreifus-0.0.5/src/dreifus/trajectory.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:55.000000 dreifus-0.0.5/src/dreifus/util/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 10:08:11.000000 dreifus-0.0.5/src/dreifus/util/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      274 2023-02-13 10:10:21.000000 dreifus-0.0.5/src/dreifus/util/typing.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:55.000000 dreifus-0.0.5/src/dreifus/vector/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      219 2023-02-13 13:27:37.000000 dreifus-0.0.5/src/dreifus/vector/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2078 2023-02-13 13:27:37.000000 dreifus-0.0.5/src/dreifus/vector/vector_base.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5371 2023-04-11 15:56:31.000000 dreifus-0.0.5/src/dreifus/vector/vector_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2340 2023-02-13 09:58:17.000000 dreifus-0.0.5/src/dreifus/vector/vector_torch.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:54.000000 dreifus-0.0.5/src/dreifus.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-04-11 22:04:53.000000 dreifus-0.0.5/src/dreifus.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      873 2023-04-11 22:04:54.000000 dreifus-0.0.5/src/dreifus.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-04-11 22:04:53.000000 dreifus-0.0.5/src/dreifus.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       63 2023-04-11 22:04:53.000000 dreifus-0.0.5/src/dreifus.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        8 2023-04-11 22:04:53.000000 dreifus-0.0.5/src/dreifus.egg-info/top_level.txt
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-11 22:04:55.000000 dreifus-0.0.5/test/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1165 2023-02-13 14:36:25.000000 dreifus-0.0.5/test/test_camera.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1439 2023-02-13 10:23:32.000000 dreifus-0.0.5/test/test_intrinsics.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3487 2023-02-13 15:28:18.000000 dreifus-0.0.5/test/test_pose.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3677 2023-02-13 11:26:58.000000 dreifus-0.0.5/test/test_vector.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:52.000000 dreifus-0.0.6/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-04-19 23:40:52.000000 dreifus-0.0.6/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       10 2023-02-13 11:32:40.000000 dreifus-0.0.6/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1087 2023-04-19 23:39:41.000000 dreifus-0.0.6/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       38 2023-04-19 23:40:52.000000 dreifus-0.0.6/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      151 2023-02-13 09:12:52.000000 dreifus-0.0.6/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:50.000000 dreifus-0.0.6/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:51.000000 dreifus-0.0.6/src/dreifus/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 08:09:12.000000 dreifus-0.0.6/src/dreifus/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5520 2023-04-11 17:10:32.000000 dreifus-0.0.6/src/dreifus/camera.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5078 2023-04-11 17:41:05.000000 dreifus-0.0.6/src/dreifus/camera_bundle.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1483 2023-02-24 11:10:52.000000 dreifus-0.0.6/src/dreifus/graphics.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:51.000000 dreifus-0.0.6/src/dreifus/matrix/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      251 2023-04-11 16:52:12.000000 dreifus-0.0.6/src/dreifus/matrix/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5852 2023-02-23 11:03:29.000000 dreifus-0.0.6/src/dreifus/matrix/intrinsics_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3655 2023-02-13 10:22:40.000000 dreifus-0.0.6/src/dreifus/matrix/intrinsics_torch.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1315 2023-02-13 11:10:42.000000 dreifus-0.0.6/src/dreifus/matrix/pose_base.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    17557 2023-04-19 21:54:10.000000 dreifus-0.0.6/src/dreifus/matrix/pose_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13757 2023-02-13 11:30:59.000000 dreifus-0.0.6/src/dreifus/matrix/pose_torch.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1329 2023-03-08 15:24:39.000000 dreifus-0.0.6/src/dreifus/matrix/transform_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     9414 2023-04-19 22:07:01.000000 dreifus-0.0.6/src/dreifus/pyvista.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3367 2023-02-24 12:49:30.000000 dreifus-0.0.6/src/dreifus/trajectory.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:51.000000 dreifus-0.0.6/src/dreifus/util/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 10:08:11.000000 dreifus-0.0.6/src/dreifus/util/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      274 2023-02-13 10:10:21.000000 dreifus-0.0.6/src/dreifus/util/typing.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:52.000000 dreifus-0.0.6/src/dreifus/vector/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      219 2023-02-13 13:27:37.000000 dreifus-0.0.6/src/dreifus/vector/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2078 2023-02-13 13:27:37.000000 dreifus-0.0.6/src/dreifus/vector/vector_base.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5371 2023-04-11 15:56:31.000000 dreifus-0.0.6/src/dreifus/vector/vector_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2340 2023-02-13 09:58:17.000000 dreifus-0.0.6/src/dreifus/vector/vector_torch.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:51.000000 dreifus-0.0.6/src/dreifus.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-04-19 23:40:50.000000 dreifus-0.0.6/src/dreifus.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      873 2023-04-19 23:40:50.000000 dreifus-0.0.6/src/dreifus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-04-19 23:40:50.000000 dreifus-0.0.6/src/dreifus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       63 2023-04-19 23:40:50.000000 dreifus-0.0.6/src/dreifus.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        8 2023-04-19 23:40:50.000000 dreifus-0.0.6/src/dreifus.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:52.000000 dreifus-0.0.6/test/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1165 2023-02-13 14:36:25.000000 dreifus-0.0.6/test/test_camera.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1439 2023-02-13 10:23:32.000000 dreifus-0.0.6/test/test_intrinsics.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3487 2023-02-13 15:28:18.000000 dreifus-0.0.6/test/test_pose.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3677 2023-02-13 11:26:58.000000 dreifus-0.0.6/test/test_vector.py
```

### Comparing `dreifus-0.0.5/pyproject.toml` & `dreifus-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dreifus"
-version = "0.0.5"
+version = "0.0.6"
 description = "dreifus lifts your 3D camera experience and facilitates computer vision applications"
 authors = [
     { name = "Tobias Kirschstein", email = "tobias.kirschstein@gmail.com" },
 ]
 readme = "README.md"
 license = { text = "Apache 2.0" }
 requires-python = ">=3.8.0"
```

### Comparing `dreifus-0.0.5/src/dreifus/camera.py` & `dreifus-0.0.6/src/dreifus/camera.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/src/dreifus/camera_bundle.py` & `dreifus-0.0.6/src/dreifus/camera_bundle.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/src/dreifus/graphics.py` & `dreifus-0.0.6/src/dreifus/graphics.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/src/dreifus/matrix/intrinsics_numpy.py` & `dreifus-0.0.6/src/dreifus/matrix/intrinsics_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/src/dreifus/matrix/intrinsics_torch.py` & `dreifus-0.0.6/src/dreifus/matrix/intrinsics_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/src/dreifus/matrix/pose_base.py` & `dreifus-0.0.6/src/dreifus/matrix/pose_base.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/src/dreifus/matrix/pose_numpy.py` & `dreifus-0.0.6/src/dreifus/matrix/pose_numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,31 +105,40 @@
     def get_rodriguez_vector(self) -> Vec3:
         return Vec3(cv2.Rodrigues(self.get_rotation_matrix())[0].squeeze())
 
     def get_quaternion(self) -> Vec4:
         return Vec4(R.from_matrix(self.get_rotation_matrix()).as_quat())
 
     def get_translation(self) -> Vec3:
-        assert self.pose_type == PoseType.CAM_2_WORLD, "camera position only makes sense for CAM_2_WORLD poses"
+        # assert self.pose_type == PoseType.CAM_2_WORLD, "camera position only makes sense for CAM_2_WORLD poses"
         return Vec3(self[:3, 3])
 
     def set_translation(self, x: Vec3TypeX, y: Optional[FloatType] = None, z: Optional[FloatType] = None):
         x, y, z = unpack_3d_params(x, y, z)
         if x is not None:
             self[0, 3] = x
         if y is not None:
             self[1, 3] = y
         if z is not None:
             self[2, 3] = z
 
-    def move(self, x: Optional[Vec3TypeX] = None, y: Optional[FloatType] = None, z: Optional[FloatType] = None):
+    def move(self, x: Optional[Vec3TypeX] = None, y: Optional[FloatType] = None, z: Optional[FloatType] = None,
+             inplace: bool = True) -> 'Pose':
         x, y, z = unpack_3d_params(x, y, z, 0)
-        self[0, 3] += x
-        self[1, 3] += y
-        self[2, 3] += z
+
+        if inplace:
+            pose = self
+        else:
+            pose = self.copy()
+
+        pose[0, 3] += x
+        pose[1, 3] += y
+        pose[2, 3] += z
+
+        return pose
 
     def scale(self, scale: float) -> 'Pose':
         self[:3, 3] *= scale
         return self
 
     def set_rotation_matrix(self, rotation_matrix: np.ndarray):
         assert is_rotation_matrix(rotation_matrix), \
@@ -221,14 +230,17 @@
                 if a[0] == '-':
                     # Axis shall be flipped
                     v = -1
 
             axis_switcher[idx, ax] = v
         axis_switcher[3, 3] = 1
 
+        if np.abs(np.linalg.det(axis_switcher) - 1) > 1e-6:
+            print("[WARNING] swap_axis changes handedness!")
+
         # Negates / Flips rows
         pose[:, :] = axis_switcher @ pose
 
         return pose
 
     def change_camera_coordinate_convention(self,
                                             new_camera_coordinate_convention: CameraCoordinateConvention,
@@ -287,15 +299,15 @@
         # Assumes an OpenCV camera coordinate system convention (x -> right, y -> down, z -> forward)
 
         assert self.pose_type == PoseType.CAM_2_WORLD
         up_direction = self.camera_coordinate_convention.up_direction
         axis = up_direction.axis_id
         sign = up_direction.sign()
 
-        up_direction = sign * Vec3(self[:3, up_direction])
+        up_direction = sign * Vec3(self[:3, axis])
 
         return up_direction
 
     def look_at(self, at: Vec3, up: Vec3 = Vec3(0, 0, 1)):
         # This method assigns meaning to the coordinate axes. Hence, the coordinate system convention is important
         # We use the OpenCV camera coordinate system convention
```

### Comparing `dreifus-0.0.5/src/dreifus/matrix/pose_torch.py` & `dreifus-0.0.6/src/dreifus/matrix/pose_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/src/dreifus/matrix/transform_numpy.py` & `dreifus-0.0.6/src/dreifus/matrix/transform_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/src/dreifus/pyvista.py` & `dreifus-0.0.6/src/dreifus/pyvista.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                        label: Optional[Union[str, int]] = None,
                        line_width: float = 1,
                        look_vector_length: float = 0):
 
     if pose.pose_type == PoseType.WORLD_2_CAM:
         pose = pose.invert()
 
-    pose = pose.change_camera_coordinate_convention(CameraCoordinateConvention.OPEN_CV)
+    pose = pose.change_camera_coordinate_convention(CameraCoordinateConvention.OPEN_CV, inplace=False)
 
     assert pose.pose_type == PoseType.CAM_2_WORLD
     assert pose.camera_coordinate_convention == CameraCoordinateConvention.OPEN_CV
 
     center = pose.get_translation()
 
     depth = size * pose.camera_coordinate_convention.forward_direction.sign()
@@ -210,32 +210,32 @@
     if label is not None:
         p_center = center
         # (p_top_left + 0.5 * (p_bottom_right - p_top_left))[:3]
         p.add_point_labels([p_center], [label],
                            fill_shape=False, shape=None, show_points=False, text_color=color)
 
 
-def add_coordinate_system(p: pv.Plotter, cam_to_world: Pose):
+def add_coordinate_system(p: pv.Plotter, cam_to_world: Pose, scale: float = 1, line_width: float = 1):
     axis_color_map = {
         0: 'r',
         1: 'g',
         2: 'b'
     }
 
     origin = cam_to_world.get_translation()
-    px = Vec4(1, 0, 0, 1)
-    py = Vec4(0, 1, 0, 1)
-    pz = Vec4(0, 0, 1, 1)
+    px = Vec4(scale, 0, 0, 1)
+    py = Vec4(0, scale, 0, 1)
+    pz = Vec4(0, 0, scale, 1)
 
     points = np.stack([px, py, pz])
     points_world = (cam_to_world @ points.T).T
 
     for i_point, point_world in enumerate(points_world):
         color = axis_color_map[i_point]
-        p.add_lines(np.array([origin, point_world[:3]]), width=1, color=color)
+        p.add_lines(np.array([origin, point_world[:3]]), width=line_width, color=color)
 
 
 def set_camera(p: pv.Plotter, cam_to_world: Pose, neg_z_forward: bool = False):
     look_direction = cam_to_world.get_look_direction()
     up_direction = cam_to_world.get_up_direction()
     if neg_z_forward:
         look_direction *= -1
```

### Comparing `dreifus-0.0.5/src/dreifus/trajectory.py` & `dreifus-0.0.6/src/dreifus/trajectory.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/src/dreifus/vector/vector_base.py` & `dreifus-0.0.6/src/dreifus/vector/vector_base.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/src/dreifus/vector/vector_numpy.py` & `dreifus-0.0.6/src/dreifus/vector/vector_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/src/dreifus/vector/vector_torch.py` & `dreifus-0.0.6/src/dreifus/vector/vector_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/src/dreifus.egg-info/SOURCES.txt` & `dreifus-0.0.6/src/dreifus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/test/test_camera.py` & `dreifus-0.0.6/test/test_camera.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/test/test_intrinsics.py` & `dreifus-0.0.6/test/test_intrinsics.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/test/test_pose.py` & `dreifus-0.0.6/test/test_pose.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.5/test/test_vector.py` & `dreifus-0.0.6/test/test_vector.py`

 * *Files identical despite different names*

