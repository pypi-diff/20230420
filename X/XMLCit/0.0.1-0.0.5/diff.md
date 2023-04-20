# Comparing `tmp/xmlcit-0.0.4.tar.gz` & `tmp/xmlcit-0.0.5.tar.gz`

## Comparing `xmlcit-0.0.4.tar` & `xmlcit-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 xmlcit-0.0.1/src/__init__.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 xmlcit-0.0.1/src/addtagfunc.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 xmlcit-0.0.1/src/tagfunctions.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 xmlcit-0.0.1/src/VIAF_functions/VIAFreffun.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 xmlcit-0.0.1/src/VIAF_functions/__init__.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 xmlcit-0.0.1/src/opcit_functions/Ibidfunc.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 xmlcit-0.0.1/src/opcit_functions/__init__.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 xmlcit-0.0.1/LICENSE
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 xmlcit-0.0.1/README.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xmlcit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 xmlcit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 xmlcit-0.0.5/src/__init__.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 xmlcit-0.0.5/src/addtagfunc.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 xmlcit-0.0.5/src/tagfunctions.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 xmlcit-0.0.5/src/VIAF_functions/VIAFreffun.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 xmlcit-0.0.5/src/VIAF_functions/__init__.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 xmlcit-0.0.5/src/opcit_functions/Ibidfunc.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 xmlcit-0.0.5/src/opcit_functions/__init__.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 xmlcit-0.0.5/LICENSE
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 xmlcit-0.0.5/README.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xmlcit-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 xmlcit-0.0.5/PKG-INFO
```

### Comparing `xmlcit-0.0.1/src/addtagfunc.py` & `xmlcit-0.0.5/src/addtagfunc.py`

 * *Files identical despite different names*

### Comparing `xmlcit-0.0.1/src/tagfunctions.py` & `xmlcit-0.0.5/src/tagfunctions.py`

 * *Files identical despite different names*

### Comparing `xmlcit-0.0.1/src/VIAF_functions/VIAFreffun.py` & `xmlcit-0.0.5/src/VIAF_functions/VIAFreffun.py`

 * *Files identical despite different names*

### Comparing `xmlcit-0.0.1/src/opcit_functions/Ibidfunc.py` & `xmlcit-0.0.5/src/opcit_functions/Ibidfunc.py`

 * *Files identical despite different names*

### Comparing `xmlcit-0.0.1/LICENSE` & `xmlcit-0.0.5/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 Research Computing Center at Florida State University
+Copyright (c) 2023 Research Computing Center
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `xmlcit-0.0.1/pyproject.toml` & `xmlcit-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "XMLCit"
-version = "0.0.1"
+version = "0.0.5"
 authors = [
   { name="Jose Hernandez", email="jose.hndz.prz@gmail.com" },
 ]
 description = "This package was made to edit XML files ( particularly TEI-XML files). The main purpose is to facilitate the tagging and edit of repeated citations; and the inclusion of VIAF records "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `xmlcit-0.0.1/PKG-INFO` & `xmlcit-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XMLCit
-Version: 0.0.1
+Version: 0.0.5
 Summary: This package was made to edit XML files ( particularly TEI-XML files). The main purpose is to facilitate the tagging and edit of repeated citations; and the inclusion of VIAF records 
 Author-email: Jose Hernandez <jose.hndz.prz@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

