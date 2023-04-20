# Comparing `tmp/wfdb-4.1.0.tar.gz` & `tmp/wfdb-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wfdb-4.1.0.tar", max compression
+gzip compressed data, was "wfdb-4.1.1.tar", max compression
```

## Comparing `wfdb-4.1.0.tar` & `wfdb-4.1.1.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0     1110 2022-12-02 21:22:42.302000 wfdb-4.1.0/LICENSE
--rw-r--r--   0        0        0     2930 2022-12-02 21:22:42.304000 wfdb-4.1.0/README.md
--rw-r--r--   0        0        0     1190 2022-12-02 21:22:42.403000 wfdb-4.1.0/pyproject.toml
--rw-r--r--   0        0        0      687 2022-12-02 21:22:45.381000 wfdb-4.1.0/wfdb/__init__.py
--rw-r--r--   0        0        0      648 2022-12-02 21:22:45.381000 wfdb-4.1.0/wfdb/io/__init__.py
--rw-r--r--   0        0        0     1917 2022-12-02 21:22:45.381000 wfdb-4.1.0/wfdb/io/_coreio.py
--rw-r--r--   0        0        0    39404 2022-12-02 21:22:45.381000 wfdb-4.1.0/wfdb/io/_header.py
--rw-r--r--   0        0        0    90295 2022-12-02 21:22:45.382000 wfdb-4.1.0/wfdb/io/_signal.py
--rw-r--r--   0        0        0    23697 2022-12-02 21:22:45.382000 wfdb-4.1.0/wfdb/io/_url.py
--rw-r--r--   0        0        0   109544 2022-12-02 21:22:45.382000 wfdb-4.1.0/wfdb/io/annotation.py
--rw-r--r--   0        0        0      256 2022-12-02 21:22:45.382000 wfdb-4.1.0/wfdb/io/convert/__init__.py
--rw-r--r--   0        0        0    29336 2022-12-02 21:22:45.382000 wfdb-4.1.0/wfdb/io/convert/csv.py
--rw-r--r--   0        0        0    45845 2022-12-02 21:22:45.383000 wfdb-4.1.0/wfdb/io/convert/edf.py
--rw-r--r--   0        0        0    12271 2022-12-02 21:22:45.383000 wfdb-4.1.0/wfdb/io/convert/matlab.py
--rw-r--r--   0        0        0    10273 2022-12-02 21:22:45.383000 wfdb-4.1.0/wfdb/io/convert/tff.py
--rw-r--r--   0        0        0    13936 2022-12-02 21:22:45.383000 wfdb-4.1.0/wfdb/io/convert/wav.py
--rw-r--r--   0        0        0     2223 2022-12-02 21:22:45.383000 wfdb-4.1.0/wfdb/io/datasource.py
--rw-r--r--   0        0        0    15105 2022-12-02 21:22:45.383000 wfdb-4.1.0/wfdb/io/download.py
--rw-r--r--   0        0        0     3150 2022-12-02 21:22:45.383000 wfdb-4.1.0/wfdb/io/header.py
--rw-r--r--   0        0        0   115675 2022-12-02 21:22:45.384000 wfdb-4.1.0/wfdb/io/record.py
--rw-r--r--   0        0        0     2696 2022-12-02 21:22:45.384000 wfdb-4.1.0/wfdb/io/util.py
--rw-r--r--   0        0        0      148 2022-12-02 21:22:45.384000 wfdb-4.1.0/wfdb/plot/__init__.py
--rw-r--r--   0        0        0    40768 2022-12-02 21:22:45.384000 wfdb-4.1.0/wfdb/plot/plot.py
--rw-r--r--   0        0        0      532 2022-12-02 21:22:45.384000 wfdb-4.1.0/wfdb/processing/__init__.py
--rw-r--r--   0        0        0     5876 2022-12-02 21:22:45.384000 wfdb-4.1.0/wfdb/processing/basic.py
--rw-r--r--   0        0        0    18430 2022-12-02 21:22:45.384000 wfdb-4.1.0/wfdb/processing/evaluate.py
--rw-r--r--   0        0        0     6595 2022-12-02 21:22:45.384000 wfdb-4.1.0/wfdb/processing/filter.py
--rw-r--r--   0        0        0     9003 2022-12-02 21:22:45.384000 wfdb-4.1.0/wfdb/processing/hr.py
--rw-r--r--   0        0        0     6850 2022-12-02 21:22:45.384000 wfdb-4.1.0/wfdb/processing/peaks.py
--rw-r--r--   0        0        0    57055 2022-12-02 21:22:45.385000 wfdb-4.1.0/wfdb/processing/qrs.py
--rw-r--r--   0        0        0       22 2022-12-02 21:22:45.385000 wfdb-4.1.0/wfdb/version.py
--rw-r--r--   0        0        0     4168 1970-01-01 00:00:00.000000 wfdb-4.1.0/setup.py
--rw-r--r--   0        0        0     4339 1970-01-01 00:00:00.000000 wfdb-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1110 2022-06-21 15:27:15.202690 wfdb-4.1.1/LICENSE
+-rw-r--r--   0        0        0     2930 2022-09-20 21:14:17.893524 wfdb-4.1.1/README.md
+-rw-r--r--   0        0        0     1192 2023-04-20 19:43:47.356150 wfdb-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0      687 2022-06-21 15:27:16.045048 wfdb-4.1.1/wfdb/__init__.py
+-rw-r--r--   0        0        0      648 2022-06-21 15:27:16.045133 wfdb-4.1.1/wfdb/io/__init__.py
+-rw-r--r--   0        0        0     1917 2022-07-05 20:20:20.605553 wfdb-4.1.1/wfdb/io/_coreio.py
+-rw-r--r--   0        0        0    39511 2023-04-20 19:29:26.058066 wfdb-4.1.1/wfdb/io/_header.py
+-rw-r--r--   0        0        0    90294 2023-04-20 19:29:26.058436 wfdb-4.1.1/wfdb/io/_signal.py
+-rw-r--r--   0        0        0    23697 2022-06-21 15:27:16.045795 wfdb-4.1.1/wfdb/io/_url.py
+-rw-r--r--   0        0        0   109541 2023-04-20 19:29:26.058858 wfdb-4.1.1/wfdb/io/annotation.py
+-rw-r--r--   0        0        0      256 2022-06-21 15:27:16.046198 wfdb-4.1.1/wfdb/io/convert/__init__.py
+-rw-r--r--   0        0        0    29336 2022-09-20 21:14:17.896813 wfdb-4.1.1/wfdb/io/convert/csv.py
+-rw-r--r--   0        0        0    45925 2023-04-20 19:29:26.059133 wfdb-4.1.1/wfdb/io/convert/edf.py
+-rw-r--r--   0        0        0    12271 2022-06-21 15:27:16.046849 wfdb-4.1.1/wfdb/io/convert/matlab.py
+-rw-r--r--   0        0        0    10273 2022-06-21 15:27:16.046949 wfdb-4.1.1/wfdb/io/convert/tff.py
+-rw-r--r--   0        0        0    13935 2023-04-20 19:29:26.059296 wfdb-4.1.1/wfdb/io/convert/wav.py
+-rw-r--r--   0        0        0     2223 2022-06-21 15:27:16.047057 wfdb-4.1.1/wfdb/io/datasource.py
+-rw-r--r--   0        0        0    15118 2023-04-20 19:29:26.059445 wfdb-4.1.1/wfdb/io/download.py
+-rw-r--r--   0        0        0     3150 2022-09-20 21:14:17.897028 wfdb-4.1.1/wfdb/io/header.py
+-rw-r--r--   0        0        0   115668 2023-04-20 19:29:26.059905 wfdb-4.1.1/wfdb/io/record.py
+-rw-r--r--   0        0        0     2733 2023-04-20 19:29:26.061050 wfdb-4.1.1/wfdb/io/util.py
+-rw-r--r--   0        0        0      148 2022-06-21 15:27:16.047594 wfdb-4.1.1/wfdb/plot/__init__.py
+-rw-r--r--   0        0        0    40768 2022-07-05 20:20:20.607453 wfdb-4.1.1/wfdb/plot/plot.py
+-rw-r--r--   0        0        0      532 2022-06-21 15:27:16.047825 wfdb-4.1.1/wfdb/processing/__init__.py
+-rw-r--r--   0        0        0     5876 2022-07-05 20:20:20.607593 wfdb-4.1.1/wfdb/processing/basic.py
+-rw-r--r--   0        0        0    18430 2022-06-21 15:27:16.048018 wfdb-4.1.1/wfdb/processing/evaluate.py
+-rw-r--r--   0        0        0     6595 2022-06-21 15:27:16.048086 wfdb-4.1.1/wfdb/processing/filter.py
+-rw-r--r--   0        0        0     9002 2023-04-20 19:29:26.061207 wfdb-4.1.1/wfdb/processing/hr.py
+-rw-r--r--   0        0        0     6850 2022-06-21 15:27:16.048237 wfdb-4.1.1/wfdb/processing/peaks.py
+-rw-r--r--   0        0        0    57054 2023-04-20 19:29:26.061489 wfdb-4.1.1/wfdb/processing/qrs.py
+-rw-r--r--   0        0        0       22 2023-04-20 19:44:04.377675 wfdb-4.1.1/wfdb/version.py
+-rw-r--r--   0        0        0     4255 1970-01-01 00:00:00.000000 wfdb-4.1.1/PKG-INFO
```

### Comparing `wfdb-4.1.0/LICENSE` & `wfdb-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/README.md` & `wfdb-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/pyproject.toml` & `wfdb-4.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "wfdb"
-version = "4.1.0"
+version = "4.1.1"
 description = "The WFDB Python package: tools for reading, writing, and processing physiologic signals and annotations."
 authors = ["The Laboratory for Computational Physiology <contact@physionet.org>"]
 readme = "README.md"
 homepage = "https://github.com/MIT-LCP/wfdb-python/"
 repository = "https://github.com/MIT-LCP/wfdb-python/"
 documentation = "https://wfdb.readthedocs.io/"
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-numpy = "^1.10.1"
-scipy = "^1.0.0"
-pandas = "^1.0.0"
-SoundFile = ">=0.10.0, <0.12.0"
-matplotlib = "^3.2.2"
-requests = "^2.8.1"
-pytest = {version = "^7.1.1", optional = true}
-pytest-xdist = {version = "^2.5.0", optional = true}
-pylint = {version = "^2.13.7", optional = true}
-black = {version = "^22.3.0", optional = true}
-Sphinx = {version = "^4.5.0", optional = true}
+python = ">=3.7"
+numpy = ">=1.10.1"
+scipy = ">=1.0.0"
+pandas = ">=1.3.0"
+SoundFile = ">=0.10.0"
+matplotlib = ">=3.2.2"
+requests = ">=2.8.1"
+pytest = {version = ">=7.1.1", optional = true}
+pytest-xdist = {version = ">=2.5.0", optional = true}
+pylint = {version = ">=2.13.7", optional = true}
+black = {version = ">=22.3.0", optional = true}
+Sphinx = {version = ">=4.5.0", optional = true}
 
 [tool.poetry.extras]
 dev = ["pytest", "pytest-xdist", "pylint", "black", "Sphinx"]
 
 # Do NOT use [tool.poetry.dev-dependencies]. See: https://github.com/python-poetry/poetry/issues/3514
 
 [tool.black]
```

### Comparing `wfdb-4.1.0/wfdb/__init__.py` & `wfdb-4.1.1/wfdb/__init__.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/io/__init__.py` & `wfdb-4.1.1/wfdb/io/__init__.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/io/_coreio.py` & `wfdb-4.1.1/wfdb/io/_coreio.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/io/_header.py` & `wfdb-4.1.1/wfdb/io/_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from typing import Collection, List, Tuple
+from typing import Any, Dict, List, Optional, Sequence, Tuple
 
 import numpy as np
 import pandas as pd
 
 from wfdb.io import _signal
 from wfdb.io import util
 from wfdb.io.header import HeaderSyntaxError, rx_record, rx_segment, rx_signal
@@ -422,15 +422,14 @@
             ):
                 return
             setattr(self, field, RECORD_SPECS.loc[field, "write_default"])
 
         # Signal specification fields
         # Setting entire list default, not filling in blanks in lists.
         elif field in SIGNAL_SPECS.index:
-
             # Specific dynamic case
             if field == "file_name" and self.file_name is None:
                 self.file_name = self._auto_signal_file_names()
                 return
 
             item = getattr(self, field)
 
@@ -468,15 +467,14 @@
         Returns
         -------
         N/A
 
         """
         # If there are no signal specification fields, there is nothing to check.
         if self.n_sig > 0:
-
             # The length of all signal specification fields must match n_sig
             # even if some of its elements are None.
             for f in sig_write_fields:
                 if len(getattr(self, f)) != self.n_sig:
                     raise ValueError(
                         "The length of field: " + f + " must match field n_sig."
                     )
@@ -594,14 +592,18 @@
 
     Attributes
     ----------
     N/A
 
     """
 
+    n_seg: int
+    seg_len: Sequence[int]
+    segments: Optional[Sequence]
+
     def set_defaults(self):
         """
         Set defaults for fields needed to write the header if they have
         defaults. This is NOT called by rdheader. It is only called by the
         gateway wrsamp for convenience. It is also not called by wrheader since
         it is supposed to be an explicit function. Not responsible for
         initializing the attributes. That is done by the constructor.
@@ -916,15 +918,15 @@
         if range_start is not None:
             ranges.append((range_start, seg_start))
 
         return ranges
 
     def contained_combined_ranges(
         self,
-        sig_names: Collection[str],
+        sig_names: Sequence[str],
     ) -> List[Tuple[int, int]]:
         """
         Given a collection of signal name, return the sample ranges that
         contain all of the specified signals, relative to the start of the
         full record. Does not account for NaNs/missing values.
 
         This function is mainly useful for variable layout records, but can also be
@@ -1006,15 +1008,15 @@
     Returns
     -------
     record_fields : dict
         The fields for the given record line.
 
     """
     # Dictionary for record fields
-    record_fields = {}
+    record_fields: Dict[str, Any] = {}
 
     # Read string fields from record line
     match = rx_record.match(record_line)
     if match is None:
         raise HeaderSyntaxError("invalid syntax in record line")
     (
         record_fields["record_name"],
```

### Comparing `wfdb-4.1.0/wfdb/io/_signal.py` & `wfdb-4.1.1/wfdb/io/_signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1981,15 +1981,14 @@
     Notes
     -----
     `fmt` is just for the correct NAN value.
     `samps_per_frame` is only used for skewing expanded signals.
 
     """
     if max(skew) > 0:
-
         # Expanded frame samples. List of arrays.
         if isinstance(sig, list):
             # Shift the channel samples
             for ch in range(n_sig):
                 if skew[ch] > 0:
                     sig[ch][: read_len * samps_per_frame[ch]] = sig[ch][
                         skew[ch] * samps_per_frame[ch] :
```

### Comparing `wfdb-4.1.0/wfdb/io/_url.py` & `wfdb-4.1.1/wfdb/io/_url.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/io/annotation.py` & `wfdb-4.1.1/wfdb/io/annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,14 @@
         aux_note=None,
         fs=None,
         label_store=None,
         description=None,
         custom_labels=None,
         contained_labels=None,
     ):
-
         self.record_name = record_name
         self.extension = extension
 
         self.sample = sample
         self.symbol = symbol
 
         self.subtype = subtype
@@ -1176,15 +1175,14 @@
         typecodes = {
             label_table.iloc[i]["symbol"]: label_table.iloc[i]["label_store"]
             for i in range(len(label_table))
         }
 
         # Iterate across all fields one index at a time
         for i in range(len(sampdiff)):
-
             # Process the samp (difference) and sym items
             data_bytes.append(
                 field2bytes(
                     "samptype", [sampdiff[i], self.symbol[i]], typecodes
                 )
             )
 
@@ -2148,15 +2146,14 @@
     # Process annotations. Iterate across byte pairs.
     # Sequence for one ann is:
     # - SKIP pair (if any)
     # - samp + sym pair
     # - other pairs (if any)
     # The last byte pair of the file is 0 indicating eof.
     while bpi < filebytes.shape[0] - 1:
-
         # Get the sample and label_store fields of the current annotation
         sample_diff, current_label_store, bpi = proc_core_fields(filebytes, bpi)
         sample_total = sample_total + sample_diff
         sample.append(sample_total)
         label_store.append(current_label_store)
 
         # Process any other fields belonging to this annotation
@@ -3014,15 +3011,14 @@
         The description provided with the annotation.
     human_reviewed : bool
         Whether the annotation was human-reviewed (True) or not (False).
 
     """
 
     def __init__(self, extension, description, human_reviewed):
-
         self.extension = extension
         self.description = description
         self.human_reviewed = human_reviewed
 
 
 ann_classes = [
     AnnotationClass("atr", "Reference ECG annotations", True),
@@ -3050,14 +3046,15 @@
     }
 )
 ann_class_table.set_index(ann_class_table["extension"].values, inplace=True)
 ann_class_table = ann_class_table[
     ["extension", "description", "human_reviewed"]
 ]
 
+
 # Individual annotation labels
 class AnnotationLabel(object):
     """
     Describes the individual annotation labels.
 
     Attributes
     ----------
```

### Comparing `wfdb-4.1.0/wfdb/io/convert/csv.py` & `wfdb-4.1.1/wfdb/io/convert/csv.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/io/convert/edf.py` & `wfdb-4.1.1/wfdb/io/convert/edf.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,14 @@
     Examples
     --------
     >>> record = read_edf('x001_FAROS.edf',
                            pn_dir='simultaneous-measurements/raw_data')
 
     """
     if pn_dir is not None:
-
         if "." not in pn_dir:
             dir_list = pn_dir.split("/")
             pn_dir = posixpath.join(
                 dir_list[0], download.get_version(dir_list[0]), *dir_list[1:]
             )
 
         file_url = posixpath.join(download.PN_INDEX_URL, pn_dir, record_name)
@@ -185,15 +184,17 @@
     if verbose:
         print("Recording Time: {}".format(start_time))
     start_hour, start_minute, start_second = [
         int(i) for i in start_time.split(".")
     ]
 
     # Number of bytes in header (8 bytes)
-    header_bytes = int(struct.unpack("<8s", edf_file.read(8))[0].decode(encoding))
+    header_bytes = int(
+        struct.unpack("<8s", edf_file.read(8))[0].decode(encoding)
+    )
     if verbose:
         print("Number of bytes in header record: {}".format(header_bytes))
 
     # Reserved (44 bytes)
     reserved_notes = (
         struct.unpack("<44s", edf_file.read(44))[0].decode(encoding).strip()
     )
@@ -218,15 +219,17 @@
         print("Number of data records: {}".format(num_blocks))
     if num_blocks == -1:
         raise Exception(
             "Number of data records in unknown (not currently supported)"
         )
 
     # Duration of a block, in seconds (8 bytes)
-    block_duration = float(struct.unpack("<8s", edf_file.read(8))[0].decode(encoding))
+    block_duration = float(
+        struct.unpack("<8s", edf_file.read(8))[0].decode(encoding)
+    )
     if verbose:
         print(
             "Duration of each data record in seconds: {}".format(block_duration)
         )
     if block_duration <= 0.0:
         block_duration = 1.0
 
@@ -236,15 +239,17 @@
         print("Number of signals: {}".format(n_sig))
     if n_sig < 1:
         raise Exception("Done: not any signals left to read")
 
     # Label (e.g., EEG FpzCz or Body temp) (16 bytes each)
     sig_name = []
     for _ in range(n_sig):
-        temp_sig = struct.unpack("<16s", edf_file.read(16))[0].decode(encoding).strip()
+        temp_sig = (
+            struct.unpack("<16s", edf_file.read(16))[0].decode(encoding).strip()
+        )
         if temp_sig == "EDF Annotations" and not rdedfann_flag:
             print(
                 "*** This may be an EDF+ Annotation file instead, please see "
                 "the `rdedfann` function. ***"
             )
         sig_name.append(temp_sig)
     if verbose:
@@ -752,15 +757,14 @@
     out_data = np.array(out_data, dtype=np.int16)
 
     # Start writing the file
     if output_filename == "":
         output_filename = record_name_out + ".edf"
 
     with open(output_filename, "wb") as f:
-
         print(
             "Converting record {} to {} ({} mode)".format(
                 record_name, output_filename, "EDF+" if edf_plus else "EDF"
             )
         )
 
         # Version of this data format (8 bytes)
@@ -1114,15 +1118,17 @@
     for chunk in rec.p_signal.flatten().astype(np.int64):
         if chunk + 1 == 0:
             continue
         else:
             adjusted_hex = hex(
                 struct.unpack("<H", struct.pack(">H", chunk + 1))[0]
             )
-            annotation_string += bytes.fromhex(adjusted_hex[2:]).decode(encoding)
+            annotation_string += bytes.fromhex(adjusted_hex[2:]).decode(
+                encoding
+            )
             # Remove all of the whitespace
             for rep in ["\x00", "\x14", "\x15"]:
                 annotation_string = annotation_string.replace(rep, " ")
 
     # Parse the resulting annotation string
     onsets = []
     onset_times = []
```

### Comparing `wfdb-4.1.0/wfdb/io/convert/matlab.py` & `wfdb-4.1.1/wfdb/io/convert/matlab.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/io/convert/tff.py` & `wfdb-4.1.1/wfdb/io/convert/tff.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/io/convert/wav.py` & `wfdb-4.1.1/wfdb/io/convert/wav.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,14 @@
     >>> record = read_wav('sample-data/SC4001E0-PSG.wav')
 
     """
     if not record_name.endswith(".wav"):
         raise Exception("Name of the input file must end in .wav")
 
     if pn_dir is not None:
-
         if "." not in pn_dir:
             dir_list = pn_dir.split("/")
             pn_dir = posixpath.join(
                 dir_list[0], download.get_version(dir_list[0]), *dir_list[1:]
             )
 
         file_url = posixpath.join(download.PN_INDEX_URL, pn_dir, record_name)
```

### Comparing `wfdb-4.1.0/wfdb/io/datasource.py` & `wfdb-4.1.1/wfdb/io/datasource.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/io/download.py` & `wfdb-4.1.1/wfdb/io/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     Attributes
     ----------
     N/A
 
     """
 
-    pass
+    db_index_url: str
 
 
 # The configuration database index url. Uses PhysioNet index by default.
 config = Config()
 config.db_index_url = PN_INDEX_URL
```

### Comparing `wfdb-4.1.0/wfdb/io/header.py` & `wfdb-4.1.1/wfdb/io/header.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/io/record.py` & `wfdb-4.1.1/wfdb/io/record.py`

 * *Files 0% similar despite different names*

```diff
@@ -809,15 +809,14 @@
         adc_zero=None,
         init_value=None,
         checksum=None,
         block_size=None,
         sig_name=None,
         comments=None,
     ):
-
         # Note the lack of the 'n_seg' field. Single segment records cannot
         # have this field. Even n_seg = 1 makes the header a multi-segment
         # header.
         super(Record, self).__init__(
             record_name=record_name,
             n_sig=n_sig,
             fs=fs,
@@ -873,15 +872,14 @@
 
         if set(att1.keys()) != set(att2.keys()):
             if verbose:
                 print("Attributes members mismatch.")
             return False
 
         for k in att1.keys():
-
             v1 = att1[k]
             v2 = att2[k]
 
             if type(v1) != type(v2):
                 if verbose:
                     print("Mismatch in attribute: %s" % k, v1, v2)
                 return False
@@ -890,15 +888,15 @@
                 # Necessary for nans
                 np.testing.assert_array_equal(v1, v2)
             elif (
                 isinstance(v1, list)
                 and len(v1) == len(v2)
                 and all(isinstance(e, np.ndarray) for e in v1)
             ):
-                for (e1, e2) in zip(v1, v2):
+                for e1, e2 in zip(v1, v2):
                     np.testing.assert_array_equal(e1, e2)
             else:
                 if v1 != v2:
                     if verbose:
                         print("Mismatch in attribute: %s" % k, v1, v2)
                     return False
 
@@ -984,15 +982,14 @@
         else:
             self.d_signal = self.smooth_frames("digital")
             self.e_d_signal = None
 
             # Checksum and init_value to be updated if present
             # unless the whole signal length was input
             if self.sig_len != self.d_signal.shape[0]:
-
                 if self.checksum is not None:
                     self.checksum = self.calc_checksum()
                 if self.init_value is not None:
                     ival = list(self.d_signal[0, :])
                     self.init_value = [int(i) for i in ival]
 
             # Update record specification parameters
@@ -1132,15 +1129,14 @@
         base_datetime=None,
         seg_name=None,
         seg_len=None,
         comments=None,
         sig_name=None,
         sig_segments=None,
     ):
-
         super(MultiRecord, self).__init__(
             record_name=record_name,
             n_sig=n_sig,
             fs=fs,
             counter_freq=counter_freq,
             base_counter=base_counter,
             sig_len=sig_len,
@@ -1199,15 +1195,14 @@
         N/A
 
         """
         if self.n_seg != len(self.segments):
             raise ValueError("Length of segments must match the 'n_seg' field")
 
         for seg_num, segment in enumerate(self.segments):
-
             # If segment 0 is a layout specification record, check that its file names are all == '~''
             if seg_num == 0 and self.seg_len[0] == 0:
                 for file_name in segment.file_name:
                     if file_name != "~":
                         raise ValueError(
                             "Layout specification records must have all file_names named '~'"
                         )
@@ -1657,15 +1652,15 @@
 # ---------------------- Type Specifications ------------------------- #
 
 
 # Allowed types of WFDB header fields, and also attributes defined in
 # this library
 ALLOWED_TYPES = dict(
     [
-        [index, _header.FIELD_SPECS.loc[index, "allowed_types"]]
+        (index, _header.FIELD_SPECS.loc[index, "allowed_types"])
         for index in _header.FIELD_SPECS.index
     ]
 )
 ALLOWED_TYPES.update(
     {
         "comments": (str,),
         "p_signal": (np.ndarray,),
```

### Comparing `wfdb-4.1.0/wfdb/io/util.py` & `wfdb-4.1.1/wfdb/io/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A module for general utility functions
 """
 import math
 import os
 
-from typing import Sequence, Tuple
+from typing import List, Sequence, Tuple
 
 
 def lines_to_file(file_name: str, write_dir: str, lines: Sequence[str]):
     """
     Write each line in a list of strings to a text file.
 
     Parameters
@@ -98,16 +98,17 @@
         The rounded up result of <x> up to nearest <base>.
 
     """
     return base * math.ceil(float(x) / base)
 
 
 def overlapping_ranges(
-    ranges_1: Tuple[int, int], ranges_2: Tuple[int, int]
-) -> Tuple[int, int]:
+    ranges_1: Sequence[Tuple[int, int]],
+    ranges_2: Sequence[Tuple[int, int]],
+) -> List[Tuple[int, int]]:
     """
     Given two collections of integer ranges, return a list of ranges
     in which both input inputs overlap.
 
     From: https://stackoverflow.com/q/40367461
 
     Slightly modified so that if the end of one range exactly equals
```

### Comparing `wfdb-4.1.0/wfdb/plot/plot.py` & `wfdb-4.1.1/wfdb/plot/plot.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/processing/__init__.py` & `wfdb-4.1.1/wfdb/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/processing/basic.py` & `wfdb-4.1.1/wfdb/processing/basic.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/processing/evaluate.py` & `wfdb-4.1.1/wfdb/processing/evaluate.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/processing/filter.py` & `wfdb-4.1.1/wfdb/processing/filter.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/processing/hr.py` & `wfdb-4.1.1/wfdb/processing/hr.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,14 @@
     extension,
     pn_dir=None,
     start_time=None,
     stop_time=None,
     format=None,
     as_array=True,
 ):
-
     """
     Obtain RR interval series from ECG annotation files.
 
     Parameters
     ----------
     record_name : str
         The record name of the WFDB annotation file. ie. for file '100.atr',
```

### Comparing `wfdb-4.1.0/wfdb/processing/peaks.py` & `wfdb-4.1.1/wfdb/processing/peaks.py`

 * *Files identical despite different names*

### Comparing `wfdb-4.1.0/wfdb/processing/qrs.py` & `wfdb-4.1.1/wfdb/processing/qrs.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,14 @@
                 noise_amps.append(self.sig_i[i])
 
             if len(qrs_inds) == n_calib_beats:
                 break
 
         # Found enough calibration beats to initialize parameters
         if len(qrs_inds) == n_calib_beats:
-
             if self.verbose:
                 print(
                     "Found %d beats during learning." % n_calib_beats
                     + " Initializing using learned parameters"
                 )
 
             # QRS amplitude is most important.
```

### Comparing `wfdb-4.1.0/PKG-INFO` & `wfdb-4.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: wfdb
-Version: 4.1.0
+Version: 4.1.1
 Summary: The WFDB Python package: tools for reading, writing, and processing physiologic signals and annotations.
 Home-page: https://github.com/MIT-LCP/wfdb-python/
 License: MIT
 Author: The Laboratory for Computational Physiology
 Author-email: contact@physionet.org
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
-Requires-Dist: SoundFile (>=0.10.0,<0.12.0)
-Requires-Dist: Sphinx (>=4.5.0,<5.0.0) ; extra == "dev"
-Requires-Dist: black (>=22.3.0,<23.0.0) ; extra == "dev"
-Requires-Dist: matplotlib (>=3.2.2,<4.0.0)
-Requires-Dist: numpy (>=1.10.1,<2.0.0)
-Requires-Dist: pandas (>=1.0.0,<2.0.0)
-Requires-Dist: pylint (>=2.13.7,<3.0.0) ; extra == "dev"
-Requires-Dist: pytest (>=7.1.1,<8.0.0) ; extra == "dev"
-Requires-Dist: pytest-xdist (>=2.5.0,<3.0.0) ; extra == "dev"
-Requires-Dist: requests (>=2.8.1,<3.0.0)
-Requires-Dist: scipy (>=1.0.0,<2.0.0)
+Requires-Dist: SoundFile (>=0.10.0)
+Requires-Dist: Sphinx (>=4.5.0) ; extra == "dev"
+Requires-Dist: black (>=22.3.0) ; extra == "dev"
+Requires-Dist: matplotlib (>=3.2.2)
+Requires-Dist: numpy (>=1.10.1)
+Requires-Dist: pandas (>=1.3.0)
+Requires-Dist: pylint (>=2.13.7) ; extra == "dev"
+Requires-Dist: pytest (>=7.1.1) ; extra == "dev"
+Requires-Dist: pytest-xdist (>=2.5.0) ; extra == "dev"
+Requires-Dist: requests (>=2.8.1)
+Requires-Dist: scipy (>=1.0.0)
 Project-URL: Documentation, https://wfdb.readthedocs.io/
 Project-URL: Repository, https://github.com/MIT-LCP/wfdb-python/
 Description-Content-Type: text/markdown
 
 # The WFDB Python Package
 
 ![signals](https://raw.githubusercontent.com/MIT-LCP/wfdb-python/main/demo-img.png)
```

