# Comparing `tmp/decentro-in-kyc-python-sdk-4.2.0.tar.gz` & `tmp/decentro-in-kyc-python-sdk-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/dylanhuang/Git/konfig-monorepo/customers/decentro/decentro-in-kyc-sdk/python/dist/.tmp-a85g6n1_/decentro-in-kyc-python-s", last modified: Wed Mar 29 00:38:03 2023, max compression
+gzip compressed data, was "/Users/dylanhuang/Git/konfig-monorepo/customers/decentro/decentro-in-kyc-sdk/python/dist/.tmp-s414k7q0/decentro-in-kyc-python-s", last modified: Thu Apr 20 19:33:43 2023, max compression
```

## Comparing `decentro-in-kyc-python-sdk-4.2.0.tar` & `decentro-in-kyc-python-sdk-4.3.0.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1081 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/LICENSE
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6433 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/PKG-INFO
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6129 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/README.md
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      824 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    63552 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/api_client.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      266 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/api_response.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      214 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2245 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/path_to_api.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/paths/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      249 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/paths/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      149 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/paths/kyc_public_registry_validate.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      133 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/paths/kyc_scan_extract_ocr.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      153 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/paths/v2_kyc_document_classification.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      146 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_face_match.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      152 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_image_quality.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      156 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_photocopy_check.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      154 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_video_liveness.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      159 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/paths/v2_kyc_identities_mask_aadhaar_uid.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      312 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/tag_to_api.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/tags/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      311 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/tags/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1147 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/tags/kyc_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      714 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/client.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    18943 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/configuration.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5669 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/exceptions.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2274 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/exceptions_base.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      356 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3998 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_image_quality400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5719 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_image_quality_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    39305 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_image_quality_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3992 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_photocopy400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5065 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_photocopy_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7404 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_photocopy_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4000 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_video_liveness400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5268 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_video_liveness_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7412 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_video_liveness_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3996 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/classify_document400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5964 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/classify_document_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7772 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/classify_document_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     8727 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/extract_text400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     8049 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/extract_text_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    14321 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/extract_text_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5059 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/mask_aadhaar_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     8525 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/mask_aadhaar_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3986 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/mask_aadhaar_uid_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3982 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/match_face400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6934 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/match_face_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7329 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/match_face_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     8177 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/validate400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6692 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/validate_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)   270536 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/validate_response.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/models/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2525 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/models/__init__.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      850 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/__init__.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      359 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    20141 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      343 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    17024 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      363 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    17133 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      357 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    16972 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      363 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    21426 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      367 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    17087 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      365 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12935 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      371 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12819 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/post.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      673 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/request_after_hook.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      674 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/request_before_hook.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    10705 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/rest.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    94541 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/schemas.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3178 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/validation_metadata.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_python_sdk.egg-info/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6433 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6428 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)        1 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)      139 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_python_sdk.egg-info/requires.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)       28 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)       69 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/setup.cfg
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1286 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/setup.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/test/
--rw-r--r--   0 dylanhuang   (501) staff       (20)    19452 2023-03-29 00:33:57.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_kyc_api.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      559 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_image_quality400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      543 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_image_quality_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      547 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_image_quality_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      546 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_photocopy400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      530 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_photocopy_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      534 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_photocopy_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      563 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_video_liveness400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      547 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_video_liveness_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      551 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_video_liveness_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      554 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_classify_document400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      538 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_classify_document_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      542 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_classify_document_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      534 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_extract_text400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      518 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_extract_text_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      522 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_extract_text_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      518 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_mask_aadhaar_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      522 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_mask_aadhaar_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      535 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_mask_aadhaar_uid_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      526 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_match_face400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      510 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_match_face_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      514 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_match_face_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      521 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_validate400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      505 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_validate_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      509 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_validate_response.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1984 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/__init__.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_kyc_public_registry_validate/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_kyc_public_registry_validate/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      760 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_kyc_public_registry_validate/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_kyc_scan_extract_ocr/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_kyc_scan_extract_ocr/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      740 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_kyc_scan_extract_ocr/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_document_classification/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_document_classification/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      773 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_document_classification/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_face_match/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_face_match/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      755 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_face_match/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_image_quality/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_image_quality/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      773 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_image_quality/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_photocopy_check/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_photocopy_check/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      775 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_photocopy_check/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_video_liveness/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_video_liveness/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      771 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_video_liveness/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:38:03.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_identities_mask_aadhaar_uid/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_identities_mask_aadhaar_uid/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      779 2023-03-29 00:26:48.000000 decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_identities_mask_aadhaar_uid/test_post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1081 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/LICENSE
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     6426 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/PKG-INFO
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     6122 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/README.md
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      824 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    63552 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/api_client.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      266 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/api_response.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      214 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     2245 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/path_to_api.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      249 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      149 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/kyc_public_registry_validate.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      133 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/kyc_scan_extract_ocr.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      153 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/v2_kyc_document_classification.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      146 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_face_match.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      152 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_image_quality.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      156 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_photocopy_check.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      154 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_video_liveness.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      159 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/v2_kyc_identities_mask_aadhaar_uid.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      312 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/tag_to_api.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/tags/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      311 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/tags/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1147 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/tags/kyc_api.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      714 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/client.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    18943 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/configuration.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     5669 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/exceptions.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     2274 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/exceptions_base.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      356 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3998 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_image_quality400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     5719 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_image_quality_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    39305 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_image_quality_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3992 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_photocopy400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     5065 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_photocopy_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     7404 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_photocopy_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     4000 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_video_liveness400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     5268 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_video_liveness_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     7412 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_video_liveness_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3996 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/classify_document400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     5964 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/classify_document_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     7772 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/classify_document_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     8727 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/extract_text400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     8049 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/extract_text_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    14321 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/extract_text_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     5059 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/mask_aadhaar_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3992 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/mask_aadhaar_uid400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     8531 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/mask_aadhaar_uid_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3982 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/match_face400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     6934 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/match_face_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     7329 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/match_face_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     8177 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/validate400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     6692 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/validate_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)   270536 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/validate_response.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/models/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     2538 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/models/__init__.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      850 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/__init__.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      359 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    20468 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      343 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    17351 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      363 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    17460 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      357 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    17299 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      363 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    21753 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      367 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    17414 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      365 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    13262 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      371 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    13165 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/post.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      673 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/request_after_hook.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      674 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/request_before_hook.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    10705 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/rest.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    95007 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/schemas.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     3178 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/validation_metadata.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_python_sdk.egg-info/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     6426 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     6442 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        1 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      139 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 dylanhuang   (501) staff       (20)       28 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 dylanhuang   (501) staff       (20)       69 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/setup.cfg
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1286 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/setup.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)    19452 2023-04-20 19:07:01.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_kyc_api.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      559 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_image_quality400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      543 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_image_quality_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      547 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_image_quality_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      546 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_photocopy400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      530 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_photocopy_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      534 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_photocopy_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      563 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_video_liveness400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      547 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_video_liveness_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      551 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_video_liveness_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      554 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_classify_document400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      538 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_classify_document_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      542 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_classify_document_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      534 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_extract_text400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      518 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_extract_text_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      522 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_extract_text_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      518 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_mask_aadhaar_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      547 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_mask_aadhaar_uid400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      535 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_mask_aadhaar_uid_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      526 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_match_face400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      510 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_match_face_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      514 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_match_face_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      521 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_validate400_response.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      505 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_validate_request.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      509 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_validate_response.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)     1984 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/__init__.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_kyc_public_registry_validate/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_kyc_public_registry_validate/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      760 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_kyc_public_registry_validate/test_post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_kyc_scan_extract_ocr/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_kyc_scan_extract_ocr/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      740 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_kyc_scan_extract_ocr/test_post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_document_classification/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_document_classification/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      773 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_document_classification/test_post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_face_match/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_face_match/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      755 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_face_match/test_post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_image_quality/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_image_quality/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      773 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_image_quality/test_post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_photocopy_check/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_photocopy_check/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      775 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_photocopy_check/test_post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_video_liveness/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_video_liveness/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      771 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_video_liveness/test_post.py
+drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_identities_mask_aadhaar_uid/
+-rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_identities_mask_aadhaar_uid/__init__.py
+-rw-r--r--   0 dylanhuang   (501) staff       (20)      779 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_identities_mask_aadhaar_uid/test_post.py
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/LICENSE` & `decentro-in-kyc-python-sdk-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/PKG-INFO` & `decentro-in-kyc-python-sdk-4.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: decentro-in-kyc-python-sdk
-Version: 4.2.0
+Version: 4.3.0
 Summary: decentro-in-kyc
 Home-page: https://decentro.tech
 Author: Decentro
 Author-email: admin@decentro.tech
 License: MIT
 Keywords: decentro-in-kyc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # decentro-in-kyc-python-sdk
 KYC & Onboarding
 
 - API version: 1.0.0
-- Package version: 4.2.0
+- Package version: 4.3.0
 For more information, please visit [https://decentro.tech](https://decentro.tech)
 
 ## Requirements.
 
 Python >=3.7
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install decentro-in-kyc-python-sdk==4.2.0
+pip install decentro-in-kyc-python-sdk==4.3.0
 ```
-(you may need to run `pip` with root permission: `sudo pip install decentro-in-kyc-python-sdk==4.2.0`)
+(you may need to run `pip` with root permission: `sudo pip install decentro-in-kyc-python-sdk==4.3.0`)
 
 Then import the package:
 ```python
 import decentro_in_kyc_client
 ```
 ## Getting Started
 
@@ -82,15 +82,15 @@
     pprint(check_image_quality_response.body["responseCode"])
     pprint(check_image_quality_response.body["message"])
     pprint(check_image_quality_response.body["data"])
     pprint(check_image_quality_response.headers)
     pprint(check_image_quality_response.status)
     pprint(check_image_quality_response.round_trip_time)
 except ApiException as e:
-    print("Exception when calling CheckImageQualityResponse.check_image_quality: %s\n" % e)
+    print("Exception when calling KYCApi.check_image_quality: %s\n" % e)
     pprint(e.body)
     if e.status == 400:
         pprint(e.body["decentroTxnId"])
         pprint(e.body["status"])
         pprint(e.body["responseCode"])
         pprint(e.body["message"])
     pprint(e.headers)
@@ -128,15 +128,15 @@
  - [ClassifyDocument400Response](docs/models/ClassifyDocument400Response.md)
  - [ClassifyDocumentRequest](docs/models/ClassifyDocumentRequest.md)
  - [ClassifyDocumentResponse](docs/models/ClassifyDocumentResponse.md)
  - [ExtractText400Response](docs/models/ExtractText400Response.md)
  - [ExtractTextRequest](docs/models/ExtractTextRequest.md)
  - [ExtractTextResponse](docs/models/ExtractTextResponse.md)
  - [MaskAadhaarRequest](docs/models/MaskAadhaarRequest.md)
- - [MaskAadhaarResponse](docs/models/MaskAadhaarResponse.md)
+ - [MaskAadhaarUid400Response](docs/models/MaskAadhaarUid400Response.md)
  - [MaskAadhaarUidResponse](docs/models/MaskAadhaarUidResponse.md)
  - [MatchFace400Response](docs/models/MatchFace400Response.md)
  - [MatchFaceRequest](docs/models/MatchFaceRequest.md)
  - [MatchFaceResponse](docs/models/MatchFaceResponse.md)
  - [Validate400Response](docs/models/Validate400Response.md)
  - [ValidateRequest](docs/models/ValidateRequest.md)
  - [ValidateResponse](docs/models/ValidateResponse.md)
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/README.md` & `decentro-in-kyc-python-sdk-4.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # decentro-in-kyc-python-sdk
 KYC & Onboarding
 
 - API version: 1.0.0
-- Package version: 4.2.0
+- Package version: 4.3.0
 For more information, please visit [https://decentro.tech](https://decentro.tech)
 
 ## Requirements.
 
 Python >=3.7
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install decentro-in-kyc-python-sdk==4.2.0
+pip install decentro-in-kyc-python-sdk==4.3.0
 ```
-(you may need to run `pip` with root permission: `sudo pip install decentro-in-kyc-python-sdk==4.2.0`)
+(you may need to run `pip` with root permission: `sudo pip install decentro-in-kyc-python-sdk==4.3.0`)
 
 Then import the package:
 ```python
 import decentro_in_kyc_client
 ```
 ## Getting Started
 
@@ -69,15 +69,15 @@
     pprint(check_image_quality_response.body["responseCode"])
     pprint(check_image_quality_response.body["message"])
     pprint(check_image_quality_response.body["data"])
     pprint(check_image_quality_response.headers)
     pprint(check_image_quality_response.status)
     pprint(check_image_quality_response.round_trip_time)
 except ApiException as e:
-    print("Exception when calling CheckImageQualityResponse.check_image_quality: %s\n" % e)
+    print("Exception when calling KYCApi.check_image_quality: %s\n" % e)
     pprint(e.body)
     if e.status == 400:
         pprint(e.body["decentroTxnId"])
         pprint(e.body["status"])
         pprint(e.body["responseCode"])
         pprint(e.body["message"])
     pprint(e.headers)
@@ -115,15 +115,15 @@
  - [ClassifyDocument400Response](docs/models/ClassifyDocument400Response.md)
  - [ClassifyDocumentRequest](docs/models/ClassifyDocumentRequest.md)
  - [ClassifyDocumentResponse](docs/models/ClassifyDocumentResponse.md)
  - [ExtractText400Response](docs/models/ExtractText400Response.md)
  - [ExtractTextRequest](docs/models/ExtractTextRequest.md)
  - [ExtractTextResponse](docs/models/ExtractTextResponse.md)
  - [MaskAadhaarRequest](docs/models/MaskAadhaarRequest.md)
- - [MaskAadhaarResponse](docs/models/MaskAadhaarResponse.md)
+ - [MaskAadhaarUid400Response](docs/models/MaskAadhaarUid400Response.md)
  - [MaskAadhaarUidResponse](docs/models/MaskAadhaarUidResponse.md)
  - [MatchFace400Response](docs/models/MatchFace400Response.md)
  - [MatchFaceRequest](docs/models/MatchFaceRequest.md)
  - [MatchFaceResponse](docs/models/MatchFaceResponse.md)
  - [Validate400Response](docs/models/Validate400Response.md)
  - [ValidateRequest](docs/models/ValidateRequest.md)
  - [ValidateResponse](docs/models/ValidateResponse.md)
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/__init__.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     KYC & Onboarding
 
     The version of the OpenAPI document: 1.0.0
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
-__version__ = "4.2.0"
+__version__ = "4.3.0"
 
 # import ApiClient
 from decentro_in_kyc_client.api_client import ApiClient
 
 # import Configuration
 from decentro_in_kyc_client.configuration import Configuration
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/api_client.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1066,15 +1066,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Konfig/4.2.0/python'
+        self.user_agent = 'Konfig/4.3.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/path_to_api.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/apis/tags/kyc_api.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/tags/kyc_api.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/client.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/client.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/configuration.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,15 +439,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 4.2.0".\
+               "SDK Package Version: 4.3.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/exceptions.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/exceptions_base.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_image_quality400_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_image_quality400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_image_quality_request.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_image_quality_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_image_quality_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_image_quality_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_photocopy400_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_photocopy400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_photocopy_request.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_photocopy_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_photocopy_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_photocopy_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_video_liveness400_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_video_liveness400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_video_liveness_request.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_video_liveness_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/check_video_liveness_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_video_liveness_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/classify_document400_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/classify_document400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/classify_document_request.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/classify_document_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/classify_document_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/classify_document_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/extract_text400_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/extract_text400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/extract_text_request.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/extract_text_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/extract_text_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/extract_text_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/mask_aadhaar_request.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/mask_aadhaar_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/mask_aadhaar_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/mask_aadhaar_uid_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from decentro_in_kyc_client import schemas  # noqa: F401
 
 
-class MaskAadhaarResponse(
+class MaskAadhaarUidResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated
     """
 
 
@@ -180,15 +180,15 @@
         data: typing.Union[MetaOapg.properties.data, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         decentroTxnId: typing.Union[MetaOapg.properties.decentroTxnId, str, schemas.Unset] = schemas.unset,
         message: typing.Union[MetaOapg.properties.message, str, schemas.Unset] = schemas.unset,
         responseCode: typing.Union[MetaOapg.properties.responseCode, str, schemas.Unset] = schemas.unset,
         status: typing.Union[MetaOapg.properties.status, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'MaskAadhaarResponse':
+    ) -> 'MaskAadhaarUidResponse':
         return super().__new__(
             cls,
             *args,
             data=data,
             decentroTxnId=decentroTxnId,
             message=message,
             responseCode=responseCode,
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/mask_aadhaar_uid_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/mask_aadhaar_uid400_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from decentro_in_kyc_client import schemas  # noqa: F401
 
 
-class MaskAadhaarUidResponse(
+class MaskAadhaarUid400Response(
     schemas.DictSchema
 ):
     """
     This class is auto generated
     """
 
 
@@ -90,15 +90,15 @@
         *args: typing.Union[dict, frozendict.frozendict, ],
         decentroTxnId: typing.Union[MetaOapg.properties.decentroTxnId, str, schemas.Unset] = schemas.unset,
         status: typing.Union[MetaOapg.properties.status, str, schemas.Unset] = schemas.unset,
         responseCode: typing.Union[MetaOapg.properties.responseCode, str, schemas.Unset] = schemas.unset,
         message: typing.Union[MetaOapg.properties.message, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'MaskAadhaarUidResponse':
+    ) -> 'MaskAadhaarUid400Response':
         return super().__new__(
             cls,
             *args,
             decentroTxnId=decentroTxnId,
             status=status,
             responseCode=responseCode,
             message=message,
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/match_face400_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/match_face400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/match_face_request.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/match_face_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/match_face_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/match_face_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/validate400_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/validate400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/validate_request.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/validate_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/model/validate_response.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/validate_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/models/__init__.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from decentro_in_kyc_client.model.classify_document400_response import ClassifyDocument400Response
 from decentro_in_kyc_client.model.classify_document_request import ClassifyDocumentRequest
 from decentro_in_kyc_client.model.classify_document_response import ClassifyDocumentResponse
 from decentro_in_kyc_client.model.extract_text400_response import ExtractText400Response
 from decentro_in_kyc_client.model.extract_text_request import ExtractTextRequest
 from decentro_in_kyc_client.model.extract_text_response import ExtractTextResponse
 from decentro_in_kyc_client.model.mask_aadhaar_request import MaskAadhaarRequest
-from decentro_in_kyc_client.model.mask_aadhaar_response import MaskAadhaarResponse
+from decentro_in_kyc_client.model.mask_aadhaar_uid400_response import MaskAadhaarUid400Response
 from decentro_in_kyc_client.model.mask_aadhaar_uid_response import MaskAadhaarUidResponse
 from decentro_in_kyc_client.model.match_face400_response import MatchFace400Response
 from decentro_in_kyc_client.model.match_face_request import MatchFaceRequest
 from decentro_in_kyc_client.model.match_face_response import MatchFaceResponse
 from decentro_in_kyc_client.model.validate400_response import Validate400Response
 from decentro_in_kyc_client.model.validate_request import ValidateRequest
 from decentro_in_kyc_client.model.validate_response import ValidateResponse
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/__init__.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/post.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from decentro_in_kyc_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -404,15 +405,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/post.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from decentro_in_kyc_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -313,15 +314,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/post.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/post.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from decentro_in_kyc_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -313,15 +314,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/post.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from decentro_in_kyc_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -313,15 +314,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/post.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from decentro_in_kyc_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -432,15 +433,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/post.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from decentro_in_kyc_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -313,15 +314,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/post.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from decentro_in_kyc_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -194,15 +195,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/post.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/post.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
+import json
 from urllib3._collections import HTTPHeaderDict
 
 from decentro_in_kyc_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -27,15 +28,15 @@
 
 import frozendict  # noqa: F401
 
 from decentro_in_kyc_client import schemas  # noqa: F401
 
 from decentro_in_kyc_client.model.mask_aadhaar_request import MaskAadhaarRequest
 from decentro_in_kyc_client.model.mask_aadhaar_uid_response import MaskAadhaarUidResponse
-from decentro_in_kyc_client.model.mask_aadhaar_response import MaskAadhaarResponse
+from decentro_in_kyc_client.model.mask_aadhaar_uid400_response import MaskAadhaarUid400Response
 
 from . import path
 
 # body param
 SchemaForRequestBodyMultipartFormData = MaskAadhaarRequest
 
 
@@ -46,15 +47,15 @@
     },
 )
 _auth = [
     'client_id',
     'client_secret',
     'module_secret',
 ]
-SchemaFor200ResponseBodyApplicationJson = MaskAadhaarResponse
+SchemaFor200ResponseBodyApplicationJson = MaskAadhaarUidResponse
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
     ]
@@ -63,15 +64,15 @@
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = MaskAadhaarUidResponse
+SchemaFor400ResponseBodyApplicationJson = MaskAadhaarUid400Response
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
     body: typing.Union[
         SchemaFor400ResponseBodyApplicationJson,
     ]
@@ -194,15 +195,18 @@
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                    response,
                                                    self.api_client.configuration,
                                                    skip_deserialization=skip_deserialization
                                                )
         else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
+                body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
 
         if not 200 <= api_response.status <= 299:
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/request_after_hook.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/request_before_hook.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/rest.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/rest.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/schemas.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,19 +225,19 @@
                              True if it is a key in a dict
                              False if our item is an item in a tuple
         """
         key_or_value = "value"
         if key_type:
             key_or_value = "key"
         valid_classes_phrase = cls.__get_valid_classes_phrase(valid_classes)
-        msg = "Invalid type. Required {1} type {2} and " "passed type was {3}".format(
-            var_name,
+        msg = "Invalid type. Required {0} type {1} and " "passed type was {2} for \"{3}\"".format(
             key_or_value,
             valid_classes_phrase,
             type(var_value).__name__,
+            var_name,
         )
         return msg
 
     @classmethod
     def __get_type_error(cls, var_value, path_to_item, valid_classes, key_type=False):
         error_msg = cls.__type_error_message(
             var_name=path_to_item[-1],
@@ -459,15 +459,15 @@
         if not __kwargs and args and not isinstance(args[0], dict):
             __arg = args[0]
         else:
             __arg = cls.__get_input_dict(*args, **__kwargs)
         __from_server = False
         __validated_path_to_schemas = {}
         __arg = cast_to_allowed_types(
-            __arg, __from_server, __validated_path_to_schemas)
+            __arg, __from_server, __validated_path_to_schemas, schema=cls)
         __validation_metadata = ValidationMetadata(
             configuration=_configuration, from_server=__from_server, validated_path_to_schemas=__validated_path_to_schemas)
         __path_to_schemas = cls.__get_new_cls(__arg, __validation_metadata)
         __new_cls = __path_to_schemas[__validation_metadata.path_to_item]
         return __new_cls._get_new_instance_without_conversion_oapg(
             __arg,
             __validation_metadata.path_to_item,
@@ -638,16 +638,16 @@
     class NoneTupleStrDecimalBoolMixin(NoneClass, tuple, str, decimal.Decimal, BoolClass):
         pass
     class FrozenDictTupleStrDecimalBoolMixin(frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass):
         pass
     # qty 6
     class NoneFrozenDictTupleStrDecimalBoolMixin(NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass):
         pass
-    # qty 8
-    class NoneFrozenDictTupleStrDecimalBoolFileBytesMixin(NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass, FileIO, bytes):
+    # qty 9
+    class NoneFrozenDictTupleStrIntDecimalBoolFileBytesMixin(NoneClass, frozendict.frozendict, tuple, str, int, decimal.Decimal, BoolClass, FileIO, bytes):
         pass
 else:
     # qty 1
     class NoneMixin:
         _types = {NoneClass}
     class FrozenDictMixin:
         _types = {frozendict.frozendict}
@@ -782,17 +782,17 @@
     class NoneTupleStrDecimalBoolMixin:
         _types = {NoneClass, tuple, str, decimal.Decimal, BoolClass}
     class FrozenDictTupleStrDecimalBoolMixin:
         _types = {frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass}
     # qty 6
     class NoneFrozenDictTupleStrDecimalBoolMixin:
         _types = {NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass}
-    # qty 8
-    class NoneFrozenDictTupleStrDecimalBoolFileBytesMixin:
-        _types = {NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass, FileIO, bytes}
+    # qty 9
+    class NoneFrozenDictTupleStrIntDecimalBoolFileBytesMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, str, int, decimal.Decimal, BoolClass, FileIO, bytes}
 
 
 class ValidatorBase:
     @staticmethod
     def _is_json_validation_enabled_oapg(schema_keyword, configuration=None):
         """Returns true if JSON schema validation is enabled for the specified
         validation keyword. This can be used to skip JSON schema structural validation
@@ -1703,14 +1703,15 @@
 
 
 def cast_to_allowed_types(
     arg: typing.Union[str, date, datetime, uuid.UUID, decimal.Decimal, int, float, None, dict, frozendict.frozendict, list, tuple, bytes, Schema, io.FileIO, io.BufferedReader],
     from_server: bool,
     validated_path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]],
     path_to_item: typing.Tuple[typing.Union[str, int], ...] = tuple(['args[0]']),
+    schema: Schema = None,
 ) -> typing.Union[frozendict.frozendict, tuple, decimal.Decimal, str, bytes, BoolClass, NoneClass, FileIO]:
     """
     Casts the input payload arg into the allowed types
     The input validated_path_to_schemas is mutated by running this function
 
     When from_server is False then
     - date/datetime is cast to str
@@ -1769,15 +1770,22 @@
         return decimal_from_float
     elif isinstance(arg, (tuple, list)):
         return tuple([cast_to_allowed_types(item, from_server, validated_path_to_schemas, path_to_item + (i,)) for i, item in enumerate(arg)])
     elif isinstance(arg, (none_type, NoneClass)):
         return NoneClass.NONE
     elif isinstance(arg, (date, datetime)):
         if not from_server:
-            return arg.isoformat()
+            # if schema itself is the DateTimeSchema class then convert to isoformat
+            # if schema itself is the DateSchema class then convert to yyyy-mm-dd using strftime
+            if schema is None:
+                return arg.isoformat()
+            if schema is DateTimeSchema:
+                return arg.isoformat()
+            if schema is DateSchema:
+                return arg.strftime('%Y-%m-%d')
         raise type_error
     elif isinstance(arg, uuid.UUID):
         if not from_server:
             return str(arg)
         raise type_error
     elif isinstance(arg, decimal.Decimal):
         return decimal.Decimal(arg)
@@ -2013,14 +2021,15 @@
     def __new__(cls, arg: None, **kwargs: Configuration):
         return super().__new__(cls, arg, **kwargs)
 
 
 class NumberSchema(
     NumberBase,
     Schema,
+    IntMixin,
     DecimalMixin
 ):
     """
     This is used for type: number with no format
     Both integers AND floats are accepted
     """
 
@@ -2337,15 +2346,15 @@
     DictBase,
     ListBase,
     NumberBase,
     StrBase,
     BoolBase,
     NoneBase,
     Schema,
-    NoneFrozenDictTupleStrDecimalBoolFileBytesMixin
+    NoneFrozenDictTupleStrIntDecimalBoolFileBytesMixin
 ):
     # Python representation of a schema defined as true or {}
     pass
 
 
 class UnsetAnyTypeSchema(AnyTypeSchema):
     # Used when additionalProperties/items was not explicitly defined and a defining schema is needed
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_client/validation_metadata.py` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_python_sdk.egg-info/PKG-INFO` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_python_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: decentro-in-kyc-python-sdk
-Version: 4.2.0
+Version: 4.3.0
 Summary: decentro-in-kyc
 Home-page: https://decentro.tech
 Author: Decentro
 Author-email: admin@decentro.tech
 License: MIT
 Keywords: decentro-in-kyc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # decentro-in-kyc-python-sdk
 KYC & Onboarding
 
 - API version: 1.0.0
-- Package version: 4.2.0
+- Package version: 4.3.0
 For more information, please visit [https://decentro.tech](https://decentro.tech)
 
 ## Requirements.
 
 Python >=3.7
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install decentro-in-kyc-python-sdk==4.2.0
+pip install decentro-in-kyc-python-sdk==4.3.0
 ```
-(you may need to run `pip` with root permission: `sudo pip install decentro-in-kyc-python-sdk==4.2.0`)
+(you may need to run `pip` with root permission: `sudo pip install decentro-in-kyc-python-sdk==4.3.0`)
 
 Then import the package:
 ```python
 import decentro_in_kyc_client
 ```
 ## Getting Started
 
@@ -82,15 +82,15 @@
     pprint(check_image_quality_response.body["responseCode"])
     pprint(check_image_quality_response.body["message"])
     pprint(check_image_quality_response.body["data"])
     pprint(check_image_quality_response.headers)
     pprint(check_image_quality_response.status)
     pprint(check_image_quality_response.round_trip_time)
 except ApiException as e:
-    print("Exception when calling CheckImageQualityResponse.check_image_quality: %s\n" % e)
+    print("Exception when calling KYCApi.check_image_quality: %s\n" % e)
     pprint(e.body)
     if e.status == 400:
         pprint(e.body["decentroTxnId"])
         pprint(e.body["status"])
         pprint(e.body["responseCode"])
         pprint(e.body["message"])
     pprint(e.headers)
@@ -128,15 +128,15 @@
  - [ClassifyDocument400Response](docs/models/ClassifyDocument400Response.md)
  - [ClassifyDocumentRequest](docs/models/ClassifyDocumentRequest.md)
  - [ClassifyDocumentResponse](docs/models/ClassifyDocumentResponse.md)
  - [ExtractText400Response](docs/models/ExtractText400Response.md)
  - [ExtractTextRequest](docs/models/ExtractTextRequest.md)
  - [ExtractTextResponse](docs/models/ExtractTextResponse.md)
  - [MaskAadhaarRequest](docs/models/MaskAadhaarRequest.md)
- - [MaskAadhaarResponse](docs/models/MaskAadhaarResponse.md)
+ - [MaskAadhaarUid400Response](docs/models/MaskAadhaarUid400Response.md)
  - [MaskAadhaarUidResponse](docs/models/MaskAadhaarUidResponse.md)
  - [MatchFace400Response](docs/models/MatchFace400Response.md)
  - [MatchFaceRequest](docs/models/MatchFaceRequest.md)
  - [MatchFaceResponse](docs/models/MatchFaceResponse.md)
  - [Validate400Response](docs/models/Validate400Response.md)
  - [ValidateRequest](docs/models/ValidateRequest.md)
  - [ValidateResponse](docs/models/ValidateResponse.md)
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/decentro_in_kyc_python_sdk.egg-info/SOURCES.txt` & `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_python_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 decentro_in_kyc_client/model/classify_document400_response.py
 decentro_in_kyc_client/model/classify_document_request.py
 decentro_in_kyc_client/model/classify_document_response.py
 decentro_in_kyc_client/model/extract_text400_response.py
 decentro_in_kyc_client/model/extract_text_request.py
 decentro_in_kyc_client/model/extract_text_response.py
 decentro_in_kyc_client/model/mask_aadhaar_request.py
-decentro_in_kyc_client/model/mask_aadhaar_response.py
+decentro_in_kyc_client/model/mask_aadhaar_uid400_response.py
 decentro_in_kyc_client/model/mask_aadhaar_uid_response.py
 decentro_in_kyc_client/model/match_face400_response.py
 decentro_in_kyc_client/model/match_face_request.py
 decentro_in_kyc_client/model/match_face_response.py
 decentro_in_kyc_client/model/validate400_response.py
 decentro_in_kyc_client/model/validate_request.py
 decentro_in_kyc_client/model/validate_response.py
@@ -90,15 +90,15 @@
 test/test_models/test_classify_document400_response.py
 test/test_models/test_classify_document_request.py
 test/test_models/test_classify_document_response.py
 test/test_models/test_extract_text400_response.py
 test/test_models/test_extract_text_request.py
 test/test_models/test_extract_text_response.py
 test/test_models/test_mask_aadhaar_request.py
-test/test_models/test_mask_aadhaar_response.py
+test/test_models/test_mask_aadhaar_uid400_response.py
 test/test_models/test_mask_aadhaar_uid_response.py
 test/test_models/test_match_face400_response.py
 test/test_models/test_match_face_request.py
 test/test_models/test_match_face_response.py
 test/test_models/test_validate400_response.py
 test/test_models/test_validate_request.py
 test/test_models/test_validate_response.py
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/setup.py` & `decentro-in-kyc-python-sdk-4.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "decentro-in-kyc-python-sdk"
-VERSION = "4.2.0"
+VERSION = "4.3.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_kyc_api.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_kyc_api.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_image_quality400_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_image_quality400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_image_quality_request.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_image_quality_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_image_quality_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_image_quality_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_photocopy400_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_photocopy400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_photocopy_request.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_photocopy_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_photocopy_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_photocopy_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_video_liveness400_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_video_liveness400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_video_liveness_request.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_video_liveness_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_check_video_liveness_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_video_liveness_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_classify_document400_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_classify_document400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_classify_document_request.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_classify_document_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_classify_document_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_classify_document_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_extract_text400_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_extract_text400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_extract_text_request.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_extract_text_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_extract_text_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_extract_text_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_mask_aadhaar_request.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_mask_aadhaar_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_mask_aadhaar_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_mask_aadhaar_uid_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
 import unittest
 
 import decentro_in_kyc_client
-from decentro_in_kyc_client.model.mask_aadhaar_response import MaskAadhaarResponse
+from decentro_in_kyc_client.model.mask_aadhaar_uid_response import MaskAadhaarUidResponse
 from decentro_in_kyc_client import configuration
 
 
-class TestMaskAadhaarResponse(unittest.TestCase):
-    """MaskAadhaarResponse unit test stubs"""
+class TestMaskAadhaarUidResponse(unittest.TestCase):
+    """MaskAadhaarUidResponse unit test stubs"""
     pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_mask_aadhaar_uid_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_match_face400_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
 import unittest
 
 import decentro_in_kyc_client
-from decentro_in_kyc_client.model.mask_aadhaar_uid_response import MaskAadhaarUidResponse
+from decentro_in_kyc_client.model.match_face400_response import MatchFace400Response
 from decentro_in_kyc_client import configuration
 
 
-class TestMaskAadhaarUidResponse(unittest.TestCase):
-    """MaskAadhaarUidResponse unit test stubs"""
+class TestMatchFace400Response(unittest.TestCase):
+    """MatchFace400Response unit test stubs"""
     pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_match_face400_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_kyc_public_registry_validate/test_post.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,20 +7,39 @@
 
     The version of the OpenAPI document: 1.0.0
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import decentro_in_kyc_client
-from decentro_in_kyc_client.model.match_face400_response import MatchFace400Response
-from decentro_in_kyc_client import configuration
+from decentro_in_kyc_client.paths.kyc_public_registry_validate import post
+from decentro_in_kyc_client import configuration, schemas, api_client
+
+from .. import ApiTestMixin
+
+
+class TestKycPublicRegistryValidate(ApiTestMixin, unittest.TestCase):
+    """
+    KycPublicRegistryValidate unit test stubs
+        Validate
+    """
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    response_status = 200
+
+
 
 
-class TestMatchFace400Response(unittest.TestCase):
-    """MatchFace400Response unit test stubs"""
-    pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_match_face_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_match_face_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_models/test_validate400_response.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_validate400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_paths/__init__.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_kyc_public_registry_validate/test_post.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_video_liveness/test_post.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,34 +12,32 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import decentro_in_kyc_client
-from decentro_in_kyc_client.paths.kyc_public_registry_validate import post
+from decentro_in_kyc_client.paths.v2_kyc_forensics_video_liveness import post
 from decentro_in_kyc_client import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestKycPublicRegistryValidate(ApiTestMixin, unittest.TestCase):
+class TestV2KycForensicsVideoLiveness(ApiTestMixin, unittest.TestCase):
     """
-    KycPublicRegistryValidate unit test stubs
-        Validate
+    V2KycForensicsVideoLiveness unit test stubs
+        Liveness Check
     """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     response_status = 200
 
 
 
 
-
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_kyc_scan_extract_ocr/test_post.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_kyc_scan_extract_ocr/test_post.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_document_classification/test_post.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_document_classification/test_post.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_face_match/test_post.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_face_match/test_post.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_image_quality/test_post.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_image_quality/test_post.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_forensics_photocopy_check/test_post.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_photocopy_check/test_post.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.2.0/test/test_paths/test_v2_kyc_identities_mask_aadhaar_uid/test_post.py` & `decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_identities_mask_aadhaar_uid/test_post.py`

 * *Files identical despite different names*

