# Comparing `tmp/ChineseNumberUtils-1.1.1.tar.gz` & `tmp/ChineseNumberUtils-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\lukai\Downloads\chinese-number-converter\dist\.tmp-l5oguddy\ChineseNumberUtils-1.1.1.tar", last modified: Tue Apr 18 12:24:02 2023, max compression
+gzip compressed data, was "C:\Users\lukai\Downloads\ChineseNumberUtils\dist\.tmp-ufwte8vs\ChineseNumberUtils-1.1.2.tar", last modified: Thu Apr 20 12:03:31 2023, max compression
```

## Comparing `ChineseNumberUtils-1.1.1.tar` & `ChineseNumberUtils-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/
--rw-rw-rw-   0        0        0     1075 2023-04-18 11:27:06.000000 ChineseNumberUtils-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     3957 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3118 2023-04-18 12:22:29.000000 ChineseNumberUtils-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/cnc/
-drwxrwxrwx   0        0        0        0 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/cnc/ChineseNumberUtils.egg-info/
--rw-rw-rw-   0        0        0     3957 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/cnc/ChineseNumberUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/cnc/ChineseNumberUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/cnc/ChineseNumberUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/cnc/ChineseNumberUtils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-18 11:27:06.000000 ChineseNumberUtils-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      883 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 12:03:31.000000 ChineseNumberUtils-1.1.2/
+-rw-rw-rw-   0        0        0     1075 2023-04-20 11:47:48.000000 ChineseNumberUtils-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3957 2023-04-20 12:03:31.000000 ChineseNumberUtils-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3118 2023-04-20 11:47:48.000000 ChineseNumberUtils-1.1.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-20 11:47:48.000000 ChineseNumberUtils-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      883 2023-04-20 12:03:31.000000 ChineseNumberUtils-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 12:03:31.000000 ChineseNumberUtils-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 12:03:31.000000 ChineseNumberUtils-1.1.2/src/ChineseNumberUtils.egg-info/
+-rw-rw-rw-   0        0        0     3957 2023-04-20 12:03:31.000000 ChineseNumberUtils-1.1.2/src/ChineseNumberUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-04-20 12:03:31.000000 ChineseNumberUtils-1.1.2/src/ChineseNumberUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 12:03:31.000000 ChineseNumberUtils-1.1.2/src/ChineseNumberUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-04-20 12:03:31.000000 ChineseNumberUtils-1.1.2/src/ChineseNumberUtils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 12:03:31.000000 ChineseNumberUtils-1.1.2/src/cnc/
+-rw-rw-rw-   0        0        0        0 2023-04-20 11:47:48.000000 ChineseNumberUtils-1.1.2/src/cnc/__init__.py
+-rw-rw-rw-   0        0        0     6953 2023-04-20 12:02:26.000000 ChineseNumberUtils-1.1.2/src/cnc/convert.py
```

### Comparing `ChineseNumberUtils-1.1.1/LICENSE` & `ChineseNumberUtils-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ChineseNumberUtils-1.1.1/PKG-INFO` & `ChineseNumberUtils-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChineseNumberUtils
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple converter between Chinese and arabic number
 Home-page: https://github.com/nrchan/chinese-number-converter
 Author: NR
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ChineseNumberUtils-1.1.1/README.md` & `ChineseNumberUtils-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ChineseNumberUtils-1.1.1/cnc/ChineseNumberUtils.egg-info/PKG-INFO` & `ChineseNumberUtils-1.1.2/src/ChineseNumberUtils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChineseNumberUtils
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple converter between Chinese and arabic number
 Home-page: https://github.com/nrchan/chinese-number-converter
 Author: NR
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ChineseNumberUtils-1.1.1/setup.cfg` & `ChineseNumberUtils-1.1.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 6869 6e65 7365 4e75 6d62 6572   = ChineseNumber
 00000020: 5574 696c 730d 0a76 6572 7369 6f6e 203d  Utils..version =
-00000030: 2031 2e31 2e31 0d0a 6175 7468 6f72 203d   1.1.1..author =
+00000030: 2031 2e31 2e32 0d0a 6175 7468 6f72 203d   1.1.2..author =
 00000040: 204e 520d 0a64 6573 6372 6970 7469 6f6e   NR..description
 00000050: 203d 2041 2073 696d 706c 6520 636f 6e76   = A simple conv
 00000060: 6572 7465 7220 6265 7477 6565 6e20 4368  erter between Ch
 00000070: 696e 6573 6520 616e 6420 6172 6162 6963  inese and arabic
 00000080: 206e 756d 6265 720d 0a6c 6f6e 675f 6465   number..long_de
 00000090: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 000000a0: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
@@ -40,17 +40,17 @@
 00000270: 7561 6765 203a 3a20 4368 696e 6573 6520  uage :: Chinese 
 00000280: 2854 7261 6469 7469 6f6e 616c 290d 0a09  (Traditional)...
 00000290: 4e61 7475 7261 6c20 4c61 6e67 7561 6765  Natural Language
 000002a0: 203a 3a20 4368 696e 6573 6520 2853 696d   :: Chinese (Sim
 000002b0: 706c 6966 6965 6429 0d0a 0954 6f70 6963  plified)...Topic
 000002c0: 203a 3a20 5574 696c 6974 6965 730d 0a0d   :: Utilities...
 000002d0: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-000002e0: 6167 655f 6469 7220 3d20 0d0a 093d 2063  age_dir = ...= c
-000002f0: 6e63 0d0a 7061 636b 6167 6573 203d 2066  nc..packages = f
+000002e0: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
+000002f0: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
 00000300: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
 00000310: 7569 7265 7320 3d20 3e3d 332e 360d 0a0d  uires = >=3.6...
 00000320: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
 00000330: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-00000340: 3d20 636e 630d 0a0d 0a5b 6567 675f 696e  = cnc....[egg_in
+00000340: 3d20 7372 630d 0a0d 0a5b 6567 675f 696e  = src....[egg_in
 00000350: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
 00000360: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
 00000370: 0a0d 0a                                  ...
```

