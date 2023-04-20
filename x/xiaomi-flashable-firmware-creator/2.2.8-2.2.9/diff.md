# Comparing `tmp/xiaomi_flashable_firmware_creator-2.2.8.tar.gz` & `tmp/xiaomi_flashable_firmware_creator-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaomi_flashable_firmware_creator-2.2.8.tar", max compression
+gzip compressed data, was "xiaomi_flashable_firmware_creator-2.2.9.tar", max compression
```

## Comparing `xiaomi_flashable_firmware_creator-2.2.8.tar` & `xiaomi_flashable_firmware_creator-2.2.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    35149 2020-10-17 08:57:59.550682 xiaomi_flashable_firmware_creator-2.2.8/LICENSE
--rw-r--r--   0        0        0     3256 2020-10-17 14:39:50.525077 xiaomi_flashable_firmware_creator-2.2.8/README.md
--rw-r--r--   0        0        0     1311 2022-09-20 09:34:44.769744 xiaomi_flashable_firmware_creator-2.2.8/pyproject.toml
--rw-r--r--   0        0        0      129 2020-10-17 08:57:59.550682 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/__init__.py
--rw-r--r--   0        0        0      182 2022-06-11 18:24:22.066127 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/__main__.py
--rw-r--r--   0        0        0   190444 2021-01-09 17:19:46.555339 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/binaries/update-binary
--rw-r--r--   0        0        0       30 2020-10-17 08:57:59.550682 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/__init__.py
--rw-r--r--   0        0        0     2245 2022-06-11 18:22:58.051897 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/handlers/android_one_zip.py
--rw-r--r--   0        0        0      457 2021-01-09 17:19:46.555339 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/handlers/base_handler.py
--rw-r--r--   0        0        0      253 2022-06-11 18:22:18.301499 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/handlers/standard_zip.py
--rw-r--r--   0        0        0       97 2021-01-08 12:58:59.551940 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/.git
--rw-r--r--   0        0        0        6 2021-01-08 12:58:59.558607 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/.gitignore
--rw-r--r--   0        0        0     1061 2022-06-11 20:02:04.580235 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/LICENSE
--rw-r--r--   0        0        0      834 2022-01-25 08:20:32.235678 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/README.md
--rw-r--r--   0        0        0     5202 2022-09-20 09:35:18.529607 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/extract_android_ota_payload.cpython-310.pyc
--rw-r--r--   0        0        0     4918 2021-01-13 18:52:26.555537 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/extract_android_ota_payload.cpython-38.pyc
--rw-r--r--   0        0        0     5184 2022-09-20 09:21:29.076220 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/extract_android_ota_payload.cpython-39.pyc
--rw-r--r--   0        0        0    29805 2022-09-20 09:35:18.536273 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/update_metadata_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    16209 2021-01-13 18:52:26.562204 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/update_metadata_pb2.cpython-38.pyc
--rw-r--r--   0        0        0    19447 2022-09-20 09:21:29.082886 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/update_metadata_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     5047 2022-06-11 20:15:29.908908 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/extract_android_ota_payload.py
--rw-r--r--   0        0        0       16 2021-01-08 12:58:59.558607 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/requirements.txt
--rw-r--r--   0        0        0    53263 2022-06-11 20:15:29.908908 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/update_metadata_pb2.py
--rw-r--r--   0        0        0     2934 2022-06-11 18:22:53.665185 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/zip_extractor.py
--rw-r--r--   0        0        0    18464 2022-09-20 09:31:38.291697 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/firmware_creator.py
--rw-r--r--   0        0        0       56 2020-10-17 08:57:59.554015 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/helpers/__init__.py
--rw-r--r--   0        0        0     2313 2022-09-20 09:30:32.612143 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/helpers/misc.py
--rw-r--r--   0        0        0     1812 2022-06-11 18:22:18.431500 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/helpers/mock_zip.py
--rw-r--r--   0        0        0      254 2022-06-11 20:26:51.829607 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/templates/partition_flashing
--rwxr-xr-x   0        0        0     1872 2021-01-09 17:19:46.555339 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/templates/recovery_ab_update-binary
--rw-r--r--   0        0        0      214 2021-01-09 17:19:46.555339 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/templates/recovery_ab_updater_script
--rw-r--r--   0        0        0      202 2021-01-09 17:19:46.555339 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/templates/recovery_updater_script
--rw-r--r--   0        0        0      643 2020-10-17 08:57:59.557349 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/types.py
--rw-r--r--   0        0        0     1640 2022-06-11 18:22:18.438166 xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/xiaomi_flashable_firmware_creator.py
--rw-r--r--   0        0        0     4643 1970-01-01 00:00:00.000000 xiaomi_flashable_firmware_creator-2.2.8/setup.py
--rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 xiaomi_flashable_firmware_creator-2.2.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-10-17 08:57:59.550682 xiaomi_flashable_firmware_creator-2.2.9/LICENSE
+-rw-r--r--   0        0        0     3256 2020-10-17 14:39:50.525077 xiaomi_flashable_firmware_creator-2.2.9/README.md
+-rw-r--r--   0        0        0     1321 2022-11-23 08:35:57.245389 xiaomi_flashable_firmware_creator-2.2.9/pyproject.toml
+-rw-r--r--   0        0        0      129 2020-10-17 08:57:59.550682 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/__init__.py
+-rw-r--r--   0        0        0      182 2022-06-11 18:24:22.066127 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/__main__.py
+-rw-r--r--   0        0        0   190444 2021-01-09 17:19:46.555339 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/binaries/update-binary
+-rw-r--r--   0        0        0       30 2020-10-17 08:57:59.550682 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/__init__.py
+-rw-r--r--   0        0        0     2245 2022-06-11 18:22:58.051897 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/handlers/android_one_zip.py
+-rw-r--r--   0        0        0      457 2021-01-09 17:19:46.555339 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/handlers/base_handler.py
+-rw-r--r--   0        0        0      253 2022-06-11 18:22:18.301499 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/handlers/standard_zip.py
+-rw-r--r--   0        0        0       97 2021-01-08 12:58:59.551940 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/.git
+-rw-r--r--   0        0        0        6 2021-01-08 12:58:59.558607 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/.gitignore
+-rw-r--r--   0        0        0     1061 2022-06-11 20:02:04.580235 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/LICENSE
+-rw-r--r--   0        0        0      834 2022-01-25 08:20:32.235678 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/README.md
+-rw-r--r--   0        0        0     5202 2022-09-20 09:35:18.529607 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/extract_android_ota_payload.cpython-310.pyc
+-rw-r--r--   0        0        0     4918 2021-01-13 18:52:26.555537 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/extract_android_ota_payload.cpython-38.pyc
+-rw-r--r--   0        0        0     5184 2022-09-20 09:21:29.076220 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/extract_android_ota_payload.cpython-39.pyc
+-rw-r--r--   0        0        0    29805 2022-09-20 09:35:18.536273 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/update_metadata_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0    16209 2021-01-13 18:52:26.562204 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/update_metadata_pb2.cpython-38.pyc
+-rw-r--r--   0        0        0    19447 2022-09-20 09:21:29.082886 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/update_metadata_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     5047 2022-06-11 20:15:29.908908 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/extract_android_ota_payload.py
+-rw-r--r--   0        0        0       16 2021-01-08 12:58:59.558607 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/requirements.txt
+-rw-r--r--   0        0        0    53263 2022-06-11 20:15:29.908908 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/update_metadata_pb2.py
+-rw-r--r--   0        0        0     2934 2022-06-11 18:22:53.665185 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/zip_extractor.py
+-rw-r--r--   0        0        0    18464 2022-09-20 09:31:38.291697 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/firmware_creator.py
+-rw-r--r--   0        0        0       56 2020-10-17 08:57:59.554015 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/helpers/__init__.py
+-rw-r--r--   0        0        0     2313 2022-09-20 09:30:32.612143 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/helpers/misc.py
+-rw-r--r--   0        0        0     1812 2022-06-11 18:22:18.431500 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/helpers/mock_zip.py
+-rw-r--r--   0        0        0      254 2022-06-11 20:26:51.829607 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/templates/partition_flashing
+-rwxr-xr-x   0        0        0     1872 2021-01-09 17:19:46.555339 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/templates/recovery_ab_update-binary
+-rw-r--r--   0        0        0      214 2021-01-09 17:19:46.555339 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/templates/recovery_ab_updater_script
+-rw-r--r--   0        0        0      202 2021-01-09 17:19:46.555339 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/templates/recovery_updater_script
+-rw-r--r--   0        0        0      643 2020-10-17 08:57:59.557349 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/types.py
+-rw-r--r--   0        0        0     1640 2022-06-11 18:22:18.438166 xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/xiaomi_flashable_firmware_creator.py
+-rw-r--r--   0        0        0     4643 1970-01-01 00:00:00.000000 xiaomi_flashable_firmware_creator-2.2.9/setup.py
+-rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 xiaomi_flashable_firmware_creator-2.2.9/PKG-INFO
```

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/LICENSE` & `xiaomi_flashable_firmware_creator-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/README.md` & `xiaomi_flashable_firmware_creator-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/pyproject.toml` & `xiaomi_flashable_firmware_creator-2.2.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xiaomi_flashable_firmware_creator"
-version = "2.2.8"
+version = "2.2.9"
 description = "Create flashable firmware zip from MIUI Recovery ROMs!"
 authors = ["yshalsager <ysh-alsager@hotmail.com>"]
 license = "GPL-3.0-only"
 repository = "https://github.com/XiaomiFirmwareUpdater/xiaomi-flashable-firmware-creator/"
 homepage = "https://xiaomifirmwareupdater.com/projects/xiaomi-flashable-firmware-creator/"
 keywords = ["xiaomi", "firmware", "android"]
 packages = [
@@ -18,20 +18,20 @@
 readme = "README.md"
 
 [tool.poetry.scripts]
 xiaomi_flashable_firmware_creator = "xiaomi_flashable_firmware_creator.xiaomi_flashable_firmware_creator:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-remotezip = "^0.9.2"
-protobuf = ">=3.15,<5.0"
+remotezip = ">=0.9.2,<0.11.0"
+protobuf = ">=3.15,<4.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.20.0"
-black = "^22.8.0"
+black = "^22.10.0"
 isort = "^5.10.1"
 flake8 = "^5.0.4"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 [tool.black]
```

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/binaries/update-binary` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/binaries/update-binary`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/handlers/android_one_zip.py` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/handlers/android_one_zip.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/LICENSE` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/README.md` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/README.md`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/extract_android_ota_payload.cpython-310.pyc` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/extract_android_ota_payload.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/extract_android_ota_payload.cpython-38.pyc` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/extract_android_ota_payload.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/extract_android_ota_payload.cpython-39.pyc` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/extract_android_ota_payload.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/update_metadata_pb2.cpython-310.pyc` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/update_metadata_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/update_metadata_pb2.cpython-38.pyc` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/update_metadata_pb2.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/update_metadata_pb2.cpython-39.pyc` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/__pycache__/update_metadata_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/extract_android_ota_payload.py` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/extract_android_ota_payload.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/update_metadata_pb2.py` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/ota_payload_extractor/update_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/extractors/zip_extractor.py` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/extractors/zip_extractor.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/firmware_creator.py` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/firmware_creator.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/helpers/misc.py` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/helpers/mock_zip.py` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/helpers/mock_zip.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/templates/recovery_ab_update-binary` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/templates/recovery_ab_update-binary`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/types.py` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/types.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/xiaomi_flashable_firmware_creator/xiaomi_flashable_firmware_creator.py` & `xiaomi_flashable_firmware_creator-2.2.9/xiaomi_flashable_firmware_creator/xiaomi_flashable_firmware_creator.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/setup.py` & `xiaomi_flashable_firmware_creator-2.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
  'xiaomi_flashable_firmware_creator.extractors.ota_payload_extractor',
  'xiaomi_flashable_firmware_creator.helpers']
 
 package_data = \
 {'': ['*'], 'xiaomi_flashable_firmware_creator': ['binaries/*', 'templates/*']}
 
 install_requires = \
-['protobuf>=3.15,<5.0', 'remotezip>=0.9.2,<0.10.0']
+['protobuf>=3.15,<4.0', 'remotezip>=0.9.2,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['xiaomi_flashable_firmware_creator = '
                      'xiaomi_flashable_firmware_creator.xiaomi_flashable_firmware_creator:main']}
 
 setup_kwargs = {
     'name': 'xiaomi-flashable-firmware-creator',
-    'version': '2.2.8',
+    'version': '2.2.9',
     'description': 'Create flashable firmware zip from MIUI Recovery ROMs!',
     'long_description': '## Xiaomi Flashable Firmware Creator\n\nCreate flashable firmware zip from MIUI Recovery ROMs!\n\n[![PyPI version](https://badge.fury.io/py/xiaomi-flashable-firmware-creator.svg)](https://pypi.org/project/xiaomi-flashable-firmware-creator/)\n[![made-with-python](https://img.shields.io/badge/Made%20with-Python%203-3776AB?style=flat\\&labelColor=3776AB\\&logo=python\\&logoColor=white\\&link=https://www.python.org/)](https://www.python.org/)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/9c1f6cee01b74ef8a2fd0f0c787596a8)](https://www.codacy.com/gh/XiaomiFirmwareUpdater/xiaomi-flashable-firmware-creator/dashboard?utm_source=github.com\\&utm_medium=referral\\&utm_content=XiaomiFirmwareUpdater/xiaomi-flashable-firmware-creator\\&utm_campaign=Badge_Grade)\n[![Open Source Love](https://badges.frapsoft.com/os/v3/open-source.svg?v=103)](#) <br />\n[![PayPal](https://img.shields.io/badge/PayPal-Donate-00457C?style=flat\\&labelColor=00457C\\&logo=PayPal\\&logoColor=white\\&link=https://www.paypal.me/yshalsager)](https://www.paypal.me/yshalsager)\n[![Patreon](https://img.shields.io/badge/Patreon-Support-F96854?style=flat\\&labelColor=F96854\\&logo=Patreon\\&logoColor=white\\&link=https://www.paypal.me/yshalsager)](https://www.paypal.me/yshalsager)\n[![Liberapay](https://img.shields.io/badge/Liberapay-Support-F6C915?style=flat\\&labelColor=F6C915\\&logo=Liberapay\\&logoColor=white\\&link=https://liberapay.com/yshalsager)](https://liberapay.com/yshalsager)\n\nXiaomi Flashable Firmware Creator is a tool that generates flashable firmware-update packages from official MIUI ROMS.\n\nIt supports creating untouched firmware, non-arb firmware, firmware + vendor flashable zip, and firmware-less ROMs from any local zip file or direct link of the zip file.\n\n### Installation\n\nYou can simply install this tool using Python pip.\n\n```shell script\npip install xiaomi_flashable_firmware_creator\n```\n\n### CLI Usage\n\n```shell script\nxiaomi_flashable_firmware_creator [-h] (-F FIRMWARE | -N NONARB | -L FIRMWARELESS | -V VENDOR) [-o OUTPUT]\n```\n\n**Examples:**\n\n*   Creating normal (untouched) firmware:\n\n```shell script\nxiaomi_flashable_firmware_creator -F [MIUI ZIP]\n```\n\n*   Creating non-arb firmware (without anti-rollback):\n\n```shell script\nxiaomi_flashable_firmware_creator -N [MIUI ZIP]\n```\n\n*   Creating firmware-less ROM (stock untouched ROM with just firmware removed):\n\n```shell script\nxiaomi_flashable_firmware_creator -L [MIUI ZIP]\n```\n\n*   Creating firmware + vendor flashable zip:\n\n```shell script\nxiaomi_flashable_firmware_creator -V [MIUI ZIP]\n```\n\n### Using from other Python scripts\n\n```python\nfrom xiaomi_flashable_firmware_creator.firmware_creator import FlashableFirmwareCreator\n\n# initialize firmware creator object with the following parameters:\n# input_file: zip file to extract from. It can be a local path or a remote direct url.\n# process: Which mode should the tool use. This must be one of "firmware", "nonarb", "firmwareless" or "vendor".\n# out_dir: The output directory to store the extracted file in.\n\nfirmware_creator = FlashableFirmwareCreator(input_zip, process, output_dir)\n# Now, you can either use auto() method to create the new zip file or do stuff at your own using firmware_creator public methods.\nnew_zip = firmware_creator.auto()\n```\n',
     'author': 'yshalsager',
     'author_email': 'ysh-alsager@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://xiaomifirmwareupdater.com/projects/xiaomi-flashable-firmware-creator/',
```

### Comparing `xiaomi_flashable_firmware_creator-2.2.8/PKG-INFO` & `xiaomi_flashable_firmware_creator-2.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: xiaomi-flashable-firmware-creator
-Version: 2.2.8
+Version: 2.2.9
 Summary: Create flashable firmware zip from MIUI Recovery ROMs!
 Home-page: https://xiaomifirmwareupdater.com/projects/xiaomi-flashable-firmware-creator/
 License: GPL-3.0-only
 Keywords: xiaomi,firmware,android
 Author: yshalsager
 Author-email: ysh-alsager@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: protobuf (>=3.15,<5.0)
-Requires-Dist: remotezip (>=0.9.2,<0.10.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: protobuf (>=3.15,<4.0)
+Requires-Dist: remotezip (>=0.9.2,<0.11.0)
 Project-URL: Repository, https://github.com/XiaomiFirmwareUpdater/xiaomi-flashable-firmware-creator/
 Description-Content-Type: text/markdown
 
 ## Xiaomi Flashable Firmware Creator
 
 Create flashable firmware zip from MIUI Recovery ROMs!
```

