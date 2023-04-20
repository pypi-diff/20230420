# Comparing `tmp/PyContracts-mirror-2.0.1.8.tar.gz` & `tmp/PyContracts-mirror-2.0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyContracts-mirror-2.0.1.8.tar", last modified: Tue Aug  9 12:04:05 2022, max compression
+gzip compressed data, was "PyContracts-mirror-2.0.1.9.tar", last modified: Tue Aug  9 14:42:44 2022, max compression
```

## Comparing `PyContracts-mirror-2.0.1.8.tar` & `PyContracts-mirror-2.0.1.9.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 12:04:05.253802 PyContracts-mirror-2.0.1.8/
--rw-rw-r--   0 xvs       (1000) xvs       (1000)       98 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/.bumpversion.cfg
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     7916 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/LICENSE.txt
--rw-rw-r--   0 xvs       (1000) xvs       (1000)       69 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/MANIFEST.in
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     6825 2022-08-09 12:04:05.253802 PyContracts-mirror-2.0.1.8/PKG-INFO
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     5622 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/README.rst
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      526 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/README_continuous_integration.md
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1302 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/pypackage.mk
--rw-rw-r--   0 xvs       (1000) xvs       (1000)       65 2022-07-28 14:24:57.000000 PyContracts-mirror-2.0.1.8/requirements.txt
--rw-rw-r--   0 xvs       (1000) xvs       (1000)       38 2022-08-09 12:04:05.253802 PyContracts-mirror-2.0.1.8/setup.cfg
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2141 2022-07-28 14:55:58.000000 PyContracts-mirror-2.0.1.8/setup.py
-drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 12:04:05.245802 PyContracts-mirror-2.0.1.8/src/
-drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 12:04:05.245802 PyContracts-mirror-2.0.1.8/src/PyContracts_mirror.egg-info/
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     6825 2022-08-09 12:04:04.000000 PyContracts-mirror-2.0.1.8/src/PyContracts_mirror.egg-info/PKG-INFO
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     3535 2022-08-09 12:04:05.000000 PyContracts-mirror-2.0.1.8/src/PyContracts_mirror.egg-info/SOURCES.txt
--rw-rw-r--   0 xvs       (1000) xvs       (1000)        1 2022-08-09 12:04:05.000000 PyContracts-mirror-2.0.1.8/src/PyContracts_mirror.egg-info/dependency_links.txt
--rw-rw-r--   0 xvs       (1000) xvs       (1000)       31 2022-08-09 12:04:05.000000 PyContracts-mirror-2.0.1.8/src/PyContracts_mirror.egg-info/requires.txt
--rw-rw-r--   0 xvs       (1000) xvs       (1000)       10 2022-08-09 12:04:05.000000 PyContracts-mirror-2.0.1.8/src/PyContracts_mirror.egg-info/top_level.txt
-drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 12:04:05.249802 PyContracts-mirror-2.0.1.8/src/contracts/
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1303 2022-08-09 06:56:58.000000 PyContracts-mirror-2.0.1.8/src/contracts/__init__.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     6647 2022-07-25 14:23:41.000000 PyContracts-mirror-2.0.1.8/src/contracts/backported.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     5146 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/docstring_parsing.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      785 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/enabling.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     3409 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/inspection.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)    19769 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/interface.py
-drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 12:04:05.249802 PyContracts-mirror-2.0.1.8/src/contracts/library/
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1322 2022-07-28 17:32:28.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/__init__.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2999 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/arithmetic.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     9266 2022-07-28 17:12:23.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/array.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     9377 2022-08-09 06:56:26.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/array_ops.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1882 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/attributes.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2515 2022-07-25 14:44:03.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/collection.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     4418 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/comparison.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     6229 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/compositions.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1256 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/datetime_tz.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2105 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/dicts.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1165 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/dummy.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     7853 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/extensions.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1023 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/files.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2361 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/isinstance_imp.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1909 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/lists.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2134 2022-07-25 14:40:32.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/map.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2997 2022-07-28 21:20:21.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/method.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1360 2022-07-25 14:41:30.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/miscellaneous_aliases.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     3424 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/scoped_variables.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      969 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/separate_context.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2751 2022-07-28 18:48:14.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/seq.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1921 2022-07-25 14:40:43.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/sets.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2033 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/simple_values.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2238 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/strings.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     3447 2022-07-28 18:57:46.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/suggester.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     3336 2022-07-28 17:28:26.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/tuple.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2800 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/types_misc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     4652 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/library/variables.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)    22388 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/main.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1408 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/main_actual.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     4288 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/metaclass.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     4959 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/pyparsing_utils.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     4050 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/syntax.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      493 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/test_registrar.py
-drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 12:04:05.253802 PyContracts-mirror-2.0.1.8/src/contracts/testing/
--rw-rw-r--   0 xvs       (1000) xvs       (1000)       23 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/__init__.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2648 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/array_extended_test.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1837 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/friendliness_statistics.py
-drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 12:04:05.253802 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      710 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/__init__.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      740 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/arithmetic_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      479 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/array_elements_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     5327 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/array_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      531 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/attr_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      677 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/collection_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      915 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/comparison_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      828 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/compositions_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      569 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/dicts_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      132 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/dummy_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      684 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/extensions_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      177 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/files_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1118 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/isinstance_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      685 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/lists_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      554 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/map_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      766 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/miscellaneous_aliases_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      684 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/separate_context_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      733 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/seq_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      123 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/simple_values_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      411 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/strings_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2161 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/test_scoped_variables.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1187 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/tuple_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      492 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/types_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      272 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/library/variables_tc.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2155 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/test_class_contracts.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     9564 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/test_decorator.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     4335 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/test_docstring_parsing.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     3645 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/test_idioms.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     3704 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/test_meta.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1803 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/test_multiple.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     9751 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/test_new_contract.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2224 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/test_particulars.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1767 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/test_pickling.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     3731 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/test_simple.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      450 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/test_unicode_literals.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     1744 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/testing/utils.py
-drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 12:04:05.253802 PyContracts-mirror-2.0.1.8/src/contracts/useful_contracts/
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      206 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/useful_contracts/__init__.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)      519 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/useful_contracts/numbers.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     2740 2022-08-09 06:58:39.000000 PyContracts-mirror-2.0.1.8/src/contracts/useful_contracts/numpy_specific.py
--rw-rw-r--   0 xvs       (1000) xvs       (1000)     7218 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.8/src/contracts/utils.py
+drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 14:42:44.510511 PyContracts-mirror-2.0.1.9/
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)       98 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/.bumpversion.cfg
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     7916 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/LICENSE.txt
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)       69 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/MANIFEST.in
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     6825 2022-08-09 14:42:44.506512 PyContracts-mirror-2.0.1.9/PKG-INFO
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     5622 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/README.rst
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      526 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/README_continuous_integration.md
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1302 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/pypackage.mk
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)       65 2022-07-28 14:24:57.000000 PyContracts-mirror-2.0.1.9/requirements.txt
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)       38 2022-08-09 14:42:44.510511 PyContracts-mirror-2.0.1.9/setup.cfg
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2141 2022-07-28 14:55:58.000000 PyContracts-mirror-2.0.1.9/setup.py
+drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 14:42:44.502512 PyContracts-mirror-2.0.1.9/src/
+drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 14:42:44.502512 PyContracts-mirror-2.0.1.9/src/PyContracts_mirror.egg-info/
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     6825 2022-08-09 14:42:44.000000 PyContracts-mirror-2.0.1.9/src/PyContracts_mirror.egg-info/PKG-INFO
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     3535 2022-08-09 14:42:44.000000 PyContracts-mirror-2.0.1.9/src/PyContracts_mirror.egg-info/SOURCES.txt
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)        1 2022-08-09 14:42:44.000000 PyContracts-mirror-2.0.1.9/src/PyContracts_mirror.egg-info/dependency_links.txt
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)       31 2022-08-09 14:42:44.000000 PyContracts-mirror-2.0.1.9/src/PyContracts_mirror.egg-info/requires.txt
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)       10 2022-08-09 14:42:44.000000 PyContracts-mirror-2.0.1.9/src/PyContracts_mirror.egg-info/top_level.txt
+drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 14:42:44.502512 PyContracts-mirror-2.0.1.9/src/contracts/
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1303 2022-08-09 14:41:01.000000 PyContracts-mirror-2.0.1.9/src/contracts/__init__.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     6725 2022-08-09 14:40:49.000000 PyContracts-mirror-2.0.1.9/src/contracts/backported.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     5146 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/docstring_parsing.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      785 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/enabling.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     3409 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/inspection.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)    19769 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/interface.py
+drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 14:42:44.506512 PyContracts-mirror-2.0.1.9/src/contracts/library/
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1322 2022-07-28 17:32:28.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/__init__.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2999 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/arithmetic.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     9266 2022-07-28 17:12:23.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/array.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     9377 2022-08-09 06:56:26.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/array_ops.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1882 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/attributes.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2515 2022-07-25 14:44:03.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/collection.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     4418 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/comparison.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     6229 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/compositions.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1256 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/datetime_tz.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2105 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/dicts.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1165 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/dummy.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     7853 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/extensions.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1023 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/files.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2361 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/isinstance_imp.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1909 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/lists.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2134 2022-07-25 14:40:32.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/map.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2997 2022-07-28 21:20:21.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/method.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1360 2022-07-25 14:41:30.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/miscellaneous_aliases.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     3424 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/scoped_variables.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      969 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/separate_context.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2751 2022-07-28 18:48:14.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/seq.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1921 2022-07-25 14:40:43.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/sets.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2033 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/simple_values.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2238 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/strings.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     3447 2022-07-28 18:57:46.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/suggester.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     3336 2022-07-28 17:28:26.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/tuple.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2800 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/types_misc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     4652 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/library/variables.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)    22388 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/main.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1408 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/main_actual.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     4288 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/metaclass.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     4959 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/pyparsing_utils.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     4050 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/syntax.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      493 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/test_registrar.py
+drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 14:42:44.506512 PyContracts-mirror-2.0.1.9/src/contracts/testing/
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)       23 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/__init__.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2648 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/array_extended_test.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1837 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/friendliness_statistics.py
+drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 14:42:44.506512 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      710 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/__init__.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      740 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/arithmetic_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      479 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/array_elements_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     5327 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/array_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      531 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/attr_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      677 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/collection_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      915 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/comparison_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      828 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/compositions_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      569 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/dicts_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      132 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/dummy_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      684 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/extensions_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      177 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/files_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1118 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/isinstance_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      685 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/lists_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      554 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/map_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      766 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/miscellaneous_aliases_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      684 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/separate_context_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      733 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/seq_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      123 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/simple_values_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      411 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/strings_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2161 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/test_scoped_variables.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1187 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/tuple_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      492 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/types_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      272 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/library/variables_tc.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2155 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/test_class_contracts.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     9564 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/test_decorator.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     4335 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/test_docstring_parsing.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     3645 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/test_idioms.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     3704 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/test_meta.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1803 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/test_multiple.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     9751 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/test_new_contract.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2224 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/test_particulars.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1767 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/test_pickling.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     3731 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/test_simple.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      450 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/test_unicode_literals.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     1744 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/testing/utils.py
+drwxrwxr-x   0 xvs       (1000) xvs       (1000)        0 2022-08-09 14:42:44.506512 PyContracts-mirror-2.0.1.9/src/contracts/useful_contracts/
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      206 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/useful_contracts/__init__.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)      519 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/useful_contracts/numbers.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     2740 2022-08-09 06:58:39.000000 PyContracts-mirror-2.0.1.9/src/contracts/useful_contracts/numpy_specific.py
+-rw-rw-r--   0 xvs       (1000) xvs       (1000)     7218 2022-07-25 13:58:31.000000 PyContracts-mirror-2.0.1.9/src/contracts/utils.py
```

### Comparing `PyContracts-mirror-2.0.1.8/LICENSE.txt` & `PyContracts-mirror-2.0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/PKG-INFO` & `PyContracts-mirror-2.0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyContracts-mirror
-Version: 2.0.1.8
+Version: 2.0.1.9
 Summary: INCOMPATIBLE FORK OF CURRENT PYCONTRACTS ON GITHUBThe version on pypi is stale, this is a fork that is updated from github andwith added support for jax. No guarantee that this will be kept up to date, or developed furtheror kept compatible with the original.See the original repo here: http://andreacensi.github.com/contracts/
 Home-page: 
 Download-URL: 
 Author: xivarri
 Author-email: xamvolagis@gmail.com
 License: LGPL
 Keywords: type checking,value checking,contracts
```

### Comparing `PyContracts-mirror-2.0.1.8/README.rst` & `PyContracts-mirror-2.0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/README_continuous_integration.md` & `PyContracts-mirror-2.0.1.9/README_continuous_integration.md`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/pypackage.mk` & `PyContracts-mirror-2.0.1.9/pypackage.mk`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/setup.py` & `PyContracts-mirror-2.0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/PyContracts_mirror.egg-info/PKG-INFO` & `PyContracts-mirror-2.0.1.9/src/PyContracts_mirror.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyContracts-mirror
-Version: 2.0.1.8
+Version: 2.0.1.9
 Summary: INCOMPATIBLE FORK OF CURRENT PYCONTRACTS ON GITHUBThe version on pypi is stale, this is a fork that is updated from github andwith added support for jax. No guarantee that this will be kept up to date, or developed furtheror kept compatible with the original.See the original repo here: http://andreacensi.github.com/contracts/
 Home-page: 
 Download-URL: 
 Author: xivarri
 Author-email: xamvolagis@gmail.com
 License: LGPL
 Keywords: type checking,value checking,contracts
```

### Comparing `PyContracts-mirror-2.0.1.8/src/PyContracts_mirror.egg-info/SOURCES.txt` & `PyContracts-mirror-2.0.1.9/src/PyContracts_mirror.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/__init__.py` & `PyContracts-mirror-2.0.1.9/src/contracts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.0.1.8"
+__version__ = "2.0.1.9"
 
 import logging
 
 # logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 from .interface import (
```

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/backported.py` & `PyContracts-mirror-2.0.1.9/src/contracts/backported.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,16 @@
             im_self = getattr(func, "im_self", None)
         else:
             im_self = getattr(func, "__self__", None)
 
         if ismethod(func) and im_self is not None:
             # implicit 'self' (or 'cls' for classmethods) argument
             positional = (im_self,) + positional
+        elif len(args) > 0 and args[0] == "self":
+            args = args[1:]
         num_pos = len(positional)
         num_total = num_pos + len(named)
         num_args = len(args)
         num_defaults = len(defaults) if defaults else 0
         for arg, value in zip(args, positional):
             assign(arg, value)
         if varargs:
```

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/docstring_parsing.py` & `PyContracts-mirror-2.0.1.9/src/contracts/docstring_parsing.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/enabling.py` & `PyContracts-mirror-2.0.1.9/src/contracts/enabling.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/inspection.py` & `PyContracts-mirror-2.0.1.9/src/contracts/inspection.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/interface.py` & `PyContracts-mirror-2.0.1.9/src/contracts/interface.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/__init__.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/__init__.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/arithmetic.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/arithmetic.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/array.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/array.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/array_ops.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/array_ops.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/attributes.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/attributes.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/collection.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/collection.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/comparison.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/comparison.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/compositions.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/compositions.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/datetime_tz.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/datetime_tz.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/dicts.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/dicts.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/dummy.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/dummy.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/extensions.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/extensions.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/files.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/files.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/isinstance_imp.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/isinstance_imp.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/lists.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/lists.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/map.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/map.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/method.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/method.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/miscellaneous_aliases.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/miscellaneous_aliases.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/scoped_variables.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/scoped_variables.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/separate_context.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/separate_context.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/seq.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/seq.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/sets.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/sets.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/simple_values.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/simple_values.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/strings.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/strings.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/suggester.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/suggester.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/tuple.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/tuple.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/types_misc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/types_misc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/library/variables.py` & `PyContracts-mirror-2.0.1.9/src/contracts/library/variables.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/main.py` & `PyContracts-mirror-2.0.1.9/src/contracts/main.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/main_actual.py` & `PyContracts-mirror-2.0.1.9/src/contracts/main_actual.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/metaclass.py` & `PyContracts-mirror-2.0.1.9/src/contracts/metaclass.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/pyparsing_utils.py` & `PyContracts-mirror-2.0.1.9/src/contracts/pyparsing_utils.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/syntax.py` & `PyContracts-mirror-2.0.1.9/src/contracts/syntax.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/array_extended_test.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/array_extended_test.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/friendliness_statistics.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/friendliness_statistics.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/__init__.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/__init__.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/arithmetic_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/arithmetic_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/array_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/array_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/attr_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/attr_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/collection_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/collection_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/comparison_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/comparison_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/compositions_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/compositions_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/dicts_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/dicts_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/extensions_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/extensions_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/isinstance_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/isinstance_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/lists_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/lists_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/map_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/map_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/miscellaneous_aliases_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/miscellaneous_aliases_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/separate_context_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/separate_context_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/seq_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/seq_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/test_scoped_variables.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/test_scoped_variables.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/library/tuple_tc.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/library/tuple_tc.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/test_class_contracts.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/test_class_contracts.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/test_decorator.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/test_decorator.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/test_docstring_parsing.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/test_docstring_parsing.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/test_idioms.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/test_idioms.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/test_meta.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/test_meta.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/test_multiple.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/test_multiple.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/test_new_contract.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/test_new_contract.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/test_particulars.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/test_particulars.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/test_pickling.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/test_pickling.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/test_simple.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/test_simple.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/testing/utils.py` & `PyContracts-mirror-2.0.1.9/src/contracts/testing/utils.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/useful_contracts/numbers.py` & `PyContracts-mirror-2.0.1.9/src/contracts/useful_contracts/numbers.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/useful_contracts/numpy_specific.py` & `PyContracts-mirror-2.0.1.9/src/contracts/useful_contracts/numpy_specific.py`

 * *Files identical despite different names*

### Comparing `PyContracts-mirror-2.0.1.8/src/contracts/utils.py` & `PyContracts-mirror-2.0.1.9/src/contracts/utils.py`

 * *Files identical despite different names*

