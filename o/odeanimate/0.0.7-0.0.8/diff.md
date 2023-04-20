# Comparing `tmp/odeanimate-0.0.7.tar.gz` & `tmp/odeanimate-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odeanimate-0.0.7.tar", last modified: Mon Apr  3 04:29:05 2023, max compression
+gzip compressed data, was "odeanimate-0.0.8.tar", last modified: Thu Apr 20 15:40:10 2023, max compression
```

## Comparing `odeanimate-0.0.7.tar` & `odeanimate-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-03 04:29:05.312871 odeanimate-0.0.7/
--rw-r--r--   0 miguel.salgado   (501) staff       (20)    18092 2022-10-25 16:21:52.000000 odeanimate-0.0.7/LICENSE.txt
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     3101 2023-04-03 04:29:05.312749 odeanimate-0.0.7/PKG-INFO
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     2298 2022-10-25 16:21:52.000000 odeanimate-0.0.7/README.md
-drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-03 04:29:05.311218 odeanimate-0.0.7/odeanimate/
--rw-r--r--   0 miguel.salgado   (501) staff       (20)      495 2023-04-03 04:27:09.000000 odeanimate-0.0.7/odeanimate/__init__.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)    12151 2023-04-03 04:28:40.000000 odeanimate-0.0.7/odeanimate/array.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     2336 2022-10-25 16:21:52.000000 odeanimate-0.0.7/odeanimate/codomain.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)      241 2022-10-25 16:21:52.000000 odeanimate-0.0.7/odeanimate/constants.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)    11326 2022-10-25 16:21:52.000000 odeanimate-0.0.7/odeanimate/curve.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     9028 2022-10-25 16:21:52.000000 odeanimate-0.0.7/odeanimate/domains.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     2308 2023-03-31 05:23:44.000000 odeanimate-0.0.7/odeanimate/fields.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)      233 2022-10-25 16:21:52.000000 odeanimate-0.0.7/odeanimate/jupyter.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     7152 2022-10-25 16:21:52.000000 odeanimate-0.0.7/odeanimate/matrix.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     4407 2022-10-25 16:21:52.000000 odeanimate-0.0.7/odeanimate/meta.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     3807 2023-03-14 04:53:39.000000 odeanimate-0.0.7/odeanimate/utils.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)    22306 2023-04-03 02:39:39.000000 odeanimate-0.0.7/odeanimate/vector.py
-drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-03 04:29:05.311909 odeanimate-0.0.7/odeanimate.egg-info/
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     3101 2023-04-03 04:29:05.000000 odeanimate-0.0.7/odeanimate.egg-info/PKG-INFO
--rw-r--r--   0 miguel.salgado   (501) staff       (20)      586 2023-04-03 04:29:05.000000 odeanimate-0.0.7/odeanimate.egg-info/SOURCES.txt
--rw-r--r--   0 miguel.salgado   (501) staff       (20)        1 2023-04-03 04:29:05.000000 odeanimate-0.0.7/odeanimate.egg-info/dependency_links.txt
--rw-r--r--   0 miguel.salgado   (501) staff       (20)       11 2023-04-03 04:29:05.000000 odeanimate-0.0.7/odeanimate.egg-info/requires.txt
--rw-r--r--   0 miguel.salgado   (501) staff       (20)       11 2023-04-03 04:29:05.000000 odeanimate-0.0.7/odeanimate.egg-info/top_level.txt
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     1289 2023-04-03 04:26:33.000000 odeanimate-0.0.7/pyproject.toml
--rw-r--r--   0 miguel.salgado   (501) staff       (20)       38 2023-04-03 04:29:05.312909 odeanimate-0.0.7/setup.cfg
-drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-03 04:29:05.312574 odeanimate-0.0.7/tests/
--rw-r--r--   0 miguel.salgado   (501) staff       (20)      571 2022-10-25 16:21:52.000000 odeanimate-0.0.7/tests/test_curves.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     1088 2023-03-31 05:23:44.000000 odeanimate-0.0.7/tests/test_trayectory.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     4236 2023-04-03 02:40:41.000000 odeanimate-0.0.7/tests/test_vector.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)      132 2023-03-31 05:23:44.000000 odeanimate-0.0.7/tests/test_vector_2d.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     1533 2022-10-25 16:21:52.000000 odeanimate-0.0.7/tests/test_vector_from_methods.py
+drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-20 15:40:10.163226 odeanimate-0.0.8/
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)    18092 2022-10-25 16:21:52.000000 odeanimate-0.0.8/LICENSE.txt
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     2714 2023-04-20 15:40:10.163066 odeanimate-0.0.8/PKG-INFO
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     1911 2023-04-03 04:36:58.000000 odeanimate-0.0.8/README.md
+drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-20 15:40:10.161141 odeanimate-0.0.8/odeanimate/
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)      495 2023-04-20 15:39:41.000000 odeanimate-0.0.8/odeanimate/__init__.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)    12849 2023-04-20 15:39:20.000000 odeanimate-0.0.8/odeanimate/array.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     1846 2023-04-20 15:38:12.000000 odeanimate-0.0.8/odeanimate/codomain.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)      241 2022-10-25 16:21:52.000000 odeanimate-0.0.8/odeanimate/constants.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)    11541 2023-04-04 04:17:56.000000 odeanimate-0.0.8/odeanimate/curve.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     9028 2022-10-25 16:21:52.000000 odeanimate-0.0.8/odeanimate/domains.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     2308 2023-03-31 05:23:44.000000 odeanimate-0.0.8/odeanimate/fields.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)      233 2022-10-25 16:21:52.000000 odeanimate-0.0.8/odeanimate/jupyter.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     7255 2023-04-03 05:27:47.000000 odeanimate-0.0.8/odeanimate/matrix.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     4407 2022-10-25 16:21:52.000000 odeanimate-0.0.8/odeanimate/meta.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     3807 2023-03-14 04:53:39.000000 odeanimate-0.0.8/odeanimate/utils.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)    22340 2023-04-20 14:21:44.000000 odeanimate-0.0.8/odeanimate/vector.py
+drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-20 15:40:10.161988 odeanimate-0.0.8/odeanimate.egg-info/
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     2714 2023-04-20 15:40:10.000000 odeanimate-0.0.8/odeanimate.egg-info/PKG-INFO
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)      586 2023-04-20 15:40:10.000000 odeanimate-0.0.8/odeanimate.egg-info/SOURCES.txt
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)        1 2023-04-20 15:40:10.000000 odeanimate-0.0.8/odeanimate.egg-info/dependency_links.txt
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)       11 2023-04-20 15:40:10.000000 odeanimate-0.0.8/odeanimate.egg-info/requires.txt
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)       11 2023-04-20 15:40:10.000000 odeanimate-0.0.8/odeanimate.egg-info/top_level.txt
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     1347 2023-04-20 14:18:41.000000 odeanimate-0.0.8/pyproject.toml
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)       38 2023-04-20 15:40:10.163278 odeanimate-0.0.8/setup.cfg
+drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-20 15:40:10.162838 odeanimate-0.0.8/tests/
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)      571 2022-10-25 16:21:52.000000 odeanimate-0.0.8/tests/test_curves.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     1146 2023-04-20 15:31:20.000000 odeanimate-0.0.8/tests/test_trayectory.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     4236 2023-04-03 02:40:41.000000 odeanimate-0.0.8/tests/test_vector.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)      132 2023-03-31 05:23:44.000000 odeanimate-0.0.8/tests/test_vector_2d.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     1533 2022-10-25 16:21:52.000000 odeanimate-0.0.8/tests/test_vector_from_methods.py
```

### Comparing `odeanimate-0.0.7/LICENSE.txt` & `odeanimate-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.7/PKG-INFO` & `odeanimate-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: odeanimate
-Version: 0.0.7
-Summary: A module for useful quick mathematical calculation, plotting and animation.
-Author-email: Miguel Alejandro Salgado Zapien <ekiim@ekiim.xyz>
-License: GPL-2.0
-Project-URL: Homepage, https://odeanimate.ekiim.xyz
-Project-URL: Source, https://github.com/ekiim/odeanimate
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # ODE Animate
 
 [![PyPI version](https://badge.fury.io/py/odeanimate.svg)](https://pypi.org/project/odeanimate/)
 
 This project aims to be a set of tools for solving, plotting, and animating curves and fields.
 
 > The rational for this is, _trying to use pure-python_ to do numerical analysis.
@@ -34,36 +15,38 @@
 
 
 ## Features
 
 > Most of this features are _W.I.P._ (work in progress)
 
  - [x] Vector objects with _basic_ operations.
+ - [x] Vector objects with _basic_ operations.
  - [x] Function utilities for _real valued_ functions.
  - [x] Automatic plotting for _real valued_ functions.
  - [ ] Generic _ODE_ integrators.
- - [ ] Utilities for curves.
+ - [X] Utilities for curves.
  - [ ] Utilities for surfaces.
  - [ ] Animation Loop and widgets
 
 ## Development
 
-> Initially this project was developed with [`pipenv`](https://pipenv.pypa.io/en/latest/), but for publishing pourpuses
-> I decided to change to [Poetry](https://python-poetry.org/).
+> This project uses [`pipenv`](https://pipenv.pypa.io/) for local development and testing.
+
+If you are intending to:
+
+- Add examples or documentation,
+- develop further this module
+- use and test in an isolated enviroment
+
+you should have `pipenv` installed.
+
+One you cloned the repository, you should be able to execute `pipenv install --dev` and everything should be working.
 
-In order to install the project for development (meaning you are intending to work with it to extend it's capabilities, or improve it's documentation),
-you should make sure you have poetry installed in your machine (check the link above), and simply execute `poetry install`, 
-and after you can start running python commands with it as
-
- - `poetry run python` will run `python` with the configuration required to use this project.
- - `poetry run jupyter lab` should run you a jupyter instance to work on top of the project.
- - `poetry run ./scripts/lint.sh` should run the code linter.
- - `poetry run ./scripts/format.sh`, to format the code.
- - `poetry run ./scripts/tests.sh` should run the test suit, and report back any fails.
- - `poetry run ./scripts/docs.sh` to build the documentation html site.
+Most of what you would need is configured in the `pyproject.toml` file, so if you are using the tools specified in
+the `scripts` section of the `Pipfile` you should be fine.
 
 ## Contribute
 
 If you wish to contribute you can contact me directly, or open an issue in the github repository.
 The main development for this module is done in a private repository, but for visibility and public
 interaction I'll host this in github too.
```

### Comparing `odeanimate-0.0.7/README.md` & `odeanimate-0.0.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: odeanimate
+Version: 0.0.8
+Summary: A module for useful quick mathematical calculation, plotting and animation.
+Author-email: Miguel Alejandro Salgado Zapien <ekiim@ekiim.xyz>
+License: GPL-2.0
+Project-URL: Homepage, https://odeanimate.ekiim.xyz
+Project-URL: Source, https://github.com/ekiim/odeanimate
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # ODE Animate
 
 [![PyPI version](https://badge.fury.io/py/odeanimate.svg)](https://pypi.org/project/odeanimate/)
 
 This project aims to be a set of tools for solving, plotting, and animating curves and fields.
 
 > The rational for this is, _trying to use pure-python_ to do numerical analysis.
@@ -15,36 +34,38 @@
 
 
 ## Features
 
 > Most of this features are _W.I.P._ (work in progress)
 
  - [x] Vector objects with _basic_ operations.
+ - [x] Vector objects with _basic_ operations.
  - [x] Function utilities for _real valued_ functions.
  - [x] Automatic plotting for _real valued_ functions.
  - [ ] Generic _ODE_ integrators.
- - [ ] Utilities for curves.
+ - [X] Utilities for curves.
  - [ ] Utilities for surfaces.
  - [ ] Animation Loop and widgets
 
 ## Development
 
-> Initially this project was developed with [`pipenv`](https://pipenv.pypa.io/en/latest/), but for publishing pourpuses
-> I decided to change to [Poetry](https://python-poetry.org/).
+> This project uses [`pipenv`](https://pipenv.pypa.io/) for local development and testing.
+
+If you are intending to:
+
+- Add examples or documentation,
+- develop further this module
+- use and test in an isolated enviroment
+
+you should have `pipenv` installed.
+
+One you cloned the repository, you should be able to execute `pipenv install --dev` and everything should be working.
 
-In order to install the project for development (meaning you are intending to work with it to extend it's capabilities, or improve it's documentation),
-you should make sure you have poetry installed in your machine (check the link above), and simply execute `poetry install`, 
-and after you can start running python commands with it as
-
- - `poetry run python` will run `python` with the configuration required to use this project.
- - `poetry run jupyter lab` should run you a jupyter instance to work on top of the project.
- - `poetry run ./scripts/lint.sh` should run the code linter.
- - `poetry run ./scripts/format.sh`, to format the code.
- - `poetry run ./scripts/tests.sh` should run the test suit, and report back any fails.
- - `poetry run ./scripts/docs.sh` to build the documentation html site.
+Most of what you would need is configured in the `pyproject.toml` file, so if you are using the tools specified in
+the `scripts` section of the `Pipfile` you should be fine.
 
 ## Contribute
 
 If you wish to contribute you can contact me directly, or open an issue in the github repository.
 The main development for this module is done in a private repository, but for visibility and public
 interaction I'll host this in github too.
```

### Comparing `odeanimate-0.0.7/odeanimate/array.py` & `odeanimate-0.0.8/odeanimate/array.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,45 +3,61 @@
 from functools import reduce
 
 
 from odeanimate.utils import RealNumber, mul
 
 
 class _ArrayHTMLDisplay:
+    _html_styles_table = (
+        'style="margin: 1em; table-layout: fixed; max-width: 100%;"'
+    )
     _html_styles_cell = 'style="border:1px solid black; text-align: center"'
     _html_styles_header = 'style="text-align: center"'
     _html_axis = False
 
+    def _html_format_element(self, element):
+        return str(element)
+
     def _repr_html_row_from_index(self, start, length):
         a = self._array
         styles = self._html_styles_cell
         returnable = (
             "<tr>",
-            *[f"<td {styles}>{a[i]}</td>" for i in range(start, length + start)],
+            *[
+                f"<td {styles}>{self._html_format_element(a[i])}</td>"
+                for i in range(start, length + start)
+            ],
             "</tr>",
         )
         return returnable
 
+    def _get_column_name(self, index):
+        return index
+
     def _html_table_header_row_for_columns(self, cols, one_dimensional=False):
         styles = self._html_styles_header
         returnable = (
             "<tr>",
-            *[f"<th {styles}>{i}</th>" for i in range(cols)],
+            "" if one_dimensional else "<th></th>",
+            *[
+                f"<th {styles}>{self._get_column_name(i)}</th>"
+                for i in range(cols)
+            ],
             "</tr>",
         )
-        if not one_dimensional:
-            returnable = (returnable[0], f"<th></th>", *returnable[1:])
         return returnable
 
     def _repr_html_(self):
         returnable = []
         if len(self._shape) == 1:
             cols = self._shape[0]
             if self._html_axis:
-                returnable.extend(self._html_table_header_row_for_columns(cols, True))
+                returnable.extend(
+                    self._html_table_header_row_for_columns(cols, True)
+                )
             returnable.extend(self._repr_html_row_from_index(0, cols))
 
         if len(self._shape) == 2:
             rows, cols = self._shape
             if self._html_axis:
                 returnable.extend(self._html_table_header_row_for_columns(cols))
             for row in range(rows):
@@ -49,48 +65,54 @@
                 if self._html_axis:
                     extendable = (
                         extendable[0],
                         f"<th {self._html_styles_header}>{row}</th>",
                         *extendable[1:],
                     )
                 returnable.extend(extendable)
-
         return "".join(
             (
-                "<table style='margin: 1rem;'>",
+                f"<table {self._html_styles_table}>",
                 *returnable,
                 "</table>",
             )
         )
 
 
 class Array(_ArrayHTMLDisplay):
     _type = RealNumber
 
     def __init__(self, *args, shape=None, flat_input=False, **kwargs):
         self._shape = (
             self._input_shape_extractor(args) if shape is None else tuple(shape)
         )
-        if not flat_input and not self._input_shape_consistent(args, self._shape):
+        if not flat_input and not self._input_shape_consistent(
+            args, self._shape
+        ):
             raise Exception("Inconsistent shape of input structure")
 
         if flat_input:
             self._array = args[0]
         else:
             self._array = tuple(self._flatten_structure(args, self._shape))
 
-        if any((not self.__class__._type.is_compatible(i) for i in self._array)):
+        if any(
+            (not self.__class__._type.is_compatible(i) for i in self._array)
+        ):
             del self._array
             raise Exception("Invalid types on values of input structure.")
 
         if len(self._array) != mul(self._shape):
             raise Exception("Inconsistency in shape and array element count.")
 
+    def _repr_data(self):
+        return f"shape={self._shape}"
+
     def __repr__(self):
-        return f"<Array shape={self._shape}>"
+        return f"<{self.__class__.__name__} {self._repr_data()}>"
 
     @classmethod
     def _key_element_to_range(cls, element, limit):
         if isinstance(element, slice):
             start = element.start
             stop = element.stop
             step = element.step or 1
@@ -153,43 +175,48 @@
         if not hasattr(keys, "__len__"):
             keys = (keys,)
         if len(keys) != len(self._shape):
             raise Exception("Insufficient values in descriptor.")
 
         only_numbers_or_slices = all(
             map(
-                lambda _slice: isinstance(_slice, int) or isinstance(_slice, slice),
+                lambda _slice: isinstance(_slice, int)
+                or isinstance(_slice, slice),
                 keys,
             )
         )
         if not only_numbers_or_slices:
-            raise KeyError("Invalid access descriptor, only admit int or slice.")
+            raise KeyError(
+                "Invalid access descriptor, only admit int or slice."
+            )
 
         only_numbers = all(map(lambda _slice: isinstance(_slice, int), keys))
 
         if only_numbers:
-            index = self.__class__._get_flat_index(self._shape, keys)
+            index = Array._get_flat_index(self._shape, keys)
             return self._array[index]
 
         sliced_keys = [
             self.__class__._key_element_to_range(element, limit - 1)
             for (element, limit) in zip(keys, self._shape)
         ]
         _sub_array_indexes = list(
             map(
                 lambda key: self.__class__._get_flat_index(self._shape, key),
                 product(*sliced_keys),
             )
         )
         _sub_array_shape = tuple(
-            len(r) for i, r in enumerate(sliced_keys) if not isinstance(keys[i], int)
+            len(r)
+            for i, r in enumerate(sliced_keys)
+            if not isinstance(keys[i], int)
         )
         _sub_array = [self._array[i] for i in _sub_array_indexes]
 
-        return self.__class__(
+        return Array(
             _sub_array,
             shape=_sub_array_shape,
             flat_input=True,
         )
 
     @property
     def shape(self):
@@ -254,15 +281,17 @@
         (2, 3)
         >>> Array._input_shape_extractor((range(1, 4), range(4, 7), range(7, 10)))
         (3, 3)
         """
         length = cls._has_len_or_none(args)
         if length:
             nested_result = tuple(
-                filter(lambda x: x is not None, cls._input_shape_extractor(args[0]))
+                filter(
+                    lambda x: x is not None, cls._input_shape_extractor(args[0])
+                )
             )
         else:
             nested_result = []
         return (length, *nested_result)
 
     @classmethod
     def _input_shape_consistent(cls, args, shape=None):
@@ -298,15 +327,17 @@
 
         """
         if shape is None:
             shape = cls._input_shape_extractor(args)
         if len(shape) == 1:
             return cls._has_len_or_none(args) == shape[0]
         else:
-            return all((cls._input_shape_consistent(arg, shape[1:]) for arg in args))
+            return all(
+                (cls._input_shape_consistent(arg, shape[1:]) for arg in args)
+            )
         return False
 
     @classmethod
     def _flatten_structure(cls, args, shape=None):
         """
         >>> tuple(Array._flatten_structure((range(3), range(3, 6))))
         (0, 1, 2, 3, 4, 5)
@@ -336,21 +367,25 @@
                 shape=self.shape,
                 flat_input=True,
             )
 
     def __mul__(self, other):
         if self.__class__._type.is_compatible(other):
             return self.__class__(
-                [a * other for a in self._array], shape=self.shape, flat_input=True
+                [a * other for a in self._array],
+                shape=self.shape,
+                flat_input=True,
             )
 
     def __truediv__(self, other):
         if self.__class__._type.is_compatible(other):
             return self.__class__(
-                [a / other for a in self._array], shape=self.shape, flat_input=True
+                [a / other for a in self._array],
+                shape=self.shape,
+                flat_input=True,
             )
 
     def __eq__(self, other):
         """
         >>> B = Array(range(3), range(3, 6), range(6, 9))
         >>> B[2, :] == Array(6, 7, 8)
         True
@@ -380,15 +415,17 @@
 
         def _iterator():
             yield from self._array
 
         return _iterator()
 
     def __hash__(self):
-        """
+        """Hash method:
+
         >>> A = Array(1, 2, 3)
         >>> A.__class__.__name__
         'Array'
         >>> hash(A) == hash(("Array", (3,), 1, 2, 3))
         True
+
         """
         return hash((self.__class__.__name__, self.shape, *self._array))
```

### Comparing `odeanimate-0.0.7/odeanimate/codomain.py` & `odeanimate-0.0.8/odeanimate/codomain.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,57 @@
+from odeanimate.array import Array, _ArrayHTMLDisplay
 from odeanimate.vector import Vector
 
 
-class Trajectory:
-    def __init__(self, *args, keys=None, **kwargs):
-        if any((not Vector.is_compatible(v) for v in args)):
-            raise Exception("Incompatible Object")
-        rows = tuple(Vector.from_compatible(v) for v in args)
-        if len(set(len(v) for v in rows)) != 1:
-            raise Exception("Inconsistent row found")
-        self._rows = rows
-        self._shape = (len(rows), len(rows[0]))
-        self.set_keys(keys)
-
-    def set_keys(self, keys=None):
-        if keys is None:
-            keys = [f"col_{i}" for i in range(1, self._shape[1] + 1)]
-
-        if any((not isinstance(k, str) for k in keys)):
-            raise Exception("Keys are not strings")
-        self._keys = tuple(keys)
-
-    def get_column_by_key(self, *keys):
-        if len(keys) == 1:
-            key = keys[0]
-        if key in self._keys:
-            index = self._keys.index(key)
-            return Vector(*[v[index] for v in self._rows])
-        raise Exception("Multiple keys not supported yet")
-
-    def __getitem__(self, key):
-        return self.__getattr__(key)
+class Trajectory(Array, _ArrayHTMLDisplay):
+    _html_styles_cell = ""
+    _html_axis = True
+
+    def _get_column_name(self, index):
+        returnable = f"col_{index}"
+        if self._keys:
+            returnable = self._keys[index]
+        return returnable
 
-    def __repr__(self):
-        rows, cols = self._shape
-        return f"<Trajectory rows={rows} cols={cols} keys={self._keys}>"
+    def __init__(self, *args, keys=None, **kwargs):
+        if hasattr(args[0][-1], "__iter__"):
+            args_super = [(*arg[:-1], *arg[-1]) for arg in args]
+        else:
+            args_super = args
+        super().__init__(*args_super, **kwargs)
+        if False and len(self._shape) != 2:
+            raise Exception("Incompatible structure for trajectory.")
+        if (
+            keys is not None
+            and hasattr(keys, "__len__")
+            and len(keys) == self._shape[1]
+        ):
+            self._keys = tuple(keys)
+        else:
+            self._keys = None
+
+    def __getitem__(self, keys):
+        if keys in (self._keys or []):
+            column = self._keys.index(keys)
+            return super().__getitem__((slice(None, None, None), column))
+        super().__getitem__(keys)
 
     def __getattr__(self, name):
-        return self.get_column_by_key(name)
-        raise Exception("Attribute doesn't exist in keys")
-
-    def _repr_html_(self):
-        keys = self._keys
-        return "".join(
-            [
-                "<table>",
-                "<thead>",
-                "<tr>",
-                *[f"<th>${k}$</th>" for k in keys],
-                "</tr>",
-                "</thead>",
-                "<tbody>",
-                *[
-                    "".join(["<tr>", *[f"<td>{str(x)}</td>" for x in row], "</tr>"])
-                    for row in self._rows
-                ],
-                "</tbody>",
-                "</table>",
-            ]
-        )
-
-    def _ipython_display_(self):
-        return self._repr_html_()
+        if name in (self._keys or []):
+            column = self._keys.index(name)
+            return super().__getitem__((slice(None, None, None), column))
+        raise AttributeError
 
     def _plot_2d(self, ax, keys=["x", "y"], **kwargs):
         x = getattr(self, keys[0])
         y = getattr(self, keys[1])
         ax.plot(x, y)
 
     def _plot_3d(self, ax, keys=["x", "y", "z"], **kwargs):
         x = getattr(self, keys[0])
         y = getattr(self, keys[1])
         z = getattr(self, keys[2])
         ax.plot(x, y, z)
+
+    def _repr_data(self):
+        rows, cols = self._shape
+        return f"rows={rows} cols={cols} keys={self._keys}"
```

### Comparing `odeanimate-0.0.7/odeanimate/curve.py` & `odeanimate-0.0.8/odeanimate/curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,16 @@
 
     def map(self, interval, h=0.1, keys=None):
         if not isinstance(interval, Interval):
             raise Exception("Must evaluate at an interval")
         if h <= 0:
             raise Exception("Delta should be greater than 0.")
         return Trajectory(
-            *[Vector(t, *self(t)) for t in interval(h)], keys=(keys or self._keys)
+            *[(t, *self(t)) for t in interval(h)],
+            keys=(keys or self._keys),
         )
 
     def derivative(self, h=_h):
         def _derivative(t):
             return (self(t + h) - self(t - h)) / (2 * h)
 
         return self.__class__(codomain=self.codomain, function=_derivative)
@@ -192,22 +193,24 @@
     def evolute(self):
         return self + self.normal() / self.curvature()
 
     def _repr_latex_(self):
         return self.__doc__
 
     def _plot_2d(self, ax, interval=None, delta=None, **kwargs):
-        mpl_kwargs = {}
+        mpl_kwargs, map_kwargs = {}, {}
         if "color" in kwargs:
             mpl_kwargs["color"] = kwargs["color"]
         if "line" in kwargs:
             mpl_kwargs["marker"] = kwargs["marker"]
+        if "keys" in kwargs:
+            map_kwargs["keys"] = kwargs["keys"]
         if not isinstance(interval, Interval):
             raise Exception("Missing interval for plot")
-        trajectory = self.map(interval, delta)
+        trajectory = self.map(interval, delta, **map_kwargs)
         ax.plot(trajectory.x, trajectory.y, **mpl_kwargs)
 
 
 class Curve1D(Curve):
     codomain = RealNumber
     _keys = ("x", "y")
 
@@ -215,15 +218,17 @@
         _integrator = cache(integrator)
         if a <= b:
             interval = Interval(a, b)
             factor = 1
         else:
             interval = Interval(b, a)
             factor = -1
-        return factor * sum(map(lambda t: _integrator(self, t, t + h), interval(h)))
+        return factor * sum(
+            map(lambda t: _integrator(self, t, t + h), interval(h))
+        )
 
     def __add__(self, other):
         """
         Examples:
             >>> (Curve1D(lambda x: x**2) + Curve1D(lambda x: -x))(1)
             0
             >>> (Curve1D(lambda x: x**2) + 1)(1)
@@ -285,23 +290,29 @@
                 return self(*args, **kwargs) ** other(*args, **kwargs)
 
         elif RealNumber.is_compatible(other):
 
             def _new_func(*args, **kwargs):
                 return self(*args, **kwargs) ** other
 
-        return cls(function=_new_fuc)
+        else:
+            raise Exception(
+                f"Incompatible operation between {self.__class__} and {other.__class__}"
+            )
+
+        return cls(function=_new_func)
 
     def map(self, interval, h=0.1, keys=None):
         if not isinstance(interval, Interval):
             raise Exception("Must evaluate at an interval")
         if h <= 0:
             raise Exception("Delta should be greater than 0.")
         return Trajectory(
-            *[Vector2D(t, self(t)) for t in interval(h)], keys=(keys or self._keys)
+            *[Vector2D(t, self(t)) for t in interval(h)],
+            keys=(keys or self._keys),
         )
 
 
 class Curve2D(Curve):
     """
     Examples:
 
@@ -330,15 +341,15 @@
 
     def normal(self):
         return self.tangent().J
 
     def curvature(self):
         d = self.derivative()
         dd = d.derivative()
-        return abs(d * dd.J) / abs(d) ** 3
+        return abs(d * dd.J) / (abs(d) ** 3)
 
     def _plot_2d(self, ax, interval=None, delta=None, **kwargs):
         mpl_kwargs = {}
         if "color" in kwargs:
             mpl_kwargs["color"] = kwargs["color"]
         if "line" in kwargs:
             mpl_kwargs["marker"] = kwargs["marker"]
@@ -390,13 +401,7 @@
             mpl_kwargs["color"] = kwargs["color"]
         if "line" in kwargs:
             mpl_kwargs["marker"] = kwargs["marker"]
         if not isinstance(interval, Interval):
             raise Exception("Missing interval for plot")
         trajectory = self.map(interval, delta, keys=["t", "x", "y", "z"])
         ax.plot(trajectory.x, trajectory.y, trajectory.z, **mpl_kwargs)
-
-
-if __name__ == "__main__":
-    import doctest
-
-    doctest.testmod(verbose=False)
```

### Comparing `odeanimate-0.0.7/odeanimate/domains.py` & `odeanimate-0.0.8/odeanimate/domains.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.7/odeanimate/fields.py` & `odeanimate-0.0.8/odeanimate/fields.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.7/odeanimate/matrix.py` & `odeanimate-0.0.8/odeanimate/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from math import sin, cos
 from numbers import Number
 from odeanimate.utils import slice_to_range, tolerance
+from odeanimate.array import Array
 from odeanimate.vector import Vector
 
 
-class Matrix:
+class Matrix(Array):
     def __init__(self, *rows, shape=None, **kwargs):  # pylint: disable=W0613
         rows_count = len(rows)
         column_count = len(rows[0])
         if shape is None:
             if any(filter(lambda row: len(row) != column_count, rows)):
                 raise Exception("Inconsistent columns")
             self._shape = (rows_count, column_count)
@@ -129,23 +130,26 @@
         Vector(2, 2)
         >>> Matrix([1, 0], [0, 1]) * 2
         <Matrix shape=(2, 2) rows=(Vector(2, 0), Vector(0, 2))>
         """
         if isinstance(other, Matrix) and self.shape[1] == other.shape[0]:
             new_shape = self.shape[0], other.shape[1]
             return Matrix(
-                [a.dot(b) for a in self.rows for b in other.columns], shape=new_shape
+                [a.dot(b) for a in self.rows for b in other.columns],
+                shape=new_shape,
             )
         if isinstance(other, Vector) and self.shape[1] == other.dimension:
             return Vector(
                 *[other.dot(a) for a in self.rows],
             )
         if isinstance(other, Number):
             return Matrix([x * other for x in self.array], shape=self.shape)
-        raise Exception(f"Unsoported Operation betwee Matrix and {other.__class__}")
+        raise Exception(
+            f"Unsoported Operation betwee Matrix and {other.__class__}"
+        )
 
     def __rmul__(self, other):
         """
         >>> 2*Matrix([1, 0], [0, 1])
         <Matrix shape=(2, 2) rows=(Vector(2, 0), Vector(0, 2))>
         """
         if isinstance(other, Number):
@@ -157,15 +161,17 @@
 
     def _cell_position_to_array_pos(self, row, col):
         return row * self.shape[1] + col
 
     def _descriptor_to_cell_positions(self, row, col):
         rows = slice_to_range(row) if isinstance(row, slice) else [row]
         cols = slice_to_range(col) if isinstance(col, slice) else [col]
-        return [self._cell_position_to_array_pos(i, j) for i in rows for j in cols]
+        return [
+            self._cell_position_to_array_pos(i, j) for i in rows for j in cols
+        ]
 
     def __eq__(self, other):
         """
         >>> Matrix([1]) == Matrix([1 + 1e-1000000])
         True
         >>> Matrix([1, 2]) == Matrix([1, 2])
         True
```

### Comparing `odeanimate-0.0.7/odeanimate/meta.py` & `odeanimate-0.0.8/odeanimate/meta.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.7/odeanimate/utils.py` & `odeanimate-0.0.8/odeanimate/utils.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.7/odeanimate/vector.py` & `odeanimate-0.0.8/odeanimate/vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,17 @@
             Traceback (most recent call last):
               ...
             Exception: Invalid types on values of input structure.
         """
         super().__init__(*args, **kwargs)
         self.origin = kwargs.get("origin", None)
         self.dimension = self.shape[0]
-        if self.origin is not None and not isinstance(self.origin, (self.__class__)):
+        if self.origin is not None and not isinstance(
+            self.origin, (self.__class__)
+        ):
             raise TypeError("Unsupported origin for the vector")
 
     def __len__(self):
         """
         Asking for the length of a vector, will provide you with the dimension.
 
         > Listening to this, might seem odd, but having `abs` to define the actual
@@ -94,15 +96,17 @@
 
             >>> Vector(1, 2).validation_dimension(Vector(1, 2, 3))
             Traceback (most recent call last):
               ...
             Exception: Object Vector(1, 2) and Vector(1, 2, 3) not compatible dimensions
         """
         if self.dimension != other.dimension:
-            raise Exception(f"Object {self} and {other} not compatible dimensions")
+            raise Exception(
+                f"Object {self} and {other} not compatible dimensions"
+            )
 
     def validation_type(self, other):
         """
         This is a helper method, used internally to validate prior making an
         operation between two objects requiring the same type.
 
         > Possible hide this by adding an underscore to the function.
@@ -448,15 +452,17 @@
             return cls(*object)
         except:
             pass
         try:
             return cls(object)
         except:
             pass
-        raise Exception(f"Object {object} not compatible with {cls.__name__} class")
+        raise Exception(
+            f"Object {object} not compatible with {cls.__name__} class"
+        )
 
 
 """
 ## Particular cases
 
 The most common vectors, are two and three dimensions (maybe for when doing
 relativity).
@@ -579,15 +585,17 @@
             >>> Vector2D.from_complex(1 + 1j)
             Vector2D(1.0, 1.0)
         """
         return cls.from_compatible(z.real, z.imag)
 
     @classmethod
     def is_compatible(cls, *value):
-        if len(value) == 2 and all([RealNumber.is_compatible(x) for x in value]):
+        if len(value) == 2 and all(
+            [RealNumber.is_compatible(x) for x in value]
+        ):
             return True
         return NotImplemented
 
     def _plot_2d(self, ax, point=False, origin=None, **kwargs):
         """
         This method is exclusively for use from the plotting mechanism, inside of the module.
         """
@@ -679,15 +687,17 @@
         if isinstance(vector, cls):
             return vector
         elif isinstance(vector, Vector) and vector.dimension == 2:
             return cls(vector[0], vector[1], vector[2])
 
     @classmethod
     def is_compatible(cls, *value):
-        if len(value) == 3 and all([RealNumber.is_compatible(x) for x in value]):
+        if len(value) == 3 and all(
+            [RealNumber.is_compatible(x) for x in value]
+        ):
             return True
         return NotImplemented
 
     def _plot_3d(self, ax, point=False, origin=None, **kwargs):
         if point:
             ax.scatter([self.x], [self.y], [self.z])
         else:
@@ -704,13 +714,7 @@
                 [self.x],
                 [self.y],
                 [self.z],
             )
 
     def to_2D(self):
         return Vector2D(self.x, self.y)
-
-
-if __name__ == "__main__":
-    import doctest
-
-    doctest.testmod(verbose=False)
```

### Comparing `odeanimate-0.0.7/odeanimate.egg-info/PKG-INFO` & `odeanimate-0.0.8/odeanimate.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odeanimate
-Version: 0.0.7
+Version: 0.0.8
 Summary: A module for useful quick mathematical calculation, plotting and animation.
 Author-email: Miguel Alejandro Salgado Zapien <ekiim@ekiim.xyz>
 License: GPL-2.0
 Project-URL: Homepage, https://odeanimate.ekiim.xyz
 Project-URL: Source, https://github.com/ekiim/odeanimate
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
@@ -34,36 +34,38 @@
 
 
 ## Features
 
 > Most of this features are _W.I.P._ (work in progress)
 
  - [x] Vector objects with _basic_ operations.
+ - [x] Vector objects with _basic_ operations.
  - [x] Function utilities for _real valued_ functions.
  - [x] Automatic plotting for _real valued_ functions.
  - [ ] Generic _ODE_ integrators.
- - [ ] Utilities for curves.
+ - [X] Utilities for curves.
  - [ ] Utilities for surfaces.
  - [ ] Animation Loop and widgets
 
 ## Development
 
-> Initially this project was developed with [`pipenv`](https://pipenv.pypa.io/en/latest/), but for publishing pourpuses
-> I decided to change to [Poetry](https://python-poetry.org/).
+> This project uses [`pipenv`](https://pipenv.pypa.io/) for local development and testing.
+
+If you are intending to:
+
+- Add examples or documentation,
+- develop further this module
+- use and test in an isolated enviroment
+
+you should have `pipenv` installed.
+
+One you cloned the repository, you should be able to execute `pipenv install --dev` and everything should be working.
 
-In order to install the project for development (meaning you are intending to work with it to extend it's capabilities, or improve it's documentation),
-you should make sure you have poetry installed in your machine (check the link above), and simply execute `poetry install`, 
-and after you can start running python commands with it as
-
- - `poetry run python` will run `python` with the configuration required to use this project.
- - `poetry run jupyter lab` should run you a jupyter instance to work on top of the project.
- - `poetry run ./scripts/lint.sh` should run the code linter.
- - `poetry run ./scripts/format.sh`, to format the code.
- - `poetry run ./scripts/tests.sh` should run the test suit, and report back any fails.
- - `poetry run ./scripts/docs.sh` to build the documentation html site.
+Most of what you would need is configured in the `pyproject.toml` file, so if you are using the tools specified in
+the `scripts` section of the `Pipfile` you should be fine.
 
 ## Contribute
 
 If you wish to contribute you can contact me directly, or open an issue in the github repository.
 The main development for this module is done in a private repository, but for visibility and public
 interaction I'll host this in github too.
```

### Comparing `odeanimate-0.0.7/odeanimate.egg-info/SOURCES.txt` & `odeanimate-0.0.8/odeanimate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.7/pyproject.toml` & `odeanimate-0.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-[metadata]
-license = "GPL 2"
-
 [project]
 name = "odeanimate"
 authors = [
     { name="Miguel Alejandro Salgado Zapien", email="ekiim@ekiim.xyz"},
 ]
 description = "A module for useful quick mathematical calculation, plotting and animation."
 readme="README.md"
@@ -20,14 +17,16 @@
     "Topic :: Scientific/Engineering :: Physics",
 ]
 dependencies = [
     "matplotlib"
 ]
 dynamic = ["version"]
 
+[metadata]
+license = "GPL 2"
 
 [project.urls]
 "Homepage" = "https://odeanimate.ekiim.xyz"
 "Source" = "https://github.com/ekiim/odeanimate"
 
 [build-system]
 requires = ["setuptools>=61.0"]
@@ -44,7 +43,12 @@
 addopts = "-q --doctest-modules --cov=odeanimate"
 testpaths = ["odeanimate", "tests"]
 python_files = "*.py"
 
 [tool.pytest.plugins]
 cov = {source = "odeanimate"}
 doctestplus = {}
+
+[tool.black]
+line-length = 80
+docstring-style = 'ignore'
+
```

### Comparing `odeanimate-0.0.7/tests/test_curves.py` & `odeanimate-0.0.8/tests/test_curves.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.7/tests/test_trayectory.py` & `odeanimate-0.0.8/tests/test_trayectory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from random import random
 import pytest
-from odeanimate.vector import (
-    Vector,
-    Vector2D,
-    Vector3D,
-)
+from odeanimate.array import Array
+from odeanimate.vector import Vector
 from odeanimate.domains import Interval
 from odeanimate.codomain import Trajectory
 
 
 def random_vector(cls=Vector, n=4):
     return cls(*(random() for _ in range(n)))
 
@@ -19,22 +16,26 @@
 
         assert isinstance(trajectory, Trajectory)
 
     def test_trayectory_constructor_with_keys(self):
         length = 100
 
         trajectory = Trajectory(
-            *[random_vector(n=4) for _ in range(length)], keys=("t", "x", "y", "z")
+            *[random_vector(n=4) for _ in range(length)],
+            keys=("t", "x", "y", "z"),
         )
 
         assert isinstance(trajectory, Trajectory)
         assert trajectory._keys == ("t", "x", "y", "z")
 
-        assert isinstance(trajectory.x, Vector)
-        assert len(trajectory.x) == length
+        trajectory_x = trajectory.x
 
-        assert isinstance(trajectory["x"], Vector)
+        assert isinstance(trajectory_x, Array)
+        assert len(trajectory_x) == length
+
+        assert isinstance(trajectory["x"], Array)
         assert len(trajectory["x"]) == length
 
         assert (
-            repr(trajectory) == "<Trajectory rows=100 cols=4 keys=('t', 'x', 'y', 'z')>"
+            repr(trajectory)
+            == "<Trajectory rows=100 cols=4 keys=('t', 'x', 'y', 'z')>"
         )
```

### Comparing `odeanimate-0.0.7/tests/test_vector.py` & `odeanimate-0.0.8/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.7/tests/test_vector_from_methods.py` & `odeanimate-0.0.8/tests/test_vector_from_methods.py`

 * *Files identical despite different names*

