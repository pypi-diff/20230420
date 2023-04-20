# Comparing `tmp/acd-sdk-2.0.1.tar.gz` & `tmp/acd-sdk-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acd-sdk-2.0.1.tar", last modified: Sat Mar 25 17:38:56 2023, max compression
+gzip compressed data, was "acd-sdk-2.0.2.tar", last modified: Thu Apr 20 18:45:36 2023, max compression
```

## Comparing `acd-sdk-2.0.1.tar` & `acd-sdk-2.0.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 17:38:56.425998 acd-sdk-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-25 17:38:56.425998 acd-sdk-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-03-25 17:38:37.000000 acd-sdk-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 17:38:56.413998 acd-sdk-2.0.1/acd_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 17:38:56.413998 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   386652 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/annotator_for_clinical_data_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 17:38:56.417998 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 17:38:56.425998 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_annotator_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_assistance_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_attribute_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_cancer_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_concept_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_concept_value_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_disambiguation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_ejection_fraction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4290 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_insight_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_lab_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_medication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_negated_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_nlu_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_procedure.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_smoking.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_spell_corrected_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_spelling_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_symptom_disease.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      921 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_temporal_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_unstructured_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/acd_sdk/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-25 17:38:37.000000 acd-sdk-2.0.1/acd_sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 17:38:56.413998 acd-sdk-2.0.1/acd_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-25 17:38:56.000000 acd-sdk-2.0.1/acd_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-25 17:38:56.000000 acd-sdk-2.0.1/acd_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 17:38:56.000000 acd-sdk-2.0.1/acd_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-25 17:38:56.000000 acd-sdk-2.0.1/acd_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-25 17:38:56.000000 acd-sdk-2.0.1/acd_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 17:38:56.000000 acd-sdk-2.0.1/acd_sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-25 17:37:55.000000 acd-sdk-2.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 17:38:56.425998 acd-sdk-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-03-25 17:38:37.000000 acd-sdk-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:45:36.734212 acd-sdk-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-20 18:45:36.734212 acd-sdk-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-20 18:45:14.000000 acd-sdk-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:45:36.730212 acd-sdk-2.0.2/acd_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:45:36.730212 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   386652 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/annotator_for_clinical_data_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:45:36.730212 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:45:36.734212 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_annotator_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_assistance_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_attribute_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_cancer_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_concept_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_concept_value_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_disambiguation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_ejection_fraction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4290 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_insight_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_lab_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_medication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_negated_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_nlu_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_smoking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_spell_corrected_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_spelling_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_symptom_disease.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      921 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_temporal_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_unstructured_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/acd_sdk/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-20 18:45:14.000000 acd-sdk-2.0.2/acd_sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:45:36.730212 acd-sdk-2.0.2/acd_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-20 18:45:36.000000 acd-sdk-2.0.2/acd_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-20 18:45:36.000000 acd-sdk-2.0.2/acd_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:45:36.000000 acd-sdk-2.0.2/acd_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-20 18:45:36.000000 acd-sdk-2.0.2/acd_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 18:45:36.000000 acd-sdk-2.0.2/acd_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:45:36.000000 acd-sdk-2.0.2/acd_sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-20 18:44:23.000000 acd-sdk-2.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 18:45:36.734212 acd-sdk-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-20 18:45:14.000000 acd-sdk-2.0.2/setup.py
```

### Comparing `acd-sdk-2.0.1/LICENSE.md` & `acd-sdk-2.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/PKG-INFO` & `acd-sdk-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: acd-sdk
-Version: 2.0.1
+Version: 2.0.2
 Summary: ('This is the Annotator for Clinical Data Python SDK',)
-Home-page: https://github.com/Merative/whcs-python-sdk
+Home-page: https://github.com/Merative/acd-python-sdk
 Author: Merative
 Author-email: acddev@merative.com
 License: Apache 2.0
 Keywords: PACKAGE_NAME
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -19,15 +19,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 
-# Merative Annotator for Clinical Data Python SDK Version 2.0.1
+# Merative Annotator for Clinical Data Python SDK Version 2.0.2
 
 ## Overview
 
 This Python SDK allows developers to programmatically interact with the following service:
 
 | Service Name | Imported Class Name |
 |--------------|-------------|
@@ -63,15 +63,15 @@
 
 For questions, refer to:
   * [Annotator for Clinical Data documentation](https://merative.github.io/acd-containers/)
   * [Annotator for Clinical Data Support page](https://merative.github.io/acd-containers/support/support/)
 
 ## Issues
 If you encounter an issue with the project, you are welcome to submit a
-[bug report](https://github.com/merative/whcs-python-sdk/issues).
+[bug report](https://github.com/merative/acd-python-sdk/issues).
 
 ## Contributing
 See [CONTRIBUTING](CONTRIBUTING.md).
 
 ## License
 
 The Annotator for Clinical Data Python SDK is released under the Apache 2.0 license.
```

### Comparing `acd-sdk-2.0.1/README.md` & `acd-sdk-2.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# Merative Annotator for Clinical Data Python SDK Version 2.0.1
+# Merative Annotator for Clinical Data Python SDK Version 2.0.2
 
 ## Overview
 
 This Python SDK allows developers to programmatically interact with the following service:
 
 | Service Name | Imported Class Name |
 |--------------|-------------|
@@ -39,15 +39,15 @@
 
 For questions, refer to:
   * [Annotator for Clinical Data documentation](https://merative.github.io/acd-containers/)
   * [Annotator for Clinical Data Support page](https://merative.github.io/acd-containers/support/support/)
 
 ## Issues
 If you encounter an issue with the project, you are welcome to submit a
-[bug report](https://github.com/merative/whcs-python-sdk/issues).
+[bug report](https://github.com/merative/acd-python-sdk/issues).
 
 ## Contributing
 See [CONTRIBUTING](CONTRIBUTING.md).
 
 ## License
 
 The Annotator for Clinical Data Python SDK is released under the Apache 2.0 license.
```

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/__init__.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/__init__.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/annotator_for_clinical_data_v1.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/annotator_for_clinical_data_v1.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_annotation.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_annotation.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_annotator_output.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_annotator_output.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_assistance_annotation.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_assistance_annotation.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_attribute_values.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_attribute_values.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_cancer_diagnosis.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_cancer_diagnosis.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_concept_annotation.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_concept_annotation.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_concept_value_annotation.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_concept_value_annotation.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_disambiguation.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_disambiguation.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_ejection_fraction.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_ejection_fraction.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_insight_model.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_insight_model.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_lab_value.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_lab_value.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_medication.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_medication.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_negated_span.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_negated_span.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_nlu_entities.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_nlu_entities.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_procedure.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_procedure.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_relation.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_relation.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_section.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_section.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_smoking.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_smoking.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_spell_corrected_text.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_spell_corrected_text.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_spelling_correction.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_spelling_correction.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_suggestion.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_suggestion.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_symptom_disease.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_symptom_disease.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_temporal_span.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_temporal_span.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/annotator_for_clinical_data/tests/common/test_unstructured_container.py` & `acd-sdk-2.0.2/acd_sdk/annotator_for_clinical_data/tests/common/test_unstructured_container.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/common.py` & `acd-sdk-2.0.2/acd_sdk/common.py`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/acd_sdk/version.py` & `acd-sdk-2.0.2/acd_sdk/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 # SPDX-License-Identifier: Apache-2.0                               
 #                                                                   
 # ***************************************************************** 
 
 """
 SDK version
 """
-__version__ = '2.0.1'
+__version__ = '2.0.2'
```

### Comparing `acd-sdk-2.0.1/acd_sdk.egg-info/PKG-INFO` & `acd-sdk-2.0.2/acd_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: acd-sdk
-Version: 2.0.1
+Version: 2.0.2
 Summary: ('This is the Annotator for Clinical Data Python SDK',)
-Home-page: https://github.com/Merative/whcs-python-sdk
+Home-page: https://github.com/Merative/acd-python-sdk
 Author: Merative
 Author-email: acddev@merative.com
 License: Apache 2.0
 Keywords: PACKAGE_NAME
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -19,15 +19,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 
-# Merative Annotator for Clinical Data Python SDK Version 2.0.1
+# Merative Annotator for Clinical Data Python SDK Version 2.0.2
 
 ## Overview
 
 This Python SDK allows developers to programmatically interact with the following service:
 
 | Service Name | Imported Class Name |
 |--------------|-------------|
@@ -63,15 +63,15 @@
 
 For questions, refer to:
   * [Annotator for Clinical Data documentation](https://merative.github.io/acd-containers/)
   * [Annotator for Clinical Data Support page](https://merative.github.io/acd-containers/support/support/)
 
 ## Issues
 If you encounter an issue with the project, you are welcome to submit a
-[bug report](https://github.com/merative/whcs-python-sdk/issues).
+[bug report](https://github.com/merative/acd-python-sdk/issues).
 
 ## Contributing
 See [CONTRIBUTING](CONTRIBUTING.md).
 
 ## License
 
 The Annotator for Clinical Data Python SDK is released under the Apache 2.0 license.
```

### Comparing `acd-sdk-2.0.1/acd_sdk.egg-info/SOURCES.txt` & `acd-sdk-2.0.2/acd_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acd-sdk-2.0.1/setup.py` & `acd-sdk-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from setuptools import setup, find_packages
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '2.0.1'
+__version__ = '2.0.2'
 PACKAGE_NAME = 'acd_sdk'
 PACKAGE_DESC = 'This is the Annotator for Clinical Data Python SDK',
 
 with open('requirements.txt') as f:
     install_requires = [str(req) for req in pkg_resources.parse_requirements(f)]
 with open('requirements-dev.txt') as f:
     tests_require = [str(req) for req in pkg_resources.parse_requirements(f)]
@@ -43,15 +43,15 @@
       license='Apache 2.0',
       install_requires=install_requires,
       tests_require=tests_require,
       author='Merative',
       author_email='acddev@merative.com',
       long_description=readme,
       long_description_content_type='text/markdown',
-      url='https://github.com/Merative/whcs-python-sdk',
+      url='https://github.com/Merative/acd-python-sdk',
       packages=find_packages(),
       include_package_data=True,
       keywords='PACKAGE_NAME',
       classifiers=[
            'Programming Language :: Python',
            'Programming Language :: Python :: 3',
            'Programming Language :: Python :: 3.7',
```

