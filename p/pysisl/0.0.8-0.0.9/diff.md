# Comparing `tmp/pysisl-0.0.8.tar.gz` & `tmp/pysisl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysisl-0.0.8.tar", last modified: Thu Jul 22 13:42:57 2021, max compression
+gzip compressed data, was "pysisl-0.0.9.tar", last modified: Thu Jul 29 10:23:09 2021, max compression
```

## Comparing `pysisl-0.0.8.tar` & `pysisl-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:42:57.338841 pysisl-0.0.8/
--rw-rw-r--   0 root         (0) root         (0)     1074 2021-07-22 13:42:47.000000 pysisl-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11511 2021-07-22 13:42:57.338841 pysisl-0.0.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    10879 2021-07-22 13:42:47.000000 pysisl-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:42:57.333841 pysisl-0.0.8/pysisl/
--rw-rw-r--   0 root         (0) root         (0)      638 2021-07-22 13:42:47.000000 pysisl-0.0.8/pysisl/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1337 2021-07-22 13:42:47.000000 pysisl-0.0.8/pysisl/deep_merger.py
--rw-rw-r--   0 root         (0) root         (0)     2425 2021-07-22 13:42:47.000000 pysisl-0.0.8/pysisl/explode_structure.py
--rw-rw-r--   0 root         (0) root         (0)       74 2021-07-22 13:42:47.000000 pysisl-0.0.8/pysisl/parser_error.py
--rw-r--r--   0 root         (0) root         (0)     2579 2021-07-22 13:42:48.000000 pysisl-0.0.8/pysisl/parsetab.py
--rw-rw-r--   0 root         (0) root         (0)     2884 2021-07-22 13:42:47.000000 pysisl-0.0.8/pysisl/remove_data.py
--rw-rw-r--   0 root         (0) root         (0)     1230 2021-07-22 13:42:47.000000 pysisl-0.0.8/pysisl/sisl_decoder.py
--rw-rw-r--   0 root         (0) root         (0)     2424 2021-07-22 13:42:47.000000 pysisl-0.0.8/pysisl/sisl_encoder.py
--rw-rw-r--   0 root         (0) root         (0)      221 2021-07-22 13:42:47.000000 pysisl-0.0.8/pysisl/sisl_joiner.py
--rw-rw-r--   0 root         (0) root         (0)     2720 2021-07-22 13:42:47.000000 pysisl-0.0.8/pysisl/sisl_lexer.py
--rw-rw-r--   0 root         (0) root         (0)      938 2021-07-22 13:42:47.000000 pysisl-0.0.8/pysisl/sisl_parser.py
--rw-rw-r--   0 root         (0) root         (0)     2058 2021-07-22 13:42:47.000000 pysisl-0.0.8/pysisl/sisl_splitter.py
--rw-rw-r--   0 root         (0) root         (0)     2029 2021-07-22 13:42:47.000000 pysisl-0.0.8/pysisl/sisl_type_flatten.py
--rw-rw-r--   0 root         (0) root         (0)     2720 2021-07-22 13:42:47.000000 pysisl-0.0.8/pysisl/sisl_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:42:57.334841 pysisl-0.0.8/pysisl.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11511 2021-07-22 13:42:57.000000 pysisl-0.0.8/pysisl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      904 2021-07-22 13:42:57.000000 pysisl-0.0.8/pysisl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-22 13:42:57.000000 pysisl-0.0.8/pysisl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2021-07-22 13:42:57.000000 pysisl-0.0.8/pysisl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2021-07-22 13:42:57.000000 pysisl-0.0.8/pysisl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-22 13:42:57.338841 pysisl-0.0.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1475 2021-07-22 13:42:47.000000 pysisl-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:42:57.337841 pysisl-0.0.8/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-07-22 13:42:47.000000 pysisl-0.0.8/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9872 2021-07-22 13:42:47.000000 pysisl-0.0.8/tests/test_deep_merger.py
--rw-rw-r--   0 root         (0) root         (0)    18744 2021-07-22 13:42:47.000000 pysisl-0.0.8/tests/test_explode_structure.py
--rw-rw-r--   0 root         (0) root         (0)    16311 2021-07-22 13:42:47.000000 pysisl-0.0.8/tests/test_remove_data.py
--rw-rw-r--   0 root         (0) root         (0)     8580 2021-07-22 13:42:47.000000 pysisl-0.0.8/tests/test_sisl_decoder.py
--rw-rw-r--   0 root         (0) root         (0)    13469 2021-07-22 13:42:47.000000 pysisl-0.0.8/tests/test_sisl_decoder_raw_types.py
--rw-rw-r--   0 root         (0) root         (0)     9278 2021-07-22 13:42:47.000000 pysisl-0.0.8/tests/test_sisl_encoder.py
--rw-rw-r--   0 root         (0) root         (0)     4994 2021-07-22 13:42:47.000000 pysisl-0.0.8/tests/test_sisl_encoder_decoder.py
--rw-rw-r--   0 root         (0) root         (0)     7479 2021-07-22 13:42:47.000000 pysisl-0.0.8/tests/test_sisl_joiner.py
--rw-rw-r--   0 root         (0) root         (0)    10163 2021-07-22 13:42:47.000000 pysisl-0.0.8/tests/test_sisl_splitter.py
--rw-rw-r--   0 root         (0) root         (0)     6004 2021-07-22 13:42:47.000000 pysisl-0.0.8/tests/test_sisl_type_flatten.py
--rw-rw-r--   0 root         (0) root         (0)     2251 2021-07-22 13:42:47.000000 pysisl-0.0.8/tests/test_sisl_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:42:57.337841 pysisl-0.0.8/tests_random_abnf/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-07-22 13:42:47.000000 pysisl-0.0.8/tests_random_abnf/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1164 2021-07-22 13:42:47.000000 pysisl-0.0.8/tests_random_abnf/random_abnf_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-29 10:23:09.565571 pysisl-0.0.9/
+-rw-rw-r--   0 root         (0) root         (0)     1074 2021-07-29 10:22:59.000000 pysisl-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11594 2021-07-29 10:23:09.565571 pysisl-0.0.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    10962 2021-07-29 10:22:59.000000 pysisl-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-29 10:23:09.561571 pysisl-0.0.9/pysisl/
+-rw-rw-r--   0 root         (0) root         (0)      638 2021-07-29 10:22:59.000000 pysisl-0.0.9/pysisl/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1337 2021-07-29 10:22:59.000000 pysisl-0.0.9/pysisl/deep_merger.py
+-rw-rw-r--   0 root         (0) root         (0)     2425 2021-07-29 10:22:59.000000 pysisl-0.0.9/pysisl/explode_structure.py
+-rw-rw-r--   0 root         (0) root         (0)       74 2021-07-29 10:22:59.000000 pysisl-0.0.9/pysisl/parser_error.py
+-rw-r--r--   0 root         (0) root         (0)     2579 2021-07-29 10:23:00.000000 pysisl-0.0.9/pysisl/parsetab.py
+-rw-rw-r--   0 root         (0) root         (0)     2884 2021-07-29 10:22:59.000000 pysisl-0.0.9/pysisl/remove_data.py
+-rw-rw-r--   0 root         (0) root         (0)     1230 2021-07-29 10:22:59.000000 pysisl-0.0.9/pysisl/sisl_decoder.py
+-rw-rw-r--   0 root         (0) root         (0)     2424 2021-07-29 10:22:59.000000 pysisl-0.0.9/pysisl/sisl_encoder.py
+-rw-rw-r--   0 root         (0) root         (0)      221 2021-07-29 10:22:59.000000 pysisl-0.0.9/pysisl/sisl_joiner.py
+-rw-rw-r--   0 root         (0) root         (0)     2720 2021-07-29 10:22:59.000000 pysisl-0.0.9/pysisl/sisl_lexer.py
+-rw-rw-r--   0 root         (0) root         (0)      938 2021-07-29 10:22:59.000000 pysisl-0.0.9/pysisl/sisl_parser.py
+-rw-rw-r--   0 root         (0) root         (0)     2058 2021-07-29 10:22:59.000000 pysisl-0.0.9/pysisl/sisl_splitter.py
+-rw-rw-r--   0 root         (0) root         (0)     2029 2021-07-29 10:22:59.000000 pysisl-0.0.9/pysisl/sisl_type_flatten.py
+-rw-rw-r--   0 root         (0) root         (0)     3370 2021-07-29 10:22:59.000000 pysisl-0.0.9/pysisl/sisl_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-29 10:23:09.562572 pysisl-0.0.9/pysisl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11594 2021-07-29 10:23:09.000000 pysisl-0.0.9/pysisl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      904 2021-07-29 10:23:09.000000 pysisl-0.0.9/pysisl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-07-29 10:23:09.000000 pysisl-0.0.9/pysisl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2021-07-29 10:23:09.000000 pysisl-0.0.9/pysisl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2021-07-29 10:23:09.000000 pysisl-0.0.9/pysisl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-07-29 10:23:09.565571 pysisl-0.0.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1475 2021-07-29 10:22:59.000000 pysisl-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-29 10:23:09.564571 pysisl-0.0.9/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-07-29 10:22:59.000000 pysisl-0.0.9/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9872 2021-07-29 10:22:59.000000 pysisl-0.0.9/tests/test_deep_merger.py
+-rw-rw-r--   0 root         (0) root         (0)    18744 2021-07-29 10:22:59.000000 pysisl-0.0.9/tests/test_explode_structure.py
+-rw-rw-r--   0 root         (0) root         (0)    16311 2021-07-29 10:22:59.000000 pysisl-0.0.9/tests/test_remove_data.py
+-rw-rw-r--   0 root         (0) root         (0)     8580 2021-07-29 10:22:59.000000 pysisl-0.0.9/tests/test_sisl_decoder.py
+-rw-rw-r--   0 root         (0) root         (0)    13469 2021-07-29 10:22:59.000000 pysisl-0.0.9/tests/test_sisl_decoder_raw_types.py
+-rw-rw-r--   0 root         (0) root         (0)     9278 2021-07-29 10:22:59.000000 pysisl-0.0.9/tests/test_sisl_encoder.py
+-rw-rw-r--   0 root         (0) root         (0)     4994 2021-07-29 10:22:59.000000 pysisl-0.0.9/tests/test_sisl_encoder_decoder.py
+-rw-rw-r--   0 root         (0) root         (0)     7479 2021-07-29 10:22:59.000000 pysisl-0.0.9/tests/test_sisl_joiner.py
+-rw-rw-r--   0 root         (0) root         (0)    10163 2021-07-29 10:22:59.000000 pysisl-0.0.9/tests/test_sisl_splitter.py
+-rw-rw-r--   0 root         (0) root         (0)     6004 2021-07-29 10:22:59.000000 pysisl-0.0.9/tests/test_sisl_type_flatten.py
+-rw-rw-r--   0 root         (0) root         (0)     3416 2021-07-29 10:22:59.000000 pysisl-0.0.9/tests/test_sisl_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-29 10:23:09.565571 pysisl-0.0.9/tests_random_abnf/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-07-29 10:22:59.000000 pysisl-0.0.9/tests_random_abnf/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1164 2021-07-29 10:22:59.000000 pysisl-0.0.9/tests_random_abnf/random_abnf_tests.py
```

### Comparing `pysisl-0.0.8/LICENSE` & `pysisl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/PKG-INFO` & `pysisl-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysisl
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python library for serialising and deserialising SISL (Simple Information Serialization Language)
 Home-page: https://github.com/oakdoor
 Author: Oakdoor
 Author-email: oakdoor.support@paconsulting.com
 License: UNKNOWN
 Project-URL: Project, https://www.paconsulting.com/services/product-design-and-engineering/data-diode/
 Platform: UNKNOWN
@@ -42,18 +42,18 @@
     pysisl.dumps(obj)  
   Serialise a basic Python object into a SISL formatted str. 
 
     pysisl.loads(sisl, schema=None)  
   Deserialise SISL str to a basic Python object. Optionally, verify the SISL schema using a json schema.
 
     pysisl.wraps(data)
-  Applies an XOR data scrambling technique to wrap and render data inert, equivalent to the Oakdoor<sup>TM</sup> data diode hardware. The XOR key is internally generated and prepended as part of a header.
+  Applies an XOR data scrambling technique to wrap and render data inert, equivalent to the Oakdoor<sup>TM</sup> data diode hardware. The data must be bytes() or bytearray(). The XOR key is internally generated and prepended as part of a header. 
 
     pysisl.unwraps(data)
-  Unwraps data scrambled with the above XOR data scrambling technique.
+  Unwraps data scrambled with the above XOR data scrambling technique. The data must be bytes() or bytearray().
   
 
 See the [conversion](#conversion-table) table on this page for more details.
 
 ### Splitting large objects into multiple SISL files
 pySISL supports a maximum length in bytes for SISL files. If the input Python object exceeds this max length it is split into multiple SISL files. A Python list is returned where each item is a SISL string.
```

### Comparing `pysisl-0.0.8/README.md` & `pysisl-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     pysisl.dumps(obj)  
   Serialise a basic Python object into a SISL formatted str. 
 
     pysisl.loads(sisl, schema=None)  
   Deserialise SISL str to a basic Python object. Optionally, verify the SISL schema using a json schema.
 
     pysisl.wraps(data)
-  Applies an XOR data scrambling technique to wrap and render data inert, equivalent to the Oakdoor<sup>TM</sup> data diode hardware. The XOR key is internally generated and prepended as part of a header.
+  Applies an XOR data scrambling technique to wrap and render data inert, equivalent to the Oakdoor<sup>TM</sup> data diode hardware. The data must be bytes() or bytearray(). The XOR key is internally generated and prepended as part of a header. 
 
     pysisl.unwraps(data)
-  Unwraps data scrambled with the above XOR data scrambling technique.
+  Unwraps data scrambled with the above XOR data scrambling technique. The data must be bytes() or bytearray().
   
 
 See the [conversion](#conversion-table) table on this page for more details.
 
 ### Splitting large objects into multiple SISL files
 pySISL supports a maximum length in bytes for SISL files. If the input Python object exceeds this max length it is split into multiple SISL files. A Python list is returned where each item is a SISL string.
```

### Comparing `pysisl-0.0.8/pysisl/__init__.py` & `pysisl-0.0.9/pysisl/__init__.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/pysisl/deep_merger.py` & `pysisl-0.0.9/pysisl/deep_merger.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/pysisl/explode_structure.py` & `pysisl-0.0.9/pysisl/explode_structure.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/pysisl/parsetab.py` & `pysisl-0.0.9/pysisl/parsetab.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/pysisl/remove_data.py` & `pysisl-0.0.9/pysisl/remove_data.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/pysisl/sisl_decoder.py` & `pysisl-0.0.9/pysisl/sisl_decoder.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/pysisl/sisl_encoder.py` & `pysisl-0.0.9/pysisl/sisl_encoder.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/pysisl/sisl_lexer.py` & `pysisl-0.0.9/pysisl/sisl_lexer.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/pysisl/sisl_parser.py` & `pysisl-0.0.9/pysisl/sisl_parser.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/pysisl/sisl_splitter.py` & `pysisl-0.0.9/pysisl/sisl_splitter.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/pysisl/sisl_type_flatten.py` & `pysisl-0.0.9/pysisl/sisl_type_flatten.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/pysisl/sisl_wrapper.py` & `pysisl-0.0.9/pysisl/sisl_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # Copyright PA Knowledge Ltd 2021
 import construct
 from itertools import cycle
 import secrets
-from pysisl import parser_error
-import pysisl
 from binascii import unhexlify
 
 
 class SislWrapper:
     def __init__(self, key_generator=None):
         self.majorVersion = 1
         self.minorVersion = 0
@@ -15,26 +13,38 @@
         self.encapsulationType = 1
         self.encapsulationConfig = 3
         self.encapsulationDataLen = 8
         self.key = SislWrapper.key_generation() if key_generator is None else key_generator
         self.padding = 0
         self.cloaked_dagger = self._build_cloaked_dagger_header()
 
-    def wraps(self, data):
-        return self.cloaked_dagger + SislWrapper._xor_data(self.key, bytes(data, 'utf-8'))
+    def wraps(self, data: str):
+        return self.cloaked_dagger + SislWrapper._xor_data(self.key, SislWrapper._is_bytes(data))
 
     @staticmethod
     def _xor_data(key, data):
         return bytes([a ^ b for (a, b) in zip(data, cycle(key))])
 
     @staticmethod
+    def _is_bytes(data):
+        if isinstance(data, (bytes, bytearray)):
+            return data
+        else:
+            raise TypeError("Input must be bytes")
+
+    @staticmethod
     def unwraps(data):
-        key = SislWrapper._extract_key_from_cloaked_dagger_header(data)
+        CloakDagger.check_valid_cloaked_dagger_header(SislWrapper._is_bytes(data))
+        key = CloakDagger.get_cloak_dagger_field_by_name(data, 'Encap_Mask')
         return SislWrapper._xor_data(key, SislWrapper._extract_payload_from_data(data))
 
+    @staticmethod
+    def _extract_payload_from_data(data):
+        return data[CloakDagger.get_cloak_dagger_field_by_name(data, 'Length'):]
+
     def _build_cloaked_dagger_header(self):
         return CloakDagger.cloak_dagger_bytes().build(
             dict(Major_Version=self.majorVersion,
                  Minor_Version=self.minorVersion,
                  Length=self.headerLen,
                  Encap_Type=self.encapsulationType,
                  Encap_Config=self.encapsulationConfig,
@@ -45,22 +55,14 @@
     @staticmethod
     def key_generation():
         key = unhexlify(secrets.token_hex(8))
         if b'\x00' in key:
             key = SislWrapper.key_generation()
         return key
 
-    @staticmethod
-    def _extract_key_from_cloaked_dagger_header(data):
-        return data[20:28]
-
-    @staticmethod
-    def _extract_payload_from_data(data):
-        return data[48:]
-
 
 class CloakDagger:
     @staticmethod
     def cloak_dagger_bytes():
         return construct.Struct("Magic_Number_1" / construct.Const(b'\xd1\xdf\x5f\xff'),
                                 "Major_Version" / construct.Int16ub,
                                 "Minor_Version" / construct.Int16ub,
@@ -68,7 +70,22 @@
                                 "Encap_Type" / construct.Int32ub,
                                 "Encap_Config" / construct.Int16ub,
                                 "Encap_Dlen" / construct.Int16ub,
                                 "Encap_Mask" / construct.Bytes(8),
                                 "RESERVED" / construct.Padding(16),
                                 "Magic_Number_2" / construct.Const(b'\xff\x5f\xdf\xd1')
                                 )
+
+    @staticmethod
+    def check_valid_cloaked_dagger_header(data):
+        try:
+            CloakDagger.cloak_dagger_bytes().parse(data)
+        except construct.core.ConstructError as e:
+            raise InvalidHeaderError(f"Header could not be validated: {e}")
+
+    @staticmethod
+    def get_cloak_dagger_field_by_name(data, field):
+        return CloakDagger.cloak_dagger_bytes().parse(data).search(field)
+
+
+class InvalidHeaderError(Exception):
+    pass
```

### Comparing `pysisl-0.0.8/pysisl.egg-info/PKG-INFO` & `pysisl-0.0.9/pysisl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysisl
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python library for serialising and deserialising SISL (Simple Information Serialization Language)
 Home-page: https://github.com/oakdoor
 Author: Oakdoor
 Author-email: oakdoor.support@paconsulting.com
 License: UNKNOWN
 Project-URL: Project, https://www.paconsulting.com/services/product-design-and-engineering/data-diode/
 Platform: UNKNOWN
@@ -42,18 +42,18 @@
     pysisl.dumps(obj)  
   Serialise a basic Python object into a SISL formatted str. 
 
     pysisl.loads(sisl, schema=None)  
   Deserialise SISL str to a basic Python object. Optionally, verify the SISL schema using a json schema.
 
     pysisl.wraps(data)
-  Applies an XOR data scrambling technique to wrap and render data inert, equivalent to the Oakdoor<sup>TM</sup> data diode hardware. The XOR key is internally generated and prepended as part of a header.
+  Applies an XOR data scrambling technique to wrap and render data inert, equivalent to the Oakdoor<sup>TM</sup> data diode hardware. The data must be bytes() or bytearray(). The XOR key is internally generated and prepended as part of a header. 
 
     pysisl.unwraps(data)
-  Unwraps data scrambled with the above XOR data scrambling technique.
+  Unwraps data scrambled with the above XOR data scrambling technique. The data must be bytes() or bytearray().
   
 
 See the [conversion](#conversion-table) table on this page for more details.
 
 ### Splitting large objects into multiple SISL files
 pySISL supports a maximum length in bytes for SISL files. If the input Python object exceeds this max length it is split into multiple SISL files. A Python list is returned where each item is a SISL string.
```

### Comparing `pysisl-0.0.8/pysisl.egg-info/SOURCES.txt` & `pysisl-0.0.9/pysisl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/setup.py` & `pysisl-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         install.run(self)
         import pysisl
         pysisl.loads("{}")
 
 
 setuptools.setup(
     name="pysisl",
-    version="0.0.8",
+    version="0.0.9",
     author="Oakdoor",
     author_email="oakdoor.support@paconsulting.com",
     description="A python library for serialising and deserialising SISL (Simple Information Serialization Language)",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/oakdoor",
     project_urls={
```

### Comparing `pysisl-0.0.8/tests/test_deep_merger.py` & `pysisl-0.0.9/tests/test_deep_merger.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/tests/test_explode_structure.py` & `pysisl-0.0.9/tests/test_explode_structure.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/tests/test_remove_data.py` & `pysisl-0.0.9/tests/test_remove_data.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/tests/test_sisl_decoder.py` & `pysisl-0.0.9/tests/test_sisl_decoder.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/tests/test_sisl_decoder_raw_types.py` & `pysisl-0.0.9/tests/test_sisl_decoder_raw_types.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/tests/test_sisl_encoder.py` & `pysisl-0.0.9/tests/test_sisl_encoder.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/tests/test_sisl_encoder_decoder.py` & `pysisl-0.0.9/tests/test_sisl_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/tests/test_sisl_joiner.py` & `pysisl-0.0.9/tests/test_sisl_joiner.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/tests/test_sisl_splitter.py` & `pysisl-0.0.9/tests/test_sisl_splitter.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/tests/test_sisl_type_flatten.py` & `pysisl-0.0.9/tests/test_sisl_type_flatten.py`

 * *Files identical despite different names*

### Comparing `pysisl-0.0.8/tests_random_abnf/random_abnf_tests.py` & `pysisl-0.0.9/tests_random_abnf/random_abnf_tests.py`

 * *Files identical despite different names*

