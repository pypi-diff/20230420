# Comparing `tmp/pytorch_volumetric-0.3.6.tar.gz` & `tmp/pytorch_volumetric-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_volumetric-0.3.6.tar", last modified: Fri Mar 17 23:31:27 2023, max compression
+gzip compressed data, was "pytorch_volumetric-0.3.7.tar", last modified: Thu Apr 20 20:38:24 2023, max compression
```

## Comparing `pytorch_volumetric-0.3.6.tar` & `pytorch_volumetric-0.3.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-03-17 23:31:27.017518 pytorch_volumetric-0.3.6/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1075 2023-02-10 04:07:46.000000 pytorch_volumetric-0.3.6/LICENSE.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7155 2023-03-17 23:31:27.013518 pytorch_volumetric-0.3.6/PKG-INFO
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     5064 2023-02-22 01:45:32.000000 pytorch_volumetric-0.3.6/README.md
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4233 2023-03-17 23:31:09.000000 pytorch_volumetric-0.3.6/pyproject.toml
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       38 2023-03-17 23:31:27.017518 pytorch_volumetric-0.3.6/setup.cfg
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-03-17 23:31:27.013518 pytorch_volumetric-0.3.6/src/
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-03-17 23:31:27.013518 pytorch_volumetric-0.3.6/src/pytorch_volumetric/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      562 2023-03-14 20:02:26.000000 pytorch_volumetric-0.3.6/src/pytorch_volumetric/__init__.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3274 2023-02-11 01:35:14.000000 pytorch_volumetric-0.3.6/src/pytorch_volumetric/chamfer.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     6714 2023-03-14 19:47:32.000000 pytorch_volumetric-0.3.6/src/pytorch_volumetric/model_to_sdf.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    25938 2023-03-17 23:30:28.000000 pytorch_volumetric-0.3.6/src/pytorch_volumetric/sdf.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3180 2023-03-14 20:00:04.000000 pytorch_volumetric-0.3.6/src/pytorch_volumetric/visualization.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4419 2023-01-14 21:17:50.000000 pytorch_volumetric-0.3.6/src/pytorch_volumetric/voxel.py
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-03-17 23:31:27.013518 pytorch_volumetric-0.3.6/src/pytorch_volumetric.egg-info/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7155 2023-03-17 23:31:27.000000 pytorch_volumetric-0.3.6/src/pytorch_volumetric.egg-info/PKG-INFO
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      520 2023-03-17 23:31:27.000000 pytorch_volumetric-0.3.6/src/pytorch_volumetric.egg-info/SOURCES.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        1 2023-03-17 23:31:27.000000 pytorch_volumetric-0.3.6/src/pytorch_volumetric.egg-info/dependency_links.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      109 2023-03-17 23:31:27.000000 pytorch_volumetric-0.3.6/src/pytorch_volumetric.egg-info/requires.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       19 2023-03-17 23:31:27.000000 pytorch_volumetric-0.3.6/src/pytorch_volumetric.egg-info/top_level.txt
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-03-17 23:31:27.013518 pytorch_volumetric-0.3.6/tests/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     9487 2023-03-17 23:28:54.000000 pytorch_volumetric-0.3.6/tests/test_model_to_sdf.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     2627 2023-03-17 21:24:34.000000 pytorch_volumetric-0.3.6/tests/test_sdf.py
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-04-20 20:38:24.085832 pytorch_volumetric-0.3.7/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1075 2023-02-10 04:07:46.000000 pytorch_volumetric-0.3.7/LICENSE.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7155 2023-04-20 20:38:24.085832 pytorch_volumetric-0.3.7/PKG-INFO
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     5064 2023-02-22 01:45:32.000000 pytorch_volumetric-0.3.7/README.md
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4233 2023-04-20 20:37:47.000000 pytorch_volumetric-0.3.7/pyproject.toml
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       38 2023-04-20 20:38:24.085832 pytorch_volumetric-0.3.7/setup.cfg
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-04-20 20:38:24.085832 pytorch_volumetric-0.3.7/src/
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-04-20 20:38:24.085832 pytorch_volumetric-0.3.7/src/pytorch_volumetric/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      582 2023-03-23 00:20:25.000000 pytorch_volumetric-0.3.7/src/pytorch_volumetric/__init__.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7181 2023-03-25 03:41:15.000000 pytorch_volumetric-0.3.7/src/pytorch_volumetric/chamfer.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     6714 2023-03-14 19:47:32.000000 pytorch_volumetric-0.3.7/src/pytorch_volumetric/model_to_sdf.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    25938 2023-03-17 23:30:28.000000 pytorch_volumetric-0.3.7/src/pytorch_volumetric/sdf.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3180 2023-03-14 20:00:04.000000 pytorch_volumetric-0.3.7/src/pytorch_volumetric/visualization.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4515 2023-03-25 02:57:41.000000 pytorch_volumetric-0.3.7/src/pytorch_volumetric/voxel.py
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-04-20 20:38:24.085832 pytorch_volumetric-0.3.7/src/pytorch_volumetric.egg-info/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7155 2023-04-20 20:38:24.000000 pytorch_volumetric-0.3.7/src/pytorch_volumetric.egg-info/PKG-INFO
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      542 2023-04-20 20:38:24.000000 pytorch_volumetric-0.3.7/src/pytorch_volumetric.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        1 2023-04-20 20:38:24.000000 pytorch_volumetric-0.3.7/src/pytorch_volumetric.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      109 2023-04-20 20:38:24.000000 pytorch_volumetric-0.3.7/src/pytorch_volumetric.egg-info/requires.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       19 2023-04-20 20:38:24.000000 pytorch_volumetric-0.3.7/src/pytorch_volumetric.egg-info/top_level.txt
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-04-20 20:38:24.085832 pytorch_volumetric-0.3.7/tests/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     5867 2023-03-23 22:59:15.000000 pytorch_volumetric-0.3.7/tests/test_chamfer.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     9487 2023-03-17 23:28:54.000000 pytorch_volumetric-0.3.7/tests/test_model_to_sdf.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     2627 2023-03-17 21:24:34.000000 pytorch_volumetric-0.3.7/tests/test_sdf.py
```

### Comparing `pytorch_volumetric-0.3.6/LICENSE.txt` & `pytorch_volumetric-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytorch_volumetric-0.3.6/PKG-INFO` & `pytorch_volumetric-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch_volumetric
-Version: 0.3.6
+Version: 0.3.7
 Summary: Volumetric structures such as voxels and SDFs implemented in pytorch
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 University of Michigan ARM Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `pytorch_volumetric-0.3.6/README.md` & `pytorch_volumetric-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pytorch_volumetric-0.3.6/pyproject.toml` & `pytorch_volumetric-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytorch_volumetric"
-version = "0.3.6"
+version = "0.3.7"
 description = "Volumetric structures such as voxels and SDFs implemented in pytorch"
 readme = "README.md" # Optional
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
```

### Comparing `pytorch_volumetric-0.3.6/src/pytorch_volumetric/__init__.py` & `pytorch_volumetric-0.3.7/src/pytorch_volumetric/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-from pytorch_volumetric.chamfer import batch_chamfer_dist
+from pytorch_volumetric.chamfer import batch_chamfer_dist, PlausibleDiversity
 from pytorch_volumetric.sdf import sample_mesh_points, ObjectFrameSDF, MeshSDF, CachedSDF, ComposedSDF, SDFQuery, \
     ObjectFactory, MeshObjectFactory
 from pytorch_volumetric.voxel import Voxels, VoxelGrid, VoxelSet, ExpandingVoxelGrid, get_divisible_range_by_resolution, \
     get_coordinates_and_points_in_grid
 from pytorch_volumetric.model_to_sdf import RobotSDF, cache_link_sdf_factory, aabb_to_ordered_end_points
 from pytorch_volumetric.visualization import draw_sdf_slice, get_transformed_meshes
```

### Comparing `pytorch_volumetric-0.3.6/src/pytorch_volumetric/model_to_sdf.py` & `pytorch_volumetric-0.3.7/src/pytorch_volumetric/model_to_sdf.py`

 * *Files identical despite different names*

### Comparing `pytorch_volumetric-0.3.6/src/pytorch_volumetric/sdf.py` & `pytorch_volumetric-0.3.7/src/pytorch_volumetric/sdf.py`

 * *Files identical despite different names*

### Comparing `pytorch_volumetric-0.3.6/src/pytorch_volumetric/visualization.py` & `pytorch_volumetric-0.3.7/src/pytorch_volumetric/visualization.py`

 * *Files identical despite different names*

### Comparing `pytorch_volumetric-0.3.6/src/pytorch_volumetric/voxel.py` & `pytorch_volumetric-0.3.7/src/pytorch_volumetric/voxel.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,31 +76,32 @@
 
     def __setitem__(self, pts, value):
         self.voxels[pts] = value
 
 
 class ExpandingVoxelGrid(VoxelGrid):
     def __setitem__(self, pts, value):
-        # if this query goes outside the range, expand the range in increments of the resolution
-        min = pts.min(dim=0).values
-        max = pts.max(dim=0).values
-        range_per_dim = copy.deepcopy(self.range_per_dim)
-        for dim in range(len(min)):
-            over = (max[dim] - self.range_per_dim[dim][1]).item()
-            under = (self.range_per_dim[dim][0] - min[dim]).item()
-            # adjust in increments of resolution
-            if over > 0:
-                range_per_dim[dim][1] += math.ceil(over / self.resolution) * self.resolution
-            if under > 0:
-                range_per_dim[dim][0] -= math.ceil(under / self.resolution) * self.resolution
-        if not np.allclose(range_per_dim, self.range_per_dim):
-            # transfer over values
-            known_pos, known_values = self.get_known_pos_and_values()
-            self._create_voxels(self.resolution, range_per_dim)
-            super().__setitem__(known_pos, known_values)
+        if pts.numel() > 0:
+            # if this query goes outside the range, expand the range in increments of the resolution
+            min = pts.min(dim=0).values
+            max = pts.max(dim=0).values
+            range_per_dim = copy.deepcopy(self.range_per_dim)
+            for dim in range(len(min)):
+                over = (max[dim] - self.range_per_dim[dim][1]).item()
+                under = (self.range_per_dim[dim][0] - min[dim]).item()
+                # adjust in increments of resolution
+                if over > 0:
+                    range_per_dim[dim][1] += math.ceil(over / self.resolution) * self.resolution
+                if under > 0:
+                    range_per_dim[dim][0] -= math.ceil(under / self.resolution) * self.resolution
+            if not np.allclose(range_per_dim, self.range_per_dim):
+                # transfer over values
+                known_pos, known_values = self.get_known_pos_and_values()
+                self._create_voxels(self.resolution, range_per_dim)
+                super().__setitem__(known_pos, known_values)
 
         return super().__setitem__(pts, value)
 
 
 class VoxelSet(Voxels):
     def __init__(self, positions, values):
         self.positions = positions
```

### Comparing `pytorch_volumetric-0.3.6/src/pytorch_volumetric.egg-info/PKG-INFO` & `pytorch_volumetric-0.3.7/src/pytorch_volumetric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-volumetric
-Version: 0.3.6
+Version: 0.3.7
 Summary: Volumetric structures such as voxels and SDFs implemented in pytorch
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 University of Michigan ARM Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `pytorch_volumetric-0.3.6/src/pytorch_volumetric.egg-info/SOURCES.txt` & `pytorch_volumetric-0.3.7/src/pytorch_volumetric.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 src/pytorch_volumetric/visualization.py
 src/pytorch_volumetric/voxel.py
 src/pytorch_volumetric.egg-info/PKG-INFO
 src/pytorch_volumetric.egg-info/SOURCES.txt
 src/pytorch_volumetric.egg-info/dependency_links.txt
 src/pytorch_volumetric.egg-info/requires.txt
 src/pytorch_volumetric.egg-info/top_level.txt
+tests/test_chamfer.py
 tests/test_model_to_sdf.py
 tests/test_sdf.py
```

### Comparing `pytorch_volumetric-0.3.6/tests/test_model_to_sdf.py` & `pytorch_volumetric-0.3.7/tests/test_model_to_sdf.py`

 * *Files identical despite different names*

### Comparing `pytorch_volumetric-0.3.6/tests/test_sdf.py` & `pytorch_volumetric-0.3.7/tests/test_sdf.py`

 * *Files identical despite different names*

