# Comparing `tmp/xyz_py-5.2.1.tar.gz` & `tmp/xyz_py-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyz_py-5.2.1.tar", last modified: Tue Mar 21 21:06:47 2023, max compression
+gzip compressed data, was "xyz_py-5.3.0.tar", last modified: Thu Apr 20 17:15:06 2023, max compression
```

## Comparing `xyz_py-5.2.1.tar` & `xyz_py-5.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 21:06:47.217008 xyz_py-5.2.1/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2023-03-21 21:06:21.000000 xyz_py-5.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1303 2023-03-21 21:06:47.217008 xyz_py-5.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-03-21 21:06:21.000000 xyz_py-5.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-03-21 21:06:21.000000 xyz_py-5.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-21 21:06:47.217008 xyz_py-5.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-03-21 21:06:44.000000 xyz_py-5.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 21:06:47.214008 xyz_py-5.2.1/xyz_py/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-03-21 21:06:21.000000 xyz_py-5.2.1/xyz_py/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7447 2023-03-21 21:06:21.000000 xyz_py-5.2.1/xyz_py/atomic.py
--rw-rw-rw-   0 root         (0) root         (0)     6728 2023-03-21 21:06:21.000000 xyz_py-5.2.1/xyz_py/cli.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-21 21:06:44.000000 xyz_py-5.2.1/xyz_py/version.py
--rw-rw-rw-   0 root         (0) root         (0)    33988 2023-03-21 21:06:21.000000 xyz_py-5.2.1/xyz_py/xyz_py.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 21:06:47.217008 xyz_py-5.2.1/xyz_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1303 2023-03-21 21:06:47.000000 xyz_py-5.2.1/xyz_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-03-21 21:06:47.000000 xyz_py-5.2.1/xyz_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-21 21:06:47.000000 xyz_py-5.2.1/xyz_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-03-21 21:06:47.000000 xyz_py-5.2.1/xyz_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-21 21:06:47.000000 xyz_py-5.2.1/xyz_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-21 21:06:47.000000 xyz_py-5.2.1/xyz_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:15:06.202299 xyz_py-5.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2023-04-20 17:14:29.000000 xyz_py-5.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-20 17:15:06.201299 xyz_py-5.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-20 17:14:29.000000 xyz_py-5.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-20 17:14:29.000000 xyz_py-5.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 17:15:06.202299 xyz_py-5.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-20 17:15:03.000000 xyz_py-5.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:15:06.198299 xyz_py-5.3.0/xyz_py/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-20 17:14:29.000000 xyz_py-5.3.0/xyz_py/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7408 2023-04-20 17:14:29.000000 xyz_py-5.3.0/xyz_py/atomic.py
+-rw-rw-rw-   0 root         (0) root         (0)     8316 2023-04-20 17:14:29.000000 xyz_py-5.3.0/xyz_py/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-20 17:15:03.000000 xyz_py-5.3.0/xyz_py/version.py
+-rw-rw-rw-   0 root         (0) root         (0)    37690 2023-04-20 17:14:29.000000 xyz_py-5.3.0/xyz_py/xyz_py.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:15:06.201299 xyz_py-5.3.0/xyz_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-20 17:15:06.000000 xyz_py-5.3.0/xyz_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-20 17:15:06.000000 xyz_py-5.3.0/xyz_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 17:15:06.000000 xyz_py-5.3.0/xyz_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-20 17:15:06.000000 xyz_py-5.3.0/xyz_py.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-20 17:15:06.000000 xyz_py-5.3.0/xyz_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-20 17:15:06.000000 xyz_py-5.3.0/xyz_py.egg-info/top_level.txt
```

### Comparing `xyz_py-5.2.1/LICENSE` & `xyz_py-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xyz_py-5.2.1/PKG-INFO` & `xyz_py-5.3.0/xyz_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xyz_py
-Version: 5.2.1
+Name: xyz-py
+Version: 5.3.0
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xyz_py-5.2.1/README.md` & `xyz_py-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `xyz_py-5.2.1/setup.py` & `xyz_py-5.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "5.2.1"
+__version__ = "5.3.0"
 
 setuptools.setup(
     name="xyz_py",
     version=__version__,
     author="Jon Kragskow",
     author_email="jonkragskow@gmail.com",
     description="A package for manipulating xyz files and chemical structures",
```

### Comparing `xyz_py-5.2.1/xyz_py/atomic.py` & `xyz_py-5.3.0/xyz_py/atomic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 
-from pyparsing import dbl_quoted_string
-
 
 s_block_col_1 = ["Li", "Na", "K", "Rb", "Cs", "Fr"]
 s_block_col_2 = ["Be", "Mg", "Ca", "Sr", "Ba", "Ra"]
 
 s_block = s_block_col_1 + s_block_col_2
 
 p_block_row_1 = ["He"]
@@ -105,15 +103,16 @@
 }
 
 num_lab = dict(zip(lab_num.values(), lab_num.keys()))
 
 # Atomic radii
 # also called vdW radii
 # https://www.rsc.org/periodic-table/
-# CRC Handbook of Chemistry and Physics, 97th Ed.; Haynes, W. M. Ed. CRC Press/Taylor and Francis: Boca Raton, 2016 (accessed 2022-10-01).
+# CRC Handbook of Chemistry and Physics, 97th Ed.; Haynes, W. M. Ed. CRC
+# Press/Taylor and Francis: Boca Raton, 2016 (accessed 2022-10-01).
 atomic_radii = {
     "H": 1.1, "He": 1.4, "Li": 1.82, "Be": 1.53, "B": 1.92, "C": 1.7,
     "N": 1.55, "O": 1.52, "F": 1.47, "Ne": 1.54, "Na": 2.27, "Mg": 1.73,
     "Al": 1.84, "Si": 2.1, "P": 1.8, "S": 1.8, "Cl": 1.75, "Ar": 1.88,
     "K": 2.75, "Ca": 2.31, "Sc": 2.15, "Ti": 2.11, "V": 2.07, "Cr": 2.06,
     "Mn": 2.05, "Fe": 2.04, "Co": 2.0, "Ni": 1.97, "Cu": 1.96, "Zn": 2.01,
     "Ga": 1.87, "Ge": 2.11, "As": 1.85, "Se": 1.9, "Br": 1.85, "Kr": 2.02,
```

### Comparing `xyz_py-5.2.1/xyz_py/xyz_py.py` & `xyz_py-5.3.0/xyz_py/xyz_py.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 #! /usr/bin/env python3
 
-"""
+'''
 This is the main part of xyz_py
-"""
+'''
 
 import numpy as np
 import numpy.linalg as la
 from ase import neighborlist, Atoms
 from ase.geometry.analysis import Analysis
 import copy
 import re
 import scipy.optimize as spo
 import sys
 from collections import defaultdict
 import deprecation
+
 from . import version
 from . import atomic
 
 __version__ = version.__version__
 
 
 def load_xyz(f_name: str, atomic_numbers: bool = False,
              add_indices: bool = False, capitalise: bool = True):
-    """
+    '''
     Load labels and coordinates from a .xyz file
 
     Parameters
     ----------
     f_name : str
         File name
     atomic_numbers : bool, default False
@@ -39,15 +40,15 @@
 
     Returns
     -------
     list
         atomic labels
     np.ndarray
         (n_atoms,3) array containing xyz coordinates of each atom
-    """
+    '''
 
     if atomic_numbers:
         _numbers = np.loadtxt(
             f_name, skiprows=2, usecols=0, dtype=int, ndmin=1
         )
         _labels = num_to_lab(_numbers.tolist())
     else:
@@ -55,26 +56,26 @@
         _labels = _labels.tolist()
 
     # Set labels as capitals
     if capitalise:
         _labels = [lab.capitalize() for lab in _labels]
 
     if add_indices:
-        _labels = remove_numbers(_labels)
-        _labels = add_numbers(_labels)
+        _labels = remove_label_indices(_labels)
+        _labels = add_label_indices(_labels)
 
     _coords = np.loadtxt(f_name, skiprows=2, usecols=(1, 2, 3), ndmin=2)
 
     return _labels, _coords
 
 
 def save_xyz(f_name: str, labels: list, coords: np.ndarray,
              with_numbers: bool = False, verbose: bool = True,
              mask: list = [], atomic_numbers: bool = False):
-    """
+    '''
     Save an xyz file containing labels and coordinates
 
     Parameters
     ----------
     f_name : str
         File name
     labels : list
@@ -90,88 +91,66 @@
         atoms to print
     atomic_numbers : bool, default False
         If true, will save xyz file with atomic numbers
 
     Returns
     -------
     None
-    """
+    '''
 
     # Option to have numbers added
     if with_numbers:
         # Remove and re-add numbers to be safe
-        _labels = remove_numbers(labels)
-        _labels = add_numbers(_labels)
+        _labels = remove_label_indices(labels)
+        _labels = add_label_indices(_labels)
     else:
         _labels = labels
 
     # Set up masks
     if mask:
         coords = np.delete(coords, mask, axis=0)
         _labels = np.delete(_labels, mask, axis=0).tolist()
 
     n_atoms = len(_labels)
 
     if atomic_numbers:
-        _labels = remove_numbers(_labels)
+        _labels = remove_label_indices(_labels)
         _numbers = lab_to_num(_labels)
         _identifier = _numbers
     else:
         _identifier = _labels
 
     with open(f_name, 'w') as f:
-        f.write("{:d}\n\n".format(n_atoms))
+        f.write('{:d}\n\n'.format(n_atoms))
         for it, (ident, trio) in enumerate(zip(_identifier, coords)):
-            f.write("{:5} {:15.7f} {:15.7f} {:15.7f} \n".format(ident, *trio))
+            f.write('{:5} {:15.7f} {:15.7f} {:15.7f} \n'.format(ident, *trio))
 
     if verbose:
-        print("New xyz file written to {}".format(f_name))
+        print('New xyz file written to {}'.format(f_name))
 
     return
 
 
-@deprecation.deprecated(
-    deprecated_in="4.2.0", removed_in="5.1.0", current_version=__version__,
-    details="Use the remove_label_indices function instead"
-)
-def remove_numbers(labels):
-    """
-    Remove numbers from a list of atomic labels
-
-    Parameters
-    ----------
-    labels : list
-        atomic labels
-
-    Returns
-    -------
-    list
-        atomic labels without numbers
-    """
-
-    return remove_label_indices(labels)
-
-
 def remove_label_indices(labels):
-    """
+    '''
     Remove label indexing from atomic symbols
     indexing is either numbers or numbers followed by letters:
     e.g. H1, H2, H3
     or H1a, H2a, H3a
 
     Parameters
     ----------
     labels : list
         atomic labels
 
     Returns
     -------
     list
         atomic labels without indexing
-    """
+    '''
 
     labels_nn = []
     for label in labels:
         no_digits = []
         for i in label:
             if not i.isdigit():
                 no_digits.append(i)
@@ -179,42 +158,16 @@
                 break
         result = ''.join(no_digits)
         labels_nn.append(result)
 
     return labels_nn
 
 
-@deprecation.deprecated(
-    deprecated_in="4.2.0", removed_in="5.1.0", current_version=__version__,
-    details="Use the add_label_indices function instead"
-)
-def add_numbers(labels, style='per_element'):
-    """
-    Add numbers to a list of atomic labels
-
-    Parameters
-    ----------
-    labels : list
-        atomic labels
-    style : str, optional
-        {'per_element', 'sequential'}
-            'per_element' : Number by element e.g. Dy1, Dy2, N1, N2, etc.
-            'sequential' : Number the atoms 1->N regardless of element
-
-    Returns
-    -------
-    list
-        atomic labels with numbers
-    """
-
-    return add_label_indices(labels, style=style)
-
-
 def add_label_indices(labels, style='per_element', start_index=1):
-    """
+    '''
     Add label indexing to atomic symbols - either element or per atom.
 
     Parameters
     ----------
     labels : list
         atomic labels
     style : str, optional
@@ -224,197 +177,213 @@
     start_index : int
         integer at which indexing will start
 
     Returns
     -------
     list
         atomic labels with indexing
-    """
+    '''
 
     # remove numbers just in case
-    labels_nn = remove_numbers(labels)
+    labels_nn = remove_label_indices(labels)
 
     # Just number the atoms 1->N regardless of element
     if style == 'sequential':
-        labels_wn = ['{}{:d}'.format(lab, it+start_index)
+        labels_wn = ['{}{:d}'.format(lab, it + start_index)
                      for (it, lab) in enumerate(labels)]
 
     # Index by element Dy1, Dy2, N1, N2, etc.
     if style == 'per_element':
         # Get list of unique elements
         atoms = set(labels_nn)
         # Create dict to keep track of index of current atom of each element
         atom_count = {atom: start_index for atom in atoms}
         # Create labelled list of elements
         labels_wn = []
+        
         for lab in labels_nn:
             # Index according to dictionary
-            labels_wn.append("{}{:d}".format(lab, atom_count[lab]))
+            labels_wn.append('{}{:d}'.format(lab, atom_count[lab]))
             # Then add one to dictionary
             atom_count[lab] += 1
 
     return labels_wn
 
 
 def count_n_atoms(form_str):
-    """
+    '''
     Count number of atoms in a chemical formula
 
     Parameters
     ----------
     form_str : str
         chemical formula string
 
     Returns
     -------
     int
         number of atoms in chemical formula
-    """
+    '''
 
     form_dict = formstr_to_formdict(form_str)
 
     n_atoms = sum(form_dict.values())
 
     return n_atoms
 
 
 def index_elements(labels, shift=0):
-    """
+    '''
     Return dictionary of element (keys) and indices (values) from list
     of labels
 
     Parameters
     ----------
     labels : list
         atomic labels
     shift : int, optional
         additive shift to apply to all indices
 
     Returns
     -------
     dict
         element (keys) and indices (values)
-    """
+    '''
 
-    labels_nn = remove_numbers(labels)
+    labels_nn = remove_label_indices(labels)
 
     ele_index = {}
 
     for it, lab in enumerate(labels_nn):
         try:
-            ele_index[lab].append(it+shift)
+            ele_index[lab].append(it + shift)
         except KeyError:
-            ele_index[lab] = [it+shift]
+            ele_index[lab] = [it + shift]
 
     return ele_index
 
 
 def count_elements(labels):
-    """
+    '''
     Count number of each element in a list of elements
 
     Parameters
     ----------
     labels : list
         atomic labels
     Returns
     -------
     dict
         dictionary of elements (keys) and counts (vals)
-    """
+    '''
 
-    labels_nn = remove_numbers(labels)
+    labels_nn = remove_label_indices(labels)
 
     ele_count = {}
 
     for lab in labels_nn:
         try:
             ele_count[lab] += 1
         except KeyError:
             ele_count[lab] = 1
 
     return ele_count
 
 
 def get_formula(labels):
-    """
+    '''
     Generates empirical formula in alphabetical order given a list of labels
 
     Parameters
     ----------
     labels : list
         atomic labels
     Returns
     -------
     str
         Empirical formula in alphabetical order
-    """
+    '''
 
     formdict = count_elements(labels)
 
     formula = formdict_to_formstr(formdict)
 
     return formula
 
 
 def formstr_to_formdict(form_str):
-    """
+    '''
     Converts formula string into dictionary of {atomic label:quantity} pairs
 
     Parameters
     ----------
     form_string : str
         Chemical formula as string
 
     Returns
     -------
     dict
         dictionary of {atomic label:quantity} pairs
-    """
+    '''
 
     form_dict = {}
     # Thanks stack exchange!
     s = re.sub
-    f = s("[()',]", '', str(eval(s(',?(\d+)', r'*\1,', s('([A-Z][a-z]*)', # noqa
-          r'("\1",),', form_str))))).split()
+    f = s(
+        "[()',]",
+        '',
+        str(
+            eval(
+                s(
+                    r',?(\d+)',
+                    r'*\1,',
+                    s(
+                        '([A-Z][a-z]*)',
+                        r'("\1",),',
+                        form_str
+                    )
+                )
+            )
+        )
+    ).split()
     for c in set(f):
         form_dict[c] = f.count(c)
 
     return form_dict
 
 
 def formdict_to_formstr(form_dict, include_one=False):
-    """
+    '''
     Converts dictionary of {atomic label:quantity} pairs into
     a single formula string in alphabetical order
 
     Parameters
     ----------
     form_dict : dict
         dictionary of {atomic label:quantity} pairs
     include_one : bool, default False
         Include 1 in final chemical formula e.g. C1H4
 
     Returns
     -------
     str
         Chemical formula as string in alphabetical order
-    """
+    '''
 
     # Formula labels and quantities as separate lists with same order
-    form_labels = ["{:s}".format(key) for key in form_dict.keys()]
+    form_labels = ['{:s}'.format(key) for key in form_dict.keys()]
     form_quants = [val for val in form_dict.values()]
 
     # Quantities of each element as a string
     if include_one:
-        form_quants_str = ["{:d}".format(quant)
+        form_quants_str = ['{:d}'.format(quant)
                            for quant in form_quants]
     else:
-        form_quants_str = ["{:d}".format(quant)
-                           if quant > 1 else ""
+        form_quants_str = ['{:d}'.format(quant)
+                           if quant > 1 else ''
                            for quant in form_quants]
 
     # Sort labels in alphabetical order
     order = np.argsort(form_labels).tolist()
     form_labels_o = [form_labels[o] for o in order]
     # Use same ordering for quantities
     form_quants_str_o = [form_quants_str[o] for o in order]
@@ -426,39 +395,39 @@
     # Join strings together into empirical formula
     form_string = ''.join(form_list)
 
     return form_string
 
 
 def contains_metal(form_string):
-    """
+    '''
     Indicates if a metal is found in a chemical formula string
 
     Parameters
     ----------
     form_string : str
         Chemical formula as string
 
     Returns
     -------
     bool
         True if metal found, else False
-    """
+    '''
     metal_found = False
 
     for metal in atomic.metals:
         if metal in form_string:
             metal_found = True
             break
 
     return metal_found
 
 
 def combine_xyz(labels_1, labels_2, coords_1, coords_2):
-    """
+    '''
     Combine two sets of labels and coordinates
 
     Parameters
     ----------
     labels_1 : list
         Atomic labels
     coords_1 : list
@@ -470,27 +439,27 @@
 
     Returns
     -------
     list
         Combined atomic labels
     np.ndarray
         Combined xyz coordinates as (n_atoms, 3) array
-    """
+    '''
 
     # Concatenate labels lists
-    labels = labels_1+labels_2
+    labels = labels_1 + labels_2
 
     # Concatenate coordinate lists
-    coords = coords_1+coords_2
+    coords = coords_1 + coords_2
 
     return labels, coords
 
 
 def get_neighborlist(labels, coords, adjust_cutoff={}):
-    """
+    '''
     Calculate ASE neighbourlist based on covalent radii
 
     Parameters
     ----------
     labels : list
         Atomic labels
     coords : np.ndarray
@@ -498,21 +467,21 @@
     adjust_cutoff : dict, optional
         dictionary of atoms (keys) and new cutoffs (values)
 
     Returns
     -------
     ASE neighbourlist object
         Neighbourlist for system
-    """
+    '''
 
     # Remove labels if present
-    labels_nn = remove_numbers(labels)
+    labels_nn = remove_label_indices(labels)
 
     # Load molecule
-    mol = Atoms("".join(labels_nn), positions=coords)
+    mol = Atoms(''.join(labels_nn), positions=coords)
 
     # Define cutoffs for each atom using atomic radii
     cutoffs = neighborlist.natural_cutoffs(mol)
 
     # Modify cutoff if requested
     if adjust_cutoff:
         for it, label in enumerate(labels_nn):
@@ -529,15 +498,15 @@
     # Update this list by specifying the atomic positions
     neigh_list.update(mol)
 
     return neigh_list
 
 
 def get_adjacency(labels, coords, adjust_cutoff={}):
-    """
+    '''
     Calculate adjacency matrix using ASE based on covalent radii.
 
     Parameters
     ----------
     labels : list
         Atomic labels
     coords : np.ndarray
@@ -550,64 +519,107 @@
         If save true, this name is used for the file containing the adjacency
         matrix
 
     Returns
     -------
     np.array
         Adjacency matrix with same order as labels/coords
-    """
+    '''
 
     # Remove labels if present
-    labels_nn = remove_numbers(labels)
+    labels_nn = remove_label_indices(labels)
 
     # Get ASE neighbourlist object
     neigh_list = get_neighborlist(labels_nn, coords,
                                   adjust_cutoff=adjust_cutoff)
 
     # Create adjacency matrix
     adjacency = neigh_list.get_connectivity_matrix(sparse=False)
 
     return adjacency
 
 
+@deprecation.deprecated(
+    deprecated_in='5.3.0', removed_in='6.3.0', current_version=__version__,
+    details='Use find_bonds instead'
+)
 def get_bonds(labels, coords, neigh_list=None, verbose=True, style='indices'):
-    """
+    '''
     Calculate list of atoms between which there is a bond.
     Using ASE. Only unique bonds are retained.
     e.g. 0-1 and not 1-0
 
     Parameters
     ----------
     labels : list
         Atomic labels
     coords : np.ndarray
-        xyz coordinates as (n_atoms, 3) array
+        xyz coordinates as (n_atoms, 3) array in Angstrom
     neigh_list : ASE neighbourlist object, optional
         neighbourlist of system
     f_name : str, 'bonds.dat'
         filename to save bond list to
     save : bool, default False
         Save bond list to file
     verbose : bool, default True
         Print number of bonds to screen
     style : str, {'indices','labels'}
             indices : Bond list contains atom number
             labels  : Bond list contains atom label
 
     Returns
     -------
-    list
+    list[list[int | str]]
+        list of lists of unique bonds (atom pairs)
+    '''
+
+    bonds, _ = find_bonds(
+        labels, coords, neigh_list=neigh_list, verbose=verbose, style=style
+    )
+
+    return bonds
+
+
+def find_bonds(labels, coords, neigh_list=None, verbose=True, style='indices'):
+    '''
+    Calculate list of atoms between which there is a bond.
+    Using ASE. Only unique bonds are retained.
+    e.g. 0-1 and not 1-0
+
+    Parameters
+    ----------
+    labels : list
+        Atomic labels
+    coords : np.ndarray
+        xyz coordinates as (n_atoms, 3) array in Angstrom
+    neigh_list : ASE neighbourlist object, optional
+        neighbourlist of system
+    f_name : str, 'bonds.dat'
+        filename to save bond list to
+    save : bool, default False
+        Save bond list to file
+    verbose : bool, default True
+        Print number of bonds to screen
+    style : str, {'indices','labels'}
+            indices : Bond list contains atom number
+            labels  : Bond list contains atom label
+
+    Returns
+    -------
+    list[list[int | str]]
         list of lists of unique bonds (atom pairs)
-    """
+    list[float]
+        Bond length in Angstrom
+    '''
 
     # Remove labels if present
-    labels_nn = remove_numbers(labels)
+    labels_nn = remove_label_indices(labels)
 
     # Create molecule object
-    mol = Atoms("".join(labels_nn), positions=coords)
+    mol = Atoms(''.join(labels_nn), positions=coords)
 
     # Get neighbourlist if not provided to function
     if not neigh_list:
         neigh_list = get_neighborlist(labels, coords)
 
     # Get object containing analysis of molecular structure
     ana = Analysis(mol, nl=neigh_list)
@@ -622,41 +634,53 @@
     is_bonded_to = ana.unique_bonds
 
     # Remove weird outer list wrapping the entire thing twice...
     is_bonded_to = is_bonded_to[0]
     # Create list of bonds (atom pairs) by appending lhs of above
     # definition to each element of the rhs
     bonds = []
-    for it, ibt in enumerate(is_bonded_to):
-        for atom in ibt:
-            bonds.append([it, atom])
+    bonds = [
+        [it, atom]
+        for it, ibt in enumerate(is_bonded_to)
+        for atom in ibt
+    ]
 
     # Count bonds
     n_bonds = len(bonds)
 
+    # Calculate actual values
+    values = [
+        ana.get_bond_value(0, bond)
+        for bond in bonds
+    ]
+
     # Set format and convert to atomic labels if requested
-    if style == "labels":
+    if style == 'labels':
         bonds = [
             [labels[atom1], labels[atom2]]
             for atom1, atom2 in bonds
         ]
-    elif style == "indices":
+    elif style == 'indices':
         pass
     else:
-        sys.exit("Unknown style specified")
+        sys.exit('Unknown style specified')
 
     # Print number of bonds to screen
     if verbose:
-        print('{:d}'.format(n_bonds)+' bonds')
+        print('{:d} bonds'.format(n_bonds))
 
-    return bonds
+    return bonds, values
 
 
+@deprecation.deprecated(
+    deprecated_in='5.3.0', removed_in='6.3.0', current_version=__version__,
+    details='Use find_angles instead'
+)
 def get_angles(labels, coords, neigh_list=None, verbose=True, style='indices'):
-    """
+    '''
     Calculate list of atoms between which there is a bond angle.
     Using ASE. Only unique angles are retained.
     e.g. 0-1-2 but not 2-1-0
 
     Parameters
     ----------
     labels : list
@@ -670,26 +694,66 @@
     save : bool, default False
         Save angle list to file
     verbose : bool, default True
         Print number of angles to screen
     style : str, {'indices','labels'}
             indices : Angle list contains atom number
             labels  : Angle list contains atom label
+            values  : Angle list is values in degrees
 
     Returns
     -------
-    list
+    list[list[int | str | float]]
         list of lists of unique angles (atom trios)
-    """
+    '''
+
+    angles, _ = find_angles(
+        labels, coords, neigh_list=neigh_list, verbose=verbose, style=style
+    )
+
+    return angles
+
+
+def find_angles(labels, coords, neigh_list=None, verbose=True,
+                style='indices'):
+    '''
+    Calculate all angles using ASE. Only unique angles are retained.
+    e.g. 0-1-2 but not 2-1-0
+
+    Parameters
+    ----------
+    labels : list
+        Atomic labels
+    coords : np.ndarray
+        xyz coordinates as (n_atoms, 3) array
+    neigh_list : ASE neighbourlist object, optional
+        neighbourlist of system
+    f_name : str, default 'angles.dat'
+        filename to save angle list to
+    save : bool, default False
+        Save angle list to file
+    verbose : bool, default True
+        Print number of angles to screen
+    style : str, {'indices','labels'}
+            indices : Angle labels are atom number
+            labels  : Angle labels are atom label
+
+    Returns
+    -------
+    list[list[int | str]]
+        list of lists of unique angles (atom trios) as labels or indices
+    list[float]
+        Angles in degrees
+    '''
 
     # Remove labels if present
-    labels_nn = remove_numbers(labels)
+    labels_nn = remove_label_indices(labels)
 
     # Create molecule object
-    mol = Atoms("".join(labels_nn), positions=coords)
+    mol = Atoms(''.join(labels_nn), positions=coords)
 
     # Get neighbourlist if not provided to function
     if not neigh_list:
         neigh_list = get_neighborlist(labels, coords)
 
     # Get object containing analysis of molecular structure
     ana = Analysis(mol, nl=neigh_list)
@@ -711,35 +775,45 @@
     for it, ibt in enumerate(is_angled_to):
         for atoms in ibt:
             angles.append([it, *atoms])
 
     # Count angles
     n_angles = len(angles)
 
+    # Calculate actual values
+    values = [
+        ana.get_angle_value(0, angle)
+        for angle in angles
+    ]
+
     # Set format and convert to atomic labels if requested
-    if style == "labels":
+    if style == 'labels':
         angles = [
             [labels[atom1], labels[atom2], labels[atom3]]
             for atom1, atom2, atom3 in angles
         ]
-    elif style == "indices":
+    elif style == 'indices':
         pass
     else:
-        sys.exit("Unknown style specified")
+        sys.exit('Unknown style specified')
 
     # Print number of angles to screen
     if verbose:
-        print('{:d}'.format(n_angles)+' angles')
+        print('{:d} angles'.format(n_angles))
 
-    return angles
+    return angles, values
 
 
+@deprecation.deprecated(
+    deprecated_in='5.3.0', removed_in='6.3.0', current_version=__version__,
+    details='Use find_dihedrals instead'
+)
 def get_dihedrals(labels, coords, neigh_list=None, verbose=True,
                   style='indices'):
-    """
+    '''
     Calculate and list of atoms between which there is a dihedral.
     Using ASE. Only unique dihedrals are retained.
     e.g. 0-1-2-3 but not 3-2-1-0
 
     Parameters
     ----------
     labels : list
@@ -756,23 +830,62 @@
         Print number of dihedrals to screen
     style : str, {'indices','labels'}
             indices : Dihedral list contains atom number
             labels  : Dihedral list contains atom label
 
     Returns
     -------
-    list
+    list[list[int | str]]
         list of lists of unique dihedrals (atom quads)
-    """
+    '''
+    dihedrals, _ = find_dihedrals(
+        labels, coords, neigh_list=neigh_list, verbose=verbose, style=style
+    )
+
+    return dihedrals
+
+
+def find_dihedrals(labels, coords, neigh_list=None, verbose=True,
+                   style='indices'):
+    '''
+    Calculate and list of atoms between which there is a dihedral.
+    Using ASE. Only unique dihedrals are retained.
+    e.g. 0-1-2-3 but not 3-2-1-0
+
+    Parameters
+    ----------
+    labels : list
+        Atomic labels
+    coords : np.ndarray
+        xyz coordinates as (n_atoms, 3) array
+    neigh_list : ASE neighbourlist object, optional
+        neighbourlist of system
+    f_name : str, default 'dihedrals.dat'
+        filename to save angle list to
+    save : bool, default False
+        Save angle list to file
+    verbose : bool, default True
+        Print number of dihedrals to screen
+    style : str, {'indices','labels'}
+            indices : Dihedral list contains atom number
+            labels  : Dihedral list contains atom label
+
+    Returns
+    -------
+    list[list[int | str]]
+        list of lists of unique dihedrals (atom quads)
+    list[float]
+        Dihedral angles in degrees
+    '''
 
     # Remove labels if present
-    labels_nn = remove_numbers(labels)
+    labels_nn = remove_label_indices(labels)
 
     # Create molecule object
-    mol = Atoms("".join(labels_nn), positions=coords)
+    mol = Atoms(''.join(labels_nn), positions=coords)
 
     # Get neighbourlist if not provided to function
     if not neigh_list:
         neigh_list = get_neighborlist(labels, coords)
 
     # Get object containing analysis of molecular structure
     ana = Analysis(mol, nl=neigh_list)
@@ -791,185 +904,191 @@
     # Create list of dihedrals (atom quads) by appending lhs of above
     # definition to each element of the rhs
     dihedrals = []
     for it, ibt in enumerate(is_dihedraled_to):
         for atoms in ibt:
             dihedrals.append([it, *atoms])
 
+    # Calculate actual values
+    values = [
+        ana.get_dihedral_value(0, dihedral)
+        for dihedral in dihedrals
+    ]
+
     # Count dihedrals
     n_dihedrals = len(dihedrals)
 
     # Set format and convert to atomic labels if requested
-    if style == "labels":
+    if style == 'labels':
         dihedrals = [
             [
                 labels[atom1],
                 labels[atom2],
                 labels[atom3],
                 labels[atom4]
             ]
             for atom1, atom2, atom3, atom4 in dihedrals
         ]
-    elif style == "indices":
+    elif style == 'indices':
         pass
     else:
-        sys.exit("Unknown style specified")
+        sys.exit('Unknown style specified')
 
     # Print number of dihedrals to screen
     if verbose:
-        print('{:d}'.format(n_dihedrals)+' dihedrals')
+        print('{:d} dihedrals'.format(n_dihedrals))
 
-    return dihedrals
+    return dihedrals, values
 
 
 def lab_to_num(labels):
-    """
+    '''
     Convert atomic label to atomic number
 
     Parameters
     ----------
-    labels : list
+    labels : list[str]
         Atomic labels
 
     Returns
     -------
-    list
+    list[int]
         Atomic numbers
-    """
+    '''
 
-    labels_nn = remove_numbers(labels)
+    labels_nn = remove_label_indices(labels)
 
     numbers = [atomic.lab_num[lab] for lab in labels_nn]
 
     return numbers
 
 
 def num_to_lab(numbers, numbered=True):
-    """
+    '''
     Convert atomic number to atomic labels
 
     Parameters
     ----------
-    numbers : list
+    numbers : list[int]
         Atomic numbers
     numbered : bool, optional
         Add indexing number to end of atomic labels
 
     Returns
     -------
-    list
+    list[str]
         Atomic labels
-    """
+    '''
 
     labels = [atomic.num_lab[num] for num in numbers]
 
     if numbered:
-        labels_wn = add_numbers(labels)
+        labels_wn = add_label_indices(labels)
     else:
         labels_wn = labels
 
     return labels_wn
 
 
 def reflect_coords(coords):
-    """
+    '''
     Reflect coordinates through xy plane
 
     Parameters
     ----------
     coords : np.ndarray
         xyz coordinates as (n_atoms, 3) array
 
     Returns
     -------
     np.ndarray
         xyz coordinates as (n_atoms, 3) array
 
-    """
+    '''
 
     # Calculate normal to plane
     x = [1, 0, 0]
     y = [0, 1, 0]
     normal = np.cross(x, y)
 
     # Set up transformation matrix
     # https://en.wikipedia.org/wiki/Transformation_matrix#Reflection_2
     trans_mat = np.zeros([3, 3])
 
-    trans_mat[0, 0] = 1. - 2.*normal[0]**2.
-    trans_mat[1, 0] = -2.*normal[0]*normal[1]
-    trans_mat[2, 0] = -2.*normal[0]*normal[2]
-    trans_mat[0, 1] = -2.*normal[0]*normal[1]
-    trans_mat[1, 1] = 1. - 2.*normal[1]**2.
-    trans_mat[2, 1] = -2.*normal[1]*normal[2]
-    trans_mat[0, 2] = -2.*normal[0]*normal[2]
-    trans_mat[1, 2] = -2.*normal[1]*normal[2]
-    trans_mat[2, 2] = 1. - 2.*normal[2]**2.
+    trans_mat[0, 0] = 1. - 2. * normal[0] ** 2.
+    trans_mat[1, 0] = -2. * normal[0] * normal[1]
+    trans_mat[2, 0] = -2. * normal[0] * normal[2]
+    trans_mat[0, 1] = -2. * normal[0] * normal[1]
+    trans_mat[1, 1] = 1. - 2. * normal[1] ** 2.
+    trans_mat[2, 1] = -2. * normal[1] * normal[2]
+    trans_mat[0, 2] = -2. * normal[0] * normal[2]
+    trans_mat[1, 2] = -2. * normal[1] * normal[2]
+    trans_mat[2, 2] = 1. - 2. * normal[2] ** 2.
 
     # Apply operations
     coords = coords @ trans_mat
 
     return coords
 
 
 def find_entities(labels, coords, adjust_cutoff={}):
-    """
+    '''
     Finds formulae of entities given in labels and coords using adjacency
     matrix
 
     Parameters
     ----------
-    labels : list
+    labels : list[str]
         atomic labels
     coords : np.ndarray
         xyz coordinates of each atom as (n_atoms, 3) array
     adjust_cutoff : dict, optional
         dictionary of atoms (keys) and new cutoffs (values) used in generating
         adjacency matrix
 
     Returns
     -------
-    dict
+    dict[str:list[list[int]]]
         keys = molecular formula,
         vals = list of lists, where each list contains the indices of a single
                 occurrence of the `key`, and the indices match the order given
                 in `labels` and `coords`
-    """
+    '''
 
     # Remove label numbers if present
-    labels_nn = remove_numbers(labels)
+    labels_nn = remove_label_indices(labels)
 
     # Generate adjacency matrix using ASE
     adjacency = get_adjacency(labels_nn, coords, adjust_cutoff=adjust_cutoff)
 
     # Find entities
     mol_indices = find_entities_from_adjacency(labels_nn, adjacency)
 
     return mol_indices
 
 
 def find_entities_from_adjacency(labels_nn, adjacency):
-    """
+    '''
     Finds formulae of entities given in labels and adjacency matrix
 
     Parameters
     ----------
-    labels : list
+    labels : list[str]
         atomic labels
     adjacency : np.ndarray
         Adjacency matrix (0,1) with same order as labels
 
     Returns
     -------
-    dict
+    dict[str:list[list[int]]]
         keys = molecular formula,
         vals = list of lists, where each list contains the indices of a single
                 occurrence of the `key`, and the indices match the order given
                 in `labels` and `coords`
-    """
+    '''
 
     # Count number of atoms
     n_atoms = len(labels_nn)
 
     # Set current fragment as start atom
     curr_frag = {0}
 
@@ -1013,15 +1132,15 @@
 
     mol_indices = dict(mol_indices)
 
     return mol_indices
 
 
 def _calculate_rmsd(coords_1, coords_2):
-    """
+    '''
     Calculates RMSD between two structures
     RMSD = sqrt(mean(deviations**2))
     Where deviations are defined as norm([x1,y1,z1]-[x2,y2,z2])
 
     Parameters
     ----------
     coords_1 : np.ndarray
@@ -1029,18 +1148,18 @@
     coords_2 : np.ndarray
         xyz coordinates as (n_atoms, 3) array
 
     Returns
     -------
     float
         Root mean square of norms of deviation between two structures
-    """
+    '''
 
     # Check there are the same number of coordinates
-    assert(len(coords_1) == len(coords_2))
+    assert len(coords_1) == len(coords_2)
 
     # Calculate difference between [x,y,z] of atom pairs
     diff = [trio_1 - trio_2 for trio_1, trio_2 in zip(coords_1, coords_2)]
 
     # Calculate square norm of difference
     norms_sq = [la.norm(trio)**2 for trio in diff]
 
@@ -1051,15 +1170,15 @@
     rmsd = np.sqrt(mean)
 
     return rmsd
 
 
 def calculate_rmsd(coords_1, coords_2, mask_1=[], mask_2=[], order_1=[],
                    order_2=[]):
-    """
+    '''
     Calculates RMSD between two structures
     RMSD = sqrt(mean(deviations**2))
     Where deviations are defined as norm([x1,y1,z1]-[x2,y2,z2])
     If coords_1 and coords_2 are not the same length, then a mask array can be
     provided for either/both and is applied prior to the calculation
     coords_1 and coords_2 can also be reordered if new orders are specified
         - note this occurs BEFORE masking
@@ -1080,15 +1199,15 @@
     order_2 : list
         list of new indices for coords_2 - applied BEFORE masking
 
     Returns
     -------
     float
         Root mean square of norms of deviation between two structures
-    """
+    '''
 
     # Set up new ordering
     if order_1:
         _order_1 = order_1
     else:
         _order_1 = range(len(coords_1))
 
@@ -1112,15 +1231,15 @@
     # Calculate rmsd
     rmsd = _calculate_rmsd(_coords_1, _coords_2)
 
     return rmsd
 
 
 def rotate_coords(coords, alpha, beta, gamma):
-    """
+    '''
     Rotates coordinates by alpha, beta, gamma using the zyz convention
     https://easyspin.org/easyspin/documentation/eulerangles.html
 
     Parameters
     ----------
     coords : np.ndarray
         xyz coordinates as (n_atoms, 3) array
@@ -1132,27 +1251,27 @@
         gamma angle in radians
 
     Returns
     -------
     np.ndarray
         xyz coordinates as (n_atoms, 3) array after rotation
         in same order as input coordinates
-    """
+    '''
 
     R = np.zeros([3, 3])
 
     # Build rotation matrix
-    R[0, 0] = np.cos(gamma)*np.cos(beta)*np.cos(alpha) - np.sin(gamma) * np.sin(alpha) # noqa
-    R[0, 1] = np.cos(gamma)*np.cos(beta)*np.sin(alpha) + np.sin(gamma) * np.cos(alpha) # noqa
-    R[0, 2] = -np.cos(gamma)*np.sin(beta)
-    R[1, 0] = -np.sin(gamma)*np.cos(beta)*np.cos(alpha) - np.cos(gamma) * np.sin(alpha) # noqa
-    R[1, 1] = -np.sin(gamma)*np.cos(beta)*np.sin(alpha) + np.cos(gamma) * np.cos(alpha) # noqa
-    R[1, 2] = np.sin(gamma)*np.sin(beta)
-    R[2, 0] = np.sin(beta)*np.cos(alpha)
-    R[2, 1] = np.sin(beta)*np.sin(alpha)
+    R[0, 0] = np.cos(gamma) * np.cos(beta) * np.cos(alpha) - np.sin(gamma) * np.sin(alpha) # noqa
+    R[0, 1] = np.cos(gamma) * np.cos(beta) * np.sin(alpha) + np.sin(gamma) * np.cos(alpha) # noqa
+    R[0, 2] = -np.cos(gamma) * np.sin(beta)
+    R[1, 0] = -np.sin(gamma) * np.cos(beta) * np.cos(alpha) - np.cos(gamma) * np.sin(alpha) # noqa
+    R[1, 1] = -np.sin(gamma) * np.cos(beta) * np.sin(alpha) + np.cos(gamma) * np.cos(alpha) # noqa
+    R[1, 2] = np.sin(gamma) * np.sin(beta)
+    R[2, 0] = np.sin(beta) * np.cos(alpha)
+    R[2, 1] = np.sin(beta) * np.sin(alpha)
     R[2, 2] = np.cos(beta)
 
     # Create (n,3) matrix from coords list
     _coords = coords.T
 
     # Apply rotation matrix
     rot_coords = R @ _coords
@@ -1161,15 +1280,15 @@
     rot_coords = rot_coords.T
 
     return rot_coords
 
 
 def minimise_rmsd(coords_1, coords_2, mask_1=[], mask_2=[], order_1=[],
                   order_2=[]):
-    """
+    '''
     Minimising the RMSD between two structures
     If coords_1 and coords_2 are not the same length, then a mask array can be
     provided for either/both and is applied prior to the calculation
     coords_1 and coords_2 can also be reordered if new orders are specified
     **note reordering occurs before masking**
 
     Parameters
@@ -1187,15 +1306,15 @@
     order_2 : list
         list of new indices for coords_2 - applied BEFORE masking
 
     Returns
     -------
     float
         Root mean square of norms of deviation between two structures
-    """
+    '''
 
     # Set up new ordering
     if order_1:
         _order_1 = order_1
     else:
         _order_1 = range(len(coords_1))
 
@@ -1213,26 +1332,31 @@
         _coords_1 = np.delete(_coords_1, mask_1, axis=0)
 
     # Set up masks
     if mask_2:
         _coords_2 = np.delete(_coords_2, mask_2, axis=0)
 
     # Fit alpha, beta, and gamma to minimise rmsd
-    result = spo.least_squares(lambda angs: _rotate_and_rmsd(
-            angs, _coords_1, _coords_2), x0=(1., 1., 1.), jac='3-point')
+    result = spo.least_squares(
+        lambda angs: _rotate_and_rmsd(
+            angs, _coords_1, _coords_2
+        ),
+        x0=(1., 1., 1.),
+        jac='3-point'
+    )
 
     # Get optimum angles
     [alpha, beta, gamma] = result.x
     rmsd = result.cost
 
     return rmsd, alpha, beta, gamma
 
 
 def _rotate_and_rmsd(angs, coords_1, coords_2):
-    """
+    '''
     Rotates coords_1 by alpha, beta, gamma using the zyz convention
     https://easyspin.org/easyspin/documentation/eulerangles.html
     then calcualtes the rmsd between coords_1 and coords_2
 
     Parameters
     ----------
     coords_1 : np.ndarray
@@ -1243,45 +1367,46 @@
         alpha, beta, gamma in radians
 
     Returns
     -------
     np.ndarray
         xyz coordinates as (n_atoms, 3) array after rotation
         in same order as input coordinates
-    """
+    '''
 
     # Rotate coordinates of first system
     _coords_1 = rotate_coords(coords_1, angs[0], angs[1], angs[2])
 
     # Calculate rmsd between rotated first system and original second system
     rmsd = _calculate_rmsd(_coords_1, coords_2)
 
     return rmsd
 
 
 def calculate_com(labels, coords):
-    """
+    '''
     Calculates centre-of-mass using relative atomic masses
     Parameters
     ----------
     labels : list
         list of atomic labels
     coords : np.ndarray
         xyz coordinates as (n_atoms, 3) array
 
     Returns
     -------
     np.ndarray
         xyz coordinates of centre of mass as (3) array
-    """
+    '''
 
-    labels_nn = remove_numbers(labels)
+    labels_nn = remove_label_indices(labels)
 
     masses = [atomic.masses[lab] for lab in labels_nn]
 
     com_coords = np.zeros(3)
+    
     for trio, mass in zip(coords, masses):
         com_coords += trio * mass
 
     com_coords /= np.sum(masses)
 
     return com_coords
```

### Comparing `xyz_py-5.2.1/xyz_py.egg-info/PKG-INFO` & `xyz_py-5.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xyz-py
-Version: 5.2.1
+Name: xyz_py
+Version: 5.3.0
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

