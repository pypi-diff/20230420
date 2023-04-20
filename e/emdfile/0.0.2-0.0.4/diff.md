# Comparing `tmp/emdfile-0.0.2.tar.gz` & `tmp/emdfile-0.0.4.tar.gz`

## Comparing `emdfile-0.0.2.tar` & `emdfile-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,49 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.2/.pytest_cache/README.md
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 emdfile-0.0.2/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 emdfile-0.0.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     8681 2020-02-02 00:00:00.000000 emdfile-0.0.2/src/emdfile/README.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 emdfile-0.0.2/src/emdfile/__init__.py
--rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 emdfile-0.0.2/src/emdfile/read.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 emdfile-0.0.2/src/emdfile/tqdmnd.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 emdfile-0.0.2/src/emdfile/version.py
--rw-r--r--   0        0        0    18997 2020-02-02 00:00:00.000000 emdfile-0.0.2/src/emdfile/write.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 emdfile-0.0.2/src/emdfile/classes/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 emdfile-0.0.2/src/emdfile/classes/array.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 emdfile-0.0.2/src/emdfile/classes/custom.py
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 emdfile-0.0.2/src/emdfile/classes/metadata.py
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 emdfile-0.0.2/src/emdfile/classes/pointlist.py
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 emdfile-0.0.2/src/emdfile/classes/pointlistarray.py
--rw-r--r--   0        0        0    23010 2020-02-02 00:00:00.000000 emdfile-0.0.2/src/emdfile/classes/tree.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 emdfile-0.0.2/src/emdfile/classes/utils.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 emdfile-0.0.2/test/clear_h5_files.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 emdfile-0.0.2/test/test_base_classes.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 emdfile-0.0.2/test/test_emd.py
--rw-r--r--   0        0        0    29281 2020-02-02 00:00:00.000000 emdfile-0.0.2/test/test_tree.py
--rw-r--r--   0        0        0   336331 2020-02-02 00:00:00.000000 emdfile-0.0.2/tutorials/emd_intro_example.ipynb
--rw-r--r--   0        0        0   111978 2020-02-02 00:00:00.000000 emdfile-0.0.2/tutorials/emd_package_walkthrough.ipynb
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 emdfile-0.0.2/tutorials/test_custom_class.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 emdfile-0.0.2/tutorials/sample_custom_class_module/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 emdfile-0.0.2/tutorials/sample_custom_class_module/classes/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 emdfile-0.0.2/tutorials/sample_custom_class_module/classes/my_custom_class.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 emdfile-0.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 emdfile-0.0.2/LICENSE
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 emdfile-0.0.2/README.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 emdfile-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 emdfile-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.4/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.4/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.4/.pytest_cache/README.md
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 emdfile-0.0.4/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 emdfile-0.0.4/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.4/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     8681 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/README.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/__init__.py
+-rw-r--r--   0        0        0    10373 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/read.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/tqdmnd.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/version.py
+-rw-r--r--   0        0        0    31055 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/write.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/array.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/custom.py
+-rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/metadata.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/pointlist.py
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/pointlistarray.py
+-rw-r--r--   0        0        0    23442 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/tree.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/utils.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/clear_h5_files.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/test_base_classes.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/test_emd.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/test_header.py
+-rw-r--r--   0        0        0    28996 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/test_tree.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0   384837 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/emdfile_intro_example.ipynb
+-rw-r--r--   0        0        0   167826 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/emdfile_package_walkthrough.ipynb
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/test_custom_class.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/.pytest_cache/README.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0    81358 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/pngs/node.png
+-rw-r--r--   0        0        0    41590 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/pngs/tree.png
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/sample_custom_class_module/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/sample_custom_class_module/my_custom_classes.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 emdfile-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 emdfile-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 emdfile-0.0.4/README.md
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 emdfile-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 emdfile-0.0.4/PKG-INFO
```

### Comparing `emdfile-0.0.2/.pytest_cache/v/cache/nodeids` & `emdfile-0.0.4/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.2/src/emdfile/README.md` & `emdfile-0.0.4/src/emdfile/README.md`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.2/src/emdfile/read.py` & `emdfile-0.0.4/src/emdfile/read.py`

 * *Files 9% similar despite different names*

```diff
@@ -104,16 +104,16 @@
 
 
 
 ########## EMD 1.0+ reader ##########
 
 def read(
     filepath,
-    tree: Optional[Union[bool,str]] = True,
     emdpath: Optional[str] = None,
+    tree: Optional[Union[bool,str]] = True,
     **legacy_options,
     ):
     """
     File reader for EMD 1.0+ files.
 
     Args:
         filepath (str or Path): the file path
@@ -142,21 +142,19 @@
     er2 = f"specified filepath '{filepath}' was not found on the filesystem"
     er3 = f"{filepath} isn't a valid EMD 1.0 file."
     assert(isinstance(filepath, (str,pathlib.Path) )), er1
     assert(exists(filepath)), er2
     assert(_is_EMD_file(filepath)), er3
 
 
-    # get version
+    # get/check version
     v = _get_EMD_version(filepath)
-
-
-    # TODO: catch for older versions...
-    if v[0] < 1:
-        raise Exception('Reader does not currently support EMD v<1.0')
+    if v != (1,0,0):
+        #raise Exception('oh dear')
+        pass
 
 
 
     # determine `emdpath` if it was left as None
     if emdpath is None:
         rootgroups = _get_EMD_rootgroups(filepath)
         if len(rootgroups) == 0:
@@ -203,40 +201,52 @@
                 return root
 
         # Read...
 
         # ...if the whole tree was requested
         if nodegroup is rootgroup and tree in (True,'branch'):
             # build the tree
-            _populate_tree(root,rootgroup)
+            n = _populate_tree(root,rootgroup)
+            # return...
+            if n == 1:
+                # ...if there's one node, return it
+                key = list(root._branch.keys())[0]
+                node = root.tree(key)
+            elif n == 0 and len(root.metadata) == 1:
+                # ...if there's no nodes and one dictionary,
+                # return it
+                key = list(root.metadata.keys())[0]
+                node = root.metadata[key]
+            else:
+                # ...otherwise, return the root
+                node = root
 
         # ...if a single node was requested
         elif tree is False:
             # read the node
             node = _read_single_node(nodegroup)
             # build the tree and return
             root.add_to_tree(node)
-            return root
 
         # ...if a branch was requested
         elif tree is True:
             # read source node and add to tree
             node = _read_single_node(nodegroup)
             root.add_to_tree(node)
             # build the tree
             _populate_tree(node,nodegroup)
 
         # ...if `tree == 'branch'`
         else:
             # build the tree
             _populate_tree(root,nodegroup)
-
+            node = root
 
     # Return
-    return root
+    return node
 
 
 
 
 
 # group / tree reading utilities
 
@@ -246,40 +256,44 @@
     instantiates and returns an instance of the class with
     this group's data and metadata
     """
     __class__ = _get_class(grp)
     data = __class__.from_h5(grp)
     return data
 
-def _populate_tree(node,group):
+def _populate_tree(node,group,count=0):
     """
     `node` is a Node and `group` is its parallel h5py Group.
     Reads the tree underneath this nodegroup in the h5 file and adds it
     to the runtime tree underneath this node. Does *not* read `group`
     itself - this function grafts everything underneath `group` onto node
+
+    Returns the number of new nodes added to the tree
     """
     keys = [k for k in group.keys() if isinstance(group[k],h5py.Group)]
     keys = [k for k in keys if 'emd_group_type' in group[k].attrs.keys()]
     keys = [k for k in keys if group[k].attrs['emd_group_type'] in \
         EMD_data_group_types]
 
     for key in keys:
         #print(f"Reading group {group[key].name}")
         new_node = _read_single_node(group[key])
+        count += 1
         # Handle RootedNodes, which need to be grafted rather than added
         if isinstance(new_node,RootedNode):
             new_node.graft(node)
             new_node._add_root_links(node)
         else:
             node.add_to_tree(new_node)
         _populate_tree(
             new_node,
-            group[key]
+            group[key],
+            count = count
         )
-    pass
+    return count
 
 
 
 
 
 
 
@@ -302,20 +316,20 @@
         linelevels.append(tablevel)
     keys = [k for k in f.keys() if isinstance(f[k],h5py.Group)]
     if not show_metadata:
         keys = [k for k in keys if k != 'metadatabundle']
     N = len(keys)
     for i,k in enumerate(keys):
         string = ''
-        string += '|' if 0 in linelevels else ''
+        string += '|' if 0 in linelevels else ' '
         for idx in range(tablevel):
-            l = '|' if idx+1 in linelevels else ''
-            string += '\t'+l
+            l = '|' if idx+1 in linelevels else ' '
+            string += '   '+l
         #print(string)
-        print(string+'--'+k)
+        print(string+'---'+k)
         if i == N-1:
             linelevels.remove(tablevel)
         _print_h5pyFile_tree(
             f[k],
             tablevel=tablevel+1,
             linelevels=linelevels,
             show_metadata=show_metadata)
```

### Comparing `emdfile-0.0.2/src/emdfile/tqdmnd.py` & `emdfile-0.0.4/src/emdfile/tqdmnd.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.2/src/emdfile/write.py` & `emdfile-0.0.4/src/emdfile/write.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # Write EMD 1.0 formatted HDF5 files.
 
 import h5py
 import numpy as np
-from os.path import exists
+from warnings import warn
+from os.path import exists,basename
 from os import remove
+from uuid import uuid4
 from emdfile.read import _is_EMD_file, _get_EMD_rootgroups
 from emdfile.classes.utils import EMD_data_group_types
 from emdfile.classes import (
     Node,
     Root,
     Array,
     Metadata
 )
 
 
 def write(
     filepath,
     data,
     mode = 'w',
-    tree = True,
     emdpath = None,
+    tree = True,
     ):
     """
     Saves data to a .h5 file at filepath. Specific behavior depends on the
     `data`, `mode`, `tree`, and `emdpath` arguments.
 
     Calling
 
@@ -43,15 +45,15 @@
     emd.Array or emd.Metadata instance, assigns the name 'np.array' or
     'dictionary', places the object in a root of this name and saves. If
     `data` is a list of objects which are all numpy arrays, Python dictionaries,
     or emd.Node instances, places all these objects into a single root, assigns
     the roots name according to the first object in the list, and saves.
 
     To write a single node from a tree,  set `tree` to False. To write the
-    tree underneath a node but exclude the node itself set `tree` to 'noroot'.
+    tree underneath a node but exclude the node itself set `tree` to None.
 
     To add to an existing EMD file, use the `mode` argument to set append or
     appendover mode. If the `emdpath` variable is not set and `data` has a
     runtime root that does not exist in the EMD root groups already present,
     adds the new root and writes as described above. If `emdpath` is not set
     and the runtime root group matches a root group that's already present,
     this function performs a diff operation between the root metadata and
@@ -99,15 +101,15 @@
             between the data passed and that present in the extent HDF5 file
             tree, add any data not already in the H5, and then either skips
             or overwrites conflicting nodes in append or appendover mode,
             respectively.
         tree: indicates how the object tree nested inside `data` should
             be treated.  If `True` (default), the entire tree is saved.
             If `False`, only this object is saved, without its tree. If
-            `"noroot"`, saves the entire tree underneath `data`, but not
+            `None`, saves the entire tree underneath `data`, but not
             the node at `data` itself.
         emdpath (str or None): optional parameter used in conjunction with
             append or appendover mode; if passed in write or overwrite mode,
             this argument is ignored. Indicates where in an existing EMD
             file tree to place the data. Must be a '/' delimited string
             pointing to an existing EMD file tree node.
     """
@@ -130,70 +132,122 @@
         'ao',
         'o+',
         '+o',
         'appendover'
     ]
     allmodes = writemode + overwritemode + appendmode + appendovermode
 
+    # emdpath implies append mode
+    if emdpath is not None and mode not in appendovermode:
+        mode = 'a'
+
+
+    # validate `mode` and `tree` inputs
+    er = f"unrecognized mode {mode}; mode must be in {allmodes}"
+    assert(mode in allmodes), er
+    if tree == 'noroot':
+        warn("`tree = 'noroot'` is deprecated and will be removed in a future version. Use `tree = None` instead.")
+        tree = None
+    assert(tree in (True,False,None)), f"invalid value {tree} passed for `tree`"
+    if mode in writemode:
+        assert(not(exists(filepath))), "A file already exists at this destination; use append or overwrite mode, or choose a new file path."
+
+
+    # validate `data` inputs, and
     # handle non-Node `data` inputs
+
+    # numpy array -> Array
     if isinstance(data, np.ndarray):
-        root = Root(name='np.array')
+        root = Root(name='root')
         data = Array(name='np.array',data=data)
         root.add_to_tree(data)
+
+    # dictionaries -> Metadata
     elif isinstance(data, dict):
-        root = Root(name='dictionary')
+        root = Root(name='root')
         md = Metadata(name='dictionary',data=data)
         root.metadata = md
         data = root
+
+    # for lists...
     elif isinstance(data, (list,tuple)):
         assert(all( [isinstance(x,(np.ndarray,dict,Node)) for x in data] )), \
             "can only save np.array, dictionary, or emd.Node objects"
-        if isinstance(data[0],Node): name=data[0].name
-        elif isinstance(data[0],np.ndarray): name='np.array'
-        else: name='dictionary'
-        root = Root(name=name)
+
+        # ...save lists of Roots as multiple EMD trees
+        if any([isinstance(x,Root) for x in data]):
+            assert(all([isinstance(x,Root) for x in data])), \
+            "if saving a list containing a Root, all list elements must be Roots"
+            # save the first root with a call to save, then
+            # change to append mode and save other roots
+            write(
+                filepath,
+                data[0],
+                mode=mode,
+                tree=tree
+            )
+            if mode in writemode:
+                mode = 'a'
+            elif mode in overwritemode:
+                mode = 'ao'
+            for x in data[1:]:
+                write(
+                    filepath,
+                    x,
+                    mode=mode,
+                    tree=tree
+                )
+            return
+
+        # ...otherwise store all list elements in a single tree...
+        root = Root(name='root')
         ar_ind,md_ind = 0,0
         for d in data:
+
+            # ...with numpy arrays as Arrays
             if isinstance(d,np.ndarray):
                 d = Array(name=f'np.array_{ar_ind}',data=d)
                 ar_ind += 1
                 root.add_to_tree(d)
+
+            # ...dictionaries as Metadata
             elif isinstance(d,dict):
                 d = Metadata(name=f'dictionary_{md_ind}',data=d)
                 md_ind += 1
                 root.metadata = d
+
+            # ...and Nodes as themselves
             else:
+                assert(isinstance(d,Node)), f"invalid data type in `data` list, {type(d)}"
                 root.add_to_tree(d)
         data = root
 
-    # validate inputs
-    er = f"unrecognized mode {mode}; mode must be in {allmodes}"
-    assert(mode in allmodes), er
-    assert(tree in (True,False,'noroot')), f"invalid value {tree} passed for `tree`"
+    # `data` should now be a Node!
     assert(isinstance(data,Node)), f"invalid type {type(data)} found for `data`"
-    if mode in writemode:
-        assert(not(exists(filepath))), "A file already exists at this destination; use append or overwrite mode, or choose a new file path."
-
-    # overwrite: delete existing file
-    if mode in overwritemode:
-        if exists(filepath):
-            remove(filepath)
-        mode = 'w'
 
     # handle rootless data
     added_a_root = False
     if data._root is None:
         added_a_root = True
         root = Root(name=data.name)
         root.add_to_tree(data)
     else:
         # get the root
         root = data.root
 
 
+
+    # overwrite mode - delete existing file
+    if mode in overwritemode:
+        if exists(filepath):
+            remove(filepath)
+        mode = 'w'
+
+
+
     # write a new file
     if mode in writemode or (
         mode in appendmode+appendovermode and not exists(filepath)):
 
 
         # open the file
         with h5py.File(filepath, 'w') as f:
@@ -207,37 +261,118 @@
             _write_from_root(
                 file = f,
                 root = root,
                 data = data,
                 tree = tree
             )
 
+
+
     # append to an existing file
     else:
 
         # validate that its an EMD file
         # get the rootgroups
         assert(_is_EMD_file(filepath)), "{filepath} does not point to an EMD 1.0 file"
         emd_rootgroups = _get_EMD_rootgroups(filepath)
 
         # open the file
         with h5py.File(filepath, 'a') as f:
 
-            # if the root doesn't already exist, do a simple write as above
-            if not( root.name in emd_rootgroups ):
+
+
+            # if the root doesn't already exist and emdpath is None,
+            # do a simple write as above
+            if not(root.name in emd_rootgroups) and (emdpath is None):
 
                 _write_from_root(
                     file = f,
                     root = root,
                     data = data,
                     tree = tree
                 )
 
-            # otherwise, peform a diff...
-            else:
+
+
+            # if the root doesn't already exist and emdpath is specified,
+            # append the data to the target node
+            elif not(root.name in emd_rootgroups):
+
+                # parse emdpath
+                if emdpath[0] == '/':
+                    emdpath = emdpath[1:]
+                l = emdpath.split('/')
+                rootname = l[0]
+                treepath = '/'.join(l[1:])
+
+                # get the rootgroup
+                assert(rootname in f.keys()), f"No root called {rootname} found - check your `emdpath`"
+                rootgroup = f[rootname]
+
+                # validate the emdpath
+                # set target_grp to targeted EMD node
+                where = _validate_treepath(
+                    rootgroup,
+                    treepath
+                )
+                #print(treepath)
+                #print(data._treepath)
+                #print(where)
+                #print(where[0].name)
+                if where is False:
+                    raise Exception(f"No node found at {emdpath} in the EMD tree called {rootname} - check your `emdpath`")
+                elif where[1] is False:
+                    raise Exception(f"No node found at {emdpath} in the EMD tree called {rootname} - check your `emdpath`")
+                else:
+                    target_grp = where[0]
+
+
+                # append to the tree...
+
+                # ...if data is Root and tree is False
+                if isinstance(data,Root) and (tree is False):
+                    raise Exception("Incompatible inputs: if appending from a Root to an existing tree, `tree` can't be False.  Try changing `data` or `tree`.")
+
+                # ...if data is Root and tree is True or None
+                elif isinstance(data,Root):
+                    _write_tree(
+                        target_grp,
+                        data
+                    )
+
+                # ...if data is a Node and tree is False
+                elif tree is False:
+                    _write_single_node(
+                        target_grp,
+                        data
+                    )
+
+                # ...if data is a Node and tree is True
+                elif tree is True:
+                    target_grp = _write_single_node(
+                        target_grp,
+                        data
+                    )
+                    _write_tree(
+                        target_grp,
+                        data
+                    )
+
+                # ...if data is a Node and tree is None
+                else:
+                    _write_tree(
+                        target_grp,
+                        data
+                    )
+
+
+
+            # if the root does exist and emdpath is None,
+            # peform diffmerge A
+            elif emdpath is None:
 
                 # choose how to handle conflicts
                 appendover = True if mode in appendovermode else False
 
                 # get the rootgroup
                 rootgroup = f[root.name]
 
@@ -319,37 +454,201 @@
                                 pass
                             else:
                                 _write_tree(
                                     where,
                                     data
                                 )
 
+
+
+            # if the root does exist and emdpath is specified,
+            # peform diffmerge B
+            else:
+
+                # choose how to handle conflicts
+                appendover = True if mode in appendovermode else False
+
+                # parse emdpath
+                if emdpath[0] == '/':
+                    emdpath = emdpath[1:]
+                l = emdpath.split('/')
+                rootname = l[0]
+                treepath = '/'.join(l[1:])
+
+                # get the rootgroup
+                rootgroup = f[root.name]
+
+                # validate the emdpath
+                # set target_grp to targeted EMD node
+                where = _validate_treepath(
+                    rootgroup,
+                    treepath
+                )
+                if where is False:
+                    raise Exception(f"No node found at {emdpath} in the EMD tree called {rootname} - check your `emdpath`")
+                elif where[1] is False:
+                    raise Exception(f"No node found at {emdpath} in the EMD tree called {rootname} - check your `emdpath`")
+                else:
+                    target_grp = where[0]
+
+
+                # compare/append root metadata
+                _append_root_metadata(
+                    rootgroup = rootgroup,
+                    root = root,
+                    appendover = appendover
+                )
+
+
+
+                # choose behavior and write...
+
+                # ...if the data is the root
+                if data is root:
+
+                    # Confirm that the target node is downstream of the root...
+                    assert(rootgroup.__contains__(target_grp.name)), "Specified target node not found in the EMD file - check your emdpath."
+
+                    # get the path from source to target, then
+                    # move `data` to the target node point
+                    path_to_target = target_grp.name.replace(rootgroup.name,'')[1:]
+                    try:
+                        data = data.tree(path_to_target)
+                    except AssertionError:
+                        raise Exception("Append failure - the target EMD node exists downstream of the source EMD node, however the target is not present in the corresponding runtime tree")
+                    # write
+                    if appendover and tree in (True,False):
+                        target_grp = _overwrite_single_node(
+                            target_grp,
+                            data
+                        )
+                    if tree in (True,None):
+                        _append_branch(
+                            target_grp,
+                            data,
+                            appendover
+                        )
+
+
+                # ...if the data is a node...
+                else:
+                    # validate the source node path
+                    where = _validate_treepath(
+                        rootgroup,
+                        data._treepath
+                    )
+                    # ...if the source node is not in the H5
+                    if where is False:
+                        raise Exception("The data passed can't be appended to it's corresponding H5 tree - the source runtime node can't be matched to the existing tree")
+                    else:
+                        source_grp,inside = where
+
+                        # ...if the source node is one node beyond the H5
+                        if inside is False:
+                            # ...if it is one node past the targetted node, write
+                            if source_grp.name == target_grp.name:
+                                if tree in (True,None):
+                                    _append_branch(
+                                        target_grp,
+                                        data,
+                                        appendover
+                                    )
+                                else:
+                                    _write_single_node(
+                                        target_grp,
+                                        data
+                                    )
+                            # ...otherwise, raise an Exception
+                            else:
+                                raise Exception("The data passed can't be added to it's corresponding H5 tree - check that the data's `.tree()` path is present in the existing EMD file")
+
+                        # ...if the source node is in inside the H5
+                        else:
+                            # ...if the source node is the target node, write
+                            if source_grp.name == target_grp.name:
+                                if appendover and tree in (True,False):
+                                    target_grp = _overwrite_single_node(
+                                        target_grp,
+                                        data
+                                    )
+                                if tree in (True,None):
+                                    _append_branch(
+                                        target_grp,
+                                        data,
+                                        appendover
+                                    )
+                            # ...if the source node is one node downstream of the target, write
+                            elif basename(source_grp.name) in list(target_grp.keys()):
+                                target_grp = source_grp
+                                if appendover and tree in (True,False):
+                                    target_grp = _overwrite_single_node(
+                                        target_grp,
+                                        data
+                                    )
+                                if tree in (True,None):
+                                    _append_branch(
+                                        target_grp,
+                                        data,
+                                        appendover
+                                    )
+                            # ...if the target node is downstream of the source node...
+                            elif source_grp.__contains__(target_grp.name):
+                                # get the path from source to target, then
+                                # move `data` to the target node point
+                                path_to_target = target_grp.name.replace(source_grp.name,'')[1:]
+                                try:
+                                    data = data.tree(path_to_target)
+                                except AssertionError:
+                                    raise Exception("Append failure - the target EMD node exists downstream of the source EMD node, however the target is not present in the corresponding runtime tree")
+                                # write
+                                if appendover and tree in (True,False):
+                                    target_grp = _overwrite_single_node(
+                                        target_grp,
+                                        data
+                                    )
+                                if tree in (True,None):
+                                    _append_branch(
+                                        target_grp,
+                                        data,
+                                        appendover
+                                    )
+
+                            # ...otherwise raise an exception
+                            else:
+                                raise Exception("Append failure - target node may not be downstream of source node.  Check the emdpath and the runtime data tree.")
+
+
+
+
     # if a root was added, remove it
     if added_a_root:
         data._root = None
 
 
+    # end
+    pass
 
 
 
 
 
 
 # Utilities
 
 def _write_header(
     file
     ):
+    from emdfile import _PROGRAM_NAME, _USER_NAME
     file.attrs.create("emd_group_type",'file')
     file.attrs.create("version_major",1)
     file.attrs.create("version_minor",0)
     #file.attrs.create("version_release",0)
-    #file.attrs.create("UUID",UUID)
-    #file.attrs.create("authoring_program",PROGRAM_NAME)
-    #file.attrs.create("authoring_user",USER_NAME)
+    file.attrs.create("UUID",str(uuid4()))
+    file.attrs.create("authoring_program",_PROGRAM_NAME)
+    file.attrs.create("authoring_user",_USER_NAME)
 
 
 def _write_from_root(
     file,
     root,
     data,
     tree
@@ -463,15 +762,18 @@
     Accepts a file rootgroup and a runtime `treepath` string.
     If the treepath is not in the file, returns False.
     If the treepath is in the file, returns (grp, True) and
     if the treepath is one node beyond the file, returns (grp, False),
     where `grp` is the final h5py Group on treepath in the file tree.
     """
     grp_names = treepath.split('/')
-    grp_names.remove('')
+    try:
+        grp_names.remove('')
+    except ValueError:
+        pass
     group = rootgroup
     for i,name in enumerate(grp_names):
         if name not in group.keys():
             # catch for being one node beyond
             if i == len(grp_names)-1:
                 return group, False
             return False
```

### Comparing `emdfile-0.0.2/src/emdfile/classes/array.py` & `emdfile-0.0.4/src/emdfile/classes/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,14 +291,17 @@
     def get_dim(self,n):
         """ Return the n'th dim vector
         """
         assert(isinstance(n,(int,np.integer))), f"Can't retrieve the {n}th dim vector - {n} must be an integer, not type {type(n)}."
         assert(n < len(self._dims)), f"Can't retrieve the {n}th dim vector - {n} must be <= {len(self._dims)-1}"
         return self._dims[n]
 
+    # alias
+    dim = get_dim
+
     def set_dim(
         self,
         n:int,
         dim:Union[list,np.ndarray],
         units:Optional[str]=None,
         name:Optional[str]=None
         ):
@@ -442,37 +445,37 @@
     # Shape properties
 
     @property
     def shape(self):
         if not self.is_stack:
             return self.data.shape
         else:
-            return self.data.shape[:-1]
+            return self.data.shape[1:]
 
     @property
     def depth(self):
         if not self.is_stack:
             return 0
         else:
-            return self.data.shape[-1]
+            return self.data.shape[0]
 
     @property
     def rank(self):
         if not self.is_stack:
             return self.data.ndim
         else:
             return self.data.ndim - 1
 
 
     ## Slicing
 
     def get_slice(self,label,name=None):
         idx = self.slicelabels._dict[label]
         return Array(
-            data = self.data[..., idx],
+            data = self.data[idx],
             name = name if name is not None else self.name+'_'+label,
             units = self.units,
             dims = self.dims,
             dim_units = self.dim_units,
             dim_names = self.dim_names
         )
 
@@ -569,23 +572,22 @@
             )
             dset.attrs.create('name',name)
             dset.attrs.create('units',units)
 
         # Add stack dim vector, if present
         if self.is_stack:
             n = self.rank
-            name = '_labels_'
             dim = [s.encode('utf-8') for s in self.slicelabels]
 
             # write
             dset = grp.create_dataset(
                 f"dim{n}",
                 data = dim
             )
-            dset.attrs.create('name',name)
+            dset.attrs.create('name','_labels_')
 
         # Return
         return grp
```

### Comparing `emdfile-0.0.2/src/emdfile/classes/custom.py` & `emdfile-0.0.4/src/emdfile/classes/custom.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.2/src/emdfile/classes/metadata.py` & `emdfile-0.0.4/src/emdfile/classes/metadata.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.2/src/emdfile/classes/pointlist.py` & `emdfile-0.0.4/src/emdfile/classes/pointlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,16 @@
     ## Add, remove, sort data
 
     def add(self, data):
         """
         Appends a numpy structured array. Its dtypes must agree with the existing data.
         """
         assert self.dtype == data.dtype, "Error: dtypes must agree"
+        if isinstance(data,PointList):
+            data = data.data
         self.data = np.append(self.data, data)
 
     def remove(self, mask):
         """ Removes points wherever mask==True
         """
         assert np.atleast_1d(mask).shape[0] == self.length, "deletemask must be same length as the data"
         inds = mask.nonzero()[0]
```

### Comparing `emdfile-0.0.2/src/emdfile/classes/pointlistarray.py` & `emdfile-0.0.4/src/emdfile/classes/pointlistarray.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.2/src/emdfile/classes/tree.py` & `emdfile-0.0.4/src/emdfile/classes/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
     # displays top level contents of the node
     def __repr__(self):
         space = ' '*len(self.__class__.__name__)+'  '
         string = f"{self.__class__.__name__}( A Node called '{self.name}', containing the following top-level objects in its tree:"
         string += "\n"
         for k,v in self._branch.items():
-            string += "\n"+space+f"    {k} \t\t ({v.__class__.__name__})"
+            string += "\n"+space+f"    {k.ljust(24,' ')} \t ({v.__class__.__name__})"
         string += "\n)"
         return string
 
 
 
     # tree methods
 
@@ -236,20 +236,39 @@
         # find upstream and root nodes
         old_root = self.root
         node_list = self._treepath.split('/')
         this_node = node_list.pop()
         treepath = '/'.join(node_list)
         upstream_node = self.get_from_tree(treepath)
 
-        # remove connection from upstream to this node
-        del(upstream_node._branch[this_node])
 
-        # add to a new tree
-        self._root = None
-        node.add_to_tree(self)
+        # if grafting from a non-root node
+        if this_node != '':
+
+            # remove connection from upstream to this node
+            del(upstream_node._branch[this_node])
+
+            # add to a new tree
+            self._root = None
+            node.add_to_tree(self)
+
+        # if grafting from a root node
+        else:
+
+            # add objects one by one
+            keys = list(upstream_node._branch.keys())
+            for k in keys:
+                n = upstream_node.tree(k)
+                n._root = None
+                node.add_to_tree(n)
+                # remove upstream connections
+                del(upstream_node._branch[k])
+
+#                upstream_node.tree(k).graft(node, merge_metadata=False)
+
 
         # add old root metadata to this node
         assert(merge_metadata in [True,False,'copy'])
         if merge_metadata is False:
             # add no root metadata
             pass
         elif merge_metadata is True:
@@ -277,15 +296,15 @@
                 metadata to the new root; if False adds no metadata to the new
                 root; if 'copy' adds copies of all metadata from the old root to
                 the new root.
 
         Returns:
             (Node) the new root node
         """
-        new_root = Root(name=self.name)
+        new_root = Root( name=self.root.name+'_cut_'+self.name)
         return self.graft(new_root,merge_metadata=root_metadata)
 
 
     def tree(
         self,
         arg = None,
         **kwargs,
@@ -309,14 +328,15 @@
 
         The show, add, and get methods can be accessed directly with
 
             >>> .tree(arg)
 
         for an arg of the appropriate type (bool, Node, and string).
         """
+
         # if `arg` is passed, choose behavior from its type
         if isinstance(arg,bool):
             self.show_tree(root=arg)
             return
         elif isinstance(arg,Node):
             self.add_to_tree(arg)
             return
@@ -629,16 +649,14 @@
         return self._dict.keys()
     def items(self):
         return self._dict.items()
 
 
 
     # print the full tree contents to screen
-    # TODO - this seems to have a bug when I run obj.tree()...
-    # TODO: unclear if this bug still exists - need to check
     def print(self):
         """
         Prints the tree contents to screen.
         """
         print('/')
         self._print_tree_to_screen(self)
         pass
@@ -649,20 +667,19 @@
         """
         if tablevel not in linelevels:
             linelevels.append(tablevel)
         keys = [k for k in tree.keys()]
         N = len(keys)
         for i,k in enumerate(keys):
             string = ''
-            string += '|' if 0 in linelevels else ''
+            string += '|' if 0 in linelevels else ' '
             for idx in range(tablevel):
-                l = '|' if idx+1 in linelevels else ''
-                string += '\t'+l
-            #print(string)
-            print(string+'--'+k)
+                l = '|' if idx+1 in linelevels else ' '
+                string += '   '+l
+            print(string+'---'+k)
             if i == N-1:
                 linelevels.remove(tablevel)
             try:
                 tree._print_tree_to_screen(
                     tree[k]._branch,
                     tablevel=tablevel+1,
                     linelevels=linelevels)
```

### Comparing `emdfile-0.0.2/test/clear_h5_files.py` & `emdfile-0.0.4/test/clear_h5_files.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.2/test/test_base_classes.py` & `emdfile-0.0.4/test/test_base_classes.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.2/test/test_emd.py` & `emdfile-0.0.4/test/test_emd.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,28 +102,26 @@
     def test_array(self):
         """ Save then read as array, and compare its contents before/after
         """
         assert(isinstance(self.array,Array))
         # save and read
         print(path_h5)
         save(path_h5,self.array)
-        root = read(path_h5)
-        new_array = root.tree('array')
+        new_array = read(path_h5)
         # check it's the same
         assert(isinstance(new_array,Array))
         assert(array_equal(self.array.data,new_array.data))
 
     def test_array2(self):
         """ Save then read as array, and compare its contents before/after
         """
         assert(isinstance(self.array2,Array))
         # save and read
         save(path_h5,self.array2)
-        root = read(path_h5)
-        new_array = root.tree('array2')
+        new_array = read(path_h5)
         # check it's the same
         assert(isinstance(new_array,Array))
         assert(array_equal(self.array2.data,new_array.data))
         # check that metadata passed through
         assert(self.array2.name == new_array.name)
         assert(self.array2.units == new_array.units)
         assert(array_equal(self.array2.dims[0],new_array.dims[0]))
```

### Comparing `emdfile-0.0.2/test/test_tree.py` & `emdfile-0.0.4/test/test_tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -431,17 +431,16 @@
         """
         # Load data
         loaded_data = read(
             single_node_path
         )
 
         # Does the tree look as it should?
-        assert(isinstance(loaded_data,Root))
-        lar = loaded_data.tree('array')
-        assert(isinstance(lar,Array))
+        assert(isinstance(loaded_data,Array))
+        lar = loaded_data
 
         # Did the root metadata load correctly
         lmd1 = lar.root.metadata['metadata_root']
         lmd2 = lar.root.metadata['metadata_root2']
         assert(lmd1 is not self.md_root)
         assert(lmd2 is not self.md_root2)
         assert(lmd1._params == self.md_root._params)
@@ -461,23 +460,22 @@
 
 
     def test_single_node_io_emdpath(self):
         """ Should contain a single array 'array' inside a single root 'root',
         and 'array' should match self.ar
         """
         # Load data
-        loaded_data = read(
+        lar = read(
             single_node_path,
             emdpath = '/root/array'
         )
 
         # Does the tree look as it should?
-        assert(isinstance(loaded_data,Root))
-        lar = loaded_data.tree('array')
         assert(isinstance(lar,Array))
+        assert(isinstance(lar.root,Root))
 
         # Did the root metadata load correctly
         lmd1 = lar.root.metadata['metadata_root']
         lmd2 = lar.root.metadata['metadata_root2']
         assert(lmd1 is not self.md_root)
         assert(lmd2 is not self.md_root2)
         assert(lmd1._params == self.md_root._params)
@@ -501,18 +499,17 @@
         """
         # Load data
         loaded_data = read(
             unrooted_node_path
         )
 
         # Does the tree look as it should?
-        assert(isinstance(loaded_data,Root))
+        assert(isinstance(loaded_data,Array))
         assert(loaded_data.name == 'unrooted_array')
-        lar = loaded_data.tree('unrooted_array')
-        assert(isinstance(lar,Array))
+        lar = loaded_data
 
         # Did the root metadata load correctly
         assert(len(lar.root.metadata.keys())==0)
 
         # Did the array load correctly?
         assert(lar is not self.ar_unrooted)
         assert(lar.name == self.ar_unrooted.name)
@@ -622,58 +619,56 @@
         loaded_data = read(
             whole_tree_path,
             emdpath = '/root/array/pointlistarray',
             tree = False
         )
 
         # Does the tree look as it should?
-        assert(isinstance(loaded_data,Root))
-        assert(loaded_data.name == 'root')
+        assert(isinstance(loaded_data,PointListArray))
+        assert(loaded_data.name == 'pointlistarray')
 
-        lmd_root = loaded_data.metadata['metadata_root']
-        lmd_root2 = loaded_data.metadata['metadata_root2']
-        lpla = loaded_data.tree('pointlistarray')
+        lmd_root = loaded_data.root.metadata['metadata_root']
+        lmd_root2 = loaded_data.root.metadata['metadata_root2']
 
         # Check types
         assert(isinstance(lmd_root,Metadata))
         assert(isinstance(lmd_root2,Metadata))
-        assert(isinstance(lpla,PointListArray))
 
         # New objects are distinct from old objects
         assert(lmd_root is not self.md_root)
         assert(lmd_root2 is not self.md_root2)
-        assert(lpla is not self.pla)
+        assert(loaded_data is not self.pla)
 
         # New objects carry identical data to old objects
         assert(lmd_root._params == self.md_root._params)
         assert(lmd_root2._params == self.md_root2._params)
-        for x in range(lpla.shape[0]):
-            for y in range(lpla.shape[1]):
-                assert(self.pointlist_equal(lpla[x,y], self.pla[x,y]))
+        for x in range(loaded_data.shape[0]):
+            for y in range(loaded_data.shape[1]):
+                assert(self.pointlist_equal(loaded_data[x,y], self.pla[x,y]))
 
         pass
 
 
     def test_subtree_io(self):
         """ Tree should be root/pointlist3/pointlist4, plus
         metadata at root and pl4
         """
         # Load data
         loaded_data = read(
             subtree_path
         )
 
         # Does the tree look as it should?
-        assert(isinstance(loaded_data,Root))
-        assert(loaded_data.name == 'root')
+        assert(isinstance(loaded_data,PointList))
+        assert(loaded_data.name == 'pointlist3')
 
-        lmd_root = loaded_data.metadata['metadata_root']
-        lmd_root2 = loaded_data.metadata['metadata_root2']
-        lpl3 = loaded_data.tree('/pointlist3')
-        lpl4 = loaded_data.tree('pointlist3/pointlist4')
+        lmd_root = loaded_data.root.metadata['metadata_root']
+        lmd_root2 = loaded_data.root.metadata['metadata_root2']
+        lpl3 = loaded_data
+        lpl4 = loaded_data.tree('pointlist4')
         lmd3 = lpl4.metadata['metadata3']
 
         # Check types
         assert(isinstance(lmd_root,Metadata))
         assert(isinstance(lmd_root2,Metadata))
         assert(isinstance(lpl3,PointList))
         assert(isinstance(lpl4,PointList))
@@ -703,26 +698,25 @@
         """
         # Load data
         loaded_data = read(
             subtree_noroot_path
         )
 
         # Does the tree look as it should?
-        assert(isinstance(loaded_data,Root))
-        assert(loaded_data.name == 'root')
+        assert(isinstance(loaded_data,PointList))
+        assert(loaded_data.name == 'pointlist4')
 
-        lmd_root = loaded_data.metadata['metadata_root']
-        lmd_root2 = loaded_data.metadata['metadata_root2']
-        lpl4 = loaded_data.tree('pointlist4')
+        lmd_root = loaded_data.root.metadata['metadata_root']
+        lmd_root2 = loaded_data.root.metadata['metadata_root2']
+        lpl4 = loaded_data
         lmd3 = lpl4.metadata['metadata3']
 
         # Check types
         assert(isinstance(lmd_root,Metadata))
         assert(isinstance(lmd_root2,Metadata))
-        assert(isinstance(lpl4,PointList))
         assert(isinstance(lmd3,Metadata))
 
         # New objects are distinct from old objects
         assert(lmd_root is not self.md_root)
         assert(lmd_root2 is not self.md_root2)
         assert(lpl4 is not self.pl4)
         assert(lmd3 is not self.md3)
@@ -744,27 +738,27 @@
         """
         # Load data
         loaded_data = read(
             subtree_append_to_path
         )
 
         # Does the tree look as it should?
-        assert(isinstance(loaded_data,Root))
-        assert(loaded_data.name == 'root')
+        assert(isinstance(loaded_data,Array))
+        assert(loaded_data.name == 'array')
 
-        lmd_root = loaded_data.metadata['metadata_root']
-        lmd_root2 = loaded_data.metadata['metadata_root2']
-        lar = loaded_data.tree('array')
+        lmd_root = loaded_data.root.metadata['metadata_root']
+        lmd_root2 = loaded_data.root.metadata['metadata_root2']
+        lar = loaded_data
         lmd = lar.metadata['metadata']
         lmd2 = lar.metadata['metadata2']
-        lpl5 = loaded_data.tree('array/pointlist5')
+        lpl5 = loaded_data.tree('pointlist5')
 
         # Ensure the data that shouldn't be here, isn't
-        assert('pointlist3' not in loaded_data._branch.keys())
-        assert('array' in loaded_data._branch.keys())
+        assert('pointlist3' not in loaded_data.root._branch.keys())
+        assert('array' in loaded_data.root._branch.keys())
 
         # Check types
         assert(isinstance(lmd_root,Metadata))
         assert(isinstance(lmd_root2,Metadata))
         assert(isinstance(lar,Array))
         assert(isinstance(lmd,Metadata))
         assert(isinstance(lmd2,Metadata))
@@ -800,44 +794,42 @@
         """
         # Load data
         loaded_data = read(
             subtree_append_over_path
         )
 
         # Does the tree look as it should?
-        assert(isinstance(loaded_data,Root))
-        assert(loaded_data.name == 'root')
+        assert(isinstance(loaded_data,Array))
+        assert(loaded_data.name == 'array')
 
-        lmd_root = loaded_data.metadata['metadata_root']
-        lmd_root2 = loaded_data.metadata['metadata_root2']
-        lar = loaded_data.tree('array')
-        assert(len(lar.metadata)==0)
-        lpl5 = loaded_data.tree('array/pointlist5')
+        lmd_root = loaded_data.root.metadata['metadata_root']
+        lmd_root2 = loaded_data.root.metadata['metadata_root2']
+        assert(len(loaded_data.metadata)==0)
+        lpl5 = loaded_data.tree('pointlist5')
 
         # Ensure the data that shouldn't be here, isn't
-        assert('pointlist3' not in loaded_data._branch.keys())
-        assert('array' in loaded_data._branch.keys())
+        assert('pointlist3' not in loaded_data.root._branch.keys())
+        assert('array' in loaded_data.root._branch.keys())
 
         # Check types
         assert(isinstance(lmd_root,Metadata))
         assert(isinstance(lmd_root2,Metadata))
-        assert(isinstance(lar,Array))
         assert(isinstance(lpl5,PointList))
 
         # New objects are distinct from old objects
         assert(lmd_root is not self.md_root)
         assert(lmd_root2 is not self.md_root2)
-        assert(lar is not self.ar2)
+        assert(loaded_data is not self.ar2)
         assert(lpl5 is not self.pl5)
 
         # New objects carry identical data to old objects
         assert(lmd_root._params == self.md_root._params)
         assert(lmd_root2._params == self.md_root2._params)
-        assert(array_equal(lar.data, self.ar2.data))    # ensure we did overwrite
-        assert(not(array_equal(lar.data, self.ar.data)))
+        assert(array_equal(loaded_data.data, self.ar2.data))    # ensure we did overwrite
+        assert(not(array_equal(loaded_data.data, self.ar.data)))
         assert(self.pointlist_equal(lpl5, self.pl5))
 
         pass
 
 
 
 
@@ -887,15 +879,15 @@
     def _write_h5_subtree_noroot(self):
         """
         Write a subtree tree to file without it's root dataset
         """
         save(
             subtree_noroot_path,
             self.pl3,
-            tree = "noroot"
+            tree = None
         )
 
     def _append_to_h5(self):
         """
         Append to an existing h5 file
         """
         save(
```

### Comparing `emdfile-0.0.2/LICENSE` & `emdfile-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.2/README.md` & `emdfile-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,32 +11,35 @@
 filetree-like representations of data and metadata.
 
 
 ## Installation
 
 Run
 
->>> pip install emdfile
+> pip install emdfile
 
 Or, to install from source code, clone this repository and from the
 distribution level directory (i.e. where pyproject.toml lives) run
 
->>> pip install .
+> pip install .
 
 
 
 ## Examples and syntax
 
+For a narrative introduction, see
+[tutorials/emd_narrative_intro.md](tutorials/emd_narrative_intro.md).
+
 For an example, see
 [tutorials/emd_intro_example.ipynb](./tutorials/emd_intro_example.ipynb).
 
 For an walkthrough of the syntax, see
 [tutorials/emd_package_walkthrough.ipynb](./tutorials/emd_package_walkthrough.ipynb).
 
-For an example of a downstream Python package with it's IO build on emdfile, see
+For an example of a downstream Python package using emdfile for IO, see
 [tutorials/test_custom_class.py](./tutorials/test_custom_class.py) and
 [tutorials/sample_custom_class_module](./tutorials/sample_custom_class_module).
```

### Comparing `emdfile-0.0.2/pyproject.toml` & `emdfile-0.0.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "emdfile"
-version = "0.0.2"
+dynamic = ["version"]
 authors = [
-    { name="Ben Savitzky", email="ben.savitzky@gmail.com" }
+    { name="Benjamin H. Savitzky", email="ben.savitzky@gmail.com" }
 ]
 descriptor = "An HDF5 / Python interface for scientific data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -18,11 +18,15 @@
 dependencies = [
     'h5py >= 3.2.0',
     'tqdm >= 4.46.1',
     'numpy',
     'scipy'
 ]
 
+[tool.hatch.version]
+path = "src/emdfile/version.py"
+#validate-bump = false
+
 [project.urls]
 "github" = "https://github.com/py4dstem/emdfile"
 "emdatasets" = "https://emdatasets.com/format/"
```

### Comparing `emdfile-0.0.2/PKG-INFO` & `emdfile-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: emdfile
-Version: 0.0.2
+Version: 0.0.4
 Project-URL: github, https://github.com/py4dstem/emdfile
 Project-URL: emdatasets, https://emdatasets.com/format/
-Author-email: Ben Savitzky <ben.savitzky@gmail.com>
+Author-email: "Benjamin H. Savitzky" <ben.savitzky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: h5py>=3.2.0
 Requires-Dist: numpy
 Requires-Dist: scipy
@@ -27,32 +27,35 @@
 filetree-like representations of data and metadata.
 
 
 ## Installation
 
 Run
 
->>> pip install emdfile
+> pip install emdfile
 
 Or, to install from source code, clone this repository and from the
 distribution level directory (i.e. where pyproject.toml lives) run
 
->>> pip install .
+> pip install .
 
 
 
 ## Examples and syntax
 
+For a narrative introduction, see
+[tutorials/emd_narrative_intro.md](tutorials/emd_narrative_intro.md).
+
 For an example, see
 [tutorials/emd_intro_example.ipynb](./tutorials/emd_intro_example.ipynb).
 
 For an walkthrough of the syntax, see
 [tutorials/emd_package_walkthrough.ipynb](./tutorials/emd_package_walkthrough.ipynb).
 
-For an example of a downstream Python package with it's IO build on emdfile, see
+For an example of a downstream Python package using emdfile for IO, see
 [tutorials/test_custom_class.py](./tutorials/test_custom_class.py) and
 [tutorials/sample_custom_class_module](./tutorials/sample_custom_class_module).
```

