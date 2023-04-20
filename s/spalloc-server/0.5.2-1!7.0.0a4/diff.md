# Comparing `tmp/spalloc_server-0.5.2.tar.gz` & `tmp/spalloc_server-1!7.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spalloc_server-0.5.2.tar", last modified: Mon Aug 22 19:11:43 2016, max compression
+gzip compressed data, was "spalloc_server-1!7.0.0a4.tar", last modified: Wed Apr 19 15:13:53 2023, max compression
```

## Comparing `spalloc_server-0.5.2.tar` & `spalloc_server-1!7.0.0a4.tar`

### file list

```diff
@@ -1,24 +1,46 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2016-08-22 19:11:43.000000 spalloc_server-0.5.2/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1444 2016-08-22 18:43:43.000000 spalloc_server-0.5.2/setup.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      991 2016-08-22 19:11:43.000000 spalloc_server-0.5.2/PKG-INFO
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2016-08-22 19:11:43.000000 spalloc_server-0.5.2/spalloc_server/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    14028 2016-02-18 12:41:22.000000 spalloc_server-0.5.2/spalloc_server/pack_tree.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    19710 2016-02-24 09:31:51.000000 spalloc_server-0.5.2/spalloc_server/job_queue.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    41412 2016-07-18 11:56:03.000000 spalloc_server-0.5.2/spalloc_server/server.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    11052 2016-05-10 11:02:38.000000 spalloc_server-0.5.2/spalloc_server/async_bmp_controller.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    49373 2016-07-18 11:56:03.000000 spalloc_server-0.5.2/spalloc_server/controller.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     9323 2016-02-24 16:53:34.000000 spalloc_server-0.5.2/spalloc_server/coordinates.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    21148 2016-02-24 14:35:56.000000 spalloc_server-0.5.2/spalloc_server/configuration.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       22 2016-08-22 19:10:23.000000 spalloc_server-0.5.2/spalloc_server/version.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    42815 2016-02-24 09:27:41.000000 spalloc_server-0.5.2/spalloc_server/allocator.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5257 2016-02-18 12:45:23.000000 spalloc_server-0.5.2/spalloc_server/area_to_rect.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       47 2016-02-14 17:47:17.000000 spalloc_server-0.5.2/spalloc_server/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1335 2016-08-22 18:42:42.000000 spalloc_server-0.5.2/README.rst
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2016-08-22 19:11:43.000000 spalloc_server-0.5.2/spalloc_server.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      991 2016-08-22 19:11:42.000000 spalloc_server-0.5.2/spalloc_server.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      107 2016-08-22 19:11:42.000000 spalloc_server-0.5.2/spalloc_server.egg-info/entry_points.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       40 2016-08-22 19:11:42.000000 spalloc_server-0.5.2/spalloc_server.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      572 2016-08-22 19:11:43.000000 spalloc_server-0.5.2/spalloc_server.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       15 2016-08-22 19:11:42.000000 spalloc_server-0.5.2/spalloc_server.egg-info/top_level.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2016-08-22 19:11:42.000000 spalloc_server-0.5.2/spalloc_server.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       59 2016-08-22 19:11:43.000000 spalloc_server-0.5.2/setup.cfg
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-19 15:13:53.083365 spalloc_server-1!7.0.0a4/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5082 2023-03-10 13:05:58.000000 spalloc_server-1!7.0.0a4/CITATION.cff
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    11360 2023-04-17 09:36:59.000000 spalloc_server-1!7.0.0a4/LICENSE
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      967 2023-03-10 13:05:58.000000 spalloc_server-1!7.0.0a4/LICENSE_POLICY.md
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       74 2023-04-11 11:02:16.000000 spalloc_server-1!7.0.0a4/MANIFEST.in
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2587 2023-04-19 15:13:53.083365 spalloc_server-1!7.0.0a4/PKG-INFO
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1406 2023-03-10 13:05:58.000000 spalloc_server-1!7.0.0a4/README.rst
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      678 2023-04-18 10:28:23.000000 spalloc_server-1!7.0.0a4/pyproject.toml
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1513 2023-04-19 15:13:53.083365 spalloc_server-1!7.0.0a4/setup.cfg
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1316 2023-04-11 11:05:20.000000 spalloc_server-1!7.0.0a4/setup.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-19 15:13:53.079365 spalloc_server-1!7.0.0a4/spalloc_server/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      660 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a4/spalloc_server/__init__.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      735 2023-04-19 15:13:49.000000 spalloc_server-1!7.0.0a4/spalloc_server/_version.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    45607 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a4/spalloc_server/allocator.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5891 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a4/spalloc_server/area_to_rect.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    12605 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a4/spalloc_server/async_bmp_controller.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    22151 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a4/spalloc_server/configuration.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5164 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a4/spalloc_server/configuration_reloader.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    58141 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a4/spalloc_server/controller.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     9919 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a4/spalloc_server/coordinates.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    21347 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a4/spalloc_server/job_queue.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5478 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a4/spalloc_server/links.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    14536 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a4/spalloc_server/pack_tree.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5178 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a4/spalloc_server/polling_server_core.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    45502 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a4/spalloc_server/server.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-19 15:13:53.079365 spalloc_server-1!7.0.0a4/spalloc_server.egg-info/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2587 2023-04-19 15:13:53.000000 spalloc_server-1!7.0.0a4/spalloc_server.egg-info/PKG-INFO
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1098 2023-04-19 15:13:53.000000 spalloc_server-1!7.0.0a4/spalloc_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-04-19 15:13:53.000000 spalloc_server-1!7.0.0a4/spalloc_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      106 2023-04-19 15:13:53.000000 spalloc_server-1!7.0.0a4/spalloc_server.egg-info/entry_points.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       65 2023-04-19 15:13:53.000000 spalloc_server-1!7.0.0a4/spalloc_server.egg-info/requires.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       15 2023-04-19 15:13:53.000000 spalloc_server-1!7.0.0a4/spalloc_server.egg-info/top_level.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-04-19 15:13:52.000000 spalloc_server-1!7.0.0a4/spalloc_server.egg-info/zip-safe
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-19 15:13:53.083365 spalloc_server-1!7.0.0a4/tests/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    33475 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a4/tests/test_allocator.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5859 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a4/tests/test_area_to_rect.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    11980 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a4/tests/test_async_bmp_controller.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    10633 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a4/tests/test_configuration.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    44669 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a4/tests/test_controller.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5331 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a4/tests/test_coordinates.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1069 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a4/tests/test_import_all.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    17782 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a4/tests/test_job_queue.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3198 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a4/tests/test_links.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    22346 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a4/tests/test_pack_tree.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1251 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a4/tests/test_polling_server_core.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    34764 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a4/tests/test_server.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spalloc_server-0.5.2/spalloc_server/pack_tree.py` & `spalloc_server-1!7.0.0a4/spalloc_server/pack_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,43 @@
-"""An algorithm/datastructure for allocating/packing rectangles into a fixed 2D
-space.
-
-This algorithm is used to allocate triads of boards in SpiNNaker systems but is
-otherwise a relatively generic 2D packing algorithm.
-"""
+# Copyright (c) 2016 The University of Manchester
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
+""" An algorithm/datastructure for allocating/packing rectangles into a fixed\
+    2D space.
 
-from spalloc_server.area_to_rect import area_to_rect
+This algorithm is used to allocate triads of boards in SpiNNaker systems but\
+is otherwise a relatively generic 2D packing algorithm.
+"""
+from .area_to_rect import area_to_rect
 
 
 class PackTree(object):
-    r"""A tree-based datastructure for allocating/packing rectangles into a
+    r""" A tree-based datastructure for allocating/packing rectangles into a
     fixed 2D space.
 
     This tree structure is used to allocate/pack rectangular subregions of
     SpiNNaker machine in a fashion similar to `this lightmap packing algorithm
-    <http://www.blackpawn.com/texts/lightmaps/default.html>`_. It is certainly
+    <https://www.blackpawn.com/texts/lightmaps/default.html>`_. It is certainly
     not the most efficient or flexible packing algorithm available but due to
     time constraints it is ideal due to its simplicity.
     """
 
     def __init__(self, x, y, width, height):
-        """Defines a region of which may be allocated and/or divided in two.
+        """ Defines a region of which may be allocated and/or divided in two.
 
         Parameters
         ----------
         x, y : int
             The (absolute) location of the bottom left corner of the region.
         width, height : int
             The dimensions of the region.
@@ -40,42 +52,41 @@
         self.allocated = False
 
         # Either None (leaf node) or a pair (PackTree, PackTree) giving the
         # children of this node.
         self.children = None
 
     def __contains__(self, xy):
-        """Test whether a coordinate is inside this region."""
+        """ Test whether a coordinate is inside this region."""
         x, y = xy
         return (self.x <= x < (self.x + self.width) and
                 self.y <= y < (self.y + self.height))
 
     def hsplit(self, y):
-        """Split this node along the X axis.
+        """ Split this node along the X axis.
 
         The bottom half of split will be just before the "y" position.
 
         ::
 
                +-----------+
                |           |
             ---+-----------+---
                |           |
                +-----------+
         """
         assert self.children is None
         assert not self.allocated
 
-        self.children = (PackTree(self.x, self.y,
-                                  self.width, (y - self.y)),
-                         PackTree(self.x, y,
-                                  self.width, self.height - (y - self.y)))
+        self.children = (
+            PackTree(self.x, self.y, self.width, (y - self.y)),
+            PackTree(self.x, y, self.width, self.height - (y - self.y)))
 
     def vsplit(self, x):
-        """Split this node along the Y axis.
+        """ Split this node along the Y axis.
 
         The left half of split will be just before the "x" position.
 
         ::
 
                   |
             +-----+-----+
@@ -84,21 +95,34 @@
             |     |     |
             +-----+-----+
                   |
         """
         assert self.children is None
         assert not self.allocated
 
-        self.children = (PackTree(self.x, self.y,
-                                  (x - self.x), self.height),
-                         PackTree(x, self.y,
-                                  self.width - (x - self.x), self.height))
+        self.children = (
+            PackTree(self.x, self.y, (x - self.x), self.height),
+            PackTree(x, self.y, self.width - (x - self.x), self.height))
+
+    def _find_acceptable(self, width, height, candidate_filter):
+        tried = set()
+        if candidate_filter is None:
+            # Dummy filter that always accepts a candidate
+            candidate_filter = (lambda _a, _b, _c, _d: True)
+        for x, y in ((self.x + x, self.y + y)
+                     for x in (0, self.width - width)
+                     for y in (0, self.height - height)):
+            key = (x, y)
+            if key not in tried and candidate_filter(x, y, width, height):
+                return key
+            tried.add(key)
+        return None
 
     def alloc(self, width, height, candidate_filter=None):
-        """Attempt to allocate a rectangular region of a specified size.
+        """ Attempt to allocate a rectangular region of a specified size.
 
         Parameters
         ----------
         width, height : int
             The dimensions of the region to attempt to allocate. Must be
             strictly 1x1 or greater.
         candidate_filter : None or function(x, y, w, h) -> bool
@@ -134,32 +158,24 @@
         if self.children is not None:
             # Try the smallest child first
             for child in sorted(self.children,
                                 key=(lambda c: c.width * c.height)):
                 allocation = child.alloc(width, height, candidate_filter)
                 if allocation:
                     return allocation
-            else:
-                # No child could fit the allocation, fail
-                return None
+            # No child could fit the allocation, fail
+            return None
 
         # This node is an empty leaf with enough room. Try and find a corner
         # into which this allocation can fit which is acceptable to the caller.
-        tried = set()
-        for x, y in ((self.x + x, self.y + y)
-                     for x in (0, self.width - width)
-                     for y in (0, self.height - height)):
-            if ((x, y) not in tried and
-                    (candidate_filter is None or
-                     candidate_filter(x, y, width, height))):
-                break
-            tried.add((x, y))
-        else:
+        xy = self._find_acceptable(width, height, candidate_filter)
+        if xy is None:
             # No acceptable subregion could be found, give up.
             return None
+        x, y = xy
 
         # If the region fits exactly, just become allocated
         if width == self.width and height == self.height:
             self.allocated = True
             assert x == self.x and y == self.y  # Sanity check...
             return (self.x, self.y)
 
@@ -193,21 +209,21 @@
         elif child.height != height:
             child.hsplit(y if y != child.y else child.y + height)
             grandchild = (child.children[0]
                           if y == child.y else
                           child.children[1])
             grandchild.allocated = True
             return (grandchild.x, grandchild.y)
-        else:
-            child.allocated = True
-            return (child.x, child.y)
+        child.allocated = True
+        return (child.x, child.y)
 
     def alloc_area(self, area, min_ratio=0.0, candidate_filter=None):
-        """Attempt to allocate a rectangular region with at least the specified
-        area which is 'at least as square' as the specified aspect ratio.
+        """ Attempt to allocate a rectangular region with at least the\
+            specified area which is 'at least as square' as the specified\
+            aspect ratio.
 
         Parameters
         ----------
         area : int
             The *minimum* area to allocate, must be at least 1.
         min_ratio : float
             The aspect ratio which the allocated region must be 'at least as
@@ -243,39 +259,37 @@
 
         # If this node is split (i.e. has children), try inserting into the
         # children.
         if self.children is not None:
             # Try the smallest child first
             for child in sorted(self.children,
                                 key=(lambda c: c.width * c.height)):
-                allocation = child.alloc_area(area, min_ratio,
-                                              candidate_filter)
+                allocation = child.alloc_area(
+                    area, min_ratio, candidate_filter)
                 if allocation:
                     return allocation
-            else:
-                # No child could fit the allocation, fail
-                return None
+            # No child could fit the allocation, fail
+            return None
 
         # This is a child node, try to work out a suitable size for the
         # allocation if possible
         rect = area_to_rect(area, self.width, self.height, min_ratio)
         if not rect:
             return None
 
         # Try allocating that size
         width, height = rect
         allocation = self.alloc(width, height, candidate_filter)
-        if allocation:
-            x, y = allocation
-            return (x, y, width, height)
-        else:
+        if not allocation:
             return None
+        x, y = allocation
+        return (x, y, width, height)
 
     def request(self, x, y):
-        """Request the allocation of a specific 1x1 block.
+        """ Request the allocation of a specific 1x1 block.
 
         This function may be useful when, e.g., specific boards are required
         for testing.
 
         Returns
         -------
         allocation : (x, y) or None
@@ -311,41 +325,38 @@
         # if trying to divvy-up the space to fit something we look for the side
         # with the greatest amount of space on it to divide on first. This
         # procedure is then used recursively to divvy the world up until we
         # have a 1x1 allocation.
         #
         #     +---------------+
         #     |         a     |
-        #     |<---l--->#<-r->|
+        #     |<--_l--->#<-r->|
         #     |         ^     |
         #     |         b     |
         #     |         v     |
         #     +---------------+
-        l = x - self.x
+        _l = x - self.x
         r = (self.x + self.width) - x - 1
         a = (self.y + self.height) - y - 1
         b = y - self.y
 
-        largest = max(l, r, a, b)
+        largest = max(_l, r, a, b)
 
-        if l == largest:
+        if _l == largest:
             self.vsplit(x=x)
-            return self.request(x, y)
         elif r == largest:
             self.vsplit(x=x + 1)
-            return self.request(x, y)
         elif a == largest:
             self.hsplit(y=y + 1)
-            return self.request(x, y)
         else:  # b == largest
             self.hsplit(y=y)
-            return self.request(x, y)
+        return self.request(x, y)
 
     def free(self, x, y):
-        """Free a previous allocation, allowing the space to be reused.
+        """ Free a previous allocation, allowing the space to be reused.
 
         Parameters
         ----------
         x, y : int
             The bottom-left corner of the allocation.
         """
         # If the region to be freed is this one, do so (but only if it is a
@@ -364,18 +375,16 @@
                 child.free(x, y)
 
                 # If both of our children are now empty leaves, we can remove
                 # them and make this node a leaf.
                 if all(not c.allocated and c.children is None
                        for c in self.children):
                     self.children = None
-
                 return
-        else:
-            # No child contains the location to be freed. Crash out!
-            raise FreeError(
-                "Cannot free {}, {} which is outside the region.".format(x, y))
+        # No child contains the location to be freed. Crash out!
+        raise FreeError(
+            "Cannot free {}, {} which is outside the region.".format(x, y))
 
 
 class FreeError(Exception):
-    """Thrown when attempting to free a region fails."""
-    pass
+    """ Thrown when attempting to free a region fails.
+    """
```

### Comparing `spalloc_server-0.5.2/spalloc_server/job_queue.py` & `spalloc_server-1!7.0.0a4/spalloc_server/job_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,30 @@
-"""A multi-machine and job queueing and allocation mechanism.
-"""
+# Copyright (c) 2016 The University of Manchester
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
+""" A multi-machine and job queueing and allocation mechanism.
+"""
 from collections import deque, OrderedDict
-
-from six import itervalues
-
-from spalloc_server.allocator import Allocator
+from .allocator import Allocator
 
 
 class JobQueue(object):
-    """A mechanism for matching incoming allocation requests (jobs) to a set of
-    available machines.
+    """ A mechanism for matching incoming allocation requests (jobs) to a set
+    of available machines.
 
     For every :py:class:`._Machine` being managed this object contains a queue
     of outstanding jobs and an :py:class:`spalloc_server.allocator.Allocator`
     which manages allocation of jobs onto that machine. A simplistic scheduling
     mechanism is used (see :py:meth:`._enqueue_job`) which simultaneously
     enqueues all jobs to every candidate machine the job could possibly fit on.
     The first machine to accept the job is allocated the job (all other
@@ -36,30 +46,32 @@
 
     Once the :py:meth:`.on_allocate` callback has been called for a
     job, a job may be considered to be allocated to the specific machine
     indicated in the callback. This remains true until the :py:meth:`.on_free`
     callback is produced (as a result of calling :py:class:`.destroy_job`).
     """
 
-    def __init__(self, on_allocate, on_free, on_cancel):
-        """Create a new (empty) job queue with no machines.
+    def __init__(self, on_allocate, on_free, on_cancel,
+                 seconds_before_free=30):
+        """ Create a new (empty) job queue with no machines.
 
         Parameters
         ----------
         on_allocate : f(job_id, machine_name, boards, periphery, torus)
             A callback function which is called when a job is successfully
             allocated resources on a machine.
 
             job_id : int
                 The job's unique identifier.
             machine_name : str
                 The name of the machine the job was allocated on.
             boards : set([(x, y, z), ...])
                 Enumerates the boards in the allocation.
-            periphery : set([(x, y, z, :py:class:`rig.links.Links`), ...])
+            periphery : set([(x, y, z,\
+                             :py:class:`spalloc_server.links.Links`), ...])
                 Enumerates the links which leave the set of allocated boards.
             torus : :py:class:`spalloc_server.coordinates.WrapAround`
                 Specifies which types of wrap-around links may be present.
 
         on_free : f(job_id, reason)
             A callback called when a job which was previously allocated
             resources has had those resources withdrawn or freed them.
@@ -76,33 +88,38 @@
             due to user action.
 
             job_id : int
                 The job's unique identifier.
             reason : str or None
                 A human readable string explaining why the job was cancelled or
                 None if no reason was given.
+
+        seconds_before_free : int
+            The number of seconds between a board being freed and it becoming
+            available again
         """
         self.on_allocate = on_allocate
         self.on_free = on_free
         self.on_cancel = on_cancel
+        self.seconds_before_free = seconds_before_free
 
         # The machines onto which jobs may be queued.
         # {name: _Machine, ...}
         self._machines = OrderedDict()
 
         # The currently queued or allocated jobs
         # {job_id: _Job, ...}
         self._jobs = OrderedDict()
 
         # When non-zero, queues are not changed. Set when using this object as
         # a context manager.
         self._postpone_queue_management = 0
 
     def __enter__(self):
-        """This context manager will cause all changes to machines to be made
+        """ This context manager will cause all changes to machines to be made
         atomically, without regenerating queues between each change.
 
         This is useful when modifying multiple machines at once or destroying
         multiple jobs at once since it prevents jobs being allocated and then
         immediately destroyed.
 
         Usage example::
@@ -114,20 +131,20 @@
 
         .. note::
             This context manager should be used sparingly as it causes all
             job queues to be regenerated from scratch when it exits.
         """
         self._postpone_queue_management += 1
 
-    def __exit__(self, type=None, value=None, traceback=None):
+    def __exit__(self, _type=None, _value=None, _traceback=None):
         self._postpone_queue_management -= 1
         self._regenerate_queues()
 
     def __getstate__(self):
-        """Called when pickling this object.
+        """ Called when pickling this object.
 
         In Python 2, references to methods cannot be pickled. Since this
         object maintains a number of function pointers as callbacks (which may
         often be methods) we must remove these before pickling. When
         unpickling, these pointers should be recreated externally.
         """
         state = self.__dict__.copy()
@@ -136,15 +153,15 @@
         state["on_allocate"] = None
         state["on_free"] = None
         state["on_cancel"] = None
 
         return state
 
     def _try_job(self, job, machine):
-        """Attempt to allocate a job on a given machine.
+        """ Attempt to allocate a job on a given machine.
 
         Returns
         -------
         job_allocated : bool
             Was the job successfully allocated? If True, the internal metadata
             associated with the job is updated and the :py:attr:`.on_allocate`
             callback is called.
@@ -162,15 +179,15 @@
 
         # Report this to the user
         self.on_allocate(job.id, machine.name, boards, periphery, torus)
 
         return True
 
     def _enqueue_job(self, job):
-        """Either allocate or enqueue a new job.
+        """ Either allocate or enqueue a new job.
 
         Given a new job which is not yet running or enqueued use a simple
         scheduling mechanism to decided what to do with it:
 
         * Attempt to allocate the job on each machine matching the job's
           requirements in turn.
         * If no machine can allocate the job immediately, add the job to the
@@ -187,16 +204,16 @@
         # Get the list of machines the job would like to be executed on.
         if job.machine_name is not None:
             # A specific machine was given
             machine = self._machines.get(job.machine_name, None)
             machines = [machine] if machine is not None else []
         else:
             # Select machines according to the job's tags
-            machines = [m for m in itervalues(self._machines)
-                        if job.tags.issubset(m.tags)]
+            machines = (m for m in self._machines.values()
+                        if job.tags.issubset(m.tags))
 
         # Queue the job on all suitable machines
         found_machine = False
         for machine in machines:
             if machine.allocator.alloc_possible(*job.args, **job.kwargs):
                 machine.queue.append(job)
                 found_machine = True
@@ -206,63 +223,64 @@
         if not found_machine:
             self.destroy_job(job.id, "No suitable machines available.")
 
         # Advance the queues where possible.
         self._process_queue()
 
     def _process_queue(self):
-        """Try and process any queued jobs."""
+        """ Try and process any queued jobs.
+        """
         if self._postpone_queue_management:
             return
 
         # Keep going until no more jobs can be started
         changed = True
         while changed:
             changed = False
 
             # For each machine, attempt to process the current head of their
             # job queue.
-            for machine in itervalues(self._machines):
+            for machine in self._machines.values():
                 while machine.queue:
                     if not machine.queue[0].pending:
                         # Skip queued jobs which have been allocated
                         # elsewhere/cancelled
                         machine.queue.popleft()
                         continue
                     elif self._try_job(machine.queue[0], machine):
                         # Try running the job
                         machine.queue.popleft()
                         changed = True
 
                     break
 
     def _regenerate_queues(self):
-        """Regenerate all queues to account for any significant changes to the
+        """ Regenerate all queues to account for any significant changes to the
         machines available.
 
         This function clears all machine queues and then reinserts the jobs
         using :py:class:`._enqueue_job`, potentially allocating the job to a
         running machine. Since the jobs are re-enqueued in the order they were
         supplied, the queueing priorities are unaffected.
         """
         if self._postpone_queue_management:
             return
 
         # Empty all job queues
-        for machine in itervalues(self._machines):
+        for machine in self._machines.values():
             machine.queue.clear()
 
         # Re-allocate/queue all pending jobs
-        for job in itervalues(self._jobs):
+        for job in self._jobs.values():
             if job.pending:
                 self._enqueue_job(job)
 
     def add_machine(self, name, width, height, tags=None,
-                    dead_boards=set(), dead_links=set()):
-        """Add a new machine for processing jobs.
+                    dead_boards=frozenset(), dead_links=frozenset()):
+        """ Add a new machine for processing jobs.
 
         Jobs are offered for allocation on machines in the order the machines
         are inserted to this list.
 
         Parameters
         ----------
         name : str
@@ -271,65 +289,66 @@
             The dimensions of the machine in triads.
         tags : set([str, ...])
             The set of tags jobs may select to indicate they wish to use this
             machine. Note that the tag default is given to any job whose
             tags are not otherwise specified. Defaults to set(["default"])
         dead_boards : set([(x, y, z), ...])
             The boards in the machine which do not work.
-        dead_links : set([(x, y, z, :py:class:`rig.links.Links`), ...])
+        dead_links : set([(x, y, z,\
+                          :py:class:`spalloc_server.links.Links`), ...])
             The board-to-board links in the machine which do not work.
 
         See Also
         --------
         __enter__ : A context manager to allow atomic changes to be made to
                     machines.
         move_machine_to_end : Modify machine priorities
         modify_machine : Modify certain machine parameters without removing and
                          then re-adding it.
         remove_machine : Remove a machine.
         """
+        # pylint: disable=too-many-arguments
         if name in self._machines:
             raise ValueError("Machine name {} already in use.".format(name))
 
-        allocator = Allocator(width, height, dead_boards, dead_links)
+        allocator = Allocator(width, height, dead_boards, dead_links,
+                              seconds_before_free=self.seconds_before_free)
         self._machines[name] = _Machine(name, tags, allocator)
 
         self._regenerate_queues()
 
     def move_machine_to_end(self, name):
-        """Move the specified machine to the end of the OrderedDict of
+        """ Move the specified machine to the end of the OrderedDict of
         machines.
 
         Parameters
         ----------
         name : str
             The name of the machine to move.
         """
-        # Python 2.7 does not have move_to_end
-        m = self._machines.pop(name)
-        self._machines[name] = m
-
+        self._machines.move_to_end(name)
         # NB: No queue regeneration required
 
     def modify_machine(self, name, tags=None,
                        dead_boards=None, dead_links=None):
-        """Make minor modifications to the description of an existing machine.
+        """ Make minor modifications to the description of an existing machine.
 
         Note that any changes made will not impact already allocated jobs but
         may alter queued jobs.
 
         Parameters
         ----------
         name : str
             The name of the machine to change.
         tags : set([str, ...]) or None
             If not None, change the Machine's tags to match the supplied set.
         dead_boards : set([(x, y, z), ...])
             If not None, change the set of dead boards in the machine.
-        dead_links : set([(x, y, z, :py:class:`rig.links.Links`), ...])
+        dead_links : set([(x, y, z,\
+                          :py:class:`spalloc_server.links.Links`), ...])
             If not None, change the set of dead links in the machine.
         """
         machine = self._machines[name]
 
         if tags is not None:
             machine.tags = tags
 
@@ -338,33 +357,35 @@
 
         if dead_links is not None:
             machine.allocator.dead_links = dead_links
 
         self._regenerate_queues()
 
     def remove_machine(self, name):
-        """Remove a machine from the available set.
+        """ Remove a machine from the available set.
 
         All jobs allocated on that machine will be freed and then the machine
         will be removed.
         """
         machine = self._machines[name]
 
         # Regenerate the queues only after removing the machine
         with self:
             # Free all jobs allocated on the machine.
-            for job in list(itervalues(self._jobs)):
+            # NB: Copy the list of jobs to avoid concurrent modification
+            for job in list(self._jobs.values()):
                 if job.machine is machine:
                     self.destroy_job(job.id, "Machine removed.")
+                    self.free(job.id)
 
             # Remove the machine from service
             del self._machines[name]
 
     def create_job(self, *args, **kwargs):
-        """Attempt to create a new job.
+        """ Attempt to create a new job.
 
         If no machine is immediately available to allocate the job the job is
         placed in the queues of all machines into which it can fit. The first
         machine to be able to allocate the job will get the job. This means
         that identical jobs are handled in a FIFO fashion but jobs which can
         only be executed on certain machines may be 'overtaken' by jobs which
         can run on machines the overtaken job cannot.
@@ -406,51 +427,69 @@
                 "Only one of machine and tags may be specified for a job.")
 
         # If a specific machine is selected, we must not filter on tags
         if machine_name is not None:
             tags = set()
 
         # Create the job
-        job = _Job(id=job_id, pending=True,
+        job = _Job(_id=job_id, pending=True,
                    machine_name=machine_name, tags=tags,
                    args=args, kwargs=kwargs)
         self._jobs[job.id] = job
         self._enqueue_job(job)
 
     def destroy_job(self, job_id, reason=None):
-        """Destroy a queued or allocated job.
+        """ Destroy a queued or allocated job.
 
         If the job is already allocated, this frees the job resulting in the
         :py:attr:`.on_free` callback being called.  If the job is queued, this
         removes the job from all queues and the :py:attr:`.on_cancel` callback
         being called.
 
         Parameters
         ----------
         job_id : int
             The ID of the job to destroy.
         reason : str or None
             *Optional.* A human-readable reason that the job was destroyed.
         """
-        job = self._jobs.pop(job_id)
+        job = self._jobs.get(job_id)
 
         if job.pending:
             # Mark the job as no longer pending to prevent it being processed
             job.pending = False
             self.on_cancel(job.id, reason)
+            self._jobs.pop(job_id)
         else:
             # Job was allocated somewhere, deallocate it
-            job.machine.allocator.free(job.allocation_id)
             self.on_free(job.id, reason)
 
         self._process_queue()
 
+    def free(self, job_id):
+        if job_id in self._jobs:
+            job = self._jobs.pop(job_id)
+            job.machine.allocator.free(job.allocation_id)
+            self._process_queue()
+
+    def check_free(self):
+        """ Check for freed machines that are now available
+        """
+        if self._postpone_queue_management:
+            return
+        changed = False
+        for machine in self._machines:
+            if self._machines[machine].allocator.check_free():
+                changed = True
+        if changed:
+            self._process_queue()
+
 
 class _Job(object):
-    """The internal state representing a job.
+    """ The internal state representing a job.
 
     Attributes
     ----------
     id : int
         A unique ID assigned to the job.
     pending : bool
         If True, the job is currently queued for execution, if False the job
@@ -464,36 +503,32 @@
     args, kwargs : tuple, dict
         The arguments to the alloc function for this job.
     machine : :py:class:`._Machine` or None
         The machine the job has been allocated on.
     allocation_id : int or None
         The allocation ID for the Job's allocation.
     """
-    def __init__(self, id,
-                 pending=True,
-                 machine_name=None,
-                 tags=set(),
-                 args=tuple(), kwargs={},
-                 machine=None,
-                 allocation_id=None):
-        self.id = id
+    def __init__(self, _id, pending=True, machine_name=None, tags=frozenset(),
+                 args=tuple(), kwargs=None, machine=None, allocation_id=None):
+        # pylint: disable=too-many-arguments
+        self.id = _id
         self.pending = pending
         self.machine_name = machine_name
-        self.tags = tags if tags is not None else set(["default"])
+        self.tags = set(tags if tags is not None else ["default"])
         self.args = args
-        self.kwargs = kwargs
+        self.kwargs = dict({} if kwargs is None else kwargs)
         self.machine = machine
         self.allocation_id = allocation_id
 
     def __repr__(self):  # pragma: no cover
         return "<{} id={}>".format(self.__class__.__name__, self.id)
 
 
 class _Machine(object):
-    """Internal data which maintains state information about machine on which
+    """ Internal data which maintains state information about machine on which
     jobs may run.
 
     Attributes
     ----------
     name : str
         The name of the machine.
     tags : set([str, ...])
```

### Comparing `spalloc_server-0.5.2/spalloc_server/server.py` & `spalloc_server-1!7.0.0a4/spalloc_server/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,509 +1,555 @@
-"""A TCP server which exposes a public interface for allocating boards.
-
-This module is essentially the 'top level' module for the functionality of the
-SpiNNaker Partitioning Server, containing the :py:func:`function <.main>` which
-is mapped to the ``spalloc-server`` command-line tool.
+# Copyright (c) 2016 The University of Manchester
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+""" A TCP server which exposes a public interface for allocating boards.
+
+This module is essentially the 'top level' module for the functionality of the\
+SpiNNaker Partitioning Server, containing the :py:func:`function <.main>`\
+which is mapped to the ``spalloc-server`` command-line tool.
 """
 
-import os
-import os.path
-import logging
-import pickle
-import socket
-import select
-import threading
-import json
-import argparse
-import time
-
+from argparse import ArgumentParser
 from collections import OrderedDict
-
-from inotify_simple import INotify
-from inotify_simple import flags as inotify_flags
-
-from six import itervalues, iteritems
-
+from json import dumps as json, loads as dejson
+import logging as log
+from os import path
+from pickle import dump as pickle, load as unpickle
+from threading import Thread
+from time import sleep
+from spinn_utilities.overrides import overrides
 from spalloc_server import __version__, coordinates, configuration
 from spalloc_server.configuration import Configuration
 from spalloc_server.controller import Controller
+from spalloc_server.polling_server_core import PollingServerCore
+from spalloc_server.configuration_reloader import ConfigurationReloader
 
+BUFFER_SIZE = 1024
 
-_COMMANDS = OrderedDict()
-"""A dictionary from command names to (unbound) methods of the
-:py:class:`.Server` class.
+_COMMANDS = {}
+""" A dictionary from command names to (unbound) methods of the\
+    :py:class:`.Server` class.
 """
 
 
-def _command(f):
-    """Decorator which marks a class function of :py:class:`.Server` as a
-    command which may be called by a client.
+def spalloc_command(f):
+    """ Decorator which marks a class function of :py:class:`.Server` as a\
+        command which may be called by a client.
     """
     _COMMANDS[f.__name__] = f
     return f
 
 
-class Server(object):
-    """A TCP server which manages, power, partitioning and scheduling of jobs
-    on SpiNNaker machines.
-
-    Once constructed the server starts a background thread
-    (:py:attr:`._server_thread`, :py:meth:`._run`) which implements the main
-    server logic and handles communication with clients, monitoring of
-    asynchronous board control events (e.g. board power-on completion) and
-    watches the config file for changes. All members of this object are assumed
-    to be accessed only from this thread while it is running. The thread is
-    stopped, and its completion awaited by calling :py:meth:`.stop_and_join`,
-    stopping the server.
-
-    The server uses a :py:class:`~spalloc_server.Controller` object to
-    implement scheduling, allocation and machine management functionality. This
-    object is :py:mod:`pickled <pickle>` when the server shuts down in order to
-    preserve the state of all managed machines (e.g. allocated jobs etc.).
-
-    To allow the interruption of the server thread on asynchronous events from
-    the Controller a :py:func:`~socket.socketpair` (:py:attr:`._notify_send`
-    and :py:attr:`._notify_send`) is used which monitored allong with client
-    connections and config file changes.
-
-    A number of callable commands are implemented by the server in the form of
-    a subset of the :py:class:`.Server`'s methods indicated by the
-    :py:func:`._command` decorator. These may be called by a client by sending
-    a line ``{"command": "...", "args": [...], "kwargs": {...}}``. If the
-    function throws an exception, the client is disconnected. If the function
-    returns, it is packed as a JSON line ``{"return": ...}``.
+class _CriticalStop(Exception):
+    pass
+
+
+class Server(PollingServerCore, ConfigurationReloader):
+    """ A TCP server which manages, power, partitioning and scheduling of jobs\
+        on SpiNNaker machines.
+
+    Once constructed the server starts a background thread\
+    (:py:attr:`._server_thread`, :py:meth:`._run`) which implements the main\
+    server logic and handles communication with clients, monitoring of\
+    asynchronous board control events (e.g. board power-on completion) and\
+    watches for selected signals. All members of this object are assumed to be\
+    accessed only from this thread while it is running. The thread is stopped,\
+    and its completion awaited by calling\
+    :py:meth:`.stop_and_join`, stopping the server.
+
+    The server uses a :py:class:`~spalloc_server.Controller` object to\
+    implement scheduling, allocation and machine management functionality.\
+    This object is :py:mod:`pickled <pickle>` when the server shuts down in\
+    order to preserve the state of all managed machines (e.g. allocated jobs\
+    etc.).
+
+    To allow the interruption of the server thread on asynchronous events from\
+    the Controller a :py:func:`~socket.socketpair` (:py:attr:`._notify_send`\
+    and :py:attr:`._notify_send`) is used which monitored along with client\
+    connections and SIGHUP signals (used to trigger config file reloading).
+
+    A number of callable commands are implemented by the server in the form of\
+    a subset of the :py:class:`.Server`'s methods indicated by the\
+    :py:func:`.spalloc_command` decorator. These may be called by a client by\
+    sending a line ``{"command": "...", "args": [...], "kwargs": {...}}``. If\
+    the function throws an exception, the client is disconnected. If the\
+    function returns, it is packed as a JSON line ``{"return": ...}``, and if\
+    the function raises an exception, it is packed as a JSON line\
+    ``{"exception": "the message"}``.
     """
 
-    def __init__(self, config_filename, cold_start=False):
+    def __init__(self, config_filename, cold_start=False, port=22244):
         """
-        Parameters
-        ----------
-        config_filename : str
-            The filename of the config file for the server which describes the
+        :param config_filename: \
+            The filename of the config file for the server which describes the\
             machines to be controlled.
-        cold_start : bool
-            If False (the default), the server will attempt to restore its
+        :type config_filename: str
+        :param cold_start: \
+            If False (the default), the server will attempt to restore its\
             previous state, if True, the server will start from scratch.
+        :type cold_start: bool
+        :param port: Which port to listen on. Defaults to 22244.
+        :type port: int
         """
-        self._config_filename = config_filename
+        # ============ STATE THAT NEEDS TO BE ALWAYS DEFINED ============
+
         self._cold_start = cold_start
+        self._port = port
 
         # Should the background thread terminate?
         self._stop = False
 
-        # The background thread in which the server will run
-        self._server_thread = threading.Thread(target=self._run,
-                                               name="Server Thread")
-
-        # The poll object used for listening for connections
-        self._poll = select.poll()
-
-        # This socket pair is used by background threads to interrupt the main
-        # event loop.
-        self._notify_send, self._notify_recv = socket.socketpair()
-        self._poll.register(self._notify_recv, select.POLLIN)
+        # Flag for checking if the server is still alive
+        self._running = False
 
         # Currently open sockets to clients. Once server started, should only
         # be accessed from the server thread.
         self._server_socket = None
-        # {fd: socket, ...}
-        self._client_sockets = {}
+
+        # The server core object that the object that is persisted
+        self._controller = None
 
         # Buffered data received from each socket
         # {fd: buf, ...}
         self._client_buffers = {}
 
-        # For each client, contains a set() of job IDs and machine names that
-        # the client is watching for changes or None if all changes are to be
-        # monitored.
-        # {socket: set or None, ...}
-        self._client_job_watches = {}
-        self._client_machine_watches = {}
+        # ============ SUPERCLASS INITIALISATION ============
+
+        super().__init__()
+        ConfigurationReloader.__init__(self, config_filename, self.wake)
+
+        # ============ ACTIVE OBJECTS ============
+
+        # The background thread in which the server will run
+        self._server_thread = Thread(target=self._run, name="Server Thread")
 
         # The current server configuration options. Once server started, should
         # only be accessed from the server thread.
         self._configuration = Configuration()
 
         # Infer the saved-state location
-        self._state_filename = os.path.join(
-            os.path.dirname(self._config_filename),
-            ".{}.state.{}".format(os.path.basename(self._config_filename),
-                                  __version__)
-        )
+        self._state_filename = self._get_state_filename(
+            self.configuration_file)
 
         # Attempt to restore saved state if required
-        self._controller = None
-        if not self._cold_start:
-            if os.path.isfile(self._state_filename):
-                try:
-                    with open(self._state_filename, "rb") as f:
-                        self._controller = pickle.load(f)
-                    logging.info("Server warm-starting from %s.",
-                                 self._state_filename)
-                except:
-                    # Some other error occurred during unpickling.
-                    logging.exception(
-                        "Server state could not be unpacked from %s.",
-                        self._state_filename)
+        if not self._cold_start and path.isfile(self._state_filename):
+            try:
+                with open(self._state_filename, "rb") as f:
+                    self._controller = unpickle(f)
+                log.info("Server warm-starting from %s.",
+                         self._state_filename)
+            except Exception:  # pylint: disable=broad-except
+                # Some other error occurred during unpickling.
+                log.exception(
+                    "Server state could not be unpacked from %s.",
+                    self._state_filename)
+                self._controller = None
 
         # Perform cold-start if no saved state was loaded
         if self._controller is None:
-            logging.info("Server cold-starting.")
+            log.info("Server cold-starting.")
             self._controller = Controller()
 
         # Notify the background thread when something changes in the background
         # of the controller (e.g. power state changes).
-        self._controller.on_background_state_change = self._notify
+        self._controller.on_background_state_change = self.wake
 
         # Read configuration file. This must succeed when the server is first
         # being started.
-        if not self._read_config_file():
-            raise Exception("Config file could not be loaded.")
-
-        # Set up inotify watcher for config file changes
-        self._config_inotify = INotify()
-        self._poll.register(self._config_inotify.fd, select.POLLIN)
-        self._watch_config_file()
+        if not self.read_config_file():
+            self._controller.stop()
+            raise _CriticalStop("Config file could not be loaded.")
 
         # Start the server
         self._server_thread.start()
-
-        # Flag for checking if the server is still alive
         self._running = True
 
-    def _notify(self):
-        """Notify the background thread that something has happened.
-
-        Calling this method simply wakes up the server thread causing it to
-        perform all its usual checks and processing steps.
-        """
-        self._notify_send.send(b"x")
+    def _send_change_notifications(self):
+        raise NotImplementedError
 
-    def _watch_config_file(self):
-        """Create an inotify watch on the config file.
-
-        This watch is monitored by the main server threead and if the config
-        file is changed, the config file is re-read.
-        """
-        # A one-shot watch is used since some editors cause a delete event to
-        # be produced when the file is saved, removing the watch anyway. Using
-        # a one-shot watch simplifies implementation as it requires the watch
-        # to *always* be recreated, rather than just 'sometimes'.
-        self._config_inotify.add_watch(self._config_filename,
-                                       inotify_flags.MODIFY |
-                                       inotify_flags.ATTRIB |
-                                       inotify_flags.CLOSE_WRITE |
-                                       inotify_flags.MOVED_TO |
-                                       inotify_flags.CREATE |
-                                       inotify_flags.DELETE |
-                                       inotify_flags.DELETE_SELF |
-                                       inotify_flags.MOVE_SELF |
-                                       inotify_flags.ONESHOT)
-
-    def _read_config_file(self):
-        """(Re-)read the server configuration.
-
-        If reading of the config file fails, the current configuration is
-        retained, unchanged.
-
-        Returns
-        -------
-        bool
-            True if reading succeded, False otherwise.
-        """
-        try:
-            with open(self._config_filename, "r") as f:
-                config_script = f.read()  # pragma: no branch
-        except (IOError, OSError):
-            logging.exception("Could not read "
-                              "config file %s", self._config_filename)
-            return False
+    def _clear_watches(self, client):
+        raise NotImplementedError
 
-        # The environment in which the configuration script is exexcuted (and
-        # where the script will store its options.)
-        try:
-            g = {}
-            g.update(configuration.__dict__)
-            g.update(coordinates.__dict__)
-            exec(config_script, g)
-        except:
-            # Executing the config file failed, don't update any settings
-            logging.exception("Error while evaluating "
-                              "config file %s", self._config_filename)
-            return False
-
-        # Make sure a configuration object is specified
-        new = g.get("configuration", None)
-        if not isinstance(new, Configuration):
-            logging.error("'configuration' must be a Configuration object "
-                          "in config file %s", self._config_filename)
-            return False
+    def _get_state_filename(self, cfg):
+        """ How to get the name of the state file from the name of another\
+            file (expected to be the config file). Assumes that the config\
+            file is in a directory that can be written to.
+
+        :param cfg: The name of the file to use as a base.
+        :type cfg: str
+        :return: The full filename
+        """
+        # Factored out for ease of reading.
+        dirname = path.dirname(cfg)
+        basename = path.basename(cfg)
+        filename = ".{}.state.{}".format(basename, __version__)
+        return path.join(dirname, filename)
+
+    @overrides(ConfigurationReloader._parse_config)
+    def _parse_config(self, config_file_contents):
+        g = {}
+        g.update(configuration.__dict__)
+        g.update(coordinates.__dict__)
+        exec(config_file_contents, g)  # pylint: disable=exec-used
+        return g
+
+    @overrides(ConfigurationReloader._validate_config)
+    def _validate_config(self, parsed_config):
+        new = parsed_config.get("configuration", None)
+        if new is None or not isinstance(new, Configuration):
+            return None
+        return new
 
-        # Update the configuration
+    @overrides(ConfigurationReloader._load_valid_config)
+    def _load_valid_config(self, validated_config):
         old = self._configuration
-        self._configuration = new
+        self._configuration = validated_config
 
         # Restart the server if the port or IP has changed (or if the server
         # has not yet been started...)
-        if (new.port != old.port or
-                new.ip != old.ip or
-                self._server_socket is None):
+        if validated_config.ip != old.ip or self._server_socket is None:
             # Close all open connections
-            self._close()
+            if self._close():  # pragma: no cover
+                sleep(0.25)  # Ugly hack; fully release socket now
 
-            # Create a new server socket
-            self._server_socket = socket.socket(socket.AF_INET,
-                                                socket.SOCK_STREAM)
-            self._server_socket.setsockopt(socket.SOL_SOCKET,
-                                           socket.SO_REUSEADDR, 1)
-            self._server_socket.bind((new.ip, new.port))
-            self._server_socket.listen(5)
-            self._poll.register(self._server_socket,
-                                select.POLLIN)
+            # Create a validated_config server socket
+            self._server_socket = self._open_server_socket(
+                validated_config.ip, self._port)
 
         # Update the controller
-        self._controller.max_retired_jobs = new.max_retired_jobs
-        self._controller.machines = OrderedDict((m.name, m)
-                                                for m in new.machines)
-
-        logging.info("Config file %s read successfully.",
-                     self._config_filename)
-        return True
+        self._controller.max_retired_jobs = validated_config.max_retired_jobs
+        self._controller.seconds_before_free = \
+            validated_config.seconds_before_free
+        self._controller.machines = OrderedDict(
+            (m.name, m) for m in validated_config.machines)
+        self.wake()
 
     def _close(self):
-        """Close all server sockets and disconnect all client connections."""
+        """ Close all server sockets and disconnect all client connections.
+
+        :return: Whether the server socket itself was closed.
+        """
+        result = False
         if self._server_socket is not None:
-            self._poll.unregister(self._server_socket)
+            self.unregister_channel(self._server_socket)
+            log.info("closing server socket")
             self._server_socket.close()
-        for client_socket in list(itervalues(self._client_sockets)):
+            result = True
+            self._server_socket = None
+        for client_socket in list(self._client_buffers.keys()):
             self._disconnect_client(client_socket)
+        return result
 
     def _disconnect_client(self, client):
-        """Disconnect a client.
+        """ Disconnect a client.
 
-        Parameters
-        ----------
-        client : :py:class:`socket.Socket`
+        :param client: The client to disconnect
+        :type client: :py:class:`socket.Socket`
         """
         try:
-            logging.info("Client %s disconnected.", client.getpeername())
-        except:
-            logging.info("Client %s disconnected.", client)
-
-        # Remove from the client list
-        del self._client_sockets[client.fileno()]
-
-        # Clear input buffer
-        del self._client_buffers[client]
+            log.info("Client %s disconnected.", client.getpeername())
+        except Exception:  # pylint: disable=broad-except
+            log.info("Client %s disconnected.", client)
+
+        # Clear input buffer if created
+        if client in self._client_buffers:
+            del self._client_buffers[client]
 
         # Clear any watches
-        self._client_job_watches.pop(client, None)
-        self._client_machine_watches.pop(client, None)
+        self._clear_watches(client)
 
         # Stop watching the client's socket for data
-        self._poll.unregister(client)
+        try:
+            self.unregister_channel(client)
+        except KeyError:
+            # The odd case of the unregistered client -
+            # this can be ignored as it wasn't registered anyway
+            pass
 
         # Disconnect the client
         client.close()
 
     def _accept_client(self):
-        """Accept a new client."""
-        client, addr = self._server_socket.accept()
-        logging.info("New client connected from %s", addr)
-
-        # Watch the client's socket for datat
-        self._poll.register(client, select.POLLIN)
+        """ Accept a new client.
+        """
+        try:
+            client, addr = self._server_socket.accept()
+        except IOError as e:  # pragma: no cover
+            log.warning("problem when accepting connection", exc_info=e)
+            return
+        log.info("New client connected from %s", addr)
 
-        # Keep a reference to the socket
-        self._client_sockets[client.fileno()] = client
+        # Watch the client's socket for data
+        self.register_channel(client)
 
         # Create a buffer for data sent by the client
         self._client_buffers[client] = b""
 
+    def _msg_client(self, client, message):
+        """ Low-level way to send a message to a client.
+
+        :param client: The client that we are sending a message to.
+        :type client: :py:class:`socket.Socket`
+        :param message: The object or array to send. Will be converted to JSON.
+        """
+        try:
+            client.send(json(message).encode("utf-8") + b"\n")
+        except Exception:
+            self._disconnect_client(client)
+            raise
+
+    def _handle_command(self, client, line):
+        """ Dispatch a single command.
+
+        :param client: \
+            The client that made the request, used to provide a session\
+            context where relevant.
+        :type client: :py:class:`socket.Socket`
+        :param line: \
+            The line parsed from the socket. Should be a complete JSON object\
+            with at least a 'command' key.
+        :type line: str
+        :return: Dictionary describing the result of the operation.
+        :rtype: dict
+        :raises IOError: \
+            If something really bad goes wrong with message decoding. The\
+            expected response at this point would be simply closing the socket.
+        """
+        cmd_obj = dejson(line.decode("utf-8"))
+        if "command" not in cmd_obj:
+            raise IOError("no command name given")
+        command_name = cmd_obj["command"]
+        if not isinstance(command_name, str):
+            raise IOError("parsed gibberish from user")
+        if command_name not in _COMMANDS:
+            log.info("lookup failure: %s", command_name)
+            raise IOError("unrecognised command name")
+        command = _COMMANDS[command_name]
+        if command is None:  # pragma: no cover
+            # Should be unreachable
+            log.critical("unexpected lookup failure: %s", command_name)
+            raise IOError("unrecognised command name")
+        args = cmd_obj["args"] if "args" in cmd_obj else []
+        if not isinstance(args, list):
+            raise IOError("bad args; must be JSON array")
+        kwargs = cmd_obj["kwargs"] if "kwargs" in cmd_obj else {}
+        if not isinstance(kwargs, dict):
+            raise IOError("bad kwargs: must be JSON dictionary")
+        elif "client" in kwargs:
+            del kwargs["client"]
+        # Execute the specified command
+        try:
+            return {"return": command(self, client, *args, **kwargs)}
+        except Exception as e:  # pylint: disable=broad-except
+            return {"exception": str(e)}
+
     def _handle_commands(self, client):
-        """Handle an incomming command from a client.
+        """ Handle incoming commands from a client.
 
-        Parameters
-        ----------
-        client : :py:class:`socket.Socket`
+        :param client: \
+            The client that made the request, used to provide a session\
+            context where relevant.
+        :type client: :py:class:`socket.Socket`
         """
         try:
-            data = client.recv(1024)
+            data = client.recv(BUFFER_SIZE)
         except (OSError, IOError):
             data = b""
 
         # Did the client disconnect?
-        if len(data) == 0:
+        if not data:
             self._disconnect_client(client)
             return
 
-        self._client_buffers[client] += data
-
-        # Process any complete commands (whole lines)
-        while b"\n" in self._client_buffers[client]:
-            line, _, self._client_buffers[client] = \
-                self._client_buffers[client].partition(b"\n")
-
-            try:
-                cmd_obj = json.loads(line.decode("utf-8"))
-
-                # Execute the specified command
-                ret_val = _COMMANDS[cmd_obj["command"]](
-                    self, client, *cmd_obj["args"], **cmd_obj["kwargs"])
-
-                # Return the response
-                client.send(json.dumps({"return": ret_val}).encode("utf-8") +
-                            b"\n")
-            except:
-                # If any of the above fails for any reason (e.g. invalid JSON,
-                # unrecognised command, command crashes, etc.), just disconnect
-                # the client.
-                logging.exception("Client %s sent bad command %r, "
-                                  "disconnecting",
-                                  client.getpeername(), line)
-                self._disconnect_client(client)
-                return
-
-    def _send_change_notifications(self):
-        """Send any registered change notifications to clients.
+        peer = "UNKNOWN"
+        line = ""
+        try:
+            peer = client.getpeername()
+            self._client_buffers[client] += data
 
-        Sends notifications of the forms ``{"jobs_changed": [job_id, ...]}``
-        and ``{"machines_changed": [machine_name, ...]}`` to clients who have
-        subscribed to be notified of changes to jobs or machines.
-        """
-        # Notify clients about jobs which have changed
-        changed_jobs = self._controller.changed_jobs
-        if changed_jobs:
-            for client, jobs in list(iteritems(self._client_job_watches)):
-                if jobs is None or not jobs.isdisjoint(changed_jobs):
-                    try:
-                        client.send(
-                            json.dumps(
-                                {"jobs_changed":
-                                 list(changed_jobs)
-                                 if jobs is None else
-                                 list(changed_jobs.intersection(jobs))}
-                            ).encode("utf-8") + b"\n")
-                    except (OSError, IOError):
-                        logging.exception(
-                            "Could not send notification.")
-                        self._disconnect_client(client)
+            # Process any complete commands (whole lines)
+            while b"\n" in self._client_buffers[client]:
+                line, _, self._client_buffers[client] = \
+                    self._client_buffers[client].partition(b"\n")
+                # Note that we skip blank lines
+                if line:
+                    self._msg_client(client,
+                                     self._handle_command(client, line))
+        except Exception:  # pylint: disable=broad-except
+            # If any of the above fails for any reason (e.g. invalid JSON,
+            # unrecognised command, command crashes, etc.), just disconnect
+            # the client.
+            log.exception("Client %s sent bad command %r, disconnecting",
+                          peer, line)
+            self._disconnect_client(client)
 
-        # Notify clients about machines which have changed
-        changed_machines = self._controller.changed_machines
-        if changed_machines:
-            for client, machines in list(
-                    iteritems(self._client_machine_watches)):
-                if (machines is None or
-                        not machines.isdisjoint(changed_machines)):
+    def _send_notifications(self, label, changes, watches):
+        """ How to actually send requested notifications."""
+        if changes:
+            for client, items in list(watches.items()):
+                if items is None or not items.isdisjoint(changes):
                     try:
-                        client.send(
-                            json.dumps(
-                                {"machines_changed":
-                                 list(changed_machines)
-                                 if machines is None else
-                                 list(changed_machines.intersection(machines))}
-                            ).encode("utf-8") + b"\n")
+                        self._msg_client(client, {
+                            label: list(changes) if items is None else
+                            list(changes.intersection(items))})
                     except (OSError, IOError):
-                        logging.exception(
-                            "Could not send notification.")
-                        self._disconnect_client(client)
+                        log.exception("Could not send notification.")
 
     def _run(self):
-        """The main server thread.
+        """ The main server thread.
 
-        This 'infinate' loop runs in a background thread and waits for and
-        processes events such as the :py:meth:`._notify` method being called,
-        the config file changing, clients sending commands or new clients
-        connecting. It also periodically calls destroy_timed_out_jobs on the
+        This 'infinite' loop runs in a background thread and waits for and\
+        processes events such as the :py:meth:`.PollingServerCore.wake` method\
+        being called, the config file changing, clients sending commands or\
+        new clients connecting. It also periodically calls\
+        :py:meth:`.controller.Controller.destroy_timed_out_jobs` on the\
         controller.
         """
-        logging.info("Server running.")
+        log.info("Server running.")
         while not self._stop:
             # Wait for a connection to get opened/closed, a command to arrive,
-            # the config file to change or the timeout to ellapse.
-            events = self._poll.poll(
+            # the config file to change or the timeout to elapse.
+            channels = self.ready_channels(
                 self._configuration.timeout_check_interval)
 
-            # Cull any jobs which have timed out
-            self._controller.destroy_timed_out_jobs()
-
-            for fd, event in events:
-                if fd == self._notify_recv.fileno():
-                    # _notify was called
-                    self._notify_recv.recv(1024)
-                elif fd == self._server_socket.fileno():
+            for channel in channels:
+                if channel is None:  # pragma: no cover
+                    continue
+                if channel == self._server_socket:
                     # New client connected
                     self._accept_client()
-                elif fd in self._client_sockets:
+                else:
                     # Incoming data from client
-                    self._handle_commands(self._client_sockets[fd])
-                elif fd == self._config_inotify.fd:
-                    # Config file changed, re-read it
-                    time.sleep(0.1)
-                    self._config_inotify.read()
-                    self._watch_config_file()
-                    self._read_config_file()
-                else:  # pragma: no cover
-                    # Should not get here...
-                    assert False
+                    self._handle_commands(channel)
+
+            # Cull any jobs which have timed out
+            self._controller.destroy_timed_out_jobs()
+
+            # Check if any new free spaces have appeared
+            self._controller.check_free()
 
             # Send any job/machine change notifications out
             self._send_change_notifications()
 
+            # Config file changed, re-read it
+            if self.config_needs_reloading:
+                if not self.read_config_file():  # pragma: no cover
+                    log.warning("failed to reread configuration file")
+
     def is_alive(self):
-        """Is the server running?"""
+        """ Is the server running?
+        """
         return self._running
 
     def join(self):
-        """Wait for the server to completely shut down."""
+        """ Wait for the server to completely shut down.
+        """
         self._server_thread.join()
         self._controller.join()
 
     def stop_and_join(self):
-        """Stop the server and wait for it to shut down completely."""
-        logging.info("Server shutting down, please wait...")
-
-        # Shut down server thread
-        self._stop = True
-        self._notify()
-        self._server_thread.join()
-
-        # Stop watching config file
-        self._config_inotify.close()
+        """ Stop the server and wait for it to shut down completely.
+        """
+        log.info("Server shutting down, please wait...")
 
-        # Close all connections
-        logging.info("Closing connections...")
-        self._close()
+        try:
+            # Shut down server thread
+            self._stop = True
+            self.wake()
+            self._server_thread.join()
+        finally:
+            # Close all connections; this is the critical part as it closes
+            # the server socket itself.
+            log.info("Closing connections...")
+            self._close()
 
         # Shut down the controller and flush all BMP commands
-        logging.info("Waiting for all queued BMP commands...")
+        log.info("Waiting for all queued BMP commands...")
         self._controller.stop()
         self._controller.join()
 
         # Dump controller state to file
         with open(self._state_filename, "wb") as f:
-            pickle.dump(self._controller, f)
+            pickle(self._controller, f)
 
-        logging.info("Server shut down.")
+        log.info("Server shut down.")
 
         self._running = False
 
-    @_command
-    def version(self, client):
+    @staticmethod
+    def _name(client):
+        """ Get the 'name' of the client. This is the string form of the IP\
+            address, or None if the concept isn't well defined.
+
+        :return: The client's name (for logging).
+        """
+        try:
+            return None if client is None else str(client.getpeername()[0])
+        except Exception:  # pylint: disable=broad-except
+            # pragma: no cover
+            return None
+
+
+class SpallocServer(Server):
+    def __init__(self, config_filename, cold_start=False, port=22244):
+        # For each client, contains a set() of job IDs and machine names that
+        # the client is watching for changes or None if all changes are to be
+        # monitored.
+        # {socket: set or None, ...}
+        self._client_job_watches = {}
+        self._client_machine_watches = {}
+
+        super().__init__(config_filename, cold_start, port)
+
+    def _send_change_notifications(self):
+        """ Send any registered change notifications to clients.
+
+        Sends notifications of the forms ``{"jobs_changed": [job_id, ...]}``\
+        and ``{"machines_changed": [machine_name, ...]}`` to clients who have\
+        subscribed to be notified of changes to jobs or machines.
+        """
+        # Notify clients about jobs which have changed
+        self._send_notifications("jobs_changed",
+                                 self._controller.changed_jobs,
+                                 self._client_job_watches)
+        # Notify clients about machines which have changed
+        self._send_notifications("machines_changed",
+                                 self._controller.changed_machines,
+                                 self._client_machine_watches)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, _type, _value, _tb):
+        if self._running:
+            self.stop_and_join()
+        return False
+
+    @spalloc_command
+    def version(self, _client):
+        """
+        :rtype: str
+        :return: The server's version number.
         """
-        Returns
-        -------
-        str
-            The server's version number."""
         return __version__
 
-    @_command
+    @spalloc_command
     def create_job(self, client, *args, **kwargs):
-        """Create a new job (i.e. allocation of boards).
+        """ Create a new job (i.e. allocation of boards).
 
         This function should be called in one of the following styles::
 
             # Any single (SpiNN-5) board
             job_id = create_job(owner="me")
             job_id = create_job(1, owner="me")
 
@@ -520,452 +566,461 @@
             # Any 4x5 triad segment of a machine (may or may-not be a
             # torus/full machine)
             job_id = create_job(4, 5, owner="me")
 
             # Any torus-connected (full machine) 4x2 machine
             job_id = create_job(4, 2, require_torus=True, owner="me")
 
-        The 'other parameters' enumerated below may be used to further restrict
-        what machines the job may be allocated onto.
+        The 'other parameters' enumerated below may be used to further\
+        restrict what machines the job may be allocated onto.
 
-        Jobs for which no suitable machines are available are immediately
+        Jobs for which no suitable machines are available are immediately\
         destroyed (and the reason given).
 
-        Once a job has been created, it must be 'kept alive' by a simple
-        watchdog_ mechanism. Jobs may be kept alive by periodically calling the
-        :py:meth:`.job_keepalive` command or by calling any other job-specific
-        command. Jobs are culled if no keep alive message is received for
-        ``keepalive`` seconds. If absolutely necessary, a job's keepalive value
-        may be set to None, disabling the keepalive mechanism.
+        Once a job has been created, it must be 'kept alive' by a simple\
+        watchdog_ mechanism. Jobs may be kept alive by periodically calling\
+        the :py:meth:`.job_keepalive` command or by calling any other\
+        job-specific command. Jobs are culled if no keep alive message is\
+        received for ``keepalive`` seconds. If absolutely necessary, a job's\
+        keepalive value may be set to None, disabling the keepalive mechanism.
 
         .. _watchdog: https://en.wikipedia.org/wiki/Watchdog_timer
 
-        Once a job has been allocated some boards, these boards will be
+        Once a job has been allocated some boards, these boards will be\
         automatically powered on and left unbooted ready for use.
 
-        Parameters
-        ----------
-        owner : str
+        :param str owner:
             **Required.** The name of the owner of this job.
-        keepalive : float or None
-            *Optional.* The maximum number of seconds which may elapse between
-            a query on this job before it is automatically destroyed. If None,
-            no timeout is used. (Default: 60.0)
-
-        Other Parameters
-        ----------------
-        machine : str or None
-            *Optional.* Specify the name of a machine which this job must be
-            executed on. If None, the first suitable machine available will be
-            used, according to the tags selected below. Must be None when tags
-            are given. (Default: None)
-        tags : [str, ...] or None
-            *Optional.* The set of tags which any machine running this job must
-            have. If None is supplied, only machines with the "default" tag
-            will be used. If machine is given, this argument must be None.
+        :param keepalive:
+            The maximum number of seconds which may elapse between a query on
+            this job before it is automatically destroyed. If None, no timeout
+            is used. (Default: 60.0)
+        :type keepalive: float or None
+        :param machine:
+            Specify the name of a machine which this job must be executed on.
+            If None, the first suitable machine available will be used,
+            according to the tags selected below. Must be None when tags are
+            given. (Default: None)
+        :type machine: str or None
+        :param tags:
+            The set of tags which any machine running this job must have. If
+            None is supplied, only machines with the "default" tag will be
+            used. If machine is given, this argument must be None.
             (Default: None)
-        min_ratio : float
-            The aspect ratio (h/w) which the allocated region must be 'at least
-            as square as'. Set to 0.0 for any allowable shape, 1.0 to be
+        :type tags: list(str) or None
+        :param float min_ratio:
+            The aspect ratio (h/w) which the allocated region must be 'at
+            least as square as'. Set to 0.0 for any allowable shape, 1.0 to be
             exactly square. Ignored when allocating single boards or specific
             rectangles of triads.
-        max_dead_boards : int or None
+        :param max_dead_boards:
             The maximum number of broken or unreachable boards to allow in the
             allocated region. If None, any number of dead boards is permitted,
             as long as the board on the bottom-left corner is alive (Default:
             None).
-        max_dead_links : int or None
+        :type max_dead_boards: int or None
+        :param max_dead_links:
             The maximum number of broken links allow in the allocated region.
             When require_torus is True this includes wrap-around links,
-            otherwise peripheral links are not counted.  If None, any number of
-            broken links is allowed. (Default: None).
-        require_torus : bool
+            otherwise peripheral links are not counted.  If None, any number
+            of broken links is allowed. (Default: None).
+        :type max_dead_links: int or None
+        :param bool require_torus:
             If True, only allocate blocks with torus connectivity. In general
             this will only succeed for requests to allocate an entire machine
             (when the machine is otherwise not in use!). Must be False when
             allocating boards. (Default: False)
-
-        Returns
-        -------
-        int
-            The job ID given to the newly allocated job.
+        :return: The job ID given to the newly allocated job.
+        :rtype: int
         """
         if kwargs.get("tags", None) is not None:
             kwargs["tags"] = set(kwargs["tags"])
-        return self._controller.create_job(*args, **kwargs)
+        owner = kwargs.get("owner", None)
+        if owner is None:
+            raise TypeError("owner must be specified for all jobs")
+        kwargs["owner"] = str(owner)
+        keepalive = kwargs.get("keepalive", 60.0)
+        kwargs["keepalive"] = (None if keepalive is None else float(keepalive))
+        return self._controller.create_job(self._name(client), *args, **kwargs)
 
-    @_command
+    @spalloc_command
     def job_keepalive(self, client, job_id):
-        """Reset the keepalive timer for the specified job.
+        """ Reset the keepalive timer for the specified job.
 
-        Note all other job-specific commands implicitly do this.
+        .. note::
+
+            All other job-specific commands implicitly do this.
+
+        :param job_id: A job ID to be kept alive.
+        :type job_id: int
         """
-        self._controller.job_keepalive(job_id)
+        self._controller.job_keepalive(self._name(client), job_id)
 
-    @_command
+    @spalloc_command
     def get_job_state(self, client, job_id):
-        """Poll the state of a running job.
+        """ Poll the state of a running job.
 
-        Returns
-        -------
-        {"state": state, "power": power
-         "keepalive": keepalive, "reason": reason}
-            Where:
+        :param int job_id: A job ID to get the state of.
+        :rtype: dict(str, ...)
+        :return: A dictionary with the following keys:
 
-            state : :py:class:`~spalloc_server.controller.JobState`
+            ``state`` : :py:class:`~spalloc_server.controller.JobState`
                 The current state of the queried job.
-            power : bool or None
+            ``power`` : bool or None
                 If job is in the ready or power states, indicates whether the
-                boards are power{ed,ing} on (True), or power{ed,ing} off
-                (False). In other states, this value is None.
-            keepalive : float or None
+                boards are power{ed,ing} on (``True``), or power{ed,ing} off
+                (``False``). In other states, this value is ``None``.
+            ``keepalive`` : float or None
                 The Job's keepalive value: the number of seconds between
                 queries about the job before it is automatically destroyed.
-                None if no timeout is active (or when the job has been
+                ``None`` if no timeout is active (or when the job has been
                 destroyed).
-            reason : str or None
+            ``reason`` : str or None
                 If the job has been destroyed, this may be a string describing
                 the reason the job was terminated.
-            start_time : float or None
+            ``start_time`` : float or None
                 For queued and allocated jobs, gives the Unix time (UTC) at
                 which the job was created (or None otherwise).
         """
-        out = self._controller.get_job_state(job_id)._asdict()
+        out = self._controller.get_job_state(
+            self._name(client), job_id)._asdict()
         out["state"] = int(out["state"])
         return out
 
-    @_command
+    @spalloc_command
     def get_job_machine_info(self, client, job_id):
-        """Get the list of Ethernet connections to the allocated machine.
+        """ Get the list of Ethernet connections to the allocated machine.
 
-        Returns
-        -------
-        {"width": width, "height": height, \
-         "connections": connections, "machine_name": machine_name}
-            Where:
+        :param int job_id: A job ID to get the machine info for.
+        :rtype: dict(str, ...)
+        :return: A dictionary with the following keys:
 
-            width, height : int or None
+            ``width``, ``height`` : int or None
                 The dimensions of the machine in chips, e.g. for booting.
-
-                None if no boards are allocated to the job.
-            connections : [[[x, y], hostname], ...] or None
+                ``None`` if no boards are allocated to the job.
+            ``connections`` : [[[x, y], hostname], ...] or None
                 A list giving Ethernet-connected chip coordinates in the
                 machine to hostname.
-
-                None if no boards are allocated to the job.
-            machine_name : str or None
+                ``None`` if no boards are allocated to the job.
+            ``machine_name`` : str or None
                 The name of the machine the job is allocated on.
-
-                None if no boards are allocated to the job.
-            boards : [[x, y, z], ...] or None
-                All the boards allocated to the job or None if no boards
+                ``None`` if no boards are allocated to the job.
+            ``boards`` : [[x, y, z], ...] or None
+                All the boards allocated to the job or ``None`` if no boards
                 allocated.
         """
         width, height, connections, machine_name, boards = \
-            self._controller.get_job_machine_info(job_id)
+            self._controller.get_job_machine_info(self._name(client), job_id)
 
         if connections is not None:
-            connections = list(iteritems(connections))
+            connections = list(connections.items())
         if boards is not None:
             boards = list(boards)
 
         return {"width": width, "height": height,
                 "connections": connections,
                 "machine_name": machine_name,
                 "boards": boards}
 
-    @_command
+    @spalloc_command
     def power_on_job_boards(self, client, job_id):
-        """Power on (or reset if already on) boards associated with a job.
+        """ Power on (or reset if already on) boards associated with a job.
 
-        Once called, the job will enter the 'power' state until the power state
-        change is complete, this may take some time.
+        Once called, the job will enter the 'power' state until the power
+        state change is complete, this may take some time.
+
+        :param int job_id: A job ID to turn boards on for.
         """
-        self._controller.power_on_job_boards(job_id)
+        self._controller.power_on_job_boards(self._name(client), job_id)
 
-    @_command
+    @spalloc_command
     def power_off_job_boards(self, client, job_id):
-        """Power off boards associated with a job.
+        """ Power off boards associated with a job.
+
+        Once called, the job will enter the 'power' state until the power
+        state change is complete, this may take some time.
 
-        Once called, the job will enter the 'power' state until the power state
-        change is complete, this may take some time.
+        :param int job_id: A job ID to turn boards off for.
         """
-        self._controller.power_off_job_boards(job_id)
+        self._controller.power_off_job_boards(self._name(client), job_id)
 
-    @_command
+    @spalloc_command
     def destroy_job(self, client, job_id, reason=None):
-        """Destroy a job.
+        """ Destroy a job.
 
         Call when the job is finished, or to terminate it early, this function
         releases any resources consumed by the job and removes it from any
         queues.
 
-        Parameters
-        ----------
-        reason : str or None
-            *Optional.* A human-readable string describing the reason for the
-            job's destruction.
+        :param int job_id: A job ID to destroy.
+        :param str reason:
+            An optional human-readable description of the reason for the job's
+            destruction.
+        """
+        self._controller.destroy_job(self._name(client), job_id, reason)
+
+    def _register_for_notifications(self, client, watchset, _id):
+        """ Helper method that handles the protocol for registration for\
+            notifications.
+        """
+        if _id is None:
+            watchset[client] = None
+        elif client not in watchset:
+            watchset[client] = set([_id])
+        elif watchset[client] is not None:
+            watchset[client].add(_id)
+        else:
+            # Client is already notified about all changes, do nothing!
+            pass
+
+    def _unregister_for_notifications(self, client, watchset, _id):
+        """ Helper method that handles the protocol for unregistration for\
+            notifications.
         """
-        self._controller.destroy_job(job_id, reason)
+        if client not in watchset:
+            return
+        if _id is None:
+            del watchset[client]
+            return
+        watches = watchset[client]
+        if watches is not None:
+            watches.discard(_id)
+            if not watches:
+                del watchset[client]
+
+    def _clear_watches(self, client):
+        self._client_job_watches.pop(client, None)
+        self._client_machine_watches.pop(client, None)
 
-    @_command
+    @spalloc_command
     def notify_job(self, client, job_id=None):
-        r"""Register to be notified about changes to a specific job ID.
+        """ Register to be notified about changes to a specific job ID.
 
         Once registered, a client will be asynchronously be sent notifications
-        form ``{"jobs_changed": [job_id, ...]}\n`` enumerating job IDs which
+        form ``{"jobs_changed": [job_id, ...]}\\n`` enumerating job IDs which
         have changed. Notifications are sent when a job changes state, for
         example when created, queued, powering on/off, powered on and
         destroyed. The specific nature of the change is not reflected in the
         notification.
 
-        Parameters
-        ----------
-        job_id : int or None
+        :param job_id:
             A job ID to be notified of or None if all job state changes should
-            be reported.
+            be reported. Defaults to None (i.e., all jobs).
+        :type job_id: int or None
 
         See Also
         --------
         no_notify_job : Stop being notified about a job.
         notify_machine : Register to be notified about changes to machines.
         """
-        if job_id is None:
-            self._client_job_watches[client] = None
-        else:
-            if client not in self._client_job_watches:
-                self._client_job_watches[client] = set([job_id])
-            elif self._client_job_watches[client] is not None:
-                self._client_job_watches[client].add(job_id)
-            else:
-                # Client is already notified about all changes, do nothing!
-                pass
+        self._register_for_notifications(
+            client, self._client_job_watches, job_id)
 
-    @_command
+    @spalloc_command
     def no_notify_job(self, client, job_id=None):
-        """Stop being notified about a specific job ID.
+        """ Stop being notified about a specific job ID.
 
         Once this command returns, no further notifications for the specified
         ID will be received.
 
-        Parameters
-        ----------
-        job_id : id or None
+        :param job_id:
             A job ID to no longer be notified of or None to not be notified of
             any jobs. Note that if all job IDs were registered for
             notification, this command only has an effect if the specified
-            job_id is None.
+            job_id is None. Defaults to None (i.e., all jobs).
+        :type job_id: int or None
 
         See Also
         --------
         notify_job : Register to be notified about changes to a specific job.
         """
-        if client not in self._client_job_watches:
-            return
-
-        if job_id is None:
-            del self._client_job_watches[client]
-        else:
-            watches = self._client_job_watches[client]
-            if watches is not None:
-                watches.discard(job_id)
-                if len(watches) == 0:
-                    del self._client_job_watches[client]
+        self._unregister_for_notifications(
+            client, self._client_job_watches, job_id)
 
-    @_command
+    @spalloc_command
     def notify_machine(self, client, machine_name=None):
-        r"""Register to be notified about a specific machine name.
+        """ Register to be notified about a specific machine name.
 
         Once registered, a client will be asynchronously be sent notifications
-        of the form ``{"machines_changed": [machine_name, ...]}\n`` enumerating
-        machine names which have changed. Notifications are sent when a machine
-        changes state, for example when created, change, removed, allocated a
-        job or an allocated job is destroyed.
-
-        Parameters
-        ----------
-        machine_name : machine or None
+        of the form ``{"machines_changed": [machine_name, ...]}\\n``
+        enumerating machine names which have changed. Notifications are sent
+        when a machine changes state, for example when created, change,
+        removed, allocated a job or an allocated job is destroyed.
+
+        :param machine_name:
             A machine name to be notified of or None if all machine state
-            changes should be reported.
+            changes should be reported. Defaults to None (i.e., all machines).
+        :type machine_name: str or None
 
         See Also
         --------
         no_notify_machine : Stop being notified about a machine.
         notify_job : Register to be notified about changes to jobs.
         """
-        if machine_name is None:
-            self._client_machine_watches[client] = None
-        else:
-            if client not in self._client_machine_watches:
-                self._client_machine_watches[client] = set([machine_name])
-            elif self._client_machine_watches[client] is not None:
-                self._client_machine_watches[client].add(machine_name)
-            else:
-                # Client is already notified about all changes, do nothing!
-                pass
+        self._register_for_notifications(
+            client, self._client_machine_watches, machine_name)
 
-    @_command
+    @spalloc_command
     def no_notify_machine(self, client, machine_name=None):
-        """Unregister to be notified about a specific machine name.
+        """ Unregister to be notified about a specific machine name.
 
         Once this command returns, no further notifications for the specified
         ID will be received.
 
-        Parameters
-        ----------
-        machine_name : name or None
+        :param machine_name:
             A machine name to no longer be notified of or None to not be
-            notified of any machines. Note that if all machines were registered
-            for notification, this command only has an effect if the specified
-            machine_name is None.
+            notified of any machines. Note that if all machines were
+            registered for notification, this command only has an effect if
+            the specified machine_name is None. Defaults to None (i.e., all
+            machines).
+        :type machine_name: str or None
 
         See Also
         --------
         notify_machine : Register to be notified about changes to a machine.
         """
-        if client not in self._client_machine_watches:
-            return
+        self._unregister_for_notifications(
+            client, self._client_machine_watches, machine_name)
 
-        if machine_name is None:
-            del self._client_machine_watches[client]
-        else:
-            watches = self._client_machine_watches[client]
-            if watches is not None:
-                watches.discard(machine_name)
-                if len(watches) == 0:
-                    del self._client_machine_watches[client]
-
-    @_command
-    def list_jobs(self, client):
-        """Enumerate all non-destroyed jobs.
-
-        Returns
-        -------
-        jobs : [{...}, ...]
+    @spalloc_command
+    def list_jobs(self, _client):
+        """ Enumerate all non-destroyed jobs.
+
+        :rtype: list(dict(str, ...))
+        :return:
             A list of allocated/queued jobs in order of creation from oldest
             (first) to newest (last). Each job is described by a dictionary
             with the following keys:
 
-            "job_id" is the ID of the job.
-
-            "owner" is the string giving the name of the Job's owner.
-
-            "start_time" is the time the job was created (Unix time, UTC).
+            ``job_id``
+                the ID of the job.
 
-            "keepalive" is the maximum time allowed between queries for this
-            job before it is automatically destroyed (or None if the job can
-            remain allocated indefinitely).
+            ``owner``
+                the string giving the name of the Job's owner.
 
-            "state" is the current
-            :py:class:`~spalloc_server.controller.JobState` of the job.
+            ``start_time``
+                the time the job was created (Unix time, UTC).
 
-            "power" indicates whether the boards are powered on or not. If job
-            is in the ready or power states, indicates whether the boards are
-            power{ed,ing} on (True), or power{ed,ing} off (False). In other
-            states, this value is None.
-
-            "args" and "kwargs" are the arguments to the alloc function
-            which specifies the type/size of allocation requested and the
-            restrictions on dead boards, links and torus connectivity.
-
-            "allocated_machine_name" is the name of the machine the job has
-            been allocated to run on (or None if not allocated yet).
-
-            "boards" is a list [(x, y, z), ...] of boards allocated to the job.
+            ``keepalive``
+                the maximum time allowed between queries for this job before
+                it is automatically destroyed (or ``None`` if the job can
+                remain allocated indefinitely).
+
+            ``state``
+                the current
+                :py:class:`~spalloc_server.controller.JobState` of the job.
+
+            ``power``
+                indicates whether the boards are powered on or not. If job
+                is in the ready or power states, indicates whether the boards
+                are power{ed,ing} on (``True``), or power{ed,ing} off
+                (``False``). In other states, this value is ``None``.
+
+            ``args`` and ``kwargs``
+                the arguments to the alloc function which specifies the
+                type/size of allocation requested and the restrictions on
+                dead boards, links and torus connectivity.
+
+            ``allocated_machine_name``
+                the name of the machine the job has been allocated to run on
+                (or ``None`` if not allocated yet).
+
+            ``boards``
+                a list [(x, y, z), ...] of boards allocated to the job.
+
+            ``keepalivehost``
+                the IP address of the host reckoned to be keeping this job
+                alive (i.e., the host that did a request most recently that
+                updated the internal keep-alive timeout).
         """
         out = []
         for job in self._controller.list_jobs():
             job = job._asdict()
             job["state"] = int(job["state"])
             if job["boards"] is not None:
                 job["boards"] = list(job["boards"])
             if job["kwargs"].get("tags", None) is not None:
                 job["kwargs"]["tags"] = list(job["kwargs"]["tags"])
             out.append(job)
         return out
 
-    @_command
-    def list_machines(self, client):
-        """Enumerates all machines known to the system.
-
-        Returns
-        -------
-        machines : [{...}, ...]
+    @spalloc_command
+    def list_machines(self, _client):
+        """ Enumerates all machines known to the system.
+
+        :rtype: list(dict(str, ...))
+        :return:
             The list of machines known to the system in order of priority from
             highest (first) to lowest (last). Each machine is described by a
             dictionary with the following keys:
 
-            "name" is the name of the machine.
-
-            "tags" is the list ['tag', ...] of tags the machine has.
+            ``name``
+                the name of the machine.
 
-            "width" and "height" are the dimensions of the machine in
-            triads.
+            ``tags``
+                the list ['tag', ...] of tags the machine has.
 
-            "dead_boards" is a list([(x, y, z), ...]) giving the coordinates
-            of known-dead boards.
+            ``width`` and ``height``
+                the dimensions of the machine in triads.
 
-            "dead_links" is a list([(x, y, z, link), ...]) giving the
-            locations of known-dead links from the perspective of the sender.
-            Links to dead boards may or may not be included in this list.
+            ``dead_boards``
+                a list([(x, y, z), ...]) giving the coordinates
+                of known-dead boards.
+
+            ``dead_links``
+                a list([(x, y, z, link), ...]) giving the locations of
+                known-dead links from the perspective of the sender.
+                Links to dead boards may or may not be included in this list.
         """
         out = []
         for machine in self._controller.list_machines():
             machine = machine._asdict()
             machine["tags"] = list(machine["tags"])
             machine["dead_boards"] = list(machine["dead_boards"])
             machine["dead_links"] = [(x, y, z, int(link))
                                      for x, y, z, link
                                      in machine["dead_links"]]
             out.append(machine)
         return out
 
-    @_command
-    def get_board_position(self, client, machine_name, x, y, z):
-        """Get the physical location of a specified board.
-
-        Parameters
-        ----------
-        machine_name : str
-            The name of the machine containing the board.
-        x, y, z : int
-            The logical board location within the machine.
-
-        Returns
-        -------
-        (cabinet, frame, board) or None
-            The physical location of the board at the specified location or
-            None if the machine/board are not recognised.
+    @spalloc_command
+    def get_board_position(self, _client, machine_name, x, y, z):
+        """ Get the physical location of a specified board.
+
+        :param str machine_name: The name of the machine containing the board.
+        :param int x: Logical address within machine: first coordinate.
+        :param int y: Logical address within machine: second coordinate.
+        :param int z: Logical address within machine: third coordinate.
+        :return:
+            The physical location of the board (cabinet, frame, board) at the
+            specified location or None if the machine/board are not recognised.
+        :rtype: list(int) or None
         """
         return self._controller.get_board_position(machine_name, x, y, z)
 
-    @_command
-    def get_board_at_position(self, client, machine_name, x, y, z):
-        """Get the logical location of a board at the specified physical
-        location.
-
-        Parameters
-        ----------
-        machine_name : str
-            The name of the machine containing the board.
-        cabinet, frame, board : int
-            The physical board location within the machine.
-
-        Returns
-        -------
-        (x, y, z) or None
-            The logical location of the board at the specified location or None
-            if the machine/board are not recognised.
+    @spalloc_command
+    def get_board_at_position(self, _client, machine_name, x, y, z):
+        """ Get the logical location of a board at the specified physical\
+            location.
+
+        :param str machine_name: The name of the machine containing the board.
+        :param int x: Physical address within machine: cabinet ID.
+        :param int y: Physical address within machine: frame ID.
+        :param int z: Physical address within machine: board ID.
+        :return:
+            The logical location of the board (a triple) at the specified
+            location or None if the machine/board are not recognised.
+        :rtype: list(int) or None
         """
         return self._controller.get_board_at_position(machine_name, x, y, z)
 
-    @_command
-    def where_is(self, client, **kwargs):
-        """Find out where a SpiNNaker board or chip is located, logically and
-        physically.
+    @spalloc_command
+    def where_is(self, _client, **kwargs):
+        """ Find out where a SpiNNaker board or chip is located, logically and\
+            physically.
 
         May be called in one of the following styles::
 
             >>> # Query by logical board coordinate within a machine.
             >>> where_is(machine=..., x=..., y=..., z=...)
 
             >>> # Query by physical board location within a machine.
@@ -975,88 +1030,108 @@
             >>> # one large machine).
             >>> where_is(machine=..., chip_x=..., chip_y=...)
 
             >>> # Query by chip coordinate, within the boards allocated to a
             >>> # job.
             >>> where_is(job_id=..., chip_x=..., chip_y=...)
 
-        Returns
-        -------
-        {"machine": ..., "logical": ..., "physical": ..., "chip": ..., \
-                "board_chip": ..., "job_chip": ..., "job_id": ...} or None
-            If a board exists at the supplied location, a dictionary giving the
-            location of the board/chip, supplied in a number of alternative
-            forms. If the supplied coordinates do not specify a specific chip,
-            the chip coordinates given are those of the Ethernet connected chip
-            on that board.
+        Only these patterns of use are supported; all keyword arguments\
+        listed above are mandatory when used for a particular query.
 
-            If no board exists at the supplied position, None is returned
+        :rtype: dict(str, ...) or None
+        :return:
+            If a board exists at the supplied location, a dictionary giving
+            the location of the board/chip, supplied in a number of
+            alternative forms. If the supplied coordinates do not specify a
+            specific chip, the chip coordinates given are those of the
+            Ethernet connected chip on that board.
+
+            If no board exists at the supplied position, ``None`` is returned
             instead.
 
-            ``machine`` gives the name of the machine containing the board.
+            The dictionary will have the following keys:
+
+            ``machine``
+                the name of the machine containing the board.
 
-            ``logical`` the logical board coordinate, (x, y, z) within the
-            machine.
+            ``logical``
+                the logical board coordinate, (x, y, z) within the machine.
 
-            ``physical`` the physical board location, (cabinet, frame, board),
-            within the machine.
+            ``physical``
+                the physical board location, (cabinet, frame, board),
+                within the machine.
 
-            ``chip`` the coordinates of the chip, (x, y), if the whole machine
-            were booted as a single machine.
+            ``chip``
+                the coordinates of the chip, (x, y), if the whole machine
+                were booted as a single machine.
 
-            ``board_chip`` the coordinates of the chip, (x, y), within its
-            board.
+            ``board_chip``
+                the coordinates of the chip, (x, y), within its board.
 
-            ``job_id`` is the job ID of the job currently allocated to the
-            board identified or None if the board is not allocated to a job.
+            ``job_id``
+                the job ID of the job currently allocated to the board
+                identified or ``None`` if the board is not allocated to a job.
 
-            ``job_chip`` the coordinates of the chip, (x, y), within its
-            job, if a job is allocated to the board or None otherwise.
+            ``job_chip``
+                the coordinates of the chip, (x, y), within its job,
+                if a job is allocated to the board, or ``None`` otherwise.
         """
         return self._controller.where_is(**kwargs)
 
 
 def main(args=None):
-    """Command-line launcher for the server.
+    """ Command-line launcher for the server.
 
-    The server may be cleanly terminated using a keyboard interrupt (e.g.
-    ctrl+c).
+    The server may be cleanly terminated using a keyboard interrupt (e.g.,\
+    :kbd:`Ctrl+c`), and may be told to reload its configuration via `SIGHUP`.
 
-    Parameters
-    ----------
-    args : [arg, ...]
-        The command-line arguments passed to the program.
+    :param args: The command-line arguments passed to the program.
     """
-    parser = argparse.ArgumentParser(
+    parser = ArgumentParser(
         description="Start a SpiNNaker machine partitioning server.")
     parser.add_argument("--version", "-V", action="version",
                         version="%(prog)s {}".format(__version__))
     parser.add_argument("--quiet", "-q", action="store_true",
                         help="hide non-error output")
     parser.add_argument("config", type=str,
                         help="configuration filename to use for the server.")
     parser.add_argument("--cold-start", action="store_true",
                         default=False,
                         help="force a cold start, erasing any existing "
                              "saved state")
+    parser.add_argument("--port", "-p", type=int, default=22244,
+                        help="port to run the service on")
     args = parser.parse_args(args)
 
     if not args.quiet:
-        logging.basicConfig(level=logging.INFO)
+        log.basicConfig(
+            level=log.INFO,
+            format="%(asctime)s: %(name)s: %(levelname)s: %(message)s")
 
-    server = Server(config_filename=args.config,
-                    cold_start=args.cold_start)
     try:
+        server = SpallocServer(config_filename=args.config,
+                               cold_start=args.cold_start, port=args.port)
         # NB: Originally this loop was replaced with a call to server.join
-        # however in Python 2, such blocking calls are not interruptable so we
+        # however in Python 2, such blocking calls are not interruptible so we
         # use this rather ugly workaround instead.
         while server.is_alive():  # pragma: no cover
-            time.sleep(0.1)
+            try:
+                sleep(0.1)
+            except IOError:
+                pass
+    except _CriticalStop as e:
+        # NB: No stack trace from a critical stop! The code that threw should
+        # have logged the issue if a trace was relevant.
+        log.error(str(e))
+        return 1
     except KeyboardInterrupt:
         server.stop_and_join()
+    except Exception:  # pylint: disable=broad-except
+        log.exception("unexpected failure")
+        return 2
 
     return 0
 
 
 if __name__ == "__main__":  # pragma: no cover
     import sys
     sys.exit(main())
```

### Comparing `spalloc_server-0.5.2/spalloc_server/async_bmp_controller.py` & `spalloc_server-1!7.0.0a4/spalloc_server/async_bmp_controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,305 +1,343 @@
-"""Provide (basic) asynchronous control over a BMP responsible for controlling
+# Copyright (c) 2016 The University of Manchester
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+""" Provide (basic) asynchronous control over a BMP responsible for controlling
 a whole rack.
 """
-
 import threading
-
+import logging
 from collections import namedtuple, deque
+from spinnman.exceptions import SpallocException
+from spinnman.transceiver import create_transceiver_from_hostname
+from spinnman.model import BMPConnectionData
+from spinnman.constants import SCP_SCAMP_PORT
+from .links import Links
+import time
 
-from rig.links import Links
-from rig.machine_control import BMPController
+# The first BMP version with FPGA register support
+_BMP_VER_MIN = 2
 
-import logging
+_N_FPGA_RETRIES = 3
+
+_N_REQUEST_TRIES = 2
+
+_SECONDS_BETWEEN_TRIES = 15
 
 
 class AsyncBMPController(object):
-    """An object which provides an asynchronous interface to a power and link
+    """ An object which provides an asynchronous interface to a power and link
     control commands of a SpiNNaker BMP.
 
     Since BMP commands, particularly power-on commands, take some time to
     complete, it is desirable for them to be executed asynchronously. This
-    object uses a Rig :py:class:`~rig.machine_control.BMPController` object to
-    communicate with a BMP controlling a single frame of boards.
+    object uses a SpiNNMan :py:class:`~spinnman.transceiver.Transceiver` object
+    to communicate with a BMP controlling a single frame of boards.
 
     Power and link configuration commands are queued and executed in a
     background thread. When a command completes, a user-supplied callback is
     called.
 
     Sequential power commands of the same type (on/off) are coalesced into a
     single power on command. When a power command is sent, all previous link
     configuration commands queued for that board are skipped. Additionally, all
     power commands are completed before link configuration commands are carried
     out.
     """
 
     def __init__(self, hostname, on_thread_start=None):
-        """Start a new asynchronous BMP Controller
+        """ Start a new asynchronous BMP Controller
 
         Parameters
         ----------
         hostname : str
             The hostname/IP of the BMP to connect to.
         on_thread_start : function() or None
             *Optional.* A function to be called by the controller's background
-            thread before it starts. This can be used to ensure propper
+            thread before it starts. This can be used to ensure proper
             sequencing/handing-over between two AsyncBMPControllers connected
             to the same machine.
         """
         self._on_thread_start = on_thread_start
 
-        self._bc = BMPController(hostname)
+        self._transceiver = create_transceiver_from_hostname(
+            None, 5, bmp_connection_data=[
+                BMPConnectionData(0, 0, hostname, [0], SCP_SCAMP_PORT)])
+        self._hostname = hostname
 
         self._stop = False
 
         # A lock which must be held when modifying the state of this object
         self._lock = threading.RLock()
 
         # An event fired whenever some new interaction with the BMP is
         # required.
         self._requests_pending = threading.Event()
 
-        # A queue of power change states
-        self._power_requests = deque()
-
-        # A queue of link-enabled state changes
-        self._link_requests = deque()
+        # A queue of requests to be done
+        self._requests = deque()
 
         self._thread = threading.Thread(
             target=self._run,
             name="<BMP control thread for {}>".format(hostname))
         self._thread.start()
 
     def __enter__(self):
-        """When used as a context manager, make requests 'atomic'."""
+        """ When used as a context manager, make requests 'atomic'.
+        """
         self._lock.acquire()
 
-    def __exit__(self, type=None, value=None, traceback=None):
+    def __exit__(self, _type=None, _value=None, _traceback=None):
         self._lock.release()
+        return False
 
-    def set_power(self, board, state, on_done):
-        """Set the power state of a single board.
-
-        Parameters
-        ----------
-        board : int
-            The board to control.
-        state : bool
-            True = on, False = off.
-        on_done : function(success)
-            Function to call when the command completes. May be called from
-            another thread. Success is a bool which is True if the command
-            completed successfully and False if it did not (or was cancelled).
+    def add_requests(self, atomic_requests):
+        """ Add an atomic request to be performed
         """
         with self._lock:
             assert not self._stop
-
-            # Enqueue the request
-            self._power_requests.append(_PowerRequest(state, board, on_done))
-            self._requests_pending.set()
-
-            # Cancel any existing link enable commands for this board
-            cancelled = []
-            for request in list(self._link_requests):
-                if request.board == board:
-                    self._link_requests.remove(request)
-                    cancelled.append(request)
-
-        for request in cancelled:
-            request.on_done(False)
-
-    def set_link_enable(self, board, link, enable, on_done):
-        """Enable or disable a link.
-
-        Parameters
-        ----------
-        board : int
-            The board on which the link resides.
-        link : :py:class:`rig.links.Links`
-            The link to configure.
-        enable : bool
-            True = link enabled, False = link disabled.
-        on_done : function(success)
-            Function to call when the command completes. May be called from
-            another thread. Success is a bool which is True if the command
-            completed successfully and False if it did not (or was cancelled).
-        """
-        with self._lock:
-            assert not self._stop
-
-            # Enqueue the request
-            self._link_requests.append(
-                _LinkRequest(board, link, enable, on_done))
+            self._requests.append(atomic_requests)
             self._requests_pending.set()
 
     def stop(self):
-        """Stop the background thread, as soon as possible after completing all
-        queued actions.
+        """ Stop the background thread, as soon as possible after completing\
+            all queued actions.
         """
         with self._lock:
             self._stop = True
             self._requests_pending.set()
 
     def join(self):
-        """Wait for the thread to actually stop."""
+        """ Wait for the thread to actually stop.
+        """
         self._thread.join()
 
+    def _good_fpga(self, board, fpga):
+        fpga_id = self._transceiver.read_fpga_register(
+            fpga_num=fpga, register=_FPGA_FLAG_REGISTER_ADDRESS,
+            board=board, cabinet=0, frame=0)
+        ok = (fpga_id & _FPGA_FLAG_ID_MASK) == fpga
+        if not ok:  # pragma: no cover
+            logging.warning(
+                "FPGA %d on board %d of %s has incorrect FPGA ID flag %d",
+                fpga, board, self._hostname, fpga_id & _FPGA_FLAG_ID_MASK)
+        return ok
+
+    def _power_on_and_check(self, boards):
+        # FPGAs are checked after power on - assume incorrect to start
+        boards_to_power = boards
+        for _try in range(_N_FPGA_RETRIES):
+            # Power on - note don't need to power off if in subsequent
+            # run of the loop as the BMP handles this correctly
+            self._transceiver.power_on(
+                boards=boards_to_power, frame=0, cabinet=0)
+
+            # Check if the FPGA number is correct on each FPGA
+            retry_boards = []
+            for board in boards_to_power:
+                # skip board if old BMP version
+                vi = self._transceiver.read_bmp_version(
+                    board=board, frame=0, cabinet=0)
+                if vi.version_number[0] < _BMP_VER_MIN:
+                    continue
+
+                # check each FPGA on board
+                if not all(self._good_fpga(board, fpga)
+                           for fpga in range(_N_FPGAS)):
+                    retry_boards.append(board)
+
+            # try again with incorrect boards only
+            if not len(retry_boards):
+                return
+            boards_to_power = retry_boards
+        raise SpallocException(
+            "Could not get correct FPGA ID after {} tries".format(
+                _N_FPGA_RETRIES))
+
+    def _set_link_state(self, link, enable, board):
+        """ Set the power state of a link.
+
+        :param link: The link (direction) to set the enable-state of.
+        :type link: value in Links enum
+        :param state: What to set the state to. True for on, False for off.
+        :type state: bool
+        :param board: Which board or boards to set the link enable-state of.
+        :type board: int or iterable
+        """
+        # skip FPGA link configuration if old BMP version
+        vi = self._transceiver.read_bmp_version(
+            board=board, frame=0, cabinet=0)
+        if vi.version_number[0] < _BMP_VER_MIN:
+            return
+
+        fpga, addr = FPGA_LINK_STOP_REGISTERS[link]
+        self._transceiver.write_fpga_register(
+            fpga, addr, int(not enable), board=board, frame=0, cabinet=0)
+
     def _run(self):
-        """The background thread for interacting with the BMP.
+        """ The background thread for interacting with the BMP.
         """
         try:
             if self._on_thread_start is not None:
                 self._on_thread_start()
 
             while True:
                 self._requests_pending.wait()
 
-                # Priority 0: Power commands
-                power_request = self._get_atomic_power_request()
-                if power_request:
-                    # Send the power command
-                    try:
-                        self._bc.set_power(state=power_request.state,
-                                           board=power_request.board)
-                        success = True
-                    except IOError:
-                        # Communication issue with the machine, log it but not
-                        # much we can do for the end-user.
-                        logging.exception("Failed to set board power.")
-                        success = False
-
-                    # Alert all waiting threads
-                    for on_done in power_request.on_done:
-                        on_done(success)
-
-                    continue
-
-                # Priority 1: Link enable/disable commands
-                link_request = self._get_atomic_link_request()
-                if link_request:
-                    # Set the link state, as required
-                    try:
-                        fpga, addr \
-                            = FPGA_LINK_STOP_REGISTERS[link_request.link]
-                        self._bc.write_fpga_reg(fpga, addr,
-                                                not link_request.enable,
-                                                board=link_request.board)
-                        success = True
-                    except IOError:
-                        # Communication issue with the machine, log it but not
-                        # much we can do for the end-user.
-                        logging.exception("Failed to set link state.")
-                        success = False
-
-                    # Alert waiting thread
-                    link_request.on_done(success)
+                if self._requests:
+                    request = self._requests.popleft()
 
-                    continue
+                    for n_tries in range(_N_REQUEST_TRIES):
+                        try:
+                            # Send any power on commands
+                            if request.power_on_boards:
+                                self._power_on_and_check(
+                                    request.power_on_boards)
+
+                            # Process link requests next
+                            for link_request in request.link_requests:
+                                # Set the link state, as required
+                                self._set_link_state(
+                                    link_request.link, link_request.enable,
+                                    link_request.board)
+
+                            # Finally send any power off commands
+                            if request.power_off_boards:
+                                self._transceiver.power_off(
+                                    boards=request.power_off_boards,
+                                    frame=0, cabinet=0)
+
+                            # Exit the retry loop if the requests all worked
+                            request.on_done(True, None)
+                            break
+                        except Exception as e:  # pylint: disable=broad-except
+                            if n_tries + 1 == _N_REQUEST_TRIES:
+                                reason = "Requests failed on BMP {}".format(
+                                    self._hostname)
+                                logging.exception("%s: %s", reason, str(e))
+                                request.on_done(False, reason)
+                                break
+                            logging.exception(
+                                "Retrying requests on BMP %s after %d"
+                                " seconds: %s",
+                                self._hostname, _SECONDS_BETWEEN_TRIES,
+                                str(e))
+                            time.sleep(_SECONDS_BETWEEN_TRIES)
 
                 # If nothing left in the queues, clear the request flag and
                 # break out of queue-processing loop.
                 with self._lock:
-                    if (not self._power_requests and  # pragma: no branch
-                            not self._link_requests):
+                    if not self._requests:
                         self._requests_pending.clear()
 
                         # If we've been told to stop, actually stop the thread
                         # now
                         if self._stop:  # pragma: no branch
                             return
-        except:  # pragma: no cover
+        except Exception:  # pragma: no cover
             # If the thread crashes something has gone wrong with this program
             # (not the machine), setting _stop will cause set_power and
-            # set_link_enable to fail, hopefully propogating news of this
+            # set_link_enable to fail, hopefully propagating news of this
             # crash..
             with self._lock:
                 self._stop = True
             raise
 
-    def _get_atomic_power_request(self):
-        """If any power requests are outstanding, return a (boards, state)
-        tuple which combines as many of the requests at the head of the queue
-        as possible.
-
-        Returns
-        -------
-        :py:class:`._PowerRequest` or None
-        """
-        with self._lock:
-            # Special case: no requests
-            if not self._power_requests:
-                return None
-
-            # Otherwise, accumulate as many boards as possible
-            state = self._power_requests[0].state
-            boards = set()
-            on_done = []
-            while (self._power_requests and
-                   self._power_requests[0].state == state):
-                request = self._power_requests.popleft()
-                boards.add(request.board)
-                on_done.append(request.on_done)
-            return _PowerRequest(state, boards, on_done)
-
-    def _get_atomic_link_request(self):
-        """Pop the next link state change request, if one exists.
-
-        Returns
-        -------
-        :py:class:`._LinkRequest` or None
-        """
-        with self._lock:
-            if not self._link_requests:
-                return None
-            else:
-                return self._link_requests.popleft()
-
+    @property
+    def hostname(self):
+        return self._hostname
 
-class _PowerRequest(namedtuple("_PowerRequest", "state board on_done")):
-    """Reuqests that a specific board should have its power state set to a
-    particular value.
 
-    Parameters
-    ----------
-    state : bool
-        On (True) or off (False).
-    board : int
-        Board to change the state of
-    on_done : function(success)
-        A function to call when the request has been completed.
+class AtomicRequests(object):
+    """ A list of requests that need to be done atomically; these are carried
+        out in order of power on, link enable or disable, power off
     """
 
-    # Python 3.4 Workaround: https://bugs.python.org/issue24931
-    __slots__ = tuple()
+    __slots__ = [
+        "_on_done",
+        "_power_on_boards",
+        "_power_off_boards",
+        "_link_requests"
+    ]
+
+    def __init__(self, on_done):
+        self._on_done = on_done
+        self._power_on_boards = list()
+        self._power_off_boards = list()
+        self._link_requests = list()
+
+    def power(self, board, power):
+        if power:
+            self._power_on_boards.append(board)
+        else:
+            self._power_off_boards.append(board)
+
+    def link(self, board, link, enable):
+        self._link_requests.append(LinkRequest(board, link, enable))
+
+    @property
+    def on_done(self):
+        return self._on_done
+
+    @property
+    def power_on_boards(self):
+        return self._power_on_boards
+
+    @property
+    def power_off_boards(self):
+        return self._power_off_boards
+
+    @property
+    def link_requests(self):
+        return self._link_requests
 
 
-class _LinkRequest(namedtuple("_LinkRequest", "board link enable on_done")):
-    """Reuqests that a specific board should have its power state set to a
+class LinkRequest(namedtuple("LinkRequest", "board link enable")):
+    """ Requests that a specific board should have its power state set to a
     particular value.
 
     Parameters
     ----------
     board : int
         Board whose link should be blocked/unblocked
-    link : :py:class:`rig.links.Link`
+    link : :py:class:`spalloc_server.links.Link`
         The link whose state should be changed
     enable : bool
         State of the link: Enabled (True), disabled (False).
-    on_done : function(success)
-        A function to call when the request has been completed.
     """
 
     # Python 3.4 Workaround: https://bugs.python.org/issue24931
     __slots__ = tuple()
 
+
+# The number of FPGAs
+_N_FPGAS = 3
+
+# The FLAG register address in the FPGAs
+_FPGA_FLAG_REGISTER_ADDRESS = 0x40004
+
+# The FPGA ID field within the FLAG register value
+_FPGA_FLAG_ID_MASK = 0x3
+
 # Gives the FPGA number and register addresses for the STOP register (which
 # disables outgoing traffic on a high-speed link) for each link direction.
 # https://github.com/SpiNNakerManchester/spio/tree/master/designs/spinnaker_fpgas#spi-interface
-REG_STOP_OFFSET = 0x5C
+_REG_STOP_OFFSET = 0x5C
 FPGA_LINK_STOP_REGISTERS = {
-    Links.east: (0, 0x00000000 + REG_STOP_OFFSET),
-    Links.south: (0, 0x00010000 + REG_STOP_OFFSET),
-    Links.south_west: (1, 0x00000000 + REG_STOP_OFFSET),
-    Links.west: (1, 0x00010000 + REG_STOP_OFFSET),
-    Links.north: (2, 0x00000000 + REG_STOP_OFFSET),
-    Links.north_east: (2, 0x00010000 + REG_STOP_OFFSET),
+    Links.east: (0, 0x00000000 + _REG_STOP_OFFSET),
+    Links.south: (0, 0x00010000 + _REG_STOP_OFFSET),
+    Links.south_west: (1, 0x00000000 + _REG_STOP_OFFSET),
+    Links.west: (1, 0x00010000 + _REG_STOP_OFFSET),
+    Links.north: (2, 0x00000000 + _REG_STOP_OFFSET),
+    Links.north_east: (2, 0x00010000 + _REG_STOP_OFFSET),
 }
```

### Comparing `spalloc_server-0.5.2/spalloc_server/controller.py` & `spalloc_server-1!7.0.0a4/spalloc_server/controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,50 @@
-"""A high-level control interface for scheduling and allocating jobs and
+# Copyright (c) 2016 The University of Manchester
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+""" A high-level control interface for scheduling and allocating jobs and
 managing hardware in a collection of SpiNNaker machines.
 """
-
-import threading
-
-from enum import IntEnum
-
 from collections import namedtuple, OrderedDict, defaultdict
-
-from functools import partial
-
-from six import itervalues, iteritems
-
-import time
-
 from datetime import datetime
-
+from enum import IntEnum
+import logging
+from logging.handlers import TimedRotatingFileHandler
+from threading import RLock
+from time import time as timestamp
+from functools import partial
 from pytz import utc
-
-from rig.geometry import spinn5_chip_coord
-
-from spalloc_server.coordinates import \
-    board_to_chip, chip_to_board, triad_dimensions_to_chips, WrapAround
-from spalloc_server.job_queue import JobQueue
-from spalloc_server.async_bmp_controller import AsyncBMPController
+from spinn_machine import SpiNNakerTriadGeometry
+from .coordinates import (
+    board_to_chip, chip_to_board, triad_dimensions_to_chips, WrapAround)
+from .job_queue import JobQueue
+from .async_bmp_controller import AsyncBMPController, AtomicRequests
+
+job_log = logging.Logger("jobs")
+job_log.propagate = False
+job_log_handler = TimedRotatingFileHandler(
+    "spalloc_jobs.log", when="D")
+job_log_formatter = logging.Formatter('%(asctime)s: %(message)s')
+job_log_handler.setFormatter(job_log_formatter)
+job_log.addHandler(job_log_handler)
 
 
 class Controller(object):
-    """An object which allocates jobs to machines and manages said machines'
+    """ An object which allocates jobs to machines and manages said machines'
     hardware.
 
     This object is intended to form the core of a server which manages the
     queueing and execution of jobs on several SpiNNaker machines at once using
     a :py:class:`~spalloc_server.job_queue.JobQueue` and interacts with
     the hardware of said machines using
     :py:class:`~spalloc_server.async_bmp_controller.AsyncBMPController`.
@@ -96,35 +109,40 @@
         object.
 
         Note that this attribute is not pickled and unpicking a controller sets
         this attribute to None.
     """
 
     def __init__(self, next_id=1, max_retired_jobs=1200,
-                 on_background_state_change=None):
+                 on_background_state_change=None,
+                 seconds_before_free=30):
         """
         Parameters
         ----------
-        next_id : int
+        next_id : int, optional
             The next Job ID to assign
-        max_retired_jobs : int
+        max_retired_jobs : int, optional
             See attribute of same name.
-        on_background_state_change : function
+        on_background_state_change : function, optional
             See attribute of same name.
+        seconds_before_free : int
+            The number of seconds between a board being freed and it becoming
+            available again
         """
         # The next job ID to assign
         self._next_id = next_id
 
         self._on_background_state_change = on_background_state_change
 
         # The job queue which manages the scheduling and
         # allocation of all jobs.
         self._job_queue = JobQueue(self._job_queue_on_allocate,
                                    self._job_queue_on_free,
-                                   self._job_queue_on_cancel)
+                                   self._job_queue_on_cancel,
+                                   seconds_before_free)
 
         # The machines available.
         # {name: Machine, ...}
         self._machines = OrderedDict()
 
         # The jobs which are currently queued or allocated.
         # {id: _Job, ...}
@@ -152,15 +170,15 @@
         # The connections to BMPs in the system.
         # {machine_name: {(c, f): AsyncBMPController, ...}, ...}
         self._bmp_controllers = None
 
         self._init_dynamic_state()
 
     def __getstate__(self):
-        """Called when pickling this object.
+        """ Called when pickling this object.
 
         This object may only be pickled once :py:meth:`.stop` and
         :py:meth:`.join` have returned.
         """
         state = self.__dict__.copy()
 
         # Do not keep the reference to any state-change callbacks
@@ -169,15 +187,15 @@
         # Do not keep references to unpickleable dynamic state
         state["_bmp_controllers"] = None
         state["_lock"] = None
 
         return state
 
     def __setstate__(self, state):
-        """Called when unpickling this object.
+        """ Called when unpickling this object.
 
         Note that though the object must be pickled when stopped, the unpickled
         object will start running immediately.
         """
         self.__dict__.update(state)
 
         # Restore callback function pointers in JobQueue (removed by JobQueue
@@ -186,39 +204,39 @@
         self._job_queue.on_allocate = self._job_queue_on_allocate
         self._job_queue.on_free = self._job_queue_on_free
         self._job_queue.on_cancel = self._job_queue_on_cancel
 
         self._init_dynamic_state()
 
     def stop(self):
-        """Request that all background threads stop.
+        """ Request that all background threads stop.
 
         This will cause all outstanding BMP commands to be flushed.
 
         .. warning::
 
             Apart from :py:meth:`.join`, no methods of this controller object
             may be called once this method has been called.
 
         See Also
         --------
         join: to wait for the threads to actually terminate.
         """
         # Stop the BMP controllers
         for machine in self._machines:
-            for controller in itervalues(self._bmp_controllers[machine]):
+            for controller in self._bmp_controllers[machine].values():
                 controller.stop()
 
     def join(self):
-        """Block until all background threads have halted and all queued BMP
+        """ Block until all background threads have halted and all queued BMP
         commands completed.
         """
         # Wait for the BMP controller threads
-        for controllers in itervalues(self._bmp_controllers):
-            for controller in itervalues(controllers):
+        for controllers in self._bmp_controllers.values():
+            for controller in controllers.values():
                 controller.join()
 
     @property
     def on_background_state_change(self):
         with self._lock:
             return self._on_background_state_change
 
@@ -242,15 +260,15 @@
     @property
     def machines(self):
         with self._lock:
             return self._machines.copy()
 
     @machines.setter
     def machines(self, machines):
-        """Update the set of machines available to the controller.
+        """ Update the set of machines available to the controller.
 
         Attempt to update the information about available machines without
         destroying jobs where possible. Machines are matched with existing
         machines by name and are only recreated if dimensions or connectivity
         information is altered.
 
         Note that changing the tags, set of dead boards or set of dead links
@@ -307,15 +325,15 @@
                     # Remove the machine from the queue causing all jobs
                     # allocated on it to be freed and all boards powered down.
                     self._job_queue.remove_machine(name)
 
                     # Remove the board and its BMP connections
                     old = self._machines.pop(name)
                     shut_down_controllers.extend(
-                        itervalues(self._bmp_controllers.pop(name)))
+                        self._bmp_controllers.pop(name).values())
 
                 # Shut-down the now defunct controllers
                 for controller in shut_down_controllers:
                     controller.stop()
 
                 def wait_for_old_controllers_to_shutdown():
                     # All new BMPControllers must wait for all the old
@@ -344,18 +362,15 @@
                                                 height=new.height,
                                                 tags=new.tags,
                                                 dead_boards=new.dead_boards,
                                                 dead_links=new.dead_links)
 
                 # Re-order machines to match the specification
                 for name in machines:
-                    # Python 2.7 does not have move_to_end
-                    m = self._machines.pop(name)
-                    self._machines[name] = m
-
+                    self._machines.move_to_end(name)
                     self._job_queue.move_machine_to_end(name)
 
             # Mark all effected machines as changed
             self._changed_machines.update(added)
             self._changed_machines.update(changed)
             self._changed_machines.update(removed)
 
@@ -369,16 +384,16 @@
     @property
     def changed_machines(self):
         with self._lock:
             changed_machines = self._changed_machines
             self._changed_machines = set()
             return changed_machines
 
-    def create_job(self, *args, **kwargs):
-        """Create a new job (i.e. allocation of boards).
+    def create_job(self, ownerhost, *args, **kwargs):
+        """ Create a new job (i.e. allocation of boards).
 
         This function is a wrapper around
         :py:meth:`JobQueue.create_job()
         <spalloc_server.job_queue.JobQueue.create_job>` which
         automatically selects (and returns) a new job_id. As such, the
         following *additional* (keyword) arguments are accepted:
 
@@ -392,66 +407,69 @@
             no timeout is used. (Default: 60.0)
 
         Returns
         -------
         job_id : int
             The Job ID assigned to the job.
         """
-        with self._lock:
-            # Extract non-allocator arguments
-            owner = kwargs.pop("owner", None)
-            if owner is None:
-                raise TypeError("owner must be specified for all jobs.")
-            keepalive = kwargs.pop("keepalive", 60.0)
+        job_log.info("create_job(%s,%s) from %s", args, kwargs, ownerhost)
+        # Extract non-allocator arguments
+        owner = kwargs.pop("owner")
+        keepalive = kwargs.pop("keepalive")
 
+        with self._lock:
             # Generate a job ID
             job_id = self._next_id
             self._next_id += 1
 
             kwargs["job_id"] = job_id
 
             # Create job and begin attempting to allocate it
-            job = _Job(id=job_id, owner=owner,
+            job = _Job(_id=job_id, owner=owner,
                        keepalive=keepalive,
+                       lasthost=ownerhost,
                        args=args, kwargs=kwargs)
             self._jobs[job_id] = job
             self._job_queue.create_job(*args, **kwargs)
 
             self._changed_jobs.add(job_id)
 
             return job_id
 
-    def job_keepalive(self, job_id):
-        """Reset the keepalive timer for the specified job.
+    def job_keepalive(self, clienthost, job_id):
+        """ Reset the keepalive timer for the specified job.
 
         Note all other job-specific functions implicitly call this method.
         """
         with self._lock:
             job = self._jobs.get(job_id, None)
-            if job is not None and job.keepalive is not None:
-                job.keepalive_until = time.time() + job.keepalive
+            if job is not None:
+                job.update_keepalive(clienthost)
 
-    def get_job_state(self, job_id):
-        """Poll the state of a running job.
+    def get_job_state(self, clienthost, job_id):
+        """ Poll the state of a running job.
 
         Returns
         -------
         :py:class:`.JobStateTuple`
         """
         with self._lock:
-            self.job_keepalive(job_id)
+            self.job_keepalive(clienthost, job_id)
 
             job = self._jobs.get(job_id)
+            host = None
             if job is not None:
                 # Job is live
                 state = job.state
                 power = job.power
                 keepalive = job.keepalive
                 reason = None
                 start_time = job.start_time
+                host = job.lasthost
+                # Note that we update the keepalive after the readout
             elif job_id in self._retired_jobs:
                 # Job has been destroyed at some point
                 state = JobState.destroyed
                 power = None
                 keepalive = None
                 reason = self._retired_jobs[job_id]
                 start_time = None
@@ -459,125 +477,136 @@
                 # Job ID not recognised
                 state = JobState.unknown
                 power = None
                 keepalive = None
                 reason = None
                 start_time = None
 
-            return JobStateTuple(state, power, keepalive, reason, start_time)
+        return JobStateTuple(state, power, keepalive, reason, start_time, host)
 
-    def get_job_machine_info(self, job_id):
-        """Get information about the machine the job has been allocated.
+    def get_job_machine_info(self, clienthost, job_id):
+        """ Get information about the machine the job has been allocated.
 
         Returns
         -------
         :py:class:`.JobMachineInfoTuple`
         """
         with self._lock:
-            self.job_keepalive(job_id)
+            self.job_keepalive(clienthost, job_id)
 
             job = self._jobs.get(job_id, None)
             if job is not None and job.boards is not None:
                 return JobMachineInfoTuple(
                     job.width, job.height,
                     job.connections,
                     job.allocated_machine.name,
                     job.boards)
-            else:
-                # Job doesn't exist or no boards allocated yet
-                return JobMachineInfoTuple(None, None, None, None, None)
+        # Job doesn't exist or no boards allocated yet
+        return JobMachineInfoTuple(None, None, None, None, None)
 
-    def power_on_job_boards(self, job_id):
-        """Power on (or reset if already on) boards associated with a job."""
+    def power_on_job_boards(self, clienthost, job_id):
+        """ Power on (or reset if already on) boards associated with a job.
+        """
+        job_log.info("power_job(%s,On) from %s", job_id, clienthost)
         with self._lock:
-            self.job_keepalive(job_id)
+            self.job_keepalive(clienthost, job_id)
 
             job = self._jobs.get(job_id)
             if job is not None and job.boards is not None:
                 self._set_job_power_and_links(
                     job, power=True, link_enable=False)
 
-    def power_off_job_boards(self, job_id):
-        """Power off boards associated with a job."""
+    def power_off_job_boards(self, clienthost, job_id):
+        """ Power off boards associated with a job.
+        """
+        job_log.info("power_job(%s,Off) from %s", job_id, clienthost)
         with self._lock:
-            self.job_keepalive(job_id)
+            self.job_keepalive(clienthost, job_id)
 
             job = self._jobs.get(job_id)
             if job is not None and job.boards is not None:
                 self._set_job_power_and_links(
                     job, power=False, link_enable=None)
 
-    def destroy_job(self, job_id, reason=None):
-        """Destroy a job.
+    def destroy_job(self, clienthost, job_id, reason=None):
+        """ Destroy a job.
 
         When the job is finished, or to terminate it early, this function
         releases any resources consumed by the job and removes it from any
         queues.
 
         Parameters
         ----------
-        reason : str or None
-            *Optional.* A human-readable string describing the reason for the
+        reason : str or None, optional
+            A human-readable string describing the reason for the
             job's destruction.
         """
+        if clienthost is None:
+            clienthost = "internal"
+        if reason is None:
+            job_log.info("destroy_job(%s) from %s", job_id, clienthost)
+        else:
+            job_log.info("destroy_job(%s,%s) from %s",
+                         job_id, reason, clienthost)
         with self._lock:
             job = self._jobs.get(job_id, None)
             if job is not None:
                 # Free the boards used by the job (the JobQueue will then call
                 # _job_queue_on_free which will trigger power-down and removal
                 # of the job from self._jobs).
                 self._job_queue.destroy_job(job_id, reason)
 
     def list_jobs(self):
-        """Enumerate all current jobs.
+        """ Enumerate all current jobs.
 
         Returns
         -------
-        jobs : [:py:class`.JobTuple`, ...]
+        jobs : [:py:class:`.JobTuple`, ...]
             A list of allocated/queued jobs in order of creation from oldest
             (first) to newest (last).
         """
         with self._lock:
             job_list = []
-            for job in itervalues(self._jobs):
+            for job in self._jobs.values():
                 # Strip "job_id" which is only used internally
-                kwargs = {k: v for k, v in iteritems(job.kwargs)
+                kwargs = {k: v for k, v in job.kwargs.items()
                           if k != "job_id"}
 
                 # Machine may not exist
                 allocated_machine_name = None
                 if job.allocated_machine is not None:
                     allocated_machine_name = job.allocated_machine.name
 
                 job_list.append(JobTuple(
                     job.id, job.owner, job.start_time, job.keepalive,
                     job.state, job.power, job.args, kwargs,
-                    allocated_machine_name, job.boards))
+                    allocated_machine_name, job.boards,
+                    str(job.lasthost) if job.lasthost is not None else ""))
 
             return job_list
 
     def list_machines(self):
-        """Enumerates all machines known to the system.
+        """ Enumerates all machines known to the system.
 
         Returns
         -------
         machines : [:py:class:`.MachineTuple`, ...]
             The list of machines known to the system in order of priority from
             highest (first) to lowest (last).
         """
         with self._lock:
             return [
                 MachineTuple(machine.name, machine.tags,
                              machine.width, machine.height,
                              machine.dead_boards, machine.dead_links)
-                for machine in itervalues(self._machines)
+                for machine in self._machines.values()
             ]
 
     def get_board_position(self, machine_name, x, y, z):
-        """Get the physical location of a specified board.
+        """ Get the physical location of a specified board.
 
         Parameters
         ----------
         machine_name : str
             The name of the machine containing the board.
         x, y, z : int
             The logical board location within the machine.
@@ -588,19 +617,18 @@
             The physical location of the board at the specified location or
             None if the machine/board are not recognised.
         """
         with self._lock:
             machine = self._machines.get(machine_name, None)
             if machine is None:
                 return None
-            else:
-                return machine.board_locations.get((x, y, z), None)
+            return machine.board_locations.get((x, y, z), None)
 
     def get_board_at_position(self, machine_name, cabinet, frame, board):
-        """Get the logical location of a board at the specified physical
+        """ Get the logical location of a board at the specified physical
         location.
 
         Parameters
         ----------
         machine_name : str
             The name of the machine containing the board.
         cabinet, frame, board : int
@@ -612,27 +640,251 @@
             The logical location of the board at the specified location or None
             if the machine/board are not recognised.
         """
         with self._lock:
             machine = self._machines.get(machine_name, None)
             if machine is None:
                 return None
-            else:
-                # NB: Assuming this function is only called very rarely,
-                # constructing and maintaining a reverse lookup is not worth
-                # the trouble so instead we just search.
-                for (x, y, z), (c, f, b) in iteritems(machine.board_locations):
-                    if (c, f, b) == (cabinet, frame, board):
-                        return (x, y, z)
-                else:
-                    # No board found
-                    return None
+            # NB: Assuming this function is only called very rarely,
+            # constructing and maintaining a reverse lookup is not worth
+            # the trouble so instead we just search.
+            for (x, y, z), (c, f, b) in machine.board_locations.items():
+                if (c, f, b) == (cabinet, frame, board):
+                    return (x, y, z)
+        # No board found
+        return None
+
+    def _job_for_location(self, machine, x, y, z):
+        """ Determine what job is running on the given board.
+        """
+        for job_id, job in self._jobs.items():
+            # NB: If machine is defined, boards must also be defined.
+            if (job.allocated_machine == machine and (x, y, z) in job.boards):
+                return job_id, job
+        # No job is allocated to the board
+        return None, None
+
+    def _where_is_by_logical_triple(self, machine_name, x, y, z):
+        """ Helper for :py:meth:`where_is`
+        """
+        with self._lock:
+            # Get the actual Machine
+            machine = self._machines.get(machine_name, None)
+            if machine is None:
+                return None
+
+            chip_x, chip_y = board_to_chip(x, y, z)
+
+            # Compensate chip coordinates for wrap-around
+            chip_w, chip_h = triad_dimensions_to_chips(
+                machine.width, machine.height, WrapAround.both)
+            chip_x %= chip_w
+            chip_y %= chip_h
+
+            # Determine the chip within the board
+            board_chip = SpiNNakerTriadGeometry.get_spinn5_geometry()\
+                .get_local_chip_coordinate(chip_x, chip_y)
+
+            # Determine the logical board coordinates (and compensate for
+            # wrap-around)
+            x, y, z = chip_to_board(chip_x, chip_y, chip_w, chip_h)
+
+            # Determine the board's physical location (fail if board does not
+            # exist)
+            cfb = machine.board_locations.get((x, y, z), None)
+            if cfb is None:  # pragma: no cover
+                return None
+            cabinet, frame, board = cfb
+
+            # Determine what job is running on that board
+            job_id, job = self._job_for_location(machine, x, y, z)
+
+            return {
+                "machine": machine_name,
+                "logical": (x, y, z),
+                "physical": (cabinet, frame, board),
+                "chip": (chip_x, chip_y),
+                "board_chip": board_chip,
+                "job_id": job_id,
+                "job_chip": self._get_job_chip(job, x, y, z, board_chip)
+            }
+
+    def _where_is_by_physical_triple(self, machine_name, cabinet, frame,
+                                     board):
+        """ Helper for :py:meth:`where_is`
+        """
+        with self._lock:
+            # Get the actual Machine
+            machine = self._machines.get(machine_name, None)
+            if machine is None:
+                return None
+
+            xyz = self.get_board_at_position(machine_name, cabinet, frame,
+                                             board)
+            if xyz is None:
+                return None
+            chip_x, chip_y = board_to_chip(*xyz)
+
+            # Compensate chip coordinates for wrap-around
+            chip_w, chip_h = triad_dimensions_to_chips(
+                machine.width, machine.height, WrapAround.both)
+            chip_x %= chip_w
+            chip_y %= chip_h
+
+            # Determine the chip within the board
+            board_chip = SpiNNakerTriadGeometry.get_spinn5_geometry()\
+                .get_local_chip_coordinate(chip_x, chip_y)
+
+            # Determine the logical board coordinates (and compensate for
+            # wrap-around)
+            x, y, z = chip_to_board(chip_x, chip_y, chip_w, chip_h)
+
+            # Determine the board's physical location (fail if board does not
+            # exist)
+            cfb = machine.board_locations.get((x, y, z), None)
+            if cfb is None:  # pragma: no cover
+                return None
+            cabinet, frame, board = cfb
+
+            # Determine what job is running on that board
+            job_id, job = self._job_for_location(machine, x, y, z)
+
+            return {
+                "machine": machine_name,
+                "logical": (x, y, z),
+                "physical": (cabinet, frame, board),
+                "chip": (chip_x, chip_y),
+                "board_chip": board_chip,
+                "job_id": job_id,
+                "job_chip": self._get_job_chip(job, x, y, z, board_chip)
+            }
+
+    def _where_is_by_chip_coordinate(self, machine_name, chip_x, chip_y):
+        """ Helper for :py:meth:`where_is`
+        """
+        with self._lock:
+            # Get the actual Machine
+            machine = self._machines.get(machine_name, None)
+            if machine is None:
+                return None
+
+            # Compensate chip coordinates for wrap-around
+            chip_w, chip_h = triad_dimensions_to_chips(
+                machine.width, machine.height, WrapAround.both)
+            chip_x %= chip_w
+            chip_y %= chip_h
+
+            # Determine the chip within the board
+            board_chip = SpiNNakerTriadGeometry.get_spinn5_geometry()\
+                .get_local_chip_coordinate(chip_x, chip_y)
+
+            # Determine the logical board coordinates (and compensate for
+            # wrap-around)
+            x, y, z = chip_to_board(chip_x, chip_y, chip_w, chip_h)
+
+            # Determine the board's physical location (fail if board does not
+            # exist)
+            cfb = machine.board_locations.get((x, y, z), None)
+            if cfb is None:
+                return None
+            cabinet, frame, board = cfb
+
+            # Determine what job is running on that board
+            job_id, job = self._job_for_location(machine, x, y, z)
+
+            return {
+                "machine": machine_name,
+                "logical": (x, y, z),
+                "physical": (cabinet, frame, board),
+                "chip": (chip_x, chip_y),
+                "board_chip": board_chip,
+                "job_id": job_id,
+                "job_chip": self._get_job_chip(job, x, y, z, board_chip)
+            }
+
+    def _where_is_by_job_chip_coordinate(self, job_id, chip_x, chip_y):
+        """ Helper for :py:meth:`where_is`
+        """
+        with self._lock:
+            # Covert from job-relative chip location
+            job = self._jobs.get(job_id, None)
+            if job is None or job.boards is None:
+                return None
+            machine_name = job.allocated_machine.name
+            job_x, job_y, job_z = map(min, zip(*job.boards))
+            dx, dy = board_to_chip(job_x, job_y, job_z)
+            chip_x += dx
+            chip_y += dy
+
+            # Get the actual Machine
+            machine = self._machines.get(machine_name, None)
+            if machine is None:  # pragma: no cover
+                return None
+
+            # Compensate chip coordinates for wrap-around
+            chip_w, chip_h = triad_dimensions_to_chips(
+                machine.width, machine.height, WrapAround.both)
+            chip_x %= chip_w
+            chip_y %= chip_h
+
+            # Determine the chip within the board
+            board_chip = SpiNNakerTriadGeometry.get_spinn5_geometry()\
+                .get_local_chip_coordinate(chip_x, chip_y)
+
+            # Determine the logical board coordinates (and compensate for
+            # wrap-around)
+            x, y, z = chip_to_board(chip_x, chip_y, chip_w, chip_h)
+
+            # Determine the board's physical location (fail if board does not
+            # exist)
+            cfb = machine.board_locations.get((x, y, z), None)
+            if cfb is None:
+                return None
+            cabinet, frame, board = cfb
+
+            # Determine what job is running on that board
+            found_job_id, job = self._job_for_location(machine, x, y, z)
+
+            # Make sure the board found is actually running that job (this
+            # won't be the case, e.g. if a user specifies a board within their
+            # machine which is actually dead or allocated to a neighbouring
+            # job)
+            if found_job_id != job_id:
+                return None
+
+            return {
+                "machine": machine_name,
+                "logical": (x, y, z),
+                "physical": (cabinet, frame, board),
+                "chip": (chip_x, chip_y),
+                "board_chip": board_chip,
+                "job_id": job_id,
+                "job_chip": self._get_job_chip(job, x, y, z, board_chip)
+            }
+
+    def _get_job_chip(self, job, x, y, z, board_chip):
+        # pylint: disable=too-many-arguments
+        if job is None:
+            return None
+        board_chip_x, board_chip_y = board_chip
+
+        # Determine the board coordinate within the job
+        job_x, job_y, job_z = map(min, zip(*job.boards))
+        job_x = x - job_x
+        job_y = y - job_y
+        job_z = z - job_z
+
+        # Turn that into a chip coordinate and wrap-around according to the
+        # boards actually available in the allocated machine
+        job_chip_x, job_chip_y = board_to_chip(job_x, job_y, job_z)
+        return ((job_chip_x + board_chip_x) % job.width,
+                (job_chip_y + board_chip_y) % job.height)
 
     def where_is(self, **kwargs):
-        """Find out where a SpiNNaker board or chip is located, logically and
+        """ Find out where a SpiNNaker board or chip is located, logically and
         physically.
 
         May be called in one of the following styles::
 
             >>> # Query by logical board coordinate within a machine.
             >>> where_is(machine=..., x=..., y=..., z=...)
 
@@ -676,149 +928,63 @@
 
             ``job_id`` is the job ID of the job currently allocated to the
             board identified or None if the board is not allocated to a job.
 
             ``job_chip`` the coordinates of the chip, (x, y), within its
             job, if a job is allocated to the board or None otherwise.
         """
-        with self._lock:
-            # Initially, we normalise the input coordinate into:
-            #
-            #     machine_name, chip_x, chip_y
-            #
-            # and then convert this back into all the output formats required.
-            # At various points, if we encounter a board/job/chip which doesn't
-            # exist we'll drop out.
-
-            keywords = set(kwargs)
-            if keywords == set("machine x y z".split()):
-                # Covert from logical position
-                machine_name = kwargs["machine"]
-                chip_x, chip_y = board_to_chip(
-                    kwargs["x"], kwargs["y"], kwargs["z"])
-            elif keywords == set("machine cabinet frame board".split()):
-                # Covert from physical position (fail if location does not
-                # exist)
-                machine_name = kwargs["machine"]
-                xyz = self.get_board_at_position(machine_name,
-                                                 kwargs["cabinet"],
-                                                 kwargs["frame"],
-                                                 kwargs["board"])
-                if xyz is None:
-                    return None
-                chip_x, chip_y = board_to_chip(*xyz)
-            elif keywords == set("machine chip_x chip_y".split()):
-                # Covert from chip location
-                machine_name = kwargs["machine"]
-                chip_x = kwargs["chip_x"]
-                chip_y = kwargs["chip_y"]
-            elif keywords == set("job_id chip_x chip_y".split()):
-                # Covert from job-relative chip location
-                job = self._jobs.get(kwargs["job_id"], None)
-                if job is None or job.boards is None:
-                    return None
-                machine_name = job.allocated_machine.name
-                job_x, job_y, job_z = map(min, zip(*job.boards))
-                dx, dy = board_to_chip(job_x, job_y, job_z)
-                chip_x = kwargs["chip_x"] + dx
-                chip_y = kwargs["chip_y"] + dy
-
-                # NB: We double-check later that this coordinate is actually a
-                # board within the boards allocated to the job!
-            else:
-                raise TypeError(
-                    "Invalid arguments: {}".format(", ".join(keywords)))
-
-            # Get the actual Machine
-            machine = self._machines.get(machine_name, None)
-            if machine is None:
-                return None
-
-            # Compensate chip coordinates for wrap-around
-            chip_w, chip_h = triad_dimensions_to_chips(
-                self._machines[machine_name].width,
-                self._machines[machine_name].height,
-                WrapAround.both)
-            chip_x %= chip_w
-            chip_y %= chip_h
-
-            # Determine the chip within the board
-            # Workaround: spinn5_chip_coord (until at least Rig 0.13.2) returns
-            # numpy integer types which are not JSON serialiseable.
-            board_chip_x, board_chip_y = map(
-                int, spinn5_chip_coord(chip_x, chip_y))
-
-            # Determine the logical board coordinates (and compensate for
-            # wrap-around)
-            x, y, z = chip_to_board(chip_x, chip_y, chip_w, chip_h)
-
-            # Determine the board's physical location (fail if board does not
-            # exist)
-            cfb = self.get_board_position(machine_name, x, y, z)
-            if cfb is None:
-                return None
-            cabinet, frame, board = cfb
-
-            # Determine what job is running on that board
-            for job_id, job in iteritems(self._jobs):
-                # NB: If machine is defined, boards must also be defined.
-                if (job.allocated_machine == machine and
-                        (x, y, z) in job.boards):
-                    # Found the job
-                    break
-            else:
-                # No job is allocated to the board
-                job_id = None
-                job = None
-
-            # If selected by job, make sure the board found is actually running
-            # that job (this won't be the case, e.g. if a user specifies a
-            # board within their machine which is actually dead or allocated to
-            # a neighbouring job)
-            if "job_id" in kwargs and job_id != kwargs["job_id"]:
-                return None
-
-            # Determine chip coordinate within job
-            if job is not None:
-                # Determine the board coordinate within the job
-                job_x, job_y, job_z = map(min, zip(*job.boards))
-                job_x = x - job_x
-                job_y = y - job_y
-                job_z = z - job_z
-
-                # Turn that into a chip coordinate and wrap-around according to
-                # the boards actually available in the allocated machine
-                job_chip_x, job_chip_y = board_to_chip(job_x, job_y, job_z)
-                job_chip = ((job_chip_x + board_chip_x) % job.width,
-                            (job_chip_y + board_chip_y) % job.height)
-            else:
-                job_chip = None
-
-            return {
-                "machine": machine_name,
-                "logical": (x, y, z),
-                "physical": (cabinet, frame, board),
-                "chip": (chip_x, chip_y),
-                "board_chip": (board_chip_x, board_chip_y),
-                "job_id": job_id,
-                "job_chip": job_chip,
-            }
+        # Internally, we normalise the input coordinate into:
+        #
+        #     machine_name, chip_x, chip_y
+        #
+        # and then convert this back into all the output formats required.
+        # At various points, if we encounter a board/job/chip which doesn't
+        # exist we'll drop out.
+
+        keywords = set(kwargs)
+        if keywords == set("machine x y z".split()):
+            return self._where_is_by_logical_triple(kwargs["machine"],
+                                                    kwargs["x"], kwargs["y"],
+                                                    kwargs["z"])
+        elif keywords == set("machine cabinet frame board".split()):
+            return self._where_is_by_physical_triple(kwargs["machine"],
+                                                     kwargs["cabinet"],
+                                                     kwargs["frame"],
+                                                     kwargs["board"])
+        elif keywords == set("machine chip_x chip_y".split()):
+            return self._where_is_by_chip_coordinate(kwargs["machine"],
+                                                     kwargs["chip_x"],
+                                                     kwargs["chip_y"])
+        elif keywords == set("job_id chip_x chip_y".split()):
+            return self._where_is_by_job_chip_coordinate(kwargs["job_id"],
+                                                         kwargs["chip_x"],
+                                                         kwargs["chip_y"])
+        else:
+            raise TypeError(
+                "Invalid arguments: {}".format(", ".join(keywords)))
 
     def destroy_timed_out_jobs(self):
-        """Destroy any jobs which have timed out."""
+        """ Destroy any jobs which have timed out.
+        """
         with self._lock:
-            now = time.time()
-            for job in list(itervalues(self._jobs)):
-                if (job.keepalive is not None and
-                        job.keepalive_until < now):
+            now = timestamp()
+            # NB: Copy the list of jobs because we will be modifying it
+            for job in list(self._jobs.values()):
+                if job.keepalive is not None and job.keepalive_until < now:
                     # Job timed out, destroy it
-                    self.destroy_job(job.id, "Job timed out.")
+                    self.destroy_job(None, job.id, "Job timed out.")
+
+    def check_free(self):
+        """ Check for freed machines that are now available
+        """
+        with self._lock:
+            self._job_queue.check_free()
 
-    def _bmp_on_request_complete(self, job, success):
-        """Callback function called by an AsyncBMPController when it completes
+    def _bmp_on_request_complete(self, job, success, reason=None):
+        """ Callback function called by an AsyncBMPController when it completes
         a previously issued request.
 
         This function sets the specified Job's state to JobState.ready when
         this function has been called job.bmp_requests_until_ready times.
 
         This function should be passed partially-called with the job the
         callback is associated it.
@@ -830,88 +996,93 @@
             method in a partial).
         success : bool
             Command success indicator provided by the AsyncBMPController.
         """
         with self._lock:
             # If a BMP command failed, cancel the job
             if not success:
-                self.destroy_job(
-                    job.id,
-                    "Machine configuration failed, please try again later.")
+                message = "Machine configuration failed."
+                if reason is not None:
+                    message += " Error: " + reason
+                self.destroy_job(None, job.id, message)
 
             # Count down the number of outstanding requests before the job is
             # ready
             job.bmp_requests_until_ready -= 1
             assert job.bmp_requests_until_ready >= 0
             if job.bmp_requests_until_ready == 0:
                 job.state = JobState.ready
+                if job.id in self._retired_jobs:
+                    self._job_queue.free(job.id)
 
                 # Report state changes for jobs which are still running
                 if job.id in self._jobs:
                     self._changed_jobs.add(job.id)
                     if self._on_background_state_change is not None:
                         self._on_background_state_change()
 
     def _set_job_power_and_links(self, job, power, link_enable=None):
-        """Power on/off and configure links for the boards associated with a
+        """ Power on/off and configure links for the boards associated with a
         specific job.
 
         Parameters
         ----------
         job : :py:class:`._Job`
             The job whose boards should be controlled.
         power : bool
             The power state to apply to the boards. True = on, False = off.
-        link_enable : bool or None
+        link_enable : bool or None, optional
             Whether to enable (True) or disable (False) peripheral links or
             leave them unchanged (None).
         """
         with self._lock:
             machine = job.allocated_machine
 
             on_done = partial(self._bmp_on_request_complete, job)
 
             # Group commands by the frame they interact with to allow all
             # commands within a frame to be sent atomically
-            frame_commands = defaultdict(list)
+            frame_commands = defaultdict(partial(AtomicRequests, on_done))
 
             controllers = self._bmp_controllers[machine.name]
 
             # Power commands
-            job.bmp_requests_until_ready += len(job.boards)
             for xyz in job.boards:
                 c, f, b = machine.board_locations[xyz]
                 controller = controllers[(c, f)]
-                frame_commands[controller].append(
-                    partial(controller.set_power, b, power, on_done))
+                job_log.info("power(%s, %s) on BMP %s for job %s",
+                             b, power, controller.hostname, job.id)
+                frame_commands[controller].power(b, bool(power))
 
             # Link state commands
             if link_enable is not None:
-                job.bmp_requests_until_ready += len(job.periphery)
                 for x, y, z, link in job.periphery:
                     c, f, b = machine.board_locations[(x, y, z)]
                     controller = controllers[(c, f)]
-                    frame_commands[controller].append(
-                        partial(controller.set_link_enable,
-                                b, link, link_enable, on_done))
+                    job_log.info(
+                        "link(%s, %s, %s) on BMP %s for job %s",
+                        b, link, link_enable, controller.hostname, job.id)
+                    frame_commands[controller].link(b, link, bool(link_enable))
 
             # Send power/link commands atomically for each frame
-            for controller, commands in iteritems(frame_commands):
+            job.bmp_requests_until_ready += len(frame_commands)
+            for controller, commands in frame_commands.items():
                 with controller:
-                    for command in commands:
-                        command()
+                    controller.add_requests(commands)
 
             # Update job state
             job.state = JobState.power
             job.power = power
             self._changed_jobs.add(job.id)
 
     def _job_queue_on_allocate(self, job_id, machine_name, boards,
                                periphery, torus):
-        """Called when a job is successfully allocated to a machine."""
+        """ Called when a job is successfully allocated to a machine.
+        """
+        # pylint: disable=too-many-arguments
         with self._lock:
             # Update job metadata
             job = self._jobs[job_id]
             job.allocated_machine = self._machines[machine_name]
             job.boards = boards
             job.periphery = periphery
             job.torus = torus
@@ -920,15 +1091,15 @@
 
             # Compute dimensions of machine the job will run on. Note that the
             # formulae used below for converting from board to chip coordinates
             # is only valid when either 'oz' is zero or only a single board is
             # allocated. Since we only allocate multi-board regions by the
             # triad this will be the case.
             ox, oy, oz = min(job.boards)  # Origin
-            bx, by, bz = max(job.boards)  # Top-right bound
+            bx, by, _ = max(job.boards)  # Top-right bound
 
             # Get system bounds in chips
             if len(job.boards) > 1:
                 job.width, job.height = triad_dimensions_to_chips((bx-ox) + 1,
                                                                   (by-oy) + 1,
                                                                   job.torus)
             else:
@@ -940,27 +1111,29 @@
             job.connections = {
                 board_to_chip(x-ox, y-oy, z-oz):
                 job.allocated_machine.spinnaker_ips[(x, y, z)]
                 for (x, y, z) in job.boards
             }
 
             # Initialise the boards
-            self.power_on_job_boards(job_id)
+            self.power_on_job_boards(job.lasthost, job_id)
 
     def _job_queue_on_free(self, job_id, reason):
-        """Called when a job is freed."""
+        """ Called when a job is freed.
+        """
         self._changed_machines.add(self._jobs[job_id].allocated_machine.name)
         self._teardown_job(job_id, reason)
 
     def _job_queue_on_cancel(self, job_id, reason):
-        """Called when a job is cancelled before having been allocated."""
+        """ Called when a job is cancelled before having been allocated.
+        """
         self._teardown_job(job_id, "Cancelled: {}".format(reason or ""))
 
     def _teardown_job(self, job_id, reason):
-        """Called once job has been removed from the JobQueue.
+        """ Called once job has been removed from the JobQueue.
 
         Powers down any hardware in use and finally removes the job from _jobs.
         """
         with self._lock:
             job = self._jobs.pop(job_id)
             self._retired_jobs[job_id] = reason
             self._changed_jobs.add(job.id)
@@ -969,76 +1142,99 @@
             # accumulating memory consumption forever.
             if len(self._retired_jobs) > self._max_retired_jobs:
                 self._retired_jobs.pop(next(iter(self._retired_jobs)))
 
             # Power-down any boards that were in use
             if job.boards is not None:
                 self._set_job_power_and_links(job, power=False)
+            if job.lasthost is None:
+                job_log.info("completed shutdown of job %s", job_id)
+            else:
+                job_log.info("completed shutdown of job %s (owner-host: %s)",
+                             job_id, job.lasthost)
 
     def _create_machine_bmp_controllers(self, machine, on_thread_start=None):
-        """Create BMP controllers for a machine."""
+        """ Create BMP controllers for a machine.
+        """
         with self._lock:
             controllers = {}
-            for (c, f), hostname in iteritems(machine.bmp_ips):
+            self._bmp_controllers[machine.name] = controllers
+            for (c, f), hostname in machine.bmp_ips.items():
                 controllers[(c, f)] = AsyncBMPController(
                     hostname, on_thread_start)
-            self._bmp_controllers[machine.name] = controllers
 
     def _init_dynamic_state(self):
-        """Initialise all dynamic (non-pickleable) state.
+        """ Initialise all dynamic (non-pickleable) state.
 
         Specifically:
 
         * Creates the global controller lock
         * Creates connections to BMPs.
         * Reset keepalive_until on all existing jobs (e.g. allowing remote
           devices a chance to reconnect before terminating their jobs).
         """
         # Recreate the lock
         assert self._lock is None
-        self._lock = threading.RLock()
+        self._lock = RLock()
 
         with self._lock:
             # Create connections to BMPs
             assert self._bmp_controllers is None
             self._bmp_controllers = {}
-            for machine in itervalues(self._machines):
-                self._create_machine_bmp_controllers(machine)
+            try:
+                for machine in self._machines.values():
+                    self._create_machine_bmp_controllers(machine)
+
+                # Reset keepalives to allow remote clients time to reconnect
+                for job_id in self._jobs:
+                    self.job_keepalive(None, job_id)
+            except Exception:
+                self.stop()
+                raise
 
-            # Reset keepalives to allow remote clients time to reconnect
-            for job_id in self._jobs:
-                self.job_keepalive(job_id)
+    @property
+    def seconds_before_free(self):
+        return self._job_queue.seconds_before_free
+
+    @seconds_before_free.setter
+    def seconds_before_free(self, seconds_before_free):
+        self._job_queue.seconds_before_free = seconds_before_free
 
 
 class JobState(IntEnum):
-    """All the possible states that a job may be in."""
+    """ All the possible states that a job may be in.
+    """
 
     unknown = 0
-    """The job ID requested was not recognised"""
+    """ The job ID requested was not recognised.
+    """
 
     queued = 1
-    """The job is waiting in a queue for a suitable machine"""
+    """ The job is waiting in a queue for a suitable machine.
+    """
 
     power = 2
-    """The boards allocated to the job are currently being powered on or
+    """ The boards allocated to the job are currently being powered on or
     powered off.
     """
 
     ready = 3
-    """The job has been allocated boards and the boards are not currently
+    """ The job has been allocated boards and the boards are not currently
     powering on or powering off.
     """
 
     destroyed = 4
-    """The job has been destroyed"""
+    """ The job has been destroyed.
+    """
 
 
 class JobStateTuple(namedtuple("JobStateTuple",
-                               "state,power,keepalive,reason,start_time")):
-    """Tuple describing the state of a particular job, returned by
+                               "state,power,keepalive,reason,start_time,"
+                               "keepalivehost")):
+    """ Tuple describing the state of a particular job, returned by
     :py:meth:`.Controller.get_job_state`.
 
     Parameters
     ----------
     state : :py:class:`.JobState`
         The current state of the queried job.
     power : bool or None
@@ -1050,24 +1246,27 @@
         about the job before it is automatically destroyed. None if no
         timeout is active (or when the job has been destroyed).
     reason : str or None
         If the job has been destroyed, this may be a string describing the
         reason the job was terminated.
     start_time : float or None
         The Unix time (UTC) at which the job was created.
+    keepalivehost : str or None
+        The IP address of the last system to take an action that caused the
+        job to be kept alive.
     """
 
     # Python 3.4 Workaround: https://bugs.python.org/issue24931
     __slots__ = tuple()
 
 
 class JobMachineInfoTuple(namedtuple("JobMachineInfoTuple",
                                      "width,height,connections,"
                                      "machine_name,boards")):
-    """Tuple describing the machine alloated to a job, returned by
+    """ Tuple describing the machine alloated to a job, returned by
     :py:meth:`.Controller.get_job_machine_info`.
 
     Parameters
     ----------
     width, height : int or None
         The dimensions of the machine in *chips* or None if no machine
         allocated.
@@ -1083,16 +1282,17 @@
 
     # Python 3.4 Workaround: https://bugs.python.org/issue24931
     __slots__ = tuple()
 
 
 class JobTuple(namedtuple("JobTuple",
                           "job_id,owner,start_time,keepalive,state,power,"
-                          "args,kwargs,allocated_machine_name,boards")):
-    """Tuple describing a job in the list of jobs returned by
+                          "args,kwargs,allocated_machine_name,boards,"
+                          "keepalivehost")):
+    """ Tuple describing a job in the list of jobs returned by
     :py:meth:`.Controller.list_jobs`.
 
     Parameters
     ----------
     job_id : int
         The ID of the job.
     owner : str
@@ -1117,47 +1317,51 @@
         allocation requested and the restrictions on dead boards, links and
         torus connectivity.
     allocated_machine_name : str or None
         The name of the machine the job has been allocated to run on (or None
         if not allocated yet).
     boards : set([(x, y, z), ...])
         The boards allocated to the job.
+    keepalivehost : str
+        The name of the host that is reckoned to be keeping this job alive.
+        Will be the empty string if no known host is doing so (a possible
+        state after a service restart).
     """
 
     # Python 3.4 Workaround: https://bugs.python.org/issue24931
     __slots__ = tuple()
 
 
 class MachineTuple(namedtuple("MachineTuple",
                               "name,tags,width,height,"
                               "dead_boards,dead_links")):
-    """Tuple describing a machine in the list of machines returned by
+    """ Tuple describing a machine in the list of machines returned by
     :py:meth:`.Controller.list_machines`.
 
     Parameters
     ----------
     name : str
         The name of the machine.
     tags : set(['tag', ...])
         The tags the machine has.
     width, height : int
         The dimensions of the machine in triads.
     dead_boards : set([(x, y, z), ...])
         The coordinates of known-dead boards.
-    dead_links : set([(x, y, z, :py:class:`rig.links.Links`), ...])
+    dead_links : set([(x, y, z, :py:class:`spalloc_server.links.Links`), ...])
         The locations of known-dead links from the perspective of the sender.
         Links to dead boards may or may not be included in this list.
     """
 
     # Python 3.4 Workaround: https://bugs.python.org/issue24931
     __slots__ = tuple()
 
 
 class _Job(object):
-    """The metadata, used internally, associated with a non-destroyed job.
+    """ The metadata, used internally, associated with a non-destroyed job.
 
     Attributes
     ----------
     id : int
         The ID of the job.
     owner : str
         The job's owner.
@@ -1182,15 +1386,16 @@
         torus connectivity.
     allocated_machine : \
             :py:class:`spalloc_server.configuration.Machine` or None
         The machine the job has been allocated to run on (or None if not
         allocated yet).
     boards : set([(x, y, z), ...]) or None
         The boards allocated to the job or None if not allocated.
-    periphery : set([(x, y, z, :py:class:`rig.links.Links`), ...]) or None
+    periphery : set([(x, y, z,\
+                     :py:class:`spalloc_server.links.Links`), ...]) or None
         The links around the periphery of the job or None if not allocated.
     torus : :py:class:`spalloc_server.coordinates.WrapAround` or None
         Does the allocated set of boards have wrap-around links? None if
         not allocated.
     width, height : int or None
         The dimensions of the SpiNNaker network in the allocated boards or None
         if not allocated any boards.
@@ -1200,58 +1405,59 @@
     bmp_requests_until_ready : int
         A counter incremented whenever a BMP command is started and
         decremented when the command completes. When this counter reaches
         zero, the user sets the state of the job to
         :py:class:`.JobState.ready`.
     """
 
-    def __init__(self, id, owner,
+    def __init__(self, _id, owner,
                  start_time=None,
                  keepalive=60.0,
+                 lasthost=None,
                  state=JobState.queued,
                  power=None,
-                 args=tuple(), kwargs={},
+                 args=tuple(), kwargs=None,
                  allocated_machine=None,
                  boards=None,
                  periphery=None,
                  torus=None,
                  width=None,
                  height=None,
                  connections=None,
                  bmp_requests_until_ready=0):
-
-        self.id = id
-
+        # pylint: disable=too-many-arguments
+        self.id = _id
         self.owner = owner
 
         if start_time is not None:  # pragma: no branch
             self.start_time = start_time  # pragma: no cover
         else:
             now = datetime.now(utc)
             epoch = datetime(1970, 1, 1, tzinfo=utc)
             self.start_time = (now - epoch).total_seconds()
 
         # If None, never kill this job due to inactivity. Otherwise, stop the
         # job if the time exceeds this value. It is the allocator's
         # responsibility to update this periodically.
         self.keepalive = keepalive
         if self.keepalive is not None:
-            self.keepalive_until = time.time() + self.keepalive
+            self.keepalive_until = timestamp() + self.keepalive
         else:
             self.keepalive_until = None
+        self.lasthost = lasthost
 
         # The current life-cycle state of the job
         self.state = state
 
         # False
         self.power = power
 
         # Arguments for the allocator
         self.args = args
-        self.kwargs = kwargs
+        self.kwargs = dict({} if kwargs is None else kwargs)
 
         # The hardware allocated to this job (if any)
         self.allocated_machine = allocated_machine
         self.boards = boards
         self.periphery = periphery
         self.torus = torus
         self.width = width
@@ -1259,7 +1465,13 @@
 
         # IP address lookup for allocated boards
         self.connections = connections
 
         # The number of BMP requests which must complete before this job may
         # return to the ready state.
         self.bmp_requests_until_ready = bmp_requests_until_ready
+
+    def update_keepalive(self, host):
+        if host is not None:
+            self.lasthost = host
+        if self.keepalive is not None:
+            self.keepalive_until = timestamp() + self.keepalive
```

### Comparing `spalloc_server-0.5.2/spalloc_server/coordinates.py` & `spalloc_server-1!7.0.0a4/spalloc_server/coordinates.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-r"""Utilities for working with board/triad coordinates.
+# Copyright (c) 2016 The University of Manchester
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+r""" Utilities for working with board/triad coordinates.
 
 This software assumes that all machines provided to it are interconnected in a
 valid (subset of) a hexagonal torus topology. Boards locations are expressed
 in one of several forms depending on circumstance.
 
 * **Board coordinates** ``(x, y, z)`` giving the logical location of the board
   within a hexagonal torus configuration. This is the most frequently used
@@ -92,19 +106,18 @@
     |             |  |  | | | | |  |  |             |
     +-------------+  +--|-|-|-|-|--+  +-------------+
                         | | | | |
              Board -----+-+-+-+-+
                         4 3 2 1 0
 
 A mapping from board coordinates to physical coordinates is supplied by the
-user and is unique to the machine being built. A tool such as SpiNNer_ may be
+user and is unique to the machine being built. A tool such as
+`SpiNNer <https://github.com/SpiNNakerManchester/SpiNNer>`__ may be
 used to generate such mappings.
 
-.. _SpiNNer: https://github.com/SpiNNakerManchester/SpiNNer
-
 
 Ethernet chip coordinates
 `````````````````````````
 
 Ethernet chip coordinates are given as a tuple ``(x, y)``.
 
 Ethernet chip coordinates give the chip coordinates of Ethernet connected chips
@@ -112,63 +125,60 @@
 
 Utilities
 `````````
 
 The following utilities are provided for working with the above coordinate
 systems.
 """
-
 from enum import IntEnum
-
-from six import iteritems
-
-from rig.links import Links
-from rig.geometry import spinn5_local_eth_coord
-
+from spinn_machine import SpiNNakerTriadGeometry
+from .links import Links
 
 link_to_vector = {
     (0, Links.north): (0, 0, 2),
     (0, Links.north_east): (0, 0, 1),
     (0, Links.east): (0, -1, 2),
 
     (1, Links.north): (1, 1, -1),
     (1, Links.north_east): (1, 0, 1),
     (1, Links.east): (1, 0, -1),
 
     (2, Links.north): (0, 1, -1),
     (2, Links.north_east): (1, 1, -2),
     (2, Links.east): (0, 0, -1),
 }
-"""A lookup from (z, :py:class:`rig.links.Links`) to (dx, dy, dz)."""
 
+""" A lookup from (z, :py:class:`spalloc_server.links.Links`) to (dx, dy, dz).
+"""
 link_to_vector.update({
     (z + dz, link.opposite): (-dx, -dy, -dz)
-    for (z, link), (dx, dy, dz) in iteritems(link_to_vector)
+    for (z, link), (dx, dy, dz) in link_to_vector.items()
 })
 
 
 def board_down_link(x1, y1, z1, link, width, height):
-    """Get the coordinates of the board down the specified link.
+    """ Get the coordinates of the board down the specified link.
 
     Parameters
     ----------
     x1, y1, z1 : int
         The board coordinates from which a link will be traversed.
-    link : :py:class:`rig.links.Link`
+    link : :py:class:`spalloc_server.links.Link`
         The link to follow.
     width, height : int
         The dimensions of the system in triads.
 
     Returns
     -------
     x, y, z : int
         The coordinates of the board down the specified link.
     wrapped : :py:class:`.WrapAround`
         In what way did we wrap-around when following that link?
     """
+    # pylint: disable=too-many-arguments
     dx, dy, dz = link_to_vector[(z1, link)]
 
     x2_ = (x1 + dx)
     y2_ = (y1 + dy)
 
     x2 = x2_ % width
     y2 = y2_ % height
@@ -178,15 +188,15 @@
     wrapped = WrapAround((WrapAround.x if x2_ != x2 else 0) |
                          (WrapAround.y if y2_ != y2 else 0))
 
     return (x2, y2, z2, wrapped)
 
 
 def board_to_chip(x, y, z):
-    """Convert a board coordinate into a chip coordinate.
+    """ Convert a board coordinate into a chip coordinate.
 
     Assumes a regular torus composed of SpiNN-5 boards.
 
     Parameters
     ----------
     x, y, z : int
         Board coordinates.
@@ -207,15 +217,15 @@
         x += 4
         y += 8
 
     return (x, y)
 
 
 def chip_to_board(x, y, w, h):
-    """Convert a chip coordinate into a board coordinate.
+    """ Convert a chip coordinate into a board coordinate.
 
     Assumes a regular torus composed of SpiNN-5 boards.
 
     Parameters
     ----------
     x, y : int
         Chip coordinates.
@@ -224,17 +234,18 @@
 
     Returns
     -------
     x, y, z : int
         Board coordinates.
     """
     # Convert to coordinate of chip at the bottom-left-corner of the board
-    # Workaround: spinn5_chip_coord (until at least Rig 0.13.2) returns
-    # numpy integer types which are not JSON serialiseable.
-    x, y = map(int, spinn5_local_eth_coord(x, y, w, h))
+    x, y = map(
+        int,
+        SpiNNakerTriadGeometry.get_spinn5_geometry()
+        .get_ethernet_chip_coordinates(x, y, w, h))
 
     # The coordinates of the chip within its triad
     tx = x % 12
     ty = y % 12
 
     x //= 12
     y //= 12
@@ -248,24 +259,24 @@
     else:  # pragma: no cover
         assert False
 
     return (x, y, z)
 
 
 def triad_dimensions_to_chips(w, h, torus):
-    """Convert the dimensions of a system from numbers of triads to numbers of
+    """ Convert the dimensions of a system from numbers of triads to numbers of
     chips in the underlying network.
 
     Assumes a regular torus composed of SpiNN-5 boards.
 
     Parameters
     ----------
     w, h : int
         Dimensions of the system in triads.
-    torus : :py:class`.WrapAround`
+    torus : :py:class:`.WrapAround`
         What wrap-around connections are present?
 
     Returns
     -------
     w, h : int
         Dimensions of the SpiNNaker chip network in the specified machine, e.g.
         for booting.
@@ -282,15 +293,15 @@
     if not (torus & WrapAround.y):
         h += 4
 
     return (w, h)
 
 
 class WrapAround(IntEnum):
-    """Defines what type of wrap-around links a torus has, if any.
+    """ Defines what type of wrap-around links a torus has, if any.
 
     Values chosen have the following useful properties::
 
         >>> # Can be meaningfully cast to bool
         >>> assert bool(WrapAround.none) is False
         >>> assert bool(WrapAround.x) is True
         >>> assert bool(WrapAround.y) is True
@@ -300,17 +311,21 @@
         >>> assert bool(WrapAround.both & WrapAround.x) is True
         >>> assert bool(WrapAround.both & WrapAround.y) is True
         >>> assert bool(WrapAround.x & WrapAround.x) is True
         >>> assert bool(WrapAround.x & WrapAround.y) is False
     """
 
     none = 0b00
-    """No wrap-around links."""
+    """ No wrap-around links.
+    """
 
     x = 0b01
-    """Has wrap around links around X-axis."""
+    """ Has wrap around links around X-axis.
+    """
 
     y = 0b10
-    """Has wrap around links around Y-axis."""
+    """ Has wrap around links around Y-axis.
+    """
 
     both = 0b11
-    """Has wrap around links on X and Y axes."""
+    """ Has wrap around links on X and Y axes.
+    """
```

### Comparing `spalloc_server-0.5.2/spalloc_server/configuration.py` & `spalloc_server-1!7.0.0a4/spalloc_server/configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-"""A configuration file is used to describe the machines which are to be
+# Copyright (c) 2016 The University of Manchester
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+""" A configuration file is used to describe the machines which are to be
 managed.  Configuration files are Python scripts which define a global
 ``configuration`` variable which is an instance of the
 :py:class:`.Configuration` class.
 
 .. note::
 
     Everything in :py:mod:`spalloc_server.configuration` and
@@ -23,15 +37,15 @@
 dimensions, broken boards and links, physical layout and IP addresses of a
 SpiNNaker machine. All machines are presumed to be interconnected in a valid
 hexagonal torus topology constructed from a rectangular array of triads of
 boards. (See also :py:mod:`spalloc_server.coordinates` for details of
 the coordinate systems used when referring to boards.)
 
 Defining Machines
-`````````````````
+=================
 
 Since defining machines completely by hand can be quite verbose (see example
 below), a some convenience functions are provided to deal with the common case
 of machines constructed in the standard manner.
 
 To define an isolated single-board machine, the
 :py:meth:`.Machine.single_board` constructor may be used as follows::
@@ -39,20 +53,21 @@
     m = Machine.single_board("my-board",
                              bmp_ip="spinn-board-bmp",
                              spinnaker_ip="spinn-board")
     configuration = Configuration(machines=[m])
 
 Most multi-board systems follow a standardised IP addressing scheme and have
 their physical layout defined by `SpiNNer
-<http://spinner.readthedocs.org/en/stable>`_. The
+<https://spinner.readthedocs.org/en/stable>`_. The
 :py:func:`.board_locations_from_spinner` function reads CSV files produced by
 `spinner-ethernet-chips
-<http://spinner.readthedocs.org/en/stable/spinner-ethernet-chips.html>`_
+<https://spinner.readthedocs.org/en/stable/spinner-ethernet-chips.html>`_
 describing machine layouts and the :py:meth:`.Machine.with_standard_ips`
-constructor produces :py:class:`.Machine`\ s with IP addresses based on the
+constructor produces a :py:class:`~spalloc_server.configuration.Machine`
+with IP addresses based on the
 standard IP addressing scheme. These may be used together like so::
 
     # spinner-ethernet-chips -n 1200 > ethernet_chips.csv
     m = Machine.with_standard_ips(
         "million-core-machine",
         board_locations=board_locations_from_spinner("ethernet_chips.csv"),
         base_ip="10.2.0.0",
@@ -85,92 +100,97 @@
                 })
     configuration = Configuration(machines=[m])
 
 Remember, since the configuration file is just a normal Python file, you can
 use any code you like to pragmatically specify machines, etc. which you use.
 
 Configuration File API Reference
-````````````````````````````````
-"""
+================================
+"""  # noqa: W605
 
 from collections import namedtuple
-
 import re
 import csv
-
 from itertools import chain
+from .coordinates import chip_to_board
 
-from six import iteritems, itervalues
 
-from spalloc_server.coordinates import chip_to_board
+def _empty_default_dict(d):
+    return dict(d) if d is not None else {}
 
 
 class Configuration(namedtuple("Configuration",
                                "machines,port,ip,timeout_check_interval,"
-                               "max_retired_jobs")):
-    """Defines the configuration of a server.
+                               "max_retired_jobs,seconds_before_free")):
+    """ Defines the configuration of a server.
 
     Parameters
     ----------
     machines : [:py:class:`~.Machine`, ...]
         The list of machines, highest priority first, the server is to
         manage. (Default: [])
     port : int
-        The port number the server should listen on. (Default: 22244)
+        The port number the server should listen on. Note that this is now
+        deprecated; the port should be specified by the ``--port`` option on
+        the spalloc_server command line. (Default: 22244)
     ip : str
         The IP the server should listen on. (Default: "", i.e. all interfaces)
     timeout_check_interval : float
         The number of seconds between the server's checks for job timeouts.
         (Default: 5.0)
     max_retired_jobs : int
         The number of retired jobs to keep records of. (Default: 1200)
     """
 
-    def __new__(cls, machines=[], port=22244, ip="",
+    def __new__(cls, machines=None, port=22244, ip="",
                 timeout_check_interval=5.0,
-                max_retired_jobs=1200):
+                max_retired_jobs=1200,
+                seconds_before_free=30):
+        # pylint: disable=too-many-arguments
+
         # Validate machine definitions
         used_names = set()
         used_bmp_ips = set()
         used_spinnaker_ips = set()
+        machines = list([] if machines is None else machines)
         for m in machines:
             # Typecheck...
             if not isinstance(m, Machine):
                 raise TypeError("All machines must be of type Machine.")
 
             # Machine names must be unique
             if m.name in used_names:
                 raise ValueError("Machine name '{}' used multiple "
                                  "times.".format(m.name))
             used_names.add(m.name)
 
             # All BMP IPs must be unique
-            for bmp_ip in itervalues(m.bmp_ips):
+            for bmp_ip in m.bmp_ips.values():
                 if bmp_ip in used_bmp_ips:
                     raise ValueError("BMP IP '{}' used multiple "
                                      "times.".format(bmp_ip))
                 used_bmp_ips.add(bmp_ip)
 
             # All SpiNNaker IPs must be unique
-            for spinnaker_ip in itervalues(m.spinnaker_ips):
+            for spinnaker_ip in m.spinnaker_ips.values():
                 if spinnaker_ip in used_spinnaker_ips:
                     raise ValueError("SpiNNaker IP '{}' used multiple "
                                      "times.".format(spinnaker_ip))
                 used_spinnaker_ips.add(spinnaker_ip)
 
-        return super(Configuration, cls).__new__(cls, machines, port, ip,
-                                                 timeout_check_interval,
-                                                 max_retired_jobs)
+        return super().__new__(
+            cls, machines, port, ip, timeout_check_interval, max_retired_jobs,
+            seconds_before_free)
 
 
 class Machine(namedtuple("Machine", "name,tags,width,height,"
                                     "dead_boards,dead_links,"
                                     "board_locations,"
                                     "bmp_ips,spinnaker_ips")):
-    """Defines a SpiNNaker machine.
+    """ Defines a SpiNNaker machine.
 
     Parameters
     ----------
     name : str
         The name of the machine.
     tags : set([str, ...])
         A set of tags which jobs may use to filter machines by. Note that by
@@ -178,44 +198,47 @@
         ought have this tag too.
     width, height : int
         The dimensions of the machine in triads of boards. If omitted, these
         are inferred from the boards defined in board_locations and
         dead_boards.
     dead_boards : set([(x, y, z), ...])
         The board coordinates of all dead boards in the machine.
-    dead_links : set([(x, y, z, :py:class:`~rig.links.Links`), ...])
+    dead_links : set([(x, y, z, :py:class:`~spalloc_server.links.Links`), ...])
         The board coordinates of all dead links in the machine. Links to dead
         boards are implicitly dead and may or may not be included in this set.
     board_locations : {(x, y, z): (c, f, b), ...}
         Lookup from board coordinate to its physical in a SpiNNaker
         machine in terms of cabinet, frame and board position. Must give the
         coordinates of *all* working boards.
     bmp_ips : {(c, f): hostname, ...}
         The IP address of a BMP in every frame of the machine which contains
         working boards.
     spinnaker_ips : {(x, y, z): hostname, ...}
         For every working board gives the IP address of the SpiNNaker board's
         Ethernet connected chip.
     """
 
-    def __new__(cls, name, tags=set(["default"]),
+    def __new__(cls, name, tags=frozenset(["default"]),
                 width=None, height=None,
-                dead_boards=set(), dead_links=set(),
-                board_locations={},
-                bmp_ips={},
-                spinnaker_ips={}):
+                dead_boards=frozenset(), dead_links=frozenset(),
+                board_locations=None, bmp_ips=None, spinnaker_ips=None):
+        # pylint: disable=too-many-arguments
 
         # Make sure the set-type arguments are the correct type...
-        if not isinstance(tags, set):
+        if not isinstance(tags, (set, frozenset)):
             raise TypeError("tags should be a set.")
-        if not isinstance(dead_boards, set):
+        if not isinstance(dead_boards, (set, frozenset)):
             raise TypeError("dead_boards should be a set.")
-        if not isinstance(dead_links, set):
+        if not isinstance(dead_links, (set, frozenset)):
             raise TypeError("dead_links should be a set.")
 
+        board_locations = _empty_default_dict(board_locations)
+        bmp_ips = _empty_default_dict(bmp_ips)
+        spinnaker_ips = _empty_default_dict(spinnaker_ips)
+
         # If not specified, infer the dimensions of the system
         if width is None and height is None:
             width, height, _ = map(max, zip(*chain(board_locations,
                                                    dead_boards)))
             width += 1
             height += 1
         if width is None or height is None:
@@ -225,24 +248,24 @@
         # All dead boards and links should be within the size of the system
         for x, y, z in dead_boards:
             if not (0 <= x < width and
                     0 <= y < height and
                     0 <= z < 3):
                 raise ValueError("Dead board ({}, {}, {}) "
                                  "outside system.".format(x, y, z))
-        for x, y, z, link in dead_links:
+        for x, y, z, _ in dead_links:
             if not (0 <= x < width and
                     0 <= y < height and
                     0 <= z < 3):
                 raise ValueError("Dead link ({}, {}, {}) "
                                  "outside system.".format(x, y, z))
 
         # All board locations must be sensible
         locations = set()
-        for (x, y, z), (c, f, b) in iteritems(board_locations):
+        for (x, y, z), (c, f, b) in board_locations.items():
             # Board should be within system
             if not (0 <= x < width and
                     0 <= y < height and
                     0 <= z < 3):
                 raise ValueError("Board location given for board "
                                  "not in system ({}, {}, {}).".format(x, y, z))
             # No two boards should be in the same location
@@ -260,35 +283,33 @@
                          if (x, y, z) not in dead_boards)
         missing_boards = live_bords - set(board_locations)
         if missing_boards:
             raise ValueError(
                 "Board locations missing for {}".format(missing_boards))
 
         # BMP IPs should be given for all frames which have been used
-        frames = set((c, f) for c, f, b in locations)
-        missing_bmp_ips = frames - set(bmp_ips)
+        missing_bmp_ips = set((c, f) for c, f, _ in locations) - set(bmp_ips)
         if missing_bmp_ips:
             raise ValueError(
                 "BMP IPs not given for frames {}".format(missing_bmp_ips))
 
         # SpiNNaker IPs should be given for all live boards
         missing_ips = live_bords - set(spinnaker_ips)
         if missing_ips:
             raise ValueError(
                 "SpiNNaker IPs not given for boards {}".format(missing_ips))
 
-        return super(Machine, cls).__new__(cls, name, tags, width, height,
-                                           dead_boards, dead_links,
-                                           board_locations,
-                                           bmp_ips, spinnaker_ips)
+        return super().__new__(
+            cls, name, tags, width, height, frozenset(dead_boards),
+            frozenset(dead_links), board_locations, bmp_ips, spinnaker_ips)
 
     @classmethod
-    def single_board(cls, name, tags=set(["default"]),
+    def single_board(cls, name, tags=frozenset(["default"]),
                      bmp_ip=None, spinnaker_ip=None):
-        """Convenience constructor. Construct a :py:class:`.Machine`
+        """ Convenience constructor. Construct a :py:class:`.Machine`
         representing a single SpiNNaker board.
 
         Parameters
         ----------
         name : str
             The name of the machine
         tags : set([tag, ...])
@@ -299,32 +320,31 @@
             The hostname of the SpiNNaker board.
         """
         if bmp_ip is None:
             raise TypeError("bmp_ip must be given.")
         if spinnaker_ip is None:
             raise TypeError("spinnaker_ip must be given.")
 
-        return cls(name, tags, 1, 1,
-                   dead_boards=set([(0, 0, 1), (0, 0, 2)]), dead_links=set(),
-                   board_locations={(0, 0, 0): (0, 0, 0)},
-                   bmp_ips={(0, 0): bmp_ip},
-                   spinnaker_ips={(0, 0, 0): spinnaker_ip})
+        return cls(
+            name, tags, 1, 1, dead_boards=set([(0, 0, 1), (0, 0, 2)]),
+            dead_links=set(), board_locations={(0, 0, 0): (0, 0, 0)},
+            bmp_ips={(0, 0): bmp_ip}, spinnaker_ips={(0, 0, 0): spinnaker_ip})
 
     @classmethod
-    def with_standard_ips(cls, name, tags=set(["default"]),
+    def with_standard_ips(cls, name, tags=frozenset(["default"]),
                           width=None, height=None,
-                          dead_boards=set(), dead_links=set(),
-                          board_locations={},
+                          dead_boards=frozenset(), dead_links=frozenset(),
+                          board_locations=None,
                           base_ip="192.168.0.0",
                           cabinet_stride="0.0.5.0",
                           frame_stride="0.0.1.0",
                           board_stride="0.0.0.8",
                           bmp_offset="0.0.0.0",
                           spinnaker_offset="0.0.0.1"):
-        """Convenience constructor. Construct a :py:class:`.Machine` which
+        """ Convenience constructor. Construct a :py:class:`.Machine` which
         infers IP addresses of the form conventionally used by SpiNNaker
         installations.
 
         In standard SpiNNaker installations, IP addresses are allocated in a
         regular fashion as described below.
 
         IP addresses for a particular machine are allocated within an address
@@ -361,25 +381,26 @@
         Finally, we assume that board 0's BMP is to be used as the BMP for
         controlling all boards in its frame.
 
         Parameters
         ----------
         name : str
             The name of the machine.
-        tags : set([str, ...])
+        tags : iterable([str, ...])
             A set of tags which jobs may use to filter machines by. Note that
             by default jobs are assigned the 'default' tag and thus machines
             probably ought have this tag too.
         width, height : int
             The dimensions of the machine in triads of boards. If omitted,
             these are inferred from the boards defined in board_locations and
             dead_boards.
-        dead_boards : set([(x, y, z), ...])
+        dead_boards : iterable([(x, y, z), ...])
             The board coordinates of all dead boards in the machine.
-        dead_links : set([(x, y, z, :py:class:`~rig.links.Links`), ...])
+        dead_links : iterable([(x, y, z,\
+                           :py:class:`~spalloc_server.links.Links`), ...])
             The board coordinates of all dead links in the machine. Links to
             dead boards are implicitly dead and may or may not be included in
             this set.
         board_locations : {(x, y, z): (c, f, b), ...}
             Lookup from board coordinate to its physical in a SpiNNaker machine
             in terms of cabinet, frame and board position. Must give the
             coordinates of *all* working boards.
@@ -399,70 +420,71 @@
             The offset of a board's BMP IP from the start of a board's IP
             address range, expressed as an IPv4 address.
         spinnaker_offset : str
             The offset of a board's Ethernet-connected SpiNNaker chip IP from
             the start of a board's IP address range, expressed as an IPv4
             address.
         """
+        # pylint: disable=too-many-arguments
 
         def ip_to_int(ip):
-            """Convert from string-based IP to a 32-bit integer."""
-            match = re.match("^(\d+).(\d+).(\d+).(\d+)$", ip)
+            """ Convert from string-based IP to a 32-bit integer.
+            """
+            match = re.match(r"^(\d+).(\d+).(\d+).(\d+)$", ip)
             if not match:
                 raise ValueError("Malformed IPv4 address '{}'".format(ip))
 
             ip_int = 0
             for group in map(int, match.groups()):
                 if group & ~0xFF:
                     raise ValueError("Malformed IPv4 address '{}'".format(ip))
                 ip_int <<= 8
                 ip_int |= group
 
             return ip_int
 
         def int_to_ip(ip_int):
-            """Convert from 32-bit integer to string-based IP address."""
+            """ Convert from 32-bit integer to string-based IP address.
+            """
             return ".".join(str((ip_int >> b) & 0xFF)
                             for b in range(24, -8, -8))
 
         base_ip = ip_to_int(base_ip)
         cabinet_stride = ip_to_int(cabinet_stride)
         frame_stride = ip_to_int(frame_stride)
         board_stride = ip_to_int(board_stride)
         bmp_offset = ip_to_int(bmp_offset)
         spinnaker_offset = ip_to_int(spinnaker_offset)
+        board_locations = _empty_default_dict(board_locations)
 
         # Generate IP addresses for BMPs
-        cabinets_and_frames = set((c, f) for c, f, b in
-                                  itervalues(board_locations))
-        bmp_ips = {(c, f): int_to_ip(base_ip +
-                                     (cabinet_stride * c) +
-                                     (frame_stride * f) +
-                                     bmp_offset)
-                   for (c, f) in cabinets_and_frames}
+        cabinets_and_frames = set(
+            (c, f) for c, f, _ in board_locations.values())
+        bmp_ips = {
+            (c, f): int_to_ip(base_ip + (cabinet_stride * c) +
+                              (frame_stride * f) + bmp_offset)
+            for (c, f) in cabinets_and_frames}
 
         # Generate IP addresses for SpiNNaker boards
-        spinnaker_ips = {(x, y, z): int_to_ip(base_ip +
-                                              (cabinet_stride * c) +
-                                              (frame_stride * f) +
-                                              (board_stride * b) +
-                                              spinnaker_offset)
-                         for (x, y, z), (c, f, b)
-                         in iteritems(board_locations)}
-
-        return cls(name, tags, width, height,
-                   dead_boards=dead_boards, dead_links=dead_links,
-                   board_locations=board_locations,
+        spinnaker_ips = {
+            (x, y, z): int_to_ip(base_ip + (cabinet_stride * c) +
+                                 (frame_stride * f) + (board_stride * b) +
+                                 spinnaker_offset)
+            for (x, y, z), (c, f, b) in board_locations.items()}
+
+        return cls(name, set(tags), width, height,
+                   dead_boards=set(dead_boards), dead_links=set(dead_links),
+                   board_locations=dict(board_locations),
                    bmp_ips=bmp_ips, spinnaker_ips=spinnaker_ips)
 
 
 def board_locations_from_spinner(filename):
-    """Utility function which converts a CSV file produced by
+    """ Utility function which converts a CSV file produced by
     the `spinner-ethernet-chips
-    <http://spinner.readthedocs.org/en/stable/spinner-ethernet-chips.html>`_
+    <https://spinner.readthedocs.org/en/stable/spinner-ethernet-chips.html>`_
     utility into a ``board_locations`` dictionary suitable for defining
     :py:class:`.Machine` objects.
 
     Parameters
     ----------
     filename : str
         The name of a CSV file produced by spinner-ethernet-chips defining the
@@ -475,15 +497,15 @@
     Returns
     -------
     {(x, y, z): (c, f, b), ...}
         The mapping from board coordinates to physical locations.
     """
     # Extract lookup from Ethernet connected chips to locations
     chip_locations = {}
-    with open(filename, "r") as f:
+    with open(filename, "r", encoding="utf-8") as f:
         for entry in csv.DictReader(f):
             cfb = tuple(map(int, (entry["cabinet"],
                                   entry["frame"],
                                   entry["board"])))
 
             chip_xy = (int(entry["x"]), int(entry["y"]))
 
@@ -495,9 +517,9 @@
     width_triads = (max_x // 12) + 1
     height_triads = (max_y // 12) + 1
 
     # Convert from chip to board coordinates
     return {
         chip_to_board(chip_x, chip_y, width_triads * 12, height_triads * 12):
         cfb
-        for (chip_x, chip_y), cfb in iteritems(chip_locations)
+        for (chip_x, chip_y), cfb in chip_locations.items()
     }
```

### Comparing `spalloc_server-0.5.2/spalloc_server/allocator.py` & `spalloc_server-1!7.0.0a4/spalloc_server/allocator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,39 @@
-"""Algorithm/data structure for allocating boards in SpiNNaker machines at
+# Copyright (c) 2016 The University of Manchester
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+""" Algorithm/data structure for allocating boards in SpiNNaker machines at
 the granularity of individual SpiNNaker boards and with awareness of the
 functionality of a machine.
 """
-
 from enum import Enum
-
 from collections import deque
-
 from math import ceil
-
-from six import next
-
-from rig.links import Links
-
-from spalloc_server.pack_tree import PackTree
-from spalloc_server.area_to_rect import area_to_rect
-from spalloc_server.coordinates import board_down_link, WrapAround
+from datetime import datetime
+from .links import Links
+from .pack_tree import PackTree
+from .area_to_rect import area_to_rect
+from .coordinates import board_down_link, WrapAround
+from threading import RLock
 
 
 class Allocator(object):
-    """This object allows high-level allocation of SpiNNaker boards from a
-    larger, possibly faulty, toroidal machine.
+    """ Performs high-level allocation of SpiNNaker boards from a larger,
+    possibly faulty, toroidal machine.
 
     Internally this object uses a
     :py:class:`spalloc_server.pack_tree.PackTree` to allocate
     rectangular blocks of triads in a machine. A :py:class:`._CandidateFilter`
     to restrict the allocations made by
     :py:class:`~spalloc_server.pack_tree.PackTree` to those which match
     the needs of the user (e.g. specific connectivity requirements).
@@ -33,37 +42,43 @@
     individual boards. When allocating individual boards, the allocator
     allocates a 1x1 triad block from the
     :py:class:`~spalloc_server.pack_tree.PackTree` and returns one of
     the boards from that block. Subsequent single-board allocations will use up
     spare boards left in triads allocated for single-board allocations before
     allocating new 1x1 triads.
     """
+    # pylint: disable=too-many-arguments, unused-argument
 
     def __init__(self, width, height, dead_boards=None, dead_links=None,
-                 next_id=1):
+                 next_id=1, seconds_before_free=30):
         """
         Parameters
         ----------
         width, height : int
             Dimensions of the machine in triads.
         dead_boards : set([(x, y, z), ...])
             The set of boards which are dead and which must not be allocated.
-        dead_links : set([(x, y, z, :py:class:`rig.links.Links`), ...])
+        dead_links :set([(x, y, z,\
+                         :py:class:`spalloc_server.links.Links`), ...])
             The set of links leaving boards which are known not to be working.
             Connections to boards in the set dead_boards are assumed to be
             dead and need not be included in this list. Note that both link
             directions must be flagged as dead (if the link is bidirectionally
             down).
         next_id : int
             The ID of the next allocation to be made.
+        seconds_before_free : int
+            The number of seconds between a board being freed and it becoming
+            available again
         """
         self.width = width
         self.height = height
         self.dead_boards = dead_boards if dead_boards is not None else set()
         self.dead_links = dead_links if dead_links is not None else set()
+        self.seconds_before_free = seconds_before_free
 
         # Unique IDs are assigned to every new allocation. The next ID to be
         # allocated.
         self.next_id = next_id
 
         # A 2D tree at the granularity of triads used for board allocation.
         self.pack_tree = PackTree(0, 0, width, height)
@@ -71,14 +86,18 @@
         # Provides a lookup from (live) allocation IDs to the type of
         # allocation.
         self.allocation_types = {}
 
         # Lookup from allocation IDs to the bottom-left board in the allocation
         self.allocation_board = {}
 
+        # Storage for delayed freeing of boards
+        self.to_free = deque()
+        self.to_free_lock = RLock()
+
         # Since we cannot allocate individual boards in the pack_tree, whenever
         # an individual board is requested a whole triad may be allocated and
         # one of the boards from the triad returned. This dictionary records
         # what triads have been allocated like this and which boards are
         # unused. These may then be used for future single-board allocations
         # rather than allocating another whole triad.
 
@@ -87,18 +106,43 @@
         # {(x, y): [z, ...], ...}
         self.single_board_triads = {}
 
         # When all the boards in a triad in single_board_triads are used up the
         # triad is removed from that dictionary and placed into the set below.
         self.full_single_board_triads = set()
 
+    def __getstate__(self):
+        """ Called when pickling this object.
+
+        This object may only be pickled once
+        :py:meth:`~spalloc_server.controller.Controller.stop` and
+        :py:meth:`~spalloc_server.controller.Controller.join` have returned.
+        """
+        state = self.__dict__.copy()
+
+        # Do not keep references to unpickleable dynamic state
+        state["to_free_lock"] = None
+
+        return state
+
+    def __setstate__(self, state):
+        """ Called when unpickling this object.
+
+        Note that though the object must be pickled when stopped, the unpickled
+        object will start running immediately.
+        """
+        self.__dict__.update(state)
+
+        # Restore lock
+        self.to_free_lock = RLock()
+
     def _alloc_triads_possible(self, width, height, max_dead_boards=None,
                                max_dead_links=None, require_torus=False,
-                               min_ratio=0.0):
-        """Is it guaranteed that the specified allocation *could* succeed if
+                               min_ratio=0.0):  # @UnusedVariable
+        """ Is it guaranteed that the specified allocation *could* succeed if
         enough of the machine is free?
 
         This function may be conservative. If the specified request would fail
         when no resources have been allocated, we return False, even if some
         circumstances the allocation may succeed. For example, if one board in
         each of the four corners of the machine is dead, no allocation with
         max_dead_boards==0 can succeed when the machine is empty but may
@@ -159,16 +203,16 @@
                 return True
 
         # No possible allocation could be made...
         return False
 
     def _alloc_triads(self, width, height, max_dead_boards=None,
                       max_dead_links=None, require_torus=False,
-                      min_ratio=0.0):
-        """Allocate a rectangular block of triads of interconnected boards.
+                      min_ratio=0.0):  # @UnusedVariable
+        """ Allocate a rectangular block of triads of interconnected boards.
 
         Parameters
         ----------
         width, height : int
             The size of the block to allocate, in triads.
         max_dead_boards : int or None
             The maximum number of broken or unreachable boards to allow in the
@@ -233,15 +277,15 @@
         self.allocation_board[allocation_id] = (x, y, 0)
 
         return (allocation_id, cf.boards, cf.periphery, cf.torus)
 
     def _alloc_boards_possible(self, boards, min_ratio=0.0,
                                max_dead_boards=None, max_dead_links=None,
                                require_torus=False):
-        """Is it guaranteed that the specified allocation *could* succeed if
+        """ Is it guaranteed that the specified allocation *could* succeed if
         enough of the machine is free?
 
         This function may be conservative. If the specified request would fail
         when no resources have been allocated, we return False, even if some
         circumstances the allocation may succeed. For example, if one board in
         each of the four corners of the machine is dead, no allocation with
         max_dead_boards==0 can succeed when the machine is empty but may
@@ -312,15 +356,15 @@
                 return True
 
         # No possible allocation could be made...
         return False
 
     def _alloc_boards(self, boards, min_ratio=0.0, max_dead_boards=None,
                       max_dead_links=None, require_torus=False):
-        """Allocate a rectangular block of triads with at least the specified
+        """ Allocate a rectangular block of triads with at least the specified
         number of boards which is 'at least as square' as the specified aspect
         ratio.
 
         Parameters
         ----------
         boards : int
             The *minimum* number of boards, must be at least 1. Note that if
@@ -388,23 +432,24 @@
         if xywh is None:
             return None
 
         # If a block was allocated, store the allocation
         allocation_id = self.next_id
         self.next_id += 1
         self.allocation_types[allocation_id] = _AllocationType.triads
-        x, y, w, h = xywh
+        x, y, _, _ = xywh
         self.allocation_board[allocation_id] = (x, y, 0)
 
         return (allocation_id, cf.boards, cf.periphery, cf.torus)
 
-    def _alloc_board_possible(self, x=None, y=None, z=None,
-                              max_dead_boards=None, max_dead_links=None,
-                              require_torus=False, min_ratio=0.0):
-        """Is it guaranteed that the specified allocation *could* succeed if
+    def _alloc_board_possible(
+            self, x=None, y=None, z=None,
+            max_dead_boards=None, max_dead_links=None,  # @UnusedVariable
+            require_torus=False, min_ratio=0.0):  # @UnusedVariable
+        """ Is it guaranteed that the specified allocation *could* succeed if
         enough of the machine is free?
 
         Parameters
         ----------
         x, y, z : ints or None
             If specified, requests a specific board.
         max_dead_boards : int or None
@@ -429,34 +474,35 @@
         assert (((x is None) == (y is None) == (z is None)) or
                 ((x == 1) == (y is None) == (z is None)))
 
         board_requested = y is not None
 
         # If the requested board is outside the dimensions of the machine, the
         # request definitely can't be met.
-        if board_requested and not(0 <= x < self.width and
-                                   0 <= y < self.height and
-                                   0 <= z < 3):
+        if board_requested and not (0 <= x < self.width and
+                                    0 <= y < self.height and
+                                    0 <= z < 3):
             return False
 
         # If the requested board is dead, this should fail
         if board_requested and (x, y, z) in self.dead_boards:
             return False
 
         # If there are no working boards, we must also fail
         if len(self.dead_boards) >= (self.width * self.height * 3):
             return False
 
         # Should be possible!
         return True
 
-    def _alloc_board(self, x=None, y=None, z=None,
-                     max_dead_boards=None, max_dead_links=None,
-                     require_torus=False, min_ratio=0.0):
-        """Allocate a single board, optionally specifying a specific board to
+    def _alloc_board(
+            self, x=None, y=None, z=None,
+            max_dead_boards=None, max_dead_links=None,  # @UnusedVariable
+            require_torus=False, min_ratio=0.0):  # @UnusedVariable
+        """ Allocate a single board, optionally specifying a specific board to
         allocate.
 
         Parameters
         ----------
         x, y, z : ints or None
             If None, an arbitrary free board will be returned if possible. If
             all are defined, attempts to allocate the specific board requested
@@ -509,33 +555,35 @@
                 z = available.pop()
             else:
                 # A specific board was requested (and is available), get that
                 # one
                 available = self.single_board_triads[(x, y)]
                 available.remove(z)
 
-            # If we used up the last board, move the traid to the full list
+            # If we used up the last board, move the triad to the full list
             if not available:
                 del self.single_board_triads[(x, y)]
                 self.full_single_board_triads.add((x, y))
 
             # Allocate the board
             allocation_id = self.next_id
             self.next_id += 1
             self.allocation_types[allocation_id] = _AllocationType.board
             self.allocation_board[allocation_id] = (x, y, z)
+            # pylint: disable=not-an-iterable
             return (allocation_id,
                     set([(x, y, z)]),
                     set((x, y, z, link) for link in Links),
                     WrapAround.none)
 
         # The desired board was not available in an already-allocated triad.
         # Attempt to request that triad.
 
-        def has_at_least_one_working_board(x, y, width, height):
+        def has_at_least_one_working_board(
+                x, y, width, height):  # @UnusedVariable
             num_dead = 0
             for z in range(3):
                 if (x, y, z) in self.dead_boards:
                     num_dead += 1
 
             return num_dead < 3
 
@@ -554,18 +602,19 @@
         self.single_board_triads[xy] = \
             set(z for z in range(3)
                 if (xy[0], xy[1], z) not in self.dead_boards)
 
         # Recursing will return a board from the triad
         return self._alloc_board(x, y, z)
 
-    def _alloc_type(self, x_or_num_or_width=None, y_or_height=None, z=None,
-                    max_dead_boards=None, max_dead_links=None,
-                    require_torus=False, min_ratio=0.0):
-        """Returns the type of allocation the user is attempting to make (and
+    def _alloc_type(
+            self, x_or_num_or_width=None, y_or_height=None, z=None,
+            max_dead_boards=None, max_dead_links=None,  # @UnusedVariable
+            require_torus=False, min_ratio=0.0):  # @UnusedVariable
+        """ Returns the type of allocation the user is attempting to make (and
         fails if it is invalid.
 
         Usage::
 
             a.alloc()  # Allocate any single board
             a.alloc(1)  # Allocate any single board
             a.alloc(3, 2, 1)  # Allocate the specific board (3, 2, 1)
@@ -609,15 +658,15 @@
             args.append(x_or_num_or_width)
             if y_or_height is not None:
                 args.append(y_or_height)
                 if z is not None:
                     args.append(z)
 
         # Select allocation type
-        if len(args) == 0:
+        if not args:
             alloc_type = _AllocationType.board
         elif len(args) == 1:
             if args[0] == 1:
                 alloc_type = _AllocationType.board
             else:
                 alloc_type = _AllocationType.boards
         elif len(args) == 2:
@@ -630,15 +679,15 @@
             if require_torus:
                 raise ValueError(
                     "require_torus must be False when allocating boards.")
 
         return alloc_type
 
     def alloc_possible(self, *args, **kwargs):
-        """Is the specified allocation actually possible on this machine?
+        """ Is the specified allocation actually possible on this machine?
 
         Usage::
 
             a.alloc_possible()  # Can allocate a single board?
             a.alloc_possible(1)  # Can allocate a single board?
             a.alloc_possible(4)  # Can allocate at least 4 boards?
             a.alloc_possible(3, 2, 1)  # Can allocate a board (3, 2, 1)?
@@ -680,19 +729,18 @@
         bool
         """
         alloc_type = self._alloc_type(*args, **kwargs)
         if alloc_type is _AllocationType.board:
             return self._alloc_board_possible(*args, **kwargs)
         elif alloc_type is _AllocationType.boards:
             return self._alloc_boards_possible(*args, **kwargs)
-        else:
-            return self._alloc_triads_possible(*args, **kwargs)
+        return self._alloc_triads_possible(*args, **kwargs)
 
     def alloc(self, *args, **kwargs):
-        """Attempt to allocate a board or rectangular region of triads of
+        """ Attempt to allocate a board or rectangular region of triads of
         boards.
 
         Usage::
 
             a.alloc()  # Allocate a single board
             a.alloc(1)  # Allocate a single board
             a.alloc(4)  # Allocate at least 4 boards
@@ -740,38 +788,61 @@
             the allocation with the :py:meth:`.free` method. ``boards`` is a
             set of (x, y, z) tuples giving the locations of to allocated
             boards.  ``periphery`` is a set of (x, y, z, link) tuples giving
             the links which leave the allocated set of boards. ``torus`` is a
             :py:class:`.WrapAround` value indicating torus connectivity when at
             least one torus may exist.
         """
+        # Free things that can now be freed
+        self.check_free()
+
+        # Do the allocation
         alloc_type = self._alloc_type(*args, **kwargs)
         if alloc_type is _AllocationType.board:
             return self._alloc_board(*args, **kwargs)
         elif alloc_type is _AllocationType.boards:
             return self._alloc_boards(*args, **kwargs)
-        else:
-            return self._alloc_triads(*args, **kwargs)
+        return self._alloc_triads(*args, **kwargs)
 
     def free(self, allocation_id):
-        """Free the resources consumed by the specified allocation.
+        """ Free the resources consumed by the specified allocation.
 
         Parameters
         ----------
         allocation_id : int
             The ID of the allocation to free.
         """
-        type = self.allocation_types.pop(allocation_id)
+        _type = self.allocation_types.pop(allocation_id)
         x, y, z = self.allocation_board.pop(allocation_id)
+        with self.to_free_lock:
+            self.to_free.append((datetime.now(), _type, x, y, z))
 
-        if type is _AllocationType.triads:
+    def check_free(self):
+        """ Free any of the items on the "to free" list that have expired
+        """
+        changed = False
+        with self.to_free_lock:
+            while self.to_free:
+                free_time, _, _, _, _ = self.to_free[0]
+                time_diff = (datetime.now() - free_time).total_seconds()
+                if time_diff < self.seconds_before_free:
+                    break
+                self._free_next()
+                changed = True
+        return changed
+
+    def _free_next(self):
+        """ Free the next item on the "to_free" list
+        """
+        _, _type, x, y, z = self.to_free.popleft()
+        if _type is _AllocationType.triads:
             # Simply free the allocation
             self.pack_tree.free(x, y)
-        elif type is _AllocationType.board:
-            # If the traid the board came from was full, it now isn't...
+        elif _type is _AllocationType.board:
+            # If the triad the board came from was full, it now isn't...
             if (x, y) in self.full_single_board_triads:
                 self.full_single_board_triads.remove((x, y))
                 self.single_board_triads[(x, y)] = set()
 
             # Return the board to the set available in that triad
             self.single_board_triads[(x, y)].add(z)
 
@@ -783,63 +854,67 @@
                 del self.single_board_triads[(x, y)]
                 self.pack_tree.free(x, y)
         else:  # pragma: no cover
             assert False, "Unknown allocation type!"
 
 
 class _AllocationType(Enum):
-    """Type identifiers for allocations."""
+    """ Type identifiers for allocations.
+    """
 
     triads = 0
-    """A rectangular block of triads."""
+    """ A rectangular block of triads.
+    """
 
     board = 1
-    """A single board."""
+    """ A single board.
+    """
 
     boards = 2
-    """Two or more boards, to be allocated as triads.
+    """ Two or more boards, to be allocated as triads.
 
     This type only returned by :py:meth:`.Allocator._alloc_type` and is never
     used as an allocation type.
     """
 
 
 class _CandidateFilter(object):
-    """A callable object which, given a rectangular region of triads will check
+    """ A filter which, given a rectangular region of triads, will check
     to see if it meets some set of criteria.
 
     If any candidate is accepted the following attributes are set according to
     the last accepted candidate.
 
     Attributes
     ----------
     boards : set([(x, y, z), ...])
         The working boards present in the accepted candidate. None if no
         candidate has been accepted.
-    periphery : set([(x, y, z, :py:class:`rig.links.Links`), ...])
+    periphery : set([(x, y, z, :py:class:`spalloc_server.links.Links`), ...])
         The links around the periphery of the selection of boards which should
         be disabled to isolate the system. None if no candidate has been
         accepted.
     torus : :py:class:`.WrapAround`
         Describes the types of wrap-around links the candidate has.
     """
 
     def __init__(self, width, height, dead_boards, dead_links,
                  max_dead_boards, max_dead_links, require_torus,
                  expected_boards=None):
-        """Create a new candidate filter.
+        """ Create a new candidate filter.
 
         Parameters
         ----------
         width, height : int
             Dimensions (in triads) of the system within which candidates are
             being chosen.
         dead_boards : set([(x, y, z), ...])
             The set of boards which are dead and which must not be allocated.
-        dead_links : set([(x, y, z, :py:class:`rig.links.Links`), ...])
+        dead_links : set([(x, y, z,\
+                           :py:class:`spalloc_server.links.Links`), ...])
             The set of links leaving boards which are known not to be working.
             Connections to boards in the set dead_boards are assumed to be
             dead and need not be included in this list. Note that both link
             directions must be flagged as dead (if the link is bidirectionally
             down).
         max_dead_boards : int or None
             The maximum number of broken or unreachable boards to allow in the
@@ -848,39 +923,40 @@
             None).
         max_dead_links : int or None
             The maximum number of broken links allow in the allocated region.
             When require_torus is True this includes wrap-around links,
             otherwise peripheral links are not counted.  If None, any number of
             broken links is allowed. (Default: None).
         require_torus : bool
-            If True, only allocatae blocks with torus connectivity. In general
+            If True, only allocate blocks with torus connectivity. In general
             this will only succeed for requests to allocate an entire machine
             (when the machine is otherwise not in use!). (Default: False)
         expected_boards : int or None
             If given, specifies the number of boards which are expected to be
             in a candidate. This ensures that when an over-allocation is made,
             the max_dead_boards figure is offset by any over-allocation.
 
             If None, assumes the candidate width * candidate height * 3.
         """
+        # pylint: disable=too-many-arguments
         self.width = width
         self.height = height
         self.dead_boards = dead_boards
         self.dead_links = dead_links
         self.max_dead_boards = max_dead_boards
         self.max_dead_links = max_dead_links
         self.require_torus = require_torus
         self.expected_boards = expected_boards
 
         self.boards = None
         self.periphery = None
         self.torus = None
 
     def _enumerate_boards(self, x, y, width, height):
-        """Starting from board (x, y, 0), enumerate as many reachable and
+        """ Starting from board (x, y, 0), enumerate as many reachable and
         working boards as possible within the rectangle width x height triads.
 
         Returns
         -------
         set([(x, y, z), ...])
         """
         # The set of visited (and working) boards
@@ -894,97 +970,92 @@
             if ((x1, y1, z1) in self.dead_boards or
                     (x1, y1, z1) in boards):
                 continue
 
             boards.add((x1, y1, z1))
 
             # Visit neighbours which are within the range
-            for link in Links:
+            for link in Links:  # pylint: disable=not-an-iterable
                 # Skip dead links
                 if (x1, y1, z1, link) in self.dead_links:
                     continue
 
-                x2, y2, z2, _ = board_down_link(x1, y1, z1, link,
-                                                self.width, self.height)
+                x2, y2, z2, _ = board_down_link(
+                    x1, y1, z1, link, self.width, self.height)
 
-                # Skip links to boards outside the specified range
-                if not (x <= x2 < x + width and
+                # Only process links to boards in the specified range
+                if (x <= x2 < x + width and
                         y <= y2 < y + height):
-                    continue
-
-                to_visit.append((x2, y2, z2))
+                    to_visit.append((x2, y2, z2))
 
         # Return the set of boards we could reach
         return boards
 
     def _classify_links(self, boards):
-        """Get a list of links of various classes connected to the supplied set
-        of boards.
+        """ Get a list of links of various classes connected to the supplied
+        set of boards.
 
         Parameters
         ----------
         boards : set([(x, y, z), ...])
             A set of fully-connected, alive boards.
 
         Returns
         -------
-        alive : set([(x, y, z, :py:class:`rig.links.Links`), ...])
+        alive : set([(x, y, z, :py:class:`.links.Links`), ...])
             Links which are working and connect one board
             in the set to another.
-        wrap : set([(x, y, z, :py:class:`rig.links.Links`), ...])
+        wrap : set([(x, y, z, :py:class:`.links.Links`), ...])
             Working links between working boards in the set which wrap-around
             the toroid.
-        dead : set([(x, y, z, :py:class:`rig.links.Links`), ...])
+        dead : set([(x, y, z, :py:class:`.links.Links`), ...])
             Links which are not working and connect one board in the set to
             another.
-        dead_wrap : set([(x, y, z, :py:class:`rig.links.Links`), ...])
+        dead_wrap : set([(x, y, z, :py:class:`.links.Links`), ...])
             Dead links between working boards in the set which wrap-around the
             toroid.
-        periphery : set([(x, y, z, :py:class:`rig.links.Links`), ...])
+        periphery : set([(x, y, z, :py:class:`.links.Links`), ...])
             Links are those which connect from one board in the set to a board
             outside the set. These links may be dead or alive.
         wrap_around_type : :py:class:`~spalloc_server.coordinates.WrapAround`
             What types of wrap-around links are present (making no distinction
             between dead and alive links)?
         """
+        # pylint: disable=too-many-locals
         alive = set()
         wrap = set()
         dead = set()
         dead_wrap = set()
         periphery = set()
         wrap_around_type = WrapAround.none
 
         for x1, y1, z1 in boards:
-            for link in Links:
-                is_dead = (x1, y1, z1, link) in self.dead_links
-                x2, y2, z2, wrapped = board_down_link(x1, y1, z1, link,
-                                                      self.width, self.height)
-                in_set = (x2, y2, z2) in boards
-
-                if in_set:
+            for link in Links:  # pylint: disable=not-an-iterable
+                x2, y2, z2, wrapped = board_down_link(
+                    x1, y1, z1, link, self.width, self.height)
+                if (x2, y2, z2) in boards:
                     wrap_around_type |= wrapped
-
                     if wrapped:
-                        if is_dead:
+                        if (x1, y1, z1, link) in self.dead_links:
                             dead_wrap.add((x1, y1, z1, link))
                         else:
                             wrap.add((x1, y1, z1, link))
                     else:
-                        if is_dead:
+                        if (x1, y1, z1, link) in self.dead_links:
                             dead.add((x1, y1, z1, link))
                         else:
                             alive.add((x1, y1, z1, link))
                 else:
                     periphery.add((x1, y1, z1, link))
 
-        return (alive, wrap, dead, dead_wrap, periphery,
-                WrapAround(wrap_around_type))
+        return alive, wrap, dead, dead_wrap, periphery, \
+            WrapAround(wrap_around_type)
 
     def __call__(self, x, y, width, height):
-        """Test whether the region specified meets the stated requirements.
+        """ Test whether the region specified meets the stated requirements.
 
         If True is returned, the set of boards in the region is stored in
         self.boards and the set of links on the periphery are stored in
         self.periphery.
         """
         boards = self._enumerate_boards(x, y, width, height)
 
@@ -994,29 +1065,27 @@
                 expected_boards = self.expected_boards
             else:
                 expected_boards = width * height * 3
             alive = len(boards)
             dead = expected_boards - alive
             if alive == 0 or dead > self.max_dead_boards:
                 return False
-        else:
-            if len(boards) == 0:
-                return False
+        elif not boards:
+            return False
 
         # Make sure the maximum dead links limit isn't exceeded (and that torus
         # links exist if requested)
-        (alive, wrap, dead, dead_wrap, periphery, wrap_around_type) = \
+        alive, _, dead, dead_wrap, periphery, wrap_around_type = \
             self._classify_links(boards)
         if self.require_torus and wrap_around_type == WrapAround.none:
             return False
         if self.max_dead_links is not None:
+            dead_links = len(dead)
             if self.require_torus:
-                dead_links = len(dead) + len(dead_wrap)
-            else:
-                dead_links = len(dead)
+                dead_links += len(dead_wrap)
             if dead_links > self.max_dead_links:
                 return False
 
         # All looks good, accept this region and keep the enumerated boards and
         # peripheral links
         self.boards = boards
         self.periphery = periphery
```

### Comparing `spalloc_server-0.5.2/spalloc_server/area_to_rect.py` & `spalloc_server-1!7.0.0a4/spalloc_server/area_to_rect.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,30 @@
-"""Utility functions for working out sensible sizes of machine to allocate
+# Copyright (c) 2016 The University of Manchester
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+""" Utility functions for working out sensible sizes of machine to allocate
 given a minimum number of boards and worst-case aspect ratio.
 """
 
 from math import sqrt, ceil
 
 
 def area_to_rect(area, bound_width, bound_height, min_ratio=0.0):
-    """Given an area requirement, select a rectangular subregion of the given
+    """ Given an area requirement, select a rectangular subregion of the given
     width and height bounds whose aspect ratio (when rotated into a landscape
     orientation) is at least that specified.
 
     Parameters
     ----------
     area : int
         Lower-bound on area requirement.
@@ -74,28 +88,28 @@
 
     # If squishing didn't violate the aspect ratio requirement, we're good.
     # Note: We know that the requested area fits within the bounds of the
     # system and thus squishing can never result in something which doesn't
     # fit.
     if float(min(w, h)) / float(max(w, h)) >= min_ratio:
         return (w, h)
-    else:
-        return None
+    return None
 
 
 def squarest_rectangle(area):
-    """Given a specific area, calculate the squarest possible rectangle with
+    """ Given a specific area, calculate the squarest possible rectangle with
     exactly that area, preferring landscape rectangles.
 
     Returns
     -------
     (w, h)
         Width and height of a rectangle with the area specified where w and h
         are as similar as possible and w >= h.
     """
+    # pylint: disable=undefined-loop-variable
     assert area >= 0
 
     # Special case
     if area == 0:
         return (0, 0)
 
     # Find the largest pair of factors to discover the squarest rectangle
@@ -107,15 +121,15 @@
 
     w = area // h
 
     return (w, h)
 
 
 def rectangle_with_aspect_ratio(area, ratio):
-    """Return a (landscape) rectangle with at least the specified area and
+    """ Return a (landscape) rectangle with at least the specified area and
     aspect ratio.
 
     Note that the returned rectangles are not at all guaranteed to be the
     'squarest' possible, just greater than the specified ratio. This is
     intended to generate alternatives to the very wide rectangles produced by
     squarest_rectangle when prime (or 'nearly prime') numbers of boards are
     requested.
```

### Comparing `spalloc_server-0.5.2/README.rst` & `spalloc_server-1!7.0.0a4/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 SpiNNaker Machine Partitioning and Allocation Server (``spalloc_server``)
 =========================================================================
 
 .. image:: https://img.shields.io/pypi/v/spalloc_server.svg?style=flat
-   :alt: PyPi version
-   :target: https://pypi.python.org/pypi/spalloc_server/
+ :target: https://pypi.python.org/pypi/spalloc_server/
+ :alt: PyPi version
 .. image:: https://readthedocs.org/projects/spalloc_server/badge/?version=stable
-   :alt: Documentation
-   :target: http://spalloc_server.readthedocs.org/
-.. image:: https://travis-ci.org/SpiNNakerManchester/spalloc_server.svg?branch=master
-   :alt: Build Status
-   :target: https://travis-ci.org/SpiNNakerManchester/spalloc_server
+ :target: https://spalloc_server.readthedocs.org/
+ :alt: Documentation
+.. image:: https://github.com/SpiNNakerManchester/spalloc_server/workflows/Python%20Build/badge.svg?branch=master
+ :alt: Build Status
+ :target: https://github.com/SpiNNakerManchester/spalloc_server/actions?query=workflow%3A%22Python+Build%22+branch%3Amaster
 .. image:: https://coveralls.io/repos/SpiNNakerManchester/spalloc_server/badge.svg?branch=master
-   :alt: Coverage Status
-   :target: https://coveralls.io/r/SpiNNakerManchester/spalloc_server?branch=master
+ :target: https://coveralls.io/r/SpiNNakerManchester/spalloc_server?branch=master
+ :alt: Coverage Status
 
 A SpiNNaker machine management application which manages the partitioning and
 allocation of large SpiNNaker machines into smaller fragments for many
 simultaneous users.
 
 This package just contains a server which exposes a simple TCP interface to
 clients to enable them to request hardware.
 
-The `documentation <http://spalloc-server.readthedocs.org/>`_ describes the
+The `documentation <https://spalloc-server.readthedocs.org/>`_ describes the
 process of configuring and running servers, the simple JSON-based client
 protocol and an overview of the server's implementation.
```

