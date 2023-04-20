# Comparing `tmp/PyQt6_sip-13.5.0.tar.gz` & `tmp/PyQt6_sip-13.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6_sip-13.5.0.tar", last modified: Tue Apr  4 14:14:07 2023, max compression
+gzip compressed data, was "PyQt6_sip-13.5.1.tar", last modified: Thu Apr 13 15:05:22 2023, max compression
```

## Comparing `PyQt6_sip-13.5.0.tar` & `PyQt6_sip-13.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 14:14:07.134402 PyQt6_sip-13.5.0/
--rw-r--r--   0 phil       (501) staff       (20)     2766 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)    18161 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/LICENSE-GPL2
--rw-r--r--   0 phil       (501) staff       (20)    35297 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/LICENSE-GPL3
--rw-r--r--   0 phil       (501) staff       (20)       56 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)      505 2023-04-04 14:14:07.134490 PyQt6_sip-13.5.0/PKG-INFO
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 14:14:07.134192 PyQt6_sip-13.5.0/PyQt6_sip.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      505 2023-04-04 14:14:07.000000 PyQt6_sip-13.5.0/PyQt6_sip.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      389 2023-04-04 14:14:07.000000 PyQt6_sip-13.5.0/PyQt6_sip.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-04 14:14:07.000000 PyQt6_sip-13.5.0/PyQt6_sip.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)        6 2023-04-04 14:14:07.000000 PyQt6_sip-13.5.0/PyQt6_sip.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)      108 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/README
--rw-r--r--   0 phil       (501) staff       (20)       57 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)      296 2023-04-04 14:14:07.134861 PyQt6_sip-13.5.0/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)     1630 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/setup.py
--rw-r--r--   0 phil       (501) staff       (20)    49929 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/sip.h
--rw-r--r--   0 phil       (501) staff       (20)    21140 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/sip_array.c
--rw-r--r--   0 phil       (501) staff       (20)     1285 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/sip_array.h
--rw-r--r--   0 phil       (501) staff       (20)      859 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/sip_bool.cpp
--rw-r--r--   0 phil       (501) staff       (20)   312458 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/sip_core.c
--rw-r--r--   0 phil       (501) staff       (20)     5397 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/sip_core.h
--rw-r--r--   0 phil       (501) staff       (20)    13913 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/sip_descriptors.c
--rw-r--r--   0 phil       (501) staff       (20)    14690 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/sip_enum.c
--rw-r--r--   0 phil       (501) staff       (20)     1296 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/sip_enum.h
--rw-r--r--   0 phil       (501) staff       (20)     5650 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/sip_int_convertors.c
--rw-r--r--   0 phil       (501) staff       (20)    13795 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/sip_object_map.c
--rw-r--r--   0 phil       (501) staff       (20)     4788 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/sip_threads.c
--rw-r--r--   0 phil       (501) staff       (20)    19169 2023-04-04 14:14:06.000000 PyQt6_sip-13.5.0/sip_voidptr.c
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-13 15:05:22.851240 PyQt6_sip-13.5.1/
+-rw-r--r--   0 phil       (501) staff       (20)     2766 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)    18161 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/LICENSE-GPL2
+-rw-r--r--   0 phil       (501) staff       (20)    35297 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/LICENSE-GPL3
+-rw-r--r--   0 phil       (501) staff       (20)       56 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)      505 2023-04-13 15:05:22.851324 PyQt6_sip-13.5.1/PKG-INFO
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-13 15:05:22.851032 PyQt6_sip-13.5.1/PyQt6_sip.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      505 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/PyQt6_sip.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      389 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/PyQt6_sip.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/PyQt6_sip.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)        6 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/PyQt6_sip.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)      108 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/README
+-rw-r--r--   0 phil       (501) staff       (20)       57 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)      296 2023-04-13 15:05:22.851799 PyQt6_sip-13.5.1/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)     1630 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/setup.py
+-rw-r--r--   0 phil       (501) staff       (20)    49929 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip.h
+-rw-r--r--   0 phil       (501) staff       (20)    21140 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_array.c
+-rw-r--r--   0 phil       (501) staff       (20)     1285 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_array.h
+-rw-r--r--   0 phil       (501) staff       (20)      859 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_bool.cpp
+-rw-r--r--   0 phil       (501) staff       (20)   312458 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_core.c
+-rw-r--r--   0 phil       (501) staff       (20)     5397 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_core.h
+-rw-r--r--   0 phil       (501) staff       (20)    13975 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_descriptors.c
+-rw-r--r--   0 phil       (501) staff       (20)    14690 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_enum.c
+-rw-r--r--   0 phil       (501) staff       (20)     1296 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_enum.h
+-rw-r--r--   0 phil       (501) staff       (20)     5650 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_int_convertors.c
+-rw-r--r--   0 phil       (501) staff       (20)    13795 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_object_map.c
+-rw-r--r--   0 phil       (501) staff       (20)     4788 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_threads.c
+-rw-r--r--   0 phil       (501) staff       (20)    19169 2023-04-13 15:05:22.000000 PyQt6_sip-13.5.1/sip_voidptr.c
```

### Comparing `PyQt6_sip-13.5.0/LICENSE` & `PyQt6_sip-13.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.0/LICENSE-GPL2` & `PyQt6_sip-13.5.1/LICENSE-GPL2`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.0/LICENSE-GPL3` & `PyQt6_sip-13.5.1/LICENSE-GPL3`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.0/setup.py` & `PyQt6_sip-13.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,12 +34,12 @@
     module_src.append('sip_bool.cpp')
 
 module = Extension('PyQt6.sip', module_src)
 
 # Do the setup.
 setup(
         name='PyQt6_sip',
-        version='13.5.0',
+        version='13.5.1',
         license='SIP',
         python_requires='>=3.7',
         ext_modules=[module]
      )
```

### Comparing `PyQt6_sip-13.5.0/sip.h` & `PyQt6_sip-13.5.1/sip.h`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 extern "C" {
 #endif
 
 
 /* The version of the ABI. */
 #define SIP_ABI_MAJOR_VERSION       13
 #define SIP_ABI_MINOR_VERSION       5
-#define SIP_MODULE_PATCH_VERSION    0
+#define SIP_MODULE_PATCH_VERSION    1
 
 
 /*
  * The change history of the ABI.
  *
  * v13.5
  *  - Added the '#' conversion character to the argument parsers.
@@ -70,16 +70,16 @@
  *
  * v13.1
  *  - Added sipNextExceptionHandler().
  */
 
 
 /* The version of the code generator. */
-#define SIP_VERSION                 0x60708
-#define SIP_VERSION_STR             "6.7.8"
+#define SIP_VERSION                 0x60709
+#define SIP_VERSION_STR             "6.7.9"
 
 /* These are all dependent on the user-specified name of the sip module. */
 #define _SIP_MODULE_FQ_NAME         "PyQt6.sip"
 #define _SIP_MODULE_NAME            "sip"
 #define _SIP_MODULE_SHARED          1
 #define _SIP_MODULE_ENTRY           PyInit_sip
```

### Comparing `PyQt6_sip-13.5.0/sip_array.c` & `PyQt6_sip-13.5.1/sip_array.c`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.0/sip_array.h` & `PyQt6_sip-13.5.1/sip_array.h`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.0/sip_bool.cpp` & `PyQt6_sip-13.5.1/sip_bool.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.0/sip_core.c` & `PyQt6_sip-13.5.1/sip_core.c`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.0/sip_core.h` & `PyQt6_sip-13.5.1/sip_core.h`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.0/sip_descriptors.c` & `PyQt6_sip-13.5.1/sip_descriptors.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The implementation of the different descriptors.
  *
- * Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+ * Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
  *
  * This file is part of SIP.
  *
  * This copy of SIP is licensed for use under the terms of the SIP License
  * Agreement.  See the file LICENSE for more details.
  *
  * This copy of SIP may also used under the terms of the GNU General Public
@@ -226,14 +226,15 @@
 
 
 /*
  * The descriptor's dealloc slot.
  */
 static void sipMethodDescr_dealloc(PyObject *self)
 {
+    PyObject_GC_UnTrack(self);
     sipMethodDescr_clear(self);
     Py_TYPE(self)->tp_free(self);
 }
 
 
 /*****************************************************************************
  * A variable descriptor.  We don't use the similar Python descriptor because
@@ -487,10 +488,11 @@
 
 
 /*
  * The descriptor's dealloc slot.
  */
 static void sipVariableDescr_dealloc(PyObject *self)
 {
+    PyObject_GC_UnTrack(self);
     sipVariableDescr_clear(self);
     Py_TYPE(self)->tp_free(self);
 }
```

### Comparing `PyQt6_sip-13.5.0/sip_enum.c` & `PyQt6_sip-13.5.1/sip_enum.c`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.0/sip_enum.h` & `PyQt6_sip-13.5.1/sip_enum.h`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.0/sip_int_convertors.c` & `PyQt6_sip-13.5.1/sip_int_convertors.c`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.0/sip_object_map.c` & `PyQt6_sip-13.5.1/sip_object_map.c`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.0/sip_threads.c` & `PyQt6_sip-13.5.1/sip_threads.c`

 * *Files identical despite different names*

### Comparing `PyQt6_sip-13.5.0/sip_voidptr.c` & `PyQt6_sip-13.5.1/sip_voidptr.c`

 * *Files identical despite different names*

