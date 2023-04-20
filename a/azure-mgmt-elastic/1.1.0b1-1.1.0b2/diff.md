# Comparing `tmp/azure-mgmt-elastic-1.1.0b1.zip` & `tmp/azure-mgmt-elastic-1.1.0b2.zip`

## zipinfo {}

```diff
@@ -1,85 +1,87 @@
-Zip file size: 155998 bytes, number of entries: 83
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/azure/
--rw-rw-r--  2.0 unx     1358 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/README.md
--rw-rw-r--  2.0 unx       38 b- defN 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/setup.cfg
--rw-rw-r--  2.0 unx     2820 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/setup.py
--rw-rw-r--  2.0 unx     1074 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/LICENSE
--rw-rw-r--  2.0 unx      213 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/MANIFEST.in
--rw-rw-r--  2.0 unx     3074 b- defN 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/PKG-INFO
--rw-rw-r--  2.0 unx      622 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/_meta.json
--rw-rw-r--  2.0 unx      827 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/CHANGELOG.md
--rw-rw-r--  2.0 unx     3582 b- defN 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        6 b- defN 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/top_level.txt
--rw-rw-r--  2.0 unx     3074 b- defN 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx      116 b- defN 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        1 b- defN 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/dependency_links.txt
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/
--rw-rw-r--  2.0 unx       65 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/models/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/
--rw-rw-r--  2.0 unx     1169 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_vendor.py
--rw-rw-r--  2.0 unx      902 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/__init__.py
--rw-rw-r--  2.0 unx    10018 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_microsoft_elastic.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_patch.py
--rw-rw-r--  2.0 unx    77450 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_serialization.py
--rw-rw-r--  2.0 unx      488 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_version.py
--rw-rw-r--  2.0 unx     3867 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_configuration.py
--rw-rw-r--  2.0 unx       26 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/py.typed
--rw-rw-r--  2.0 unx     4245 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/models/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/models/_patch.py
--rw-rw-r--  2.0 unx    55549 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/models/_models_py3.py
--rw-rw-r--  2.0 unx     3008 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/models/_microsoft_elastic_enums.py
--rw-rw-r--  2.0 unx     8237 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_monitored_resources_operations.py
--rw-rw-r--  2.0 unx     6721 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_vm_ingestion_operations.py
--rw-rw-r--  2.0 unx    10202 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_create_and_associate_ip_filter_operations.py
--rw-rw-r--  2.0 unx     6782 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_traffic_filters_operations.py
--rw-rw-r--  2.0 unx     6871 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_detach_and_delete_traffic_filter_operations.py
--rw-rw-r--  2.0 unx     2678 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/__init__.py
--rw-rw-r--  2.0 unx     6663 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_all_traffic_filters_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_patch.py
--rw-rw-r--  2.0 unx    11032 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_create_and_associate_pl_filter_operations.py
--rw-rw-r--  2.0 unx    10276 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_vm_collection_operations.py
--rw-rw-r--  2.0 unx     9875 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_associate_traffic_filter_operations.py
--rw-rw-r--  2.0 unx     8155 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_vm_host_operations.py
--rw-rw-r--  2.0 unx    44902 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_monitors_operations.py
--rw-rw-r--  2.0 unx    11045 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_external_user_operations.py
--rw-rw-r--  2.0 unx     6730 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_deployment_info_operations.py
--rw-rw-r--  2.0 unx    28851 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_tag_rules_operations.py
--rw-rw-r--  2.0 unx     9830 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_detach_traffic_filter_operations.py
--rw-rw-r--  2.0 unx    14515 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_monitor_operations.py
--rw-rw-r--  2.0 unx     6667 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_upgradable_versions_operations.py
--rw-rw-r--  2.0 unx     6740 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_list_associated_traffic_filters_operations.py
--rw-rw-r--  2.0 unx     6947 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-09 05:32 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/
--rw-rw-r--  2.0 unx      849 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/__init__.py
--rw-rw-r--  2.0 unx    10163 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/_microsoft_elastic.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/_patch.py
--rw-rw-r--  2.0 unx     3871 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/_configuration.py
--rw-rw-r--  2.0 unx     6911 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_monitored_resources_operations.py
--rw-rw-r--  2.0 unx     5345 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_vm_ingestion_operations.py
--rw-rw-r--  2.0 unx     8667 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_create_and_associate_ip_filter_operations.py
--rw-rw-r--  2.0 unx     5224 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_traffic_filters_operations.py
--rw-rw-r--  2.0 unx     5321 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_detach_and_delete_traffic_filter_operations.py
--rw-rw-r--  2.0 unx     2678 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     5297 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_all_traffic_filters_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_patch.py
--rw-rw-r--  2.0 unx     9204 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_create_and_associate_pl_filter_operations.py
--rw-rw-r--  2.0 unx     8670 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_vm_collection_operations.py
--rw-rw-r--  2.0 unx     8426 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_associate_traffic_filter_operations.py
--rw-rw-r--  2.0 unx     6815 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_vm_host_operations.py
--rw-rw-r--  2.0 unx    37353 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_monitors_operations.py
--rw-rw-r--  2.0 unx     9431 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_external_user_operations.py
--rw-rw-r--  2.0 unx     5349 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_deployment_info_operations.py
--rw-rw-r--  2.0 unx    23153 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_tag_rules_operations.py
--rw-rw-r--  2.0 unx     8381 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_detach_traffic_filter_operations.py
--rw-rw-r--  2.0 unx    13067 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_monitor_operations.py
--rw-rw-r--  2.0 unx     5294 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_upgradable_versions_operations.py
--rw-rw-r--  2.0 unx     5379 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_list_associated_traffic_filters_operations.py
--rw-rw-r--  2.0 unx     6192 b- defN 22-Nov-09 05:31 azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_operations.py
-83 files, 601787 bytes uncompressed, 137776 bytes compressed:  77.1%
+Zip file size: 164022 bytes, number of entries: 85
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/
+-rw-rw-r--  2.0 unx     1136 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/CHANGELOG.md
+-rw-rw-r--  2.0 unx     2130 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/README.md
+-rw-rw-r--  2.0 unx       38 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/setup.cfg
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/setup.py
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/LICENSE
+-rw-rw-r--  2.0 unx      622 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/_meta.json
+-rw-rw-r--  2.0 unx     4155 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/PKG-INFO
+-rw-rw-r--  2.0 unx      213 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/MANIFEST.in
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/
+-rw-rw-r--  2.0 unx     1302 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_vendor.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_patch.py
+-rw-rw-r--  2.0 unx    78824 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_serialization.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_microsoft_elastic.py
+-rw-rw-r--  2.0 unx     3815 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_configuration.py
+-rw-rw-r--  2.0 unx      887 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/__init__.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/py.typed
+-rw-rw-r--  2.0 unx      488 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_version.py
+-rw-rw-r--  2.0 unx     9932 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_associate_traffic_filter_operations.py
+-rw-rw-r--  2.0 unx     6790 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_traffic_filters_operations.py
+-rw-rw-r--  2.0 unx     6879 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_detach_and_delete_traffic_filter_operations.py
+-rw-rw-r--  2.0 unx    14489 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitor_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_patch.py
+-rw-rw-r--  2.0 unx    10264 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_create_and_associate_ip_filter_operations.py
+-rw-rw-r--  2.0 unx     6729 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_ingestion_operations.py
+-rw-rw-r--  2.0 unx     9887 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_detach_traffic_filter_operations.py
+-rw-rw-r--  2.0 unx     8167 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_host_operations.py
+-rw-rw-r--  2.0 unx     6748 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_list_associated_traffic_filters_operations.py
+-rw-rw-r--  2.0 unx    11094 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_create_and_associate_pl_filter_operations.py
+-rw-rw-r--  2.0 unx    28858 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_tag_rules_operations.py
+-rw-rw-r--  2.0 unx     6671 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_all_traffic_filters_operations.py
+-rw-rw-r--  2.0 unx     6675 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_upgradable_versions_operations.py
+-rw-rw-r--  2.0 unx    44918 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitors_operations.py
+-rw-rw-r--  2.0 unx    10290 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_collection_operations.py
+-rw-rw-r--  2.0 unx     2757 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/__init__.py
+-rw-rw-r--  2.0 unx    11048 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_external_user_operations.py
+-rw-rw-r--  2.0 unx    10467 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_organizations_operations.py
+-rw-rw-r--  2.0 unx     6738 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_deployment_info_operations.py
+-rw-rw-r--  2.0 unx     6924 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_operations.py
+-rw-rw-r--  2.0 unx     8249 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitored_resources_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_patch.py
+-rw-rw-r--  2.0 unx     2605 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_microsoft_elastic_enums.py
+-rw-rw-r--  2.0 unx     4461 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/__init__.py
+-rw-rw-r--  2.0 unx    60730 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_models_py3.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_patch.py
+-rw-rw-r--  2.0 unx    10496 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_microsoft_elastic.py
+-rw-rw-r--  2.0 unx     3863 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_configuration.py
+-rw-rw-r--  2.0 unx      834 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/__init__.py
+-rw-rw-r--  2.0 unx     8470 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_associate_traffic_filter_operations.py
+-rw-rw-r--  2.0 unx     5219 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_traffic_filters_operations.py
+-rw-rw-r--  2.0 unx     5316 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_detach_and_delete_traffic_filter_operations.py
+-rw-rw-r--  2.0 unx    13036 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitor_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx     8716 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_create_and_associate_ip_filter_operations.py
+-rw-rw-r--  2.0 unx     5340 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_ingestion_operations.py
+-rw-rw-r--  2.0 unx     8425 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_detach_traffic_filter_operations.py
+-rw-rw-r--  2.0 unx     6814 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_host_operations.py
+-rw-rw-r--  2.0 unx     5374 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_list_associated_traffic_filters_operations.py
+-rw-rw-r--  2.0 unx     9253 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_create_and_associate_pl_filter_operations.py
+-rw-rw-r--  2.0 unx    23116 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_tag_rules_operations.py
+-rw-rw-r--  2.0 unx     5292 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_all_traffic_filters_operations.py
+-rw-rw-r--  2.0 unx     5289 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_upgradable_versions_operations.py
+-rw-rw-r--  2.0 unx    37307 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitors_operations.py
+-rw-rw-r--  2.0 unx     8679 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_collection_operations.py
+-rw-rw-r--  2.0 unx     2757 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx     9429 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_external_user_operations.py
+-rw-rw-r--  2.0 unx     8978 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_organizations_operations.py
+-rw-rw-r--  2.0 unx     5344 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_deployment_info_operations.py
+-rw-rw-r--  2.0 unx     6177 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx     6910 b- defN 23-Apr-20 03:16 azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitored_resources_operations.py
+-rw-rw-r--  2.0 unx        1 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        6 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx      124 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/requires.txt
+-rw-rw-r--  2.0 unx     3704 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     4155 b- defN 23-Apr-20 03:17 azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/PKG-INFO
+85 files, 632117 bytes uncompressed, 145300 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -1,250 +1,256 @@
-Filename: azure-mgmt-elastic-1.1.0b1/
+Filename: azure-mgmt-elastic-1.1.0b2/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/
+Filename: azure-mgmt-elastic-1.1.0b2/azure/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/
+Filename: azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/README.md
+Filename: azure-mgmt-elastic-1.1.0b2/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/setup.cfg
+Filename: azure-mgmt-elastic-1.1.0b2/README.md
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/setup.py
+Filename: azure-mgmt-elastic-1.1.0b2/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/LICENSE
+Filename: azure-mgmt-elastic-1.1.0b2/setup.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/MANIFEST.in
+Filename: azure-mgmt-elastic-1.1.0b2/LICENSE
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/PKG-INFO
+Filename: azure-mgmt-elastic-1.1.0b2/_meta.json
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/_meta.json
+Filename: azure-mgmt-elastic-1.1.0b2/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/CHANGELOG.md
+Filename: azure-mgmt-elastic-1.1.0b2/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/SOURCES.txt
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/top_level.txt
+Filename: azure-mgmt-elastic-1.1.0b2/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/PKG-INFO
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/requires.txt
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/not-zip-safe
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/dependency_links.txt
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/__init__.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/__init__.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/models/
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_microsoft_elastic.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_vendor.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/py.typed
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/__init__.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_version.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_microsoft_elastic.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_associate_traffic_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_patch.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_traffic_filters_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_serialization.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_detach_and_delete_traffic_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_version.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitor_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_configuration.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/py.typed
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_create_and_associate_ip_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/models/__init__.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_ingestion_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/models/_patch.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_detach_traffic_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/models/_models_py3.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_host_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/models/_microsoft_elastic_enums.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_list_associated_traffic_filters_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_monitored_resources_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_create_and_associate_pl_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_vm_ingestion_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_tag_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_create_and_associate_ip_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_all_traffic_filters_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_traffic_filters_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_upgradable_versions_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_detach_and_delete_traffic_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitors_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/__init__.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_collection_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_all_traffic_filters_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_patch.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_external_user_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_create_and_associate_pl_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_organizations_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_vm_collection_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_deployment_info_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_associate_traffic_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_vm_host_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitored_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_monitors_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_external_user_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_microsoft_elastic_enums.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_deployment_info_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_tag_rules_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_detach_traffic_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_monitor_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_upgradable_versions_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_microsoft_elastic.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_list_associated_traffic_filters_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_associate_traffic_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/__init__.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_traffic_filters_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/_microsoft_elastic.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_detach_and_delete_traffic_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/_patch.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitor_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/_configuration.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_monitored_resources_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_create_and_associate_ip_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_vm_ingestion_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_ingestion_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_create_and_associate_ip_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_detach_traffic_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_traffic_filters_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_host_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_detach_and_delete_traffic_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_list_associated_traffic_filters_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/__init__.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_create_and_associate_pl_filter_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_all_traffic_filters_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_tag_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_patch.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_all_traffic_filters_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_create_and_associate_pl_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_upgradable_versions_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_vm_collection_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitors_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_associate_traffic_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_collection_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_vm_host_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_monitors_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_external_user_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_external_user_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_organizations_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_deployment_info_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_deployment_info_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_tag_rules_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_detach_traffic_filter_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitored_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_monitor_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_upgradable_versions_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_list_associated_traffic_filters_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_operations.py
+Filename: azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/SOURCES.txt
+Comment: 
+
+Filename: azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/dependency_links.txt
+Comment: 
+
+Filename: azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/PKG-INFO
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-elastic-1.1.0b1/setup.py` & `azure-mgmt-elastic-1.1.0b2/setup.py`

 * *Files 9% similar despite different names*

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

## Comparing `azure-mgmt-elastic-1.1.0b1/LICENSE` & `azure-mgmt-elastic-1.1.0b2/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b1/PKG-INFO` & `azure-mgmt-elastic-1.1.0b2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-elastic
-Version: 1.1.0b1
+Version: 1.1.0b2
 Summary: Microsoft Azure Elastic Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -27,36 +27,81 @@
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
-Code samples for this package can be found at [Elastic Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
-Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+- Python 3.7+ is required to use this package.
+- [Azure subscription](https://azure.microsoft.com/free/)
 
+### Install the package
 
-# Provide Feedback
+```bash
+pip install azure-mgmt-elastic
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
+from azure.mgmt.elastic import MicrosoftElastic
+import os
+
+sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
+client = MicrosoftElastic(credential=DefaultAzureCredential(), subscription_id=sub_id)
+```
+
+## Examples
+
+Code samples for this package can be found at:
+- [Search Elastic Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
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
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-elastic%2FREADME.png)
 
 
 # Release History
 
+## 1.1.0b2 (2023-04-20)
+
+### Features Added
+
+  - Added operation group OrganizationsOperations
+  - Model DeploymentInfoResponse has a new parameter deployment_url
+  - Model DeploymentInfoResponse has a new parameter marketplace_saas_info
+  - Model ElasticMonitorResource has a new parameter generate_api_key
+
 ## 1.1.0b1 (2022-11-08)
 
 ### Features Added
 
   - Added operation group AllTrafficFiltersOperations
   - Added operation group AssociateTrafficFilterOperations
   - Added operation group CreateAndAssociateIPFilterOperations
```

## Comparing `azure-mgmt-elastic-1.1.0b1/_meta.json` & `azure-mgmt-elastic-1.1.0b2/_meta.json`

 * *Files 14% similar despite different names*

### Pretty-printed

 * *Similarity: 0.7777777777777777%*

 * *Differences: {"'autorest_command'": "'autorest specification/elastic/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.4.3 --use=@autorest/modelerfour@4.24.3 '*

 * *                       "--version=3.9.2 --version-tolerant=False'",*

 * * "'commit'": "'969fd0c2634fbcc1975d7abe3749330a5145a97c'",*

 * * "'use'": "{insert: […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.2",
-    "autorest_command": "autorest specification/elastic/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.2.1 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
-    "commit": "4903b1ed79e30f689d7c469cfa06734cfcd106d6",
+    "autorest_command": "autorest specification/elastic/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.4.3 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
+    "commit": "969fd0c2634fbcc1975d7abe3749330a5145a97c",
     "readme": "specification/elastic/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.2.1",
+        "@autorest/python@6.4.3",
         "@autorest/modelerfour@4.24.3"
     ]
 }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/SOURCES.txt` & `azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 azure/mgmt/elastic/aio/operations/_detach_traffic_filter_operations.py
 azure/mgmt/elastic/aio/operations/_external_user_operations.py
 azure/mgmt/elastic/aio/operations/_list_associated_traffic_filters_operations.py
 azure/mgmt/elastic/aio/operations/_monitor_operations.py
 azure/mgmt/elastic/aio/operations/_monitored_resources_operations.py
 azure/mgmt/elastic/aio/operations/_monitors_operations.py
 azure/mgmt/elastic/aio/operations/_operations.py
+azure/mgmt/elastic/aio/operations/_organizations_operations.py
 azure/mgmt/elastic/aio/operations/_patch.py
 azure/mgmt/elastic/aio/operations/_tag_rules_operations.py
 azure/mgmt/elastic/aio/operations/_traffic_filters_operations.py
 azure/mgmt/elastic/aio/operations/_upgradable_versions_operations.py
 azure/mgmt/elastic/aio/operations/_vm_collection_operations.py
 azure/mgmt/elastic/aio/operations/_vm_host_operations.py
 azure/mgmt/elastic/aio/operations/_vm_ingestion_operations.py
@@ -53,14 +54,15 @@
 azure/mgmt/elastic/operations/_detach_traffic_filter_operations.py
 azure/mgmt/elastic/operations/_external_user_operations.py
 azure/mgmt/elastic/operations/_list_associated_traffic_filters_operations.py
 azure/mgmt/elastic/operations/_monitor_operations.py
 azure/mgmt/elastic/operations/_monitored_resources_operations.py
 azure/mgmt/elastic/operations/_monitors_operations.py
 azure/mgmt/elastic/operations/_operations.py
+azure/mgmt/elastic/operations/_organizations_operations.py
 azure/mgmt/elastic/operations/_patch.py
 azure/mgmt/elastic/operations/_tag_rules_operations.py
 azure/mgmt/elastic/operations/_traffic_filters_operations.py
 azure/mgmt/elastic/operations/_upgradable_versions_operations.py
 azure/mgmt/elastic/operations/_vm_collection_operations.py
 azure/mgmt/elastic/operations/_vm_host_operations.py
 azure/mgmt/elastic/operations/_vm_ingestion_operations.py
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure_mgmt_elastic.egg-info/PKG-INFO` & `azure-mgmt-elastic-1.1.0b2/azure_mgmt_elastic.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-elastic
-Version: 1.1.0b1
+Version: 1.1.0b2
 Summary: Microsoft Azure Elastic Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -27,36 +27,81 @@
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
-Code samples for this package can be found at [Elastic Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
-Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+- Python 3.7+ is required to use this package.
+- [Azure subscription](https://azure.microsoft.com/free/)
 
+### Install the package
 
-# Provide Feedback
+```bash
+pip install azure-mgmt-elastic
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
+from azure.mgmt.elastic import MicrosoftElastic
+import os
+
+sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
+client = MicrosoftElastic(credential=DefaultAzureCredential(), subscription_id=sub_id)
+```
+
+## Examples
+
+Code samples for this package can be found at:
+- [Search Elastic Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
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
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-elastic%2FREADME.png)
 
 
 # Release History
 
+## 1.1.0b2 (2023-04-20)
+
+### Features Added
+
+  - Added operation group OrganizationsOperations
+  - Model DeploymentInfoResponse has a new parameter deployment_url
+  - Model DeploymentInfoResponse has a new parameter marketplace_saas_info
+  - Model ElasticMonitorResource has a new parameter generate_api_key
+
 ## 1.1.0b1 (2022-11-08)
 
 ### Features Added
 
   - Added operation group AllTrafficFiltersOperations
   - Added operation group AssociateTrafficFilterOperations
   - Added operation group CreateAndAssociateIPFilterOperations
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_vendor.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_vendor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from typing import List, cast
+
 from azure.core.pipeline.transport import HttpRequest
 
 
 def _convert_request(request, files=None):
     data = request.content if not files else None
     request = HttpRequest(method=request.method, url=request.url, headers=request.headers, data=data)
     if files:
@@ -18,10 +20,11 @@
 
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
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/__init__.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,18 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._microsoft_elastic import MicrosoftElastic
-from ._version import VERSION
-
-__version__ = VERSION
 
 try:
     from ._patch import __all__ as _patch_all
-    from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+    from ._patch import *  # pylint: disable=unused-wildcard-import
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "MicrosoftElastic",
 ]
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_microsoft_elastic.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_microsoft_elastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from copy import deepcopy
 from typing import Any, TYPE_CHECKING
 
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
 
-from . import models
+from . import models as _models
 from ._configuration import MicrosoftElasticConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import (
     AllTrafficFiltersOperations,
     AssociateTrafficFilterOperations,
     CreateAndAssociateIPFilterOperations,
     CreateAndAssociatePLFilterOperations,
@@ -25,14 +25,15 @@
     DetachTrafficFilterOperations,
     ExternalUserOperations,
     ListAssociatedTrafficFiltersOperations,
     MonitorOperations,
     MonitoredResourcesOperations,
     MonitorsOperations,
     Operations,
+    OrganizationsOperations,
     TagRulesOperations,
     TrafficFiltersOperations,
     UpgradableVersionsOperations,
     VMCollectionOperations,
     VMHostOperations,
     VMIngestionOperations,
 )
@@ -84,39 +85,41 @@
     :ivar detach_and_delete_traffic_filter: DetachAndDeleteTrafficFilterOperations operations
     :vartype detach_and_delete_traffic_filter:
      azure.mgmt.elastic.operations.DetachAndDeleteTrafficFilterOperations
     :ivar detach_traffic_filter: DetachTrafficFilterOperations operations
     :vartype detach_traffic_filter: azure.mgmt.elastic.operations.DetachTrafficFilterOperations
     :ivar traffic_filters: TrafficFiltersOperations operations
     :vartype traffic_filters: azure.mgmt.elastic.operations.TrafficFiltersOperations
+    :ivar organizations: OrganizationsOperations operations
+    :vartype organizations: azure.mgmt.elastic.operations.OrganizationsOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The Azure subscription ID. This is a GUID-formatted string (e.g.
      00000000-0000-0000-0000-000000000000). Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-07-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-02-01-preview". Note that overriding
      this default value may result in unsupported behavior.
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
         self._config = MicrosoftElasticConfiguration(credential=credential, subscription_id=subscription_id, **kwargs)
-        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
-        client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
+        client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.monitors = MonitorsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.monitored_resources = MonitoredResourcesOperations(
             self._client, self._config, self._serialize, self._deserialize
@@ -149,14 +152,15 @@
         self.detach_and_delete_traffic_filter = DetachAndDeleteTrafficFilterOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.detach_traffic_filter = DetachTrafficFilterOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.traffic_filters = TrafficFiltersOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.organizations = OrganizationsOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
@@ -172,19 +176,16 @@
         :rtype: ~azure.core.rest.HttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, **kwargs)
 
-    def close(self):
-        # type: () -> None
+    def close(self) -> None:
         self._client.close()
 
-    def __enter__(self):
-        # type: () -> MicrosoftElastic
+    def __enter__(self) -> "MicrosoftElastic":
         self._client.__enter__()
         return self
 
-    def __exit__(self, *exc_details):
-        # type: (Any) -> None
+    def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_patch.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_serialization.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,56 +21,71 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 #
 # --------------------------------------------------------------------------
 
 # pylint: skip-file
+# pyright: reportUnnecessaryTypeIgnoreComment=false
 
 from base64 import b64decode, b64encode
 import calendar
 import datetime
 import decimal
 import email
 from enum import Enum
 import json
 import logging
 import re
 import sys
 import codecs
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
-    from urllib.parse import quote  # type: ignore
+    from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
-import isodate
-
-from typing import Dict, Any, cast, TYPE_CHECKING
+import isodate  # type: ignore
 
 from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
+from azure.core.serialization import NULL as AzureCoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
-if TYPE_CHECKING:
-    from typing import Optional, Union, AnyStr, IO, Mapping
+ModelType = TypeVar("ModelType", bound="Model")
+JSON = MutableMapping[str, Any]
 
 
 class RawDeserializer:
 
     # Accept "text" because we're open minded people...
     JSON_REGEXP = re.compile(r"^(application|text)/([a-z+.]+\+)?json$")
 
     # Name used in context
     CONTEXT_NAME = "deserialized_data"
 
     @classmethod
-    def deserialize_from_text(cls, data, content_type=None):
-        # type: (Optional[Union[AnyStr, IO]], Optional[str]) -> Any
+    def deserialize_from_text(cls, data: Optional[Union[AnyStr, IO]], content_type: Optional[str] = None) -> Any:
         """Decode data according to content-type.
 
         Accept a stream of data as well, but will be load at once in memory for now.
 
         If no content-type, will return the string version (not bytes, not stream)
 
         :param data: Input, could be bytes or stream (will be decoded with UTF8) or text
@@ -128,16 +143,15 @@
                 # The function hack is because Py2.7 messes up with exception
                 # context otherwise.
                 _LOGGER.critical("Wasn't XML not JSON, failing")
                 raise_with_traceback(DeserializationError, "XML is invalid")
         raise DeserializationError("Cannot deserialize content-type: {}".format(content_type))
 
     @classmethod
-    def deserialize_from_http_generics(cls, body_bytes, headers):
-        # type: (Optional[Union[AnyStr, IO]], Mapping) -> Any
+    def deserialize_from_http_generics(cls, body_bytes: Optional[Union[AnyStr, IO]], headers: Mapping) -> Any:
         """Deserialize from HTTP response.
 
         Use bytes and headers to NOT use any requests/aiohttp or whatever
         specific implementation.
         Headers will tested for "content-type"
         """
         # Try to use content-type from headers if available
@@ -156,16 +170,16 @@
         return None
 
 
 try:
     basestring  # type: ignore
     unicode_str = unicode  # type: ignore
 except NameError:
-    basestring = str  # type: ignore
-    unicode_str = str  # type: ignore
+    basestring = str
+    unicode_str = str
 
 _LOGGER = logging.getLogger(__name__)
 
 try:
     _long_type = long  # type: ignore
 except NameError:
     _long_type = int
@@ -184,15 +198,15 @@
 
     def dst(self, dt):
         """No daylight saving for UTC."""
         return datetime.timedelta(hours=1)
 
 
 try:
-    from datetime import timezone as _FixedOffset
+    from datetime import timezone as _FixedOffset  # type: ignore
 except ImportError:  # Python 2.7
 
     class _FixedOffset(datetime.tzinfo):  # type: ignore
         """Fixed offset in minutes east from UTC.
         Copy/pasted from Python doc
         :param datetime.timedelta offset: offset in timedelta format
         """
@@ -215,15 +229,15 @@
         def __getinitargs__(self):
             return (self.__offset,)
 
 
 try:
     from datetime import timezone
 
-    TZ_UTC = timezone.utc  # type: ignore
+    TZ_UTC = timezone.utc
 except ImportError:
     TZ_UTC = UTC()  # type: ignore
 
 _FLATTEN = re.compile(r"(?<!\\)\.")
 
 
 def attribute_transformer(key, attr_desc, value):
@@ -272,79 +286,84 @@
 
 
 class Model(object):
     """Mixin for all client request body/response body models to support
     serialization and deserialization.
     """
 
-    _subtype_map = {}  # type: Dict[str, Dict[str, Any]]
-    _attribute_map = {}  # type: Dict[str, Dict[str, Any]]
-    _validation = {}  # type: Dict[str, Dict[str, Any]]
+    _subtype_map: Dict[str, Dict[str, Any]] = {}
+    _attribute_map: Dict[str, Dict[str, Any]] = {}
+    _validation: Dict[str, Dict[str, Any]] = {}
 
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
-            cls._xml_map
+            cls._xml_map  # type: ignore
         except AttributeError:
             return False
         return True
 
     @classmethod
     def _create_xml_node(cls):
         """Create XML node."""
         try:
-            xml_map = cls._xml_map
+            xml_map = cls._xml_map  # type: ignore
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
@@ -383,41 +402,46 @@
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
@@ -449,15 +473,15 @@
             if subtype_value:
                 # Try to match base class. Can be class name only
                 # (bug to fix in Autorest to support x-ms-discriminator-name)
                 if cls.__name__ == subtype_value:
                     return cls
                 flatten_mapping_type = cls._flatten_subtype(subtype_key, objects)
                 try:
-                    return objects[flatten_mapping_type[subtype_value]]
+                    return objects[flatten_mapping_type[subtype_value]]  # type: ignore
                 except KeyError:
                     _LOGGER.warning(
                         "Subtype value %s has no mapping, use base class %s.",
                         subtype_value,
                         cls.__name__,
                     )
                     break
@@ -517,15 +541,15 @@
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
@@ -533,15 +557,15 @@
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
@@ -602,46 +626,45 @@
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
                                 xml_name = "{}{}".format(xml_ns, xml_name)
-                            serialized.set(xml_name, new_attr)
+                            serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
-                            serialized.text = new_attr
+                            serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
-                            serialized.extend(new_attr)
+                            serialized.extend(new_attr)  # type: ignore
                         elif isinstance(new_attr, ET.Element):
                             # If the down XML has no XML/Name, we MUST replace the tag with the local tag. But keeping the namespaces.
                             if "name" not in getattr(orig_attr, "_xml_map", {}):
                                 splitted_tag = new_attr.tag.split("}")
                                 if len(splitted_tag) == 2:  # Namespace
                                     new_attr.tag = "}".join([splitted_tag[0], xml_name])
                                 else:
                                     new_attr.tag = xml_name
-                            serialized.append(new_attr)
+                            serialized.append(new_attr)  # type: ignore
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
                             local_node.text = unicode_str(new_attr)
-                            serialized.append(local_node)
+                            serialized.append(local_node)  # type: ignore
                     else:  # JSON
-                        for k in reversed(keys):
-                            unflattened = {k: new_attr}
-                            new_attr = unflattened
+                        for k in reversed(keys):  # type: ignore
+                            new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
-                        for k in keys:
+                        for k in keys:  # type: ignore
                             if k not in _serialized:
-                                _serialized.update(_new_attr)
-                            _new_attr = _new_attr[k]
+                                _serialized.update(_new_attr)  # type: ignore
+                            _new_attr = _new_attr[k]  # type: ignore
                             _serialized = _serialized[k]
                 except ValueError:
                     continue
 
         except (AttributeError, KeyError, TypeError) as err:
             msg = "Attribute {} in object {} cannot be serialized.\n{}".format(attr_name, class_name, str(target_obj))
             raise_with_traceback(SerializationError, msg, err)
@@ -655,31 +678,31 @@
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
         if internal_data_type and not isinstance(internal_data_type, Enum):
             try:
                 deserializer = Deserializer(self.dependencies)
                 # Since it's on serialization, it's almost sure that format is not JSON REST
                 # We're not able to deal with additional properties for now.
                 deserializer.additional_properties_detection = False
                 if is_xml_model_serialization:
-                    deserializer.key_extractors = [
+                    deserializer.key_extractors = [  # type: ignore
                         attribute_key_case_insensitive_extractor,
                     ]
                 else:
                     deserializer.key_extractors = [
                         rest_key_case_insensitive_extractor,
                         attribute_key_case_insensitive_extractor,
                         last_rest_key_case_insensitive_extractor,
@@ -776,14 +799,16 @@
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
@@ -839,15 +864,15 @@
         """
         try:  # If I received an enum, return its value
             return data.value
         except AttributeError:
             pass
 
         try:
-            if isinstance(data, unicode):
+            if isinstance(data, unicode):  # type: ignore
                 # Don't change it, JSON and XML ElementTree are totally able
                 # to serialize correctly u'' strings
                 return data
         except NameError:
             return str(data)
         else:
             return str(data)
@@ -997,18 +1022,18 @@
     @staticmethod
     def serialize_enum(attr, enum_obj=None):
         try:
             result = attr.value
         except AttributeError:
             result = attr
         try:
-            enum_obj(result)
+            enum_obj(result)  # type: ignore
             return result
         except ValueError:
-            for enum_value in enum_obj:
+            for enum_value in enum_obj:  # type: ignore
                 if enum_value.value.lower() == str(attr).lower():
                     return enum_value.value
             error = "{!r} is not valid value for enum {!r}"
             raise SerializationError(error.format(attr, enum_obj))
 
     @staticmethod
     def serialize_bytearray(attr, **kwargs):
@@ -1160,15 +1185,16 @@
 
 
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
@@ -1331,15 +1357,15 @@
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
@@ -1351,15 +1377,15 @@
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
@@ -1412,15 +1438,15 @@
             return self.deserialize_data(data, response)
         elif isinstance(response, type) and issubclass(response, Enum):
             return self.deserialize_enum(data, response)
 
         if data is None:
             return data
         try:
-            attributes = response._attribute_map
+            attributes = response._attribute_map  # type: ignore
             d_attrs = {}
             for attr, attr_desc in attributes.items():
                 # Check empty string. If it's not empty, someone has a real "additionalProperties"...
                 if attr == "additional_properties" and attr_desc["key"] == "":
                     continue
                 raw_value = None
                 # Enhance attr_desc with some dynamic data
@@ -1440,15 +1466,15 @@
                             _LOGGER.warning(msg, found_value, key_extractor, attr)
                             continue
                         raw_value = found_value
 
                 value = self.deserialize_data(raw_value, attr_desc["type"])
                 d_attrs[attr] = value
         except (AttributeError, TypeError, KeyError) as err:
-            msg = "Unable to deserialize to object: " + class_name
+            msg = "Unable to deserialize to object: " + class_name  # type: ignore
             raise_with_traceback(DeserializationError, msg, err)
         else:
             additional_properties = self._build_additional_properties(attributes, data)
             return self._instantiate_model(response, d_attrs, additional_properties)
 
     def _build_additional_properties(self, attribute_map, data):
         if not self.additional_properties_detection:
@@ -1470,40 +1496,40 @@
 
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
@@ -1539,15 +1565,15 @@
             return RawDeserializer.deserialize_from_http_generics(raw_data.text(), raw_data.headers)
 
         # Assume this enough to recognize requests.Response without importing it.
         if hasattr(raw_data, "_content_consumed"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text, raw_data.headers)
 
         if isinstance(raw_data, (basestring, bytes)) or hasattr(raw_data, "read"):
-            return RawDeserializer.deserialize_from_text(raw_data, content_type)
+            return RawDeserializer.deserialize_from_text(raw_data, content_type)  # type: ignore
         return raw_data
 
     def _instantiate_model(self, response, attrs, additional_properties=None):
         """Instantiate a response model passing in deserialized args.
 
         :param response: The response model class.
         :param d_attrs: The deserialized response attributes.
@@ -1561,15 +1587,15 @@
                 response_obj = response(**kwargs)
                 for attr in readonly:
                     setattr(response_obj, attr, attrs.get(attr))
                 if additional_properties:
                     response_obj.additional_properties = additional_properties
                 return response_obj
             except TypeError as err:
-                msg = "Unable to deserialize {} into model {}. ".format(kwargs, response)
+                msg = "Unable to deserialize {} into model {}. ".format(kwargs, response)  # type: ignore
                 raise DeserializationError(msg + str(err))
         else:
             try:
                 for attr, value in attrs.items():
                     setattr(response, attr, value)
                 return response
             except Exception as exp:
@@ -1743,15 +1769,15 @@
         # We might be here because we have an enum modeled as string,
         # and we try to deserialize a partial dict with enum inside
         if isinstance(data, Enum):
             return data
 
         # Consider this is real string
         try:
-            if isinstance(data, unicode):
+            if isinstance(data, unicode):  # type: ignore
                 return data
         except NameError:
             return str(data)
         else:
             return str(data)
 
     @staticmethod
@@ -1794,58 +1820,58 @@
 
         :param str attr: response string to be deserialized.
         :rtype: bytearray
         :raises: TypeError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        return bytearray(b64decode(attr))
+        return bytearray(b64decode(attr))  # type: ignore
 
     @staticmethod
     def deserialize_base64(attr):
         """Deserialize base64 encoded string into string.
 
         :param str attr: response string to be deserialized.
         :rtype: bytearray
         :raises: TypeError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        padding = "=" * (3 - (len(attr) + 3) % 4)
-        attr = attr + padding
+        padding = "=" * (3 - (len(attr) + 3) % 4)  # type: ignore
+        attr = attr + padding  # type: ignore
         encoded = attr.replace("-", "+").replace("_", "/")
         return b64decode(encoded)
 
     @staticmethod
     def deserialize_decimal(attr):
         """Deserialize string into Decimal object.
 
         :param str attr: response string to be deserialized.
         :rtype: Decimal
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            return decimal.Decimal(attr)
+            return decimal.Decimal(attr)  # type: ignore
         except decimal.DecimalException as err:
             msg = "Invalid decimal {}".format(attr)
             raise_with_traceback(DeserializationError, msg, err)
 
     @staticmethod
     def deserialize_long(attr):
         """Deserialize string into long (Py2) or int (Py3).
 
         :param str attr: response string to be deserialized.
         :rtype: long or int
         :raises: ValueError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        return _long_type(attr)
+        return _long_type(attr)  # type: ignore
 
     @staticmethod
     def deserialize_duration(attr):
         """Deserialize ISO-8601 formatted string into TimeDelta object.
 
         :param str attr: response string to be deserialized.
         :rtype: TimeDelta
@@ -1867,45 +1893,45 @@
 
         :param str attr: response string to be deserialized.
         :rtype: Date
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        if re.search(r"[^\W\d_]", attr, re.I + re.U):
+        if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         # This must NOT use defaultmonth/defaultday. Using None ensure this raises an exception.
         return isodate.parse_date(attr, defaultmonth=None, defaultday=None)
 
     @staticmethod
     def deserialize_time(attr):
         """Deserialize ISO-8601 formatted string into time object.
 
         :param str attr: response string to be deserialized.
         :rtype: datetime.time
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        if re.search(r"[^\W\d_]", attr, re.I + re.U):
+        if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         return isodate.parse_time(attr)
 
     @staticmethod
     def deserialize_rfc(attr):
         """Deserialize RFC-1123 formatted string into Datetime object.
 
         :param str attr: response string to be deserialized.
         :rtype: Datetime
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            parsed_date = email.utils.parsedate_tz(attr)
+            parsed_date = email.utils.parsedate_tz(attr)  # type: ignore
             date_obj = datetime.datetime(
                 *parsed_date[:6], tzinfo=_FixedOffset(datetime.timedelta(minutes=(parsed_date[9] or 0) / 60))
             )
             if not date_obj.tzinfo:
                 date_obj = date_obj.astimezone(tz=TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to rfc datetime object."
@@ -1920,15 +1946,15 @@
         :param str attr: response string to be deserialized.
         :rtype: Datetime
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            attr = attr.upper()
+            attr = attr.upper()  # type: ignore
             match = Deserializer.valid_date.match(attr)
             if not match:
                 raise ValueError("Invalid datetime string: " + attr)
 
             check_decimal = attr.split(".")
             if len(check_decimal) > 1:
                 decimal_str = ""
@@ -1956,15 +1982,15 @@
         This is represented as seconds.
 
         :param int attr: Object to be serialized.
         :rtype: Datetime
         :raises: DeserializationError if format invalid
         """
         if isinstance(attr, ET.Element):
-            attr = int(attr.text)
+            attr = int(attr.text)  # type: ignore
         try:
             date_obj = datetime.datetime.fromtimestamp(attr, TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to unix datetime object."
             raise_with_traceback(DeserializationError, msg, err)
         else:
             return date_obj
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/_configuration.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,39 +32,36 @@
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The Azure subscription ID. This is a GUID-formatted string (e.g.
      00000000-0000-0000-0000-000000000000). Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-07-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-02-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(MicrosoftElasticConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "2022-07-01-preview")  # type: Literal["2022-07-01-preview"]
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop("api_version", "2023-02-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-elastic/{}".format(VERSION))
         self._configure(**kwargs)
 
-    def _configure(
-        self, **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+    def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
         self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/models/__init__.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,46 +20,49 @@
 from ._models_py3 import ElasticTrafficFilterRule
 from ._models_py3 import ErrorResponseBody
 from ._models_py3 import ExternalUserCreationResponse
 from ._models_py3 import ExternalUserInfo
 from ._models_py3 import FilteringTag
 from ._models_py3 import IdentityProperties
 from ._models_py3 import LogRules
+from ._models_py3 import MarketplaceSaaSInfo
+from ._models_py3 import MarketplaceSaaSInfoMarketplaceSubscription
 from ._models_py3 import MonitorProperties
 from ._models_py3 import MonitoredResource
 from ._models_py3 import MonitoredResourceListResponse
 from ._models_py3 import MonitoringTagRules
 from ._models_py3 import MonitoringTagRulesListResponse
 from ._models_py3 import MonitoringTagRulesProperties
 from ._models_py3 import OperationDisplay
 from ._models_py3 import OperationListResult
 from ._models_py3 import OperationResult
 from ._models_py3 import ResourceProviderDefaultErrorResponse
 from ._models_py3 import ResourceSku
 from ._models_py3 import SystemData
 from ._models_py3 import UpgradableVersionsList
+from ._models_py3 import UserApiKeyResponse
+from ._models_py3 import UserEmailId
 from ._models_py3 import UserInfo
 from ._models_py3 import VMCollectionUpdate
 from ._models_py3 import VMHostListResponse
 from ._models_py3 import VMIngestionDetailsResponse
 from ._models_py3 import VMResources
 
-from ._microsoft_elastic_enums import ApiVersionParameter
 from ._microsoft_elastic_enums import CreatedByType
 from ._microsoft_elastic_enums import ElasticDeploymentStatus
 from ._microsoft_elastic_enums import LiftrResourceCategories
 from ._microsoft_elastic_enums import ManagedIdentityTypes
 from ._microsoft_elastic_enums import MonitoringStatus
 from ._microsoft_elastic_enums import OperationName
 from ._microsoft_elastic_enums import ProvisioningState
 from ._microsoft_elastic_enums import SendingLogs
 from ._microsoft_elastic_enums import TagAction
 from ._microsoft_elastic_enums import Type
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "CompanyInfo",
     "DeploymentInfoResponse",
     "ElasticCloudDeployment",
     "ElasticCloudUser",
@@ -73,33 +76,36 @@
     "ElasticTrafficFilterRule",
     "ErrorResponseBody",
     "ExternalUserCreationResponse",
     "ExternalUserInfo",
     "FilteringTag",
     "IdentityProperties",
     "LogRules",
+    "MarketplaceSaaSInfo",
+    "MarketplaceSaaSInfoMarketplaceSubscription",
     "MonitorProperties",
     "MonitoredResource",
     "MonitoredResourceListResponse",
     "MonitoringTagRules",
     "MonitoringTagRulesListResponse",
     "MonitoringTagRulesProperties",
     "OperationDisplay",
     "OperationListResult",
     "OperationResult",
     "ResourceProviderDefaultErrorResponse",
     "ResourceSku",
     "SystemData",
     "UpgradableVersionsList",
+    "UserApiKeyResponse",
+    "UserEmailId",
     "UserInfo",
     "VMCollectionUpdate",
     "VMHostListResponse",
     "VMIngestionDetailsResponse",
     "VMResources",
-    "ApiVersionParameter",
     "CreatedByType",
     "ElasticDeploymentStatus",
     "LiftrResourceCategories",
     "ManagedIdentityTypes",
     "MonitoringStatus",
     "OperationName",
     "ProvisioningState",
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/models/_patch.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/models/_models_py3.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_models_py3.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 import datetime
-from typing import Dict, List, Optional, TYPE_CHECKING, Union
+from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union
 
 from .. import _serialization
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from .. import models as _models
 
@@ -30,18 +30,18 @@
     :vartype state: str
     :ivar country: Country of the company location.
     :vartype country: str
     """
 
     _validation = {
         "domain": {"max_length": 250},
-        "business": {"max_length": 50},
+        "business": {"max_length": 64},
         "employees_number": {"max_length": 20},
-        "state": {"max_length": 50},
-        "country": {"max_length": 50},
+        "state": {"max_length": 64},
+        "country": {"max_length": 64},
     }
 
     _attribute_map = {
         "domain": {"key": "domain", "type": "str"},
         "business": {"key": "business", "type": "str"},
         "employees_number": {"key": "employeesNumber", "type": "str"},
         "state": {"key": "state", "type": "str"},
@@ -52,16 +52,16 @@
         self,
         *,
         domain: Optional[str] = None,
         business: Optional[str] = None,
         employees_number: Optional[str] = None,
         state: Optional[str] = None,
         country: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword domain: Domain of the company.
         :paramtype domain: str
         :keyword business: Business of the company.
         :paramtype business: str
         :keyword employees_number: Number of employees in the company.
         :paramtype employees_number: str
@@ -87,37 +87,47 @@
     :vartype status: str or ~azure.mgmt.elastic.models.ElasticDeploymentStatus
     :ivar version: Version of the elasticsearch in Elastic cloud deployment.
     :vartype version: str
     :ivar memory_capacity: RAM capacity of the elasticsearch in Elastic cloud deployment.
     :vartype memory_capacity: str
     :ivar disk_capacity: Disk capacity of the elasticsearch in Elastic cloud deployment.
     :vartype disk_capacity: str
+    :ivar deployment_url: Deployment URL of the elasticsearch in Elastic cloud deployment.
+    :vartype deployment_url: str
+    :ivar marketplace_saas_info: Marketplace SaaS Info of the resource.
+    :vartype marketplace_saas_info: ~azure.mgmt.elastic.models.MarketplaceSaaSInfo
     """
 
     _validation = {
         "status": {"readonly": True},
         "version": {"readonly": True},
         "memory_capacity": {"readonly": True},
         "disk_capacity": {"readonly": True},
+        "deployment_url": {"readonly": True},
+        "marketplace_saas_info": {"readonly": True},
     }
 
     _attribute_map = {
         "status": {"key": "status", "type": "str"},
         "version": {"key": "version", "type": "str"},
         "memory_capacity": {"key": "memoryCapacity", "type": "str"},
         "disk_capacity": {"key": "diskCapacity", "type": "str"},
+        "deployment_url": {"key": "deploymentUrl", "type": "str"},
+        "marketplace_saas_info": {"key": "marketplaceSaasInfo", "type": "MarketplaceSaaSInfo"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.status = None
         self.version = None
         self.memory_capacity = None
         self.disk_capacity = None
+        self.deployment_url = None
+        self.marketplace_saas_info = None
 
 
 class ElasticCloudDeployment(_serialization.Model):
     """Details of the user's elastic deployment associated with the monitor resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -153,15 +163,15 @@
         "azure_subscription_id": {"key": "azureSubscriptionId", "type": "str"},
         "elasticsearch_region": {"key": "elasticsearchRegion", "type": "str"},
         "elasticsearch_service_url": {"key": "elasticsearchServiceUrl", "type": "str"},
         "kibana_service_url": {"key": "kibanaServiceUrl", "type": "str"},
         "kibana_sso_url": {"key": "kibanaSsoUrl", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.name = None
         self.deployment_id = None
         self.azure_subscription_id = None
         self.elasticsearch_region = None
         self.elasticsearch_service_url = None
@@ -191,15 +201,15 @@
 
     _attribute_map = {
         "email_address": {"key": "emailAddress", "type": "str"},
         "id": {"key": "id", "type": "str"},
         "elastic_cloud_sso_default_url": {"key": "elasticCloudSsoDefaultUrl", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.email_address = None
         self.id = None
         self.elastic_cloud_sso_default_url = None
 
 
@@ -218,52 +228,56 @@
     :vartype type: str
     :ivar sku: SKU of the monitor resource.
     :vartype sku: ~azure.mgmt.elastic.models.ResourceSku
     :ivar properties: Properties of the monitor resource.
     :vartype properties: ~azure.mgmt.elastic.models.MonitorProperties
     :ivar identity: Identity properties of the monitor resource.
     :vartype identity: ~azure.mgmt.elastic.models.IdentityProperties
+    :ivar generate_api_key: Flag to determine if User API Key has to be generated and shared.
+    :vartype generate_api_key: bool
     :ivar tags: The tags of the monitor resource.
     :vartype tags: dict[str, str]
     :ivar location: The location of the monitor resource. Required.
     :vartype location: str
     :ivar system_data: The system metadata relating to this resource.
     :vartype system_data: ~azure.mgmt.elastic.models.SystemData
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
+        "generate_api_key": {"readonly": True},
         "location": {"required": True},
         "system_data": {"readonly": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "sku": {"key": "sku", "type": "ResourceSku"},
         "properties": {"key": "properties", "type": "MonitorProperties"},
         "identity": {"key": "identity", "type": "IdentityProperties"},
+        "generate_api_key": {"key": "generateApiKey", "type": "bool"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
     def __init__(
         self,
         *,
         location: str,
         sku: Optional["_models.ResourceSku"] = None,
         properties: Optional["_models.MonitorProperties"] = None,
         identity: Optional["_models.IdentityProperties"] = None,
         tags: Optional[Dict[str, str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword sku: SKU of the monitor resource.
         :paramtype sku: ~azure.mgmt.elastic.models.ResourceSku
         :keyword properties: Properties of the monitor resource.
         :paramtype properties: ~azure.mgmt.elastic.models.MonitorProperties
         :keyword identity: Identity properties of the monitor resource.
         :paramtype identity: ~azure.mgmt.elastic.models.IdentityProperties
@@ -275,14 +289,15 @@
         super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.sku = sku
         self.properties = properties
         self.identity = identity
+        self.generate_api_key = None
         self.tags = tags
         self.location = location
         self.system_data = None
 
 
 class ElasticMonitorResourceListResponse(_serialization.Model):
     """Response of a list operation.
@@ -299,16 +314,16 @@
     }
 
     def __init__(
         self,
         *,
         value: Optional[List["_models.ElasticMonitorResource"]] = None,
         next_link: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: Results of a list operation.
         :paramtype value: list[~azure.mgmt.elastic.models.ElasticMonitorResource]
         :keyword next_link: Link to the next set of results, if any.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
@@ -323,15 +338,15 @@
     :vartype tags: dict[str, str]
     """
 
     _attribute_map = {
         "tags": {"key": "tags", "type": "{str}"},
     }
 
-    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: elastic monitor resource tags.
         :paramtype tags: dict[str, str]
         """
         super().__init__(**kwargs)
         self.tags = tags
 
@@ -343,15 +358,15 @@
     :vartype version: str
     """
 
     _attribute_map = {
         "version": {"key": "version", "type": "str"},
     }
 
-    def __init__(self, *, version: Optional[str] = None, **kwargs):
+    def __init__(self, *, version: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword version: Version to which the elastic monitor should be upgraded to.
         :paramtype version: str
         """
         super().__init__(**kwargs)
         self.version = version
 
@@ -371,16 +386,16 @@
     }
 
     def __init__(
         self,
         *,
         elastic_cloud_user: Optional["_models.ElasticCloudUser"] = None,
         elastic_cloud_deployment: Optional["_models.ElasticCloudDeployment"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword elastic_cloud_user: Details of the user's elastic account.
         :paramtype elastic_cloud_user: ~azure.mgmt.elastic.models.ElasticCloudUser
         :keyword elastic_cloud_deployment: Details of the elastic cloud deployment.
         :paramtype elastic_cloud_deployment: ~azure.mgmt.elastic.models.ElasticCloudDeployment
         """
         super().__init__(**kwargs)
@@ -423,16 +438,16 @@
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         name: Optional[str] = None,
         description: Optional[str] = None,
         region: Optional[str] = None,
         type: Optional[Union[str, "_models.Type"]] = None,
         include_by_default: Optional[bool] = None,
         rules: Optional[List["_models.ElasticTrafficFilterRule"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword id: Id of the elastic filter.
         :paramtype id: str
         :keyword name: Name of the elastic filter.
         :paramtype name: str
         :keyword description: Description of the elastic filter.
         :paramtype description: str
@@ -462,15 +477,15 @@
     :vartype rulesets: list[~azure.mgmt.elastic.models.ElasticTrafficFilter]
     """
 
     _attribute_map = {
         "rulesets": {"key": "rulesets", "type": "[ElasticTrafficFilter]"},
     }
 
-    def __init__(self, *, rulesets: Optional[List["_models.ElasticTrafficFilter"]] = None, **kwargs):
+    def __init__(self, *, rulesets: Optional[List["_models.ElasticTrafficFilter"]] = None, **kwargs: Any) -> None:
         """
         :keyword rulesets: List of elastic traffic filters in the account.
         :paramtype rulesets: list[~azure.mgmt.elastic.models.ElasticTrafficFilter]
         """
         super().__init__(**kwargs)
         self.rulesets = rulesets
 
@@ -502,16 +517,16 @@
         self,
         *,
         source: Optional[str] = None,
         description: Optional[str] = None,
         azure_endpoint_guid: Optional[str] = None,
         azure_endpoint_name: Optional[str] = None,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword source: IP of the elastic filter rule.
         :paramtype source: str
         :keyword description: Description of the elastic filter rule.
         :paramtype description: str
         :keyword azure_endpoint_guid: Guid of Private Endpoint in the elastic filter rule.
         :paramtype azure_endpoint_guid: str
@@ -551,16 +566,16 @@
     def __init__(
         self,
         *,
         code: Optional[str] = None,
         message: Optional[str] = None,
         target: Optional[str] = None,
         details: Optional[List["_models.ErrorResponseBody"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword code: Error code.
         :paramtype code: str
         :keyword message: Error message.
         :paramtype message: str
         :keyword target: Error target.
         :paramtype target: str
@@ -587,15 +602,15 @@
         "created": {"readonly": True},
     }
 
     _attribute_map = {
         "created": {"key": "created", "type": "bool"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.created = None
 
 
 class ExternalUserInfo(_serialization.Model):
     """The properties of the request required for creating user on elastic side.
@@ -624,16 +639,16 @@
         self,
         *,
         user_name: Optional[str] = None,
         full_name: Optional[str] = None,
         password: Optional[str] = None,
         email_id: Optional[str] = None,
         roles: Optional[List[str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword user_name: Username of the user to be created or updated.
         :paramtype user_name: str
         :keyword full_name: Full name of the user to be created or updated.
         :paramtype full_name: str
         :keyword password: Password of the user to be created or updated.
         :paramtype password: str
@@ -647,15 +662,16 @@
         self.full_name = full_name
         self.password = password
         self.email_id = email_id
         self.roles = roles
 
 
 class FilteringTag(_serialization.Model):
-    """The definition of a filtering tag. Filtering tags are used for capturing resources and include/exclude them from being monitored.
+    """The definition of a filtering tag. Filtering tags are used for capturing resources and
+    include/exclude them from being monitored.
 
     :ivar name: The name (also known as the key) of the tag.
     :vartype name: str
     :ivar value: The value of the tag.
     :vartype value: str
     :ivar action: Valid actions for a filtering tag. Known values are: "Include" and "Exclude".
     :vartype action: str or ~azure.mgmt.elastic.models.TagAction
@@ -669,16 +685,16 @@
 
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         value: Optional[str] = None,
         action: Optional[Union[str, "_models.TagAction"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: The name (also known as the key) of the tag.
         :paramtype name: str
         :keyword value: The value of the tag.
         :paramtype value: str
         :keyword action: Valid actions for a filtering tag. Known values are: "Include" and "Exclude".
         :paramtype action: str or ~azure.mgmt.elastic.models.TagAction
@@ -709,15 +725,15 @@
 
     _attribute_map = {
         "principal_id": {"key": "principalId", "type": "str"},
         "tenant_id": {"key": "tenantId", "type": "str"},
         "type": {"key": "type", "type": "str"},
     }
 
-    def __init__(self, *, type: Optional[Union[str, "_models.ManagedIdentityTypes"]] = None, **kwargs):
+    def __init__(self, *, type: Optional[Union[str, "_models.ManagedIdentityTypes"]] = None, **kwargs: Any) -> None:
         """
         :keyword type: Managed identity type. "SystemAssigned"
         :paramtype type: str or ~azure.mgmt.elastic.models.ManagedIdentityTypes
         """
         super().__init__(**kwargs)
         self.principal_id = None
         self.tenant_id = None
@@ -752,16 +768,16 @@
     def __init__(
         self,
         *,
         send_aad_logs: Optional[bool] = None,
         send_subscription_logs: Optional[bool] = None,
         send_activity_logs: Optional[bool] = None,
         filtering_tags: Optional[List["_models.FilteringTag"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword send_aad_logs: Flag specifying if AAD logs should be sent for the Monitor resource.
         :paramtype send_aad_logs: bool
         :keyword send_subscription_logs: Flag specifying if subscription logs should be sent for the
          Monitor resource.
         :paramtype send_subscription_logs: bool
         :keyword send_activity_logs: Flag specifying if activity logs from Azure resources should be
@@ -776,14 +792,78 @@
         super().__init__(**kwargs)
         self.send_aad_logs = send_aad_logs
         self.send_subscription_logs = send_subscription_logs
         self.send_activity_logs = send_activity_logs
         self.filtering_tags = filtering_tags
 
 
+class MarketplaceSaaSInfo(_serialization.Model):
+    """Marketplace SAAS Info of the resource.
+
+    :ivar marketplace_subscription: Marketplace Subscription Id.
+    :vartype marketplace_subscription:
+     ~azure.mgmt.elastic.models.MarketplaceSaaSInfoMarketplaceSubscription
+    :ivar marketplace_name: Subscription Details: Marketplace SAAS Name.
+    :vartype marketplace_name: str
+    :ivar marketplace_resource_id: Subscription Details: Marketplace Resource URI.
+    :vartype marketplace_resource_id: str
+    """
+
+    _attribute_map = {
+        "marketplace_subscription": {
+            "key": "marketplaceSubscription",
+            "type": "MarketplaceSaaSInfoMarketplaceSubscription",
+        },
+        "marketplace_name": {"key": "marketplaceName", "type": "str"},
+        "marketplace_resource_id": {"key": "marketplaceResourceId", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        marketplace_subscription: Optional["_models.MarketplaceSaaSInfoMarketplaceSubscription"] = None,
+        marketplace_name: Optional[str] = None,
+        marketplace_resource_id: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword marketplace_subscription: Marketplace Subscription Id.
+        :paramtype marketplace_subscription:
+         ~azure.mgmt.elastic.models.MarketplaceSaaSInfoMarketplaceSubscription
+        :keyword marketplace_name: Subscription Details: Marketplace SAAS Name.
+        :paramtype marketplace_name: str
+        :keyword marketplace_resource_id: Subscription Details: Marketplace Resource URI.
+        :paramtype marketplace_resource_id: str
+        """
+        super().__init__(**kwargs)
+        self.marketplace_subscription = marketplace_subscription
+        self.marketplace_name = marketplace_name
+        self.marketplace_resource_id = marketplace_resource_id
+
+
+class MarketplaceSaaSInfoMarketplaceSubscription(_serialization.Model):
+    """Marketplace Subscription Id.
+
+    :ivar id: Marketplace Subscription Id. This is a GUID-formatted string.
+    :vartype id: str
+    """
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+    }
+
+    def __init__(self, *, id: Optional[str] = None, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
+        """
+        :keyword id: Marketplace Subscription Id. This is a GUID-formatted string.
+        :paramtype id: str
+        """
+        super().__init__(**kwargs)
+        self.id = id
+
+
 class MonitoredResource(_serialization.Model):
     """The properties of a resource currently being monitored by the Elastic monitor resource.
 
     :ivar id: The ARM id of the resource.
     :vartype id: str
     :ivar sending_logs: Flag indicating the status of the resource for sending logs operation to
      Elastic. Known values are: "True" and "False".
@@ -801,16 +881,16 @@
 
     def __init__(
         self,
         *,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         sending_logs: Optional[Union[str, "_models.SendingLogs"]] = None,
         reason_for_logs_status: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword id: The ARM id of the resource.
         :paramtype id: str
         :keyword sending_logs: Flag indicating the status of the resource for sending logs operation to
          Elastic. Known values are: "True" and "False".
         :paramtype sending_logs: str or ~azure.mgmt.elastic.models.SendingLogs
         :keyword reason_for_logs_status: Reason for why the resource is sending logs (or why it is not
@@ -834,16 +914,20 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[MonitoredResource]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.MonitoredResource"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        value: Optional[List["_models.MonitoredResource"]] = None,
+        next_link: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: Results of a list operation.
         :paramtype value: list[~azure.mgmt.elastic.models.MonitoredResource]
         :keyword next_link: Link to the next set of results, if any.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
@@ -879,15 +963,15 @@
         "name": {"key": "name", "type": "str"},
         "id": {"key": "id", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "properties": {"key": "properties", "type": "MonitoringTagRulesProperties"},
         "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(self, *, properties: Optional["_models.MonitoringTagRulesProperties"] = None, **kwargs):
+    def __init__(self, *, properties: Optional["_models.MonitoringTagRulesProperties"] = None, **kwargs: Any) -> None:
         """
         :keyword properties: Properties of the monitoring tag rules.
         :paramtype properties: ~azure.mgmt.elastic.models.MonitoringTagRulesProperties
         """
         super().__init__(**kwargs)
         self.name = None
         self.id = None
@@ -907,16 +991,20 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[MonitoringTagRules]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.MonitoringTagRules"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        value: Optional[List["_models.MonitoringTagRules"]] = None,
+        next_link: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: Results of a list operation.
         :paramtype value: list[~azure.mgmt.elastic.models.MonitoringTagRules]
         :keyword next_link: Link to the next set of results, if any.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
@@ -941,16 +1029,16 @@
     }
 
     def __init__(
         self,
         *,
         provisioning_state: Optional[Union[str, "_models.ProvisioningState"]] = None,
         log_rules: Optional["_models.LogRules"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword provisioning_state: Provisioning state of the monitoring tag rules. Known values are:
          "Accepted", "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted",
          and "NotSpecified".
         :paramtype provisioning_state: str or ~azure.mgmt.elastic.models.ProvisioningState
         :keyword log_rules: Rules for sending logs.
         :paramtype log_rules: ~azure.mgmt.elastic.models.LogRules
@@ -1003,16 +1091,16 @@
         self,
         *,
         provisioning_state: Optional[Union[str, "_models.ProvisioningState"]] = None,
         monitoring_status: Optional[Union[str, "_models.MonitoringStatus"]] = None,
         elastic_properties: Optional["_models.ElasticProperties"] = None,
         user_info: Optional["_models.UserInfo"] = None,
         version: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword provisioning_state: Provisioning state of the monitor resource. Known values are:
          "Accepted", "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Canceled", "Deleted",
          and "NotSpecified".
         :paramtype provisioning_state: str or ~azure.mgmt.elastic.models.ProvisioningState
         :keyword monitoring_status: Flag specifying if the resource monitoring is enabled or disabled.
          Known values are: "Enabled" and "Disabled".
@@ -1057,16 +1145,16 @@
     def __init__(
         self,
         *,
         provider: Optional[str] = None,
         resource: Optional[str] = None,
         operation: Optional[str] = None,
         description: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword provider: Service provider, i.e., Microsoft.Elastic.
         :paramtype provider: str
         :keyword resource: Type on which the operation is performed, e.g., 'monitors'.
         :paramtype resource: str
         :keyword operation: Operation type, e.g., read, write, delete, etc.
         :paramtype operation: str
@@ -1091,16 +1179,16 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[OperationResult]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.OperationResult"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self, *, value: Optional[List["_models.OperationResult"]] = None, next_link: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword value: List of operations supported by the Microsoft.Elastic provider.
         :paramtype value: list[~azure.mgmt.elastic.models.OperationResult]
         :keyword next_link: URL to get the next set of operation list results if there are any.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
@@ -1131,16 +1219,16 @@
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         is_data_action: Optional[bool] = None,
         display: Optional["_models.OperationDisplay"] = None,
         origin: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Operation name, i.e., {provider}/{resource}/{operation}.
         :paramtype name: str
         :keyword is_data_action: Indicates whether the operation is a data action.
         :paramtype is_data_action: bool
         :keyword display: The object that represents the operation.
         :paramtype display: ~azure.mgmt.elastic.models.OperationDisplay
@@ -1167,15 +1255,15 @@
         "error": {"readonly": True},
     }
 
     _attribute_map = {
         "error": {"key": "error", "type": "ErrorResponseBody"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.error = None
 
 
 class ResourceSku(_serialization.Model):
     """Microsoft.Elastic SKU.
@@ -1190,15 +1278,15 @@
         "name": {"required": True},
     }
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
     }
 
-    def __init__(self, *, name: str, **kwargs):
+    def __init__(self, *, name: str, **kwargs: Any) -> None:
         """
         :keyword name: Name of the SKU. Required.
         :paramtype name: str
         """
         super().__init__(**kwargs)
         self.name = name
 
@@ -1236,16 +1324,16 @@
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
         :paramtype created_by_type: str or ~azure.mgmt.elastic.models.CreatedByType
         :keyword created_at: The timestamp of resource creation (UTC).
@@ -1278,27 +1366,70 @@
 
     _attribute_map = {
         "current_version": {"key": "currentVersion", "type": "str"},
         "upgradable_versions": {"key": "upgradableVersions", "type": "[str]"},
     }
 
     def __init__(
-        self, *, current_version: Optional[str] = None, upgradable_versions: Optional[List[str]] = None, **kwargs
-    ):
+        self, *, current_version: Optional[str] = None, upgradable_versions: Optional[List[str]] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword current_version: Current version of the elastic monitor.
         :paramtype current_version: str
         :keyword upgradable_versions: Stack Versions that this version can upgrade to.
         :paramtype upgradable_versions: list[str]
         """
         super().__init__(**kwargs)
         self.current_version = current_version
         self.upgradable_versions = upgradable_versions
 
 
+class UserApiKeyResponse(_serialization.Model):
+    """The User Api Key created for the Organization associated with the User Email Id that was passed
+    in the request.
+
+    :ivar api_key: The User Api Key Generated based on ReturnApiKey flag. This is applicable for
+     non-Portal clients only.
+    :vartype api_key: str
+    """
+
+    _attribute_map = {
+        "api_key": {"key": "apiKey", "type": "str"},
+    }
+
+    def __init__(self, *, api_key: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword api_key: The User Api Key Generated based on ReturnApiKey flag. This is applicable for
+         non-Portal clients only.
+        :paramtype api_key: str
+        """
+        super().__init__(**kwargs)
+        self.api_key = api_key
+
+
+class UserEmailId(_serialization.Model):
+    """Email Id of the User Organization, of which the API Key must be returned.
+
+    :ivar email_id: The User email Id.
+    :vartype email_id: str
+    """
+
+    _attribute_map = {
+        "email_id": {"key": "emailId", "type": "str"},
+    }
+
+    def __init__(self, *, email_id: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword email_id: The User email Id.
+        :paramtype email_id: str
+        """
+        super().__init__(**kwargs)
+        self.email_id = email_id
+
+
 class UserInfo(_serialization.Model):
     """User Information to be passed to partners.
 
     :ivar first_name: First name of the user.
     :vartype first_name: str
     :ivar last_name: Last name of the user.
     :vartype last_name: str
@@ -1309,15 +1440,15 @@
     :ivar company_info: Company information of the user to be passed to partners.
     :vartype company_info: ~azure.mgmt.elastic.models.CompanyInfo
     """
 
     _validation = {
         "first_name": {"max_length": 50},
         "last_name": {"max_length": 50},
-        "company_name": {"max_length": 50},
+        "company_name": {"max_length": 64},
         "email_address": {
             "pattern": r'^([^<>()\[\]\.,;:\s@"]+(\.[^<>()\[\]\.,;:\s@"]+)*)@(([a-zA-Z-_0-9]+\.)+[a-zA-Z]{2,})$'
         },
     }
 
     _attribute_map = {
         "first_name": {"key": "firstName", "type": "str"},
@@ -1331,16 +1462,16 @@
         self,
         *,
         first_name: Optional[str] = None,
         last_name: Optional[str] = None,
         company_name: Optional[str] = None,
         email_address: Optional[str] = None,
         company_info: Optional["_models.CompanyInfo"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword first_name: First name of the user.
         :paramtype first_name: str
         :keyword last_name: Last name of the user.
         :paramtype last_name: str
         :keyword company_name: Company name of the user.
         :paramtype company_name: str
@@ -1373,16 +1504,16 @@
     }
 
     def __init__(
         self,
         *,
         vm_resource_id: Optional[str] = None,
         operation_name: Optional[Union[str, "_models.OperationName"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword vm_resource_id: ARM id of the VM resource.
         :paramtype vm_resource_id: str
         :keyword operation_name: Operation to be performed for given VM. Known values are: "Add" and
          "Delete".
         :paramtype operation_name: str or ~azure.mgmt.elastic.models.OperationName
         """
@@ -1402,16 +1533,16 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[VMResources]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.VMResources"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self, *, value: Optional[List["_models.VMResources"]] = None, next_link: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword value: Results of a list operation.
         :paramtype value: list[~azure.mgmt.elastic.models.VMResources]
         :keyword next_link: Link to the next Vm resource Id, if any.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
@@ -1429,15 +1560,15 @@
     """
 
     _attribute_map = {
         "cloud_id": {"key": "cloudId", "type": "str"},
         "ingestion_key": {"key": "ingestionKey", "type": "str"},
     }
 
-    def __init__(self, *, cloud_id: Optional[str] = None, ingestion_key: Optional[str] = None, **kwargs):
+    def __init__(self, *, cloud_id: Optional[str] = None, ingestion_key: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword cloud_id: The cloudId of given Elastic monitor resource.
         :paramtype cloud_id: str
         :keyword ingestion_key: Ingestion details to install agent on given VM.
         :paramtype ingestion_key: str
         """
         super().__init__(**kwargs)
@@ -1452,14 +1583,14 @@
     :vartype vm_resource_id: str
     """
 
     _attribute_map = {
         "vm_resource_id": {"key": "vmResourceId", "type": "str"},
     }
 
-    def __init__(self, *, vm_resource_id: Optional[str] = None, **kwargs):
+    def __init__(self, *, vm_resource_id: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword vm_resource_id: The ARM id of the VM resource.
         :paramtype vm_resource_id: str
         """
         super().__init__(**kwargs)
         self.vm_resource_id = vm_resource_id
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/models/_microsoft_elastic_enums.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_microsoft_elastic_enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,14 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
 
 
-class ApiVersionParameter(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """ApiVersionParameter."""
-
-    TWO_THOUSAND_TWENTY07_01_PREVIEW = "2020-07-01-preview"
-    TWO_THOUSAND_TWENTY07_01 = "2020-07-01"
-    TWO_THOUSAND_TWENTY_ONE09_01_PREVIEW = "2021-09-01-preview"
-    TWO_THOUSAND_TWENTY_ONE10_01_PREVIEW = "2021-10-01-preview"
-    TWO_THOUSAND_TWENTY_TWO05_05_PREVIEW = "2022-05-05-preview"
-
-
 class CreatedByType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The type of identity that created the resource."""
 
     USER = "User"
     APPLICATION = "Application"
     MANAGED_IDENTITY = "ManagedIdentity"
     KEY = "Key"
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_monitored_resources_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitored_resources_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,31 +41,31 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listMonitoredResources",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -106,18 +106,18 @@
         :return: An iterator like instance of either MonitoredResource or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elastic.models.MonitoredResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.MonitoredResourceListResponse]
+        )
+        cls: ClsType[_models.MonitoredResourceListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -132,15 +132,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -148,38 +148,41 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("MonitoredResourceListResponse", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(
                     _models.ResourceProviderDefaultErrorResponse, pipeline_response
                 )
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listMonitoredResources"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listMonitoredResources"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_vm_ingestion_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_ingestion_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,31 +41,31 @@
 
 def build_details_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/vmIngestionDetails",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -114,33 +114,34 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VMIngestionDetailsResponse]
+        )
+        cls: ClsType[_models.VMIngestionDetailsResponse] = kwargs.pop("cls", None)
 
         request = build_details_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.details.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -151,8 +152,10 @@
         deserialized = self._deserialize("VMIngestionDetailsResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    details.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/vmIngestionDetails"}  # type: ignore
+    details.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/vmIngestionDetails"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_create_and_associate_ip_filter_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_create_and_associate_ip_filter_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,31 +49,31 @@
     ips: Optional[str] = None,
     name: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociateIPFilter",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
     if ips is not None:
         _params["ips"] = _SERIALIZER.query("ips", ips, "str")
     if name is not None:
         _params["name"] = _SERIALIZER.query("name", name, "str")
@@ -118,50 +118,53 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ips=ips,
             name=name,
             api_version=api_version,
             template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [201]:
+        if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _create_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociateIPFilter"}  # type: ignore
+    _create_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociateIPFilter"
+    }
 
     @distributed_trace
     def begin_create(
         self,
         resource_group_name: str,
         monitor_name: str,
         ips: Optional[str] = None,
@@ -192,21 +195,21 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 ips=ips,
                 name=name,
                 api_version=api_version,
@@ -218,22 +221,26 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_create.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociateIPFilter"}  # type: ignore
+    begin_create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociateIPFilter"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_traffic_filters_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_detach_and_delete_traffic_filter_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,51 +46,51 @@
     *,
     ruleset_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/deleteTrafficFilter",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachAndDeleteTrafficFilter",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
     if ruleset_id is not None:
         _params["rulesetId"] = _SERIALIZER.query("ruleset_id", ruleset_id, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class TrafficFiltersOperations:
+class DetachAndDeleteTrafficFilterOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.MicrosoftElastic`'s
-        :attr:`traffic_filters` attribute.
+        :attr:`detach_and_delete_traffic_filter` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
@@ -98,17 +98,17 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def delete(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, monitor_name: str, ruleset_id: Optional[str] = None, **kwargs: Any
     ) -> None:
-        """Delete traffic filter from the account.
+        """Detach and Delete traffic filter from the given deployment.
 
-        Delete traffic filter from the account.
+        Detach and Delete traffic filter from the given deployment.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :param ruleset_id: Ruleset Id of the filter. Default value is None.
@@ -125,42 +125,45 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ruleset_id=ruleset_id,
             api_version=api_version,
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/deleteTrafficFilter"}  # type: ignore
+    delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachAndDeleteTrafficFilter"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_detach_and_delete_traffic_filter_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_all_traffic_filters_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,132 +35,125 @@
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_delete_request(
-    resource_group_name: str,
-    monitor_name: str,
-    subscription_id: str,
-    *,
-    ruleset_id: Optional[str] = None,
-    **kwargs: Any
-) -> HttpRequest:
+def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachAndDeleteTrafficFilter",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAllTrafficFilters",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-    if ruleset_id is not None:
-        _params["rulesetId"] = _SERIALIZER.query("ruleset_id", ruleset_id, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class DetachAndDeleteTrafficFilterOperations:
+class AllTrafficFiltersOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.MicrosoftElastic`'s
-        :attr:`detach_and_delete_traffic_filter` attribute.
+        :attr:`all_traffic_filters` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def delete(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, monitor_name: str, ruleset_id: Optional[str] = None, **kwargs: Any
-    ) -> None:
-        """Detach and Delete traffic filter from the given deployment.
+    def list(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> _models.ElasticTrafficFilterResponse:
+        """Get the list of all traffic filters for the account.
 
-        Detach and Delete traffic filter from the given deployment.
+        Get the list of all traffic filters for the account.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
-        :param ruleset_id: Ruleset Id of the filter. Default value is None.
-        :type ruleset_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None or the result of cls(response)
-        :rtype: None
+        :return: ElasticTrafficFilterResponse or the result of cls(response)
+        :rtype: ~azure.mgmt.elastic.models.ElasticTrafficFilterResponse
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
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[_models.ElasticTrafficFilterResponse] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        request = build_list_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
-            ruleset_id=ruleset_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
+            template_url=self.list.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        deserialized = self._deserialize("ElasticTrafficFilterResponse", pipeline_response)
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, deserialized, {})
 
-    delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachAndDeleteTrafficFilter"}  # type: ignore
+        return deserialized
+
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAllTrafficFilters"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/__init__.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 from ._list_associated_traffic_filters_operations import ListAssociatedTrafficFiltersOperations
 from ._create_and_associate_ip_filter_operations import CreateAndAssociateIPFilterOperations
 from ._create_and_associate_pl_filter_operations import CreateAndAssociatePLFilterOperations
 from ._associate_traffic_filter_operations import AssociateTrafficFilterOperations
 from ._detach_and_delete_traffic_filter_operations import DetachAndDeleteTrafficFilterOperations
 from ._detach_traffic_filter_operations import DetachTrafficFilterOperations
 from ._traffic_filters_operations import TrafficFiltersOperations
+from ._organizations_operations import OrganizationsOperations
 
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Operations",
     "MonitorsOperations",
     "MonitoredResourcesOperations",
     "DeploymentInfoOperations",
@@ -46,10 +47,11 @@
     "ListAssociatedTrafficFiltersOperations",
     "CreateAndAssociateIPFilterOperations",
     "CreateAndAssociatePLFilterOperations",
     "AssociateTrafficFilterOperations",
     "DetachAndDeleteTrafficFilterOperations",
     "DetachTrafficFilterOperations",
     "TrafficFiltersOperations",
+    "OrganizationsOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_all_traffic_filters_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_list_associated_traffic_filters_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,65 +39,65 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAllTrafficFilters",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAssociatedTrafficFilters",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class AllTrafficFiltersOperations:
+class ListAssociatedTrafficFiltersOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.MicrosoftElastic`'s
-        :attr:`all_traffic_filters` attribute.
+        :attr:`list_associated_traffic_filters` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> _models.ElasticTrafficFilterResponse:
-        """Get the list of all traffic filters for the account.
+        """Get the list of all associated traffic filters for the given deployment.
 
-        Get the list of all traffic filters for the account.
+        Get the list of all associated traffic filters for the given deployment.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -112,33 +112,34 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticTrafficFilterResponse]
+        )
+        cls: ClsType[_models.ElasticTrafficFilterResponse] = kwargs.pop("cls", None)
 
         request = build_list_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -149,8 +150,10 @@
         deserialized = self._deserialize("ElasticTrafficFilterResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAllTrafficFilters"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAssociatedTrafficFilters"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_patch.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_create_and_associate_pl_filter_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_create_and_associate_pl_filter_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,31 +50,31 @@
     private_endpoint_guid: Optional[str] = None,
     private_endpoint_name: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociatePLFilter",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
     if name is not None:
         _params["name"] = _SERIALIZER.query("name", name, "str")
     if private_endpoint_guid is not None:
         _params["privateEndpointGuid"] = _SERIALIZER.query("private_endpoint_guid", private_endpoint_guid, "str")
@@ -122,51 +122,54 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             name=name,
             private_endpoint_guid=private_endpoint_guid,
             private_endpoint_name=private_endpoint_name,
             api_version=api_version,
             template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [201]:
+        if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _create_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociatePLFilter"}  # type: ignore
+    _create_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociatePLFilter"
+    }
 
     @distributed_trace
     def begin_create(
         self,
         resource_group_name: str,
         monitor_name: str,
         name: Optional[str] = None,
@@ -200,21 +203,21 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 name=name,
                 private_endpoint_guid=private_endpoint_guid,
                 private_endpoint_name=private_endpoint_name,
@@ -227,22 +230,26 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_create.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociatePLFilter"}  # type: ignore
+    begin_create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociatePLFilter"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_vm_collection_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_collection_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,32 +41,32 @@
 
 def build_update_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/vmCollectionUpdate",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -167,15 +167,16 @@
         Update the vm details that will be monitored by the Elastic monitor resource.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
-        :param body: VM resource Id. Is either a model type or a IO type. Default value is None.
+        :param body: VM resource Id. Is either a VMCollectionUpdate type or a IO type. Default value is
+         None.
         :type body: ~azure.mgmt.elastic.models.VMCollectionUpdate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
@@ -188,19 +189,19 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
@@ -218,26 +219,29 @@
             json=_json,
             content=_content,
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/vmCollectionUpdate"}  # type: ignore
+    update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/vmCollectionUpdate"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_associate_traffic_filter_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_associate_traffic_filter_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,31 +48,31 @@
     *,
     ruleset_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/associateTrafficFilter",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
     if ruleset_id is not None:
         _params["rulesetId"] = _SERIALIZER.query("ruleset_id", ruleset_id, "str")
 
     # Construct headers
@@ -110,49 +110,52 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_associate_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ruleset_id=ruleset_id,
             api_version=api_version,
             template_url=self._associate_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _associate_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/associateTrafficFilter"}  # type: ignore
+    _associate_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/associateTrafficFilter"
+    }
 
     @distributed_trace
     def begin_associate(
         self, resource_group_name: str, monitor_name: str, ruleset_id: Optional[str] = None, **kwargs: Any
     ) -> LROPoller[None]:
         """Associate traffic filter for the given deployment.
 
@@ -176,21 +179,21 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._associate_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 ruleset_id=ruleset_id,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
@@ -201,22 +204,26 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_associate.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/associateTrafficFilter"}  # type: ignore
+    begin_associate.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/associateTrafficFilter"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_vm_host_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_vm_host_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,31 +41,31 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listVMHost",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -106,18 +106,18 @@
         :return: An iterator like instance of either VMResources or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elastic.models.VMResources]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VMHostListResponse]
+        )
+        cls: ClsType[_models.VMHostListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -132,15 +132,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -148,38 +148,41 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("VMHostListResponse", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(
                     _models.ResourceProviderDefaultErrorResponse, pipeline_response
                 )
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listVMHost"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listVMHost"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_monitors_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitors_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,87 +43,87 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Elastic/monitors")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -132,32 +132,32 @@
 
 def build_create_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -168,32 +168,32 @@
 
 def build_update_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -204,31 +204,31 @@
 
 def build_delete_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -265,18 +265,18 @@
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elastic.models.ElasticMonitorResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticMonitorResourceListResponse]
+        )
+        cls: ClsType[_models.ElasticMonitorResourceListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -289,15 +289,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -305,45 +305,46 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ElasticMonitorResourceListResponse", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(
                     _models.ResourceProviderDefaultErrorResponse, pipeline_response
                 )
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Elastic/monitors"}  # type: ignore
+    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Elastic/monitors"}
 
     @distributed_trace
     def list_by_resource_group(
         self, resource_group_name: str, **kwargs: Any
     ) -> Iterable["_models.ElasticMonitorResource"]:
         """List all monitors under the specified resource group.
 
@@ -357,18 +358,18 @@
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elastic.models.ElasticMonitorResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticMonitorResourceListResponse]
+        )
+        cls: ClsType[_models.ElasticMonitorResourceListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -382,15 +383,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list_by_resource_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -398,45 +399,48 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ElasticMonitorResourceListResponse", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(
                     _models.ResourceProviderDefaultErrorResponse, pipeline_response
                 )
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors"}  # type: ignore
+    list_by_resource_group.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors"
+    }
 
     @distributed_trace
     def get(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> _models.ElasticMonitorResource:
         """Get the properties of a specific monitor resource.
 
         Get the properties of a specific monitor resource.
 
@@ -457,33 +461,34 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticMonitorResource]
+        )
+        cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -494,15 +499,17 @@
         deserialized = self._deserialize("ElasticMonitorResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"
+    }
 
     def _create_initial(
         self,
         resource_group_name: str,
         monitor_name: str,
         body: Optional[Union[_models.ElasticMonitorResource, IO]] = None,
         **kwargs: Any
@@ -514,19 +521,19 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticMonitorResource]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
@@ -544,18 +551,19 @@
             json=_json,
             content=_content,
             template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -566,19 +574,21 @@
         if response.status_code == 200:
             deserialized = self._deserialize("ElasticMonitorResource", pipeline_response)
 
         if response.status_code == 201:
             deserialized = self._deserialize("ElasticMonitorResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _create_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"}  # type: ignore
+    _create_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"
+    }
 
     @overload
     def begin_create(
         self,
         resource_group_name: str,
         monitor_name: str,
         body: Optional[_models.ElasticMonitorResource] = None,
@@ -665,16 +675,16 @@
         Create a monitor resource.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
-        :param body: Elastic monitor resource model. Is either a model type or a IO type. Default value
-         is None.
+        :param body: Elastic monitor resource model. Is either a ElasticMonitorResource type or a IO
+         type. Default value is None.
         :type body: ~azure.mgmt.elastic.models.ElasticMonitorResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -687,24 +697,24 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.elastic.models.ElasticMonitorResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticMonitorResource]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._create_initial(  # type: ignore
+            raw_result = self._create_initial(
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 body=body,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -716,31 +726,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ElasticMonitorResource", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(
+            polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
-            )  # type: PollingMethod
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_create.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"}  # type: ignore
+    begin_create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"
+    }
 
     @overload
     def update(
         self,
         resource_group_name: str,
         monitor_name: str,
         body: Optional[_models.ElasticMonitorResourceUpdateParameters] = None,
@@ -811,16 +823,16 @@
         Update a monitor resource.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
-        :param body: Elastic resource model update parameters. Is either a model type or a IO type.
-         Default value is None.
+        :param body: Elastic resource model update parameters. Is either a
+         ElasticMonitorResourceUpdateParameters type or a IO type. Default value is None.
         :type body: ~azure.mgmt.elastic.models.ElasticMonitorResourceUpdateParameters or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ElasticMonitorResource or the result of cls(response)
         :rtype: ~azure.mgmt.elastic.models.ElasticMonitorResource
@@ -833,19 +845,19 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticMonitorResource]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
@@ -863,18 +875,19 @@
             json=_json,
             content=_content,
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -885,15 +898,17 @@
         deserialized = self._deserialize("ElasticMonitorResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"}  # type: ignore
+    update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"
+    }
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, monitor_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -901,48 +916,51 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"
+    }
 
     @distributed_trace
     def begin_delete(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> LROPoller[None]:
         """Delete a monitor resource.
 
         Delete a monitor resource.
 
@@ -962,21 +980,21 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -986,22 +1004,24 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_external_user_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_external_user_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,32 +41,32 @@
 
 def build_create_or_update_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createOrUpdateExternalUser",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -173,16 +173,16 @@
         elastic deployment.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
-        :param body: Elastic External User Creation Parameters. Is either a model type or a IO type.
-         Default value is None.
+        :param body: Elastic External User Creation Parameters. Is either a ExternalUserInfo type or a
+         IO type. Default value is None.
         :type body: ~azure.mgmt.elastic.models.ExternalUserInfo or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ExternalUserCreationResponse or the result of cls(response)
         :rtype: ~azure.mgmt.elastic.models.ExternalUserCreationResponse
@@ -195,19 +195,19 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ExternalUserCreationResponse]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ExternalUserCreationResponse] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
@@ -225,18 +225,19 @@
             json=_json,
             content=_content,
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -247,8 +248,10 @@
         deserialized = self._deserialize("ExternalUserCreationResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createOrUpdateExternalUser"}  # type: ignore
+    create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createOrUpdateExternalUser"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_deployment_info_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_deployment_info_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,31 +39,31 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listDeploymentInfo",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -114,33 +114,34 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.DeploymentInfoResponse]
+        )
+        cls: ClsType[_models.DeploymentInfoResponse] = kwargs.pop("cls", None)
 
         request = build_list_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -151,8 +152,10 @@
         deserialized = self._deserialize("DeploymentInfoResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listDeploymentInfo"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listDeploymentInfo"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_tag_rules_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_tag_rules_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,31 +43,31 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -76,33 +76,33 @@
 
 def build_create_or_update_request(
     resource_group_name: str, monitor_name: str, rule_set_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
         "ruleSetName": _SERIALIZER.url("rule_set_name", rule_set_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -113,32 +113,32 @@
 
 def build_get_request(
     resource_group_name: str, monitor_name: str, rule_set_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
         "ruleSetName": _SERIALIZER.url("rule_set_name", rule_set_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -147,32 +147,32 @@
 
 def build_delete_request(
     resource_group_name: str, monitor_name: str, rule_set_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
         "ruleSetName": _SERIALIZER.url("rule_set_name", rule_set_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -215,18 +215,18 @@
         :return: An iterator like instance of either MonitoringTagRules or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elastic.models.MonitoringTagRules]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.MonitoringTagRulesListResponse]
+        )
+        cls: ClsType[_models.MonitoringTagRulesListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -241,15 +241,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -257,45 +257,48 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("MonitoringTagRulesListResponse", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(
                     _models.ResourceProviderDefaultErrorResponse, pipeline_response
                 )
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules"
+    }
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
         monitor_name: str,
         rule_set_name: str,
@@ -375,16 +378,16 @@
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :param rule_set_name: Tag Rule Set resource name. Required.
         :type rule_set_name: str
-        :param body: request body of MonitoringTagRules. Is either a model type or a IO type. Default
-         value is None.
+        :param body: request body of MonitoringTagRules. Is either a MonitoringTagRules type or a IO
+         type. Default value is None.
         :type body: ~azure.mgmt.elastic.models.MonitoringTagRules or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MonitoringTagRules or the result of cls(response)
         :rtype: ~azure.mgmt.elastic.models.MonitoringTagRules
@@ -397,19 +400,19 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.MonitoringTagRules]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.MonitoringTagRules] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
@@ -428,18 +431,19 @@
             json=_json,
             content=_content,
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -450,15 +454,17 @@
         deserialized = self._deserialize("MonitoringTagRules", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"}  # type: ignore
+    create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"
+    }
 
     @distributed_trace
     def get(
         self, resource_group_name: str, monitor_name: str, rule_set_name: str, **kwargs: Any
     ) -> _models.MonitoringTagRules:
         """Get a tag rule set for a given monitor resource.
 
@@ -483,34 +489,35 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.MonitoringTagRules]
+        )
+        cls: ClsType[_models.MonitoringTagRules] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             rule_set_name=rule_set_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -521,15 +528,17 @@
         deserialized = self._deserialize("MonitoringTagRules", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"
+    }
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, monitor_name: str, rule_set_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -537,49 +546,52 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             rule_set_name=rule_set_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"
+    }
 
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, monitor_name: str, rule_set_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Delete a tag rule set for a given monitor resource.
 
@@ -603,21 +615,21 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 rule_set_name=rule_set_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
@@ -628,22 +640,24 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_detach_traffic_filter_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_detach_traffic_filter_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,31 +48,31 @@
     *,
     ruleset_id: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachTrafficFilter",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
     if ruleset_id is not None:
         _params["rulesetId"] = _SERIALIZER.query("ruleset_id", ruleset_id, "str")
 
     # Construct headers
@@ -110,49 +110,52 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ruleset_id=ruleset_id,
             api_version=api_version,
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachTrafficFilter"}  # type: ignore
+    _update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachTrafficFilter"
+    }
 
     @distributed_trace
     def begin_update(
         self, resource_group_name: str, monitor_name: str, ruleset_id: Optional[str] = None, **kwargs: Any
     ) -> LROPoller[None]:
         """Detach traffic filter for the given deployment.
 
@@ -176,21 +179,21 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._update_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 ruleset_id=ruleset_id,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
@@ -201,22 +204,26 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachTrafficFilter"}  # type: ignore
+    begin_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachTrafficFilter"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_monitor_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_monitor_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,32 +43,32 @@
 
 def build_upgrade_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/upgrade",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -110,19 +110,19 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
@@ -140,33 +140,36 @@
             json=_json,
             content=_content,
             template_url=self._upgrade_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _upgrade_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/upgrade"}  # type: ignore
+    _upgrade_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/upgrade"
+    }
 
     @overload
     def begin_upgrade(
         self,
         resource_group_name: str,
         monitor_name: str,
         body: Optional[_models.ElasticMonitorUpgrade] = None,
@@ -251,16 +254,16 @@
         Upgradable version for a monitor resource.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
-        :param body: Elastic Monitor Upgrade Parameters. Is either a model type or a IO type. Default
-         value is None.
+        :param body: Elastic Monitor Upgrade Parameters. Is either a ElasticMonitorUpgrade type or a IO
+         type. Default value is None.
         :type body: ~azure.mgmt.elastic.models.ElasticMonitorUpgrade or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -272,22 +275,22 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._upgrade_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 body=body,
                 api_version=api_version,
                 content_type=content_type,
@@ -299,22 +302,24 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_upgrade.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/upgrade"}  # type: ignore
+    begin_upgrade.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/upgrade"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_upgradable_versions_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_upgradable_versions_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,31 +41,31 @@
 
 def build_details_request(
     resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listUpgradableVersions",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -114,33 +114,34 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.UpgradableVersionsList]
+        )
+        cls: ClsType[_models.UpgradableVersionsList] = kwargs.pop("cls", None)
 
         request = build_details_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.details.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -151,8 +152,10 @@
         deserialized = self._deserialize("UpgradableVersionsList", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    details.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listUpgradableVersions"}  # type: ignore
+    details.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listUpgradableVersions"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_list_associated_traffic_filters_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_traffic_filters_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,122 +35,135 @@
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_list_request(resource_group_name: str, monitor_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+def build_delete_request(
+    resource_group_name: str,
+    monitor_name: str,
+    subscription_id: str,
+    *,
+    ruleset_id: Optional[str] = None,
+    **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAssociatedTrafficFilters",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/deleteTrafficFilter",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "monitorName": _SERIALIZER.url("monitor_name", monitor_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+    if ruleset_id is not None:
+        _params["rulesetId"] = _SERIALIZER.query("ruleset_id", ruleset_id, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class ListAssociatedTrafficFiltersOperations:
+class TrafficFiltersOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.MicrosoftElastic`'s
-        :attr:`list_associated_traffic_filters` attribute.
+        :attr:`traffic_filters` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> _models.ElasticTrafficFilterResponse:
-        """Get the list of all associated traffic filters for the given deployment.
+    def delete(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, monitor_name: str, ruleset_id: Optional[str] = None, **kwargs: Any
+    ) -> None:
+        """Delete traffic filter from the account.
 
-        Get the list of all associated traffic filters for the given deployment.
+        Delete traffic filter from the account.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
+        :param ruleset_id: Ruleset Id of the filter. Default value is None.
+        :type ruleset_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: ElasticTrafficFilterResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.elastic.models.ElasticTrafficFilterResponse
+        :return: None or the result of cls(response)
+        :rtype: None
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
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticTrafficFilterResponse]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_list_request(
+        request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
+            ruleset_id=ruleset_id,
             api_version=api_version,
-            template_url=self.list.metadata["url"],
+            template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("ElasticTrafficFilterResponse", pipeline_response)
-
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, None, {})
 
-        return deserialized
-
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAssociatedTrafficFilters"}  # type: ignore
+    delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/deleteTrafficFilter"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/operations/_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-07-01-preview")
-    )  # type: Literal["2022-07-01-preview"]
+    api_version: Literal["2023-02-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-02-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.Elastic/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -91,18 +91,18 @@
         :return: An iterator like instance of either OperationResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elastic.models.OperationResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.OperationListResult]
+        )
+        cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -114,15 +114,15 @@
                 request = build_list_request(
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -130,38 +130,39 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("OperationListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(
                     _models.ResourceProviderDefaultErrorResponse, pipeline_response
                 )
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/providers/Microsoft.Elastic/operations"}  # type: ignore
+    list.metadata = {"url": "/providers/Microsoft.Elastic/operations"}
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/__init__.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._microsoft_elastic import MicrosoftElastic
+from ._version import VERSION
+
+__version__ = VERSION
 
 try:
     from ._patch import __all__ as _patch_all
-    from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+    from ._patch import *  # pylint: disable=unused-wildcard-import
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "MicrosoftElastic",
 ]
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/_microsoft_elastic.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_microsoft_elastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from copy import deepcopy
 from typing import Any, Awaitable, TYPE_CHECKING
 
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
 
-from .. import models
+from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import MicrosoftElasticConfiguration
 from .operations import (
     AllTrafficFiltersOperations,
     AssociateTrafficFilterOperations,
     CreateAndAssociateIPFilterOperations,
     CreateAndAssociatePLFilterOperations,
@@ -25,14 +25,15 @@
     DetachTrafficFilterOperations,
     ExternalUserOperations,
     ListAssociatedTrafficFiltersOperations,
     MonitorOperations,
     MonitoredResourcesOperations,
     MonitorsOperations,
     Operations,
+    OrganizationsOperations,
     TagRulesOperations,
     TrafficFiltersOperations,
     UpgradableVersionsOperations,
     VMCollectionOperations,
     VMHostOperations,
     VMIngestionOperations,
 )
@@ -84,39 +85,41 @@
     :ivar detach_and_delete_traffic_filter: DetachAndDeleteTrafficFilterOperations operations
     :vartype detach_and_delete_traffic_filter:
      azure.mgmt.elastic.aio.operations.DetachAndDeleteTrafficFilterOperations
     :ivar detach_traffic_filter: DetachTrafficFilterOperations operations
     :vartype detach_traffic_filter: azure.mgmt.elastic.aio.operations.DetachTrafficFilterOperations
     :ivar traffic_filters: TrafficFiltersOperations operations
     :vartype traffic_filters: azure.mgmt.elastic.aio.operations.TrafficFiltersOperations
+    :ivar organizations: OrganizationsOperations operations
+    :vartype organizations: azure.mgmt.elastic.aio.operations.OrganizationsOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The Azure subscription ID. This is a GUID-formatted string (e.g.
      00000000-0000-0000-0000-000000000000). Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-07-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-02-01-preview". Note that overriding
      this default value may result in unsupported behavior.
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
         self._config = MicrosoftElasticConfiguration(credential=credential, subscription_id=subscription_id, **kwargs)
-        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
-        client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
+        client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.monitors = MonitorsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.monitored_resources = MonitoredResourcesOperations(
             self._client, self._config, self._serialize, self._deserialize
@@ -149,14 +152,15 @@
         self.detach_and_delete_traffic_filter = DetachAndDeleteTrafficFilterOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.detach_traffic_filter = DetachTrafficFilterOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.traffic_filters = TrafficFiltersOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.organizations = OrganizationsOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
@@ -179,9 +183,9 @@
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "MicrosoftElastic":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
+    async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/_patch.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/_configuration.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,22 @@
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The Azure subscription ID. This is a GUID-formatted string (e.g.
      00000000-0000-0000-0000-000000000000). Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-07-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-02-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(MicrosoftElasticConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "2022-07-01-preview")  # type: Literal["2022-07-01-preview"]
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop("api_version", "2023-02-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_monitored_resources_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_host_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,68 +24,66 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._monitored_resources_operations import build_list_request
+from ...operations._vm_host_operations import build_list_request
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
     from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class MonitoredResourcesOperations:
+class VMHostOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.aio.MicrosoftElastic`'s
-        :attr:`monitored_resources` attribute.
+        :attr:`vm_host` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(
-        self, resource_group_name: str, monitor_name: str, **kwargs: Any
-    ) -> AsyncIterable["_models.MonitoredResource"]:
-        """List the resources currently being monitored by the Elastic monitor resource.
+    def list(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> AsyncIterable["_models.VMResources"]:
+        """List the vm resources currently being monitored by the Elastic monitor resource.
 
-        List the resources currently being monitored by the Elastic monitor resource.
+        List the vm resources currently being monitored by the Elastic monitor resource.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either MonitoredResource or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.MonitoredResource]
+        :return: An iterator like instance of either VMResources or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.VMResources]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.MonitoredResourceListResponse]
+        )
+        cls: ClsType[_models.VMHostListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -100,15 +98,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -116,38 +114,41 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("MonitoredResourceListResponse", pipeline_response)
+            deserialized = self._deserialize("VMHostListResponse", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(
                     _models.ResourceProviderDefaultErrorResponse, pipeline_response
                 )
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listMonitoredResources"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listVMHost"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_vm_ingestion_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_ingestion_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,33 +80,34 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VMIngestionDetailsResponse]
+        )
+        cls: ClsType[_models.VMIngestionDetailsResponse] = kwargs.pop("cls", None)
 
         request = build_details_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.details.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -117,8 +118,10 @@
         deserialized = self._deserialize("VMIngestionDetailsResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    details.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/vmIngestionDetails"}  # type: ignore
+    details.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/vmIngestionDetails"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_create_and_associate_ip_filter_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_create_and_associate_ip_filter_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,50 +72,53 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ips=ips,
             name=name,
             api_version=api_version,
             template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [201]:
+        if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _create_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociateIPFilter"}  # type: ignore
+    _create_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociateIPFilter"
+    }
 
     @distributed_trace_async
     async def begin_create(
         self,
         resource_group_name: str,
         monitor_name: str,
         ips: Optional[str] = None,
@@ -146,21 +149,21 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 ips=ips,
                 name=name,
                 api_version=api_version,
@@ -172,22 +175,26 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_create.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociateIPFilter"}  # type: ignore
+    begin_create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociateIPFilter"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_traffic_filters_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_traffic_filters_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,42 +82,45 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ruleset_id=ruleset_id,
             api_version=api_version,
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/deleteTrafficFilter"}  # type: ignore
+    delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/deleteTrafficFilter"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_detach_and_delete_traffic_filter_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_detach_and_delete_traffic_filter_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,42 +82,45 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ruleset_id=ruleset_id,
             api_version=api_version,
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachAndDeleteTrafficFilter"}  # type: ignore
+    delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachAndDeleteTrafficFilter"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/__init__.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 from ._list_associated_traffic_filters_operations import ListAssociatedTrafficFiltersOperations
 from ._create_and_associate_ip_filter_operations import CreateAndAssociateIPFilterOperations
 from ._create_and_associate_pl_filter_operations import CreateAndAssociatePLFilterOperations
 from ._associate_traffic_filter_operations import AssociateTrafficFilterOperations
 from ._detach_and_delete_traffic_filter_operations import DetachAndDeleteTrafficFilterOperations
 from ._detach_traffic_filter_operations import DetachTrafficFilterOperations
 from ._traffic_filters_operations import TrafficFiltersOperations
+from ._organizations_operations import OrganizationsOperations
 
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Operations",
     "MonitorsOperations",
     "MonitoredResourcesOperations",
     "DeploymentInfoOperations",
@@ -46,10 +47,11 @@
     "ListAssociatedTrafficFiltersOperations",
     "CreateAndAssociateIPFilterOperations",
     "CreateAndAssociatePLFilterOperations",
     "AssociateTrafficFilterOperations",
     "DetachAndDeleteTrafficFilterOperations",
     "DetachTrafficFilterOperations",
     "TrafficFiltersOperations",
+    "OrganizationsOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_all_traffic_filters_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_list_associated_traffic_filters_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,32 +22,32 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._all_traffic_filters_operations import build_list_request
+from ...operations._list_associated_traffic_filters_operations import build_list_request
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
     from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class AllTrafficFiltersOperations:
+class ListAssociatedTrafficFiltersOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.aio.MicrosoftElastic`'s
-        :attr:`all_traffic_filters` attribute.
+        :attr:`list_associated_traffic_filters` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
@@ -55,17 +55,17 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace_async
     async def list(
         self, resource_group_name: str, monitor_name: str, **kwargs: Any
     ) -> _models.ElasticTrafficFilterResponse:
-        """Get the list of all traffic filters for the account.
+        """Get the list of all associated traffic filters for the given deployment.
 
-        Get the list of all traffic filters for the account.
+        Get the list of all associated traffic filters for the given deployment.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -80,33 +80,34 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticTrafficFilterResponse]
+        )
+        cls: ClsType[_models.ElasticTrafficFilterResponse] = kwargs.pop("cls", None)
 
         request = build_list_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -117,8 +118,10 @@
         deserialized = self._deserialize("ElasticTrafficFilterResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAllTrafficFilters"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAssociatedTrafficFilters"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_patch.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_create_and_associate_pl_filter_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_create_and_associate_pl_filter_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,51 +73,54 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             name=name,
             private_endpoint_guid=private_endpoint_guid,
             private_endpoint_name=private_endpoint_name,
             api_version=api_version,
             template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [201]:
+        if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _create_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociatePLFilter"}  # type: ignore
+    _create_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociatePLFilter"
+    }
 
     @distributed_trace_async
     async def begin_create(
         self,
         resource_group_name: str,
         monitor_name: str,
         name: Optional[str] = None,
@@ -151,21 +154,21 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 name=name,
                 private_endpoint_guid=private_endpoint_guid,
                 private_endpoint_name=private_endpoint_name,
@@ -178,22 +181,26 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_create.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociatePLFilter"}  # type: ignore
+    begin_create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createAndAssociatePLFilter"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_vm_collection_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_vm_collection_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,15 +128,16 @@
         Update the vm details that will be monitored by the Elastic monitor resource.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
-        :param body: VM resource Id. Is either a model type or a IO type. Default value is None.
+        :param body: VM resource Id. Is either a VMCollectionUpdate type or a IO type. Default value is
+         None.
         :type body: ~azure.mgmt.elastic.models.VMCollectionUpdate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
@@ -149,19 +150,19 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
@@ -179,26 +180,29 @@
             json=_json,
             content=_content,
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/vmCollectionUpdate"}  # type: ignore
+    update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/vmCollectionUpdate"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_associate_traffic_filter_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_associate_traffic_filter_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,49 +67,52 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_associate_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ruleset_id=ruleset_id,
             api_version=api_version,
             template_url=self._associate_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _associate_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/associateTrafficFilter"}  # type: ignore
+    _associate_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/associateTrafficFilter"
+    }
 
     @distributed_trace_async
     async def begin_associate(
         self, resource_group_name: str, monitor_name: str, ruleset_id: Optional[str] = None, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Associate traffic filter for the given deployment.
 
@@ -133,21 +136,21 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._associate_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 ruleset_id=ruleset_id,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
@@ -158,22 +161,26 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_associate.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/associateTrafficFilter"}  # type: ignore
+    begin_associate.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/associateTrafficFilter"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_vm_host_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,89 +24,81 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._vm_host_operations import build_list_request
+from ...operations._operations import build_list_request
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
     from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class VMHostOperations:
+class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.aio.MicrosoftElastic`'s
-        :attr:`vm_host` attribute.
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
-    def list(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> AsyncIterable["_models.VMResources"]:
-        """List the vm resources currently being monitored by the Elastic monitor resource.
+    def list(self, **kwargs: Any) -> AsyncIterable["_models.OperationResult"]:
+        """List all operations provided by Microsoft.Elastic.
 
-        List the vm resources currently being monitored by the Elastic monitor resource.
+        List all operations provided by Microsoft.Elastic.
 
-        :param resource_group_name: The name of the resource group to which the Elastic resource
-         belongs. Required.
-        :type resource_group_name: str
-        :param monitor_name: Monitor resource name. Required.
-        :type monitor_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either VMResources or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.VMResources]
+        :return: An iterator like instance of either OperationResult or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.OperationResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VMHostListResponse]
+        )
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
-                    resource_group_name=resource_group_name,
-                    monitor_name=monitor_name,
-                    subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -114,38 +106,39 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("VMHostListResponse", pipeline_response)
+            deserialized = self._deserialize("OperationListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(
                     _models.ResourceProviderDefaultErrorResponse, pipeline_response
                 )
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listVMHost"}  # type: ignore
+    list.metadata = {"url": "/providers/Microsoft.Elastic/operations"}
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_monitors_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitors_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,18 +79,18 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.ElasticMonitorResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticMonitorResourceListResponse]
+        )
+        cls: ClsType[_models.ElasticMonitorResourceListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -103,15 +103,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -119,45 +119,46 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ElasticMonitorResourceListResponse", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(
                     _models.ResourceProviderDefaultErrorResponse, pipeline_response
                 )
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Elastic/monitors"}  # type: ignore
+    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Elastic/monitors"}
 
     @distributed_trace
     def list_by_resource_group(
         self, resource_group_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.ElasticMonitorResource"]:
         """List all monitors under the specified resource group.
 
@@ -172,18 +173,18 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.ElasticMonitorResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticMonitorResourceListResponse]
+        )
+        cls: ClsType[_models.ElasticMonitorResourceListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -197,15 +198,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list_by_resource_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -213,45 +214,48 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ElasticMonitorResourceListResponse", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(
                     _models.ResourceProviderDefaultErrorResponse, pipeline_response
                 )
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors"}  # type: ignore
+    list_by_resource_group.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors"
+    }
 
     @distributed_trace_async
     async def get(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> _models.ElasticMonitorResource:
         """Get the properties of a specific monitor resource.
 
         Get the properties of a specific monitor resource.
 
@@ -272,33 +276,34 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticMonitorResource]
+        )
+        cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -309,15 +314,17 @@
         deserialized = self._deserialize("ElasticMonitorResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"
+    }
 
     async def _create_initial(
         self,
         resource_group_name: str,
         monitor_name: str,
         body: Optional[Union[_models.ElasticMonitorResource, IO]] = None,
         **kwargs: Any
@@ -329,19 +336,19 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticMonitorResource]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
@@ -359,18 +366,19 @@
             json=_json,
             content=_content,
             template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -381,19 +389,21 @@
         if response.status_code == 200:
             deserialized = self._deserialize("ElasticMonitorResource", pipeline_response)
 
         if response.status_code == 201:
             deserialized = self._deserialize("ElasticMonitorResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _create_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"}  # type: ignore
+    _create_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"
+    }
 
     @overload
     async def begin_create(
         self,
         resource_group_name: str,
         monitor_name: str,
         body: Optional[_models.ElasticMonitorResource] = None,
@@ -480,16 +490,16 @@
         Create a monitor resource.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
-        :param body: Elastic monitor resource model. Is either a model type or a IO type. Default value
-         is None.
+        :param body: Elastic monitor resource model. Is either a ElasticMonitorResource type or a IO
+         type. Default value is None.
         :type body: ~azure.mgmt.elastic.models.ElasticMonitorResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -502,24 +512,24 @@
          of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.elastic.models.ElasticMonitorResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticMonitorResource]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_initial(  # type: ignore
+            raw_result = await self._create_initial(
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 body=body,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -531,32 +541,34 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ElasticMonitorResource", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(
+            polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
-            )  # type: AsyncPollingMethod
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_create.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"}  # type: ignore
+    begin_create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"
+    }
 
     @overload
     async def update(
         self,
         resource_group_name: str,
         monitor_name: str,
         body: Optional[_models.ElasticMonitorResourceUpdateParameters] = None,
@@ -627,16 +639,16 @@
         Update a monitor resource.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
-        :param body: Elastic resource model update parameters. Is either a model type or a IO type.
-         Default value is None.
+        :param body: Elastic resource model update parameters. Is either a
+         ElasticMonitorResourceUpdateParameters type or a IO type. Default value is None.
         :type body: ~azure.mgmt.elastic.models.ElasticMonitorResourceUpdateParameters or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ElasticMonitorResource or the result of cls(response)
         :rtype: ~azure.mgmt.elastic.models.ElasticMonitorResource
@@ -649,19 +661,19 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticMonitorResource]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ElasticMonitorResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
@@ -679,18 +691,19 @@
             json=_json,
             content=_content,
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -701,15 +714,17 @@
         deserialized = self._deserialize("ElasticMonitorResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"}  # type: ignore
+    update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"
+    }
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, monitor_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -717,48 +732,51 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"
+    }
 
     @distributed_trace_async
     async def begin_delete(self, resource_group_name: str, monitor_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
         """Delete a monitor resource.
 
         Delete a monitor resource.
 
@@ -778,21 +796,21 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -802,22 +820,24 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_external_user_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_external_user_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,16 +134,16 @@
         elastic deployment.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
-        :param body: Elastic External User Creation Parameters. Is either a model type or a IO type.
-         Default value is None.
+        :param body: Elastic External User Creation Parameters. Is either a ExternalUserInfo type or a
+         IO type. Default value is None.
         :type body: ~azure.mgmt.elastic.models.ExternalUserInfo or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ExternalUserCreationResponse or the result of cls(response)
         :rtype: ~azure.mgmt.elastic.models.ExternalUserCreationResponse
@@ -156,19 +156,19 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ExternalUserCreationResponse]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ExternalUserCreationResponse] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
@@ -186,18 +186,19 @@
             json=_json,
             content=_content,
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -208,8 +209,10 @@
         deserialized = self._deserialize("ExternalUserCreationResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createOrUpdateExternalUser"}  # type: ignore
+    create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/createOrUpdateExternalUser"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_deployment_info_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_deployment_info_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -80,33 +80,34 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.DeploymentInfoResponse]
+        )
+        cls: ClsType[_models.DeploymentInfoResponse] = kwargs.pop("cls", None)
 
         request = build_list_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -117,8 +118,10 @@
         deserialized = self._deserialize("DeploymentInfoResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listDeploymentInfo"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listDeploymentInfo"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_tag_rules_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_tag_rules_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,18 +82,18 @@
         :return: An iterator like instance of either MonitoringTagRules or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.MonitoringTagRules]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.MonitoringTagRulesListResponse]
+        )
+        cls: ClsType[_models.MonitoringTagRulesListResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -108,15 +108,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -124,45 +124,48 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("MonitoringTagRulesListResponse", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(
                     _models.ResourceProviderDefaultErrorResponse, pipeline_response
                 )
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules"
+    }
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         monitor_name: str,
         rule_set_name: str,
@@ -242,16 +245,16 @@
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :param rule_set_name: Tag Rule Set resource name. Required.
         :type rule_set_name: str
-        :param body: request body of MonitoringTagRules. Is either a model type or a IO type. Default
-         value is None.
+        :param body: request body of MonitoringTagRules. Is either a MonitoringTagRules type or a IO
+         type. Default value is None.
         :type body: ~azure.mgmt.elastic.models.MonitoringTagRules or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MonitoringTagRules or the result of cls(response)
         :rtype: ~azure.mgmt.elastic.models.MonitoringTagRules
@@ -264,19 +267,19 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.MonitoringTagRules]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.MonitoringTagRules] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
@@ -295,18 +298,19 @@
             json=_json,
             content=_content,
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -317,15 +321,17 @@
         deserialized = self._deserialize("MonitoringTagRules", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"}  # type: ignore
+    create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"
+    }
 
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, monitor_name: str, rule_set_name: str, **kwargs: Any
     ) -> _models.MonitoringTagRules:
         """Get a tag rule set for a given monitor resource.
 
@@ -350,34 +356,35 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.MonitoringTagRules]
+        )
+        cls: ClsType[_models.MonitoringTagRules] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             rule_set_name=rule_set_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -388,15 +395,17 @@
         deserialized = self._deserialize("MonitoringTagRules", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"
+    }
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, monitor_name: str, rule_set_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -404,49 +413,52 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             rule_set_name=rule_set_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"
+    }
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, monitor_name: str, rule_set_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Delete a tag rule set for a given monitor resource.
 
@@ -470,21 +482,21 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 rule_set_name=rule_set_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
@@ -495,22 +507,24 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/tagRules/{ruleSetName}"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_detach_traffic_filter_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_detach_traffic_filter_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,49 +67,52 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             ruleset_id=ruleset_id,
             api_version=api_version,
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachTrafficFilter"}  # type: ignore
+    _update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachTrafficFilter"
+    }
 
     @distributed_trace_async
     async def begin_update(
         self, resource_group_name: str, monitor_name: str, ruleset_id: Optional[str] = None, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Detach traffic filter for the given deployment.
 
@@ -133,21 +136,21 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        )
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._update_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 ruleset_id=ruleset_id,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
@@ -158,22 +161,26 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachTrafficFilter"}  # type: ignore
+    begin_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/detachTrafficFilter"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_monitor_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitor_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,19 +71,19 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
@@ -101,33 +101,36 @@
             json=_json,
             content=_content,
             template_url=self._upgrade_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
                 _models.ResourceProviderDefaultErrorResponse, pipeline_response
             )
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _upgrade_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/upgrade"}  # type: ignore
+    _upgrade_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/upgrade"
+    }
 
     @overload
     async def begin_upgrade(
         self,
         resource_group_name: str,
         monitor_name: str,
         body: Optional[_models.ElasticMonitorUpgrade] = None,
@@ -212,16 +215,16 @@
         Upgradable version for a monitor resource.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
-        :param body: Elastic Monitor Upgrade Parameters. Is either a model type or a IO type. Default
-         value is None.
+        :param body: Elastic Monitor Upgrade Parameters. Is either a ElasticMonitorUpgrade type or a IO
+         type. Default value is None.
         :type body: ~azure.mgmt.elastic.models.ElasticMonitorUpgrade or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -233,22 +236,22 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        )
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._upgrade_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 monitor_name=monitor_name,
                 body=body,
                 api_version=api_version,
                 content_type=content_type,
@@ -260,22 +263,24 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_upgrade.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/upgrade"}  # type: ignore
+    begin_upgrade.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/upgrade"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_upgradable_versions_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_upgradable_versions_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,33 +80,34 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.UpgradableVersionsList]
+        )
+        cls: ClsType[_models.UpgradableVersionsList] = kwargs.pop("cls", None)
 
         request = build_details_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.details.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -117,8 +118,10 @@
         deserialized = self._deserialize("UpgradableVersionsList", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    details.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listUpgradableVersions"}  # type: ignore
+    details.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listUpgradableVersions"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_list_associated_traffic_filters_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_all_traffic_filters_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,32 +22,32 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._list_associated_traffic_filters_operations import build_list_request
+from ...operations._all_traffic_filters_operations import build_list_request
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
     from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class ListAssociatedTrafficFiltersOperations:
+class AllTrafficFiltersOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.aio.MicrosoftElastic`'s
-        :attr:`list_associated_traffic_filters` attribute.
+        :attr:`all_traffic_filters` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
@@ -55,17 +55,17 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace_async
     async def list(
         self, resource_group_name: str, monitor_name: str, **kwargs: Any
     ) -> _models.ElasticTrafficFilterResponse:
-        """Get the list of all associated traffic filters for the given deployment.
+        """Get the list of all traffic filters for the account.
 
-        Get the list of all associated traffic filters for the given deployment.
+        Get the list of all traffic filters for the account.
 
         :param resource_group_name: The name of the resource group to which the Elastic resource
          belongs. Required.
         :type resource_group_name: str
         :param monitor_name: Monitor resource name. Required.
         :type monitor_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -80,33 +80,34 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticTrafficFilterResponse]
+        )
+        cls: ClsType[_models.ElasticTrafficFilterResponse] = kwargs.pop("cls", None)
 
         request = build_list_request(
             resource_group_name=resource_group_name,
             monitor_name=monitor_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(
@@ -117,8 +118,10 @@
         deserialized = self._deserialize("ElasticTrafficFilterResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAssociatedTrafficFilters"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listAllTrafficFilters"
+    }
```

## Comparing `azure-mgmt-elastic-1.1.0b1/azure/mgmt/elastic/aio/operations/_operations.py` & `azure-mgmt-elastic-1.1.0b2/azure/mgmt/elastic/aio/operations/_monitored_resources_operations.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,81 +24,91 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._operations import build_list_request
+from ...operations._monitored_resources_operations import build_list_request
 
 if sys.version_info >= (3, 8):
     from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
 else:
     from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class Operations:
+class MonitoredResourcesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.elastic.aio.MicrosoftElastic`'s
-        :attr:`operations` attribute.
+        :attr:`monitored_resources` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> AsyncIterable["_models.OperationResult"]:
-        """List all operations provided by Microsoft.Elastic.
-
-        List all operations provided by Microsoft.Elastic.
-
+    def list(
+        self, resource_group_name: str, monitor_name: str, **kwargs: Any
+    ) -> AsyncIterable["_models.MonitoredResource"]:
+        """List the resources currently being monitored by the Elastic monitor resource.
+
+        List the resources currently being monitored by the Elastic monitor resource.
+
+        :param resource_group_name: The name of the resource group to which the Elastic resource
+         belongs. Required.
+        :type resource_group_name: str
+        :param monitor_name: Monitor resource name. Required.
+        :type monitor_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either OperationResult or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.OperationResult]
+        :return: An iterator like instance of either MonitoredResource or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elastic.models.MonitoredResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
+        api_version: Literal["2023-02-01-preview"] = kwargs.pop(
             "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-07-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.OperationListResult]
+        )
+        cls: ClsType[_models.MonitoredResourceListResponse] = kwargs.pop("cls", None)
 
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
+                    resource_group_name=resource_group_name,
+                    monitor_name=monitor_name,
+                    subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -106,38 +116,41 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("OperationListResult", pipeline_response)
+            deserialized = self._deserialize("MonitoredResourceListResponse", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(
                     _models.ResourceProviderDefaultErrorResponse, pipeline_response
                 )
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/providers/Microsoft.Elastic/operations"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Elastic/monitors/{monitorName}/listMonitoredResources"
+    }
```

