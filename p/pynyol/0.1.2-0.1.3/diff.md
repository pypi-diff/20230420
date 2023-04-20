# Comparing `tmp/pynyol-0.1.2.tar.gz` & `tmp/pynyol-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynyol-0.1.2.tar", last modified: Tue Mar 21 12:22:18 2023, max compression
+gzip compressed data, was "pynyol-0.1.3.tar", last modified: Thu Apr 20 14:41:17 2023, max compression
```

## Comparing `pynyol-0.1.2.tar` & `pynyol-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 zagador123  (1000) zagador123  (1000)        0 2023-03-21 12:22:18.899998 pynyol-0.1.2/
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)      110 2023-03-21 12:21:59.000000 pynyol-0.1.2/CHANGES.txt
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)        0 2023-03-15 19:53:12.000000 pynyol-0.1.2/LICENSE.txt
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)       42 2023-03-15 20:16:49.000000 pynyol-0.1.2/MANIFEST.in
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)     1266 2023-03-21 12:22:18.899998 pynyol-0.1.2/PKG-INFO
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)      993 2023-03-15 22:23:01.000000 pynyol-0.1.2/README.txt
-drwxr-xr-x   0 zagador123  (1000) zagador123  (1000)        0 2023-03-21 12:22:18.889998 pynyol-0.1.2/bin/
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)      309 2023-03-15 20:12:34.000000 pynyol-0.1.2/bin/express_a_num.py
-drwxr-xr-x   0 zagador123  (1000) zagador123  (1000)        0 2023-03-21 12:22:18.889998 pynyol-0.1.2/docs/
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)       37 2023-03-15 20:16:28.000000 pynyol-0.1.2/docs/dictanum.txt
-drwxr-xr-x   0 zagador123  (1000) zagador123  (1000)        0 2023-03-21 12:22:18.889998 pynyol-0.1.2/pynyol/
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)        0 2023-03-15 19:54:58.000000 pynyol-0.1.2/pynyol/__init__.py
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)     5421 2023-03-21 12:20:25.000000 pynyol-0.1.2/pynyol/cleaner.py
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)     3832 2023-03-15 19:59:36.000000 pynyol-0.1.2/pynyol/dictanum.py
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)       72 2023-03-15 20:03:51.000000 pynyol-0.1.2/pynyol/numadict.py
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)      127 2023-03-15 20:05:04.000000 pynyol-0.1.2/pynyol/silabizer.py
-drwxr-xr-x   0 zagador123  (1000) zagador123  (1000)        0 2023-03-21 12:22:18.889998 pynyol-0.1.2/pynyol/test/
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)        0 2023-03-15 20:26:12.000000 pynyol-0.1.2/pynyol/test/__init__.py
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)      439 2023-03-21 12:16:49.000000 pynyol-0.1.2/pynyol/test/test_cleaner.py
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)      508 2023-03-15 20:26:24.000000 pynyol-0.1.2/pynyol/test/test_dictanum.py
-drwxr-xr-x   0 zagador123  (1000) zagador123  (1000)        0 2023-03-21 12:22:18.889998 pynyol-0.1.2/pynyol.egg-info/
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)     1266 2023-03-21 12:22:18.000000 pynyol-0.1.2/pynyol.egg-info/PKG-INFO
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)      414 2023-03-21 12:22:18.000000 pynyol-0.1.2/pynyol.egg-info/SOURCES.txt
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)        1 2023-03-21 12:22:18.000000 pynyol-0.1.2/pynyol.egg-info/dependency_links.txt
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)        7 2023-03-21 12:22:18.000000 pynyol-0.1.2/pynyol.egg-info/top_level.txt
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)       38 2023-03-21 12:22:18.899998 pynyol-0.1.2/setup.cfg
--rw-r--r--   0 zagador123  (1000) zagador123  (1000)      486 2023-03-21 12:21:15.000000 pynyol-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:41:17.157827 pynyol-0.1.3/
+-rw-rw-rw-   0        0        0      110 2023-03-21 12:21:59.000000 pynyol-0.1.3/CHANGES.txt
+-rw-rw-rw-   0        0        0        0 2023-03-15 19:53:12.000000 pynyol-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       42 2023-03-15 20:16:49.000000 pynyol-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1314 2023-04-20 14:41:17.156828 pynyol-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      993 2023-03-15 22:23:01.000000 pynyol-0.1.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 14:41:17.145679 pynyol-0.1.3/bin/
+-rw-rw-rw-   0        0        0      309 2023-03-15 20:12:34.000000 pynyol-0.1.3/bin/express_a_num.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:41:17.146843 pynyol-0.1.3/docs/
+-rw-rw-rw-   0        0        0       37 2023-03-15 20:16:28.000000 pynyol-0.1.3/docs/dictanum.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 14:41:17.140166 pynyol-0.1.3/pynyol/
+-rw-rw-rw-   0        0        0        0 2023-03-15 19:54:58.000000 pynyol-0.1.3/pynyol/__init__.py
+-rw-rw-rw-   0        0        0     5778 2023-03-21 13:53:26.000000 pynyol-0.1.3/pynyol/cleaner.py
+-rw-rw-rw-   0        0        0     3832 2023-03-15 19:59:36.000000 pynyol-0.1.3/pynyol/dictanum.py
+-rw-rw-rw-   0        0        0       72 2023-03-15 20:03:51.000000 pynyol-0.1.3/pynyol/numadict.py
+-rw-rw-rw-   0        0        0      127 2023-03-15 20:05:04.000000 pynyol-0.1.3/pynyol/silabizer.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:41:17.144679 pynyol-0.1.3/pynyol/test/
+-rw-rw-rw-   0        0        0        0 2023-03-15 20:26:12.000000 pynyol-0.1.3/pynyol/test/__init__.py
+-rw-rw-rw-   0        0        0      439 2023-03-21 13:53:33.000000 pynyol-0.1.3/pynyol/test/test_cleaner.py
+-rw-rw-rw-   0        0        0      508 2023-03-15 20:26:24.000000 pynyol-0.1.3/pynyol/test/test_dictanum.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:41:17.153830 pynyol-0.1.3/pynyol.egg-info/
+-rw-rw-rw-   0        0        0     1314 2023-04-20 14:41:17.000000 pynyol-0.1.3/pynyol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2023-04-20 14:41:17.000000 pynyol-0.1.3/pynyol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 14:41:17.000000 pynyol-0.1.3/pynyol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 14:41:17.000000 pynyol-0.1.3/pynyol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 14:41:17.157827 pynyol-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      485 2023-04-20 14:40:19.000000 pynyol-0.1.3/setup.py
```

### Comparing `pynyol-0.1.2/PKG-INFO` & `pynyol-0.1.3/README.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: pynyol
-Version: 0.1.2
-Summary: Package aimed at helping with processing the spanish language.
-Home-page: https://pypi.org/project/pynyol
-Author: Juanma López
-Author-email: lopezjuanma96@gmail.com
-License: LICENSE.txt
-License-File: LICENSE.txt
-
 ===========
 pynyol
 ===========
 
 pynyol is the Python implementation of the Nyol package. This package is aimed at helping with processing the spanish language.
 
 Each module inside the package provides help in a different area of language processing. These modules are:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pynyol-0.1.2/pynyol/cleaner.py` & `pynyol-0.1.3/pynyol/cleaner.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,15 +24,22 @@
 ]
     
 _SYMBOLS = [
     (r";|:", ","),
     (r"'|´|`", "\""),
     (r"(\w)-(\w)", "\\1 \\2"), #numeric reference on replace needs backslash scaping or else it treats as a unicode
     (r"-", "—"),
-    (r"ł", "l")
+    #this can not be "detected" as accents and replaced with normalization, maybe find another way, else keep them in symbols but add this to docs
+    (r"ł", "l"), #l with stroke
+    (r"ø", "o"), #o with stroke
+    (r"ã", "a"), #a with tilde
+    (r"ã", "a"), #a and tilde
+    (r"õ", "o"), #o with tilde
+    (r"õ", "o")  #o and tilde
+    (r"ñ", "ñ")  #n and tilde
 ]
 
 _KEEP_THIS_ACCENTS = "áéíóú"
 
 _WHITESPACE_RE = re.compile('\s+')
 _DOTTED_NUMBER_RE = re.compile(r'([0-9][0-9\.]+[0-9])')
 _DECIMAL_NUMBER_RE = re.compile(r'([0-9]+\,[0-9]+)')
```

### Comparing `pynyol-0.1.2/pynyol/dictanum.py` & `pynyol-0.1.3/pynyol/dictanum.py`

 * *Files identical despite different names*

### Comparing `pynyol-0.1.2/pynyol.egg-info/PKG-INFO` & `pynyol-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-Metadata-Version: 2.1
-Name: pynyol
-Version: 0.1.2
-Summary: Package aimed at helping with processing the spanish language.
-Home-page: https://pypi.org/project/pynyol
-Author: Juanma López
-Author-email: lopezjuanma96@gmail.com
-License: LICENSE.txt
-License-File: LICENSE.txt
-
-===========
-pynyol
-===========
-
-pynyol is the Python implementation of the Nyol package. This package is aimed at helping with processing the spanish language.
-
-Each module inside the package provides help in a different area of language processing. These modules are:
-
-    #!/usr/bin/env python
-
-    from towelstuff import location
-    from towelstuff import utils
-
-    if utils.has_towel():
-        print "Your towel is located:", location.where_is_my_towel()
-
-(Note the double-colon and 4-space indent formatting above.)
-
-Paragraphs are separated by blank lines. *Italics*, **bold**,
-and ``monospace`` look like this.
-
-
-Dictanum
-=========
-
-Useful for getting the spelling of numbers.
-The spelling is handled by different *parser* whith different number ranges.
-This is one example for it:
-
-    #!/usr/bin/env python
-
-    from pynyol.dictanum import IntParser
-    
-    mynum = #insert a number here
-
-    ip = IntParser(mynum)
-
-    print(f'the spelling for {mynum} in spanish is: {ip.text}')
+Metadata-Version: 2.1
+Name: pynyol
+Version: 0.1.3
+Summary: Package aimed at helping with processing the spanish language.
+Home-page: https://pypi.org/project/pynyol
+Author: Juanma López
+Author-email: lopezjuanma96@gmail.com
+License: LICENSE.txt
+License-File: LICENSE.txt
+
+===========
+pynyol
+===========
+
+pynyol is the Python implementation of the Nyol package. This package is aimed at helping with processing the spanish language.
+
+Each module inside the package provides help in a different area of language processing. These modules are:
+
+    #!/usr/bin/env python
+
+    from towelstuff import location
+    from towelstuff import utils
+
+    if utils.has_towel():
+        print "Your towel is located:", location.where_is_my_towel()
+
+(Note the double-colon and 4-space indent formatting above.)
+
+Paragraphs are separated by blank lines. *Italics*, **bold**,
+and ``monospace`` look like this.
+
+
+Dictanum
+=========
+
+Useful for getting the spelling of numbers.
+The spelling is handled by different *parser* whith different number ranges.
+This is one example for it:
+
+    #!/usr/bin/env python
+
+    from pynyol.dictanum import IntParser
+    
+    mynum = #insert a number here
+
+    ip = IntParser(mynum)
+
+    print(f'the spelling for {mynum} in spanish is: {ip.text}')
```

