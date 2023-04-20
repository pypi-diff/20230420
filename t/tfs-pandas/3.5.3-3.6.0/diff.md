# Comparing `tmp/tfs-pandas-3.5.3.tar.gz` & `tmp/tfs-pandas-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/tfs/tfs/dist/.tmp-09jg2gx3/tfs-pandas-3.5.3.tar", last modified: Thu Apr 20 12:37:56 2023, max compression
+gzip compressed data, was "/home/runner/work/tfs/tfs/dist/.tmp-slo_bz1h/tfs-pandas-3.6.0.tar", last modified: Thu Apr 20 12:48:49 2023, max compression
```

## Comparing `tfs-pandas-3.5.3.tar` & `tfs-pandas-3.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:37:56.000000 tfs-pandas-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-20 12:37:56.000000 tfs-pandas-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:37:56.000000 tfs-pandas-3.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:37:56.000000 tfs-pandas-3.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tests/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tests/test_hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:37:56.000000 tfs-pandas-3.5.3/tfs/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tfs/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tfs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tfs/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    18460 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tfs/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tfs/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tfs/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tfs/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-04-20 12:37:36.000000 tfs-pandas-3.5.3/tfs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:37:56.000000 tfs-pandas-3.5.3/tfs_pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-20 12:37:56.000000 tfs-pandas-3.5.3/tfs_pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-20 12:37:56.000000 tfs-pandas-3.5.3/tfs_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:37:56.000000 tfs-pandas-3.5.3/tfs_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-20 12:37:56.000000 tfs-pandas-3.5.3/tfs_pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-20 12:37:56.000000 tfs-pandas-3.5.3/tfs_pandas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tests/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tests/test_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tfs_pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tfs_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tfs_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tfs_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tfs_pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tfs_pandas.egg-info/top_level.txt
```

### Comparing `tfs-pandas-3.5.3/LICENSE` & `tfs-pandas-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.3/PKG-INFO` & `tfs-pandas-3.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfs-pandas
-Version: 3.5.3
+Version: 3.6.0
 Summary: Read and write tfs files.
 Home-page: https://github.com/pylhc/tfs
 Author: pylhc
 Author-email: pylhc@github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tfs-pandas-3.5.3/README.md` & `tfs-pandas-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.3/setup.py` & `tfs-pandas-3.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 with README.open("r") as docs:
     long_description = docs.read()
 
 # Dependencies for the package itself
 DEPENDENCIES = [
     "numpy>=1.19.0",
-    "pandas<2.0",
+    "pandas>=1.0",
 ]
 
 # Extra dependencies
 EXTRA_DEPENDENCIES = {
     "test": ["pytest>=5.2", "pytest-cov>=2.9", "cpymad>=1.8.1", "zstandard>=0.15.2"],
     "hdf5": ["h5py>=2.9.0", "tables>=3.6.0"],
     "doc": ["sphinx", "sphinx_rtd_theme", "sphinx_copybutton", "sphinx-prompt", "sphinx_codeautolink"],
```

### Comparing `tfs-pandas-3.5.3/tests/test_collection.py` & `tfs-pandas-3.6.0/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.3/tests/test_compression.py` & `tfs-pandas-3.6.0/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.3/tests/test_frame.py` & `tfs-pandas-3.6.0/tests/test_frame.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,46 @@
         headers_left = OrderedDict()
         headers_right = OrderedDict()
 
         with pytest.raises(ValueError):
             merge_headers(headers_left, headers_right, how=how)
 
 
+class TestTfsDataFrameMerging:
+    @pytest.mark.parametrize("how_headers", [None, "left", "right"])
+    @pytest.mark.parametrize("how", ["left", "right", "outer", "inner"])
+    @pytest.mark.parametrize("on", ["NAME", "S", "NUMBER", "CO", "CORMS", "BPM_RES"])
+    def test_correct_merging(self, _tfs_file_x_pathlib, _tfs_file_y_pathlib, how_headers, how, on):
+        dframe_x = tfs.read(_tfs_file_x_pathlib)
+        dframe_y = tfs.read(_tfs_file_y_pathlib)
+        result = dframe_x.merge(dframe_y, how_headers=how_headers, how=how, on=on)
+
+        assert isinstance(result, TfsDataFrame)
+        assert isinstance(result.headers, OrderedDict)
+        assert_dict_equal(result.headers, merge_headers(dframe_x.headers, dframe_y.headers, how=how_headers))
+        assert_frame_equal(result, pd.DataFrame(dframe_x).merge(pd.DataFrame(dframe_y), how=how, on=on))
+
+    @pytest.mark.parametrize("how_headers", [None, "left", "right"])
+    @pytest.mark.parametrize("how", ["left", "right", "outer", "inner"])
+    @pytest.mark.parametrize("on", ["NAME", "S", "NUMBER", "CO", "CORMS", "BPM_RES"])
+    def test_merging_accepts_pandas_dataframe(
+        self, _tfs_file_x_pathlib, _tfs_file_y_pathlib, how_headers, how, on
+    ):
+        dframe_x = tfs.read(_tfs_file_x_pathlib)
+        dframe_y = pd.DataFrame(tfs.read(_tfs_file_y_pathlib))  # for test, loses headers here
+        result = dframe_x.merge(dframe_y, how_headers=how_headers, how=how, on=on)
+
+        assert isinstance(result, TfsDataFrame)
+        assert isinstance(result.headers, OrderedDict)
+
+        # using empty OrderedDict here as it's what dframe_y is getting when converted in the call
+        assert_dict_equal(result.headers, merge_headers(dframe_x.headers, OrderedDict(), how=how_headers))
+        assert_frame_equal(result, pd.DataFrame(dframe_x).merge(pd.DataFrame(dframe_y), how=how, on=on))
+
+
 class TestHeadersMerging:
     @pytest.mark.parametrize("how", ["left", "LEFT", "Left", "lEfT"])  # we're case-insensitive
     def test_headers_merging_left(self, _tfs_file_x_pathlib, _tfs_file_y_pathlib, how):
         headers_left = tfs.read(_tfs_file_x_pathlib).headers
         headers_right = tfs.read(_tfs_file_y_pathlib).headers
         result = merge_headers(headers_left, headers_right, how=how)
 
@@ -60,24 +92,20 @@
         result = merge_headers(headers_left, headers_right, how=how)
         assert result == OrderedDict()  # giving None returns empty headers
 
     def test_providing_new_headers_overrides_merging(self, _tfs_file_x_pathlib, _tfs_file_y_pathlib):
         dframe_x = tfs.read(_tfs_file_x_pathlib)
         dframe_y = tfs.read(_tfs_file_y_pathlib)
 
-        assert dframe_x.append(other=dframe_y, new_headers={}).headers == OrderedDict()
-        assert dframe_y.append(other=dframe_x, new_headers={}).headers == OrderedDict()
-
-        # we provide lsuffix (or rsuffix) since dframes have the same columns
-        assert dframe_x.join(other=dframe_y, lsuffix="_l", new_headers={}).headers == OrderedDict()
-        assert dframe_y.join(other=dframe_x, lsuffix="_l", new_headers={}).headers == OrderedDict()
-
         assert dframe_x.merge(right=dframe_y, new_headers={}).headers == OrderedDict()
         assert dframe_y.merge(right=dframe_x, new_headers={}).headers == OrderedDict()
 
+        assert tfs.concat([dframe_x, dframe_y], new_headers={}).headers == OrderedDict()
+        assert tfs.concat([dframe_y, dframe_x], new_headers={}).headers == OrderedDict()
+
 
 class TestPrinting:
     def test_header_print(self):
         headers = {"param": 3, "other": "hello"}
         df = TfsDataFrame(headers=headers)
         print_out = str(df)
         assert "Headers" in print_out
@@ -99,108 +127,14 @@
 
     def test_empty_headers_print(self):
         print_tfs = str(TfsDataFrame())
         print_df = str(pd.DataFrame())
         assert print_tfs == print_df.replace(pd.DataFrame.__name__, TfsDataFrame.__name__)
 
 
-class TestTfsDataFrameAppending:
-    @pytest.mark.parametrize("how_headers", [None, "left", "right"])
-    def test_correct_appending(self, _tfs_file_x_pathlib, _tfs_file_y_pathlib, how_headers):
-        dframe_x = tfs.read(_tfs_file_x_pathlib)
-        dframe_y = tfs.read(_tfs_file_y_pathlib)
-        result = dframe_x.append(dframe_y, how_headers=how_headers)
-
-        assert isinstance(result, TfsDataFrame)
-        assert isinstance(result.headers, OrderedDict)
-        assert_dict_equal(result.headers, merge_headers(dframe_x.headers, dframe_y.headers, how=how_headers))
-        assert_frame_equal(result, pd.DataFrame(dframe_x).append(pd.DataFrame(dframe_y)))
-
-    @pytest.mark.parametrize("how_headers", [None, "left", "right"])
-    def test_appending_accepts_pandas_dataframe(self, _tfs_file_x_pathlib, _tfs_file_y_pathlib, how_headers):
-        dframe_x = tfs.read(_tfs_file_x_pathlib)
-        dframe_y = pd.DataFrame(tfs.read(_tfs_file_y_pathlib))  # for test, loses headers here
-        result = dframe_x.append(dframe_y, how_headers=how_headers)
-
-        assert isinstance(result, TfsDataFrame)
-        assert isinstance(result.headers, OrderedDict)
-
-        # using empty OrderedDict here as it's what dframe_y is getting when converted in the call
-        assert_dict_equal(result.headers, merge_headers(dframe_x.headers, OrderedDict(), how=how_headers))
-        assert_frame_equal(result, pd.DataFrame(dframe_x).append(dframe_y))  # dframe_y already pandas
-
-
-class TestTfsDataFrameJoining:
-    @pytest.mark.parametrize("how_headers", [None, "left", "right"])
-    @pytest.mark.parametrize("lsuffix", ["left", "_x"])
-    @pytest.mark.parametrize("rsuffix", ["right", "_y"])
-    def test_correct_joining(self, _tfs_file_x_pathlib, _tfs_file_y_pathlib, how_headers, lsuffix, rsuffix):
-        dframe_x = tfs.read(_tfs_file_x_pathlib)
-        dframe_y = tfs.read(_tfs_file_y_pathlib)
-        result = dframe_x.join(dframe_y, how_headers=how_headers, lsuffix=lsuffix, rsuffix=rsuffix)
-
-        assert isinstance(result, TfsDataFrame)
-        assert isinstance(result.headers, OrderedDict)
-        assert_dict_equal(result.headers, merge_headers(dframe_x.headers, dframe_y.headers, how=how_headers))
-        assert_frame_equal(
-            result, pd.DataFrame(dframe_x).join(pd.DataFrame(dframe_y), lsuffix=lsuffix, rsuffix=rsuffix)
-        )
-
-    @pytest.mark.parametrize("how_headers", [None, "left", "right"])
-    @pytest.mark.parametrize("lsuffix", ["left", "_x"])
-    @pytest.mark.parametrize("rsuffix", ["right", "_y"])
-    def test_joining_accepts_pandas_dataframe(
-        self, _tfs_file_x_pathlib, _tfs_file_y_pathlib, how_headers, lsuffix, rsuffix
-    ):
-        dframe_x = tfs.read(_tfs_file_x_pathlib)
-        dframe_y = pd.DataFrame(tfs.read(_tfs_file_y_pathlib))  # for test, loses headers here
-        result = dframe_x.join(dframe_y, how_headers=how_headers, lsuffix=lsuffix, rsuffix=rsuffix)
-
-        assert isinstance(result, TfsDataFrame)
-        assert isinstance(result.headers, OrderedDict)
-
-        # using empty OrderedDict here as it's what dframe_y is getting when converted in the call
-        assert_dict_equal(result.headers, merge_headers(dframe_x.headers, OrderedDict(), how=how_headers))
-        assert_frame_equal(
-            result, pd.DataFrame(dframe_x).join(pd.DataFrame(dframe_y), lsuffix=lsuffix, rsuffix=rsuffix)
-        )
-
-
-class TestTfsDataFrameMerging:
-    @pytest.mark.parametrize("how_headers", [None, "left", "right"])
-    @pytest.mark.parametrize("how", ["left", "right", "outer", "inner"])
-    @pytest.mark.parametrize("on", ["NAME", "S", "NUMBER", "CO", "CORMS", "BPM_RES"])
-    def test_correct_merging(self, _tfs_file_x_pathlib, _tfs_file_y_pathlib, how_headers, how, on):
-        dframe_x = tfs.read(_tfs_file_x_pathlib)
-        dframe_y = tfs.read(_tfs_file_y_pathlib)
-        result = dframe_x.merge(dframe_y, how_headers=how_headers, how=how, on=on)
-
-        assert isinstance(result, TfsDataFrame)
-        assert isinstance(result.headers, OrderedDict)
-        assert_dict_equal(result.headers, merge_headers(dframe_x.headers, dframe_y.headers, how=how_headers))
-        assert_frame_equal(result, pd.DataFrame(dframe_x).merge(pd.DataFrame(dframe_y), how=how, on=on))
-
-    @pytest.mark.parametrize("how_headers", [None, "left", "right"])
-    @pytest.mark.parametrize("how", ["left", "right", "outer", "inner"])
-    @pytest.mark.parametrize("on", ["NAME", "S", "NUMBER", "CO", "CORMS", "BPM_RES"])
-    def test_merging_accepts_pandas_dataframe(
-        self, _tfs_file_x_pathlib, _tfs_file_y_pathlib, how_headers, how, on
-    ):
-        dframe_x = tfs.read(_tfs_file_x_pathlib)
-        dframe_y = pd.DataFrame(tfs.read(_tfs_file_y_pathlib))  # for test, loses headers here
-        result = dframe_x.merge(dframe_y, how_headers=how_headers, how=how, on=on)
-
-        assert isinstance(result, TfsDataFrame)
-        assert isinstance(result.headers, OrderedDict)
-
-        # using empty OrderedDict here as it's what dframe_y is getting when converted in the call
-        assert_dict_equal(result.headers, merge_headers(dframe_x.headers, OrderedDict(), how=how_headers))
-        assert_frame_equal(result, pd.DataFrame(dframe_x).merge(pd.DataFrame(dframe_y), how=how, on=on))
-
-
 class TestTfsDataFramesConcatenating:
     @pytest.mark.parametrize("how_headers", [None, "left", "right"])
     @pytest.mark.parametrize("axis", [0, 1])
     @pytest.mark.parametrize("join", ["inner", "outer"])
     def test_correct_concatenating(self, _tfs_file_x_pathlib, _tfs_file_y_pathlib, how_headers, axis, join):
         dframe_x = tfs.read(_tfs_file_x_pathlib)
         dframe_y = tfs.read(_tfs_file_y_pathlib)
```

### Comparing `tfs-pandas-3.5.3/tests/test_hdf.py` & `tfs-pandas-3.6.0/tests/test_hdf.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.3/tests/test_reader.py` & `tfs-pandas-3.6.0/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.3/tests/test_tools.py` & `tfs-pandas-3.6.0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.3/tests/test_writer.py` & `tfs-pandas-3.6.0/tests/test_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,16 @@
         )
 
         write_location = tmp_path / "test.tfs"
         write_tfs(write_location, df)
         assert write_location.is_file()
 
         new = read_tfs(write_location)
-        assert_frame_equal(df, new)
+        # with pandas 2.0 the index of new is empty but of type integer, which is fine
+        assert_frame_equal(df, new, check_index_type=False)
         assert_dict_equal(df.headers, new.headers, compare_keys=True)
 
     def test_write_int_float_str_columns(self, tmp_path):
         """This test is more of an extension of the test below
         (this dataframe was not affected by the bug)"""
         df = TfsDataFrame(
             data=[[1, 1.0, "one"], [2, 2.0, "two"], [3, 3.0, "three"]],
```

### Comparing `tfs-pandas-3.5.3/tfs/__init__.py` & `tfs-pandas-3.6.0/tfs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from tfs.hdf import read_hdf, write_hdf
 from tfs.reader import read_tfs
 from tfs.writer import write_tfs
 
 __title__ = "tfs-pandas"
 __description__ = "Read and write tfs files."
 __url__ = "https://github.com/pylhc/tfs"
-__version__ = "3.5.3"
+__version__ = "3.6.0"
 __author__ = "pylhc"
 __author_email__ = "pylhc@github.com"
 __license__ = "MIT"
 
 # aliases
 read = read_tfs
 write = write_tfs
```

### Comparing `tfs-pandas-3.5.3/tfs/collection.py` & `tfs-pandas-3.6.0/tfs/collection.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.3/tfs/constants.py` & `tfs-pandas-3.6.0/tfs/constants.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.3/tfs/frame.py` & `tfs-pandas-3.6.0/tfs/frame.py`

 * *Files 20% similar despite different names*

```diff
@@ -77,115 +77,14 @@
             s += "\n"
         return s
 
     def __repr__(self) -> str:
         headers_string = self._headers_repr()
         return f"{headers_string}{super().__repr__()}"
 
-    def append(
-        self,
-        other: Union["TfsDataFrame", pd.DataFrame],
-        how_headers: str = None,
-        new_headers: dict = None,
-        **kwargs,
-    ) -> "TfsDataFrame":
-        """
-        Append rows of the other ``TfsDataFrame`` to the end of caller, returning a new object. Data
-        manipulation is done by the ``pandas.Dataframe`` method of the same name. Resulting headers are
-        either merged according to the provided **how_headers** method or as given via **new_headers**.
-
-        ..warning::
-            This method uses ``pandas.DataFrame.append`` internally, which has been deprecated for a
-            while and removed with pandas 2.0. It will be removed from ``tfs-pandas`` as well in the
-            next release.
-
-        Args:
-            other (Union[TfsDataFrame, pd.DataFrame]): The ``TfsDataFrame`` to append to the caller.
-            how_headers (str): Type of merge to be performed for the headers. Either **left** or **right**.
-                Refer to :func:`tfs.frame.merge_headers` for behavior. If ``None`` is provided and
-                **new_headers** is not provided, the final headers will be empty. Case insensitive,
-                defaults to ``None``.
-            new_headers (dict): If provided, will be used as new_headers for the merged ``TfsDataFrame``.
-                Otherwise these are determined by merging the headers from the caller and the other
-                ``TfsDataFrame`` according to the method defined by the **how_headers** argument.
-
-        Keyword Args:
-            Any keyword argument is given to ``pandas.DataFrame.append()``. The default values for all these
-            parameters are left as set in the ``pandas`` codebase. To see these, refer to the pandas
-            [DataFrame.append documentation](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.append.html).
-
-        Returns:
-            A new ``TfsDataFrame`` with the appended data and merged headers.
-        """
-        LOGGER.warn("This method has been removed in pandas 2.0 and will be removed from TfsDataFrames too. Please use 'tfs.frame.concat' instead.")
-        LOGGER.debug("Appending data through 'pandas'")
-        if not hasattr(other, "headers"):
-            LOGGER.debug("Converting 'other' to TfsDataFrame for appending")
-            other = TfsDataFrame(other)  # so we accept pandas.DataFrame input here
-
-        dframe = super().append(other, **kwargs)
-
-        LOGGER.debug("Determining headers")
-        new_headers = (
-            new_headers
-            if new_headers is not None
-            else merge_headers(self.headers, other.headers, how=how_headers)
-        )
-        return TfsDataFrame(data=dframe, headers=new_headers)
-
-    def join(
-        self,
-        other: Union["TfsDataFrame", pd.DataFrame],
-        how_headers: str = None,
-        new_headers: dict = None,
-        **kwargs,
-    ) -> "TfsDataFrame":
-        """
-        Join columns of another ``TfsDataFrame``. Data manipulation is done by the ``pandas.Dataframe``
-        method of the same name. Resulting headers are either merged according to the provided
-        **how_headers** method or as given via **new_headers**.
-
-        ..warning::
-            This method uses ``pandas.DataFrame.join`` internally, which has been deprecated for a
-            while and removed with pandas 2.0. It will be removed from ``tfs-pandas`` as well in the
-            next release.
-
-        Args:
-            other (Union[TfsDataFrame, pd.DataFrame]): The ``TfsDataFrame`` to join into the caller.
-            how_headers (str): Type of merge to be performed for the headers. Either **left** or **right**.
-                Refer to :func:`tfs.frame.merge_headers` for behavior. If ``None`` is provided and
-                **new_headers** is not provided, the final headers will be empty. Case insensitive,
-                defaults to ``None``.
-            new_headers (dict): If provided, will be used as new_headers for the merged ``TfsDataFrame``.
-                Otherwise these are determined by merging the headers from the caller and the other
-                ``TfsDataFrame`` according to the method defined by the **how_headers** argument.
-
-        Keyword Args:
-            Any keyword argument is given to ``pandas.DataFrame.join()``. The default values for all these
-            parameters are left as set in the ``pandas`` codebase. To see these, refer to the pandas
-            [DataFrame.join documentation](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.join.html).
-
-        Returns:
-            A new ``TfsDataFrame`` with the joined columns and merged headers.
-        """
-        LOGGER.warn("This method has been removed in pandas 2.0 and will be removed from TfsDataFrames too. Please use 'tfs.frame.concat' instead.")
-        LOGGER.debug("Joining data through 'pandas'")
-        if not hasattr(other, "headers"):
-            LOGGER.debug("Converting 'other' to TfsDataFrame for joining")
-            other = TfsDataFrame(other)  # so we accept pandas.DataFrame input here
-        dframe = super().join(other, **kwargs)
-
-        LOGGER.debug("Determining headers")
-        new_headers = (
-            new_headers
-            if new_headers is not None
-            else merge_headers(self.headers, other.headers, how=how_headers)
-        )
-        return TfsDataFrame(data=dframe, headers=new_headers)
-
     def merge(
         self,
         right: Union["TfsDataFrame", pd.DataFrame],
         how_headers: str = None,
         new_headers: dict = None,
         **kwargs,
     ) -> "TfsDataFrame":
@@ -377,8 +276,8 @@
         LOGGER.debug(f"Some column-names are not of string-type, dataframe {info_str} is invalid.")
         raise TfsFormatError("TFS-Columns need to be strings.")
 
     if any(" " in c for c in data_frame.columns):
         LOGGER.debug(f"Space(s) found in TFS columns, dataframe {info_str} is invalid")
         raise TfsFormatError("TFS-Columns can not contain spaces.")
 
-    LOGGER.debug(f"DataFrame {info_str} validated")
+    LOGGER.debug(f"DataFrame {info_str} validated")
```

### Comparing `tfs-pandas-3.5.3/tfs/hdf.py` & `tfs-pandas-3.6.0/tfs/hdf.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.3/tfs/reader.py` & `tfs-pandas-3.6.0/tfs/reader.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.3/tfs/tools.py` & `tfs-pandas-3.6.0/tfs/tools.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.3/tfs/writer.py` & `tfs-pandas-3.6.0/tfs/writer.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.5.3/tfs_pandas.egg-info/PKG-INFO` & `tfs-pandas-3.6.0/tfs_pandas.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfs-pandas
-Version: 3.5.3
+Version: 3.6.0
 Summary: Read and write tfs files.
 Home-page: https://github.com/pylhc/tfs
 Author: pylhc
 Author-email: pylhc@github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

