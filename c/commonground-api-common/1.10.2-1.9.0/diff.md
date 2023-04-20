# Comparing `tmp/commonground-api-common-1.10.2.tar.gz` & `tmp/commonground-api-common-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonground-api-common-1.10.2.tar", last modified: Thu Apr 20 11:59:42 2023, max compression
+gzip compressed data, was "commonground-api-common-1.9.0.tar", last modified: Mon Dec 12 13:57:55 2022, max compression
```

## Comparing `commonground-api-common-1.10.2.tar` & `commonground-api-common-1.9.0.tar`

### file list

```diff
@@ -1,290 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.550491 commonground-api-common-1.10.2/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-20 11:59:42.550491 commonground-api-common-1.10.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.514490 commonground-api-common-1.10.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      952 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/bin/generate_schema
--rwxr-xr-x   0 runner    (1001) docker     (123)      319 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/bin/patch_content_types
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/bin/use_external_components
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.514490 commonground-api-common-1.10.2/commonground_api_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-20 11:59:42.000000 commonground-api-common-1.10.2/commonground_api_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12353 2023-04-20 11:59:42.000000 commonground-api-common-1.10.2/commonground_api_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:59:42.000000 commonground-api-common-1.10.2/commonground_api_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:59:42.000000 commonground-api-common-1.10.2/commonground_api_common.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-20 11:59:42.000000 commonground-api-common-1.10.2/commonground_api_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 11:59:42.000000 commonground-api-common-1.10.2/commonground_api_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-20 11:59:42.550491 commonground-api-common-1.10.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.514490 commonground-api-common-1.10.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_autorisatie_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_cache_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_check_query_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_content_type_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_gegevensgroepen.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_get_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_jwt_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_jwtsecrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_nested_serializer_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_publish_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_schema_root_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_server_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/tests/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.518490 commonground-api-common-1.10.2/vng_api_common/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.518490 commonground-api-common-1.10.2/vng_api_common/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/api/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.522490 commonground-api-common-1.10.2/vng_api_common/audittrails/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.522490 commonground-api-common-1.10.2/vng_api_common/audittrails/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/api/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/audits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.522490 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0002_auto_20190516_0830.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0003_auto_20190517_0844.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0004_auto_20190520_1238.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0005_auto_20190520_1450.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0006_audittrail_toelichting.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0007_auto_20190522_0916.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0008_audittrail_resource_weergave.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0009_auto_20190712_1643.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0010_audittrail_request_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0011_auto_20190918_1335.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0012_auto_20200619_0545.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0012_remove_audittrail_request_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0013_audittrail_logrecord_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0013_auto_20201207_0846.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0014_auto_20201221_0905.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0014_auto_20210323_1654.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0015_auto_20220318_1608.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0016_merge_20220607_0517.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0017_alter_audittrail_bron.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0018_auto_20221212_0745.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/audittrails/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.526490 commonground-api-common-1.10.2/vng_api_common/authorizations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.526490 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0002_authorizationsconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0003_auto_20190502_0409.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0004_auto_20190503_0941.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0005_auto_20190506_0842.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0006_auto_20190506_0901.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0007_auto_20190506_1212.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0008_auto_20190712_1541.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0009_update_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0010_auto_20190712_1643.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0011_auto_20191114_0728.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0012_auto_20200619_0545.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0013_auto_20201207_0846.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0014_auto_20201221_0905.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0015_auto_20220318_1608.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/authorizations/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.526490 commonground-api-common-1.10.2/vng_api_common/caching/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/caching/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/caching/etags.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/caching/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/caching/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/caching/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/caching/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.526490 commonground-api-common-1.10.2/vng_api_common/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/conf/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.526490 commonground-api-common-1.10.2/vng_api_common/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/db/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/exception_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/geo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.530490 commonground-api-common-1.10.2/vng_api_common/inspectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/inspectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/inspectors/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/inspectors/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/inspectors/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    12575 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/inspectors/geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/inspectors/polymorphic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/inspectors/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/inspectors/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20425 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/inspectors/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.510490 commonground-api-common-1.10.2/vng_api_common/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.510490 commonground-api-common-1.10.2/vng_api_common/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.530490 commonground-api-common-1.10.2/vng_api_common/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19495 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.530490 commonground-api-common-1.10.2/vng_api_common/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.530490 commonground-api-common-1.10.2/vng_api_common/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/management/commands/generate_autorisaties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/management/commands/generate_notificaties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/management/commands/generate_swagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/management/commands/patch_error_contenttypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/management/commands/use_external_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.530490 commonground-api-common-1.10.2/vng_api_common/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/migrations/0002_apicredential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/migrations/0003_auto_20190417_1145.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/migrations/0004_auto_20190517_0903.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/migrations/0005_auto_20190614_1346.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.530490 commonground-api-common-1.10.2/vng_api_common/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.530490 commonground-api-common-1.10.2/vng_api_common/notifications/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.534490 commonground-api-common-1.10.2/vng_api_common/notifications/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0002_subscription__subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0003_auto_20190319_1048.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0004_auto_20190325_1313.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0005_fix_default_nrc.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0006_auto_20190417_1142.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0007_auto_20190429_1442.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0008_auto_20190502_0415.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0009_auto_20190729_0427.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0010_auto_20220704_1419.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/oas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/polymorphism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.510490 commonground-api-common-1.10.2/vng_api_common/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.510490 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.510490 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/css/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.534490 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/css/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/css/admin/admin_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.534490 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/ico/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/ico/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.534490 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/img/
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/img/vng.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.510490 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.534490 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.538491 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)    64548 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (123)   151749 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    48488 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   108539 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (123)    76483 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    32461 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   192348 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)   492048 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   155758 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   625953 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.542491 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)   222911 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   402249 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    78635 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   311949 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   131637 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)   250568 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    58072 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   190253 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.542491 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.542491 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/css/
--rw-r--r--   0 runner    (1001) docker     (123)    69015 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.css
--rw-r--r--   0 runner    (1001) docker     (123)    55111 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.546491 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   129916 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   694583 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)   129612 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    87688 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    74768 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    34388 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   144451 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   186728 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)   816926 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)   186444 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    96256 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    74256 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.546491 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/jquery/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/jquery/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   218897 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.js
--rw-r--r--   0 runner    (1001) docker     (123)    69917 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.546491 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/popper/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/popper/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    87203 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/popper/popper.js
--rw-r--r--   0 runner    (1001) docker     (123)    21004 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/popper/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.510490 commonground-api-common-1.10.2/vng_api_common/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.546491 commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.546491 commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/admin/base_site.html
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/api_schema_to_markdown_table.md
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/autorisaties.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.546491 commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/includes/kanalen_card.html
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/master.html
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/notificaties.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.550491 commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/ref/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/ref/error_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/ref/scopes.html
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/view_config.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.550491 commonground-api-common-1.10.2/vng_api_common/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/templatetags/vng_api_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:42.550491 commonground-api-common-1.10.2/vng_api_common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/tests/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/tests/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-20 11:59:33.000000 commonground-api-common-1.10.2/vng_api_common/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.644428 commonground-api-common-1.9.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      952 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/bin/generate_schema
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/bin/generate_schema.cmd
+-rwxr-xr-x   0 runner    (1001) docker     (123)      319 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/bin/patch_content_types
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/bin/patch_content_types.cmd
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/bin/use_external_components
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/bin/use_external_components.cmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.644428 commonground-api-common-1.9.0/commonground_api_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2022-12-12 13:57:55.000000 commonground-api-common-1.9.0/commonground_api_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2022-12-12 13:57:55.000000 commonground-api-common-1.9.0/commonground_api_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 13:57:55.000000 commonground-api-common-1.9.0/commonground_api_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 13:57:55.000000 commonground-api-common-1.9.0/commonground_api_common.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2022-12-12 13:57:55.000000 commonground-api-common-1.9.0/commonground_api_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-12 13:57:55.000000 commonground-api-common-1.9.0/commonground_api_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.648428 commonground-api-common-1.9.0/vng_api_common/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.652428 commonground-api-common-1.9.0/vng_api_common/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/api/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.652428 commonground-api-common-1.9.0/vng_api_common/audittrails/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.652428 commonground-api-common-1.9.0/vng_api_common/audittrails/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/api/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/audits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.656429 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0002_auto_20190516_0830.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0003_auto_20190517_0844.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0004_auto_20190520_1238.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0005_auto_20190520_1450.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0006_audittrail_toelichting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0007_auto_20190522_0916.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0008_audittrail_resource_weergave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0009_auto_20190712_1643.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0010_audittrail_request_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0011_auto_20190918_1335.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0012_auto_20200619_0545.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0012_remove_audittrail_request_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0013_audittrail_logrecord_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0013_auto_20201207_0846.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0014_auto_20201221_0905.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0014_auto_20210323_1654.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0015_auto_20220318_1608.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0016_merge_20220607_0517.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0017_alter_audittrail_bron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0018_auto_20221212_0745.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.656429 commonground-api-common-1.9.0/vng_api_common/authorizations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.656429 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0002_authorizationsconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0003_auto_20190502_0409.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0004_auto_20190503_0941.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0005_auto_20190506_0842.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0006_auto_20190506_0901.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0007_auto_20190506_1212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0008_auto_20190712_1541.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0009_update_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0010_auto_20190712_1643.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0011_auto_20191114_0728.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0012_auto_20200619_0545.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0013_auto_20201207_0846.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0014_auto_20201221_0905.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0015_auto_20220318_1608.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/caching/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/caching/etags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/caching/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/caching/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/caching/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/caching/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/conf/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/db/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/exception_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/geo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/inspectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12575 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/polymorphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20425 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.640428 commonground-api-common-1.9.0/vng_api_common/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.640428 commonground-api-common-1.9.0/vng_api_common/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19495 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/management/commands/generate_autorisaties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/management/commands/generate_notificaties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/management/commands/generate_swagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/management/commands/patch_error_contenttypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/management/commands/use_external_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/migrations/0002_apicredential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/migrations/0003_auto_20190417_1145.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/migrations/0004_auto_20190517_0903.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/migrations/0005_auto_20190614_1346.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.664429 commonground-api-common-1.9.0/vng_api_common/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.664429 commonground-api-common-1.9.0/vng_api_common/notifications/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.664429 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0002_subscription__subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0003_auto_20190319_1048.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0004_auto_20190325_1313.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0005_fix_default_nrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0006_auto_20190417_1142.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0007_auto_20190429_1442.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0008_auto_20190502_0415.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0009_auto_20190729_0427.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0010_auto_20220704_1419.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/oas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/polymorphism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.640428 commonground-api-common-1.9.0/vng_api_common/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.644428 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.640428 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/css/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.664429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/css/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/css/admin/admin_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.664429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/ico/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/ico/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.664429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/img/vng.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.644428 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.664429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.668429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    64548 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)   151749 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    48488 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   108539 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (123)    76483 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32461 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   192348 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   492048 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   155758 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   625953 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.672429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   222911 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   402249 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    78635 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   311949 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   131637 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)   250568 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    58072 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   190253 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.672429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.672429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    69015 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.css
+-rw-r--r--   0 runner    (1001) docker     (123)    55111 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.676429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   129916 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   694583 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   129612 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    87688 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    74768 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    34388 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   144451 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   186728 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   816926 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   186444 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    96256 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    74256 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.676429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/jquery/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   218897 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.js
+-rw-r--r--   0 runner    (1001) docker     (123)    69917 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.676429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/popper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/popper/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    87203 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/popper/popper.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21004 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/popper/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.644428 commonground-api-common-1.9.0/vng_api_common/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/admin/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/api_schema_to_markdown_table.md
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/autorisaties.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/includes/kanalen_card.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/master.html
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/notificaties.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/ref/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/ref/error_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/ref/scopes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/view_config.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/vng_api_common/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templatetags/vng_api_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/vng_api_common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/tests/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/tests/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12868 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/viewsets.py
```

### Comparing `commonground-api-common-1.10.2/PKG-INFO` & `commonground-api-common-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: commonground-api-common
-Version: 1.10.2
+Version: 1.9.0
 Summary: Commonground API tooling
 Home-page: https://github.com/maykinmedia/commonground-api-common
 Author: Maykin Media, VNG-Realisatie
 Author-email: support@maykinmedia.nl
 License: EUPL 1.2
 Keywords: openapi,swagger,django
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `commonground-api-common-1.10.2/README.rst` & `commonground-api-common-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/bin/generate_schema` & `commonground-api-common-1.9.0/bin/generate_schema`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/commonground_api_common.egg-info/PKG-INFO` & `commonground-api-common-1.9.0/commonground_api_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: commonground-api-common
-Version: 1.10.2
+Version: 1.9.0
 Summary: Commonground API tooling
 Home-page: https://github.com/maykinmedia/commonground-api-common
 Author: Maykin Media, VNG-Realisatie
 Author-email: support@maykinmedia.nl
 License: EUPL 1.2
 Keywords: openapi,swagger,django
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `commonground-api-common-1.10.2/commonground_api_common.egg-info/SOURCES.txt` & `commonground-api-common-1.9.0/commonground_api_common.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,23 @@
 MANIFEST.in
 README.rst
-pyproject.toml
 setup.cfg
 setup.py
 bin/generate_schema
+bin/generate_schema.cmd
 bin/patch_content_types
+bin/patch_content_types.cmd
 bin/use_external_components
+bin/use_external_components.cmd
 commonground_api_common.egg-info/PKG-INFO
 commonground_api_common.egg-info/SOURCES.txt
 commonground_api_common.egg-info/dependency_links.txt
 commonground_api_common.egg-info/not-zip-safe
 commonground_api_common.egg-info/requires.txt
 commonground_api_common.egg-info/top_level.txt
-tests/test_autorisatie_validation.py
-tests/test_cache_headers.py
-tests/test_check_query_params.py
-tests/test_checks.py
-tests/test_config.py
-tests/test_content_type_headers.py
-tests/test_filters.py
-tests/test_gegevensgroepen.py
-tests/test_get_resource.py
-tests/test_jwt_decoding.py
-tests/test_jwtsecrets.py
-tests/test_nested_serializer_validation.py
-tests/test_permissions.py
-tests/test_publish_validator.py
-tests/test_schema_root_tags.py
-tests/test_server_errors.py
-tests/test_utils.py
-tests/test_validators.py
 vng_api_common/__init__.py
 vng_api_common/admin.py
 vng_api_common/apps.py
 vng_api_common/checks.py
 vng_api_common/client.py
 vng_api_common/compat.py
 vng_api_common/constants.py
```

### Comparing `commonground-api-common-1.10.2/commonground_api_common.egg-info/requires.txt` & `commonground-api-common-1.9.0/commonground_api_common.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-django<4.2,>=3.2.0
+django>=3.2.0
 django-choices
 django-filter>=2.0
 django-solo
 djangorestframework~=3.12.0
 djangorestframework_camel_case>=1.2.0
 django-rest-framework-condition
 drf-yasg>=1.20.0
 drf-nested-routers>=0.93.3
 gemma-zds-client>=0.14.0
 iso-639
 isodate
-notifications-api-common>=0.2.2
+notifications-api-common
 oyaml
 PyJWT>=2.0.0
 pyyaml
 requests
 
 [coverage]
 pytest-cov
```

### Comparing `commonground-api-common-1.10.2/setup.cfg` & `commonground-api-common-1.9.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [metadata]
 name = commonground-api-common
-version = 1.10.2
+version = 1.9.0
 description = Commonground API tooling
 long_description = file: README.rst
 url = https://github.com/maykinmedia/commonground-api-common
 license = EUPL 1.2
 author = Maykin Media, VNG-Realisatie
 author_email = support@maykinmedia.nl
 keywords = openapi, swagger, django
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 3.2
-	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Operating System :: Unix
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
@@ -27,30 +26,33 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 scripts = 
 	bin/generate_schema
+	bin/generate_schema.cmd
 	bin/patch_content_types
+	bin/patch_content_types.cmd
 	bin/use_external_components
+	bin/use_external_components.cmd
 install_requires = 
-	django>=3.2.0,<4.2
+	django>=3.2.0
 	django-choices
 	django-filter>=2.0
 	django-solo
 	djangorestframework~=3.12.0
 	djangorestframework_camel_case>=1.2.0
 	django-rest-framework-condition
 	drf-yasg>=1.20.0
 	drf-nested-routers>=0.93.3
 	gemma-zds-client>=0.14.0
 	iso-639
 	isodate
-	notifications-api-common>=0.2.2
+	notifications-api-common
 	oyaml
 	PyJWT>=2.0.0
 	pyyaml
 	requests
 tests_require = 
 	pytest
 	pytest-django
@@ -59,15 +61,16 @@
 	isort
 	black
 	requests-mock
 	freezegun
 
 [options.packages.find]
 include = 
-	vng_api_common*
+	vng_api_common
+	vng_api_common.*
 
 [options.extras_require]
 markdown_docs = 
 	django-markup<=1.3
 	markdown
 tests = 
 	psycopg2
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/admin.py` & `commonground-api-common-1.9.0/vng_api_common/admin.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/api/permissions.py` & `commonground-api-common-1.9.0/vng_api_common/api/permissions.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/apps.py` & `commonground-api-common-1.9.0/vng_api_common/apps.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/api/serializers.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/api/serializers.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0001_initial.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import django.contrib.postgres.fields.jsonb
 import django.core.serializers.json
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="AuditTrail",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0002_auto_20190516_0830.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0002_auto_20190516_0830.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-05-16 08:30
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0001_initial")]
 
     operations = [
         migrations.AddField(
             model_name="audittrail",
             name="applicatie_id",
             field=models.CharField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0003_auto_20190517_0844.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0003_auto_20190517_0844.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import django.contrib.postgres.fields.jsonb
 import django.core.serializers.json
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0002_auto_20190516_0830")]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
             name="aanmaakdatum",
             field=models.DateTimeField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0004_auto_20190520_1238.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0004_auto_20190520_1238.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-05-20 12:38
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0003_auto_20190517_0844")]
 
     operations = [
         migrations.AddField(
             model_name="audittrail",
             name="gebruikers_id",
             field=models.CharField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0005_auto_20190520_1450.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0005_auto_20190520_1450.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 2.0.13 on 2019-05-20 14:50
 
 import django.core.validators
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0004_auto_20190520_1238")]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
             name="bron",
             field=models.CharField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0006_audittrail_toelichting.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0006_audittrail_toelichting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-05-21 08:22
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0005_auto_20190520_1450")]
 
     operations = [
         migrations.AddField(
             model_name="audittrail",
             name="toelichting",
             field=models.CharField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0007_auto_20190522_0916.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0007_auto_20190522_0916.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-05-22 09:16
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0006_audittrail_toelichting")]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
             name="toelichting",
             field=models.TextField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0008_audittrail_resource_weergave.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0008_audittrail_resource_weergave.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.2 on 2019-06-06 12:04
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0007_auto_20190522_0916")]
 
     operations = [
         migrations.AddField(
             model_name="audittrail",
             name="resource_weergave",
             field=models.CharField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0009_auto_20190712_1643.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0009_auto_20190712_1643.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import django.contrib.postgres.fields.jsonb
 import django.core.serializers.json
 import django.core.validators
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0008_audittrail_resource_weergave")]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
             name="aanmaakdatum",
             field=models.DateTimeField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0010_audittrail_request_id.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0006_auto_20190417_1142.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-# Generated by Django 2.1.1 on 2019-08-19 12:01
+# Generated by Django 2.0.13 on 2019-04-17 11:42
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-    dependencies = [("audittrails", "0009_auto_20190712_1643")]
+
+    dependencies = [("notifications", "0005_fix_default_nrc")]
 
     operations = [
-        migrations.AddField(
-            model_name="audittrail",
-            name="request_id",
-            field=models.CharField(
-                blank=True,
-                help_text='Een globaal "request" ID om een verzoek door het netwerk heen te traceren.',
-                max_length=255,
+        migrations.RemoveField(model_name="notificationsconfig", name="client_id"),
+        migrations.RemoveField(model_name="notificationsconfig", name="secret"),
+        migrations.AlterField(
+            model_name="notificationsconfig",
+            name="api_root",
+            field=models.URLField(
+                default="https://ref.tst.vng.cloud/nrc/api/v1",
+                unique=True,
+                verbose_name="api root",
             ),
-        )
+        ),
     ]
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0011_auto_20190918_1335.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0011_auto_20190918_1335.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import django.contrib.postgres.indexes
 from django.contrib.postgres.operations import TrigramExtension
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0010_audittrail_request_id")]
 
     operations = [
         TrigramExtension(),
         migrations.AddIndex(
             model_name="audittrail",
             index=django.contrib.postgres.indexes.GinIndex(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0012_auto_20200619_0545.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0012_auto_20200619_0545.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.6 on 2020-06-19 05:45
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0011_auto_20190918_1335"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0013_audittrail_logrecord_id.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0013_audittrail_logrecord_id.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.db import migrations, models
 
 from ._operations import AddField
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0012_remove_audittrail_request_id"),
     ]
 
     operations = [
         AddField(
             model_name="audittrail",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0013_auto_20201207_0846.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0013_auto_20201207_0846.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.8 on 2020-12-07 08:46
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0012_auto_20200619_0545"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0014_auto_20201221_0905.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0014_auto_20201221_0905.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.db import migrations, models
 
 from ._operations import AddField, RemoveField
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0013_auto_20201207_0846"),
     ]
 
     operations = [
         RemoveField(
             model_name="audittrail",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0014_auto_20210323_1654.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0014_auto_20210323_1654.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.17 on 2021-03-23 16:54
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0013_audittrail_logrecord_id"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0015_auto_20220318_1608.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0015_auto_20220318_1608.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.27 on 2022-03-18 16:08
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0014_auto_20201221_0905"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0017_alter_audittrail_bron.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0017_alter_audittrail_bron.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.14 on 2022-07-26 08:41
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0016_merge_20220607_0517"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/0018_auto_20221212_0745.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0018_auto_20221212_0745.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.2.16 on 2022-12-12 07:45
 
 import django.core.serializers.json
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0017_alter_audittrail_bron"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/migrations/_operations.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/_operations.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/models.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/models.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/audittrails/viewsets.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/viewsets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
-from typing import Optional
 
 from django.db import transaction
 from django.http import Http404
 
-from rest_framework import serializers, viewsets
+from rest_framework import viewsets
 
 from ..compat import get_header
 from ..constants import CommonResourceAction
 from ..permissions import AuthScopesRequired
 from ..utils import get_uuid_from_path
 from ..viewsets import NestedViewSetMixin
 from .api.scopes import SCOPE_AUDITTRAILS_LEZEN
@@ -88,44 +87,33 @@
             oud=version_before_edit,
             nieuw=version_after_edit,
         )
         trail.save()
 
 
 class AuditTrailCreateMixin(AuditTrailMixin):
-    _audittrail_serializer: Optional[serializers.Serializer] = None
-
     def get_audittrail_instance(self, response):
-        if self._audittrail_serializer is not None:
-            return self._audittrail_serializer.instance
         zaak_uuid = get_uuid_from_path(response.data["url"])
         instance = self.get_queryset().get(uuid=zaak_uuid)
         return instance
 
-    def perform_create(self, serializer):
-        super().perform_create(serializer)
-        # cache for future re-use
-        self._audittrail_serializer = serializer
-
     def create(self, request, *args, **kwargs):
         response = super().create(request, *args, **kwargs)
         instance = self.get_audittrail_instance(response)
         self.create_audittrail(
             response.status_code,
             CommonResourceAction.create,
             version_before_edit=None,
             version_after_edit=response.data,
             unique_representation=instance.unique_representation(),
         )
         return response
 
 
 class AuditTrailUpdateMixin(AuditTrailMixin):
-    # TODO: cache serializer(s) via perform_update?
-
     def update(self, request, *args, **kwargs):
         # Retrieve the data stored in the object before updating
         instance = self.get_object()
         serializer = self.get_serializer(instance)
         version_before_edit = serializer.data
 
         action = (
@@ -142,16 +130,14 @@
             version_after_edit=response.data,
             unique_representation=instance.unique_representation(),
         )
         return response
 
 
 class AuditTrailDestroyMixin(AuditTrailMixin):
-    # TODO: cache serializer(s) via perform_update?
-
     def destroy(self, request, *args, **kwargs):
         # Retrieve the data stored in the object before updating
         instance = self.get_object()
         serializer = self.get_serializer(instance)
         version_before_edit = serializer.data
 
         # If the resource being deleted is the main resource, delete all the
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/admin.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/admin.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0001_initial.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from django.db import migrations, models
 
 import vng_api_common.fields
 import vng_api_common.models
 
 
 class Migration(migrations.Migration):
+
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="Applicatie",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0002_authorizationsconfig.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0002_authorizationsconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.1.8 on 2019-05-02 04:04
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0001_initial")]
 
     operations = [
         migrations.CreateModel(
             name="AuthorizationsConfig",
             fields=[
                 (
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0003_auto_20190502_0409.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0003_auto_20190502_0409.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.1.8 on 2019-05-02 04:09
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0002_authorizationsconfig")]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
             name="api_root",
             field=models.URLField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0004_auto_20190503_0941.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0004_auto_20190503_0941.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.db import migrations, models
 
 import vng_api_common.fields
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0003_auto_20190502_0409")]
 
     operations = [
         migrations.AlterField(
             model_name="autorisatie",
             name="max_vertrouwelijkheidaanduiding",
             field=vng_api_common.fields.VertrouwelijkheidsAanduidingField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0005_auto_20190506_0842.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0005_auto_20190506_0842.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.1.8 on 2019-05-06 08:42
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0004_auto_20190503_0941")]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
             name="component",
             field=models.CharField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0006_auto_20190506_0901.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0006_auto_20190506_0901.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import django.db.models.deletion
 from django.db import migrations, models
 
 import vng_api_common.fields
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0005_auto_20190506_0842")]
 
     operations = [
         migrations.AlterField(
             model_name="applicatie",
             name="client_ids",
             field=django.contrib.postgres.fields.ArrayField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0007_auto_20190506_1212.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0007_auto_20190506_1212.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.1.8 on 2019-05-06 12:12
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0006_auto_20190506_0901")]
 
     operations = [
         migrations.AddField(
             model_name="autorisatie",
             name="besluittype",
             field=models.URLField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0008_auto_20190712_1541.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0008_auto_20190712_1541.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.db import migrations, models
 
 import vng_api_common.fields
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0007_auto_20190506_1212")]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
             name="component",
             field=models.CharField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0009_update_enums.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0009_update_enums.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,10 +15,11 @@
         max_vertrouwelijkheidaanduiding=Lower(
             Replace(F("max_vertrouwelijkheidaanduiding"), Value(" "), Value("_"))
         ),
     )
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0008_auto_20190712_1541")]
 
     operations = [migrations.RunPython(forward, migrations.RunPython.noop)]
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0010_auto_20190712_1643.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0010_auto_20190712_1643.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.2 on 2019-07-12 14:43
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0009_update_enums")]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
             name="api_root",
             field=models.URLField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0011_auto_20191114_0728.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0011_auto_20191114_0728.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     def patch_scope(self, scope: str) -> str:
         if not scope.startswith(f"{self.old}."):
             return scope
         return scope.replace(f"{self.old}.", f"{self.new}.", 1)
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("authorizations", "0010_auto_20190712_1643"),
     ]
 
     operations = [
         migrations.RunPython(
             Renamer("zaaktypes", "catalogi"),
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0012_auto_20200619_0545.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0012_auto_20200619_0545.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.6 on 2020-06-19 05:45
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("authorizations", "0011_auto_20191114_0728"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0013_auto_20201207_0846.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0013_auto_20201207_0846.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.8 on 2020-12-07 08:46
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("authorizations", "0012_auto_20200619_0545"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0014_auto_20201221_0905.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0014_auto_20201221_0905.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.14 on 2020-12-21 09:05
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("authorizations", "0013_auto_20201207_0846"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/migrations/0015_auto_20220318_1608.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0015_auto_20220318_1608.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.27 on 2022-03-18 16:08
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("authorizations", "0014_auto_20201221_0905"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/models.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/models.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/serializers.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/serializers.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/authorizations/validators.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/validators.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/caching/__init__.py` & `commonground-api-common-1.9.0/vng_api_common/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/caching/decorators.py` & `commonground-api-common-1.9.0/vng_api_common/caching/decorators.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/caching/introspection.py` & `commonground-api-common-1.9.0/vng_api_common/caching/introspection.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/caching/models.py` & `commonground-api-common-1.9.0/vng_api_common/caching/models.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/caching/registry.py` & `commonground-api-common-1.9.0/vng_api_common/caching/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,41 +55,31 @@
     @property
     def affected_model(self) -> ModelBase:
         return self.field.model
 
     def __hash__(self):
         return hash(self.field)
 
-    def get_related_objects(
-        self,
-        instance: models.Model,
-        is_delete: bool = False,
-    ) -> Iterable[models.Model]:
+    def get_related_objects(self, instance: models.Model) -> Iterable[models.Model]:
         assert isinstance(
             instance, self.source_model
         ), "Instance is not of expected model class"
 
         reverse_relation_field = self.field.remote_field
 
         try:
             if isinstance(reverse_relation_field, ForeignObjectRel):
-                on_delete = self.field.remote_field.on_delete
                 query_like = getattr(
                     instance, reverse_relation_field.get_accessor_name()
                 )
             else:
-                on_delete = self.field.on_delete
                 query_like = getattr(instance, reverse_relation_field.name)
         except ObjectDoesNotExist:  # nullable OneToOneField, for example
             return []
 
-        if is_delete and on_delete is models.CASCADE:
-            # no point in trying to update records that will be cascade deleted
-            return []
-
         # reverse FK or m2m
         if isinstance(query_like, (models.Manager, models.QuerySet)):
             related_objects = query_like.all()
         # one-to-one field or FK
         else:
             related_objects = [query_like] if query_like is not None else []
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/caching/signals.py` & `commonground-api-common-1.9.0/vng_api_common/caching/signals.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,32 +15,30 @@
 from django.dispatch import receiver
 
 from .etags import EtagUpdate
 from .registry import DEPENDENCY_REGISTRY, Dependency
 
 
 def mark_affected_objects(
-    dependencies: Optional[Set[Dependency]],
-    instance: models.Model,
-    is_delete: bool = False,
+    dependencies: Optional[Set[Dependency]], instance: models.Model
 ):
     if dependencies is None:
         return
 
     for dependency in dependencies:
         if not is_etag_model(dependency.affected_model):
             continue
 
-        for obj in dependency.get_related_objects(instance, is_delete=is_delete):
+        for obj in dependency.get_related_objects(instance):
             EtagUpdate.mark_affected(obj)
 
 
 @receiver([post_save, post_delete])
 def mark_related_instances_for_etag_update(
-    sender: ModelBase, instance: models.Model, signal, **kwargs
+    sender: ModelBase, instance: models.Model, **kwargs
 ) -> None:
     """
     Determine which instances are affected by changes in ``instance``.
 
     The sender/instance may be a model supporting ETag-based caching, or may be related
     to such a model. We must determine which instances are affected and ensure that
     the ETag value is properly scheduled for re-computation based on the new data.
@@ -53,21 +51,20 @@
         return
 
     # prevent infinite recursion caused by the save of the new _etag value
     if kwargs.get("update_fields") == {"_etag"}:
         return
 
     # if the model is itself something that has an etag, mark it for update
-    is_delete = signal is post_delete
-    if is_etag_model(sender) and not is_delete:
+    if is_etag_model(sender) and not kwargs["signal"] is post_delete:
         EtagUpdate.mark_affected(instance)
 
     # otherwise, find out which relations are affected
     dependency_for = DEPENDENCY_REGISTRY.get(sender)
-    mark_affected_objects(dependency_for, instance, is_delete=is_delete)
+    mark_affected_objects(dependency_for, instance)
 
 
 @receiver(m2m_changed)
 def mark_m2m_related_instances_for_etag_update(
     sender: ModelBase,
     instance: models.Model,
     action: str,
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/checks.py` & `commonground-api-common-1.9.0/vng_api_common/checks.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/client.py` & `commonground-api-common-1.9.0/vng_api_common/client.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/compat.py` & `commonground-api-common-1.9.0/vng_api_common/compat.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/conf/api.py` & `commonground-api-common-1.9.0/vng_api_common/conf/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,9 +106,7 @@
 NOTIFICATIONS_DISABLED = False
 
 vng_repo = "VNG-Realisatie/vng-api-common"
 vng_branch = "ref-responses"
 COMMON_SPEC = f"https://raw.githubusercontent.com/{vng_repo}/feature/{vng_branch}/vng_api_common/schemas/common.yaml"
 
 JWT_LEEWAY = 0  # default in PyJWT
-
-COMMONGROUND_API_COMMON_GET_DOMAIN = "vng_api_common.utils.get_site_domain"
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/constants.py` & `commonground-api-common-1.9.0/vng_api_common/constants.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/db/operations.py` & `commonground-api-common-1.9.0/vng_api_common/db/operations.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/descriptors.py` & `commonground-api-common-1.9.0/vng_api_common/descriptors.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/doc.py` & `commonground-api-common-1.9.0/vng_api_common/doc.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/exception_handling.py` & `commonground-api-common-1.9.0/vng_api_common/exception_handling.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/exceptions.py` & `commonground-api-common-1.9.0/vng_api_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/fields.py` & `commonground-api-common-1.9.0/vng_api_common/fields.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/filters.py` & `commonground-api-common-1.9.0/vng_api_common/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from .utils import NotAViewSet, get_resource_for_path
 from .validators import validate_rsin
 
 logger = logging.getLogger(__name__)
 
 
 class Backend(DjangoFilterBackend):
+
     # Taken from drf_yasg.inspectors.field.CamelCaseJSONFilter
     def _is_camel_case(self, view):
         return any(
             issubclass(parser, CamelCaseJSONParser) for parser in view.parser_classes
         ) or any(
             issubclass(renderer, CamelCaseJSONRenderer)
             for renderer in view.renderer_classes
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/filtersets.py` & `commonground-api-common-1.9.0/vng_api_common/filtersets.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/generators.py` & `commonground-api-common-1.9.0/vng_api_common/generators.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/geo.py` & `commonground-api-common-1.9.0/vng_api_common/geo.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/inspectors/cache.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/cache.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/inspectors/fields.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/fields.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/inspectors/files.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/files.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/inspectors/geojson.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/geojson.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/inspectors/polymorphic.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/polymorphic.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/inspectors/query.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 from django.db import models
-
-try:
-    from django.utils.encoding import force_str
-except ImportError:  # Django < 4.0
-    from django.utils.encoding import force_text as force_str
-
+from django.utils.encoding import force_text
 from django.utils.translation import gettext as _
 
 from django_filters.filters import BaseCSVFilter, ChoiceFilter
 from drf_yasg import openapi
 from drf_yasg.inspectors.query import CoreAPICompatInspector
 from rest_framework.filters import OrderingFilter
 
@@ -73,15 +68,15 @@
                     parameter.enum = [
                         choice[0] for choice in filter_field.extra["choices"]
                     ]
                 elif model_field and isinstance(model_field, models.URLField):
                     parameter.format = openapi.FORMAT_URI
 
                 if not parameter.description and help_text:
-                    parameter.description = force_str(help_text)
+                    parameter.description = force_text(help_text)
 
                 if "max_length" in filter_field.extra:
                     parameter.max_length = filter_field.extra["max_length"]
                 if "min_length" in filter_field.extra:
                     parameter.min_length = filter_field.extra["min_length"]
 
         return fields
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/inspectors/utils.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/utils.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/inspectors/view.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/view.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/locale/nl/LC_MESSAGES/django.mo` & `commonground-api-common-1.9.0/vng_api_common/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/locale/nl/LC_MESSAGES/django.po` & `commonground-api-common-1.9.0/vng_api_common/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/management/commands/generate_autorisaties.py` & `commonground-api-common-1.9.0/vng_api_common/management/commands/generate_autorisaties.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/management/commands/generate_notificaties.py` & `commonground-api-common-1.9.0/vng_api_common/management/commands/generate_notificaties.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/management/commands/generate_swagger.py` & `commonground-api-common-1.9.0/vng_api_common/management/commands/generate_swagger.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/management/commands/patch_error_contenttypes.py` & `commonground-api-common-1.9.0/vng_api_common/management/commands/patch_error_contenttypes.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/management/commands/use_external_components.py` & `commonground-api-common-1.9.0/vng_api_common/management/commands/use_external_components.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/middleware.py` & `commonground-api-common-1.9.0/vng_api_common/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,14 +211,15 @@
             for autorisatie in autorisaties:
                 scopes_provided.update(autorisatie.scopes)
 
         return scopes.is_contained_in(list(scopes_provided))
 
 
 class AuthMiddleware:
+
     header = "HTTP_AUTHORIZATION"
     auth_type = "Bearer"
 
     def __init__(self, get_response=None):
         self.get_response = get_response
 
     def __call__(self, request):
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/migrations/0001_initial.py` & `commonground-api-common-1.9.0/vng_api_common/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.6 on 2018-11-05 15:27
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="JWTSecret",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/migrations/0002_apicredential.py` & `commonground-api-common-1.9.0/vng_api_common/migrations/0002_apicredential.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.6 on 2018-11-19 11:09
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("vng_api_common", "0001_initial")]
 
     operations = [
         migrations.CreateModel(
             name="APICredential",
             fields=[
                 (
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/migrations/0003_auto_20190417_1145.py` & `commonground-api-common-1.9.0/vng_api_common/migrations/0003_auto_20190417_1145.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-04-17 11:45
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("vng_api_common", "0002_apicredential")]
 
     operations = [
         migrations.AlterModelOptions(
             name="apicredential",
             options={
                 "verbose_name": "external API credential",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/migrations/0004_auto_20190517_0903.py` & `commonground-api-common-1.9.0/vng_api_common/migrations/0004_auto_20190517_0903.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-05-17 09:03
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("vng_api_common", "0003_auto_20190417_1145")]
 
     operations = [
         migrations.AddField(
             model_name="apicredential",
             name="user_id",
             field=models.CharField(default="", max_length=255, verbose_name="user id"),
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/migrations/0005_auto_20190614_1346.py` & `commonground-api-common-1.9.0/vng_api_common/migrations/0005_auto_20190614_1346.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.1.1 on 2019-06-14 13:46
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("vng_api_common", "0004_auto_20190517_0903")]
 
     operations = [
         migrations.AlterField(
             model_name="apicredential",
             name="api_root",
             field=models.URLField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/mocks.py` & `commonground-api-common-1.9.0/vng_api_common/mocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
         return self.data.get(resource)[index]
 
     def create(self, resource: str, *args, **kwargs):
         return self.data.get(resource, {})
 
 
 class ZTCMockClient(MockClient):
+
     data = {
         "statustype": [
             {
                 "url": "https://ztc/api/v1/catalogussen/{catalogus_uuid}/zaaktypen/{zaaktype_uuid}/statustypen/{uuid}",
                 "volgnummer": 1,
                 "isEindstatus": False,
             },
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/models.py` & `commonground-api-common-1.9.0/vng_api_common/models.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/notifications/api/views.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/api/views.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/notifications/handlers.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/handlers.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0001_initial.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import django.contrib.postgres.fields
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="NotificationsConfig",
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0002_subscription__subscription.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0002_subscription__subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-03-12 10:36
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("notifications", "0001_initial")]
 
     operations = [
         migrations.AddField(
             model_name="subscription",
             name="_subscription",
             field=models.URLField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0003_auto_20190319_1048.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0003_auto_20190319_1048.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.1.1 on 2019-03-19 09:48
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("notifications", "0002_subscription__subscription")]
 
     operations = [
         migrations.RenameField(
             model_name="notificationsconfig", old_name="location", new_name="api_root"
         ),
         migrations.AddField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0004_auto_20190325_1313.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0004_auto_20190325_1313.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-03-25 13:13
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("notifications", "0003_auto_20190319_1048")]
 
     operations = [
         migrations.AlterField(
             model_name="notificationsconfig",
             name="api_root",
             field=models.URLField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0005_fix_default_nrc.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0005_fix_default_nrc.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,11 @@
 
     if config.api_root == "https://ref.tst.vng.cloud/nc/api/v1":
         config.api_root = "https://ref.tst.vng.cloud/nrc/api/v1"
         config.save()
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("notifications", "0004_auto_20190325_1313")]
 
     operations = [migrations.RunPython(fix_config, migrations.RunPython.noop)]
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0006_auto_20190417_1142.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0009_auto_20190729_0427.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Generated by Django 2.0.13 on 2019-04-17 11:42
+# Generated by Django 2.1.8 on 2019-07-29 04:27
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-    dependencies = [("notifications", "0005_fix_default_nrc")]
+
+    dependencies = [("notifications", "0008_auto_20190502_0415")]
 
     operations = [
-        migrations.RemoveField(model_name="notificationsconfig", name="client_id"),
-        migrations.RemoveField(model_name="notificationsconfig", name="secret"),
         migrations.AlterField(
             model_name="notificationsconfig",
             name="api_root",
             field=models.URLField(
-                default="https://ref.tst.vng.cloud/nrc/api/v1",
+                default="https://notificaties-api.vng.cloud/api/v1/",
                 unique=True,
                 verbose_name="api root",
             ),
-        ),
+        )
     ]
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0008_auto_20190502_0415.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0008_auto_20190502_0415.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.1.8 on 2019-05-02 04:15
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("notifications", "0007_auto_20190429_1442")]
 
     operations = [
         migrations.AlterField(
             model_name="notificationsconfig",
             name="api_root",
             field=models.URLField(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/notifications/migrations/0010_auto_20220704_1419.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0010_auto_20220704_1419.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
             )
         old_subscriptions.delete()
 
     return migrate_data
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("notifications", "0009_auto_20190729_0427"),
         ("notifications_api_common", "0001_initial"),
     ]
 
     operations = [
         migrations.RunPython(
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/notifications/models.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/models.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/oas.py` & `commonground-api-common-1.9.0/vng_api_common/oas.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/permissions.py` & `commonground-api-common-1.9.0/vng_api_common/permissions.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/polymorphism.py` & `commonground-api-common-1.9.0/vng_api_common/polymorphism.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/routers.py` & `commonground-api-common-1.9.0/vng_api_common/routers.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/schema.py` & `commonground-api-common-1.9.0/vng_api_common/schema.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/scopes.py` & `commonground-api-common-1.9.0/vng_api_common/scopes.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/search.py` & `commonground-api-common-1.9.0/vng_api_common/search.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/serializers.py` & `commonground-api-common-1.9.0/vng_api_common/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,35 +238,34 @@
     Usage: include the mixin on the ModelSerializer that has gegevensgroepen.
     """
 
     def _is_gegevensgroep(self, name: str):
         attr = getattr(self.Meta.model, name)
         return isinstance(attr, GegevensGroepType)
 
+    @transaction.atomic
     def create(self, validated_data):
         """
         Handle nested writes.
         """
         gegevensgroepen = {}
+
         for name in list(validated_data.keys()):
             if not self._is_gegevensgroep(name):
                 continue
 
             gegevensgroepen[name] = validated_data.pop(name)
 
-        # avoid a number of queries if there's no gegevensgroep actions to perform
-        if not gegevensgroepen:
-            return super().create(validated_data)
-
-        with transaction.atomic():
-            # perform the default create
-            obj = super().create(validated_data)
-            for name, gegevensgroepdata in gegevensgroepen.items():
-                setattr(obj, name, gegevensgroepdata)
-            obj.save()
+        # perform the default create
+        obj = super().create(validated_data)
+
+        for name, gegevensgroepdata in gegevensgroepen.items():
+            setattr(obj, name, gegevensgroepdata)
+
+        obj.save()
 
         return obj
 
     def update(self, instance, validated_data):
         """
         Handle nested writes.
         """
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/css/admin/admin_overrides.css` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/css/admin/admin_overrides.css`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/img/vng.svg` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/img/vng.svg`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/LICENSE.txt` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css.map` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css.map` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css.map` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css.map` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css.map` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css.map` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js.map` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js.map` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js.map` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js.map` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/LICENSE.txt` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.css` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.css`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.min.css` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.eot` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.svg` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.ttf` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff2` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.eot` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.svg` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.ttf` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff2` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.eot` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.svg` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.ttf` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff2` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/jquery/LICENSE.txt` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/jquery/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.js` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.js`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.min.js` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/popper/LICENSE.md` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/popper/LICENSE.md`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/popper/popper.js` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/popper/popper.js`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/static/vng_api_common/libs/popper/popper.min.js` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/popper/popper.min.js`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/admin/base_site.html` & `commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/api_schema_to_markdown_table.md` & `commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/api_schema_to_markdown_table.md`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/index.html` & `commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/index.html`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/master.html` & `commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/master.html`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/notificaties.md` & `commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/notificaties.md`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/ref/error_detail.html` & `commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/ref/error_detail.html`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/ref/scopes.html` & `commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/ref/scopes.html`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/templates/vng_api_common/view_config.html` & `commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/view_config.html`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/templatetags/vng_api_common.py` & `commonground-api-common-1.9.0/vng_api_common/templatetags/vng_api_common.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/tests/auth.py` & `commonground-api-common-1.9.0/vng_api_common/tests/auth.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/tests/caching.py` & `commonground-api-common-1.9.0/vng_api_common/tests/caching.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/tests/schema.py` & `commonground-api-common-1.9.0/vng_api_common/tests/schema.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/tests/urls.py` & `commonground-api-common-1.9.0/vng_api_common/tests/urls.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/utils.py` & `commonground-api-common-1.9.0/vng_api_common/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import logging
 import re
 import uuid
 from typing import TYPE_CHECKING, List, Optional, Union
 
 from django.apps import apps
 from django.conf import settings
-from django.core.exceptions import ImproperlyConfigured
 from django.db import models
 from django.http import HttpRequest
 from django.urls import Resolver404, ResolverMatch, get_resolver, get_script_prefix
 from django.utils.encoding import smart_str
-from django.utils.module_loading import import_string
 
 from rest_framework.utils import formatting
 from zds_client.client import ClientError
 
 from .client import get_client
 
 try:
@@ -210,22 +208,23 @@
     model_name = getattr(model, "IDENTIFICATIE_PREFIX", model._meta.model_name.upper())
 
     year = getattr(instance, date_field_name).year
     prefix = f"{model_name}-{year}"
 
     pattern = prefix + r"-\d{10}"
 
-    # ⚡ start_with is added to use index in DB query
-    issued_ids_for_year = model._default_manager.filter(
-        identificatie__startswith=prefix, identificatie__regex=pattern
-    )
-    max_id = issued_ids_for_year.aggregate(models.Max("identificatie"))[
-        "identificatie__max"
-    ]
-    number = int(max_id.split("-")[-1]) + 1 if max_id is not None else 1
+    issued_ids_for_year = model._default_manager.filter(identificatie__regex=pattern)
+
+    if issued_ids_for_year.exists():
+        max_id = issued_ids_for_year.aggregate(models.Max("identificatie"))[
+            "identificatie__max"
+        ]
+        number = int(max_id.split("-")[-1]) + 1
+    else:
+        number = 1
 
     padded_number = str(number).zfill(10)
     return f"{prefix}-{padded_number}"
 
 
 def get_help_text(model_string: str, field_name: str) -> str:
     ModelClass = apps.get_model(model_string, require_ready=False)
@@ -266,34 +265,7 @@
 
 def get_field_attribute(
     model_string: str, field_name: str, attr_name: str
 ) -> Optional[str]:
     ModelClass = apps.get_model(model_string, require_ready=False)
     field = ModelClass._meta.get_field(field_name)
     return getattr(field, attr_name, None)
-
-
-def get_domain() -> str:
-    """
-    Derive the domain where the application is hosted.
-    """
-    getter = import_string(settings.COMMONGROUND_API_COMMON_GET_DOMAIN)
-    return getter()
-
-
-def get_site_domain() -> str:
-    """
-    Derive the domain where the application is hosted.
-
-    You can provide an alternative implementation via the
-    ``COMMONGROUND_API_COMMON_GET_DOMAIN`` setting, which takes a dotted path to a
-    callable taking no arguments.
-    """
-    if not apps.is_installed("django.contrib.sites"):
-        raise ImproperlyConfigured(
-            "'django.contrib.sites' is not installed in INSTALLED_APPS"
-        )
-
-    from django.contrib.sites.models import Site
-
-    site = Site.objects.get_current()
-    return site.domain
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/validators.py` & `commonground-api-common-1.9.0/vng_api_common/validators.py`

 * *Files identical despite different names*

### Comparing `commonground-api-common-1.10.2/vng_api_common/views.py` & `commonground-api-common-1.9.0/vng_api_common/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import os
 from collections import OrderedDict
 
 from django.apps import apps
 from django.conf import settings
-from django.core.exceptions import ImproperlyConfigured
 from django.http import Http404, HttpRequest
 from django.utils.translation import gettext_lazy as _
 from django.views.generic import TemplateView
 
 import requests
 from rest_framework import exceptions as drf_exceptions, status
 from rest_framework.response import Response
@@ -16,15 +15,14 @@
 from zds_client import ClientError
 
 from . import exceptions
 from .compat import sentry_client
 from .constants import ComponentTypes
 from .exception_handling import HandledException
 from .scopes import SCOPE_REGISTRY
-from .utils import get_domain
 
 logger = logging.getLogger(__name__)
 
 ERROR_CONTENT_TYPE = "application/problem+json"
 
 
 def exception_handler(exc, context):
@@ -105,20 +103,23 @@
 
         context["config"] = config
 
         return context
 
 
 def _test_sites_config(request: HttpRequest) -> list:
-    try:
-        domain = get_domain()
-    except ImproperlyConfigured:
+    if not apps.is_installed("django.contrib.sites"):
         return []
+
+    from django.contrib.sites.models import Site
+
+    site = Site.objects.get_current()
+
     return [
-        (_("Site domain"), domain, request.get_host() == domain),
+        (_("Site domain"), site.domain, request.get_host() == site.domain),
         (_("HTTPS"), settings.IS_HTTPS, settings.IS_HTTPS == request.is_secure()),
     ]
 
 
 def _test_ac_config() -> list:
     if not apps.is_installed("vng_api_common.authorizations"):
         return []
```

### Comparing `commonground-api-common-1.10.2/vng_api_common/viewsets.py` & `commonground-api-common-1.9.0/vng_api_common/viewsets.py`

 * *Files identical despite different names*

