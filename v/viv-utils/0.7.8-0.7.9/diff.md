# Comparing `tmp/viv_utils-0.7.8.tar.gz` & `tmp/viv_utils-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viv_utils-0.7.8.tar", last modified: Thu Mar  2 12:10:40 2023, max compression
+gzip compressed data, was "viv_utils-0.7.9.tar", last modified: Thu Apr 20 07:59:29 2023, max compression
```

## Comparing `viv_utils-0.7.8.tar` & `viv_utils-0.7.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:10:40.715032 viv_utils-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-02 12:10:31.000000 viv_utils-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-02 12:10:40.715032 viv_utils-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-02 12:10:31.000000 viv_utils-0.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-02 12:10:40.715032 viv_utils-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-02 12:10:31.000000 viv_utils-0.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:10:40.715032 viv_utils-0.7.8/viv_utils/
--rw-r--r--   0 runner    (1001) docker     (123)    22822 2023-03-02 12:10:31.000000 viv_utils-0.7.8/viv_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-03-02 12:10:31.000000 viv_utils-0.7.8/viv_utils/emulator_drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13879 2023-03-02 12:10:31.000000 viv_utils-0.7.8/viv_utils/flirt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-03-02 12:10:31.000000 viv_utils-0.7.8/viv_utils/idaloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:10:40.715032 viv_utils-0.7.8/viv_utils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 12:10:31.000000 viv_utils-0.7.8/viv_utils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-03-02 12:10:31.000000 viv_utils-0.7.8/viv_utils/scripts/get_flirt_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-03-02 12:10:31.000000 viv_utils-0.7.8/viv_utils/scripts/get_function_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-03-02 12:10:31.000000 viv_utils-0.7.8/viv_utils/scripts/show_flirt_references.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-02 12:10:31.000000 viv_utils-0.7.8/viv_utils/scripts/trace_function_emulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-02 12:10:31.000000 viv_utils-0.7.8/viv_utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:10:40.715032 viv_utils-0.7.8/viv_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-02 12:10:40.000000 viv_utils-0.7.8/viv_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-02 12:10:40.000000 viv_utils-0.7.8/viv_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 12:10:40.000000 viv_utils-0.7.8/viv_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-02 12:10:40.000000 viv_utils-0.7.8/viv_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 12:10:40.000000 viv_utils-0.7.8/viv_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-02 12:10:40.000000 viv_utils-0.7.8/viv_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-02 12:10:40.000000 viv_utils-0.7.8/viv_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:59:29.448585 viv_utils-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 07:59:18.000000 viv_utils-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-20 07:59:29.448585 viv_utils-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 07:59:18.000000 viv_utils-0.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-20 07:59:29.448585 viv_utils-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-20 07:59:18.000000 viv_utils-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:59:29.448585 viv_utils-0.7.9/viv_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    22822 2023-04-20 07:59:18.000000 viv_utils-0.7.9/viv_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29160 2023-04-20 07:59:18.000000 viv_utils-0.7.9/viv_utils/emulator_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-04-20 07:59:18.000000 viv_utils-0.7.9/viv_utils/flirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-04-20 07:59:18.000000 viv_utils-0.7.9/viv_utils/idaloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:59:29.448585 viv_utils-0.7.9/viv_utils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:59:18.000000 viv_utils-0.7.9/viv_utils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-20 07:59:18.000000 viv_utils-0.7.9/viv_utils/scripts/get_flirt_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-20 07:59:18.000000 viv_utils-0.7.9/viv_utils/scripts/get_function_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-20 07:59:18.000000 viv_utils-0.7.9/viv_utils/scripts/show_flirt_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-20 07:59:18.000000 viv_utils-0.7.9/viv_utils/scripts/trace_function_emulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-20 07:59:18.000000 viv_utils-0.7.9/viv_utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:59:29.448585 viv_utils-0.7.9/viv_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-20 07:59:29.000000 viv_utils-0.7.9/viv_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-20 07:59:29.000000 viv_utils-0.7.9/viv_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:59:29.000000 viv_utils-0.7.9/viv_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-20 07:59:29.000000 viv_utils-0.7.9/viv_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:59:29.000000 viv_utils-0.7.9/viv_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-20 07:59:29.000000 viv_utils-0.7.9/viv_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 07:59:29.000000 viv_utils-0.7.9/viv_utils.egg-info/top_level.txt
```

### Comparing `viv_utils-0.7.8/LICENSE` & `viv_utils-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `viv_utils-0.7.8/PKG-INFO` & `viv_utils-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viv_utils
-Version: 0.7.8
+Version: 0.7.9
 Summary: Utilities for binary analysis using vivisect.
 Home-page: https://github.com/williballenthin/viv-utils
 Author: Willi Ballenthin
 Author-email: william.ballenthin@mandiant.com
 Keywords: viv_utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `viv_utils-0.7.8/setup.py` & `viv_utils-0.7.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import sys
 
 import setuptools
 
 requirements = [
-    "funcy==1.18",
+    "funcy>=2.0",
     "pefile>=2023.2.7",
-    "vivisect==1.1.0",
-    "intervaltree==3.1.0",
-    "typing_extensions==4.5.0",
+    "vivisect>=1.1.0",
+    "intervaltree>=3.1.0",
+    "typing_extensions>=4.5.0",
 ]
 
 setuptools.setup(
     name="viv_utils",
-    version="0.7.8",
+    version="0.7.9",
     description="Utilities for binary analysis using vivisect.",
     long_description="Utilities for binary analysis using vivisect.",
     author="Willi Ballenthin",
     author_email="william.ballenthin@mandiant.com",
     url="https://github.com/williballenthin/viv-utils",
     packages=setuptools.find_packages(),
     package_dir={"viv_utils": "viv_utils"},
@@ -32,22 +32,22 @@
     include_package_data=True,
     install_requires=requirements,
     extras_require={
         "flirt": [
             "python-flirt==0.8.6",
         ],
         "dev": [
-            "pytest==7.2.1",
+            "pytest==7.3.1",
             "pytest-sugar==0.9.6",
             "pytest-instafail==0.4.2",
             "pycodestyle==2.10.0",
-            "black==22.12.0",
+            "black==23.3.0",
             "isort==5.11.5",  # last version supporting Python 3.7
-            "mypy==1.0.1",
-            "types-setuptools==67.4.0.3",
+            "mypy==1.2.0",
+            "types-setuptools==67.6.0.7",
         ],
     },
     zip_safe=False,
     keywords="viv_utils",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `viv_utils-0.7.8/viv_utils/__init__.py` & `viv_utils-0.7.9/viv_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `viv_utils-0.7.8/viv_utils/emulator_drivers.py` & `viv_utils-0.7.9/viv_utils/emulator_drivers.py`

 * *Files 0% similar despite different names*

```diff
@@ -783,15 +783,14 @@
                     break
 
                 elif does_fallthrough:
                     # common case: middle of BB, keep stepping.
 
                     nextpc = emu.getProgramCounter()
                     if nextpc in seen:
-
                         if nextpc == lastpc:
                             # candidates:
                             #   - jump to self
                             #   - REP instruction
                             #   - ???
                             op = emu.parseOpcode(lastpc)
                             if op.prefixes & envi.archs.i386.disasm.PREFIX_REP:
```

### Comparing `viv_utils-0.7.8/viv_utils/flirt.py` & `viv_utils-0.7.9/viv_utils/flirt.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     args:
       match (flirt.FlirtSignature): the signature to get a name from.
 
     returns:
       str: the best name of the function matched by the given signature.
     """
-    for (name, type_, offset) in match.names:
+    for name, type_, offset in match.names:
         if offset == 0:
             return name
     raise ValueError("flirt: match: no best name: %s", match.names)
 
 
 def match_function_flirt_signatures(matcher, vw, va, cache=None):
     """
@@ -176,29 +176,28 @@
             # and check the name matches (or doesn't).
 
             # at the end of the following loop,
             # if this flag is still true,
             # then all the references have been validated.
             does_match_references = True
 
-            for (ref_name, _, ref_offset) in references:
+            for ref_name, _, ref_offset in references:
                 ref_va = va + ref_offset
 
                 # the reference offset may be inside an instruction,
                 # so we use getLocation to select the containing instruction address.
                 loc_va = vw.getLocation(ref_va)[vivisect.const.L_VA]
 
                 # an instruction may have multiple xrefs from
                 # so we loop through all code references,
                 # searching for that name.
                 #
                 # if the name is found, then this flag will be set.
                 does_match_the_reference = False
                 for xref in vw.getXrefsFrom(loc_va):
-
                     if ref_name == ".":
                         # special case: reference named `.`
                         # which right now we interpret to mean "any data reference".
                         # see: https://github.com/williballenthin/lancelot/issues/112#issuecomment-802379966
                         #
                         # unfortunately, viv doesn't extract the xref for this one sample,
                         # so this is untested.
@@ -257,15 +256,15 @@
     # there's one candidate name,
     # so all the matches *should* be about the same, i'd assume.
     match = matches[0]
 
     # first add local names, then we'll do public names
     # this way public names have precedence.
     # see: https://github.com/williballenthin/lancelot/issues/112#issuecomment-802221966
-    for (name, type_, offset) in match.names:
+    for name, type_, offset in match.names:
         if type_ != "local":
             continue
 
         if not vw.isFunction(va + offset):
             # since we're registered as a function analyzer,
             # we have to deal with a race condition:
             # the location for which we have a name may not yet be a function.
@@ -281,15 +280,15 @@
             add_function_flirt_match(vw, va + offset, name)
         except vivisect.exc.InvalidFunction:
             continue
         else:
             cache[va + offset] = name
             logger.debug("found local function name: 0x%x: %s", va + offset, name)
 
-    for (name, type_, offset) in match.names:
+    for name, type_, offset in match.names:
         if type_ != "public":
             continue
 
         try:
             add_function_flirt_match(vw, va + offset, name)
         except vivisect.exc.InvalidFunction:
             continue
```

### Comparing `viv_utils-0.7.8/viv_utils/idaloader.py` & `viv_utils-0.7.9/viv_utils/idaloader.py`

 * *Files identical despite different names*

### Comparing `viv_utils-0.7.8/viv_utils/scripts/get_flirt_matches.py` & `viv_utils-0.7.9/viv_utils/scripts/get_flirt_matches.py`

 * *Files identical despite different names*

### Comparing `viv_utils-0.7.8/viv_utils/scripts/get_function_args.py` & `viv_utils-0.7.9/viv_utils/scripts/get_function_args.py`

 * *Files identical despite different names*

### Comparing `viv_utils-0.7.8/viv_utils/scripts/show_flirt_references.py` & `viv_utils-0.7.9/viv_utils/scripts/show_flirt_references.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                 continue
 
             print("matching function: 0x%x" % (function))
             print("  candidate match: 0x%x: %s" % (function, match))
 
             print("  references:")
 
-            for (ref_name, _, ref_offset) in references:
+            for ref_name, _, ref_offset in references:
                 ref_va = function + ref_offset
                 seen.add(ref_va)
 
                 print("  - 0x%x: %s" % (ref_va, ref_name))
 
                 loc = vw.getLocation(ref_va)
                 loc_va = loc[vivisect.const.L_VA]
```

### Comparing `viv_utils-0.7.8/viv_utils/scripts/trace_function_emulation.py` & `viv_utils-0.7.9/viv_utils/scripts/trace_function_emulation.py`

 * *Files identical despite different names*

### Comparing `viv_utils-0.7.8/viv_utils/types.py` & `viv_utils-0.7.9/viv_utils/types.py`

 * *Files identical despite different names*

### Comparing `viv_utils-0.7.8/viv_utils.egg-info/PKG-INFO` & `viv_utils-0.7.9/viv_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viv-utils
-Version: 0.7.8
+Version: 0.7.9
 Summary: Utilities for binary analysis using vivisect.
 Home-page: https://github.com/williballenthin/viv-utils
 Author: Willi Ballenthin
 Author-email: william.ballenthin@mandiant.com
 Keywords: viv_utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `viv_utils-0.7.8/viv_utils.egg-info/SOURCES.txt` & `viv_utils-0.7.9/viv_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

