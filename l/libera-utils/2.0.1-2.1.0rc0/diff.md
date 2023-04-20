# Comparing `tmp/libera_utils-2.0.1.tar.gz` & `tmp/libera_utils-2.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libera_utils-2.0.1.tar", max compression
+gzip compressed data, was "libera_utils-2.1.0rc0.tar", max compression
```

## Comparing `libera_utils-2.0.1.tar` & `libera_utils-2.1.0rc0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
--rw-r--r--   0        0        0     1051 2023-02-01 18:21:25.653113 libera_utils-2.0.1/CHANGES.md
--rw-r--r--   0        0        0     1465 2023-01-31 20:56:19.358288 libera_utils-2.0.1/LICENSE
--rw-r--r--   0        0        0     1293 2022-10-12 19:41:52.141872 libera_utils-2.0.1/README.md
--rw-r--r--   0        0        0       54 2023-02-07 21:10:06.403935 libera_utils-2.0.1/libera_utils/__init__.py
--rw-r--r--   0        0        0     4313 2023-01-31 20:56:19.378515 libera_utils-2.0.1/libera_utils/cli.py
--rw-r--r--   0        0        0     4921 2023-01-31 20:56:19.379785 libera_utils-2.0.1/libera_utils/config.py
--rw-r--r--   0        0        0     1940 2023-01-31 20:56:19.381102 libera_utils-2.0.1/libera_utils/data/config.json
--rw-r--r--   0        0        0    14209 2022-09-23 15:27:25.065932 libera_utils-2.0.1/libera_utils/data/jpss1_geolocation_xtce_v1.xml
--rw-r--r--   0        0        0     7522 2022-09-23 15:27:25.067154 libera_utils-2.0.1/libera_utils/data/spice/earth_assoc_itrf93.tf
--rw-r--r--   0        0        0     1608 2022-09-23 15:27:25.068514 libera_utils-2.0.1/libera_utils/data/spice/jpss_sclk_v01.tsc
--rw-r--r--   0        0        0     7990 2022-09-23 15:27:25.069901 libera_utils-2.0.1/libera_utils/data/spice/libera_fk_v01.tf
--rw-r--r--   0        0        0     1359 2023-02-07 21:10:06.406223 libera_utils-2.0.1/libera_utils/db/__init__.py
--rw-r--r--   0        0        0     6127 2023-02-07 21:10:06.407492 libera_utils-2.0.1/libera_utils/db/database.py
--rw-r--r--   0        0        0     3924 2023-01-31 20:56:19.384792 libera_utils-2.0.1/libera_utils/db/mixins.py
--rw-r--r--   0        0        0     7833 2023-01-31 20:56:19.385945 libera_utils-2.0.1/libera_utils/db/models.py
--rw-r--r--   0        0        0    19390 2022-09-23 15:27:25.074690 libera_utils-2.0.1/libera_utils/geolocation.py
--rw-r--r--   0        0        0        0 2022-09-23 15:27:25.074796 libera_utils-2.0.1/libera_utils/io/__init__.py
--rw-r--r--   0        0        0     1581 2022-09-23 15:27:25.076003 libera_utils-2.0.1/libera_utils/io/caching.py
--rw-r--r--   0        0        0    21143 2023-01-31 20:56:19.387716 libera_utils-2.0.1/libera_utils/io/construction_record.py
--rw-r--r--   0        0        0    12108 2023-01-31 20:56:19.389078 libera_utils-2.0.1/libera_utils/io/filenaming.py
--rw-r--r--   0        0        0     1856 2023-01-31 20:56:19.390630 libera_utils-2.0.1/libera_utils/io/hdf.py
--rw-r--r--   0        0        0     5442 2023-01-31 20:56:19.390974 libera_utils-2.0.1/libera_utils/io/manifest.py
--rw-r--r--   0        0        0     6841 2023-01-31 20:56:19.391242 libera_utils-2.0.1/libera_utils/io/smart_open.py
--rw-r--r--   0        0        0    17103 2023-01-31 20:56:19.391610 libera_utils-2.0.1/libera_utils/kernel_maker.py
--rw-r--r--   0        0        0     6239 2023-01-31 20:56:19.393238 libera_utils-2.0.1/libera_utils/logutil.py
--rw-r--r--   0        0        0     3464 2023-01-31 20:56:19.393539 libera_utils-2.0.1/libera_utils/packets.py
--rw-r--r--   0        0        0     8496 2023-01-31 20:56:19.393760 libera_utils-2.0.1/libera_utils/quality_flags.py
--rw-r--r--   0        0        0    17074 2022-09-23 15:27:25.084642 libera_utils-2.0.1/libera_utils/spice_utils.py
--rw-r--r--   0        0        0     7428 2023-01-31 20:56:19.394993 libera_utils-2.0.1/libera_utils/time.py
--rw-r--r--   0        0        0      203 2022-09-23 15:27:25.087434 libera_utils-2.0.1/libera_utils/version.py
--rw-r--r--   0        0        0     1516 2023-02-08 00:05:35.486467 libera_utils-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 libera_utils-2.0.1/setup.py
--rw-r--r--   0        0        0     1059 1970-01-01 00:00:00.000000 libera_utils-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1410 2023-04-20 20:33:03.948878 libera_utils-2.1.0rc0/CHANGES.md
+-rw-r--r--   0        0        0     1465 2023-01-31 20:56:19.358288 libera_utils-2.1.0rc0/LICENSE
+-rw-r--r--   0        0        0     1416 2023-04-03 23:48:10.022450 libera_utils-2.1.0rc0/README.md
+-rw-r--r--   0        0        0       54 2023-02-07 21:10:06.403935 libera_utils-2.1.0rc0/libera_utils/__init__.py
+-rw-r--r--   0        0        0       95 2023-04-20 20:30:46.629417 libera_utils-2.1.0rc0/libera_utils/backports/__init__.py
+-rw-r--r--   0        0        0    78894 2023-04-20 20:30:46.630392 libera_utils-2.1.0rc0/libera_utils/backports/enum_3_11.py
+-rw-r--r--   0        0        0     5124 2023-04-03 23:48:10.023492 libera_utils-2.1.0rc0/libera_utils/cli.py
+-rw-r--r--   0        0        0     4916 2023-04-03 23:48:10.023746 libera_utils-2.1.0rc0/libera_utils/config.py
+-rw-r--r--   0        0        0     1940 2023-01-31 20:56:19.381102 libera_utils-2.1.0rc0/libera_utils/data/config.json
+-rw-r--r--   0        0        0    14209 2022-09-23 15:27:25.065932 libera_utils-2.1.0rc0/libera_utils/data/jpss1_geolocation_xtce_v1.xml
+-rw-r--r--   0        0        0     7522 2022-09-23 15:27:25.067154 libera_utils-2.1.0rc0/libera_utils/data/spice/earth_assoc_itrf93.tf
+-rw-r--r--   0        0        0     1608 2022-09-23 15:27:25.068514 libera_utils-2.1.0rc0/libera_utils/data/spice/jpss_sclk_v01.tsc
+-rw-r--r--   0        0        0     7990 2022-09-23 15:27:25.069901 libera_utils-2.1.0rc0/libera_utils/data/spice/libera_fk_v01.tf
+-rw-r--r--   0        0        0     1359 2023-02-07 21:10:06.406223 libera_utils-2.1.0rc0/libera_utils/db/__init__.py
+-rw-r--r--   0        0        0     6127 2023-02-07 21:10:06.407492 libera_utils-2.1.0rc0/libera_utils/db/database.py
+-rw-r--r--   0        0        0     3924 2023-01-31 20:56:19.384792 libera_utils-2.1.0rc0/libera_utils/db/mixins.py
+-rw-r--r--   0        0        0     7833 2023-01-31 20:56:19.385945 libera_utils-2.1.0rc0/libera_utils/db/models.py
+-rw-r--r--   0        0        0    19390 2022-09-23 15:27:25.074690 libera_utils-2.1.0rc0/libera_utils/geolocation.py
+-rw-r--r--   0        0        0        0 2022-09-23 15:27:25.074796 libera_utils-2.1.0rc0/libera_utils/io/__init__.py
+-rw-r--r--   0        0        0     1581 2022-09-23 15:27:25.076003 libera_utils-2.1.0rc0/libera_utils/io/caching.py
+-rw-r--r--   0        0        0    21721 2023-04-03 23:48:10.024153 libera_utils-2.1.0rc0/libera_utils/io/construction_record.py
+-rw-r--r--   0        0        0    32093 2023-04-20 20:30:46.631652 libera_utils-2.1.0rc0/libera_utils/io/filenaming.py
+-rw-r--r--   0        0        0     1856 2023-01-31 20:56:19.390630 libera_utils-2.1.0rc0/libera_utils/io/hdf.py
+-rw-r--r--   0        0        0     8596 2023-04-03 23:48:10.025919 libera_utils-2.1.0rc0/libera_utils/io/manifest.py
+-rw-r--r--   0        0        0     7380 2023-04-03 23:48:10.026152 libera_utils-2.1.0rc0/libera_utils/io/packet_ingest.py
+-rw-r--r--   0        0        0     7262 2023-04-03 23:48:10.026427 libera_utils-2.1.0rc0/libera_utils/io/smart_open.py
+-rw-r--r--   0        0        0    17414 2023-04-20 20:30:46.633307 libera_utils-2.1.0rc0/libera_utils/kernel_maker.py
+-rw-r--r--   0        0        0     6239 2023-01-31 20:56:19.393238 libera_utils-2.1.0rc0/libera_utils/logutil.py
+-rw-r--r--   0        0        0     3417 2023-04-03 23:48:10.027250 libera_utils-2.1.0rc0/libera_utils/packets.py
+-rw-r--r--   0        0        0     4620 2023-04-20 20:30:46.634535 libera_utils-2.1.0rc0/libera_utils/quality_flags.py
+-rw-r--r--   0        0        0    17074 2022-09-23 15:27:25.084642 libera_utils-2.1.0rc0/libera_utils/spice_utils.py
+-rw-r--r--   0        0        0     7482 2023-04-20 20:30:46.635212 libera_utils-2.1.0rc0/libera_utils/time.py
+-rw-r--r--   0        0        0      203 2022-09-23 15:27:25.087434 libera_utils-2.1.0rc0/libera_utils/version.py
+-rw-r--r--   0        0        0     1525 2023-04-20 20:46:20.133500 libera_utils-2.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1436 1970-01-01 00:00:00.000000 libera_utils-2.1.0rc0/setup.py
+-rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 libera_utils-2.1.0rc0/PKG-INFO
```

### Comparing `libera_utils-2.0.1/CHANGES.md` & `libera_utils-2.1.0rc0/CHANGES.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Version Changes
 
+# 2.1.0 (released)
+- Improve API to Manifest and Manifest.add_files
+- Add manifest filename enforcement to Manifest class
+- Update filenaming conventions for product filenames and SPICE kernels
+- Allow adding an s3 bucket/prefix as a basepath for filenames
+
+# 2.0.1 (released)
+- Remove the extras dependency spec because of the way SQLAlchemy imports models
+
 # 2.0.0 (released)
 - Add filenaming classes
 - Add manifest file class
 - Add construction record parser
 - Update DB schema to store construction records
 - Update kernel generation CLI to use manifest file pattern
 - Shift database and spice related libraries to extras (not installed by default)
```

### Comparing `libera_utils-2.0.1/LICENSE` & `libera_utils-2.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/README.md` & `libera_utils-2.1.0rc0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -40,7 +40,13 @@
 
 
 #### Sub-Command `libera-utils make-kernel azel-ck`
 Not yet implemented
 ```shell
 libera-utils make-kernel azel-ck [-h]
 ```
+
+
+#### Sub-Command `packet-ingest input-manifest.json`
+```shell
+libera-utils packet-ingest [-h] [packet_data_filepath]
+```
```

### Comparing `libera_utils-2.0.1/libera_utils/cli.py` & `libera_utils-2.1.0rc0/libera_utils/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,27 +6,28 @@
         jpss-ck
         azel-ck
 """
 # Standard
 import argparse
 # Local
 from libera_utils import kernel_maker
+from libera_utils.io import packet_ingest
 from libera_utils.version import version as libera_utils_version
 
 
 def main(cli_args: list = None):
     """Main CLI entrypoint that runs the function inferred from the specified subcommand"""
     args = parse_cli_args(cli_args)
     args.func(args)
 
 
 def print_version_info(*args):
     """Print CLI version information"""
     print(f"Libera SDC utilities CLI\n\tVersion {libera_utils_version()}"
-          f"\n\tCopyright 2022 University of Colorado\n\tReleased under BSD3 license")
+          f"\n\tCopyright 2023 University of Colorado\n\tReleased under BSD3 license")
 
 
 def parse_cli_args(cli_args: list):
     """Parse CLI arguments
 
     Parameters
     ----------
@@ -41,14 +42,24 @@
     parser = argparse.ArgumentParser(prog="libera-utils", description="Libera SDC utilities CLI")
     parser.add_argument("--version",
                         action='store_const', dest='func', const=print_version_info,
                         help="print current version of the CLI")
 
     subparsers = parser.add_subparsers(description="sub-commands for libera-utils CLI")
 
+    # packet-ingest
+    packet_ingest_parser = subparsers.add_parser('packet-ingest',
+                                                 help='write construction record data to database')
+    packet_ingest_parser.set_defaults(func=packet_ingest.ingest)
+    packet_ingest_parser.add_argument('manifest_filepath', type=str,
+                                      help="path to L0 manifest file")
+    packet_ingest_parser.add_argument('-d', '--delete', action='store_false',
+                                      help='Deletes data files from s3 bucket once they are moved.')
+    packet_ingest_parser.add_argument('-v', '--verbose', action='store_true',
+                                      help="set DEBUG level logging output (otherwise set by LIBERA_CONSOLE_LOG_LEVEL)")
     # make-kernel
     make_kernel_parser = subparsers.add_parser('make-kernel',
                                                help='generate SPICE kernel from telemetry data')
 
     make_kernel_subparsers = make_kernel_parser.add_subparsers(description="sub-commands for make-kernel sub-command")
 
     # make-kernel jpss-spk
```

### Comparing `libera_utils-2.0.1/libera_utils/config.py` & `libera_utils-2.1.0rc0/libera_utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Configuration reader. To modify the configuration, see file: emus_config.json"""
+"""Configuration reader. To modify the configuration, see file: config.json"""
 # Standard
 import json
 import logging
 import os
 from pathlib import Path
 import re
 import string
```

### Comparing `libera_utils-2.0.1/libera_utils/data/config.json` & `libera_utils-2.1.0rc0/libera_utils/data/config.json`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/libera_utils/data/jpss1_geolocation_xtce_v1.xml` & `libera_utils-2.1.0rc0/libera_utils/data/jpss1_geolocation_xtce_v1.xml`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/libera_utils/data/spice/earth_assoc_itrf93.tf` & `libera_utils-2.1.0rc0/libera_utils/data/spice/earth_assoc_itrf93.tf`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/libera_utils/data/spice/jpss_sclk_v01.tsc` & `libera_utils-2.1.0rc0/libera_utils/data/spice/jpss_sclk_v01.tsc`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/libera_utils/data/spice/libera_fk_v01.tf` & `libera_utils-2.1.0rc0/libera_utils/data/spice/libera_fk_v01.tf`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/libera_utils/db/__init__.py` & `libera_utils-2.1.0rc0/libera_utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/libera_utils/db/database.py` & `libera_utils-2.1.0rc0/libera_utils/db/database.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/libera_utils/db/mixins.py` & `libera_utils-2.1.0rc0/libera_utils/db/mixins.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/libera_utils/db/models.py` & `libera_utils-2.1.0rc0/libera_utils/db/models.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/libera_utils/geolocation.py` & `libera_utils-2.1.0rc0/libera_utils/geolocation.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/libera_utils/io/caching.py` & `libera_utils-2.1.0rc0/libera_utils/io/caching.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/libera_utils/io/construction_record.py` & `libera_utils-2.1.0rc0/libera_utils/io/construction_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Module for manifest file handling"""
 # Standard
+import datetime
 import logging
 from pathlib import Path
 from bitstring import ConstBitStream
 # Installed
 from cloudpathlib import S3Path, AnyPath
 # Local
 from libera_utils.io.smart_open import smart_open
@@ -111,14 +112,30 @@
                 first_packet_sc_time=self.apid_first_packet_sc_time,
                 last_packet_sc_time=self.apid_last_packet_sc_time,
                 first_packet_utc_time=self.apid_first_packet_utc,
                 last_packet_utc_time=self.apid_last_packet_utc
             )
 
 
+class PDSRecord:
+    """
+    Object representation of a Production Data Set (PDS). This object is created as part of
+    reading in a PDS filename and storing that filename and ingest time in a database.
+    """
+    def __init__(self, pds_filename: str):
+        self.pds_filename = pds_filename
+
+    def to_orm(self):
+        """Convert this class instance to a corresponding ORM object for entry into the database"""
+        return libera_db_models.PdsFile(
+            file_name=self.pds_filename,
+            ingested=datetime.datetime.utcnow()
+        )
+
+
 class PDSFileFromConstructionRecord:
     """
     Object representation of the information directly related to a Production Data Set (PDS). This corresponds to a
     database table and connects to a Construction Record (CR). This object is created as part of reading in a CR and
     requires an open bitstream to read from.
     """
     def __init__(self, cr_bitstream: ConstBitStream):
@@ -144,15 +161,15 @@
             apids=apids_list
         )
 
 
 class SSCGapInformationFromConstructionRecord:
     """
     Object representation of the information of Spacecraft Contact Sessions (SCS). This corresponds to a database table
-    and connects to a Construction Record (CR). This object iscreated as part of reading in a CR and thus requires an
+    and connects to a Construction Record (CR). This object is created as part of reading in a CR and thus requires an
     open bitstream to read from.
     """
     def __init__(self, cr_bitstream: ConstBitStream):
         self.apid_gap_first_missing_ssc_packet = cr_bitstream.read("uint:32")
         self.apid_gap_byte_offset = cr_bitstream.read("uint:64")
         self.apid_num_ssc_packets_missed = cr_bitstream.read("uint:32")
 
@@ -430,16 +447,16 @@
         scs_start_stops = []
         for i in range(self.scs_num_start_stop_times):
             scs_start_stops.append(self.scs_start_stop_times_list[i].to_orm())
         apids = []
         for i in range(self.apid_count):
             apids.append(self.apid_data_list[i].to_orm())
         pds_files = []
-        for i in range(self.pds_file_count):
-            pds_files.append(self.pds_files_list[i].to_orm())
+        for i, pds_file in enumerate(self.pds_files_list):
+            pds_files.append(pds_file.to_orm())
         return libera_db_models.Cr(
             file_name=self.file_name,
             edos_software_version=self.edos_version,
             construction_record_type=self.construction_record_type,
             test_flag=self.test_flag,
             n_scs_start_stops=self.scs_num_start_stop_times,
             scs_start_stop_times=scs_start_stops,
```

### Comparing `libera_utils-2.0.1/libera_utils/io/hdf.py` & `libera_utils-2.1.0rc0/libera_utils/io/hdf.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/libera_utils/io/smart_open.py` & `libera_utils-2.1.0rc0/libera_utils/io/smart_open.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,27 +95,29 @@
     if isinstance(path, (Path, S3Path)):
         return _gzip_wrapper(path.open(mode=mode))
 
     # AnyPath is polymorphic to Path and S3Path. Disable false pylint error
     return _gzip_wrapper(AnyPath(path).open(mode=mode))  # pylint: disable=E1101
 
 
-def smart_copy_file(source_path: str or Path or S3Path, dest_path: str or Path or S3Path):
+def smart_copy_file(source_path: str or Path or S3Path, dest_path: str or Path or S3Path, delete=False):
     """
         Copy function that can handle local files or files in an S3 bucket.
         Returns the path to the newly created file.
 
         Parameters
         ----------
         source_path : str or Path or S3Path
             Path to the source file to be copied. Files residing in an s3 bucket must begin
             with "s3://".
-        dest_path: str or Path or S3Path
+        dest_path : str or Path or S3Path
             Path to the Destination file to be copied to. Files residing in an s3 bucket
             must begin with "s3://".
+        delete : bool
+            If true, deletes files copied from source (default = False)
 
         Returns
         -------
         : Path or S3Path
             The path to the newly created file
         """
     if not is_s3(source_path) and not is_s3(dest_path):
@@ -126,14 +128,17 @@
         # Warning if no suffix is used in destination.
         if len(local_dest_path.suffix) == 0:
             warnings.warn(f'You have copied to a location without a file extension.'
                           f'Source location: {local_source_path} to destination:'
                           f'{local_dest_path}.')
 
         # Returns a PosixPath of the newly created file
+        if delete:
+            return shutil.move(source_path, dest_path)
+
         return shutil.copy(source_path, dest_path)
 
     # Check if either source or destination is remote and allocate remote resources
     s3 = boto3.resource("s3")
     client = boto3.client("s3")
 
     if is_s3(dest_path) and not is_s3(source_path):
@@ -145,14 +150,16 @@
         if len(s3_dest_path.suffix) == 0:
             warnings.warn(f'You have copied a file to S3 without a file extension.'
                           f'Source location: {local_source_path} to S3 location:'
                           f'{s3_dest_path}.')
 
         # Has no return, but will raise exceptions on problems
         s3.Bucket(s3_dest_path.bucket).upload_file(str(local_source_path), s3_dest_path.key)
+        if delete:
+            local_source_path.unlink()
         return s3_dest_path
 
     if is_s3(source_path) and not is_s3(dest_path):
         # This is a remote to local copy and uses S3 download
         s3_source_path = S3Path(source_path)
         local_dest_path = Path(dest_path)
 
@@ -167,14 +174,16 @@
         if len(local_dest_path.suffix) == 0:
             warnings.warn(f'You have copied a file without a file extension.'
                           f'Source: {s3_source_path} to destination:'
                           f'{local_dest_path}.')
 
         # Has no return, but will raise exceptions on problems
         s3.Bucket(s3_source_path.bucket).download_file(s3_source_path.key, str(local_dest_path))
+        if delete:
+            s3.Object(s3_source_path.bucket, s3_source_path.key).delete()
         return Path(local_dest_path)
 
     # This is a remote to remote copy and uses S3 copy
     s3_source_path = S3Path(source_path)
     s3_dest_path = S3Path(dest_path)
 
     copy_source = {
@@ -186,8 +195,11 @@
     if len(s3_dest_path.suffix) == 0:
         warnings.warn(f'You have copied a file to S3 without a file extension.'
                       f'Source location: {s3_source_path} to S3 location:'
                       f'{s3_dest_path}.')
 
     # Has no return, but will raise exceptions
     client.copy(copy_source, s3_dest_path.bucket, s3_dest_path.key)
+
+    if delete:
+        s3.Object(copy_source['Bucket'], copy_source['Key']).delete()
     return s3_dest_path
```

### Comparing `libera_utils-2.0.1/libera_utils/kernel_maker.py` & `libera_utils-2.1.0rc0/libera_utils/kernel_maker.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     """
     # TODO: Consider cases to return/error if the entire range is not covered
 
     m = Manifest.from_file(manifest_file_path)
     m.validate_checksums()
     files_in_range = []
 
-    if "start_time" not in m.configuration.keys():
+    if "start_time" not in m.configuration:
         # No time range information is provided. Process all files in the manifest
         for file_entry in m.files:
             files_in_range.append(str(file_entry["filename"]))
     else:
         # Load desired time range from the manifest configuration
         start_time_text = m.configuration["start_time"]
         desired_start_time = datetime.strptime(start_time_text, '%Y-%m-%d:%H:%M:%S')
@@ -126,14 +126,15 @@
 
     packet_parser = parser.PacketParser(packet_definition=packet_definition)
 
     packet_data = libera_packets.parse_packets(packet_parser, packet_data_filepaths)
 
     return packet_data
 
+
 def make_jpss_spk(parsed_args: argparse.Namespace):
     """Create a JPSS SPK from APID 11 CCSDS packets.
 
     Parameters
     ----------
     parsed_args : argparse.Namespace
         Namespace of parsed CLI arguments
@@ -173,18 +174,23 @@
         logger.info("MKSPK input data written to %s", spk_data_filepath)
 
         spk_setup_filepath = write_kernel_setup_file(
             config.get("MKSPK_SETUPFILE_CONTENTS"),
             filepath=tmp_path / 'mkspk_setup.txt')
         logger.info("MKSPK setup file written to %s", spk_setup_filepath)
 
-        utc_start_str = time.et_2_datetime(ephemeris_time[0])
-        utc_end_str = time.et_2_datetime(ephemeris_time[-1])
+        utc_start = time.et_2_datetime(ephemeris_time[0])
+        utc_end = time.et_2_datetime(ephemeris_time[-1])
+        revision_time = datetime.utcnow()
         spk_filename = filenaming.EphemerisKernelFilename.from_filename_parts(
-            spk_object='jpss', utc_start=utc_start_str, utc_end=utc_end_str)
+            spk_object='jpss',
+            utc_start=utc_start,
+            utc_end=utc_end,
+            version=filenaming.get_current_version_str('libera_utils'),
+            revision=revision_time)
         output_filepath = tmp_path / spk_filename.path.name  # pylint: disable=no-member
 
         if parsed_args.overwrite is True:
             output_filepath.unlink(missing_ok=True)
 
         logger.info("Running MKSPK...")
         try:
@@ -252,18 +258,23 @@
         logger.info("MSOPCK input data written to %s", ck_data_filepath)
 
         ck_setup_filepath = write_kernel_setup_file(
             config.get("MSOPCK_SETUPFILE_CONTENTS"),
             filepath=tmp_path / 'msopck_setup.txt')
         logger.info("MSOPCK setup file written to %s", ck_setup_filepath)
 
-        utc_start_str = time.et_2_datetime(time.scs2e_wrapper(attitude_sclk_string[0]))
-        utc_end_str = time.et_2_datetime(time.scs2e_wrapper(attitude_sclk_string[-1]))
+        utc_start = time.et_2_datetime(time.scs2e_wrapper(attitude_sclk_string[0]))
+        utc_end = time.et_2_datetime(time.scs2e_wrapper(attitude_sclk_string[-1]))
+        revision_time = datetime.utcnow()
         ck_filename = filenaming.AttitudeKernelFilename.from_filename_parts(
-            ck_object='jpss', utc_start=utc_start_str, utc_end=utc_end_str)
+            ck_object='jpss',
+            utc_start=utc_start,
+            utc_end=utc_end,
+            version=filenaming.get_current_version_str('libera_utils'),
+            revision=revision_time)
         output_filepath = tmp_path / ck_filename.path.name  # pylint: disable=no-member
 
         if parsed_args.overwrite is True:
             output_filepath.unlink(missing_ok=True)
 
         logger.info("Running MSOPCK...")
         try:
@@ -283,14 +294,15 @@
 
         output_full_path = output_dir / ck_filename.path.name  # pylint: disable=no-member
         # Use smart copy here to avoiding using two nested smart_open calls
         # one call would be to open the newly created file, and one to open the desired location
         smart_copy_file(output_filepath, output_full_path)
         logger.info("CK copied to %s", output_full_path)
 
+
 def make_azel_ck(parsed_args: argparse.Namespace):
     """Create a Libera Az-El CK from CCSDS packets
 
     Parameters
     ----------
     parsed_args : argparse.Namespace
         Namespace of parsed CLI arguments
```

### Comparing `libera_utils-2.0.1/libera_utils/logutil.py` & `libera_utils-2.1.0rc0/libera_utils/logutil.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/libera_utils/packets.py` & `libera_utils-2.1.0rc0/libera_utils/packets.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Local
 from libera_utils.io.smart_open import smart_open
 
 logger = logging.getLogger(__name__)
 
 
 def array_from_packets(packets: list, apid: int = None):
-    """Create an array from a packet generator, as returned from a lasp_packets PacketParser. This function assumes
+    """Create an array from a list of packets. This function assumes
     that the fields and format for every packet is identical for a given APID.
 
     Parameters
     ----------
     packets : list
         List of lasp_packets.parser.Packet objects.
     apid : int
```

### Comparing `libera_utils-2.0.1/libera_utils/spice_utils.py` & `libera_utils-2.1.0rc0/libera_utils/spice_utils.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.0.1/libera_utils/time.py` & `libera_utils-2.1.0rc0/libera_utils/time.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 3. All functions should have robust type-hinting.
 """
 # Standard
 import re
 from datetime import datetime, timedelta
 from typing import Union, Collection
-import pytz
+from zoneinfo import ZoneInfo
 # Installed
 import numpy as np
 import spiceypy as spice
 # Local
 from libera_utils.config import config
 from libera_utils.spice_utils import ensure_spice
 
@@ -29,14 +29,16 @@
 
 PRINTABLE_TS_REGEX = re.compile(r"^(?P<year>[0-9]{4})(?P<month>[0-9]{2})(?P<day>[0-9]{2})"
                                 r"[T|t]"
                                 r"(?P<hour>[0-9]{2})(?P<minute>[0-9]{2})(?P<second>[0-9]{2})$")
 
 PRINTABLE_TS_FORMAT = "%Y%m%dt%H%M%S"
 
+EDOS_TS_FORMAT = "%y%j%H%M%S"
+
 
 def et_2_timestamp(et: Union[float, Collection[float], np.ndarray],
                    fmt: str = '%Y%m%dt%H%M%S.%f') -> Union[str, Collection[str]]:
     """
     Convert ephemeris time to a custom formatted timestamp (default is lowercase version of ISO).
 
     Parameters
@@ -184,31 +186,31 @@
     return spice.sce2s(sc_id, et)
 
 
 def convert_cds_integer_to_datetime(satellite_time: int):
     """Helper function to convert a satellite time given as an CCSDS Day Segmented Time Code (CDS) form as 8 byte
     integer to a timezone aware datetime object
 
-     Parameters
+    Parameters
     ----------
     satellite_time : int
         A 64-bit unsigned integer that represents CDS time
 
-     Returns
+    Returns
     -------
     cds_time : datetime
      """
     byte_data = satellite_time.to_bytes(8, 'big')
     int_days = int.from_bytes([byte_data[0], byte_data[1]], byteorder="big")
     int_millisec = int.from_bytes([byte_data[2], byte_data[3],
                                     byte_data[4], byte_data[5]],
                                    byteorder="big")
     int_microsec = int.from_bytes([byte_data[6], byte_data[7]], byteorder="big")
 
-    reference_date = datetime(1958, 1, 1, 0, 0, 0, 0, pytz.UTC)
+    reference_date = datetime(1958, 1, 1, 0, 0, 0, 0, ZoneInfo("UTC"))
     cds_time = (reference_date +
                 timedelta(days=int_days) +
                 timedelta(milliseconds=int_millisec) +
                 timedelta(microseconds=int_microsec))
 
     # TODO: Check with EDOS on this time conversion. The commented out below gives approximately a 70 second difference
     # TODO: to the method above.
```

### Comparing `libera_utils-2.0.1/pyproject.toml` & `libera_utils-2.1.0rc0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "libera_utils"
-version = "2.0.1"
+version = "2.1.0rc"
 description = "Utility package for Libera Science Data Processing and the Libera Science Data Center. Copyright 2022 University of Colorado."
 authors = [  # Alphabetical
     "Stephane Beland <stephane.beland@lasp.colorado.edu>",
     "Gavin Medley <gavin.medley@lasp.colorado.edu>",
     "Laura Sandoval <laura.sandoval@lasp.colorado.edu>",
     "Matt Watwood <matt.watwood@lasp.colorado.edu>"
 ]
 license = "BSD-3-Clause"
 include = ["CHANGES.md", "LICENSE", "README.md"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.8,<3.12"
 astropy = "^5.1"
 cloudpathlib = {extras = ["s3"], version = "^0"}
 h5netcdf = "^1.1.0"
 h5py = "^3.3"
 lasp-packets = "^2.0"
 numpy = "^1.21"
 psycopg2 = "^2.9"
```

### Comparing `libera_utils-2.0.1/setup.py` & `libera_utils-2.1.0rc0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['libera_utils', 'libera_utils.db', 'libera_utils.io']
+['libera_utils', 'libera_utils.backports', 'libera_utils.db', 'libera_utils.io']
 
 package_data = \
 {'': ['*'],
  'libera_utils': ['data/config.json',
                   'data/config.json',
                   'data/jpss1_geolocation_xtce_v1.xml',
                   'data/jpss1_geolocation_xtce_v1.xml',
@@ -28,24 +28,24 @@
  'xarray>=2023.1.0,<2024.0.0']
 
 entry_points = \
 {'console_scripts': ['libera-utils = libera_utils.cli:main']}
 
 setup_kwargs = {
     'name': 'libera-utils',
-    'version': '2.0.1',
+    'version': '2.1.0rc0',
     'description': 'Utility package for Libera Science Data Processing and the Libera Science Data Center. Copyright 2022 University of Colorado.',
     'long_description': 'None',
     'author': 'Stephane Beland',
     'author_email': 'stephane.beland@lasp.colorado.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `libera_utils-2.0.1/PKG-INFO` & `libera_utils-2.1.0rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: libera-utils
-Version: 2.0.1
+Version: 2.1.0rc0
 Summary: Utility package for Libera Science Data Processing and the Libera Science Data Center. Copyright 2022 University of Colorado.
 License: BSD-3-Clause
 Author: Stephane Beland
 Author-email: stephane.beland@lasp.colorado.edu
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy (>=1.4,<2.0)
 Requires-Dist: astropy (>=5.1,<6.0)
 Requires-Dist: cloudpathlib[s3] (>=0,<1)
 Requires-Dist: h5netcdf (>=1.1.0,<2.0.0)
```

