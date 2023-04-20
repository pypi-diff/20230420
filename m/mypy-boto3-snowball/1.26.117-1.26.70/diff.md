# Comparing `tmp/mypy-boto3-snowball-1.26.117.tar.gz` & `tmp/mypy-boto3-snowball-1.26.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-snowball-1.26.117.tar", last modified: Thu Apr 20 19:33:50 2023, max compression
+gzip compressed data, was "mypy-boto3-snowball-1.26.70.tar", last modified: Mon Feb 13 20:27:09 2023, max compression
```

## Comparing `mypy-boto3-snowball-1.26.117.tar` & `mypy-boto3-snowball-1.26.70.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:50.611274 mypy-boto3-snowball-1.26.117/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 19:33:26.000000 mypy-boto3-snowball-1.26.117/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16794 2023-04-20 19:33:50.611274 mypy-boto3-snowball-1.26.117/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15301 2023-04-20 19:33:26.000000 mypy-boto3-snowball-1.26.117/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:50.611274 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-20 19:33:26.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-20 19:33:26.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-20 19:33:26.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23506 2023-04-20 19:33:26.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23467 2023-04-20 19:33:26.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-04-20 19:33:26.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-04-20 19:33:26.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-04-20 19:33:26.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-04-20 19:33:26.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:26.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27556 2023-04-20 19:33:27.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27535 2023-04-20 19:33:27.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 19:33:26.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:50.611274 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16794 2023-04-20 19:33:50.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-20 19:33:50.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:33:50.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:33:50.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 19:33:50.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 19:33:50.000000 mypy-boto3-snowball-1.26.117/mypy_boto3_snowball.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:33:50.611274 mypy-boto3-snowball-1.26.117/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-20 19:33:26.000000 mypy-boto3-snowball-1.26.117/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:27:09.130620 mypy-boto3-snowball-1.26.70/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-02-13 20:27:09.130620 mypy-boto3-snowball-1.26.70/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15277 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:27:09.130620 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23307 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26960 2023-02-13 20:27:00.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26939 2023-02-13 20:27:00.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:27:09.130620 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-02-13 20:27:09.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-13 20:27:09.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 20:27:09.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 20:27:09.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-13 20:27:09.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-13 20:27:09.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 20:27:09.130620 mypy-boto3-snowball-1.26.70/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/setup.py
```

### Comparing `mypy-boto3-snowball-1.26.117/LICENSE` & `mypy-boto3-snowball-1.26.70/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-snowball-1.26.117/PKG-INFO` & `mypy-boto3-snowball-1.26.70/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-snowball
-Version: 1.26.117
-Summary: Type annotations for boto3.Snowball 1.26.117 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.70
+Summary: Type annotations for boto3.Snowball 1.26.70 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-snowball"></a>
 
 # mypy-boto3-snowball
 
 [![PyPI - mypy-boto3-snowball](https://img.shields.io/pypi/v/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.26.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,15 +362,14 @@
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
     NotificationTypeDef,
     CompatibleImageTypeDef,
     ResponseMetadataTypeDef,
-    JobListEntryTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
     DataTransferTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeAddressesRequestRequestTypeDef,
@@ -380,56 +379,56 @@
     EKSOnDeviceServiceConfigurationTypeDef,
     Ec2AmiResourceTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
     INDTaxDocumentsTypeDef,
+    JobListEntryTypeDef,
     JobLogsTypeDef,
     KeyRangeTypeDef,
     ListClusterJobsRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
-    S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
     CreateAddressRequestRequestTypeDef,
     CreateAddressResultTypeDef,
+    CreateClusterResultTypeDef,
     CreateJobResultTypeDef,
     CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
     DescribeReturnShippingLabelResultTypeDef,
     GetJobManifestResultTypeDef,
     GetJobUnlockCodeResultTypeDef,
     GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
-    CreateClusterResultTypeDef,
-    ListClusterJobsResultTypeDef,
-    ListJobsResultTypeDef,
     DependentServiceTypeDef,
     DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     LambdaResourceTypeDef,
     TaxDocumentsTypeDef,
+    ListClusterJobsResultTypeDef,
+    ListJobsResultTypeDef,
     ListLongTermPricingResultTypeDef,
     OnDeviceServiceConfigurationTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
     SnowconeDeviceConfigurationTypeDef,
     ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
@@ -453,42 +452,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-snowball-1.26.117/README.md` & `mypy-boto3-snowball-1.26.70/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-snowball"></a>
 
 # mypy-boto3-snowball
 
 [![PyPI - mypy-boto3-snowball](https://img.shields.io/pypi/v/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.26.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,15 +330,14 @@
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
     NotificationTypeDef,
     CompatibleImageTypeDef,
     ResponseMetadataTypeDef,
-    JobListEntryTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
     DataTransferTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeAddressesRequestRequestTypeDef,
@@ -348,56 +347,56 @@
     EKSOnDeviceServiceConfigurationTypeDef,
     Ec2AmiResourceTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
     INDTaxDocumentsTypeDef,
+    JobListEntryTypeDef,
     JobLogsTypeDef,
     KeyRangeTypeDef,
     ListClusterJobsRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
-    S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
     CreateAddressRequestRequestTypeDef,
     CreateAddressResultTypeDef,
+    CreateClusterResultTypeDef,
     CreateJobResultTypeDef,
     CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
     DescribeReturnShippingLabelResultTypeDef,
     GetJobManifestResultTypeDef,
     GetJobUnlockCodeResultTypeDef,
     GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
-    CreateClusterResultTypeDef,
-    ListClusterJobsResultTypeDef,
-    ListJobsResultTypeDef,
     DependentServiceTypeDef,
     DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     LambdaResourceTypeDef,
     TaxDocumentsTypeDef,
+    ListClusterJobsResultTypeDef,
+    ListJobsResultTypeDef,
     ListLongTermPricingResultTypeDef,
     OnDeviceServiceConfigurationTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
     SnowconeDeviceConfigurationTypeDef,
     ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
@@ -421,42 +420,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/__init__.py` & `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/__init__.pyi` & `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/__main__.py` & `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Snowball 1.26.117\nVersion:         1.26.117\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Snowball 1.26.70\nVersion:         1.26.70\nBuilder version:"
+        " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.117")
+    print("1.26.70")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/client.py` & `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,30 +155,26 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_address)
         """
 
     def create_cluster(
         self,
         *,
         JobType: JobTypeType,
+        Resources: JobResourceTypeDef,
         AddressId: str,
+        RoleARN: str,
         SnowballType: SnowballTypeType,
         ShippingOption: ShippingOptionType,
-        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         KmsKeyARN: str = ...,
-        RoleARN: str = ...,
         Notification: NotificationTypeDef = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
-        RemoteManagement: RemoteManagementType = ...,
-        InitialClusterSize: int = ...,
-        ForceCreateJobs: bool = ...,
-        LongTermPricingIds: Sequence[str] = ...,
-        SnowballCapacityPreference: SnowballCapacityType = ...
+        RemoteManagement: RemoteManagementType = ...
     ) -> CreateClusterResultTypeDef:
         """
         Creates an empty cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_cluster)
         """
@@ -324,15 +320,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.get_snowball_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#get_snowball_usage)
         """
 
     def get_software_updates(self, *, JobId: str) -> GetSoftwareUpdatesResultTypeDef:
         """
         Returns an Amazon S3 presigned URL for an update file associated with a
-        specified `JobId`.
+        specified `JobId` .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.get_software_updates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#get_software_updates)
         """
 
     def list_cluster_jobs(
         self, *, ClusterId: str, MaxResults: int = ..., NextToken: str = ...
@@ -431,15 +427,15 @@
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Description: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ForwardingAddressId: str = ...
     ) -> Dict[str, Any]:
         """
-        While a job's `JobState` value is `New`, you can update some of the information
+        While a job's `JobState` value is `New` , you can update some of the information
         associated with a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#update_job)
         """
 
     def update_job_shipment_state(
```

### Comparing `mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/client.pyi` & `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -145,30 +145,26 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_address)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_address)
         """
     def create_cluster(
         self,
         *,
         JobType: JobTypeType,
+        Resources: JobResourceTypeDef,
         AddressId: str,
+        RoleARN: str,
         SnowballType: SnowballTypeType,
         ShippingOption: ShippingOptionType,
-        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         KmsKeyARN: str = ...,
-        RoleARN: str = ...,
         Notification: NotificationTypeDef = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
-        RemoteManagement: RemoteManagementType = ...,
-        InitialClusterSize: int = ...,
-        ForceCreateJobs: bool = ...,
-        LongTermPricingIds: Sequence[str] = ...,
-        SnowballCapacityPreference: SnowballCapacityType = ...
+        RemoteManagement: RemoteManagementType = ...
     ) -> CreateClusterResultTypeDef:
         """
         Creates an empty cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_cluster)
         """
@@ -301,15 +297,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.get_snowball_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#get_snowball_usage)
         """
     def get_software_updates(self, *, JobId: str) -> GetSoftwareUpdatesResultTypeDef:
         """
         Returns an Amazon S3 presigned URL for an update file associated with a
-        specified `JobId`.
+        specified `JobId` .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.get_software_updates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#get_software_updates)
         """
     def list_cluster_jobs(
         self, *, ClusterId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListClusterJobsResultTypeDef:
@@ -400,15 +396,15 @@
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Description: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ForwardingAddressId: str = ...
     ) -> Dict[str, Any]:
         """
-        While a job's `JobState` value is `New`, you can update some of the information
+        While a job's `JobState` value is `New` , you can update some of the information
         associated with a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#update_job)
         """
     def update_job_shipment_state(
         self, *, JobId: str, ShipmentState: ShipmentStateType
```

### Comparing `mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/literals.py` & `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,25 +68,25 @@
 ]
 JobTypeType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 ListClusterJobsPaginatorName = Literal["list_cluster_jobs"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListCompatibleImagesPaginatorName = Literal["list_compatible_images"]
 ListJobsPaginatorName = Literal["list_jobs"]
 ListLongTermPricingPaginatorName = Literal["list_long_term_pricing"]
-LongTermPricingTypeType = Literal["OneMonth", "OneYear", "ThreeYear"]
+LongTermPricingTypeType = Literal["OneYear", "ThreeYear"]
 RemoteManagementType = Literal["INSTALLED_AUTOSTART", "INSTALLED_ONLY"]
 ServiceNameType = Literal["EKS_ANYWHERE", "KUBERNETES"]
 ShipmentStateType = Literal["RECEIVED", "RETURNED"]
 ShippingLabelStatusType = Literal["Failed", "InProgress", "Succeeded", "TimedOut"]
 ShippingOptionType = Literal["EXPRESS", "NEXT_DAY", "SECOND_DAY", "STANDARD"]
 SnowballCapacityType = Literal[
-    "NoPreference", "T100", "T14", "T240", "T32", "T42", "T50", "T8", "T80", "T98"
+    "NoPreference", "T100", "T14", "T32", "T42", "T50", "T8", "T80", "T98"
 ]
 SnowballTypeType = Literal[
-    "EDGE", "EDGE_C", "EDGE_CG", "EDGE_S", "SNC1_HDD", "SNC1_SSD", "STANDARD", "V3_5C", "V3_5S"
+    "EDGE", "EDGE_C", "EDGE_CG", "EDGE_S", "SNC1_HDD", "SNC1_SSD", "STANDARD", "V3_5C"
 ]
 StorageUnitType = Literal["TB"]
 TransferOptionType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 SnowballServiceName = Literal["snowball"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -231,15 +231,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -250,15 +249,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -409,20 +407,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -465,14 +461,13 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
-    "me-central-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/literals.pyi` & `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -66,25 +66,25 @@
 ]
 JobTypeType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 ListClusterJobsPaginatorName = Literal["list_cluster_jobs"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListCompatibleImagesPaginatorName = Literal["list_compatible_images"]
 ListJobsPaginatorName = Literal["list_jobs"]
 ListLongTermPricingPaginatorName = Literal["list_long_term_pricing"]
-LongTermPricingTypeType = Literal["OneMonth", "OneYear", "ThreeYear"]
+LongTermPricingTypeType = Literal["OneYear", "ThreeYear"]
 RemoteManagementType = Literal["INSTALLED_AUTOSTART", "INSTALLED_ONLY"]
 ServiceNameType = Literal["EKS_ANYWHERE", "KUBERNETES"]
 ShipmentStateType = Literal["RECEIVED", "RETURNED"]
 ShippingLabelStatusType = Literal["Failed", "InProgress", "Succeeded", "TimedOut"]
 ShippingOptionType = Literal["EXPRESS", "NEXT_DAY", "SECOND_DAY", "STANDARD"]
 SnowballCapacityType = Literal[
-    "NoPreference", "T100", "T14", "T240", "T32", "T42", "T50", "T8", "T80", "T98"
+    "NoPreference", "T100", "T14", "T32", "T42", "T50", "T8", "T80", "T98"
 ]
 SnowballTypeType = Literal[
-    "EDGE", "EDGE_C", "EDGE_CG", "EDGE_S", "SNC1_HDD", "SNC1_SSD", "STANDARD", "V3_5C", "V3_5S"
+    "EDGE", "EDGE_C", "EDGE_CG", "EDGE_S", "SNC1_HDD", "SNC1_SSD", "STANDARD", "V3_5C"
 ]
 StorageUnitType = Literal["TB"]
 TransferOptionType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 SnowballServiceName = Literal["snowball"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -229,15 +229,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -248,15 +247,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -407,20 +405,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -463,14 +459,13 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
-    "me-central-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/paginator.py` & `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/paginator.pyi` & `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/type_defs.py` & `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
     "NotificationTypeDef",
     "CompatibleImageTypeDef",
     "ResponseMetadataTypeDef",
-    "JobListEntryTypeDef",
     "CreateLongTermPricingRequestRequestTypeDef",
     "CreateReturnShippingLabelRequestRequestTypeDef",
     "DataTransferTypeDef",
     "ServiceVersionTypeDef",
     "DescribeAddressRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeAddressesRequestRequestTypeDef",
@@ -63,56 +62,56 @@
     "EKSOnDeviceServiceConfigurationTypeDef",
     "Ec2AmiResourceTypeDef",
     "EventTriggerDefinitionTypeDef",
     "GetJobManifestRequestRequestTypeDef",
     "GetJobUnlockCodeRequestRequestTypeDef",
     "GetSoftwareUpdatesRequestRequestTypeDef",
     "INDTaxDocumentsTypeDef",
+    "JobListEntryTypeDef",
     "JobLogsTypeDef",
     "KeyRangeTypeDef",
     "ListClusterJobsRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListCompatibleImagesRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListLongTermPricingRequestRequestTypeDef",
     "LongTermPricingListEntryTypeDef",
     "NFSOnDeviceServiceConfigurationTypeDef",
-    "S3OnDeviceServiceConfigurationTypeDef",
     "TGWOnDeviceServiceConfigurationTypeDef",
     "TargetOnDeviceServiceTypeDef",
     "ShipmentTypeDef",
     "WirelessConnectionTypeDef",
     "UpdateJobShipmentStateRequestRequestTypeDef",
     "UpdateLongTermPricingRequestRequestTypeDef",
     "CreateAddressRequestRequestTypeDef",
     "CreateAddressResultTypeDef",
+    "CreateClusterResultTypeDef",
     "CreateJobResultTypeDef",
     "CreateLongTermPricingResultTypeDef",
     "CreateReturnShippingLabelResultTypeDef",
     "DescribeAddressResultTypeDef",
     "DescribeAddressesResultTypeDef",
     "DescribeReturnShippingLabelResultTypeDef",
     "GetJobManifestResultTypeDef",
     "GetJobUnlockCodeResultTypeDef",
     "GetSnowballUsageResultTypeDef",
     "GetSoftwareUpdatesResultTypeDef",
     "ListClustersResultTypeDef",
     "ListCompatibleImagesResultTypeDef",
-    "CreateClusterResultTypeDef",
-    "ListClusterJobsResultTypeDef",
-    "ListJobsResultTypeDef",
     "DependentServiceTypeDef",
     "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "LambdaResourceTypeDef",
     "TaxDocumentsTypeDef",
+    "ListClusterJobsResultTypeDef",
+    "ListJobsResultTypeDef",
     "ListLongTermPricingResultTypeDef",
     "OnDeviceServiceConfigurationTypeDef",
     "S3ResourceTypeDef",
     "ShippingDetailsTypeDef",
     "SnowconeDeviceConfigurationTypeDef",
     "ListServiceVersionsRequestRequestTypeDef",
     "ListServiceVersionsResultTypeDef",
@@ -200,28 +199,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-JobListEntryTypeDef = TypedDict(
-    "JobListEntryTypeDef",
-    {
-        "JobId": str,
-        "JobState": JobStateType,
-        "IsMaster": bool,
-        "JobType": JobTypeType,
-        "SnowballType": SnowballTypeType,
-        "CreationDate": datetime,
-        "Description": str,
-    },
-    total=False,
-)
-
 _RequiredCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLongTermPricingRequestRequestTypeDef",
     {
         "LongTermPricingType": LongTermPricingTypeType,
     },
 )
 _OptionalCreateLongTermPricingRequestRequestTypeDef = TypedDict(
@@ -390,14 +375,28 @@
     "INDTaxDocumentsTypeDef",
     {
         "GSTIN": str,
     },
     total=False,
 )
 
+JobListEntryTypeDef = TypedDict(
+    "JobListEntryTypeDef",
+    {
+        "JobId": str,
+        "JobState": JobStateType,
+        "IsMaster": bool,
+        "JobType": JobTypeType,
+        "SnowballType": SnowballTypeType,
+        "CreationDate": datetime,
+        "Description": str,
+    },
+    total=False,
+)
+
 JobLogsTypeDef = TypedDict(
     "JobLogsTypeDef",
     {
         "JobCompletionReportURI": str,
         "JobSuccessLogURI": str,
         "JobFailureLogURI": str,
     },
@@ -493,25 +492,14 @@
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
 )
 
-S3OnDeviceServiceConfigurationTypeDef = TypedDict(
-    "S3OnDeviceServiceConfigurationTypeDef",
-    {
-        "StorageLimit": float,
-        "StorageUnit": Literal["TB"],
-        "ServiceSize": int,
-        "FaultTolerance": int,
-    },
-    total=False,
-)
-
 TGWOnDeviceServiceConfigurationTypeDef = TypedDict(
     "TGWOnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
@@ -585,14 +573,22 @@
     "CreateAddressResultTypeDef",
     {
         "AddressId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateClusterResultTypeDef = TypedDict(
+    "CreateClusterResultTypeDef",
+    {
+        "ClusterId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateJobResultTypeDef = TypedDict(
     "CreateJobResultTypeDef",
     {
         "JobId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -687,41 +683,14 @@
     {
         "CompatibleImages": List[CompatibleImageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateClusterResultTypeDef = TypedDict(
-    "CreateClusterResultTypeDef",
-    {
-        "ClusterId": str,
-        "JobListEntries": List[JobListEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListClusterJobsResultTypeDef = TypedDict(
-    "ListClusterJobsResultTypeDef",
-    {
-        "JobListEntries": List[JobListEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListJobsResultTypeDef = TypedDict(
-    "ListJobsResultTypeDef",
-    {
-        "JobListEntries": List[JobListEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DependentServiceTypeDef = TypedDict(
     "DependentServiceTypeDef",
     {
         "ServiceName": ServiceNameType,
         "ServiceVersion": ServiceVersionTypeDef,
     },
     total=False,
@@ -802,14 +771,32 @@
     "TaxDocumentsTypeDef",
     {
         "IND": INDTaxDocumentsTypeDef,
     },
     total=False,
 )
 
+ListClusterJobsResultTypeDef = TypedDict(
+    "ListClusterJobsResultTypeDef",
+    {
+        "JobListEntries": List[JobListEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListJobsResultTypeDef = TypedDict(
+    "ListJobsResultTypeDef",
+    {
+        "JobListEntries": List[JobListEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListLongTermPricingResultTypeDef = TypedDict(
     "ListLongTermPricingResultTypeDef",
     {
         "LongTermPricingEntries": List[LongTermPricingListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -817,15 +804,14 @@
 
 OnDeviceServiceConfigurationTypeDef = TypedDict(
     "OnDeviceServiceConfigurationTypeDef",
     {
         "NFSOnDeviceService": NFSOnDeviceServiceConfigurationTypeDef,
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationTypeDef,
         "EKSOnDeviceService": EKSOnDeviceServiceConfigurationTypeDef,
-        "S3OnDeviceService": S3OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
 S3ResourceTypeDef = TypedDict(
     "S3ResourceTypeDef",
     {
@@ -929,35 +915,31 @@
     total=False,
 )
 
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "JobType": JobTypeType,
+        "Resources": JobResourceTypeDef,
         "AddressId": str,
+        "RoleARN": str,
         "SnowballType": SnowballTypeType,
         "ShippingOption": ShippingOptionType,
     },
 )
 _OptionalCreateClusterRequestRequestTypeDef = TypedDict(
     "_OptionalCreateClusterRequestRequestTypeDef",
     {
-        "Resources": JobResourceTypeDef,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
         "Description": str,
         "KmsKeyARN": str,
-        "RoleARN": str,
         "Notification": NotificationTypeDef,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "RemoteManagement": RemoteManagementType,
-        "InitialClusterSize": int,
-        "ForceCreateJobs": bool,
-        "LongTermPricingIds": Sequence[str],
-        "SnowballCapacityPreference": SnowballCapacityType,
     },
     total=False,
 )
 
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
```

### Comparing `mypy-boto3-snowball-1.26.117/mypy_boto3_snowball/type_defs.pyi` & `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
     "NotificationTypeDef",
     "CompatibleImageTypeDef",
     "ResponseMetadataTypeDef",
-    "JobListEntryTypeDef",
     "CreateLongTermPricingRequestRequestTypeDef",
     "CreateReturnShippingLabelRequestRequestTypeDef",
     "DataTransferTypeDef",
     "ServiceVersionTypeDef",
     "DescribeAddressRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeAddressesRequestRequestTypeDef",
@@ -62,56 +61,56 @@
     "EKSOnDeviceServiceConfigurationTypeDef",
     "Ec2AmiResourceTypeDef",
     "EventTriggerDefinitionTypeDef",
     "GetJobManifestRequestRequestTypeDef",
     "GetJobUnlockCodeRequestRequestTypeDef",
     "GetSoftwareUpdatesRequestRequestTypeDef",
     "INDTaxDocumentsTypeDef",
+    "JobListEntryTypeDef",
     "JobLogsTypeDef",
     "KeyRangeTypeDef",
     "ListClusterJobsRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListCompatibleImagesRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListLongTermPricingRequestRequestTypeDef",
     "LongTermPricingListEntryTypeDef",
     "NFSOnDeviceServiceConfigurationTypeDef",
-    "S3OnDeviceServiceConfigurationTypeDef",
     "TGWOnDeviceServiceConfigurationTypeDef",
     "TargetOnDeviceServiceTypeDef",
     "ShipmentTypeDef",
     "WirelessConnectionTypeDef",
     "UpdateJobShipmentStateRequestRequestTypeDef",
     "UpdateLongTermPricingRequestRequestTypeDef",
     "CreateAddressRequestRequestTypeDef",
     "CreateAddressResultTypeDef",
+    "CreateClusterResultTypeDef",
     "CreateJobResultTypeDef",
     "CreateLongTermPricingResultTypeDef",
     "CreateReturnShippingLabelResultTypeDef",
     "DescribeAddressResultTypeDef",
     "DescribeAddressesResultTypeDef",
     "DescribeReturnShippingLabelResultTypeDef",
     "GetJobManifestResultTypeDef",
     "GetJobUnlockCodeResultTypeDef",
     "GetSnowballUsageResultTypeDef",
     "GetSoftwareUpdatesResultTypeDef",
     "ListClustersResultTypeDef",
     "ListCompatibleImagesResultTypeDef",
-    "CreateClusterResultTypeDef",
-    "ListClusterJobsResultTypeDef",
-    "ListJobsResultTypeDef",
     "DependentServiceTypeDef",
     "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "LambdaResourceTypeDef",
     "TaxDocumentsTypeDef",
+    "ListClusterJobsResultTypeDef",
+    "ListJobsResultTypeDef",
     "ListLongTermPricingResultTypeDef",
     "OnDeviceServiceConfigurationTypeDef",
     "S3ResourceTypeDef",
     "ShippingDetailsTypeDef",
     "SnowconeDeviceConfigurationTypeDef",
     "ListServiceVersionsRequestRequestTypeDef",
     "ListServiceVersionsResultTypeDef",
@@ -199,28 +198,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-JobListEntryTypeDef = TypedDict(
-    "JobListEntryTypeDef",
-    {
-        "JobId": str,
-        "JobState": JobStateType,
-        "IsMaster": bool,
-        "JobType": JobTypeType,
-        "SnowballType": SnowballTypeType,
-        "CreationDate": datetime,
-        "Description": str,
-    },
-    total=False,
-)
-
 _RequiredCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLongTermPricingRequestRequestTypeDef",
     {
         "LongTermPricingType": LongTermPricingTypeType,
     },
 )
 _OptionalCreateLongTermPricingRequestRequestTypeDef = TypedDict(
@@ -383,14 +368,28 @@
     "INDTaxDocumentsTypeDef",
     {
         "GSTIN": str,
     },
     total=False,
 )
 
+JobListEntryTypeDef = TypedDict(
+    "JobListEntryTypeDef",
+    {
+        "JobId": str,
+        "JobState": JobStateType,
+        "IsMaster": bool,
+        "JobType": JobTypeType,
+        "SnowballType": SnowballTypeType,
+        "CreationDate": datetime,
+        "Description": str,
+    },
+    total=False,
+)
+
 JobLogsTypeDef = TypedDict(
     "JobLogsTypeDef",
     {
         "JobCompletionReportURI": str,
         "JobSuccessLogURI": str,
         "JobFailureLogURI": str,
     },
@@ -484,25 +483,14 @@
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
 )
 
-S3OnDeviceServiceConfigurationTypeDef = TypedDict(
-    "S3OnDeviceServiceConfigurationTypeDef",
-    {
-        "StorageLimit": float,
-        "StorageUnit": Literal["TB"],
-        "ServiceSize": int,
-        "FaultTolerance": int,
-    },
-    total=False,
-)
-
 TGWOnDeviceServiceConfigurationTypeDef = TypedDict(
     "TGWOnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
@@ -574,14 +562,22 @@
     "CreateAddressResultTypeDef",
     {
         "AddressId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateClusterResultTypeDef = TypedDict(
+    "CreateClusterResultTypeDef",
+    {
+        "ClusterId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateJobResultTypeDef = TypedDict(
     "CreateJobResultTypeDef",
     {
         "JobId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -676,41 +672,14 @@
     {
         "CompatibleImages": List[CompatibleImageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateClusterResultTypeDef = TypedDict(
-    "CreateClusterResultTypeDef",
-    {
-        "ClusterId": str,
-        "JobListEntries": List[JobListEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListClusterJobsResultTypeDef = TypedDict(
-    "ListClusterJobsResultTypeDef",
-    {
-        "JobListEntries": List[JobListEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListJobsResultTypeDef = TypedDict(
-    "ListJobsResultTypeDef",
-    {
-        "JobListEntries": List[JobListEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DependentServiceTypeDef = TypedDict(
     "DependentServiceTypeDef",
     {
         "ServiceName": ServiceNameType,
         "ServiceVersion": ServiceVersionTypeDef,
     },
     total=False,
@@ -789,14 +758,32 @@
     "TaxDocumentsTypeDef",
     {
         "IND": INDTaxDocumentsTypeDef,
     },
     total=False,
 )
 
+ListClusterJobsResultTypeDef = TypedDict(
+    "ListClusterJobsResultTypeDef",
+    {
+        "JobListEntries": List[JobListEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListJobsResultTypeDef = TypedDict(
+    "ListJobsResultTypeDef",
+    {
+        "JobListEntries": List[JobListEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListLongTermPricingResultTypeDef = TypedDict(
     "ListLongTermPricingResultTypeDef",
     {
         "LongTermPricingEntries": List[LongTermPricingListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -804,15 +791,14 @@
 
 OnDeviceServiceConfigurationTypeDef = TypedDict(
     "OnDeviceServiceConfigurationTypeDef",
     {
         "NFSOnDeviceService": NFSOnDeviceServiceConfigurationTypeDef,
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationTypeDef,
         "EKSOnDeviceService": EKSOnDeviceServiceConfigurationTypeDef,
-        "S3OnDeviceService": S3OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
 S3ResourceTypeDef = TypedDict(
     "S3ResourceTypeDef",
     {
@@ -914,35 +900,31 @@
     total=False,
 )
 
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "JobType": JobTypeType,
+        "Resources": JobResourceTypeDef,
         "AddressId": str,
+        "RoleARN": str,
         "SnowballType": SnowballTypeType,
         "ShippingOption": ShippingOptionType,
     },
 )
 _OptionalCreateClusterRequestRequestTypeDef = TypedDict(
     "_OptionalCreateClusterRequestRequestTypeDef",
     {
-        "Resources": JobResourceTypeDef,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
         "Description": str,
         "KmsKeyARN": str,
-        "RoleARN": str,
         "Notification": NotificationTypeDef,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "RemoteManagement": RemoteManagementType,
-        "InitialClusterSize": int,
-        "ForceCreateJobs": bool,
-        "LongTermPricingIds": Sequence[str],
-        "SnowballCapacityPreference": SnowballCapacityType,
     },
     total=False,
 )
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
```

### Comparing `mypy-boto3-snowball-1.26.117/mypy_boto3_snowball.egg-info/PKG-INFO` & `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-snowball
-Version: 1.26.117
-Summary: Type annotations for boto3.Snowball 1.26.117 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.70
+Summary: Type annotations for boto3.Snowball 1.26.70 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-snowball"></a>
 
 # mypy-boto3-snowball
 
 [![PyPI - mypy-boto3-snowball](https://img.shields.io/pypi/v/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.26.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,15 +362,14 @@
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
     NotificationTypeDef,
     CompatibleImageTypeDef,
     ResponseMetadataTypeDef,
-    JobListEntryTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
     DataTransferTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeAddressesRequestRequestTypeDef,
@@ -380,56 +379,56 @@
     EKSOnDeviceServiceConfigurationTypeDef,
     Ec2AmiResourceTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
     INDTaxDocumentsTypeDef,
+    JobListEntryTypeDef,
     JobLogsTypeDef,
     KeyRangeTypeDef,
     ListClusterJobsRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
-    S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
     CreateAddressRequestRequestTypeDef,
     CreateAddressResultTypeDef,
+    CreateClusterResultTypeDef,
     CreateJobResultTypeDef,
     CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
     DescribeReturnShippingLabelResultTypeDef,
     GetJobManifestResultTypeDef,
     GetJobUnlockCodeResultTypeDef,
     GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
-    CreateClusterResultTypeDef,
-    ListClusterJobsResultTypeDef,
-    ListJobsResultTypeDef,
     DependentServiceTypeDef,
     DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     LambdaResourceTypeDef,
     TaxDocumentsTypeDef,
+    ListClusterJobsResultTypeDef,
+    ListJobsResultTypeDef,
     ListLongTermPricingResultTypeDef,
     OnDeviceServiceConfigurationTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
     SnowconeDeviceConfigurationTypeDef,
     ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
@@ -453,42 +452,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-snowball-1.26.117/mypy_boto3_snowball.egg-info/SOURCES.txt` & `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.26.117/setup.py` & `mypy-boto3-snowball-1.26.70/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-snowball.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-snowball",
-    version="1.26.117",
+    version="1.26.70",
     packages=["mypy_boto3_snowball"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Snowball 1.26.117 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Snowball 1.26.70 service generated with mypy-boto3-builder"
+        " 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

