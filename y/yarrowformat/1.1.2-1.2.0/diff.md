# Comparing `tmp/yarrowformat-1.1.2.tar.gz` & `tmp/yarrowformat-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yarrowformat-1.1.2.tar", last modified: Fri Feb  3 17:34:20 2023, max compression
+gzip compressed data, was "dist/yarrowformat-1.2.0.tar", last modified: Thu Apr 20 09:47:27 2023, max compression
```

## Comparing `yarrowformat-1.1.2.tar` & `yarrowformat-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)      884 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11380 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    81180 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/versioneer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1899 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/src/yarrowformat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/src/yarrowformat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/src/yarrowformat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/src/yarrowformat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/src/yarrowformat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/src/yarrowformat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/src/yarrowformat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/src/yarrowformat.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/src/yarrow/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/src/yarrow/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/src/yarrow/cli/check.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/src/yarrow/cli/save.py
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/src/yarrow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/src/yarrow/cli/open.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-02-03 17:34:20.000000 yarrowformat-1.1.2/src/yarrow/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    21762 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/src/yarrow/yarrow.py
--rw-r--r--   0 runner    (1001) docker     (122)    24514 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/src/yarrow/yarrow_cls.py
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/src/yarrow/_yarrow_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/src/yarrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/src/yarrow/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     6466 2023-02-03 17:34:15.000000 yarrowformat-1.1.2/src/yarrow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2037 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    81180 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrow/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/_yarrow_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29424 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/yarrow_cls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrow/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/cli/save.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/cli/open.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/cli/check.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrow/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13733 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/yarrow.py
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6466 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      884 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    11380 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/setup.py
```

### Comparing `yarrowformat-1.1.2/setup.cfg` & `yarrowformat-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.1.2/PKG-INFO` & `yarrowformat-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yarrowformat
-Version: 1.1.2
+Version: 1.2.0
 Summary: Yarrow Format parsing lib
 Home-page: https://github.com/michelin/YarrowFormat
 Author: Mathieu Pichon
 Author-email: mathieu.pichon_ext@michelin.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -22,14 +22,16 @@
 
 **yarrow** is a python package to parse, manipulate and serialize data
 following the yarrow [data schema](/schema/yarrow_schema.json). This format is
 oriented around computer vision data and is heavily inspired by the COCO
 [dataset format](https://cocodataset.org/#format-data) and was initially developed
 and used in Michelin projects.
 
+The full description can be found [here](schema/description.md) with the rules on how to fill different fields.
+
 ## How to install
 
 ```sh
 pip install yarrowformat
 ```
 
 ## How to use
@@ -53,12 +55,16 @@
 
 # now save it somewhere else
 with open("path/to/other/file.yarrow.json", "w") as fp:
     json.dump(yar_set.pydantic().dict(), fp, default=str)
 
 ```
 
+## Format explanation
+
+
+
 ## License
 
 [Apache 2.0](LICENSE)
```

### Comparing `yarrowformat-1.1.2/LICENSE` & `yarrowformat-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.1.2/versioneer.py` & `yarrowformat-1.2.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.1.2/README.md` & `yarrowformat-1.2.0/src/yarrowformat.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,37 @@
+Metadata-Version: 2.1
+Name: yarrowformat
+Version: 1.2.0
+Summary: Yarrow Format parsing lib
+Home-page: https://github.com/michelin/YarrowFormat
+Author: Mathieu Pichon
+Author-email: mathieu.pichon_ext@michelin.com
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # Yarrow: a data format for computer vision
 
 ---------------
 
 [![PyPI version](https://badge.fury.io/py/yarrowformat.svg)](https://badge.fury.io/py/yarrowformat) [![Documentation Status](https://readthedocs.org/projects/yarrowformat/badge/?version=latest)](https://yarrowformat.readthedocs.io/en/latest/?badge=latest) [![Test and Deploy](https://github.com/michelin/YarrowFormat/actions/workflows/test-deploy.yaml/badge.svg)](https://github.com/michelin/YarrowFormat/actions/workflows/test-deploy.yaml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 ## What is it ?
 
 **yarrow** is a python package to parse, manipulate and serialize data
 following the yarrow [data schema](/schema/yarrow_schema.json). This format is
 oriented around computer vision data and is heavily inspired by the COCO
 [dataset format](https://cocodataset.org/#format-data) and was initially developed
 and used in Michelin projects.
 
+The full description can be found [here](schema/description.md) with the rules on how to fill different fields.
+
 ## How to install
 
 ```sh
 pip install yarrowformat
 ```
 
 ## How to use
@@ -39,10 +55,16 @@
 
 # now save it somewhere else
 with open("path/to/other/file.yarrow.json", "w") as fp:
     json.dump(yar_set.pydantic().dict(), fp, default=str)
 
 ```
 
+## Format explanation
+
+
+
 ## License
 
 [Apache 2.0](LICENSE)
+
+
```

### Comparing `yarrowformat-1.1.2/src/yarrowformat.egg-info/SOURCES.txt` & `yarrowformat-1.2.0/src/yarrowformat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.1.2/src/yarrowformat.egg-info/PKG-INFO` & `yarrowformat-1.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,23 @@
-Metadata-Version: 2.1
-Name: yarrowformat
-Version: 1.1.2
-Summary: Yarrow Format parsing lib
-Home-page: https://github.com/michelin/YarrowFormat
-Author: Mathieu Pichon
-Author-email: mathieu.pichon_ext@michelin.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Yarrow: a data format for computer vision
 
 ---------------
 
 [![PyPI version](https://badge.fury.io/py/yarrowformat.svg)](https://badge.fury.io/py/yarrowformat) [![Documentation Status](https://readthedocs.org/projects/yarrowformat/badge/?version=latest)](https://yarrowformat.readthedocs.io/en/latest/?badge=latest) [![Test and Deploy](https://github.com/michelin/YarrowFormat/actions/workflows/test-deploy.yaml/badge.svg)](https://github.com/michelin/YarrowFormat/actions/workflows/test-deploy.yaml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 ## What is it ?
 
 **yarrow** is a python package to parse, manipulate and serialize data
 following the yarrow [data schema](/schema/yarrow_schema.json). This format is
 oriented around computer vision data and is heavily inspired by the COCO
 [dataset format](https://cocodataset.org/#format-data) and was initially developed
 and used in Michelin projects.
 
+The full description can be found [here](schema/description.md) with the rules on how to fill different fields.
+
 ## How to install
 
 ```sh
 pip install yarrowformat
 ```
 
 ## How to use
@@ -53,12 +41,14 @@
 
 # now save it somewhere else
 with open("path/to/other/file.yarrow.json", "w") as fp:
     json.dump(yar_set.pydantic().dict(), fp, default=str)
 
 ```
 
-## License
+## Format explanation
 
-[Apache 2.0](LICENSE)
 
 
+## License
+
+[Apache 2.0](LICENSE)
```

### Comparing `yarrowformat-1.1.2/src/yarrow/cli/check.py` & `yarrowformat-1.2.0/src/yarrow/cli/check.py`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.1.2/src/yarrow/cli/save.py` & `yarrowformat-1.2.0/src/yarrow/cli/save.py`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.1.2/src/yarrow/cli/open.py` & `yarrowformat-1.2.0/src/yarrow/cli/open.py`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.1.2/src/yarrow/yarrow_cls.py` & `yarrowformat-1.2.0/src/yarrow/yarrow_cls.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Yarrow classes, enable the schema to be used more efficiently at runtime.
 
 Contains all the non-pydantic class definitions
 
-    To pydantic conversion:
-    
-    img = Image(...)
+Each class has a pydantic conversion:
+
+>>> img = Image(...)
     img_pydantic = img.pydantic() # you have a Image_pydantic instance
-    
     img_as_dict = img_pydantic.dict() # now you have a dict
+
 """
+from copy import copy
 from datetime import datetime
 from warnings import warn
 
 from pydantic import StrBytes
 
 from .yarrow import *
 
@@ -26,14 +27,15 @@
         date_captured: datetime,
         id: str = None,
         azure_url: str = None,
         confidential: Clearance = None,
         meta: dict = None,
         comment: str = None,
         asset_id: str = None,
+        split: str = None,
         **kwargs
     ) -> None:
         """Image object, not a pydantic class, represents the image informations
 
         Args:
             width (int): image width in pixel
             height (int): image height in pixel
@@ -41,26 +43,28 @@
             date_captured (datetime): date of acquisition
             id (str, optional): pydantic identifier
             azure_url (str, optional): complete azure url. Defaults to None.
             confidential (Clearance, optional): clearance information, not necessary. Defaults to None.
             meta (dict, optional): optional metadata. Defaults to None.
             comment (str, optional): optional comment. Defaults to None.
             asset_id (str, optional): unique identifier of the asset that created the picture, not used. Defaults to None.
+            split(str, optional): string to specify to which split the image belong, used to assign images to "train", "validate" or "test" when training models for example.
         """
 
         self.id = id or uuid_init()
         self.width = width
         self.height = height
         self.file_name = file_name
         self.date_captured = date_captured
         self.azure_url = azure_url
         self.confidential = confidential
-        self.meta = meta
+        self.meta = meta or {}
         self.comment = comment
         self.asset_id = asset_id
+        self.split = split
 
         self._pydantic_self = None
 
     def pydantic(self, id: str = None, reset: bool = False) -> Image_pydantic:
         """Returns the pydantic object mapping this class. After the first call_
         the object reference is kept. Pass reset=True to reinstantiate the object
 
@@ -113,14 +117,15 @@
         mask: RLE = None,
         area: float = None,
         bbox: List[float] = None,
         keypoints: List[List[Union[int, float]]] = None,
         num_keypoints: int = None,
         weight: float = None,
         date_captured: datetime = None,
+        meta: dict = None,
         **kwargs
     ) -> None:
         """Annotation class, can handle bbox, polygon, mask and keypoint annotation types \
         and a single annotation can be applied to multiple images.
 
         ```python
         images = [Image(...), ...]
@@ -150,14 +155,15 @@
             area (float, optional): relative surface area of the image covered by the annotation. Defaults to None.
             bbox (List[float], optional): bounding box, order[left, top, right, bot]. Defaults to None.
             keypoints (List[List[Union[int, float]]], optional): keypoint annotation, [[x,y,v], ...]; \
                 v=0 not labeled, v=1 labeled not visible, v=2 labeled and visible. Defaults to None.
             num_keypoints (int, optional): number of labelled keypoints. Defaults to None.
             weight (float, optional): weight given to the quality of the annotation. Defaults to None.
             date_captured (datetime, optional): datetime at which the annotation was created. Defaults to None.
+            meta (dict, optional): a free metadata information key. If the Annotation cannot hold your information then put it here
         """
         self.name = name
 
         self.images = images or []
         assert isinstance(self.images, List), "images is not a list"
 
         self.categories = categories or []
@@ -191,28 +197,31 @@
 
         self.area = area
         self.bbox = bbox
         self.keypoints = keypoints
         self.num_keypoints = num_keypoints
         self.weight = weight
         self.date_captured = date_captured
+        self.meta = meta or {}
 
         self._pydantic_self = None
 
     def __hash__(self) -> int:
-        return hash((self.name, *self.images, *self.categories, self.contributor))
+        return hash(
+            (self.name, *set(self.images), *set(self.categories), self.contributor)
+        )
 
     def __eq__(self, other) -> bool:
         if isinstance(other, Annotation):
             return all(
                 (
                     self.name == other.name,
-                    self.images == other.images,
+                    set(self.images) == set(other.images),
                     self.contributor == other.contributor,
-                    self.categories == other.categories,
+                    set(self.categories) == set(other.categories),
                     self.polygon == other.polygon,
                     self.polyline == other.polyline,
                     self.mask == other.mask,
                     self.bbox == other.bbox,
                     self.keypoints == other.keypoints,
                 )
             )
@@ -280,14 +289,15 @@
 class MultilayerImage:
     def __init__(
         self,
         images: List[Image] = None,
         name: str = None,
         meta: dict = None,
         id: str = None,
+        split: str = None,
     ) -> None:
         """MultilayerImage class. Represents a collection of `Image` that should be
         considered as one element.
 
         Here is an example on how to insert it in an Annotation
 
         ```python
@@ -305,41 +315,69 @@
         ```
 
         Args:
             id (str, optional): unique id of the object, will generate a uuid if None. Defaults to uuid4().hex.
             images (List[Image], optional): Defaults to [].
             name (str, optional): Name of the collection. Defaults to "".
             meta (dict, optional): Metadata. Defaults to {}.
+            split(str, optional): string to specify to which split the image belong, used to assign images to "train", "validate" or "test" when training models for example.
         """
         self.id = id or uuid_init()
         self.images = images or []
         self.name = name or ""
         self.meta = meta or {}
+        self.split = split
 
         self._pydantic = None
 
     def __hash__(self):
-        return hash((*self.images, self.name))
+        # return hash((*set(self.images), self.name))
+        return hash((*sorted(self.images, key=lambda x: hash(x)), self.name))
 
     def __eq__(self, other):
         if isinstance(other, MultilayerImage):
-            return all((self.images == other.images, self.name == other.name))
+            return all(
+                (
+                    set(self.images) == set(other.images),
+                    self.name == other.name,
+                )
+            )
         return NotImplemented
 
+    def set_split(self, split: str):
+        """Set the split for the current MultilayerImage and all its Images
+
+        Args:
+            split (str): The split value to assign
+        """
+        self.split = split
+        for img in self.images:
+            img.split = split
+
     def pydantic(self, reset: bool = False):
+        """Returns the pydantic object mapping this class. After the first call_
+        the object reference is kept. Pass reset=True to reinstantiate the object
+
+        Args:
+            reset (bool, optional): Pass True to reinstantiate the object, previous object will be lost. Defaults to False.
+
+        Returns:
+            Image_pydantic: pydantic image class
+        """
         if self._pydantic is None or reset:
             self._pydantic = self._pydantic_call()
         return self._pydantic
 
     def _pydantic_call(self, **kwargs):
         return MultilayerImage_pydantic(
             id=self.id,
             name=self.name,
             image_id=[img.pydantic().id for img in self.images],
             meta=self.meta,
+            split=self.split,
         )
 
 
 class YarrowDataset:
     def __init__(
         self,
         info: Info,
@@ -380,65 +418,51 @@
         self.categories = categories or []
         self.multilayer_images = multilayer_images or []
 
     def __eq__(self, other: "YarrowDataset"):
         if isinstance(other, YarrowDataset):
             return all(
                 (
-                    not len(set(self.images).symmetric_difference(set(other.images))),
-                    not len(
-                        set(self.annotations).symmetric_difference(
-                            set(other.annotations)
-                        )
-                    ),
-                    not len(
-                        set(self.contributors).symmetric_difference(
-                            set(other.contributors)
-                        )
-                    ),
-                    not len(
-                        set(self.confidential).symmetric_difference(
-                            set(other.confidential)
-                        )
-                    ),
-                    not len(
-                        set(self.categories).symmetric_difference(set(other.categories))
-                    ),
-                    not len(
-                        set(self.multilayer_images).symmetric_difference(
-                            set(other.multilayer_images)
-                        )
-                    ),
+                    set(self.images) == set(other.images),
+                    set(self.annotations) == set(other.annotations),
+                    set(self.contributors) == set(other.contributors),
+                    set(self.confidential) == set(other.confidential),
+                    set(self.categories) == set(other.categories),
+                    set(self.multilayer_images) == set(other.multilayer_images),
                 )
             )
         return NotImplemented
 
     def add_annotations(self, annots: List[Annotation]) -> List[Annotation]:
         """DONT NEED TO ADD IMAGE AFTER THIS. Insertion is done in place
 
         Args:
             annots (List[Annotation])
 
         Return:
             (List[Annotation]). Returns the annotation that were added
         """
-        result = []
+        result = set()
         for annot in annots:
-            result.append(self.add_annotation(annot))
-        return result
+            result.add(self.add_annotation(annot))
+        return list(result)
 
     def add_annotation(self, annot: Annotation) -> Annotation:
-        """DONT NEED TO ADD IMAGE AFTER THIS. Insertion is done in place
+        """YOU DO NOT NEED TO ADD IMAGE AFTER THIS. Insertion is done in place
+        If the annotation already exists in the dataset, it will not be added and this function will return the one found
+
+        Be careful, to overwrite metadata you should modify directly the object and not try to overwrite it
 
         Args:
             annot (Annotation)
 
         Return:
             (Annotation)
         """
+        annot = copy(annot)
         annot.images = self.add_images(annot.images)
 
         out_cat = set(annot.categories)
         for cat in annot.categories:
             elem_in = next((elem for elem in self.categories if elem == cat), None)
             if elem_in is None:
                 self.categories.append(cat)
@@ -452,44 +476,49 @@
             (elem for elem in self.contributors if elem == annot.contributor), None
         )
         if elem_in is None:
             self.contributors.append(annot.contributor)
         else:
             annot.contributor = elem_in
 
-        self.annotations.append(annot)
+        elem_in = next((elem for elem in self.annotations if elem == annot), None)
+        if elem_in is None:
+            self.annotations.append(annot)
+        else:
+            return elem_in
         return annot
 
     def add_images(self, images: List[Image]) -> List[Image]:
         """Add an image list and its confidential objects if they exists
         and returns the actual images found in the yarrow in case they
         are already present
 
         Args:
             images (List[Image])
 
         Return:
             (List[Images])
         """
-        result = []
+        result = set()
         for img in images:
-            result.append(self.add_image(img))
+            result.add(self.add_image(img))
 
-        return result
+        return list(result)
 
     def add_image(self, image: Image) -> Image:
         """Add an image and its confidential object if it exists
         Returns the
 
         Args:
             image (Image)
 
         Return:
             (Image)
         """
+        image = copy(image)
         if not image.confidential is None:
             elem_in = next(
                 (elem for elem in self.confidential if elem == image.confidential), None
             )
             if elem_in is None:
                 self.confidential.append(image.confidential)
             else:
@@ -498,26 +527,53 @@
         elem_in = next((elem for elem in self.images if elem == image), None)
         if elem_in is None:
             self.images.append(image)
         else:
             return elem_in
         return image
 
-    def add_multilayer_image(self, multilayer: MultilayerImage):
+    def add_multilayer_image(self, multilayer: MultilayerImage) -> MultilayerImage:
+        """Add a multilayer image object, the returned multilayer object will be
+        the one in the current YarrowDataset and the original will remain unchanged
+
+        Args:
+            multilayer (MultilayerImage): input multilayer image object
+
+        Returns:
+            MultilayerImage: A copy of the original multilayer image object contained in the current YarrowDataset
+        """
+        multilayer = copy(multilayer)
         multilayer.images = self.add_images(multilayer.images)
 
         elem_in = next(
             (elem for elem in self.multilayer_images if elem == multilayer), None
         )
         if elem_in is None:
             self.multilayer_images.append(multilayer)
         else:
             return elem_in
         return multilayer
 
+    def add_multilayer_images(
+        self, multilayer_list: List[MultilayerImage]
+    ) -> List[MultilayerImage]:
+        """Adds a list of multilayer images and returns the actual multilayer images that are present in the dataset.
+        The returned list will contain links to the objects in the current YarrowDataset
+
+        Args:
+            multilayer_list (List[MultilayerImage]): Input MultilayerImage list
+
+        Returns:
+            List[MultilayerImage]: MultilayerImage list with the current dataset objects linked
+        """
+        result = set()
+        for multi in multilayer_list:
+            result.add(self.add_multilayer_image(multi))
+        return list(result)
+
     def pydantic(
         self, img_id: str = None, reset: bool = False
     ) -> YarrowDataset_pydantic:
         """Returns the pydantic YarrowDataset with all elements object links replaced by \
         id links. The returned object can then be used to serialize the dataset using \
         `dict()` and `json()` functions following a pydantic behaviour. See `pydantic` and \
         the `BaseModel` class to understand how it behaves.
@@ -545,14 +601,74 @@
                 multilayer.pydantic(reset=reset)
                 for multilayer in self.multilayer_images
             ]
             if len(self.multilayer_images) > 0
             else None,
         )
 
+    def set_split(self, split: str) -> None:
+        """Assigns the value of `split` to all the images and multilayer images
+
+        Args:
+            split (str): Describes the split, used to set "train"/"validate"/"test" for example
+        """
+        for image in self.images:
+            image.split = split
+        for multilayer in self.multilayer_images:
+            multilayer.split = split
+
+    def get_split(self, split: str) -> "YarrowDataset":
+        """Returns a new dataset based on a `split` value. 
+        
+        The returned YarrowDataset will copy all the internal elements,\
+        meaning modifications on the new YarrowDataset won't impact the original YarrowDataset
+
+        Args:
+            split (str): The split to retrieve
+
+        Returns:
+            YarrowDataset: A copy of the current dataset containing only the elements linked to a given split value
+        """
+        new_yarrow_set = YarrowDataset(info=self.info)
+
+        for annot in self.annotations:
+            # Very strong assumption that all images of the annotation have the same value for split
+            if len(annot.images) > 0 and annot.images[0].split == split:
+                new_yarrow_set.add_annotation(annot)
+
+        for multi in self.multilayer_images:
+            if multi.split == split:
+                new_yarrow_set.add_multilayer_image(multi)
+
+        return new_yarrow_set
+
+    def append(self, yarrow: "YarrowDataset") -> None:
+        """Appends another YarrowDataset to this dataset. The resulting dataset is this object.
+        The objects added will be the annotations, the multilayer_images and the images
+
+        Args:
+            yarrow (YarrowDataset): Input Yarrow to be merge
+        """
+        self.add_annotations(yarrow.annotations)
+        self.add_multilayer_images(yarrow.multilayer_images)
+        self.add_images(yarrow.images)
+
+        for cat in yarrow.categories:
+            if cat not in self.categories:
+                self.categories.append(cat)
+
+    def extend(self, yarrows: List["YarrowDataset"]) -> None:
+        """Extends a YarrowDataset with a list of YarrowDatasets
+
+        Args:
+            yarrows (List[YarrowDataset]): List of YarrowDatasets, they will remain unchanged
+        """
+        for yarrow in yarrows:
+            self.append(yarrow)
+
     @classmethod
     def from_yarrow(cls, yarrow: YarrowDataset_pydantic) -> "YarrowDataset":
         """Constructor to transform a `YarrowDataset_pydantic` and replace all id links \
         with direct object references. Be careful when using directly, it is better \
         to use `parse_*()` functions and not this one directly.
 
         Args:
```

### Comparing `yarrowformat-1.1.2/src/yarrow/utils.py` & `yarrowformat-1.2.0/src/yarrow/utils.py`

 * *Files identical despite different names*

