# Comparing `tmp/mozilla-version-1.2.0.tar.gz` & `tmp/mozilla-version-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-version-1.2.0.tar", last modified: Fri Nov 25 16:17:59 2022, max compression
+gzip compressed data, was "mozilla-version-2.0.0.tar", last modified: Thu Apr 20 11:56:40 2023, max compression
```

## Comparing `mozilla-version-1.2.0.tar` & `mozilla-version-2.0.0.tar`

### file list

```diff
@@ -1,45 +1,41 @@
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2022-11-25 16:17:59.135987 mozilla-version-1.2.0/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    15922 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/LICENSE
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      139 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/MANIFEST.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      501 2022-11-25 16:17:59.135861 mozilla-version-1.2.0/PKG-INFO
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     7491 2022-11-25 16:16:39.000000 mozilla-version-1.2.0/README.md
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2022-11-25 16:17:59.132225 mozilla-version-1.2.0/mozilla_version/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       60 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/mozilla_version/__init__.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     4989 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/mozilla_version/balrog.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     2586 2022-11-25 16:16:39.000000 mozilla-version-1.2.0/mozilla_version/errors.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      199 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/mozilla_version/fenix.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    25152 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/mozilla_version/gecko.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     2057 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/mozilla_version/maven.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     9623 2022-11-25 16:16:39.000000 mozilla-version-1.2.0/mozilla_version/mobile.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     1359 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/mozilla_version/parser.py
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2022-11-25 16:17:59.134456 mozilla-version-1.2.0/mozilla_version/test/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       87 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/mozilla_version/test/__init__.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     7839 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/mozilla_version/test/test_balrog.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      933 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/mozilla_version/test/test_errors.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      193 2022-07-07 15:15:03.000000 mozilla-version-1.2.0/mozilla_version/test/test_fenix.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    24359 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/mozilla_version/test/test_gecko.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     3534 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/mozilla_version/test/test_maven.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    11956 2022-11-25 16:16:39.000000 mozilla-version-1.2.0/mozilla_version/test/test_mobile.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     7441 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/mozilla_version/test/test_version.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     8080 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/mozilla_version/version.py
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2022-11-25 16:17:59.132996 mozilla-version-1.2.0/mozilla_version.egg-info/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      501 2022-11-25 16:17:58.000000 mozilla-version-1.2.0/mozilla_version.egg-info/PKG-INFO
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     1046 2022-11-25 16:17:59.000000 mozilla-version-1.2.0/mozilla_version.egg-info/SOURCES.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)        1 2022-11-25 16:17:58.000000 mozilla-version-1.2.0/mozilla_version.egg-info/dependency_links.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)        1 2022-11-25 13:12:40.000000 mozilla-version-1.2.0/mozilla_version.egg-info/not-zip-safe
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       19 2022-11-25 16:17:59.000000 mozilla-version-1.2.0/mozilla_version.egg-info/requires.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       16 2022-11-25 16:17:59.000000 mozilla-version-1.2.0/mozilla_version.egg-info/top_level.txt
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2022-11-25 16:17:59.135675 mozilla-version-1.2.0/requirements/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       50 2022-11-25 14:28:46.000000 mozilla-version-1.2.0/requirements/base_py2.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      769 2022-11-25 15:08:21.000000 mozilla-version-1.2.0/requirements/base_py2.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       19 2022-11-25 14:28:49.000000 mozilla-version-1.2.0/requirements/base_py3.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      505 2022-11-25 16:16:39.000000 mozilla-version-1.2.0/requirements/base_py3.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       70 2022-11-25 14:28:49.000000 mozilla-version-1.2.0/requirements/docs.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     8959 2022-11-25 16:16:39.000000 mozilla-version-1.2.0/requirements/docs.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      283 2022-11-25 14:28:46.000000 mozilla-version-1.2.0/requirements/test_py2.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    12052 2022-11-25 16:16:39.000000 mozilla-version-1.2.0/requirements/test_py2.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      147 2022-11-25 14:28:49.000000 mozilla-version-1.2.0/requirements/test_py3.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     8452 2022-11-25 16:16:39.000000 mozilla-version-1.2.0/requirements/test_py3.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       38 2022-11-25 16:17:59.136023 mozilla-version-1.2.0/setup.cfg
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     1345 2022-06-29 08:41:37.000000 mozilla-version-1.2.0/setup.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)        6 2022-11-25 16:16:39.000000 mozilla-version-1.2.0/version.txt
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-04-20 11:56:40.925603 mozilla-version-2.0.0/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    15922 2021-07-20 18:27:27.000000 mozilla-version-2.0.0/LICENSE
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      139 2021-07-20 18:27:27.000000 mozilla-version-2.0.0/MANIFEST.in
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      451 2023-04-20 11:56:40.925603 mozilla-version-2.0.0/PKG-INFO
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7491 2023-04-11 13:53:15.000000 mozilla-version-2.0.0/README.md
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-04-20 11:56:40.921603 mozilla-version-2.0.0/mozilla_version/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)       60 2021-07-20 18:27:27.000000 mozilla-version-2.0.0/mozilla_version/__init__.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4961 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/balrog.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2468 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/errors.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      199 2022-08-25 14:26:48.000000 mozilla-version-2.0.0/mozilla_version/fenix.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    24783 2023-04-20 11:46:42.000000 mozilla-version-2.0.0/mozilla_version/gecko.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1988 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/maven.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     9520 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/mobile.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1335 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/parser.py
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-04-20 11:56:40.925603 mozilla-version-2.0.0/mozilla_version/test/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)       87 2021-07-20 18:27:27.000000 mozilla-version-2.0.0/mozilla_version/test/__init__.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7839 2021-07-20 18:27:27.000000 mozilla-version-2.0.0/mozilla_version/test/test_balrog.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      933 2021-07-20 18:27:27.000000 mozilla-version-2.0.0/mozilla_version/test/test_errors.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      193 2022-08-25 14:26:48.000000 mozilla-version-2.0.0/mozilla_version/test/test_fenix.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    24494 2023-04-20 11:46:42.000000 mozilla-version-2.0.0/mozilla_version/test/test_gecko.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3526 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/test/test_maven.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    11948 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/test/test_mobile.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7441 2021-07-20 18:27:27.000000 mozilla-version-2.0.0/mozilla_version/test/test_version.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7929 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/mozilla_version/version.py
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-04-20 11:56:40.921603 mozilla-version-2.0.0/mozilla_version.egg-info/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      451 2023-04-20 11:56:40.000000 mozilla-version-2.0.0/mozilla_version.egg-info/PKG-INFO
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      928 2023-04-20 11:56:40.000000 mozilla-version-2.0.0/mozilla_version.egg-info/SOURCES.txt
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)        1 2023-04-20 11:56:40.000000 mozilla-version-2.0.0/mozilla_version.egg-info/dependency_links.txt
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)        1 2023-04-11 14:24:42.000000 mozilla-version-2.0.0/mozilla_version.egg-info/not-zip-safe
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)       12 2023-04-20 11:56:40.000000 mozilla-version-2.0.0/mozilla_version.egg-info/requires.txt
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)       16 2023-04-20 11:56:40.000000 mozilla-version-2.0.0/mozilla_version.egg-info/top_level.txt
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-04-20 11:56:40.925603 mozilla-version-2.0.0/requirements/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)       12 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/requirements/base.in
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      363 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/requirements/base.txt
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)       70 2022-08-25 14:26:48.000000 mozilla-version-2.0.0/requirements/docs.in
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    15614 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/requirements/docs.txt
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      143 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/requirements/test.in
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     8589 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/requirements/test.txt
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)       38 2023-04-20 11:56:40.925603 mozilla-version-2.0.0/setup.cfg
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1194 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/setup.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)        6 2023-04-12 09:33:15.000000 mozilla-version-2.0.0/version.txt
```

### Comparing `mozilla-version-1.2.0/LICENSE` & `mozilla-version-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-version-1.2.0/README.md` & `mozilla-version-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mozilla-version-1.2.0/mozilla_version/balrog.py` & `mozilla-version-2.0.0/mozilla_version/balrog.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,21 +54,21 @@
         raise PatternNotMatchedError(string, patterns=('unknown product',))
     return product
 
 
 def _products_must_be_identical(method):
     def checker(this, other):
         if this.product != other.product:
-            raise ValueError('Cannot compare "{}" and "{}"'.format(this.product, other.product))
+            raise ValueError(f'Cannot compare "{this.product}" and "{other.product}"')
         return method(this, other)
     return checker
 
 
 @attr.s(frozen=True, eq=False, hash=True)
-class BalrogReleaseName(object):
+class BalrogReleaseName:
     """Class that validates and handles Balrog release names.
 
     Raises:
         PatternNotMatchedError: if a parsed string doesn't match the pattern of a valid release
         MissingFieldError: if a mandatory field is missing in the string. Mandatory fields are
             `product`, `major_number`, `minor_number`, and `build_number`
         ValueError: if an integer can't be cast or is not (strictly) positive
@@ -105,15 +105,15 @@
 
     def __str__(self):
         """Implement string representation.
 
         Computes a new string based on the given attributes.
         """
         version_string = str(self.version).replace('build', '-build')
-        return '{}-{}'.format(self.product, version_string)
+        return f'{self.product}-{version_string}'
 
     @_products_must_be_identical
     def __eq__(self, other):
         """Implement `==` operator."""
         return self.version == other.version
 
     @_products_must_be_identical
```

### Comparing `mozilla-version-1.2.0/mozilla_version/errors.py` & `mozilla-version-2.0.0/mozilla_version/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,34 +11,34 @@
 
     def __init__(self, string, patterns):
         """Initialize error."""
         number_of_patterns = len(patterns)
         if number_of_patterns == 0:
             raise ValueError('At least one pattern must be provided')
         elif number_of_patterns == 1:
-            message = '"{}" does not match the pattern: {}'.format(string, patterns[0])
+            message = f'"{string}" does not match the pattern: {patterns[0]}'
         else:
             message = '"{}" does not match the patterns:\n - {}'.format(
                 string,
                 '\n - '.join(patterns)
             )
 
-        super(PatternNotMatchedError, self).__init__(message)
+        super().__init__(message)
 
 
 class NoVersionTypeError(ValueError):
     """Error when `version_string` matched the pattern, but was unable to find its type.
 
     Args:
         version_string (str): The string it was unable to guess the type.
     """
 
     def __init__(self, version_string):
         """Initialize error."""
-        super(NoVersionTypeError, self).__init__(
+        super().__init__(
             'Version "{}" matched the pattern of a valid version, but it is unable to '
             'find what type it is. This is likely a bug in mozilla-version'.format(
                 version_string
             )
         )
 
 
@@ -48,28 +48,28 @@
     Args:
         version_string (str): The string it was unable to extract a given field.
         field_name (str): The name of the missing field.
     """
 
     def __init__(self, version_string, field_name):
         """Initialize error."""
-        super(MissingFieldError, self).__init__(
-            'Release "{}" does not contain a valid {}'.format(version_string, field_name)
+        super().__init__(
+            f'Release "{version_string}" does not contain a valid {field_name}'
         )
 
 
 class TooManyTypesError(ValueError):
     """Error when `version_string` has too many types.
 
     Args:
         version_string (str): The string that gave too many types.
         first_matched_type (str): The name of the first detected type.
         second_matched_type (str): The name of the second detected type
     """
 
     def __init__(self, version_string, first_matched_type, second_matched_type):
         """Initialize error."""
-        super(TooManyTypesError, self).__init__(
+        super().__init__(
             'Release "{}" cannot match types "{}" and "{}"'.format(
                 version_string, first_matched_type, second_matched_type
             )
         )
```

### Comparing `mozilla-version-1.2.0/mozilla_version/gecko.py` & `mozilla-version-2.0.0/mozilla_version/gecko.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,16 +45,14 @@
         FirefoxVersion(60, 0, 1, is_esr=True))      # '60.0.1esr'
 
 """
 
 import attr
 import re
 
-from future.utils import raise_from
-
 from mozilla_version.errors import (
     PatternNotMatchedError, TooManyTypesError, NoVersionTypeError
 )
 from mozilla_version.parser import strictly_positive_int_or_none
 from mozilla_version.version import BaseVersion, VersionType
 
 
@@ -129,15 +127,15 @@
 
     _OPTIONAL_NUMBERS = BaseVersion._OPTIONAL_NUMBERS + (
         'old_fourth_number', 'release_candidate_number', 'beta_number', 'build_number'
     )
 
     _ALL_NUMBERS = BaseVersion._ALL_NUMBERS + _OPTIONAL_NUMBERS
 
-    _KNOWN_ESR_MAJOR_NUMBERS = (10, 17, 24, 31, 38, 45, 52, 60, 68, 78, 91, 102)
+    _KNOWN_ESR_MAJOR_NUMBERS = (10, 17, 24, 31, 38, 45, 52, 60, 68, 78, 91, 102, 115)
 
     _LAST_AURORA_DEVEDITION_AS_VERSION_TYPE = 54
 
     build_number = attr.ib(type=int, converter=strictly_positive_int_or_none, default=None)
     beta_number = attr.ib(type=int, converter=strictly_positive_int_or_none, default=None)
     is_nightly = attr.ib(type=bool, default=False)
     is_aurora_or_devedition = attr.ib(type=bool, default=False)
@@ -221,15 +219,15 @@
 
         if error_messages:
             raise PatternNotMatchedError(self, patterns=error_messages)
 
     @classmethod
     def parse(cls, version_string):
         """Construct an object representing a valid Firefox version number."""
-        return super(GeckoVersion, cls).parse(
+        return super().parse(
             version_string, regex_groups=('is_nightly', 'is_aurora_or_devedition', 'is_esr')
         )
 
     @property
     def is_beta(self):
         """Return `True` if `GeckoVersion` was built with a string matching a beta version."""
         return self.beta_number is not None
@@ -264,32 +262,32 @@
         ))
 
     def __str__(self):
         """Implement string representation.
 
         Computes a new string based on the given attributes.
         """
-        string = super(GeckoVersion, self).__str__()
+        string = super().__str__()
 
         if self.old_fourth_number is not None:
-            string = '{}.{}'.format(string, self.old_fourth_number)
+            string = f'{string}.{self.old_fourth_number}'
 
         if self.is_nightly:
-            string = '{}a1'.format(string)
+            string = f'{string}a1'
         elif self.is_aurora_or_devedition:
-            string = '{}a2'.format(string)
+            string = f'{string}a2'
         elif self.is_beta:
-            string = '{}b{}'.format(string, self.beta_number)
+            string = f'{string}b{self.beta_number}'
         elif self.is_release_candidate:
-            string = '{}rc{}'.format(string, self.release_candidate_number)
+            string = f'{string}rc{self.release_candidate_number}'
         elif self.is_esr:
-            string = '{}esr'.format(string)
+            string = f'{string}esr'
 
         if self.build_number is not None:
-            string = '{}build{}'.format(string, self.build_number)
+            string = f'{string}build{self.build_number}'
 
         return string
 
     def __eq__(self, other):
         """Implement `==` operator.
 
         A version is considered equal to another if all numbers match and if they are of the same
@@ -310,31 +308,31 @@
                 assert GeckoVersion.parse('60.0') != GeckoVersion.parse('60.0.1')
                 assert GeckoVersion.parse('60.0') != GeckoVersion.parse('60.0a1')
                 assert GeckoVersion.parse('60.0') != GeckoVersion.parse('60.0a2')
                 assert GeckoVersion.parse('60.0') != GeckoVersion.parse('60.0b1')
                 assert GeckoVersion.parse('60.0build1') != GeckoVersion.parse('60.0build2')
 
         """
-        return super(GeckoVersion, self).__eq__(other)
+        return super().__eq__(other)
 
     def _compare(self, other):
         """Compare this release with another.
 
         Returns:
             0 if equal
             < 0 is this precedes the other
             > 0 if the other precedes this
 
         """
         if isinstance(other, str):
             other = GeckoVersion.parse(other)
         elif not isinstance(other, GeckoVersion):
-            raise ValueError('Cannot compare "{}", type not supported!'.format(other))
+            raise ValueError(f'Cannot compare "{other}", type not supported!')
 
-        difference = super(GeckoVersion, self)._compare(other)
+        difference = super()._compare(other)
         if difference != 0:
             return difference
 
         difference = self._substract_other_number_from_this_number(other, 'old_fourth_number')
         if difference != 0:
             return difference
 
@@ -365,15 +363,15 @@
     def _compare_version_type(self, other):
         return self.version_type.compare(other.version_type)
 
     def _create_bump_kwargs(self, field):
         if field == 'build_number' and self.build_number is None:
             raise ValueError('Cannot bump the build number if it is not already set')
 
-        bump_kwargs = super(GeckoVersion, self)._create_bump_kwargs(field)
+        bump_kwargs = super()._create_bump_kwargs(field)
 
         if field == 'major_number' and self.is_esr:
             current_esr_index = self._KNOWN_ESR_MAJOR_NUMBERS.index(self.major_number)
             try:
                 next_major_esr_number = self._KNOWN_ESR_MAJOR_NUMBERS[current_esr_index + 1]
             except IndexError:
                 raise ValueError(
@@ -431,19 +429,18 @@
              * 31.0build1 is bumped to 31.0esrbuild1
              * 31.0build2 is bumped to 31.0esrbuild1
 
         """
         try:
             return self.__class__(**self._create_bump_version_type_kwargs())
         except (ValueError, PatternNotMatchedError) as e:
-            # TODO Use "raise from" statement once Python 2 support is dropped
-            raise_from(ValueError(
+            raise ValueError(
                 'Cannot bump version type for version "{}". New version number is not valid. '
                 'Cause: {}'.format(self, e)
-            ), e)
+            ) from e
 
     def _create_bump_version_type_kwargs(self):
         bump_version_type_kwargs = {
             'major_number': self.major_number,
             'minor_number': self.minor_number,
             'patch_number': self.patch_number,
         }
@@ -477,15 +474,15 @@
                 if number_type != 'build_number'
             ):
                 if self.build_number is None:
                     return
                 elif self.build_number == edge_case.get('build_number', None):
                     return
 
-        super(_VersionWithEdgeCases, self).__attrs_post_init__()
+        super().__attrs_post_init__()
 
 
 class FirefoxVersion(_VersionWithEdgeCases):
     """Class that validates and handles Firefox version numbers."""
 
     _RELEASED_EDGE_CASES = ({
         'major_number': 1,
@@ -579,21 +576,21 @@
             self.minor_number > 0 and
             self.patch_number is None
         ):
             return
 
         if self.major_number > self._LAST_FENNEC_VERSION:
             raise PatternNotMatchedError(
-                self, patterns=('Last Fennec version is {}'.format(self._LAST_FENNEC_VERSION),)
+                self, patterns=(f'Last Fennec version is {self._LAST_FENNEC_VERSION}',)
             )
 
-        super(FennecVersion, self).__attrs_post_init__()
+        super().__attrs_post_init__()
 
     def _create_bump_kwargs(self, field):
-        kwargs = super(FennecVersion, self)._create_bump_kwargs(field)
+        kwargs = super()._create_bump_kwargs(field)
 
         if (
             field != 'patch_number' and
             kwargs['major_number'] == self._LAST_FENNEC_VERSION and
             (kwargs['is_nightly'] or kwargs.get('beta_number'))
         ):
             del kwargs['patch_number']
@@ -667,9 +664,9 @@
         -(?P<build_number>\d+)$""", re.VERBOSE)
 
     def __str__(self):
         """Implement string representation.
 
         Returns format like "63.0b7-1"
         """
-        string = super(GeckoSnapVersion, self).__str__()
+        string = super().__str__()
         return string.replace('build', '-')
```

### Comparing `mozilla-version-1.2.0/mozilla_version/maven.py` & `mozilla-version-2.0.0/mozilla_version/maven.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,35 +22,35 @@
         \.(?P<minor_number>\d+)
         (\.(?P<patch_number>\d+))?
         (?P<is_snapshot>-SNAPSHOT)?$""", re.VERBOSE)
 
     @classmethod
     def parse(cls, version_string):
         """Construct an object representing a valid Maven version number."""
-        return super(MavenVersion, cls).parse(version_string, regex_groups=('is_snapshot', ))
+        return super().parse(version_string, regex_groups=('is_snapshot', ))
 
     def __str__(self):
         """Implement string representation.
 
         Computes a new string based on the given attributes.
         """
-        string = super(MavenVersion, self).__str__()
+        string = super().__str__()
 
         if self.is_snapshot:
-            string = '{}-SNAPSHOT'.format(string)
+            string = f'{string}-SNAPSHOT'
 
         return string
 
     def _compare(self, other):
         if isinstance(other, str):
             other = MavenVersion.parse(other)
         elif not isinstance(other, MavenVersion):
-            raise ValueError('Cannot compare "{}", type not supported!'.format(other))
+            raise ValueError(f'Cannot compare "{other}", type not supported!')
 
-        difference = super(MavenVersion, self)._compare(other)
+        difference = super()._compare(other)
         if difference != 0:
             return difference
 
         if not self.is_snapshot and other.is_snapshot:
             return 1
         elif self.is_snapshot and not other.is_snapshot:
             return -1
```

### Comparing `mozilla-version-1.2.0/mozilla_version/mobile.py` & `mozilla-version-2.0.0/mozilla_version/mobile.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
         if error_messages:
             raise PatternNotMatchedError(self, patterns=error_messages)
 
     @classmethod
     def parse(cls, version_string):
         """Construct an object representing a valid Firefox version number."""
-        mobile_version = super(MobileVersion, cls).parse(
+        mobile_version = super().parse(
             version_string, regex_groups=('is_nightly',)
         )
 
         # Betas are supported in both the old and the gecko pattern. Let's make sure
         # the string we got follows the right rules
         if mobile_version.is_beta:
             if mobile_version.is_gecko_pattern and '-beta.' in version_string:
@@ -184,29 +184,29 @@
                 minor_number=self.minor_number,
                 patch_number=self.patch_number,
                 build_number=self.build_number,
                 beta_number=self.beta_number,
                 is_nightly=self.is_nightly,
             ))
         else:
-            string = super(MobileVersion, self).__str__()
+            string = super().__str__()
             if self.is_beta:
-                string = '{}-beta.{}'.format(string, self.beta_number)
+                string = f'{string}-beta.{self.beta_number}'
             elif self.is_release_candidate:
-                string = '{}-rc.{}'.format(string, self.release_candidate_number)
+                string = f'{string}-rc.{self.release_candidate_number}'
 
         return string
 
     def _compare(self, other):
         if isinstance(other, str):
             other = MobileVersion.parse(other)
         elif not isinstance(other, MobileVersion):
-            raise ValueError('Cannot compare "{}", type not supported!'.format(other))
+            raise ValueError(f'Cannot compare "{other}", type not supported!')
 
-        difference = super(MobileVersion, self)._compare(other)
+        difference = super()._compare(other)
         if difference != 0:
             return difference
 
         channel_difference = self._compare_version_type(other)
         if channel_difference != 0:
             return channel_difference
 
@@ -222,15 +222,15 @@
 
         return 0
 
     def _compare_version_type(self, other):
         return self.version_type.compare(other.version_type)
 
     def _create_bump_kwargs(self, field):
-        bump_kwargs = super(MobileVersion, self)._create_bump_kwargs(field)
+        bump_kwargs = super()._create_bump_kwargs(field)
 
         if field != 'build_number' and bump_kwargs.get('build_number') == 0:
             del bump_kwargs['build_number']
         if bump_kwargs.get('beta_number') == 0:
             if self.is_beta:
                 bump_kwargs['beta_number'] = 1
             else:
```

### Comparing `mozilla-version-1.2.0/mozilla_version/parser.py` & `mozilla-version-2.0.0/mozilla_version/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,27 +22,27 @@
     except IndexError:
         return False
 
 
 def positive_int(val):
     """Parse `val` into a positive integer."""
     if isinstance(val, float):
-        raise ValueError('"{}" must not be a float'.format(val))
+        raise ValueError(f'"{val}" must not be a float')
     val = int(val)
     if val >= 0:
         return val
-    raise ValueError('"{}" must be positive'.format(val))
+    raise ValueError(f'"{val}" must be positive')
 
 
 def positive_int_or_none(val):
     """Parse `val` into either `None` or a positive integer."""
     if val is None:
         return val
     return positive_int(val)
 
 
 def strictly_positive_int_or_none(val):
     """Parse `val` into either `None` or a strictly positive integer."""
     val = positive_int_or_none(val)
     if val is None or val > 0:
         return val
-    raise ValueError('"{}" must be strictly positive'.format(val))
+    raise ValueError(f'"{val}" must be strictly positive')
```

### Comparing `mozilla-version-1.2.0/mozilla_version/test/test_balrog.py` & `mozilla-version-2.0.0/mozilla_version/test/test_balrog.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-1.2.0/mozilla_version/test/test_errors.py` & `mozilla-version-2.0.0/mozilla_version/test/test_errors.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-1.2.0/mozilla_version/test/test_gecko.py` & `mozilla-version-2.0.0/mozilla_version/test/test_gecko.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
  - Release candidate number cannot be defined starting Gecko 5
  - Minor number and patch number cannot be both equal to 0'''
 
 
 @pytest.mark.parametrize('version_string, expected_type', VALID_VERSIONS.items())
 def test_gecko_version_is_of_a_defined_type(version_string, expected_type):
     release = GeckoVersion.parse(version_string)
-    assert getattr(release, 'is_{}'.format(expected_type))
+    assert getattr(release, f'is_{expected_type}')
 
 
 @pytest.mark.parametrize('previous, next', (
     ('32.0', '33.0'),
     ('32.0', '32.1.0'),
     ('32.0', '32.0.1'),
     ('32.0build1', '32.0build2'),
@@ -347,14 +347,18 @@
     ('78.0esr', 'major_number', '91.0esr'),
     ('78.0.1esr', 'major_number', '91.0esr'),
     ('78.1.0esr', 'major_number', '91.0esr'),
 
     ('91.0esr', 'major_number', '102.0esr'),
     ('91.0.1esr', 'major_number', '102.0esr'),
     ('91.1.0esr', 'major_number', '102.0esr'),
+
+    ('102.0esr', 'major_number', '115.0esr'),
+    ('102.0.1esr', 'major_number', '115.0esr'),
+    ('102.1.0esr', 'major_number', '115.0esr'),
 ))
 def test_gecko_version_bump(version_string, field, expected):
     version = GeckoVersion.parse(version_string)
     assert str(version.bump(field)) == expected
 
 
 @pytest.mark.parametrize('version_string, field', (
@@ -381,17 +385,17 @@
     ('32.0b1', 'patch_number'),
     ('32.0b1', 'release_candidate_number'),
     ('32.0b1', 'old_fourth_number'),
     ('32.0a2', 'build_number'),
 
     ('32.0', 'build_number'),
 
-    ('102.0esr', 'major_number'),
-    ('102.0.1esr', 'major_number'),
-    ('102.1.0esr', 'major_number'),
+    ('115.0esr', 'major_number'),
+    ('115.0.1esr', 'major_number'),
+    ('115.1.0esr', 'major_number'),
 ))
 def test_gecko_version_bump_raises(version_string, field):
     version = GeckoVersion.parse(version_string)
     with pytest.raises(ValueError):
         version.bump(field)
```

### Comparing `mozilla-version-1.2.0/mozilla_version/test/test_maven.py` & `mozilla-version-2.0.0/mozilla_version/test/test_maven.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 @pytest.mark.parametrize('version_string, expected_type', (
     ('32.0', 'release'),
     ('32.0-SNAPSHOT', 'snapshot'),
 ))
 def test_maven_version_is_of_a_defined_type(version_string, expected_type):
     release = MavenVersion.parse(version_string)
-    assert getattr(release, 'is_{}'.format(expected_type))
+    assert getattr(release, f'is_{expected_type}')
 
 
 def test_maven_version_are_never_of_certain_types():
     release = MavenVersion(32, 0)
     assert not release.is_beta
     assert not release.is_release_candidate
```

### Comparing `mozilla-version-1.2.0/mozilla_version/test/test_mobile.py` & `mozilla-version-2.0.0/mozilla_version/test/test_mobile.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     with pytest.raises(ExpectedErrorType):
         MobileVersion.parse(version_string)
 
 
 @pytest.mark.parametrize('version_string, expected_type', VALID_VERSIONS.items())
 def test_mobile_version_is_of_a_defined_type(version_string, expected_type):
     release = MobileVersion.parse(version_string)
-    assert getattr(release, 'is_{}'.format(expected_type))
+    assert getattr(release, f'is_{expected_type}')
 
 
 @pytest.mark.parametrize('previous, next', (
     ('2.0.0', '3.0.0'),
     ('2.0.0', '3.1.0'),
     ('2.0.0', '3.0.1'),
```

### Comparing `mozilla-version-1.2.0/mozilla_version/test/test_version.py` & `mozilla-version-2.0.0/mozilla_version/test/test_version.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-1.2.0/mozilla_version/version.py` & `mozilla-version-2.0.0/mozilla_version/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Defines common characteristics of a version at Mozilla."""
 
 import attr
 import re
 
 from enum import Enum
-from future.utils import raise_from
 
 from mozilla_version.errors import MissingFieldError, PatternNotMatchedError
 from mozilla_version.parser import (
     get_value_matched_by_regex,
     does_regex_have_group,
     positive_int,
     positive_int_or_none
 )
 
 
 @attr.s(frozen=True, eq=False, hash=True)
-class BaseVersion(object):
+class BaseVersion:
     """Class that validates and handles general version numbers."""
 
     major_number = attr.ib(type=int, converter=positive_int)
     minor_number = attr.ib(type=int, converter=positive_int)
     patch_number = attr.ib(type=int, converter=positive_int_or_none, default=None)
 
     _MANDATORY_NUMBERS = ('major_number', 'minor_number')
@@ -98,15 +97,15 @@
             < 0 is this precedes the other
             > 0 if the other precedes this
 
         """
         if isinstance(other, str):
             other = BaseVersion.parse(other)
         elif not isinstance(other, BaseVersion):
-            raise ValueError('Cannot compare "{}", type not supported!'.format(other))
+            raise ValueError(f'Cannot compare "{other}", type not supported!')
 
         for field in ('major_number', 'minor_number', 'patch_number'):
             difference = self._substract_other_number_from_this_number(other, field)
             if difference != 0:
                 return difference
 
         return 0
@@ -136,22 +135,21 @@
              * 32.0 is bumped to 32.1.0, because patch number must be defined if the minor number
                is not 0.
 
         """
         try:
             return self.__class__(**self._create_bump_kwargs(field))
         except (ValueError, PatternNotMatchedError) as e:
-            # TODO Use "raise from" statement once Python 2 support is dropped
-            raise_from(ValueError(
-                'Cannot bump "{}". New version number is not valid. Cause: {}'.format(field, e)
-            ), e)
+            raise ValueError(
+                f'Cannot bump "{field}". New version number is not valid. Cause: {e}'
+            ) from e
 
     def _create_bump_kwargs(self, field):
         if field not in self._ALL_NUMBERS:
-            raise ValueError('Unknown field "{}"'.format(field))
+            raise ValueError(f'Unknown field "{field}"')
 
         kwargs = {}
         has_requested_field_been_met = False
         should_set_optional_numbers = False
         for current_field in self._ALL_NUMBERS:
             current_number = getattr(self, current_field, None)
             if current_field == field:
```

### Comparing `mozilla-version-1.2.0/mozilla_version.egg-info/SOURCES.txt` & `mozilla-version-2.0.0/mozilla_version.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -22,17 +22,13 @@
 mozilla_version/test/test_balrog.py
 mozilla_version/test/test_errors.py
 mozilla_version/test/test_fenix.py
 mozilla_version/test/test_gecko.py
 mozilla_version/test/test_maven.py
 mozilla_version/test/test_mobile.py
 mozilla_version/test/test_version.py
-requirements/base_py2.in
-requirements/base_py2.txt
-requirements/base_py3.in
-requirements/base_py3.txt
+requirements/base.in
+requirements/base.txt
 requirements/docs.in
 requirements/docs.txt
-requirements/test_py2.in
-requirements/test_py2.txt
-requirements/test_py3.in
-requirements/test_py3.txt
+requirements/test.in
+requirements/test.txt
```

### Comparing `mozilla-version-1.2.0/requirements/docs.txt` & `mozilla-version-2.0.0/requirements/test.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,157 +1,145 @@
-# SHA1:4c6e4eac10254b990df3cb2db19acfb029cfe305
+# SHA1:30222ce55ac54f3046b8d206ba4d1d77f7540408
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-alabaster==0.7.12 \
-    --hash=sha256:446438bdcca0e05bd45ea2de1668c1d9b032e1a9154c2c259092d77031ddd359 \
-    --hash=sha256:a661d72d58e6ea8a57f7a86e37d86716863ee5e92788398526d58b26a4e4dc02
-    # via sphinx
-babel==2.11.0 \
-    --hash=sha256:1ad3eca1c885218f6dce2ab67291178944f810a10a9b5f3cb8382a5a232b64fe \
-    --hash=sha256:5ef4b3226b0180dedded4229651c8b0e1a3a6a2837d45a073272f313e4cf97f6
-    # via sphinx
-certifi==2022.9.24 \
-    --hash=sha256:0d9c601124e5a6ba9712dbc60d9c53c21e34f5f641fe83002317394311bdce14 \
-    --hash=sha256:90c1a32f1d68f940488354e36370f6cca89f0f106db09518524c88d6ed83f382
-    # via requests
-charset-normalizer==2.1.1 \
-    --hash=sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845 \
-    --hash=sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f
-    # via requests
-docutils==0.19 \
-    --hash=sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6 \
-    --hash=sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc
+-r base.txt
+coverage[toml]==7.2.3 \
+    --hash=sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93 \
+    --hash=sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013 \
+    --hash=sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f \
+    --hash=sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21 \
+    --hash=sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462 \
+    --hash=sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc \
+    --hash=sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df \
+    --hash=sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1 \
+    --hash=sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235 \
+    --hash=sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934 \
+    --hash=sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9 \
+    --hash=sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1 \
+    --hash=sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48 \
+    --hash=sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4 \
+    --hash=sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe \
+    --hash=sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a \
+    --hash=sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b \
+    --hash=sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21 \
+    --hash=sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d \
+    --hash=sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa \
+    --hash=sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367 \
+    --hash=sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535 \
+    --hash=sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152 \
+    --hash=sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e \
+    --hash=sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539 \
+    --hash=sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1 \
+    --hash=sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925 \
+    --hash=sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0 \
+    --hash=sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2 \
+    --hash=sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab \
+    --hash=sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841 \
+    --hash=sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30 \
+    --hash=sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91 \
+    --hash=sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c \
+    --hash=sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257 \
+    --hash=sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9 \
+    --hash=sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040 \
+    --hash=sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911 \
+    --hash=sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623 \
+    --hash=sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259 \
+    --hash=sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c \
+    --hash=sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79 \
+    --hash=sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5 \
+    --hash=sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4 \
+    --hash=sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4 \
+    --hash=sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22 \
+    --hash=sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd \
+    --hash=sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1 \
+    --hash=sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910 \
+    --hash=sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859 \
+    --hash=sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312
     # via
-    #   m2r2
-    #   sphinx
-idna==3.4 \
-    --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
-    --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
-    # via requests
-imagesize==1.4.1 \
-    --hash=sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b \
-    --hash=sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a
-    # via sphinx
-jinja2==3.1.2 \
-    --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
-    --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
+    #   -r requirements/test.in
+    #   pytest-cov
+exceptiongroup==1.1.1 \
+    --hash=sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e \
+    --hash=sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785
+    # via pytest
+flake8==5.0.4 \
+    --hash=sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db \
+    --hash=sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248
     # via
-    #   readthedocs-sphinx-ext
-    #   sphinx
-m2r2==0.3.3 \
-    --hash=sha256:2ee32a5928c3598b67c70e6d22981ec936c03d5bfd2f64229e77678731952f16 \
-    --hash=sha256:f9b6e9efbc2b6987dbd43d2fd15a6d115ba837d8158ae73295542635b4086e75
-    # via -r requirements/docs.in
-markupsafe==2.1.1 \
-    --hash=sha256:0212a68688482dc52b2d45013df70d169f542b7394fc744c02a57374a4207003 \
-    --hash=sha256:089cf3dbf0cd6c100f02945abeb18484bd1ee57a079aefd52cffd17fba910b88 \
-    --hash=sha256:10c1bfff05d95783da83491be968e8fe789263689c02724e0c691933c52994f5 \
-    --hash=sha256:33b74d289bd2f5e527beadcaa3f401e0df0a89927c1559c8566c066fa4248ab7 \
-    --hash=sha256:3799351e2336dc91ea70b034983ee71cf2f9533cdff7c14c90ea126bfd95d65a \
-    --hash=sha256:3ce11ee3f23f79dbd06fb3d63e2f6af7b12db1d46932fe7bd8afa259a5996603 \
-    --hash=sha256:421be9fbf0ffe9ffd7a378aafebbf6f4602d564d34be190fc19a193232fd12b1 \
-    --hash=sha256:43093fb83d8343aac0b1baa75516da6092f58f41200907ef92448ecab8825135 \
-    --hash=sha256:46d00d6cfecdde84d40e572d63735ef81423ad31184100411e6e3388d405e247 \
-    --hash=sha256:4a33dea2b688b3190ee12bd7cfa29d39c9ed176bda40bfa11099a3ce5d3a7ac6 \
-    --hash=sha256:4b9fe39a2ccc108a4accc2676e77da025ce383c108593d65cc909add5c3bd601 \
-    --hash=sha256:56442863ed2b06d19c37f94d999035e15ee982988920e12a5b4ba29b62ad1f77 \
-    --hash=sha256:671cd1187ed5e62818414afe79ed29da836dde67166a9fac6d435873c44fdd02 \
-    --hash=sha256:694deca8d702d5db21ec83983ce0bb4b26a578e71fbdbd4fdcd387daa90e4d5e \
-    --hash=sha256:6a074d34ee7a5ce3effbc526b7083ec9731bb3cbf921bbe1d3005d4d2bdb3a63 \
-    --hash=sha256:6d0072fea50feec76a4c418096652f2c3238eaa014b2f94aeb1d56a66b41403f \
-    --hash=sha256:6fbf47b5d3728c6aea2abb0589b5d30459e369baa772e0f37a0320185e87c980 \
-    --hash=sha256:7f91197cc9e48f989d12e4e6fbc46495c446636dfc81b9ccf50bb0ec74b91d4b \
-    --hash=sha256:86b1f75c4e7c2ac2ccdaec2b9022845dbb81880ca318bb7a0a01fbf7813e3812 \
-    --hash=sha256:8dc1c72a69aa7e082593c4a203dcf94ddb74bb5c8a731e4e1eb68d031e8498ff \
-    --hash=sha256:8e3dcf21f367459434c18e71b2a9532d96547aef8a871872a5bd69a715c15f96 \
-    --hash=sha256:8e576a51ad59e4bfaac456023a78f6b5e6e7651dcd383bcc3e18d06f9b55d6d1 \
-    --hash=sha256:96e37a3dc86e80bf81758c152fe66dbf60ed5eca3d26305edf01892257049925 \
-    --hash=sha256:97a68e6ada378df82bc9f16b800ab77cbf4b2fada0081794318520138c088e4a \
-    --hash=sha256:99a2a507ed3ac881b975a2976d59f38c19386d128e7a9a18b7df6fff1fd4c1d6 \
-    --hash=sha256:a49907dd8420c5685cfa064a1335b6754b74541bbb3706c259c02ed65b644b3e \
-    --hash=sha256:b09bf97215625a311f669476f44b8b318b075847b49316d3e28c08e41a7a573f \
-    --hash=sha256:b7bd98b796e2b6553da7225aeb61f447f80a1ca64f41d83612e6139ca5213aa4 \
-    --hash=sha256:b87db4360013327109564f0e591bd2a3b318547bcef31b468a92ee504d07ae4f \
-    --hash=sha256:bcb3ed405ed3222f9904899563d6fc492ff75cce56cba05e32eff40e6acbeaa3 \
-    --hash=sha256:d4306c36ca495956b6d568d276ac11fdd9c30a36f1b6eb928070dc5360b22e1c \
-    --hash=sha256:d5ee4f386140395a2c818d149221149c54849dfcfcb9f1debfe07a8b8bd63f9a \
-    --hash=sha256:dda30ba7e87fbbb7eab1ec9f58678558fd9a6b8b853530e176eabd064da81417 \
-    --hash=sha256:e04e26803c9c3851c931eac40c695602c6295b8d432cbe78609649ad9bd2da8a \
-    --hash=sha256:e1c0b87e09fa55a220f058d1d49d3fb8df88fbfab58558f1198e08c1e1de842a \
-    --hash=sha256:e72591e9ecd94d7feb70c1cbd7be7b3ebea3f548870aa91e2732960fa4d57a37 \
-    --hash=sha256:e8c843bbcda3a2f1e3c2ab25913c80a3c5376cd00c6e8c4a86a89a28c8dc5452 \
-    --hash=sha256:efc1913fd2ca4f334418481c7e595c00aad186563bbc1ec76067848c7ca0a933 \
-    --hash=sha256:f121a1420d4e173a5d96e47e9a0c0dcff965afdf1626d28de1460815f7c4ee7a \
-    --hash=sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7
-    # via jinja2
-mistune==0.8.4 \
-    --hash=sha256:59a3429db53c50b5c6bcc8a07f8848cb00d7dc8bdb431a4ab41920d201d4756e \
-    --hash=sha256:88a1051873018da288eee8538d476dffe1262495144b33ecb586c4ab266bb8d4
-    # via m2r2
-packaging==21.3 \
-    --hash=sha256:dd47c42927d89ab911e606518907cc2d3a1f38bbd026385970643f9c5b8ecfeb \
-    --hash=sha256:ef103e05f519cdc783ae24ea4e2e0f508a9c99b2d4969652eed6a2e1ea5bd522
+    #   -r requirements/test.in
+    #   flake8-docstrings
+flake8-docstrings==1.7.0 \
+    --hash=sha256:4c8cc748dc16e6869728699e5d0d685da9a10b0ea718e090b1ba088e67a941af \
+    --hash=sha256:51f2344026da083fc084166a9353f5082b01f72901df422f74b4d953ae88ac75
+    # via -r requirements/test.in
+importlib-metadata==4.2.0 \
+    --hash=sha256:057e92c15bc8d9e8109738a48db0ccb31b4d9d5cfbee5a8670879a30be66304b \
+    --hash=sha256:b7e52a1f8dec14a75ea73e0891f3060099ca1d8e6a462a4dff11c3e119ea1b31
     # via
-    #   readthedocs-sphinx-ext
-    #   sphinx
-pygments==2.13.0 \
-    --hash=sha256:56a8508ae95f98e2b9bdf93a6be5ae3f7d8af858b43e02c5a2ff083726be40c1 \
-    --hash=sha256:f643f331ab57ba3c9d89212ee4a2dabc6e94f117cf4eefde99a0574720d14c42
-    # via sphinx
-pyparsing==3.0.9 \
-    --hash=sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb \
-    --hash=sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc
-    # via packaging
-pytz==2022.6 \
-    --hash=sha256:222439474e9c98fced559f1709d89e6c9cbf8d79c794ff3eb9f8800064291427 \
-    --hash=sha256:e89512406b793ca39f5971bc999cc538ce125c0e51c27941bef4568b460095e2
-    # via babel
-readthedocs-sphinx-ext==2.2.0 \
-    --hash=sha256:d801f0bfb125d2837f18f40451462528d4a97eefd8de8a12ad526b4f1ce14205 \
-    --hash=sha256:e5effcd825816111a377ab7a897b819215138f8e5e8acc86f99218328f957240
-    # via -r requirements/docs.in
-requests==2.28.1 \
-    --hash=sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983 \
-    --hash=sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349
+    #   flake8
+    #   pluggy
+    #   pydocstyle
+    #   pytest
+iniconfig==2.0.0 \
+    --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
+    --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
+    # via pytest
+mccabe==0.7.0 \
+    --hash=sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325 \
+    --hash=sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e
+    # via flake8
+more-itertools==9.1.0 ; python_version >= "3.0" \
+    --hash=sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d \
+    --hash=sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3
+    # via -r requirements/test.in
+packaging==23.0 \
+    --hash=sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2 \
+    --hash=sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97
+    # via pytest
+pluggy==1.0.0 \
+    --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
+    --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
+    # via pytest
+pycodestyle==2.9.1 \
+    --hash=sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785 \
+    --hash=sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b
+    # via flake8
+pydocstyle==6.3.0 \
+    --hash=sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019 \
+    --hash=sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1
+    # via flake8-docstrings
+pyflakes==2.5.0 \
+    --hash=sha256:4579f67d887f804e67edb544428f264b7b24f435b263c4614f384135cea553d2 \
+    --hash=sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3
+    # via flake8
+pytest==7.3.0 ; python_version >= "3.0" \
+    --hash=sha256:58ecc27ebf0ea643ebfdf7fb1249335da761a00c9f955bcd922349bcb68ee57d \
+    --hash=sha256:933051fa1bfbd38a21e73c3960cebdad4cf59483ddba7696c48509727e17f201
     # via
-    #   readthedocs-sphinx-ext
-    #   sphinx
+    #   -r requirements/test.in
+    #   pytest-cov
+pytest-cov==4.0.0 \
+    --hash=sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b \
+    --hash=sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470
+    # via -r requirements/test.in
 snowballstemmer==2.2.0 \
     --hash=sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1 \
     --hash=sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a
-    # via sphinx
-sphinx==5.3.0 \
-    --hash=sha256:060ca5c9f7ba57a08a1219e547b269fadf125ae25b06b9fa7f66768efb652d6d \
-    --hash=sha256:51026de0a9ff9fc13c05d74913ad66047e104f56a129ff73e174eb5c3ee794b5
-    # via -r requirements/docs.in
-sphinxcontrib-applehelp==1.0.2 \
-    --hash=sha256:806111e5e962be97c29ec4c1e7fe277bfd19e9652fb1a4392105b43e01af885a \
-    --hash=sha256:a072735ec80e7675e3f432fcae8610ecf509c5f1869d17e2eecff44389cdbc58
-    # via sphinx
-sphinxcontrib-devhelp==1.0.2 \
-    --hash=sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e \
-    --hash=sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4
-    # via sphinx
-sphinxcontrib-htmlhelp==2.0.0 \
-    --hash=sha256:d412243dfb797ae3ec2b59eca0e52dac12e75a241bf0e4eb861e450d06c6ed07 \
-    --hash=sha256:f5f8bb2d0d629f398bf47d0d69c07bc13b65f75a81ad9e2f71a63d4b7a2f6db2
-    # via sphinx
-sphinxcontrib-jsmath==1.0.1 \
-    --hash=sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178 \
-    --hash=sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8
-    # via sphinx
-sphinxcontrib-qthelp==1.0.3 \
-    --hash=sha256:4c33767ee058b70dba89a6fc5c1892c0d57a54be67ddd3e7875a18d14cba5a72 \
-    --hash=sha256:bd9fc24bcb748a8d51fd4ecaade681350aa63009a347a8c14e637895444dfab6
-    # via sphinx
-sphinxcontrib-serializinghtml==1.1.5 \
-    --hash=sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd \
-    --hash=sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952
-    # via sphinx
-urllib3==1.26.13 \
-    --hash=sha256:47cc05d99aaa09c9e72ed5809b60e7ba354e64b59c9c173ac3018642d8bb41fc \
-    --hash=sha256:c083dd0dce68dbfbe1129d5271cb90f9447dea7d52097c6e0126120c521ddea8
-    # via requests
+    # via pydocstyle
+tomli==2.0.1 \
+    --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
+    --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
+    # via
+    #   coverage
+    #   pytest
+typing-extensions==4.5.0 \
+    --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
+    --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
+    # via importlib-metadata
+zipp==3.15.0 \
+    --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
+    --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
+    # via importlib-metadata
```

### Comparing `mozilla-version-1.2.0/setup.py` & `mozilla-version-2.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 project_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(project_dir, 'version.txt')) as f:
     version = f.read().rstrip()
 
 # We use the .in file because a library shouldn't pin versions, it breaks consumers' updates.
 # We allow commented lines in this file
-requirements_file_name = 'base_py3.in' if (sys.version_info > (3, 0)) else 'base_py2.in'
-with open(os.path.join(project_dir, 'requirements', requirements_file_name)) as f:
+with open(os.path.join(project_dir, 'requirements', 'base.in')) as f:
     requirements_raw = f.readlines()
 
 requirements_without_comments = [
     line for line in requirements_raw if line and not line.startswith('#')
 ]
 
 setup(
@@ -29,11 +28,10 @@
     url='https://github.com/mozilla-releng/mozilla-version',
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     license='MPL2',
     install_requires=requirements_without_comments,
     classifiers=[
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
     ],
 )
```

