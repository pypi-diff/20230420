# Comparing `tmp/google-cloud-resource-manager-1.9.0.tar.gz` & `tmp/google-cloud-resource-manager-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-resource-manager-1.9.0.tar", last modified: Tue Feb 28 18:11:55 2023, max compression
+gzip compressed data, was "google-cloud-resource-manager-1.9.1.tar", last modified: Mon Mar 27 15:33:15 2023, max compression
```

## Comparing `google-cloud-resource-manager-1.9.0.tar` & `google-cloud-resource-manager-1.9.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.841622 google-cloud-resource-manager-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4712 2023-02-28 18:11:55.841622 google-cloud-resource-manager-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3769 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.817624 google-cloud-resource-manager-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.817624 google-cloud-resource-manager-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.821624 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager/
--rw-rw-r--   0 root         (0)     1003     6056 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.821624 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/
--rw-rw-r--   0 root         (0)     1003     5119 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/__init__.py
--rw-rw-r--   0 root         (0)     1003    19535 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.821624 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.825624 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/
--rw-rw-r--   0 root         (0)     1003      741 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/__init__.py
--rw-rw-r--   0 root         (0)     1003    75733 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/async_client.py
--rw-rw-r--   0 root         (0)     1003    84496 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/client.py
--rw-rw-r--   0 root         (0)     1003    10676 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.825624 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/transports/
--rw-rw-r--   0 root         (0)     1003     1302 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11744 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/transports/base.py
--rw-rw-r--   0 root         (0)     1003    30094 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    30586 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    70608 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.825624 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/
--rw-rw-r--   0 root         (0)     1003      765 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/__init__.py
--rw-rw-r--   0 root         (0)     1003    40947 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/async_client.py
--rw-rw-r--   0 root         (0)     1003    49258 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/client.py
--rw-rw-r--   0 root         (0)     1003     6028 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.825624 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8806 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17878 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18184 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    39530 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.829623 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/
--rw-rw-r--   0 root         (0)     1003      745 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/__init__.py
--rw-rw-r--   0 root         (0)     1003    78035 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/async_client.py
--rw-rw-r--   0 root         (0)     1003    86826 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/client.py
--rw-rw-r--   0 root         (0)     1003    10765 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.829623 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/transports/
--rw-rw-r--   0 root         (0)     1003     1316 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11831 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/transports/base.py
--rw-rw-r--   0 root         (0)     1003    30246 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    30767 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    72325 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.829623 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/
--rw-rw-r--   0 root         (0)     1003      757 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/__init__.py
--rw-rw-r--   0 root         (0)     1003    24209 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/async_client.py
--rw-rw-r--   0 root         (0)     1003    33146 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/client.py
--rw-rw-r--   0 root         (0)     1003     5911 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.829623 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7648 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15143 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15471 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    23936 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.829623 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/
--rw-rw-r--   0 root         (0)     1003      741 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/__init__.py
--rw-rw-r--   0 root         (0)     1003    54344 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/async_client.py
--rw-rw-r--   0 root         (0)     1003    62745 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/client.py
--rw-rw-r--   0 root         (0)     1003     5731 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.833623 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/transports/
--rw-rw-r--   0 root         (0)     1003     1302 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10489 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/transports/base.py
--rw-rw-r--   0 root         (0)     1003    21376 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    21802 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    55492 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.833623 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/
--rw-rw-r--   0 root         (0)     1003      749 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/__init__.py
--rw-rw-r--   0 root         (0)     1003    54919 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/async_client.py
--rw-rw-r--   0 root         (0)     1003    63338 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/client.py
--rw-rw-r--   0 root         (0)     1003     5821 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.833623 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/transports/
--rw-rw-r--   0 root         (0)     1003     1330 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10607 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/transports/base.py
--rw-rw-r--   0 root         (0)     1003    21696 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22151 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    56221 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.837623 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/
--rw-rw-r--   0 root         (0)     1003     4227 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    15250 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/folders.py
--rw-rw-r--   0 root         (0)     1003     8390 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/organizations.py
--rw-rw-r--   0 root         (0)     1003    19187 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/projects.py
--rw-rw-r--   0 root         (0)     1003     5808 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/tag_bindings.py
--rw-rw-r--   0 root         (0)     1003     9023 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/tag_keys.py
--rw-rw-r--   0 root         (0)     1003     9092 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/tag_values.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.837623 google-cloud-resource-manager-1.9.0/google_cloud_resource_manager.egg-info/
--rw-r--r--   0 root         (0)     1003     4712 2023-02-28 18:11:55.000000 google-cloud-resource-manager-1.9.0/google_cloud_resource_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     5317 2023-02-28 18:11:55.000000 google-cloud-resource-manager-1.9.0/google_cloud_resource_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-02-28 18:11:55.000000 google-cloud-resource-manager-1.9.0/google_cloud_resource_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-02-28 18:11:55.000000 google-cloud-resource-manager-1.9.0/google_cloud_resource_manager.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-02-28 18:11:55.000000 google-cloud-resource-manager-1.9.0/google_cloud_resource_manager.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-02-28 18:11:55.000000 google-cloud-resource-manager-1.9.0/google_cloud_resource_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-02-28 18:11:55.000000 google-cloud-resource-manager-1.9.0/google_cloud_resource_manager.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-02-28 18:11:55.841622 google-cloud-resource-manager-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3010 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.837623 google-cloud-resource-manager-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.837623 google-cloud-resource-manager-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.837623 google-cloud-resource-manager-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-28 18:11:55.841622 google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/__init__.py
--rw-rw-r--   0 root         (0)     1003   259022 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/test_folders.py
--rw-rw-r--   0 root         (0)     1003   151357 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/test_organizations.py
--rw-rw-r--   0 root         (0)     1003   261141 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/test_projects.py
--rw-rw-r--   0 root         (0)     1003   113833 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/test_tag_bindings.py
--rw-rw-r--   0 root         (0)     1003   205013 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/test_tag_keys.py
--rw-rw-r--   0 root         (0)     1003   207468 2023-02-28 18:09:34.000000 google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/test_tag_values.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.157776 google-cloud-resource-manager-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4712 2023-03-27 15:33:15.157776 google-cloud-resource-manager-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3769 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.133775 google-cloud-resource-manager-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.133775 google-cloud-resource-manager-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.137775 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager/
+-rw-rw-r--   0 root         (0)     1003     6056 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.137775 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/
+-rw-rw-r--   0 root         (0)     1003     5119 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19535 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.137775 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.141775 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/
+-rw-rw-r--   0 root         (0)     1003      741 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/__init__.py
+-rw-rw-r--   0 root         (0)     1003    75695 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/async_client.py
+-rw-rw-r--   0 root         (0)     1003    84458 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/client.py
+-rw-rw-r--   0 root         (0)     1003    10676 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.141775 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/transports/
+-rw-rw-r--   0 root         (0)     1003     1302 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11744 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    30094 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    30586 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    70662 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.141775 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/
+-rw-rw-r--   0 root         (0)     1003      765 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/__init__.py
+-rw-rw-r--   0 root         (0)     1003    40897 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/async_client.py
+-rw-rw-r--   0 root         (0)     1003    49208 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/client.py
+-rw-rw-r--   0 root         (0)     1003     6028 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.141775 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8806 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17878 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18184 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    39585 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.145776 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/
+-rw-rw-r--   0 root         (0)     1003      745 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/__init__.py
+-rw-rw-r--   0 root         (0)     1003    77983 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/async_client.py
+-rw-rw-r--   0 root         (0)     1003    86774 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/client.py
+-rw-rw-r--   0 root         (0)     1003    10765 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.145776 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/transports/
+-rw-rw-r--   0 root         (0)     1003     1316 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11831 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    30246 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    30767 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    72373 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.145776 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/
+-rw-rw-r--   0 root         (0)     1003      757 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24209 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/async_client.py
+-rw-rw-r--   0 root         (0)     1003    33146 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/client.py
+-rw-rw-r--   0 root         (0)     1003     5911 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.145776 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7648 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15143 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15471 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    23933 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.145776 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/
+-rw-rw-r--   0 root         (0)     1003      741 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/__init__.py
+-rw-rw-r--   0 root         (0)     1003    54302 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/async_client.py
+-rw-rw-r--   0 root         (0)     1003    62703 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/client.py
+-rw-rw-r--   0 root         (0)     1003     5731 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.149776 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/transports/
+-rw-rw-r--   0 root         (0)     1003     1302 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10489 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    21376 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21802 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    55543 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.149776 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/
+-rw-rw-r--   0 root         (0)     1003      749 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/__init__.py
+-rw-rw-r--   0 root         (0)     1003    54877 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/async_client.py
+-rw-rw-r--   0 root         (0)     1003    63296 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/client.py
+-rw-rw-r--   0 root         (0)     1003     5821 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.149776 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/transports/
+-rw-rw-r--   0 root         (0)     1003     1330 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10607 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    21696 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22151 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    56272 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.153776 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/
+-rw-rw-r--   0 root         (0)     1003     4227 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15250 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/folders.py
+-rw-rw-r--   0 root         (0)     1003     8390 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/organizations.py
+-rw-rw-r--   0 root         (0)     1003    19187 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/projects.py
+-rw-rw-r--   0 root         (0)     1003     5808 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/tag_bindings.py
+-rw-rw-r--   0 root         (0)     1003     9023 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/tag_keys.py
+-rw-rw-r--   0 root         (0)     1003     9092 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/tag_values.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.153776 google-cloud-resource-manager-1.9.1/google_cloud_resource_manager.egg-info/
+-rw-r--r--   0 root         (0)     1003     4712 2023-03-27 15:33:15.000000 google-cloud-resource-manager-1.9.1/google_cloud_resource_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     5317 2023-03-27 15:33:15.000000 google-cloud-resource-manager-1.9.1/google_cloud_resource_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:33:15.000000 google-cloud-resource-manager-1.9.1/google_cloud_resource_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:33:15.000000 google-cloud-resource-manager-1.9.1/google_cloud_resource_manager.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:33:15.000000 google-cloud-resource-manager-1.9.1/google_cloud_resource_manager.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-03-27 15:33:15.000000 google-cloud-resource-manager-1.9.1/google_cloud_resource_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:33:15.000000 google-cloud-resource-manager-1.9.1/google_cloud_resource_manager.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:33:15.157776 google-cloud-resource-manager-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3009 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.153776 google-cloud-resource-manager-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.153776 google-cloud-resource-manager-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.153776 google-cloud-resource-manager-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:33:15.157776 google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/__init__.py
+-rw-rw-r--   0 root         (0)     1003   259022 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/test_folders.py
+-rw-rw-r--   0 root         (0)     1003   151357 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/test_organizations.py
+-rw-rw-r--   0 root         (0)     1003   261141 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/test_projects.py
+-rw-rw-r--   0 root         (0)     1003   113833 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/test_tag_bindings.py
+-rw-rw-r--   0 root         (0)     1003   205013 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/test_tag_keys.py
+-rw-rw-r--   0 root         (0)     1003   207468 2023-03-27 15:30:25.000000 google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/test_tag_values.py
```

### Comparing `google-cloud-resource-manager-1.9.0/LICENSE` & `google-cloud-resource-manager-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/MANIFEST.in` & `google-cloud-resource-manager-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/PKG-INFO` & `google-cloud-resource-manager-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-resource-manager
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Resource Manager API client library
 Home-page: https://github.com/googleapis/python-resource-manager
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-resource-manager-1.9.0/README.rst` & `google-cloud-resource-manager-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager/gapic_version.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/gapic_metadata.json` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/gapic_version.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/async_client.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -812,18 +812,18 @@
 
         Args:
             request (Optional[Union[google.cloud.resourcemanager_v3.types.UpdateFolderRequest, dict]]):
                 The request object. The request sent to the
                 [UpdateFolder][google.cloud.resourcemanager.v3.Folder.UpdateFolder]
                 method.
 
-                Only the `display_name` field can be changed. All other
-                fields will be ignored. Use the
+                Only the ``display_name`` field can be changed. All
+                other fields will be ignored. Use the
                 [MoveFolder][google.cloud.resourcemanager.v3.Folders.MoveFolder]
-                method to change the `parent` field.
+                method to change the ``parent`` field.
             folder (:class:`google.cloud.resourcemanager_v3.types.Folder`):
                 Required. The new definition of the Folder. It must
                 include the ``name`` field, which cannot be changed.
 
                 This corresponds to the ``folder`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -1341,16 +1341,15 @@
                 response = await client.get_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]]):
-                The request object. Request message for `GetIamPolicy`
-                method.
+                The request object. Request message for ``GetIamPolicy`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1520,16 +1519,15 @@
                 response = await client.set_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]]):
-                The request object. Request message for `SetIamPolicy`
-                method.
+                The request object. Request message for ``SetIamPolicy`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1692,16 +1690,15 @@
                 response = await client.test_iam_permissions(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]]):
-                The request object. Request message for
-                `TestIamPermissions` method.
+                The request object. Request message for ``TestIamPermissions`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
                 the operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/client.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1022,18 +1022,18 @@
 
         Args:
             request (Union[google.cloud.resourcemanager_v3.types.UpdateFolderRequest, dict]):
                 The request object. The request sent to the
                 [UpdateFolder][google.cloud.resourcemanager.v3.Folder.UpdateFolder]
                 method.
 
-                Only the `display_name` field can be changed. All other
-                fields will be ignored. Use the
+                Only the ``display_name`` field can be changed. All
+                other fields will be ignored. Use the
                 [MoveFolder][google.cloud.resourcemanager.v3.Folders.MoveFolder]
-                method to change the `parent` field.
+                method to change the ``parent`` field.
             folder (google.cloud.resourcemanager_v3.types.Folder):
                 Required. The new definition of the Folder. It must
                 include the ``name`` field, which cannot be changed.
 
                 This corresponds to the ``folder`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -1551,16 +1551,15 @@
                 response = client.get_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]):
-                The request object. Request message for `GetIamPolicy`
-                method.
+                The request object. Request message for ``GetIamPolicy`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1718,16 +1717,15 @@
                 response = client.set_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]):
-                The request object. Request message for `SetIamPolicy`
-                method.
+                The request object. Request message for ``SetIamPolicy`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1887,16 +1885,15 @@
                 response = client.test_iam_permissions(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]):
-                The request object. Request message for
-                `TestIamPermissions` method.
+                The request object. Request message for ``TestIamPermissions`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
                 the operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/pagers.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/transports/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/transports/base.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/transports/grpc.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/transports/grpc_asyncio.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/folders/transports/rest.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/folders/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -881,15 +881,16 @@
                           "role": "roles/resourcemanager.organizationViewer",
                           "members": [
                             "user:eve@example.com"
                           ],
                           "condition": {
                             "title": "expirable access",
                             "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time < timestamp('2020-10-01T00:00:00.000Z')",
+                            "expression": "request.time <
+                            timestamp('2020-10-01T00:00:00.000Z')",
                           }
                         }
                       ],
                       "etag": "BwWWja0YfJA=",
                       "version": 3
                     }
 
@@ -1174,15 +1175,14 @@
         ) -> folders.SearchFoldersResponse:
             r"""Call the search folders method over HTTP.
 
             Args:
                 request (~.folders.SearchFoldersRequest):
                     The request object. The request message for searching
                 folders.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1313,15 +1313,16 @@
                           "role": "roles/resourcemanager.organizationViewer",
                           "members": [
                             "user:eve@example.com"
                           ],
                           "condition": {
                             "title": "expirable access",
                             "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time < timestamp('2020-10-01T00:00:00.000Z')",
+                            "expression": "request.time <
+                            timestamp('2020-10-01T00:00:00.000Z')",
                           }
                         }
                       ],
                       "etag": "BwWWja0YfJA=",
                       "version": 3
                     }
 
@@ -1633,15 +1634,14 @@
                 [UpdateFolder][google.cloud.resourcemanager.v3.Folder.UpdateFolder]
                 method.
 
                 Only the ``display_name`` field can be changed. All
                 other fields will be ignored. Use the
                 [MoveFolder][google.cloud.resourcemanager.v3.Folders.MoveFolder]
                 method to change the ``parent`` field.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/async_client.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,17 +254,17 @@
                 response = await client.get_organization(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.resourcemanager_v3.types.GetOrganizationRequest, dict]]):
-                The request object. The request sent to the
-                `GetOrganization` method. The `name` field is required.
-                `organization_id` is no longer accepted.
+                The request object. The request sent to the ``GetOrganization`` method. The
+                ``name`` field is required. ``organization_id`` is no
+                longer accepted.
             name (:class:`str`):
                 Required. The resource name of the Organization to
                 fetch. This is the organization's relative path in the
                 API, formatted as "organizations/[organizationId]". For
                 example, "organizations/1234".
 
                 This corresponds to the ``name`` field
@@ -377,16 +377,15 @@
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.resourcemanager_v3.types.SearchOrganizationsRequest, dict]]):
-                The request object. The request sent to the
-                `SearchOrganizations` method.
+                The request object. The request sent to the ``SearchOrganizations`` method.
             query (:class:`str`):
                 Optional. An optional query string used to filter the
                 Organizations to return in the response. Query rules are
                 case-insensitive.
 
                 ::
 
@@ -513,16 +512,15 @@
                 response = await client.get_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]]):
-                The request object. Request message for `GetIamPolicy`
-                method.
+                The request object. Request message for ``GetIamPolicy`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -695,16 +693,15 @@
                 response = await client.set_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]]):
-                The request object. Request message for `SetIamPolicy`
-                method.
+                The request object. Request message for ``SetIamPolicy`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -867,16 +864,15 @@
                 response = await client.test_iam_permissions(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]]):
-                The request object. Request message for
-                `TestIamPermissions` method.
+                The request object. Request message for ``TestIamPermissions`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
                 the operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/client.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -474,17 +474,17 @@
                 response = client.get_organization(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.resourcemanager_v3.types.GetOrganizationRequest, dict]):
-                The request object. The request sent to the
-                `GetOrganization` method. The `name` field is required.
-                `organization_id` is no longer accepted.
+                The request object. The request sent to the ``GetOrganization`` method. The
+                ``name`` field is required. ``organization_id`` is no
+                longer accepted.
             name (str):
                 Required. The resource name of the Organization to
                 fetch. This is the organization's relative path in the
                 API, formatted as "organizations/[organizationId]". For
                 example, "organizations/1234".
 
                 This corresponds to the ``name`` field
@@ -588,16 +588,15 @@
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.resourcemanager_v3.types.SearchOrganizationsRequest, dict]):
-                The request object. The request sent to the
-                `SearchOrganizations` method.
+                The request object. The request sent to the ``SearchOrganizations`` method.
             query (str):
                 Optional. An optional query string used to filter the
                 Organizations to return in the response. Query rules are
                 case-insensitive.
 
                 ::
 
@@ -724,16 +723,15 @@
                 response = client.get_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]):
-                The request object. Request message for `GetIamPolicy`
-                method.
+                The request object. Request message for ``GetIamPolicy`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -894,16 +892,15 @@
                 response = client.set_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]):
-                The request object. Request message for `SetIamPolicy`
-                method.
+                The request object. Request message for ``SetIamPolicy`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1063,16 +1060,15 @@
                 response = client.test_iam_permissions(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]):
-                The request object. Request message for
-                `TestIamPermissions` method.
+                The request object. Request message for ``TestIamPermissions`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
                 the operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/pagers.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/transports/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/transports/base.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/transports/grpc.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/transports/grpc_asyncio.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/organizations/transports/rest.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/organizations/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,15 +394,16 @@
                           "role": "roles/resourcemanager.organizationViewer",
                           "members": [
                             "user:eve@example.com"
                           ],
                           "condition": {
                             "title": "expirable access",
                             "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time < timestamp('2020-10-01T00:00:00.000Z')",
+                            "expression": "request.time <
+                            timestamp('2020-10-01T00:00:00.000Z')",
                           }
                         }
                       ],
                       "etag": "BwWWja0YfJA=",
                       "version": 3
                     }
 
@@ -514,15 +515,14 @@
             r"""Call the get organization method over HTTP.
 
             Args:
                 request (~.organizations.GetOrganizationRequest):
                     The request object. The request sent to the ``GetOrganization`` method. The
                 ``name`` field is required. ``organization_id`` is no
                 longer accepted.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -737,15 +737,16 @@
                           "role": "roles/resourcemanager.organizationViewer",
                           "members": [
                             "user:eve@example.com"
                           ],
                           "condition": {
                             "title": "expirable access",
                             "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time < timestamp('2020-10-01T00:00:00.000Z')",
+                            "expression": "request.time <
+                            timestamp('2020-10-01T00:00:00.000Z')",
                           }
                         }
                       ],
                       "etag": "BwWWja0YfJA=",
                       "version": 3
                     }
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/async_client.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -805,18 +805,18 @@
 
         Args:
             request (Optional[Union[google.cloud.resourcemanager_v3.types.UpdateProjectRequest, dict]]):
                 The request object. The request sent to the
                 [UpdateProject][google.cloud.resourcemanager.v3.Projects.UpdateProject]
                 method.
 
-                Only the `display_name` and `labels` fields can be
+                Only the ``display_name`` and ``labels`` fields can be
                 change. Use the
                 [MoveProject][google.cloud.resourcemanager.v3.Projects.MoveProject]
-                method to change the `parent` field.
+                method to change the ``parent`` field.
             project (:class:`google.cloud.resourcemanager_v3.types.Project`):
                 Required. The new definition of the
                 project.
 
                 This corresponds to the ``project`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -1233,16 +1233,15 @@
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.resourcemanager_v3.types.UndeleteProjectRequest, dict]]):
-                The request object. The request sent to the
-                [UndeleteProject]
+                The request object. The request sent to the [UndeleteProject]
                 [google.cloud.resourcemanager.v3.Projects.UndeleteProject]
                 method.
             name (:class:`str`):
                 Required. The name of the project (for example,
                 ``projects/415104041262``).
 
                 Required.
@@ -1353,16 +1352,15 @@
                 response = await client.get_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]]):
-                The request object. Request message for `GetIamPolicy`
-                method.
+                The request object. Request message for ``GetIamPolicy`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1579,16 +1577,15 @@
                 response = await client.set_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]]):
-                The request object. Request message for `SetIamPolicy`
-                method.
+                The request object. Request message for ``SetIamPolicy`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1748,16 +1745,15 @@
                 response = await client.test_iam_permissions(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]]):
-                The request object. Request message for
-                `TestIamPermissions` method.
+                The request object. Request message for ``TestIamPermissions`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
                 the operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/client.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1015,18 +1015,18 @@
 
         Args:
             request (Union[google.cloud.resourcemanager_v3.types.UpdateProjectRequest, dict]):
                 The request object. The request sent to the
                 [UpdateProject][google.cloud.resourcemanager.v3.Projects.UpdateProject]
                 method.
 
-                Only the `display_name` and `labels` fields can be
+                Only the ``display_name`` and ``labels`` fields can be
                 change. Use the
                 [MoveProject][google.cloud.resourcemanager.v3.Projects.MoveProject]
-                method to change the `parent` field.
+                method to change the ``parent`` field.
             project (google.cloud.resourcemanager_v3.types.Project):
                 Required. The new definition of the
                 project.
 
                 This corresponds to the ``project`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -1443,16 +1443,15 @@
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.resourcemanager_v3.types.UndeleteProjectRequest, dict]):
-                The request object. The request sent to the
-                [UndeleteProject]
+                The request object. The request sent to the [UndeleteProject]
                 [google.cloud.resourcemanager.v3.Projects.UndeleteProject]
                 method.
             name (str):
                 Required. The name of the project (for example,
                 ``projects/415104041262``).
 
                 Required.
@@ -1563,16 +1562,15 @@
                 response = client.get_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]):
-                The request object. Request message for `GetIamPolicy`
-                method.
+                The request object. Request message for ``GetIamPolicy`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1777,16 +1775,15 @@
                 response = client.set_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]):
-                The request object. Request message for `SetIamPolicy`
-                method.
+                The request object. Request message for ``SetIamPolicy`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1943,16 +1940,15 @@
                 response = client.test_iam_permissions(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]):
-                The request object. Request message for
-                `TestIamPermissions` method.
+                The request object. Request message for ``TestIamPermissions`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
                 the operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/pagers.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/transports/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/transports/base.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/transports/grpc.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/transports/grpc_asyncio.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/projects/transports/rest.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/projects/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -565,15 +565,14 @@
             r"""Call the create project method over HTTP.
 
             Args:
                 request (~.projects.CreateProjectRequest):
                     The request object. The request sent to the
                 [CreateProject][google.cloud.resourcemanager.v3.Projects.CreateProject]
                 method.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -663,15 +662,14 @@
         ) -> operations_pb2.Operation:
             r"""Call the delete project method over HTTP.
 
             Args:
                 request (~.projects.DeleteProjectRequest):
                     The request object. [DeleteProject][google.cloud.resourcemanager.v3.Projects.DeleteProject]
                 method.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -802,15 +800,16 @@
                           "role": "roles/resourcemanager.organizationViewer",
                           "members": [
                             "user:eve@example.com"
                           ],
                           "condition": {
                             "title": "expirable access",
                             "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time < timestamp('2020-10-01T00:00:00.000Z')",
+                            "expression": "request.time <
+                            timestamp('2020-10-01T00:00:00.000Z')",
                           }
                         }
                       ],
                       "etag": "BwWWja0YfJA=",
                       "version": 3
                     }
 
@@ -922,15 +921,14 @@
             r"""Call the get project method over HTTP.
 
             Args:
                 request (~.projects.GetProjectRequest):
                     The request object. The request sent to the
                 [GetProject][google.cloud.resourcemanager.v3.Projects.GetProject]
                 method.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1017,15 +1015,14 @@
             r"""Call the list projects method over HTTP.
 
             Args:
                 request (~.projects.ListProjectsRequest):
                     The request object. The request sent to the
                 [ListProjects][google.cloud.resourcemanager.v3.Projects.ListProjects]
                 method.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1117,15 +1114,14 @@
             r"""Call the move project method over HTTP.
 
             Args:
                 request (~.projects.MoveProjectRequest):
                     The request object. The request sent to
                 [MoveProject][google.cloud.resourcemanager.v3.Projects.MoveProject]
                 method.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1206,15 +1202,14 @@
             r"""Call the search projects method over HTTP.
 
             Args:
                 request (~.projects.SearchProjectsRequest):
                     The request object. The request sent to the
                 [SearchProjects][google.cloud.resourcemanager.v3.Projects.SearchProjects]
                 method.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1350,15 +1345,16 @@
                           "role": "roles/resourcemanager.organizationViewer",
                           "members": [
                             "user:eve@example.com"
                           ],
                           "condition": {
                             "title": "expirable access",
                             "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time < timestamp('2020-10-01T00:00:00.000Z')",
+                            "expression": "request.time <
+                            timestamp('2020-10-01T00:00:00.000Z')",
                           }
                         }
                       ],
                       "etag": "BwWWja0YfJA=",
                       "version": 3
                     }
 
@@ -1567,15 +1563,14 @@
             r"""Call the undelete project method over HTTP.
 
             Args:
                 request (~.projects.UndeleteProjectRequest):
                     The request object. The request sent to the [UndeleteProject]
                 [google.cloud.resourcemanager.v3.Projects.UndeleteProject]
                 method.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1673,15 +1668,14 @@
                 [UpdateProject][google.cloud.resourcemanager.v3.Projects.UpdateProject]
                 method.
 
                 Only the ``display_name`` and ``labels`` fields can be
                 change. Use the
                 [MoveProject][google.cloud.resourcemanager.v3.Projects.MoveProject]
                 method to change the ``parent`` field.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/async_client.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/client.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/pagers.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/transports/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/transports/base.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/transports/grpc.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/transports/grpc_asyncio.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_bindings/transports/rest.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_bindings/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,15 +328,14 @@
         ) -> operations_pb2.Operation:
             r"""Call the create tag binding method over HTTP.
 
             Args:
                 request (~.tag_bindings.CreateTagBindingRequest):
                     The request object. The request message to create a
                 TagBinding.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -428,15 +427,14 @@
         ) -> operations_pb2.Operation:
             r"""Call the delete tag binding method over HTTP.
 
             Args:
                 request (~.tag_bindings.DeleteTagBindingRequest):
                     The request object. The request message to delete a
                 TagBinding.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -521,15 +519,14 @@
         ) -> tag_bindings.ListTagBindingsResponse:
             r"""Call the list tag bindings method over HTTP.
 
             Args:
                 request (~.tag_bindings.ListTagBindingsRequest):
                     The request object. The request message to list all
                 TagBindings for a parent.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/async_client.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -861,16 +861,15 @@
                 response = await client.get_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]]):
-                The request object. Request message for `GetIamPolicy`
-                method.
+                The request object. Request message for ``GetIamPolicy`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1040,16 +1039,15 @@
                 response = await client.set_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]]):
-                The request object. Request message for `SetIamPolicy`
-                method.
+                The request object. Request message for ``SetIamPolicy`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1212,16 +1210,15 @@
                 response = await client.test_iam_permissions(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]]):
-                The request object. Request message for
-                `TestIamPermissions` method.
+                The request object. Request message for ``TestIamPermissions`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
                 the operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/client.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1071,16 +1071,15 @@
                 response = client.get_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]):
-                The request object. Request message for `GetIamPolicy`
-                method.
+                The request object. Request message for ``GetIamPolicy`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1238,16 +1237,15 @@
                 response = client.set_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]):
-                The request object. Request message for `SetIamPolicy`
-                method.
+                The request object. Request message for ``SetIamPolicy`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1407,16 +1405,15 @@
                 response = client.test_iam_permissions(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]):
-                The request object. Request message for
-                `TestIamPermissions` method.
+                The request object. Request message for ``TestIamPermissions`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
                 the operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/pagers.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/transports/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/transports/base.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/transports/grpc.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/transports/grpc_asyncio.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_keys/transports/rest.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_keys/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,15 +467,14 @@
         ) -> operations_pb2.Operation:
             r"""Call the create tag key method over HTTP.
 
             Args:
                 request (~.tag_keys.CreateTagKeyRequest):
                     The request object. The request message for creating a
                 TagKey.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -565,15 +564,14 @@
         ) -> operations_pb2.Operation:
             r"""Call the delete tag key method over HTTP.
 
             Args:
                 request (~.tag_keys.DeleteTagKeyRequest):
                     The request object. The request message for deleting a
                 TagKey.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -704,15 +702,16 @@
                           "role": "roles/resourcemanager.organizationViewer",
                           "members": [
                             "user:eve@example.com"
                           ],
                           "condition": {
                             "title": "expirable access",
                             "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time < timestamp('2020-10-01T00:00:00.000Z')",
+                            "expression": "request.time <
+                            timestamp('2020-10-01T00:00:00.000Z')",
                           }
                         }
                       ],
                       "etag": "BwWWja0YfJA=",
                       "version": 3
                     }
 
@@ -823,15 +822,14 @@
         ) -> tag_keys.TagKey:
             r"""Call the get tag key method over HTTP.
 
             Args:
                 request (~.tag_keys.GetTagKeyRequest):
                     The request object. The request message for getting a
                 TagKey.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -915,15 +913,14 @@
         ) -> tag_keys.ListTagKeysResponse:
             r"""Call the list tag keys method over HTTP.
 
             Args:
                 request (~.tag_keys.ListTagKeysRequest):
                     The request object. The request message for listing all
                 TagKeys under a parent resource.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1053,15 +1050,16 @@
                           "role": "roles/resourcemanager.organizationViewer",
                           "members": [
                             "user:eve@example.com"
                           ],
                           "condition": {
                             "title": "expirable access",
                             "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time < timestamp('2020-10-01T00:00:00.000Z')",
+                            "expression": "request.time <
+                            timestamp('2020-10-01T00:00:00.000Z')",
                           }
                         }
                       ],
                       "etag": "BwWWja0YfJA=",
                       "version": 3
                     }
 
@@ -1269,15 +1267,14 @@
         ) -> operations_pb2.Operation:
             r"""Call the update tag key method over HTTP.
 
             Args:
                 request (~.tag_keys.UpdateTagKeyRequest):
                     The request object. The request message for updating a
                 TagKey.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/async_client.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -861,16 +861,15 @@
                 response = await client.get_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]]):
-                The request object. Request message for `GetIamPolicy`
-                method.
+                The request object. Request message for ``GetIamPolicy`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1040,16 +1039,15 @@
                 response = await client.set_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]]):
-                The request object. Request message for `SetIamPolicy`
-                method.
+                The request object. Request message for ``SetIamPolicy`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1212,16 +1210,15 @@
                 response = await client.test_iam_permissions(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]]):
-                The request object. Request message for
-                `TestIamPermissions` method.
+                The request object. Request message for ``TestIamPermissions`` method.
             resource (:class:`str`):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
                 the operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/client.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1069,16 +1069,15 @@
                 response = client.get_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.GetIamPolicyRequest, dict]):
-                The request object. Request message for `GetIamPolicy`
-                method.
+                The request object. Request message for ``GetIamPolicy`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being requested. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1236,16 +1235,15 @@
                 response = client.set_iam_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.SetIamPolicyRequest, dict]):
-                The request object. Request message for `SetIamPolicy`
-                method.
+                The request object. Request message for ``SetIamPolicy`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy is being specified. See the
                 operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
@@ -1405,16 +1403,15 @@
                 response = client.test_iam_permissions(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.iam.v1.iam_policy_pb2.TestIamPermissionsRequest, dict]):
-                The request object. Request message for
-                `TestIamPermissions` method.
+                The request object. Request message for ``TestIamPermissions`` method.
             resource (str):
                 REQUIRED: The resource for which the
                 policy detail is being requested. See
                 the operation documentation for the
                 appropriate value for this field.
 
                 This corresponds to the ``resource`` field
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/pagers.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/transports/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/transports/base.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/transports/grpc.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/transports/grpc_asyncio.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/services/tag_values/transports/rest.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/services/tag_values/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,15 +477,14 @@
         ) -> operations_pb2.Operation:
             r"""Call the create tag value method over HTTP.
 
             Args:
                 request (~.tag_values.CreateTagValueRequest):
                     The request object. The request message for creating a
                 TagValue.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -577,15 +576,14 @@
         ) -> operations_pb2.Operation:
             r"""Call the delete tag value method over HTTP.
 
             Args:
                 request (~.tag_values.DeleteTagValueRequest):
                     The request object. The request message for deleting a
                 TagValue.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -718,15 +716,16 @@
                           "role": "roles/resourcemanager.organizationViewer",
                           "members": [
                             "user:eve@example.com"
                           ],
                           "condition": {
                             "title": "expirable access",
                             "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time < timestamp('2020-10-01T00:00:00.000Z')",
+                            "expression": "request.time <
+                            timestamp('2020-10-01T00:00:00.000Z')",
                           }
                         }
                       ],
                       "etag": "BwWWja0YfJA=",
                       "version": 3
                     }
 
@@ -837,15 +836,14 @@
         ) -> tag_values.TagValue:
             r"""Call the get tag value method over HTTP.
 
             Args:
                 request (~.tag_values.GetTagValueRequest):
                     The request object. The request message for getting a
                 TagValue.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -931,15 +929,14 @@
         ) -> tag_values.ListTagValuesResponse:
             r"""Call the list tag values method over HTTP.
 
             Args:
                 request (~.tag_values.ListTagValuesRequest):
                     The request object. The request message for listing
                 TagValues for the specified TagKey.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1069,15 +1066,16 @@
                           "role": "roles/resourcemanager.organizationViewer",
                           "members": [
                             "user:eve@example.com"
                           ],
                           "condition": {
                             "title": "expirable access",
                             "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time < timestamp('2020-10-01T00:00:00.000Z')",
+                            "expression": "request.time <
+                            timestamp('2020-10-01T00:00:00.000Z')",
                           }
                         }
                       ],
                       "etag": "BwWWja0YfJA=",
                       "version": 3
                     }
 
@@ -1285,15 +1283,14 @@
         ) -> operations_pb2.Operation:
             r"""Call the update tag value method over HTTP.
 
             Args:
                 request (~.tag_values.UpdateTagValueRequest):
                     The request object. The request message for updating a
                 TagValue.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
```

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/__init__.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/folders.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/folders.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/organizations.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/organizations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/projects.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/projects.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/tag_bindings.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/tag_bindings.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/tag_keys.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/tag_keys.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google/cloud/resourcemanager_v3/types/tag_values.py` & `google-cloud-resource-manager-1.9.1/google/cloud/resourcemanager_v3/types/tag_values.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/google_cloud_resource_manager.egg-info/PKG-INFO` & `google-cloud-resource-manager-1.9.1/google_cloud_resource_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-resource-manager
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Resource Manager API client library
 Home-page: https://github.com/googleapis/python-resource-manager
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-resource-manager-1.9.0/google_cloud_resource_manager.egg-info/SOURCES.txt` & `google-cloud-resource-manager-1.9.1/google_cloud_resource_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/setup.py` & `google-cloud-resource-manager-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     release_status = "Development Status :: 5 - Production/Stable"
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
-    "grpc-google-iam-v1 >= 0.12.4, < 1.0.0dev",
+    "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
 url = "https://github.com/googleapis/python-resource-manager"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
```

### Comparing `google-cloud-resource-manager-1.9.0/tests/__init__.py` & `google-cloud-resource-manager-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/tests/unit/__init__.py` & `google-cloud-resource-manager-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-resource-manager-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/__init__.py` & `google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/test_folders.py` & `google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/test_folders.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/test_organizations.py` & `google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/test_organizations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/test_projects.py` & `google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/test_projects.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/test_tag_bindings.py` & `google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/test_tag_bindings.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/test_tag_keys.py` & `google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/test_tag_keys.py`

 * *Files identical despite different names*

### Comparing `google-cloud-resource-manager-1.9.0/tests/unit/gapic/resourcemanager_v3/test_tag_values.py` & `google-cloud-resource-manager-1.9.1/tests/unit/gapic/resourcemanager_v3/test_tag_values.py`

 * *Files identical despite different names*

