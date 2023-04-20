# Comparing `tmp/adh_sample_library_preview-0.9.8rc0.tar.gz` & `tmp/adh_sample_library_preview-0.9.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adh_sample_library_preview-0.9.8rc0.tar", last modified: Thu Sep 22 15:34:01 2022, max compression
+gzip compressed data, was "adh_sample_library_preview-0.9.9rc0.tar", last modified: Tue Sep 27 17:52:53 2022, max compression
```

## Comparing `adh_sample_library_preview-0.9.8rc0.tar` & `adh_sample_library_preview-0.9.9rc0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 15:34:01.268743 adh_sample_library_preview-0.9.8rc0/
--rw-r--r--   0 root         (0) root         (0)     7433 2022-09-22 15:34:01.264743 adh_sample_library_preview-0.9.8rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6057 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 15:34:01.196741 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/
--rw-r--r--   0 root         (0) root         (0)     6219 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/ADHClient.py
--rw-r--r--   0 root         (0) root         (0)      606 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/AbstractBaseClient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 15:34:01.200741 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/
--rw-r--r--   0 root         (0) root         (0)     5756 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Asset.py
--rw-r--r--   0 root         (0) root         (0)     2019 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/AssetRule.py
--rw-r--r--   0 root         (0) root         (0)     4916 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/AssetType.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 15:34:01.204742 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Data/
--rw-r--r--   0 root         (0) root         (0)     2032 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Data/DataErrors.py
--rw-r--r--   0 root         (0) root         (0)     1437 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Data/DataResults.py
--rw-r--r--   0 root         (0) root         (0)       72 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3925 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/MetadataItem.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 15:34:01.208742 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/
--rw-r--r--   0 root         (0) root         (0)     5147 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/ResolvedAsset.py
--rw-r--r--   0 root         (0) root         (0)      958 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/ResolvedEnum.py
--rw-r--r--   0 root         (0) root         (0)     3741 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/ResolvedProperty.py
--rw-r--r--   0 root         (0) root         (0)     1733 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/ResolvedSdsType.py
--rw-r--r--   0 root         (0) root         (0)     1090 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/ResolvedSource.py
--rw-r--r--   0 root         (0) root         (0)     1496 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/ResolvedStatus.py
--rw-r--r--   0 root         (0) root         (0)     1536 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/ResolvedStream.py
--rw-r--r--   0 root         (0) root         (0)      982 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/UnresolvedStream.py
--rw-r--r--   0 root         (0) root         (0)      348 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 15:34:01.212742 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Status/
--rw-r--r--   0 root         (0) root         (0)     1870 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Status/StatusConfiguration.py
--rw-r--r--   0 root         (0) root         (0)     2274 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Status/StatusData.py
--rw-r--r--   0 root         (0) root         (0)      153 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Status/StatusDefinitionType.py
--rw-r--r--   0 root         (0) root         (0)      150 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Status/StatusEnum.py
--rw-r--r--   0 root         (0) root         (0)     3052 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Status/StatusMapping.py
--rw-r--r--   0 root         (0) root         (0)     2224 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Status/ValueStatusMapping.py
--rw-r--r--   0 root         (0) root         (0)      270 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Status/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2589 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/StreamReference.py
--rw-r--r--   0 root         (0) root         (0)     3028 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/TypeReference.py
--rw-r--r--   0 root         (0) root         (0)      282 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3106 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/AssetRules.py
--rw-r--r--   0 root         (0) root         (0)     6210 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/AssetTypes.py
--rw-r--r--   0 root         (0) root         (0)    18400 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Assets.py
--rw-r--r--   0 root         (0) root         (0)     5462 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Authentication.py
--rw-r--r--   0 root         (0) root         (0)     8287 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/BaseClient.py
--rw-r--r--   0 root         (0) root         (0)     1274 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/BaseClientStub.py
--rw-r--r--   0 root         (0) root         (0)     6170 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Communities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 15:34:01.220742 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Community/
--rw-r--r--   0 root         (0) root         (0)     4020 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Community/Community.py
--rw-r--r--   0 root         (0) root         (0)     1229 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Community/CommunityInput.py
--rw-r--r--   0 root         (0) root         (0)     1328 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Community/CommunitySummaryInformation.py
--rw-r--r--   0 root         (0) root         (0)     2442 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Community/CommunityTenant.py
--rw-r--r--   0 root         (0) root         (0)      185 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Community/CommunityTenantStatus.py
--rw-r--r--   0 root         (0) root         (0)     3344 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Community/StreamSearchResult.py
--rw-r--r--   0 root         (0) root         (0)      298 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Community/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2447 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/ContentResolvers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 15:34:01.228742 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/
--rw-r--r--   0 root         (0) root         (0)     5163 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/DataItem.py
--rw-r--r--   0 root         (0) root         (0)     2478 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/DataItemField.py
--rw-r--r--   0 root         (0) root         (0)      132 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/DataItemResourceType.py
--rw-r--r--   0 root         (0) root         (0)     4793 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/DataMapping.py
--rw-r--r--   0 root         (0) root         (0)     9439 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/DataView.py
--rw-r--r--   0 root         (0) root         (0)      128 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/DataViewShape.py
--rw-r--r--   0 root         (0) root         (0)     5756 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/Field.py
--rw-r--r--   0 root         (0) root         (0)      184 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/FieldKind.py
--rw-r--r--   0 root         (0) root         (0)     4765 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/FieldMapping.py
--rw-r--r--   0 root         (0) root         (0)     2868 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/FieldSet.py
--rw-r--r--   0 root         (0) root         (0)     1579 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/FieldSets.py
--rw-r--r--   0 root         (0) root         (0)      210 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/FieldSource.py
--rw-r--r--   0 root         (0) root         (0)     2125 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/MetadataValue.py
--rw-r--r--   0 root         (0) root         (0)     2126 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/Query.py
--rw-r--r--   0 root         (0) root         (0)     1574 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/ResolvedDataItems.py
--rw-r--r--   0 root         (0) root         (0)      132 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/SummaryDirection.py
--rw-r--r--   0 root         (0) root         (0)      604 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17826 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataViews.py
--rw-r--r--   0 root         (0) root         (0)     2853 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/EDSClient.py
--rw-r--r--   0 root         (0) root         (0)     2060 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Namespaces.py
--rw-r--r--   0 root         (0) root         (0)     1062 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/OCSClient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 15:34:01.232742 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/OMF/
--rw-r--r--   0 root         (0) root         (0)     2027 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/OMF/Subscription.py
--rw-r--r--   0 root         (0) root         (0)     2006 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/OMF/Topic.py
--rw-r--r--   0 root         (0) root         (0)       63 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/OMF/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2920 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/PatchableSecurable.py
--rw-r--r--   0 root         (0) root         (0)     4116 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Roles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 15:34:01.248742 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/
--rw-r--r--   0 root         (0) root         (0)      169 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsBoundaryType.py
--rw-r--r--   0 root         (0) root         (0)      161 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsExtrapolationMode.py
--rw-r--r--   0 root         (0) root         (0)      302 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsInterpolationMode.py
--rw-r--r--   0 root         (0) root         (0)      690 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsNamespace.py
--rw-r--r--   0 root         (0) root         (0)     8263 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsResolvedStream.py
--rw-r--r--   0 root         (0) root         (0)     1369 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsResultPage.py
--rw-r--r--   0 root         (0) root         (0)      184 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsSearchMode.py
--rw-r--r--   0 root         (0) root         (0)     7006 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStream.py
--rw-r--r--   0 root         (0) root         (0)     1110 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStreamIndex.py
--rw-r--r--   0 root         (0) root         (0)     2700 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStreamPropertyOverride.py
--rw-r--r--   0 root         (0) root         (0)     4377 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStreamView.py
--rw-r--r--   0 root         (0) root         (0)     2826 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStreamViewMap.py
--rw-r--r--   0 root         (0) root         (0)     3144 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStreamViewMapProperty.py
--rw-r--r--   0 root         (0) root         (0)      250 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStreamViewMode.py
--rw-r--r--   0 root         (0) root         (0)     2373 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStreamViewProperty.py
--rw-r--r--   0 root         (0) root         (0)      417 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsSummaryType.py
--rw-r--r--   0 root         (0) root         (0)    10516 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsType.py
--rw-r--r--   0 root         (0) root         (0)     1806 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsTypeCode.py
--rw-r--r--   0 root         (0) root         (0)     6771 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsTypeProperty.py
--rw-r--r--   0 root         (0) root         (0)      877 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/__init__.py
--rw-r--r--   0 root         (0) root         (0)      355 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SdsError.py
--rw-r--r--   0 root         (0) root         (0)     6772 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Securable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 15:34:01.260743 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/
--rw-r--r--   0 root         (0) root         (0)     2219 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/AccessControlEntry.py
--rw-r--r--   0 root         (0) root         (0)     1679 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/AccessControlList.py
--rw-r--r--   0 root         (0) root         (0)      118 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/AccessType.py
--rw-r--r--   0 root         (0) root         (0)      220 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/CommonAccessRightsEnum.py
--rw-r--r--   0 root         (0) root         (0)     1612 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/Owner.py
--rw-r--r--   0 root         (0) root         (0)     3078 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/Role.py
--rw-r--r--   0 root         (0) root         (0)      154 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/RoleScope.py
--rw-r--r--   0 root         (0) root         (0)     1706 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/Trustee.py
--rw-r--r--   0 root         (0) root         (0)      129 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/TrusteeType.py
--rw-r--r--   0 root         (0) root         (0)     6283 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/User.py
--rw-r--r--   0 root         (0) root         (0)     4700 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/UserInvitation.py
--rw-r--r--   0 root         (0) root         (0)      163 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/UserInvitationState.py
--rw-r--r--   0 root         (0) root         (0)      459 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25916 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SharedStreams.py
--rw-r--r--   0 root         (0) root         (0)     7011 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/StreamViews.py
--rw-r--r--   0 root         (0) root         (0)    56108 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Streams.py
--rw-r--r--   0 root         (0) root         (0)     2583 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Subscriptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 15:34:01.260743 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Tenant/
--rw-r--r--   0 root         (0) root         (0)     4185 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Tenant/Namespace.py
--rw-r--r--   0 root         (0) root         (0)      167 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Tenant/NamespaceProvisioningState.py
--rw-r--r--   0 root         (0) root         (0)       99 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Tenant/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 15:34:01.264743 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       90 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1277 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Tests/test_baseclient.py
--rw-r--r--   0 root         (0) root         (0)     7150 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Tests/test_streams.py
--rw-r--r--   0 root         (0) root         (0)     2366 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Topics.py
--rw-r--r--   0 root         (0) root         (0)     5648 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Types.py
--rw-r--r--   0 root         (0) root         (0)     8969 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Users.py
--rw-r--r--   0 root         (0) root         (0)      814 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 15:34:01.196741 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7433 2022-09-22 15:34:00.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6178 2022-09-22 15:34:01.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-22 15:34:00.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2022-09-22 15:34:00.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2022-09-22 15:34:00.000000 adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-22 15:34:01.268743 adh_sample_library_preview-0.9.8rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      965 2022-09-22 15:33:42.000000 adh_sample_library_preview-0.9.8rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 17:52:53.959690 adh_sample_library_preview-0.9.9rc0/
+-rw-r--r--   0 root         (0) root         (0)     7433 2022-09-27 17:52:53.959690 adh_sample_library_preview-0.9.9rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6057 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 17:52:53.899687 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/
+-rw-r--r--   0 root         (0) root         (0)     6219 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/ADHClient.py
+-rw-r--r--   0 root         (0) root         (0)      606 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/AbstractBaseClient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 17:52:53.911687 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/
+-rw-r--r--   0 root         (0) root         (0)     5756 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Asset.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/AssetRule.py
+-rw-r--r--   0 root         (0) root         (0)     4916 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/AssetType.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 17:52:53.911687 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Data/
+-rw-r--r--   0 root         (0) root         (0)     2032 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Data/DataErrors.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Data/DataResults.py
+-rw-r--r--   0 root         (0) root         (0)       72 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3925 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/MetadataItem.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 17:52:53.919688 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/
+-rw-r--r--   0 root         (0) root         (0)     5147 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/ResolvedAsset.py
+-rw-r--r--   0 root         (0) root         (0)      958 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/ResolvedEnum.py
+-rw-r--r--   0 root         (0) root         (0)     3741 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/ResolvedProperty.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/ResolvedSdsType.py
+-rw-r--r--   0 root         (0) root         (0)     1090 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/ResolvedSource.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/ResolvedStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/ResolvedStream.py
+-rw-r--r--   0 root         (0) root         (0)      982 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/UnresolvedStream.py
+-rw-r--r--   0 root         (0) root         (0)      348 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 17:52:53.923688 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Status/
+-rw-r--r--   0 root         (0) root         (0)     1870 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Status/StatusConfiguration.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Status/StatusData.py
+-rw-r--r--   0 root         (0) root         (0)      153 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Status/StatusDefinitionType.py
+-rw-r--r--   0 root         (0) root         (0)      150 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Status/StatusEnum.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Status/StatusMapping.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Status/ValueStatusMapping.py
+-rw-r--r--   0 root         (0) root         (0)      270 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Status/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/StreamReference.py
+-rw-r--r--   0 root         (0) root         (0)     3028 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/TypeReference.py
+-rw-r--r--   0 root         (0) root         (0)      282 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3106 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/AssetRules.py
+-rw-r--r--   0 root         (0) root         (0)     6210 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/AssetTypes.py
+-rw-r--r--   0 root         (0) root         (0)    18400 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Assets.py
+-rw-r--r--   0 root         (0) root         (0)     5462 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Authentication.py
+-rw-r--r--   0 root         (0) root         (0)     8287 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/BaseClient.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/BaseClientStub.py
+-rw-r--r--   0 root         (0) root         (0)     6170 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Communities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 17:52:53.927688 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Community/
+-rw-r--r--   0 root         (0) root         (0)     4020 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Community/Community.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Community/CommunityInput.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Community/CommunitySummaryInformation.py
+-rw-r--r--   0 root         (0) root         (0)     2442 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Community/CommunityTenant.py
+-rw-r--r--   0 root         (0) root         (0)      185 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Community/CommunityTenantStatus.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Community/StreamSearchResult.py
+-rw-r--r--   0 root         (0) root         (0)      298 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Community/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/ContentResolvers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 17:52:53.935688 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/
+-rw-r--r--   0 root         (0) root         (0)     5163 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/DataItem.py
+-rw-r--r--   0 root         (0) root         (0)     2478 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/DataItemField.py
+-rw-r--r--   0 root         (0) root         (0)      132 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/DataItemResourceType.py
+-rw-r--r--   0 root         (0) root         (0)     4793 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/DataMapping.py
+-rw-r--r--   0 root         (0) root         (0)     9439 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/DataView.py
+-rw-r--r--   0 root         (0) root         (0)      128 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/DataViewShape.py
+-rw-r--r--   0 root         (0) root         (0)     5756 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/Field.py
+-rw-r--r--   0 root         (0) root         (0)      184 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/FieldKind.py
+-rw-r--r--   0 root         (0) root         (0)     4765 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/FieldMapping.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/FieldSet.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/FieldSets.py
+-rw-r--r--   0 root         (0) root         (0)      210 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/FieldSource.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/MetadataValue.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/Query.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/ResolvedDataItems.py
+-rw-r--r--   0 root         (0) root         (0)      132 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/SummaryDirection.py
+-rw-r--r--   0 root         (0) root         (0)      604 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17826 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataViews.py
+-rw-r--r--   0 root         (0) root         (0)     2853 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/EDSClient.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Namespaces.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/OCSClient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 17:52:53.935688 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/OMF/
+-rw-r--r--   0 root         (0) root         (0)     2027 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/OMF/Subscription.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/OMF/Topic.py
+-rw-r--r--   0 root         (0) root         (0)       63 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/OMF/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2920 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/PatchableSecurable.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Roles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 17:52:53.947689 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/
+-rw-r--r--   0 root         (0) root         (0)      169 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsBoundaryType.py
+-rw-r--r--   0 root         (0) root         (0)      161 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsExtrapolationMode.py
+-rw-r--r--   0 root         (0) root         (0)      302 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsInterpolationMode.py
+-rw-r--r--   0 root         (0) root         (0)      690 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsNamespace.py
+-rw-r--r--   0 root         (0) root         (0)     8263 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsResolvedStream.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsResultPage.py
+-rw-r--r--   0 root         (0) root         (0)      184 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsSearchMode.py
+-rw-r--r--   0 root         (0) root         (0)     7006 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStream.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStreamIndex.py
+-rw-r--r--   0 root         (0) root         (0)     2700 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStreamPropertyOverride.py
+-rw-r--r--   0 root         (0) root         (0)     4377 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStreamView.py
+-rw-r--r--   0 root         (0) root         (0)     2826 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStreamViewMap.py
+-rw-r--r--   0 root         (0) root         (0)     3144 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStreamViewMapProperty.py
+-rw-r--r--   0 root         (0) root         (0)      250 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStreamViewMode.py
+-rw-r--r--   0 root         (0) root         (0)     2373 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStreamViewProperty.py
+-rw-r--r--   0 root         (0) root         (0)      417 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsSummaryType.py
+-rw-r--r--   0 root         (0) root         (0)    10516 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsType.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsTypeCode.py
+-rw-r--r--   0 root         (0) root         (0)     6771 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsTypeProperty.py
+-rw-r--r--   0 root         (0) root         (0)      877 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      355 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SdsError.py
+-rw-r--r--   0 root         (0) root         (0)     6772 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Securable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 17:52:53.955689 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/
+-rw-r--r--   0 root         (0) root         (0)     2219 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/AccessControlEntry.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/AccessControlList.py
+-rw-r--r--   0 root         (0) root         (0)      118 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/AccessType.py
+-rw-r--r--   0 root         (0) root         (0)      220 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/CommonAccessRightsEnum.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/Owner.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/Role.py
+-rw-r--r--   0 root         (0) root         (0)      154 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/RoleScope.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/Trustee.py
+-rw-r--r--   0 root         (0) root         (0)      129 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/TrusteeType.py
+-rw-r--r--   0 root         (0) root         (0)     6283 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/User.py
+-rw-r--r--   0 root         (0) root         (0)     4700 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/UserInvitation.py
+-rw-r--r--   0 root         (0) root         (0)      163 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/UserInvitationState.py
+-rw-r--r--   0 root         (0) root         (0)      459 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25916 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SharedStreams.py
+-rw-r--r--   0 root         (0) root         (0)     7011 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/StreamViews.py
+-rw-r--r--   0 root         (0) root         (0)    56108 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Streams.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 17:52:53.955689 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Tenant/
+-rw-r--r--   0 root         (0) root         (0)     4185 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Tenant/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)      167 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Tenant/NamespaceProvisioningState.py
+-rw-r--r--   0 root         (0) root         (0)       99 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Tenant/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 17:52:53.959690 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       90 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Tests/test_baseclient.py
+-rw-r--r--   0 root         (0) root         (0)     7150 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Tests/test_streams.py
+-rw-r--r--   0 root         (0) root         (0)     2366 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Topics.py
+-rw-r--r--   0 root         (0) root         (0)     5648 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Types.py
+-rw-r--r--   0 root         (0) root         (0)     8969 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Users.py
+-rw-r--r--   0 root         (0) root         (0)      814 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 17:52:53.907687 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7433 2022-09-27 17:52:53.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6178 2022-09-27 17:52:53.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-27 17:52:53.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2022-09-27 17:52:53.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2022-09-27 17:52:53.000000 adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-27 17:52:53.959690 adh_sample_library_preview-0.9.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      965 2022-09-27 17:52:37.000000 adh_sample_library_preview-0.9.9rc0/setup.py
```

### Comparing `adh_sample_library_preview-0.9.8rc0/PKG-INFO` & `adh_sample_library_preview-0.9.9rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: adh_sample_library_preview
-Version: 0.9.8rc0
+Version: 0.9.9rc0
 Summary: A preview of an ADH (Aveva Data Hub) client library
 Home-page: https://github.com/osisoft/sample-adh-sample_libraries-python
 Author: OSIsoft
 Author-email: samples@osisoft.com
 License: Apache 2.0
 Description: # AVEVA Data Hub Python Library Sample
         
         | :loudspeaker: **Notice**: This library is an AVEVA Data Hub targeted version of the ocs_sample_library_preview. The ocs_sample_library_preview library is being deprecated and this library should be used moving forward. |
         | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
         
-        **Version:** 0.9.8_preview
+        **Version:** 0.9.9_preview
         
         [![Build Status](https://dev.azure.com/osieng/engineering/_apis/build/status/product-readiness/ADH/aveva.sample-adh-sample_libraries-python?branchName=main)](https://dev.azure.com/osieng/engineering/_build/latest?definitionId=4674&branchName=main)
         
         This sample library requires Python 3.7+. You can download Python [here](https://www.python.org/downloads/).
         
         - **NOTE**: The library previously required Python 3.9+ to take advantage of type annotations. To provide compatibility with environments that cannot upgrade Python to 3.9, `from __future__ import annotations` was added to each necessary file. [This provides backwards compatibility down to Python 3.7](https://docs.python.org/3/library/__future__.html).
```

### Comparing `adh_sample_library_preview-0.9.8rc0/README.md` & `adh_sample_library_preview-0.9.9rc0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AVEVA Data Hub Python Library Sample
 
 | :loudspeaker: **Notice**: This library is an AVEVA Data Hub targeted version of the ocs_sample_library_preview. The ocs_sample_library_preview library is being deprecated and this library should be used moving forward. |
 | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 
-**Version:** 0.9.8_preview
+**Version:** 0.9.9_preview
 
 [![Build Status](https://dev.azure.com/osieng/engineering/_apis/build/status/product-readiness/ADH/aveva.sample-adh-sample_libraries-python?branchName=main)](https://dev.azure.com/osieng/engineering/_build/latest?definitionId=4674&branchName=main)
 
 This sample library requires Python 3.7+. You can download Python [here](https://www.python.org/downloads/).
 
 - **NOTE**: The library previously required Python 3.9+ to take advantage of type annotations. To provide compatibility with environments that cannot upgrade Python to 3.9, `from __future__ import annotations` was added to each necessary file. [This provides backwards compatibility down to Python 3.7](https://docs.python.org/3/library/__future__.html).
```

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/ADHClient.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/ADHClient.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/AbstractBaseClient.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/AbstractBaseClient.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Asset.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Asset.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/AssetRule.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/AssetRule.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/AssetType.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/AssetType.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Data/DataErrors.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Data/DataErrors.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Data/DataResults.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Data/DataResults.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/MetadataItem.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/MetadataItem.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/ResolvedAsset.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/ResolvedAsset.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/ResolvedEnum.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/ResolvedEnum.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/ResolvedProperty.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/ResolvedProperty.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/ResolvedSdsType.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/ResolvedSdsType.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/ResolvedSource.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/ResolvedSource.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/ResolvedStatus.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/ResolvedStatus.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/ResolvedStream.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/ResolvedStream.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Resolved/UnresolvedStream.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Resolved/UnresolvedStream.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Status/StatusConfiguration.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Status/StatusConfiguration.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Status/StatusData.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Status/StatusData.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Status/StatusMapping.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Status/StatusMapping.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/Status/ValueStatusMapping.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/Status/ValueStatusMapping.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/StreamReference.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/StreamReference.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Asset/TypeReference.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Asset/TypeReference.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/AssetRules.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/AssetRules.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/AssetTypes.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/AssetTypes.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Assets.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Assets.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Authentication.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Authentication.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/BaseClient.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/BaseClient.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/BaseClientStub.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/BaseClientStub.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Communities.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Communities.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Community/Community.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Community/Community.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Community/CommunityInput.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Community/CommunityInput.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Community/CommunitySummaryInformation.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Community/CommunitySummaryInformation.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Community/CommunityTenant.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Community/CommunityTenant.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Community/StreamSearchResult.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Community/StreamSearchResult.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/ContentResolvers.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/ContentResolvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 
 class ContentResolver(ABC):
     def __init__(self, response, value_class = None, content = None) -> None:
         self.value_class = value_class
         self.response = response
-        self.content = content if not None else self.response.json()
+        self.content = content if content else self.response.json()
 
 
     def resolve(self):
         if self.value_class is None:
             return self.content
         else:
             return self._resolve()
```

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/DataItem.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/DataItem.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/DataItemField.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/DataItemField.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/DataMapping.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/DataMapping.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/DataView.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/DataView.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/Field.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/Field.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/FieldMapping.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/FieldMapping.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/FieldSet.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/FieldSet.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/FieldSets.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/FieldSets.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/MetadataValue.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/MetadataValue.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/Query.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/Query.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/ResolvedDataItems.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/ResolvedDataItems.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataView/__init__.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataView/__init__.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/DataViews.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/DataViews.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/EDSClient.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/EDSClient.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Namespaces.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Namespaces.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/OCSClient.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/OCSClient.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/OMF/Subscription.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/OMF/Subscription.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/OMF/Topic.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/OMF/Topic.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/PatchableSecurable.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/PatchableSecurable.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Roles.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Roles.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsNamespace.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsNamespace.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsResolvedStream.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsResolvedStream.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsResultPage.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsResultPage.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStream.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStream.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStreamIndex.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStreamIndex.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStreamPropertyOverride.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStreamPropertyOverride.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStreamView.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStreamView.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStreamViewMap.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStreamViewMap.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStreamViewMapProperty.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStreamViewMapProperty.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsStreamViewProperty.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsStreamViewProperty.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsType.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsType.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsTypeCode.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsTypeCode.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/SdsTypeProperty.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/SdsTypeProperty.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SDS/__init__.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SDS/__init__.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Securable.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Securable.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/AccessControlEntry.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/AccessControlEntry.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/AccessControlList.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/AccessControlList.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/Owner.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/Owner.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/Role.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/Role.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/Trustee.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/Trustee.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/User.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/User.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Security/UserInvitation.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Security/UserInvitation.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/SharedStreams.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/SharedStreams.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/StreamViews.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/StreamViews.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Streams.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Streams.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Subscriptions.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Subscriptions.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Tenant/Namespace.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Tenant/Namespace.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Tests/test_baseclient.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Tests/test_baseclient.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Tests/test_streams.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Topics.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Topics.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Types.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Types.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/Users.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/Users.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview/__init__.py` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview/__init__.py`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview.egg-info/PKG-INFO` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: adh-sample-library-preview
-Version: 0.9.8rc0
+Version: 0.9.9rc0
 Summary: A preview of an ADH (Aveva Data Hub) client library
 Home-page: https://github.com/osisoft/sample-adh-sample_libraries-python
 Author: OSIsoft
 Author-email: samples@osisoft.com
 License: Apache 2.0
 Description: # AVEVA Data Hub Python Library Sample
         
         | :loudspeaker: **Notice**: This library is an AVEVA Data Hub targeted version of the ocs_sample_library_preview. The ocs_sample_library_preview library is being deprecated and this library should be used moving forward. |
         | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
         
-        **Version:** 0.9.8_preview
+        **Version:** 0.9.9_preview
         
         [![Build Status](https://dev.azure.com/osieng/engineering/_apis/build/status/product-readiness/ADH/aveva.sample-adh-sample_libraries-python?branchName=main)](https://dev.azure.com/osieng/engineering/_build/latest?definitionId=4674&branchName=main)
         
         This sample library requires Python 3.7+. You can download Python [here](https://www.python.org/downloads/).
         
         - **NOTE**: The library previously required Python 3.9+ to take advantage of type annotations. To provide compatibility with environments that cannot upgrade Python to 3.9, `from __future__ import annotations` was added to each necessary file. [This provides backwards compatibility down to Python 3.7](https://docs.python.org/3/library/__future__.html).
```

### Comparing `adh_sample_library_preview-0.9.8rc0/adh_sample_library_preview.egg-info/SOURCES.txt` & `adh_sample_library_preview-0.9.9rc0/adh_sample_library_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adh_sample_library_preview-0.9.8rc0/setup.py` & `adh_sample_library_preview-0.9.9rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='adh_sample_library_preview',
-    version='0.9.8_preview',
+    version='0.9.9_preview',
     author='OSIsoft',
     license='Apache 2.0',
     author_email='samples@osisoft.com',
     description='A preview of an ADH (Aveva Data Hub) client library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/osisoft/sample-adh-sample_libraries-python',
```

