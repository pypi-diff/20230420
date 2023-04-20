# Comparing `tmp/pylovelace-2023.1.2-py3-none-any.whl.zip` & `tmp/pylovelace-2023.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17982 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      228 b- defN 23-Apr-19 05:09 pylovelace/__init__.py
+Zip file size: 18004 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      228 b- defN 23-Apr-20 01:17 pylovelace/__init__.py
 -rw-rw-rw-  2.0 fat     8086 b- defN 23-Apr-19 05:09 pylovelace/__main__.py
 -rw-rw-rw-  2.0 fat     4383 b- defN 23-Apr-19 05:09 pylovelace/protect.py
--rw-rw-rw-  2.0 fat    35149 b- defN 23-Apr-19 05:09 pylovelace-2023.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1596 b- defN 23-Apr-19 05:09 pylovelace-2023.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 05:09 pylovelace-2023.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       56 b- defN 23-Apr-19 05:09 pylovelace-2023.1.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-19 05:09 pylovelace-2023.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      753 b- defN 23-Apr-19 05:09 pylovelace-2023.1.2.dist-info/RECORD
-9 files, 50354 bytes uncompressed, 16676 bytes compressed:  66.9%
+-rw-rw-rw-  2.0 fat    35149 b- defN 23-Apr-20 01:20 pylovelace-2023.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1737 b- defN 23-Apr-20 01:20 pylovelace-2023.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 01:20 pylovelace-2023.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       56 b- defN 23-Apr-20 01:20 pylovelace-2023.1.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-20 01:20 pylovelace-2023.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      753 b- defN 23-Apr-20 01:20 pylovelace-2023.1.3.dist-info/RECORD
+9 files, 50495 bytes uncompressed, 16698 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: pylovelace/__main__.py
 Comment: 
 
 Filename: pylovelace/protect.py
 Comment: 
 
-Filename: pylovelace-2023.1.2.dist-info/LICENSE
+Filename: pylovelace-2023.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: pylovelace-2023.1.2.dist-info/METADATA
+Filename: pylovelace-2023.1.3.dist-info/METADATA
 Comment: 
 
-Filename: pylovelace-2023.1.2.dist-info/WHEEL
+Filename: pylovelace-2023.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pylovelace-2023.1.2.dist-info/entry_points.txt
+Filename: pylovelace-2023.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: pylovelace-2023.1.2.dist-info/top_level.txt
+Filename: pylovelace-2023.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pylovelace-2023.1.2.dist-info/RECORD
+Filename: pylovelace-2023.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylovelace/__init__.py

```diff
@@ -4,9 +4,9 @@
 Copyright (c) 2023 PyLovelace
 All rights reserved.
 
 @Author: nshout
 @File: __init__.py
 """
 
-__version__ = "2023.1.2"
+__version__ = "2023.1.3"
 __description__ = "Python code protection/obfuscation tool"
```

## Comparing `pylovelace-2023.1.2.dist-info/LICENSE` & `pylovelace-2023.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pylovelace-2023.1.2.dist-info/METADATA` & `pylovelace-2023.1.3.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: pylovelace
-Version: 2023.1.2
+Version: 2023.1.3
 Summary: Python code protection/obfuscation tool
 Home-page: https://github.com/pylovelace/pylovelace
 Author: nshout
 Keywords: obfuscate obfuscation distribute production tool
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Topic :: Security
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Requires-Python: >=3.10, <3.13
 License-File: LICENSE
-Requires-Dist: pylovelace.kernel
+Requires-Dist: pylovelace.kernel (>=0)
 
 PyLovelace Python protection tool.
 ===================================
 
 PyLovelace is a Python protection tool that can be used to protect
 Python source code from being reverse engineered.
 
@@ -39,9 +42,9 @@
 -------------------------
 PyLovelace supports Python 3.11 with 3.10 and 3.12 support coming soon.
 Windows only for now.
 
 More information
 ----------------
 - PyLovelace on PyPI: https://pypi.org/project/pylovelace/
-- PyLovelace on GitHub: https://github.com/pyintellect/pylovelace
+- PyLovelace on GitHub: https://github.com/pylovelace/pylovelace
 - PyLovelace documentation: https://pylovelace.com/docs/
```

## Comparing `pylovelace-2023.1.2.dist-info/RECORD` & `pylovelace-2023.1.3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pylovelace/__init__.py,sha256=ccyRZeCCDxgaIr2p9U276uAntqAFXM7rMuTGgf89WtA,228
+pylovelace/__init__.py,sha256=nPTLXUylcDtJHivPe5Vn5OSO0IyXAnPwweRJhcsWT3E,228
 pylovelace/__main__.py,sha256=R-eforVO5Zt0n1GyadLvkdS2yauOdOYnXtC1fowUgwU,8086
 pylovelace/protect.py,sha256=66aY-0v6W0Y0cQj1YLiJpkQm0ZNEUNcGjibrTkgCAto,4383
-pylovelace-2023.1.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-pylovelace-2023.1.2.dist-info/METADATA,sha256=xVPN3u18CZq_fTmDQPiav53koJThLDBTvbrJM_V6ypE,1596
-pylovelace-2023.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pylovelace-2023.1.2.dist-info/entry_points.txt,sha256=-vPFZeB5Oi5SzSri14fSMwAF-co3sgO2M6Fr7ScfPeo,56
-pylovelace-2023.1.2.dist-info/top_level.txt,sha256=J7DsoNzAcCKQQcB_uVPOh9mNcQSDemGF9xpSWgkWUDs,11
-pylovelace-2023.1.2.dist-info/RECORD,,
+pylovelace-2023.1.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+pylovelace-2023.1.3.dist-info/METADATA,sha256=hRdim0bpn-acePWgzmSTEZrgPLOP2_83qp_J80dUF1c,1737
+pylovelace-2023.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pylovelace-2023.1.3.dist-info/entry_points.txt,sha256=-vPFZeB5Oi5SzSri14fSMwAF-co3sgO2M6Fr7ScfPeo,56
+pylovelace-2023.1.3.dist-info/top_level.txt,sha256=J7DsoNzAcCKQQcB_uVPOh9mNcQSDemGF9xpSWgkWUDs,11
+pylovelace-2023.1.3.dist-info/RECORD,,
```

