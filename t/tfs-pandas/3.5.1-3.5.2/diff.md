# Comparing `tmp/tfs-pandas-3.5.1.tar.gz` & `tmp/tfs-pandas-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/tfs/tfs/dist/.tmp-tw4bhui7/tfs-pandas-3.5.1.tar", last modified: Mon Mar 20 10:17:00 2023, max compression
+gzip compressed data, was "/home/runner/work/tfs/tfs/dist/.tmp-xxkvcfgk/tfs-pandas-3.5.2.tar", last modified: Thu Apr 20 10:24:39 2023, max compression
```

## Comparing `tfs-pandas-3.5.1.tar` & `tfs-pandas-3.5.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:17:00.000000 tfs-pandas-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-03-20 10:17:00.000000 tfs-pandas-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 10:17:00.000000 tfs-pandas-3.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:17:00.000000 tfs-pandas-3.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tests/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tests/test_hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:17:00.000000 tfs-pandas-3.5.1/tfs/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tfs/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tfs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tfs/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17666 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tfs/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tfs/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tfs/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tfs/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-03-20 10:16:32.000000 tfs-pandas-3.5.1/tfs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:17:00.000000 tfs-pandas-3.5.1/tfs_pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-03-20 10:17:00.000000 tfs-pandas-3.5.1/tfs_pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-20 10:17:00.000000 tfs-pandas-3.5.1/tfs_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 10:17:00.000000 tfs-pandas-3.5.1/tfs_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-20 10:17:00.000000 tfs-pandas-3.5.1/tfs_pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-20 10:17:00.000000 tfs-pandas-3.5.1/tfs_pandas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:24:39.000000 tfs-pandas-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-20 10:24:39.000000 tfs-pandas-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:24:39.000000 tfs-pandas-3.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:24:39.000000 tfs-pandas-3.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tests/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tests/test_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:24:39.000000 tfs-pandas-3.5.2/tfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tfs/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tfs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tfs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18857 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tfs/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tfs/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tfs/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tfs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-04-20 10:24:18.000000 tfs-pandas-3.5.2/tfs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:24:39.000000 tfs-pandas-3.5.2/tfs_pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-20 10:24:39.000000 tfs-pandas-3.5.2/tfs_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-20 10:24:39.000000 tfs-pandas-3.5.2/tfs_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:24:39.000000 tfs-pandas-3.5.2/tfs_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-20 10:24:39.000000 tfs-pandas-3.5.2/tfs_pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-20 10:24:39.000000 tfs-pandas-3.5.2/tfs_pandas.egg-info/top_level.txt
```

### Comparing `tfs-pandas-3.5.1/LICENSE` & `tfs-pandas-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/PKG-INFO` & `tfs-pandas-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfs-pandas
-Version: 3.5.1
+Version: 3.5.2
 Summary: Read and write tfs files.
 Home-page: https://github.com/pylhc/tfs
 Author: pylhc
 Author-email: pylhc@github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tfs-pandas-3.5.1/README.md` & `tfs-pandas-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/setup.py` & `tfs-pandas-3.5.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 with README.open("r") as docs:
     long_description = docs.read()
 
 # Dependencies for the package itself
 DEPENDENCIES = [
     "numpy>=1.19.0",
-    "pandas>=1.0",
+    "pandas<2.0",
 ]
 
 # Extra dependencies
 EXTRA_DEPENDENCIES = {
     "test": ["pytest>=5.2", "pytest-cov>=2.9", "cpymad>=1.8.1", "zstandard>=0.15.2"],
     "hdf5": ["h5py>=2.9.0", "tables>=3.6.0"],
     "doc": ["sphinx", "sphinx_rtd_theme", "sphinx_copybutton", "sphinx-prompt", "sphinx_codeautolink"],
```

### Comparing `tfs-pandas-3.5.1/tests/test_collection.py` & `tfs-pandas-3.5.2/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/tests/test_compression.py` & `tfs-pandas-3.5.2/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/tests/test_frame.py` & `tfs-pandas-3.5.2/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/tests/test_hdf.py` & `tfs-pandas-3.5.2/tests/test_hdf.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/tests/test_reader.py` & `tfs-pandas-3.5.2/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/tests/test_tools.py` & `tfs-pandas-3.5.2/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/tests/test_writer.py` & `tfs-pandas-3.5.2/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/tfs/__init__.py` & `tfs-pandas-3.5.2/tfs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from tfs.hdf import read_hdf, write_hdf
 from tfs.reader import read_tfs
 from tfs.writer import write_tfs
 
 __title__ = "tfs-pandas"
 __description__ = "Read and write tfs files."
 __url__ = "https://github.com/pylhc/tfs"
-__version__ = "3.5.1"
+__version__ = "3.5.2"
 __author__ = "pylhc"
 __author_email__ = "pylhc@github.com"
 __license__ = "MIT"
 
 # aliases
 read = read_tfs
 write = write_tfs
```

### Comparing `tfs-pandas-3.5.1/tfs/collection.py` & `tfs-pandas-3.5.2/tfs/collection.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/tfs/constants.py` & `tfs-pandas-3.5.2/tfs/constants.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/tfs/frame.py` & `tfs-pandas-3.5.2/tfs/frame.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,14 +89,19 @@
         **kwargs,
     ) -> "TfsDataFrame":
         """
         Append rows of the other ``TfsDataFrame`` to the end of caller, returning a new object. Data
         manipulation is done by the ``pandas.Dataframe`` method of the same name. Resulting headers are
         either merged according to the provided **how_headers** method or as given via **new_headers**.
 
+        ..warning::
+            This method uses ``pandas.DataFrame.append`` internally, which has been deprecated for a
+            while and removed with pandas 2.0. It will be removed from ``tfs-pandas`` as well in the
+            next release.
+
         Args:
             other (Union[TfsDataFrame, pd.DataFrame]): The ``TfsDataFrame`` to append to the caller.
             how_headers (str): Type of merge to be performed for the headers. Either **left** or **right**.
                 Refer to :func:`tfs.frame.merge_headers` for behavior. If ``None`` is provided and
                 **new_headers** is not provided, the final headers will be empty. Case insensitive,
                 defaults to ``None``.
             new_headers (dict): If provided, will be used as new_headers for the merged ``TfsDataFrame``.
@@ -107,14 +112,15 @@
             Any keyword argument is given to ``pandas.DataFrame.append()``. The default values for all these
             parameters are left as set in the ``pandas`` codebase. To see these, refer to the pandas
             [DataFrame.append documentation](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.append.html).
 
         Returns:
             A new ``TfsDataFrame`` with the appended data and merged headers.
         """
+        LOGGER.warn("This method has been removed in pandas 2.0 and will be removed from TfsDataFrames too. Please use 'tfs.frame.concat' instead.")
         LOGGER.debug("Appending data through 'pandas'")
         if not hasattr(other, "headers"):
             LOGGER.debug("Converting 'other' to TfsDataFrame for appending")
             other = TfsDataFrame(other)  # so we accept pandas.DataFrame input here
 
         dframe = super().append(other, **kwargs)
 
@@ -134,14 +140,19 @@
         **kwargs,
     ) -> "TfsDataFrame":
         """
         Join columns of another ``TfsDataFrame``. Data manipulation is done by the ``pandas.Dataframe``
         method of the same name. Resulting headers are either merged according to the provided
         **how_headers** method or as given via **new_headers**.
 
+        ..warning::
+            This method uses ``pandas.DataFrame.join`` internally, which has been deprecated for a
+            while and removed with pandas 2.0. It will be removed from ``tfs-pandas`` as well in the
+            next release.
+
         Args:
             other (Union[TfsDataFrame, pd.DataFrame]): The ``TfsDataFrame`` to join into the caller.
             how_headers (str): Type of merge to be performed for the headers. Either **left** or **right**.
                 Refer to :func:`tfs.frame.merge_headers` for behavior. If ``None`` is provided and
                 **new_headers** is not provided, the final headers will be empty. Case insensitive,
                 defaults to ``None``.
             new_headers (dict): If provided, will be used as new_headers for the merged ``TfsDataFrame``.
@@ -152,14 +163,15 @@
             Any keyword argument is given to ``pandas.DataFrame.join()``. The default values for all these
             parameters are left as set in the ``pandas`` codebase. To see these, refer to the pandas
             [DataFrame.join documentation](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.join.html).
 
         Returns:
             A new ``TfsDataFrame`` with the joined columns and merged headers.
         """
+        LOGGER.warn("This method has been removed in pandas 2.0 and will be removed from TfsDataFrames too. Please use 'tfs.frame.concat' instead.")
         LOGGER.debug("Joining data through 'pandas'")
         if not hasattr(other, "headers"):
             LOGGER.debug("Converting 'other' to TfsDataFrame for joining")
             other = TfsDataFrame(other)  # so we accept pandas.DataFrame input here
         dframe = super().join(other, **kwargs)
 
         LOGGER.debug("Determining headers")
@@ -178,14 +190,19 @@
         **kwargs,
     ) -> "TfsDataFrame":
         """
         Merge ``TfsDataFrame`` objects with a database-style join. Data manipulation is done by the
         ``pandas.Dataframe`` method of the same name. Resulting headers are either merged according to the
         provided **how_headers** method or as given via **new_headers**.
 
+        ..warning::
+            This method uses ``pandas.DataFrame.merge`` internally, which has been deprecated for a
+            while and removed with pandas 2.0. It will be removed from ``tfs-pandas`` as well in the
+            next release.
+
         Args:
             right (Union[TfsDataFrame, pd.DataFrame]): The ``TfsDataFrame`` to merge with the caller.
             how_headers (str): Type of merge to be performed for the headers. Either **left** or **right**.
                 Refer to :func:`tfs.frame.merge_headers` for behavior. If ``None`` is provided and
                 **new_headers** is not provided, the final headers will be empty. Case insensitive,
                 defaults to ``None``.
             new_headers (dict): If provided, will be used as headers for the merged ``TfsDataFrame``.
@@ -196,14 +213,15 @@
             Any keyword argument is given to ``pandas.DataFrame.merge()``. The default values for all these
             parameters are left as set in the ``pandas`` codebase. To see these, refer to the pandas
             [DataFrame.merge documentation](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.merge.html).
 
         Returns:
             A new ``TfsDataFrame`` with the merged data and merged headers.
         """
+        LOGGER.warn("This method has been removed in pandas 2.0 and will be removed from TfsDataFrames too. Please use 'tfs.frame.concat' instead.")
         LOGGER.debug("Merging data through 'pandas'")
         if not hasattr(right, "headers"):
             LOGGER.debug("Converting 'right' to TfsDataFrame for merging")
             right = TfsDataFrame(right)  # so we accept pandas.DataFrame input here
         dframe = super().merge(right, **kwargs)
 
         LOGGER.debug("Determining headers")
```

### Comparing `tfs-pandas-3.5.1/tfs/hdf.py` & `tfs-pandas-3.5.2/tfs/hdf.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/tfs/reader.py` & `tfs-pandas-3.5.2/tfs/reader.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/tfs/tools.py` & `tfs-pandas-3.5.2/tfs/tools.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/tfs/writer.py` & `tfs-pandas-3.5.2/tfs/writer.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.1/tfs_pandas.egg-info/PKG-INFO` & `tfs-pandas-3.5.2/tfs_pandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfs-pandas
-Version: 3.5.1
+Version: 3.5.2
 Summary: Read and write tfs files.
 Home-page: https://github.com/pylhc/tfs
 Author: pylhc
 Author-email: pylhc@github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

