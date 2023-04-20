# Comparing `tmp/azure-mgmt-imagebuilder-1.2.0.zip` & `tmp/azure-mgmt-imagebuilder-1.2.0b1.zip`

## zipinfo {}

```diff
@@ -1,55 +1,53 @@
-Zip file size: 92424 bytes, number of entries: 53
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/
--rw-rw-r--  2.0 unx      632 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/_meta.json
--rw-rw-r--  2.0 unx     1074 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/LICENSE
--rw-rw-r--  2.0 unx     9203 b- defN 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/PKG-INFO
--rw-rw-r--  2.0 unx     6177 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/CHANGELOG.md
--rw-rw-r--  2.0 unx     2139 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/README.md
--rw-rw-r--  2.0 unx       38 b- defN 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/setup.cfg
--rw-rw-r--  2.0 unx     2828 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/setup.py
--rw-rw-r--  2.0 unx      218 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/MANIFEST.in
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/
--rw-rw-r--  2.0 unx       65 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/models/
--rw-rw-r--  2.0 unx     1302 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_vendor.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/py.typed
--rw-rw-r--  2.0 unx     4797 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_image_builder_client.py
--rw-rw-r--  2.0 unx      894 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/__init__.py
--rw-rw-r--  2.0 unx     3843 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_configuration.py
--rw-rw-r--  2.0 unx     1530 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_patch.py
--rw-rw-r--  2.0 unx    78824 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_serialization.py
--rw-rw-r--  2.0 unx      486 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_version.py
--rw-rw-r--  2.0 unx      982 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/__init__.py
--rw-rw-r--  2.0 unx     6692 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/_patch.py
--rw-rw-r--  2.0 unx    33175 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/_triggers_operations.py
--rw-rw-r--  2.0 unx    72489 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/_virtual_machine_image_templates_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/
--rw-rw-r--  2.0 unx     4941 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/_image_builder_client.py
--rw-rw-r--  2.0 unx      841 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/__init__.py
--rw-rw-r--  2.0 unx     3891 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/_configuration.py
--rw-rw-r--  2.0 unx     1530 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/_patch.py
--rw-rw-r--  2.0 unx      982 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     5962 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    27185 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/_triggers_operations.py
--rw-rw-r--  2.0 unx    59095 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/_virtual_machine_image_templates_operations.py
--rw-rw-r--  2.0 unx     5369 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/models/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/models/_patch.py
--rw-rw-r--  2.0 unx   107960 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/models/_models_py3.py
--rw-rw-r--  2.0 unx     3254 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/models/_image_builder_client_enums.py
--rw-rw-r--  2.0 unx     5336 b- defN 23-Apr-20 07:54 azure-mgmt-imagebuilder-1.2.0/tests/disable_test_cli_mgmt_imagebuilder.py
--rw-rw-r--  2.0 unx     9203 b- defN 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        6 b- defN 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx      124 b- defN 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/requires.txt
--rw-rw-r--  2.0 unx     1689 b- defN 23-Apr-20 07:55 azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/SOURCES.txt
-53 files, 466871 bytes uncompressed, 81436 bytes compressed:  82.6%
+Zip file size: 79962 bytes, number of entries: 51
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/
+-rw-rw-r--  2.0 unx     1074 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/LICENSE
+-rw-rw-r--  2.0 unx     5733 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/CHANGELOG.md
+-rw-rw-r--  2.0 unx      218 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/MANIFEST.in
+-rw-rw-r--  2.0 unx     1353 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/README.md
+-rw-rw-r--  2.0 unx     7975 b- defN 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/PKG-INFO
+-rw-rw-r--  2.0 unx      632 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/_meta.json
+-rw-rw-r--  2.0 unx       38 b- defN 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/setup.cfg
+-rw-rw-r--  2.0 unx     2820 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/setup.py
+-rw-rw-r--  2.0 unx     5336 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/tests/disable_test_cli_mgmt_imagebuilder.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/
+-rw-rw-r--  2.0 unx       65 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/models/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/
+-rw-rw-r--  2.0 unx     4519 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_image_builder_client.py
+-rw-rw-r--  2.0 unx      488 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_version.py
+-rw-rw-r--  2.0 unx     1169 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_vendor.py
+-rw-rw-r--  2.0 unx       26 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/py.typed
+-rw-rw-r--  2.0 unx     3843 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_configuration.py
+-rw-rw-r--  2.0 unx     1530 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_patch.py
+-rw-rw-r--  2.0 unx    77872 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_serialization.py
+-rw-rw-r--  2.0 unx      894 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/__init__.py
+-rw-rw-r--  2.0 unx    87957 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/models/_models_py3.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/models/_patch.py
+-rw-rw-r--  2.0 unx     2931 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/models/_image_builder_client_enums.py
+-rw-rw-r--  2.0 unx     4512 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/models/__init__.py
+-rw-rw-r--  2.0 unx     6662 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/operations/_operations.py
+-rw-rw-r--  2.0 unx    72011 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/operations/_virtual_machine_image_templates_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/operations/_patch.py
+-rw-rw-r--  2.0 unx      903 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/operations/
+-rw-rw-r--  2.0 unx     4654 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/_image_builder_client.py
+-rw-rw-r--  2.0 unx     3891 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/_configuration.py
+-rw-rw-r--  2.0 unx     1530 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/_patch.py
+-rw-rw-r--  2.0 unx      841 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/__init__.py
+-rw-rw-r--  2.0 unx     5932 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    58634 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/operations/_virtual_machine_image_templates_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      903 b- defN 22-Nov-29 09:31 azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx      116 b- defN 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        1 b- defN 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        6 b- defN 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx     7975 b- defN 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        1 b- defN 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     1567 b- defN 22-Nov-29 09:32 azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/SOURCES.txt
+51 files, 378699 bytes uncompressed, 69282 bytes compressed:  81.7%
```

## zipnote {}

```diff
@@ -1,160 +1,154 @@
-Filename: azure-mgmt-imagebuilder-1.2.0/
+Filename: azure-mgmt-imagebuilder-1.2.0b1/
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/
+Filename: azure-mgmt-imagebuilder-1.2.0b1/tests/
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/tests/
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/_meta.json
+Filename: azure-mgmt-imagebuilder-1.2.0b1/LICENSE
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/LICENSE
+Filename: azure-mgmt-imagebuilder-1.2.0b1/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/PKG-INFO
+Filename: azure-mgmt-imagebuilder-1.2.0b1/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/CHANGELOG.md
+Filename: azure-mgmt-imagebuilder-1.2.0b1/README.md
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/README.md
+Filename: azure-mgmt-imagebuilder-1.2.0b1/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/setup.cfg
+Filename: azure-mgmt-imagebuilder-1.2.0b1/_meta.json
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/setup.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/MANIFEST.in
+Filename: azure-mgmt-imagebuilder-1.2.0b1/setup.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/
+Filename: azure-mgmt-imagebuilder-1.2.0b1/tests/disable_test_cli_mgmt_imagebuilder.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/__init__.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/__init__.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/models/
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/models/
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/operations/
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_vendor.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/py.typed
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_image_builder_client.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_image_builder_client.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_version.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/__init__.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_configuration.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/py.typed
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_patch.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_serialization.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_patch.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_version.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/__init__.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/__init__.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/_operations.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/_patch.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/_triggers_operations.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/models/_image_builder_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/_virtual_machine_image_templates_operations.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/_image_builder_client.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/operations/_virtual_machine_image_templates_operations.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/__init__.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/_configuration.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/_patch.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/__init__.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/_image_builder_client.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/_operations.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/_patch.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/_triggers_operations.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/_virtual_machine_image_templates_operations.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/models/__init__.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/operations/_virtual_machine_image_templates_operations.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/models/_patch.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/models/_models_py3.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/models/_image_builder_client_enums.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/tests/disable_test_cli_mgmt_imagebuilder.py
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/PKG-INFO
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/not-zip-safe
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/top_level.txt
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/dependency_links.txt
-Comment: 
-
-Filename: azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/requires.txt
-Comment: 
-
-Filename: azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/SOURCES.txt
+Filename: azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/SOURCES.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/_meta.json` & `azure-mgmt-imagebuilder-1.2.0b1/_meta.json`

 * *Files 22% similar despite different names*

### Pretty-printed

 * *Similarity: 0.7777777777777777%*

 * *Differences: {"'autorest_command'": "'autorest specification/imagebuilder/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.2.7 --use=@autorest/modelerfour@4.24.3 '*

 * *                       "--version=3.9.2 --version-tolerant=False'",*

 * * "'commit'": "'1fefe3f5cee88319b17c08a2dbf95e1e983a9f8c'",*

 * * "'use'": "{in […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.2",
-    "autorest_command": "autorest specification/imagebuilder/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.4.3 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
-    "commit": "ee157d6bbf6e4c4fdc8a47b380e00ddd56a0e852",
+    "autorest_command": "autorest specification/imagebuilder/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.2.7 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
+    "commit": "1fefe3f5cee88319b17c08a2dbf95e1e983a9f8c",
     "readme": "specification/imagebuilder/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.4.3",
+        "@autorest/python@6.2.7",
         "@autorest/modelerfour@4.24.3"
     ]
 }
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/LICENSE` & `azure-mgmt-imagebuilder-1.2.0b1/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-imagebuilder-1.2.0/PKG-INFO` & `azure-mgmt-imagebuilder-1.2.0b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-imagebuilder
-Version: 1.2.0
+Version: 1.2.0b1
 Summary: Microsoft Azure Image Builder Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -27,83 +27,36 @@
 This package has been tested with Python 3.7+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
-## Getting started
+# Usage
 
-### Prerequisites
 
-- Python 3.7+ is required to use this package.
-- [Azure subscription](https://azure.microsoft.com/free/)
+To learn how to use this package, see the [quickstart guide](https://aka.ms/azsdk/python/mgmt)
+ 
+For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/)
+Code samples for this package can be found at [Image Builder](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
+Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
-### Install the package
 
-```bash
-pip install azure-mgmt-imagebuilder
-pip install azure-identity
-```
-
-### Authentication
-
-By default, [Azure Active Directory](https://aka.ms/awps/aad) token authentication depends on correct configure of following environment variables.
-
-- `AZURE_CLIENT_ID` for Azure client ID.
-- `AZURE_TENANT_ID` for Azure tenant ID.
-- `AZURE_CLIENT_SECRET` for Azure client secret.
-
-In addition, Azure subscription ID can be configured via environment variable `AZURE_SUBSCRIPTION_ID`.
-
-With above configuration, client can be authenticated by following code:
-
-```python
-from azure.identity import DefaultAzureCredential
-from azure.mgmt.imagebuilder import ImageBuilderClient
-import os
-
-sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
-client = ImageBuilderClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
-```
-
-## Examples
-
-Code samples for this package can be found at:
-- [Search Image Builder](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
-- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
-
-
-## Troubleshooting
-
-## Next steps
-
-## Provide Feedback
+# Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-imagebuilder%2FREADME.png)
 
 
 # Release History
 
-## 1.2.0 (2023-04-20)
-
-### Features Added
-
-  - Added operation group TriggersOperations
-  - Model ImageTemplate has a new parameter optimize
-  - Model ImageTemplateSharedImageDistributor has a new parameter target_regions
-  - Model ImageTemplateSharedImageDistributor has a new parameter versioning
-  - Model ImageTemplateSharedImageVersionSource has a new parameter exact_version
-  - Model ImageTemplateVhdDistributor has a new parameter uri
-
 ## 1.2.0b1 (2022-11-28)
 
 ### Other Changes
 
   - Added generated samples in github repo
   - Drop support for python<3.7.0
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/CHANGELOG.md` & `azure-mgmt-imagebuilder-1.2.0b1/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,9 @@
 # Release History
 
-## 1.2.0 (2023-04-20)
-
-### Features Added
-
-  - Added operation group TriggersOperations
-  - Model ImageTemplate has a new parameter optimize
-  - Model ImageTemplateSharedImageDistributor has a new parameter target_regions
-  - Model ImageTemplateSharedImageDistributor has a new parameter versioning
-  - Model ImageTemplateSharedImageVersionSource has a new parameter exact_version
-  - Model ImageTemplateVhdDistributor has a new parameter uri
-
 ## 1.2.0b1 (2022-11-28)
 
 ### Other Changes
 
   - Added generated samples in github repo
   - Drop support for python<3.7.0
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/setup.py` & `azure-mgmt-imagebuilder-1.2.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,14 @@
         'azure.mgmt',
     ]),
     include_package_data=True,
     package_data={
         'pytyped': ['py.typed'],
     },
     install_requires=[
-        "isodate<1.0.0,>=0.6.1",
+        "msrest>=0.7.1",
         "azure-common~=1.1",
         "azure-mgmt-core>=1.3.2,<2.0.0",
         "typing-extensions>=4.3.0; python_version<'3.8.0'",
     ],
     python_requires=">=3.7"
 )
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_vendor.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_vendor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from typing import List, cast
-
 from azure.core.pipeline.transport import HttpRequest
 
 
 def _convert_request(request, files=None):
     data = request.content if not files else None
     request = HttpRequest(method=request.method, url=request.url, headers=request.headers, data=data)
     if files:
@@ -20,11 +18,10 @@
 
 def _format_url_section(template, **kwargs):
     components = template.split("/")
     while components:
         try:
             return template.format(**kwargs)
         except KeyError as key:
-            # Need the cast, as for some reasons "split" is typed as list[str | Any]
-            formatted_components = cast(List[str], template.split("/"))
+            formatted_components = template.split("/")
             components = [c for c in formatted_components if "{}".format(key.args[0]) not in c]
             template = "/".join(components)
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_image_builder_client.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_image_builder_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,63 +11,60 @@
 
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
 
 from . import models as _models
 from ._configuration import ImageBuilderClientConfiguration
 from ._serialization import Deserializer, Serializer
-from .operations import Operations, TriggersOperations, VirtualMachineImageTemplatesOperations
+from .operations import Operations, VirtualMachineImageTemplatesOperations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
 class ImageBuilderClient:  # pylint: disable=client-accepts-api-version-keyword
     """Azure Virtual Machine Image Builder Client.
 
     :ivar virtual_machine_image_templates: VirtualMachineImageTemplatesOperations operations
     :vartype virtual_machine_image_templates:
      azure.mgmt.imagebuilder.operations.VirtualMachineImageTemplatesOperations
-    :ivar triggers: TriggersOperations operations
-    :vartype triggers: azure.mgmt.imagebuilder.operations.TriggersOperations
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.imagebuilder.operations.Operations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure
      subscription. The subscription Id forms part of the URI for every service call. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-07-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2022-02-14". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
         credential: "TokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = ImageBuilderClientConfiguration(credential=credential, subscription_id=subscription_id, **kwargs)
-        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.virtual_machine_image_templates = VirtualMachineImageTemplatesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
-        self.triggers = TriggersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
@@ -91,9 +88,9 @@
     def close(self) -> None:
         self._client.close()
 
     def __enter__(self) -> "ImageBuilderClient":
         self._client.__enter__()
         return self
 
-    def __exit__(self, *exc_details: Any) -> None:
+    def __exit__(self, *exc_details) -> None:
         self._client.__exit__(*exc_details)
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/__init__.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_configuration.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,22 @@
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure
      subscription. The subscription Id forms part of the URI for every service call. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-07-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2022-02-14". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(ImageBuilderClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2022-07-01"] = kwargs.pop("api_version", "2022-07-01")
+        api_version: Literal["2022-02-14"] = kwargs.pop("api_version", "2022-02-14")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_patch.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/_serialization.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,47 +34,30 @@
 import email
 from enum import Enum
 import json
 import logging
 import re
 import sys
 import codecs
-from typing import (
-    Dict,
-    Any,
-    cast,
-    Optional,
-    Union,
-    AnyStr,
-    IO,
-    Mapping,
-    Callable,
-    TypeVar,
-    MutableMapping,
-    Type,
-    List,
-    Mapping,
-)
+from typing import Optional, Union, AnyStr, IO, Mapping
 
 try:
     from urllib import quote  # type: ignore
 except ImportError:
     from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
 import isodate  # type: ignore
 
+from typing import Dict, Any, cast
+
 from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
-from azure.core.serialization import NULL as AzureCoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
-ModelType = TypeVar("ModelType", bound="Model")
-JSON = MutableMapping[str, Any]
-
 
 class RawDeserializer:
 
     # Accept "text" because we're open minded people...
     JSON_REGEXP = re.compile(r"^(application|text)/([a-z+.]+\+)?json$")
 
     # Name used in context
@@ -290,43 +273,43 @@
     serialization and deserialization.
     """
 
     _subtype_map: Dict[str, Dict[str, Any]] = {}
     _attribute_map: Dict[str, Dict[str, Any]] = {}
     _validation: Dict[str, Dict[str, Any]] = {}
 
-    def __init__(self, **kwargs: Any) -> None:
-        self.additional_properties: Dict[str, Any] = {}
+    def __init__(self, **kwargs):
+        self.additional_properties = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other):
         """Compare objects by comparing all attributes."""
         if isinstance(other, self.__class__):
             return self.__dict__ == other.__dict__
         return False
 
-    def __ne__(self, other: Any) -> bool:
+    def __ne__(self, other):
         """Compare objects by comparing all attributes."""
         return not self.__eq__(other)
 
-    def __str__(self) -> str:
+    def __str__(self):
         return str(self.__dict__)
 
     @classmethod
-    def enable_additional_properties_sending(cls) -> None:
+    def enable_additional_properties_sending(cls):
         cls._attribute_map["additional_properties"] = {"key": "", "type": "{object}"}
 
     @classmethod
-    def is_xml_model(cls) -> bool:
+    def is_xml_model(cls):
         try:
             cls._xml_map  # type: ignore
         except AttributeError:
             return False
         return True
 
     @classmethod
@@ -335,35 +318,30 @@
         try:
             xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
-    def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
+    def serialize(self, keep_readonly=False, **kwargs):
         """Return the JSON that would be sent to azure from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
         return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
 
-    def as_dict(
-        self,
-        keep_readonly: bool = True,
-        key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
-        **kwargs: Any
-    ) -> JSON:
-        """Return a dict that can be serialized using json.dump.
+    def as_dict(self, keep_readonly=True, key_transformer=attribute_transformer, **kwargs):
+        """Return a dict that can be JSONify using json.dump.
 
         Advanced usage might optionally use a callback as parameter:
 
         .. code::python
 
             def my_key_transformer(key, attr_desc, value):
                 return key
@@ -402,46 +380,41 @@
                 raise ValueError("Not Autorest generated code")
         except Exception:
             # Assume it's not Autorest generated (tests?). Add ourselves as dependencies.
             client_models = {cls.__name__: cls}
         return client_models
 
     @classmethod
-    def deserialize(cls: Type[ModelType], data: Any, content_type: Optional[str] = None) -> ModelType:
+    def deserialize(cls, data, content_type=None):
         """Parse a str using the RestAPI syntax and return a model.
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
         return deserializer(cls.__name__, data, content_type=content_type)
 
     @classmethod
-    def from_dict(
-        cls: Type[ModelType],
-        data: Any,
-        key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
-        content_type: Optional[str] = None,
-    ) -> ModelType:
+    def from_dict(cls, data, key_extractors=None, content_type=None):
         """Parse a dict using given key extractor return a model.
 
         By default consider key
         extractors (rest_key_case_insensitive_extractor, attribute_key_case_insensitive_extractor
         and last_rest_key_case_insensitive_extractor)
 
         :param dict data: A dict using RestAPI structure
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        deserializer.key_extractors = (  # type: ignore
-            [  # type: ignore
+        deserializer.key_extractors = (
+            [
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
@@ -541,15 +514,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
+    def __init__(self, classes=None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -557,15 +530,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
+        self.dependencies = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -649,15 +622,16 @@
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
                             local_node.text = unicode_str(new_attr)
                             serialized.append(local_node)  # type: ignore
                     else:  # JSON
                         for k in reversed(keys):  # type: ignore
-                            new_attr = {k: new_attr}
+                            unflattened = {k: new_attr}
+                            new_attr = unflattened
 
                         _new_attr = new_attr
                         _serialized = serialized
                         for k in keys:  # type: ignore
                             if k not in _serialized:
                                 _serialized.update(_new_attr)  # type: ignore
                             _new_attr = _new_attr[k]  # type: ignore
@@ -678,16 +652,16 @@
         :param str data_type: The type to be serialized from.
         :rtype: dict
         :raises: SerializationError if serialization fails.
         :raises: ValueError if data is None
         """
 
         # Just in case this is a dict
-        internal_data_type_str = data_type.strip("[]{}")
-        internal_data_type = self.dependencies.get(internal_data_type_str, None)
+        internal_data_type = data_type.strip("[]{}")
+        internal_data_type = self.dependencies.get(internal_data_type, None)
         try:
             is_xml_model_serialization = kwargs["is_xml"]
         except KeyError:
             if internal_data_type and issubclass(internal_data_type, Model):
                 is_xml_model_serialization = kwargs.setdefault("is_xml", internal_data_type.is_xml_model())
             else:
                 is_xml_model_serialization = False
@@ -799,16 +773,14 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
-            if data is AzureCoreNull:
-                return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
             # If dependencies is empty, try with current data class
@@ -1185,16 +1157,15 @@
 
 
 def rest_key_extractor(attr, attr_desc, data):
     key = attr_desc["key"]
     working_data = data
 
     while "." in key:
-        # Need the cast, as for some reasons "split" is typed as list[str | Any]
-        dict_keys = cast(List[str], _FLATTEN.split(key))
+        dict_keys = _FLATTEN.split(key)
         if len(dict_keys) == 1:
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
@@ -1357,15 +1328,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
+    def __init__(self, classes=None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1377,15 +1348,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
+        self.dependencies = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1496,40 +1467,40 @@
 
     def _classify_target(self, target, data):
         """Check to see whether the deserialization target object can
         be classified into a subclass.
         Once classification has been determined, initialize object.
 
         :param str target: The target object type to deserialize to.
-        :param str/dict data: The response data to deserialize.
+        :param str/dict data: The response data to deseralize.
         """
         if target is None:
             return None, None
 
         if isinstance(target, basestring):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
             target = target._classify(data, self.dependencies)
         except AttributeError:
             pass  # Target is not a Model, no classify
-        return target, target.__class__.__name__  # type: ignore
+        return target, target.__class__.__name__
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
         for use in error deserialization, as we want to return the
         HttpResponseError to users, and not have them deal with
         a deserialization error.
 
         :param str target_obj: The target object type to deserialize to.
-        :param str/dict data: The response data to deserialize.
+        :param str/dict data: The response data to deseralize.
         :param str content_type: Swagger "produces" if available.
         """
         try:
             return self(target_obj, data, content_type=content_type)
         except:
             _LOGGER.debug(
                 "Ran into a deserialization error. Ignoring since this is failsafe deserialization", exc_info=True
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/__init__.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/operations/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._virtual_machine_image_templates_operations import VirtualMachineImageTemplatesOperations
-from ._triggers_operations import TriggersOperations
 from ._operations import Operations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "VirtualMachineImageTemplatesOperations",
-    "TriggersOperations",
     "Operations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/_operations.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-07-01"))
+    api_version: Literal["2022-02-14"] = kwargs.pop("api_version", _params.pop("api-version", "2022-02-14"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.VirtualMachineImages/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -87,15 +87,15 @@
         :return: An iterator like instance of either Operation or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.imagebuilder.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -140,17 +140,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/_patch.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/operations/_virtual_machine_image_templates_operations.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/operations/_virtual_machine_image_templates_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-07-01"))
+    api_version: Literal["2022-02-14"] = kwargs.pop("api_version", _params.pop("api-version", "2022-02-14"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.VirtualMachineImages/imageTemplates"
     )  # pylint: disable=line-too-long
     path_format_arguments = {
@@ -69,15 +69,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-07-01"))
+    api_version: Literal["2022-02-14"] = kwargs.pop("api_version", _params.pop("api-version", "2022-02-14"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.VirtualMachineImages/imageTemplates",
     )  # pylint: disable=line-too-long
@@ -99,15 +99,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, image_template_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-07-01"))
+    api_version: Literal["2022-02-14"] = kwargs.pop("api_version", _params.pop("api-version", "2022-02-14"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.VirtualMachineImages/imageTemplates/{imageTemplateName}",
@@ -135,15 +135,15 @@
 
 def build_update_request(
     resource_group_name: str, image_template_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-07-01"))
+    api_version: Literal["2022-02-14"] = kwargs.pop("api_version", _params.pop("api-version", "2022-02-14"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.VirtualMachineImages/imageTemplates/{imageTemplateName}",
@@ -171,15 +171,15 @@
 
 def build_get_request(
     resource_group_name: str, image_template_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-07-01"))
+    api_version: Literal["2022-02-14"] = kwargs.pop("api_version", _params.pop("api-version", "2022-02-14"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.VirtualMachineImages/imageTemplates/{imageTemplateName}",
     )  # pylint: disable=line-too-long
@@ -204,15 +204,15 @@
 
 def build_delete_request(
     resource_group_name: str, image_template_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-07-01"))
+    api_version: Literal["2022-02-14"] = kwargs.pop("api_version", _params.pop("api-version", "2022-02-14"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.VirtualMachineImages/imageTemplates/{imageTemplateName}",
     )  # pylint: disable=line-too-long
@@ -237,15 +237,15 @@
 
 def build_run_request(
     resource_group_name: str, image_template_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-07-01"))
+    api_version: Literal["2022-02-14"] = kwargs.pop("api_version", _params.pop("api-version", "2022-02-14"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.VirtualMachineImages/imageTemplates/{imageTemplateName}/run",
     )  # pylint: disable=line-too-long
@@ -270,15 +270,15 @@
 
 def build_cancel_request(
     resource_group_name: str, image_template_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-07-01"))
+    api_version: Literal["2022-02-14"] = kwargs.pop("api_version", _params.pop("api-version", "2022-02-14"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.VirtualMachineImages/imageTemplates/{imageTemplateName}/cancel",
     )  # pylint: disable=line-too-long
@@ -303,15 +303,15 @@
 
 def build_list_run_outputs_request(
     resource_group_name: str, image_template_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-07-01"))
+    api_version: Literal["2022-02-14"] = kwargs.pop("api_version", _params.pop("api-version", "2022-02-14"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.VirtualMachineImages/imageTemplates/{imageTemplateName}/runOutputs",
     )  # pylint: disable=line-too-long
@@ -336,15 +336,15 @@
 
 def build_get_run_output_request(
     resource_group_name: str, image_template_name: str, run_output_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-07-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-07-01"))
+    api_version: Literal["2022-02-14"] = kwargs.pop("api_version", _params.pop("api-version", "2022-02-14"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.VirtualMachineImages/imageTemplates/{imageTemplateName}/runOutputs/{runOutputName}",
     )  # pylint: disable=line-too-long
@@ -395,15 +395,15 @@
         :return: An iterator like instance of either ImageTemplate or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.imagebuilder.models.ImageTemplate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.ImageTemplateListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -449,17 +449,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -479,15 +478,15 @@
         :return: An iterator like instance of either ImageTemplate or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.imagebuilder.models.ImageTemplate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.ImageTemplateListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -534,17 +533,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -570,15 +568,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ImageTemplate] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -599,17 +597,16 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -709,16 +706,16 @@
     ) -> LROPoller[_models.ImageTemplate]:
         """Create or update a virtual machine image template.
 
         :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param image_template_name: The name of the image Template. Required.
         :type image_template_name: str
-        :param parameters: Parameters supplied to the CreateImageTemplate operation. Is either a
-         ImageTemplate type or a IO type. Required.
+        :param parameters: Parameters supplied to the CreateImageTemplate operation. Is either a model
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.imagebuilder.models.ImageTemplate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -731,15 +728,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.imagebuilder.models.ImageTemplate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ImageTemplate] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -798,15 +795,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.ImageTemplate]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -827,17 +824,16 @@
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -935,16 +931,16 @@
     ) -> LROPoller[_models.ImageTemplate]:
         """Update the tags for this Virtual Machine Image Template.
 
         :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param image_template_name: The name of the image Template. Required.
         :type image_template_name: str
-        :param parameters: Additional parameters for Image Template update. Is either a
-         ImageTemplateUpdateParameters type or a IO type. Required.
+        :param parameters: Additional parameters for Image Template update. Is either a model type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.imagebuilder.models.ImageTemplateUpdateParameters or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -957,15 +953,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.imagebuilder.models.ImageTemplate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ImageTemplate] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -1030,15 +1026,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.ImageTemplate] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             image_template_name=image_template_name,
@@ -1047,17 +1043,16 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1083,15 +1078,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             image_template_name=image_template_name,
@@ -1100,31 +1095,26 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        response_headers = {}
-        if response.status_code == 202:
-            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-
         if cls:
-            return cls(pipeline_response, None, response_headers)
+            return cls(pipeline_response, None, {})
 
     _delete_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.VirtualMachineImages/imageTemplates/{imageTemplateName}"
     }
 
     @distributed_trace
     def begin_delete(self, resource_group_name: str, image_template_name: str, **kwargs: Any) -> LROPoller[None]:
@@ -1145,15 +1135,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -1170,15 +1160,15 @@
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
             polling_method: PollingMethod = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
@@ -1203,15 +1193,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_run_request(
             resource_group_name=resource_group_name,
             image_template_name=image_template_name,
@@ -1220,17 +1210,16 @@
             template_url=self._run_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1261,15 +1250,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -1319,15 +1308,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_cancel_request(
             resource_group_name=resource_group_name,
             image_template_name=image_template_name,
@@ -1336,17 +1325,16 @@
             template_url=self._cancel_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1377,15 +1365,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -1439,15 +1427,15 @@
         :return: An iterator like instance of either RunOutput or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.imagebuilder.models.RunOutput]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.RunOutputCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1495,17 +1483,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1541,15 +1528,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.RunOutput] = kwargs.pop("cls", None)
 
         request = build_get_run_output_request(
             resource_group_name=resource_group_name,
             image_template_name=image_template_name,
@@ -1559,17 +1546,16 @@
             template_url=self.get_run_output.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/_image_builder_client.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/_image_builder_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,63 +11,60 @@
 
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
 
 from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import ImageBuilderClientConfiguration
-from .operations import Operations, TriggersOperations, VirtualMachineImageTemplatesOperations
+from .operations import Operations, VirtualMachineImageTemplatesOperations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
 class ImageBuilderClient:  # pylint: disable=client-accepts-api-version-keyword
     """Azure Virtual Machine Image Builder Client.
 
     :ivar virtual_machine_image_templates: VirtualMachineImageTemplatesOperations operations
     :vartype virtual_machine_image_templates:
      azure.mgmt.imagebuilder.aio.operations.VirtualMachineImageTemplatesOperations
-    :ivar triggers: TriggersOperations operations
-    :vartype triggers: azure.mgmt.imagebuilder.aio.operations.TriggersOperations
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.imagebuilder.aio.operations.Operations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure
      subscription. The subscription Id forms part of the URI for every service call. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-07-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2022-02-14". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
         credential: "AsyncTokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = ImageBuilderClientConfiguration(credential=credential, subscription_id=subscription_id, **kwargs)
-        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.virtual_machine_image_templates = VirtualMachineImageTemplatesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
-        self.triggers = TriggersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
@@ -91,9 +88,9 @@
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "ImageBuilderClient":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *exc_details: Any) -> None:
+    async def __aexit__(self, *exc_details) -> None:
         await self._client.__aexit__(*exc_details)
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/__init__.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/_configuration.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,22 +32,22 @@
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure
      subscription. The subscription Id forms part of the URI for every service call. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-07-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2022-02-14". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(ImageBuilderClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2022-07-01"] = kwargs.pop("api_version", "2022-07-01")
+        api_version: Literal["2022-02-14"] = kwargs.pop("api_version", "2022-02-14")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/_patch.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/__init__.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/operations/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._virtual_machine_image_templates_operations import VirtualMachineImageTemplatesOperations
-from ._triggers_operations import TriggersOperations
 from ._operations import Operations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "VirtualMachineImageTemplatesOperations",
-    "TriggersOperations",
     "Operations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/_operations.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         :return: An iterator like instance of either Operation or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.imagebuilder.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -118,17 +118,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/_patch.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/aio/operations/_virtual_machine_image_templates_operations.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/operations/_virtual_machine_image_templates_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         :return: An iterator like instance of either ImageTemplate or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.imagebuilder.models.ImageTemplate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.ImageTemplateListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -133,17 +133,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -163,15 +162,15 @@
         :return: An iterator like instance of either ImageTemplate or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.imagebuilder.models.ImageTemplate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.ImageTemplateListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -218,17 +217,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -254,15 +252,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ImageTemplate] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -283,17 +281,16 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -393,16 +390,16 @@
     ) -> AsyncLROPoller[_models.ImageTemplate]:
         """Create or update a virtual machine image template.
 
         :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param image_template_name: The name of the image Template. Required.
         :type image_template_name: str
-        :param parameters: Parameters supplied to the CreateImageTemplate operation. Is either a
-         ImageTemplate type or a IO type. Required.
+        :param parameters: Parameters supplied to the CreateImageTemplate operation. Is either a model
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.imagebuilder.models.ImageTemplate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -415,15 +412,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.imagebuilder.models.ImageTemplate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ImageTemplate] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -483,15 +480,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.ImageTemplate]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -512,17 +509,16 @@
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -620,16 +616,16 @@
     ) -> AsyncLROPoller[_models.ImageTemplate]:
         """Update the tags for this Virtual Machine Image Template.
 
         :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param image_template_name: The name of the image Template. Required.
         :type image_template_name: str
-        :param parameters: Additional parameters for Image Template update. Is either a
-         ImageTemplateUpdateParameters type or a IO type. Required.
+        :param parameters: Additional parameters for Image Template update. Is either a model type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.imagebuilder.models.ImageTemplateUpdateParameters or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -642,15 +638,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.imagebuilder.models.ImageTemplate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ImageTemplate] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -716,15 +712,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.ImageTemplate] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             image_template_name=image_template_name,
@@ -733,17 +729,16 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -769,15 +764,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             image_template_name=image_template_name,
@@ -786,31 +781,26 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        response_headers = {}
-        if response.status_code == 202:
-            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-
         if cls:
-            return cls(pipeline_response, None, response_headers)
+            return cls(pipeline_response, None, {})
 
     _delete_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.VirtualMachineImages/imageTemplates/{imageTemplateName}"
     }
 
     @distributed_trace_async
     async def begin_delete(
@@ -833,15 +823,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -858,15 +848,16 @@
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
@@ -891,15 +882,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_run_request(
             resource_group_name=resource_group_name,
             image_template_name=image_template_name,
@@ -908,17 +899,16 @@
             template_url=self._run_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -951,15 +941,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -1010,15 +1000,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_cancel_request(
             resource_group_name=resource_group_name,
             image_template_name=image_template_name,
@@ -1027,17 +1017,16 @@
             template_url=self._cancel_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1070,15 +1059,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -1133,15 +1122,15 @@
         :return: An iterator like instance of either RunOutput or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.imagebuilder.models.RunOutput]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.RunOutputCollection] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1189,17 +1178,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1235,15 +1223,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-07-01"] = kwargs.pop(
+        api_version: Literal["2022-02-14"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.RunOutput] = kwargs.pop("cls", None)
 
         request = build_get_run_output_request(
             resource_group_name=resource_group_name,
             image_template_name=image_template_name,
@@ -1253,17 +1241,16 @@
             template_url=self.get_run_output.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/models/__init__.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,33 +3,30 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._models_py3 import CloudErrorBody
-from ._models_py3 import DistributeVersioner
-from ._models_py3 import DistributeVersionerLatest
-from ._models_py3 import DistributeVersionerSource
+from ._models_py3 import (
+    ComponentsVrq145SchemasImagetemplateidentityPropertiesUserassignedidentitiesAdditionalproperties,
+)
 from ._models_py3 import ImageTemplate
 from ._models_py3 import ImageTemplateCustomizer
 from ._models_py3 import ImageTemplateDistributor
 from ._models_py3 import ImageTemplateFileCustomizer
-from ._models_py3 import ImageTemplateFileValidator
 from ._models_py3 import ImageTemplateIdentity
 from ._models_py3 import ImageTemplateInVMValidator
 from ._models_py3 import ImageTemplateLastRunStatus
 from ._models_py3 import ImageTemplateListResult
 from ._models_py3 import ImageTemplateManagedImageDistributor
 from ._models_py3 import ImageTemplateManagedImageSource
 from ._models_py3 import ImageTemplatePlatformImageSource
 from ._models_py3 import ImageTemplatePowerShellCustomizer
 from ._models_py3 import ImageTemplatePowerShellValidator
-from ._models_py3 import ImageTemplatePropertiesOptimize
-from ._models_py3 import ImageTemplatePropertiesOptimizeVmBoot
 from ._models_py3 import ImageTemplatePropertiesValidate
 from ._models_py3 import ImageTemplateRestartCustomizer
 from ._models_py3 import ImageTemplateSharedImageDistributor
 from ._models_py3 import ImageTemplateSharedImageVersionSource
 from ._models_py3 import ImageTemplateShellCustomizer
 from ._models_py3 import ImageTemplateShellValidator
 from ._models_py3 import ImageTemplateSource
@@ -42,58 +39,45 @@
 from ._models_py3 import OperationListResult
 from ._models_py3 import PlatformImagePurchasePlan
 from ._models_py3 import ProvisioningError
 from ._models_py3 import ProxyResource
 from ._models_py3 import Resource
 from ._models_py3 import RunOutput
 from ._models_py3 import RunOutputCollection
-from ._models_py3 import SourceImageTriggerProperties
 from ._models_py3 import SystemData
-from ._models_py3 import TargetRegion
 from ._models_py3 import TrackedResource
-from ._models_py3 import Trigger
-from ._models_py3 import TriggerCollection
-from ._models_py3 import TriggerProperties
-from ._models_py3 import TriggerStatus
-from ._models_py3 import UserAssignedIdentity
 from ._models_py3 import VirtualNetworkConfig
 
 from ._image_builder_client_enums import CreatedByType
 from ._image_builder_client_enums import ProvisioningErrorCode
 from ._image_builder_client_enums import ProvisioningState
 from ._image_builder_client_enums import ResourceIdentityType
 from ._image_builder_client_enums import RunState
 from ._image_builder_client_enums import RunSubState
 from ._image_builder_client_enums import SharedImageStorageAccountType
-from ._image_builder_client_enums import VMBootOptimizationState
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "CloudErrorBody",
-    "DistributeVersioner",
-    "DistributeVersionerLatest",
-    "DistributeVersionerSource",
+    "ComponentsVrq145SchemasImagetemplateidentityPropertiesUserassignedidentitiesAdditionalproperties",
     "ImageTemplate",
     "ImageTemplateCustomizer",
     "ImageTemplateDistributor",
     "ImageTemplateFileCustomizer",
-    "ImageTemplateFileValidator",
     "ImageTemplateIdentity",
     "ImageTemplateInVMValidator",
     "ImageTemplateLastRunStatus",
     "ImageTemplateListResult",
     "ImageTemplateManagedImageDistributor",
     "ImageTemplateManagedImageSource",
     "ImageTemplatePlatformImageSource",
     "ImageTemplatePowerShellCustomizer",
     "ImageTemplatePowerShellValidator",
-    "ImageTemplatePropertiesOptimize",
-    "ImageTemplatePropertiesOptimizeVmBoot",
     "ImageTemplatePropertiesValidate",
     "ImageTemplateRestartCustomizer",
     "ImageTemplateSharedImageDistributor",
     "ImageTemplateSharedImageVersionSource",
     "ImageTemplateShellCustomizer",
     "ImageTemplateShellValidator",
     "ImageTemplateSource",
@@ -106,28 +90,20 @@
     "OperationListResult",
     "PlatformImagePurchasePlan",
     "ProvisioningError",
     "ProxyResource",
     "Resource",
     "RunOutput",
     "RunOutputCollection",
-    "SourceImageTriggerProperties",
     "SystemData",
-    "TargetRegion",
     "TrackedResource",
-    "Trigger",
-    "TriggerCollection",
-    "TriggerProperties",
-    "TriggerStatus",
-    "UserAssignedIdentity",
     "VirtualNetworkConfig",
     "CreatedByType",
     "ProvisioningErrorCode",
     "ProvisioningState",
     "ResourceIdentityType",
     "RunState",
     "RunSubState",
     "SharedImageStorageAccountType",
-    "VMBootOptimizationState",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/models/_patch.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/models/_models_py3.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/models/_models_py3.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     def __init__(
         self,
         *,
         code: Optional[str] = None,
         message: Optional[str] = None,
         target: Optional[str] = None,
         details: Optional[List["_models.CloudErrorBody"]] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword code: An identifier for the error. Codes are invariant and are intended to be consumed
          programmatically.
         :paramtype code: str
         :keyword message: A message describing the error, intended to be suitable for display in a user
          interface.
         :paramtype message: str
@@ -72,96 +72,42 @@
         super().__init__(**kwargs)
         self.code = code
         self.message = message
         self.target = target
         self.details = details
 
 
-class DistributeVersioner(_serialization.Model):
-    """Describes how to generate new x.y.z version number for distribution.
+class ComponentsVrq145SchemasImagetemplateidentityPropertiesUserassignedidentitiesAdditionalproperties(
+    _serialization.Model
+):
+    """ComponentsVrq145SchemasImagetemplateidentityPropertiesUserassignedidentitiesAdditionalproperties.
 
-    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
-    DistributeVersionerLatest, DistributeVersionerSource
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar scheme: Version numbering scheme to be used. Required.
-    :vartype scheme: str
-    """
-
-    _validation = {
-        "scheme": {"required": True},
-    }
-
-    _attribute_map = {
-        "scheme": {"key": "scheme", "type": "str"},
-    }
-
-    _subtype_map = {"scheme": {"Latest": "DistributeVersionerLatest", "Source": "DistributeVersionerSource"}}
-
-    def __init__(self, **kwargs: Any) -> None:
-        """ """
-        super().__init__(**kwargs)
-        self.scheme: Optional[str] = None
-
-
-class DistributeVersionerLatest(DistributeVersioner):
-    """Generates version number that will be latest based on existing version numbers.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar scheme: Version numbering scheme to be used. Required.
-    :vartype scheme: str
-    :ivar major: Major version for the generated version number. Determine what is "latest" based
-     on versions with this value as the major version. -1 is equivalent to leaving it unset.
-    :vartype major: int
-    """
-
-    _validation = {
-        "scheme": {"required": True},
-        "major": {"minimum": -1},
-    }
-
-    _attribute_map = {
-        "scheme": {"key": "scheme", "type": "str"},
-        "major": {"key": "major", "type": "int"},
-    }
-
-    def __init__(self, *, major: int = -1, **kwargs: Any) -> None:
-        """
-        :keyword major: Major version for the generated version number. Determine what is "latest"
-         based on versions with this value as the major version. -1 is equivalent to leaving it unset.
-        :paramtype major: int
-        """
-        super().__init__(**kwargs)
-        self.scheme: str = "Latest"
-        self.major = major
-
-
-class DistributeVersionerSource(DistributeVersioner):
-    """Generates version number based on version number of source image.
-
-    All required parameters must be populated in order to send to Azure.
+    Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar scheme: Version numbering scheme to be used. Required.
-    :vartype scheme: str
+    :ivar principal_id: The principal id of user assigned identity.
+    :vartype principal_id: str
+    :ivar client_id: The client id of user assigned identity.
+    :vartype client_id: str
     """
 
     _validation = {
-        "scheme": {"required": True},
+        "principal_id": {"readonly": True},
+        "client_id": {"readonly": True},
     }
 
     _attribute_map = {
-        "scheme": {"key": "scheme", "type": "str"},
+        "principal_id": {"key": "principalId", "type": "str"},
+        "client_id": {"key": "clientId", "type": "str"},
     }
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(self, **kwargs):
         """ """
         super().__init__(**kwargs)
-        self.scheme: str = "Source"
+        self.principal_id = None
+        self.client_id = None
 
 
 class Resource(_serialization.Model):
     """Common fields that are returned in the response for all Azure Resource Manager resources.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -188,26 +134,25 @@
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(self, **kwargs):
         """ """
         super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.system_data = None
 
 
 class TrackedResource(Resource):
-    """The resource model definition for an Azure Resource Manager tracked top level resource which
-    has 'tags' and a 'location'.
+    """The resource model definition for an Azure Resource Manager tracked top level resource which has 'tags' and a 'location'.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
@@ -239,15 +184,15 @@
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
     }
 
-    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
+    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs):
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         """
         super().__init__(**kwargs)
@@ -280,31 +225,29 @@
     :ivar identity: The identity of the image template, if configured. Required.
     :vartype identity: ~azure.mgmt.imagebuilder.models.ImageTemplateIdentity
     :ivar source: Specifies the properties used to describe the source image.
     :vartype source: ~azure.mgmt.imagebuilder.models.ImageTemplateSource
     :ivar customize: Specifies the properties used to describe the customization steps of the
      image, like Image source etc.
     :vartype customize: list[~azure.mgmt.imagebuilder.models.ImageTemplateCustomizer]
-    :ivar optimize: Specifies optimization to be performed on image.
-    :vartype optimize: ~azure.mgmt.imagebuilder.models.ImageTemplatePropertiesOptimize
     :ivar validate: Configuration options and list of validations to be performed on the resulting
      image.
     :vartype validate: ~azure.mgmt.imagebuilder.models.ImageTemplatePropertiesValidate
     :ivar distribute: The distribution targets where the image output needs to go to.
     :vartype distribute: list[~azure.mgmt.imagebuilder.models.ImageTemplateDistributor]
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Creating",
-     "Updating", "Succeeded", "Failed", "Deleting", and "Canceled".
+     "Updating", "Succeeded", "Failed", and "Deleting".
     :vartype provisioning_state: str or ~azure.mgmt.imagebuilder.models.ProvisioningState
     :ivar provisioning_error: Provisioning error, if any.
     :vartype provisioning_error: ~azure.mgmt.imagebuilder.models.ProvisioningError
     :ivar last_run_status: State of 'run' that is currently executing or was last executed.
     :vartype last_run_status: ~azure.mgmt.imagebuilder.models.ImageTemplateLastRunStatus
     :ivar build_timeout_in_minutes: Maximum duration to wait while building the image template
-     (includes all customizations, optimization, validations, and distributions). Omit or specify 0
-     to use the default (4 hours).
+     (includes all customizations, validations, and distributions). Omit or specify 0 to use the
+     default (4 hours).
     :vartype build_timeout_in_minutes: int
     :ivar vm_profile: Describes how virtual machine is set up to build images.
     :vartype vm_profile: ~azure.mgmt.imagebuilder.models.ImageTemplateVmProfile
     :ivar staging_resource_group: The staging resource group id in the same subscription as the
      image template that will be used to build the image. If this field is empty, a resource group
      with a random name will be created. If the resource group specified in this field doesn't
      exist, it will be created with the same name. If the resource group specified exists, it must
@@ -340,15 +283,14 @@
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "identity": {"key": "identity", "type": "ImageTemplateIdentity"},
         "source": {"key": "properties.source", "type": "ImageTemplateSource"},
         "customize": {"key": "properties.customize", "type": "[ImageTemplateCustomizer]"},
-        "optimize": {"key": "properties.optimize", "type": "ImageTemplatePropertiesOptimize"},
         "validate": {"key": "properties.validate", "type": "ImageTemplatePropertiesValidate"},
         "distribute": {"key": "properties.distribute", "type": "[ImageTemplateDistributor]"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
         "provisioning_error": {"key": "properties.provisioningError", "type": "ProvisioningError"},
         "last_run_status": {"key": "properties.lastRunStatus", "type": "ImageTemplateLastRunStatus"},
         "build_timeout_in_minutes": {"key": "properties.buildTimeoutInMinutes", "type": "int"},
         "vm_profile": {"key": "properties.vmProfile", "type": "ImageTemplateVmProfile"},
@@ -360,44 +302,41 @@
         self,
         *,
         location: str,
         identity: "_models.ImageTemplateIdentity",
         tags: Optional[Dict[str, str]] = None,
         source: Optional["_models.ImageTemplateSource"] = None,
         customize: Optional[List["_models.ImageTemplateCustomizer"]] = None,
-        optimize: Optional["_models.ImageTemplatePropertiesOptimize"] = None,
         validate: Optional["_models.ImageTemplatePropertiesValidate"] = None,
         distribute: Optional[List["_models.ImageTemplateDistributor"]] = None,
         build_timeout_in_minutes: int = 0,
         vm_profile: Optional["_models.ImageTemplateVmProfile"] = None,
         staging_resource_group: Optional[str] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword identity: The identity of the image template, if configured. Required.
         :paramtype identity: ~azure.mgmt.imagebuilder.models.ImageTemplateIdentity
         :keyword source: Specifies the properties used to describe the source image.
         :paramtype source: ~azure.mgmt.imagebuilder.models.ImageTemplateSource
         :keyword customize: Specifies the properties used to describe the customization steps of the
          image, like Image source etc.
         :paramtype customize: list[~azure.mgmt.imagebuilder.models.ImageTemplateCustomizer]
-        :keyword optimize: Specifies optimization to be performed on image.
-        :paramtype optimize: ~azure.mgmt.imagebuilder.models.ImageTemplatePropertiesOptimize
         :keyword validate: Configuration options and list of validations to be performed on the
          resulting image.
         :paramtype validate: ~azure.mgmt.imagebuilder.models.ImageTemplatePropertiesValidate
         :keyword distribute: The distribution targets where the image output needs to go to.
         :paramtype distribute: list[~azure.mgmt.imagebuilder.models.ImageTemplateDistributor]
         :keyword build_timeout_in_minutes: Maximum duration to wait while building the image template
-         (includes all customizations, optimization, validations, and distributions). Omit or specify 0
-         to use the default (4 hours).
+         (includes all customizations, validations, and distributions). Omit or specify 0 to use the
+         default (4 hours).
         :paramtype build_timeout_in_minutes: int
         :keyword vm_profile: Describes how virtual machine is set up to build images.
         :paramtype vm_profile: ~azure.mgmt.imagebuilder.models.ImageTemplateVmProfile
         :keyword staging_resource_group: The staging resource group id in the same subscription as the
          image template that will be used to build the image. If this field is empty, a resource group
          with a random name will be created. If the resource group specified in this field doesn't
          exist, it will be created with the same name. If the resource group specified exists, it must
@@ -407,15 +346,14 @@
          will be deleted during template deletion and the resource group itself will remain.
         :paramtype staging_resource_group: str
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.identity = identity
         self.source = source
         self.customize = customize
-        self.optimize = optimize
         self.validate = validate
         self.distribute = distribute
         self.provisioning_state = None
         self.provisioning_error = None
         self.last_run_status = None
         self.build_timeout_in_minutes = build_timeout_in_minutes
         self.vm_profile = vm_profile
@@ -454,15 +392,15 @@
             "PowerShell": "ImageTemplatePowerShellCustomizer",
             "Shell": "ImageTemplateShellCustomizer",
             "WindowsRestart": "ImageTemplateRestartCustomizer",
             "WindowsUpdate": "ImageTemplateWindowsUpdateCustomizer",
         }
     }
 
-    def __init__(self, *, name: Optional[str] = None, **kwargs: Any) -> None:
+    def __init__(self, *, name: Optional[str] = None, **kwargs):
         """
         :keyword name: Friendly Name to provide context on what this customization step does.
         :paramtype name: str
         """
         super().__init__(**kwargs)
         self.type: Optional[str] = None
         self.name = name
@@ -501,15 +439,15 @@
         "type": {
             "ManagedImage": "ImageTemplateManagedImageDistributor",
             "SharedImage": "ImageTemplateSharedImageDistributor",
             "VHD": "ImageTemplateVhdDistributor",
         }
     }
 
-    def __init__(self, *, run_output_name: str, artifact_tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
+    def __init__(self, *, run_output_name: str, artifact_tags: Optional[Dict[str, str]] = None, **kwargs):
         """
         :keyword run_output_name: The name to be used for the associated RunOutput. Required.
         :paramtype run_output_name: str
         :keyword artifact_tags: Tags that will be applied to the artifact once it has been
          created/updated by the distributor.
         :paramtype artifact_tags: dict[str, str]
         """
@@ -554,16 +492,16 @@
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         source_uri: Optional[str] = None,
         sha256_checksum: str = "",
         destination: Optional[str] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword name: Friendly Name to provide context on what this customization step does.
         :paramtype name: str
         :keyword source_uri: The URI of the file to be uploaded for customizing the VM. It can be a
          github link, SAS URI for Azure Storage, etc.
         :paramtype source_uri: str
         :keyword sha256_checksum: SHA256 checksum of the file provided in the sourceUri field above.
@@ -575,171 +513,110 @@
         super().__init__(name=name, **kwargs)
         self.type: str = "File"
         self.source_uri = source_uri
         self.sha256_checksum = sha256_checksum
         self.destination = destination
 
 
-class ImageTemplateInVMValidator(_serialization.Model):
-    """Describes a unit of in-VM validation of image.
-
-    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
-    ImageTemplateFileValidator, ImageTemplatePowerShellValidator, ImageTemplateShellValidator
-
-    All required parameters must be populated in order to send to Azure.
+class ImageTemplateIdentity(_serialization.Model):
+    """Identity for the image template.
 
-    :ivar type: The type of validation you want to use on the Image. For example, "Shell" can be
-     shell validation. Required.
-    :vartype type: str
-    :ivar name: Friendly Name to provide context on what this validation step does.
-    :vartype name: str
+    :ivar type: The type of identity used for the image template. The type 'None' will remove any
+     identities from the image template. Known values are: "UserAssigned" and "None".
+    :vartype type: str or ~azure.mgmt.imagebuilder.models.ResourceIdentityType
+    :ivar user_assigned_identities: The list of user identities associated with the image template.
+     The user identity dictionary key references will be ARM resource ids in the form:
+     '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}'.
+    :vartype user_assigned_identities: dict[str,
+     ~azure.mgmt.imagebuilder.models.ComponentsVrq145SchemasImagetemplateidentityPropertiesUserassignedidentitiesAdditionalproperties]
     """
 
-    _validation = {
-        "type": {"required": True},
-    }
-
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
-        "name": {"key": "name", "type": "str"},
+        "user_assigned_identities": {
+            "key": "userAssignedIdentities",
+            "type": "{ComponentsVrq145SchemasImagetemplateidentityPropertiesUserassignedidentitiesAdditionalproperties}",
+        },
     }
 
-    _subtype_map = {
-        "type": {
-            "File": "ImageTemplateFileValidator",
-            "PowerShell": "ImageTemplatePowerShellValidator",
-            "Shell": "ImageTemplateShellValidator",
-        }
-    }
-
-    def __init__(self, *, name: Optional[str] = None, **kwargs: Any) -> None:
+    def __init__(
+        self,
+        *,
+        type: Optional[Union[str, "_models.ResourceIdentityType"]] = None,
+        user_assigned_identities: Optional[
+            Dict[
+                str,
+                "_models.ComponentsVrq145SchemasImagetemplateidentityPropertiesUserassignedidentitiesAdditionalproperties",
+            ]
+        ] = None,
+        **kwargs
+    ):
         """
-        :keyword name: Friendly Name to provide context on what this validation step does.
-        :paramtype name: str
+        :keyword type: The type of identity used for the image template. The type 'None' will remove
+         any identities from the image template. Known values are: "UserAssigned" and "None".
+        :paramtype type: str or ~azure.mgmt.imagebuilder.models.ResourceIdentityType
+        :keyword user_assigned_identities: The list of user identities associated with the image
+         template. The user identity dictionary key references will be ARM resource ids in the form:
+         '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}'.
+        :paramtype user_assigned_identities: dict[str,
+         ~azure.mgmt.imagebuilder.models.ComponentsVrq145SchemasImagetemplateidentityPropertiesUserassignedidentitiesAdditionalproperties]
         """
         super().__init__(**kwargs)
-        self.type: Optional[str] = None
-        self.name = name
+        self.type = type
+        self.user_assigned_identities = user_assigned_identities
 
 
-class ImageTemplateFileValidator(ImageTemplateInVMValidator):
-    """Uploads files required for validation to VMs (Linux, Windows). Corresponds to Packer file
-    provisioner.
+class ImageTemplateInVMValidator(_serialization.Model):
+    """Describes a unit of in-VM validation of image.
+
+    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
+    ImageTemplatePowerShellValidator, ImageTemplateShellValidator
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar type: The type of validation you want to use on the Image. For example, "Shell" can be
      shell validation. Required.
     :vartype type: str
     :ivar name: Friendly Name to provide context on what this validation step does.
     :vartype name: str
-    :ivar source_uri: The URI of the file to be uploaded to the VM for validation. It can be a
-     github link, Azure Storage URI (authorized or SAS), etc.
-    :vartype source_uri: str
-    :ivar sha256_checksum: SHA256 checksum of the file provided in the sourceUri field above.
-    :vartype sha256_checksum: str
-    :ivar destination: The absolute path to a file (with nested directory structures already
-     created) where the file (from sourceUri) will be uploaded to in the VM.
-    :vartype destination: str
     """
 
     _validation = {
         "type": {"required": True},
     }
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "name": {"key": "name", "type": "str"},
-        "source_uri": {"key": "sourceUri", "type": "str"},
-        "sha256_checksum": {"key": "sha256Checksum", "type": "str"},
-        "destination": {"key": "destination", "type": "str"},
     }
 
-    def __init__(
-        self,
-        *,
-        name: Optional[str] = None,
-        source_uri: Optional[str] = None,
-        sha256_checksum: str = "",
-        destination: Optional[str] = None,
-        **kwargs: Any
-    ) -> None:
+    _subtype_map = {"type": {"PowerShell": "ImageTemplatePowerShellValidator", "Shell": "ImageTemplateShellValidator"}}
+
+    def __init__(self, *, name: Optional[str] = None, **kwargs):
         """
         :keyword name: Friendly Name to provide context on what this validation step does.
         :paramtype name: str
-        :keyword source_uri: The URI of the file to be uploaded to the VM for validation. It can be a
-         github link, Azure Storage URI (authorized or SAS), etc.
-        :paramtype source_uri: str
-        :keyword sha256_checksum: SHA256 checksum of the file provided in the sourceUri field above.
-        :paramtype sha256_checksum: str
-        :keyword destination: The absolute path to a file (with nested directory structures already
-         created) where the file (from sourceUri) will be uploaded to in the VM.
-        :paramtype destination: str
-        """
-        super().__init__(name=name, **kwargs)
-        self.type: str = "File"
-        self.source_uri = source_uri
-        self.sha256_checksum = sha256_checksum
-        self.destination = destination
-
-
-class ImageTemplateIdentity(_serialization.Model):
-    """Identity for the image template.
-
-    :ivar type: The type of identity used for the image template. The type 'None' will remove any
-     identities from the image template. Known values are: "UserAssigned" and "None".
-    :vartype type: str or ~azure.mgmt.imagebuilder.models.ResourceIdentityType
-    :ivar user_assigned_identities: The set of user assigned identities associated with the
-     resource. The userAssignedIdentities dictionary keys will be ARM resource ids in the form:
-     '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}.
-     The dictionary values can be empty objects ({}) in requests.
-    :vartype user_assigned_identities: dict[str,
-     ~azure.mgmt.imagebuilder.models.UserAssignedIdentity]
-    """
-
-    _attribute_map = {
-        "type": {"key": "type", "type": "str"},
-        "user_assigned_identities": {"key": "userAssignedIdentities", "type": "{UserAssignedIdentity}"},
-    }
-
-    def __init__(
-        self,
-        *,
-        type: Optional[Union[str, "_models.ResourceIdentityType"]] = None,
-        user_assigned_identities: Optional[Dict[str, "_models.UserAssignedIdentity"]] = None,
-        **kwargs: Any
-    ) -> None:
-        """
-        :keyword type: The type of identity used for the image template. The type 'None' will remove
-         any identities from the image template. Known values are: "UserAssigned" and "None".
-        :paramtype type: str or ~azure.mgmt.imagebuilder.models.ResourceIdentityType
-        :keyword user_assigned_identities: The set of user assigned identities associated with the
-         resource. The userAssignedIdentities dictionary keys will be ARM resource ids in the form:
-         '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}.
-         The dictionary values can be empty objects ({}) in requests.
-        :paramtype user_assigned_identities: dict[str,
-         ~azure.mgmt.imagebuilder.models.UserAssignedIdentity]
         """
         super().__init__(**kwargs)
-        self.type = type
-        self.user_assigned_identities = user_assigned_identities
+        self.type: Optional[str] = None
+        self.name = name
 
 
 class ImageTemplateLastRunStatus(_serialization.Model):
     """Describes the latest status of running an image template.
 
     :ivar start_time: Start time of the last run (UTC).
     :vartype start_time: ~datetime.datetime
     :ivar end_time: End time of the last run (UTC).
     :vartype end_time: ~datetime.datetime
     :ivar run_state: State of the last run. Known values are: "Running", "Canceling", "Succeeded",
      "PartiallySucceeded", "Failed", and "Canceled".
     :vartype run_state: str or ~azure.mgmt.imagebuilder.models.RunState
     :ivar run_sub_state: Sub-state of the last run. Known values are: "Queued", "Building",
-     "Customizing", "Optimizing", "Validating", and "Distributing".
+     "Customizing", "Validating", and "Distributing".
     :vartype run_sub_state: str or ~azure.mgmt.imagebuilder.models.RunSubState
     :ivar message: Verbose information about the last run state.
     :vartype message: str
     """
 
     _attribute_map = {
         "start_time": {"key": "startTime", "type": "iso-8601"},
@@ -753,26 +630,26 @@
         self,
         *,
         start_time: Optional[datetime.datetime] = None,
         end_time: Optional[datetime.datetime] = None,
         run_state: Optional[Union[str, "_models.RunState"]] = None,
         run_sub_state: Optional[Union[str, "_models.RunSubState"]] = None,
         message: Optional[str] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword start_time: Start time of the last run (UTC).
         :paramtype start_time: ~datetime.datetime
         :keyword end_time: End time of the last run (UTC).
         :paramtype end_time: ~datetime.datetime
         :keyword run_state: State of the last run. Known values are: "Running", "Canceling",
          "Succeeded", "PartiallySucceeded", "Failed", and "Canceled".
         :paramtype run_state: str or ~azure.mgmt.imagebuilder.models.RunState
         :keyword run_sub_state: Sub-state of the last run. Known values are: "Queued", "Building",
-         "Customizing", "Optimizing", "Validating", and "Distributing".
+         "Customizing", "Validating", and "Distributing".
         :paramtype run_sub_state: str or ~azure.mgmt.imagebuilder.models.RunSubState
         :keyword message: Verbose information about the last run state.
         :paramtype message: str
         """
         super().__init__(**kwargs)
         self.start_time = start_time
         self.end_time = end_time
@@ -792,16 +669,16 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[ImageTemplate]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.ImageTemplate"]] = None, next_link: Optional[str] = None, **kwargs: Any
-    ) -> None:
+        self, *, value: Optional[List["_models.ImageTemplate"]] = None, next_link: Optional[str] = None, **kwargs
+    ):
         """
         :keyword value: An array of image templates.
         :paramtype value: list[~azure.mgmt.imagebuilder.models.ImageTemplate]
         :keyword next_link: The continuation token.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
@@ -845,16 +722,16 @@
     def __init__(
         self,
         *,
         run_output_name: str,
         image_id: str,
         location: str,
         artifact_tags: Optional[Dict[str, str]] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword run_output_name: The name to be used for the associated RunOutput. Required.
         :paramtype run_output_name: str
         :keyword artifact_tags: Tags that will be applied to the artifact once it has been
          created/updated by the distributor.
         :paramtype artifact_tags: dict[str, str]
         :keyword image_id: Resource Id of the Managed Disk Image. Required.
@@ -894,23 +771,22 @@
         "type": {
             "ManagedImage": "ImageTemplateManagedImageSource",
             "PlatformImage": "ImageTemplatePlatformImageSource",
             "SharedImageVersion": "ImageTemplateSharedImageVersionSource",
         }
     }
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(self, **kwargs):
         """ """
         super().__init__(**kwargs)
         self.type: Optional[str] = None
 
 
 class ImageTemplateManagedImageSource(ImageTemplateSource):
-    """Describes an image source that is a managed image in customer subscription. This image must
-    reside in the same subscription and region as the Image Builder template.
+    """Describes an image source that is a managed image in customer subscription. This image must reside in the same subscription and region as the Image Builder template.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar type: Specifies the type of source image you want to start with. Required.
     :vartype type: str
     :ivar image_id: ARM resource id of the managed image in customer subscription. Required.
     :vartype image_id: str
@@ -922,27 +798,26 @@
     }
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "image_id": {"key": "imageId", "type": "str"},
     }
 
-    def __init__(self, *, image_id: str, **kwargs: Any) -> None:
+    def __init__(self, *, image_id: str, **kwargs):
         """
         :keyword image_id: ARM resource id of the managed image in customer subscription. Required.
         :paramtype image_id: str
         """
         super().__init__(**kwargs)
         self.type: str = "ManagedImage"
         self.image_id = image_id
 
 
 class ImageTemplatePlatformImageSource(ImageTemplateSource):
-    """Describes an image source from `Azure Gallery Images
-    <https://docs.microsoft.com/en-us/rest/api/compute/virtualmachineimages>`_.
+    """Describes an image source from `Azure Gallery Images <https://docs.microsoft.com/en-us/rest/api/compute/virtualmachineimages>`_.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar type: Specifies the type of source image you want to start with. Required.
     :vartype type: str
@@ -987,16 +862,16 @@
         self,
         *,
         publisher: Optional[str] = None,
         offer: Optional[str] = None,
         sku: Optional[str] = None,
         version: Optional[str] = None,
         plan_info: Optional["_models.PlatformImagePurchasePlan"] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword publisher: Image Publisher in `Azure Gallery Images
          <https://docs.microsoft.com/en-us/rest/api/compute/virtualmachineimages>`_.
         :paramtype publisher: str
         :keyword offer: Image offer from the `Azure Gallery Images
          <https://docs.microsoft.com/en-us/rest/api/compute/virtualmachineimages>`_.
         :paramtype offer: str
@@ -1018,16 +893,15 @@
         self.sku = sku
         self.version = version
         self.exact_version = None
         self.plan_info = plan_info
 
 
 class ImageTemplatePowerShellCustomizer(ImageTemplateCustomizer):
-    """Runs the specified PowerShell on the VM (Windows). Corresponds to Packer powershell
-    provisioner. Exactly one of 'scriptUri' or 'inline' can be specified.
+    """Runs the specified PowerShell on the VM (Windows). Corresponds to Packer powershell provisioner. Exactly one of 'scriptUri' or 'inline' can be specified.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar type: The type of customization tool you want to use on the Image. For example, "Shell"
      can be shell customizer. Required.
     :vartype type: str
     :ivar name: Friendly Name to provide context on what this customization step does.
@@ -1070,16 +944,16 @@
         name: Optional[str] = None,
         script_uri: Optional[str] = None,
         sha256_checksum: str = "",
         inline: Optional[List[str]] = None,
         run_elevated: bool = False,
         run_as_system: bool = False,
         valid_exit_codes: Optional[List[int]] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword name: Friendly Name to provide context on what this customization step does.
         :paramtype name: str
         :keyword script_uri: URI of the PowerShell script to be run for customizing. It can be a github
          link, SAS URI for Azure Storage, etc.
         :paramtype script_uri: str
         :keyword sha256_checksum: SHA256 checksum of the power shell script provided in the scriptUri
@@ -1104,16 +978,15 @@
         self.inline = inline
         self.run_elevated = run_elevated
         self.run_as_system = run_as_system
         self.valid_exit_codes = valid_exit_codes
 
 
 class ImageTemplatePowerShellValidator(ImageTemplateInVMValidator):
-    """Runs the specified PowerShell script during the validation phase (Windows). Corresponds to
-    Packer powershell provisioner. Exactly one of 'scriptUri' or 'inline' can be specified.
+    """Runs the specified PowerShell script during the validation phase (Windows). Corresponds to Packer powershell provisioner. Exactly one of 'scriptUri' or 'inline' can be specified.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar type: The type of validation you want to use on the Image. For example, "Shell" can be
      shell validation. Required.
     :vartype type: str
     :ivar name: Friendly Name to provide context on what this validation step does.
@@ -1156,16 +1029,16 @@
         name: Optional[str] = None,
         script_uri: Optional[str] = None,
         sha256_checksum: str = "",
         inline: Optional[List[str]] = None,
         run_elevated: bool = False,
         run_as_system: bool = False,
         valid_exit_codes: Optional[List[int]] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword name: Friendly Name to provide context on what this validation step does.
         :paramtype name: str
         :keyword script_uri: URI of the PowerShell script to be run for validation. It can be a github
          link, Azure Storage URI, etc.
         :paramtype script_uri: str
         :keyword sha256_checksum: SHA256 checksum of the power shell script provided in the scriptUri
@@ -1189,58 +1062,14 @@
         self.sha256_checksum = sha256_checksum
         self.inline = inline
         self.run_elevated = run_elevated
         self.run_as_system = run_as_system
         self.valid_exit_codes = valid_exit_codes
 
 
-class ImageTemplatePropertiesOptimize(_serialization.Model):
-    """Specifies optimization to be performed on image.
-
-    :ivar vm_boot: Optimization is applied on the image for a faster VM boot.
-    :vartype vm_boot: ~azure.mgmt.imagebuilder.models.ImageTemplatePropertiesOptimizeVmBoot
-    """
-
-    _attribute_map = {
-        "vm_boot": {"key": "vmBoot", "type": "ImageTemplatePropertiesOptimizeVmBoot"},
-    }
-
-    def __init__(
-        self, *, vm_boot: Optional["_models.ImageTemplatePropertiesOptimizeVmBoot"] = None, **kwargs: Any
-    ) -> None:
-        """
-        :keyword vm_boot: Optimization is applied on the image for a faster VM boot.
-        :paramtype vm_boot: ~azure.mgmt.imagebuilder.models.ImageTemplatePropertiesOptimizeVmBoot
-        """
-        super().__init__(**kwargs)
-        self.vm_boot = vm_boot
-
-
-class ImageTemplatePropertiesOptimizeVmBoot(_serialization.Model):
-    """Optimization is applied on the image for a faster VM boot.
-
-    :ivar state: Enabling this field will improve VM boot time by optimizing the final customized
-     image output. Known values are: "Enabled" and "Disabled".
-    :vartype state: str or ~azure.mgmt.imagebuilder.models.VMBootOptimizationState
-    """
-
-    _attribute_map = {
-        "state": {"key": "state", "type": "str"},
-    }
-
-    def __init__(self, *, state: Optional[Union[str, "_models.VMBootOptimizationState"]] = None, **kwargs: Any) -> None:
-        """
-        :keyword state: Enabling this field will improve VM boot time by optimizing the final
-         customized image output. Known values are: "Enabled" and "Disabled".
-        :paramtype state: str or ~azure.mgmt.imagebuilder.models.VMBootOptimizationState
-        """
-        super().__init__(**kwargs)
-        self.state = state
-
-
 class ImageTemplatePropertiesValidate(_serialization.Model):
     """Configuration options and list of validations to be performed on the resulting image.
 
     :ivar continue_distribute_on_failure: If validation fails and this field is set to false,
      output image(s) will not be distributed. This is the default behavior. If validation fails and
      this field is set to true, output image(s) will still be distributed. Please use this option
      with caution as it may result in bad images being distributed for use. In either case (true or
@@ -1263,16 +1092,16 @@
 
     def __init__(
         self,
         *,
         continue_distribute_on_failure: bool = False,
         source_validation_only: bool = False,
         in_vm_validations: Optional[List["_models.ImageTemplateInVMValidator"]] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword continue_distribute_on_failure: If validation fails and this field is set to false,
          output image(s) will not be distributed. This is the default behavior. If validation fails and
          this field is set to true, output image(s) will still be distributed. Please use this option
          with caution as it may result in bad images being distributed for use. In either case (true or
          false), the end to end image run will be reported as having failed in case of a validation
          failure. [Note: This field has no effect if validation succeeds.].
@@ -1287,16 +1116,15 @@
         super().__init__(**kwargs)
         self.continue_distribute_on_failure = continue_distribute_on_failure
         self.source_validation_only = source_validation_only
         self.in_vm_validations = in_vm_validations
 
 
 class ImageTemplateRestartCustomizer(ImageTemplateCustomizer):
-    """Reboots a VM and waits for it to come back online (Windows). Corresponds to Packer
-    windows-restart provisioner.
+    """Reboots a VM and waits for it to come back online (Windows). Corresponds to Packer windows-restart provisioner.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar type: The type of customization tool you want to use on the Image. For example, "Shell"
      can be shell customizer. Required.
     :vartype type: str
     :ivar name: Friendly Name to provide context on what this customization step does.
@@ -1326,16 +1154,16 @@
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         restart_command: Optional[str] = None,
         restart_check_command: Optional[str] = None,
         restart_timeout: Optional[str] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword name: Friendly Name to provide context on what this customization step does.
         :paramtype name: str
         :keyword restart_command: Command to execute the restart [Default: 'shutdown /r /f /t 0 /c
          "packer restart"'].
         :paramtype restart_command: str
         :keyword restart_check_command: Command to check if restart succeeded [Default: ''].
@@ -1348,163 +1176,127 @@
         self.type: str = "WindowsRestart"
         self.restart_command = restart_command
         self.restart_check_command = restart_check_command
         self.restart_timeout = restart_timeout
 
 
 class ImageTemplateSharedImageDistributor(ImageTemplateDistributor):
-    """Distribute via Azure Compute Gallery.
+    """Distribute via Shared Image Gallery.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar type: Type of distribution. Required.
     :vartype type: str
     :ivar run_output_name: The name to be used for the associated RunOutput. Required.
     :vartype run_output_name: str
     :ivar artifact_tags: Tags that will be applied to the artifact once it has been created/updated
      by the distributor.
     :vartype artifact_tags: dict[str, str]
-    :ivar gallery_image_id: Resource Id of the Azure Compute Gallery image. Required.
+    :ivar gallery_image_id: Resource Id of the Shared Image Gallery image. Required.
     :vartype gallery_image_id: str
-    :ivar replication_regions: [Deprecated] A list of regions that the image will be replicated to.
-     This list can be specified only if targetRegions is not specified. This field is deprecated -
-     use targetRegions instead.
+    :ivar replication_regions: A list of regions that the image will be replicated to. Required.
     :vartype replication_regions: list[str]
     :ivar exclude_from_latest: Flag that indicates whether created image version should be excluded
      from latest. Omit to use the default (false).
     :vartype exclude_from_latest: bool
-    :ivar storage_account_type: [Deprecated] Storage account type to be used to store the shared
-     image. Omit to use the default (Standard_LRS). This field can be specified only if
-     replicationRegions is specified. This field is deprecated - use targetRegions instead. Known
-     values are: "Standard_LRS", "Standard_ZRS", and "Premium_LRS".
+    :ivar storage_account_type: Storage account type to be used to store the shared image. Omit to
+     use the default (Standard_LRS). Known values are: "Standard_LRS" and "Standard_ZRS".
     :vartype storage_account_type: str or
      ~azure.mgmt.imagebuilder.models.SharedImageStorageAccountType
-    :ivar target_regions: The target regions where the distributed Image Version is going to be
-     replicated to. This object supersedes replicationRegions and can be specified only if
-     replicationRegions is not specified.
-    :vartype target_regions: list[~azure.mgmt.imagebuilder.models.TargetRegion]
-    :ivar versioning: Describes how to generate new x.y.z version number for distribution.
-    :vartype versioning: ~azure.mgmt.imagebuilder.models.DistributeVersioner
     """
 
     _validation = {
         "type": {"required": True},
         "run_output_name": {"required": True, "pattern": r"^[A-Za-z0-9-_.]{1,64}$"},
         "gallery_image_id": {"required": True},
+        "replication_regions": {"required": True},
     }
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "run_output_name": {"key": "runOutputName", "type": "str"},
         "artifact_tags": {"key": "artifactTags", "type": "{str}"},
         "gallery_image_id": {"key": "galleryImageId", "type": "str"},
         "replication_regions": {"key": "replicationRegions", "type": "[str]"},
         "exclude_from_latest": {"key": "excludeFromLatest", "type": "bool"},
         "storage_account_type": {"key": "storageAccountType", "type": "str"},
-        "target_regions": {"key": "targetRegions", "type": "[TargetRegion]"},
-        "versioning": {"key": "versioning", "type": "DistributeVersioner"},
     }
 
     def __init__(
         self,
         *,
         run_output_name: str,
         gallery_image_id: str,
+        replication_regions: List[str],
         artifact_tags: Optional[Dict[str, str]] = None,
-        replication_regions: Optional[List[str]] = None,
         exclude_from_latest: bool = False,
         storage_account_type: Optional[Union[str, "_models.SharedImageStorageAccountType"]] = None,
-        target_regions: Optional[List["_models.TargetRegion"]] = None,
-        versioning: Optional["_models.DistributeVersioner"] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword run_output_name: The name to be used for the associated RunOutput. Required.
         :paramtype run_output_name: str
         :keyword artifact_tags: Tags that will be applied to the artifact once it has been
          created/updated by the distributor.
         :paramtype artifact_tags: dict[str, str]
-        :keyword gallery_image_id: Resource Id of the Azure Compute Gallery image. Required.
+        :keyword gallery_image_id: Resource Id of the Shared Image Gallery image. Required.
         :paramtype gallery_image_id: str
-        :keyword replication_regions: [Deprecated] A list of regions that the image will be replicated
-         to. This list can be specified only if targetRegions is not specified. This field is deprecated
-         - use targetRegions instead.
+        :keyword replication_regions: A list of regions that the image will be replicated to. Required.
         :paramtype replication_regions: list[str]
         :keyword exclude_from_latest: Flag that indicates whether created image version should be
          excluded from latest. Omit to use the default (false).
         :paramtype exclude_from_latest: bool
-        :keyword storage_account_type: [Deprecated] Storage account type to be used to store the shared
-         image. Omit to use the default (Standard_LRS). This field can be specified only if
-         replicationRegions is specified. This field is deprecated - use targetRegions instead. Known
-         values are: "Standard_LRS", "Standard_ZRS", and "Premium_LRS".
+        :keyword storage_account_type: Storage account type to be used to store the shared image. Omit
+         to use the default (Standard_LRS). Known values are: "Standard_LRS" and "Standard_ZRS".
         :paramtype storage_account_type: str or
          ~azure.mgmt.imagebuilder.models.SharedImageStorageAccountType
-        :keyword target_regions: The target regions where the distributed Image Version is going to be
-         replicated to. This object supersedes replicationRegions and can be specified only if
-         replicationRegions is not specified.
-        :paramtype target_regions: list[~azure.mgmt.imagebuilder.models.TargetRegion]
-        :keyword versioning: Describes how to generate new x.y.z version number for distribution.
-        :paramtype versioning: ~azure.mgmt.imagebuilder.models.DistributeVersioner
         """
         super().__init__(run_output_name=run_output_name, artifact_tags=artifact_tags, **kwargs)
         self.type: str = "SharedImage"
         self.gallery_image_id = gallery_image_id
         self.replication_regions = replication_regions
         self.exclude_from_latest = exclude_from_latest
         self.storage_account_type = storage_account_type
-        self.target_regions = target_regions
-        self.versioning = versioning
 
 
 class ImageTemplateSharedImageVersionSource(ImageTemplateSource):
-    """Describes an image source that is an image version in an Azure Compute Gallery or a Direct
-    Shared Gallery.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
+    """Describes an image source that is an image version in a shared image gallery.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar type: Specifies the type of source image you want to start with. Required.
     :vartype type: str
-    :ivar image_version_id: ARM resource id of the image version. When image version name is
-     'latest', the version is evaluated when the image build takes place. Required.
+    :ivar image_version_id: ARM resource id of the image version in the shared image gallery.
+     Required.
     :vartype image_version_id: str
-    :ivar exact_version: Exact ARM resource id of the image version. This readonly field differs
-     from the image version Id in 'imageVersionId' only if the version name specified in
-     'imageVersionId' field is 'latest'.
-    :vartype exact_version: str
     """
 
     _validation = {
         "type": {"required": True},
         "image_version_id": {"required": True},
-        "exact_version": {"readonly": True},
     }
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "image_version_id": {"key": "imageVersionId", "type": "str"},
-        "exact_version": {"key": "exactVersion", "type": "str"},
     }
 
-    def __init__(self, *, image_version_id: str, **kwargs: Any) -> None:
+    def __init__(self, *, image_version_id: str, **kwargs):
         """
-        :keyword image_version_id: ARM resource id of the image version. When image version name is
-         'latest', the version is evaluated when the image build takes place. Required.
+        :keyword image_version_id: ARM resource id of the image version in the shared image gallery.
+         Required.
         :paramtype image_version_id: str
         """
         super().__init__(**kwargs)
         self.type: str = "SharedImageVersion"
         self.image_version_id = image_version_id
-        self.exact_version = None
 
 
 class ImageTemplateShellCustomizer(ImageTemplateCustomizer):
-    """Runs a shell script during the customization phase (Linux). Corresponds to Packer shell
-    provisioner. Exactly one of 'scriptUri' or 'inline' can be specified.
+    """Runs a shell script during the customization phase (Linux). Corresponds to Packer shell provisioner. Exactly one of 'scriptUri' or 'inline' can be specified.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar type: The type of customization tool you want to use on the Image. For example, "Shell"
      can be shell customizer. Required.
     :vartype type: str
     :ivar name: Friendly Name to provide context on what this customization step does.
@@ -1533,16 +1325,16 @@
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         script_uri: Optional[str] = None,
         sha256_checksum: str = "",
         inline: Optional[List[str]] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword name: Friendly Name to provide context on what this customization step does.
         :paramtype name: str
         :keyword script_uri: URI of the shell script to be run for customizing. It can be a github
          link, SAS URI for Azure Storage, etc.
         :paramtype script_uri: str
         :keyword sha256_checksum: SHA256 checksum of the shell script provided in the scriptUri field.
@@ -1554,16 +1346,15 @@
         self.type: str = "Shell"
         self.script_uri = script_uri
         self.sha256_checksum = sha256_checksum
         self.inline = inline
 
 
 class ImageTemplateShellValidator(ImageTemplateInVMValidator):
-    """Runs the specified shell script during the validation phase (Linux). Corresponds to Packer
-    shell provisioner. Exactly one of 'scriptUri' or 'inline' can be specified.
+    """Runs the specified shell script during the validation phase (Linux). Corresponds to Packer shell provisioner. Exactly one of 'scriptUri' or 'inline' can be specified.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar type: The type of validation you want to use on the Image. For example, "Shell" can be
      shell validation. Required.
     :vartype type: str
     :ivar name: Friendly Name to provide context on what this validation step does.
@@ -1592,16 +1383,16 @@
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         script_uri: Optional[str] = None,
         sha256_checksum: str = "",
         inline: Optional[List[str]] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword name: Friendly Name to provide context on what this validation step does.
         :paramtype name: str
         :keyword script_uri: URI of the shell script to be run for validation. It can be a github link,
          Azure Storage URI, etc.
         :paramtype script_uri: str
         :keyword sha256_checksum: SHA256 checksum of the shell script provided in the scriptUri field.
@@ -1631,16 +1422,16 @@
     }
 
     def __init__(
         self,
         *,
         identity: Optional["_models.ImageTemplateIdentity"] = None,
         tags: Optional[Dict[str, str]] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword identity: The identity of the image template, if configured.
         :paramtype identity: ~azure.mgmt.imagebuilder.models.ImageTemplateIdentity
         :keyword tags: The user-specified tags associated with the image template.
         :paramtype tags: dict[str, str]
         """
         super().__init__(**kwargs)
@@ -1656,54 +1447,37 @@
     :ivar type: Type of distribution. Required.
     :vartype type: str
     :ivar run_output_name: The name to be used for the associated RunOutput. Required.
     :vartype run_output_name: str
     :ivar artifact_tags: Tags that will be applied to the artifact once it has been created/updated
      by the distributor.
     :vartype artifact_tags: dict[str, str]
-    :ivar uri: Optional Azure Storage URI for the distributed VHD blob. Omit to use the default
-     (empty string) in which case VHD would be published to the storage account in the staging
-     resource group.
-    :vartype uri: str
     """
 
     _validation = {
         "type": {"required": True},
         "run_output_name": {"required": True, "pattern": r"^[A-Za-z0-9-_.]{1,64}$"},
     }
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "run_output_name": {"key": "runOutputName", "type": "str"},
         "artifact_tags": {"key": "artifactTags", "type": "{str}"},
-        "uri": {"key": "uri", "type": "str"},
     }
 
-    def __init__(
-        self,
-        *,
-        run_output_name: str,
-        artifact_tags: Optional[Dict[str, str]] = None,
-        uri: Optional[str] = None,
-        **kwargs: Any
-    ) -> None:
+    def __init__(self, *, run_output_name: str, artifact_tags: Optional[Dict[str, str]] = None, **kwargs):
         """
         :keyword run_output_name: The name to be used for the associated RunOutput. Required.
         :paramtype run_output_name: str
         :keyword artifact_tags: Tags that will be applied to the artifact once it has been
          created/updated by the distributor.
         :paramtype artifact_tags: dict[str, str]
-        :keyword uri: Optional Azure Storage URI for the distributed VHD blob. Omit to use the default
-         (empty string) in which case VHD would be published to the storage account in the staging
-         resource group.
-        :paramtype uri: str
         """
         super().__init__(run_output_name=run_output_name, artifact_tags=artifact_tags, **kwargs)
         self.type: str = "VHD"
-        self.uri = uri
 
 
 class ImageTemplateVmProfile(_serialization.Model):
     """Describes the virtual machines used to build and validate images.
 
     :ivar vm_size: Size of the virtual machine used to build, customize and capture images. Omit or
      specify empty string to use the default (Standard_D1_v2 for Gen1 images and Standard_D2ds_v4
@@ -1735,16 +1509,16 @@
     def __init__(
         self,
         *,
         vm_size: str = "",
         os_disk_size_gb: int = 0,
         user_assigned_identities: Optional[List[str]] = None,
         vnet_config: Optional["_models.VirtualNetworkConfig"] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword vm_size: Size of the virtual machine used to build, customize and capture images. Omit
          or specify empty string to use the default (Standard_D1_v2 for Gen1 images and Standard_D2ds_v4
          for Gen2 images).
         :paramtype vm_size: str
         :keyword os_disk_size_gb: Size of the OS disk in GB. Omit or specify 0 to use Azure's default
          OS disk size.
@@ -1761,16 +1535,15 @@
         self.vm_size = vm_size
         self.os_disk_size_gb = os_disk_size_gb
         self.user_assigned_identities = user_assigned_identities
         self.vnet_config = vnet_config
 
 
 class ImageTemplateWindowsUpdateCustomizer(ImageTemplateCustomizer):
-    """Installs Windows Updates. Corresponds to Packer Windows Update Provisioner
-    (https://github.com/rgl/packer-provisioner-windows-update).
+    """Installs Windows Updates. Corresponds to Packer Windows Update Provisioner (https://github.com/rgl/packer-provisioner-windows-update).
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar type: The type of customization tool you want to use on the Image. For example, "Shell"
      can be shell customizer. Required.
     :vartype type: str
     :ivar name: Friendly Name to provide context on what this customization step does.
@@ -1802,17 +1575,17 @@
 
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         search_criteria: Optional[str] = None,
         filters: Optional[List[str]] = None,
-        update_limit: int = 0,
-        **kwargs: Any
-    ) -> None:
+        update_limit: Optional[int] = None,
+        **kwargs
+    ):
         """
         :keyword name: Friendly Name to provide context on what this customization step does.
         :paramtype name: str
         :keyword search_criteria: Criteria to search updates. Omit or specify empty string to use the
          default (search all). Refer to above link for examples and detailed description of this field.
         :paramtype search_criteria: str
         :keyword filters: Array of filters to select updates to apply. Omit or specify empty array to
@@ -1857,16 +1630,16 @@
         self,
         *,
         name: Optional[str] = None,
         display: Optional["_models.OperationDisplay"] = None,
         origin: Optional[str] = None,
         properties: Optional[JSON] = None,
         is_data_action: Optional[bool] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword name: This is of the format {provider}/{resource}/{operation}.
         :paramtype name: str
         :keyword display: The object that describes the operation.
         :paramtype display: ~azure.mgmt.imagebuilder.models.OperationDisplay
         :keyword origin: The intended executor of the operation.
         :paramtype origin: str
@@ -1906,16 +1679,16 @@
     def __init__(
         self,
         *,
         provider: Optional[str] = None,
         operation: Optional[str] = None,
         resource: Optional[str] = None,
         description: Optional[str] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword provider: Friendly name of the resource provider.
         :paramtype provider: str
         :keyword operation: For example: read, write, delete, or listKeys/action.
         :paramtype operation: str
         :keyword resource: The resource type on which the operation is performed.
         :paramtype resource: str
@@ -1926,31 +1699,28 @@
         self.provider = provider
         self.operation = operation
         self.resource = resource
         self.description = description
 
 
 class OperationListResult(_serialization.Model):
-    """Result of the request to list REST API operations. It contains a list of operations and a URL
-    nextLink to get the next set of results.
+    """Result of the request to list REST API operations. It contains a list of operations and a URL nextLink to get the next set of results.
 
     :ivar value: The list of operations supported by the resource provider.
     :vartype value: list[~azure.mgmt.imagebuilder.models.Operation]
     :ivar next_link: The URL to get the next set of operation list results if there are any.
     :vartype next_link: str
     """
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Operation]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(
-        self, *, value: Optional[List["_models.Operation"]] = None, next_link: Optional[str] = None, **kwargs: Any
-    ) -> None:
+    def __init__(self, *, value: Optional[List["_models.Operation"]] = None, next_link: Optional[str] = None, **kwargs):
         """
         :keyword value: The list of operations supported by the resource provider.
         :paramtype value: list[~azure.mgmt.imagebuilder.models.Operation]
         :keyword next_link: The URL to get the next set of operation list results if there are any.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
@@ -1979,15 +1749,15 @@
 
     _attribute_map = {
         "plan_name": {"key": "planName", "type": "str"},
         "plan_product": {"key": "planProduct", "type": "str"},
         "plan_publisher": {"key": "planPublisher", "type": "str"},
     }
 
-    def __init__(self, *, plan_name: str, plan_product: str, plan_publisher: str, **kwargs: Any) -> None:
+    def __init__(self, *, plan_name: str, plan_product: str, plan_publisher: str, **kwargs):
         """
         :keyword plan_name: Name of the purchase plan. Required.
         :paramtype plan_name: str
         :keyword plan_product: Product of the purchase plan. Required.
         :paramtype plan_product: str
         :keyword plan_publisher: Publisher of the purchase plan. Required.
         :paramtype plan_publisher: str
@@ -2017,16 +1787,16 @@
     }
 
     def __init__(
         self,
         *,
         provisioning_error_code: Optional[Union[str, "_models.ProvisioningErrorCode"]] = None,
         message: Optional[str] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword provisioning_error_code: Error code of the provisioning failure. Known values are:
          "BadSourceType", "BadPIRSource", "BadManagedImageSource", "BadSharedImageVersionSource",
          "BadCustomizerType", "UnsupportedCustomizerType", "NoCustomizerScript", "BadValidatorType",
          "UnsupportedValidatorType", "NoValidatorScript", "BadDistributeType",
          "BadSharedImageDistribute", "BadStagingResourceGroup", "ServerError", and "Other".
         :paramtype provisioning_error_code: str or
@@ -2036,16 +1806,15 @@
         """
         super().__init__(**kwargs)
         self.provisioning_error_code = provisioning_error_code
         self.message = message
 
 
 class ProxyResource(Resource):
-    """The resource model definition for a Azure Resource Manager proxy resource. It will not have
-    tags and a location.
+    """The resource model definition for a Azure Resource Manager proxy resource. It will not have tags and a location.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
     :vartype id: str
     :ivar name: The name of the resource.
@@ -2068,15 +1837,15 @@
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(self, **kwargs):
         """ """
         super().__init__(**kwargs)
 
 
 class RunOutput(ProxyResource):
     """Represents an output that was created by running an image template.
 
@@ -2094,15 +1863,15 @@
      information.
     :vartype system_data: ~azure.mgmt.imagebuilder.models.SystemData
     :ivar artifact_id: The resource id of the artifact.
     :vartype artifact_id: str
     :ivar artifact_uri: The location URI of the artifact.
     :vartype artifact_uri: str
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Creating",
-     "Updating", "Succeeded", "Failed", "Deleting", and "Canceled".
+     "Updating", "Succeeded", "Failed", and "Deleting".
     :vartype provisioning_state: str or ~azure.mgmt.imagebuilder.models.ProvisioningState
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
@@ -2116,15 +1885,15 @@
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "artifact_id": {"key": "properties.artifactId", "type": "str"},
         "artifact_uri": {"key": "properties.artifactUri", "type": "str"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
     }
 
-    def __init__(self, *, artifact_id: Optional[str] = None, artifact_uri: Optional[str] = None, **kwargs: Any) -> None:
+    def __init__(self, *, artifact_id: Optional[str] = None, artifact_uri: Optional[str] = None, **kwargs):
         """
         :keyword artifact_id: The resource id of the artifact.
         :paramtype artifact_id: str
         :keyword artifact_uri: The location URI of the artifact.
         :paramtype artifact_uri: str
         """
         super().__init__(**kwargs)
@@ -2143,103 +1912,26 @@
     """
 
     _attribute_map = {
         "value": {"key": "value", "type": "[RunOutput]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(
-        self, *, value: Optional[List["_models.RunOutput"]] = None, next_link: Optional[str] = None, **kwargs: Any
-    ) -> None:
+    def __init__(self, *, value: Optional[List["_models.RunOutput"]] = None, next_link: Optional[str] = None, **kwargs):
         """
         :keyword value: An array of run outputs.
         :paramtype value: list[~azure.mgmt.imagebuilder.models.RunOutput]
         :keyword next_link: The continuation token.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
-class TriggerProperties(_serialization.Model):
-    """Describes the properties of a trigger.
-
-    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
-    SourceImageTriggerProperties
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar kind: The kind of trigger. Required.
-    :vartype kind: str
-    :ivar status: Trigger status.
-    :vartype status: ~azure.mgmt.imagebuilder.models.TriggerStatus
-    :ivar provisioning_state: Provisioning state of the resource. Known values are: "Creating",
-     "Updating", "Succeeded", "Failed", "Deleting", and "Canceled".
-    :vartype provisioning_state: str or ~azure.mgmt.imagebuilder.models.ProvisioningState
-    """
-
-    _validation = {
-        "kind": {"required": True},
-        "status": {"readonly": True},
-        "provisioning_state": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "kind": {"key": "kind", "type": "str"},
-        "status": {"key": "status", "type": "TriggerStatus"},
-        "provisioning_state": {"key": "provisioningState", "type": "str"},
-    }
-
-    _subtype_map = {"kind": {"SourceImage": "SourceImageTriggerProperties"}}
-
-    def __init__(self, **kwargs: Any) -> None:
-        """ """
-        super().__init__(**kwargs)
-        self.kind: Optional[str] = None
-        self.status = None
-        self.provisioning_state = None
-
-
-class SourceImageTriggerProperties(TriggerProperties):
-    """Properties of SourceImage kind of trigger.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar kind: The kind of trigger. Required.
-    :vartype kind: str
-    :ivar status: Trigger status.
-    :vartype status: ~azure.mgmt.imagebuilder.models.TriggerStatus
-    :ivar provisioning_state: Provisioning state of the resource. Known values are: "Creating",
-     "Updating", "Succeeded", "Failed", "Deleting", and "Canceled".
-    :vartype provisioning_state: str or ~azure.mgmt.imagebuilder.models.ProvisioningState
-    """
-
-    _validation = {
-        "kind": {"required": True},
-        "status": {"readonly": True},
-        "provisioning_state": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "kind": {"key": "kind", "type": "str"},
-        "status": {"key": "status", "type": "TriggerStatus"},
-        "provisioning_state": {"key": "provisioningState", "type": "str"},
-    }
-
-    def __init__(self, **kwargs: Any) -> None:
-        """ """
-        super().__init__(**kwargs)
-        self.kind: str = "SourceImage"
-
-
 class SystemData(_serialization.Model):
     """Metadata pertaining to creation and last modification of the resource.
 
     :ivar created_by: The identity that created the resource.
     :vartype created_by: str
     :ivar created_by_type: The type of identity that created the resource. Known values are:
      "User", "Application", "ManagedIdentity", and "Key".
@@ -2269,16 +1961,16 @@
         *,
         created_by: Optional[str] = None,
         created_by_type: Optional[Union[str, "_models.CreatedByType"]] = None,
         created_at: Optional[datetime.datetime] = None,
         last_modified_by: Optional[str] = None,
         last_modified_by_type: Optional[Union[str, "_models.CreatedByType"]] = None,
         last_modified_at: Optional[datetime.datetime] = None,
-        **kwargs: Any
-    ) -> None:
+        **kwargs
+    ):
         """
         :keyword created_by: The identity that created the resource.
         :paramtype created_by: str
         :keyword created_by_type: The type of identity that created the resource. Known values are:
          "User", "Application", "ManagedIdentity", and "Key".
         :paramtype created_by_type: str or ~azure.mgmt.imagebuilder.models.CreatedByType
         :keyword created_at: The timestamp of resource creation (UTC).
@@ -2296,213 +1988,14 @@
         self.created_by_type = created_by_type
         self.created_at = created_at
         self.last_modified_by = last_modified_by
         self.last_modified_by_type = last_modified_by_type
         self.last_modified_at = last_modified_at
 
 
-class TargetRegion(_serialization.Model):
-    """Describes the target region information.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar name: The name of the region. Required.
-    :vartype name: str
-    :ivar replica_count: The number of replicas of the Image Version to be created in this region.
-     Omit to use the default (1).
-    :vartype replica_count: int
-    :ivar storage_account_type: Specifies the storage account type to be used to store the image in
-     this region. Omit to use the default (Standard_LRS). Known values are: "Standard_LRS",
-     "Standard_ZRS", and "Premium_LRS".
-    :vartype storage_account_type: str or
-     ~azure.mgmt.imagebuilder.models.SharedImageStorageAccountType
-    """
-
-    _validation = {
-        "name": {"required": True},
-        "replica_count": {"minimum": 1},
-    }
-
-    _attribute_map = {
-        "name": {"key": "name", "type": "str"},
-        "replica_count": {"key": "replicaCount", "type": "int"},
-        "storage_account_type": {"key": "storageAccountType", "type": "str"},
-    }
-
-    def __init__(
-        self,
-        *,
-        name: str,
-        replica_count: int = 1,
-        storage_account_type: Optional[Union[str, "_models.SharedImageStorageAccountType"]] = None,
-        **kwargs: Any
-    ) -> None:
-        """
-        :keyword name: The name of the region. Required.
-        :paramtype name: str
-        :keyword replica_count: The number of replicas of the Image Version to be created in this
-         region. Omit to use the default (1).
-        :paramtype replica_count: int
-        :keyword storage_account_type: Specifies the storage account type to be used to store the image
-         in this region. Omit to use the default (Standard_LRS). Known values are: "Standard_LRS",
-         "Standard_ZRS", and "Premium_LRS".
-        :paramtype storage_account_type: str or
-         ~azure.mgmt.imagebuilder.models.SharedImageStorageAccountType
-        """
-        super().__init__(**kwargs)
-        self.name = name
-        self.replica_count = replica_count
-        self.storage_account_type = storage_account_type
-
-
-class Trigger(ProxyResource):
-    """Represents a trigger that can invoke an image template build.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
-    :vartype id: str
-    :ivar name: The name of the resource.
-    :vartype name: str
-    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
-     "Microsoft.Storage/storageAccounts".
-    :vartype type: str
-    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
-     information.
-    :vartype system_data: ~azure.mgmt.imagebuilder.models.SystemData
-    :ivar kind: The kind of trigger.
-    :vartype kind: str
-    :ivar status: Trigger status.
-    :vartype status: ~azure.mgmt.imagebuilder.models.TriggerStatus
-    :ivar provisioning_state: Provisioning state of the resource. Known values are: "Creating",
-     "Updating", "Succeeded", "Failed", "Deleting", and "Canceled".
-    :vartype provisioning_state: str or ~azure.mgmt.imagebuilder.models.ProvisioningState
-    """
-
-    _validation = {
-        "id": {"readonly": True},
-        "name": {"readonly": True},
-        "type": {"readonly": True},
-        "system_data": {"readonly": True},
-        "status": {"readonly": True},
-        "provisioning_state": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "id": {"key": "id", "type": "str"},
-        "name": {"key": "name", "type": "str"},
-        "type": {"key": "type", "type": "str"},
-        "system_data": {"key": "systemData", "type": "SystemData"},
-        "kind": {"key": "properties.kind", "type": "str"},
-        "status": {"key": "properties.status", "type": "TriggerStatus"},
-        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
-    }
-
-    def __init__(self, **kwargs: Any) -> None:
-        """ """
-        super().__init__(**kwargs)
-        self.kind: Optional[str] = None
-        self.status = None
-        self.provisioning_state = None
-
-
-class TriggerCollection(_serialization.Model):
-    """The result of List triggers operation.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar value: An array of triggers. Required.
-    :vartype value: list[~azure.mgmt.imagebuilder.models.Trigger]
-    :ivar next_link: The continuation token.
-    :vartype next_link: str
-    """
-
-    _validation = {
-        "value": {"required": True},
-    }
-
-    _attribute_map = {
-        "value": {"key": "value", "type": "[Trigger]"},
-        "next_link": {"key": "nextLink", "type": "str"},
-    }
-
-    def __init__(self, *, value: List["_models.Trigger"], next_link: Optional[str] = None, **kwargs: Any) -> None:
-        """
-        :keyword value: An array of triggers. Required.
-        :paramtype value: list[~azure.mgmt.imagebuilder.models.Trigger]
-        :keyword next_link: The continuation token.
-        :paramtype next_link: str
-        """
-        super().__init__(**kwargs)
-        self.value = value
-        self.next_link = next_link
-
-
-class TriggerStatus(_serialization.Model):
-    """Describes the status of a trigger.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    :ivar code: The status code.
-    :vartype code: str
-    :ivar message: The detailed status message, including for alerts and error messages.
-    :vartype message: str
-    :ivar time: The time of the status.
-    :vartype time: ~datetime.datetime
-    """
-
-    _validation = {
-        "code": {"readonly": True},
-        "message": {"readonly": True},
-        "time": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "code": {"key": "code", "type": "str"},
-        "message": {"key": "message", "type": "str"},
-        "time": {"key": "time", "type": "iso-8601"},
-    }
-
-    def __init__(self, **kwargs: Any) -> None:
-        """ """
-        super().__init__(**kwargs)
-        self.code = None
-        self.message = None
-        self.time = None
-
-
-class UserAssignedIdentity(_serialization.Model):
-    """User assigned identity properties.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    :ivar principal_id: The principal ID of the assigned identity.
-    :vartype principal_id: str
-    :ivar client_id: The client ID of the assigned identity.
-    :vartype client_id: str
-    """
-
-    _validation = {
-        "principal_id": {"readonly": True},
-        "client_id": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "principal_id": {"key": "principalId", "type": "str"},
-        "client_id": {"key": "clientId", "type": "str"},
-    }
-
-    def __init__(self, **kwargs: Any) -> None:
-        """ """
-        super().__init__(**kwargs)
-        self.principal_id = None
-        self.client_id = None
-
-
 class VirtualNetworkConfig(_serialization.Model):
     """Virtual Network configuration.
 
     :ivar subnet_id: Resource id of a pre-existing subnet.
     :vartype subnet_id: str
     :ivar proxy_vm_size: Size of the proxy virtual machine used to pass traffic to the build VM and
      validation VM. Omit or specify empty string to use the default (Standard_A1_v2).
@@ -2510,15 +2003,15 @@
     """
 
     _attribute_map = {
         "subnet_id": {"key": "subnetId", "type": "str"},
         "proxy_vm_size": {"key": "proxyVmSize", "type": "str"},
     }
 
-    def __init__(self, *, subnet_id: Optional[str] = None, proxy_vm_size: str = "", **kwargs: Any) -> None:
+    def __init__(self, *, subnet_id: Optional[str] = None, proxy_vm_size: str = "", **kwargs):
         """
         :keyword subnet_id: Resource id of a pre-existing subnet.
         :paramtype subnet_id: str
         :keyword proxy_vm_size: Size of the proxy virtual machine used to pass traffic to the build VM
          and validation VM. Omit or specify empty string to use the default (Standard_A1_v2).
         :paramtype proxy_vm_size: str
         """
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure/mgmt/imagebuilder/models/_image_builder_client_enums.py` & `azure-mgmt-imagebuilder-1.2.0b1/azure/mgmt/imagebuilder/models/_image_builder_client_enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     """Provisioning state of the resource."""
 
     CREATING = "Creating"
     UPDATING = "Updating"
     SUCCEEDED = "Succeeded"
     FAILED = "Failed"
     DELETING = "Deleting"
-    CANCELED = "Canceled"
 
 
 class ResourceIdentityType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The type of identity used for the image template. The type 'None' will remove any identities
     from the image template.
     """
 
@@ -72,27 +71,18 @@
 
 class RunSubState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Sub-state of the last run."""
 
     QUEUED = "Queued"
     BUILDING = "Building"
     CUSTOMIZING = "Customizing"
-    OPTIMIZING = "Optimizing"
     VALIDATING = "Validating"
     DISTRIBUTING = "Distributing"
 
 
 class SharedImageStorageAccountType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Specifies the storage account type to be used to store the Azure Compute Gallery image version
-    in.
+    """Storage account type to be used to store the shared image. Omit to use the default
+    (Standard_LRS).
     """
 
     STANDARD_LRS = "Standard_LRS"
     STANDARD_ZRS = "Standard_ZRS"
-    PREMIUM_LRS = "Premium_LRS"
-
-
-class VMBootOptimizationState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Enabling this field will improve VM boot time by optimizing the final customized image output."""
-
-    ENABLED = "Enabled"
-    DISABLED = "Disabled"
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/tests/disable_test_cli_mgmt_imagebuilder.py` & `azure-mgmt-imagebuilder-1.2.0b1/tests/disable_test_cli_mgmt_imagebuilder.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/PKG-INFO` & `azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-imagebuilder
-Version: 1.2.0
+Version: 1.2.0b1
 Summary: Microsoft Azure Image Builder Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -27,83 +27,36 @@
 This package has been tested with Python 3.7+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
-## Getting started
+# Usage
 
-### Prerequisites
 
-- Python 3.7+ is required to use this package.
-- [Azure subscription](https://azure.microsoft.com/free/)
+To learn how to use this package, see the [quickstart guide](https://aka.ms/azsdk/python/mgmt)
+ 
+For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/)
+Code samples for this package can be found at [Image Builder](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
+Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
-### Install the package
 
-```bash
-pip install azure-mgmt-imagebuilder
-pip install azure-identity
-```
-
-### Authentication
-
-By default, [Azure Active Directory](https://aka.ms/awps/aad) token authentication depends on correct configure of following environment variables.
-
-- `AZURE_CLIENT_ID` for Azure client ID.
-- `AZURE_TENANT_ID` for Azure tenant ID.
-- `AZURE_CLIENT_SECRET` for Azure client secret.
-
-In addition, Azure subscription ID can be configured via environment variable `AZURE_SUBSCRIPTION_ID`.
-
-With above configuration, client can be authenticated by following code:
-
-```python
-from azure.identity import DefaultAzureCredential
-from azure.mgmt.imagebuilder import ImageBuilderClient
-import os
-
-sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
-client = ImageBuilderClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
-```
-
-## Examples
-
-Code samples for this package can be found at:
-- [Search Image Builder](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
-- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
-
-
-## Troubleshooting
-
-## Next steps
-
-## Provide Feedback
+# Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-imagebuilder%2FREADME.png)
 
 
 # Release History
 
-## 1.2.0 (2023-04-20)
-
-### Features Added
-
-  - Added operation group TriggersOperations
-  - Model ImageTemplate has a new parameter optimize
-  - Model ImageTemplateSharedImageDistributor has a new parameter target_regions
-  - Model ImageTemplateSharedImageDistributor has a new parameter versioning
-  - Model ImageTemplateSharedImageVersionSource has a new parameter exact_version
-  - Model ImageTemplateVhdDistributor has a new parameter uri
-
 ## 1.2.0b1 (2022-11-28)
 
 ### Other Changes
 
   - Added generated samples in github repo
   - Drop support for python<3.7.0
```

## Comparing `azure-mgmt-imagebuilder-1.2.0/azure_mgmt_imagebuilder.egg-info/SOURCES.txt` & `azure-mgmt-imagebuilder-1.2.0b1/azure_mgmt_imagebuilder.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,22 @@
 azure/mgmt/imagebuilder/aio/__init__.py
 azure/mgmt/imagebuilder/aio/_configuration.py
 azure/mgmt/imagebuilder/aio/_image_builder_client.py
 azure/mgmt/imagebuilder/aio/_patch.py
 azure/mgmt/imagebuilder/aio/operations/__init__.py
 azure/mgmt/imagebuilder/aio/operations/_operations.py
 azure/mgmt/imagebuilder/aio/operations/_patch.py
-azure/mgmt/imagebuilder/aio/operations/_triggers_operations.py
 azure/mgmt/imagebuilder/aio/operations/_virtual_machine_image_templates_operations.py
 azure/mgmt/imagebuilder/models/__init__.py
 azure/mgmt/imagebuilder/models/_image_builder_client_enums.py
 azure/mgmt/imagebuilder/models/_models_py3.py
 azure/mgmt/imagebuilder/models/_patch.py
 azure/mgmt/imagebuilder/operations/__init__.py
 azure/mgmt/imagebuilder/operations/_operations.py
 azure/mgmt/imagebuilder/operations/_patch.py
-azure/mgmt/imagebuilder/operations/_triggers_operations.py
 azure/mgmt/imagebuilder/operations/_virtual_machine_image_templates_operations.py
 azure_mgmt_imagebuilder.egg-info/PKG-INFO
 azure_mgmt_imagebuilder.egg-info/SOURCES.txt
 azure_mgmt_imagebuilder.egg-info/dependency_links.txt
 azure_mgmt_imagebuilder.egg-info/not-zip-safe
 azure_mgmt_imagebuilder.egg-info/requires.txt
 azure_mgmt_imagebuilder.egg-info/top_level.txt
```

