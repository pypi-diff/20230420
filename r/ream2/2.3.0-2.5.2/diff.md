# Comparing `tmp/ream2-2.3.0.tar.gz` & `tmp/ream2-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ream2-2.3.0.tar", max compression
+gzip compressed data, was "ream2-2.5.2.tar", max compression
```

## Comparing `ream2-2.3.0.tar` & `ream2-2.5.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1064 2023-02-28 18:34:04.035349 ream2-2.3.0/LICENSE
--rw-r--r--   0        0        0     5267 2023-02-28 18:34:04.035349 ream2-2.3.0/README.md
--rw-r--r--   0        0        0      752 2023-02-28 18:34:04.035349 ream2-2.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/__init__.py
--rw-r--r--   0        0        0    13032 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/actor_graph.py
--rw-r--r--   0        0        0     2152 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/actor_state.py
--rw-r--r--   0        0        0     2040 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/actor_version.py
--rw-r--r--   0        0        0        0 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/actors/__init__.py
--rw-r--r--   0        0        0     3129 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/actors/base.py
--rw-r--r--   0        0        0     1685 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/actors/interface.py
--rw-r--r--   0        0        0    37327 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/cache_helper.py
--rw-r--r--   0        0        0    33795 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/data_model_helper.py
--rw-r--r--   0        0        0    10020 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/dataset_helper.py
--rw-r--r--   0        0        0     8875 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/fs.py
--rw-r--r--   0        0        0     5309 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/helper.py
--rw-r--r--   0        0        0     3482 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/params_helper.py
--rw-r--r--   0        0        0     1090 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/prelude.py
--rw-r--r--   0        0        0     2169 2023-02-28 18:34:04.035349 ream2-2.3.0/ream/workspace.py
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-10-28 21:58:46.047247 ream2-2.5.2/LICENSE
+-rw-r--r--   0        0        0     5267 2022-11-01 19:46:31.826604 ream2-2.5.2/README.md
+-rw-r--r--   0        0        0      752 2023-04-03 05:40:13.167043 ream2-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-10-28 21:58:46.047770 ream2-2.5.2/ream/__init__.py
+-rw-r--r--   0        0        0    13032 2023-02-03 20:33:43.995322 ream2-2.5.2/ream/actor_graph.py
+-rw-r--r--   0        0        0     2173 2023-04-03 05:40:13.167289 ream2-2.5.2/ream/actor_state.py
+-rw-r--r--   0        0        0     2040 2023-04-03 05:40:13.167458 ream2-2.5.2/ream/actor_version.py
+-rw-r--r--   0        0        0        0 2022-10-28 21:58:46.048025 ream2-2.5.2/ream/actors/__init__.py
+-rw-r--r--   0        0        0     3242 2023-04-03 05:40:13.167703 ream2-2.5.2/ream/actors/base.py
+-rw-r--r--   0        0        0     1685 2022-10-28 21:58:46.048171 ream2-2.5.2/ream/actors/interface.py
+-rw-r--r--   0        0        0    37487 2023-04-03 05:40:13.168051 ream2-2.5.2/ream/cache_helper.py
+-rw-r--r--   0        0        0     3393 2023-04-19 22:09:20.839645 ream2-2.5.2/ream/cli_helper.py
+-rw-r--r--   0        0        0    34149 2023-04-03 05:40:13.168657 ream2-2.5.2/ream/data_model_helper.py
+-rw-r--r--   0        0        0    12489 2023-04-03 05:40:13.168961 ream2-2.5.2/ream/dataset_helper.py
+-rw-r--r--   0        0        0     8875 2023-02-03 20:33:43.997558 ream2-2.5.2/ream/fs.py
+-rw-r--r--   0        0        0     6636 2023-04-19 22:09:20.839850 ream2-2.5.2/ream/helper.py
+-rw-r--r--   0        0        0     3607 2023-04-19 22:09:20.840085 ream2-2.5.2/ream/params_helper.py
+-rw-r--r--   0        0        0     1090 2023-04-03 05:40:13.169487 ream2-2.5.2/ream/prelude.py
+-rw-r--r--   0        0        0     2169 2023-04-03 05:40:13.169660 ream2-2.5.2/ream/workspace.py
+-rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 ream2-2.5.2/setup.py
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.5.2/PKG-INFO
```

### Comparing `ream2-2.3.0/LICENSE` & `ream2-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ream2-2.3.0/README.md` & `ream2-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `ream2-2.3.0/pyproject.toml` & `ream2-2.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ream2"
-version = "2.3.0"
+version = "2.5.2"
 description = "An actor architecture for research software"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/binh-vu/ream"
 repository = "https://github.com/binh-vu/ream"
 packages = [
```

### Comparing `ream2-2.3.0/ream/actor_graph.py` & `ream2-2.5.2/ream/actor_graph.py`

 * *Files identical despite different names*

### Comparing `ream2-2.3.0/ream/actor_state.py` & `ream2-2.5.2/ream/actor_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 
     @staticmethod
     def create(
         CLS: Type,
         args: Union[
             DataClassInstance, List[DataClassInstance], Dict[str, DataClassInstance]
         ],
-        version: Optional[Union[int, str]] = None,
+        version: Optional[Union[int, str, ActorVersion]] = None,
         dependencies: Optional[List[ActorState]] = None,
     ) -> ActorState:
         """Compute a unique cache id"""
         if version is None:
-            assert hasattr(CLS, "VERSION"), "Class must have a VERSION attribute"
+            assert hasattr(CLS, "VERSION"), f"Class {CLS} must have a VERSION attribute"
             version = getattr(CLS, "VERSION")
 
         assert isinstance(
             version, (int, str, ActorVersion)
         ), "Version must be a string, a number, or an ActorVersion"
 
         return ActorState(
```

### Comparing `ream2-2.3.0/ream/actor_version.py` & `ream2-2.5.2/ream/actor_version.py`

 * *Files identical despite different names*

### Comparing `ream2-2.3.0/ream/actors/base.py` & `ream2-2.5.2/ream/actors/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,19 +33,21 @@
         self.logger = logger.bind(name=self.__class__.__name__)
 
     def get_actor_state(self) -> ActorState:
         """Get the state of this actor"""
         deps = [actor.get_actor_state() for actor in self.dep_actors]
 
         if isinstance(self.params, EnumParams):
-            deps.append(
-                ActorState.create(
-                    self.params.get_method_class(), self.params.get_method_params()
+            for field in self.params.get_method_fields():
+                deps.append(
+                    ActorState.create(
+                        self.params.get_method_class(field),
+                        self.params.get_method_params(field),
+                    )
                 )
-            )
             params = self.params.without_method_args()
         else:
             params = self.params
 
         return ActorState.create(
             self.__class__,
             params,
```

### Comparing `ream2-2.3.0/ream/actors/interface.py` & `ream2-2.5.2/ream/actors/interface.py`

 * *Files identical despite different names*

### Comparing `ream2-2.3.0/ream/cache_helper.py` & `ream2-2.5.2/ream/cache_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,26 +250,22 @@
         def ser(
             items: Sequence[Optional[SaveLoadProtocol | SaveLoadDirProtocol]],
             file: Path,
             *args,
         ):
             for i, item in enumerate(items):
                 if item is not None:
-                    ifile = file.parent / (
-                        file.name + f"_{i}.{exts[i]}" if exts is not None else f"_{i}"
-                    )
+                    ifile = file / (f"_{i}.{exts[i]}" if exts is not None else f"_{i}")
                     item.save(ifile, *args)
             file.touch()
 
         def deser(file: Path, *args):
             output = []
             for i, cls in enumerate(classes):
-                ifile = file.parent / (
-                    file.name + f"_{i}.{exts[i]}" if exts is not None else f"_{i}"
-                )
+                ifile = file / (f"_{i}.{exts[i]}" if exts is not None else f"_{i}")
                 if ifile.exists():
                     output.append(cls.load(ifile, *args))
                 else:
                     output.append(None)
             return tuple(output)
 
         return {
@@ -862,20 +858,27 @@
     logger: Logger
 
     def get_working_fs(self) -> FS:
         ...
 
 
 class Cacheable:
-    """A class that implement HasWorkingFSTrait so it can be used with @Cache.file decorator."""
+    """A class that implement HasWorkingFSTrait so it can be used with @Cache.file decorator.
 
-    def __init__(self, workdir: Path):
-        self.workdir = FS(workdir)
+    Args:
+        workdir: directory to store cached files.
+        disable: set to True to disable caching. The wrapper method needs to use this flag to be effective!
+    """
+
+    def __init__(self, workdir: Union[FS, Path], disable: bool = False):
+        self.workdir = FS(workdir) if isinstance(workdir, Path) else workdir
         self.logger = logger.bind(name=self.__class__.__name__)
 
+        self.disable = disable
+
     def get_working_fs(self) -> FS:
         return self.workdir
 
 
 class SaveLoadProtocol(Protocol):
     def save(self, file: Path) -> None:
         ...
```

### Comparing `ream2-2.3.0/ream/data_model_helper.py` & `ream2-2.5.2/ream/data_model_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,33 @@
 
 import pickle
 import struct
 from dataclasses import dataclass, fields, is_dataclass
 from pathlib import Path, PosixPath, WindowsPath
 from typing import (
     IO,
+    Annotated,
     BinaryIO,
     Callable,
     Generic,
     List,
     Literal,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
     get_origin,
     get_type_hints,
 )
+from typing_extensions import Self
 from copy import deepcopy
+from nptyping import NDArray, Shape
+from nptyping.typing_ import Float64
 import numpy as np
 import orjson
 import pyarrow as pa
 import pyarrow.parquet as pq
 from nptyping.ndarray import NDArrayMeta  # type: ignore
 from nptyping.shape_expression import get_dimensions  # type: ignore
 from ream.helper import has_dict_with_nonstr_keys
@@ -174,15 +178,15 @@
             )
 
     def __len__(self):
         """Get length of the array"""
         metadata: NumpyDataModelMetadata = self._metadata  # type: ignore
         return len(getattr(self, metadata.array_props[0]))
 
-    def shallow_clone(self):
+    def shallow_clone(self) -> Self:
         return self.__class__(*(getattr(self, name) for name in self.__slots__))
 
     def replace(self, field: str, value: np.ndarray):
         assert getattr(self, field).shape == value.shape
         newobj = self.shallow_clone()
         setattr(newobj, field, value)
         return newobj
@@ -869,14 +873,25 @@
 
         for obj, key in pending_lst:
             obj[key] = tuple(obj[key])
 
         return index
 
 
+class SingleNumpyArray(NumpyDataModel):
+    __slots__ = ["value"]
+
+    value: NDArray[Shape["*"], Float64]
+
+    def __init__(self, value: NDArray[Shape["*"], Float64]):
+        self.value = value
+
+
+SingleNumpyArray.init()
+
 # dir = VirtualDir("/tmp", filetrack=FileTrack())
 # print(dir.name2file, dir.filetrack)
 # dir / "test.h5"
 # print(dir.name2file, dir.filetrack)
 # subdir = dir / "abc"
 # print(dir.name2file, dir.filetrack)
 # print(type(subdir))
```

### Comparing `ream2-2.3.0/ream/dataset_helper.py` & `ream2-2.5.2/ream/dataset_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 from __future__ import annotations
+import random
 import re, functools, orjson
-from typing import TypedDict, Dict, Optional, Tuple, List, Callable, TypeVar
+from typing_extensions import TypeGuard
+from typing import (
+    Iterator,
+    TypedDict,
+    Dict,
+    Optional,
+    Tuple,
+    List,
+    Callable,
+    TypeVar,
+)
 from loguru import logger
 from dataclasses import dataclass
 from ream.actors.interface import E
 from pathlib import Path
-from serde.helper import AVAILABLE_COMPRESSIONS, get_compression, get_filepath
+from serde.helper import AVAILABLE_COMPRESSIONS, get_filepath
 import serde.pickle
 import serde.json
 
-RawSlice = TypedDict("Slice", value=int, is_percentage=bool, absolute_value=int)
+RawSlice = TypedDict(
+    "Slice", value=float, is_percentage=bool, absolute_value=Optional[int]
+)
 E2 = TypeVar("E2")
 
 
-class DatasetDict(Dict[str, E]):
+class DatasetDict(dict[str, E]):
     serde: tuple[Callable, Callable, Optional[str]] = (
         serde.pickle.ser,
         serde.pickle.deser,
         "pkl",
     )
 
     def __init__(self, name: str, subsets: Dict[str, E], provenance: str = ""):
         super().__init__(subsets)
         self.name = name
         self.provenance = provenance
 
+    def into_single_value(self) -> E:
+        assert len(self) == 1
+        return list(self.values())[0]
+
     @classmethod
     def molt(cls, obj: DatasetDict[E]):
         """Change the class of the datasetdict without changing the underlying data. This is useful
         because it relies on the class variable `serde` to determine how to serialize and deserialize examples
         """
         return cls(obj.name, dict(obj), obj.provenance)
 
@@ -84,132 +101,214 @@
                 filepath = dir / (subset if subset != "" else "_empty")
                 ds[subset] = cls.serde[1](filepath, compression)
 
         return ds
 
 
 @dataclass
+class AbsoluteRangeSelection:
+    start: int
+    end: int
+
+    def __len__(self):
+        return self.end - self.start
+
+    def __str__(self):
+        if self.start == 0:
+            return f"[:{self.end}]"
+        return f"[{self.start}:{self.end}]"
+
+    def select(self, array: list[E]) -> list[E]:
+        return array[self.start : self.end]
+
+
+@dataclass
+class PercentageRangeSelection:
+    start: int  # value percentage
+    end: int
+
+    def to_absolute(self, size: int) -> AbsoluteRangeSelection:
+        return AbsoluteRangeSelection(
+            start=int(size * self.start / 100), end=int(size * self.end / 100)
+        )
+
+    def __len__(self):
+        return self.end - self.start
+
+    def __str__(self):
+        if self.start == 0 and self.end == 100:
+            return ""
+        return f"[{self.start}%:{self.end}%]"
+
+    def select(self, array: list[E]) -> list[E]:
+        raise Exception(
+            "PercentageRangeSelection does not support select. Convert it to AbsoluteRangeSelection first using to_absolute"
+        )
+
+
+@dataclass
+class IndexSelection:
+    index: List[int]
+
+    def __len__(self):
+        return len(self.index)
+
+    def __str__(self):
+        return "[" + ",".join([str(i) for i in self.index]) + "]"
+
+    def select(self, array: list[E]) -> list[E]:
+        return [array[i] for i in self.index]
+
+
+@dataclass
 class DatasetQuery:
     dataset: str
-    subsets: Dict[str, Tuple[RawSlice, RawSlice]]
-    shuffle: bool
+    subsets: Dict[
+        str, AbsoluteRangeSelection | PercentageRangeSelection | IndexSelection
+    ]
+    shuffle: bool  # the shuffle is done before splitting
     seed: Optional[int]
 
     @staticmethod
     @functools.lru_cache(maxsize=1024)
     def from_string(query: str) -> DatasetQuery:
         """Query format:
         - <dataset>:(<subset>[<start>:<end>]+)*(:shuffle)?(:seed)?
         - <dataset>[<start>:<end>](:shuffle)?(:seed)?
+        - <dataset>[number(,number)*](:shuffle)?(:seed)?
+        - <dataset>:<subset>
         """
         m = re.match(
-            r"^(?P<ds>[^:\[]+):?(?P<query>(?:[^\[]*\[(?:\d+\%?)?:(?:\d+\%?)?\]\+?)*)(?P<shuffle>:shuffle)?(?P<seed>:\d+)?$",
+            r"^(?P<ds>[^:\[]+):?(?P<query>(?:[^\[]*\[?[^\]]+\]?\+?)*)(?P<shuffle>:shuffle)?(?P<seed>:\d+)?$",
             query,
         )
         if m is None:
             raise ValueError(f"Invalid dataset query: {query}")
 
         dataset = m.group("ds")
         splitquery = m.group("query")
         shuffle = m.group("shuffle") is not None
         seed = int(m.group("seed")[1:]) if m.group("seed") is not None else None
 
-        subsets = {}
+        subsets: dict[
+            str, AbsoluteRangeSelection | PercentageRangeSelection | IndexSelection
+        ] = {}
         if splitquery != "":
             for subset in splitquery.split("+"):
                 m = re.match(
-                    r"^(?P<sname>[^\[]*)\[(?P<start>\d+\%?)?:(?P<end>\d+\%?)\]", subset
+                    r"^(?P<sname>[^\[]*)\[(?P<start>\d+\%?)?:(?P<end>\d+\%?)?\]", subset
                 )
-                assert (
-                    m is not None
-                ), f"Invalid subset spec: `{subset}` in `{splitquery}` in `{query}`"
-                slices = []
-                for name in ["end", "start"]:
-                    if name == "start" and m.group(name) is None:
-                        slices.append(
-                            {
-                                "value": 0,
-                                "is_percentage": slices[-1]["is_percentage"],
-                                "absolute_value": 0,
-                            }
+                if m is not None:
+                    grpstart = m.group("start")
+                    grpend = m.group("end")
+
+                    is_percentage = (
+                        any(
+                            [
+                                grp.endswith("%")
+                                for grp in [grpstart, grpend]
+                                if grp is not None
+                            ]
                         )
-                        continue
-                    value = m.group(name)
-                    is_percentage = value.endswith("%")
+                        or grpend is None
+                    )
+
+                    if grpstart is None:
+                        start = 0
+                    else:
+                        start = (
+                            int(grpstart[:-1])
+                            if grpstart.endswith("%")
+                            else int(grpstart)
+                        )
+
+                    if grpend is None:
+                        assert (
+                            is_percentage
+                        ), "do not support lazy initialization to mixed between absolute and percentage selection"
+                        end = 100
+                    else:
+                        end = int(grpend[:-1]) if grpend.endswith("%") else int(grpend)
+
                     if is_percentage:
-                        value = int(value[:-1]) / 100
+                        subsets[m.group("sname")] = PercentageRangeSelection(start, end)
                     else:
-                        value = int(value)
-                    slices.append(
-                        {
-                            "value": value,
-                            "is_percentage": is_percentage,
-                            "absolute_value": value,
-                        }
+                        subsets[m.group("sname")] = AbsoluteRangeSelection(start, end)
+                else:
+                    m = re.match(
+                        r"^(?P<sname>[^\[]*)\[(?P<index>\d+(?:,\d+)*)\]", subset
                     )
-
-                assert (
-                    len({x["is_percentage"] for x in slices}) == 1
-                ), f"Slices must be either percentage or absolute: {slices}"
-
-                start = slices[1]
-                end = slices[0]
-                subsets[m.group("sname")] = (start, end)
+                    if m is not None:
+                        subsets[m.group("sname")] = IndexSelection(
+                            [int(x) for x in m.group("index").split(",")]
+                        )
+                    else:
+                        m = re.match(r"^(?P<sname>[a-zA-Z]+)$", subset)
+                        assert (
+                            m is not None
+                        ), f"Invalid subset spec: `{subset}` in `{splitquery}` in `{query}`"
+                        subsets[m.group("sname")] = PercentageRangeSelection(0, 100)
         else:
-            subsets: Dict[str, Tuple[RawSlice, RawSlice]] = {
-                "": (
-                    {"value": 0, "is_percentage": True, "absolute_value": 0},
-                    {"value": 1, "is_percentage": True, "absolute_value": 1},
-                )
-            }
+            subsets: Dict[
+                str, AbsoluteRangeSelection | PercentageRangeSelection | IndexSelection
+            ] = {"": PercentageRangeSelection(0, 100)}
         return DatasetQuery(dataset, subsets, shuffle, seed)
 
     def select(self, array: List[E]) -> DatasetDict[List[E]]:
         n_exs = len(array)
 
-        if all(start["is_percentage"] for (start, end) in self.subsets.values()):
-            # convert percentage to absolute
-            for (start, end) in self.subsets.values():
-                start["absolute_value"] = int(start["value"] * n_exs)
-                end["absolute_value"] = int(end["value"] * n_exs)
-
+        # gate check for percentage range selection that select all data
+        subsets = {
+            subset: selection.to_absolute(n_exs)
+            if isinstance(selection, PercentageRangeSelection)
+            else selection
+            for subset, selection in self.subsets.items()
+        }
+        if all(isinstance(s, PercentageRangeSelection) for s in self.subsets.values()):
             total_percentage = sum(
-                [
-                    (end["value"] - start["value"]) * 100
-                    for start, end in self.subsets.values()
-                ]
-            )
-            n_selected = sum(
-                [
-                    end["absolute_value"] - start["absolute_value"]
-                    for start, end in self.subsets.values()
-                ]
+                len(selection) for selection in self.subsets.values()
             )
+            n_selected = sum(len(selection) for selection in subsets.values())
             if total_percentage == 100 and n_selected != n_exs:
                 logger.debug(
                     "Total percentage is 100%, but the number of selected examples do not match, adjusting the first subset"
                 )
                 assert n_selected < n_exs
-                for i, (start, end) in enumerate(self.subsets.values()):
+
+                for i, selection in enumerate(subsets.values()):
+                    assert isinstance(selection, AbsoluteRangeSelection)
                     if i != 0:
-                        start["absolute_value"] += n_exs - n_selected
-                    end["absolute_value"] += n_exs - n_selected
-                assert n_exs == sum(
-                    [
-                        end["absolute_value"] - start["absolute_value"]
-                        for start, end in self.subsets.values()
+                        selection.start += n_exs - n_selected
+                    selection.end += n_exs - n_selected
+
+                assert n_exs == sum(len(selection) for selection in subsets.values())
+
+        if self.shuffle:
+            array_index = list(range(n_exs))
+            random.Random(self.seed).shuffle(array_index)
+
+            output_subsets = {}
+            for subset, selection in subsets.items():
+                if isinstance(selection, IndexSelection):
+                    indices = set(selection.index)
+                    output_subsets[subset] = [
+                        array[i] for i in array_index if i in indices
                     ]
-                )
+                else:
+                    output_subsets[subset] = [
+                        array[idx] for idx in selection.select(array_index)
+                    ]
+        else:
+            output_subsets = {
+                subset: selection.select(array) for subset, selection in subsets.items()
+            }
 
         return DatasetDict(
             self.dataset,
-            {
-                subset: array[start["absolute_value"] : end["absolute_value"]]
-                for subset, (start, end) in self.subsets.items()
-            },
+            output_subsets,
         )
 
     def strip(self) -> DatasetQuery:
         """Remove the subset name from the query. Error when there are multiple subsets."""
         if len(self.subsets) > 1:
             raise ValueError(
                 f"Cannot strip subsets from query when there are multiple subsets: {self.subsets}"
@@ -223,42 +322,30 @@
 
     def subset(self, subset: str) -> DatasetQuery:
         """Select a subset from the query. Error when the subset does not exist."""
         return DatasetQuery(
             self.dataset, {subset: self.subsets[subset]}, self.shuffle, self.seed
         )
 
-    def get_query(self, subsets: Optional[str | List[str]]) -> str:
+    def iter_subset(self) -> Iterator[Tuple[str, DatasetQuery]]:
+        """Iterate over the subsets in the query."""
+        return ((subset, self.subset(subset)) for subset in self.subsets)
+
+    def get_query(self, subsets: Optional[str | List[str]] = None) -> str:
         """Generate a query string for retrieving the subsets of the dataset."""
         if subsets is None:
             subsets = list(self.subsets.keys())
         elif isinstance(subsets, str):
             subsets = [subsets]
         else:
             assert all(subset in self.subsets for subset in subsets)
 
-        filters = []
-        for subset in subsets:
-            start, end = self.subsets[subset]
-            if start["is_percentage"]:
-                start = f"{int(start['value'] * 100)}%"
-            else:
-                start = start["value"]
-            if end["is_percentage"]:
-                end = f"{int(end['value'] * 100)}%"
-            else:
-                end = end["value"]
-            if start == "0%" and end == "100%":
-                filters.append(f"{subset}")
-            elif start == 0:
-                filters.append(f"{subset}[:{end}]")
-            else:
-                filters.append(f"{subset}[{start}:{end}]")
-
-        filter = "+".join(filters)
+        filter = "+".join(
+            [f"{subset}{str(self.subsets[subset])}" for subset in subsets]
+        )
         if len(subsets) > 1 or "" not in subsets:
             filter = f":{filter}"
 
         return f"{self.dataset}{filter}{':shuffle' if self.shuffle else ''}{f':{self.seed}' if self.seed is not None else ''}"
 
     def get_subset_disk_names(self) -> Dict[str, str]:
         return {name: "_empty" if name == "" else name for name in self.subsets.keys()}
```

### Comparing `ream2-2.3.0/ream/fs.py` & `ream2-2.5.2/ream/fs.py`

 * *Files identical despite different names*

### Comparing `ream2-2.3.0/ream/helper.py` & `ream2-2.5.2/ream/helper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import atexit
+import cProfile
+from contextlib import contextmanager
+import functools
 from pathlib import Path
 import sys
 from typing import Type, TypeVar, Union, get_args, get_origin, Tuple
 from loguru import logger
 import orjson
 
 TYPE_ALIASES = {"typing.List": "list", "typing.Dict": "dict", "typing.Set": "set"}
@@ -128,7 +132,61 @@
     args = get_args(ann)
 
     if origin is None or len(args) == 0:
         return False
     if origin is dict and args[0] is not str:
         return True
     return any(has_dict_with_nonstr_keys(arg) for arg in args)
+
+
+@contextmanager
+def profile(
+    outfile: Union[str, Path] = "/tmp/profile.prof",
+    engine="yappi",
+    clock="wall",
+    output_type="pstat",
+):
+    """Profile the execution of the code using Yappi"""
+    if engine == "yappi":
+        import yappi
+
+        yappi.set_clock_type(clock)
+        try:
+            yappi.start(builtins=True, profile_threads=False)
+            yield
+        finally:
+            yappi.stop()
+            stats = yappi.get_func_stats()
+            stats.save(outfile, type=output_type)
+    else:
+        profile = cProfile.Profile()
+        try:
+            profile.enable()
+            yield
+        finally:
+            profile.disable()
+            profile.dump_stats(outfile)
+
+
+def profile_fn(
+    outfile: Union[str, Path] = "/tmp/profile.prof",
+):
+    profile = cProfile.Profile()
+
+    def flush_profile():
+        profile.disable()
+        profile.dump_stats(outfile)
+
+    atexit.register(flush_profile)
+
+    def wrapper_fn(func):
+        @functools.wraps(func)
+        def fn(*args, **kwargs):
+            try:
+                profile.enable()
+                return func(*args, **kwargs)
+            finally:
+                profile.disable()
+
+        return fn
+
+    return wrapper_fn  # type: ignore
```

### Comparing `ream2-2.3.0/ream/params_helper.py` & `ream2-2.5.2/ream/params_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from dataclasses import Field, asdict, dataclass, fields, is_dataclass, replace
 from typing import Any, Dict, List, Type, Union
 
 DataClassInstance = Any
 
 
 @dataclass
@@ -32,49 +33,51 @@
     The field `method` also needs a metadata `variants` to specify the method's class.
 
     At the same time, it should only only parameters of a method. For example, if `method` is `method_a`,
     then `method_a` is not None and `method_b` is `None`.
     """
 
     def __post_init__(self):
-        method_field = self._get_method_field()
-        method = getattr(self, method_field.name)
-        assert hasattr(self, method)
-
-        for name in method_field.metadata["variants"].keys():
-            if name != method:
-                # set params of other methods to None
-                setattr(self, name, None)
+        for method_field in self.get_method_fields():
+            method = getattr(self, method_field.name)
+            assert hasattr(self, method)
+            for name in method_field.metadata["variants"].keys():
+                if name != method:
+                    # set params of other methods to None
+                    setattr(self, name, None)
 
     def without_method_args(self):
-        """Return a shallow copy of this object with the method's parameters set to None."""
+        """Return a shallow copy of this object with the methods' parameters set to None."""
         other = replace(self)  # type: ignore -- method in dataclass
-        setattr(other, getattr(self, self._get_method_field().name), None)
+        for field in self.get_method_fields():
+            setattr(other, getattr(self, field.name), None)
         return other
 
-    def get_method_class(self) -> Type:
-        method_field = self._get_method_field()
+    def get_method_class(self, method_field: Field) -> Type:
         method = getattr(self, method_field.name)
-        return self._get_method_field().metadata["variants"][method]
+        return method_field.metadata["variants"][method]
 
-    def get_method_params(self) -> DataClassInstance:
-        method_field = self._get_method_field()
+    def get_method_params(self, method_field: Field) -> DataClassInstance:
         method = getattr(self, method_field.name)
         return getattr(self, method)
 
-    def _get_method_field(self) -> Field:
-        if not hasattr(self, "__method_field"):
+    def get_method_fields(self) -> list[Field]:
+        if not hasattr(self, "__method_fields"):
+            method_fields = []
             for field in fields(self):
                 if "variants" in field.metadata:
-                    self.__method_field = field
-                    return self.__method_field
-            raise ValueError(
-                f"No method field found in {self.__class__}. The method field is the one has `variants` property (dict type) in its metadata"
-            )
-        return self.__method_field
+                    method_fields.append(field)
+
+            if len(method_fields) == 0:
+                raise ValueError(
+                    f"No method field found in {self.__class__}. The method field is the one has `variants` property (dict type) in its metadata"
+                )
+
+            self.__method_fields = method_fields
+        return self.__method_fields
 
 
 def are_valid_parameters(
     params: Union[
         DataClassInstance, List[DataClassInstance], Dict[str, DataClassInstance]
     ]
 ):
```

### Comparing `ream2-2.3.0/ream/prelude.py` & `ream2-2.5.2/ream/prelude.py`

 * *Files identical despite different names*

### Comparing `ream2-2.3.0/ream/workspace.py` & `ream2-2.5.2/ream/workspace.py`

 * *Files identical despite different names*

### Comparing `ream2-2.3.0/PKG-INFO` & `ream2-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ream2
-Version: 2.3.0
+Version: 2.5.2
 Summary: An actor architecture for research software
 Home-page: https://github.com/binh-vu/ream
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

