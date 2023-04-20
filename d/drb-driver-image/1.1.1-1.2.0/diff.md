# Comparing `tmp/drb-driver-image-1.1.1.tar.gz` & `tmp/drb-driver-image-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-image-1.1.1.tar", last modified: Fri Feb 10 10:45:58 2023, max compression
+gzip compressed data, was "drb-driver-image-1.2.0.tar", last modified: Thu Apr 20 13:45:43 2023, max compression
```

## Comparing `drb-driver-image-1.1.1.tar` & `drb-driver-image-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:45:58.080877 drb-driver-image-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-18 15:53:50.000000 drb-driver-image-1.1.1/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-12-20 15:01:55.000000 drb-driver-image-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2170 2023-02-10 10:45:58.080877 drb-driver-image-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1539 2022-12-20 15:01:55.000000 drb-driver-image-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:45:58.072877 drb-driver-image-1.1.1/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:45:58.072877 drb-driver-image-1.1.1/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:45:58.084877 drb-driver-image-1.1.1/drb/drivers/image/
--rw-rw-rw-   0 root         (0) root         (0)      310 2022-12-20 15:01:55.000000 drb-driver-image-1.1.1/drb/drivers/image/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-02-10 10:45:58.084877 drb-driver-image-1.1.1/drb/drivers/image/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     7586 2022-12-20 15:01:55.000000 drb-driver-image-1.1.1/drb/drivers/image/base_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3562 2022-12-20 15:01:55.000000 drb-driver-image-1.1.1/drb/drivers/image/list_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3588 2022-12-20 15:01:55.000000 drb-driver-image-1.1.1/drb/drivers/image/simple_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:45:58.080877 drb-driver-image-1.1.1/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)      188 2022-12-20 15:01:55.000000 drb-driver-image-1.1.1/drb/exceptions/image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:45:58.072877 drb-driver-image-1.1.1/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:45:58.080877 drb-driver-image-1.1.1/drb/topics/image/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 15:01:55.000000 drb-driver-image-1.1.1/drb/topics/image/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2022-12-20 15:01:55.000000 drb-driver-image-1.1.1/drb/topics/image/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 10:45:58.080877 drb-driver-image-1.1.1/drb_driver_image.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2170 2023-02-10 10:45:57.000000 drb-driver-image-1.1.1/drb_driver_image.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      561 2023-02-10 10:45:57.000000 drb-driver-image-1.1.1/drb_driver_image.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-10 10:45:57.000000 drb-driver-image-1.1.1/drb_driver_image.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2023-02-10 10:45:57.000000 drb-driver-image-1.1.1/drb_driver_image.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-02-10 10:45:57.000000 drb-driver-image-1.1.1/drb_driver_image.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-02-10 10:45:57.000000 drb-driver-image-1.1.1/drb_driver_image.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-02-10 10:06:58.000000 drb-driver-image-1.1.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-02-10 10:45:58.084877 drb-driver-image-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1339 2023-02-10 10:35:43.000000 drb-driver-image-1.1.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    78254 2022-03-22 16:40:06.000000 drb-driver-image-1.1.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.915057 drb-driver-image-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-18 15:53:50.000000 drb-driver-image-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       60 2022-12-20 15:01:55.000000 drb-driver-image-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2084 2023-04-20 13:45:43.915057 drb-driver-image-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2022-12-20 15:01:55.000000 drb-driver-image-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.871056 drb-driver-image-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.871056 drb-driver-image-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.919057 drb-driver-image-1.2.0/drb/drivers/image/
+-rw-rw-rw-   0 root         (0) root         (0)      310 2022-12-20 15:01:55.000000 drb-driver-image-1.2.0/drb/drivers/image/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-20 13:45:43.919057 drb-driver-image-1.2.0/drb/drivers/image/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     7904 2023-04-20 13:23:36.000000 drb-driver-image-1.2.0/drb/drivers/image/base_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2023-04-19 16:07:18.000000 drb-driver-image-1.2.0/drb/drivers/image/list_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1979 2023-04-19 16:07:18.000000 drb-driver-image-1.2.0/drb/drivers/image/simple_node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.895056 drb-driver-image-1.2.0/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2022-12-20 15:01:55.000000 drb-driver-image-1.2.0/drb/exceptions/image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.871056 drb-driver-image-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.895056 drb-driver-image-1.2.0/drb/topics/image/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 15:01:55.000000 drb-driver-image-1.2.0/drb/topics/image/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-04-20 13:44:38.000000 drb-driver-image-1.2.0/drb/topics/image/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.899056 drb-driver-image-1.2.0/drb_driver_image.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2084 2023-04-20 13:45:43.000000 drb-driver-image-1.2.0/drb_driver_image.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-20 13:45:43.000000 drb-driver-image-1.2.0/drb_driver_image.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 13:45:43.000000 drb-driver-image-1.2.0/drb_driver_image.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-04-20 13:45:43.000000 drb-driver-image-1.2.0/drb_driver_image.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 13:45:43.000000 drb-driver-image-1.2.0/drb_driver_image.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2023-04-20 13:45:43.000000 drb-driver-image-1.2.0/drb_driver_image.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-20 13:45:43.000000 drb-driver-image-1.2.0/drb_driver_image.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-20 12:54:00.000000 drb-driver-image-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-19 16:07:18.000000 drb-driver-image-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-04-20 13:45:43.919057 drb-driver-image-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-19 16:07:18.000000 drb-driver-image-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:45:43.915057 drb-driver-image-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3441 2023-03-29 11:51:14.000000 drb-driver-image-1.2.0/tests/test_drb_image_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6710 2022-12-20 15:01:55.000000 drb-driver-image-1.2.0/tests/test_drb_image_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2694 2023-04-19 16:07:18.000000 drb-driver-image-1.2.0/tests/test_drb_image_node_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-04-19 16:07:18.000000 drb-driver-image-1.2.0/tests/test_drb_image_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     3622 2022-12-20 15:01:55.000000 drb-driver-image-1.2.0/tests/test_drb_image_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3534 2023-03-29 11:51:14.000000 drb-driver-image-1.2.0/tests/test_drb_image_value_node.py
+-rw-rw-rw-   0 root         (0) root         (0)    78254 2022-03-22 16:40:06.000000 drb-driver-image-1.2.0/versioneer.py
```

### Comparing `drb-driver-image-1.1.1/LICENCE.txt` & `drb-driver-image-1.2.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.1.1/PKG-INFO` & `drb-driver-image-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: drb-driver-image
-Version: 1.1.1
+Version: 1.2.0
 Summary: DRB Image driver
-Home-page: https://gitlab.com/drb-python/impl/image
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/image
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/image
 Project-URL: Source, https://gitlab.com/drb-python/impl/image
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # ImageNode Implementation
 This drb-driver-image module implements images data formats to be accessed with DRB data model. It is able to navigates among the images contents and accessing the image data.
 
@@ -38,9 +36,7 @@
 ## limitations
 The current version does not manage child modification and insertion. ImageNode is currently read only.
 ## Using this module
 To include this module into your project, the `drb-driver-image` module shall be referenced into `requirement.txt` file, or the following pip line can be run:
 ```commandline
 pip install drb-driver-image
 ```
-
-
```

### Comparing `drb-driver-image-1.1.1/README.md` & `drb-driver-image-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.1.1/drb/drivers/image/base_node.py` & `drb-driver-image-1.2.0/drb/drivers/image/base_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 from typing import Any, List, Optional, Dict, Tuple
 
-import drb
 import numpy
 import rasterio as rasterio
 import xarray
+from deprecated.classic import deprecated
 from rasterio.io import MemoryFile
 
 from drb.core import DrbNode
 from drb.nodes.abstract_node import AbstractNode
 from drb.exceptions.core import DrbNotImplementationException
 from drb.core.factory import DrbFactory
 from drb.core.path import ParsedPath
@@ -24,15 +24,25 @@
     def __init__(self, base_node: DrbNode):
         super().__init__()
 
         self.base_node = base_node
         self._data_set = None
         self._data_set_file_source = None
         self._data_xarray = None
+        self.parent = self.base_node.parent
+        self.name = self.base_node.name
+        self.namespace_uri = self.base_node.namespace_uri
+        self.value = self.base_node.value
         self._children: List[DrbNode] = None
+        self._available_impl = [
+            rasterio.DatasetReader,
+            numpy.ndarray,
+            xarray.DataArray
+        ]
+        self._available_impl += self.base_node._available_impl
 
     def _get_rasterio_impl(self):
         return self._get_data_set()
 
     def _get_numpy_ndarray_impl(self):
         return self._get_data_set().read()
 
@@ -41,38 +51,32 @@
 
     supported_impl = {
         rasterio.DatasetReader: _get_rasterio_impl,
         numpy.ndarray: _get_numpy_ndarray_impl,
         xarray.DataArray: get_xarray_impl
     }
 
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return self.base_node.parent
+    def __setitem__(self, key, value):
+        raise NotImplementedError
+
+    def __delitem__(self, key):
+        raise NotImplementedError
 
     @property
     def path(self) -> ParsedPath:
         return self.base_node.path
 
     @property
-    def name(self) -> str:
-        return self.base_node.name
-
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return self.base_node.namespace_uri
-
-    @property
-    def value(self) -> Optional[Any]:
-        return self.base_node.value
-
-    @property
+    @deprecated(version='1.2.0',
+                reason='Usage of the @ operator is recommended')
     def attributes(self) -> Dict[Tuple[str, str], Any]:
         return self.base_node.attributes
 
+    @deprecated(version='1.2.0',
+                reason='Usage of the @ operator is recommended')
     def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
         return self.base_node.get_attribute(name, namespace_uri)
 
     def close(self):
         if self._data_set is not None:
             self._data_set.close()
         if self._data_set_file_source is not None:
@@ -163,14 +167,16 @@
         for node_name, value in dictionary.items():
             node_value = DrbImageSimpleValueNode(list_node, node_name, value)
             list_node.append_child(node_value)
 
         self._children.append(list_node)
 
     @property
+    @deprecated(version='1.2.0',
+                reason='Usage of the bracket is recommended')
     @resolve_children
     def children(self) -> List[DrbNode]:
         """
         Initiate the list of children containing some metadata,
         and the data of the image.
 
         Returns:
@@ -198,19 +204,14 @@
                 self._add_values_from_dict(DrbImageNodesValueNames.TAGS.value,
                                            data_set.tags())
             if data_set.tags() is not None:
                 self._add_values_from_dict(DrbImageNodesValueNames.META.value,
                                            data_set.meta)
         return self._children
 
-    def has_impl(self, impl: type) -> bool:
-        if self.base_node.has_impl(impl):
-            return True
-        return impl in self.supported_impl.keys()
-
     def get_impl(self, impl: type) -> Any:
         if self.base_node.has_impl(impl):
             return self.base_node.get_impl(impl)
         try:
             return self.supported_impl[impl](self)
         except KeyError:
             raise DrbNotImplementationException(
```

### Comparing `drb-driver-image-1.1.1/drb/topics/image/cortex.yml` & `drb-driver-image-1.2.0/drb/topics/image/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-driver-image-1.1.1/drb_driver_image.egg-info/PKG-INFO` & `drb-driver-image-1.2.0/drb_driver_image.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: drb-driver-image
-Version: 1.1.1
+Version: 1.2.0
 Summary: DRB Image driver
-Home-page: https://gitlab.com/drb-python/impl/image
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/image
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/image
 Project-URL: Source, https://gitlab.com/drb-python/impl/image
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # ImageNode Implementation
 This drb-driver-image module implements images data formats to be accessed with DRB data model. It is able to navigates among the images contents and accessing the image data.
 
@@ -38,9 +36,7 @@
 ## limitations
 The current version does not manage child modification and insertion. ImageNode is currently read only.
 ## Using this module
 To include this module into your project, the `drb-driver-image` module shall be referenced into `requirement.txt` file, or the following pip line can be run:
 ```commandline
 pip install drb-driver-image
 ```
-
-
```

### Comparing `drb-driver-image-1.1.1/versioneer.py` & `drb-driver-image-1.2.0/versioneer.py`

 * *Files identical despite different names*

