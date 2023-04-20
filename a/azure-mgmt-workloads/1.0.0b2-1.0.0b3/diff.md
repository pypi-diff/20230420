# Comparing `tmp/azure-mgmt-workloads-1.0.0b2.zip` & `tmp/azure-mgmt-workloads-1.0.0b3.zip`

## zipinfo {}

```diff
@@ -1,70 +1,66 @@
-Zip file size: 173361 bytes, number of entries: 68
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/
--rw-rw-r--  2.0 unx     2824 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/setup.py
--rw-rw-r--  2.0 unx      626 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/_meta.json
--rw-rw-r--  2.0 unx     1254 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/CHANGELOG.md
--rw-rw-r--  2.0 unx     1074 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/LICENSE
--rw-rw-r--  2.0 unx     1364 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/README.md
--rw-rw-r--  2.0 unx      215 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/MANIFEST.in
--rw-rw-r--  2.0 unx     3511 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/PKG-INFO
--rw-rw-r--  2.0 unx       38 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/setup.cfg
--rw-rw-r--  2.0 unx        1 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        6 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     3511 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx     2643 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx      116 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/requires.txt
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/
--rw-rw-r--  2.0 unx       65 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/models/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/
--rw-rw-r--  2.0 unx       26 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/py.typed
--rw-rw-r--  2.0 unx      884 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/__init__.py
--rw-rw-r--  2.0 unx    77872 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_serialization.py
--rw-rw-r--  2.0 unx      488 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_version.py
--rw-rw-r--  2.0 unx     1530 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_patch.py
--rw-rw-r--  2.0 unx     1696 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_vendor.py
--rw-rw-r--  2.0 unx     7086 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_workloads_client.py
--rw-rw-r--  2.0 unx     3740 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_configuration.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/
--rw-rw-r--  2.0 unx      831 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/__init__.py
--rw-rw-r--  2.0 unx     1530 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/_patch.py
--rw-rw-r--  2.0 unx     1045 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/_vendor.py
--rw-rw-r--  2.0 unx     7268 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/_workloads_client.py
--rw-rw-r--  2.0 unx     3788 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/_configuration.py
--rw-rw-r--  2.0 unx     1817 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    56166 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_sap_virtual_instances_operations.py
--rw-rw-r--  2.0 unx     6148 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_skus_operations.py
--rw-rw-r--  2.0 unx    42560 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_sap_database_instances_operations.py
--rw-rw-r--  2.0 unx    36961 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_monitors_operations.py
--rw-rw-r--  2.0 unx     6062 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_operations.py
--rw-rw-r--  2.0 unx    37085 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_php_workloads_operations.py
--rw-rw-r--  2.0 unx    24240 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_wordpress_instances_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    26691 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_workloads_client_operations.py
--rw-rw-r--  2.0 unx    43010 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_sap_application_server_instances_operations.py
--rw-rw-r--  2.0 unx    29090 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_provider_instances_operations.py
--rw-rw-r--  2.0 unx    43341 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_sap_central_instances_operations.py
--rw-rw-r--  2.0 unx    14599 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/models/__init__.py
--rw-rw-r--  2.0 unx   275869 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/models/_models_py3.py
--rw-rw-r--  2.0 unx    11607 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/models/_workloads_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/models/_patch.py
--rw-rw-r--  2.0 unx     1817 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/__init__.py
--rw-rw-r--  2.0 unx    67321 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_sap_virtual_instances_operations.py
--rw-rw-r--  2.0 unx     7159 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_skus_operations.py
--rw-rw-r--  2.0 unx    50610 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_sap_database_instances_operations.py
--rw-rw-r--  2.0 unx    44876 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_monitors_operations.py
--rw-rw-r--  2.0 unx     6790 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_operations.py
--rw-rw-r--  2.0 unx    45338 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_php_workloads_operations.py
--rw-rw-r--  2.0 unx    29941 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_wordpress_instances_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_patch.py
--rw-rw-r--  2.0 unx    32460 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_workloads_client_operations.py
--rw-rw-r--  2.0 unx    51125 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_sap_application_server_instances_operations.py
--rw-rw-r--  2.0 unx    35066 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_provider_instances_operations.py
--rw-rw-r--  2.0 unx    51313 b- defN 22-Dec-02 06:53 azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_sap_central_instances_operations.py
-68 files, 1206182 bytes uncompressed, 158641 bytes compressed:  86.8%
+Zip file size: 159697 bytes, number of entries: 64
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/
+-rw-rw-r--  2.0 unx     4213 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/CHANGELOG.md
+-rw-rw-r--  2.0 unx     2109 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/README.md
+-rw-rw-r--  2.0 unx      215 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/MANIFEST.in
+-rw-rw-r--  2.0 unx     2824 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/setup.py
+-rw-rw-r--  2.0 unx     7215 b- defN 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/PKG-INFO
+-rw-rw-r--  2.0 unx       38 b- defN 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/setup.cfg
+-rw-rw-r--  2.0 unx      628 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/_meta.json
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/LICENSE
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/
+-rw-rw-r--  2.0 unx      488 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_version.py
+-rw-rw-r--  2.0 unx     3740 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_configuration.py
+-rw-rw-r--  2.0 unx      884 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/__init__.py
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_patch.py
+-rw-rw-r--  2.0 unx     1810 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_vendor.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/py.typed
+-rw-rw-r--  2.0 unx     6583 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_workloads_client.py
+-rw-rw-r--  2.0 unx    78824 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_serialization.py
+-rw-rw-r--  2.0 unx    32774 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_landscape_monitor_operations.py
+-rw-rw-r--  2.0 unx    73003 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_database_instances_operations.py
+-rw-rw-r--  2.0 unx     1662 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_patch.py
+-rw-rw-r--  2.0 unx    67321 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_virtual_instances_operations.py
+-rw-rw-r--  2.0 unx    73681 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_central_instances_operations.py
+-rw-rw-r--  2.0 unx    32460 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_workloads_client_operations.py
+-rw-rw-r--  2.0 unx    44876 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_monitors_operations.py
+-rw-rw-r--  2.0 unx    35066 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_provider_instances_operations.py
+-rw-rw-r--  2.0 unx    73463 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_application_server_instances_operations.py
+-rw-rw-r--  2.0 unx     6790 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_operations.py
+-rw-rw-r--  2.0 unx    13509 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/models/_patch.py
+-rw-rw-r--  2.0 unx     7958 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/models/_workloads_client_enums.py
+-rw-rw-r--  2.0 unx   263851 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/models/_models_py3.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/
+-rw-rw-r--  2.0 unx     3788 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/_configuration.py
+-rw-rw-r--  2.0 unx      831 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/__init__.py
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/_patch.py
+-rw-rw-r--  2.0 unx     1045 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/_vendor.py
+-rw-rw-r--  2.0 unx     6762 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/_workloads_client.py
+-rw-rw-r--  2.0 unx    25234 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_sap_landscape_monitor_operations.py
+-rw-rw-r--  2.0 unx    61641 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_sap_database_instances_operations.py
+-rw-rw-r--  2.0 unx     1662 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx    56166 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_sap_virtual_instances_operations.py
+-rw-rw-r--  2.0 unx    62409 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_sap_central_instances_operations.py
+-rw-rw-r--  2.0 unx    26691 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_workloads_client_operations.py
+-rw-rw-r--  2.0 unx    36961 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_monitors_operations.py
+-rw-rw-r--  2.0 unx    29090 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_provider_instances_operations.py
+-rw-rw-r--  2.0 unx    62000 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_sap_application_server_instances_operations.py
+-rw-rw-r--  2.0 unx     6062 b- defN 23-Feb-16 06:34 azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx     2413 b- defN 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        1 b- defN 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     7215 b- defN 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx      116 b- defN 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-Feb-16 06:35 azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/top_level.txt
+64 files, 1232391 bytes uncompressed, 145965 bytes compressed:  88.2%
```

## zipnote {}

```diff
@@ -1,205 +1,193 @@
-Filename: azure-mgmt-workloads-1.0.0b2/
+Filename: azure-mgmt-workloads-1.0.0b3/
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/
+Filename: azure-mgmt-workloads-1.0.0b3/azure/
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/
+Filename: azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/setup.py
+Filename: azure-mgmt-workloads-1.0.0b3/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/_meta.json
+Filename: azure-mgmt-workloads-1.0.0b3/README.md
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/CHANGELOG.md
+Filename: azure-mgmt-workloads-1.0.0b3/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/LICENSE
+Filename: azure-mgmt-workloads-1.0.0b3/setup.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/README.md
+Filename: azure-mgmt-workloads-1.0.0b3/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/MANIFEST.in
+Filename: azure-mgmt-workloads-1.0.0b3/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/PKG-INFO
+Filename: azure-mgmt-workloads-1.0.0b3/_meta.json
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/setup.cfg
+Filename: azure-mgmt-workloads-1.0.0b3/LICENSE
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/not-zip-safe
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/top_level.txt
+Filename: azure-mgmt-workloads-1.0.0b3/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/dependency_links.txt
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/PKG-INFO
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/SOURCES.txt
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/requires.txt
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/models/
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/__init__.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_version.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/__init__.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/__init__.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_patch.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/models/
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/py.typed
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/py.typed
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_workloads_client.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/__init__.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_serialization.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_landscape_monitor_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_version.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_database_instances_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_patch.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_vendor.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_workloads_client.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_virtual_instances_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_configuration.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_central_instances_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_workloads_client_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/__init__.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_monitors_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/_patch.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_provider_instances_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/_vendor.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_application_server_instances_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/_workloads_client.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/_configuration.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/__init__.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_sap_virtual_instances_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/models/_workloads_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_skus_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_sap_database_instances_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_monitors_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_php_workloads_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_wordpress_instances_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_patch.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/_workloads_client.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_workloads_client_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_sap_landscape_monitor_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_sap_application_server_instances_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_sap_database_instances_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_provider_instances_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_sap_central_instances_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/models/__init__.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_sap_virtual_instances_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/models/_models_py3.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_sap_central_instances_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/models/_workloads_client_enums.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_workloads_client_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/models/_patch.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_monitors_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/__init__.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_provider_instances_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_sap_virtual_instances_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_sap_application_server_instances_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_skus_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_sap_database_instances_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_monitors_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_php_workloads_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_wordpress_instances_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_patch.py
-Comment: 
-
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_workloads_client_operations.py
-Comment: 
-
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_sap_application_server_instances_operations.py
-Comment: 
-
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_provider_instances_operations.py
-Comment: 
-
-Filename: azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_sap_central_instances_operations.py
+Filename: azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-workloads-1.0.0b2/setup.py` & `azure-mgmt-workloads-1.0.0b3/setup.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-workloads-1.0.0b2/_meta.json` & `azure-mgmt-workloads-1.0.0b3/_meta.json`

 * *Files 22% similar despite different names*

### Pretty-printed

 * *Similarity: 0.7777777777777777%*

 * *Differences: {"'autorest_command'": "'autorest specification/workloads/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.2.16 --use=@autorest/modelerfour@4.24.3 '*

 * *                       "--version=3.9.2 --version-tolerant=False'",*

 * * "'commit'": "'630ec444f8dd7c09b9cdd5fa99951f8a0d1ad41f'",*

 * * "'use'": "{inse […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.2",
-    "autorest_command": "autorest specification/workloads/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.2.7 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
-    "commit": "2f2e48923cebd95f7d184608a29bcd06d9cb3653",
+    "autorest_command": "autorest specification/workloads/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.2.16 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
+    "commit": "630ec444f8dd7c09b9cdd5fa99951f8a0d1ad41f",
     "readme": "specification/workloads/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.2.7",
+        "@autorest/python@6.2.16",
         "@autorest/modelerfour@4.24.3"
     ]
 }
```

## Comparing `azure-mgmt-workloads-1.0.0b2/LICENSE` & `azure-mgmt-workloads-1.0.0b3/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-workloads-1.0.0b2/azure_mgmt_workloads.egg-info/SOURCES.txt` & `azure-mgmt-workloads-1.0.0b3/azure_mgmt_workloads.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,39 +19,35 @@
 azure/mgmt/workloads/aio/_patch.py
 azure/mgmt/workloads/aio/_vendor.py
 azure/mgmt/workloads/aio/_workloads_client.py
 azure/mgmt/workloads/aio/operations/__init__.py
 azure/mgmt/workloads/aio/operations/_monitors_operations.py
 azure/mgmt/workloads/aio/operations/_operations.py
 azure/mgmt/workloads/aio/operations/_patch.py
-azure/mgmt/workloads/aio/operations/_php_workloads_operations.py
 azure/mgmt/workloads/aio/operations/_provider_instances_operations.py
 azure/mgmt/workloads/aio/operations/_sap_application_server_instances_operations.py
 azure/mgmt/workloads/aio/operations/_sap_central_instances_operations.py
 azure/mgmt/workloads/aio/operations/_sap_database_instances_operations.py
+azure/mgmt/workloads/aio/operations/_sap_landscape_monitor_operations.py
 azure/mgmt/workloads/aio/operations/_sap_virtual_instances_operations.py
-azure/mgmt/workloads/aio/operations/_skus_operations.py
-azure/mgmt/workloads/aio/operations/_wordpress_instances_operations.py
 azure/mgmt/workloads/aio/operations/_workloads_client_operations.py
 azure/mgmt/workloads/models/__init__.py
 azure/mgmt/workloads/models/_models_py3.py
 azure/mgmt/workloads/models/_patch.py
 azure/mgmt/workloads/models/_workloads_client_enums.py
 azure/mgmt/workloads/operations/__init__.py
 azure/mgmt/workloads/operations/_monitors_operations.py
 azure/mgmt/workloads/operations/_operations.py
 azure/mgmt/workloads/operations/_patch.py
-azure/mgmt/workloads/operations/_php_workloads_operations.py
 azure/mgmt/workloads/operations/_provider_instances_operations.py
 azure/mgmt/workloads/operations/_sap_application_server_instances_operations.py
 azure/mgmt/workloads/operations/_sap_central_instances_operations.py
 azure/mgmt/workloads/operations/_sap_database_instances_operations.py
+azure/mgmt/workloads/operations/_sap_landscape_monitor_operations.py
 azure/mgmt/workloads/operations/_sap_virtual_instances_operations.py
-azure/mgmt/workloads/operations/_skus_operations.py
-azure/mgmt/workloads/operations/_wordpress_instances_operations.py
 azure/mgmt/workloads/operations/_workloads_client_operations.py
 azure_mgmt_workloads.egg-info/PKG-INFO
 azure_mgmt_workloads.egg-info/SOURCES.txt
 azure_mgmt_workloads.egg-info/dependency_links.txt
 azure_mgmt_workloads.egg-info/not-zip-safe
 azure_mgmt_workloads.egg-info/requires.txt
 azure_mgmt_workloads.egg-info/top_level.txt
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/__init__.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_serialization.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_serialization.py`

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

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_patch.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_vendor.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_vendor.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from abc import ABC
-from typing import TYPE_CHECKING
+from typing import List, TYPE_CHECKING, cast
 
 from azure.core.pipeline.transport import HttpRequest
 
 from ._configuration import WorkloadsClientConfiguration
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
@@ -29,15 +29,16 @@
 
 def _format_url_section(template, **kwargs):
     components = template.split("/")
     while components:
         try:
             return template.format(**kwargs)
         except KeyError as key:
-            formatted_components = template.split("/")
+            # Need the cast, as for some reasons "split" is typed as list[str | Any]
+            formatted_components = cast(List[str], template.split("/"))
             components = [c for c in formatted_components if "{}".format(key.args[0]) not in c]
             template = "/".join(components)
 
 
 class WorkloadsClientMixinABC(ABC):
     """DO NOT use this class. It is for internal typing use only."""
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_workloads_client.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/_workloads_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,141 +3,137 @@
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
 from ._configuration import WorkloadsClientConfiguration
-from ._serialization import Deserializer, Serializer
 from .operations import (
     MonitorsOperations,
     Operations,
-    PhpWorkloadsOperations,
     ProviderInstancesOperations,
     SAPApplicationServerInstancesOperations,
     SAPCentralInstancesOperations,
     SAPDatabaseInstancesOperations,
     SAPVirtualInstancesOperations,
-    SkusOperations,
-    WordpressInstancesOperations,
+    SapLandscapeMonitorOperations,
     WorkloadsClientOperationsMixin,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials import TokenCredential
+    from azure.core.credentials_async import AsyncTokenCredential
 
 
 class WorkloadsClient(
     WorkloadsClientOperationsMixin
 ):  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """Workloads client provides access to various workload operations.
 
-    :ivar php_workloads: PhpWorkloadsOperations operations
-    :vartype php_workloads: azure.mgmt.workloads.operations.PhpWorkloadsOperations
-    :ivar wordpress_instances: WordpressInstancesOperations operations
-    :vartype wordpress_instances: azure.mgmt.workloads.operations.WordpressInstancesOperations
     :ivar sap_virtual_instances: SAPVirtualInstancesOperations operations
-    :vartype sap_virtual_instances: azure.mgmt.workloads.operations.SAPVirtualInstancesOperations
+    :vartype sap_virtual_instances:
+     azure.mgmt.workloads.aio.operations.SAPVirtualInstancesOperations
     :ivar sap_central_instances: SAPCentralInstancesOperations operations
-    :vartype sap_central_instances: azure.mgmt.workloads.operations.SAPCentralInstancesOperations
+    :vartype sap_central_instances:
+     azure.mgmt.workloads.aio.operations.SAPCentralInstancesOperations
     :ivar sap_database_instances: SAPDatabaseInstancesOperations operations
-    :vartype sap_database_instances: azure.mgmt.workloads.operations.SAPDatabaseInstancesOperations
+    :vartype sap_database_instances:
+     azure.mgmt.workloads.aio.operations.SAPDatabaseInstancesOperations
     :ivar sap_application_server_instances: SAPApplicationServerInstancesOperations operations
     :vartype sap_application_server_instances:
-     azure.mgmt.workloads.operations.SAPApplicationServerInstancesOperations
-    :ivar operations: Operations operations
-    :vartype operations: azure.mgmt.workloads.operations.Operations
+     azure.mgmt.workloads.aio.operations.SAPApplicationServerInstancesOperations
     :ivar monitors: MonitorsOperations operations
-    :vartype monitors: azure.mgmt.workloads.operations.MonitorsOperations
+    :vartype monitors: azure.mgmt.workloads.aio.operations.MonitorsOperations
     :ivar provider_instances: ProviderInstancesOperations operations
-    :vartype provider_instances: azure.mgmt.workloads.operations.ProviderInstancesOperations
-    :ivar skus: SkusOperations operations
-    :vartype skus: azure.mgmt.workloads.operations.SkusOperations
+    :vartype provider_instances: azure.mgmt.workloads.aio.operations.ProviderInstancesOperations
+    :ivar sap_landscape_monitor: SapLandscapeMonitorOperations operations
+    :vartype sap_landscape_monitor:
+     azure.mgmt.workloads.aio.operations.SapLandscapeMonitorOperations
+    :ivar operations: Operations operations
+    :vartype operations: azure.mgmt.workloads.aio.operations.Operations
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials.TokenCredential
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2021-12-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
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
         self._config = WorkloadsClientConfiguration(credential=credential, subscription_id=subscription_id, **kwargs)
-        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
-        self.php_workloads = PhpWorkloadsOperations(self._client, self._config, self._serialize, self._deserialize)
-        self.wordpress_instances = WordpressInstancesOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
         self.sap_virtual_instances = SAPVirtualInstancesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.sap_central_instances = SAPCentralInstancesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.sap_database_instances = SAPDatabaseInstancesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.sap_application_server_instances = SAPApplicationServerInstancesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
-        self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.monitors = MonitorsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.provider_instances = ProviderInstancesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
-        self.skus = SkusOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.sap_landscape_monitor = SapLandscapeMonitorOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
+        self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
 
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
 
-    def __enter__(self) -> "WorkloadsClient":
-        self._client.__enter__()
+    async def __aenter__(self) -> "WorkloadsClient":
+        await self._client.__aenter__()
         return self
 
-    def __exit__(self, *exc_details) -> None:
-        self._client.__exit__(*exc_details)
+    async def __aexit__(self, *exc_details) -> None:
+        await self._client.__aexit__(*exc_details)
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/_configuration.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2021-12-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(WorkloadsClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop("api_version", "2021-12-01-preview")
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop("api_version", "2022-11-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/__init__.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/_patch.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/_vendor.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/_workloads_client.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/_workloads_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,144 +3,133 @@
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
 from ._configuration import WorkloadsClientConfiguration
+from ._serialization import Deserializer, Serializer
 from .operations import (
     MonitorsOperations,
     Operations,
-    PhpWorkloadsOperations,
     ProviderInstancesOperations,
     SAPApplicationServerInstancesOperations,
     SAPCentralInstancesOperations,
     SAPDatabaseInstancesOperations,
     SAPVirtualInstancesOperations,
-    SkusOperations,
-    WordpressInstancesOperations,
+    SapLandscapeMonitorOperations,
     WorkloadsClientOperationsMixin,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials_async import AsyncTokenCredential
+    from azure.core.credentials import TokenCredential
 
 
 class WorkloadsClient(
     WorkloadsClientOperationsMixin
 ):  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """Workloads client provides access to various workload operations.
 
-    :ivar php_workloads: PhpWorkloadsOperations operations
-    :vartype php_workloads: azure.mgmt.workloads.aio.operations.PhpWorkloadsOperations
-    :ivar wordpress_instances: WordpressInstancesOperations operations
-    :vartype wordpress_instances: azure.mgmt.workloads.aio.operations.WordpressInstancesOperations
     :ivar sap_virtual_instances: SAPVirtualInstancesOperations operations
-    :vartype sap_virtual_instances:
-     azure.mgmt.workloads.aio.operations.SAPVirtualInstancesOperations
+    :vartype sap_virtual_instances: azure.mgmt.workloads.operations.SAPVirtualInstancesOperations
     :ivar sap_central_instances: SAPCentralInstancesOperations operations
-    :vartype sap_central_instances:
-     azure.mgmt.workloads.aio.operations.SAPCentralInstancesOperations
+    :vartype sap_central_instances: azure.mgmt.workloads.operations.SAPCentralInstancesOperations
     :ivar sap_database_instances: SAPDatabaseInstancesOperations operations
-    :vartype sap_database_instances:
-     azure.mgmt.workloads.aio.operations.SAPDatabaseInstancesOperations
+    :vartype sap_database_instances: azure.mgmt.workloads.operations.SAPDatabaseInstancesOperations
     :ivar sap_application_server_instances: SAPApplicationServerInstancesOperations operations
     :vartype sap_application_server_instances:
-     azure.mgmt.workloads.aio.operations.SAPApplicationServerInstancesOperations
-    :ivar operations: Operations operations
-    :vartype operations: azure.mgmt.workloads.aio.operations.Operations
+     azure.mgmt.workloads.operations.SAPApplicationServerInstancesOperations
     :ivar monitors: MonitorsOperations operations
-    :vartype monitors: azure.mgmt.workloads.aio.operations.MonitorsOperations
+    :vartype monitors: azure.mgmt.workloads.operations.MonitorsOperations
     :ivar provider_instances: ProviderInstancesOperations operations
-    :vartype provider_instances: azure.mgmt.workloads.aio.operations.ProviderInstancesOperations
-    :ivar skus: SkusOperations operations
-    :vartype skus: azure.mgmt.workloads.aio.operations.SkusOperations
+    :vartype provider_instances: azure.mgmt.workloads.operations.ProviderInstancesOperations
+    :ivar sap_landscape_monitor: SapLandscapeMonitorOperations operations
+    :vartype sap_landscape_monitor: azure.mgmt.workloads.operations.SapLandscapeMonitorOperations
+    :ivar operations: Operations operations
+    :vartype operations: azure.mgmt.workloads.operations.Operations
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2021-12-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
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
         self._config = WorkloadsClientConfiguration(credential=credential, subscription_id=subscription_id, **kwargs)
-        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
-        self.php_workloads = PhpWorkloadsOperations(self._client, self._config, self._serialize, self._deserialize)
-        self.wordpress_instances = WordpressInstancesOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
         self.sap_virtual_instances = SAPVirtualInstancesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.sap_central_instances = SAPCentralInstancesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.sap_database_instances = SAPDatabaseInstancesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.sap_application_server_instances = SAPApplicationServerInstancesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
-        self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.monitors = MonitorsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.provider_instances = ProviderInstancesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
-        self.skus = SkusOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.sap_landscape_monitor = SapLandscapeMonitorOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
+        self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
 
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
 
-    async def __aenter__(self) -> "WorkloadsClient":
-        await self._client.__aenter__()
+    def __enter__(self) -> "WorkloadsClient":
+        self._client.__enter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
-        await self._client.__aexit__(*exc_details)
+    def __exit__(self, *exc_details) -> None:
+        self._client.__exit__(*exc_details)
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/_configuration.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2021-12-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(WorkloadsClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop("api_version", "2021-12-01-preview")
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop("api_version", "2022-11-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/__init__.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,38 +2,34 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._php_workloads_operations import PhpWorkloadsOperations
-from ._wordpress_instances_operations import WordpressInstancesOperations
 from ._workloads_client_operations import WorkloadsClientOperationsMixin
 from ._sap_virtual_instances_operations import SAPVirtualInstancesOperations
 from ._sap_central_instances_operations import SAPCentralInstancesOperations
 from ._sap_database_instances_operations import SAPDatabaseInstancesOperations
 from ._sap_application_server_instances_operations import SAPApplicationServerInstancesOperations
-from ._operations import Operations
 from ._monitors_operations import MonitorsOperations
 from ._provider_instances_operations import ProviderInstancesOperations
-from ._skus_operations import SkusOperations
+from ._sap_landscape_monitor_operations import SapLandscapeMonitorOperations
+from ._operations import Operations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "PhpWorkloadsOperations",
-    "WordpressInstancesOperations",
     "WorkloadsClientOperationsMixin",
     "SAPVirtualInstancesOperations",
     "SAPCentralInstancesOperations",
     "SAPDatabaseInstancesOperations",
     "SAPApplicationServerInstancesOperations",
-    "Operations",
     "MonitorsOperations",
     "ProviderInstancesOperations",
-    "SkusOperations",
+    "SapLandscapeMonitorOperations",
+    "Operations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_sap_virtual_instances_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_sap_virtual_instances_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPVirtualInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -254,15 +254,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.SAPVirtualInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPVirtualInstance] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -332,15 +332,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPVirtualInstance] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -469,15 +469,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPVirtualInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -537,15 +537,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -607,15 +607,15 @@
          of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -672,15 +672,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.SAPVirtualInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPVirtualInstanceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -758,15 +758,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.SAPVirtualInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPVirtualInstanceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -844,15 +844,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         request = build_start_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -914,15 +914,15 @@
          of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -979,15 +979,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -1152,15 +1152,15 @@
          of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_skus_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,74 +24,73 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._skus_operations import build_list_request
+from ...operations._operations import build_list_request
 from .._vendor import WorkloadsClientMixinABC
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
     from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class SkusOperations:
+class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.workloads.aio.WorkloadsClient`'s
-        :attr:`skus` attribute.
+        :attr:`operations` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> AsyncIterable["_models.SkuDefinition"]:
-        """Lists all the available SKUs under this PR.
+    def list(self, **kwargs: Any) -> AsyncIterable["_models.Operation"]:
+        """Lists all the available API operations under this PR.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either SkuDefinition or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.SkuDefinition]
+        :return: An iterator like instance of either Operation or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
-        cls: ClsType[_models.SkusListResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
                 request = build_list_request(
-                    subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
@@ -111,15 +110,15 @@
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("SkusListResult", pipeline_response)
+            deserialized = self._deserialize("OperationListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
@@ -134,8 +133,8 @@
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Workloads/skus"}
+    list.metadata = {"url": "/providers/Microsoft.Workloads/operations"}
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_sap_database_instances_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_sap_database_instances_operations.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._sap_database_instances_operations import (
     build_create_request,
     build_delete_request,
     build_get_request,
     build_list_request,
+    build_start_instance_request,
+    build_stop_instance_request,
     build_update_request,
 )
 from .._vendor import WorkloadsClientMixinABC
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
@@ -94,15 +96,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPDatabaseInstance] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -153,15 +155,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPDatabaseInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -342,15 +344,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.SAPDatabaseInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPDatabaseInstance] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -412,15 +414,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPDatabaseInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -595,15 +597,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.SAPDatabaseInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPDatabaseInstance] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -660,15 +662,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -735,15 +737,15 @@
          of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -804,15 +806,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.SAPDatabaseInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPDatabaseInstanceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -877,7 +879,393 @@
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
     list.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances"
     }
+
+    async def _start_instance_initial(
+        self, resource_group_name: str, sap_virtual_instance_name: str, database_instance_name: str, **kwargs: Any
+    ) -> Optional[_models.OperationStatusResult]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
+
+        request = build_start_instance_request(
+            resource_group_name=resource_group_name,
+            sap_virtual_instance_name=sap_virtual_instance_name,
+            database_instance_name=database_instance_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self._start_instance_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    _start_instance_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances/{databaseInstanceName}/start"
+    }
+
+    @distributed_trace_async
+    async def begin_start_instance(
+        self, resource_group_name: str, sap_virtual_instance_name: str, database_instance_name: str, **kwargs: Any
+    ) -> AsyncLROPoller[_models.OperationStatusResult]:
+        """Starts the database instance of the SAP system.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param database_instance_name: Database resource name string modeled as parameter for auto
+         generation to work correctly. Required.
+        :type database_instance_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either OperationStatusResult or the result
+         of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._start_instance_initial(
+                resource_group_name=resource_group_name,
+                sap_virtual_instance_name=sap_virtual_instance_name,
+                database_instance_name=database_instance_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            )
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_start_instance.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances/{databaseInstanceName}/start"
+    }
+
+    async def _stop_instance_initial(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        database_instance_name: str,
+        body: Optional[Union[_models.StopRequest, IO]] = None,
+        **kwargs: Any
+    ) -> Optional[_models.OperationStatusResult]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IO, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "StopRequest")
+            else:
+                _json = None
+
+        request = build_stop_instance_request(
+            resource_group_name=resource_group_name,
+            sap_virtual_instance_name=sap_virtual_instance_name,
+            database_instance_name=database_instance_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self._stop_instance_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    _stop_instance_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances/{databaseInstanceName}/stop"
+    }
+
+    @overload
+    async def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        database_instance_name: str,
+        body: Optional[_models.StopRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.OperationStatusResult]:
+        """Stops the database instance of the SAP system.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param database_instance_name: Database resource name string modeled as parameter for auto
+         generation to work correctly. Required.
+        :type database_instance_name: str
+        :param body: Stop request for the database instance of the SAP system. Default value is None.
+        :type body: ~azure.mgmt.workloads.models.StopRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either OperationStatusResult or the result
+         of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        database_instance_name: str,
+        body: Optional[IO] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.OperationStatusResult]:
+        """Stops the database instance of the SAP system.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param database_instance_name: Database resource name string modeled as parameter for auto
+         generation to work correctly. Required.
+        :type database_instance_name: str
+        :param body: Stop request for the database instance of the SAP system. Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either OperationStatusResult or the result
+         of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        database_instance_name: str,
+        body: Optional[Union[_models.StopRequest, IO]] = None,
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.OperationStatusResult]:
+        """Stops the database instance of the SAP system.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param database_instance_name: Database resource name string modeled as parameter for auto
+         generation to work correctly. Required.
+        :type database_instance_name: str
+        :param body: Stop request for the database instance of the SAP system. Is either a model type
+         or a IO type. Default value is None.
+        :type body: ~azure.mgmt.workloads.models.StopRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either OperationStatusResult or the result
+         of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._stop_instance_initial(
+                resource_group_name=resource_group_name,
+                sap_virtual_instance_name=sap_virtual_instance_name,
+                database_instance_name=database_instance_name,
+                body=body,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            )
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_stop_instance.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances/{databaseInstanceName}/stop"
+    }
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_monitors_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_monitors_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         :return: An iterator like instance of either Monitor or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.Monitor]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.MonitorListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -166,15 +166,15 @@
         :return: An iterator like instance of either Monitor or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.Monitor]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.MonitorListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -267,15 +267,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.Monitor] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
@@ -320,15 +320,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Monitor] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -486,15 +486,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.Monitor]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Monitor] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -550,15 +550,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
@@ -620,15 +620,15 @@
          of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -765,15 +765,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Monitor] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_operations.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,78 +3,101 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import sys
-from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
+from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._operations import build_list_request
-from .._vendor import WorkloadsClientMixinABC
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import WorkloadsClientMixinABC, _convert_request
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
     from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_list_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/providers/Microsoft.Workloads/operations")
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.workloads.aio.WorkloadsClient`'s
+        :class:`~azure.mgmt.workloads.WorkloadsClient`'s
         :attr:`operations` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> AsyncIterable["_models.Operation"]:
+    def list(self, **kwargs: Any) -> Iterable["_models.Operation"]:
         """Lists all the available API operations under this PR.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Operation or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.Operation]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.workloads.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -109,32 +132,32 @@
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
-        async def extract_data(pipeline_response):
+        def extract_data(pipeline_response):
             deserialized = self._deserialize("OperationListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+            return deserialized.next_link or None, iter(list_of_elem)
 
-        async def get_next(next_link=None):
+        def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
                 request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(get_next, extract_data)
+        return ItemPaged(get_next, extract_data)
 
     list.metadata = {"url": "/providers/Microsoft.Workloads/operations"}
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_php_workloads_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_provider_instances_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,199 +3,255 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import sys
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
-from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
+from azure.core.pipeline.transport import HttpResponse
+from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
-from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
+from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._php_workloads_operations import (
-    build_create_or_update_request,
-    build_delete_request,
-    build_get_request,
-    build_list_by_resource_group_request,
-    build_list_by_subscription_request,
-    build_update_request,
-)
-from .._vendor import WorkloadsClientMixinABC
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import WorkloadsClientMixinABC, _convert_request, _format_url_section
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
     from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
 
-class PhpWorkloadsOperations:
-    """
-    .. warning::
-        **DO NOT** instantiate this class directly.
 
-        Instead, you should access the following operations through
-        :class:`~azure.mgmt.workloads.aio.WorkloadsClient`'s
-        :attr:`php_workloads` attribute.
-    """
+def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
+    }
 
-    models = _models
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
-    def __init__(self, *args, **kwargs) -> None:
-        input_args = list(args)
-        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
-        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
-        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
-        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
-    @distributed_trace
-    def list_by_subscription(self, **kwargs: Any) -> AsyncIterable["_models.PhpWorkloadResource"]:
-        """Lists PHP workload resources for a subscription.
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either PhpWorkloadResource or the result of cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.PhpWorkloadResource]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_get_request(
+    resource_group_name: str, monitor_name: str, provider_instance_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
+        "providerInstanceName": _SERIALIZER.url("provider_instance_name", provider_instance_name, "str"),
+    }
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.PhpWorkloadResourceList] = kwargs.pop("cls", None)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
-        def prepare_request(next_link=None):
-            if not next_link:
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-                request = build_list_by_subscription_request(
-                    subscription_id=self._config.subscription_id,
-                    api_version=api_version,
-                    template_url=self.list_by_subscription.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_create_request(
+    resource_group_name: str, monitor_name: str, provider_instance_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
+        "providerInstanceName": _SERIALIZER.url("provider_instance_name", provider_instance_name, "str"),
+    }
 
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("PhpWorkloadResourceList", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_delete_request(
+    resource_group_name: str, monitor_name: str, provider_instance_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
+        "providerInstanceName": _SERIALIZER.url("provider_instance_name", provider_instance_name, "str"),
+    }
 
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
-            )
-            response = pipeline_response.http_response
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
-            return pipeline_response
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-        return AsyncItemPaged(get_next, extract_data)
+    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
-    list_by_subscription.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.Workloads/phpWorkloads"
-    }
+
+class ProviderInstancesOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~azure.mgmt.workloads.WorkloadsClient`'s
+        :attr:`provider_instances` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list_by_resource_group(
-        self, resource_group_name: str, **kwargs: Any
-    ) -> AsyncIterable["_models.PhpWorkloadResource"]:
-        """Lists PHP workload resources in a resource group.
+    def list(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> Iterable["_models.ProviderInstance"]:
+        """Gets a list of provider instances in the specified SAP monitor.
+
+        Gets a list of provider instances in the specified SAP monitor. The operations returns various
+        properties of each provider instances.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either PhpWorkloadResource or the result of cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.PhpWorkloadResource]
+        :return: An iterator like instance of either ProviderInstance or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.workloads.models.ProviderInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
-        cls: ClsType[_models.PhpWorkloadResourceList] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ProviderInstanceListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_resource_group_request(
+                request = build_list_request(
                     resource_group_name=resource_group_name,
+                    monitor_name=monitor_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
+                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
 
             else:
@@ -212,598 +268,493 @@
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("PhpWorkloadResourceList", pipeline_response)
+        def extract_data(pipeline_response):
+            deserialized = self._deserialize("ProviderInstanceListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+            return deserialized.next_link or None, iter(list_of_elem)
 
-        async def get_next(next_link=None):
+        def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
                 request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(get_next, extract_data)
+        return ItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/phpWorkloads"
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances"
     }
 
-    @distributed_trace_async
-    async def get(self, resource_group_name: str, php_workload_name: str, **kwargs: Any) -> _models.PhpWorkloadResource:
-        """Gets the PHP workload resource.
+    @distributed_trace
+    def get(
+        self, resource_group_name: str, monitor_name: str, provider_instance_name: str, **kwargs: Any
+    ) -> _models.ProviderInstance:
+        """Gets properties of a provider instance.
+
+        Gets properties of a provider instance for the specified subscription, resource group, SAP
+        monitor name, and resource name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param php_workload_name: Php workload name. Required.
-        :type php_workload_name: str
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
+        :param provider_instance_name: Name of the provider instance. Required.
+        :type provider_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: PhpWorkloadResource or the result of cls(response)
-        :rtype: ~azure.mgmt.workloads.models.PhpWorkloadResource
+        :return: ProviderInstance or the result of cls(response)
+        :rtype: ~azure.mgmt.workloads.models.ProviderInstance
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
-        cls: ClsType[_models.PhpWorkloadResource] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ProviderInstance] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
-            php_workload_name=php_workload_name,
+            monitor_name=monitor_name,
+            provider_instance_name=provider_instance_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("PhpWorkloadResource", pipeline_response)
+        deserialized = self._deserialize("ProviderInstance", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/phpWorkloads/{phpWorkloadName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
     }
 
-    async def _create_or_update_initial(
+    def _create_initial(
         self,
         resource_group_name: str,
-        php_workload_name: str,
-        php_workload_resource: Union[_models.PhpWorkloadResource, IO],
+        monitor_name: str,
+        provider_instance_name: str,
+        provider_instance_parameter: Union[_models.ProviderInstance, IO],
         **kwargs: Any
-    ) -> _models.PhpWorkloadResource:
+    ) -> _models.ProviderInstance:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.PhpWorkloadResource] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ProviderInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(php_workload_resource, (IO, bytes)):
-            _content = php_workload_resource
+        if isinstance(provider_instance_parameter, (IO, bytes)):
+            _content = provider_instance_parameter
         else:
-            _json = self._serialize.body(php_workload_resource, "PhpWorkloadResource")
+            _json = self._serialize.body(provider_instance_parameter, "ProviderInstance")
 
-        request = build_create_or_update_request(
+        request = build_create_request(
             resource_group_name=resource_group_name,
-            php_workload_name=php_workload_name,
+            monitor_name=monitor_name,
+            provider_instance_name=provider_instance_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
+            template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
-            deserialized = self._deserialize("PhpWorkloadResource", pipeline_response)
+            deserialized = self._deserialize("ProviderInstance", pipeline_response)
 
         if response.status_code == 201:
-            deserialized = self._deserialize("PhpWorkloadResource", pipeline_response)
+            deserialized = self._deserialize("ProviderInstance", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/phpWorkloads/{phpWorkloadName}"
+    _create_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
     }
 
     @overload
-    async def begin_create_or_update(
+    def begin_create(
         self,
         resource_group_name: str,
-        php_workload_name: str,
-        php_workload_resource: _models.PhpWorkloadResource,
+        monitor_name: str,
+        provider_instance_name: str,
+        provider_instance_parameter: _models.ProviderInstance,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.PhpWorkloadResource]:
-        """Create or updated PHP workload resource.
+    ) -> LROPoller[_models.ProviderInstance]:
+        """Creates a provider instance.
+
+        Creates a provider instance for the specified subscription, resource group, SAP monitor name,
+        and resource name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param php_workload_name: Php workload name. Required.
-        :type php_workload_name: str
-        :param php_workload_resource: Resource create or update request payload. Required.
-        :type php_workload_resource: ~azure.mgmt.workloads.models.PhpWorkloadResource
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
+        :param provider_instance_name: Name of the provider instance. Required.
+        :type provider_instance_name: str
+        :param provider_instance_parameter: Request body representing a provider instance. Required.
+        :type provider_instance_parameter: ~azure.mgmt.workloads.models.ProviderInstance
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either PhpWorkloadResource or the result of
+        :return: An instance of LROPoller that returns either ProviderInstance or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.PhpWorkloadResource]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.ProviderInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def begin_create_or_update(
+    def begin_create(
         self,
         resource_group_name: str,
-        php_workload_name: str,
-        php_workload_resource: IO,
+        monitor_name: str,
+        provider_instance_name: str,
+        provider_instance_parameter: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.PhpWorkloadResource]:
-        """Create or updated PHP workload resource.
+    ) -> LROPoller[_models.ProviderInstance]:
+        """Creates a provider instance.
+
+        Creates a provider instance for the specified subscription, resource group, SAP monitor name,
+        and resource name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param php_workload_name: Php workload name. Required.
-        :type php_workload_name: str
-        :param php_workload_resource: Resource create or update request payload. Required.
-        :type php_workload_resource: IO
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
+        :param provider_instance_name: Name of the provider instance. Required.
+        :type provider_instance_name: str
+        :param provider_instance_parameter: Request body representing a provider instance. Required.
+        :type provider_instance_parameter: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either PhpWorkloadResource or the result of
+        :return: An instance of LROPoller that returns either ProviderInstance or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.PhpWorkloadResource]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.ProviderInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace_async
-    async def begin_create_or_update(
+    @distributed_trace
+    def begin_create(
         self,
         resource_group_name: str,
-        php_workload_name: str,
-        php_workload_resource: Union[_models.PhpWorkloadResource, IO],
+        monitor_name: str,
+        provider_instance_name: str,
+        provider_instance_parameter: Union[_models.ProviderInstance, IO],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.PhpWorkloadResource]:
-        """Create or updated PHP workload resource.
+    ) -> LROPoller[_models.ProviderInstance]:
+        """Creates a provider instance.
+
+        Creates a provider instance for the specified subscription, resource group, SAP monitor name,
+        and resource name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param php_workload_name: Php workload name. Required.
-        :type php_workload_name: str
-        :param php_workload_resource: Resource create or update request payload. Is either a model type
-         or a IO type. Required.
-        :type php_workload_resource: ~azure.mgmt.workloads.models.PhpWorkloadResource or IO
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
+        :param provider_instance_name: Name of the provider instance. Required.
+        :type provider_instance_name: str
+        :param provider_instance_parameter: Request body representing a provider instance. Is either a
+         model type or a IO type. Required.
+        :type provider_instance_parameter: ~azure.mgmt.workloads.models.ProviderInstance or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either PhpWorkloadResource or the result of
+        :return: An instance of LROPoller that returns either ProviderInstance or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.PhpWorkloadResource]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.ProviderInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.PhpWorkloadResource] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        cls: ClsType[_models.ProviderInstance] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_or_update_initial(
+            raw_result = self._create_initial(
                 resource_group_name=resource_group_name,
-                php_workload_name=php_workload_name,
-                php_workload_resource=php_workload_resource,
+                monitor_name=monitor_name,
+                provider_instance_name=provider_instance_name,
+                provider_instance_parameter=provider_instance_parameter,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("PhpWorkloadResource", pipeline_response)
+            deserialized = self._deserialize("ProviderInstance", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/phpWorkloads/{phpWorkloadName}"
-    }
-
-    @overload
-    async def update(
-        self,
-        resource_group_name: str,
-        php_workload_name: str,
-        resource_patch_request_body: _models.PatchResourceRequestBody,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> _models.PhpWorkloadResource:
-        """Update PHP workload resource.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param php_workload_name: Php workload name. Required.
-        :type php_workload_name: str
-        :param resource_patch_request_body: Workload resource update data. Required.
-        :type resource_patch_request_body: ~azure.mgmt.workloads.models.PatchResourceRequestBody
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: PhpWorkloadResource or the result of cls(response)
-        :rtype: ~azure.mgmt.workloads.models.PhpWorkloadResource
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-
-    @overload
-    async def update(
-        self,
-        resource_group_name: str,
-        php_workload_name: str,
-        resource_patch_request_body: IO,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> _models.PhpWorkloadResource:
-        """Update PHP workload resource.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param php_workload_name: Php workload name. Required.
-        :type php_workload_name: str
-        :param resource_patch_request_body: Workload resource update data. Required.
-        :type resource_patch_request_body: IO
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: PhpWorkloadResource or the result of cls(response)
-        :rtype: ~azure.mgmt.workloads.models.PhpWorkloadResource
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-
-    @distributed_trace_async
-    async def update(
-        self,
-        resource_group_name: str,
-        php_workload_name: str,
-        resource_patch_request_body: Union[_models.PatchResourceRequestBody, IO],
-        **kwargs: Any
-    ) -> _models.PhpWorkloadResource:
-        """Update PHP workload resource.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param php_workload_name: Php workload name. Required.
-        :type php_workload_name: str
-        :param resource_patch_request_body: Workload resource update data. Is either a model type or a
-         IO type. Required.
-        :type resource_patch_request_body: ~azure.mgmt.workloads.models.PatchResourceRequestBody or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: PhpWorkloadResource or the result of cls(response)
-        :rtype: ~azure.mgmt.workloads.models.PhpWorkloadResource
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.PhpWorkloadResource] = kwargs.pop("cls", None)
-
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(resource_patch_request_body, (IO, bytes)):
-            _content = resource_patch_request_body
-        else:
-            _json = self._serialize.body(resource_patch_request_body, "PatchResourceRequestBody")
-
-        request = build_update_request(
-            resource_group_name=resource_group_name,
-            php_workload_name=php_workload_name,
-            subscription_id=self._config.subscription_id,
-            api_version=api_version,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            template_url=self.update.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
-        )
-
-        response = pipeline_response.http_response
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        deserialized = self._deserialize("PhpWorkloadResource", pipeline_response)
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
-
-    update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/phpWorkloads/{phpWorkloadName}"
+    begin_create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
     }
 
-    async def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, php_workload_name: str, delete_infra: Optional[str] = None, **kwargs: Any
-    ) -> None:
+    def _delete_initial(
+        self, resource_group_name: str, monitor_name: str, provider_instance_name: str, **kwargs: Any
+    ) -> Optional[_models.OperationStatusResult]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
-        cls: ClsType[None] = kwargs.pop("cls", None)
+        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
-            php_workload_name=php_workload_name,
+            monitor_name=monitor_name,
+            provider_instance_name=provider_instance_name,
             subscription_id=self._config.subscription_id,
-            delete_infra=delete_infra,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
 
     _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/phpWorkloads/{phpWorkloadName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
     }
 
-    @distributed_trace_async
-    async def begin_delete(
-        self, resource_group_name: str, php_workload_name: str, delete_infra: Optional[str] = None, **kwargs: Any
-    ) -> AsyncLROPoller[None]:
-        """Delete PHP workload resource.
+    @distributed_trace
+    def begin_delete(
+        self, resource_group_name: str, monitor_name: str, provider_instance_name: str, **kwargs: Any
+    ) -> LROPoller[_models.OperationStatusResult]:
+        """Deletes a provider instance.
+
+        Deletes a provider instance for the specified subscription, resource group, SAP monitor name,
+        and resource name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param php_workload_name: Php workload name. Required.
-        :type php_workload_name: str
-        :param delete_infra: Whether to delete infra along with workload resource. Default value is
-         None.
-        :type delete_infra: str
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
+        :param provider_instance_name: Name of the provider instance. Required.
+        :type provider_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :return: An instance of LROPoller that returns either OperationStatusResult or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
-        cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._delete_initial(  # type: ignore
+            raw_result = self._delete_initial(
                 resource_group_name=resource_group_name,
-                php_workload_name=php_workload_name,
-                delete_infra=delete_infra,
+                monitor_name=monitor_name,
+                provider_instance_name=provider_instance_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
-        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/phpWorkloads/{phpWorkloadName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
     }
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_wordpress_instances_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_provider_instances_operations.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,89 +27,90 @@
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._wordpress_instances_operations import (
-    build_create_or_update_request,
+from ...operations._provider_instances_operations import (
+    build_create_request,
     build_delete_request,
     build_get_request,
     build_list_request,
 )
 from .._vendor import WorkloadsClientMixinABC
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
     from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class WordpressInstancesOperations:
+class ProviderInstancesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.workloads.aio.WorkloadsClient`'s
-        :attr:`wordpress_instances` attribute.
+        :attr:`provider_instances` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(
-        self, resource_group_name: str, php_workload_name: str, **kwargs: Any
-    ) -> AsyncIterable["_models.WordpressInstanceResource"]:
-        """Lists WordPress instance resources under a phpWorkload resource.
+        self, resource_group_name: str, monitor_name: str, **kwargs: Any
+    ) -> AsyncIterable["_models.ProviderInstance"]:
+        """Gets a list of provider instances in the specified SAP monitor.
+
+        Gets a list of provider instances in the specified SAP monitor. The operations returns various
+        properties of each provider instances.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param php_workload_name: Php workload name. Required.
-        :type php_workload_name: str
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either WordpressInstanceResource or the result of
-         cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.WordpressInstanceResource]
+        :return: An iterator like instance of either ProviderInstance or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.ProviderInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
-        cls: ClsType[_models.WordpressInstanceResourceList] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ProviderInstanceListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
                 request = build_list_request(
                     resource_group_name=resource_group_name,
-                    php_workload_name=php_workload_name,
+                    monitor_name=monitor_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
@@ -130,15 +131,15 @@
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("WordpressInstanceResourceList", pipeline_response)
+            deserialized = self._deserialize("ProviderInstanceListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
@@ -154,52 +155,58 @@
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
     list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/phpWorkloads/{phpWorkloadName}/wordpressInstances"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances"
     }
 
     @distributed_trace_async
     async def get(
-        self, resource_group_name: str, php_workload_name: str, **kwargs: Any
-    ) -> _models.WordpressInstanceResource:
-        """Gets the WordPress instance resource.
+        self, resource_group_name: str, monitor_name: str, provider_instance_name: str, **kwargs: Any
+    ) -> _models.ProviderInstance:
+        """Gets properties of a provider instance.
+
+        Gets properties of a provider instance for the specified subscription, resource group, SAP
+        monitor name, and resource name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param php_workload_name: Php workload name. Required.
-        :type php_workload_name: str
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
+        :param provider_instance_name: Name of the provider instance. Required.
+        :type provider_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: WordpressInstanceResource or the result of cls(response)
-        :rtype: ~azure.mgmt.workloads.models.WordpressInstanceResource
+        :return: ProviderInstance or the result of cls(response)
+        :rtype: ~azure.mgmt.workloads.models.ProviderInstance
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
-        cls: ClsType[_models.WordpressInstanceResource] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ProviderInstance] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
-            php_workload_name=php_workload_name,
+            monitor_name=monitor_name,
+            provider_instance_name=provider_instance_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
@@ -212,66 +219,68 @@
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("WordpressInstanceResource", pipeline_response)
+        deserialized = self._deserialize("ProviderInstance", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/phpWorkloads/{phpWorkloadName}/wordpressInstances/default"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
     }
 
-    async def _create_or_update_initial(
+    async def _create_initial(
         self,
         resource_group_name: str,
-        php_workload_name: str,
-        wordpress_instance_resource: Union[_models.WordpressInstanceResource, IO],
+        monitor_name: str,
+        provider_instance_name: str,
+        provider_instance_parameter: Union[_models.ProviderInstance, IO],
         **kwargs: Any
-    ) -> _models.WordpressInstanceResource:
+    ) -> _models.ProviderInstance:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.WordpressInstanceResource] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ProviderInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(wordpress_instance_resource, (IO, bytes)):
-            _content = wordpress_instance_resource
+        if isinstance(provider_instance_parameter, (IO, bytes)):
+            _content = provider_instance_parameter
         else:
-            _json = self._serialize.body(wordpress_instance_resource, "WordpressInstanceResource")
+            _json = self._serialize.body(provider_instance_parameter, "ProviderInstance")
 
-        request = build_create_or_update_request(
+        request = build_create_request(
             resource_group_name=resource_group_name,
-            php_workload_name=php_workload_name,
+            monitor_name=monitor_name,
+            provider_instance_name=provider_instance_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
+            template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
@@ -282,164 +291,180 @@
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
-            deserialized = self._deserialize("WordpressInstanceResource", pipeline_response)
+            deserialized = self._deserialize("ProviderInstance", pipeline_response)
 
         if response.status_code == 201:
-            deserialized = self._deserialize("WordpressInstanceResource", pipeline_response)
+            deserialized = self._deserialize("ProviderInstance", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/phpWorkloads/{phpWorkloadName}/wordpressInstances/default"
+    _create_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
     }
 
     @overload
-    async def begin_create_or_update(
+    async def begin_create(
         self,
         resource_group_name: str,
-        php_workload_name: str,
-        wordpress_instance_resource: _models.WordpressInstanceResource,
+        monitor_name: str,
+        provider_instance_name: str,
+        provider_instance_parameter: _models.ProviderInstance,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.WordpressInstanceResource]:
-        """Create or updated WordPress instance resource.
+    ) -> AsyncLROPoller[_models.ProviderInstance]:
+        """Creates a provider instance.
+
+        Creates a provider instance for the specified subscription, resource group, SAP monitor name,
+        and resource name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param php_workload_name: Php workload name. Required.
-        :type php_workload_name: str
-        :param wordpress_instance_resource: Resource create or update request payload. Required.
-        :type wordpress_instance_resource: ~azure.mgmt.workloads.models.WordpressInstanceResource
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
+        :param provider_instance_name: Name of the provider instance. Required.
+        :type provider_instance_name: str
+        :param provider_instance_parameter: Request body representing a provider instance. Required.
+        :type provider_instance_parameter: ~azure.mgmt.workloads.models.ProviderInstance
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either WordpressInstanceResource or the
-         result of cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.WordpressInstanceResource]
+        :return: An instance of AsyncLROPoller that returns either ProviderInstance or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.ProviderInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def begin_create_or_update(
+    async def begin_create(
         self,
         resource_group_name: str,
-        php_workload_name: str,
-        wordpress_instance_resource: IO,
+        monitor_name: str,
+        provider_instance_name: str,
+        provider_instance_parameter: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.WordpressInstanceResource]:
-        """Create or updated WordPress instance resource.
+    ) -> AsyncLROPoller[_models.ProviderInstance]:
+        """Creates a provider instance.
+
+        Creates a provider instance for the specified subscription, resource group, SAP monitor name,
+        and resource name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param php_workload_name: Php workload name. Required.
-        :type php_workload_name: str
-        :param wordpress_instance_resource: Resource create or update request payload. Required.
-        :type wordpress_instance_resource: IO
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
+        :param provider_instance_name: Name of the provider instance. Required.
+        :type provider_instance_name: str
+        :param provider_instance_parameter: Request body representing a provider instance. Required.
+        :type provider_instance_parameter: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either WordpressInstanceResource or the
-         result of cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.WordpressInstanceResource]
+        :return: An instance of AsyncLROPoller that returns either ProviderInstance or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.ProviderInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
-    async def begin_create_or_update(
+    async def begin_create(
         self,
         resource_group_name: str,
-        php_workload_name: str,
-        wordpress_instance_resource: Union[_models.WordpressInstanceResource, IO],
+        monitor_name: str,
+        provider_instance_name: str,
+        provider_instance_parameter: Union[_models.ProviderInstance, IO],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.WordpressInstanceResource]:
-        """Create or updated WordPress instance resource.
+    ) -> AsyncLROPoller[_models.ProviderInstance]:
+        """Creates a provider instance.
+
+        Creates a provider instance for the specified subscription, resource group, SAP monitor name,
+        and resource name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param php_workload_name: Php workload name. Required.
-        :type php_workload_name: str
-        :param wordpress_instance_resource: Resource create or update request payload. Is either a
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
+        :param provider_instance_name: Name of the provider instance. Required.
+        :type provider_instance_name: str
+        :param provider_instance_parameter: Request body representing a provider instance. Is either a
          model type or a IO type. Required.
-        :type wordpress_instance_resource: ~azure.mgmt.workloads.models.WordpressInstanceResource or IO
+        :type provider_instance_parameter: ~azure.mgmt.workloads.models.ProviderInstance or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either WordpressInstanceResource or the
-         result of cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.WordpressInstanceResource]
+        :return: An instance of AsyncLROPoller that returns either ProviderInstance or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.ProviderInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.WordpressInstanceResource] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ProviderInstance] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_or_update_initial(
+            raw_result = await self._create_initial(
                 resource_group_name=resource_group_name,
-                php_workload_name=php_workload_name,
-                wordpress_instance_resource=wordpress_instance_resource,
+                monitor_name=monitor_name,
+                provider_instance_name=provider_instance_name,
+                provider_instance_parameter=provider_instance_parameter,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("WordpressInstanceResource", pipeline_response)
+            deserialized = self._deserialize("ProviderInstance", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
@@ -454,72 +479,146 @@
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/phpWorkloads/{phpWorkloadName}/wordpressInstances/default"
+    begin_create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
     }
 
-    @distributed_trace_async
-    async def delete(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, php_workload_name: str, **kwargs: Any
-    ) -> None:
-        """Delete WordPress instance resource.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param php_workload_name: Php workload name. Required.
-        :type php_workload_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None or the result of cls(response)
-        :rtype: None
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
+    async def _delete_initial(
+        self, resource_group_name: str, monitor_name: str, provider_instance_name: str, **kwargs: Any
+    ) -> Optional[_models.OperationStatusResult]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
-        cls: ClsType[None] = kwargs.pop("cls", None)
+        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
-            php_workload_name=php_workload_name,
+            monitor_name=monitor_name,
+            provider_instance_name=provider_instance_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
+            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 204]:
+        if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
+    }
+
+    @distributed_trace_async
+    async def begin_delete(
+        self, resource_group_name: str, monitor_name: str, provider_instance_name: str, **kwargs: Any
+    ) -> AsyncLROPoller[_models.OperationStatusResult]:
+        """Deletes a provider instance.
+
+        Deletes a provider instance for the specified subscription, resource group, SAP monitor name,
+        and resource name.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
+        :param provider_instance_name: Name of the provider instance. Required.
+        :type provider_instance_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either OperationStatusResult or the result
+         of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._delete_initial(
+                resource_group_name=resource_group_name,
+                monitor_name=monitor_name,
+                provider_instance_name=provider_instance_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            )
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/phpWorkloads/{phpWorkloadName}/wordpressInstances/default"
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
     }
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_patch.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_workloads_client_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_workloads_client_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPSizingRecommendationResult] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -260,15 +260,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPSupportedResourceSkusResult] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -394,15 +394,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPDiskConfigurationsResult] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -532,15 +532,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPAvailabilityZoneDetailsResult] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_sap_application_server_instances_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_sap_application_server_instances_operations.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._sap_application_server_instances_operations import (
     build_create_request,
     build_delete_request,
     build_get_request,
     build_list_request,
+    build_start_instance_request,
+    build_stop_instance_request,
     build_update_request,
 )
 from .._vendor import WorkloadsClientMixinABC
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
@@ -95,15 +97,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPApplicationServerInstance] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -154,15 +156,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPApplicationServerInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -343,15 +345,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.SAPApplicationServerInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPApplicationServerInstance] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -413,15 +415,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPApplicationServerInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -599,15 +601,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.SAPApplicationServerInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPApplicationServerInstance] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -664,15 +666,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -738,15 +740,15 @@
          of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -809,15 +811,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.SAPApplicationServerInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPApplicationServerInstanceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -882,7 +884,393 @@
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
     list.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances"
     }
+
+    async def _start_instance_initial(
+        self, resource_group_name: str, sap_virtual_instance_name: str, application_instance_name: str, **kwargs: Any
+    ) -> Optional[_models.OperationStatusResult]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
+
+        request = build_start_instance_request(
+            resource_group_name=resource_group_name,
+            sap_virtual_instance_name=sap_virtual_instance_name,
+            application_instance_name=application_instance_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self._start_instance_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    _start_instance_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances/{applicationInstanceName}/start"
+    }
+
+    @distributed_trace_async
+    async def begin_start_instance(
+        self, resource_group_name: str, sap_virtual_instance_name: str, application_instance_name: str, **kwargs: Any
+    ) -> AsyncLROPoller[_models.OperationStatusResult]:
+        """Starts the SAP Application Server Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param application_instance_name: The name of SAP Application Server instance resource.
+         Required.
+        :type application_instance_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either OperationStatusResult or the result
+         of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._start_instance_initial(
+                resource_group_name=resource_group_name,
+                sap_virtual_instance_name=sap_virtual_instance_name,
+                application_instance_name=application_instance_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            )
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_start_instance.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances/{applicationInstanceName}/start"
+    }
+
+    async def _stop_instance_initial(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        application_instance_name: str,
+        body: Optional[Union[_models.StopRequest, IO]] = None,
+        **kwargs: Any
+    ) -> Optional[_models.OperationStatusResult]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IO, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "StopRequest")
+            else:
+                _json = None
+
+        request = build_stop_instance_request(
+            resource_group_name=resource_group_name,
+            sap_virtual_instance_name=sap_virtual_instance_name,
+            application_instance_name=application_instance_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self._stop_instance_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    _stop_instance_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances/{applicationInstanceName}/stop"
+    }
+
+    @overload
+    async def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        application_instance_name: str,
+        body: Optional[_models.StopRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.OperationStatusResult]:
+        """Stops the SAP Application Server Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param application_instance_name: The name of SAP Application Server instance resource.
+         Required.
+        :type application_instance_name: str
+        :param body: SAP Application server instance stop request body. Default value is None.
+        :type body: ~azure.mgmt.workloads.models.StopRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either OperationStatusResult or the result
+         of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        application_instance_name: str,
+        body: Optional[IO] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.OperationStatusResult]:
+        """Stops the SAP Application Server Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param application_instance_name: The name of SAP Application Server instance resource.
+         Required.
+        :type application_instance_name: str
+        :param body: SAP Application server instance stop request body. Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either OperationStatusResult or the result
+         of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        application_instance_name: str,
+        body: Optional[Union[_models.StopRequest, IO]] = None,
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.OperationStatusResult]:
+        """Stops the SAP Application Server Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param application_instance_name: The name of SAP Application Server instance resource.
+         Required.
+        :type application_instance_name: str
+        :param body: SAP Application server instance stop request body. Is either a model type or a IO
+         type. Default value is None.
+        :type body: ~azure.mgmt.workloads.models.StopRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either OperationStatusResult or the result
+         of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._stop_instance_initial(
+                resource_group_name=resource_group_name,
+                sap_virtual_instance_name=sap_virtual_instance_name,
+                application_instance_name=application_instance_name,
+                body=body,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            )
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_stop_instance.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances/{applicationInstanceName}/stop"
+    }
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_provider_instances_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_landscape_monitor_operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,622 +3,747 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import sys
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
-import urllib.parse
+from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
-from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
+from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
-from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._provider_instances_operations import (
-    build_create_request,
-    build_delete_request,
-    build_get_request,
-    build_list_request,
-)
-from .._vendor import WorkloadsClientMixinABC
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import WorkloadsClientMixinABC, _convert_request, _format_url_section
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
     from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_get_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/sapLandscapeMonitor/default",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_create_request(
+    resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/sapLandscapeMonitor/default",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_delete_request(
+    resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/sapLandscapeMonitor/default",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
-class ProviderInstancesOperations:
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_update_request(
+    resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/sapLandscapeMonitor/default",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/sapLandscapeMonitor",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+class SapLandscapeMonitorOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.workloads.aio.WorkloadsClient`'s
-        :attr:`provider_instances` attribute.
+        :class:`~azure.mgmt.workloads.WorkloadsClient`'s
+        :attr:`sap_landscape_monitor` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(
-        self, resource_group_name: str, monitor_name: str, **kwargs: Any
-    ) -> AsyncIterable["_models.ProviderInstance"]:
-        """Gets a list of provider instances in the specified SAP monitor.
-
-        Gets a list of provider instances in the specified SAP monitor. The operations returns various
-        properties of each provider instances.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param monitor_name: Name of the SAP monitor resource. Required.
-        :type monitor_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ProviderInstance or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.ProviderInstance]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.ProviderInstanceListResult] = kwargs.pop("cls", None)
-
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        def prepare_request(next_link=None):
-            if not next_link:
-
-                request = build_list_request(
-                    resource_group_name=resource_group_name,
-                    monitor_name=monitor_name,
-                    subscription_id=self._config.subscription_id,
-                    api_version=api_version,
-                    template_url=self.list.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
-
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("ProviderInstanceListResult", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
-
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
-
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
-            )
-            response = pipeline_response.http_response
-
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-            return pipeline_response
-
-        return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances"
-    }
-
-    @distributed_trace_async
-    async def get(
-        self, resource_group_name: str, monitor_name: str, provider_instance_name: str, **kwargs: Any
-    ) -> _models.ProviderInstance:
-        """Gets properties of a provider instance.
+    def get(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> _models.SapLandscapeMonitor:
+        """Gets configuration values for Single Pane Of Glass for SAP monitor.
 
-        Gets properties of a provider instance for the specified subscription, resource group, SAP
-        monitor name, and resource name.
+        Gets configuration values for Single Pane Of Glass for SAP monitor for the specified
+        subscription, resource group, and resource name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param monitor_name: Name of the SAP monitor resource. Required.
         :type monitor_name: str
-        :param provider_instance_name: Name of the provider instance. Required.
-        :type provider_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: ProviderInstance or the result of cls(response)
-        :rtype: ~azure.mgmt.workloads.models.ProviderInstance
+        :return: SapLandscapeMonitor or the result of cls(response)
+        :rtype: ~azure.mgmt.workloads.models.SapLandscapeMonitor
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
-        cls: ClsType[_models.ProviderInstance] = kwargs.pop("cls", None)
+        cls: ClsType[_models.SapLandscapeMonitor] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
-            provider_instance_name=provider_instance_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("ProviderInstance", pipeline_response)
+        deserialized = self._deserialize("SapLandscapeMonitor", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/sapLandscapeMonitor/default"
     }
 
-    async def _create_initial(
+    @overload
+    def create(
         self,
         resource_group_name: str,
         monitor_name: str,
-        provider_instance_name: str,
-        provider_instance_parameter: Union[_models.ProviderInstance, IO],
+        sap_landscape_monitor_parameter: _models.SapLandscapeMonitor,
+        *,
+        content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.ProviderInstance:
+    ) -> _models.SapLandscapeMonitor:
+        """Creates a SAP Landscape Monitor Dashboard.
+
+        Creates a SAP Landscape Monitor Dashboard for the specified subscription, resource group, and
+        resource name.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
+        :param sap_landscape_monitor_parameter: Request body representing a configuration for Sap
+         Landscape Monitor Dashboard. Required.
+        :type sap_landscape_monitor_parameter: ~azure.mgmt.workloads.models.SapLandscapeMonitor
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: SapLandscapeMonitor or the result of cls(response)
+        :rtype: ~azure.mgmt.workloads.models.SapLandscapeMonitor
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def create(
+        self,
+        resource_group_name: str,
+        monitor_name: str,
+        sap_landscape_monitor_parameter: IO,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.SapLandscapeMonitor:
+        """Creates a SAP Landscape Monitor Dashboard.
+
+        Creates a SAP Landscape Monitor Dashboard for the specified subscription, resource group, and
+        resource name.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
+        :param sap_landscape_monitor_parameter: Request body representing a configuration for Sap
+         Landscape Monitor Dashboard. Required.
+        :type sap_landscape_monitor_parameter: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: SapLandscapeMonitor or the result of cls(response)
+        :rtype: ~azure.mgmt.workloads.models.SapLandscapeMonitor
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def create(
+        self,
+        resource_group_name: str,
+        monitor_name: str,
+        sap_landscape_monitor_parameter: Union[_models.SapLandscapeMonitor, IO],
+        **kwargs: Any
+    ) -> _models.SapLandscapeMonitor:
+        """Creates a SAP Landscape Monitor Dashboard.
+
+        Creates a SAP Landscape Monitor Dashboard for the specified subscription, resource group, and
+        resource name.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
+        :param sap_landscape_monitor_parameter: Request body representing a configuration for Sap
+         Landscape Monitor Dashboard. Is either a model type or a IO type. Required.
+        :type sap_landscape_monitor_parameter: ~azure.mgmt.workloads.models.SapLandscapeMonitor or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: SapLandscapeMonitor or the result of cls(response)
+        :rtype: ~azure.mgmt.workloads.models.SapLandscapeMonitor
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.ProviderInstance] = kwargs.pop("cls", None)
+        cls: ClsType[_models.SapLandscapeMonitor] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(provider_instance_parameter, (IO, bytes)):
-            _content = provider_instance_parameter
+        if isinstance(sap_landscape_monitor_parameter, (IO, bytes)):
+            _content = sap_landscape_monitor_parameter
         else:
-            _json = self._serialize.body(provider_instance_parameter, "ProviderInstance")
+            _json = self._serialize.body(sap_landscape_monitor_parameter, "SapLandscapeMonitor")
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
-            provider_instance_name=provider_instance_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_initial.metadata["url"],
+            template_url=self.create.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
-            deserialized = self._deserialize("ProviderInstance", pipeline_response)
+            deserialized = self._deserialize("SapLandscapeMonitor", pipeline_response)
 
         if response.status_code == 201:
-            deserialized = self._deserialize("ProviderInstance", pipeline_response)
+            deserialized = self._deserialize("SapLandscapeMonitor", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
+    create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/sapLandscapeMonitor/default"
+    }
+
+    @distributed_trace
+    def delete(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, monitor_name: str, **kwargs: Any
+    ) -> None:
+        """Deletes a SAP Landscape Monitor Dashboard.
+
+        Deletes a SAP Landscape Monitor Dashboard with the specified subscription, resource group, and
+        SAP monitor name.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param monitor_name: Name of the SAP monitor resource. Required.
+        :type monitor_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: None or the result of cls(response)
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        request = build_delete_request(
+            resource_group_name=resource_group_name,
+            monitor_name=monitor_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.delete.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/sapLandscapeMonitor/default"
     }
 
     @overload
-    async def begin_create(
+    def update(
         self,
         resource_group_name: str,
         monitor_name: str,
-        provider_instance_name: str,
-        provider_instance_parameter: _models.ProviderInstance,
+        sap_landscape_monitor_parameter: _models.SapLandscapeMonitor,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.ProviderInstance]:
-        """Creates a provider instance.
+    ) -> _models.SapLandscapeMonitor:
+        """Patches the SAP Landscape Monitor Dashboard.
 
-        Creates a provider instance for the specified subscription, resource group, SAP monitor name,
-        and resource name.
+        Patches the SAP Landscape Monitor Dashboard for the specified subscription, resource group, and
+        SAP monitor name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param monitor_name: Name of the SAP monitor resource. Required.
         :type monitor_name: str
-        :param provider_instance_name: Name of the provider instance. Required.
-        :type provider_instance_name: str
-        :param provider_instance_parameter: Request body representing a provider instance. Required.
-        :type provider_instance_parameter: ~azure.mgmt.workloads.models.ProviderInstance
+        :param sap_landscape_monitor_parameter: Request body representing a configuration for Sap
+         Landscape Monitor Dashboard. Required.
+        :type sap_landscape_monitor_parameter: ~azure.mgmt.workloads.models.SapLandscapeMonitor
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either ProviderInstance or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.ProviderInstance]
+        :return: SapLandscapeMonitor or the result of cls(response)
+        :rtype: ~azure.mgmt.workloads.models.SapLandscapeMonitor
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def begin_create(
+    def update(
         self,
         resource_group_name: str,
         monitor_name: str,
-        provider_instance_name: str,
-        provider_instance_parameter: IO,
+        sap_landscape_monitor_parameter: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.ProviderInstance]:
-        """Creates a provider instance.
+    ) -> _models.SapLandscapeMonitor:
+        """Patches the SAP Landscape Monitor Dashboard.
 
-        Creates a provider instance for the specified subscription, resource group, SAP monitor name,
-        and resource name.
+        Patches the SAP Landscape Monitor Dashboard for the specified subscription, resource group, and
+        SAP monitor name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param monitor_name: Name of the SAP monitor resource. Required.
         :type monitor_name: str
-        :param provider_instance_name: Name of the provider instance. Required.
-        :type provider_instance_name: str
-        :param provider_instance_parameter: Request body representing a provider instance. Required.
-        :type provider_instance_parameter: IO
+        :param sap_landscape_monitor_parameter: Request body representing a configuration for Sap
+         Landscape Monitor Dashboard. Required.
+        :type sap_landscape_monitor_parameter: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either ProviderInstance or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.ProviderInstance]
+        :return: SapLandscapeMonitor or the result of cls(response)
+        :rtype: ~azure.mgmt.workloads.models.SapLandscapeMonitor
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace_async
-    async def begin_create(
+    @distributed_trace
+    def update(
         self,
         resource_group_name: str,
         monitor_name: str,
-        provider_instance_name: str,
-        provider_instance_parameter: Union[_models.ProviderInstance, IO],
+        sap_landscape_monitor_parameter: Union[_models.SapLandscapeMonitor, IO],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.ProviderInstance]:
-        """Creates a provider instance.
+    ) -> _models.SapLandscapeMonitor:
+        """Patches the SAP Landscape Monitor Dashboard.
 
-        Creates a provider instance for the specified subscription, resource group, SAP monitor name,
-        and resource name.
+        Patches the SAP Landscape Monitor Dashboard for the specified subscription, resource group, and
+        SAP monitor name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param monitor_name: Name of the SAP monitor resource. Required.
         :type monitor_name: str
-        :param provider_instance_name: Name of the provider instance. Required.
-        :type provider_instance_name: str
-        :param provider_instance_parameter: Request body representing a provider instance. Is either a
-         model type or a IO type. Required.
-        :type provider_instance_parameter: ~azure.mgmt.workloads.models.ProviderInstance or IO
+        :param sap_landscape_monitor_parameter: Request body representing a configuration for Sap
+         Landscape Monitor Dashboard. Is either a model type or a IO type. Required.
+        :type sap_landscape_monitor_parameter: ~azure.mgmt.workloads.models.SapLandscapeMonitor or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either ProviderInstance or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.ProviderInstance]
+        :return: SapLandscapeMonitor or the result of cls(response)
+        :rtype: ~azure.mgmt.workloads.models.SapLandscapeMonitor
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.ProviderInstance] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
-        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
-        if cont_token is None:
-            raw_result = await self._create_initial(
-                resource_group_name=resource_group_name,
-                monitor_name=monitor_name,
-                provider_instance_name=provider_instance_name,
-                provider_instance_parameter=provider_instance_parameter,
-                api_version=api_version,
-                content_type=content_type,
-                cls=lambda x, y, z: x,
-                headers=_headers,
-                params=_params,
-                **kwargs
-            )
-        kwargs.pop("error_map", None)
-
-        def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("ProviderInstance", pipeline_response)
-            if cls:
-                return cls(pipeline_response, deserialized, {})
-            return deserialized
-
-        if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
-            )
-        elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
-        else:
-            polling_method = polling
-        if cont_token:
-            return AsyncLROPoller.from_continuation_token(
-                polling_method=polling_method,
-                continuation_token=cont_token,
-                client=self._client,
-                deserialization_callback=get_long_running_output,
-            )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
-    }
-
-    async def _delete_initial(
-        self, resource_group_name: str, monitor_name: str, provider_instance_name: str, **kwargs: Any
-    ) -> Optional[_models.OperationStatusResult]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = kwargs.pop("headers", {}) or {}
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
-        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.SapLandscapeMonitor] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(sap_landscape_monitor_parameter, (IO, bytes)):
+            _content = sap_landscape_monitor_parameter
+        else:
+            _json = self._serialize.body(sap_landscape_monitor_parameter, "SapLandscapeMonitor")
+
+        request = build_update_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
-            provider_instance_name=provider_instance_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202, 204]:
+        if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = None
-        if response.status_code == 200:
-            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+        deserialized = self._deserialize("SapLandscapeMonitor", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
+    update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/sapLandscapeMonitor/default"
     }
 
-    @distributed_trace_async
-    async def begin_delete(
-        self, resource_group_name: str, monitor_name: str, provider_instance_name: str, **kwargs: Any
-    ) -> AsyncLROPoller[_models.OperationStatusResult]:
-        """Deletes a provider instance.
+    @distributed_trace
+    def list(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> _models.SapLandscapeMonitorListResult:
+        """Gets configuration values for Single Pane Of Glass for SAP monitor.
 
-        Deletes a provider instance for the specified subscription, resource group, SAP monitor name,
-        and resource name.
+        Gets configuration values for Single Pane Of Glass for SAP monitor for the specified
+        subscription, resource group, and resource name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param monitor_name: Name of the SAP monitor resource. Required.
         :type monitor_name: str
-        :param provider_instance_name: Name of the provider instance. Required.
-        :type provider_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either OperationStatusResult or the result
-         of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :return: SapLandscapeMonitorListResult or the result of cls(response)
+        :rtype: ~azure.mgmt.workloads.models.SapLandscapeMonitorListResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
-        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
-        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
-        if cont_token is None:
-            raw_result = await self._delete_initial(
-                resource_group_name=resource_group_name,
-                monitor_name=monitor_name,
-                provider_instance_name=provider_instance_name,
-                api_version=api_version,
-                cls=lambda x, y, z: x,
-                headers=_headers,
-                params=_params,
-                **kwargs
-            )
-        kwargs.pop("error_map", None)
-
-        def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
-            if cls:
-                return cls(pipeline_response, deserialized, {})
-            return deserialized
-
-        if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
-            )
-        elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
-        else:
-            polling_method = polling
-        if cont_token:
-            return AsyncLROPoller.from_continuation_token(
-                polling_method=polling_method,
-                continuation_token=cont_token,
-                client=self._client,
-                deserialization_callback=get_long_running_output,
-            )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+        cls: ClsType[_models.SapLandscapeMonitorListResult] = kwargs.pop("cls", None)
+
+        request = build_list_request(
+            resource_group_name=resource_group_name,
+            monitor_name=monitor_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.list.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/providerInstances/{providerInstanceName}"
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize("SapLandscapeMonitorListResult", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}/sapLandscapeMonitor"
     }
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/aio/operations/_sap_central_instances_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_sap_central_instances_operations.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._sap_central_instances_operations import (
     build_create_request,
     build_delete_request,
     build_get_request,
     build_list_request,
+    build_start_instance_request,
+    build_stop_instance_request,
     build_update_request,
 )
 from .._vendor import WorkloadsClientMixinABC
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
@@ -94,15 +96,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPCentralServerInstance] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -153,15 +155,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPCentralServerInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -342,15 +344,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.SAPCentralServerInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPCentralServerInstance] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -412,15 +414,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPCentralServerInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -601,15 +603,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.SAPCentralServerInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPCentralServerInstance] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -666,15 +668,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -742,15 +744,15 @@
          of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -813,15 +815,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.workloads.models.SAPCentralServerInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPCentralInstanceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -886,7 +888,393 @@
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
     list.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances"
     }
+
+    async def _start_instance_initial(
+        self, resource_group_name: str, sap_virtual_instance_name: str, central_instance_name: str, **kwargs: Any
+    ) -> Optional[_models.OperationStatusResult]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
+
+        request = build_start_instance_request(
+            resource_group_name=resource_group_name,
+            sap_virtual_instance_name=sap_virtual_instance_name,
+            central_instance_name=central_instance_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self._start_instance_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    _start_instance_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances/{centralInstanceName}/start"
+    }
+
+    @distributed_trace_async
+    async def begin_start_instance(
+        self, resource_group_name: str, sap_virtual_instance_name: str, central_instance_name: str, **kwargs: Any
+    ) -> AsyncLROPoller[_models.OperationStatusResult]:
+        """Starts the SAP Central Services Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param central_instance_name: Central Services Instance resource name string modeled as
+         parameter for auto generation to work correctly. Required.
+        :type central_instance_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either OperationStatusResult or the result
+         of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._start_instance_initial(
+                resource_group_name=resource_group_name,
+                sap_virtual_instance_name=sap_virtual_instance_name,
+                central_instance_name=central_instance_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            )
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_start_instance.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances/{centralInstanceName}/start"
+    }
+
+    async def _stop_instance_initial(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        central_instance_name: str,
+        body: Optional[Union[_models.StopRequest, IO]] = None,
+        **kwargs: Any
+    ) -> Optional[_models.OperationStatusResult]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IO, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "StopRequest")
+            else:
+                _json = None
+
+        request = build_stop_instance_request(
+            resource_group_name=resource_group_name,
+            sap_virtual_instance_name=sap_virtual_instance_name,
+            central_instance_name=central_instance_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self._stop_instance_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    _stop_instance_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances/{centralInstanceName}/stop"
+    }
+
+    @overload
+    async def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        central_instance_name: str,
+        body: Optional[_models.StopRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.OperationStatusResult]:
+        """Stops the SAP Central Services Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param central_instance_name: Central Services Instance resource name string modeled as
+         parameter for auto generation to work correctly. Required.
+        :type central_instance_name: str
+        :param body: SAP Central Services instance stop request body. Default value is None.
+        :type body: ~azure.mgmt.workloads.models.StopRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either OperationStatusResult or the result
+         of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        central_instance_name: str,
+        body: Optional[IO] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.OperationStatusResult]:
+        """Stops the SAP Central Services Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param central_instance_name: Central Services Instance resource name string modeled as
+         parameter for auto generation to work correctly. Required.
+        :type central_instance_name: str
+        :param body: SAP Central Services instance stop request body. Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either OperationStatusResult or the result
+         of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        central_instance_name: str,
+        body: Optional[Union[_models.StopRequest, IO]] = None,
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.OperationStatusResult]:
+        """Stops the SAP Central Services Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param central_instance_name: Central Services Instance resource name string modeled as
+         parameter for auto generation to work correctly. Required.
+        :type central_instance_name: str
+        :param body: SAP Central Services instance stop request body. Is either a model type or a IO
+         type. Default value is None.
+        :type body: ~azure.mgmt.workloads.models.StopRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either OperationStatusResult or the result
+         of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._stop_instance_initial(
+                resource_group_name=resource_group_name,
+                sap_virtual_instance_name=sap_virtual_instance_name,
+                central_instance_name=central_instance_name,
+                body=body,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            )
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_stop_instance.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances/{centralInstanceName}/stop"
+    }
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/models/__init__.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,81 +3,80 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._models_py3 import ApplicationServerConfiguration
-from ._models_py3 import BackupProfile
-from ._models_py3 import CacheProfile
+from ._models_py3 import ApplicationServerFullResourceNames
+from ._models_py3 import ApplicationServerVmDetails
 from ._models_py3 import CentralServerConfiguration
+from ._models_py3 import CentralServerFullResourceNames
 from ._models_py3 import CentralServerVmDetails
+from ._models_py3 import CreateAndMountFileShareConfiguration
 from ._models_py3 import DB2ProviderInstanceProperties
 from ._models_py3 import DatabaseConfiguration
-from ._models_py3 import DatabaseProfile
+from ._models_py3 import DatabaseServerFullResourceNames
 from ._models_py3 import DatabaseVmDetails
 from ._models_py3 import DeployerVmPackages
 from ._models_py3 import DeploymentConfiguration
 from ._models_py3 import DeploymentWithOSConfiguration
 from ._models_py3 import DiscoveryConfiguration
-from ._models_py3 import DiskInfo
+from ._models_py3 import DiskConfiguration
+from ._models_py3 import DiskDetails
+from ._models_py3 import DiskSku
+from ._models_py3 import DiskVolumeConfiguration
 from ._models_py3 import EnqueueReplicationServerProperties
 from ._models_py3 import EnqueueServerProperties
 from ._models_py3 import Error
 from ._models_py3 import ErrorAdditionalInfo
 from ._models_py3 import ErrorDefinition
 from ._models_py3 import ErrorDetail
 from ._models_py3 import ErrorInnerError
 from ._models_py3 import ErrorResponse
 from ._models_py3 import ExternalInstallationSoftwareConfiguration
-from ._models_py3 import FileshareProfile
+from ._models_py3 import FileShareConfiguration
 from ._models_py3 import GatewayServerProperties
 from ._models_py3 import HanaDbProviderInstanceProperties
 from ._models_py3 import HighAvailabilityConfiguration
 from ._models_py3 import HighAvailabilitySoftwareConfiguration
 from ._models_py3 import ImageReference
 from ._models_py3 import InfrastructureConfiguration
 from ._models_py3 import LinuxConfiguration
+from ._models_py3 import LoadBalancerDetails
+from ._models_py3 import LoadBalancerResourceNames
 from ._models_py3 import ManagedRGConfiguration
 from ._models_py3 import MessageServerProperties
 from ._models_py3 import Monitor
 from ._models_py3 import MonitorListResult
 from ._models_py3 import MonitorPropertiesErrors
+from ._models_py3 import MountFileShareConfiguration
 from ._models_py3 import MsSqlServerProviderInstanceProperties
 from ._models_py3 import NetworkConfiguration
-from ._models_py3 import NetworkProfile
-from ._models_py3 import NodeProfile
+from ._models_py3 import NetworkInterfaceResourceNames
 from ._models_py3 import OSConfiguration
 from ._models_py3 import OSProfile
 from ._models_py3 import Operation
 from ._models_py3 import OperationDisplay
 from ._models_py3 import OperationListResult
 from ._models_py3 import OperationStatusResult
 from ._models_py3 import OperationsContent
 from ._models_py3 import OperationsDefinition
 from ._models_py3 import OperationsDefinitionArrayResponseWithContinuation
 from ._models_py3 import OperationsDefinitionDisplay
 from ._models_py3 import OperationsDisplayDefinition
-from ._models_py3 import OsImageProfile
 from ._models_py3 import OsSapConfiguration
-from ._models_py3 import PatchResourceRequestBody
-from ._models_py3 import PatchResourceRequestBodyIdentity
-from ._models_py3 import PhpProfile
-from ._models_py3 import PhpWorkloadResource
-from ._models_py3 import PhpWorkloadResourceIdentity
-from ._models_py3 import PhpWorkloadResourceList
 from ._models_py3 import PrometheusHaClusterProviderInstanceProperties
 from ._models_py3 import PrometheusOSProviderInstanceProperties
 from ._models_py3 import ProviderInstance
 from ._models_py3 import ProviderInstanceListResult
 from ._models_py3 import ProviderInstancePropertiesErrors
 from ._models_py3 import ProviderSpecificProperties
 from ._models_py3 import ProxyResource
 from ._models_py3 import Resource
-from ._models_py3 import RestrictionInfo
 from ._models_py3 import SAPApplicationServerInstance
 from ._models_py3 import SAPApplicationServerInstanceList
 from ._models_py3 import SAPAvailabilityZoneDetailsRequest
 from ._models_py3 import SAPAvailabilityZoneDetailsResult
 from ._models_py3 import SAPAvailabilityZonePair
 from ._models_py3 import SAPCentralInstanceList
 from ._models_py3 import SAPCentralServerInstance
@@ -92,176 +91,153 @@
 from ._models_py3 import SAPSizingRecommendationResult
 from ._models_py3 import SAPSupportedResourceSkusResult
 from ._models_py3 import SAPSupportedSku
 from ._models_py3 import SAPSupportedSkusRequest
 from ._models_py3 import SAPVirtualInstance
 from ._models_py3 import SAPVirtualInstanceError
 from ._models_py3 import SAPVirtualInstanceList
+from ._models_py3 import SapLandscapeMonitor
+from ._models_py3 import SapLandscapeMonitorListResult
+from ._models_py3 import SapLandscapeMonitorMetricThresholds
+from ._models_py3 import SapLandscapeMonitorPropertiesGrouping
+from ._models_py3 import SapLandscapeMonitorSidMapping
 from ._models_py3 import SapNetWeaverProviderInstanceProperties
-from ._models_py3 import SearchProfile
 from ._models_py3 import ServiceInitiatedSoftwareConfiguration
+from ._models_py3 import SharedStorageResourceNames
 from ._models_py3 import SingleServerConfiguration
+from ._models_py3 import SingleServerCustomResourceNames
+from ._models_py3 import SingleServerFullResourceNames
 from ._models_py3 import SingleServerRecommendationResult
-from ._models_py3 import SiteProfile
-from ._models_py3 import Sku
-from ._models_py3 import SkuCapability
-from ._models_py3 import SkuCapacity
-from ._models_py3 import SkuCost
-from ._models_py3 import SkuDefinition
-from ._models_py3 import SkuLocationAndZones
-from ._models_py3 import SkuRestriction
-from ._models_py3 import SkuZoneDetail
-from ._models_py3 import SkusListResult
+from ._models_py3 import SkipFileShareConfiguration
 from ._models_py3 import SoftwareConfiguration
 from ._models_py3 import SshConfiguration
 from ._models_py3 import SshKeyPair
 from ._models_py3 import SshPublicKey
 from ._models_py3 import StopRequest
+from ._models_py3 import StorageConfiguration
+from ._models_py3 import StorageInformation
 from ._models_py3 import SystemData
 from ._models_py3 import Tags
 from ._models_py3 import ThreeTierConfiguration
+from ._models_py3 import ThreeTierCustomResourceNames
+from ._models_py3 import ThreeTierFullResourceNames
 from ._models_py3 import ThreeTierRecommendationResult
 from ._models_py3 import TrackedResource
 from ._models_py3 import UpdateMonitorRequest
 from ._models_py3 import UpdateSAPApplicationInstanceRequest
 from ._models_py3 import UpdateSAPCentralInstanceRequest
 from ._models_py3 import UpdateSAPDatabaseInstanceRequest
 from ._models_py3 import UpdateSAPVirtualInstanceRequest
 from ._models_py3 import UserAssignedIdentity
 from ._models_py3 import UserAssignedServiceIdentity
-from ._models_py3 import UserProfile
 from ._models_py3 import VirtualMachineConfiguration
-from ._models_py3 import VmssNodesProfile
+from ._models_py3 import VirtualMachineResourceNames
 from ._models_py3 import WindowsConfiguration
-from ._models_py3 import WordpressInstanceResource
-from ._models_py3 import WordpressInstanceResourceList
 
 from ._workloads_client_enums import ActionType
-from ._workloads_client_enums import ApplicationProvisioningState
-from ._workloads_client_enums import AzureFrontDoorEnabled
+from ._workloads_client_enums import ApplicationServerVirtualMachineType
 from ._workloads_client_enums import CentralServerVirtualMachineType
+from ._workloads_client_enums import ConfigurationType
 from ._workloads_client_enums import CreatedByType
-from ._workloads_client_enums import DatabaseTier
-from ._workloads_client_enums import DatabaseType
-from ._workloads_client_enums import DiskStorageType
-from ._workloads_client_enums import EnableBackup
-from ._workloads_client_enums import EnableSslEnforcement
+from ._workloads_client_enums import DiskSkuName
 from ._workloads_client_enums import EnqueueReplicationServerType
-from ._workloads_client_enums import FileShareStorageType
-from ._workloads_client_enums import FileShareType
-from ._workloads_client_enums import HAEnabled
-from ._workloads_client_enums import LoadBalancerType
-from ._workloads_client_enums import LocationType
 from ._workloads_client_enums import ManagedServiceIdentityType
-from ._workloads_client_enums import OSImageOffer
-from ._workloads_client_enums import OSImagePublisher
-from ._workloads_client_enums import OSImageSku
-from ._workloads_client_enums import OSImageVersion
+from ._workloads_client_enums import NamingPatternType
 from ._workloads_client_enums import OSType
 from ._workloads_client_enums import OperationProperties
 from ._workloads_client_enums import Origin
-from ._workloads_client_enums import PHPVersion
-from ._workloads_client_enums import PhpWorkloadProvisioningState
-from ._workloads_client_enums import RedisCacheFamily
 from ._workloads_client_enums import RoutingPreference
 from ._workloads_client_enums import SAPConfigurationType
 from ._workloads_client_enums import SAPDatabaseScaleMethod
 from ._workloads_client_enums import SAPDatabaseType
 from ._workloads_client_enums import SAPDeploymentType
 from ._workloads_client_enums import SAPEnvironmentType
 from ._workloads_client_enums import SAPHealthState
 from ._workloads_client_enums import SAPHighAvailabilityType
 from ._workloads_client_enums import SAPProductType
 from ._workloads_client_enums import SAPSoftwareInstallationType
 from ._workloads_client_enums import SAPVirtualInstanceState
 from ._workloads_client_enums import SAPVirtualInstanceStatus
+from ._workloads_client_enums import SapLandscapeMonitorProvisioningState
 from ._workloads_client_enums import SapVirtualInstanceProvisioningState
-from ._workloads_client_enums import SearchType
-from ._workloads_client_enums import SkuRestrictionReasonCode
-from ._workloads_client_enums import SkuRestrictionType
-from ._workloads_client_enums import SkuScaleType
-from ._workloads_client_enums import SkuTier
 from ._workloads_client_enums import SslPreference
-from ._workloads_client_enums import WordpressVersions
-from ._workloads_client_enums import WorkloadKind
 from ._workloads_client_enums import WorkloadMonitorActionType
 from ._workloads_client_enums import WorkloadMonitorProvisioningState
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "ApplicationServerConfiguration",
-    "BackupProfile",
-    "CacheProfile",
+    "ApplicationServerFullResourceNames",
+    "ApplicationServerVmDetails",
     "CentralServerConfiguration",
+    "CentralServerFullResourceNames",
     "CentralServerVmDetails",
+    "CreateAndMountFileShareConfiguration",
     "DB2ProviderInstanceProperties",
     "DatabaseConfiguration",
-    "DatabaseProfile",
+    "DatabaseServerFullResourceNames",
     "DatabaseVmDetails",
     "DeployerVmPackages",
     "DeploymentConfiguration",
     "DeploymentWithOSConfiguration",
     "DiscoveryConfiguration",
-    "DiskInfo",
+    "DiskConfiguration",
+    "DiskDetails",
+    "DiskSku",
+    "DiskVolumeConfiguration",
     "EnqueueReplicationServerProperties",
     "EnqueueServerProperties",
     "Error",
     "ErrorAdditionalInfo",
     "ErrorDefinition",
     "ErrorDetail",
     "ErrorInnerError",
     "ErrorResponse",
     "ExternalInstallationSoftwareConfiguration",
-    "FileshareProfile",
+    "FileShareConfiguration",
     "GatewayServerProperties",
     "HanaDbProviderInstanceProperties",
     "HighAvailabilityConfiguration",
     "HighAvailabilitySoftwareConfiguration",
     "ImageReference",
     "InfrastructureConfiguration",
     "LinuxConfiguration",
+    "LoadBalancerDetails",
+    "LoadBalancerResourceNames",
     "ManagedRGConfiguration",
     "MessageServerProperties",
     "Monitor",
     "MonitorListResult",
     "MonitorPropertiesErrors",
+    "MountFileShareConfiguration",
     "MsSqlServerProviderInstanceProperties",
     "NetworkConfiguration",
-    "NetworkProfile",
-    "NodeProfile",
+    "NetworkInterfaceResourceNames",
     "OSConfiguration",
     "OSProfile",
     "Operation",
     "OperationDisplay",
     "OperationListResult",
     "OperationStatusResult",
     "OperationsContent",
     "OperationsDefinition",
     "OperationsDefinitionArrayResponseWithContinuation",
     "OperationsDefinitionDisplay",
     "OperationsDisplayDefinition",
-    "OsImageProfile",
     "OsSapConfiguration",
-    "PatchResourceRequestBody",
-    "PatchResourceRequestBodyIdentity",
-    "PhpProfile",
-    "PhpWorkloadResource",
-    "PhpWorkloadResourceIdentity",
-    "PhpWorkloadResourceList",
     "PrometheusHaClusterProviderInstanceProperties",
     "PrometheusOSProviderInstanceProperties",
     "ProviderInstance",
     "ProviderInstanceListResult",
     "ProviderInstancePropertiesErrors",
     "ProviderSpecificProperties",
     "ProxyResource",
     "Resource",
-    "RestrictionInfo",
     "SAPApplicationServerInstance",
     "SAPApplicationServerInstanceList",
     "SAPAvailabilityZoneDetailsRequest",
     "SAPAvailabilityZoneDetailsResult",
     "SAPAvailabilityZonePair",
     "SAPCentralInstanceList",
     "SAPCentralServerInstance",
@@ -276,98 +252,76 @@
     "SAPSizingRecommendationResult",
     "SAPSupportedResourceSkusResult",
     "SAPSupportedSku",
     "SAPSupportedSkusRequest",
     "SAPVirtualInstance",
     "SAPVirtualInstanceError",
     "SAPVirtualInstanceList",
+    "SapLandscapeMonitor",
+    "SapLandscapeMonitorListResult",
+    "SapLandscapeMonitorMetricThresholds",
+    "SapLandscapeMonitorPropertiesGrouping",
+    "SapLandscapeMonitorSidMapping",
     "SapNetWeaverProviderInstanceProperties",
-    "SearchProfile",
     "ServiceInitiatedSoftwareConfiguration",
+    "SharedStorageResourceNames",
     "SingleServerConfiguration",
+    "SingleServerCustomResourceNames",
+    "SingleServerFullResourceNames",
     "SingleServerRecommendationResult",
-    "SiteProfile",
-    "Sku",
-    "SkuCapability",
-    "SkuCapacity",
-    "SkuCost",
-    "SkuDefinition",
-    "SkuLocationAndZones",
-    "SkuRestriction",
-    "SkuZoneDetail",
-    "SkusListResult",
+    "SkipFileShareConfiguration",
     "SoftwareConfiguration",
     "SshConfiguration",
     "SshKeyPair",
     "SshPublicKey",
     "StopRequest",
+    "StorageConfiguration",
+    "StorageInformation",
     "SystemData",
     "Tags",
     "ThreeTierConfiguration",
+    "ThreeTierCustomResourceNames",
+    "ThreeTierFullResourceNames",
     "ThreeTierRecommendationResult",
     "TrackedResource",
     "UpdateMonitorRequest",
     "UpdateSAPApplicationInstanceRequest",
     "UpdateSAPCentralInstanceRequest",
     "UpdateSAPDatabaseInstanceRequest",
     "UpdateSAPVirtualInstanceRequest",
     "UserAssignedIdentity",
     "UserAssignedServiceIdentity",
-    "UserProfile",
     "VirtualMachineConfiguration",
-    "VmssNodesProfile",
+    "VirtualMachineResourceNames",
     "WindowsConfiguration",
-    "WordpressInstanceResource",
-    "WordpressInstanceResourceList",
     "ActionType",
-    "ApplicationProvisioningState",
-    "AzureFrontDoorEnabled",
+    "ApplicationServerVirtualMachineType",
     "CentralServerVirtualMachineType",
+    "ConfigurationType",
     "CreatedByType",
-    "DatabaseTier",
-    "DatabaseType",
-    "DiskStorageType",
-    "EnableBackup",
-    "EnableSslEnforcement",
+    "DiskSkuName",
     "EnqueueReplicationServerType",
-    "FileShareStorageType",
-    "FileShareType",
-    "HAEnabled",
-    "LoadBalancerType",
-    "LocationType",
     "ManagedServiceIdentityType",
-    "OSImageOffer",
-    "OSImagePublisher",
-    "OSImageSku",
-    "OSImageVersion",
+    "NamingPatternType",
     "OSType",
     "OperationProperties",
     "Origin",
-    "PHPVersion",
-    "PhpWorkloadProvisioningState",
-    "RedisCacheFamily",
     "RoutingPreference",
     "SAPConfigurationType",
     "SAPDatabaseScaleMethod",
     "SAPDatabaseType",
     "SAPDeploymentType",
     "SAPEnvironmentType",
     "SAPHealthState",
     "SAPHighAvailabilityType",
     "SAPProductType",
     "SAPSoftwareInstallationType",
     "SAPVirtualInstanceState",
     "SAPVirtualInstanceStatus",
+    "SapLandscapeMonitorProvisioningState",
     "SapVirtualInstanceProvisioningState",
-    "SearchType",
-    "SkuRestrictionReasonCode",
-    "SkuRestrictionType",
-    "SkuScaleType",
-    "SkuTier",
     "SslPreference",
-    "WordpressVersions",
-    "WorkloadKind",
     "WorkloadMonitorActionType",
     "WorkloadMonitorProvisioningState",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/models/_models_py3.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/models/_models_py3.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,28 +4,21 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 import datetime
-import sys
 from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union
 
 from .. import _serialization
 
-if sys.version_info >= (3, 9):
-    from collections.abc import MutableMapping
-else:
-    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
-
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from .. import models as _models
-JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 
 
 class ApplicationServerConfiguration(_serialization.Model):
     """Gets or sets the application server configuration.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -52,16 +45,16 @@
 
     def __init__(
         self,
         *,
         subnet_id: str,
         virtual_machine_configuration: "_models.VirtualMachineConfiguration",
         instance_count: int,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword subnet_id: The subnet id. Required.
         :paramtype subnet_id: str
         :keyword virtual_machine_configuration: Gets or sets the virtual machine configuration.
          Required.
         :paramtype virtual_machine_configuration:
          ~azure.mgmt.workloads.models.VirtualMachineConfiguration
@@ -70,108 +63,82 @@
         """
         super().__init__(**kwargs)
         self.subnet_id = subnet_id
         self.virtual_machine_configuration = virtual_machine_configuration
         self.instance_count = instance_count
 
 
-class BackupProfile(_serialization.Model):
-    """Backup profile.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    All required parameters must be populated in order to send to Azure.
+class ApplicationServerFullResourceNames(_serialization.Model):
+    """The full resource names object for application layer resources. The number of entries in this
+    list should be equal to the number VMs to be created for application layer.
 
-    :ivar backup_enabled: Whether to enable Azure backup for the workload. Required. Known values
-     are: "Enabled" and "Disabled".
-    :vartype backup_enabled: str or ~azure.mgmt.workloads.models.EnableBackup
-    :ivar vault_resource_id: Backup vault resource Id.
-    :vartype vault_resource_id: str
+    :ivar virtual_machines: The list of virtual machine naming details.
+    :vartype virtual_machines: list[~azure.mgmt.workloads.models.VirtualMachineResourceNames]
+    :ivar availability_set_name: The full name for availability set. In case name is not provided,
+     it will be defaulted to {SID}-App-AvSet.
+    :vartype availability_set_name: str
     """
 
-    _validation = {
-        "backup_enabled": {"required": True},
-        "vault_resource_id": {"readonly": True},
-    }
-
     _attribute_map = {
-        "backup_enabled": {"key": "backupEnabled", "type": "str"},
-        "vault_resource_id": {"key": "vaultResourceId", "type": "str"},
+        "virtual_machines": {"key": "virtualMachines", "type": "[VirtualMachineResourceNames]"},
+        "availability_set_name": {"key": "availabilitySetName", "type": "str"},
     }
 
-    def __init__(self, *, backup_enabled: Union[str, "_models.EnableBackup"], **kwargs):
+    def __init__(
+        self,
+        *,
+        virtual_machines: Optional[List["_models.VirtualMachineResourceNames"]] = None,
+        availability_set_name: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword backup_enabled: Whether to enable Azure backup for the workload. Required. Known
-         values are: "Enabled" and "Disabled".
-        :paramtype backup_enabled: str or ~azure.mgmt.workloads.models.EnableBackup
+        :keyword virtual_machines: The list of virtual machine naming details.
+        :paramtype virtual_machines: list[~azure.mgmt.workloads.models.VirtualMachineResourceNames]
+        :keyword availability_set_name: The full name for availability set. In case name is not
+         provided, it will be defaulted to {SID}-App-AvSet.
+        :paramtype availability_set_name: str
         """
         super().__init__(**kwargs)
-        self.backup_enabled = backup_enabled
-        self.vault_resource_id = None
+        self.virtual_machines = virtual_machines
+        self.availability_set_name = availability_set_name
 
 
-class CacheProfile(_serialization.Model):
-    """Cache profile.
+class ApplicationServerVmDetails(_serialization.Model):
+    """The Application Server VM Details.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar name: Cache name.
-    :vartype name: str
-    :ivar sku_name: Cache SKU name. Required.
-    :vartype sku_name: str
-    :ivar family: Cache family. Required. Known values are: "C" and "P".
-    :vartype family: str or ~azure.mgmt.workloads.models.RedisCacheFamily
-    :ivar capacity: Cache capacity. Required.
-    :vartype capacity: int
-    :ivar cache_resource_id: Cache resource Id.
-    :vartype cache_resource_id: str
+    :ivar type: Defines the type of application server VM. Known values are: "Active", "Standby",
+     and "Unknown".
+    :vartype type: str or ~azure.mgmt.workloads.models.ApplicationServerVirtualMachineType
+    :ivar virtual_machine_id:
+    :vartype virtual_machine_id: str
+    :ivar storage_details: Storage details of all the Storage Accounts attached to the App Virtual
+     Machine. For e.g. NFS on AFS Shared Storage.
+    :vartype storage_details: list[~azure.mgmt.workloads.models.StorageInformation]
     """
 
     _validation = {
-        "sku_name": {"required": True},
-        "family": {"required": True},
-        "capacity": {"required": True},
-        "cache_resource_id": {"readonly": True},
+        "type": {"readonly": True},
+        "virtual_machine_id": {"readonly": True},
+        "storage_details": {"readonly": True},
     }
 
     _attribute_map = {
-        "name": {"key": "name", "type": "str"},
-        "sku_name": {"key": "skuName", "type": "str"},
-        "family": {"key": "family", "type": "str"},
-        "capacity": {"key": "capacity", "type": "int"},
-        "cache_resource_id": {"key": "cacheResourceId", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "virtual_machine_id": {"key": "virtualMachineId", "type": "str"},
+        "storage_details": {"key": "storageDetails", "type": "[StorageInformation]"},
     }
 
-    def __init__(
-        self,
-        *,
-        sku_name: str,
-        family: Union[str, "_models.RedisCacheFamily"],
-        capacity: int,
-        name: Optional[str] = None,
-        **kwargs
-    ):
-        """
-        :keyword name: Cache name.
-        :paramtype name: str
-        :keyword sku_name: Cache SKU name. Required.
-        :paramtype sku_name: str
-        :keyword family: Cache family. Required. Known values are: "C" and "P".
-        :paramtype family: str or ~azure.mgmt.workloads.models.RedisCacheFamily
-        :keyword capacity: Cache capacity. Required.
-        :paramtype capacity: int
-        """
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
         super().__init__(**kwargs)
-        self.name = name
-        self.sku_name = sku_name
-        self.family = family
-        self.capacity = capacity
-        self.cache_resource_id = None
+        self.type = None
+        self.virtual_machine_id = None
+        self.storage_details = None
 
 
 class CentralServerConfiguration(_serialization.Model):
     """Gets or sets the central server configuration.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -198,16 +165,16 @@
 
     def __init__(
         self,
         *,
         subnet_id: str,
         virtual_machine_configuration: "_models.VirtualMachineConfiguration",
         instance_count: int,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword subnet_id: The subnet id. Required.
         :paramtype subnet_id: str
         :keyword virtual_machine_configuration: Gets or sets the virtual machine configuration.
          Required.
         :paramtype virtual_machine_configuration:
          ~azure.mgmt.workloads.models.VirtualMachineConfiguration
@@ -216,41 +183,175 @@
         """
         super().__init__(**kwargs)
         self.subnet_id = subnet_id
         self.virtual_machine_configuration = virtual_machine_configuration
         self.instance_count = instance_count
 
 
+class CentralServerFullResourceNames(_serialization.Model):
+    """The full resource names object for central server layer resources.
+
+    :ivar virtual_machines: The list of names for all ASCS virtual machines to be deployed. The
+     number of entries in this list should be equal to the number VMs to be created for ASCS layer.
+     At maximum, there can be two virtual machines at this layer: ASCS and ERS.
+    :vartype virtual_machines: list[~azure.mgmt.workloads.models.VirtualMachineResourceNames]
+    :ivar availability_set_name: The full name for availability set. In case name is not provided,
+     it will be defaulted to {SID}-ASCS-AvSet.
+    :vartype availability_set_name: str
+    :ivar load_balancer: The resource names object for load balancer and related resources.
+    :vartype load_balancer: ~azure.mgmt.workloads.models.LoadBalancerResourceNames
+    """
+
+    _validation = {
+        "virtual_machines": {"max_items": 2, "min_items": 0},
+    }
+
+    _attribute_map = {
+        "virtual_machines": {"key": "virtualMachines", "type": "[VirtualMachineResourceNames]"},
+        "availability_set_name": {"key": "availabilitySetName", "type": "str"},
+        "load_balancer": {"key": "loadBalancer", "type": "LoadBalancerResourceNames"},
+    }
+
+    def __init__(
+        self,
+        *,
+        virtual_machines: Optional[List["_models.VirtualMachineResourceNames"]] = None,
+        availability_set_name: Optional[str] = None,
+        load_balancer: Optional["_models.LoadBalancerResourceNames"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword virtual_machines: The list of names for all ASCS virtual machines to be deployed. The
+         number of entries in this list should be equal to the number VMs to be created for ASCS layer.
+         At maximum, there can be two virtual machines at this layer: ASCS and ERS.
+        :paramtype virtual_machines: list[~azure.mgmt.workloads.models.VirtualMachineResourceNames]
+        :keyword availability_set_name: The full name for availability set. In case name is not
+         provided, it will be defaulted to {SID}-ASCS-AvSet.
+        :paramtype availability_set_name: str
+        :keyword load_balancer: The resource names object for load balancer and related resources.
+        :paramtype load_balancer: ~azure.mgmt.workloads.models.LoadBalancerResourceNames
+        """
+        super().__init__(**kwargs)
+        self.virtual_machines = virtual_machines
+        self.availability_set_name = availability_set_name
+        self.load_balancer = load_balancer
+
+
 class CentralServerVmDetails(_serialization.Model):
     """The SAP Central Services Instance VM details.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar type: Defines the type of central server VM. Known values are: "Primary", "Secondary",
      "Unknown", "ASCS", "ERSInactive", "ERS", and "Standby".
     :vartype type: str or ~azure.mgmt.workloads.models.CentralServerVirtualMachineType
     :ivar virtual_machine_id:
     :vartype virtual_machine_id: str
+    :ivar storage_details: Storage details of all the Storage Accounts attached to the ASCS Virtual
+     Machine. For e.g. NFS on AFS Shared Storage.
+    :vartype storage_details: list[~azure.mgmt.workloads.models.StorageInformation]
     """
 
     _validation = {
         "type": {"readonly": True},
         "virtual_machine_id": {"readonly": True},
+        "storage_details": {"readonly": True},
     }
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "virtual_machine_id": {"key": "virtualMachineId", "type": "str"},
+        "storage_details": {"key": "storageDetails", "type": "[StorageInformation]"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.type = None
         self.virtual_machine_id = None
+        self.storage_details = None
+
+
+class FileShareConfiguration(_serialization.Model):
+    """File Share configuration details, populated with information on storage configuration mounted
+    on the VIS. The createAndMount option is selected in case of missing input.
+
+    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
+    CreateAndMountFileShareConfiguration, MountFileShareConfiguration, SkipFileShareConfiguration
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar configuration_type: The type of file share config. Required. Known values are: "Skip",
+     "CreateAndMount", and "Mount".
+    :vartype configuration_type: str or ~azure.mgmt.workloads.models.ConfigurationType
+    """
+
+    _validation = {
+        "configuration_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "configuration_type": {"key": "configurationType", "type": "str"},
+    }
+
+    _subtype_map = {
+        "configuration_type": {
+            "CreateAndMount": "CreateAndMountFileShareConfiguration",
+            "Mount": "MountFileShareConfiguration",
+            "Skip": "SkipFileShareConfiguration",
+        }
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.configuration_type: Optional[str] = None
+
+
+class CreateAndMountFileShareConfiguration(FileShareConfiguration):
+    """Gets or sets the file share configuration for file share created with the VIS case.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar configuration_type: The type of file share config. Required. Known values are: "Skip",
+     "CreateAndMount", and "Mount".
+    :vartype configuration_type: str or ~azure.mgmt.workloads.models.ConfigurationType
+    :ivar resource_group: The name of file share resource group. The app rg is used in case of
+     missing input.
+    :vartype resource_group: str
+    :ivar storage_account_name: The name of file share storage account name . A custom name is used
+     in case of missing input.
+    :vartype storage_account_name: str
+    """
+
+    _validation = {
+        "configuration_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "configuration_type": {"key": "configurationType", "type": "str"},
+        "resource_group": {"key": "resourceGroup", "type": "str"},
+        "storage_account_name": {"key": "storageAccountName", "type": "str"},
+    }
+
+    def __init__(
+        self, *, resource_group: Optional[str] = None, storage_account_name: Optional[str] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword resource_group: The name of file share resource group. The app rg is used in case of
+         missing input.
+        :paramtype resource_group: str
+        :keyword storage_account_name: The name of file share storage account name . A custom name is
+         used in case of missing input.
+        :paramtype storage_account_name: str
+        """
+        super().__init__(**kwargs)
+        self.configuration_type: str = "CreateAndMount"
+        self.resource_group = resource_group
+        self.storage_account_name = storage_account_name
 
 
 class DatabaseConfiguration(_serialization.Model):
     """Gets or sets the database configuration.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -259,201 +360,143 @@
     :ivar subnet_id: The subnet id. Required.
     :vartype subnet_id: str
     :ivar virtual_machine_configuration: Gets or sets the virtual machine configuration. Required.
     :vartype virtual_machine_configuration:
      ~azure.mgmt.workloads.models.VirtualMachineConfiguration
     :ivar instance_count: The number of database VMs. Required.
     :vartype instance_count: int
+    :ivar disk_configuration: Gets or sets the disk configuration.
+    :vartype disk_configuration: ~azure.mgmt.workloads.models.DiskConfiguration
     """
 
     _validation = {
         "subnet_id": {"required": True},
         "virtual_machine_configuration": {"required": True},
         "instance_count": {"required": True},
     }
 
     _attribute_map = {
         "database_type": {"key": "databaseType", "type": "str"},
         "subnet_id": {"key": "subnetId", "type": "str"},
         "virtual_machine_configuration": {"key": "virtualMachineConfiguration", "type": "VirtualMachineConfiguration"},
         "instance_count": {"key": "instanceCount", "type": "int"},
+        "disk_configuration": {"key": "diskConfiguration", "type": "DiskConfiguration"},
     }
 
     def __init__(
         self,
         *,
         subnet_id: str,
         virtual_machine_configuration: "_models.VirtualMachineConfiguration",
         instance_count: int,
         database_type: Optional[Union[str, "_models.SAPDatabaseType"]] = None,
-        **kwargs
-    ):
+        disk_configuration: Optional["_models.DiskConfiguration"] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword database_type: The database type. Known values are: "HANA" and "DB2".
         :paramtype database_type: str or ~azure.mgmt.workloads.models.SAPDatabaseType
         :keyword subnet_id: The subnet id. Required.
         :paramtype subnet_id: str
         :keyword virtual_machine_configuration: Gets or sets the virtual machine configuration.
          Required.
         :paramtype virtual_machine_configuration:
          ~azure.mgmt.workloads.models.VirtualMachineConfiguration
         :keyword instance_count: The number of database VMs. Required.
         :paramtype instance_count: int
+        :keyword disk_configuration: Gets or sets the disk configuration.
+        :paramtype disk_configuration: ~azure.mgmt.workloads.models.DiskConfiguration
         """
         super().__init__(**kwargs)
         self.database_type = database_type
         self.subnet_id = subnet_id
         self.virtual_machine_configuration = virtual_machine_configuration
         self.instance_count = instance_count
+        self.disk_configuration = disk_configuration
 
 
-class DatabaseProfile(_serialization.Model):  # pylint: disable=too-many-instance-attributes
-    """Workload database profile.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    All required parameters must be populated in order to send to Azure.
+class DatabaseServerFullResourceNames(_serialization.Model):
+    """The full resource names object for database layer resources. The number of entries in this list
+    should be equal to the number VMs to be created for database layer.
 
-    :ivar type: Database type. Required. "MySql"
-    :vartype type: str or ~azure.mgmt.workloads.models.DatabaseType
-    :ivar server_name: Database server name.
-    :vartype server_name: str
-    :ivar version: Database version.
-    :vartype version: str
-    :ivar sku: The name of the server SKU, e.g. Standard_D32s_v4. Required.
-    :vartype sku: str
-    :ivar tier: Tier of the server SKU. Required. Known values are: "Burstable", "GeneralPurpose",
-     and "MemoryOptimized".
-    :vartype tier: str or ~azure.mgmt.workloads.models.DatabaseTier
-    :ivar ha_enabled: Whether to enable HA for the server. Known values are: "Enabled" and
-     "Disabled".
-    :vartype ha_enabled: str or ~azure.mgmt.workloads.models.HAEnabled
-    :ivar storage_sku: SKU name for database storage.
-    :vartype storage_sku: str
-    :ivar storage_in_gb: Database storage size in GB.
-    :vartype storage_in_gb: int
-    :ivar storage_iops: Storage IOPS for the server.
-    :vartype storage_iops: int
-    :ivar backup_retention_days: Backup retention days for the server.
-    :vartype backup_retention_days: int
-    :ivar ssl_enforcement_enabled: Whether to enable SSL enforcement on the database. Known values
-     are: "Enabled" and "Disabled".
-    :vartype ssl_enforcement_enabled: str or ~azure.mgmt.workloads.models.EnableSslEnforcement
-    :ivar server_resource_id: Azure Database Server resource Id.
-    :vartype server_resource_id: str
+    :ivar virtual_machines: The list of virtual machine naming details.
+    :vartype virtual_machines: list[~azure.mgmt.workloads.models.VirtualMachineResourceNames]
+    :ivar availability_set_name: The full name for availability set. In case name is not provided,
+     it will be defaulted to {SID}-DB-AvSet.
+    :vartype availability_set_name: str
+    :ivar load_balancer: The resource names object for load balancer and related resources.
+    :vartype load_balancer: ~azure.mgmt.workloads.models.LoadBalancerResourceNames
     """
 
     _validation = {
-        "type": {"required": True},
-        "sku": {"required": True},
-        "tier": {"required": True},
-        "storage_in_gb": {"minimum": 1},
-        "server_resource_id": {"readonly": True},
+        "virtual_machines": {"max_items": 2, "min_items": 0},
     }
 
     _attribute_map = {
-        "type": {"key": "type", "type": "str"},
-        "server_name": {"key": "serverName", "type": "str"},
-        "version": {"key": "version", "type": "str"},
-        "sku": {"key": "sku", "type": "str"},
-        "tier": {"key": "tier", "type": "str"},
-        "ha_enabled": {"key": "haEnabled", "type": "str"},
-        "storage_sku": {"key": "storageSku", "type": "str"},
-        "storage_in_gb": {"key": "storageInGB", "type": "int"},
-        "storage_iops": {"key": "storageIops", "type": "int"},
-        "backup_retention_days": {"key": "backupRetentionDays", "type": "int"},
-        "ssl_enforcement_enabled": {"key": "sslEnforcementEnabled", "type": "str"},
-        "server_resource_id": {"key": "serverResourceId", "type": "str"},
+        "virtual_machines": {"key": "virtualMachines", "type": "[VirtualMachineResourceNames]"},
+        "availability_set_name": {"key": "availabilitySetName", "type": "str"},
+        "load_balancer": {"key": "loadBalancer", "type": "LoadBalancerResourceNames"},
     }
 
     def __init__(
         self,
         *,
-        type: Union[str, "_models.DatabaseType"],
-        sku: str,
-        tier: Union[str, "_models.DatabaseTier"],
-        server_name: Optional[str] = None,
-        version: Optional[str] = None,
-        ha_enabled: Optional[Union[str, "_models.HAEnabled"]] = None,
-        storage_sku: Optional[str] = None,
-        storage_in_gb: Optional[int] = None,
-        storage_iops: Optional[int] = None,
-        backup_retention_days: Optional[int] = None,
-        ssl_enforcement_enabled: Optional[Union[str, "_models.EnableSslEnforcement"]] = None,
-        **kwargs
-    ):
-        """
-        :keyword type: Database type. Required. "MySql"
-        :paramtype type: str or ~azure.mgmt.workloads.models.DatabaseType
-        :keyword server_name: Database server name.
-        :paramtype server_name: str
-        :keyword version: Database version.
-        :paramtype version: str
-        :keyword sku: The name of the server SKU, e.g. Standard_D32s_v4. Required.
-        :paramtype sku: str
-        :keyword tier: Tier of the server SKU. Required. Known values are: "Burstable",
-         "GeneralPurpose", and "MemoryOptimized".
-        :paramtype tier: str or ~azure.mgmt.workloads.models.DatabaseTier
-        :keyword ha_enabled: Whether to enable HA for the server. Known values are: "Enabled" and
-         "Disabled".
-        :paramtype ha_enabled: str or ~azure.mgmt.workloads.models.HAEnabled
-        :keyword storage_sku: SKU name for database storage.
-        :paramtype storage_sku: str
-        :keyword storage_in_gb: Database storage size in GB.
-        :paramtype storage_in_gb: int
-        :keyword storage_iops: Storage IOPS for the server.
-        :paramtype storage_iops: int
-        :keyword backup_retention_days: Backup retention days for the server.
-        :paramtype backup_retention_days: int
-        :keyword ssl_enforcement_enabled: Whether to enable SSL enforcement on the database. Known
-         values are: "Enabled" and "Disabled".
-        :paramtype ssl_enforcement_enabled: str or ~azure.mgmt.workloads.models.EnableSslEnforcement
+        virtual_machines: Optional[List["_models.VirtualMachineResourceNames"]] = None,
+        availability_set_name: Optional[str] = None,
+        load_balancer: Optional["_models.LoadBalancerResourceNames"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword virtual_machines: The list of virtual machine naming details.
+        :paramtype virtual_machines: list[~azure.mgmt.workloads.models.VirtualMachineResourceNames]
+        :keyword availability_set_name: The full name for availability set. In case name is not
+         provided, it will be defaulted to {SID}-DB-AvSet.
+        :paramtype availability_set_name: str
+        :keyword load_balancer: The resource names object for load balancer and related resources.
+        :paramtype load_balancer: ~azure.mgmt.workloads.models.LoadBalancerResourceNames
         """
         super().__init__(**kwargs)
-        self.type = type
-        self.server_name = server_name
-        self.version = version
-        self.sku = sku
-        self.tier = tier
-        self.ha_enabled = ha_enabled
-        self.storage_sku = storage_sku
-        self.storage_in_gb = storage_in_gb
-        self.storage_iops = storage_iops
-        self.backup_retention_days = backup_retention_days
-        self.ssl_enforcement_enabled = ssl_enforcement_enabled
-        self.server_resource_id = None
+        self.virtual_machines = virtual_machines
+        self.availability_set_name = availability_set_name
+        self.load_balancer = load_balancer
 
 
 class DatabaseVmDetails(_serialization.Model):
     """Database VM details.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar virtual_machine_id:
     :vartype virtual_machine_id: str
     :ivar status: Defines the SAP Instance status. Known values are: "Starting", "Running",
-     "Stopping", "Offline", "PartiallyRunning", and "Unavailable".
+     "Stopping", "Offline", "PartiallyRunning", "Unavailable", and "SoftShutdown".
     :vartype status: str or ~azure.mgmt.workloads.models.SAPVirtualInstanceStatus
+    :ivar storage_details: Storage details of all the Storage Accounts attached to the Database
+     Virtual Machine. For e.g. NFS on AFS Shared Storage.
+    :vartype storage_details: list[~azure.mgmt.workloads.models.StorageInformation]
     """
 
     _validation = {
         "virtual_machine_id": {"readonly": True},
         "status": {"readonly": True},
+        "storage_details": {"readonly": True},
     }
 
     _attribute_map = {
         "virtual_machine_id": {"key": "virtualMachineId", "type": "str"},
         "status": {"key": "status", "type": "str"},
+        "storage_details": {"key": "storageDetails", "type": "[StorageInformation]"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.virtual_machine_id = None
         self.status = None
+        self.storage_details = None
 
 
 class ProviderSpecificProperties(_serialization.Model):
     """Gets or sets the provider specific properties.
 
     You probably want to use the sub-classes and not this class directly. Known sub-classes are:
     DB2ProviderInstanceProperties, MsSqlServerProviderInstanceProperties,
@@ -481,15 +524,15 @@
             "PrometheusHaCluster": "PrometheusHaClusterProviderInstanceProperties",
             "PrometheusOS": "PrometheusOSProviderInstanceProperties",
             "SapHana": "HanaDbProviderInstanceProperties",
             "SapNetWeaver": "SapNetWeaverProviderInstanceProperties",
         }
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.provider_type: Optional[str] = None
 
 
 class DB2ProviderInstanceProperties(ProviderSpecificProperties):
     """Gets or sets the DB2 provider properties.
@@ -544,16 +587,16 @@
         db_port: Optional[str] = None,
         db_username: Optional[str] = None,
         db_password: Optional[str] = None,
         db_password_uri: Optional[str] = None,
         sap_sid: Optional[str] = None,
         ssl_preference: Optional[Union[str, "_models.SslPreference"]] = None,
         ssl_certificate_uri: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword hostname: Gets or sets the target virtual machine name.
         :paramtype hostname: str
         :keyword db_name: Gets or sets the db2 database name.
         :paramtype db_name: str
         :keyword db_port: Gets or sets the db2 database sql port.
         :paramtype db_port: str
@@ -595,15 +638,15 @@
     """
 
     _attribute_map = {
         "url": {"key": "url", "type": "str"},
         "storage_account_id": {"key": "storageAccountId", "type": "str"},
     }
 
-    def __init__(self, *, url: Optional[str] = None, storage_account_id: Optional[str] = None, **kwargs):
+    def __init__(self, *, url: Optional[str] = None, storage_account_id: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword url: The URL to the deployer VM packages file.
         :paramtype url: str
         :keyword storage_account_id: The deployer VM packages storage account id.
         :paramtype storage_account_id: str
         """
         super().__init__(**kwargs)
@@ -636,15 +679,15 @@
         "configuration_type": {
             "Deployment": "DeploymentConfiguration",
             "DeploymentWithOSConfig": "DeploymentWithOSConfiguration",
             "Discovery": "DiscoveryConfiguration",
         }
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.configuration_type: Optional[str] = None
 
 
 class DeploymentConfiguration(SAPConfiguration):
     """Deployment Configuration.
@@ -675,16 +718,16 @@
 
     def __init__(
         self,
         *,
         app_location: Optional[str] = None,
         infrastructure_configuration: Optional["_models.InfrastructureConfiguration"] = None,
         software_configuration: Optional["_models.SoftwareConfiguration"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword app_location: The geo-location where the SAP system is to be created.
         :paramtype app_location: str
         :keyword infrastructure_configuration: The infrastructure configuration.
         :paramtype infrastructure_configuration:
          ~azure.mgmt.workloads.models.InfrastructureConfiguration
         :keyword software_configuration: The software configuration.
@@ -730,16 +773,16 @@
     def __init__(
         self,
         *,
         app_location: Optional[str] = None,
         infrastructure_configuration: Optional["_models.InfrastructureConfiguration"] = None,
         software_configuration: Optional["_models.SoftwareConfiguration"] = None,
         os_sap_configuration: Optional["_models.OsSapConfiguration"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword app_location: The geo-location where the SAP system is to be created.
         :paramtype app_location: str
         :keyword infrastructure_configuration: The infrastructure configuration.
         :paramtype infrastructure_configuration:
          ~azure.mgmt.workloads.models.InfrastructureConfiguration
         :keyword software_configuration: The software configuration.
@@ -763,74 +806,218 @@
     All required parameters must be populated in order to send to Azure.
 
     :ivar configuration_type: The configuration Type. Required. Known values are: "Deployment",
      "Discovery", and "DeploymentWithOSConfig".
     :vartype configuration_type: str or ~azure.mgmt.workloads.models.SAPConfigurationType
     :ivar central_server_vm_id: The virtual machine ID of the Central Server.
     :vartype central_server_vm_id: str
+    :ivar managed_rg_storage_account_name: The custom storage account name for the storage account
+     created by the service in the managed resource group created as part of VIS
+     deployment.:code:`<br>`:code:`<br>`Refer to the storage account naming rules `here
+     <https://learn.microsoft.com/azure/azure-resource-manager/management/resource-name-rules#microsoftstorage>`_.:code:`<br>`:code:`<br>`If
+     not provided, the service will create the storage account with a random name.
+    :vartype managed_rg_storage_account_name: str
     :ivar app_location: The geo-location where the SAP system exists.
     :vartype app_location: str
     """
 
     _validation = {
         "configuration_type": {"required": True},
+        "managed_rg_storage_account_name": {"max_length": 24, "min_length": 3},
         "app_location": {"readonly": True},
     }
 
     _attribute_map = {
         "configuration_type": {"key": "configurationType", "type": "str"},
         "central_server_vm_id": {"key": "centralServerVmId", "type": "str"},
+        "managed_rg_storage_account_name": {"key": "managedRgStorageAccountName", "type": "str"},
         "app_location": {"key": "appLocation", "type": "str"},
     }
 
-    def __init__(self, *, central_server_vm_id: Optional[str] = None, **kwargs):
+    def __init__(
+        self,
+        *,
+        central_server_vm_id: Optional[str] = None,
+        managed_rg_storage_account_name: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword central_server_vm_id: The virtual machine ID of the Central Server.
         :paramtype central_server_vm_id: str
+        :keyword managed_rg_storage_account_name: The custom storage account name for the storage
+         account created by the service in the managed resource group created as part of VIS
+         deployment.:code:`<br>`:code:`<br>`Refer to the storage account naming rules `here
+         <https://learn.microsoft.com/azure/azure-resource-manager/management/resource-name-rules#microsoftstorage>`_.:code:`<br>`:code:`<br>`If
+         not provided, the service will create the storage account with a random name.
+        :paramtype managed_rg_storage_account_name: str
         """
         super().__init__(**kwargs)
         self.configuration_type: str = "Discovery"
         self.central_server_vm_id = central_server_vm_id
+        self.managed_rg_storage_account_name = managed_rg_storage_account_name
         self.app_location = None
 
 
-class DiskInfo(_serialization.Model):
-    """Disk resource creation details.
+class DiskConfiguration(_serialization.Model):
+    """The Disk Configuration Details.
 
-    All required parameters must be populated in order to send to Azure.
+    :ivar disk_volume_configurations: The disk configuration for the db volume. For HANA, Required
+     volumes are: ['hana/data', 'hana/log', hana/shared', 'usr/sap', 'os'], Optional volume :
+     ['backup'].
+    :vartype disk_volume_configurations: dict[str,
+     ~azure.mgmt.workloads.models.DiskVolumeConfiguration]
+    """
 
-    :ivar storage_type: Storage type. Required. Known values are: "Premium_LRS", "Standard_LRS",
-     and "StandardSSD_LRS".
-    :vartype storage_type: str or ~azure.mgmt.workloads.models.DiskStorageType
-    :ivar size_in_gb: Disk size in GB.
-    :vartype size_in_gb: int
+    _attribute_map = {
+        "disk_volume_configurations": {"key": "diskVolumeConfigurations", "type": "{DiskVolumeConfiguration}"},
+    }
+
+    def __init__(
+        self,
+        *,
+        disk_volume_configurations: Optional[Dict[str, "_models.DiskVolumeConfiguration"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword disk_volume_configurations: The disk configuration for the db volume. For HANA,
+         Required volumes are: ['hana/data', 'hana/log', hana/shared', 'usr/sap', 'os'], Optional volume
+         : ['backup'].
+        :paramtype disk_volume_configurations: dict[str,
+         ~azure.mgmt.workloads.models.DiskVolumeConfiguration]
+        """
+        super().__init__(**kwargs)
+        self.disk_volume_configurations = disk_volume_configurations
+
+
+class DiskDetails(_serialization.Model):
+    """The supported disk size details for a disk type.
+
+    :ivar sku: The disk sku.
+    :vartype sku: ~azure.mgmt.workloads.models.DiskSku
+    :ivar size_gb: The disk size in GB.
+    :vartype size_gb: int
+    :ivar minimum_supported_disk_count: The minimum supported disk count.
+    :vartype minimum_supported_disk_count: int
+    :ivar maximum_supported_disk_count: The maximum supported disk count.
+    :vartype maximum_supported_disk_count: int
+    :ivar iops_read_write: The disk Iops.
+    :vartype iops_read_write: int
+    :ivar mbps_read_write: The disk provisioned throughput in MBps.
+    :vartype mbps_read_write: int
+    :ivar disk_tier: The disk tier, e.g. P10, E10.
+    :vartype disk_tier: str
     """
 
-    _validation = {
-        "storage_type": {"required": True},
+    _attribute_map = {
+        "sku": {"key": "sku", "type": "DiskSku"},
+        "size_gb": {"key": "sizeGB", "type": "int"},
+        "minimum_supported_disk_count": {"key": "minimumSupportedDiskCount", "type": "int"},
+        "maximum_supported_disk_count": {"key": "maximumSupportedDiskCount", "type": "int"},
+        "iops_read_write": {"key": "iopsReadWrite", "type": "int"},
+        "mbps_read_write": {"key": "mbpsReadWrite", "type": "int"},
+        "disk_tier": {"key": "diskTier", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        sku: Optional["_models.DiskSku"] = None,
+        size_gb: Optional[int] = None,
+        minimum_supported_disk_count: Optional[int] = None,
+        maximum_supported_disk_count: Optional[int] = None,
+        iops_read_write: Optional[int] = None,
+        mbps_read_write: Optional[int] = None,
+        disk_tier: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword sku: The disk sku.
+        :paramtype sku: ~azure.mgmt.workloads.models.DiskSku
+        :keyword size_gb: The disk size in GB.
+        :paramtype size_gb: int
+        :keyword minimum_supported_disk_count: The minimum supported disk count.
+        :paramtype minimum_supported_disk_count: int
+        :keyword maximum_supported_disk_count: The maximum supported disk count.
+        :paramtype maximum_supported_disk_count: int
+        :keyword iops_read_write: The disk Iops.
+        :paramtype iops_read_write: int
+        :keyword mbps_read_write: The disk provisioned throughput in MBps.
+        :paramtype mbps_read_write: int
+        :keyword disk_tier: The disk tier, e.g. P10, E10.
+        :paramtype disk_tier: str
+        """
+        super().__init__(**kwargs)
+        self.sku = sku
+        self.size_gb = size_gb
+        self.minimum_supported_disk_count = minimum_supported_disk_count
+        self.maximum_supported_disk_count = maximum_supported_disk_count
+        self.iops_read_write = iops_read_write
+        self.mbps_read_write = mbps_read_write
+        self.disk_tier = disk_tier
+
+
+class DiskSku(_serialization.Model):
+    """The disk sku.
+
+    :ivar name: Defines the disk sku name. Known values are: "Standard_LRS", "Premium_LRS",
+     "StandardSSD_LRS", "UltraSSD_LRS", "Premium_ZRS", "StandardSSD_ZRS", and "PremiumV2_LRS".
+    :vartype name: str or ~azure.mgmt.workloads.models.DiskSkuName
+    """
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
     }
 
+    def __init__(self, *, name: Optional[Union[str, "_models.DiskSkuName"]] = None, **kwargs: Any) -> None:
+        """
+        :keyword name: Defines the disk sku name. Known values are: "Standard_LRS", "Premium_LRS",
+         "StandardSSD_LRS", "UltraSSD_LRS", "Premium_ZRS", "StandardSSD_ZRS", and "PremiumV2_LRS".
+        :paramtype name: str or ~azure.mgmt.workloads.models.DiskSkuName
+        """
+        super().__init__(**kwargs)
+        self.name = name
+
+
+class DiskVolumeConfiguration(_serialization.Model):
+    """The disk configuration required for the selected volume.
+
+    :ivar count: The total number of disks required for the concerned volume.
+    :vartype count: int
+    :ivar size_gb: The disk size in GB.
+    :vartype size_gb: int
+    :ivar sku: The disk SKU details.
+    :vartype sku: ~azure.mgmt.workloads.models.DiskSku
+    """
+
     _attribute_map = {
-        "storage_type": {"key": "storageType", "type": "str"},
-        "size_in_gb": {"key": "sizeInGB", "type": "int"},
+        "count": {"key": "count", "type": "int"},
+        "size_gb": {"key": "sizeGB", "type": "int"},
+        "sku": {"key": "sku", "type": "DiskSku"},
     }
 
     def __init__(
-        self, *, storage_type: Union[str, "_models.DiskStorageType"], size_in_gb: Optional[int] = None, **kwargs
-    ):
+        self,
+        *,
+        count: Optional[int] = None,
+        size_gb: Optional[int] = None,
+        sku: Optional["_models.DiskSku"] = None,
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword storage_type: Storage type. Required. Known values are: "Premium_LRS", "Standard_LRS",
-         and "StandardSSD_LRS".
-        :paramtype storage_type: str or ~azure.mgmt.workloads.models.DiskStorageType
-        :keyword size_in_gb: Disk size in GB.
-        :paramtype size_in_gb: int
+        :keyword count: The total number of disks required for the concerned volume.
+        :paramtype count: int
+        :keyword size_gb: The disk size in GB.
+        :paramtype size_gb: int
+        :keyword sku: The disk SKU details.
+        :paramtype sku: ~azure.mgmt.workloads.models.DiskSku
         """
         super().__init__(**kwargs)
-        self.storage_type = storage_type
-        self.size_in_gb = size_in_gb
+        self.count = count
+        self.size_gb = size_gb
+        self.sku = sku
 
 
 class EnqueueReplicationServerProperties(_serialization.Model):
     """Defines the SAP Enqueue Replication Server (ERS) properties.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -868,15 +1055,15 @@
         "hostname": {"key": "hostname", "type": "str"},
         "kernel_version": {"key": "kernelVersion", "type": "str"},
         "kernel_patch": {"key": "kernelPatch", "type": "str"},
         "ip_address": {"key": "ipAddress", "type": "str"},
         "health": {"key": "health", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.ers_version = None
         self.instance_no = None
         self.hostname = None
         self.kernel_version = None
         self.kernel_patch = None
@@ -910,15 +1097,15 @@
     _attribute_map = {
         "hostname": {"key": "hostname", "type": "str"},
         "ip_address": {"key": "ipAddress", "type": "str"},
         "port": {"key": "port", "type": "int"},
         "health": {"key": "health", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.hostname = None
         self.ip_address = None
         self.port = None
         self.health = None
 
@@ -953,15 +1140,15 @@
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
         "target": {"key": "target", "type": "str"},
         "details": {"key": "details", "type": "[Error]"},
         "inner_error": {"key": "innerError", "type": "ErrorInnerError"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.code = None
         self.message = None
         self.target = None
         self.details = None
         self.inner_error = None
@@ -984,15 +1171,15 @@
     }
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "info": {"key": "info", "type": "object"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.type = None
         self.info = None
 
 
 class ErrorDefinition(_serialization.Model):
@@ -1016,15 +1203,15 @@
 
     _attribute_map = {
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
         "details": {"key": "details", "type": "[ErrorDefinition]"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.code = None
         self.message = None
         self.details = None
 
 
@@ -1057,15 +1244,15 @@
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
         "target": {"key": "target", "type": "str"},
         "details": {"key": "details", "type": "[ErrorDetail]"},
         "additional_info": {"key": "additionalInfo", "type": "[ErrorAdditionalInfo]"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.code = None
         self.message = None
         self.target = None
         self.details = None
         self.additional_info = None
@@ -1078,35 +1265,36 @@
     :vartype inner_error: ~azure.mgmt.workloads.models.Error
     """
 
     _attribute_map = {
         "inner_error": {"key": "innerError", "type": "Error"},
     }
 
-    def __init__(self, *, inner_error: Optional["_models.Error"] = None, **kwargs):
+    def __init__(self, *, inner_error: Optional["_models.Error"] = None, **kwargs: Any) -> None:
         """
         :keyword inner_error: Standard error object.
         :paramtype inner_error: ~azure.mgmt.workloads.models.Error
         """
         super().__init__(**kwargs)
         self.inner_error = inner_error
 
 
 class ErrorResponse(_serialization.Model):
-    """Common error response for all Azure Resource Manager APIs to return error details for failed operations. (This also follows the OData error response format.).
+    """Common error response for all Azure Resource Manager APIs to return error details for failed
+    operations. (This also follows the OData error response format.).
 
     :ivar error: The error object.
     :vartype error: ~azure.mgmt.workloads.models.ErrorDetail
     """
 
     _attribute_map = {
         "error": {"key": "error", "type": "ErrorDetail"},
     }
 
-    def __init__(self, *, error: Optional["_models.ErrorDetail"] = None, **kwargs):
+    def __init__(self, *, error: Optional["_models.ErrorDetail"] = None, **kwargs: Any) -> None:
         """
         :keyword error: The error object.
         :paramtype error: ~azure.mgmt.workloads.models.ErrorDetail
         """
         super().__init__(**kwargs)
         self.error = error
 
@@ -1138,22 +1326,23 @@
         "software_installation_type": {
             "External": "ExternalInstallationSoftwareConfiguration",
             "SAPInstallWithoutOSConfig": "SAPInstallWithoutOSConfigSoftwareConfiguration",
             "ServiceInitiated": "ServiceInitiatedSoftwareConfiguration",
         }
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.software_installation_type: Optional[str] = None
 
 
 class ExternalInstallationSoftwareConfiguration(SoftwareConfiguration):
-    """The SAP Software configuration Input when the software is installed externally outside the service.
+    """The SAP Software configuration Input when the software is installed externally outside the
+    service.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar software_installation_type: The SAP software installation Type. Required. Known values
      are: "ServiceInitiated", "SAPInstallWithoutOSConfig", and "External".
     :vartype software_installation_type: str or
      ~azure.mgmt.workloads.models.SAPSoftwareInstallationType
@@ -1167,87 +1356,25 @@
     }
 
     _attribute_map = {
         "software_installation_type": {"key": "softwareInstallationType", "type": "str"},
         "central_server_vm_id": {"key": "centralServerVmId", "type": "str"},
     }
 
-    def __init__(self, *, central_server_vm_id: Optional[str] = None, **kwargs):
+    def __init__(self, *, central_server_vm_id: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword central_server_vm_id: The resource ID of the virtual machine containing the central
          server instance.
         :paramtype central_server_vm_id: str
         """
         super().__init__(**kwargs)
         self.software_installation_type: str = "External"
         self.central_server_vm_id = central_server_vm_id
 
 
-class FileshareProfile(_serialization.Model):
-    """File share profile.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar share_type: Share type. Required. Known values are: "NfsOnController" and "AzureFiles".
-    :vartype share_type: str or ~azure.mgmt.workloads.models.FileShareType
-    :ivar storage_type: File share backing storage type. Required. Known values are:
-     "Standard_LRS", "Standard_GRS", "Standard_ZRS", and "Premium_LRS".
-    :vartype storage_type: str or ~azure.mgmt.workloads.models.FileShareStorageType
-    :ivar share_size_in_gb: File share size in GB.
-    :vartype share_size_in_gb: int
-    :ivar storage_resource_id: File share storage resource id.
-    :vartype storage_resource_id: str
-    :ivar share_name: File share name.
-    :vartype share_name: str
-    """
-
-    _validation = {
-        "share_type": {"required": True},
-        "storage_type": {"required": True},
-        "share_size_in_gb": {"minimum": 1},
-        "storage_resource_id": {"readonly": True},
-        "share_name": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "share_type": {"key": "shareType", "type": "str"},
-        "storage_type": {"key": "storageType", "type": "str"},
-        "share_size_in_gb": {"key": "shareSizeInGB", "type": "int"},
-        "storage_resource_id": {"key": "storageResourceId", "type": "str"},
-        "share_name": {"key": "shareName", "type": "str"},
-    }
-
-    def __init__(
-        self,
-        *,
-        share_type: Union[str, "_models.FileShareType"],
-        storage_type: Union[str, "_models.FileShareStorageType"],
-        share_size_in_gb: Optional[int] = None,
-        **kwargs
-    ):
-        """
-        :keyword share_type: Share type. Required. Known values are: "NfsOnController" and
-         "AzureFiles".
-        :paramtype share_type: str or ~azure.mgmt.workloads.models.FileShareType
-        :keyword storage_type: File share backing storage type. Required. Known values are:
-         "Standard_LRS", "Standard_GRS", "Standard_ZRS", and "Premium_LRS".
-        :paramtype storage_type: str or ~azure.mgmt.workloads.models.FileShareStorageType
-        :keyword share_size_in_gb: File share size in GB.
-        :paramtype share_size_in_gb: int
-        """
-        super().__init__(**kwargs)
-        self.share_type = share_type
-        self.storage_type = storage_type
-        self.share_size_in_gb = share_size_in_gb
-        self.storage_resource_id = None
-        self.share_name = None
-
-
 class GatewayServerProperties(_serialization.Model):
     """Defines the SAP Gateway Server properties.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar port: Gateway Port.
     :vartype port: int
@@ -1262,15 +1389,15 @@
     }
 
     _attribute_map = {
         "port": {"key": "port", "type": "int"},
         "health": {"key": "health", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.port = None
         self.health = None
 
 
 class HanaDbProviderInstanceProperties(ProviderSpecificProperties):  # pylint: disable=too-many-instance-attributes
@@ -1290,23 +1417,23 @@
     :vartype instance_number: str
     :ivar db_username: Gets or sets the database user name.
     :vartype db_username: str
     :ivar db_password: Gets or sets the database password.
     :vartype db_password: str
     :ivar db_password_uri: Gets or sets the key vault URI to secret with the database password.
     :vartype db_password_uri: str
-    :ivar db_ssl_certificate_uri: Gets or sets the blob URI to SSL certificate for the DB.
-    :vartype db_ssl_certificate_uri: str
     :ivar ssl_certificate_uri: Gets or sets the blob URI to SSL certificate for the DB.
     :vartype ssl_certificate_uri: str
     :ivar ssl_host_name_in_certificate: Gets or sets the hostname(s) in the SSL certificate.
     :vartype ssl_host_name_in_certificate: str
     :ivar ssl_preference: Gets or sets certificate preference if secure communication is enabled.
      Known values are: "Disabled", "RootCertificate", and "ServerCertificate".
     :vartype ssl_preference: str or ~azure.mgmt.workloads.models.SslPreference
+    :ivar sap_sid: Gets or sets the SAP System Identifier.
+    :vartype sap_sid: str
     """
 
     _validation = {
         "provider_type": {"required": True},
     }
 
     _attribute_map = {
@@ -1314,36 +1441,36 @@
         "hostname": {"key": "hostname", "type": "str"},
         "db_name": {"key": "dbName", "type": "str"},
         "sql_port": {"key": "sqlPort", "type": "str"},
         "instance_number": {"key": "instanceNumber", "type": "str"},
         "db_username": {"key": "dbUsername", "type": "str"},
         "db_password": {"key": "dbPassword", "type": "str"},
         "db_password_uri": {"key": "dbPasswordUri", "type": "str"},
-        "db_ssl_certificate_uri": {"key": "dbSslCertificateUri", "type": "str"},
         "ssl_certificate_uri": {"key": "sslCertificateUri", "type": "str"},
         "ssl_host_name_in_certificate": {"key": "sslHostNameInCertificate", "type": "str"},
         "ssl_preference": {"key": "sslPreference", "type": "str"},
+        "sap_sid": {"key": "sapSid", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         hostname: Optional[str] = None,
         db_name: Optional[str] = None,
         sql_port: Optional[str] = None,
         instance_number: Optional[str] = None,
         db_username: Optional[str] = None,
         db_password: Optional[str] = None,
         db_password_uri: Optional[str] = None,
-        db_ssl_certificate_uri: Optional[str] = None,
         ssl_certificate_uri: Optional[str] = None,
         ssl_host_name_in_certificate: Optional[str] = None,
         ssl_preference: Optional[Union[str, "_models.SslPreference"]] = None,
-        **kwargs
-    ):
+        sap_sid: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword hostname: Gets or sets the target virtual machine size.
         :paramtype hostname: str
         :keyword db_name: Gets or sets the hana database name.
         :paramtype db_name: str
         :keyword sql_port: Gets or sets the database sql port.
         :paramtype sql_port: str
@@ -1351,37 +1478,37 @@
         :paramtype instance_number: str
         :keyword db_username: Gets or sets the database user name.
         :paramtype db_username: str
         :keyword db_password: Gets or sets the database password.
         :paramtype db_password: str
         :keyword db_password_uri: Gets or sets the key vault URI to secret with the database password.
         :paramtype db_password_uri: str
-        :keyword db_ssl_certificate_uri: Gets or sets the blob URI to SSL certificate for the DB.
-        :paramtype db_ssl_certificate_uri: str
         :keyword ssl_certificate_uri: Gets or sets the blob URI to SSL certificate for the DB.
         :paramtype ssl_certificate_uri: str
         :keyword ssl_host_name_in_certificate: Gets or sets the hostname(s) in the SSL certificate.
         :paramtype ssl_host_name_in_certificate: str
         :keyword ssl_preference: Gets or sets certificate preference if secure communication is
          enabled. Known values are: "Disabled", "RootCertificate", and "ServerCertificate".
         :paramtype ssl_preference: str or ~azure.mgmt.workloads.models.SslPreference
+        :keyword sap_sid: Gets or sets the SAP System Identifier.
+        :paramtype sap_sid: str
         """
         super().__init__(**kwargs)
         self.provider_type: str = "SapHana"
         self.hostname = hostname
         self.db_name = db_name
         self.sql_port = sql_port
         self.instance_number = instance_number
         self.db_username = db_username
         self.db_password = db_password
         self.db_password_uri = db_password_uri
-        self.db_ssl_certificate_uri = db_ssl_certificate_uri
         self.ssl_certificate_uri = ssl_certificate_uri
         self.ssl_host_name_in_certificate = ssl_host_name_in_certificate
         self.ssl_preference = ssl_preference
+        self.sap_sid = sap_sid
 
 
 class HighAvailabilityConfiguration(_serialization.Model):
     """Gets or sets the high availability configuration.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -1394,15 +1521,15 @@
         "high_availability_type": {"required": True},
     }
 
     _attribute_map = {
         "high_availability_type": {"key": "highAvailabilityType", "type": "str"},
     }
 
-    def __init__(self, *, high_availability_type: Union[str, "_models.SAPHighAvailabilityType"], **kwargs):
+    def __init__(self, *, high_availability_type: Union[str, "_models.SAPHighAvailabilityType"], **kwargs: Any) -> None:
         """
         :keyword high_availability_type: The high availability type. Required. Known values are:
          "AvailabilitySet" and "AvailabilityZone".
         :paramtype high_availability_type: str or ~azure.mgmt.workloads.models.SAPHighAvailabilityType
         """
         super().__init__(**kwargs)
         self.high_availability_type = high_availability_type
@@ -1426,29 +1553,33 @@
     }
 
     _attribute_map = {
         "fencing_client_id": {"key": "fencingClientId", "type": "str"},
         "fencing_client_password": {"key": "fencingClientPassword", "type": "str"},
     }
 
-    def __init__(self, *, fencing_client_id: str, fencing_client_password: str, **kwargs):
+    def __init__(self, *, fencing_client_id: str, fencing_client_password: str, **kwargs: Any) -> None:
         """
         :keyword fencing_client_id: The fencing client id. Required.
         :paramtype fencing_client_id: str
         :keyword fencing_client_password: The fencing client id secret/password. The secret should
          never expire. This will be used pacemaker to start/stop the cluster VMs. Required.
         :paramtype fencing_client_password: str
         """
         super().__init__(**kwargs)
         self.fencing_client_id = fencing_client_id
         self.fencing_client_password = fencing_client_password
 
 
 class ImageReference(_serialization.Model):
-    """Specifies information about the image to use. You can specify information about platform images, marketplace images, or virtual machine images. This element is required when you want to use a platform image, marketplace image, or virtual machine image, but is not used in other creation operations. NOTE: Image reference publisher and offer can only be set when you create the scale set.
+    """Specifies information about the image to use. You can specify information about platform
+    images, marketplace images, or virtual machine images. This element is required when you want
+    to use a platform image, marketplace image, or virtual machine image, but is not used in other
+    creation operations. NOTE: Image reference publisher and offer can only be set when you create
+    the scale set.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar publisher: The image publisher.
     :vartype publisher: str
     :ivar offer: Specifies the offer of the platform image or marketplace image used to create the
      virtual machine.
@@ -1487,16 +1618,16 @@
         self,
         *,
         publisher: Optional[str] = None,
         offer: Optional[str] = None,
         sku: Optional[str] = None,
         version: Optional[str] = None,
         shared_gallery_image_id: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword publisher: The image publisher.
         :paramtype publisher: str
         :keyword offer: Specifies the offer of the platform image or marketplace image used to create
          the virtual machine.
         :paramtype offer: str
         :keyword sku: The image SKU.
@@ -1546,15 +1677,15 @@
         "app_resource_group": {"key": "appResourceGroup", "type": "str"},
     }
 
     _subtype_map = {
         "deployment_type": {"SingleServer": "SingleServerConfiguration", "ThreeTier": "ThreeTierConfiguration"}
     }
 
-    def __init__(self, *, app_resource_group: str, **kwargs):
+    def __init__(self, *, app_resource_group: str, **kwargs: Any) -> None:
         """
         :keyword app_resource_group: The application resource group where SAP system resources will be
          deployed. Required.
         :paramtype app_resource_group: str
         """
         super().__init__(**kwargs)
         self.deployment_type: Optional[str] = None
@@ -1579,22 +1710,25 @@
 
     _attribute_map = {
         "os_type": {"key": "osType", "type": "str"},
     }
 
     _subtype_map = {"os_type": {"Linux": "LinuxConfiguration", "Windows": "WindowsConfiguration"}}
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.os_type: Optional[str] = None
 
 
 class LinuxConfiguration(OSConfiguration):
-    """Specifies the Linux operating system settings on the virtual machine. :code:`<br>`:code:`<br>`For a list of supported Linux distributions, see `Linux on Azure-Endorsed Distributions <https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros>`_.
+    """Specifies the Linux operating system settings on the virtual machine.
+    :code:`<br>`:code:`<br>`For a list of supported Linux distributions, see `Linux on
+    Azure-Endorsed Distributions
+    <https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros>`_.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar os_type: The OS Type. Required. Known values are: "Linux" and "Windows".
     :vartype os_type: str or ~azure.mgmt.workloads.models.OSType
     :ivar disable_password_authentication: Specifies whether password authentication should be
      disabled.
@@ -1619,16 +1753,16 @@
 
     def __init__(
         self,
         *,
         disable_password_authentication: Optional[bool] = None,
         ssh: Optional["_models.SshConfiguration"] = None,
         ssh_key_pair: Optional["_models.SshKeyPair"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword disable_password_authentication: Specifies whether password authentication should be
          disabled.
         :paramtype disable_password_authentication: bool
         :keyword ssh: Specifies the ssh key configuration for a Linux OS. (This property is deprecated,
          please use 'sshKeyPair' instead).
         :paramtype ssh: ~azure.mgmt.workloads.models.SshConfiguration
@@ -1638,26 +1772,110 @@
         super().__init__(**kwargs)
         self.os_type: str = "Linux"
         self.disable_password_authentication = disable_password_authentication
         self.ssh = ssh
         self.ssh_key_pair = ssh_key_pair
 
 
+class LoadBalancerDetails(_serialization.Model):
+    """The Load Balancer details such as Load Balancer ID.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id:
+    :vartype id: str
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.id = None
+
+
+class LoadBalancerResourceNames(_serialization.Model):
+    """The resource names object for load balancer and related resources.
+
+    :ivar load_balancer_name: The full resource name for load balancer. If this value is not
+     provided, load balancer will be name as {ASCS/DB}-loadBalancer.
+    :vartype load_balancer_name: str
+    :ivar frontend_ip_configuration_names: The list of frontend IP configuration names. If provided
+     as input, size of this list should be 2 for cs layer and should be 1 for database layer.
+    :vartype frontend_ip_configuration_names: list[str]
+    :ivar backend_pool_names: The list of backend pool names. Currently, ACSS deploys only one
+     backend pool and hence, size of this list should be 1.
+    :vartype backend_pool_names: list[str]
+    :ivar health_probe_names: The list of health probe names. If provided as input, size of this
+     list should be 2 for cs layer and should be 1 for database layer.
+    :vartype health_probe_names: list[str]
+    """
+
+    _validation = {
+        "frontend_ip_configuration_names": {"max_items": 2, "min_items": 0},
+        "backend_pool_names": {"max_items": 1, "min_items": 0},
+        "health_probe_names": {"max_items": 2, "min_items": 0},
+    }
+
+    _attribute_map = {
+        "load_balancer_name": {"key": "loadBalancerName", "type": "str"},
+        "frontend_ip_configuration_names": {"key": "frontendIpConfigurationNames", "type": "[str]"},
+        "backend_pool_names": {"key": "backendPoolNames", "type": "[str]"},
+        "health_probe_names": {"key": "healthProbeNames", "type": "[str]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        load_balancer_name: Optional[str] = None,
+        frontend_ip_configuration_names: Optional[List[str]] = None,
+        backend_pool_names: Optional[List[str]] = None,
+        health_probe_names: Optional[List[str]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword load_balancer_name: The full resource name for load balancer. If this value is not
+         provided, load balancer will be name as {ASCS/DB}-loadBalancer.
+        :paramtype load_balancer_name: str
+        :keyword frontend_ip_configuration_names: The list of frontend IP configuration names. If
+         provided as input, size of this list should be 2 for cs layer and should be 1 for database
+         layer.
+        :paramtype frontend_ip_configuration_names: list[str]
+        :keyword backend_pool_names: The list of backend pool names. Currently, ACSS deploys only one
+         backend pool and hence, size of this list should be 1.
+        :paramtype backend_pool_names: list[str]
+        :keyword health_probe_names: The list of health probe names. If provided as input, size of this
+         list should be 2 for cs layer and should be 1 for database layer.
+        :paramtype health_probe_names: list[str]
+        """
+        super().__init__(**kwargs)
+        self.load_balancer_name = load_balancer_name
+        self.frontend_ip_configuration_names = frontend_ip_configuration_names
+        self.backend_pool_names = backend_pool_names
+        self.health_probe_names = health_probe_names
+
+
 class ManagedRGConfiguration(_serialization.Model):
     """Managed resource group configuration.
 
     :ivar name: Managed resource group name.
     :vartype name: str
     """
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
     }
 
-    def __init__(self, *, name: Optional[str] = None, **kwargs):
+    def __init__(self, *, name: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword name: Managed resource group name.
         :paramtype name: str
         """
         super().__init__(**kwargs)
         self.name = name
 
@@ -1700,15 +1918,15 @@
         "http_port": {"key": "httpPort", "type": "int"},
         "https_port": {"key": "httpsPort", "type": "int"},
         "hostname": {"key": "hostname", "type": "str"},
         "ip_address": {"key": "ipAddress", "type": "str"},
         "health": {"key": "health", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.ms_port = None
         self.internal_ms_port = None
         self.http_port = None
         self.https_port = None
         self.hostname = None
@@ -1744,25 +1962,26 @@
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.system_data = None
 
 
 class TrackedResource(Resource):
-    """The resource model definition for an Azure Resource Manager tracked top level resource which has 'tags' and a 'location'.
+    """The resource model definition for an Azure Resource Manager tracked top level resource which
+    has 'tags' and a 'location'.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
@@ -1794,15 +2013,15 @@
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
     }
 
-    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         """
         super().__init__(**kwargs)
@@ -1906,16 +2125,16 @@
         identity: Optional["_models.UserAssignedServiceIdentity"] = None,
         app_location: Optional[str] = None,
         routing_preference: Optional[Union[str, "_models.RoutingPreference"]] = None,
         zone_redundancy_preference: Optional[str] = None,
         managed_resource_group_configuration: Optional["_models.ManagedRGConfiguration"] = None,
         log_analytics_workspace_arm_id: Optional[str] = None,
         monitor_subnet: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword identity: Managed service identity (user assigned identities).
         :paramtype identity: ~azure.mgmt.workloads.models.UserAssignedServiceIdentity
@@ -1962,15 +2181,17 @@
     """
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Monitor]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.Monitor"]] = None, next_link: Optional[str] = None, **kwargs):
+    def __init__(
+        self, *, value: Optional[List["_models.Monitor"]] = None, next_link: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword value: The list of SAP monitors.
         :paramtype value: list[~azure.mgmt.workloads.models.Monitor]
         :keyword next_link: The URL to get the next set of SAP monitors.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
@@ -2008,19 +2229,60 @@
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
         "target": {"key": "target", "type": "str"},
         "details": {"key": "details", "type": "[Error]"},
         "inner_error": {"key": "innerError", "type": "ErrorInnerError"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
 
 
+class MountFileShareConfiguration(FileShareConfiguration):
+    """Gets or sets the file share configuration for externally mounted cases.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar configuration_type: The type of file share config. Required. Known values are: "Skip",
+     "CreateAndMount", and "Mount".
+    :vartype configuration_type: str or ~azure.mgmt.workloads.models.ConfigurationType
+    :ivar id: The fileshare resource ID. Required.
+    :vartype id: str
+    :ivar private_endpoint_id: The private endpoint resource ID. Required.
+    :vartype private_endpoint_id: str
+    """
+
+    _validation = {
+        "configuration_type": {"required": True},
+        "id": {"required": True},
+        "private_endpoint_id": {"required": True},
+    }
+
+    _attribute_map = {
+        "configuration_type": {"key": "configurationType", "type": "str"},
+        "id": {"key": "id", "type": "str"},
+        "private_endpoint_id": {"key": "privateEndpointId", "type": "str"},
+    }
+
+    def __init__(
+        self, *, id: str, private_endpoint_id: str, **kwargs: Any  # pylint: disable=redefined-builtin
+    ) -> None:
+        """
+        :keyword id: The fileshare resource ID. Required.
+        :paramtype id: str
+        :keyword private_endpoint_id: The private endpoint resource ID. Required.
+        :paramtype private_endpoint_id: str
+        """
+        super().__init__(**kwargs)
+        self.configuration_type: str = "Mount"
+        self.id = id
+        self.private_endpoint_id = private_endpoint_id
+
+
 class MsSqlServerProviderInstanceProperties(ProviderSpecificProperties):
     """Gets or sets the SQL server provider properties.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar provider_type: The provider type. For example, the value can be SapHana. Required.
     :vartype provider_type: str
@@ -2066,16 +2328,16 @@
         db_port: Optional[str] = None,
         db_username: Optional[str] = None,
         db_password: Optional[str] = None,
         db_password_uri: Optional[str] = None,
         sap_sid: Optional[str] = None,
         ssl_preference: Optional[Union[str, "_models.SslPreference"]] = None,
         ssl_certificate_uri: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword hostname: Gets or sets the SQL server host name.
         :paramtype hostname: str
         :keyword db_port: Gets or sets the database sql port.
         :paramtype db_port: str
         :keyword db_username: Gets or sets the database user name.
         :paramtype db_username: str
@@ -2112,180 +2374,52 @@
     :vartype is_secondary_ip_enabled: bool
     """
 
     _attribute_map = {
         "is_secondary_ip_enabled": {"key": "isSecondaryIpEnabled", "type": "bool"},
     }
 
-    def __init__(self, *, is_secondary_ip_enabled: bool = False, **kwargs):
+    def __init__(self, *, is_secondary_ip_enabled: bool = False, **kwargs: Any) -> None:
         """
         :keyword is_secondary_ip_enabled: Specifies whether a secondary IP address should be added to
          the network interface on all VMs of the SAP system being deployed.
         :paramtype is_secondary_ip_enabled: bool
         """
         super().__init__(**kwargs)
         self.is_secondary_ip_enabled = is_secondary_ip_enabled
 
 
-class NetworkProfile(_serialization.Model):
-    """Network profile.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar load_balancer_type: Load balancer type. Required. Known values are: "ApplicationGateway"
-     and "LoadBalancer".
-    :vartype load_balancer_type: str or ~azure.mgmt.workloads.models.LoadBalancerType
-    :ivar load_balancer_sku: Load balancer SKU.
-    :vartype load_balancer_sku: str
-    :ivar load_balancer_tier: Load balancer tier.
-    :vartype load_balancer_tier: str
-    :ivar capacity: Capacity, applicable only for Application Gateway.
-    :vartype capacity: int
-    :ivar azure_front_door_enabled: Whether to enable Azure front door. Known values are: "Enabled"
-     and "Disabled".
-    :vartype azure_front_door_enabled: str or ~azure.mgmt.workloads.models.AzureFrontDoorEnabled
-    :ivar v_net_resource_id: Virtual network resource Id.
-    :vartype v_net_resource_id: str
-    :ivar load_balancer_resource_id: Azure Loadbalancer or ApplicationGateway resource Id.
-    :vartype load_balancer_resource_id: str
-    :ivar azure_front_door_resource_id: Azure front door resource id.
-    :vartype azure_front_door_resource_id: str
-    :ivar front_end_public_ip_resource_id: Loadbalancer front-end IP address resource Id.
-    :vartype front_end_public_ip_resource_id: str
-    :ivar outbound_public_ip_resource_ids: List of outbound public IP resource IDs.
-    :vartype outbound_public_ip_resource_ids: list[str]
-    """
-
-    _validation = {
-        "load_balancer_type": {"required": True},
-        "v_net_resource_id": {"readonly": True},
-        "load_balancer_resource_id": {"readonly": True},
-        "azure_front_door_resource_id": {"readonly": True},
-        "front_end_public_ip_resource_id": {"readonly": True},
-        "outbound_public_ip_resource_ids": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "load_balancer_type": {"key": "loadBalancerType", "type": "str"},
-        "load_balancer_sku": {"key": "loadBalancerSku", "type": "str"},
-        "load_balancer_tier": {"key": "loadBalancerTier", "type": "str"},
-        "capacity": {"key": "capacity", "type": "int"},
-        "azure_front_door_enabled": {"key": "azureFrontDoorEnabled", "type": "str"},
-        "v_net_resource_id": {"key": "vNetResourceId", "type": "str"},
-        "load_balancer_resource_id": {"key": "loadBalancerResourceId", "type": "str"},
-        "azure_front_door_resource_id": {"key": "azureFrontDoorResourceId", "type": "str"},
-        "front_end_public_ip_resource_id": {"key": "frontEndPublicIpResourceId", "type": "str"},
-        "outbound_public_ip_resource_ids": {"key": "outboundPublicIpResourceIds", "type": "[str]"},
-    }
-
-    def __init__(
-        self,
-        *,
-        load_balancer_type: Union[str, "_models.LoadBalancerType"],
-        load_balancer_sku: Optional[str] = None,
-        load_balancer_tier: Optional[str] = None,
-        capacity: Optional[int] = None,
-        azure_front_door_enabled: Optional[Union[str, "_models.AzureFrontDoorEnabled"]] = None,
-        **kwargs
-    ):
-        """
-        :keyword load_balancer_type: Load balancer type. Required. Known values are:
-         "ApplicationGateway" and "LoadBalancer".
-        :paramtype load_balancer_type: str or ~azure.mgmt.workloads.models.LoadBalancerType
-        :keyword load_balancer_sku: Load balancer SKU.
-        :paramtype load_balancer_sku: str
-        :keyword load_balancer_tier: Load balancer tier.
-        :paramtype load_balancer_tier: str
-        :keyword capacity: Capacity, applicable only for Application Gateway.
-        :paramtype capacity: int
-        :keyword azure_front_door_enabled: Whether to enable Azure front door. Known values are:
-         "Enabled" and "Disabled".
-        :paramtype azure_front_door_enabled: str or ~azure.mgmt.workloads.models.AzureFrontDoorEnabled
-        """
-        super().__init__(**kwargs)
-        self.load_balancer_type = load_balancer_type
-        self.load_balancer_sku = load_balancer_sku
-        self.load_balancer_tier = load_balancer_tier
-        self.capacity = capacity
-        self.azure_front_door_enabled = azure_front_door_enabled
-        self.v_net_resource_id = None
-        self.load_balancer_resource_id = None
-        self.azure_front_door_resource_id = None
-        self.front_end_public_ip_resource_id = None
-        self.outbound_public_ip_resource_ids = None
-
-
-class NodeProfile(_serialization.Model):
-    """VM or VMSS node profile.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    All required parameters must be populated in order to send to Azure.
+class NetworkInterfaceResourceNames(_serialization.Model):
+    """The resource names object for network interface and related resources.
 
-    :ivar name: VM or VMSS name.
-    :vartype name: str
-    :ivar node_sku: VM SKU for node(s). Required.
-    :vartype node_sku: str
-    :ivar os_image: OS image used for creating the nodes. Required.
-    :vartype os_image: ~azure.mgmt.workloads.models.OsImageProfile
-    :ivar os_disk: OS disk details. Required.
-    :vartype os_disk: ~azure.mgmt.workloads.models.DiskInfo
-    :ivar data_disks: Data disks details. This property is not in use right now.
-    :vartype data_disks: list[~azure.mgmt.workloads.models.DiskInfo]
-    :ivar node_resource_ids: VM/VMSS resource ARM Ids.
-    :vartype node_resource_ids: list[str]
+    :ivar network_interface_name: The full name for network interface. If name is not provided,
+     service uses a default name based on the deployment type. For SingleServer, default name is
+     {SID}-Nic. In case of HA-AvZone systems, default name will be {SID}-{App/ASCS/DB}-Zone{A/B}-Nic
+     with an incrementor at the end in case of more than 1 instance per layer. For distributed and
+     HA-AvSet systems, default name will be {SID}-{App/ASCS/DB}-Nic with an incrementor at the end
+     in case of more than 1 instance per layer.
+    :vartype network_interface_name: str
     """
 
-    _validation = {
-        "node_sku": {"required": True},
-        "os_image": {"required": True},
-        "os_disk": {"required": True},
-        "node_resource_ids": {"readonly": True},
-    }
-
     _attribute_map = {
-        "name": {"key": "name", "type": "str"},
-        "node_sku": {"key": "nodeSku", "type": "str"},
-        "os_image": {"key": "osImage", "type": "OsImageProfile"},
-        "os_disk": {"key": "osDisk", "type": "DiskInfo"},
-        "data_disks": {"key": "dataDisks", "type": "[DiskInfo]"},
-        "node_resource_ids": {"key": "nodeResourceIds", "type": "[str]"},
+        "network_interface_name": {"key": "networkInterfaceName", "type": "str"},
     }
 
-    def __init__(
-        self,
-        *,
-        node_sku: str,
-        os_image: "_models.OsImageProfile",
-        os_disk: "_models.DiskInfo",
-        name: Optional[str] = None,
-        data_disks: Optional[List["_models.DiskInfo"]] = None,
-        **kwargs
-    ):
+    def __init__(self, *, network_interface_name: Optional[str] = None, **kwargs: Any) -> None:
         """
-        :keyword name: VM or VMSS name.
-        :paramtype name: str
-        :keyword node_sku: VM SKU for node(s). Required.
-        :paramtype node_sku: str
-        :keyword os_image: OS image used for creating the nodes. Required.
-        :paramtype os_image: ~azure.mgmt.workloads.models.OsImageProfile
-        :keyword os_disk: OS disk details. Required.
-        :paramtype os_disk: ~azure.mgmt.workloads.models.DiskInfo
-        :keyword data_disks: Data disks details. This property is not in use right now.
-        :paramtype data_disks: list[~azure.mgmt.workloads.models.DiskInfo]
+        :keyword network_interface_name: The full name for network interface. If name is not provided,
+         service uses a default name based on the deployment type. For SingleServer, default name is
+         {SID}-Nic. In case of HA-AvZone systems, default name will be {SID}-{App/ASCS/DB}-Zone{A/B}-Nic
+         with an incrementor at the end in case of more than 1 instance per layer. For distributed and
+         HA-AvSet systems, default name will be {SID}-{App/ASCS/DB}-Nic with an incrementor at the end
+         in case of more than 1 instance per layer.
+        :paramtype network_interface_name: str
         """
         super().__init__(**kwargs)
-        self.name = name
-        self.node_sku = node_sku
-        self.os_image = os_image
-        self.os_disk = os_disk
-        self.data_disks = data_disks
-        self.node_resource_ids = None
+        self.network_interface_name = network_interface_name
 
 
 class Operation(_serialization.Model):
     """Details of a REST API operation, returned from the Resource Provider Operations API.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -2317,15 +2451,15 @@
         "name": {"key": "name", "type": "str"},
         "is_data_action": {"key": "isDataAction", "type": "bool"},
         "display": {"key": "display", "type": "OperationDisplay"},
         "origin": {"key": "origin", "type": "str"},
         "action_type": {"key": "actionType", "type": "str"},
     }
 
-    def __init__(self, *, display: Optional["_models.OperationDisplay"] = None, **kwargs):
+    def __init__(self, *, display: Optional["_models.OperationDisplay"] = None, **kwargs: Any) -> None:
         """
         :keyword display: Localized display information for this particular operation.
         :paramtype display: ~azure.mgmt.workloads.models.OperationDisplay
         """
         super().__init__(**kwargs)
         self.name = None
         self.is_data_action = None
@@ -2363,25 +2497,26 @@
     _attribute_map = {
         "provider": {"key": "provider", "type": "str"},
         "resource": {"key": "resource", "type": "str"},
         "operation": {"key": "operation", "type": "str"},
         "description": {"key": "description", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.provider = None
         self.resource = None
         self.operation = None
         self.description = None
 
 
 class OperationListResult(_serialization.Model):
-    """A list of REST API operations supported by an Azure Resource Provider. It contains an URL link to get the next set of results.
+    """A list of REST API operations supported by an Azure Resource Provider. It contains an URL link
+    to get the next set of results.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar value: List of operations supported by the resource provider.
     :vartype value: list[~azure.mgmt.workloads.models.Operation]
     :ivar next_link: URL to get the next set of operation list results (if there are any).
     :vartype next_link: str
@@ -2393,15 +2528,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Operation]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.value = None
         self.next_link = None
 
 
 class OperationsContent(Resource):
@@ -2461,16 +2596,16 @@
         *,
         name_properties_name: Optional[str] = None,
         is_data_action: Optional[bool] = None,
         origin: Optional[Union[str, "_models.OperationProperties"]] = None,
         display: Optional["_models.OperationsDefinitionDisplay"] = None,
         action_type: Optional[Union[str, "_models.WorkloadMonitorActionType"]] = None,
         properties: Optional[Any] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name_properties_name: Name of the operation.
         :paramtype name_properties_name: str
         :keyword is_data_action: Indicates whether the operation applies to data-plane.
         :paramtype is_data_action: bool
         :keyword origin: Defines the workload operation origin. Known values are: "NotSpecified",
          "User", and "System".
@@ -2532,16 +2667,16 @@
         *,
         name: str,
         display: "_models.OperationsDefinitionDisplay",
         is_data_action: Optional[bool] = None,
         origin: Optional[Union[str, "_models.OperationProperties"]] = None,
         action_type: Optional[Union[str, "_models.WorkloadMonitorActionType"]] = None,
         properties: Optional[Any] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Name of the operation. Required.
         :paramtype name: str
         :keyword is_data_action: Indicates whether the operation applies to data-plane.
         :paramtype is_data_action: bool
         :keyword origin: Defines the workload operation origin. Known values are: "NotSpecified",
          "User", and "System".
@@ -2574,16 +2709,20 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[OperationsDefinition]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.OperationsDefinition"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        value: Optional[List["_models.OperationsDefinition"]] = None,
+        next_link: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: Defines the workload operation definition response properties.
         :paramtype value: list[~azure.mgmt.workloads.models.OperationsDefinition]
         :keyword next_link: The URL to get to the next set of results, if there are any.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
@@ -2616,15 +2755,15 @@
     _attribute_map = {
         "provider": {"key": "provider", "type": "str"},
         "resource": {"key": "resource", "type": "str"},
         "operation": {"key": "operation", "type": "str"},
         "description": {"key": "description", "type": "str"},
     }
 
-    def __init__(self, *, provider: str, resource: str, operation: str, description: str, **kwargs):
+    def __init__(self, *, provider: str, resource: str, operation: str, description: str, **kwargs: Any) -> None:
         """
         :keyword provider: Defines the workload provider. Required.
         :paramtype provider: str
         :keyword resource: Defines the workload resource. Required.
         :paramtype resource: str
         :keyword operation: Defines the workload operation. Required.
         :paramtype operation: str
@@ -2663,15 +2802,15 @@
     _attribute_map = {
         "provider": {"key": "provider", "type": "str"},
         "resource": {"key": "resource", "type": "str"},
         "operation": {"key": "operation", "type": "str"},
         "description": {"key": "description", "type": "str"},
     }
 
-    def __init__(self, *, provider: str, resource: str, operation: str, description: str, **kwargs):
+    def __init__(self, *, provider: str, resource: str, operation: str, description: str, **kwargs: Any) -> None:
         """
         :keyword provider: Defines the workload provider. Required.
         :paramtype provider: str
         :keyword resource: Defines the workload resource. Required.
         :paramtype resource: str
         :keyword operation: Defines the workload operation. Required.
         :paramtype operation: str
@@ -2727,16 +2866,16 @@
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         name: Optional[str] = None,
         percent_complete: Optional[float] = None,
         start_time: Optional[datetime.datetime] = None,
         end_time: Optional[datetime.datetime] = None,
         operations: Optional[List["_models.OperationStatusResult"]] = None,
         error: Optional["_models.ErrorDetail"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword id: Fully qualified ID for the async operation.
         :paramtype id: str
         :keyword name: Name of the async operation.
         :paramtype name: str
         :keyword status: Operation status. Required.
         :paramtype status: str
@@ -2758,62 +2897,17 @@
         self.percent_complete = percent_complete
         self.start_time = start_time
         self.end_time = end_time
         self.operations = operations
         self.error = error
 
 
-class OsImageProfile(_serialization.Model):
-    """OS image profile.
-
-    :ivar publisher: OS image publisher. "Canonical"
-    :vartype publisher: str or ~azure.mgmt.workloads.models.OSImagePublisher
-    :ivar offer: OS image offer. "UbuntuServer"
-    :vartype offer: str or ~azure.mgmt.workloads.models.OSImageOffer
-    :ivar sku: OS image sku. Known values are: "18.04-LTS" and "16.04-LTS".
-    :vartype sku: str or ~azure.mgmt.workloads.models.OSImageSku
-    :ivar version: OS image version. "latest"
-    :vartype version: str or ~azure.mgmt.workloads.models.OSImageVersion
-    """
-
-    _attribute_map = {
-        "publisher": {"key": "publisher", "type": "str"},
-        "offer": {"key": "offer", "type": "str"},
-        "sku": {"key": "sku", "type": "str"},
-        "version": {"key": "version", "type": "str"},
-    }
-
-    def __init__(
-        self,
-        *,
-        publisher: Optional[Union[str, "_models.OSImagePublisher"]] = None,
-        offer: Optional[Union[str, "_models.OSImageOffer"]] = None,
-        sku: Optional[Union[str, "_models.OSImageSku"]] = None,
-        version: Optional[Union[str, "_models.OSImageVersion"]] = None,
-        **kwargs
-    ):
-        """
-        :keyword publisher: OS image publisher. "Canonical"
-        :paramtype publisher: str or ~azure.mgmt.workloads.models.OSImagePublisher
-        :keyword offer: OS image offer. "UbuntuServer"
-        :paramtype offer: str or ~azure.mgmt.workloads.models.OSImageOffer
-        :keyword sku: OS image sku. Known values are: "18.04-LTS" and "16.04-LTS".
-        :paramtype sku: str or ~azure.mgmt.workloads.models.OSImageSku
-        :keyword version: OS image version. "latest"
-        :paramtype version: str or ~azure.mgmt.workloads.models.OSImageVersion
-        """
-        super().__init__(**kwargs)
-        self.publisher = publisher
-        self.offer = offer
-        self.sku = sku
-        self.version = version
-
-
 class OSProfile(_serialization.Model):
-    """Specifies the operating system settings for the virtual machine. Some of the settings cannot be changed once VM is provisioned.
+    """Specifies the operating system settings for the virtual machine. Some of the settings cannot be
+    changed once VM is provisioned.
 
     :ivar admin_username: Specifies the name of the administrator account. :code:`<br>`:code:`<br>`
      This property cannot be updated after the VM is created. :code:`<br>`:code:`<br>`
      **Windows-only restriction:** Cannot end in "." :code:`<br>`:code:`<br>` **Disallowed values:**
      "administrator", "admin", "user", "user1", "test", "user2", "test1", "user3", "admin1", "1",
      "123", "a", "actuser", "adm", "admin2", "aspnet", "backup", "console", "david", "guest",
      "john", "owner", "root", "server", "sql", "support", "support_388945a0", "sys", "test2",
@@ -2848,16 +2942,16 @@
 
     def __init__(
         self,
         *,
         admin_username: Optional[str] = None,
         admin_password: Optional[str] = None,
         os_configuration: Optional["_models.OSConfiguration"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword admin_username: Specifies the name of the administrator account.
          :code:`<br>`:code:`<br>` This property cannot be updated after the VM is created.
          :code:`<br>`:code:`<br>` **Windows-only restriction:** Cannot end in "."
          :code:`<br>`:code:`<br>` **Disallowed values:** "administrator", "admin", "user", "user1",
          "test", "user2", "test1", "user3", "admin1", "1", "123", "a", "actuser", "adm", "admin2",
          "aspnet", "backup", "console", "david", "guest", "john", "owner", "root", "server", "sql",
@@ -2906,413 +3000,28 @@
     }
 
     def __init__(
         self,
         *,
         deployer_vm_packages: Optional["_models.DeployerVmPackages"] = None,
         sap_fqdn: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword deployer_vm_packages: The url and storage account ID where deployer VM packages are
          uploaded.
         :paramtype deployer_vm_packages: ~azure.mgmt.workloads.models.DeployerVmPackages
         :keyword sap_fqdn: The FQDN to set for the SAP system.
         :paramtype sap_fqdn: str
         """
         super().__init__(**kwargs)
         self.deployer_vm_packages = deployer_vm_packages
         self.sap_fqdn = sap_fqdn
 
 
-class PatchResourceRequestBody(_serialization.Model):
-    """Resource patch request body.
-
-    :ivar tags: Resource tags.
-    :vartype tags: dict[str, str]
-    :ivar identity:
-    :vartype identity: ~azure.mgmt.workloads.models.PatchResourceRequestBodyIdentity
-    """
-
-    _attribute_map = {
-        "tags": {"key": "tags", "type": "{str}"},
-        "identity": {"key": "identity", "type": "PatchResourceRequestBodyIdentity"},
-    }
-
-    def __init__(
-        self,
-        *,
-        tags: Optional[Dict[str, str]] = None,
-        identity: Optional["_models.PatchResourceRequestBodyIdentity"] = None,
-        **kwargs
-    ):
-        """
-        :keyword tags: Resource tags.
-        :paramtype tags: dict[str, str]
-        :keyword identity:
-        :paramtype identity: ~azure.mgmt.workloads.models.PatchResourceRequestBodyIdentity
-        """
-        super().__init__(**kwargs)
-        self.tags = tags
-        self.identity = identity
-
-
-class UserAssignedServiceIdentity(_serialization.Model):
-    """Managed service identity (user assigned identities).
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar type: Type of manage identity. Required. Known values are: "None" and "UserAssigned".
-    :vartype type: str or ~azure.mgmt.workloads.models.ManagedServiceIdentityType
-    :ivar user_assigned_identities: User assigned identities dictionary.
-    :vartype user_assigned_identities: dict[str, ~azure.mgmt.workloads.models.UserAssignedIdentity]
-    """
-
-    _validation = {
-        "type": {"required": True},
-    }
-
-    _attribute_map = {
-        "type": {"key": "type", "type": "str"},
-        "user_assigned_identities": {"key": "userAssignedIdentities", "type": "{UserAssignedIdentity}"},
-    }
-
-    def __init__(
-        self,
-        *,
-        type: Union[str, "_models.ManagedServiceIdentityType"],
-        user_assigned_identities: Optional[Dict[str, "_models.UserAssignedIdentity"]] = None,
-        **kwargs
-    ):
-        """
-        :keyword type: Type of manage identity. Required. Known values are: "None" and "UserAssigned".
-        :paramtype type: str or ~azure.mgmt.workloads.models.ManagedServiceIdentityType
-        :keyword user_assigned_identities: User assigned identities dictionary.
-        :paramtype user_assigned_identities: dict[str,
-         ~azure.mgmt.workloads.models.UserAssignedIdentity]
-        """
-        super().__init__(**kwargs)
-        self.type = type
-        self.user_assigned_identities = user_assigned_identities
-
-
-class PatchResourceRequestBodyIdentity(UserAssignedServiceIdentity):
-    """PatchResourceRequestBodyIdentity.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar type: Type of manage identity. Required. Known values are: "None" and "UserAssigned".
-    :vartype type: str or ~azure.mgmt.workloads.models.ManagedServiceIdentityType
-    :ivar user_assigned_identities: User assigned identities dictionary.
-    :vartype user_assigned_identities: dict[str, ~azure.mgmt.workloads.models.UserAssignedIdentity]
-    """
-
-    _validation = {
-        "type": {"required": True},
-    }
-
-    _attribute_map = {
-        "type": {"key": "type", "type": "str"},
-        "user_assigned_identities": {"key": "userAssignedIdentities", "type": "{UserAssignedIdentity}"},
-    }
-
-    def __init__(
-        self,
-        *,
-        type: Union[str, "_models.ManagedServiceIdentityType"],
-        user_assigned_identities: Optional[Dict[str, "_models.UserAssignedIdentity"]] = None,
-        **kwargs
-    ):
-        """
-        :keyword type: Type of manage identity. Required. Known values are: "None" and "UserAssigned".
-        :paramtype type: str or ~azure.mgmt.workloads.models.ManagedServiceIdentityType
-        :keyword user_assigned_identities: User assigned identities dictionary.
-        :paramtype user_assigned_identities: dict[str,
-         ~azure.mgmt.workloads.models.UserAssignedIdentity]
-        """
-        super().__init__(type=type, user_assigned_identities=user_assigned_identities, **kwargs)
-
-
-class PhpProfile(_serialization.Model):
-    """PHP profile.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar version: PHP version. Required. Known values are: "7.2", "7.3", and "7.4".
-    :vartype version: str or ~azure.mgmt.workloads.models.PHPVersion
-    """
-
-    _validation = {
-        "version": {"required": True},
-    }
-
-    _attribute_map = {
-        "version": {"key": "version", "type": "str"},
-    }
-
-    def __init__(self, *, version: Union[str, "_models.PHPVersion"], **kwargs):
-        """
-        :keyword version: PHP version. Required. Known values are: "7.2", "7.3", and "7.4".
-        :paramtype version: str or ~azure.mgmt.workloads.models.PHPVersion
-        """
-        super().__init__(**kwargs)
-        self.version = version
-
-
-class PhpWorkloadResource(TrackedResource):  # pylint: disable=too-many-instance-attributes
-    """Php workload resource.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    All required parameters must be populated in order to send to Azure.
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
-    :vartype system_data: ~azure.mgmt.workloads.models.SystemData
-    :ivar tags: Resource tags.
-    :vartype tags: dict[str, str]
-    :ivar location: The geo-location where the resource lives. Required.
-    :vartype location: str
-    :ivar kind: Indicates which kind of php workload this resource represent e.g WordPress.
-     Required. "WordPress"
-    :vartype kind: str or ~azure.mgmt.workloads.models.WorkloadKind
-    :ivar sku: Php workloads SKU.
-    :vartype sku: ~azure.mgmt.workloads.models.Sku
-    :ivar identity: Identity for the resource. Currently not supported.
-    :vartype identity: ~azure.mgmt.workloads.models.PhpWorkloadResourceIdentity
-    :ivar app_location: The infra resources for PHP workload will be created in this location.
-    :vartype app_location: str
-    :ivar managed_resource_group_configuration: Managed resource group configuration of the
-     workload.
-    :vartype managed_resource_group_configuration:
-     ~azure.mgmt.workloads.models.ManagedRGConfiguration
-    :ivar admin_user_profile: Admin user profile used for VM and VMSS.
-    :vartype admin_user_profile: ~azure.mgmt.workloads.models.UserProfile
-    :ivar web_nodes_profile: VMSS web nodes profile.
-    :vartype web_nodes_profile: ~azure.mgmt.workloads.models.VmssNodesProfile
-    :ivar controller_profile: Controller VM profile.
-    :vartype controller_profile: ~azure.mgmt.workloads.models.NodeProfile
-    :ivar network_profile: Network profile.
-    :vartype network_profile: ~azure.mgmt.workloads.models.NetworkProfile
-    :ivar database_profile: Database profile.
-    :vartype database_profile: ~azure.mgmt.workloads.models.DatabaseProfile
-    :ivar site_profile: Site profile.
-    :vartype site_profile: ~azure.mgmt.workloads.models.SiteProfile
-    :ivar fileshare_profile: File share profile.
-    :vartype fileshare_profile: ~azure.mgmt.workloads.models.FileshareProfile
-    :ivar php_profile: PHP profile.
-    :vartype php_profile: ~azure.mgmt.workloads.models.PhpProfile
-    :ivar search_profile: Search profile.
-    :vartype search_profile: ~azure.mgmt.workloads.models.SearchProfile
-    :ivar cache_profile: Cache profile.
-    :vartype cache_profile: ~azure.mgmt.workloads.models.CacheProfile
-    :ivar backup_profile: Backup profile.
-    :vartype backup_profile: ~azure.mgmt.workloads.models.BackupProfile
-    :ivar provisioning_state: Php workload resource provisioning state. Known values are:
-     "NotSpecified", "Accepted", "Created", "Succeeded", "Failed", "Canceled", "Provisioning", and
-     "Deleting".
-    :vartype provisioning_state: str or ~azure.mgmt.workloads.models.PhpWorkloadProvisioningState
-    """
-
-    _validation = {
-        "id": {"readonly": True},
-        "name": {"readonly": True},
-        "type": {"readonly": True},
-        "system_data": {"readonly": True},
-        "location": {"required": True},
-        "kind": {"required": True},
-        "provisioning_state": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "id": {"key": "id", "type": "str"},
-        "name": {"key": "name", "type": "str"},
-        "type": {"key": "type", "type": "str"},
-        "system_data": {"key": "systemData", "type": "SystemData"},
-        "tags": {"key": "tags", "type": "{str}"},
-        "location": {"key": "location", "type": "str"},
-        "kind": {"key": "kind", "type": "str"},
-        "sku": {"key": "sku", "type": "Sku"},
-        "identity": {"key": "identity", "type": "PhpWorkloadResourceIdentity"},
-        "app_location": {"key": "properties.appLocation", "type": "str"},
-        "managed_resource_group_configuration": {
-            "key": "properties.managedResourceGroupConfiguration",
-            "type": "ManagedRGConfiguration",
-        },
-        "admin_user_profile": {"key": "properties.adminUserProfile", "type": "UserProfile"},
-        "web_nodes_profile": {"key": "properties.webNodesProfile", "type": "VmssNodesProfile"},
-        "controller_profile": {"key": "properties.controllerProfile", "type": "NodeProfile"},
-        "network_profile": {"key": "properties.networkProfile", "type": "NetworkProfile"},
-        "database_profile": {"key": "properties.databaseProfile", "type": "DatabaseProfile"},
-        "site_profile": {"key": "properties.siteProfile", "type": "SiteProfile"},
-        "fileshare_profile": {"key": "properties.fileshareProfile", "type": "FileshareProfile"},
-        "php_profile": {"key": "properties.phpProfile", "type": "PhpProfile"},
-        "search_profile": {"key": "properties.searchProfile", "type": "SearchProfile"},
-        "cache_profile": {"key": "properties.cacheProfile", "type": "CacheProfile"},
-        "backup_profile": {"key": "properties.backupProfile", "type": "BackupProfile"},
-        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
-    }
-
-    def __init__(
-        self,
-        *,
-        location: str,
-        kind: Union[str, "_models.WorkloadKind"],
-        tags: Optional[Dict[str, str]] = None,
-        sku: Optional["_models.Sku"] = None,
-        identity: Optional["_models.PhpWorkloadResourceIdentity"] = None,
-        app_location: Optional[str] = None,
-        managed_resource_group_configuration: Optional["_models.ManagedRGConfiguration"] = None,
-        admin_user_profile: Optional["_models.UserProfile"] = None,
-        web_nodes_profile: Optional["_models.VmssNodesProfile"] = None,
-        controller_profile: Optional["_models.NodeProfile"] = None,
-        network_profile: Optional["_models.NetworkProfile"] = None,
-        database_profile: Optional["_models.DatabaseProfile"] = None,
-        site_profile: Optional["_models.SiteProfile"] = None,
-        fileshare_profile: Optional["_models.FileshareProfile"] = None,
-        php_profile: Optional["_models.PhpProfile"] = None,
-        search_profile: Optional["_models.SearchProfile"] = None,
-        cache_profile: Optional["_models.CacheProfile"] = None,
-        backup_profile: Optional["_models.BackupProfile"] = None,
-        **kwargs
-    ):
-        """
-        :keyword tags: Resource tags.
-        :paramtype tags: dict[str, str]
-        :keyword location: The geo-location where the resource lives. Required.
-        :paramtype location: str
-        :keyword kind: Indicates which kind of php workload this resource represent e.g WordPress.
-         Required. "WordPress"
-        :paramtype kind: str or ~azure.mgmt.workloads.models.WorkloadKind
-        :keyword sku: Php workloads SKU.
-        :paramtype sku: ~azure.mgmt.workloads.models.Sku
-        :keyword identity: Identity for the resource. Currently not supported.
-        :paramtype identity: ~azure.mgmt.workloads.models.PhpWorkloadResourceIdentity
-        :keyword app_location: The infra resources for PHP workload will be created in this location.
-        :paramtype app_location: str
-        :keyword managed_resource_group_configuration: Managed resource group configuration of the
-         workload.
-        :paramtype managed_resource_group_configuration:
-         ~azure.mgmt.workloads.models.ManagedRGConfiguration
-        :keyword admin_user_profile: Admin user profile used for VM and VMSS.
-        :paramtype admin_user_profile: ~azure.mgmt.workloads.models.UserProfile
-        :keyword web_nodes_profile: VMSS web nodes profile.
-        :paramtype web_nodes_profile: ~azure.mgmt.workloads.models.VmssNodesProfile
-        :keyword controller_profile: Controller VM profile.
-        :paramtype controller_profile: ~azure.mgmt.workloads.models.NodeProfile
-        :keyword network_profile: Network profile.
-        :paramtype network_profile: ~azure.mgmt.workloads.models.NetworkProfile
-        :keyword database_profile: Database profile.
-        :paramtype database_profile: ~azure.mgmt.workloads.models.DatabaseProfile
-        :keyword site_profile: Site profile.
-        :paramtype site_profile: ~azure.mgmt.workloads.models.SiteProfile
-        :keyword fileshare_profile: File share profile.
-        :paramtype fileshare_profile: ~azure.mgmt.workloads.models.FileshareProfile
-        :keyword php_profile: PHP profile.
-        :paramtype php_profile: ~azure.mgmt.workloads.models.PhpProfile
-        :keyword search_profile: Search profile.
-        :paramtype search_profile: ~azure.mgmt.workloads.models.SearchProfile
-        :keyword cache_profile: Cache profile.
-        :paramtype cache_profile: ~azure.mgmt.workloads.models.CacheProfile
-        :keyword backup_profile: Backup profile.
-        :paramtype backup_profile: ~azure.mgmt.workloads.models.BackupProfile
-        """
-        super().__init__(tags=tags, location=location, **kwargs)
-        self.kind = kind
-        self.sku = sku
-        self.identity = identity
-        self.app_location = app_location
-        self.managed_resource_group_configuration = managed_resource_group_configuration
-        self.admin_user_profile = admin_user_profile
-        self.web_nodes_profile = web_nodes_profile
-        self.controller_profile = controller_profile
-        self.network_profile = network_profile
-        self.database_profile = database_profile
-        self.site_profile = site_profile
-        self.fileshare_profile = fileshare_profile
-        self.php_profile = php_profile
-        self.search_profile = search_profile
-        self.cache_profile = cache_profile
-        self.backup_profile = backup_profile
-        self.provisioning_state = None
-
-
-class PhpWorkloadResourceIdentity(UserAssignedServiceIdentity):
-    """Identity for the resource. Currently not supported.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar type: Type of manage identity. Required. Known values are: "None" and "UserAssigned".
-    :vartype type: str or ~azure.mgmt.workloads.models.ManagedServiceIdentityType
-    :ivar user_assigned_identities: User assigned identities dictionary.
-    :vartype user_assigned_identities: dict[str, ~azure.mgmt.workloads.models.UserAssignedIdentity]
-    """
-
-    _validation = {
-        "type": {"required": True},
-    }
-
-    _attribute_map = {
-        "type": {"key": "type", "type": "str"},
-        "user_assigned_identities": {"key": "userAssignedIdentities", "type": "{UserAssignedIdentity}"},
-    }
-
-    def __init__(
-        self,
-        *,
-        type: Union[str, "_models.ManagedServiceIdentityType"],
-        user_assigned_identities: Optional[Dict[str, "_models.UserAssignedIdentity"]] = None,
-        **kwargs
-    ):
-        """
-        :keyword type: Type of manage identity. Required. Known values are: "None" and "UserAssigned".
-        :paramtype type: str or ~azure.mgmt.workloads.models.ManagedServiceIdentityType
-        :keyword user_assigned_identities: User assigned identities dictionary.
-        :paramtype user_assigned_identities: dict[str,
-         ~azure.mgmt.workloads.models.UserAssignedIdentity]
-        """
-        super().__init__(type=type, user_assigned_identities=user_assigned_identities, **kwargs)
-
-
-class PhpWorkloadResourceList(_serialization.Model):
-    """Php workload resource list.
-
-    :ivar value: List of resources in current page.
-    :vartype value: list[~azure.mgmt.workloads.models.PhpWorkloadResource]
-    :ivar next_link: Link to next page of resources.
-    :vartype next_link: str
-    """
-
-    _attribute_map = {
-        "value": {"key": "value", "type": "[PhpWorkloadResource]"},
-        "next_link": {"key": "nextLink", "type": "str"},
-    }
-
-    def __init__(
-        self, *, value: Optional[List["_models.PhpWorkloadResource"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
-        """
-        :keyword value: List of resources in current page.
-        :paramtype value: list[~azure.mgmt.workloads.models.PhpWorkloadResource]
-        :keyword next_link: Link to next page of resources.
-        :paramtype next_link: str
-        """
-        super().__init__(**kwargs)
-        self.value = value
-        self.next_link = next_link
-
-
 class PrometheusHaClusterProviderInstanceProperties(ProviderSpecificProperties):
     """Gets or sets the PrometheusHaCluster provider properties.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar provider_type: The provider type. For example, the value can be SapHana. Required.
     :vartype provider_type: str
@@ -3351,16 +3060,16 @@
         *,
         prometheus_url: Optional[str] = None,
         hostname: Optional[str] = None,
         sid: Optional[str] = None,
         cluster_name: Optional[str] = None,
         ssl_preference: Optional[Union[str, "_models.SslPreference"]] = None,
         ssl_certificate_uri: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword prometheus_url: URL of the Node Exporter endpoint.
         :paramtype prometheus_url: str
         :keyword hostname: Gets or sets the target machine name.
         :paramtype hostname: str
         :keyword sid: Gets or sets the cluster sid.
         :paramtype sid: str
@@ -3394,54 +3103,62 @@
     :vartype prometheus_url: str
     :ivar ssl_preference: Gets or sets certificate preference if secure communication is enabled.
      Known values are: "Disabled", "RootCertificate", and "ServerCertificate".
     :vartype ssl_preference: str or ~azure.mgmt.workloads.models.SslPreference
     :ivar ssl_certificate_uri: Gets or sets the blob URI to SSL certificate for the prometheus node
      exporter.
     :vartype ssl_certificate_uri: str
+    :ivar sap_sid: Gets or sets the SAP System Identifier.
+    :vartype sap_sid: str
     """
 
     _validation = {
         "provider_type": {"required": True},
     }
 
     _attribute_map = {
         "provider_type": {"key": "providerType", "type": "str"},
         "prometheus_url": {"key": "prometheusUrl", "type": "str"},
         "ssl_preference": {"key": "sslPreference", "type": "str"},
         "ssl_certificate_uri": {"key": "sslCertificateUri", "type": "str"},
+        "sap_sid": {"key": "sapSid", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         prometheus_url: Optional[str] = None,
         ssl_preference: Optional[Union[str, "_models.SslPreference"]] = None,
         ssl_certificate_uri: Optional[str] = None,
-        **kwargs
-    ):
+        sap_sid: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword prometheus_url: URL of the Node Exporter endpoint.
         :paramtype prometheus_url: str
         :keyword ssl_preference: Gets or sets certificate preference if secure communication is
          enabled. Known values are: "Disabled", "RootCertificate", and "ServerCertificate".
         :paramtype ssl_preference: str or ~azure.mgmt.workloads.models.SslPreference
         :keyword ssl_certificate_uri: Gets or sets the blob URI to SSL certificate for the prometheus
          node exporter.
         :paramtype ssl_certificate_uri: str
+        :keyword sap_sid: Gets or sets the SAP System Identifier.
+        :paramtype sap_sid: str
         """
         super().__init__(**kwargs)
         self.provider_type: str = "PrometheusOS"
         self.prometheus_url = prometheus_url
         self.ssl_preference = ssl_preference
         self.ssl_certificate_uri = ssl_certificate_uri
+        self.sap_sid = sap_sid
 
 
 class ProxyResource(Resource):
-    """The resource model definition for a Azure Resource Manager proxy resource. It will not have tags and a location.
+    """The resource model definition for a Azure Resource Manager proxy resource. It will not have
+    tags and a location.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
     :vartype id: str
     :ivar name: The name of the resource.
@@ -3464,15 +3181,15 @@
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
 
 
 class ProviderInstance(ProxyResource):
     """A provider instance associated with SAP monitor.
 
@@ -3522,16 +3239,16 @@
     }
 
     def __init__(
         self,
         *,
         identity: Optional["_models.UserAssignedServiceIdentity"] = None,
         provider_settings: Optional["_models.ProviderSpecificProperties"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword identity: Managed service identity (user assigned identities).
         :paramtype identity: ~azure.mgmt.workloads.models.UserAssignedServiceIdentity
         :keyword provider_settings: Defines the provider instance errors.
         :paramtype provider_settings: ~azure.mgmt.workloads.models.ProviderSpecificProperties
         """
         super().__init__(**kwargs)
@@ -3552,16 +3269,20 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[ProviderInstance]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.ProviderInstance"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        value: Optional[List["_models.ProviderInstance"]] = None,
+        next_link: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: The list of provider instances.
         :paramtype value: list[~azure.mgmt.workloads.models.ProviderInstance]
         :keyword next_link: The URL to get the next set of provider instances.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
@@ -3599,45 +3320,19 @@
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
         "target": {"key": "target", "type": "str"},
         "details": {"key": "details", "type": "[Error]"},
         "inner_error": {"key": "innerError", "type": "ErrorInnerError"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
 
 
-class RestrictionInfo(_serialization.Model):
-    """The SKU restriction information.
-
-    :ivar locations: The restriction locations.
-    :vartype locations: list[str]
-    :ivar zones: The restriction zones.
-    :vartype zones: list[str]
-    """
-
-    _attribute_map = {
-        "locations": {"key": "locations", "type": "[str]"},
-        "zones": {"key": "zones", "type": "[str]"},
-    }
-
-    def __init__(self, *, locations: Optional[List[str]] = None, zones: Optional[List[str]] = None, **kwargs):
-        """
-        :keyword locations: The restriction locations.
-        :paramtype locations: list[str]
-        :keyword zones: The restriction zones.
-        :paramtype zones: list[str]
-        """
-        super().__init__(**kwargs)
-        self.locations = locations
-        self.zones = zones
-
-
 class SAPApplicationServerInstance(TrackedResource):  # pylint: disable=too-many-instance-attributes
     """Define the SAP Application Server Instance resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -3670,18 +3365,21 @@
     :vartype ip_address: str
     :ivar gateway_port: Application server instance gateway Port.
     :vartype gateway_port: int
     :ivar icm_http_port: Application server instance ICM HTTP Port.
     :vartype icm_http_port: int
     :ivar icm_https_port: Application server instance ICM HTTPS Port.
     :vartype icm_https_port: int
-    :ivar virtual_machine_id: The virtual machine.
-    :vartype virtual_machine_id: str
+    :ivar load_balancer_details: The Load Balancer details such as LoadBalancer ID attached to
+     Application Server Virtual Machines.
+    :vartype load_balancer_details: ~azure.mgmt.workloads.models.LoadBalancerDetails
+    :ivar vm_details: The list of virtual machines.
+    :vartype vm_details: list[~azure.mgmt.workloads.models.ApplicationServerVmDetails]
     :ivar status: Defines the SAP Instance status. Known values are: "Starting", "Running",
-     "Stopping", "Offline", "PartiallyRunning", and "Unavailable".
+     "Stopping", "Offline", "PartiallyRunning", "Unavailable", and "SoftShutdown".
     :vartype status: str or ~azure.mgmt.workloads.models.SAPVirtualInstanceStatus
     :ivar health: Defines the health of SAP Instances. Known values are: "Unknown", "Healthy",
      "Unhealthy", and "Degraded".
     :vartype health: str or ~azure.mgmt.workloads.models.SAPHealthState
     :ivar provisioning_state: Defines the provisioning states. Known values are: "Succeeded",
      "Updating", "Creating", "Failed", and "Deleting".
     :vartype provisioning_state: str or
@@ -3701,15 +3399,16 @@
         "hostname": {"readonly": True},
         "kernel_version": {"readonly": True},
         "kernel_patch": {"readonly": True},
         "ip_address": {"readonly": True},
         "gateway_port": {"readonly": True},
         "icm_http_port": {"readonly": True},
         "icm_https_port": {"readonly": True},
-        "virtual_machine_id": {"readonly": True},
+        "load_balancer_details": {"readonly": True},
+        "vm_details": {"readonly": True},
         "status": {"readonly": True},
         "health": {"readonly": True},
         "provisioning_state": {"readonly": True},
         "errors": {"readonly": True},
     }
 
     _attribute_map = {
@@ -3724,22 +3423,23 @@
         "hostname": {"key": "properties.hostname", "type": "str"},
         "kernel_version": {"key": "properties.kernelVersion", "type": "str"},
         "kernel_patch": {"key": "properties.kernelPatch", "type": "str"},
         "ip_address": {"key": "properties.ipAddress", "type": "str"},
         "gateway_port": {"key": "properties.gatewayPort", "type": "int"},
         "icm_http_port": {"key": "properties.icmHttpPort", "type": "int"},
         "icm_https_port": {"key": "properties.icmHttpsPort", "type": "int"},
-        "virtual_machine_id": {"key": "properties.virtualMachineId", "type": "str"},
+        "load_balancer_details": {"key": "properties.loadBalancerDetails", "type": "LoadBalancerDetails"},
+        "vm_details": {"key": "properties.vmDetails", "type": "[ApplicationServerVmDetails]"},
         "status": {"key": "properties.status", "type": "str"},
         "health": {"key": "properties.health", "type": "str"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
         "errors": {"key": "properties.errors", "type": "SAPVirtualInstanceError"},
     }
 
-    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         """
         super().__init__(tags=tags, location=location, **kwargs)
@@ -3748,15 +3448,16 @@
         self.hostname = None
         self.kernel_version = None
         self.kernel_patch = None
         self.ip_address = None
         self.gateway_port = None
         self.icm_http_port = None
         self.icm_https_port = None
-        self.virtual_machine_id = None
+        self.load_balancer_details = None
+        self.vm_details = None
         self.status = None
         self.health = None
         self.provisioning_state = None
         self.errors = None
 
 
 class SAPApplicationServerInstanceList(_serialization.Model):
@@ -3774,16 +3475,16 @@
     }
 
     def __init__(
         self,
         *,
         value: Optional[List["_models.SAPApplicationServerInstance"]] = None,
         next_link: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: Gets the list of SAP Application Server instance resources.
         :paramtype value: list[~azure.mgmt.workloads.models.SAPApplicationServerInstance]
         :keyword next_link: Gets the value of next link.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
@@ -3820,16 +3521,16 @@
 
     def __init__(
         self,
         *,
         app_location: str,
         sap_product: Union[str, "_models.SAPProductType"],
         database_type: Union[str, "_models.SAPDatabaseType"],
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword app_location: The geo-location where the SAP resources will be created. Required.
         :paramtype app_location: str
         :keyword sap_product: Defines the SAP Product type. Required. Known values are: "ECC",
          "S4HANA", and "Other".
         :paramtype sap_product: str or ~azure.mgmt.workloads.models.SAPProductType
         :keyword database_type: The database type. Eg: HANA, DB2, etc. Required. Known values are:
@@ -3849,15 +3550,17 @@
     :vartype availability_zone_pairs: list[~azure.mgmt.workloads.models.SAPAvailabilityZonePair]
     """
 
     _attribute_map = {
         "availability_zone_pairs": {"key": "availabilityZonePairs", "type": "[SAPAvailabilityZonePair]"},
     }
 
-    def __init__(self, *, availability_zone_pairs: Optional[List["_models.SAPAvailabilityZonePair"]] = None, **kwargs):
+    def __init__(
+        self, *, availability_zone_pairs: Optional[List["_models.SAPAvailabilityZonePair"]] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword availability_zone_pairs: Gets the list of availability zone pairs.
         :paramtype availability_zone_pairs: list[~azure.mgmt.workloads.models.SAPAvailabilityZonePair]
         """
         super().__init__(**kwargs)
         self.availability_zone_pairs = availability_zone_pairs
 
@@ -3872,15 +3575,15 @@
     """
 
     _attribute_map = {
         "zone_a": {"key": "zoneA", "type": "int"},
         "zone_b": {"key": "zoneB", "type": "int"},
     }
 
-    def __init__(self, *, zone_a: Optional[int] = None, zone_b: Optional[int] = None, **kwargs):
+    def __init__(self, *, zone_a: Optional[int] = None, zone_b: Optional[int] = None, **kwargs: Any) -> None:
         """
         :keyword zone_a: The zone A.
         :paramtype zone_a: int
         :keyword zone_b: The zone B.
         :paramtype zone_b: int
         """
         super().__init__(**kwargs)
@@ -3903,16 +3606,16 @@
     }
 
     def __init__(
         self,
         *,
         value: Optional[List["_models.SAPCentralServerInstance"]] = None,
         next_link: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: Gets the list of SAP central services instance resources.
         :paramtype value: list[~azure.mgmt.workloads.models.SAPCentralServerInstance]
         :keyword next_link: Gets the value of next link.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
@@ -3956,18 +3659,21 @@
      properties.
     :vartype enqueue_replication_server_properties:
      ~azure.mgmt.workloads.models.EnqueueReplicationServerProperties
     :ivar kernel_version: The central services instance Kernel Version.
     :vartype kernel_version: str
     :ivar kernel_patch: The central services instance Kernel Patch level.
     :vartype kernel_patch: str
+    :ivar load_balancer_details: The Load Balancer details such as LoadBalancer ID attached to ASCS
+     Virtual Machines.
+    :vartype load_balancer_details: ~azure.mgmt.workloads.models.LoadBalancerDetails
     :ivar vm_details: The list of virtual machines corresponding to the Central Services instance.
     :vartype vm_details: list[~azure.mgmt.workloads.models.CentralServerVmDetails]
     :ivar status: Defines the SAP Instance status. Known values are: "Starting", "Running",
-     "Stopping", "Offline", "PartiallyRunning", and "Unavailable".
+     "Stopping", "Offline", "PartiallyRunning", "Unavailable", and "SoftShutdown".
     :vartype status: str or ~azure.mgmt.workloads.models.SAPVirtualInstanceStatus
     :ivar health: Defines the health of SAP Instances. Known values are: "Unknown", "Healthy",
      "Unhealthy", and "Degraded".
     :vartype health: str or ~azure.mgmt.workloads.models.SAPHealthState
     :ivar provisioning_state: Defines the provisioning states. Known values are: "Succeeded",
      "Updating", "Creating", "Failed", and "Deleting".
     :vartype provisioning_state: str or
@@ -3982,14 +3688,15 @@
         "type": {"readonly": True},
         "system_data": {"readonly": True},
         "location": {"required": True},
         "instance_no": {"readonly": True},
         "subnet": {"readonly": True},
         "kernel_version": {"readonly": True},
         "kernel_patch": {"readonly": True},
+        "load_balancer_details": {"readonly": True},
         "vm_details": {"readonly": True},
         "status": {"readonly": True},
         "health": {"readonly": True},
         "provisioning_state": {"readonly": True},
         "errors": {"readonly": True},
     }
 
@@ -4007,14 +3714,15 @@
         "gateway_server_properties": {"key": "properties.gatewayServerProperties", "type": "GatewayServerProperties"},
         "enqueue_replication_server_properties": {
             "key": "properties.enqueueReplicationServerProperties",
             "type": "EnqueueReplicationServerProperties",
         },
         "kernel_version": {"key": "properties.kernelVersion", "type": "str"},
         "kernel_patch": {"key": "properties.kernelPatch", "type": "str"},
+        "load_balancer_details": {"key": "properties.loadBalancerDetails", "type": "LoadBalancerDetails"},
         "vm_details": {"key": "properties.vmDetails", "type": "[CentralServerVmDetails]"},
         "status": {"key": "properties.status", "type": "str"},
         "health": {"key": "properties.health", "type": "str"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
         "errors": {"key": "properties.errors", "type": "SAPVirtualInstanceError"},
     }
 
@@ -4023,16 +3731,16 @@
         *,
         location: str,
         tags: Optional[Dict[str, str]] = None,
         message_server_properties: Optional["_models.MessageServerProperties"] = None,
         enqueue_server_properties: Optional["_models.EnqueueServerProperties"] = None,
         gateway_server_properties: Optional["_models.GatewayServerProperties"] = None,
         enqueue_replication_server_properties: Optional["_models.EnqueueReplicationServerProperties"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword message_server_properties: Defines the SAP Message Server properties.
         :paramtype message_server_properties: ~azure.mgmt.workloads.models.MessageServerProperties
@@ -4050,14 +3758,15 @@
         self.subnet = None
         self.message_server_properties = message_server_properties
         self.enqueue_server_properties = enqueue_server_properties
         self.gateway_server_properties = gateway_server_properties
         self.enqueue_replication_server_properties = enqueue_replication_server_properties
         self.kernel_version = None
         self.kernel_patch = None
+        self.load_balancer_details = None
         self.vm_details = None
         self.status = None
         self.health = None
         self.provisioning_state = None
         self.errors = None
 
 
@@ -4088,18 +3797,21 @@
     :ivar database_sid: Database SID name.
     :vartype database_sid: str
     :ivar database_type: Database type, that is if the DB is HANA, DB2, Oracle, SAP ASE, Max DB or
      MS SQL Server.
     :vartype database_type: str
     :ivar ip_address: Database IP Address.
     :vartype ip_address: str
+    :ivar load_balancer_details: The Load Balancer details such as LoadBalancer ID attached to
+     Database Virtual Machines.
+    :vartype load_balancer_details: ~azure.mgmt.workloads.models.LoadBalancerDetails
     :ivar vm_details: The list of virtual machines corresponding to the Database resource.
     :vartype vm_details: list[~azure.mgmt.workloads.models.DatabaseVmDetails]
     :ivar status: Defines the SAP Instance status. Known values are: "Starting", "Running",
-     "Stopping", "Offline", "PartiallyRunning", and "Unavailable".
+     "Stopping", "Offline", "PartiallyRunning", "Unavailable", and "SoftShutdown".
     :vartype status: str or ~azure.mgmt.workloads.models.SAPVirtualInstanceStatus
     :ivar provisioning_state: Defines the provisioning states. Known values are: "Succeeded",
      "Updating", "Creating", "Failed", and "Deleting".
     :vartype provisioning_state: str or
      ~azure.mgmt.workloads.models.SapVirtualInstanceProvisioningState
     :ivar errors: Defines the errors related to Database resource.
     :vartype errors: ~azure.mgmt.workloads.models.SAPVirtualInstanceError
@@ -4111,14 +3823,15 @@
         "type": {"readonly": True},
         "system_data": {"readonly": True},
         "location": {"required": True},
         "subnet": {"readonly": True},
         "database_sid": {"readonly": True},
         "database_type": {"readonly": True},
         "ip_address": {"readonly": True},
+        "load_balancer_details": {"readonly": True},
         "vm_details": {"readonly": True},
         "status": {"readonly": True},
         "provisioning_state": {"readonly": True},
         "errors": {"readonly": True},
     }
 
     _attribute_map = {
@@ -4128,32 +3841,34 @@
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "subnet": {"key": "properties.subnet", "type": "str"},
         "database_sid": {"key": "properties.databaseSid", "type": "str"},
         "database_type": {"key": "properties.databaseType", "type": "str"},
         "ip_address": {"key": "properties.ipAddress", "type": "str"},
+        "load_balancer_details": {"key": "properties.loadBalancerDetails", "type": "LoadBalancerDetails"},
         "vm_details": {"key": "properties.vmDetails", "type": "[DatabaseVmDetails]"},
         "status": {"key": "properties.status", "type": "str"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
         "errors": {"key": "properties.errors", "type": "SAPVirtualInstanceError"},
     }
 
-    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.subnet = None
         self.database_sid = None
         self.database_type = None
         self.ip_address = None
+        self.load_balancer_details = None
         self.vm_details = None
         self.status = None
         self.provisioning_state = None
         self.errors = None
 
 
 class SAPDatabaseInstanceList(_serialization.Model):
@@ -4167,92 +3882,62 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[SAPDatabaseInstance]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.SAPDatabaseInstance"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        value: Optional[List["_models.SAPDatabaseInstance"]] = None,
+        next_link: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: Gets the list of SAP Database instances.
         :paramtype value: list[~azure.mgmt.workloads.models.SAPDatabaseInstance]
         :keyword next_link: Gets the value of next link.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
 class SAPDiskConfiguration(_serialization.Model):
-    """The SAP Disk Configuration.
+    """The SAP Disk Configuration contains 'recommended disk' details and list of supported disks
+    detail for a volume type.
+
+    :ivar recommended_configuration: The recommended disk details for a given VM Sku.
+    :vartype recommended_configuration: ~azure.mgmt.workloads.models.DiskVolumeConfiguration
+    :ivar supported_configurations: The list of supported disks for a given VM Sku.
+    :vartype supported_configurations: list[~azure.mgmt.workloads.models.DiskDetails]
+    """
 
-    :ivar volume: The volume name.
-    :vartype volume: str
-    :ivar disk_type: The disk type.
-    :vartype disk_type: str
-    :ivar disk_count: The disk count.
-    :vartype disk_count: int
-    :ivar disk_size_gb: The disk size in GB.
-    :vartype disk_size_gb: int
-    :ivar disk_iops_read_write: The disk Iops.
-    :vartype disk_iops_read_write: int
-    :ivar disk_m_bps_read_write: The disk provisioned throughput in MBps.
-    :vartype disk_m_bps_read_write: int
-    :ivar disk_storage_type: The disk storage type.
-    :vartype disk_storage_type: str
-    """
-
-    _attribute_map = {
-        "volume": {"key": "volume", "type": "str"},
-        "disk_type": {"key": "diskType", "type": "str"},
-        "disk_count": {"key": "diskCount", "type": "int"},
-        "disk_size_gb": {"key": "diskSizeGB", "type": "int"},
-        "disk_iops_read_write": {"key": "diskIopsReadWrite", "type": "int"},
-        "disk_m_bps_read_write": {"key": "diskMBpsReadWrite", "type": "int"},
-        "disk_storage_type": {"key": "diskStorageType", "type": "str"},
+    _attribute_map = {
+        "recommended_configuration": {"key": "recommendedConfiguration", "type": "DiskVolumeConfiguration"},
+        "supported_configurations": {"key": "supportedConfigurations", "type": "[DiskDetails]"},
     }
 
     def __init__(
         self,
         *,
-        volume: Optional[str] = None,
-        disk_type: Optional[str] = None,
-        disk_count: Optional[int] = None,
-        disk_size_gb: Optional[int] = None,
-        disk_iops_read_write: Optional[int] = None,
-        disk_m_bps_read_write: Optional[int] = None,
-        disk_storage_type: Optional[str] = None,
-        **kwargs
-    ):
-        """
-        :keyword volume: The volume name.
-        :paramtype volume: str
-        :keyword disk_type: The disk type.
-        :paramtype disk_type: str
-        :keyword disk_count: The disk count.
-        :paramtype disk_count: int
-        :keyword disk_size_gb: The disk size in GB.
-        :paramtype disk_size_gb: int
-        :keyword disk_iops_read_write: The disk Iops.
-        :paramtype disk_iops_read_write: int
-        :keyword disk_m_bps_read_write: The disk provisioned throughput in MBps.
-        :paramtype disk_m_bps_read_write: int
-        :keyword disk_storage_type: The disk storage type.
-        :paramtype disk_storage_type: str
-        """
-        super().__init__(**kwargs)
-        self.volume = volume
-        self.disk_type = disk_type
-        self.disk_count = disk_count
-        self.disk_size_gb = disk_size_gb
-        self.disk_iops_read_write = disk_iops_read_write
-        self.disk_m_bps_read_write = disk_m_bps_read_write
-        self.disk_storage_type = disk_storage_type
+        recommended_configuration: Optional["_models.DiskVolumeConfiguration"] = None,
+        supported_configurations: Optional[List["_models.DiskDetails"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword recommended_configuration: The recommended disk details for a given VM Sku.
+        :paramtype recommended_configuration: ~azure.mgmt.workloads.models.DiskVolumeConfiguration
+        :keyword supported_configurations: The list of supported disks for a given VM Sku.
+        :paramtype supported_configurations: list[~azure.mgmt.workloads.models.DiskDetails]
+        """
+        super().__init__(**kwargs)
+        self.recommended_configuration = recommended_configuration
+        self.supported_configurations = supported_configurations
 
 
 class SAPDiskConfigurationsRequest(_serialization.Model):
     """The SAP request to get list of disk configurations.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -4297,16 +3982,16 @@
         *,
         app_location: str,
         environment: Union[str, "_models.SAPEnvironmentType"],
         sap_product: Union[str, "_models.SAPProductType"],
         database_type: Union[str, "_models.SAPDatabaseType"],
         deployment_type: Union[str, "_models.SAPDeploymentType"],
         db_vm_sku: str,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword app_location: The geo-location where the SAP resources will be created. Required.
         :paramtype app_location: str
         :keyword environment: Defines the environment type - Production/Non Production. Required. Known
          values are: "NonProd" and "Prod".
         :paramtype environment: str or ~azure.mgmt.workloads.models.SAPEnvironmentType
         :keyword sap_product: Defines the SAP Product type. Required. Known values are: "ECC",
@@ -4329,33 +4014,40 @@
         self.deployment_type = deployment_type
         self.db_vm_sku = db_vm_sku
 
 
 class SAPDiskConfigurationsResult(_serialization.Model):
     """The list of disk configuration for vmSku which are part of SAP deployment.
 
-    :ivar disk_configurations: Gets the list of Disk Configurations.
-    :vartype disk_configurations: list[~azure.mgmt.workloads.models.SAPDiskConfiguration]
+    :ivar volume_configurations: The disk configuration for the db volume. For HANA, Required
+     volumes are: ['hana/data', 'hana/log', hana/shared', 'usr/sap', 'os'], Optional volume :
+     ['backup'].
+    :vartype volume_configurations: dict[str, ~azure.mgmt.workloads.models.SAPDiskConfiguration]
     """
 
     _attribute_map = {
-        "disk_configurations": {"key": "diskConfigurations", "type": "[SAPDiskConfiguration]"},
+        "volume_configurations": {"key": "volumeConfigurations", "type": "{SAPDiskConfiguration}"},
     }
 
-    def __init__(self, *, disk_configurations: Optional[List["_models.SAPDiskConfiguration"]] = None, **kwargs):
+    def __init__(
+        self, *, volume_configurations: Optional[Dict[str, "_models.SAPDiskConfiguration"]] = None, **kwargs: Any
+    ) -> None:
         """
-        :keyword disk_configurations: Gets the list of Disk Configurations.
-        :paramtype disk_configurations: list[~azure.mgmt.workloads.models.SAPDiskConfiguration]
+        :keyword volume_configurations: The disk configuration for the db volume. For HANA, Required
+         volumes are: ['hana/data', 'hana/log', hana/shared', 'usr/sap', 'os'], Optional volume :
+         ['backup'].
+        :paramtype volume_configurations: dict[str, ~azure.mgmt.workloads.models.SAPDiskConfiguration]
         """
         super().__init__(**kwargs)
-        self.disk_configurations = disk_configurations
+        self.volume_configurations = volume_configurations
 
 
 class SAPInstallWithoutOSConfigSoftwareConfiguration(SoftwareConfiguration):
-    """The SAP Software configuration Input when the software is to be installed by service without OS Configurations.
+    """The SAP Software configuration Input when the software is to be installed by service without OS
+    Configurations.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar software_installation_type: The SAP software installation Type. Required. Known values
      are: "ServiceInitiated", "SAPInstallWithoutOSConfig", and "External".
     :vartype software_installation_type: str or
      ~azure.mgmt.workloads.models.SAPSoftwareInstallationType
@@ -4391,16 +4083,16 @@
     def __init__(
         self,
         *,
         bom_url: str,
         sap_bits_storage_account_id: str,
         software_version: str,
         high_availability_software_configuration: Optional["_models.HighAvailabilitySoftwareConfiguration"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword bom_url: The URL to the SAP Build of Materials(BOM) file. Required.
         :paramtype bom_url: str
         :keyword sap_bits_storage_account_id: The SAP bits storage account id. Required.
         :paramtype sap_bits_storage_account_id: str
         :keyword software_version: The software version to install. Required.
         :paramtype software_version: str
@@ -4412,14 +4104,220 @@
         self.software_installation_type: str = "SAPInstallWithoutOSConfig"
         self.bom_url = bom_url
         self.sap_bits_storage_account_id = sap_bits_storage_account_id
         self.software_version = software_version
         self.high_availability_software_configuration = high_availability_software_configuration
 
 
+class SapLandscapeMonitor(ProxyResource):
+    """configuration associated with SAP Landscape Monitor Dashboard.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. Ex -
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.workloads.models.SystemData
+    :ivar provisioning_state: State of provisioning of the SAP monitor. Known values are:
+     "Accepted", "Created", "Failed", "Succeeded", and "Canceled".
+    :vartype provisioning_state: str or
+     ~azure.mgmt.workloads.models.SapLandscapeMonitorProvisioningState
+    :ivar grouping: Gets or sets the SID groupings by landscape and Environment.
+    :vartype grouping: ~azure.mgmt.workloads.models.SapLandscapeMonitorPropertiesGrouping
+    :ivar top_metrics_thresholds: Gets or sets the list Top Metric Thresholds for SAP Landscape
+     Monitor Dashboard.
+    :vartype top_metrics_thresholds:
+     list[~azure.mgmt.workloads.models.SapLandscapeMonitorMetricThresholds]
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "provisioning_state": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "grouping": {"key": "properties.grouping", "type": "SapLandscapeMonitorPropertiesGrouping"},
+        "top_metrics_thresholds": {
+            "key": "properties.topMetricsThresholds",
+            "type": "[SapLandscapeMonitorMetricThresholds]",
+        },
+    }
+
+    def __init__(
+        self,
+        *,
+        grouping: Optional["_models.SapLandscapeMonitorPropertiesGrouping"] = None,
+        top_metrics_thresholds: Optional[List["_models.SapLandscapeMonitorMetricThresholds"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword grouping: Gets or sets the SID groupings by landscape and Environment.
+        :paramtype grouping: ~azure.mgmt.workloads.models.SapLandscapeMonitorPropertiesGrouping
+        :keyword top_metrics_thresholds: Gets or sets the list Top Metric Thresholds for SAP Landscape
+         Monitor Dashboard.
+        :paramtype top_metrics_thresholds:
+         list[~azure.mgmt.workloads.models.SapLandscapeMonitorMetricThresholds]
+        """
+        super().__init__(**kwargs)
+        self.provisioning_state = None
+        self.grouping = grouping
+        self.top_metrics_thresholds = top_metrics_thresholds
+
+
+class SapLandscapeMonitorListResult(_serialization.Model):
+    """The response from the List SAP Landscape Monitor Dashboard operation.
+
+    :ivar value: The list of Sap Landscape Monitor configuration.
+    :vartype value: list[~azure.mgmt.workloads.models.SapLandscapeMonitor]
+    :ivar next_link: The URL to get the next set of SAP Landscape Monitor Dashboard.
+    :vartype next_link: str
+    """
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[SapLandscapeMonitor]"},
+        "next_link": {"key": "nextLink", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        value: Optional[List["_models.SapLandscapeMonitor"]] = None,
+        next_link: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword value: The list of Sap Landscape Monitor configuration.
+        :paramtype value: list[~azure.mgmt.workloads.models.SapLandscapeMonitor]
+        :keyword next_link: The URL to get the next set of SAP Landscape Monitor Dashboard.
+        :paramtype next_link: str
+        """
+        super().__init__(**kwargs)
+        self.value = value
+        self.next_link = next_link
+
+
+class SapLandscapeMonitorMetricThresholds(_serialization.Model):
+    """Gets or sets the Threshold Values for Top Metrics Health.
+
+    :ivar name: Gets or sets the name of the threshold.
+    :vartype name: str
+    :ivar green: Gets or sets the threshold value for Green.
+    :vartype green: float
+    :ivar yellow: Gets or sets the threshold value for Yellow.
+    :vartype yellow: float
+    :ivar red: Gets or sets the threshold value for Red.
+    :vartype red: float
+    """
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "green": {"key": "green", "type": "float"},
+        "yellow": {"key": "yellow", "type": "float"},
+        "red": {"key": "red", "type": "float"},
+    }
+
+    def __init__(
+        self,
+        *,
+        name: Optional[str] = None,
+        green: Optional[float] = None,
+        yellow: Optional[float] = None,
+        red: Optional[float] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword name: Gets or sets the name of the threshold.
+        :paramtype name: str
+        :keyword green: Gets or sets the threshold value for Green.
+        :paramtype green: float
+        :keyword yellow: Gets or sets the threshold value for Yellow.
+        :paramtype yellow: float
+        :keyword red: Gets or sets the threshold value for Red.
+        :paramtype red: float
+        """
+        super().__init__(**kwargs)
+        self.name = name
+        self.green = green
+        self.yellow = yellow
+        self.red = red
+
+
+class SapLandscapeMonitorPropertiesGrouping(_serialization.Model):
+    """Gets or sets the SID groupings by landscape and Environment.
+
+    :ivar landscape: Gets or sets the list of landscape to SID mappings.
+    :vartype landscape: list[~azure.mgmt.workloads.models.SapLandscapeMonitorSidMapping]
+    :ivar sap_application: Gets or sets the list of Sap Applications to SID mappings.
+    :vartype sap_application: list[~azure.mgmt.workloads.models.SapLandscapeMonitorSidMapping]
+    """
+
+    _attribute_map = {
+        "landscape": {"key": "landscape", "type": "[SapLandscapeMonitorSidMapping]"},
+        "sap_application": {"key": "sapApplication", "type": "[SapLandscapeMonitorSidMapping]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        landscape: Optional[List["_models.SapLandscapeMonitorSidMapping"]] = None,
+        sap_application: Optional[List["_models.SapLandscapeMonitorSidMapping"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword landscape: Gets or sets the list of landscape to SID mappings.
+        :paramtype landscape: list[~azure.mgmt.workloads.models.SapLandscapeMonitorSidMapping]
+        :keyword sap_application: Gets or sets the list of Sap Applications to SID mappings.
+        :paramtype sap_application: list[~azure.mgmt.workloads.models.SapLandscapeMonitorSidMapping]
+        """
+        super().__init__(**kwargs)
+        self.landscape = landscape
+        self.sap_application = sap_application
+
+
+class SapLandscapeMonitorSidMapping(_serialization.Model):
+    """Gets or sets the mapping for SID to Environment/Applications.
+
+    :ivar name: Gets or sets the name of the grouping.
+    :vartype name: str
+    :ivar top_sid: Gets or sets the list of SID's.
+    :vartype top_sid: list[str]
+    """
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "top_sid": {"key": "topSid", "type": "[str]"},
+    }
+
+    def __init__(self, *, name: Optional[str] = None, top_sid: Optional[List[str]] = None, **kwargs: Any) -> None:
+        """
+        :keyword name: Gets or sets the name of the grouping.
+        :paramtype name: str
+        :keyword top_sid: Gets or sets the list of SID's.
+        :paramtype top_sid: list[str]
+        """
+        super().__init__(**kwargs)
+        self.name = name
+        self.top_sid = top_sid
+
+
 class SapNetWeaverProviderInstanceProperties(
     ProviderSpecificProperties
 ):  # pylint: disable=too-many-instance-attributes
     """Gets or sets the provider properties.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -4439,16 +4337,14 @@
     :vartype sap_password: str
     :ivar sap_password_uri: Gets or sets the key vault URI to secret with the SAP password.
     :vartype sap_password_uri: str
     :ivar sap_client_id: Gets or sets the SAP Client ID.
     :vartype sap_client_id: str
     :ivar sap_port_number: Gets or sets the SAP HTTP port number.
     :vartype sap_port_number: str
-    :ivar sap_ssl_certificate_uri: Gets or sets the blob URI to SSL certificate for the SAP system.
-    :vartype sap_ssl_certificate_uri: str
     :ivar ssl_certificate_uri: Gets or sets the blob URI to SSL certificate for the SAP system.
     :vartype ssl_certificate_uri: str
     :ivar ssl_preference: Gets or sets certificate preference if secure communication is enabled.
      Known values are: "Disabled", "RootCertificate", and "ServerCertificate".
     :vartype ssl_preference: str or ~azure.mgmt.workloads.models.SslPreference
     """
 
@@ -4463,15 +4359,14 @@
         "sap_instance_nr": {"key": "sapInstanceNr", "type": "str"},
         "sap_host_file_entries": {"key": "sapHostFileEntries", "type": "[str]"},
         "sap_username": {"key": "sapUsername", "type": "str"},
         "sap_password": {"key": "sapPassword", "type": "str"},
         "sap_password_uri": {"key": "sapPasswordUri", "type": "str"},
         "sap_client_id": {"key": "sapClientId", "type": "str"},
         "sap_port_number": {"key": "sapPortNumber", "type": "str"},
-        "sap_ssl_certificate_uri": {"key": "sapSslCertificateUri", "type": "str"},
         "ssl_certificate_uri": {"key": "sslCertificateUri", "type": "str"},
         "ssl_preference": {"key": "sslPreference", "type": "str"},
     }
 
     def __init__(
         self,
         *,
@@ -4480,19 +4375,18 @@
         sap_instance_nr: Optional[str] = None,
         sap_host_file_entries: Optional[List[str]] = None,
         sap_username: Optional[str] = None,
         sap_password: Optional[str] = None,
         sap_password_uri: Optional[str] = None,
         sap_client_id: Optional[str] = None,
         sap_port_number: Optional[str] = None,
-        sap_ssl_certificate_uri: Optional[str] = None,
         ssl_certificate_uri: Optional[str] = None,
         ssl_preference: Optional[Union[str, "_models.SslPreference"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword sap_sid: Gets or sets the SAP System Identifier.
         :paramtype sap_sid: str
         :keyword sap_hostname: Gets or sets the target virtual machine IP Address/FQDN.
         :paramtype sap_hostname: str
         :keyword sap_instance_nr: Gets or sets the instance number of SAP NetWeaver.
         :paramtype sap_instance_nr: str
@@ -4504,17 +4398,14 @@
         :paramtype sap_password: str
         :keyword sap_password_uri: Gets or sets the key vault URI to secret with the SAP password.
         :paramtype sap_password_uri: str
         :keyword sap_client_id: Gets or sets the SAP Client ID.
         :paramtype sap_client_id: str
         :keyword sap_port_number: Gets or sets the SAP HTTP port number.
         :paramtype sap_port_number: str
-        :keyword sap_ssl_certificate_uri: Gets or sets the blob URI to SSL certificate for the SAP
-         system.
-        :paramtype sap_ssl_certificate_uri: str
         :keyword ssl_certificate_uri: Gets or sets the blob URI to SSL certificate for the SAP system.
         :paramtype ssl_certificate_uri: str
         :keyword ssl_preference: Gets or sets certificate preference if secure communication is
          enabled. Known values are: "Disabled", "RootCertificate", and "ServerCertificate".
         :paramtype ssl_preference: str or ~azure.mgmt.workloads.models.SslPreference
         """
         super().__init__(**kwargs)
@@ -4524,15 +4415,14 @@
         self.sap_instance_nr = sap_instance_nr
         self.sap_host_file_entries = sap_host_file_entries
         self.sap_username = sap_username
         self.sap_password = sap_password
         self.sap_password_uri = sap_password_uri
         self.sap_client_id = sap_client_id
         self.sap_port_number = sap_port_number
-        self.sap_ssl_certificate_uri = sap_ssl_certificate_uri
         self.ssl_certificate_uri = ssl_certificate_uri
         self.ssl_preference = ssl_preference
 
 
 class SAPSizingRecommendationRequest(_serialization.Model):
     """The SAP Sizing Recommendation request.
 
@@ -4592,16 +4482,16 @@
         sap_product: Union[str, "_models.SAPProductType"],
         deployment_type: Union[str, "_models.SAPDeploymentType"],
         saps: int,
         db_memory: int,
         database_type: Union[str, "_models.SAPDatabaseType"],
         db_scale_method: Optional[Union[str, "_models.SAPDatabaseScaleMethod"]] = None,
         high_availability_type: Optional[Union[str, "_models.SAPHighAvailabilityType"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword app_location: The geo-location where the resource is to be created. Required.
         :paramtype app_location: str
         :keyword environment: Defines the environment type - Production/Non Production. Required. Known
          values are: "NonProd" and "Prod".
         :paramtype environment: str or ~azure.mgmt.workloads.models.SAPEnvironmentType
         :keyword sap_product: Defines the SAP Product type. Required. Known values are: "ECC",
@@ -4658,15 +4548,15 @@
     _subtype_map = {
         "deployment_type": {
             "SingleServer": "SingleServerRecommendationResult",
             "ThreeTier": "ThreeTierRecommendationResult",
         }
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.deployment_type: Optional[str] = None
 
 
 class SAPSupportedResourceSkusResult(_serialization.Model):
     """The list of supported SKUs for different resources which are part of SAP deployment.
@@ -4675,15 +4565,15 @@
     :vartype supported_skus: list[~azure.mgmt.workloads.models.SAPSupportedSku]
     """
 
     _attribute_map = {
         "supported_skus": {"key": "supportedSkus", "type": "[SAPSupportedSku]"},
     }
 
-    def __init__(self, *, supported_skus: Optional[List["_models.SAPSupportedSku"]] = None, **kwargs):
+    def __init__(self, *, supported_skus: Optional[List["_models.SAPSupportedSku"]] = None, **kwargs: Any) -> None:
         """
         :keyword supported_skus: Gets the list of SAP supported SKUs.
         :paramtype supported_skus: list[~azure.mgmt.workloads.models.SAPSupportedSku]
         """
         super().__init__(**kwargs)
         self.supported_skus = supported_skus
 
@@ -4708,16 +4598,16 @@
 
     def __init__(
         self,
         *,
         vm_sku: Optional[str] = None,
         is_app_server_certified: Optional[bool] = None,
         is_database_certified: Optional[bool] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword vm_sku: The VM Sku.
         :paramtype vm_sku: str
         :keyword is_app_server_certified: True if the Sku is certified for App server in the SAP
          system.
         :paramtype is_app_server_certified: bool
         :keyword is_database_certified: True if the Sku is certified for Database server in the SAP
@@ -4776,16 +4666,16 @@
         *,
         app_location: str,
         environment: Union[str, "_models.SAPEnvironmentType"],
         sap_product: Union[str, "_models.SAPProductType"],
         deployment_type: Union[str, "_models.SAPDeploymentType"],
         database_type: Union[str, "_models.SAPDatabaseType"],
         high_availability_type: Optional[Union[str, "_models.SAPHighAvailabilityType"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword app_location: The geo-location where the resource is to be created. Required.
         :paramtype app_location: str
         :keyword environment: Defines the environment type - Production/Non Production. Required. Known
          values are: "NonProd" and "Prod".
         :paramtype environment: str or ~azure.mgmt.workloads.models.SAPEnvironmentType
         :keyword sap_product: Defines the SAP Product type. Required. Known values are: "ECC",
@@ -4843,15 +4733,15 @@
     :ivar configuration: Defines if the SAP system is being created using Azure Center for SAP
      solutions (ACSS) or if an existing SAP system is being registered with ACSS. Required.
     :vartype configuration: ~azure.mgmt.workloads.models.SAPConfiguration
     :ivar managed_resource_group_configuration: Managed resource group configuration.
     :vartype managed_resource_group_configuration:
      ~azure.mgmt.workloads.models.ManagedRGConfiguration
     :ivar status: Defines the SAP Instance status. Known values are: "Starting", "Running",
-     "Stopping", "Offline", "PartiallyRunning", and "Unavailable".
+     "Stopping", "Offline", "PartiallyRunning", "Unavailable", and "SoftShutdown".
     :vartype status: str or ~azure.mgmt.workloads.models.SAPVirtualInstanceStatus
     :ivar health: Defines the health of SAP Instances. Known values are: "Unknown", "Healthy",
      "Unhealthy", and "Degraded".
     :vartype health: str or ~azure.mgmt.workloads.models.SAPHealthState
     :ivar state: Defines the Virtual Instance for SAP state. Known values are:
      "InfrastructureDeploymentPending", "InfrastructureDeploymentInProgress",
      "InfrastructureDeploymentFailed", "SoftwareInstallationPending",
@@ -4911,16 +4801,16 @@
         location: str,
         environment: Union[str, "_models.SAPEnvironmentType"],
         sap_product: Union[str, "_models.SAPProductType"],
         configuration: "_models.SAPConfiguration",
         tags: Optional[Dict[str, str]] = None,
         identity: Optional["_models.UserAssignedServiceIdentity"] = None,
         managed_resource_group_configuration: Optional["_models.ManagedRGConfiguration"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
         :keyword identity: Managed service identity (user assigned identities).
         :paramtype identity: ~azure.mgmt.workloads.models.UserAssignedServiceIdentity
@@ -4957,15 +4847,15 @@
     :vartype properties: ~azure.mgmt.workloads.models.ErrorDefinition
     """
 
     _attribute_map = {
         "properties": {"key": "properties", "type": "ErrorDefinition"},
     }
 
-    def __init__(self, *, properties: Optional["_models.ErrorDefinition"] = None, **kwargs):
+    def __init__(self, *, properties: Optional["_models.ErrorDefinition"] = None, **kwargs: Any) -> None:
         """
         :keyword properties: The Virtual Instance for SAP error body.
         :paramtype properties: ~azure.mgmt.workloads.models.ErrorDefinition
         """
         super().__init__(**kwargs)
         self.properties = properties
 
@@ -4981,99 +4871,31 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[SAPVirtualInstance]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.SAPVirtualInstance"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        value: Optional[List["_models.SAPVirtualInstance"]] = None,
+        next_link: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: Gets the list of Virtual Instances for SAP solutions resources.
         :paramtype value: list[~azure.mgmt.workloads.models.SAPVirtualInstance]
         :keyword next_link: Gets the value of next link.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
-class SearchProfile(NodeProfile):
-    """Search profile.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar name: VM or VMSS name.
-    :vartype name: str
-    :ivar node_sku: VM SKU for node(s). Required.
-    :vartype node_sku: str
-    :ivar os_image: OS image used for creating the nodes. Required.
-    :vartype os_image: ~azure.mgmt.workloads.models.OsImageProfile
-    :ivar os_disk: OS disk details. Required.
-    :vartype os_disk: ~azure.mgmt.workloads.models.DiskInfo
-    :ivar data_disks: Data disks details. This property is not in use right now.
-    :vartype data_disks: list[~azure.mgmt.workloads.models.DiskInfo]
-    :ivar node_resource_ids: VM/VMSS resource ARM Ids.
-    :vartype node_resource_ids: list[str]
-    :ivar search_type: Search type. Required. "Elastic"
-    :vartype search_type: str or ~azure.mgmt.workloads.models.SearchType
-    """
-
-    _validation = {
-        "node_sku": {"required": True},
-        "os_image": {"required": True},
-        "os_disk": {"required": True},
-        "node_resource_ids": {"readonly": True},
-        "search_type": {"required": True},
-    }
-
-    _attribute_map = {
-        "name": {"key": "name", "type": "str"},
-        "node_sku": {"key": "nodeSku", "type": "str"},
-        "os_image": {"key": "osImage", "type": "OsImageProfile"},
-        "os_disk": {"key": "osDisk", "type": "DiskInfo"},
-        "data_disks": {"key": "dataDisks", "type": "[DiskInfo]"},
-        "node_resource_ids": {"key": "nodeResourceIds", "type": "[str]"},
-        "search_type": {"key": "searchType", "type": "str"},
-    }
-
-    def __init__(
-        self,
-        *,
-        node_sku: str,
-        os_image: "_models.OsImageProfile",
-        os_disk: "_models.DiskInfo",
-        search_type: Union[str, "_models.SearchType"],
-        name: Optional[str] = None,
-        data_disks: Optional[List["_models.DiskInfo"]] = None,
-        **kwargs
-    ):
-        """
-        :keyword name: VM or VMSS name.
-        :paramtype name: str
-        :keyword node_sku: VM SKU for node(s). Required.
-        :paramtype node_sku: str
-        :keyword os_image: OS image used for creating the nodes. Required.
-        :paramtype os_image: ~azure.mgmt.workloads.models.OsImageProfile
-        :keyword os_disk: OS disk details. Required.
-        :paramtype os_disk: ~azure.mgmt.workloads.models.DiskInfo
-        :keyword data_disks: Data disks details. This property is not in use right now.
-        :paramtype data_disks: list[~azure.mgmt.workloads.models.DiskInfo]
-        :keyword search_type: Search type. Required. "Elastic"
-        :paramtype search_type: str or ~azure.mgmt.workloads.models.SearchType
-        """
-        super().__init__(
-            name=name, node_sku=node_sku, os_image=os_image, os_disk=os_disk, data_disks=data_disks, **kwargs
-        )
-        self.search_type = search_type
-
-
 class ServiceInitiatedSoftwareConfiguration(SoftwareConfiguration):
     """The SAP Software configuration Input when the software is to be installed by service.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar software_installation_type: The SAP software installation Type. Required. Known values
      are: "ServiceInitiated", "SAPInstallWithoutOSConfig", and "External".
@@ -5121,16 +4943,16 @@
         *,
         bom_url: str,
         software_version: str,
         sap_bits_storage_account_id: str,
         sap_fqdn: str,
         ssh_private_key: str,
         high_availability_software_configuration: Optional["_models.HighAvailabilitySoftwareConfiguration"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword bom_url: The URL to the SAP Build of Materials(BOM) file. Required.
         :paramtype bom_url: str
         :keyword software_version: The software version to install. Required.
         :paramtype software_version: str
         :keyword sap_bits_storage_account_id: The SAP bits storage account id. Required.
         :paramtype sap_bits_storage_account_id: str
@@ -5148,14 +4970,54 @@
         self.software_version = software_version
         self.sap_bits_storage_account_id = sap_bits_storage_account_id
         self.sap_fqdn = sap_fqdn
         self.ssh_private_key = ssh_private_key
         self.high_availability_software_configuration = high_availability_software_configuration
 
 
+class SharedStorageResourceNames(_serialization.Model):
+    """The resource names object for shared storage.
+
+    :ivar shared_storage_account_name: The full name of the shared storage account. If it is not
+     provided, it will be defaulted to {SID}nfs{guid of 15 chars}.
+    :vartype shared_storage_account_name: str
+    :ivar shared_storage_account_private_end_point_name: The full name of private end point for the
+     shared storage account. If it is not provided, it will be defaulted to {storageAccountName}_pe.
+    :vartype shared_storage_account_private_end_point_name: str
+    """
+
+    _attribute_map = {
+        "shared_storage_account_name": {"key": "sharedStorageAccountName", "type": "str"},
+        "shared_storage_account_private_end_point_name": {
+            "key": "sharedStorageAccountPrivateEndPointName",
+            "type": "str",
+        },
+    }
+
+    def __init__(
+        self,
+        *,
+        shared_storage_account_name: Optional[str] = None,
+        shared_storage_account_private_end_point_name: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword shared_storage_account_name: The full name of the shared storage account. If it is not
+         provided, it will be defaulted to {SID}nfs{guid of 15 chars}.
+        :paramtype shared_storage_account_name: str
+        :keyword shared_storage_account_private_end_point_name: The full name of private end point for
+         the shared storage account. If it is not provided, it will be defaulted to
+         {storageAccountName}_pe.
+        :paramtype shared_storage_account_private_end_point_name: str
+        """
+        super().__init__(**kwargs)
+        self.shared_storage_account_name = shared_storage_account_name
+        self.shared_storage_account_private_end_point_name = shared_storage_account_private_end_point_name
+
+
 class SingleServerConfiguration(InfrastructureConfiguration):
     """Gets or sets the single server configuration.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar deployment_type: The type of SAP deployment, single server or Three tier. Required. Known
      values are: "SingleServer" and "ThreeTier".
@@ -5168,14 +5030,19 @@
     :ivar database_type: The database type. Known values are: "HANA" and "DB2".
     :vartype database_type: str or ~azure.mgmt.workloads.models.SAPDatabaseType
     :ivar subnet_id: The subnet id. Required.
     :vartype subnet_id: str
     :ivar virtual_machine_configuration: Gets or sets the virtual machine configuration. Required.
     :vartype virtual_machine_configuration:
      ~azure.mgmt.workloads.models.VirtualMachineConfiguration
+    :ivar db_disk_configuration: Gets or sets the disk configuration.
+    :vartype db_disk_configuration: ~azure.mgmt.workloads.models.DiskConfiguration
+    :ivar custom_resource_names: The set of custom names to be used for underlying azure resources
+     that are part of the SAP system.
+    :vartype custom_resource_names: ~azure.mgmt.workloads.models.SingleServerCustomResourceNames
     """
 
     _validation = {
         "deployment_type": {"required": True},
         "app_resource_group": {"required": True},
         "subnet_id": {"required": True},
         "virtual_machine_configuration": {"required": True},
@@ -5184,652 +5051,334 @@
     _attribute_map = {
         "deployment_type": {"key": "deploymentType", "type": "str"},
         "app_resource_group": {"key": "appResourceGroup", "type": "str"},
         "network_configuration": {"key": "networkConfiguration", "type": "NetworkConfiguration"},
         "database_type": {"key": "databaseType", "type": "str"},
         "subnet_id": {"key": "subnetId", "type": "str"},
         "virtual_machine_configuration": {"key": "virtualMachineConfiguration", "type": "VirtualMachineConfiguration"},
+        "db_disk_configuration": {"key": "dbDiskConfiguration", "type": "DiskConfiguration"},
+        "custom_resource_names": {"key": "customResourceNames", "type": "SingleServerCustomResourceNames"},
     }
 
     def __init__(
         self,
         *,
         app_resource_group: str,
         subnet_id: str,
         virtual_machine_configuration: "_models.VirtualMachineConfiguration",
         network_configuration: Optional["_models.NetworkConfiguration"] = None,
         database_type: Optional[Union[str, "_models.SAPDatabaseType"]] = None,
-        **kwargs
-    ):
+        db_disk_configuration: Optional["_models.DiskConfiguration"] = None,
+        custom_resource_names: Optional["_models.SingleServerCustomResourceNames"] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword app_resource_group: The application resource group where SAP system resources will be
          deployed. Required.
         :paramtype app_resource_group: str
         :keyword network_configuration: Network configuration for the server.
         :paramtype network_configuration: ~azure.mgmt.workloads.models.NetworkConfiguration
         :keyword database_type: The database type. Known values are: "HANA" and "DB2".
         :paramtype database_type: str or ~azure.mgmt.workloads.models.SAPDatabaseType
         :keyword subnet_id: The subnet id. Required.
         :paramtype subnet_id: str
         :keyword virtual_machine_configuration: Gets or sets the virtual machine configuration.
          Required.
         :paramtype virtual_machine_configuration:
          ~azure.mgmt.workloads.models.VirtualMachineConfiguration
+        :keyword db_disk_configuration: Gets or sets the disk configuration.
+        :paramtype db_disk_configuration: ~azure.mgmt.workloads.models.DiskConfiguration
+        :keyword custom_resource_names: The set of custom names to be used for underlying azure
+         resources that are part of the SAP system.
+        :paramtype custom_resource_names: ~azure.mgmt.workloads.models.SingleServerCustomResourceNames
         """
         super().__init__(app_resource_group=app_resource_group, **kwargs)
         self.deployment_type: str = "SingleServer"
         self.network_configuration = network_configuration
         self.database_type = database_type
         self.subnet_id = subnet_id
         self.virtual_machine_configuration = virtual_machine_configuration
+        self.db_disk_configuration = db_disk_configuration
+        self.custom_resource_names = custom_resource_names
 
 
-class SingleServerRecommendationResult(SAPSizingRecommendationResult):
-    """The recommended configuration for a single server SAP system.
+class SingleServerCustomResourceNames(_serialization.Model):
+    """The resource-names input to specify custom names for underlying azure resources that are part
+    of a single server SAP system.
+
+    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
+    SingleServerFullResourceNames
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar deployment_type: The type of SAP deployment, single server or Three tier. Required. Known
-     values are: "SingleServer" and "ThreeTier".
-    :vartype deployment_type: str or ~azure.mgmt.workloads.models.SAPDeploymentType
-    :ivar vm_sku: The recommended VM SKU for single server.
-    :vartype vm_sku: str
+    :ivar naming_pattern_type: The pattern type to be used for resource naming. Required.
+     "FullResourceName"
+    :vartype naming_pattern_type: str or ~azure.mgmt.workloads.models.NamingPatternType
     """
 
     _validation = {
-        "deployment_type": {"required": True},
+        "naming_pattern_type": {"required": True},
     }
 
     _attribute_map = {
-        "deployment_type": {"key": "deploymentType", "type": "str"},
-        "vm_sku": {"key": "vmSku", "type": "str"},
+        "naming_pattern_type": {"key": "namingPatternType", "type": "str"},
     }
 
-    def __init__(self, *, vm_sku: Optional[str] = None, **kwargs):
-        """
-        :keyword vm_sku: The recommended VM SKU for single server.
-        :paramtype vm_sku: str
-        """
-        super().__init__(**kwargs)
-        self.deployment_type: str = "SingleServer"
-        self.vm_sku = vm_sku
-
-
-class SiteProfile(_serialization.Model):
-    """Workload website profile.
-
-    :ivar domain_name: Domain name for the application site URL.
-    :vartype domain_name: str
-    """
+    _subtype_map = {"naming_pattern_type": {"FullResourceName": "SingleServerFullResourceNames"}}
 
-    _attribute_map = {
-        "domain_name": {"key": "domainName", "type": "str"},
-    }
-
-    def __init__(self, *, domain_name: Optional[str] = None, **kwargs):
-        """
-        :keyword domain_name: Domain name for the application site URL.
-        :paramtype domain_name: str
-        """
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
         super().__init__(**kwargs)
-        self.domain_name = domain_name
+        self.naming_pattern_type: Optional[str] = None
 
 
-class Sku(_serialization.Model):
-    """The resource model definition representing SKU.
+class SingleServerFullResourceNames(SingleServerCustomResourceNames):
+    """The resource name object where the specified values will be full resource names of the
+    corresponding resources in a single server SAP system.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar name: The name of the SKU. Ex - P3. It is typically a letter+number code. Required.
-    :vartype name: str
-    :ivar tier: This field is required to be implemented by the Resource Provider if the service
-     has more than one tier, but is not required on a PUT. Known values are: "Free", "Basic",
-     "Standard", and "Premium".
-    :vartype tier: str or ~azure.mgmt.workloads.models.SkuTier
-    :ivar size: The SKU size. When the name field is the combination of tier and some other value,
-     this would be the standalone code.
-    :vartype size: str
-    :ivar family: If the service has different generations of hardware, for the same SKU, then that
-     can be captured here.
-    :vartype family: str
-    :ivar capacity: If the SKU supports scale out/in then the capacity integer should be included.
-     If scale out/in is not possible for the resource this may be omitted.
-    :vartype capacity: int
+    :ivar naming_pattern_type: The pattern type to be used for resource naming. Required.
+     "FullResourceName"
+    :vartype naming_pattern_type: str or ~azure.mgmt.workloads.models.NamingPatternType
+    :ivar virtual_machine: The resource names object for virtual machine and related resources.
+    :vartype virtual_machine: ~azure.mgmt.workloads.models.VirtualMachineResourceNames
     """
 
     _validation = {
-        "name": {"required": True},
+        "naming_pattern_type": {"required": True},
     }
 
     _attribute_map = {
-        "name": {"key": "name", "type": "str"},
-        "tier": {"key": "tier", "type": "str"},
-        "size": {"key": "size", "type": "str"},
-        "family": {"key": "family", "type": "str"},
-        "capacity": {"key": "capacity", "type": "int"},
+        "naming_pattern_type": {"key": "namingPatternType", "type": "str"},
+        "virtual_machine": {"key": "virtualMachine", "type": "VirtualMachineResourceNames"},
     }
 
     def __init__(
-        self,
-        *,
-        name: str,
-        tier: Optional[Union[str, "_models.SkuTier"]] = None,
-        size: Optional[str] = None,
-        family: Optional[str] = None,
-        capacity: Optional[int] = None,
-        **kwargs
-    ):
+        self, *, virtual_machine: Optional["_models.VirtualMachineResourceNames"] = None, **kwargs: Any
+    ) -> None:
         """
-        :keyword name: The name of the SKU. Ex - P3. It is typically a letter+number code. Required.
-        :paramtype name: str
-        :keyword tier: This field is required to be implemented by the Resource Provider if the service
-         has more than one tier, but is not required on a PUT. Known values are: "Free", "Basic",
-         "Standard", and "Premium".
-        :paramtype tier: str or ~azure.mgmt.workloads.models.SkuTier
-        :keyword size: The SKU size. When the name field is the combination of tier and some other
-         value, this would be the standalone code.
-        :paramtype size: str
-        :keyword family: If the service has different generations of hardware, for the same SKU, then
-         that can be captured here.
-        :paramtype family: str
-        :keyword capacity: If the SKU supports scale out/in then the capacity integer should be
-         included. If scale out/in is not possible for the resource this may be omitted.
-        :paramtype capacity: int
+        :keyword virtual_machine: The resource names object for virtual machine and related resources.
+        :paramtype virtual_machine: ~azure.mgmt.workloads.models.VirtualMachineResourceNames
         """
         super().__init__(**kwargs)
-        self.name = name
-        self.tier = tier
-        self.size = size
-        self.family = family
-        self.capacity = capacity
+        self.naming_pattern_type: str = "FullResourceName"
+        self.virtual_machine = virtual_machine
 
 
-class SkuCapability(_serialization.Model):
-    """The SKU capability definition.
-
-    :ivar name: The capability name.
-    :vartype name: str
-    :ivar value: The capability value.
-    :vartype value: str
-    """
-
-    _attribute_map = {
-        "name": {"key": "name", "type": "str"},
-        "value": {"key": "value", "type": "str"},
-    }
-
-    def __init__(self, *, name: Optional[str] = None, value: Optional[str] = None, **kwargs):
-        """
-        :keyword name: The capability name.
-        :paramtype name: str
-        :keyword value: The capability value.
-        :paramtype value: str
-        """
-        super().__init__(**kwargs)
-        self.name = name
-        self.value = value
-
-
-class SkuCapacity(_serialization.Model):
-    """The SKU capacity.
-
-    :ivar minimum: Minimum capacity value.
-    :vartype minimum: int
-    :ivar maximum: Maximum capacity value.
-    :vartype maximum: int
-    :ivar default: Default capacity value.
-    :vartype default: int
-    :ivar scale_type: Scale type of the SKU capacity. Known values are: "None", "Manual", and
-     "Automatic".
-    :vartype scale_type: str or ~azure.mgmt.workloads.models.SkuScaleType
-    """
-
-    _attribute_map = {
-        "minimum": {"key": "minimum", "type": "int"},
-        "maximum": {"key": "maximum", "type": "int"},
-        "default": {"key": "default", "type": "int"},
-        "scale_type": {"key": "scaleType", "type": "str"},
-    }
-
-    def __init__(
-        self,
-        *,
-        minimum: Optional[int] = None,
-        maximum: Optional[int] = None,
-        default: Optional[int] = None,
-        scale_type: Optional[Union[str, "_models.SkuScaleType"]] = None,
-        **kwargs
-    ):
-        """
-        :keyword minimum: Minimum capacity value.
-        :paramtype minimum: int
-        :keyword maximum: Maximum capacity value.
-        :paramtype maximum: int
-        :keyword default: Default capacity value.
-        :paramtype default: int
-        :keyword scale_type: Scale type of the SKU capacity. Known values are: "None", "Manual", and
-         "Automatic".
-        :paramtype scale_type: str or ~azure.mgmt.workloads.models.SkuScaleType
-        """
-        super().__init__(**kwargs)
-        self.minimum = minimum
-        self.maximum = maximum
-        self.default = default
-        self.scale_type = scale_type
-
-
-class SkuCost(_serialization.Model):
-    """The SKU cost definition.
-
-    :ivar meter_id: Billing meter id.
-    :vartype meter_id: str
-    :ivar quantity: The quantity.
-    :vartype quantity: int
-    :ivar extended_unit: The extended unit.
-    :vartype extended_unit: str
-    """
-
-    _attribute_map = {
-        "meter_id": {"key": "meterId", "type": "str"},
-        "quantity": {"key": "quantity", "type": "int"},
-        "extended_unit": {"key": "extendedUnit", "type": "str"},
-    }
-
-    def __init__(
-        self,
-        *,
-        meter_id: Optional[str] = None,
-        quantity: Optional[int] = None,
-        extended_unit: Optional[str] = None,
-        **kwargs
-    ):
-        """
-        :keyword meter_id: Billing meter id.
-        :paramtype meter_id: str
-        :keyword quantity: The quantity.
-        :paramtype quantity: int
-        :keyword extended_unit: The extended unit.
-        :paramtype extended_unit: str
-        """
-        super().__init__(**kwargs)
-        self.meter_id = meter_id
-        self.quantity = quantity
-        self.extended_unit = extended_unit
-
-
-class SkuDefinition(_serialization.Model):  # pylint: disable=too-many-instance-attributes
-    """The SKU definition.
+class SingleServerRecommendationResult(SAPSizingRecommendationResult):
+    """The recommended configuration for a single server SAP system.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar name: The name of the SKU. Required.
-    :vartype name: str
-    :ivar resource_type: Resource type the SKU applicable for.
-    :vartype resource_type: str
-    :ivar tier: This field is required to be implemented by the Resource Provider if the service
-     has more than one tier, but is not required on a PUT.
-    :vartype tier: str
-    :ivar size: The SKU size. When the name field is the combination of tier and some other value,
-     this would be the standalone code.
-    :vartype size: str
-    :ivar family: If the service has different generations of hardware, for the same SKU, then that
-     can be captured here.
-    :vartype family: str
-    :ivar kind: If the service has different kinds of hardware, for the same SKU, then that can be
-     captured here.
-    :vartype kind: str
-    :ivar locations: List of locations where this SKU is available.
-    :vartype locations: list[str]
-    :ivar location_info: List of locations where this SKU is available.
-    :vartype location_info: list[~azure.mgmt.workloads.models.SkuLocationAndZones]
-    :ivar capacity: If the SKU supports scale out/in then the capacity integer should be included.
-     If scale out/in is not possible for the resource this may be omitted.
-    :vartype capacity: JSON
-    :ivar costs: The SKU costs.
-    :vartype costs: list[~azure.mgmt.workloads.models.SkuCost]
-    :ivar capabilities: The SKU capabilities.
-    :vartype capabilities: list[~azure.mgmt.workloads.models.SkuCapability]
-    :ivar restrictions: The SKU restrictions.
-    :vartype restrictions: list[~azure.mgmt.workloads.models.SkuRestriction]
+    :ivar deployment_type: The type of SAP deployment, single server or Three tier. Required. Known
+     values are: "SingleServer" and "ThreeTier".
+    :vartype deployment_type: str or ~azure.mgmt.workloads.models.SAPDeploymentType
+    :ivar vm_sku: The recommended VM SKU for single server.
+    :vartype vm_sku: str
     """
 
     _validation = {
-        "name": {"required": True},
-    }
-
-    _attribute_map = {
-        "name": {"key": "name", "type": "str"},
-        "resource_type": {"key": "resourceType", "type": "str"},
-        "tier": {"key": "tier", "type": "str"},
-        "size": {"key": "size", "type": "str"},
-        "family": {"key": "family", "type": "str"},
-        "kind": {"key": "kind", "type": "str"},
-        "locations": {"key": "locations", "type": "[str]"},
-        "location_info": {"key": "locationInfo", "type": "[SkuLocationAndZones]"},
-        "capacity": {"key": "capacity", "type": "object"},
-        "costs": {"key": "costs", "type": "[SkuCost]"},
-        "capabilities": {"key": "capabilities", "type": "[SkuCapability]"},
-        "restrictions": {"key": "restrictions", "type": "[SkuRestriction]"},
+        "deployment_type": {"required": True},
     }
 
-    def __init__(
-        self,
-        *,
-        name: str,
-        resource_type: Optional[str] = None,
-        tier: Optional[str] = None,
-        size: Optional[str] = None,
-        family: Optional[str] = None,
-        kind: Optional[str] = None,
-        locations: Optional[List[str]] = None,
-        location_info: Optional[List["_models.SkuLocationAndZones"]] = None,
-        capacity: Optional[JSON] = None,
-        costs: Optional[List["_models.SkuCost"]] = None,
-        capabilities: Optional[List["_models.SkuCapability"]] = None,
-        restrictions: Optional[List["_models.SkuRestriction"]] = None,
-        **kwargs
-    ):
-        """
-        :keyword name: The name of the SKU. Required.
-        :paramtype name: str
-        :keyword resource_type: Resource type the SKU applicable for.
-        :paramtype resource_type: str
-        :keyword tier: This field is required to be implemented by the Resource Provider if the service
-         has more than one tier, but is not required on a PUT.
-        :paramtype tier: str
-        :keyword size: The SKU size. When the name field is the combination of tier and some other
-         value, this would be the standalone code.
-        :paramtype size: str
-        :keyword family: If the service has different generations of hardware, for the same SKU, then
-         that can be captured here.
-        :paramtype family: str
-        :keyword kind: If the service has different kinds of hardware, for the same SKU, then that can
-         be captured here.
-        :paramtype kind: str
-        :keyword locations: List of locations where this SKU is available.
-        :paramtype locations: list[str]
-        :keyword location_info: List of locations where this SKU is available.
-        :paramtype location_info: list[~azure.mgmt.workloads.models.SkuLocationAndZones]
-        :keyword capacity: If the SKU supports scale out/in then the capacity integer should be
-         included. If scale out/in is not possible for the resource this may be omitted.
-        :paramtype capacity: JSON
-        :keyword costs: The SKU costs.
-        :paramtype costs: list[~azure.mgmt.workloads.models.SkuCost]
-        :keyword capabilities: The SKU capabilities.
-        :paramtype capabilities: list[~azure.mgmt.workloads.models.SkuCapability]
-        :keyword restrictions: The SKU restrictions.
-        :paramtype restrictions: list[~azure.mgmt.workloads.models.SkuRestriction]
-        """
-        super().__init__(**kwargs)
-        self.name = name
-        self.resource_type = resource_type
-        self.tier = tier
-        self.size = size
-        self.family = family
-        self.kind = kind
-        self.locations = locations
-        self.location_info = location_info
-        self.capacity = capacity
-        self.costs = costs
-        self.capabilities = capabilities
-        self.restrictions = restrictions
-
-
-class SkuLocationAndZones(_serialization.Model):
-    """The SKU location and zone.
-
-    :ivar location: The location of the SKU.
-    :vartype location: str
-    :ivar zones: The availability zones of SKU location.
-    :vartype zones: list[str]
-    :ivar zone_details: The availability zone details of the SKU location.
-    :vartype zone_details: list[~azure.mgmt.workloads.models.SkuZoneDetail]
-    :ivar extended_locations: The extended locations of SKU.
-    :vartype extended_locations: list[str]
-    :ivar type: Type of the extended location. Known values are: "Region" and "EdgeZone".
-    :vartype type: str or ~azure.mgmt.workloads.models.LocationType
-    """
-
     _attribute_map = {
-        "location": {"key": "location", "type": "str"},
-        "zones": {"key": "zones", "type": "[str]"},
-        "zone_details": {"key": "zoneDetails", "type": "[SkuZoneDetail]"},
-        "extended_locations": {"key": "extendedLocations", "type": "[str]"},
-        "type": {"key": "type", "type": "str"},
+        "deployment_type": {"key": "deploymentType", "type": "str"},
+        "vm_sku": {"key": "vmSku", "type": "str"},
     }
 
-    def __init__(
-        self,
-        *,
-        location: Optional[str] = None,
-        zones: Optional[List[str]] = None,
-        zone_details: Optional[List["_models.SkuZoneDetail"]] = None,
-        extended_locations: Optional[List[str]] = None,
-        type: Optional[Union[str, "_models.LocationType"]] = None,
-        **kwargs
-    ):
+    def __init__(self, *, vm_sku: Optional[str] = None, **kwargs: Any) -> None:
         """
-        :keyword location: The location of the SKU.
-        :paramtype location: str
-        :keyword zones: The availability zones of SKU location.
-        :paramtype zones: list[str]
-        :keyword zone_details: The availability zone details of the SKU location.
-        :paramtype zone_details: list[~azure.mgmt.workloads.models.SkuZoneDetail]
-        :keyword extended_locations: The extended locations of SKU.
-        :paramtype extended_locations: list[str]
-        :keyword type: Type of the extended location. Known values are: "Region" and "EdgeZone".
-        :paramtype type: str or ~azure.mgmt.workloads.models.LocationType
-        """
-        super().__init__(**kwargs)
-        self.location = location
-        self.zones = zones
-        self.zone_details = zone_details
-        self.extended_locations = extended_locations
-        self.type = type
-
-
-class SkuRestriction(_serialization.Model):
-    """The SKU restriction definition.
-
-    :ivar type: The SKU restriction type. Known values are: "NotSpecified", "Location", and "Zone".
-    :vartype type: str or ~azure.mgmt.workloads.models.SkuRestrictionType
-    :ivar values: Restriction values.
-    :vartype values: list[str]
-    :ivar restriction_info: The restriction information.
-    :vartype restriction_info: JSON
-    :ivar reason_code: The SKU restriction reason code. Known values are: "NotSpecified",
-     "QuotaId", and "NotAvailableForSubscription".
-    :vartype reason_code: str or ~azure.mgmt.workloads.models.SkuRestrictionReasonCode
-    """
-
-    _attribute_map = {
-        "type": {"key": "type", "type": "str"},
-        "values": {"key": "values", "type": "[str]"},
-        "restriction_info": {"key": "restrictionInfo", "type": "object"},
-        "reason_code": {"key": "reasonCode", "type": "str"},
-    }
-
-    def __init__(
-        self,
-        *,
-        type: Optional[Union[str, "_models.SkuRestrictionType"]] = None,
-        values: Optional[List[str]] = None,
-        restriction_info: Optional[JSON] = None,
-        reason_code: Optional[Union[str, "_models.SkuRestrictionReasonCode"]] = None,
-        **kwargs
-    ):
-        """
-        :keyword type: The SKU restriction type. Known values are: "NotSpecified", "Location", and
-         "Zone".
-        :paramtype type: str or ~azure.mgmt.workloads.models.SkuRestrictionType
-        :keyword values: Restriction values.
-        :paramtype values: list[str]
-        :keyword restriction_info: The restriction information.
-        :paramtype restriction_info: JSON
-        :keyword reason_code: The SKU restriction reason code. Known values are: "NotSpecified",
-         "QuotaId", and "NotAvailableForSubscription".
-        :paramtype reason_code: str or ~azure.mgmt.workloads.models.SkuRestrictionReasonCode
+        :keyword vm_sku: The recommended VM SKU for single server.
+        :paramtype vm_sku: str
         """
         super().__init__(**kwargs)
-        self.type = type
-        self.values = values
-        self.restriction_info = restriction_info
-        self.reason_code = reason_code
+        self.deployment_type: str = "SingleServer"
+        self.vm_sku = vm_sku
 
 
-class SkusListResult(_serialization.Model):
-    """A list of SKUs supported by an Azure Resource Provider.
+class SkipFileShareConfiguration(FileShareConfiguration):
+    """Gets or sets the skip file share configuration.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
+    All required parameters must be populated in order to send to Azure.
 
-    :ivar value: List of SKUs supported by the resource provider.
-    :vartype value: list[~azure.mgmt.workloads.models.SkuDefinition]
-    :ivar next_link: URL to get the next set of SKU list results (if there are any).
-    :vartype next_link: str
+    :ivar configuration_type: The type of file share config. Required. Known values are: "Skip",
+     "CreateAndMount", and "Mount".
+    :vartype configuration_type: str or ~azure.mgmt.workloads.models.ConfigurationType
     """
 
     _validation = {
-        "value": {"readonly": True},
-        "next_link": {"readonly": True},
+        "configuration_type": {"required": True},
     }
 
     _attribute_map = {
-        "value": {"key": "value", "type": "[SkuDefinition]"},
-        "next_link": {"key": "nextLink", "type": "str"},
+        "configuration_type": {"key": "configurationType", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
-        self.value = None
-        self.next_link = None
-
-
-class SkuZoneDetail(_serialization.Model):
-    """The SKU zone details.
-
-    :ivar zones: The physical zones.
-    :vartype zones: list[str]
-    :ivar capabilities: The capabilities.
-    :vartype capabilities: list[~azure.mgmt.workloads.models.SkuCapability]
-    """
-
-    _attribute_map = {
-        "zones": {"key": "zones", "type": "[str]"},
-        "capabilities": {"key": "capabilities", "type": "[SkuCapability]"},
-    }
-
-    def __init__(
-        self,
-        *,
-        zones: Optional[List[str]] = None,
-        capabilities: Optional[List["_models.SkuCapability"]] = None,
-        **kwargs
-    ):
-        """
-        :keyword zones: The physical zones.
-        :paramtype zones: list[str]
-        :keyword capabilities: The capabilities.
-        :paramtype capabilities: list[~azure.mgmt.workloads.models.SkuCapability]
-        """
-        super().__init__(**kwargs)
-        self.zones = zones
-        self.capabilities = capabilities
+        self.configuration_type: str = "Skip"
 
 
 class SshConfiguration(_serialization.Model):
     """SSH configuration for Linux based VMs running on Azure.
 
     :ivar public_keys: The list of SSH public keys used to authenticate with linux based VMs.
     :vartype public_keys: list[~azure.mgmt.workloads.models.SshPublicKey]
     """
 
     _attribute_map = {
         "public_keys": {"key": "publicKeys", "type": "[SshPublicKey]"},
     }
 
-    def __init__(self, *, public_keys: Optional[List["_models.SshPublicKey"]] = None, **kwargs):
+    def __init__(self, *, public_keys: Optional[List["_models.SshPublicKey"]] = None, **kwargs: Any) -> None:
         """
         :keyword public_keys: The list of SSH public keys used to authenticate with linux based VMs.
         :paramtype public_keys: list[~azure.mgmt.workloads.models.SshPublicKey]
         """
         super().__init__(**kwargs)
         self.public_keys = public_keys
 
 
 class SshKeyPair(_serialization.Model):
-    """The SSH Key-pair used to authenticate with the VM. The key needs to be at least 2048-bit and in ssh-rsa format. :code:`<br>`:code:`<br>` For creating ssh keys, see `Create SSH keys on Linux and Mac for Linux VMs in Azure <https://docs.microsoft.com/azure/virtual-machines/linux/create-ssh-keys-detailed>`_.
+    """The SSH Key-pair used to authenticate with the VM. The key needs to be at least 2048-bit and in
+    ssh-rsa format. :code:`<br>`:code:`<br>` For creating ssh keys, see `Create SSH keys on Linux
+    and Mac for Linux VMs in Azure
+    <https://docs.microsoft.com/azure/virtual-machines/linux/create-ssh-keys-detailed>`_.
 
     :ivar public_key: SSH public key.
     :vartype public_key: str
     :ivar private_key: SSH private key.
     :vartype private_key: str
     """
 
     _attribute_map = {
         "public_key": {"key": "publicKey", "type": "str"},
         "private_key": {"key": "privateKey", "type": "str"},
     }
 
-    def __init__(self, *, public_key: Optional[str] = None, private_key: Optional[str] = None, **kwargs):
+    def __init__(self, *, public_key: Optional[str] = None, private_key: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword public_key: SSH public key.
         :paramtype public_key: str
         :keyword private_key: SSH private key.
         :paramtype private_key: str
         """
         super().__init__(**kwargs)
         self.public_key = public_key
         self.private_key = private_key
 
 
 class SshPublicKey(_serialization.Model):
-    """Contains information about SSH certificate public key and the path on the Linux VM where the public key is placed.
+    """Contains information about SSH certificate public key and the path on the Linux VM where the
+    public key is placed.
 
     :ivar key_data: SSH public key certificate used to authenticate with the VM through ssh. The
      key needs to be at least 2048-bit and in ssh-rsa format. :code:`<br>`:code:`<br>` For creating
      ssh keys, see `Create SSH keys on Linux and Mac for Linux VMs in Azure
      <https://docs.microsoft.com/azure/virtual-machines/linux/create-ssh-keys-detailed>`_.
     :vartype key_data: str
     """
 
     _attribute_map = {
         "key_data": {"key": "keyData", "type": "str"},
     }
 
-    def __init__(self, *, key_data: Optional[str] = None, **kwargs):
+    def __init__(self, *, key_data: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword key_data: SSH public key certificate used to authenticate with the VM through ssh. The
          key needs to be at least 2048-bit and in ssh-rsa format. :code:`<br>`:code:`<br>` For creating
          ssh keys, see `Create SSH keys on Linux and Mac for Linux VMs in Azure
          <https://docs.microsoft.com/azure/virtual-machines/linux/create-ssh-keys-detailed>`_.
         :paramtype key_data: str
         """
         super().__init__(**kwargs)
         self.key_data = key_data
 
 
 class StopRequest(_serialization.Model):
-    """Stop SAP Request.
+    """Stop SAP instance(s) request body.
 
-    :ivar hard_stop: A boolean to specify if the SAP system should be hard-stopped.
-    :vartype hard_stop: bool
+    :ivar soft_stop_timeout_seconds: This parameter defines how long (in seconds) the soft shutdown
+     waits until the RFC/HTTP clients no longer consider the server for calls with load balancing.
+     Value 0 means that the kernel does not wait, but goes directly into the next shutdown state,
+     i.e. hard stop.
+    :vartype soft_stop_timeout_seconds: int
     """
 
     _attribute_map = {
-        "hard_stop": {"key": "hardStop", "type": "bool"},
+        "soft_stop_timeout_seconds": {"key": "softStopTimeoutSeconds", "type": "int"},
     }
 
-    def __init__(self, *, hard_stop: bool = False, **kwargs):
+    def __init__(self, *, soft_stop_timeout_seconds: int = 0, **kwargs: Any) -> None:
         """
-        :keyword hard_stop: A boolean to specify if the SAP system should be hard-stopped.
-        :paramtype hard_stop: bool
+        :keyword soft_stop_timeout_seconds: This parameter defines how long (in seconds) the soft
+         shutdown waits until the RFC/HTTP clients no longer consider the server for calls with load
+         balancing. Value 0 means that the kernel does not wait, but goes directly into the next
+         shutdown state, i.e. hard stop.
+        :paramtype soft_stop_timeout_seconds: int
         """
         super().__init__(**kwargs)
-        self.hard_stop = hard_stop
+        self.soft_stop_timeout_seconds = soft_stop_timeout_seconds
+
+
+class StorageConfiguration(_serialization.Model):
+    """Gets or sets the storage configuration.
+
+    :ivar transport_file_share_configuration: The properties of the transport directory attached to
+     the VIS. The default for transportFileShareConfiguration is the createAndMount flow if storage
+     configuration is missing.
+    :vartype transport_file_share_configuration:
+     ~azure.mgmt.workloads.models.FileShareConfiguration
+    """
+
+    _attribute_map = {
+        "transport_file_share_configuration": {
+            "key": "transportFileShareConfiguration",
+            "type": "FileShareConfiguration",
+        },
+    }
+
+    def __init__(
+        self, *, transport_file_share_configuration: Optional["_models.FileShareConfiguration"] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword transport_file_share_configuration: The properties of the transport directory attached
+         to the VIS. The default for transportFileShareConfiguration is the createAndMount flow if
+         storage configuration is missing.
+        :paramtype transport_file_share_configuration:
+         ~azure.mgmt.workloads.models.FileShareConfiguration
+        """
+        super().__init__(**kwargs)
+        self.transport_file_share_configuration = transport_file_share_configuration
+
+
+class StorageInformation(_serialization.Model):
+    """Storage details of all the Storage accounts attached to the VM. For e.g. NFS on AFS Shared
+    Storage.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id:
+    :vartype id: str
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.id = None
 
 
 class SystemData(_serialization.Model):
     """Metadata pertaining to creation and last modification of the resource.
 
     :ivar created_by: The identity that created the resource.
     :vartype created_by: str
@@ -5861,16 +5410,16 @@
         *,
         created_by: Optional[str] = None,
         created_by_type: Optional[Union[str, "_models.CreatedByType"]] = None,
         created_at: Optional[datetime.datetime] = None,
         last_modified_by: Optional[str] = None,
         last_modified_by_type: Optional[Union[str, "_models.CreatedByType"]] = None,
         last_modified_at: Optional[datetime.datetime] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword created_by: The identity that created the resource.
         :paramtype created_by: str
         :keyword created_by_type: The type of identity that created the resource. Known values are:
          "User", "Application", "ManagedIdentity", and "Key".
         :paramtype created_by_type: str or ~azure.mgmt.workloads.models.CreatedByType
         :keyword created_at: The timestamp of resource creation (UTC).
@@ -5899,15 +5448,15 @@
     :vartype tags: dict[str, str]
     """
 
     _attribute_map = {
         "tags": {"key": "tags", "type": "{str}"},
     }
 
-    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Tags field of the resource.
         :paramtype tags: dict[str, str]
         """
         super().__init__(**kwargs)
         self.tags = tags
 
@@ -5929,14 +5478,19 @@
     :vartype central_server: ~azure.mgmt.workloads.models.CentralServerConfiguration
     :ivar application_server: The application server configuration. Required.
     :vartype application_server: ~azure.mgmt.workloads.models.ApplicationServerConfiguration
     :ivar database_server: The database configuration. Required.
     :vartype database_server: ~azure.mgmt.workloads.models.DatabaseConfiguration
     :ivar high_availability_config: The high availability configuration.
     :vartype high_availability_config: ~azure.mgmt.workloads.models.HighAvailabilityConfiguration
+    :ivar storage_configuration: The storage configuration.
+    :vartype storage_configuration: ~azure.mgmt.workloads.models.StorageConfiguration
+    :ivar custom_resource_names: The set of custom names to be used for underlying azure resources
+     that are part of the SAP system.
+    :vartype custom_resource_names: ~azure.mgmt.workloads.models.ThreeTierCustomResourceNames
     """
 
     _validation = {
         "deployment_type": {"required": True},
         "app_resource_group": {"required": True},
         "central_server": {"required": True},
         "application_server": {"required": True},
@@ -5947,49 +5501,155 @@
         "deployment_type": {"key": "deploymentType", "type": "str"},
         "app_resource_group": {"key": "appResourceGroup", "type": "str"},
         "network_configuration": {"key": "networkConfiguration", "type": "NetworkConfiguration"},
         "central_server": {"key": "centralServer", "type": "CentralServerConfiguration"},
         "application_server": {"key": "applicationServer", "type": "ApplicationServerConfiguration"},
         "database_server": {"key": "databaseServer", "type": "DatabaseConfiguration"},
         "high_availability_config": {"key": "highAvailabilityConfig", "type": "HighAvailabilityConfiguration"},
+        "storage_configuration": {"key": "storageConfiguration", "type": "StorageConfiguration"},
+        "custom_resource_names": {"key": "customResourceNames", "type": "ThreeTierCustomResourceNames"},
     }
 
     def __init__(
         self,
         *,
         app_resource_group: str,
         central_server: "_models.CentralServerConfiguration",
         application_server: "_models.ApplicationServerConfiguration",
         database_server: "_models.DatabaseConfiguration",
         network_configuration: Optional["_models.NetworkConfiguration"] = None,
         high_availability_config: Optional["_models.HighAvailabilityConfiguration"] = None,
-        **kwargs
-    ):
+        storage_configuration: Optional["_models.StorageConfiguration"] = None,
+        custom_resource_names: Optional["_models.ThreeTierCustomResourceNames"] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword app_resource_group: The application resource group where SAP system resources will be
          deployed. Required.
         :paramtype app_resource_group: str
         :keyword network_configuration: Network configuration common to all servers.
         :paramtype network_configuration: ~azure.mgmt.workloads.models.NetworkConfiguration
         :keyword central_server: The central server configuration. Required.
         :paramtype central_server: ~azure.mgmt.workloads.models.CentralServerConfiguration
         :keyword application_server: The application server configuration. Required.
         :paramtype application_server: ~azure.mgmt.workloads.models.ApplicationServerConfiguration
         :keyword database_server: The database configuration. Required.
         :paramtype database_server: ~azure.mgmt.workloads.models.DatabaseConfiguration
         :keyword high_availability_config: The high availability configuration.
         :paramtype high_availability_config: ~azure.mgmt.workloads.models.HighAvailabilityConfiguration
+        :keyword storage_configuration: The storage configuration.
+        :paramtype storage_configuration: ~azure.mgmt.workloads.models.StorageConfiguration
+        :keyword custom_resource_names: The set of custom names to be used for underlying azure
+         resources that are part of the SAP system.
+        :paramtype custom_resource_names: ~azure.mgmt.workloads.models.ThreeTierCustomResourceNames
         """
         super().__init__(app_resource_group=app_resource_group, **kwargs)
         self.deployment_type: str = "ThreeTier"
         self.network_configuration = network_configuration
         self.central_server = central_server
         self.application_server = application_server
         self.database_server = database_server
         self.high_availability_config = high_availability_config
+        self.storage_configuration = storage_configuration
+        self.custom_resource_names = custom_resource_names
+
+
+class ThreeTierCustomResourceNames(_serialization.Model):
+    """The resource-names input to specify custom names for underlying azure resources that are part
+    of a three tier SAP system.
+
+    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
+    ThreeTierFullResourceNames
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar naming_pattern_type: The pattern type to be used for resource naming. Required.
+     "FullResourceName"
+    :vartype naming_pattern_type: str or ~azure.mgmt.workloads.models.NamingPatternType
+    """
+
+    _validation = {
+        "naming_pattern_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "naming_pattern_type": {"key": "namingPatternType", "type": "str"},
+    }
+
+    _subtype_map = {"naming_pattern_type": {"FullResourceName": "ThreeTierFullResourceNames"}}
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.naming_pattern_type: Optional[str] = None
+
+
+class ThreeTierFullResourceNames(ThreeTierCustomResourceNames):
+    """The resource name object where the specified values will be full resource names of the
+    corresponding resources in a three tier SAP system.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar naming_pattern_type: The pattern type to be used for resource naming. Required.
+     "FullResourceName"
+    :vartype naming_pattern_type: str or ~azure.mgmt.workloads.models.NamingPatternType
+    :ivar central_server: The full resource names object for central server layer resources.
+    :vartype central_server: ~azure.mgmt.workloads.models.CentralServerFullResourceNames
+    :ivar application_server: The full resource names object for application layer resources. The
+     number of entries in this list should be equal to the number VMs to be created for application
+     layer.
+    :vartype application_server: ~azure.mgmt.workloads.models.ApplicationServerFullResourceNames
+    :ivar database_server: The full resource names object for database layer resources. The number
+     of entries in this list should be equal to the number VMs to be created for database layer.
+    :vartype database_server: ~azure.mgmt.workloads.models.DatabaseServerFullResourceNames
+    :ivar shared_storage: The resource names object for shared storage.
+    :vartype shared_storage: ~azure.mgmt.workloads.models.SharedStorageResourceNames
+    """
+
+    _validation = {
+        "naming_pattern_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "naming_pattern_type": {"key": "namingPatternType", "type": "str"},
+        "central_server": {"key": "centralServer", "type": "CentralServerFullResourceNames"},
+        "application_server": {"key": "applicationServer", "type": "ApplicationServerFullResourceNames"},
+        "database_server": {"key": "databaseServer", "type": "DatabaseServerFullResourceNames"},
+        "shared_storage": {"key": "sharedStorage", "type": "SharedStorageResourceNames"},
+    }
+
+    def __init__(
+        self,
+        *,
+        central_server: Optional["_models.CentralServerFullResourceNames"] = None,
+        application_server: Optional["_models.ApplicationServerFullResourceNames"] = None,
+        database_server: Optional["_models.DatabaseServerFullResourceNames"] = None,
+        shared_storage: Optional["_models.SharedStorageResourceNames"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword central_server: The full resource names object for central server layer resources.
+        :paramtype central_server: ~azure.mgmt.workloads.models.CentralServerFullResourceNames
+        :keyword application_server: The full resource names object for application layer resources.
+         The number of entries in this list should be equal to the number VMs to be created for
+         application layer.
+        :paramtype application_server: ~azure.mgmt.workloads.models.ApplicationServerFullResourceNames
+        :keyword database_server: The full resource names object for database layer resources. The
+         number of entries in this list should be equal to the number VMs to be created for database
+         layer.
+        :paramtype database_server: ~azure.mgmt.workloads.models.DatabaseServerFullResourceNames
+        :keyword shared_storage: The resource names object for shared storage.
+        :paramtype shared_storage: ~azure.mgmt.workloads.models.SharedStorageResourceNames
+        """
+        super().__init__(**kwargs)
+        self.naming_pattern_type: str = "FullResourceName"
+        self.central_server = central_server
+        self.application_server = application_server
+        self.database_server = database_server
+        self.shared_storage = shared_storage
 
 
 class ThreeTierRecommendationResult(SAPSizingRecommendationResult):
     """The recommended configuration for a three tier SAP system.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -6029,16 +5689,16 @@
         *,
         db_vm_sku: Optional[str] = None,
         database_instance_count: Optional[int] = None,
         central_server_vm_sku: Optional[str] = None,
         central_server_instance_count: Optional[int] = None,
         application_server_vm_sku: Optional[str] = None,
         application_server_instance_count: Optional[int] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword db_vm_sku: The database VM SKU.
         :paramtype db_vm_sku: str
         :keyword database_instance_count: The database server instance count.
         :paramtype database_instance_count: int
         :keyword central_server_vm_sku: The central server VM SKU.
         :paramtype central_server_vm_sku: str
@@ -6074,16 +5734,16 @@
     }
 
     def __init__(
         self,
         *,
         tags: Optional[Dict[str, str]] = None,
         identity: Optional["_models.UserAssignedServiceIdentity"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Gets or sets the Resource tags.
         :paramtype tags: dict[str, str]
         :keyword identity: Managed service identity (user assigned identities).
         :paramtype identity: ~azure.mgmt.workloads.models.UserAssignedServiceIdentity
         """
         super().__init__(**kwargs)
@@ -6098,15 +5758,15 @@
     :vartype tags: dict[str, str]
     """
 
     _attribute_map = {
         "tags": {"key": "tags", "type": "{str}"},
     }
 
-    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Gets or sets the Resource tags.
         :paramtype tags: dict[str, str]
         """
         super().__init__(**kwargs)
         self.tags = tags
 
@@ -6118,15 +5778,15 @@
     :vartype tags: dict[str, str]
     """
 
     _attribute_map = {
         "tags": {"key": "tags", "type": "{str}"},
     }
 
-    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Gets or sets the Resource tags.
         :paramtype tags: dict[str, str]
         """
         super().__init__(**kwargs)
         self.tags = tags
 
@@ -6138,15 +5798,15 @@
     :vartype tags: dict[str, str]
     """
 
     _attribute_map = {
         "tags": {"key": "tags", "type": "{str}"},
     }
 
-    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Gets or sets the Resource tags.
         :paramtype tags: dict[str, str]
         """
         super().__init__(**kwargs)
         self.tags = tags
 
@@ -6166,16 +5826,16 @@
     }
 
     def __init__(
         self,
         *,
         tags: Optional[Dict[str, str]] = None,
         identity: Optional["_models.UserAssignedServiceIdentity"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Gets or sets the Resource tags.
         :paramtype tags: dict[str, str]
         :keyword identity: Managed service identity (user assigned identities).
         :paramtype identity: ~azure.mgmt.workloads.models.UserAssignedServiceIdentity
         """
         super().__init__(**kwargs)
@@ -6200,52 +5860,58 @@
     }
 
     _attribute_map = {
         "principal_id": {"key": "principalId", "type": "str"},
         "client_id": {"key": "clientId", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.principal_id = None
         self.client_id = None
 
 
-class UserProfile(_serialization.Model):
-    """User profile to configure on a compute resources such as VM, VMSS.
+class UserAssignedServiceIdentity(_serialization.Model):
+    """Managed service identity (user assigned identities).
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar user_name: User name. Required.
-    :vartype user_name: str
-    :ivar ssh_public_key: SSH public key data. Required.
-    :vartype ssh_public_key: str
+    :ivar type: Type of manage identity. Required. Known values are: "None" and "UserAssigned".
+    :vartype type: str or ~azure.mgmt.workloads.models.ManagedServiceIdentityType
+    :ivar user_assigned_identities: User assigned identities dictionary.
+    :vartype user_assigned_identities: dict[str, ~azure.mgmt.workloads.models.UserAssignedIdentity]
     """
 
     _validation = {
-        "user_name": {"required": True},
-        "ssh_public_key": {"required": True},
+        "type": {"required": True},
     }
 
     _attribute_map = {
-        "user_name": {"key": "userName", "type": "str"},
-        "ssh_public_key": {"key": "sshPublicKey", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "user_assigned_identities": {"key": "userAssignedIdentities", "type": "{UserAssignedIdentity}"},
     }
 
-    def __init__(self, *, user_name: str, ssh_public_key: str, **kwargs):
+    def __init__(
+        self,
+        *,
+        type: Union[str, "_models.ManagedServiceIdentityType"],
+        user_assigned_identities: Optional[Dict[str, "_models.UserAssignedIdentity"]] = None,
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword user_name: User name. Required.
-        :paramtype user_name: str
-        :keyword ssh_public_key: SSH public key data. Required.
-        :paramtype ssh_public_key: str
+        :keyword type: Type of manage identity. Required. Known values are: "None" and "UserAssigned".
+        :paramtype type: str or ~azure.mgmt.workloads.models.ManagedServiceIdentityType
+        :keyword user_assigned_identities: User assigned identities dictionary.
+        :paramtype user_assigned_identities: dict[str,
+         ~azure.mgmt.workloads.models.UserAssignedIdentity]
         """
         super().__init__(**kwargs)
-        self.user_name = user_name
-        self.ssh_public_key = ssh_public_key
+        self.type = type
+        self.user_assigned_identities = user_assigned_identities
 
 
 class VirtualMachineConfiguration(_serialization.Model):
     """Defines the virtual machine configuration.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -6266,108 +5932,111 @@
     _attribute_map = {
         "vm_size": {"key": "vmSize", "type": "str"},
         "image_reference": {"key": "imageReference", "type": "ImageReference"},
         "os_profile": {"key": "osProfile", "type": "OSProfile"},
     }
 
     def __init__(
-        self, *, vm_size: str, image_reference: "_models.ImageReference", os_profile: "_models.OSProfile", **kwargs
-    ):
+        self, *, vm_size: str, image_reference: "_models.ImageReference", os_profile: "_models.OSProfile", **kwargs: Any
+    ) -> None:
         """
         :keyword vm_size: The virtual machine size. Required.
         :paramtype vm_size: str
         :keyword image_reference: The image reference. Required.
         :paramtype image_reference: ~azure.mgmt.workloads.models.ImageReference
         :keyword os_profile: The OS profile. Required.
         :paramtype os_profile: ~azure.mgmt.workloads.models.OSProfile
         """
         super().__init__(**kwargs)
         self.vm_size = vm_size
         self.image_reference = image_reference
         self.os_profile = os_profile
 
 
-class VmssNodesProfile(NodeProfile):
-    """VMSS profile.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar name: VM or VMSS name.
-    :vartype name: str
-    :ivar node_sku: VM SKU for node(s). Required.
-    :vartype node_sku: str
-    :ivar os_image: OS image used for creating the nodes. Required.
-    :vartype os_image: ~azure.mgmt.workloads.models.OsImageProfile
-    :ivar os_disk: OS disk details. Required.
-    :vartype os_disk: ~azure.mgmt.workloads.models.DiskInfo
-    :ivar data_disks: Data disks details. This property is not in use right now.
-    :vartype data_disks: list[~azure.mgmt.workloads.models.DiskInfo]
-    :ivar node_resource_ids: VM/VMSS resource ARM Ids.
-    :vartype node_resource_ids: list[str]
-    :ivar auto_scale_min_count: Minimum number of nodes for autoscale.
-    :vartype auto_scale_min_count: int
-    :ivar auto_scale_max_count: Maximum number of nodes for autoscale.
-    :vartype auto_scale_max_count: int
-    """
-
-    _validation = {
-        "node_sku": {"required": True},
-        "os_image": {"required": True},
-        "os_disk": {"required": True},
-        "node_resource_ids": {"readonly": True},
-        "auto_scale_min_count": {"minimum": 1},
-        "auto_scale_max_count": {"minimum": 1},
-    }
+class VirtualMachineResourceNames(_serialization.Model):
+    """The resource names object for virtual machine and related resources.
 
-    _attribute_map = {
-        "name": {"key": "name", "type": "str"},
-        "node_sku": {"key": "nodeSku", "type": "str"},
-        "os_image": {"key": "osImage", "type": "OsImageProfile"},
-        "os_disk": {"key": "osDisk", "type": "DiskInfo"},
-        "data_disks": {"key": "dataDisks", "type": "[DiskInfo]"},
-        "node_resource_ids": {"key": "nodeResourceIds", "type": "[str]"},
-        "auto_scale_min_count": {"key": "autoScaleMinCount", "type": "int"},
-        "auto_scale_max_count": {"key": "autoScaleMaxCount", "type": "int"},
+    :ivar vm_name: The full name for virtual machine. The length of this field can be upto 64
+     characters. If name is not provided, service uses a default name based on the deployment type.
+     For SingleServer, default name is {SID}vm. In case of HA-AvZone systems, default name will be
+     {SID}{app/ascs/db}z{a/b}vm with an incrementor at the end in case of more than 1 vm per layer.
+     For distributed and HA-AvSet systems, default name will be {SID}{app/ascs/db}vm with an
+     incrementor at the end in case of more than 1 vm per layer.
+    :vartype vm_name: str
+    :ivar host_name: The full name for virtual-machine's host (computer name). Currently, ACSS only
+     supports host names which are less than or equal to 13 characters long. If this value is not
+     provided, vmName will be used as host name.
+    :vartype host_name: str
+    :ivar network_interfaces: The list of network interface name objects for the selected virtual
+     machine. Currently, only one network interface is supported per virtual machine.
+    :vartype network_interfaces: list[~azure.mgmt.workloads.models.NetworkInterfaceResourceNames]
+    :ivar os_disk_name: The full name for OS disk attached to the VM. If this value is not
+     provided, it will be named by ARM as per its default naming standards (prefixed with vm name).
+     There is only one OS disk attached per Virtual Machine.
+    :vartype os_disk_name: str
+    :ivar data_disk_names: The full resource names for virtual machine data disks. This is a
+     dictionary containing list of names of data disks per volume. Currently supported volumes for
+     database layer are ['hana/data', 'hana/log', hana/shared', 'usr/sap', 'os', 'backup']. For
+     application and cs layers, only 'default' volume is supported.
+    :vartype data_disk_names: dict[str, list[str]]
+    """
+
+    _validation = {
+        "network_interfaces": {"max_items": 1, "min_items": 0},
+    }
+
+    _attribute_map = {
+        "vm_name": {"key": "vmName", "type": "str"},
+        "host_name": {"key": "hostName", "type": "str"},
+        "network_interfaces": {"key": "networkInterfaces", "type": "[NetworkInterfaceResourceNames]"},
+        "os_disk_name": {"key": "osDiskName", "type": "str"},
+        "data_disk_names": {"key": "dataDiskNames", "type": "{[str]}"},
     }
 
     def __init__(
         self,
         *,
-        node_sku: str,
-        os_image: "_models.OsImageProfile",
-        os_disk: "_models.DiskInfo",
-        name: Optional[str] = None,
-        data_disks: Optional[List["_models.DiskInfo"]] = None,
-        auto_scale_min_count: Optional[int] = None,
-        auto_scale_max_count: Optional[int] = None,
-        **kwargs
-    ):
-        """
-        :keyword name: VM or VMSS name.
-        :paramtype name: str
-        :keyword node_sku: VM SKU for node(s). Required.
-        :paramtype node_sku: str
-        :keyword os_image: OS image used for creating the nodes. Required.
-        :paramtype os_image: ~azure.mgmt.workloads.models.OsImageProfile
-        :keyword os_disk: OS disk details. Required.
-        :paramtype os_disk: ~azure.mgmt.workloads.models.DiskInfo
-        :keyword data_disks: Data disks details. This property is not in use right now.
-        :paramtype data_disks: list[~azure.mgmt.workloads.models.DiskInfo]
-        :keyword auto_scale_min_count: Minimum number of nodes for autoscale.
-        :paramtype auto_scale_min_count: int
-        :keyword auto_scale_max_count: Maximum number of nodes for autoscale.
-        :paramtype auto_scale_max_count: int
-        """
-        super().__init__(
-            name=name, node_sku=node_sku, os_image=os_image, os_disk=os_disk, data_disks=data_disks, **kwargs
-        )
-        self.auto_scale_min_count = auto_scale_min_count
-        self.auto_scale_max_count = auto_scale_max_count
+        vm_name: Optional[str] = None,
+        host_name: Optional[str] = None,
+        network_interfaces: Optional[List["_models.NetworkInterfaceResourceNames"]] = None,
+        os_disk_name: Optional[str] = None,
+        data_disk_names: Optional[Dict[str, List[str]]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword vm_name: The full name for virtual machine. The length of this field can be upto 64
+         characters. If name is not provided, service uses a default name based on the deployment type.
+         For SingleServer, default name is {SID}vm. In case of HA-AvZone systems, default name will be
+         {SID}{app/ascs/db}z{a/b}vm with an incrementor at the end in case of more than 1 vm per layer.
+         For distributed and HA-AvSet systems, default name will be {SID}{app/ascs/db}vm with an
+         incrementor at the end in case of more than 1 vm per layer.
+        :paramtype vm_name: str
+        :keyword host_name: The full name for virtual-machine's host (computer name). Currently, ACSS
+         only supports host names which are less than or equal to 13 characters long. If this value is
+         not provided, vmName will be used as host name.
+        :paramtype host_name: str
+        :keyword network_interfaces: The list of network interface name objects for the selected
+         virtual machine. Currently, only one network interface is supported per virtual machine.
+        :paramtype network_interfaces: list[~azure.mgmt.workloads.models.NetworkInterfaceResourceNames]
+        :keyword os_disk_name: The full name for OS disk attached to the VM. If this value is not
+         provided, it will be named by ARM as per its default naming standards (prefixed with vm name).
+         There is only one OS disk attached per Virtual Machine.
+        :paramtype os_disk_name: str
+        :keyword data_disk_names: The full resource names for virtual machine data disks. This is a
+         dictionary containing list of names of data disks per volume. Currently supported volumes for
+         database layer are ['hana/data', 'hana/log', hana/shared', 'usr/sap', 'os', 'backup']. For
+         application and cs layers, only 'default' volume is supported.
+        :paramtype data_disk_names: dict[str, list[str]]
+        """
+        super().__init__(**kwargs)
+        self.vm_name = vm_name
+        self.host_name = host_name
+        self.network_interfaces = network_interfaces
+        self.os_disk_name = os_disk_name
+        self.data_disk_names = data_disk_names
 
 
 class WindowsConfiguration(OSConfiguration):
     """Specifies Windows operating system settings on the virtual machine.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -6379,117 +6048,11 @@
         "os_type": {"required": True},
     }
 
     _attribute_map = {
         "os_type": {"key": "osType", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.os_type: str = "Windows"
-
-
-class WordpressInstanceResource(ProxyResource):
-    """WordPress instance resource.
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
-    :vartype system_data: ~azure.mgmt.workloads.models.SystemData
-    :ivar version: Application version. Known values are: "5.4.3", "5.4.2", "5.4.1", and "5.4".
-    :vartype version: str or ~azure.mgmt.workloads.models.WordpressVersions
-    :ivar database_name: Database name used by the application.
-    :vartype database_name: str
-    :ivar database_user: User name used by the application to connect to database.
-    :vartype database_user: str
-    :ivar site_url: Site Url to access the WordPress application.
-    :vartype site_url: str
-    :ivar provisioning_state: WordPress instance provisioning state. Known values are:
-     "NotSpecified", "Accepted", "Created", "Succeeded", "Failed", "Canceled", and "Installing".
-    :vartype provisioning_state: str or ~azure.mgmt.workloads.models.ApplicationProvisioningState
-    """
-
-    _validation = {
-        "id": {"readonly": True},
-        "name": {"readonly": True},
-        "type": {"readonly": True},
-        "system_data": {"readonly": True},
-        "site_url": {"readonly": True},
-        "provisioning_state": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "id": {"key": "id", "type": "str"},
-        "name": {"key": "name", "type": "str"},
-        "type": {"key": "type", "type": "str"},
-        "system_data": {"key": "systemData", "type": "SystemData"},
-        "version": {"key": "properties.version", "type": "str"},
-        "database_name": {"key": "properties.databaseName", "type": "str"},
-        "database_user": {"key": "properties.databaseUser", "type": "str"},
-        "site_url": {"key": "properties.siteUrl", "type": "str"},
-        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
-    }
-
-    def __init__(
-        self,
-        *,
-        version: Optional[Union[str, "_models.WordpressVersions"]] = None,
-        database_name: Optional[str] = None,
-        database_user: Optional[str] = None,
-        **kwargs
-    ):
-        """
-        :keyword version: Application version. Known values are: "5.4.3", "5.4.2", "5.4.1", and "5.4".
-        :paramtype version: str or ~azure.mgmt.workloads.models.WordpressVersions
-        :keyword database_name: Database name used by the application.
-        :paramtype database_name: str
-        :keyword database_user: User name used by the application to connect to database.
-        :paramtype database_user: str
-        """
-        super().__init__(**kwargs)
-        self.version = version
-        self.database_name = database_name
-        self.database_user = database_user
-        self.site_url = None
-        self.provisioning_state = None
-
-
-class WordpressInstanceResourceList(_serialization.Model):
-    """WordPress instance resource list.
-
-    :ivar value: List of resources in current page.
-    :vartype value: list[~azure.mgmt.workloads.models.WordpressInstanceResource]
-    :ivar next_link: Link to next page of resources.
-    :vartype next_link: str
-    """
-
-    _attribute_map = {
-        "value": {"key": "value", "type": "[WordpressInstanceResource]"},
-        "next_link": {"key": "nextLink", "type": "str"},
-    }
-
-    def __init__(
-        self,
-        *,
-        value: Optional[List["_models.WordpressInstanceResource"]] = None,
-        next_link: Optional[str] = None,
-        **kwargs
-    ):
-        """
-        :keyword value: List of resources in current page.
-        :paramtype value: list[~azure.mgmt.workloads.models.WordpressInstanceResource]
-        :keyword next_link: Link to next page of resources.
-        :paramtype next_link: str
-        """
-        super().__init__(**kwargs)
-        self.value = value
-        self.next_link = next_link
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/models/_workloads_client_enums.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/models/_workloads_client_enums.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,141 +12,83 @@
 
 class ActionType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Enum. Indicates the action type. "Internal" refers to actions that are for internal only APIs."""
 
     INTERNAL = "Internal"
 
 
-class ApplicationProvisioningState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """WordPress instance provisioning state."""
+class ApplicationServerVirtualMachineType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Defines the type of application server VM."""
 
-    NOT_SPECIFIED = "NotSpecified"
-    ACCEPTED = "Accepted"
-    CREATED = "Created"
-    SUCCEEDED = "Succeeded"
-    FAILED = "Failed"
-    CANCELED = "Canceled"
-    INSTALLING = "Installing"
-
-
-class AzureFrontDoorEnabled(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Whether to enable Azure front door."""
-
-    ENABLED = "Enabled"
-    DISABLED = "Disabled"
+    ACTIVE = "Active"
+    STANDBY = "Standby"
+    UNKNOWN = "Unknown"
 
 
 class CentralServerVirtualMachineType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Defines the type of central server VM."""
 
     PRIMARY = "Primary"
     SECONDARY = "Secondary"
     UNKNOWN = "Unknown"
     ASCS = "ASCS"
     ERS_INACTIVE = "ERSInactive"
     ERS = "ERS"
     STANDBY = "Standby"
 
 
+class ConfigurationType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The type of file share config."""
+
+    SKIP = "Skip"
+    CREATE_AND_MOUNT = "CreateAndMount"
+    MOUNT = "Mount"
+
+
 class CreatedByType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The type of identity that created the resource."""
 
     USER = "User"
     APPLICATION = "Application"
     MANAGED_IDENTITY = "ManagedIdentity"
     KEY = "Key"
 
 
-class DatabaseTier(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Tier of the server SKU."""
+class DiskSkuName(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Defines the disk sku name."""
 
-    BURSTABLE = "Burstable"
-    GENERAL_PURPOSE = "GeneralPurpose"
-    MEMORY_OPTIMIZED = "MemoryOptimized"
-
-
-class DatabaseType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Database type."""
-
-    MY_SQL = "MySql"
-
-
-class DiskStorageType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Storage type."""
-
-    PREMIUM_LRS = "Premium_LRS"
     STANDARD_LRS = "Standard_LRS"
+    PREMIUM_LRS = "Premium_LRS"
     STANDARD_SSD_LRS = "StandardSSD_LRS"
-
-
-class EnableBackup(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Whether to enable Azure backup for the workload."""
-
-    ENABLED = "Enabled"
-    DISABLED = "Disabled"
-
-
-class EnableSslEnforcement(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Whether to enable SSL enforcement on the database."""
-
-    ENABLED = "Enabled"
-    DISABLED = "Disabled"
+    ULTRA_SSD_LRS = "UltraSSD_LRS"
+    PREMIUM_ZRS = "Premium_ZRS"
+    STANDARD_SSD_ZRS = "StandardSSD_ZRS"
+    PREMIUM_V2_LRS = "PremiumV2_LRS"
 
 
 class EnqueueReplicationServerType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Defines the type of Enqueue Replication Server."""
 
     ENQUEUE_REPLICATOR1 = "EnqueueReplicator1"
     ENQUEUE_REPLICATOR2 = "EnqueueReplicator2"
 
 
-class FileShareStorageType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """File share backing storage type."""
-
-    STANDARD_LRS = "Standard_LRS"
-    STANDARD_GRS = "Standard_GRS"
-    STANDARD_ZRS = "Standard_ZRS"
-    PREMIUM_LRS = "Premium_LRS"
-
-
-class FileShareType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Share type."""
-
-    NFS_ON_CONTROLLER = "NfsOnController"
-    AZURE_FILES = "AzureFiles"
-
-
-class HAEnabled(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Whether to enable HA for the server."""
-
-    ENABLED = "Enabled"
-    DISABLED = "Disabled"
-
-
-class LoadBalancerType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Load balancer type."""
-
-    APPLICATION_GATEWAY = "ApplicationGateway"
-    LOAD_BALANCER = "LoadBalancer"
-
-
-class LocationType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Type of the extended location."""
-
-    REGION = "Region"
-    EDGE_ZONE = "EdgeZone"
-
-
 class ManagedServiceIdentityType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Type of managed service identity (only None, UserAssigned types are allowed)."""
 
     NONE = "None"
     USER_ASSIGNED = "UserAssigned"
 
 
+class NamingPatternType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The pattern type to be used for resource naming."""
+
+    FULL_RESOURCE_NAME = "FullResourceName"
+
+
 class OperationProperties(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Defines the workload operation origin."""
 
     NOT_SPECIFIED = "NotSpecified"
     USER = "User"
     SYSTEM = "System"
 
@@ -157,74 +99,21 @@
     """
 
     USER = "user"
     SYSTEM = "system"
     USER_SYSTEM = "user,system"
 
 
-class OSImageOffer(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """OS image offer."""
-
-    UBUNTU_SERVER = "UbuntuServer"
-
-
-class OSImagePublisher(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """OS image publisher."""
-
-    CANONICAL = "Canonical"
-
-
-class OSImageSku(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """OS image sku."""
-
-    EIGHTEEN04_LTS = "18.04-LTS"
-    SIXTEEN04_LTS = "16.04-LTS"
-
-
-class OSImageVersion(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """OS image version."""
-
-    LATEST = "latest"
-
-
 class OSType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The OS Type."""
 
     LINUX = "Linux"
     WINDOWS = "Windows"
 
 
-class PHPVersion(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """PHP version."""
-
-    SEVEN2 = "7.2"
-    SEVEN3 = "7.3"
-    SEVEN4 = "7.4"
-
-
-class PhpWorkloadProvisioningState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Php workload resource provisioning state."""
-
-    NOT_SPECIFIED = "NotSpecified"
-    ACCEPTED = "Accepted"
-    CREATED = "Created"
-    SUCCEEDED = "Succeeded"
-    FAILED = "Failed"
-    CANCELED = "Canceled"
-    PROVISIONING = "Provisioning"
-    DELETING = "Deleting"
-
-
-class RedisCacheFamily(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Cache family."""
-
-    C = "C"
-    P = "P"
-
-
 class RoutingPreference(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Sets the routing preference of the SAP monitor. By default only RFC1918 traffic is routed to
     the customer VNET.
     """
 
     DEFAULT = "Default"
     ROUTE_ALL = "RouteAll"
@@ -279,14 +168,24 @@
     guarantees 99.99% availability.
     """
 
     AVAILABILITY_SET = "AvailabilitySet"
     AVAILABILITY_ZONE = "AvailabilityZone"
 
 
+class SapLandscapeMonitorProvisioningState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """State of provisioning of the SAP monitor."""
+
+    ACCEPTED = "Accepted"
+    CREATED = "Created"
+    FAILED = "Failed"
+    SUCCEEDED = "Succeeded"
+    CANCELED = "Canceled"
+
+
 class SAPProductType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Defines the SAP Product type."""
 
     ECC = "ECC"
     S4_HANA = "S4HANA"
     OTHER = "Other"
 
@@ -331,80 +230,25 @@
 
     STARTING = "Starting"
     RUNNING = "Running"
     STOPPING = "Stopping"
     OFFLINE = "Offline"
     PARTIALLY_RUNNING = "PartiallyRunning"
     UNAVAILABLE = "Unavailable"
-
-
-class SearchType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Search type."""
-
-    ELASTIC = "Elastic"
-
-
-class SkuRestrictionReasonCode(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """The SKU restriction reason code."""
-
-    NOT_SPECIFIED = "NotSpecified"
-    QUOTA_ID = "QuotaId"
-    NOT_AVAILABLE_FOR_SUBSCRIPTION = "NotAvailableForSubscription"
-
-
-class SkuRestrictionType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """The SKU restriction type."""
-
-    NOT_SPECIFIED = "NotSpecified"
-    LOCATION = "Location"
-    ZONE = "Zone"
-
-
-class SkuScaleType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Scale type of the SKU capacity."""
-
-    NONE = "None"
-    MANUAL = "Manual"
-    AUTOMATIC = "Automatic"
-
-
-class SkuTier(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """This field is required to be implemented by the Resource Provider if the service has more than
-    one tier, but is not required on a PUT.
-    """
-
-    FREE = "Free"
-    BASIC = "Basic"
-    STANDARD = "Standard"
-    PREMIUM = "Premium"
+    SOFT_SHUTDOWN = "SoftShutdown"
 
 
 class SslPreference(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Gets or sets certificate preference if secure communication is enabled."""
 
     DISABLED = "Disabled"
     ROOT_CERTIFICATE = "RootCertificate"
     SERVER_CERTIFICATE = "ServerCertificate"
 
 
-class WordpressVersions(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Application version."""
-
-    FIVE4_3 = "5.4.3"
-    FIVE4_2 = "5.4.2"
-    FIVE4_1 = "5.4.1"
-    FIVE4 = "5.4"
-
-
-class WorkloadKind(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Indicates which kind of php workload this resource represent e.g WordPress."""
-
-    WORD_PRESS = "WordPress"
-
-
 class WorkloadMonitorActionType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Defines the action type of workload operation."""
 
     NOT_SPECIFIED = "NotSpecified"
     INTERNAL = "Internal"
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/models/_patch.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/__init__.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,38 +2,34 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._php_workloads_operations import PhpWorkloadsOperations
-from ._wordpress_instances_operations import WordpressInstancesOperations
 from ._workloads_client_operations import WorkloadsClientOperationsMixin
 from ._sap_virtual_instances_operations import SAPVirtualInstancesOperations
 from ._sap_central_instances_operations import SAPCentralInstancesOperations
 from ._sap_database_instances_operations import SAPDatabaseInstancesOperations
 from ._sap_application_server_instances_operations import SAPApplicationServerInstancesOperations
-from ._operations import Operations
 from ._monitors_operations import MonitorsOperations
 from ._provider_instances_operations import ProviderInstancesOperations
-from ._skus_operations import SkusOperations
+from ._sap_landscape_monitor_operations import SapLandscapeMonitorOperations
+from ._operations import Operations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "PhpWorkloadsOperations",
-    "WordpressInstancesOperations",
     "WorkloadsClientOperationsMixin",
     "SAPVirtualInstancesOperations",
     "SAPCentralInstancesOperations",
     "SAPDatabaseInstancesOperations",
     "SAPApplicationServerInstancesOperations",
-    "Operations",
     "MonitorsOperations",
     "ProviderInstancesOperations",
-    "SkusOperations",
+    "SapLandscapeMonitorOperations",
+    "Operations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_sap_virtual_instances_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_virtual_instances_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 
 def build_create_request(
     resource_group_name: str, sap_virtual_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -83,16 +83,16 @@
 
 def build_get_request(
     resource_group_name: str, sap_virtual_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}",
@@ -118,16 +118,16 @@
 
 def build_update_request(
     resource_group_name: str, sap_virtual_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -156,16 +156,16 @@
 
 def build_delete_request(
     resource_group_name: str, sap_virtual_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}",
@@ -189,16 +189,16 @@
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances",
@@ -221,16 +221,16 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Workloads/sapVirtualInstances"
     )
@@ -251,16 +251,16 @@
 
 def build_start_request(
     resource_group_name: str, sap_virtual_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/start",
@@ -286,16 +286,16 @@
 
 def build_stop_request(
     resource_group_name: str, sap_virtual_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -355,15 +355,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPVirtualInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -525,15 +525,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.SAPVirtualInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPVirtualInstance] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -602,15 +602,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPVirtualInstance] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -739,15 +739,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPVirtualInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -807,15 +807,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -877,15 +877,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -938,15 +938,15 @@
         :return: An iterator like instance of either SAPVirtualInstance or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.workloads.models.SAPVirtualInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPVirtualInstanceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1023,15 +1023,15 @@
         :return: An iterator like instance of either SAPVirtualInstance or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.workloads.models.SAPVirtualInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPVirtualInstanceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1109,15 +1109,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         request = build_start_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -1179,15 +1179,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -1243,15 +1243,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -1416,15 +1416,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_sap_database_instances_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_database_instances_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     database_instance_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances/{databaseInstanceName}",
@@ -89,16 +89,16 @@
     database_instance_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -132,16 +132,16 @@
     database_instance_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -175,16 +175,16 @@
     database_instance_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances/{databaseInstanceName}",
@@ -211,16 +211,16 @@
 
 def build_list_request(
     resource_group_name: str, sap_virtual_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances",
@@ -240,14 +240,97 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_start_instance_request(
+    resource_group_name: str,
+    sap_virtual_instance_name: str,
+    database_instance_name: str,
+    subscription_id: str,
+    **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances/{databaseInstanceName}/start",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "sapVirtualInstanceName": _SERIALIZER.url("sap_virtual_instance_name", sap_virtual_instance_name, "str"),
+        "databaseInstanceName": _SERIALIZER.url("database_instance_name", database_instance_name, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_stop_instance_request(
+    resource_group_name: str,
+    sap_virtual_instance_name: str,
+    database_instance_name: str,
+    subscription_id: str,
+    **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances/{databaseInstanceName}/stop",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "sapVirtualInstanceName": _SERIALIZER.url("sap_virtual_instance_name", sap_virtual_instance_name, "str"),
+        "databaseInstanceName": _SERIALIZER.url("database_instance_name", database_instance_name, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 class SAPDatabaseInstancesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.workloads.WorkloadsClient`'s
@@ -290,15 +373,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPDatabaseInstance] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -349,15 +432,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPDatabaseInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -538,15 +621,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.SAPDatabaseInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPDatabaseInstance] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -607,15 +690,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPDatabaseInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -790,15 +873,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.SAPDatabaseInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPDatabaseInstance] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -854,15 +937,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -929,15 +1012,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -996,15 +1079,15 @@
         :return: An iterator like instance of either SAPDatabaseInstance or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.workloads.models.SAPDatabaseInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPDatabaseInstanceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1069,7 +1152,391 @@
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
     list.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances"
     }
+
+    def _start_instance_initial(
+        self, resource_group_name: str, sap_virtual_instance_name: str, database_instance_name: str, **kwargs: Any
+    ) -> Optional[_models.OperationStatusResult]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
+
+        request = build_start_instance_request(
+            resource_group_name=resource_group_name,
+            sap_virtual_instance_name=sap_virtual_instance_name,
+            database_instance_name=database_instance_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self._start_instance_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    _start_instance_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances/{databaseInstanceName}/start"
+    }
+
+    @distributed_trace
+    def begin_start_instance(
+        self, resource_group_name: str, sap_virtual_instance_name: str, database_instance_name: str, **kwargs: Any
+    ) -> LROPoller[_models.OperationStatusResult]:
+        """Starts the database instance of the SAP system.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param database_instance_name: Database resource name string modeled as parameter for auto
+         generation to work correctly. Required.
+        :type database_instance_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either OperationStatusResult or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._start_instance_initial(
+                resource_group_name=resource_group_name,
+                sap_virtual_instance_name=sap_virtual_instance_name,
+                database_instance_name=database_instance_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        if polling is True:
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
+            )
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_start_instance.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances/{databaseInstanceName}/start"
+    }
+
+    def _stop_instance_initial(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        database_instance_name: str,
+        body: Optional[Union[_models.StopRequest, IO]] = None,
+        **kwargs: Any
+    ) -> Optional[_models.OperationStatusResult]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IO, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "StopRequest")
+            else:
+                _json = None
+
+        request = build_stop_instance_request(
+            resource_group_name=resource_group_name,
+            sap_virtual_instance_name=sap_virtual_instance_name,
+            database_instance_name=database_instance_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self._stop_instance_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    _stop_instance_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances/{databaseInstanceName}/stop"
+    }
+
+    @overload
+    def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        database_instance_name: str,
+        body: Optional[_models.StopRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.OperationStatusResult]:
+        """Stops the database instance of the SAP system.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param database_instance_name: Database resource name string modeled as parameter for auto
+         generation to work correctly. Required.
+        :type database_instance_name: str
+        :param body: Stop request for the database instance of the SAP system. Default value is None.
+        :type body: ~azure.mgmt.workloads.models.StopRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either OperationStatusResult or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        database_instance_name: str,
+        body: Optional[IO] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.OperationStatusResult]:
+        """Stops the database instance of the SAP system.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param database_instance_name: Database resource name string modeled as parameter for auto
+         generation to work correctly. Required.
+        :type database_instance_name: str
+        :param body: Stop request for the database instance of the SAP system. Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either OperationStatusResult or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        database_instance_name: str,
+        body: Optional[Union[_models.StopRequest, IO]] = None,
+        **kwargs: Any
+    ) -> LROPoller[_models.OperationStatusResult]:
+        """Stops the database instance of the SAP system.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param database_instance_name: Database resource name string modeled as parameter for auto
+         generation to work correctly. Required.
+        :type database_instance_name: str
+        :param body: Stop request for the database instance of the SAP system. Is either a model type
+         or a IO type. Default value is None.
+        :type body: ~azure.mgmt.workloads.models.StopRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either OperationStatusResult or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._stop_instance_initial(
+                resource_group_name=resource_group_name,
+                sap_virtual_instance_name=sap_virtual_instance_name,
+                database_instance_name=database_instance_name,
+                body=body,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        if polling is True:
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
+            )
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_stop_instance.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/databaseInstances/{databaseInstanceName}/stop"
+    }
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_monitors_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_monitors_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Workloads/monitors")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
@@ -69,16 +69,16 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors",
@@ -101,16 +101,16 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}",
@@ -136,16 +136,16 @@
 
 def build_create_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -174,16 +174,16 @@
 
 def build_delete_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/monitors/{monitorName}",
@@ -209,16 +209,16 @@
 
 def build_update_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -275,15 +275,15 @@
         :return: An iterator like instance of either Monitor or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.workloads.models.Monitor]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.MonitorListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -362,15 +362,15 @@
         :return: An iterator like instance of either Monitor or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.workloads.models.Monitor]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.MonitorListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -463,15 +463,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.Monitor] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
@@ -516,15 +516,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Monitor] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -679,15 +679,15 @@
         :return: An instance of LROPoller that returns either Monitor or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.Monitor]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Monitor] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -742,15 +742,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
@@ -812,15 +812,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -956,15 +956,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Monitor] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_patch.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_workloads_client_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_workloads_client_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_sap_sizing_recommendations_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -72,16 +72,16 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_sap_supported_sku_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -105,16 +105,16 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_sap_disk_configurations_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -138,16 +138,16 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_sap_availability_zone_details_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -255,15 +255,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPSizingRecommendationResult] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -389,15 +389,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPSupportedResourceSkusResult] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -523,15 +523,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPDiskConfigurationsResult] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -661,15 +661,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPAvailabilityZoneDetailsResult] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_sap_application_server_instances_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_application_server_instances_operations.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     application_instance_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances/{applicationInstanceName}",
@@ -89,16 +89,16 @@
     application_instance_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -132,16 +132,16 @@
     application_instance_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -175,16 +175,16 @@
     application_instance_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances/{applicationInstanceName}",
@@ -211,16 +211,16 @@
 
 def build_list_request(
     resource_group_name: str, sap_virtual_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances",
@@ -240,14 +240,97 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_start_instance_request(
+    resource_group_name: str,
+    sap_virtual_instance_name: str,
+    application_instance_name: str,
+    subscription_id: str,
+    **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances/{applicationInstanceName}/start",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "sapVirtualInstanceName": _SERIALIZER.url("sap_virtual_instance_name", sap_virtual_instance_name, "str"),
+        "applicationInstanceName": _SERIALIZER.url("application_instance_name", application_instance_name, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_stop_instance_request(
+    resource_group_name: str,
+    sap_virtual_instance_name: str,
+    application_instance_name: str,
+    subscription_id: str,
+    **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances/{applicationInstanceName}/stop",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "sapVirtualInstanceName": _SERIALIZER.url("sap_virtual_instance_name", sap_virtual_instance_name, "str"),
+        "applicationInstanceName": _SERIALIZER.url("application_instance_name", application_instance_name, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 class SAPApplicationServerInstancesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.workloads.WorkloadsClient`'s
@@ -291,15 +374,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPApplicationServerInstance] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -350,15 +433,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPApplicationServerInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -539,15 +622,15 @@
         :rtype:
          ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.SAPApplicationServerInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPApplicationServerInstance] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -608,15 +691,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPApplicationServerInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -794,15 +877,15 @@
         :rtype:
          ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.SAPApplicationServerInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPApplicationServerInstance] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -858,15 +941,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -932,15 +1015,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -1001,15 +1084,15 @@
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.workloads.models.SAPApplicationServerInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPApplicationServerInstanceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1074,7 +1157,391 @@
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
     list.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances"
     }
+
+    def _start_instance_initial(
+        self, resource_group_name: str, sap_virtual_instance_name: str, application_instance_name: str, **kwargs: Any
+    ) -> Optional[_models.OperationStatusResult]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
+
+        request = build_start_instance_request(
+            resource_group_name=resource_group_name,
+            sap_virtual_instance_name=sap_virtual_instance_name,
+            application_instance_name=application_instance_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self._start_instance_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    _start_instance_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances/{applicationInstanceName}/start"
+    }
+
+    @distributed_trace
+    def begin_start_instance(
+        self, resource_group_name: str, sap_virtual_instance_name: str, application_instance_name: str, **kwargs: Any
+    ) -> LROPoller[_models.OperationStatusResult]:
+        """Starts the SAP Application Server Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param application_instance_name: The name of SAP Application Server instance resource.
+         Required.
+        :type application_instance_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either OperationStatusResult or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._start_instance_initial(
+                resource_group_name=resource_group_name,
+                sap_virtual_instance_name=sap_virtual_instance_name,
+                application_instance_name=application_instance_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        if polling is True:
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
+            )
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_start_instance.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances/{applicationInstanceName}/start"
+    }
+
+    def _stop_instance_initial(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        application_instance_name: str,
+        body: Optional[Union[_models.StopRequest, IO]] = None,
+        **kwargs: Any
+    ) -> Optional[_models.OperationStatusResult]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IO, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "StopRequest")
+            else:
+                _json = None
+
+        request = build_stop_instance_request(
+            resource_group_name=resource_group_name,
+            sap_virtual_instance_name=sap_virtual_instance_name,
+            application_instance_name=application_instance_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self._stop_instance_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    _stop_instance_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances/{applicationInstanceName}/stop"
+    }
+
+    @overload
+    def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        application_instance_name: str,
+        body: Optional[_models.StopRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.OperationStatusResult]:
+        """Stops the SAP Application Server Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param application_instance_name: The name of SAP Application Server instance resource.
+         Required.
+        :type application_instance_name: str
+        :param body: SAP Application server instance stop request body. Default value is None.
+        :type body: ~azure.mgmt.workloads.models.StopRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either OperationStatusResult or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        application_instance_name: str,
+        body: Optional[IO] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.OperationStatusResult]:
+        """Stops the SAP Application Server Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param application_instance_name: The name of SAP Application Server instance resource.
+         Required.
+        :type application_instance_name: str
+        :param body: SAP Application server instance stop request body. Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either OperationStatusResult or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        application_instance_name: str,
+        body: Optional[Union[_models.StopRequest, IO]] = None,
+        **kwargs: Any
+    ) -> LROPoller[_models.OperationStatusResult]:
+        """Stops the SAP Application Server Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param application_instance_name: The name of SAP Application Server instance resource.
+         Required.
+        :type application_instance_name: str
+        :param body: SAP Application server instance stop request body. Is either a model type or a IO
+         type. Default value is None.
+        :type body: ~azure.mgmt.workloads.models.StopRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either OperationStatusResult or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._stop_instance_initial(
+                resource_group_name=resource_group_name,
+                sap_virtual_instance_name=sap_virtual_instance_name,
+                application_instance_name=application_instance_name,
+                body=body,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        if polling is True:
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
+            )
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_stop_instance.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/applicationInstances/{applicationInstanceName}/stop"
+    }
```

## Comparing `azure-mgmt-workloads-1.0.0b2/azure/mgmt/workloads/operations/_sap_central_instances_operations.py` & `azure-mgmt-workloads-1.0.0b3/azure/mgmt/workloads/operations/_sap_central_instances_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     central_instance_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances/{centralInstanceName}",
@@ -89,16 +89,16 @@
     central_instance_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -132,16 +132,16 @@
     central_instance_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
@@ -175,16 +175,16 @@
     central_instance_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances/{centralInstanceName}",
@@ -211,16 +211,16 @@
 
 def build_list_request(
     resource_group_name: str, sap_virtual_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2021-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2021-12-01-preview")
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances",
@@ -240,14 +240,97 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_start_instance_request(
+    resource_group_name: str,
+    sap_virtual_instance_name: str,
+    central_instance_name: str,
+    subscription_id: str,
+    **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances/{centralInstanceName}/start",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "sapVirtualInstanceName": _SERIALIZER.url("sap_virtual_instance_name", sap_virtual_instance_name, "str"),
+        "centralInstanceName": _SERIALIZER.url("central_instance_name", central_instance_name, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_stop_instance_request(
+    resource_group_name: str,
+    sap_virtual_instance_name: str,
+    central_instance_name: str,
+    subscription_id: str,
+    **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2022-11-01-preview")
+    )
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances/{centralInstanceName}/stop",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "sapVirtualInstanceName": _SERIALIZER.url("sap_virtual_instance_name", sap_virtual_instance_name, "str"),
+        "centralInstanceName": _SERIALIZER.url("central_instance_name", central_instance_name, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 class SAPCentralInstancesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.workloads.WorkloadsClient`'s
@@ -290,15 +373,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPCentralServerInstance] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -349,15 +432,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPCentralServerInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -535,15 +618,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.SAPCentralServerInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPCentralServerInstance] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -604,15 +687,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPCentralServerInstance] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
@@ -790,15 +873,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.SAPCentralServerInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.SAPCentralServerInstance] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
@@ -854,15 +937,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             sap_virtual_instance_name=sap_virtual_instance_name,
@@ -930,15 +1013,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
@@ -999,15 +1082,15 @@
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.workloads.models.SAPCentralServerInstance]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2021-12-01-preview"] = kwargs.pop(
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
         )
         cls: ClsType[_models.SAPCentralInstanceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1072,7 +1155,391 @@
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
     list.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances"
     }
+
+    def _start_instance_initial(
+        self, resource_group_name: str, sap_virtual_instance_name: str, central_instance_name: str, **kwargs: Any
+    ) -> Optional[_models.OperationStatusResult]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
+
+        request = build_start_instance_request(
+            resource_group_name=resource_group_name,
+            sap_virtual_instance_name=sap_virtual_instance_name,
+            central_instance_name=central_instance_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self._start_instance_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    _start_instance_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances/{centralInstanceName}/start"
+    }
+
+    @distributed_trace
+    def begin_start_instance(
+        self, resource_group_name: str, sap_virtual_instance_name: str, central_instance_name: str, **kwargs: Any
+    ) -> LROPoller[_models.OperationStatusResult]:
+        """Starts the SAP Central Services Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param central_instance_name: Central Services Instance resource name string modeled as
+         parameter for auto generation to work correctly. Required.
+        :type central_instance_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either OperationStatusResult or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._start_instance_initial(
+                resource_group_name=resource_group_name,
+                sap_virtual_instance_name=sap_virtual_instance_name,
+                central_instance_name=central_instance_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        if polling is True:
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
+            )
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_start_instance.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances/{centralInstanceName}/start"
+    }
+
+    def _stop_instance_initial(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        central_instance_name: str,
+        body: Optional[Union[_models.StopRequest, IO]] = None,
+        **kwargs: Any
+    ) -> Optional[_models.OperationStatusResult]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.OperationStatusResult]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IO, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "StopRequest")
+            else:
+                _json = None
+
+        request = build_stop_instance_request(
+            resource_group_name=resource_group_name,
+            sap_virtual_instance_name=sap_virtual_instance_name,
+            central_instance_name=central_instance_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self._stop_instance_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    _stop_instance_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances/{centralInstanceName}/stop"
+    }
+
+    @overload
+    def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        central_instance_name: str,
+        body: Optional[_models.StopRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.OperationStatusResult]:
+        """Stops the SAP Central Services Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param central_instance_name: Central Services Instance resource name string modeled as
+         parameter for auto generation to work correctly. Required.
+        :type central_instance_name: str
+        :param body: SAP Central Services instance stop request body. Default value is None.
+        :type body: ~azure.mgmt.workloads.models.StopRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either OperationStatusResult or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        central_instance_name: str,
+        body: Optional[IO] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.OperationStatusResult]:
+        """Stops the SAP Central Services Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param central_instance_name: Central Services Instance resource name string modeled as
+         parameter for auto generation to work correctly. Required.
+        :type central_instance_name: str
+        :param body: SAP Central Services instance stop request body. Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either OperationStatusResult or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def begin_stop_instance(
+        self,
+        resource_group_name: str,
+        sap_virtual_instance_name: str,
+        central_instance_name: str,
+        body: Optional[Union[_models.StopRequest, IO]] = None,
+        **kwargs: Any
+    ) -> LROPoller[_models.OperationStatusResult]:
+        """Stops the SAP Central Services Instance.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param sap_virtual_instance_name: The name of the Virtual Instances for SAP solutions resource.
+         Required.
+        :type sap_virtual_instance_name: str
+        :param central_instance_name: Central Services Instance resource name string modeled as
+         parameter for auto generation to work correctly. Required.
+        :type central_instance_name: str
+        :param body: SAP Central Services instance stop request body. Is either a model type or a IO
+         type. Default value is None.
+        :type body: ~azure.mgmt.workloads.models.StopRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either OperationStatusResult or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.workloads.models.OperationStatusResult]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.OperationStatusResult] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._stop_instance_initial(
+                resource_group_name=resource_group_name,
+                sap_virtual_instance_name=sap_virtual_instance_name,
+                central_instance_name=central_instance_name,
+                body=body,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("OperationStatusResult", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        if polling is True:
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
+            )
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_stop_instance.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Workloads/sapVirtualInstances/{sapVirtualInstanceName}/centralInstances/{centralInstanceName}/stop"
+    }
```

