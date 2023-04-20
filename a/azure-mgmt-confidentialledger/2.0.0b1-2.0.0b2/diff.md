# Comparing `tmp/azure-mgmt-confidentialledger-2.0.0b1.zip` & `tmp/azure-mgmt-confidentialledger-2.0.0b2.zip`

## zipinfo {}

```diff
@@ -1,51 +1,56 @@
-Zip file size: 62894 bytes, number of entries: 49
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/
--rw-rw-r--  2.0 unx     1393 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/README.md
--rw-rw-r--  2.0 unx      224 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/MANIFEST.in
--rw-rw-r--  2.0 unx       38 b- defN 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/setup.cfg
--rw-rw-r--  2.0 unx     2843 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/setup.py
--rw-rw-r--  2.0 unx      458 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/CHANGELOG.md
--rw-rw-r--  2.0 unx     2763 b- defN 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/PKG-INFO
--rw-rw-r--  2.0 unx     1074 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/LICENSE
--rw-rw-r--  2.0 unx      677 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/_meta.json
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/
--rw-rw-r--  2.0 unx       65 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/models/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/
--rw-rw-r--  2.0 unx       26 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/py.typed
--rw-rw-r--  2.0 unx      488 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_version.py
--rw-rw-r--  2.0 unx      893 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/__init__.py
--rw-rw-r--  2.0 unx     1169 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_vendor.py
--rw-rw-r--  2.0 unx     3832 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_configuration.py
--rw-rw-r--  2.0 unx     1530 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_patch.py
--rw-rw-r--  2.0 unx    77872 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_serialization.py
--rw-rw-r--  2.0 unx     4359 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_confidential_ledger.py
--rw-rw-r--  2.0 unx    24005 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/models/_models_py3.py
--rw-rw-r--  2.0 unx     2073 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/models/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/models/_patch.py
--rw-rw-r--  2.0 unx     1541 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/models/_confidential_ledger_enums.py
--rw-rw-r--  2.0 unx    49953 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/operations/_ledger_operations.py
--rw-rw-r--  2.0 unx      834 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/operations/_patch.py
--rw-rw-r--  2.0 unx     6996 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/operations/_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/operations/
--rw-rw-r--  2.0 unx      840 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/__init__.py
--rw-rw-r--  2.0 unx     3880 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/_configuration.py
--rw-rw-r--  2.0 unx     1530 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/_patch.py
--rw-rw-r--  2.0 unx     4494 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/_confidential_ledger.py
--rw-rw-r--  2.0 unx    41832 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/operations/_ledger_operations.py
--rw-rw-r--  2.0 unx      834 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/operations/_patch.py
--rw-rw-r--  2.0 unx     6238 b- defN 22-Nov-28 01:57 azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/operations/_operations.py
--rw-rw-r--  2.0 unx        1 b- defN 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx      116 b- defN 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/requires.txt
--rw-rw-r--  2.0 unx        6 b- defN 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/top_level.txt
--rw-rw-r--  2.0 unx     2763 b- defN 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx     1650 b- defN 22-Nov-28 01:58 azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/SOURCES.txt
-49 files, 251378 bytes uncompressed, 51678 bytes compressed:  79.4%
+Zip file size: 80589 bytes, number of entries: 54
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/
+-rw-rw-r--  2.0 unx     2851 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/setup.py
+-rw-rw-r--  2.0 unx      644 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/_meta.json
+-rw-rw-r--  2.0 unx      776 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/CHANGELOG.md
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/LICENSE
+-rw-rw-r--  2.0 unx       38 b- defN 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/setup.cfg
+-rw-rw-r--  2.0 unx     3879 b- defN 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/PKG-INFO
+-rw-rw-r--  2.0 unx     2191 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/README.md
+-rw-rw-r--  2.0 unx      224 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/MANIFEST.in
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_patch.py
+-rw-rw-r--  2.0 unx      893 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/__init__.py
+-rw-rw-r--  2.0 unx    78836 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_serialization.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_version.py
+-rw-rw-r--  2.0 unx     1819 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_vendor.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/py.typed
+-rw-rw-r--  2.0 unx     4656 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_confidential_ledger.py
+-rw-rw-r--  2.0 unx     3501 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_configuration.py
+-rw-rw-r--  2.0 unx     2163 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/models/_confidential_ledger_enums.py
+-rw-rw-r--  2.0 unx    37976 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/models/_models_py3.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/models/_patch.py
+-rw-rw-r--  2.0 unx     2882 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/models/__init__.py
+-rw-rw-r--  2.0 unx    48056 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/_managed_ccf_operations.py
+-rw-rw-r--  2.0 unx     8268 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/_confidential_ledger_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/_patch.py
+-rw-rw-r--  2.0 unx     1040 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/__init__.py
+-rw-rw-r--  2.0 unx     6736 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/_operations.py
+-rw-rw-r--  2.0 unx    49903 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/_ledger_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/_patch.py
+-rw-rw-r--  2.0 unx      840 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/__init__.py
+-rw-rw-r--  2.0 unx     1054 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/_vendor.py
+-rw-rw-r--  2.0 unx     4800 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/_confidential_ledger.py
+-rw-rw-r--  2.0 unx     3549 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/_configuration.py
+-rw-rw-r--  2.0 unx    40147 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/_managed_ccf_operations.py
+-rw-rw-r--  2.0 unx     6991 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/_confidential_ledger_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx     1040 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx     6039 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    41976 b- defN 23-Apr-20 03:45 azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/_ledger_operations.py
+-rw-rw-r--  2.0 unx        6 b- defN 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx     3879 b- defN 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx     1991 b- defN 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx      124 b- defN 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Apr-20 03:46 azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/not-zip-safe
+54 files, 376570 bytes uncompressed, 67941 bytes compressed:  82.0%
```

## zipnote {}

```diff
@@ -1,148 +1,163 @@
-Filename: azure-mgmt-confidentialledger-2.0.0b1/
+Filename: azure-mgmt-confidentialledger-2.0.0b2/
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/README.md
+Filename: azure-mgmt-confidentialledger-2.0.0b2/setup.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/MANIFEST.in
+Filename: azure-mgmt-confidentialledger-2.0.0b2/_meta.json
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/setup.cfg
+Filename: azure-mgmt-confidentialledger-2.0.0b2/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/setup.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/LICENSE
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/CHANGELOG.md
+Filename: azure-mgmt-confidentialledger-2.0.0b2/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/PKG-INFO
+Filename: azure-mgmt-confidentialledger-2.0.0b2/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/LICENSE
+Filename: azure-mgmt-confidentialledger-2.0.0b2/README.md
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/_meta.json
+Filename: azure-mgmt-confidentialledger-2.0.0b2/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/__init__.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/__init__.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/models/
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/models/
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/operations/
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/py.typed
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_patch.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_version.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/__init__.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/__init__.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_vendor.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_version.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_configuration.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_patch.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/py.typed
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_serialization.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_confidential_ledger.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_confidential_ledger.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/models/_models_py3.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/models/_confidential_ledger_enums.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/models/__init__.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/models/_patch.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/models/_confidential_ledger_enums.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/operations/_ledger_operations.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/_managed_ccf_operations.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/operations/__init__.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/_confidential_ledger_operations.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/operations/_patch.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/operations/_operations.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/operations/
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/__init__.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/_ledger_operations.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/_configuration.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/_patch.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/_confidential_ledger.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/operations/_ledger_operations.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/operations/__init__.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/_confidential_ledger.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/operations/_patch.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/operations/_operations.py
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/_managed_ccf_operations.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/dependency_links.txt
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/_confidential_ledger_operations.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/not-zip-safe
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/requires.txt
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/top_level.txt
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/PKG-INFO
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/_ledger_operations.py
 Comment: 
 
-Filename: azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/SOURCES.txt
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/top_level.txt
+Comment: 
+
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/PKG-INFO
+Comment: 
+
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/SOURCES.txt
+Comment: 
+
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/dependency_links.txt
+Comment: 
+
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/requires.txt
+Comment: 
+
+Filename: azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/not-zip-safe
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/setup.py` & `azure-mgmt-confidentialledger-2.0.0b2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -66,14 +66,14 @@
         'azure.mgmt',
     ]),
     include_package_data=True,
     package_data={
         'pytyped': ['py.typed'],
     },
     install_requires=[
-        "msrest>=0.7.1",
+        "isodate<1.0.0,>=0.6.1",
         "azure-common~=1.1",
         "azure-mgmt-core>=1.3.2,<2.0.0",
         "typing-extensions>=4.3.0; python_version<'3.8.0'",
     ],
     python_requires=">=3.7"
 )
```

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/PKG-INFO` & `azure-mgmt-confidentialledger-2.0.0b2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-confidentialledger
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Microsoft Azure Confidential Ledger Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -27,36 +27,84 @@
 This package has been tested with Python 3.7+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
-# Usage
+## Getting started
 
+### Prerequisites
 
-To learn how to use this package, see the [quickstart guide](https://aka.ms/azsdk/python/mgmt)
- 
-For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/)
-Code samples for this package can be found at [Confidential Ledger Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
-Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+- Python 3.7+ is required to use this package.
+- [Azure subscription](https://azure.microsoft.com/free/)
 
+### Install the package
 
-# Provide Feedback
+```bash
+pip install azure-mgmt-confidentialledger
+pip install azure-identity
+```
+
+### Authentication
+
+By default, [Azure Active Directory](https://aka.ms/awps/aad) token authentication depends on correct configure of following environment variables.
+
+- `AZURE_CLIENT_ID` for Azure client ID.
+- `AZURE_TENANT_ID` for Azure tenant ID.
+- `AZURE_CLIENT_SECRET` for Azure client secret.
+
+In addition, Azure subscription ID can be configured via environment variable `AZURE_SUBSCRIPTION_ID`.
+
+With above configuration, client can be authenticated by following code:
+
+```python
+from azure.identity import DefaultAzureCredential
+from azure.mgmt.confidentialledger import ConfidentialLedger
+import os
+
+sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
+client = ConfidentialLedger(credential=DefaultAzureCredential(), subscription_id=sub_id)
+```
+
+## Examples
+
+Code samples for this package can be found at:
+- [Search Confidential Ledger Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+
+
+## Troubleshooting
+
+## Next steps
+
+## Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-confidentialledger%2FREADME.png)
 
 
 # Release History
 
+## 2.0.0b2 (2023-04-20)
+
+### Features Added
+
+  - Added operation group ManagedCCFOperations
+  - Model LedgerProperties has a new parameter running_state
+
+### Breaking Changes
+
+  - Model LedgerProperties no longer has parameter ledger_storage_account
+  - Parameter location of model ConfidentialLedger is now required
+
 ## 2.0.0b1 (2022-11-25)
 
 ### Features Added
 
   - Model LedgerProperties has a new parameter ledger_storage_account
 
 ### Breaking Changes
```

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/LICENSE` & `azure-mgmt-confidentialledger-2.0.0b2/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/__init__.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_patch.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_serialization.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,30 +34,47 @@
 import email
 from enum import Enum
 import json
 import logging
 import re
 import sys
 import codecs
-from typing import Optional, Union, AnyStr, IO, Mapping
+from typing import (
+    Dict,
+    Any,
+    cast,
+    Optional,
+    Union,
+    AnyStr,
+    IO,
+    Mapping,
+    Callable,
+    TypeVar,
+    MutableMapping,
+    Type,
+    List,
+    Mapping,
+)
 
 try:
     from urllib import quote  # type: ignore
 except ImportError:
     from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
 import isodate  # type: ignore
 
-from typing import Dict, Any, cast
-
 from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
+from azure.core.serialization import NULL as AzureCoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
+ModelType = TypeVar("ModelType", bound="Model")
+JSON = MutableMapping[str, Any]
+
 
 class RawDeserializer:
 
     # Accept "text" because we're open minded people...
     JSON_REGEXP = re.compile(r"^(application|text)/([a-z+.]+\+)?json$")
 
     # Name used in context
@@ -273,43 +290,43 @@
     serialization and deserialization.
     """
 
     _subtype_map: Dict[str, Dict[str, Any]] = {}
     _attribute_map: Dict[str, Dict[str, Any]] = {}
     _validation: Dict[str, Dict[str, Any]] = {}
 
-    def __init__(self, **kwargs):
-        self.additional_properties = {}
+    def __init__(self, **kwargs: Any) -> None:
+        self.additional_properties: Dict[str, Any] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         if isinstance(other, self.__class__):
             return self.__dict__ == other.__dict__
         return False
 
-    def __ne__(self, other):
+    def __ne__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         return not self.__eq__(other)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.__dict__)
 
     @classmethod
-    def enable_additional_properties_sending(cls):
+    def enable_additional_properties_sending(cls) -> None:
         cls._attribute_map["additional_properties"] = {"key": "", "type": "{object}"}
 
     @classmethod
-    def is_xml_model(cls):
+    def is_xml_model(cls) -> bool:
         try:
             cls._xml_map  # type: ignore
         except AttributeError:
             return False
         return True
 
     @classmethod
@@ -318,30 +335,35 @@
         try:
             xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
-    def serialize(self, keep_readonly=False, **kwargs):
+    def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
         """Return the JSON that would be sent to azure from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
         return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
 
-    def as_dict(self, keep_readonly=True, key_transformer=attribute_transformer, **kwargs):
-        """Return a dict that can be JSONify using json.dump.
+    def as_dict(
+        self,
+        keep_readonly: bool = True,
+        key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
+        **kwargs: Any
+    ) -> JSON:
+        """Return a dict that can be serialized using json.dump.
 
         Advanced usage might optionally use a callback as parameter:
 
         .. code::python
 
             def my_key_transformer(key, attr_desc, value):
                 return key
@@ -380,41 +402,46 @@
                 raise ValueError("Not Autorest generated code")
         except Exception:
             # Assume it's not Autorest generated (tests?). Add ourselves as dependencies.
             client_models = {cls.__name__: cls}
         return client_models
 
     @classmethod
-    def deserialize(cls, data, content_type=None):
+    def deserialize(cls: Type[ModelType], data: Any, content_type: Optional[str] = None) -> ModelType:
         """Parse a str using the RestAPI syntax and return a model.
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
         return deserializer(cls.__name__, data, content_type=content_type)
 
     @classmethod
-    def from_dict(cls, data, key_extractors=None, content_type=None):
+    def from_dict(
+        cls: Type[ModelType],
+        data: Any,
+        key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
+        content_type: Optional[str] = None,
+    ) -> ModelType:
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
-        deserializer.key_extractors = (
-            [
+        deserializer.key_extractors = (  # type: ignore
+            [  # type: ignore
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
@@ -514,15 +541,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -530,15 +557,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -598,15 +625,15 @@
                         xml_desc = attr_desc.get("xml", {})
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
-                                xml_name = "{}{}".format(xml_ns, xml_name)
+                                xml_name = "{{{}}}{}".format(xml_ns, xml_name)
                             serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
                             serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
                             serialized.extend(new_attr)  # type: ignore
@@ -622,16 +649,15 @@
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
                             local_node.text = unicode_str(new_attr)
                             serialized.append(local_node)  # type: ignore
                     else:  # JSON
                         for k in reversed(keys):  # type: ignore
-                            unflattened = {k: new_attr}
-                            new_attr = unflattened
+                            new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
                         for k in keys:  # type: ignore
                             if k not in _serialized:
                                 _serialized.update(_new_attr)  # type: ignore
                             _new_attr = _new_attr[k]  # type: ignore
@@ -652,16 +678,16 @@
         :param str data_type: The type to be serialized from.
         :rtype: dict
         :raises: SerializationError if serialization fails.
         :raises: ValueError if data is None
         """
 
         # Just in case this is a dict
-        internal_data_type = data_type.strip("[]{}")
-        internal_data_type = self.dependencies.get(internal_data_type, None)
+        internal_data_type_str = data_type.strip("[]{}")
+        internal_data_type = self.dependencies.get(internal_data_type_str, None)
         try:
             is_xml_model_serialization = kwargs["is_xml"]
         except KeyError:
             if internal_data_type and issubclass(internal_data_type, Model):
                 is_xml_model_serialization = kwargs.setdefault("is_xml", internal_data_type.is_xml_model())
             else:
                 is_xml_model_serialization = False
@@ -773,14 +799,16 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
+            if data is AzureCoreNull:
+                return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
             # If dependencies is empty, try with current data class
@@ -1157,15 +1185,16 @@
 
 
 def rest_key_extractor(attr, attr_desc, data):
     key = attr_desc["key"]
     working_data = data
 
     while "." in key:
-        dict_keys = _FLATTEN.split(key)
+        # Need the cast, as for some reasons "split" is typed as list[str | Any]
+        dict_keys = cast(List[str], _FLATTEN.split(key))
         if len(dict_keys) == 1:
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
@@ -1238,15 +1267,15 @@
     :rtype: tuple
     :returns: A tuple XML name + namespace dict
     """
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
     xml_name = internal_type_xml_map.get("name", internal_type.__name__)
     xml_ns = internal_type_xml_map.get("ns", None)
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
     return xml_name
 
 
 def xml_key_extractor(attr, attr_desc, data):
     if isinstance(data, dict):
         return None
 
@@ -1262,15 +1291,15 @@
     is_wrapped = xml_desc.get("wrapped", False)
     internal_type = attr_desc.get("internalType", None)
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
 
     # Integrate namespace if necessary
     xml_ns = xml_desc.get("ns", internal_type_xml_map.get("ns", None))
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
 
     # If it's an attribute, that's simple
     if xml_desc.get("attr", False):
         return data.get(xml_name)
 
     # If it's x-ms-text, that's simple too
     if xml_desc.get("text", False):
@@ -1328,15 +1357,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1348,15 +1377,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1467,40 +1496,40 @@
 
     def _classify_target(self, target, data):
         """Check to see whether the deserialization target object can
         be classified into a subclass.
         Once classification has been determined, initialize object.
 
         :param str target: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
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
-        return target, target.__class__.__name__
+        return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
         for use in error deserialization, as we want to return the
         HttpResponseError to users, and not have them deal with
         a deserialization error.
 
         :param str target_obj: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         :param str content_type: Swagger "produces" if available.
         """
         try:
             return self(target_obj, data, content_type=content_type)
         except:
             _LOGGER.debug(
                 "Ran into a deserialization error. Ignoring since this is failsafe deserialization", exc_info=True
```

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/_confidential_ledger.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/_confidential_ledger.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,91 +3,93 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
-from typing import Any, TYPE_CHECKING
+from typing import Any, Awaitable, TYPE_CHECKING
 
-from azure.core.rest import HttpRequest, HttpResponse
-from azure.mgmt.core import ARMPipelineClient
+from azure.core.rest import AsyncHttpResponse, HttpRequest
+from azure.mgmt.core import AsyncARMPipelineClient
 
-from . import models as _models
+from .. import models as _models
+from .._serialization import Deserializer, Serializer
 from ._configuration import ConfidentialLedgerConfiguration
-from ._serialization import Deserializer, Serializer
-from .operations import LedgerOperations, Operations
+from .operations import ConfidentialLedgerOperationsMixin, LedgerOperations, ManagedCCFOperations, Operations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials import TokenCredential
+    from azure.core.credentials_async import AsyncTokenCredential
 
 
-class ConfidentialLedger:  # pylint: disable=client-accepts-api-version-keyword
+class ConfidentialLedger(ConfidentialLedgerOperationsMixin):  # pylint: disable=client-accepts-api-version-keyword
     """Microsoft Azure Confidential Compute Ledger Control Plane REST API version 2020-12-01-preview.
 
     :ivar operations: Operations operations
-    :vartype operations: azure.mgmt.confidentialledger.operations.Operations
+    :vartype operations: azure.mgmt.confidentialledger.aio.operations.Operations
     :ivar ledger: LedgerOperations operations
-    :vartype ledger: azure.mgmt.confidentialledger.operations.LedgerOperations
+    :vartype ledger: azure.mgmt.confidentialledger.aio.operations.LedgerOperations
+    :ivar managed_ccf: ManagedCCFOperations operations
+    :vartype managed_ccf: azure.mgmt.confidentialledger.aio.operations.ManagedCCFOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: The Azure subscription ID. This is a GUID-formatted string (e.g.
-     00000000-0000-0000-0000-000000000000). Required.
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2020-12-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-01-26-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
-        credential: "TokenCredential",
+        credential: "AsyncTokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = ConfidentialLedgerConfiguration(credential=credential, subscription_id=subscription_id, **kwargs)
-        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.ledger = LedgerOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.managed_ccf = ManagedCCFOperations(self._client, self._config, self._serialize, self._deserialize)
 
-    def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
+    def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
-        >>> response = client._send_request(request)
-        <HttpResponse: 200 OK>
+        >>> response = await client._send_request(request)
+        <AsyncHttpResponse: 200 OK>
 
         For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
 
         :param request: The network request you want to make. Required.
         :type request: ~azure.core.rest.HttpRequest
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.rest.HttpResponse
+        :rtype: ~azure.core.rest.AsyncHttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, **kwargs)
 
-    def close(self) -> None:
-        self._client.close()
+    async def close(self) -> None:
+        await self._client.close()
 
-    def __enter__(self) -> "ConfidentialLedger":
-        self._client.__enter__()
+    async def __aenter__(self) -> "ConfidentialLedger":
+        await self._client.__aenter__()
         return self
 
-    def __exit__(self, *exc_details) -> None:
-        self._client.__exit__(*exc_details)
+    async def __aexit__(self, *exc_details: Any) -> None:
+        await self._client.__aexit__(*exc_details)
```

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/models/__init__.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/models/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,52 +4,72 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._models_py3 import AADBasedSecurityPrincipal
 from ._models_py3 import CertBasedSecurityPrincipal
+from ._models_py3 import CertificateTags
+from ._models_py3 import CheckNameAvailabilityRequest
+from ._models_py3 import CheckNameAvailabilityResponse
 from ._models_py3 import ConfidentialLedger
 from ._models_py3 import ConfidentialLedgerList
+from ._models_py3 import DeploymentType
 from ._models_py3 import ErrorAdditionalInfo
 from ._models_py3 import ErrorDetail
 from ._models_py3 import ErrorResponse
 from ._models_py3 import LedgerProperties
-from ._models_py3 import Location
+from ._models_py3 import ManagedCCF
+from ._models_py3 import ManagedCCFList
+from ._models_py3 import ManagedCCFProperties
+from ._models_py3 import MemberIdentityCertificate
 from ._models_py3 import Resource
 from ._models_py3 import ResourceProviderOperationDefinition
 from ._models_py3 import ResourceProviderOperationDisplay
 from ._models_py3 import ResourceProviderOperationList
 from ._models_py3 import SystemData
-from ._models_py3 import Tags
+from ._models_py3 import TrackedResource
 
+from ._confidential_ledger_enums import CheckNameAvailabilityReason
 from ._confidential_ledger_enums import CreatedByType
+from ._confidential_ledger_enums import LanguageRuntime
 from ._confidential_ledger_enums import LedgerRoleName
 from ._confidential_ledger_enums import LedgerType
 from ._confidential_ledger_enums import ProvisioningState
+from ._confidential_ledger_enums import RunningState
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AADBasedSecurityPrincipal",
     "CertBasedSecurityPrincipal",
+    "CertificateTags",
+    "CheckNameAvailabilityRequest",
+    "CheckNameAvailabilityResponse",
     "ConfidentialLedger",
     "ConfidentialLedgerList",
+    "DeploymentType",
     "ErrorAdditionalInfo",
     "ErrorDetail",
     "ErrorResponse",
     "LedgerProperties",
-    "Location",
+    "ManagedCCF",
+    "ManagedCCFList",
+    "ManagedCCFProperties",
+    "MemberIdentityCertificate",
     "Resource",
     "ResourceProviderOperationDefinition",
     "ResourceProviderOperationDisplay",
     "ResourceProviderOperationList",
     "SystemData",
-    "Tags",
+    "TrackedResource",
+    "CheckNameAvailabilityReason",
     "CreatedByType",
+    "LanguageRuntime",
     "LedgerRoleName",
     "LedgerType",
     "ProvisioningState",
+    "RunningState",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/models/_patch.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/models/_confidential_ledger_enums.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/models/_confidential_ledger_enums.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,37 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
 
 
+class CheckNameAvailabilityReason(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The reason why the given name is not available."""
+
+    INVALID = "Invalid"
+    ALREADY_EXISTS = "AlreadyExists"
+
+
 class CreatedByType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The type of identity that created the resource."""
 
     USER = "User"
     APPLICATION = "Application"
     MANAGED_IDENTITY = "ManagedIdentity"
     KEY = "Key"
 
 
+class LanguageRuntime(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Object representing LanguageRuntime for Manged CCF."""
+
+    CPP = "CPP"
+    JS = "JS"
+
+
 class LedgerRoleName(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """LedgerRole associated with the Security Principal of Ledger."""
 
     READER = "Reader"
     CONTRIBUTOR = "Contributor"
     ADMINISTRATOR = "Administrator"
 
@@ -41,7 +55,17 @@
     UNKNOWN = "Unknown"
     SUCCEEDED = "Succeeded"
     FAILED = "Failed"
     CANCELED = "Canceled"
     CREATING = "Creating"
     DELETING = "Deleting"
     UPDATING = "Updating"
+
+
+class RunningState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Object representing RunningState for Confidential Ledger."""
+
+    ACTIVE = "Active"
+    PAUSED = "Paused"
+    UNKNOWN = "Unknown"
+    PAUSING = "Pausing"
+    RESUMING = "Resuming"
```

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/operations/_ledger_operations.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/_ledger_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,45 +25,39 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import _convert_request, _format_url_section
+from .._vendor import ConfidentialLedgerMixinABC, _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(resource_group_name: str, ledger_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2020-12-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-26-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ConfidentialLedger/ledgers/{ledgerName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=3
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "ledgerName": _SERIALIZER.url("ledger_name", ledger_name, "str", pattern=r"^[a-zA-Z0-9]"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -78,28 +71,26 @@
 
 def build_delete_request(
     resource_group_name: str, ledger_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2020-12-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-26-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ConfidentialLedger/ledgers/{ledgerName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=3
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "ledgerName": _SERIALIZER.url("ledger_name", ledger_name, "str", pattern=r"^[a-zA-Z0-9]"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -113,29 +104,27 @@
 
 def build_create_request(
     resource_group_name: str, ledger_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2020-12-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-26-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ConfidentialLedger/ledgers/{ledgerName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=3
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "ledgerName": _SERIALIZER.url("ledger_name", ledger_name, "str", pattern=r"^[a-zA-Z0-9]"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -151,29 +140,27 @@
 
 def build_update_request(
     resource_group_name: str, ledger_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2020-12-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-26-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ConfidentialLedger/ledgers/{ledgerName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=3
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "ledgerName": _SERIALIZER.url("ledger_name", ledger_name, "str", pattern=r"^[a-zA-Z0-9]"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -189,28 +176,26 @@
 
 def build_list_by_resource_group_request(
     resource_group_name: str, subscription_id: str, *, filter: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2020-12-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-26-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ConfidentialLedger/ledgers",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=3
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -225,23 +210,21 @@
 
 def build_list_by_subscription_request(
     subscription_id: str, *, filter: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2020-12-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-26-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.ConfidentialLedger/ledgers/")
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
     if filter is not None:
@@ -274,15 +257,16 @@
 
     @distributed_trace
     def get(self, resource_group_name: str, ledger_name: str, **kwargs: Any) -> _models.ConfidentialLedger:
         """Retrieves information about a Confidential Ledger resource.
 
         Retrieves the properties of a Confidential Ledger.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfidentialLedger or the result of cls(response)
         :rtype: ~azure.mgmt.confidentialledger.models.ConfidentialLedger
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -294,33 +278,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConfidentialLedger] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             ledger_name=ledger_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -347,33 +330,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             ledger_name=ledger_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -388,15 +370,16 @@
 
     @distributed_trace
     def begin_delete(self, resource_group_name: str, ledger_name: str, **kwargs: Any) -> LROPoller[None]:
         """Deletes a Confidential Ledger resource.
 
         Deletes an existing Confidential Ledger.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
@@ -407,17 +390,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -455,31 +436,29 @@
 
     def _create_initial(
         self,
         resource_group_name: str,
         ledger_name: str,
         confidential_ledger: Union[_models.ConfidentialLedger, IO],
         **kwargs: Any
-    ) -> Optional[_models.ConfidentialLedger]:
+    ) -> _models.ConfidentialLedger:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[Optional[_models.ConfidentialLedger]] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ConfidentialLedger] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(confidential_ledger, (IO, bytes)):
             _content = confidential_ledger
         else:
@@ -496,33 +475,36 @@
             template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("ConfidentialLedger", pipeline_response)
 
+        if response.status_code == 201:
+            deserialized = self._deserialize("ConfidentialLedger", pipeline_response)
+
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
     _create_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ConfidentialLedger/ledgers/{ledgerName}"
     }
 
     @overload
     def begin_create(
@@ -534,15 +516,16 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.ConfidentialLedger]:
         """Creates a  Confidential Ledger.
 
         Creates a  Confidential Ledger with the specified ledger parameters.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
         :param confidential_ledger: Confidential Ledger Create Request Body. Required.
         :type confidential_ledger: ~azure.mgmt.confidentialledger.models.ConfidentialLedger
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -571,15 +554,16 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.ConfidentialLedger]:
         """Creates a  Confidential Ledger.
 
         Creates a  Confidential Ledger with the specified ledger parameters.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
         :param confidential_ledger: Confidential Ledger Create Request Body. Required.
         :type confidential_ledger: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -606,20 +590,21 @@
         confidential_ledger: Union[_models.ConfidentialLedger, IO],
         **kwargs: Any
     ) -> LROPoller[_models.ConfidentialLedger]:
         """Creates a  Confidential Ledger.
 
         Creates a  Confidential Ledger with the specified ledger parameters.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
-        :param confidential_ledger: Confidential Ledger Create Request Body. Is either a model type or
-         a IO type. Required.
+        :param confidential_ledger: Confidential Ledger Create Request Body. Is either a
+         ConfidentialLedger type or a IO type. Required.
         :type confidential_ledger: ~azure.mgmt.confidentialledger.models.ConfidentialLedger or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -632,17 +617,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.confidentialledger.models.ConfidentialLedger]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ConfidentialLedger] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_initial(
@@ -661,15 +644,17 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ConfidentialLedger", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
@@ -697,17 +682,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.ConfidentialLedger]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(confidential_ledger, (IO, bytes)):
@@ -726,16 +709,17 @@
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -764,15 +748,16 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.ConfidentialLedger]:
         """Update Confidential Ledger properties.
 
         Updates properties of Confidential Ledger.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
         :param confidential_ledger: Confidential Ledger request body for Updating Ledger. Required.
         :type confidential_ledger: ~azure.mgmt.confidentialledger.models.ConfidentialLedger
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -801,15 +786,16 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.ConfidentialLedger]:
         """Update Confidential Ledger properties.
 
         Updates properties of Confidential Ledger.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
         :param confidential_ledger: Confidential Ledger request body for Updating Ledger. Required.
         :type confidential_ledger: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -836,20 +822,21 @@
         confidential_ledger: Union[_models.ConfidentialLedger, IO],
         **kwargs: Any
     ) -> LROPoller[_models.ConfidentialLedger]:
         """Update Confidential Ledger properties.
 
         Updates properties of Confidential Ledger.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
         :param confidential_ledger: Confidential Ledger request body for Updating Ledger. Is either a
-         model type or a IO type. Required.
+         ConfidentialLedger type or a IO type. Required.
         :type confidential_ledger: ~azure.mgmt.confidentialledger.models.ConfidentialLedger or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -862,17 +849,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.confidentialledger.models.ConfidentialLedger]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ConfidentialLedger] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._update_initial(
@@ -918,30 +903,29 @@
         self, resource_group_name: str, filter: Optional[str] = None, **kwargs: Any
     ) -> Iterable["_models.ConfidentialLedger"]:
         """Retrieves information about all Confidential Ledger resources under the given subscription and
         resource group.
 
         Retrieves the properties of all Confidential Ledgers.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param filter: The filter to apply on the list operation. eg. $filter=ledgerType eq 'Public'.
          Default value is None.
         :type filter: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ConfidentialLedger or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.confidentialledger.models.ConfidentialLedger]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConfidentialLedgerList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -987,16 +971,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -1024,17 +1009,15 @@
         :return: An iterator like instance of either ConfidentialLedger or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.confidentialledger.models.ConfidentialLedger]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConfidentialLedgerList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1079,16 +1062,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/operations/__init__.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._operations import Operations
-from ._ledger_operations import LedgerOperations
+from ._confidential_ledger import ConfidentialLedger
 
-from ._patch import __all__ as _patch_all
-from ._patch import *  # pylint: disable=unused-wildcard-import
+try:
+    from ._patch import __all__ as _patch_all
+    from ._patch import *  # pylint: disable=unused-wildcard-import
+except ImportError:
+    _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "Operations",
-    "LedgerOperations",
+    "ConfidentialLedger",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
+
 _patch_sdk()
```

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/operations/_patch.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/operations/_operations.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/operations/_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -24,34 +23,28 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import _convert_request
+from .._vendor import ConfidentialLedgerMixinABC, _convert_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2020-12-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-26-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.ConfidentialLedger/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -93,17 +86,15 @@
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.confidentialledger.models.ResourceProviderOperationDefinition]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceProviderOperationList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -146,16 +137,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/_patch.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/_confidential_ledger.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/_confidential_ledger.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,91 +3,93 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
-from typing import Any, Awaitable, TYPE_CHECKING
+from typing import Any, TYPE_CHECKING
 
-from azure.core.rest import AsyncHttpResponse, HttpRequest
-from azure.mgmt.core import AsyncARMPipelineClient
+from azure.core.rest import HttpRequest, HttpResponse
+from azure.mgmt.core import ARMPipelineClient
 
-from .. import models as _models
-from .._serialization import Deserializer, Serializer
+from . import models as _models
 from ._configuration import ConfidentialLedgerConfiguration
-from .operations import LedgerOperations, Operations
+from ._serialization import Deserializer, Serializer
+from .operations import ConfidentialLedgerOperationsMixin, LedgerOperations, ManagedCCFOperations, Operations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials_async import AsyncTokenCredential
+    from azure.core.credentials import TokenCredential
 
 
-class ConfidentialLedger:  # pylint: disable=client-accepts-api-version-keyword
+class ConfidentialLedger(ConfidentialLedgerOperationsMixin):  # pylint: disable=client-accepts-api-version-keyword
     """Microsoft Azure Confidential Compute Ledger Control Plane REST API version 2020-12-01-preview.
 
     :ivar operations: Operations operations
-    :vartype operations: azure.mgmt.confidentialledger.aio.operations.Operations
+    :vartype operations: azure.mgmt.confidentialledger.operations.Operations
     :ivar ledger: LedgerOperations operations
-    :vartype ledger: azure.mgmt.confidentialledger.aio.operations.LedgerOperations
+    :vartype ledger: azure.mgmt.confidentialledger.operations.LedgerOperations
+    :ivar managed_ccf: ManagedCCFOperations operations
+    :vartype managed_ccf: azure.mgmt.confidentialledger.operations.ManagedCCFOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: The Azure subscription ID. This is a GUID-formatted string (e.g.
-     00000000-0000-0000-0000-000000000000). Required.
+    :type credential: ~azure.core.credentials.TokenCredential
+    :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2020-12-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-01-26-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
-        credential: "AsyncTokenCredential",
+        credential: "TokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = ConfidentialLedgerConfiguration(credential=credential, subscription_id=subscription_id, **kwargs)
-        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.ledger = LedgerOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.managed_ccf = ManagedCCFOperations(self._client, self._config, self._serialize, self._deserialize)
 
-    def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
+    def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
-        >>> response = await client._send_request(request)
-        <AsyncHttpResponse: 200 OK>
+        >>> response = client._send_request(request)
+        <HttpResponse: 200 OK>
 
         For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
 
         :param request: The network request you want to make. Required.
         :type request: ~azure.core.rest.HttpRequest
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.rest.AsyncHttpResponse
+        :rtype: ~azure.core.rest.HttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, **kwargs)
 
-    async def close(self) -> None:
-        await self._client.close()
+    def close(self) -> None:
+        self._client.close()
 
-    async def __aenter__(self) -> "ConfidentialLedger":
-        await self._client.__aenter__()
+    def __enter__(self) -> "ConfidentialLedger":
+        self._client.__enter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
-        await self._client.__aexit__(*exc_details)
+    def __exit__(self, *exc_details: Any) -> None:
+        self._client.__exit__(*exc_details)
```

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/operations/_ledger_operations.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/_ledger_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -35,19 +34,16 @@
     build_create_request,
     build_delete_request,
     build_get_request,
     build_list_by_resource_group_request,
     build_list_by_subscription_request,
     build_update_request,
 )
+from .._vendor import ConfidentialLedgerMixinABC
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class LedgerOperations:
     """
     .. warning::
@@ -69,15 +65,16 @@
 
     @distributed_trace_async
     async def get(self, resource_group_name: str, ledger_name: str, **kwargs: Any) -> _models.ConfidentialLedger:
         """Retrieves information about a Confidential Ledger resource.
 
         Retrieves the properties of a Confidential Ledger.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfidentialLedger or the result of cls(response)
         :rtype: ~azure.mgmt.confidentialledger.models.ConfidentialLedger
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -89,33 +86,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConfidentialLedger] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             ledger_name=ledger_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -142,33 +138,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             ledger_name=ledger_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -183,15 +178,16 @@
 
     @distributed_trace_async
     async def begin_delete(self, resource_group_name: str, ledger_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
         """Deletes a Confidential Ledger resource.
 
         Deletes an existing Confidential Ledger.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
@@ -202,17 +198,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -250,31 +244,29 @@
 
     async def _create_initial(
         self,
         resource_group_name: str,
         ledger_name: str,
         confidential_ledger: Union[_models.ConfidentialLedger, IO],
         **kwargs: Any
-    ) -> Optional[_models.ConfidentialLedger]:
+    ) -> _models.ConfidentialLedger:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[Optional[_models.ConfidentialLedger]] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ConfidentialLedger] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(confidential_ledger, (IO, bytes)):
             _content = confidential_ledger
         else:
@@ -291,33 +283,36 @@
             template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("ConfidentialLedger", pipeline_response)
 
+        if response.status_code == 201:
+            deserialized = self._deserialize("ConfidentialLedger", pipeline_response)
+
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
     _create_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ConfidentialLedger/ledgers/{ledgerName}"
     }
 
     @overload
     async def begin_create(
@@ -329,15 +324,16 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.ConfidentialLedger]:
         """Creates a  Confidential Ledger.
 
         Creates a  Confidential Ledger with the specified ledger parameters.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
         :param confidential_ledger: Confidential Ledger Create Request Body. Required.
         :type confidential_ledger: ~azure.mgmt.confidentialledger.models.ConfidentialLedger
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -367,15 +363,16 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.ConfidentialLedger]:
         """Creates a  Confidential Ledger.
 
         Creates a  Confidential Ledger with the specified ledger parameters.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
         :param confidential_ledger: Confidential Ledger Create Request Body. Required.
         :type confidential_ledger: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -403,20 +400,21 @@
         confidential_ledger: Union[_models.ConfidentialLedger, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.ConfidentialLedger]:
         """Creates a  Confidential Ledger.
 
         Creates a  Confidential Ledger with the specified ledger parameters.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
-        :param confidential_ledger: Confidential Ledger Create Request Body. Is either a model type or
-         a IO type. Required.
+        :param confidential_ledger: Confidential Ledger Create Request Body. Is either a
+         ConfidentialLedger type or a IO type. Required.
         :type confidential_ledger: ~azure.mgmt.confidentialledger.models.ConfidentialLedger or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -430,17 +428,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.confidentialledger.models.ConfidentialLedger]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ConfidentialLedger] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_initial(
@@ -459,15 +455,18 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ConfidentialLedger", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
@@ -495,17 +494,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.ConfidentialLedger]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(confidential_ledger, (IO, bytes)):
@@ -524,16 +521,17 @@
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -562,15 +560,16 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.ConfidentialLedger]:
         """Update Confidential Ledger properties.
 
         Updates properties of Confidential Ledger.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
         :param confidential_ledger: Confidential Ledger request body for Updating Ledger. Required.
         :type confidential_ledger: ~azure.mgmt.confidentialledger.models.ConfidentialLedger
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -600,15 +599,16 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.ConfidentialLedger]:
         """Update Confidential Ledger properties.
 
         Updates properties of Confidential Ledger.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
         :param confidential_ledger: Confidential Ledger request body for Updating Ledger. Required.
         :type confidential_ledger: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -636,20 +636,21 @@
         confidential_ledger: Union[_models.ConfidentialLedger, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.ConfidentialLedger]:
         """Update Confidential Ledger properties.
 
         Updates properties of Confidential Ledger.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param ledger_name: Name of the Confidential Ledger. Required.
         :type ledger_name: str
         :param confidential_ledger: Confidential Ledger request body for Updating Ledger. Is either a
-         model type or a IO type. Required.
+         ConfidentialLedger type or a IO type. Required.
         :type confidential_ledger: ~azure.mgmt.confidentialledger.models.ConfidentialLedger or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -663,17 +664,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.confidentialledger.models.ConfidentialLedger]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ConfidentialLedger] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._update_initial(
@@ -719,31 +718,30 @@
         self, resource_group_name: str, filter: Optional[str] = None, **kwargs: Any
     ) -> AsyncIterable["_models.ConfidentialLedger"]:
         """Retrieves information about all Confidential Ledger resources under the given subscription and
         resource group.
 
         Retrieves the properties of all Confidential Ledgers.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param filter: The filter to apply on the list operation. eg. $filter=ledgerType eq 'Public'.
          Default value is None.
         :type filter: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ConfidentialLedger or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.confidentialledger.models.ConfidentialLedger]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConfidentialLedgerList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -789,16 +787,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
@@ -827,17 +826,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.confidentialledger.models.ConfidentialLedger]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConfidentialLedgerList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -882,16 +879,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/operations/_patch.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure/mgmt/confidentialledger/aio/operations/_operations.py` & `azure-mgmt-confidentialledger-2.0.0b2/azure/mgmt/confidentialledger/aio/operations/_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -25,19 +24,16 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._operations import build_list_request
+from .._vendor import ConfidentialLedgerMixinABC
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class Operations:
     """
     .. warning::
@@ -69,17 +65,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.confidentialledger.models.ResourceProviderOperationDefinition]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2020-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceProviderOperationList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -122,16 +116,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/PKG-INFO` & `azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-confidentialledger
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Microsoft Azure Confidential Ledger Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -27,36 +27,84 @@
 This package has been tested with Python 3.7+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
-# Usage
+## Getting started
 
+### Prerequisites
 
-To learn how to use this package, see the [quickstart guide](https://aka.ms/azsdk/python/mgmt)
- 
-For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/)
-Code samples for this package can be found at [Confidential Ledger Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
-Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+- Python 3.7+ is required to use this package.
+- [Azure subscription](https://azure.microsoft.com/free/)
 
+### Install the package
 
-# Provide Feedback
+```bash
+pip install azure-mgmt-confidentialledger
+pip install azure-identity
+```
+
+### Authentication
+
+By default, [Azure Active Directory](https://aka.ms/awps/aad) token authentication depends on correct configure of following environment variables.
+
+- `AZURE_CLIENT_ID` for Azure client ID.
+- `AZURE_TENANT_ID` for Azure tenant ID.
+- `AZURE_CLIENT_SECRET` for Azure client secret.
+
+In addition, Azure subscription ID can be configured via environment variable `AZURE_SUBSCRIPTION_ID`.
+
+With above configuration, client can be authenticated by following code:
+
+```python
+from azure.identity import DefaultAzureCredential
+from azure.mgmt.confidentialledger import ConfidentialLedger
+import os
+
+sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
+client = ConfidentialLedger(credential=DefaultAzureCredential(), subscription_id=sub_id)
+```
+
+## Examples
+
+Code samples for this package can be found at:
+- [Search Confidential Ledger Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+
+
+## Troubleshooting
+
+## Next steps
+
+## Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-confidentialledger%2FREADME.png)
 
 
 # Release History
 
+## 2.0.0b2 (2023-04-20)
+
+### Features Added
+
+  - Added operation group ManagedCCFOperations
+  - Model LedgerProperties has a new parameter running_state
+
+### Breaking Changes
+
+  - Model LedgerProperties no longer has parameter ledger_storage_account
+  - Parameter location of model ConfidentialLedger is now required
+
 ## 2.0.0b1 (2022-11-25)
 
 ### Features Added
 
   - Model LedgerProperties has a new parameter ledger_storage_account
 
 ### Breaking Changes
```

## Comparing `azure-mgmt-confidentialledger-2.0.0b1/azure_mgmt_confidentialledger.egg-info/SOURCES.txt` & `azure-mgmt-confidentialledger-2.0.0b2/azure_mgmt_confidentialledger.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,24 +14,29 @@
 azure/mgmt/confidentialledger/_vendor.py
 azure/mgmt/confidentialledger/_version.py
 azure/mgmt/confidentialledger/py.typed
 azure/mgmt/confidentialledger/aio/__init__.py
 azure/mgmt/confidentialledger/aio/_confidential_ledger.py
 azure/mgmt/confidentialledger/aio/_configuration.py
 azure/mgmt/confidentialledger/aio/_patch.py
+azure/mgmt/confidentialledger/aio/_vendor.py
 azure/mgmt/confidentialledger/aio/operations/__init__.py
+azure/mgmt/confidentialledger/aio/operations/_confidential_ledger_operations.py
 azure/mgmt/confidentialledger/aio/operations/_ledger_operations.py
+azure/mgmt/confidentialledger/aio/operations/_managed_ccf_operations.py
 azure/mgmt/confidentialledger/aio/operations/_operations.py
 azure/mgmt/confidentialledger/aio/operations/_patch.py
 azure/mgmt/confidentialledger/models/__init__.py
 azure/mgmt/confidentialledger/models/_confidential_ledger_enums.py
 azure/mgmt/confidentialledger/models/_models_py3.py
 azure/mgmt/confidentialledger/models/_patch.py
 azure/mgmt/confidentialledger/operations/__init__.py
+azure/mgmt/confidentialledger/operations/_confidential_ledger_operations.py
 azure/mgmt/confidentialledger/operations/_ledger_operations.py
+azure/mgmt/confidentialledger/operations/_managed_ccf_operations.py
 azure/mgmt/confidentialledger/operations/_operations.py
 azure/mgmt/confidentialledger/operations/_patch.py
 azure_mgmt_confidentialledger.egg-info/PKG-INFO
 azure_mgmt_confidentialledger.egg-info/SOURCES.txt
 azure_mgmt_confidentialledger.egg-info/dependency_links.txt
 azure_mgmt_confidentialledger.egg-info/not-zip-safe
 azure_mgmt_confidentialledger.egg-info/requires.txt
```

