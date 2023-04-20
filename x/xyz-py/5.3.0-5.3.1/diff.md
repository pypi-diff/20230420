# Comparing `tmp/xyz_py-5.3.0.tar.gz` & `tmp/xyz_py-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyz_py-5.3.0.tar", last modified: Thu Apr 20 17:15:06 2023, max compression
+gzip compressed data, was "xyz_py-5.3.1.tar", last modified: Thu Apr 20 18:03:21 2023, max compression
```

## Comparing `xyz_py-5.3.0.tar` & `xyz_py-5.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:15:06.202299 xyz_py-5.3.0/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2023-04-20 17:14:29.000000 xyz_py-5.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1303 2023-04-20 17:15:06.201299 xyz_py-5.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-20 17:14:29.000000 xyz_py-5.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-20 17:14:29.000000 xyz_py-5.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 17:15:06.202299 xyz_py-5.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-20 17:15:03.000000 xyz_py-5.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:15:06.198299 xyz_py-5.3.0/xyz_py/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-20 17:14:29.000000 xyz_py-5.3.0/xyz_py/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7408 2023-04-20 17:14:29.000000 xyz_py-5.3.0/xyz_py/atomic.py
--rw-rw-rw-   0 root         (0) root         (0)     8316 2023-04-20 17:14:29.000000 xyz_py-5.3.0/xyz_py/cli.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-20 17:15:03.000000 xyz_py-5.3.0/xyz_py/version.py
--rw-rw-rw-   0 root         (0) root         (0)    37690 2023-04-20 17:14:29.000000 xyz_py-5.3.0/xyz_py/xyz_py.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:15:06.201299 xyz_py-5.3.0/xyz_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1303 2023-04-20 17:15:06.000000 xyz_py-5.3.0/xyz_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-04-20 17:15:06.000000 xyz_py-5.3.0/xyz_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 17:15:06.000000 xyz_py-5.3.0/xyz_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-20 17:15:06.000000 xyz_py-5.3.0/xyz_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-20 17:15:06.000000 xyz_py-5.3.0/xyz_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-20 17:15:06.000000 xyz_py-5.3.0/xyz_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:03:21.875319 xyz_py-5.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2023-04-20 18:02:56.000000 xyz_py-5.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-20 18:03:21.874319 xyz_py-5.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-20 18:02:56.000000 xyz_py-5.3.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-20 18:02:56.000000 xyz_py-5.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 18:03:21.875319 xyz_py-5.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-20 18:03:18.000000 xyz_py-5.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:03:21.871319 xyz_py-5.3.1/xyz_py/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-20 18:02:56.000000 xyz_py-5.3.1/xyz_py/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7408 2023-04-20 18:02:56.000000 xyz_py-5.3.1/xyz_py/atomic.py
+-rw-rw-rw-   0 root         (0) root         (0)     8316 2023-04-20 18:02:56.000000 xyz_py-5.3.1/xyz_py/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-20 18:03:18.000000 xyz_py-5.3.1/xyz_py/version.py
+-rw-rw-rw-   0 root         (0) root         (0)    37690 2023-04-20 18:02:56.000000 xyz_py-5.3.1/xyz_py/xyz_py.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:03:21.874319 xyz_py-5.3.1/xyz_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-20 18:03:21.000000 xyz_py-5.3.1/xyz_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-20 18:03:21.000000 xyz_py-5.3.1/xyz_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 18:03:21.000000 xyz_py-5.3.1/xyz_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-20 18:03:21.000000 xyz_py-5.3.1/xyz_py.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-20 18:03:21.000000 xyz_py-5.3.1/xyz_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-20 18:03:21.000000 xyz_py-5.3.1/xyz_py.egg-info/top_level.txt
```

### Comparing `xyz_py-5.3.0/LICENSE` & `xyz_py-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xyz_py-5.3.0/PKG-INFO` & `xyz_py-5.3.1/xyz_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xyz_py
-Version: 5.3.0
+Name: xyz-py
+Version: 5.3.1
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xyz_py-5.3.0/README.md` & `xyz_py-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `xyz_py-5.3.0/setup.py` & `xyz_py-5.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "5.3.0"
+__version__ = "5.3.1"
 
 setuptools.setup(
     name="xyz_py",
     version=__version__,
     author="Jon Kragskow",
     author_email="jonkragskow@gmail.com",
     description="A package for manipulating xyz files and chemical structures",
```

### Comparing `xyz_py-5.3.0/xyz_py/atomic.py` & `xyz_py-5.3.1/xyz_py/atomic.py`

 * *Files identical despite different names*

### Comparing `xyz_py-5.3.0/xyz_py/cli.py` & `xyz_py-5.3.1/xyz_py/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             '{:.7f}'.format(value)
         ]
         for label, value in zip(bond_labels, bond_lengths)
     ])
 
     # Save to file
     np.savetxt(
-        f'{f_head}_bonds.dat',
+        f'{f_head}_bonds.csv',
         bond_lengths,
         fmt='%s',
         header='label, length (Angstrom)'
     )
 
     # Get angles
     angle_labels, angle_values = xyz_py.find_angles(
@@ -88,15 +88,15 @@
         ]
         for label, value in zip(angle_labels, angle_values)
     ])
 
     if len(angles):
         # Save to file
         np.savetxt(
-            f'{f_head}_angles.dat',
+            f'{f_head}_angles.csv',
             angles,
             fmt='%s',
             header='label, angle (degrees)'
         )
 
     # Get dihedrals
     dihedral_labels, dihedral_values = xyz_py.find_dihedrals(
@@ -114,27 +114,27 @@
         ]
         for label, value in zip(dihedral_labels, dihedral_values)
     ])
 
     if len(dihedrals):
         # Save to file
         np.savetxt(
-            f'{f_head}_dihedrals.dat',
+            f'{f_head}_dihedrals.csv',
             dihedrals,
             fmt='%s',
             header='label, dihedral angle (degrees)'
         )
 
     if not uargs.quiet:
         msg = 'Bonds'
         if len(angles):
             msg += ', angles'
         if len(dihedrals):
             msg += ', and dihedrals'
-        msg += f' written to {f_head}_<property>.dat'
+        msg += f' written to {f_head}_<property>.csv'
         print(msg)
 
     return
 
 
 def rotate_func(uargs):
     '''
```

### Comparing `xyz_py-5.3.0/xyz_py/xyz_py.py` & `xyz_py-5.3.1/xyz_py/xyz_py.py`

 * *Files identical despite different names*

### Comparing `xyz_py-5.3.0/xyz_py.egg-info/PKG-INFO` & `xyz_py-5.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xyz-py
-Version: 5.3.0
+Name: xyz_py
+Version: 5.3.1
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

