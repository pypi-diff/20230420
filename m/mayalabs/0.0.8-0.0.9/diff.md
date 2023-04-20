# Comparing `tmp/mayalabs-0.0.8.tar.gz` & `tmp/mayalabs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayalabs-0.0.8.tar", last modified: Mon Apr 17 16:05:13 2023, max compression
+gzip compressed data, was "mayalabs-0.0.9.tar", last modified: Thu Apr 20 16:30:26 2023, max compression
```

## Comparing `mayalabs-0.0.8.tar` & `mayalabs-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-17 16:05:13.921157 mayalabs-0.0.8/
--rw-r--r--   0 shubham    (501) staff       (20)     1054 2023-03-28 13:53:19.000000 mayalabs-0.0.8/LICENCE
--rw-r--r--   0 shubham    (501) staff       (20)     3633 2023-04-17 16:05:13.920974 mayalabs-0.0.8/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)     3187 2023-04-17 12:33:36.000000 mayalabs-0.0.8/README.md
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-17 16:05:13.912380 mayalabs-0.0.8/examples/
--rw-r--r--   0 shubham    (501) staff       (20)      644 2023-04-13 07:38:39.000000 mayalabs-0.0.8/examples/add_to_google_sheet.py
--rw-r--r--   0 shubham    (501) staff       (20)      665 2023-04-13 07:38:39.000000 mayalabs-0.0.8/examples/native_memory.py
--rw-r--r--   0 shubham    (501) staff       (20)      717 2023-04-13 07:38:39.000000 mayalabs-0.0.8/examples/web_scraping.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-17 16:05:13.914455 mayalabs-0.0.8/mayalabs/
--rw-r--r--   0 shubham    (501) staff       (20)      364 2023-04-10 12:10:07.000000 mayalabs-0.0.8/mayalabs/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     8115 2023-04-14 14:01:06.000000 mayalabs-0.0.8/mayalabs/cli.py
--rw-r--r--   0 shubham    (501) staff       (20)      269 2023-04-17 14:31:38.000000 mayalabs-0.0.8/mayalabs/exceptions.py
--rw-r--r--   0 shubham    (501) staff       (20)     7959 2023-04-17 14:31:46.000000 mayalabs-0.0.8/mayalabs/function.py
--rw-r--r--   0 shubham    (501) staff       (20)     1142 2023-04-06 10:29:10.000000 mayalabs-0.0.8/mayalabs/mayalabs.py
--rw-r--r--   0 shubham    (501) staff       (20)    13356 2023-04-17 12:33:00.000000 mayalabs-0.0.8/mayalabs/session.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-17 16:05:13.918459 mayalabs-0.0.8/mayalabs/utils/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2023-03-27 23:24:06.000000 mayalabs-0.0.8/mayalabs/utils/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     1249 2023-04-10 12:10:07.000000 mayalabs-0.0.8/mayalabs/utils/defaults.py
--rw-r--r--   0 shubham    (501) staff       (20)     5315 2023-04-17 14:31:58.000000 mayalabs-0.0.8/mayalabs/utils/general.py
--rw-r--r--   0 shubham    (501) staff       (20)     1434 2023-03-29 17:05:06.000000 mayalabs-0.0.8/mayalabs/utils/log.py
--rw-r--r--   0 shubham    (501) staff       (20)      202 2023-03-29 17:04:56.000000 mayalabs-0.0.8/mayalabs/utils/logging.py
--rw-r--r--   0 shubham    (501) staff       (20)     3973 2023-03-27 23:24:06.000000 mayalabs-0.0.8/mayalabs/utils/name_gen.py
--rw-r--r--   0 shubham    (501) staff       (20)     7923 2023-04-10 12:10:07.000000 mayalabs-0.0.8/mayalabs/utils/pac_engine.py
--rw-r--r--   0 shubham    (501) staff       (20)      628 2023-03-29 10:15:45.000000 mayalabs-0.0.8/mayalabs/utils/poll.py
--rw-r--r--   0 shubham    (501) staff       (20)     5181 2023-04-13 12:38:22.000000 mayalabs-0.0.8/mayalabs/utils/websocket.py
--rw-r--r--   0 shubham    (501) staff       (20)    19095 2023-04-17 14:31:00.000000 mayalabs-0.0.8/mayalabs/worker.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-17 16:05:13.915635 mayalabs-0.0.8/mayalabs.egg-info/
--rw-r--r--   0 shubham    (501) staff       (20)     3633 2023-04-17 16:05:13.000000 mayalabs-0.0.8/mayalabs.egg-info/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)      796 2023-04-17 16:05:13.000000 mayalabs-0.0.8/mayalabs.egg-info/SOURCES.txt
--rw-r--r--   0 shubham    (501) staff       (20)        1 2023-04-17 16:05:13.000000 mayalabs-0.0.8/mayalabs.egg-info/dependency_links.txt
--rw-r--r--   0 shubham    (501) staff       (20)       46 2023-04-17 16:05:13.000000 mayalabs-0.0.8/mayalabs.egg-info/entry_points.txt
--rw-r--r--   0 shubham    (501) staff       (20)      106 2023-04-17 16:05:13.000000 mayalabs-0.0.8/mayalabs.egg-info/requires.txt
--rw-r--r--   0 shubham    (501) staff       (20)       35 2023-04-17 16:05:13.000000 mayalabs-0.0.8/mayalabs.egg-info/top_level.txt
--rw-r--r--   0 shubham    (501) staff       (20)      874 2023-04-17 16:02:31.000000 mayalabs-0.0.8/pyproject.toml
--rw-r--r--   0 shubham    (501) staff       (20)       38 2023-04-17 16:05:13.921208 mayalabs-0.0.8/setup.cfg
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-17 16:05:13.919843 mayalabs-0.0.8/tests/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2023-04-10 12:10:07.000000 mayalabs-0.0.8/tests/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)      641 2023-04-17 16:03:07.000000 mayalabs-0.0.8/tests/example_1.py
--rw-r--r--   0 shubham    (501) staff       (20)     1313 2023-04-17 16:03:43.000000 mayalabs-0.0.8/tests/example_2.py
--rw-r--r--   0 shubham    (501) staff       (20)      887 2023-04-17 16:04:03.000000 mayalabs-0.0.8/tests/example_3.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-17 16:05:13.920651 mayalabs-0.0.8/usage/
--rw-r--r--   0 shubham    (501) staff       (20)      169 2023-04-10 12:10:07.000000 mayalabs-0.0.8/usage/function.py
--rw-r--r--   0 shubham    (501) staff       (20)      414 2023-04-10 12:10:07.000000 mayalabs-0.0.8/usage/sql_test.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-20 16:30:26.317677 mayalabs-0.0.9/
+-rw-r--r--   0 shubham    (501) staff       (20)     1054 2023-03-28 13:53:19.000000 mayalabs-0.0.9/LICENCE
+-rw-r--r--   0 shubham    (501) staff       (20)     4036 2023-04-20 16:30:26.317504 mayalabs-0.0.9/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)     3590 2023-04-20 16:29:10.000000 mayalabs-0.0.9/README.md
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-20 16:30:26.309252 mayalabs-0.0.9/examples/
+-rw-r--r--   0 shubham    (501) staff       (20)      644 2023-04-18 11:54:27.000000 mayalabs-0.0.9/examples/add_to_google_sheet.py
+-rw-r--r--   0 shubham    (501) staff       (20)      665 2023-04-18 11:54:27.000000 mayalabs-0.0.9/examples/native_memory.py
+-rw-r--r--   0 shubham    (501) staff       (20)      717 2023-04-18 11:54:27.000000 mayalabs-0.0.9/examples/web_scraping.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-20 16:30:26.311207 mayalabs-0.0.9/mayalabs/
+-rw-r--r--   0 shubham    (501) staff       (20)      364 2023-04-10 12:10:07.000000 mayalabs-0.0.9/mayalabs/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     7928 2023-04-19 10:10:08.000000 mayalabs-0.0.9/mayalabs/cli.py
+-rw-r--r--   0 shubham    (501) staff       (20)      366 2023-04-20 16:22:24.000000 mayalabs-0.0.9/mayalabs/exceptions.py
+-rw-r--r--   0 shubham    (501) staff       (20)    15331 2023-04-20 16:22:24.000000 mayalabs-0.0.9/mayalabs/function.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1142 2023-04-06 10:29:10.000000 mayalabs-0.0.9/mayalabs/mayalabs.py
+-rw-r--r--   0 shubham    (501) staff       (20)    15329 2023-04-20 16:22:24.000000 mayalabs-0.0.9/mayalabs/session.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-20 16:30:26.315857 mayalabs-0.0.9/mayalabs/utils/
+-rw-r--r--   0 shubham    (501) staff       (20)        0 2023-03-27 23:24:06.000000 mayalabs-0.0.9/mayalabs/utils/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1425 2023-04-20 16:22:24.000000 mayalabs-0.0.9/mayalabs/utils/defaults.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5383 2023-04-20 16:22:24.000000 mayalabs-0.0.9/mayalabs/utils/general.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1434 2023-03-29 17:05:06.000000 mayalabs-0.0.9/mayalabs/utils/log.py
+-rw-r--r--   0 shubham    (501) staff       (20)      202 2023-03-29 17:04:56.000000 mayalabs-0.0.9/mayalabs/utils/logging.py
+-rw-r--r--   0 shubham    (501) staff       (20)     3973 2023-03-27 23:24:06.000000 mayalabs-0.0.9/mayalabs/utils/name_gen.py
+-rw-r--r--   0 shubham    (501) staff       (20)     7923 2023-04-20 14:05:18.000000 mayalabs-0.0.9/mayalabs/utils/pac_engine.py
+-rw-r--r--   0 shubham    (501) staff       (20)      628 2023-03-29 10:15:45.000000 mayalabs-0.0.9/mayalabs/utils/poll.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5181 2023-04-13 12:38:22.000000 mayalabs-0.0.9/mayalabs/utils/websocket.py
+-rw-r--r--   0 shubham    (501) staff       (20)    20185 2023-04-20 16:22:24.000000 mayalabs-0.0.9/mayalabs/worker.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-20 16:30:26.313839 mayalabs-0.0.9/mayalabs.egg-info/
+-rw-r--r--   0 shubham    (501) staff       (20)     4036 2023-04-20 16:30:26.000000 mayalabs-0.0.9/mayalabs.egg-info/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)      796 2023-04-20 16:30:26.000000 mayalabs-0.0.9/mayalabs.egg-info/SOURCES.txt
+-rw-r--r--   0 shubham    (501) staff       (20)        1 2023-04-20 16:30:26.000000 mayalabs-0.0.9/mayalabs.egg-info/dependency_links.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       46 2023-04-20 16:30:26.000000 mayalabs-0.0.9/mayalabs.egg-info/entry_points.txt
+-rw-r--r--   0 shubham    (501) staff       (20)      106 2023-04-20 16:30:26.000000 mayalabs-0.0.9/mayalabs.egg-info/requires.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       35 2023-04-20 16:30:26.000000 mayalabs-0.0.9/mayalabs.egg-info/top_level.txt
+-rw-r--r--   0 shubham    (501) staff       (20)      874 2023-04-20 16:23:12.000000 mayalabs-0.0.9/pyproject.toml
+-rw-r--r--   0 shubham    (501) staff       (20)       38 2023-04-20 16:30:26.317719 mayalabs-0.0.9/setup.cfg
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-20 16:30:26.316741 mayalabs-0.0.9/tests/
+-rw-r--r--   0 shubham    (501) staff       (20)        0 2023-04-10 12:10:07.000000 mayalabs-0.0.9/tests/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)      641 2023-04-18 11:54:27.000000 mayalabs-0.0.9/tests/example_1.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1313 2023-04-18 11:54:27.000000 mayalabs-0.0.9/tests/example_2.py
+-rw-r--r--   0 shubham    (501) staff       (20)      887 2023-04-18 11:54:27.000000 mayalabs-0.0.9/tests/example_3.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-20 16:30:26.317192 mayalabs-0.0.9/usage/
+-rw-r--r--   0 shubham    (501) staff       (20)      169 2023-04-10 12:10:07.000000 mayalabs-0.0.9/usage/function.py
+-rw-r--r--   0 shubham    (501) staff       (20)      414 2023-04-10 12:10:07.000000 mayalabs-0.0.9/usage/sql_test.py
```

### Comparing `mayalabs-0.0.8/LICENCE` & `mayalabs-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.8/PKG-INFO` & `mayalabs-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d61 7961  : 2.1.Name: maya
 00000020: 6c61 6273 0a56 6572 7369 6f6e 3a20 302e  labs.Version: 0.
-00000030: 302e 380a 5375 6d6d 6172 793a 2050 7974  0.8.Summary: Pyt
+00000030: 302e 390a 5375 6d6d 6172 793a 2050 7974  0.9.Summary: Pyt
 00000040: 686f 6e20 5344 4b20 666f 7220 4d61 7961  hon SDK for Maya
 00000050: 204c 6162 7327 206e 6174 7572 616c 206c   Labs' natural l
 00000060: 616e 6775 6167 6520 7072 6f67 7261 6d6d  anguage programm
 00000070: 696e 6720 7061 7261 6469 676d 0a41 7574  ing paradigm.Aut
 00000080: 686f 722d 656d 6169 6c3a 204d 6179 6120  hor-email: Maya 
 00000090: 5375 7070 6f72 7420 3c68 756d 616e 7340  Support <humans@
 000000a0: 6d61 7961 6c61 6273 2e69 6f3e 0a4d 6169  mayalabs.io>.Mai
@@ -25,204 +25,229 @@
 00000180: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
 00000190: 6e0a 5072 6f76 6964 6573 2d45 7874 7261  n.Provides-Extra
 000001a0: 3a20 7465 7374 0a4c 6963 656e 7365 2d46  : test.License-F
 000001b0: 696c 653a 204c 4943 454e 4345 0a0a 2320  ile: LICENCE..# 
 000001c0: 4d61 7961 204c 6162 7320 3a20 5072 6f67  Maya Labs : Prog
 000001d0: 7261 6d20 6d61 6368 696e 6573 2075 7369  ram machines usi
 000001e0: 6e67 206e 6174 7572 616c 206c 616e 6775  ng natural langu
-000001f0: 6167 652e 0a0a 5468 6520 4d61 7961 204c  age...The Maya L
-00000200: 6162 7320 5079 7468 6f6e 2053 444b 2070  abs Python SDK p
-00000210: 726f 7669 6465 7320 6561 7379 2061 7379  rovides easy asy
-00000220: 6e63 2061 6363 6573 7320 746f 206f 7572  nc access to our
-00000230: 2050 4143 2d31 2070 726f 6772 616d 2073   PAC-1 program s
-00000240: 796e 7468 6573 6973 2065 6e67 696e 652c  ynthesis engine,
-00000250: 2077 6974 6820 6120 434c 4920 746f 2069   with a CLI to i
-00000260: 6e73 7472 7563 7420 616e 6420 6765 6e65  nstruct and gene
-00000270: 7261 7465 2070 726f 6772 616d 7320 6672  rate programs fr
-00000280: 6f6d 2069 6e73 7472 7563 7469 6f6e 7320  om instructions 
-00000290: 696e 206e 6174 7572 616c 206c 616e 6775  in natural langu
-000002a0: 6167 652e 0a0a 0a23 2320 496e 7374 616c  age....## Instal
-000002b0: 6c61 7469 6f6e 0a0a 6060 600a 7069 7020  lation..```.pip 
-000002c0: 696e 7374 616c 6c20 2d2d 7570 6772 6164  install --upgrad
-000002d0: 6520 6d61 7961 6c61 6273 0a60 6060 0a23  e mayalabs.```.#
-000002e0: 2320 5072 6576 6965 770a 0a68 7474 7073  # Preview..https
-000002f0: 3a2f 2f75 7365 722d 696d 6167 6573 2e67  ://user-images.g
-00000300: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00000310: 2e63 6f6d 2f38 3733 3637 3937 2f32 3330  .com/8736797/230
-00000320: 3934 3734 3430 2d32 3430 3337 3632 642d  947440-2403762d-
-00000330: 6131 3462 2d34 6230 302d 3866 6265 2d62  a14b-4b00-8fbe-b
-00000340: 6438 3033 6162 3234 3032 382e 6d70 340a  d803ab24028.mp4.
-00000350: 0a0a 2323 2055 7361 6765 0a0a 4765 7420  ..## Usage..Get 
-00000360: 7468 6520 4d61 7961 204c 6162 7320 4150  the Maya Labs AP
-00000370: 4920 6b65 7920 6672 6f6d 2074 6865 2053  I key from the S
-00000380: 6574 7469 6e67 7320 3e20 4465 7665 6c6f  ettings > Develo
-00000390: 7065 7220 5b73 6563 7469 6f6e 5d28 6874  per [section](ht
-000003a0: 7470 733a 2f2f 6170 702e 6d61 7961 6c61  tps://app.mayala
-000003b0: 6273 2e69 6f2f 7365 7474 696e 6773 2f64  bs.io/settings/d
-000003c0: 6576 656c 6f70 6572 7329 2e0a 0a60 6060  evelopers)...```
-000003d0: 0a65 7870 6f72 7420 4d41 5941 5f41 5049  .export MAYA_API
-000003e0: 5f4b 4559 203d 2022 6d61 7961 6b65 792d  _KEY = "mayakey-
-000003f0: 2e2e 2e22 0a60 6060 0a0a 4f72 2073 6574  ...".```..Or set
-00000400: 2060 6d61 7961 6c61 6273 2e61 7069 5f6b   `mayalabs.api_k
-00000410: 6579 6020 746f 2069 7473 2076 616c 7565  ey` to its value
-00000420: 3a0a 0a60 6060 0a69 6d70 6f72 7420 6d61  :..```.import ma
-00000430: 7961 6c61 6273 0a0a 6d61 7961 6c61 6273  yalabs..mayalabs
-00000440: 2e61 7069 5f6b 6579 203d 2022 6d61 7961  .api_key = "maya
-00000450: 6b65 792d 2e2e 2e22 0a0a 7363 7269 7074  key-..."..script
-00000460: 203d 2022 2222 0a31 2e20 7472 6967 6765   = """.1. trigge
-00000470: 7220 6f6e 2072 6563 6569 7665 0a32 2e20  r on receive.2. 
-00000480: 7265 7365 6172 6368 207b 7b74 6572 6d7d  research {{term}
-00000490: 7d20 6f6e 2077 696b 6970 6564 6961 0a33  } on wikipedia.3
-000004a0: 2e20 6578 7472 6163 7420 2774 6974 6c65  . extract 'title
-000004b0: 2720 616e 6420 2773 756d 6d61 7279 2720  ' and 'summary' 
-000004c0: 6672 6f6d 2074 6162 756c 6172 2064 6174  from tabular dat
-000004d0: 610a 342e 2073 656e 6420 7265 7370 6f6e  a.4. send respon
-000004e0: 7365 2062 6163 6b0a 2222 220a 0a66 756e  se back."""..fun
-000004f0: 6374 696f 6e20 3d20 6d61 7961 6c61 6273  ction = mayalabs
-00000500: 2e46 756e 6374 696f 6e28 6e61 6d65 3d22  .Function(name="
-00000510: 5363 7261 7065 3222 290a 2320 4372 6561  Scrape2").# Crea
-00000520: 7469 6e67 206e 6577 2077 6f72 6b65 722e  ting new worker.
-00000530: 2e2e 0a0a 6675 6e63 7469 6f6e 2e75 7064  ....function.upd
-00000540: 6174 6528 7363 7269 7074 3d73 6372 6970  ate(script=scrip
-00000550: 7429 0a23 2047 656e 6572 6174 696e 6720  t).# Generating 
-00000560: 7072 6f67 7261 6d20 6772 6170 682e 2e2e  program graph...
-00000570: 0a23 2053 7461 7274 696e 6720 776f 726b  .# Starting work
-00000580: 6572 2e2e 2e0a 2320 496e 7374 616c 6c69  er....# Installi
-00000590: 6e67 2064 6570 656e 6465 6e63 6965 732e  ng dependencies.
-000005a0: 2e2e 0a23 2044 6570 6c6f 7965 6421 0a0a  ...# Deployed!..
-000005b0: 6f75 7470 7574 203d 2066 756e 6374 696f  output = functio
-000005c0: 6e2e 6361 6c6c 287b 2274 6572 6d22 3a20  n.call({"term": 
-000005d0: 2244 722e 2056 696b 7261 6d20 5361 7261  "Dr. Vikram Sara
-000005e0: 6268 6169 227d 290a 7072 696e 7428 6f75  bhai"}).print(ou
-000005f0: 7470 7574 290a 2320 6669 6e64 7320 616e  tput).# finds an
-00000600: 6420 6f75 7470 7574 7320 7469 746c 6520  d outputs title 
-00000610: 616e 6420 7375 6d6d 6172 7920 6672 6f6d  and summary from
-00000620: 2077 696b 6970 6564 6961 2072 6573 756c   wikipedia resul
-00000630: 7473 0a0a 6060 600a 0a50 4143 2d31 2074  ts..```..PAC-1 t
-00000640: 616b 6573 2069 6e20 7374 6570 7320 7772  akes in steps wr
-00000650: 6974 7465 6e20 696e 2045 6e67 6c69 7368  itten in English
-00000660: 2c20 7772 6974 6573 2026 2061 7373 656d  , writes & assem
-00000670: 626c 6573 2061 2064 6973 6372 6574 6520  bles a discrete 
-00000680: 7072 6f67 7261 6d20 6772 6170 682c 2061  program graph, a
-00000690: 6e64 2064 6570 6c6f 7973 2072 6561 6479  nd deploys ready
-000006a0: 2d74 6f2d 7573 6520 736f 6674 7761 7265  -to-use software
-000006b0: 206f 6e20 6f75 7220 636f 6d70 7574 6520   on our compute 
-000006c0: 696e 6672 6173 7472 7563 7475 7265 2c20  infrastructure, 
-000006d0: 7468 6174 2079 6f75 2063 616e 2063 616c  that you can cal
-000006e0: 6c20 7769 7468 696e 2079 6f75 7220 636f  l within your co
-000006f0: 6465 2e20 596f 7520 6361 6e20 7365 7420  de. You can set 
-00000700: 7570 206d 6973 7369 6e67 2064 6570 656e  up missing depen
-00000710: 6465 6e63 6965 7320 2f20 7669 7375 616c  dencies / visual
-00000720: 697a 6520 7468 6520 666c 6f77 206f 6620  ize the flow of 
-00000730: 6c6f 6769 6320 6279 2066 6f6c 6c6f 7769  logic by followi
-00000740: 6e67 2074 6865 206c 696e 6b20 746f 2066  ng the link to f
-00000750: 6c6f 772d 6261 7365 6420 6564 6974 6f72  low-based editor
-00000760: 2069 7420 7072 6f76 6964 6573 2061 6674   it provides aft
-00000770: 6572 2064 6570 6c6f 796d 656e 742e 0a0a  er deployment...
-00000780: 2323 2055 7365 2043 6173 6573 0a0a 2d20  ## Use Cases..- 
-00000790: 5b49 662e 2e2e 5468 656e 2043 6f6e 6469  [If...Then Condi
-000007a0: 7469 6f6e 616c 7320 616e 6420 4c6f 6f70  tionals and Loop
-000007b0: 696e 675d 282f 4558 414d 504c 4553 2e6d  ing](/EXAMPLES.m
-000007c0: 6423 6966 7468 656e 2d63 6f6e 6469 7469  d#ifthen-conditi
-000007d0: 6f6e 616c 732d 616e 642d 6c6f 6f70 696e  onals-and-loopin
-000007e0: 6729 0a2d 205b 4375 7374 6f6d 2046 756e  g).- [Custom Fun
-000007f0: 6374 696f 6e73 5d28 2f45 5841 4d50 4c45  ctions](/EXAMPLE
-00000800: 532e 6d64 2363 7573 746f 6d2d 6675 6e63  S.md#custom-func
-00000810: 7469 6f6e 7329 0a2d 205b 5765 6220 5363  tions).- [Web Sc
-00000820: 7261 7065 7273 5d28 2f45 5841 4d50 4c45  rapers](/EXAMPLE
-00000830: 532e 6d64 2377 6562 2d73 6372 6170 6572  S.md#web-scraper
-00000840: 7329 0a2d 205b 5265 7065 6174 696e 6720  s).- [Repeating 
-00000850: 576f 726b 666c 6f77 735d 282f 4558 414d  Workflows](/EXAM
-00000860: 504c 4553 2e6d 6423 7265 7065 6174 696e  PLES.md#repeatin
-00000870: 672d 776f 726b 666c 6f77 7329 0a2d 205b  g-workflows).- [
-00000880: 4375 7374 6f6d 2044 6173 6862 6f61 7264  Custom Dashboard
-00000890: 735d 282f 4558 414d 504c 4553 2e6d 6423  s](/EXAMPLES.md#
-000008a0: 6375 7374 6f6d 2d64 6173 6862 6f61 7264  custom-dashboard
-000008b0: 7329 0a2d 205b 4461 7461 2054 7261 6e73  s).- [Data Trans
-000008c0: 666f 726d 6174 696f 6e5d 282f 4558 414d  formation](/EXAM
-000008d0: 504c 4553 2e6d 6423 6461 7461 2d74 7261  PLES.md#data-tra
-000008e0: 6e73 666f 726d 6174 696f 6e29 0a2d 205b  nsformation).- [
-000008f0: 506c 6174 666f 726d 2042 6f74 735d 282f  Platform Bots](/
-00000900: 4558 414d 504c 4553 2e6d 6423 706c 6174  EXAMPLES.md#plat
-00000910: 666f 726d 2d62 6f74 7329 0a2d 205b 4275  form-bots).- [Bu
-00000920: 7369 6e65 7373 2050 726f 6365 7373 6573  siness Processes
-00000930: 5d28 2f45 5841 4d50 4c45 532e 6d64 2362  ](/EXAMPLES.md#b
-00000940: 7573 696e 6573 732d 7072 6f63 6573 7365  usiness-processe
-00000950: 7329 0a2d 205b 4c6f 6e67 2d74 6572 6d20  s).- [Long-term 
-00000960: 6d65 6d6f 7279 5d28 2f45 5841 4d50 4c45  memory](/EXAMPLE
-00000970: 532e 6d64 236c 6f6e 672d 7465 726d 2d6d  S.md#long-term-m
-00000980: 656d 6f72 7929 0a2d 205b 4469 7669 7369  emory).- [Divisi
-00000990: 6f6e 206f 6620 6c61 626f 7572 5d28 2f45  on of labour](/E
-000009a0: 5841 4d50 4c45 532e 6d64 2364 6976 6973  XAMPLES.md#divis
-000009b0: 696f 6e2d 6f66 2d6c 6162 6f75 7229 0a20  ion-of-labour). 
-000009c0: 202d 205b 5061 7261 6c6c 656c 697a 6174   - [Parallelizat
-000009d0: 696f 6e5d 282f 4558 414d 504c 4553 2e6d  ion](/EXAMPLES.m
-000009e0: 6423 7061 7261 6c6c 656c 697a 6174 696f  d#parallelizatio
-000009f0: 6e29 0a20 202d 205b 436f 6e63 7572 7265  n).  - [Concurre
-00000a00: 6e63 795d 282f 4558 414d 504c 4553 2e6d  ncy](/EXAMPLES.m
-00000a10: 6423 636f 6e63 7572 7265 6e63 7929 0a0a  d#concurrency)..
-00000a20: 2323 2043 6f6d 6d61 6e64 204c 696e 6520  ## Command Line 
-00000a30: 5573 6167 650a 0a54 6f64 6179 2c20 7363  Usage..Today, sc
-00000a40: 7269 7074 206e 6565 6420 746f 2062 6520  ript need to be 
-00000a50: 6d61 6e75 616c 6c79 2077 7269 7474 656e  manually written
-00000a60: 2073 7465 702d 6279 2d73 7465 702c 2062   step-by-step, b
-00000a70: 7574 2077 6520 6172 6520 6f66 6665 7269  ut we are offeri
-00000a80: 6e67 2065 6172 6c79 2057 4950 2070 7265  ng early WIP pre
-00000a90: 7669 6577 206f 6620 6974 6572 6174 6976  view of iterativ
-00000aa0: 6520 7363 7269 7074 2067 656e 6572 6174  e script generat
-00000ab0: 696f 6e20 7669 6120 6f75 7220 434c 492e  ion via our CLI.
-00000ac0: 2054 7279 2072 756e 6e69 6e67 3a0a 0a60   Try running:..`
-00000ad0: 6060 0a24 206d 6179 616c 6162 7320 696e  ``.$ mayalabs in
-00000ae0: 7374 7275 6374 202d 6320 2766 6574 6368  struct -c 'fetch
-00000af0: 204e 616d 6520 616e 6420 456d 6169 6c20   Name and Email 
-00000b00: 6672 6f6d 2067 7368 6565 742c 2077 7269  from gsheet, wri
-00000b10: 7465 2066 756e 6374 696f 6e20 746f 206d  te function to m
-00000b20: 6572 6765 2061 6c6c 2063 6f6c 756d 6e73  erge all columns
-00000b30: 2c20 616e 6420 7265 7475 726e 2064 6174  , and return dat
-00000b40: 6127 0a60 6060 0a0a 416e 6420 7468 656e  a'.```..And then
-00000b50: 2075 7365 2074 6865 2067 656e 6572 6174   use the generat
-00000b60: 6564 2073 6372 6970 7420 6173 2066 756e  ed script as fun
-00000b70: 6374 696f 6e2e 0a0a 6874 7470 733a 2f2f  ction...https://
-00000b80: 7573 6572 2d69 6d61 6765 732e 6769 7468  user-images.gith
-00000b90: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00000ba0: 6d2f 3532 3439 3330 3737 2f32 3331 3937  m/52493077/23197
-00000bb0: 3932 3834 2d61 3764 3163 3433 642d 6636  9284-a7d1c43d-f6
-00000bc0: 6336 2d34 3732 362d 3839 6665 2d32 3865  c6-4726-89fe-28e
-00000bd0: 3130 3363 6431 3938 662e 6d70 340a 0a23  103cd198f.mp4..#
-00000be0: 2320 5265 7175 6972 656d 656e 7473 0a0a  # Requirements..
-00000bf0: 2d20 5079 7468 6f6e 2033 2e37 2e31 2b0a  - Python 3.7.1+.
-00000c00: 0a23 2320 4973 7375 6573 0a0a 416c 6c20  .## Issues..All 
-00000c10: 6665 6564 6261 636b 2061 6e64 2062 7567  feedback and bug
-00000c20: 2072 6570 6f72 7473 2077 656c 636f 6d65   reports welcome
-00000c30: 2120 5265 706f 7274 2069 6e20 7468 6520  ! Report in the 
-00000c40: 5b69 7373 7565 7320 7365 6374 696f 6e5d  [issues section]
-00000c50: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000c60: 636f 6d2f 6d61 7961 6871 2f6d 6179 616c  com/mayahq/mayal
-00000c70: 6162 732d 7364 6b2d 7079 7468 6f6e 2f69  abs-sdk-python/i
-00000c80: 7373 7565 7329 2c20 6f72 206d 6169 6c20  ssues), or mail 
-00000c90: 7573 2061 7420 6875 6d61 6e73 406d 6179  us at humans@may
-00000ca0: 616c 6162 732e 696f 2e0a 0a46 756c 6c20  alabs.io...Full 
-00000cb0: 6c69 7374 206f 6620 6361 7061 6269 6c69  list of capabili
-00000cc0: 7469 6573 2061 6e64 206c 696d 6974 7320  ties and limits 
-00000cd0: 5b68 6572 655d 2868 7474 7073 3a2f 2f64  [here](https://d
-00000ce0: 6f63 732e 6d61 7961 6c61 6273 2e69 6f2f  ocs.mayalabs.io/
-00000cf0: 6361 7061 6269 6c69 7469 6573 2d61 6e64  capabilities-and
-00000d00: 2d6c 696d 6974 7329 2e0a 0a0a 2323 2052  -limits)....## R
-00000d10: 6f61 646d 6170 0a2d 205b 785d 2043 6c65  oadmap.- [x] Cle
-00000d20: 616e 6572 206c 6f67 7320 616e 6420 6578  aner logs and ex
-00000d30: 6365 7074 696f 6e20 6861 6e64 6c69 6e67  ception handling
-00000d40: 0a2d 205b 205d 2044 6570 656e 6465 6e63  .- [ ] Dependenc
-00000d50: 7920 636f 6e66 6967 7572 6174 696f 6e20  y configuration 
-00000d60: 5558 2069 6d70 726f 7665 6d65 6e74 0a2d  UX improvement.-
-00000d70: 205b 205d 2049 6d70 6f72 7420 736b 696c   [ ] Import skil
-00000d80: 6c20 7265 706f 7369 746f 7269 6573 2066  l repositories f
-00000d90: 6f72 2072 6575 7369 6e67 2073 6b69 6c6c  or reusing skill
-00000da0: 7320 6372 6561 7465 6420 6279 2075 7365  s created by use
-00000db0: 7220 6f72 2070 7265 7365 6e74 2069 6e20  r or present in 
-00000dc0: 7374 6f72 650a 2d20 5b20 5d20 4372 6561  store.- [ ] Crea
-00000dd0: 7465 2061 6e64 2063 616c 6c20 646f 776e  te and call down
-00000de0: 7374 7265 616d 2061 7574 6f2d 6465 706c  stream auto-depl
-00000df0: 6f79 6564 2066 756e 6374 696f 6e73 0a2d  oyed functions.-
-00000e00: 205b 205d 2041 6c6c 6f77 206d 756c 7469   [ ] Allow multi
-00000e10: 2d70 726f 6669 6c65 2061 6e64 2074 6561  -profile and tea
-00000e20: 6d20 7072 6f66 696c 6520 6163 6365 7373  m profile access
-00000e30: 0a                                       .
+000001f0: 6167 652e 0a0a 3c70 2061 6c69 676e 3d22  age...<p align="
+00000200: 6c65 6674 223e 0a20 203c 6120 6872 6566  left">.  <a href
+00000210: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
+00000220: 7267 2f70 726f 6a65 6374 2f6d 6179 616c  rg/project/mayal
+00000230: 6162 7322 3e0a 2020 2020 3c69 6d67 2073  abs">.    <img s
+00000240: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000250: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000260: 762f 6d61 7961 6c61 6273 3f73 7479 6c65  v/mayalabs?style
+00000270: 3d66 6f72 2d74 6865 2d62 6164 6765 2220  =for-the-badge" 
+00000280: 2f3e 0a20 203c 2f61 3e0a 2020 3c61 2068  />.  </a>.  <a h
+00000290: 7265 663d 2268 7474 7073 3a2f 2f6d 6179  ref="https://may
+000002a0: 616c 6162 732e 696f 2f64 6f63 7322 3e0a  alabs.io/docs">.
+000002b0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000002c0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000002d0: 732e 696f 2f62 6164 6765 2f44 6f63 756d  s.io/badge/Docum
+000002e0: 656e 7461 7469 6f6e 2d62 6c75 653f 6c6f  entation-blue?lo
+000002f0: 676f 3d47 6974 426f 6f6b 266c 6f67 6f43  go=GitBook&logoC
+00000300: 6f6c 6f72 3d77 6869 7465 2673 7479 6c65  olor=white&style
+00000310: 3d66 6f72 2d74 6865 2d62 6164 6765 2220  =for-the-badge" 
+00000320: 2f3e 0a20 203c 2f61 3e0a 3c2f 703e 0a3c  />.  </a>.</p>.<
+00000330: 6272 3e0a 0a54 6865 204d 6179 6120 4c61  br>..The Maya La
+00000340: 6273 2050 7974 686f 6e20 5344 4b20 7072  bs Python SDK pr
+00000350: 6f76 6964 6573 2065 6173 7920 6173 796e  ovides easy asyn
+00000360: 6320 6163 6365 7373 2074 6f20 6f75 7220  c access to our 
+00000370: 5041 432d 3120 7072 6f67 7261 6d20 7379  PAC-1 program sy
+00000380: 6e74 6865 7369 7320 656e 6769 6e65 2c20  nthesis engine, 
+00000390: 7769 7468 2061 2043 4c49 2074 6f20 696e  with a CLI to in
+000003a0: 7374 7275 6374 2061 6e64 2067 656e 6572  struct and gener
+000003b0: 6174 6520 7072 6f67 7261 6d73 2066 726f  ate programs fro
+000003c0: 6d20 696e 7374 7275 6374 696f 6e73 2069  m instructions i
+000003d0: 6e20 6e61 7475 7261 6c20 6c61 6e67 7561  n natural langua
+000003e0: 6765 2e0a 0a23 2320 496e 7374 616c 6c61  ge...## Installa
+000003f0: 7469 6f6e 0a0a 6060 600a 7069 7020 696e  tion..```.pip in
+00000400: 7374 616c 6c20 2d2d 7570 6772 6164 6520  stall --upgrade 
+00000410: 6d61 7961 6c61 6273 0a60 6060 0a23 2320  mayalabs.```.## 
+00000420: 5072 6576 6965 770a 0a68 7474 7073 3a2f  Preview..https:/
+00000430: 2f75 7365 722d 696d 6167 6573 2e67 6974  /user-images.git
+00000440: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000450: 6f6d 2f38 3733 3637 3937 2f32 3330 3934  om/8736797/23094
+00000460: 3734 3430 2d32 3430 3337 3632 642d 6131  7440-2403762d-a1
+00000470: 3462 2d34 6230 302d 3866 6265 2d62 6438  4b-4b00-8fbe-bd8
+00000480: 3033 6162 3234 3032 382e 6d70 340a 0a0a  03ab24028.mp4...
+00000490: 2323 2055 7361 6765 0a0a 4765 7420 7468  ## Usage..Get th
+000004a0: 6520 4d61 7961 204c 6162 7320 4150 4920  e Maya Labs API 
+000004b0: 6b65 7920 6672 6f6d 2074 6865 2053 6574  key from the Set
+000004c0: 7469 6e67 7320 3e20 4465 7665 6c6f 7065  tings > Develope
+000004d0: 7220 5b73 6563 7469 6f6e 5d28 6874 7470  r [section](http
+000004e0: 733a 2f2f 6170 702e 6d61 7961 6c61 6273  s://app.mayalabs
+000004f0: 2e69 6f2f 7365 7474 696e 6773 2f64 6576  .io/settings/dev
+00000500: 656c 6f70 6572 7329 2e0a 0a60 6060 0a65  elopers)...```.e
+00000510: 7870 6f72 7420 4d41 5941 5f41 5049 5f4b  xport MAYA_API_K
+00000520: 4559 203d 2022 6d61 7961 6b65 792d 2e2e  EY = "mayakey-..
+00000530: 2e22 0a60 6060 0a0a 4f72 2073 6574 2060  .".```..Or set `
+00000540: 6d61 7961 6c61 6273 2e61 7069 5f6b 6579  mayalabs.api_key
+00000550: 6020 746f 2069 7473 2076 616c 7565 3a0a  ` to its value:.
+00000560: 0a60 6060 0a69 6d70 6f72 7420 6d61 7961  .```.import maya
+00000570: 6c61 6273 0a0a 6d61 7961 6c61 6273 2e61  labs..mayalabs.a
+00000580: 7069 5f6b 6579 203d 2022 6d61 7961 6b65  pi_key = "mayake
+00000590: 792d 2e2e 2e22 0a0a 7363 7269 7074 203d  y-..."..script =
+000005a0: 2022 2222 0a31 2e20 7472 6967 6765 7220   """.1. trigger 
+000005b0: 6f6e 2072 6563 6569 7665 0a32 2e20 7265  on receive.2. re
+000005c0: 7365 6172 6368 207b 7b74 6572 6d7d 7d20  search {{term}} 
+000005d0: 6f6e 2077 696b 6970 6564 6961 0a33 2e20  on wikipedia.3. 
+000005e0: 6578 7472 6163 7420 2774 6974 6c65 2720  extract 'title' 
+000005f0: 616e 6420 2773 756d 6d61 7279 2720 6672  and 'summary' fr
+00000600: 6f6d 2074 6162 756c 6172 2064 6174 610a  om tabular data.
+00000610: 342e 2073 656e 6420 7265 7370 6f6e 7365  4. send response
+00000620: 2062 6163 6b0a 2222 220a 0a66 756e 6374   back."""..funct
+00000630: 696f 6e20 3d20 6d61 7961 6c61 6273 2e46  ion = mayalabs.F
+00000640: 756e 6374 696f 6e28 6e61 6d65 3d22 5363  unction(name="Sc
+00000650: 7261 7065 3222 290a 2320 4372 6561 7469  rape2").# Creati
+00000660: 6e67 206e 6577 2077 6f72 6b65 722e 2e2e  ng new worker...
+00000670: 0a0a 6675 6e63 7469 6f6e 2e75 7064 6174  ..function.updat
+00000680: 6528 7363 7269 7074 3d73 6372 6970 7429  e(script=script)
+00000690: 0a23 2047 656e 6572 6174 696e 6720 7072  .# Generating pr
+000006a0: 6f67 7261 6d20 6772 6170 682e 2e2e 0a23  ogram graph....#
+000006b0: 2053 7461 7274 696e 6720 776f 726b 6572   Starting worker
+000006c0: 2e2e 2e0a 2320 496e 7374 616c 6c69 6e67  ....# Installing
+000006d0: 2064 6570 656e 6465 6e63 6965 732e 2e2e   dependencies...
+000006e0: 0a23 2044 6570 6c6f 7965 6421 0a0a 6f75  .# Deployed!..ou
+000006f0: 7470 7574 203d 2066 756e 6374 696f 6e2e  tput = function.
+00000700: 6361 6c6c 287b 2274 6572 6d22 3a20 2244  call({"term": "D
+00000710: 722e 2056 696b 7261 6d20 5361 7261 6268  r. Vikram Sarabh
+00000720: 6169 227d 290a 7072 696e 7428 6f75 7470  ai"}).print(outp
+00000730: 7574 290a 2320 6669 6e64 7320 616e 6420  ut).# finds and 
+00000740: 6f75 7470 7574 7320 7469 746c 6520 616e  outputs title an
+00000750: 6420 7375 6d6d 6172 7920 6672 6f6d 2077  d summary from w
+00000760: 696b 6970 6564 6961 2072 6573 756c 7473  ikipedia results
+00000770: 0a0a 6060 600a 0a50 4143 2d31 2074 616b  ..```..PAC-1 tak
+00000780: 6573 2069 6e20 7374 6570 7320 7772 6974  es in steps writ
+00000790: 7465 6e20 696e 2045 6e67 6c69 7368 2c20  ten in English, 
+000007a0: 7772 6974 6573 2026 2061 7373 656d 626c  writes & assembl
+000007b0: 6573 2061 2064 6973 6372 6574 6520 7072  es a discrete pr
+000007c0: 6f67 7261 6d20 6772 6170 682c 2061 6e64  ogram graph, and
+000007d0: 2064 6570 6c6f 7973 2072 6561 6479 2d74   deploys ready-t
+000007e0: 6f2d 7573 6520 736f 6674 7761 7265 206f  o-use software o
+000007f0: 6e20 6f75 7220 636f 6d70 7574 6520 696e  n our compute in
+00000800: 6672 6173 7472 7563 7475 7265 2c20 7468  frastructure, th
+00000810: 6174 2079 6f75 2063 616e 2063 616c 6c20  at you can call 
+00000820: 7769 7468 696e 2079 6f75 7220 636f 6465  within your code
+00000830: 2e20 596f 7520 6361 6e20 7365 7420 7570  . You can set up
+00000840: 206d 6973 7369 6e67 2064 6570 656e 6465   missing depende
+00000850: 6e63 6965 7320 2f20 7669 7375 616c 697a  ncies / visualiz
+00000860: 6520 7468 6520 666c 6f77 206f 6620 6c6f  e the flow of lo
+00000870: 6769 6320 6279 2066 6f6c 6c6f 7769 6e67  gic by following
+00000880: 2074 6865 206c 696e 6b20 746f 2066 6c6f   the link to flo
+00000890: 772d 6261 7365 6420 6564 6974 6f72 2069  w-based editor i
+000008a0: 7420 7072 6f76 6964 6573 2061 6674 6572  t provides after
+000008b0: 2064 6570 6c6f 796d 656e 742e 0a0a 4368   deployment...Ch
+000008c0: 6563 6b20 6f75 7220 5b64 6f63 756d 656e  eck our [documen
+000008d0: 7461 7469 6f6e 5d28 2268 7474 7073 3a2f  tation]("https:/
+000008e0: 2f6d 6179 616c 6162 732e 696f 2f64 6f63  /mayalabs.io/doc
+000008f0: 7322 2920 666f 7220 6d6f 7265 2075 7361  s") for more usa
+00000900: 6765 2061 6e64 2074 7574 6f72 6961 6c73  ge and tutorials
+00000910: 2e0a 0a23 2320 5573 6520 4361 7365 730a  ...## Use Cases.
+00000920: 0a2d 205b 4966 2e2e 2e54 6865 6e20 436f  .- [If...Then Co
+00000930: 6e64 6974 696f 6e61 6c73 2061 6e64 204c  nditionals and L
+00000940: 6f6f 7069 6e67 5d28 2f45 5841 4d50 4c45  ooping](/EXAMPLE
+00000950: 532e 6d64 2369 6674 6865 6e2d 636f 6e64  S.md#ifthen-cond
+00000960: 6974 696f 6e61 6c73 2d61 6e64 2d6c 6f6f  itionals-and-loo
+00000970: 7069 6e67 290a 2d20 5b43 7573 746f 6d20  ping).- [Custom 
+00000980: 4675 6e63 7469 6f6e 735d 282f 4558 414d  Functions](/EXAM
+00000990: 504c 4553 2e6d 6423 6375 7374 6f6d 2d66  PLES.md#custom-f
+000009a0: 756e 6374 696f 6e73 290a 2d20 5b57 6562  unctions).- [Web
+000009b0: 2053 6372 6170 6572 735d 282f 4558 414d   Scrapers](/EXAM
+000009c0: 504c 4553 2e6d 6423 7765 622d 7363 7261  PLES.md#web-scra
+000009d0: 7065 7273 290a 2d20 5b52 6570 6561 7469  pers).- [Repeati
+000009e0: 6e67 2057 6f72 6b66 6c6f 7773 5d28 2f45  ng Workflows](/E
+000009f0: 5841 4d50 4c45 532e 6d64 2372 6570 6561  XAMPLES.md#repea
+00000a00: 7469 6e67 2d77 6f72 6b66 6c6f 7773 290a  ting-workflows).
+00000a10: 2d20 5b43 7573 746f 6d20 4461 7368 626f  - [Custom Dashbo
+00000a20: 6172 6473 5d28 2f45 5841 4d50 4c45 532e  ards](/EXAMPLES.
+00000a30: 6d64 2363 7573 746f 6d2d 6461 7368 626f  md#custom-dashbo
+00000a40: 6172 6473 290a 2d20 5b44 6174 6120 5472  ards).- [Data Tr
+00000a50: 616e 7366 6f72 6d61 7469 6f6e 5d28 2f45  ansformation](/E
+00000a60: 5841 4d50 4c45 532e 6d64 2364 6174 612d  XAMPLES.md#data-
+00000a70: 7472 616e 7366 6f72 6d61 7469 6f6e 290a  transformation).
+00000a80: 2d20 5b50 6c61 7466 6f72 6d20 426f 7473  - [Platform Bots
+00000a90: 5d28 2f45 5841 4d50 4c45 532e 6d64 2370  ](/EXAMPLES.md#p
+00000aa0: 6c61 7466 6f72 6d2d 626f 7473 290a 2d20  latform-bots).- 
+00000ab0: 5b42 7573 696e 6573 7320 5072 6f63 6573  [Business Proces
+00000ac0: 7365 735d 282f 4558 414d 504c 4553 2e6d  ses](/EXAMPLES.m
+00000ad0: 6423 6275 7369 6e65 7373 2d70 726f 6365  d#business-proce
+00000ae0: 7373 6573 290a 2d20 5b4c 6f6e 672d 7465  sses).- [Long-te
+00000af0: 726d 206d 656d 6f72 795d 282f 4558 414d  rm memory](/EXAM
+00000b00: 504c 4553 2e6d 6423 6c6f 6e67 2d74 6572  PLES.md#long-ter
+00000b10: 6d2d 6d65 6d6f 7279 290a 2d20 5b44 6976  m-memory).- [Div
+00000b20: 6973 696f 6e20 6f66 206c 6162 6f75 725d  ision of labour]
+00000b30: 282f 4558 414d 504c 4553 2e6d 6423 6469  (/EXAMPLES.md#di
+00000b40: 7669 7369 6f6e 2d6f 662d 6c61 626f 7572  vision-of-labour
+00000b50: 290a 2020 2d20 5b50 6172 616c 6c65 6c69  ).  - [Paralleli
+00000b60: 7a61 7469 6f6e 5d28 2f45 5841 4d50 4c45  zation](/EXAMPLE
+00000b70: 532e 6d64 2370 6172 616c 6c65 6c69 7a61  S.md#paralleliza
+00000b80: 7469 6f6e 290a 2020 2d20 5b43 6f6e 6375  tion).  - [Concu
+00000b90: 7272 656e 6379 5d28 2f45 5841 4d50 4c45  rrency](/EXAMPLE
+00000ba0: 532e 6d64 2363 6f6e 6375 7272 656e 6379  S.md#concurrency
+00000bb0: 290a 0a23 2320 436f 6d6d 616e 6420 4c69  )..## Command Li
+00000bc0: 6e65 2055 7361 6765 0a0a 546f 6461 792c  ne Usage..Today,
+00000bd0: 2073 6372 6970 7420 6e65 6564 2074 6f20   script need to 
+00000be0: 6265 206d 616e 7561 6c6c 7920 7772 6974  be manually writ
+00000bf0: 7465 6e20 7374 6570 2d62 792d 7374 6570  ten step-by-step
+00000c00: 2c20 6275 7420 7765 2061 7265 206f 6666  , but we are off
+00000c10: 6572 696e 6720 6561 726c 7920 5749 5020  ering early WIP 
+00000c20: 7072 6576 6965 7720 6f66 2069 7465 7261  preview of itera
+00000c30: 7469 7665 2073 6372 6970 7420 6765 6e65  tive script gene
+00000c40: 7261 7469 6f6e 2076 6961 206f 7572 2043  ration via our C
+00000c50: 4c49 2e20 5472 7920 7275 6e6e 696e 673a  LI. Try running:
+00000c60: 0a0a 6060 600a 2420 6d61 7961 6c61 6273  ..```.$ mayalabs
+00000c70: 2069 6e73 7472 7563 7420 2d63 2027 6665   instruct -c 'fe
+00000c80: 7463 6820 4e61 6d65 2061 6e64 2045 6d61  tch Name and Ema
+00000c90: 696c 2066 726f 6d20 6773 6865 6574 2c20  il from gsheet, 
+00000ca0: 7772 6974 6520 6675 6e63 7469 6f6e 2074  write function t
+00000cb0: 6f20 6d65 7267 6520 616c 6c20 636f 6c75  o merge all colu
+00000cc0: 6d6e 732c 2061 6e64 2072 6574 7572 6e20  mns, and return 
+00000cd0: 6461 7461 270a 6060 600a 0a41 6e64 2074  data'.```..And t
+00000ce0: 6865 6e20 7573 6520 7468 6520 6765 6e65  hen use the gene
+00000cf0: 7261 7465 6420 7363 7269 7074 2061 7320  rated script as 
+00000d00: 6675 6e63 7469 6f6e 2e0a 0a68 7474 7073  function...https
+00000d10: 3a2f 2f75 7365 722d 696d 6167 6573 2e67  ://user-images.g
+00000d20: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000d30: 2e63 6f6d 2f35 3234 3933 3037 372f 3233  .com/52493077/23
+00000d40: 3139 3739 3238 342d 6137 6431 6334 3364  1979284-a7d1c43d
+00000d50: 2d66 3663 362d 3437 3236 2d38 3966 652d  -f6c6-4726-89fe-
+00000d60: 3238 6531 3033 6364 3139 3866 2e6d 7034  28e103cd198f.mp4
+00000d70: 0a0a 2323 2052 6571 7569 7265 6d65 6e74  ..## Requirement
+00000d80: 730a 0a2d 2050 7974 686f 6e20 332e 372e  s..- Python 3.7.
+00000d90: 312b 0a0a 2323 2049 7373 7565 730a 0a41  1+..## Issues..A
+00000da0: 6c6c 2066 6565 6462 6163 6b20 616e 6420  ll feedback and 
+00000db0: 6275 6720 7265 706f 7274 7320 7765 6c63  bug reports welc
+00000dc0: 6f6d 6521 2052 6570 6f72 7420 696e 2074  ome! Report in t
+00000dd0: 6865 205b 6973 7375 6573 2073 6563 7469  he [issues secti
+00000de0: 6f6e 5d28 6874 7470 733a 2f2f 6769 7468  on](https://gith
+00000df0: 7562 2e63 6f6d 2f6d 6179 6168 712f 6d61  ub.com/mayahq/ma
+00000e00: 7961 6c61 6273 2d73 646b 2d70 7974 686f  yalabs-sdk-pytho
+00000e10: 6e2f 6973 7375 6573 292c 206f 7220 6d61  n/issues), or ma
+00000e20: 696c 2075 7320 6174 2068 756d 616e 7340  il us at humans@
+00000e30: 6d61 7961 6c61 6273 2e69 6f2e 0a0a 4675  mayalabs.io...Fu
+00000e40: 6c6c 206c 6973 7420 6f66 2063 6170 6162  ll list of capab
+00000e50: 696c 6974 6965 7320 616e 6420 6c69 6d69  ilities and limi
+00000e60: 7473 205b 6865 7265 5d28 6874 7470 733a  ts [here](https:
+00000e70: 2f2f 646f 6373 2e6d 6179 616c 6162 732e  //docs.mayalabs.
+00000e80: 696f 2f63 6170 6162 696c 6974 6965 732d  io/capabilities-
+00000e90: 616e 642d 6c69 6d69 7473 292e 0a0a 0a23  and-limits)....#
+00000ea0: 2320 526f 6164 6d61 700a 2d20 5b78 5d20  # Roadmap.- [x] 
+00000eb0: 436c 6561 6e65 7220 6c6f 6773 2061 6e64  Cleaner logs and
+00000ec0: 2065 7863 6570 7469 6f6e 2068 616e 646c   exception handl
+00000ed0: 696e 670a 2d20 5b78 5d20 4465 7065 6e64  ing.- [x] Depend
+00000ee0: 656e 6379 2063 6f6e 6669 6775 7261 7469  ency configurati
+00000ef0: 6f6e 2055 5820 696d 7072 6f76 656d 656e  on UX improvemen
+00000f00: 740a 2d20 5b20 5d20 496d 706f 7274 2073  t.- [ ] Import s
+00000f10: 6b69 6c6c 2072 6570 6f73 6974 6f72 6965  kill repositorie
+00000f20: 7320 666f 7220 7265 7573 696e 6720 736b  s for reusing sk
+00000f30: 696c 6c73 2063 7265 6174 6564 2062 7920  ills created by 
+00000f40: 7573 6572 206f 7220 7072 6573 656e 7420  user or present 
+00000f50: 696e 2073 746f 7265 0a2d 205b 205d 2043  in store.- [ ] C
+00000f60: 7265 6174 6520 616e 6420 6361 6c6c 2064  reate and call d
+00000f70: 6f77 6e73 7472 6561 6d20 6175 746f 2d64  ownstream auto-d
+00000f80: 6570 6c6f 7965 6420 6675 6e63 7469 6f6e  eployed function
+00000f90: 730a 2d20 5b20 5d20 416c 6c6f 7720 6d75  s.- [ ] Allow mu
+00000fa0: 6c74 692d 7072 6f66 696c 6520 616e 6420  lti-profile and 
+00000fb0: 7465 616d 2070 726f 6669 6c65 2061 6363  team profile acc
+00000fc0: 6573 730a                                ess.
```

### Comparing `mayalabs-0.0.8/README.md` & `mayalabs-0.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,200 +1,225 @@
 00000000: 2320 4d61 7961 204c 6162 7320 3a20 5072  # Maya Labs : Pr
 00000010: 6f67 7261 6d20 6d61 6368 696e 6573 2075  ogram machines u
 00000020: 7369 6e67 206e 6174 7572 616c 206c 616e  sing natural lan
-00000030: 6775 6167 652e 0a0a 5468 6520 4d61 7961  guage...The Maya
-00000040: 204c 6162 7320 5079 7468 6f6e 2053 444b   Labs Python SDK
-00000050: 2070 726f 7669 6465 7320 6561 7379 2061   provides easy a
-00000060: 7379 6e63 2061 6363 6573 7320 746f 206f  sync access to o
-00000070: 7572 2050 4143 2d31 2070 726f 6772 616d  ur PAC-1 program
-00000080: 2073 796e 7468 6573 6973 2065 6e67 696e   synthesis engin
-00000090: 652c 2077 6974 6820 6120 434c 4920 746f  e, with a CLI to
-000000a0: 2069 6e73 7472 7563 7420 616e 6420 6765   instruct and ge
-000000b0: 6e65 7261 7465 2070 726f 6772 616d 7320  nerate programs 
-000000c0: 6672 6f6d 2069 6e73 7472 7563 7469 6f6e  from instruction
-000000d0: 7320 696e 206e 6174 7572 616c 206c 616e  s in natural lan
-000000e0: 6775 6167 652e 0a0a 0a23 2320 496e 7374  guage....## Inst
-000000f0: 616c 6c61 7469 6f6e 0a0a 6060 600a 7069  allation..```.pi
-00000100: 7020 696e 7374 616c 6c20 2d2d 7570 6772  p install --upgr
-00000110: 6164 6520 6d61 7961 6c61 6273 0a60 6060  ade mayalabs.```
-00000120: 0a23 2320 5072 6576 6965 770a 0a68 7474  .## Preview..htt
-00000130: 7073 3a2f 2f75 7365 722d 696d 6167 6573  ps://user-images
-00000140: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000150: 6e74 2e63 6f6d 2f38 3733 3637 3937 2f32  nt.com/8736797/2
-00000160: 3330 3934 3734 3430 2d32 3430 3337 3632  30947440-2403762
-00000170: 642d 6131 3462 2d34 6230 302d 3866 6265  d-a14b-4b00-8fbe
-00000180: 2d62 6438 3033 6162 3234 3032 382e 6d70  -bd803ab24028.mp
-00000190: 340a 0a0a 2323 2055 7361 6765 0a0a 4765  4...## Usage..Ge
-000001a0: 7420 7468 6520 4d61 7961 204c 6162 7320  t the Maya Labs 
-000001b0: 4150 4920 6b65 7920 6672 6f6d 2074 6865  API key from the
-000001c0: 2053 6574 7469 6e67 7320 3e20 4465 7665   Settings > Deve
-000001d0: 6c6f 7065 7220 5b73 6563 7469 6f6e 5d28  loper [section](
-000001e0: 6874 7470 733a 2f2f 6170 702e 6d61 7961  https://app.maya
-000001f0: 6c61 6273 2e69 6f2f 7365 7474 696e 6773  labs.io/settings
-00000200: 2f64 6576 656c 6f70 6572 7329 2e0a 0a60  /developers)...`
-00000210: 6060 0a65 7870 6f72 7420 4d41 5941 5f41  ``.export MAYA_A
-00000220: 5049 5f4b 4559 203d 2022 6d61 7961 6b65  PI_KEY = "mayake
-00000230: 792d 2e2e 2e22 0a60 6060 0a0a 4f72 2073  y-...".```..Or s
-00000240: 6574 2060 6d61 7961 6c61 6273 2e61 7069  et `mayalabs.api
-00000250: 5f6b 6579 6020 746f 2069 7473 2076 616c  _key` to its val
-00000260: 7565 3a0a 0a60 6060 0a69 6d70 6f72 7420  ue:..```.import 
-00000270: 6d61 7961 6c61 6273 0a0a 6d61 7961 6c61  mayalabs..mayala
-00000280: 6273 2e61 7069 5f6b 6579 203d 2022 6d61  bs.api_key = "ma
-00000290: 7961 6b65 792d 2e2e 2e22 0a0a 7363 7269  yakey-..."..scri
-000002a0: 7074 203d 2022 2222 0a31 2e20 7472 6967  pt = """.1. trig
-000002b0: 6765 7220 6f6e 2072 6563 6569 7665 0a32  ger on receive.2
-000002c0: 2e20 7265 7365 6172 6368 207b 7b74 6572  . research {{ter
-000002d0: 6d7d 7d20 6f6e 2077 696b 6970 6564 6961  m}} on wikipedia
-000002e0: 0a33 2e20 6578 7472 6163 7420 2774 6974  .3. extract 'tit
-000002f0: 6c65 2720 616e 6420 2773 756d 6d61 7279  le' and 'summary
-00000300: 2720 6672 6f6d 2074 6162 756c 6172 2064  ' from tabular d
-00000310: 6174 610a 342e 2073 656e 6420 7265 7370  ata.4. send resp
-00000320: 6f6e 7365 2062 6163 6b0a 2222 220a 0a66  onse back."""..f
-00000330: 756e 6374 696f 6e20 3d20 6d61 7961 6c61  unction = mayala
-00000340: 6273 2e46 756e 6374 696f 6e28 6e61 6d65  bs.Function(name
-00000350: 3d22 5363 7261 7065 3222 290a 2320 4372  ="Scrape2").# Cr
-00000360: 6561 7469 6e67 206e 6577 2077 6f72 6b65  eating new worke
-00000370: 722e 2e2e 0a0a 6675 6e63 7469 6f6e 2e75  r.....function.u
-00000380: 7064 6174 6528 7363 7269 7074 3d73 6372  pdate(script=scr
-00000390: 6970 7429 0a23 2047 656e 6572 6174 696e  ipt).# Generatin
-000003a0: 6720 7072 6f67 7261 6d20 6772 6170 682e  g program graph.
-000003b0: 2e2e 0a23 2053 7461 7274 696e 6720 776f  ...# Starting wo
-000003c0: 726b 6572 2e2e 2e0a 2320 496e 7374 616c  rker....# Instal
-000003d0: 6c69 6e67 2064 6570 656e 6465 6e63 6965  ling dependencie
-000003e0: 732e 2e2e 0a23 2044 6570 6c6f 7965 6421  s....# Deployed!
-000003f0: 0a0a 6f75 7470 7574 203d 2066 756e 6374  ..output = funct
-00000400: 696f 6e2e 6361 6c6c 287b 2274 6572 6d22  ion.call({"term"
-00000410: 3a20 2244 722e 2056 696b 7261 6d20 5361  : "Dr. Vikram Sa
-00000420: 7261 6268 6169 227d 290a 7072 696e 7428  rabhai"}).print(
-00000430: 6f75 7470 7574 290a 2320 6669 6e64 7320  output).# finds 
-00000440: 616e 6420 6f75 7470 7574 7320 7469 746c  and outputs titl
-00000450: 6520 616e 6420 7375 6d6d 6172 7920 6672  e and summary fr
-00000460: 6f6d 2077 696b 6970 6564 6961 2072 6573  om wikipedia res
-00000470: 756c 7473 0a0a 6060 600a 0a50 4143 2d31  ults..```..PAC-1
-00000480: 2074 616b 6573 2069 6e20 7374 6570 7320   takes in steps 
-00000490: 7772 6974 7465 6e20 696e 2045 6e67 6c69  written in Engli
-000004a0: 7368 2c20 7772 6974 6573 2026 2061 7373  sh, writes & ass
-000004b0: 656d 626c 6573 2061 2064 6973 6372 6574  embles a discret
-000004c0: 6520 7072 6f67 7261 6d20 6772 6170 682c  e program graph,
-000004d0: 2061 6e64 2064 6570 6c6f 7973 2072 6561   and deploys rea
-000004e0: 6479 2d74 6f2d 7573 6520 736f 6674 7761  dy-to-use softwa
-000004f0: 7265 206f 6e20 6f75 7220 636f 6d70 7574  re on our comput
-00000500: 6520 696e 6672 6173 7472 7563 7475 7265  e infrastructure
-00000510: 2c20 7468 6174 2079 6f75 2063 616e 2063  , that you can c
-00000520: 616c 6c20 7769 7468 696e 2079 6f75 7220  all within your 
-00000530: 636f 6465 2e20 596f 7520 6361 6e20 7365  code. You can se
-00000540: 7420 7570 206d 6973 7369 6e67 2064 6570  t up missing dep
-00000550: 656e 6465 6e63 6965 7320 2f20 7669 7375  endencies / visu
-00000560: 616c 697a 6520 7468 6520 666c 6f77 206f  alize the flow o
-00000570: 6620 6c6f 6769 6320 6279 2066 6f6c 6c6f  f logic by follo
-00000580: 7769 6e67 2074 6865 206c 696e 6b20 746f  wing the link to
-00000590: 2066 6c6f 772d 6261 7365 6420 6564 6974   flow-based edit
-000005a0: 6f72 2069 7420 7072 6f76 6964 6573 2061  or it provides a
-000005b0: 6674 6572 2064 6570 6c6f 796d 656e 742e  fter deployment.
-000005c0: 0a0a 2323 2055 7365 2043 6173 6573 0a0a  ..## Use Cases..
-000005d0: 2d20 5b49 662e 2e2e 5468 656e 2043 6f6e  - [If...Then Con
-000005e0: 6469 7469 6f6e 616c 7320 616e 6420 4c6f  ditionals and Lo
-000005f0: 6f70 696e 675d 282f 4558 414d 504c 4553  oping](/EXAMPLES
-00000600: 2e6d 6423 6966 7468 656e 2d63 6f6e 6469  .md#ifthen-condi
-00000610: 7469 6f6e 616c 732d 616e 642d 6c6f 6f70  tionals-and-loop
-00000620: 696e 6729 0a2d 205b 4375 7374 6f6d 2046  ing).- [Custom F
-00000630: 756e 6374 696f 6e73 5d28 2f45 5841 4d50  unctions](/EXAMP
-00000640: 4c45 532e 6d64 2363 7573 746f 6d2d 6675  LES.md#custom-fu
-00000650: 6e63 7469 6f6e 7329 0a2d 205b 5765 6220  nctions).- [Web 
-00000660: 5363 7261 7065 7273 5d28 2f45 5841 4d50  Scrapers](/EXAMP
-00000670: 4c45 532e 6d64 2377 6562 2d73 6372 6170  LES.md#web-scrap
-00000680: 6572 7329 0a2d 205b 5265 7065 6174 696e  ers).- [Repeatin
-00000690: 6720 576f 726b 666c 6f77 735d 282f 4558  g Workflows](/EX
-000006a0: 414d 504c 4553 2e6d 6423 7265 7065 6174  AMPLES.md#repeat
-000006b0: 696e 672d 776f 726b 666c 6f77 7329 0a2d  ing-workflows).-
-000006c0: 205b 4375 7374 6f6d 2044 6173 6862 6f61   [Custom Dashboa
-000006d0: 7264 735d 282f 4558 414d 504c 4553 2e6d  rds](/EXAMPLES.m
-000006e0: 6423 6375 7374 6f6d 2d64 6173 6862 6f61  d#custom-dashboa
-000006f0: 7264 7329 0a2d 205b 4461 7461 2054 7261  rds).- [Data Tra
-00000700: 6e73 666f 726d 6174 696f 6e5d 282f 4558  nsformation](/EX
-00000710: 414d 504c 4553 2e6d 6423 6461 7461 2d74  AMPLES.md#data-t
-00000720: 7261 6e73 666f 726d 6174 696f 6e29 0a2d  ransformation).-
-00000730: 205b 506c 6174 666f 726d 2042 6f74 735d   [Platform Bots]
-00000740: 282f 4558 414d 504c 4553 2e6d 6423 706c  (/EXAMPLES.md#pl
-00000750: 6174 666f 726d 2d62 6f74 7329 0a2d 205b  atform-bots).- [
-00000760: 4275 7369 6e65 7373 2050 726f 6365 7373  Business Process
-00000770: 6573 5d28 2f45 5841 4d50 4c45 532e 6d64  es](/EXAMPLES.md
-00000780: 2362 7573 696e 6573 732d 7072 6f63 6573  #business-proces
-00000790: 7365 7329 0a2d 205b 4c6f 6e67 2d74 6572  ses).- [Long-ter
-000007a0: 6d20 6d65 6d6f 7279 5d28 2f45 5841 4d50  m memory](/EXAMP
-000007b0: 4c45 532e 6d64 236c 6f6e 672d 7465 726d  LES.md#long-term
-000007c0: 2d6d 656d 6f72 7929 0a2d 205b 4469 7669  -memory).- [Divi
-000007d0: 7369 6f6e 206f 6620 6c61 626f 7572 5d28  sion of labour](
-000007e0: 2f45 5841 4d50 4c45 532e 6d64 2364 6976  /EXAMPLES.md#div
-000007f0: 6973 696f 6e2d 6f66 2d6c 6162 6f75 7229  ision-of-labour)
-00000800: 0a20 202d 205b 5061 7261 6c6c 656c 697a  .  - [Paralleliz
-00000810: 6174 696f 6e5d 282f 4558 414d 504c 4553  ation](/EXAMPLES
-00000820: 2e6d 6423 7061 7261 6c6c 656c 697a 6174  .md#parallelizat
-00000830: 696f 6e29 0a20 202d 205b 436f 6e63 7572  ion).  - [Concur
-00000840: 7265 6e63 795d 282f 4558 414d 504c 4553  rency](/EXAMPLES
-00000850: 2e6d 6423 636f 6e63 7572 7265 6e63 7929  .md#concurrency)
-00000860: 0a0a 2323 2043 6f6d 6d61 6e64 204c 696e  ..## Command Lin
-00000870: 6520 5573 6167 650a 0a54 6f64 6179 2c20  e Usage..Today, 
-00000880: 7363 7269 7074 206e 6565 6420 746f 2062  script need to b
-00000890: 6520 6d61 6e75 616c 6c79 2077 7269 7474  e manually writt
-000008a0: 656e 2073 7465 702d 6279 2d73 7465 702c  en step-by-step,
-000008b0: 2062 7574 2077 6520 6172 6520 6f66 6665   but we are offe
-000008c0: 7269 6e67 2065 6172 6c79 2057 4950 2070  ring early WIP p
-000008d0: 7265 7669 6577 206f 6620 6974 6572 6174  review of iterat
-000008e0: 6976 6520 7363 7269 7074 2067 656e 6572  ive script gener
-000008f0: 6174 696f 6e20 7669 6120 6f75 7220 434c  ation via our CL
-00000900: 492e 2054 7279 2072 756e 6e69 6e67 3a0a  I. Try running:.
-00000910: 0a60 6060 0a24 206d 6179 616c 6162 7320  .```.$ mayalabs 
-00000920: 696e 7374 7275 6374 202d 6320 2766 6574  instruct -c 'fet
-00000930: 6368 204e 616d 6520 616e 6420 456d 6169  ch Name and Emai
-00000940: 6c20 6672 6f6d 2067 7368 6565 742c 2077  l from gsheet, w
-00000950: 7269 7465 2066 756e 6374 696f 6e20 746f  rite function to
-00000960: 206d 6572 6765 2061 6c6c 2063 6f6c 756d   merge all colum
-00000970: 6e73 2c20 616e 6420 7265 7475 726e 2064  ns, and return d
-00000980: 6174 6127 0a60 6060 0a0a 416e 6420 7468  ata'.```..And th
-00000990: 656e 2075 7365 2074 6865 2067 656e 6572  en use the gener
-000009a0: 6174 6564 2073 6372 6970 7420 6173 2066  ated script as f
-000009b0: 756e 6374 696f 6e2e 0a0a 6874 7470 733a  unction...https:
-000009c0: 2f2f 7573 6572 2d69 6d61 6765 732e 6769  //user-images.gi
-000009d0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-000009e0: 636f 6d2f 3532 3439 3330 3737 2f32 3331  com/52493077/231
-000009f0: 3937 3932 3834 2d61 3764 3163 3433 642d  979284-a7d1c43d-
-00000a00: 6636 6336 2d34 3732 362d 3839 6665 2d32  f6c6-4726-89fe-2
-00000a10: 3865 3130 3363 6431 3938 662e 6d70 340a  8e103cd198f.mp4.
-00000a20: 0a23 2320 5265 7175 6972 656d 656e 7473  .## Requirements
-00000a30: 0a0a 2d20 5079 7468 6f6e 2033 2e37 2e31  ..- Python 3.7.1
-00000a40: 2b0a 0a23 2320 4973 7375 6573 0a0a 416c  +..## Issues..Al
-00000a50: 6c20 6665 6564 6261 636b 2061 6e64 2062  l feedback and b
-00000a60: 7567 2072 6570 6f72 7473 2077 656c 636f  ug reports welco
-00000a70: 6d65 2120 5265 706f 7274 2069 6e20 7468  me! Report in th
-00000a80: 6520 5b69 7373 7565 7320 7365 6374 696f  e [issues sectio
-00000a90: 6e5d 2868 7474 7073 3a2f 2f67 6974 6875  n](https://githu
-00000aa0: 622e 636f 6d2f 6d61 7961 6871 2f6d 6179  b.com/mayahq/may
-00000ab0: 616c 6162 732d 7364 6b2d 7079 7468 6f6e  alabs-sdk-python
-00000ac0: 2f69 7373 7565 7329 2c20 6f72 206d 6169  /issues), or mai
-00000ad0: 6c20 7573 2061 7420 6875 6d61 6e73 406d  l us at humans@m
-00000ae0: 6179 616c 6162 732e 696f 2e0a 0a46 756c  ayalabs.io...Ful
-00000af0: 6c20 6c69 7374 206f 6620 6361 7061 6269  l list of capabi
-00000b00: 6c69 7469 6573 2061 6e64 206c 696d 6974  lities and limit
-00000b10: 7320 5b68 6572 655d 2868 7474 7073 3a2f  s [here](https:/
-00000b20: 2f64 6f63 732e 6d61 7961 6c61 6273 2e69  /docs.mayalabs.i
-00000b30: 6f2f 6361 7061 6269 6c69 7469 6573 2d61  o/capabilities-a
-00000b40: 6e64 2d6c 696d 6974 7329 2e0a 0a0a 2323  nd-limits)....##
-00000b50: 2052 6f61 646d 6170 0a2d 205b 785d 2043   Roadmap.- [x] C
-00000b60: 6c65 616e 6572 206c 6f67 7320 616e 6420  leaner logs and 
-00000b70: 6578 6365 7074 696f 6e20 6861 6e64 6c69  exception handli
-00000b80: 6e67 0a2d 205b 205d 2044 6570 656e 6465  ng.- [ ] Depende
-00000b90: 6e63 7920 636f 6e66 6967 7572 6174 696f  ncy configuratio
-00000ba0: 6e20 5558 2069 6d70 726f 7665 6d65 6e74  n UX improvement
-00000bb0: 0a2d 205b 205d 2049 6d70 6f72 7420 736b  .- [ ] Import sk
-00000bc0: 696c 6c20 7265 706f 7369 746f 7269 6573  ill repositories
-00000bd0: 2066 6f72 2072 6575 7369 6e67 2073 6b69   for reusing ski
-00000be0: 6c6c 7320 6372 6561 7465 6420 6279 2075  lls created by u
-00000bf0: 7365 7220 6f72 2070 7265 7365 6e74 2069  ser or present i
-00000c00: 6e20 7374 6f72 650a 2d20 5b20 5d20 4372  n store.- [ ] Cr
-00000c10: 6561 7465 2061 6e64 2063 616c 6c20 646f  eate and call do
-00000c20: 776e 7374 7265 616d 2061 7574 6f2d 6465  wnstream auto-de
-00000c30: 706c 6f79 6564 2066 756e 6374 696f 6e73  ployed functions
-00000c40: 0a2d 205b 205d 2041 6c6c 6f77 206d 756c  .- [ ] Allow mul
-00000c50: 7469 2d70 726f 6669 6c65 2061 6e64 2074  ti-profile and t
-00000c60: 6561 6d20 7072 6f66 696c 6520 6163 6365  eam profile acce
-00000c70: 7373 0a                                  ss.
+00000030: 6775 6167 652e 0a0a 3c70 2061 6c69 676e  guage...<p align
+00000040: 3d22 6c65 6674 223e 0a20 203c 6120 6872  ="left">.  <a hr
+00000050: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+00000060: 2e6f 7267 2f70 726f 6a65 6374 2f6d 6179  .org/project/may
+00000070: 616c 6162 7322 3e0a 2020 2020 3c69 6d67  alabs">.    <img
+00000080: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000090: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+000000a0: 692f 762f 6d61 7961 6c61 6273 3f73 7479  i/v/mayalabs?sty
+000000b0: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+000000c0: 2220 2f3e 0a20 203c 2f61 3e0a 2020 3c61  " />.  </a>.  <a
+000000d0: 2068 7265 663d 2268 7474 7073 3a2f 2f6d   href="https://m
+000000e0: 6179 616c 6162 732e 696f 2f64 6f63 7322  ayalabs.io/docs"
+000000f0: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+00000100: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000110: 6c64 732e 696f 2f62 6164 6765 2f44 6f63  lds.io/badge/Doc
+00000120: 756d 656e 7461 7469 6f6e 2d62 6c75 653f  umentation-blue?
+00000130: 6c6f 676f 3d47 6974 426f 6f6b 266c 6f67  logo=GitBook&log
+00000140: 6f43 6f6c 6f72 3d77 6869 7465 2673 7479  oColor=white&sty
+00000150: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+00000160: 2220 2f3e 0a20 203c 2f61 3e0a 3c2f 703e  " />.  </a>.</p>
+00000170: 0a3c 6272 3e0a 0a54 6865 204d 6179 6120  .<br>..The Maya 
+00000180: 4c61 6273 2050 7974 686f 6e20 5344 4b20  Labs Python SDK 
+00000190: 7072 6f76 6964 6573 2065 6173 7920 6173  provides easy as
+000001a0: 796e 6320 6163 6365 7373 2074 6f20 6f75  ync access to ou
+000001b0: 7220 5041 432d 3120 7072 6f67 7261 6d20  r PAC-1 program 
+000001c0: 7379 6e74 6865 7369 7320 656e 6769 6e65  synthesis engine
+000001d0: 2c20 7769 7468 2061 2043 4c49 2074 6f20  , with a CLI to 
+000001e0: 696e 7374 7275 6374 2061 6e64 2067 656e  instruct and gen
+000001f0: 6572 6174 6520 7072 6f67 7261 6d73 2066  erate programs f
+00000200: 726f 6d20 696e 7374 7275 6374 696f 6e73  rom instructions
+00000210: 2069 6e20 6e61 7475 7261 6c20 6c61 6e67   in natural lang
+00000220: 7561 6765 2e0a 0a23 2320 496e 7374 616c  uage...## Instal
+00000230: 6c61 7469 6f6e 0a0a 6060 600a 7069 7020  lation..```.pip 
+00000240: 696e 7374 616c 6c20 2d2d 7570 6772 6164  install --upgrad
+00000250: 6520 6d61 7961 6c61 6273 0a60 6060 0a23  e mayalabs.```.#
+00000260: 2320 5072 6576 6965 770a 0a68 7474 7073  # Preview..https
+00000270: 3a2f 2f75 7365 722d 696d 6167 6573 2e67  ://user-images.g
+00000280: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000290: 2e63 6f6d 2f38 3733 3637 3937 2f32 3330  .com/8736797/230
+000002a0: 3934 3734 3430 2d32 3430 3337 3632 642d  947440-2403762d-
+000002b0: 6131 3462 2d34 6230 302d 3866 6265 2d62  a14b-4b00-8fbe-b
+000002c0: 6438 3033 6162 3234 3032 382e 6d70 340a  d803ab24028.mp4.
+000002d0: 0a0a 2323 2055 7361 6765 0a0a 4765 7420  ..## Usage..Get 
+000002e0: 7468 6520 4d61 7961 204c 6162 7320 4150  the Maya Labs AP
+000002f0: 4920 6b65 7920 6672 6f6d 2074 6865 2053  I key from the S
+00000300: 6574 7469 6e67 7320 3e20 4465 7665 6c6f  ettings > Develo
+00000310: 7065 7220 5b73 6563 7469 6f6e 5d28 6874  per [section](ht
+00000320: 7470 733a 2f2f 6170 702e 6d61 7961 6c61  tps://app.mayala
+00000330: 6273 2e69 6f2f 7365 7474 696e 6773 2f64  bs.io/settings/d
+00000340: 6576 656c 6f70 6572 7329 2e0a 0a60 6060  evelopers)...```
+00000350: 0a65 7870 6f72 7420 4d41 5941 5f41 5049  .export MAYA_API
+00000360: 5f4b 4559 203d 2022 6d61 7961 6b65 792d  _KEY = "mayakey-
+00000370: 2e2e 2e22 0a60 6060 0a0a 4f72 2073 6574  ...".```..Or set
+00000380: 2060 6d61 7961 6c61 6273 2e61 7069 5f6b   `mayalabs.api_k
+00000390: 6579 6020 746f 2069 7473 2076 616c 7565  ey` to its value
+000003a0: 3a0a 0a60 6060 0a69 6d70 6f72 7420 6d61  :..```.import ma
+000003b0: 7961 6c61 6273 0a0a 6d61 7961 6c61 6273  yalabs..mayalabs
+000003c0: 2e61 7069 5f6b 6579 203d 2022 6d61 7961  .api_key = "maya
+000003d0: 6b65 792d 2e2e 2e22 0a0a 7363 7269 7074  key-..."..script
+000003e0: 203d 2022 2222 0a31 2e20 7472 6967 6765   = """.1. trigge
+000003f0: 7220 6f6e 2072 6563 6569 7665 0a32 2e20  r on receive.2. 
+00000400: 7265 7365 6172 6368 207b 7b74 6572 6d7d  research {{term}
+00000410: 7d20 6f6e 2077 696b 6970 6564 6961 0a33  } on wikipedia.3
+00000420: 2e20 6578 7472 6163 7420 2774 6974 6c65  . extract 'title
+00000430: 2720 616e 6420 2773 756d 6d61 7279 2720  ' and 'summary' 
+00000440: 6672 6f6d 2074 6162 756c 6172 2064 6174  from tabular dat
+00000450: 610a 342e 2073 656e 6420 7265 7370 6f6e  a.4. send respon
+00000460: 7365 2062 6163 6b0a 2222 220a 0a66 756e  se back."""..fun
+00000470: 6374 696f 6e20 3d20 6d61 7961 6c61 6273  ction = mayalabs
+00000480: 2e46 756e 6374 696f 6e28 6e61 6d65 3d22  .Function(name="
+00000490: 5363 7261 7065 3222 290a 2320 4372 6561  Scrape2").# Crea
+000004a0: 7469 6e67 206e 6577 2077 6f72 6b65 722e  ting new worker.
+000004b0: 2e2e 0a0a 6675 6e63 7469 6f6e 2e75 7064  ....function.upd
+000004c0: 6174 6528 7363 7269 7074 3d73 6372 6970  ate(script=scrip
+000004d0: 7429 0a23 2047 656e 6572 6174 696e 6720  t).# Generating 
+000004e0: 7072 6f67 7261 6d20 6772 6170 682e 2e2e  program graph...
+000004f0: 0a23 2053 7461 7274 696e 6720 776f 726b  .# Starting work
+00000500: 6572 2e2e 2e0a 2320 496e 7374 616c 6c69  er....# Installi
+00000510: 6e67 2064 6570 656e 6465 6e63 6965 732e  ng dependencies.
+00000520: 2e2e 0a23 2044 6570 6c6f 7965 6421 0a0a  ...# Deployed!..
+00000530: 6f75 7470 7574 203d 2066 756e 6374 696f  output = functio
+00000540: 6e2e 6361 6c6c 287b 2274 6572 6d22 3a20  n.call({"term": 
+00000550: 2244 722e 2056 696b 7261 6d20 5361 7261  "Dr. Vikram Sara
+00000560: 6268 6169 227d 290a 7072 696e 7428 6f75  bhai"}).print(ou
+00000570: 7470 7574 290a 2320 6669 6e64 7320 616e  tput).# finds an
+00000580: 6420 6f75 7470 7574 7320 7469 746c 6520  d outputs title 
+00000590: 616e 6420 7375 6d6d 6172 7920 6672 6f6d  and summary from
+000005a0: 2077 696b 6970 6564 6961 2072 6573 756c   wikipedia resul
+000005b0: 7473 0a0a 6060 600a 0a50 4143 2d31 2074  ts..```..PAC-1 t
+000005c0: 616b 6573 2069 6e20 7374 6570 7320 7772  akes in steps wr
+000005d0: 6974 7465 6e20 696e 2045 6e67 6c69 7368  itten in English
+000005e0: 2c20 7772 6974 6573 2026 2061 7373 656d  , writes & assem
+000005f0: 626c 6573 2061 2064 6973 6372 6574 6520  bles a discrete 
+00000600: 7072 6f67 7261 6d20 6772 6170 682c 2061  program graph, a
+00000610: 6e64 2064 6570 6c6f 7973 2072 6561 6479  nd deploys ready
+00000620: 2d74 6f2d 7573 6520 736f 6674 7761 7265  -to-use software
+00000630: 206f 6e20 6f75 7220 636f 6d70 7574 6520   on our compute 
+00000640: 696e 6672 6173 7472 7563 7475 7265 2c20  infrastructure, 
+00000650: 7468 6174 2079 6f75 2063 616e 2063 616c  that you can cal
+00000660: 6c20 7769 7468 696e 2079 6f75 7220 636f  l within your co
+00000670: 6465 2e20 596f 7520 6361 6e20 7365 7420  de. You can set 
+00000680: 7570 206d 6973 7369 6e67 2064 6570 656e  up missing depen
+00000690: 6465 6e63 6965 7320 2f20 7669 7375 616c  dencies / visual
+000006a0: 697a 6520 7468 6520 666c 6f77 206f 6620  ize the flow of 
+000006b0: 6c6f 6769 6320 6279 2066 6f6c 6c6f 7769  logic by followi
+000006c0: 6e67 2074 6865 206c 696e 6b20 746f 2066  ng the link to f
+000006d0: 6c6f 772d 6261 7365 6420 6564 6974 6f72  low-based editor
+000006e0: 2069 7420 7072 6f76 6964 6573 2061 6674   it provides aft
+000006f0: 6572 2064 6570 6c6f 796d 656e 742e 0a0a  er deployment...
+00000700: 4368 6563 6b20 6f75 7220 5b64 6f63 756d  Check our [docum
+00000710: 656e 7461 7469 6f6e 5d28 2268 7474 7073  entation]("https
+00000720: 3a2f 2f6d 6179 616c 6162 732e 696f 2f64  ://mayalabs.io/d
+00000730: 6f63 7322 2920 666f 7220 6d6f 7265 2075  ocs") for more u
+00000740: 7361 6765 2061 6e64 2074 7574 6f72 6961  sage and tutoria
+00000750: 6c73 2e0a 0a23 2320 5573 6520 4361 7365  ls...## Use Case
+00000760: 730a 0a2d 205b 4966 2e2e 2e54 6865 6e20  s..- [If...Then 
+00000770: 436f 6e64 6974 696f 6e61 6c73 2061 6e64  Conditionals and
+00000780: 204c 6f6f 7069 6e67 5d28 2f45 5841 4d50   Looping](/EXAMP
+00000790: 4c45 532e 6d64 2369 6674 6865 6e2d 636f  LES.md#ifthen-co
+000007a0: 6e64 6974 696f 6e61 6c73 2d61 6e64 2d6c  nditionals-and-l
+000007b0: 6f6f 7069 6e67 290a 2d20 5b43 7573 746f  ooping).- [Custo
+000007c0: 6d20 4675 6e63 7469 6f6e 735d 282f 4558  m Functions](/EX
+000007d0: 414d 504c 4553 2e6d 6423 6375 7374 6f6d  AMPLES.md#custom
+000007e0: 2d66 756e 6374 696f 6e73 290a 2d20 5b57  -functions).- [W
+000007f0: 6562 2053 6372 6170 6572 735d 282f 4558  eb Scrapers](/EX
+00000800: 414d 504c 4553 2e6d 6423 7765 622d 7363  AMPLES.md#web-sc
+00000810: 7261 7065 7273 290a 2d20 5b52 6570 6561  rapers).- [Repea
+00000820: 7469 6e67 2057 6f72 6b66 6c6f 7773 5d28  ting Workflows](
+00000830: 2f45 5841 4d50 4c45 532e 6d64 2372 6570  /EXAMPLES.md#rep
+00000840: 6561 7469 6e67 2d77 6f72 6b66 6c6f 7773  eating-workflows
+00000850: 290a 2d20 5b43 7573 746f 6d20 4461 7368  ).- [Custom Dash
+00000860: 626f 6172 6473 5d28 2f45 5841 4d50 4c45  boards](/EXAMPLE
+00000870: 532e 6d64 2363 7573 746f 6d2d 6461 7368  S.md#custom-dash
+00000880: 626f 6172 6473 290a 2d20 5b44 6174 6120  boards).- [Data 
+00000890: 5472 616e 7366 6f72 6d61 7469 6f6e 5d28  Transformation](
+000008a0: 2f45 5841 4d50 4c45 532e 6d64 2364 6174  /EXAMPLES.md#dat
+000008b0: 612d 7472 616e 7366 6f72 6d61 7469 6f6e  a-transformation
+000008c0: 290a 2d20 5b50 6c61 7466 6f72 6d20 426f  ).- [Platform Bo
+000008d0: 7473 5d28 2f45 5841 4d50 4c45 532e 6d64  ts](/EXAMPLES.md
+000008e0: 2370 6c61 7466 6f72 6d2d 626f 7473 290a  #platform-bots).
+000008f0: 2d20 5b42 7573 696e 6573 7320 5072 6f63  - [Business Proc
+00000900: 6573 7365 735d 282f 4558 414d 504c 4553  esses](/EXAMPLES
+00000910: 2e6d 6423 6275 7369 6e65 7373 2d70 726f  .md#business-pro
+00000920: 6365 7373 6573 290a 2d20 5b4c 6f6e 672d  cesses).- [Long-
+00000930: 7465 726d 206d 656d 6f72 795d 282f 4558  term memory](/EX
+00000940: 414d 504c 4553 2e6d 6423 6c6f 6e67 2d74  AMPLES.md#long-t
+00000950: 6572 6d2d 6d65 6d6f 7279 290a 2d20 5b44  erm-memory).- [D
+00000960: 6976 6973 696f 6e20 6f66 206c 6162 6f75  ivision of labou
+00000970: 725d 282f 4558 414d 504c 4553 2e6d 6423  r](/EXAMPLES.md#
+00000980: 6469 7669 7369 6f6e 2d6f 662d 6c61 626f  division-of-labo
+00000990: 7572 290a 2020 2d20 5b50 6172 616c 6c65  ur).  - [Paralle
+000009a0: 6c69 7a61 7469 6f6e 5d28 2f45 5841 4d50  lization](/EXAMP
+000009b0: 4c45 532e 6d64 2370 6172 616c 6c65 6c69  LES.md#paralleli
+000009c0: 7a61 7469 6f6e 290a 2020 2d20 5b43 6f6e  zation).  - [Con
+000009d0: 6375 7272 656e 6379 5d28 2f45 5841 4d50  currency](/EXAMP
+000009e0: 4c45 532e 6d64 2363 6f6e 6375 7272 656e  LES.md#concurren
+000009f0: 6379 290a 0a23 2320 436f 6d6d 616e 6420  cy)..## Command 
+00000a00: 4c69 6e65 2055 7361 6765 0a0a 546f 6461  Line Usage..Toda
+00000a10: 792c 2073 6372 6970 7420 6e65 6564 2074  y, script need t
+00000a20: 6f20 6265 206d 616e 7561 6c6c 7920 7772  o be manually wr
+00000a30: 6974 7465 6e20 7374 6570 2d62 792d 7374  itten step-by-st
+00000a40: 6570 2c20 6275 7420 7765 2061 7265 206f  ep, but we are o
+00000a50: 6666 6572 696e 6720 6561 726c 7920 5749  ffering early WI
+00000a60: 5020 7072 6576 6965 7720 6f66 2069 7465  P preview of ite
+00000a70: 7261 7469 7665 2073 6372 6970 7420 6765  rative script ge
+00000a80: 6e65 7261 7469 6f6e 2076 6961 206f 7572  neration via our
+00000a90: 2043 4c49 2e20 5472 7920 7275 6e6e 696e   CLI. Try runnin
+00000aa0: 673a 0a0a 6060 600a 2420 6d61 7961 6c61  g:..```.$ mayala
+00000ab0: 6273 2069 6e73 7472 7563 7420 2d63 2027  bs instruct -c '
+00000ac0: 6665 7463 6820 4e61 6d65 2061 6e64 2045  fetch Name and E
+00000ad0: 6d61 696c 2066 726f 6d20 6773 6865 6574  mail from gsheet
+00000ae0: 2c20 7772 6974 6520 6675 6e63 7469 6f6e  , write function
+00000af0: 2074 6f20 6d65 7267 6520 616c 6c20 636f   to merge all co
+00000b00: 6c75 6d6e 732c 2061 6e64 2072 6574 7572  lumns, and retur
+00000b10: 6e20 6461 7461 270a 6060 600a 0a41 6e64  n data'.```..And
+00000b20: 2074 6865 6e20 7573 6520 7468 6520 6765   then use the ge
+00000b30: 6e65 7261 7465 6420 7363 7269 7074 2061  nerated script a
+00000b40: 7320 6675 6e63 7469 6f6e 2e0a 0a68 7474  s function...htt
+00000b50: 7073 3a2f 2f75 7365 722d 696d 6167 6573  ps://user-images
+00000b60: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000b70: 6e74 2e63 6f6d 2f35 3234 3933 3037 372f  nt.com/52493077/
+00000b80: 3233 3139 3739 3238 342d 6137 6431 6334  231979284-a7d1c4
+00000b90: 3364 2d66 3663 362d 3437 3236 2d38 3966  3d-f6c6-4726-89f
+00000ba0: 652d 3238 6531 3033 6364 3139 3866 2e6d  e-28e103cd198f.m
+00000bb0: 7034 0a0a 2323 2052 6571 7569 7265 6d65  p4..## Requireme
+00000bc0: 6e74 730a 0a2d 2050 7974 686f 6e20 332e  nts..- Python 3.
+00000bd0: 372e 312b 0a0a 2323 2049 7373 7565 730a  7.1+..## Issues.
+00000be0: 0a41 6c6c 2066 6565 6462 6163 6b20 616e  .All feedback an
+00000bf0: 6420 6275 6720 7265 706f 7274 7320 7765  d bug reports we
+00000c00: 6c63 6f6d 6521 2052 6570 6f72 7420 696e  lcome! Report in
+00000c10: 2074 6865 205b 6973 7375 6573 2073 6563   the [issues sec
+00000c20: 7469 6f6e 5d28 6874 7470 733a 2f2f 6769  tion](https://gi
+00000c30: 7468 7562 2e63 6f6d 2f6d 6179 6168 712f  thub.com/mayahq/
+00000c40: 6d61 7961 6c61 6273 2d73 646b 2d70 7974  mayalabs-sdk-pyt
+00000c50: 686f 6e2f 6973 7375 6573 292c 206f 7220  hon/issues), or 
+00000c60: 6d61 696c 2075 7320 6174 2068 756d 616e  mail us at human
+00000c70: 7340 6d61 7961 6c61 6273 2e69 6f2e 0a0a  s@mayalabs.io...
+00000c80: 4675 6c6c 206c 6973 7420 6f66 2063 6170  Full list of cap
+00000c90: 6162 696c 6974 6965 7320 616e 6420 6c69  abilities and li
+00000ca0: 6d69 7473 205b 6865 7265 5d28 6874 7470  mits [here](http
+00000cb0: 733a 2f2f 646f 6373 2e6d 6179 616c 6162  s://docs.mayalab
+00000cc0: 732e 696f 2f63 6170 6162 696c 6974 6965  s.io/capabilitie
+00000cd0: 732d 616e 642d 6c69 6d69 7473 292e 0a0a  s-and-limits)...
+00000ce0: 0a23 2320 526f 6164 6d61 700a 2d20 5b78  .## Roadmap.- [x
+00000cf0: 5d20 436c 6561 6e65 7220 6c6f 6773 2061  ] Cleaner logs a
+00000d00: 6e64 2065 7863 6570 7469 6f6e 2068 616e  nd exception han
+00000d10: 646c 696e 670a 2d20 5b78 5d20 4465 7065  dling.- [x] Depe
+00000d20: 6e64 656e 6379 2063 6f6e 6669 6775 7261  ndency configura
+00000d30: 7469 6f6e 2055 5820 696d 7072 6f76 656d  tion UX improvem
+00000d40: 656e 740a 2d20 5b20 5d20 496d 706f 7274  ent.- [ ] Import
+00000d50: 2073 6b69 6c6c 2072 6570 6f73 6974 6f72   skill repositor
+00000d60: 6965 7320 666f 7220 7265 7573 696e 6720  ies for reusing 
+00000d70: 736b 696c 6c73 2063 7265 6174 6564 2062  skills created b
+00000d80: 7920 7573 6572 206f 7220 7072 6573 656e  y user or presen
+00000d90: 7420 696e 2073 746f 7265 0a2d 205b 205d  t in store.- [ ]
+00000da0: 2043 7265 6174 6520 616e 6420 6361 6c6c   Create and call
+00000db0: 2064 6f77 6e73 7472 6561 6d20 6175 746f   downstream auto
+00000dc0: 2d64 6570 6c6f 7965 6420 6675 6e63 7469  -deployed functi
+00000dd0: 6f6e 730a 2d20 5b20 5d20 416c 6c6f 7720  ons.- [ ] Allow 
+00000de0: 6d75 6c74 692d 7072 6f66 696c 6520 616e  multi-profile an
+00000df0: 6420 7465 616d 2070 726f 6669 6c65 2061  d team profile a
+00000e00: 6363 6573 730a                           ccess.
```

### Comparing `mayalabs-0.0.8/examples/add_to_google_sheet.py` & `mayalabs-0.0.9/examples/add_to_google_sheet.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.8/examples/native_memory.py` & `mayalabs-0.0.9/examples/native_memory.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.8/examples/web_scraping.py` & `mayalabs-0.0.9/examples/web_scraping.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.8/mayalabs/cli.py` & `mayalabs-0.0.9/mayalabs/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import json
+import shutil
 import time
 import argparse
 import getpass
 import requests
 from colorama import Fore, Style
 import mayalabs
 from .session import Session
@@ -129,16 +130,16 @@
     while True:
         menu_entry_index = terminal_menu.show()
         choice = str(menu_entry_index + 1)
 
         if choice == "1":
             print(Style.BRIGHT + Fore.CYAN + 'Deploying as function...\n' + Style.RESET_ALL)
             random_name = "SDK:" + get_random_name()
-            function = Function.create(name=random_name, script=recipe)
-            function.deploy()
+            function = Function(name=random_name)
+            function.update(script=recipe)
             exit()
         elif choice == "2":
             new_command = input(Style.BRIGHT + Fore.BLUE + 'How do you want to modify this program? ' + Style.RESET_ALL)
             instruct(command=new_command, from_scratch=False, session_id=session_id)
             break
         elif choice == "3":
             with open("output.nl", "w", encoding='utf-8') as output_file:
@@ -194,27 +195,19 @@
     """
     return string.replace("(*)", "").strip()
 
 def print_user_command(command):
     """
     Prints the command entered by the user in a box.
     """
-    box_height = 2
+    max_width = shutil.get_terminal_size().columns
+
+    command_lines = [command[i:i+max_width-8] for i in range(0, len(command), max_width-8)]
+
     header = ' Instruction '
     header_len = len(header)
-    box_width = len(command) + 4
-
-    # Calculate the number of blank lines above and below the command
-    remaining_height = box_height - 2
-    top_lines = remaining_height // 2
-    bottom_lines = remaining_height - top_lines
+    box_width = max(len(line) for line in command_lines) + 4
 
     print("╭" + "─" + header + "─" * (box_width - header_len - 1) + "╮")
-    for i in range(top_lines):
-        print("│  " + " " * (box_width - 4) + "  │")
-    print("│  " + command.center(box_width - 4) + "  │")
-    for i in range(bottom_lines):
-        print("│  " + " " * (box_width - 4) + "  │")
+    for line in command_lines:
+        print("│  " + line.ljust(box_width - 4) + "  │")
     print("╰" + "─" * box_width + "╯")
-
-
-
```

### Comparing `mayalabs-0.0.8/mayalabs/mayalabs.py` & `mayalabs-0.0.9/mayalabs/mayalabs.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.8/mayalabs/session.py` & `mayalabs-0.0.9/mayalabs/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,14 +97,31 @@
             }
         }
         response = requests.request(**request)
         return response.json()
     
     @staticmethod
     @authenticate
+    def reset_session(session_id, api_key=None):
+        api_base = default_api_base_url()
+        request = {
+            'url': f"{api_base}/pac/v1/session/clear",
+            'method': "post",
+            'json': {
+                'session_id': session_id
+            },
+            'headers': {
+                'x-api-key': api_key,
+            }
+        }
+        response = requests.request(**request)
+        return response.json()
+    
+    @staticmethod
+    @authenticate
     def change_session(session_id, script, api_key=None):
         api_base = default_api_base_url()
         request = {
             'url': f"{api_base}/pac/v1/session/change",
             'method': "post",
             'json': {
                 "session_id": session_id,
@@ -115,15 +132,15 @@
             'headers': {
                 'x-api-key': api_key,
             }
         }
         response = requests.request(**request)
         if response.status_code == 200:
             change_response = response.json()
-            change_status = change_response['response'].get('change_status', {}).get('is_changed', False)
+            change_status = change_response.get('change_status', {}).get('is_changed', False)
             return change_status
         else:
             raise HTTPError("Failed to update script")
 
     @authenticate
     async def deploy_session(session_id, workspace_id, api_key=None):
         data = {
@@ -189,30 +206,30 @@
 
     def check_worker_start(self):
         status = 0
         i = 0
         if (self.worker.status and self.worker.status != 'STARTED'):
             status = Fore.RED + 'PENDING' + Style.RESET_ALL
             log(
-                "Worker status:", status,
+                Style.BRIGHT + Fore.CYAN + "Worker status:", status,
                 prefix='mayalabs',
                 prefix_color=Fore.BLACK
             )
 
         while self.worker.status and self.worker.status != "STARTED":
             i += 1
             # self.worker.update()
             worker_response = WorkerClient.get_worker(self.worker.id)
             if worker_response['results']:
                 self.worker = Worker().parse_obj(worker_response['results'])
             time.sleep(2)
 
         started_status = Fore.GREEN + 'STARTED' + Style.RESET_ALL
         log(
-            'Worker status:', started_status,
+            Style.BRIGHT + Fore.CYAN + 'Worker status:', started_status,
             prefix='mayalabs',
             prefix_color=Fore.BLACK
         )
         return
 
     def _deploy(self, worker_id=None, update=False):
         # Implement this method
@@ -223,27 +240,27 @@
             result = loop.run_until_complete(coroutine)
             loop.close()
             return result
         
         if worker_id is not None:
             try:
                 self.worker = Worker.get_by_id(worker_id)
-                log("Found worker: ", self.worker.name, prefix='mayalabs')
+                log(Style.BRIGHT + Fore.CYAN + "Found worker: ", self.worker.name, prefix='mayalabs')
             except:
                 raise Exception("Worker not found")
         elif self.worker is None:
-            log("No worker found, creating new worker...", prefix='mayalabs')
+            log(Style.BRIGHT + Fore.CYAN + "No worker found, creating new worker...", prefix='mayalabs')
             random_name = "SDK:" + get_random_name()
             self.worker = WorkerClient.create_worker(worker_name=random_name, alias=random_name)
         else:
             raise Exception("Error: Could not find worker")
         
         if self.worker:
             if self.worker.status != "STARTED":
-                log("Starting worker: ", self.worker.name, prefix='mayalabs')
+                log(Style.BRIGHT + Fore.CYAN + "Starting worker: ", self.worker.name, prefix='mayalabs')
                 self.worker.start()
             with concurrent.futures.ThreadPoolExecutor() as exec:
                 result_2 = exec.submit(self.check_worker_start)
                 if (self.changed or self.changed is None):
                     if self.changed:
                         log(Style.BRIGHT + Fore.CYAN + 'Script change detected. Regenerating changes...' + Style.RESET_ALL, prefix='mayalabs')
                     else:
@@ -278,17 +295,37 @@
                     )
 
                     return deploy_task.result()
                 else:
                     log(Style.BRIGHT + Fore.LIGHTYELLOW_EX + 'Update set to false. Skipping deploy' + Style.RESET_ALL, prefix='mayalabs')
                     return
             
-            asyncio.run(async_wrapper())
-
+            response = asyncio.run(async_wrapper())
             problems = self.worker.get_flow_problems()
+
+            modules_that_need_cfgs = response['data']['modulesThatNeedCfgProfiles']
+            configure_url = self.worker.configure_url_base
+            if len(modules_that_need_cfgs) > 0:
+                log(
+                    Fore.YELLOW + Style.BRIGHT + f'The following modules need authentication:' + Style.RESET_ALL,
+                    prefix = self.worker.name,
+                    prefix_color = self.worker.prefix_color
+                )
+                for module in modules_that_need_cfgs:
+                    name = module['packageName']
+                    log(
+                        Fore.YELLOW + f'* {name}' + Style.RESET_ALL,
+                        prefix = self.worker.name,
+                        prefix_color= self.worker.prefix_color
+                    )
+                module_ids = ','.join([module['id'] for module in modules_that_need_cfgs])
+                configure_url += f'&modules={module_ids}'
+
+
+
             if len(problems) > 0:
                 log(
                     Fore.YELLOW + Style.BRIGHT + f'Found {len(problems)} missing requirement(s):' + Style.RESET_ALL,
                     prefix = self.worker.name,
                     prefix_color = self.worker.prefix_color
                 )
                 for p in problems:
@@ -297,41 +334,53 @@
                     # message = f'* Missing field {field_name} on node {node_id} (type: {node_type})'
                     message = f'* [{node_id}] Missing field {field_name} on node with type: {node_type}' if default_log_level()=="debug" else f'* Missing field {field_name} on node with type: {node_type}'
                     log(
                         Fore.YELLOW + message + Style.RESET_ALL,
                         prefix = self.worker.name,
                         prefix_color = self.worker.prefix_color
                     )
+                configure_url += '&progIssues=1'
+
+            link = None
+            fixing_needed = False
+            if len(modules_that_need_cfgs) > 0:
+                link = configure_url
+                fixing_needed = True
+            elif len(problems) > 0:
+                link = f'{self.worker.app_url}&progIssues=1'
+                fixing_needed = True
+
+            if fixing_needed:
                 log(
-                    Fore.YELLOW + Style.BRIGHT + 'To run this function, configure these requirements at the link below' + Style.RESET_ALL,
+                    Fore.YELLOW + 'Fix the above problems by going to this link:' + Style.RESET_ALL, 
+                    "\x1B[3m" + link + Style.RESET_ALL,
+                    prefix = self.worker.name,
+                    prefix_color = self.worker.prefix_color
+                )
+            else:
+                log(
+                    Fore.GREEN + 'View/modify the program graph here:' + Style.RESET_ALL, 
+                    "\x1B[3m" + self.worker.app_url + Style.RESET_ALL,
                     prefix = self.worker.name,
                     prefix_color = self.worker.prefix_color
                 )
-
-            log(
-                Fore.GREEN + 'View/modify the program graph here:' + Style.RESET_ALL, 
-                "\x1B[3m" + self.worker.app_url + Style.RESET_ALL,
-                prefix = self.worker.name,
-                prefix_color = self.worker.prefix_color
-            )
             # asyncio.run(async_wrapper())
             
         else:
             raise Exception("Error: Could not find worker") 
 
     def delete(self):
         # Implement this method
         response = SessionClient.delete_session(self.id)
         return response
     
     def change(self):
         # Implement this method
         change_response = SessionClient.change_session(session_id=self.id, script=self.script)
-        if change_response:
-            self.changed = change_response
+        self.changed = change_response
         return
 
     def parse_obj(self, obj):
         self.id = obj['session_id']
         self.script = obj['recipe']
         self.steps = obj['steps']
         self.stitched_flow = obj['stitched_flow']
```

### Comparing `mayalabs-0.0.8/mayalabs/utils/defaults.py` & `mayalabs-0.0.9/mayalabs/utils/defaults.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,8 +25,11 @@
             "No API key provided. You can set your API key in code using 'mayalabs.api_key = <API-KEY>', or you can set the environment variable MAYA_API_KEY=<API-KEY>). You can generate API keys in the Maya web interface. See https://docs.mayalabs.io for details, or email humans@mayalabs.io if you have any questions."
         )
 
 def default_log_level() -> str:
     if mayalabs.log_level is not None:
         return mayalabs.log_level
     else:
-        return "info"
+        return "info"
+    
+
+dashboard_nodes_list = ['dashboard-button', 'dashboard-table', 'dashboard-richtext', 'dashboard-form', 'dashboard-image', 'dashboard-template', 'dashboard-notification']
```

### Comparing `mayalabs-0.0.8/mayalabs/utils/general.py` & `mayalabs-0.0.9/mayalabs/utils/general.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,8 +120,13 @@
         else:
             return check_child_exists(self.children, child_id)
 
 
 class Force(Enum):
     normal = "normal"
     redeploy = "redeploy"
-    regenerate = "regenerate"
+    regenerate = "regenerate"
+
+
+class Views(Enum):
+    dashboard="dashboard"
+    editor="editor"
```

### Comparing `mayalabs-0.0.8/mayalabs/utils/log.py` & `mayalabs-0.0.9/mayalabs/utils/log.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.8/mayalabs/utils/name_gen.py` & `mayalabs-0.0.9/mayalabs/utils/name_gen.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.8/mayalabs/utils/pac_engine.py` & `mayalabs-0.0.9/mayalabs/utils/pac_engine.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.8/mayalabs/utils/poll.py` & `mayalabs-0.0.9/mayalabs/utils/poll.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.8/mayalabs/utils/websocket.py` & `mayalabs-0.0.9/mayalabs/utils/websocket.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.8/mayalabs/worker.py` & `mayalabs-0.0.9/mayalabs/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,14 +153,18 @@
 
     def get_flow_problems(self):
         problems = asyncio.run(
             self._async_get_flow_problems()
         )
 
         return problems
+    
+    def get_flow(self):
+        flow = WorkerClient.get_worker_flows_sync(self.url)
+        return flow
         
     @authenticate
     def attach_session(self, session_id, api_key=None):
         api_base = default_api_base_url()
         request = {
             'url': f"{api_base}/app/v2/brains/linkSessionToRuntime",
             'method': "post",
@@ -178,27 +182,14 @@
             error_log = [
                 'Unable to attach a session to the worker', 
                 'Please contact the Maya team at humans@mayalabs.io',
                 f'session_id = {session_id}, worker_id = {self.id}'
             ]
             raise APIException(format_error_log(error_log))
         
-    @authenticate
-    def test(self, module_name, api_key = None):
-        request = {
-            # 'url': f"{self.url}/nodes?module={module_name}",
-            'url': f"{self.url}/flows",
-            'method': "get",
-            'headers': {
-                'Authorization': 'Bearer ' + api_key,
-            },
-        }
-
-        response = requests.request(**request)
-        print(response.text)
 
     def call(self, msg : dict, session=None):
         if self.id is None:
             raise Exception("Worker ID is not set")
         if self.url is None:
             self.update()
 
@@ -263,15 +254,33 @@
         url_data = urlparse(self.url)
         origin = url_data.netloc
         parts = origin.split('.')
         env = parts[2]
 
         app_subdomain = 'devapp' if "dev" in parts else 'app'
         return f'https://{app_subdomain}.mayalabs.io/edit?id={self.id}'
+    
+    @property
+    def dash_url(self):
+        url_data = urlparse(self.url)
+        origin = url_data.netloc
+        parts = origin.split('.')
+        env = parts[2]
+
+        app_subdomain = 'devapp' if "dev" in parts else 'app'
+        return f'https://{app_subdomain}.mayalabs.io/workers/ui?id={self.id}&version=2'
+    
+    @property
+    def configure_url_base(self):
+        url_data = urlparse(self.url)
+        origin = url_data.netloc
+        parts = origin.split('.')
 
+        app_subdomain = 'devapp' if "dev" in parts else 'app'
+        return f'https://{app_subdomain}.mayalabs.io/configure?worker={self.id}'
 
 
 class WorkerClient:
     @staticmethod
     @authenticate
     def get_worker(worker_id, alias=None, api_key=None) -> Worker:
         api_base = default_api_base_url()
@@ -462,14 +471,32 @@
             'headers': {
                 'x-api-key': api_key,
             },
         }
 
         response = requests.request(**request)
         return response.json
+    
+    @staticmethod
+    @authenticate
+    def reset_worker(worker_id, api_key=None):
+        api_base = default_api_base_url()
+        request = {
+            'url': f"{api_base}/app/v2/brains/resetFlows",
+            'method': "post",
+            'json': {
+                'workerId': worker_id
+            },
+            'headers': {
+                'x-api-key': api_key,
+            },
+        }
+
+        response = requests.request(**request)
+        return response.json
 
     @staticmethod
     @authenticate
     async def call_worker(worker_url, msg, api_key=None):
         async with aiohttp.ClientSession(headers={ 'x-api-key': api_key }) as session:
             async with session.post(f"{worker_url}/send-maya-message", json=msg) as response:
                 try:
@@ -492,14 +519,20 @@
         async with aiohttp.ClientSession(headers={ 'Authorization': f'Bearer {api_key}' }) as session:
             async with session.get(f"{worker_url}/flows", json=msg) as response:
                 response_json = await response.json()
                 return response_json
             
     @staticmethod
     @authenticate
+    def get_worker_flows_sync(worker_url, api_key=None):
+        response = requests.get(f"{worker_url}/flows", headers={"Accept": "application/json", "Authorization": f"Bearer {api_key}"}, json={})
+        return response.json()
+            
+    @staticmethod
+    @authenticate
     async def get_required_fields(worker_url, api_key=None):
         msg = {}
         async with aiohttp.ClientSession(headers={ 'Authorization': f'Bearer {api_key}' }) as session:
             async with session.get(f"{worker_url}/required-fields", json=msg) as response:
                 response_json = await response.json()
                 return response_json
```

### Comparing `mayalabs-0.0.8/mayalabs.egg-info/PKG-INFO` & `mayalabs-0.0.9/mayalabs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d61 7961  : 2.1.Name: maya
 00000020: 6c61 6273 0a56 6572 7369 6f6e 3a20 302e  labs.Version: 0.
-00000030: 302e 380a 5375 6d6d 6172 793a 2050 7974  0.8.Summary: Pyt
+00000030: 302e 390a 5375 6d6d 6172 793a 2050 7974  0.9.Summary: Pyt
 00000040: 686f 6e20 5344 4b20 666f 7220 4d61 7961  hon SDK for Maya
 00000050: 204c 6162 7327 206e 6174 7572 616c 206c   Labs' natural l
 00000060: 616e 6775 6167 6520 7072 6f67 7261 6d6d  anguage programm
 00000070: 696e 6720 7061 7261 6469 676d 0a41 7574  ing paradigm.Aut
 00000080: 686f 722d 656d 6169 6c3a 204d 6179 6120  hor-email: Maya 
 00000090: 5375 7070 6f72 7420 3c68 756d 616e 7340  Support <humans@
 000000a0: 6d61 7961 6c61 6273 2e69 6f3e 0a4d 6169  mayalabs.io>.Mai
@@ -25,204 +25,229 @@
 00000180: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
 00000190: 6e0a 5072 6f76 6964 6573 2d45 7874 7261  n.Provides-Extra
 000001a0: 3a20 7465 7374 0a4c 6963 656e 7365 2d46  : test.License-F
 000001b0: 696c 653a 204c 4943 454e 4345 0a0a 2320  ile: LICENCE..# 
 000001c0: 4d61 7961 204c 6162 7320 3a20 5072 6f67  Maya Labs : Prog
 000001d0: 7261 6d20 6d61 6368 696e 6573 2075 7369  ram machines usi
 000001e0: 6e67 206e 6174 7572 616c 206c 616e 6775  ng natural langu
-000001f0: 6167 652e 0a0a 5468 6520 4d61 7961 204c  age...The Maya L
-00000200: 6162 7320 5079 7468 6f6e 2053 444b 2070  abs Python SDK p
-00000210: 726f 7669 6465 7320 6561 7379 2061 7379  rovides easy asy
-00000220: 6e63 2061 6363 6573 7320 746f 206f 7572  nc access to our
-00000230: 2050 4143 2d31 2070 726f 6772 616d 2073   PAC-1 program s
-00000240: 796e 7468 6573 6973 2065 6e67 696e 652c  ynthesis engine,
-00000250: 2077 6974 6820 6120 434c 4920 746f 2069   with a CLI to i
-00000260: 6e73 7472 7563 7420 616e 6420 6765 6e65  nstruct and gene
-00000270: 7261 7465 2070 726f 6772 616d 7320 6672  rate programs fr
-00000280: 6f6d 2069 6e73 7472 7563 7469 6f6e 7320  om instructions 
-00000290: 696e 206e 6174 7572 616c 206c 616e 6775  in natural langu
-000002a0: 6167 652e 0a0a 0a23 2320 496e 7374 616c  age....## Instal
-000002b0: 6c61 7469 6f6e 0a0a 6060 600a 7069 7020  lation..```.pip 
-000002c0: 696e 7374 616c 6c20 2d2d 7570 6772 6164  install --upgrad
-000002d0: 6520 6d61 7961 6c61 6273 0a60 6060 0a23  e mayalabs.```.#
-000002e0: 2320 5072 6576 6965 770a 0a68 7474 7073  # Preview..https
-000002f0: 3a2f 2f75 7365 722d 696d 6167 6573 2e67  ://user-images.g
-00000300: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00000310: 2e63 6f6d 2f38 3733 3637 3937 2f32 3330  .com/8736797/230
-00000320: 3934 3734 3430 2d32 3430 3337 3632 642d  947440-2403762d-
-00000330: 6131 3462 2d34 6230 302d 3866 6265 2d62  a14b-4b00-8fbe-b
-00000340: 6438 3033 6162 3234 3032 382e 6d70 340a  d803ab24028.mp4.
-00000350: 0a0a 2323 2055 7361 6765 0a0a 4765 7420  ..## Usage..Get 
-00000360: 7468 6520 4d61 7961 204c 6162 7320 4150  the Maya Labs AP
-00000370: 4920 6b65 7920 6672 6f6d 2074 6865 2053  I key from the S
-00000380: 6574 7469 6e67 7320 3e20 4465 7665 6c6f  ettings > Develo
-00000390: 7065 7220 5b73 6563 7469 6f6e 5d28 6874  per [section](ht
-000003a0: 7470 733a 2f2f 6170 702e 6d61 7961 6c61  tps://app.mayala
-000003b0: 6273 2e69 6f2f 7365 7474 696e 6773 2f64  bs.io/settings/d
-000003c0: 6576 656c 6f70 6572 7329 2e0a 0a60 6060  evelopers)...```
-000003d0: 0a65 7870 6f72 7420 4d41 5941 5f41 5049  .export MAYA_API
-000003e0: 5f4b 4559 203d 2022 6d61 7961 6b65 792d  _KEY = "mayakey-
-000003f0: 2e2e 2e22 0a60 6060 0a0a 4f72 2073 6574  ...".```..Or set
-00000400: 2060 6d61 7961 6c61 6273 2e61 7069 5f6b   `mayalabs.api_k
-00000410: 6579 6020 746f 2069 7473 2076 616c 7565  ey` to its value
-00000420: 3a0a 0a60 6060 0a69 6d70 6f72 7420 6d61  :..```.import ma
-00000430: 7961 6c61 6273 0a0a 6d61 7961 6c61 6273  yalabs..mayalabs
-00000440: 2e61 7069 5f6b 6579 203d 2022 6d61 7961  .api_key = "maya
-00000450: 6b65 792d 2e2e 2e22 0a0a 7363 7269 7074  key-..."..script
-00000460: 203d 2022 2222 0a31 2e20 7472 6967 6765   = """.1. trigge
-00000470: 7220 6f6e 2072 6563 6569 7665 0a32 2e20  r on receive.2. 
-00000480: 7265 7365 6172 6368 207b 7b74 6572 6d7d  research {{term}
-00000490: 7d20 6f6e 2077 696b 6970 6564 6961 0a33  } on wikipedia.3
-000004a0: 2e20 6578 7472 6163 7420 2774 6974 6c65  . extract 'title
-000004b0: 2720 616e 6420 2773 756d 6d61 7279 2720  ' and 'summary' 
-000004c0: 6672 6f6d 2074 6162 756c 6172 2064 6174  from tabular dat
-000004d0: 610a 342e 2073 656e 6420 7265 7370 6f6e  a.4. send respon
-000004e0: 7365 2062 6163 6b0a 2222 220a 0a66 756e  se back."""..fun
-000004f0: 6374 696f 6e20 3d20 6d61 7961 6c61 6273  ction = mayalabs
-00000500: 2e46 756e 6374 696f 6e28 6e61 6d65 3d22  .Function(name="
-00000510: 5363 7261 7065 3222 290a 2320 4372 6561  Scrape2").# Crea
-00000520: 7469 6e67 206e 6577 2077 6f72 6b65 722e  ting new worker.
-00000530: 2e2e 0a0a 6675 6e63 7469 6f6e 2e75 7064  ....function.upd
-00000540: 6174 6528 7363 7269 7074 3d73 6372 6970  ate(script=scrip
-00000550: 7429 0a23 2047 656e 6572 6174 696e 6720  t).# Generating 
-00000560: 7072 6f67 7261 6d20 6772 6170 682e 2e2e  program graph...
-00000570: 0a23 2053 7461 7274 696e 6720 776f 726b  .# Starting work
-00000580: 6572 2e2e 2e0a 2320 496e 7374 616c 6c69  er....# Installi
-00000590: 6e67 2064 6570 656e 6465 6e63 6965 732e  ng dependencies.
-000005a0: 2e2e 0a23 2044 6570 6c6f 7965 6421 0a0a  ...# Deployed!..
-000005b0: 6f75 7470 7574 203d 2066 756e 6374 696f  output = functio
-000005c0: 6e2e 6361 6c6c 287b 2274 6572 6d22 3a20  n.call({"term": 
-000005d0: 2244 722e 2056 696b 7261 6d20 5361 7261  "Dr. Vikram Sara
-000005e0: 6268 6169 227d 290a 7072 696e 7428 6f75  bhai"}).print(ou
-000005f0: 7470 7574 290a 2320 6669 6e64 7320 616e  tput).# finds an
-00000600: 6420 6f75 7470 7574 7320 7469 746c 6520  d outputs title 
-00000610: 616e 6420 7375 6d6d 6172 7920 6672 6f6d  and summary from
-00000620: 2077 696b 6970 6564 6961 2072 6573 756c   wikipedia resul
-00000630: 7473 0a0a 6060 600a 0a50 4143 2d31 2074  ts..```..PAC-1 t
-00000640: 616b 6573 2069 6e20 7374 6570 7320 7772  akes in steps wr
-00000650: 6974 7465 6e20 696e 2045 6e67 6c69 7368  itten in English
-00000660: 2c20 7772 6974 6573 2026 2061 7373 656d  , writes & assem
-00000670: 626c 6573 2061 2064 6973 6372 6574 6520  bles a discrete 
-00000680: 7072 6f67 7261 6d20 6772 6170 682c 2061  program graph, a
-00000690: 6e64 2064 6570 6c6f 7973 2072 6561 6479  nd deploys ready
-000006a0: 2d74 6f2d 7573 6520 736f 6674 7761 7265  -to-use software
-000006b0: 206f 6e20 6f75 7220 636f 6d70 7574 6520   on our compute 
-000006c0: 696e 6672 6173 7472 7563 7475 7265 2c20  infrastructure, 
-000006d0: 7468 6174 2079 6f75 2063 616e 2063 616c  that you can cal
-000006e0: 6c20 7769 7468 696e 2079 6f75 7220 636f  l within your co
-000006f0: 6465 2e20 596f 7520 6361 6e20 7365 7420  de. You can set 
-00000700: 7570 206d 6973 7369 6e67 2064 6570 656e  up missing depen
-00000710: 6465 6e63 6965 7320 2f20 7669 7375 616c  dencies / visual
-00000720: 697a 6520 7468 6520 666c 6f77 206f 6620  ize the flow of 
-00000730: 6c6f 6769 6320 6279 2066 6f6c 6c6f 7769  logic by followi
-00000740: 6e67 2074 6865 206c 696e 6b20 746f 2066  ng the link to f
-00000750: 6c6f 772d 6261 7365 6420 6564 6974 6f72  low-based editor
-00000760: 2069 7420 7072 6f76 6964 6573 2061 6674   it provides aft
-00000770: 6572 2064 6570 6c6f 796d 656e 742e 0a0a  er deployment...
-00000780: 2323 2055 7365 2043 6173 6573 0a0a 2d20  ## Use Cases..- 
-00000790: 5b49 662e 2e2e 5468 656e 2043 6f6e 6469  [If...Then Condi
-000007a0: 7469 6f6e 616c 7320 616e 6420 4c6f 6f70  tionals and Loop
-000007b0: 696e 675d 282f 4558 414d 504c 4553 2e6d  ing](/EXAMPLES.m
-000007c0: 6423 6966 7468 656e 2d63 6f6e 6469 7469  d#ifthen-conditi
-000007d0: 6f6e 616c 732d 616e 642d 6c6f 6f70 696e  onals-and-loopin
-000007e0: 6729 0a2d 205b 4375 7374 6f6d 2046 756e  g).- [Custom Fun
-000007f0: 6374 696f 6e73 5d28 2f45 5841 4d50 4c45  ctions](/EXAMPLE
-00000800: 532e 6d64 2363 7573 746f 6d2d 6675 6e63  S.md#custom-func
-00000810: 7469 6f6e 7329 0a2d 205b 5765 6220 5363  tions).- [Web Sc
-00000820: 7261 7065 7273 5d28 2f45 5841 4d50 4c45  rapers](/EXAMPLE
-00000830: 532e 6d64 2377 6562 2d73 6372 6170 6572  S.md#web-scraper
-00000840: 7329 0a2d 205b 5265 7065 6174 696e 6720  s).- [Repeating 
-00000850: 576f 726b 666c 6f77 735d 282f 4558 414d  Workflows](/EXAM
-00000860: 504c 4553 2e6d 6423 7265 7065 6174 696e  PLES.md#repeatin
-00000870: 672d 776f 726b 666c 6f77 7329 0a2d 205b  g-workflows).- [
-00000880: 4375 7374 6f6d 2044 6173 6862 6f61 7264  Custom Dashboard
-00000890: 735d 282f 4558 414d 504c 4553 2e6d 6423  s](/EXAMPLES.md#
-000008a0: 6375 7374 6f6d 2d64 6173 6862 6f61 7264  custom-dashboard
-000008b0: 7329 0a2d 205b 4461 7461 2054 7261 6e73  s).- [Data Trans
-000008c0: 666f 726d 6174 696f 6e5d 282f 4558 414d  formation](/EXAM
-000008d0: 504c 4553 2e6d 6423 6461 7461 2d74 7261  PLES.md#data-tra
-000008e0: 6e73 666f 726d 6174 696f 6e29 0a2d 205b  nsformation).- [
-000008f0: 506c 6174 666f 726d 2042 6f74 735d 282f  Platform Bots](/
-00000900: 4558 414d 504c 4553 2e6d 6423 706c 6174  EXAMPLES.md#plat
-00000910: 666f 726d 2d62 6f74 7329 0a2d 205b 4275  form-bots).- [Bu
-00000920: 7369 6e65 7373 2050 726f 6365 7373 6573  siness Processes
-00000930: 5d28 2f45 5841 4d50 4c45 532e 6d64 2362  ](/EXAMPLES.md#b
-00000940: 7573 696e 6573 732d 7072 6f63 6573 7365  usiness-processe
-00000950: 7329 0a2d 205b 4c6f 6e67 2d74 6572 6d20  s).- [Long-term 
-00000960: 6d65 6d6f 7279 5d28 2f45 5841 4d50 4c45  memory](/EXAMPLE
-00000970: 532e 6d64 236c 6f6e 672d 7465 726d 2d6d  S.md#long-term-m
-00000980: 656d 6f72 7929 0a2d 205b 4469 7669 7369  emory).- [Divisi
-00000990: 6f6e 206f 6620 6c61 626f 7572 5d28 2f45  on of labour](/E
-000009a0: 5841 4d50 4c45 532e 6d64 2364 6976 6973  XAMPLES.md#divis
-000009b0: 696f 6e2d 6f66 2d6c 6162 6f75 7229 0a20  ion-of-labour). 
-000009c0: 202d 205b 5061 7261 6c6c 656c 697a 6174   - [Parallelizat
-000009d0: 696f 6e5d 282f 4558 414d 504c 4553 2e6d  ion](/EXAMPLES.m
-000009e0: 6423 7061 7261 6c6c 656c 697a 6174 696f  d#parallelizatio
-000009f0: 6e29 0a20 202d 205b 436f 6e63 7572 7265  n).  - [Concurre
-00000a00: 6e63 795d 282f 4558 414d 504c 4553 2e6d  ncy](/EXAMPLES.m
-00000a10: 6423 636f 6e63 7572 7265 6e63 7929 0a0a  d#concurrency)..
-00000a20: 2323 2043 6f6d 6d61 6e64 204c 696e 6520  ## Command Line 
-00000a30: 5573 6167 650a 0a54 6f64 6179 2c20 7363  Usage..Today, sc
-00000a40: 7269 7074 206e 6565 6420 746f 2062 6520  ript need to be 
-00000a50: 6d61 6e75 616c 6c79 2077 7269 7474 656e  manually written
-00000a60: 2073 7465 702d 6279 2d73 7465 702c 2062   step-by-step, b
-00000a70: 7574 2077 6520 6172 6520 6f66 6665 7269  ut we are offeri
-00000a80: 6e67 2065 6172 6c79 2057 4950 2070 7265  ng early WIP pre
-00000a90: 7669 6577 206f 6620 6974 6572 6174 6976  view of iterativ
-00000aa0: 6520 7363 7269 7074 2067 656e 6572 6174  e script generat
-00000ab0: 696f 6e20 7669 6120 6f75 7220 434c 492e  ion via our CLI.
-00000ac0: 2054 7279 2072 756e 6e69 6e67 3a0a 0a60   Try running:..`
-00000ad0: 6060 0a24 206d 6179 616c 6162 7320 696e  ``.$ mayalabs in
-00000ae0: 7374 7275 6374 202d 6320 2766 6574 6368  struct -c 'fetch
-00000af0: 204e 616d 6520 616e 6420 456d 6169 6c20   Name and Email 
-00000b00: 6672 6f6d 2067 7368 6565 742c 2077 7269  from gsheet, wri
-00000b10: 7465 2066 756e 6374 696f 6e20 746f 206d  te function to m
-00000b20: 6572 6765 2061 6c6c 2063 6f6c 756d 6e73  erge all columns
-00000b30: 2c20 616e 6420 7265 7475 726e 2064 6174  , and return dat
-00000b40: 6127 0a60 6060 0a0a 416e 6420 7468 656e  a'.```..And then
-00000b50: 2075 7365 2074 6865 2067 656e 6572 6174   use the generat
-00000b60: 6564 2073 6372 6970 7420 6173 2066 756e  ed script as fun
-00000b70: 6374 696f 6e2e 0a0a 6874 7470 733a 2f2f  ction...https://
-00000b80: 7573 6572 2d69 6d61 6765 732e 6769 7468  user-images.gith
-00000b90: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00000ba0: 6d2f 3532 3439 3330 3737 2f32 3331 3937  m/52493077/23197
-00000bb0: 3932 3834 2d61 3764 3163 3433 642d 6636  9284-a7d1c43d-f6
-00000bc0: 6336 2d34 3732 362d 3839 6665 2d32 3865  c6-4726-89fe-28e
-00000bd0: 3130 3363 6431 3938 662e 6d70 340a 0a23  103cd198f.mp4..#
-00000be0: 2320 5265 7175 6972 656d 656e 7473 0a0a  # Requirements..
-00000bf0: 2d20 5079 7468 6f6e 2033 2e37 2e31 2b0a  - Python 3.7.1+.
-00000c00: 0a23 2320 4973 7375 6573 0a0a 416c 6c20  .## Issues..All 
-00000c10: 6665 6564 6261 636b 2061 6e64 2062 7567  feedback and bug
-00000c20: 2072 6570 6f72 7473 2077 656c 636f 6d65   reports welcome
-00000c30: 2120 5265 706f 7274 2069 6e20 7468 6520  ! Report in the 
-00000c40: 5b69 7373 7565 7320 7365 6374 696f 6e5d  [issues section]
-00000c50: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000c60: 636f 6d2f 6d61 7961 6871 2f6d 6179 616c  com/mayahq/mayal
-00000c70: 6162 732d 7364 6b2d 7079 7468 6f6e 2f69  abs-sdk-python/i
-00000c80: 7373 7565 7329 2c20 6f72 206d 6169 6c20  ssues), or mail 
-00000c90: 7573 2061 7420 6875 6d61 6e73 406d 6179  us at humans@may
-00000ca0: 616c 6162 732e 696f 2e0a 0a46 756c 6c20  alabs.io...Full 
-00000cb0: 6c69 7374 206f 6620 6361 7061 6269 6c69  list of capabili
-00000cc0: 7469 6573 2061 6e64 206c 696d 6974 7320  ties and limits 
-00000cd0: 5b68 6572 655d 2868 7474 7073 3a2f 2f64  [here](https://d
-00000ce0: 6f63 732e 6d61 7961 6c61 6273 2e69 6f2f  ocs.mayalabs.io/
-00000cf0: 6361 7061 6269 6c69 7469 6573 2d61 6e64  capabilities-and
-00000d00: 2d6c 696d 6974 7329 2e0a 0a0a 2323 2052  -limits)....## R
-00000d10: 6f61 646d 6170 0a2d 205b 785d 2043 6c65  oadmap.- [x] Cle
-00000d20: 616e 6572 206c 6f67 7320 616e 6420 6578  aner logs and ex
-00000d30: 6365 7074 696f 6e20 6861 6e64 6c69 6e67  ception handling
-00000d40: 0a2d 205b 205d 2044 6570 656e 6465 6e63  .- [ ] Dependenc
-00000d50: 7920 636f 6e66 6967 7572 6174 696f 6e20  y configuration 
-00000d60: 5558 2069 6d70 726f 7665 6d65 6e74 0a2d  UX improvement.-
-00000d70: 205b 205d 2049 6d70 6f72 7420 736b 696c   [ ] Import skil
-00000d80: 6c20 7265 706f 7369 746f 7269 6573 2066  l repositories f
-00000d90: 6f72 2072 6575 7369 6e67 2073 6b69 6c6c  or reusing skill
-00000da0: 7320 6372 6561 7465 6420 6279 2075 7365  s created by use
-00000db0: 7220 6f72 2070 7265 7365 6e74 2069 6e20  r or present in 
-00000dc0: 7374 6f72 650a 2d20 5b20 5d20 4372 6561  store.- [ ] Crea
-00000dd0: 7465 2061 6e64 2063 616c 6c20 646f 776e  te and call down
-00000de0: 7374 7265 616d 2061 7574 6f2d 6465 706c  stream auto-depl
-00000df0: 6f79 6564 2066 756e 6374 696f 6e73 0a2d  oyed functions.-
-00000e00: 205b 205d 2041 6c6c 6f77 206d 756c 7469   [ ] Allow multi
-00000e10: 2d70 726f 6669 6c65 2061 6e64 2074 6561  -profile and tea
-00000e20: 6d20 7072 6f66 696c 6520 6163 6365 7373  m profile access
-00000e30: 0a                                       .
+000001f0: 6167 652e 0a0a 3c70 2061 6c69 676e 3d22  age...<p align="
+00000200: 6c65 6674 223e 0a20 203c 6120 6872 6566  left">.  <a href
+00000210: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
+00000220: 7267 2f70 726f 6a65 6374 2f6d 6179 616c  rg/project/mayal
+00000230: 6162 7322 3e0a 2020 2020 3c69 6d67 2073  abs">.    <img s
+00000240: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000250: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000260: 762f 6d61 7961 6c61 6273 3f73 7479 6c65  v/mayalabs?style
+00000270: 3d66 6f72 2d74 6865 2d62 6164 6765 2220  =for-the-badge" 
+00000280: 2f3e 0a20 203c 2f61 3e0a 2020 3c61 2068  />.  </a>.  <a h
+00000290: 7265 663d 2268 7474 7073 3a2f 2f6d 6179  ref="https://may
+000002a0: 616c 6162 732e 696f 2f64 6f63 7322 3e0a  alabs.io/docs">.
+000002b0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000002c0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000002d0: 732e 696f 2f62 6164 6765 2f44 6f63 756d  s.io/badge/Docum
+000002e0: 656e 7461 7469 6f6e 2d62 6c75 653f 6c6f  entation-blue?lo
+000002f0: 676f 3d47 6974 426f 6f6b 266c 6f67 6f43  go=GitBook&logoC
+00000300: 6f6c 6f72 3d77 6869 7465 2673 7479 6c65  olor=white&style
+00000310: 3d66 6f72 2d74 6865 2d62 6164 6765 2220  =for-the-badge" 
+00000320: 2f3e 0a20 203c 2f61 3e0a 3c2f 703e 0a3c  />.  </a>.</p>.<
+00000330: 6272 3e0a 0a54 6865 204d 6179 6120 4c61  br>..The Maya La
+00000340: 6273 2050 7974 686f 6e20 5344 4b20 7072  bs Python SDK pr
+00000350: 6f76 6964 6573 2065 6173 7920 6173 796e  ovides easy asyn
+00000360: 6320 6163 6365 7373 2074 6f20 6f75 7220  c access to our 
+00000370: 5041 432d 3120 7072 6f67 7261 6d20 7379  PAC-1 program sy
+00000380: 6e74 6865 7369 7320 656e 6769 6e65 2c20  nthesis engine, 
+00000390: 7769 7468 2061 2043 4c49 2074 6f20 696e  with a CLI to in
+000003a0: 7374 7275 6374 2061 6e64 2067 656e 6572  struct and gener
+000003b0: 6174 6520 7072 6f67 7261 6d73 2066 726f  ate programs fro
+000003c0: 6d20 696e 7374 7275 6374 696f 6e73 2069  m instructions i
+000003d0: 6e20 6e61 7475 7261 6c20 6c61 6e67 7561  n natural langua
+000003e0: 6765 2e0a 0a23 2320 496e 7374 616c 6c61  ge...## Installa
+000003f0: 7469 6f6e 0a0a 6060 600a 7069 7020 696e  tion..```.pip in
+00000400: 7374 616c 6c20 2d2d 7570 6772 6164 6520  stall --upgrade 
+00000410: 6d61 7961 6c61 6273 0a60 6060 0a23 2320  mayalabs.```.## 
+00000420: 5072 6576 6965 770a 0a68 7474 7073 3a2f  Preview..https:/
+00000430: 2f75 7365 722d 696d 6167 6573 2e67 6974  /user-images.git
+00000440: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000450: 6f6d 2f38 3733 3637 3937 2f32 3330 3934  om/8736797/23094
+00000460: 3734 3430 2d32 3430 3337 3632 642d 6131  7440-2403762d-a1
+00000470: 3462 2d34 6230 302d 3866 6265 2d62 6438  4b-4b00-8fbe-bd8
+00000480: 3033 6162 3234 3032 382e 6d70 340a 0a0a  03ab24028.mp4...
+00000490: 2323 2055 7361 6765 0a0a 4765 7420 7468  ## Usage..Get th
+000004a0: 6520 4d61 7961 204c 6162 7320 4150 4920  e Maya Labs API 
+000004b0: 6b65 7920 6672 6f6d 2074 6865 2053 6574  key from the Set
+000004c0: 7469 6e67 7320 3e20 4465 7665 6c6f 7065  tings > Develope
+000004d0: 7220 5b73 6563 7469 6f6e 5d28 6874 7470  r [section](http
+000004e0: 733a 2f2f 6170 702e 6d61 7961 6c61 6273  s://app.mayalabs
+000004f0: 2e69 6f2f 7365 7474 696e 6773 2f64 6576  .io/settings/dev
+00000500: 656c 6f70 6572 7329 2e0a 0a60 6060 0a65  elopers)...```.e
+00000510: 7870 6f72 7420 4d41 5941 5f41 5049 5f4b  xport MAYA_API_K
+00000520: 4559 203d 2022 6d61 7961 6b65 792d 2e2e  EY = "mayakey-..
+00000530: 2e22 0a60 6060 0a0a 4f72 2073 6574 2060  .".```..Or set `
+00000540: 6d61 7961 6c61 6273 2e61 7069 5f6b 6579  mayalabs.api_key
+00000550: 6020 746f 2069 7473 2076 616c 7565 3a0a  ` to its value:.
+00000560: 0a60 6060 0a69 6d70 6f72 7420 6d61 7961  .```.import maya
+00000570: 6c61 6273 0a0a 6d61 7961 6c61 6273 2e61  labs..mayalabs.a
+00000580: 7069 5f6b 6579 203d 2022 6d61 7961 6b65  pi_key = "mayake
+00000590: 792d 2e2e 2e22 0a0a 7363 7269 7074 203d  y-..."..script =
+000005a0: 2022 2222 0a31 2e20 7472 6967 6765 7220   """.1. trigger 
+000005b0: 6f6e 2072 6563 6569 7665 0a32 2e20 7265  on receive.2. re
+000005c0: 7365 6172 6368 207b 7b74 6572 6d7d 7d20  search {{term}} 
+000005d0: 6f6e 2077 696b 6970 6564 6961 0a33 2e20  on wikipedia.3. 
+000005e0: 6578 7472 6163 7420 2774 6974 6c65 2720  extract 'title' 
+000005f0: 616e 6420 2773 756d 6d61 7279 2720 6672  and 'summary' fr
+00000600: 6f6d 2074 6162 756c 6172 2064 6174 610a  om tabular data.
+00000610: 342e 2073 656e 6420 7265 7370 6f6e 7365  4. send response
+00000620: 2062 6163 6b0a 2222 220a 0a66 756e 6374   back."""..funct
+00000630: 696f 6e20 3d20 6d61 7961 6c61 6273 2e46  ion = mayalabs.F
+00000640: 756e 6374 696f 6e28 6e61 6d65 3d22 5363  unction(name="Sc
+00000650: 7261 7065 3222 290a 2320 4372 6561 7469  rape2").# Creati
+00000660: 6e67 206e 6577 2077 6f72 6b65 722e 2e2e  ng new worker...
+00000670: 0a0a 6675 6e63 7469 6f6e 2e75 7064 6174  ..function.updat
+00000680: 6528 7363 7269 7074 3d73 6372 6970 7429  e(script=script)
+00000690: 0a23 2047 656e 6572 6174 696e 6720 7072  .# Generating pr
+000006a0: 6f67 7261 6d20 6772 6170 682e 2e2e 0a23  ogram graph....#
+000006b0: 2053 7461 7274 696e 6720 776f 726b 6572   Starting worker
+000006c0: 2e2e 2e0a 2320 496e 7374 616c 6c69 6e67  ....# Installing
+000006d0: 2064 6570 656e 6465 6e63 6965 732e 2e2e   dependencies...
+000006e0: 0a23 2044 6570 6c6f 7965 6421 0a0a 6f75  .# Deployed!..ou
+000006f0: 7470 7574 203d 2066 756e 6374 696f 6e2e  tput = function.
+00000700: 6361 6c6c 287b 2274 6572 6d22 3a20 2244  call({"term": "D
+00000710: 722e 2056 696b 7261 6d20 5361 7261 6268  r. Vikram Sarabh
+00000720: 6169 227d 290a 7072 696e 7428 6f75 7470  ai"}).print(outp
+00000730: 7574 290a 2320 6669 6e64 7320 616e 6420  ut).# finds and 
+00000740: 6f75 7470 7574 7320 7469 746c 6520 616e  outputs title an
+00000750: 6420 7375 6d6d 6172 7920 6672 6f6d 2077  d summary from w
+00000760: 696b 6970 6564 6961 2072 6573 756c 7473  ikipedia results
+00000770: 0a0a 6060 600a 0a50 4143 2d31 2074 616b  ..```..PAC-1 tak
+00000780: 6573 2069 6e20 7374 6570 7320 7772 6974  es in steps writ
+00000790: 7465 6e20 696e 2045 6e67 6c69 7368 2c20  ten in English, 
+000007a0: 7772 6974 6573 2026 2061 7373 656d 626c  writes & assembl
+000007b0: 6573 2061 2064 6973 6372 6574 6520 7072  es a discrete pr
+000007c0: 6f67 7261 6d20 6772 6170 682c 2061 6e64  ogram graph, and
+000007d0: 2064 6570 6c6f 7973 2072 6561 6479 2d74   deploys ready-t
+000007e0: 6f2d 7573 6520 736f 6674 7761 7265 206f  o-use software o
+000007f0: 6e20 6f75 7220 636f 6d70 7574 6520 696e  n our compute in
+00000800: 6672 6173 7472 7563 7475 7265 2c20 7468  frastructure, th
+00000810: 6174 2079 6f75 2063 616e 2063 616c 6c20  at you can call 
+00000820: 7769 7468 696e 2079 6f75 7220 636f 6465  within your code
+00000830: 2e20 596f 7520 6361 6e20 7365 7420 7570  . You can set up
+00000840: 206d 6973 7369 6e67 2064 6570 656e 6465   missing depende
+00000850: 6e63 6965 7320 2f20 7669 7375 616c 697a  ncies / visualiz
+00000860: 6520 7468 6520 666c 6f77 206f 6620 6c6f  e the flow of lo
+00000870: 6769 6320 6279 2066 6f6c 6c6f 7769 6e67  gic by following
+00000880: 2074 6865 206c 696e 6b20 746f 2066 6c6f   the link to flo
+00000890: 772d 6261 7365 6420 6564 6974 6f72 2069  w-based editor i
+000008a0: 7420 7072 6f76 6964 6573 2061 6674 6572  t provides after
+000008b0: 2064 6570 6c6f 796d 656e 742e 0a0a 4368   deployment...Ch
+000008c0: 6563 6b20 6f75 7220 5b64 6f63 756d 656e  eck our [documen
+000008d0: 7461 7469 6f6e 5d28 2268 7474 7073 3a2f  tation]("https:/
+000008e0: 2f6d 6179 616c 6162 732e 696f 2f64 6f63  /mayalabs.io/doc
+000008f0: 7322 2920 666f 7220 6d6f 7265 2075 7361  s") for more usa
+00000900: 6765 2061 6e64 2074 7574 6f72 6961 6c73  ge and tutorials
+00000910: 2e0a 0a23 2320 5573 6520 4361 7365 730a  ...## Use Cases.
+00000920: 0a2d 205b 4966 2e2e 2e54 6865 6e20 436f  .- [If...Then Co
+00000930: 6e64 6974 696f 6e61 6c73 2061 6e64 204c  nditionals and L
+00000940: 6f6f 7069 6e67 5d28 2f45 5841 4d50 4c45  ooping](/EXAMPLE
+00000950: 532e 6d64 2369 6674 6865 6e2d 636f 6e64  S.md#ifthen-cond
+00000960: 6974 696f 6e61 6c73 2d61 6e64 2d6c 6f6f  itionals-and-loo
+00000970: 7069 6e67 290a 2d20 5b43 7573 746f 6d20  ping).- [Custom 
+00000980: 4675 6e63 7469 6f6e 735d 282f 4558 414d  Functions](/EXAM
+00000990: 504c 4553 2e6d 6423 6375 7374 6f6d 2d66  PLES.md#custom-f
+000009a0: 756e 6374 696f 6e73 290a 2d20 5b57 6562  unctions).- [Web
+000009b0: 2053 6372 6170 6572 735d 282f 4558 414d   Scrapers](/EXAM
+000009c0: 504c 4553 2e6d 6423 7765 622d 7363 7261  PLES.md#web-scra
+000009d0: 7065 7273 290a 2d20 5b52 6570 6561 7469  pers).- [Repeati
+000009e0: 6e67 2057 6f72 6b66 6c6f 7773 5d28 2f45  ng Workflows](/E
+000009f0: 5841 4d50 4c45 532e 6d64 2372 6570 6561  XAMPLES.md#repea
+00000a00: 7469 6e67 2d77 6f72 6b66 6c6f 7773 290a  ting-workflows).
+00000a10: 2d20 5b43 7573 746f 6d20 4461 7368 626f  - [Custom Dashbo
+00000a20: 6172 6473 5d28 2f45 5841 4d50 4c45 532e  ards](/EXAMPLES.
+00000a30: 6d64 2363 7573 746f 6d2d 6461 7368 626f  md#custom-dashbo
+00000a40: 6172 6473 290a 2d20 5b44 6174 6120 5472  ards).- [Data Tr
+00000a50: 616e 7366 6f72 6d61 7469 6f6e 5d28 2f45  ansformation](/E
+00000a60: 5841 4d50 4c45 532e 6d64 2364 6174 612d  XAMPLES.md#data-
+00000a70: 7472 616e 7366 6f72 6d61 7469 6f6e 290a  transformation).
+00000a80: 2d20 5b50 6c61 7466 6f72 6d20 426f 7473  - [Platform Bots
+00000a90: 5d28 2f45 5841 4d50 4c45 532e 6d64 2370  ](/EXAMPLES.md#p
+00000aa0: 6c61 7466 6f72 6d2d 626f 7473 290a 2d20  latform-bots).- 
+00000ab0: 5b42 7573 696e 6573 7320 5072 6f63 6573  [Business Proces
+00000ac0: 7365 735d 282f 4558 414d 504c 4553 2e6d  ses](/EXAMPLES.m
+00000ad0: 6423 6275 7369 6e65 7373 2d70 726f 6365  d#business-proce
+00000ae0: 7373 6573 290a 2d20 5b4c 6f6e 672d 7465  sses).- [Long-te
+00000af0: 726d 206d 656d 6f72 795d 282f 4558 414d  rm memory](/EXAM
+00000b00: 504c 4553 2e6d 6423 6c6f 6e67 2d74 6572  PLES.md#long-ter
+00000b10: 6d2d 6d65 6d6f 7279 290a 2d20 5b44 6976  m-memory).- [Div
+00000b20: 6973 696f 6e20 6f66 206c 6162 6f75 725d  ision of labour]
+00000b30: 282f 4558 414d 504c 4553 2e6d 6423 6469  (/EXAMPLES.md#di
+00000b40: 7669 7369 6f6e 2d6f 662d 6c61 626f 7572  vision-of-labour
+00000b50: 290a 2020 2d20 5b50 6172 616c 6c65 6c69  ).  - [Paralleli
+00000b60: 7a61 7469 6f6e 5d28 2f45 5841 4d50 4c45  zation](/EXAMPLE
+00000b70: 532e 6d64 2370 6172 616c 6c65 6c69 7a61  S.md#paralleliza
+00000b80: 7469 6f6e 290a 2020 2d20 5b43 6f6e 6375  tion).  - [Concu
+00000b90: 7272 656e 6379 5d28 2f45 5841 4d50 4c45  rrency](/EXAMPLE
+00000ba0: 532e 6d64 2363 6f6e 6375 7272 656e 6379  S.md#concurrency
+00000bb0: 290a 0a23 2320 436f 6d6d 616e 6420 4c69  )..## Command Li
+00000bc0: 6e65 2055 7361 6765 0a0a 546f 6461 792c  ne Usage..Today,
+00000bd0: 2073 6372 6970 7420 6e65 6564 2074 6f20   script need to 
+00000be0: 6265 206d 616e 7561 6c6c 7920 7772 6974  be manually writ
+00000bf0: 7465 6e20 7374 6570 2d62 792d 7374 6570  ten step-by-step
+00000c00: 2c20 6275 7420 7765 2061 7265 206f 6666  , but we are off
+00000c10: 6572 696e 6720 6561 726c 7920 5749 5020  ering early WIP 
+00000c20: 7072 6576 6965 7720 6f66 2069 7465 7261  preview of itera
+00000c30: 7469 7665 2073 6372 6970 7420 6765 6e65  tive script gene
+00000c40: 7261 7469 6f6e 2076 6961 206f 7572 2043  ration via our C
+00000c50: 4c49 2e20 5472 7920 7275 6e6e 696e 673a  LI. Try running:
+00000c60: 0a0a 6060 600a 2420 6d61 7961 6c61 6273  ..```.$ mayalabs
+00000c70: 2069 6e73 7472 7563 7420 2d63 2027 6665   instruct -c 'fe
+00000c80: 7463 6820 4e61 6d65 2061 6e64 2045 6d61  tch Name and Ema
+00000c90: 696c 2066 726f 6d20 6773 6865 6574 2c20  il from gsheet, 
+00000ca0: 7772 6974 6520 6675 6e63 7469 6f6e 2074  write function t
+00000cb0: 6f20 6d65 7267 6520 616c 6c20 636f 6c75  o merge all colu
+00000cc0: 6d6e 732c 2061 6e64 2072 6574 7572 6e20  mns, and return 
+00000cd0: 6461 7461 270a 6060 600a 0a41 6e64 2074  data'.```..And t
+00000ce0: 6865 6e20 7573 6520 7468 6520 6765 6e65  hen use the gene
+00000cf0: 7261 7465 6420 7363 7269 7074 2061 7320  rated script as 
+00000d00: 6675 6e63 7469 6f6e 2e0a 0a68 7474 7073  function...https
+00000d10: 3a2f 2f75 7365 722d 696d 6167 6573 2e67  ://user-images.g
+00000d20: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000d30: 2e63 6f6d 2f35 3234 3933 3037 372f 3233  .com/52493077/23
+00000d40: 3139 3739 3238 342d 6137 6431 6334 3364  1979284-a7d1c43d
+00000d50: 2d66 3663 362d 3437 3236 2d38 3966 652d  -f6c6-4726-89fe-
+00000d60: 3238 6531 3033 6364 3139 3866 2e6d 7034  28e103cd198f.mp4
+00000d70: 0a0a 2323 2052 6571 7569 7265 6d65 6e74  ..## Requirement
+00000d80: 730a 0a2d 2050 7974 686f 6e20 332e 372e  s..- Python 3.7.
+00000d90: 312b 0a0a 2323 2049 7373 7565 730a 0a41  1+..## Issues..A
+00000da0: 6c6c 2066 6565 6462 6163 6b20 616e 6420  ll feedback and 
+00000db0: 6275 6720 7265 706f 7274 7320 7765 6c63  bug reports welc
+00000dc0: 6f6d 6521 2052 6570 6f72 7420 696e 2074  ome! Report in t
+00000dd0: 6865 205b 6973 7375 6573 2073 6563 7469  he [issues secti
+00000de0: 6f6e 5d28 6874 7470 733a 2f2f 6769 7468  on](https://gith
+00000df0: 7562 2e63 6f6d 2f6d 6179 6168 712f 6d61  ub.com/mayahq/ma
+00000e00: 7961 6c61 6273 2d73 646b 2d70 7974 686f  yalabs-sdk-pytho
+00000e10: 6e2f 6973 7375 6573 292c 206f 7220 6d61  n/issues), or ma
+00000e20: 696c 2075 7320 6174 2068 756d 616e 7340  il us at humans@
+00000e30: 6d61 7961 6c61 6273 2e69 6f2e 0a0a 4675  mayalabs.io...Fu
+00000e40: 6c6c 206c 6973 7420 6f66 2063 6170 6162  ll list of capab
+00000e50: 696c 6974 6965 7320 616e 6420 6c69 6d69  ilities and limi
+00000e60: 7473 205b 6865 7265 5d28 6874 7470 733a  ts [here](https:
+00000e70: 2f2f 646f 6373 2e6d 6179 616c 6162 732e  //docs.mayalabs.
+00000e80: 696f 2f63 6170 6162 696c 6974 6965 732d  io/capabilities-
+00000e90: 616e 642d 6c69 6d69 7473 292e 0a0a 0a23  and-limits)....#
+00000ea0: 2320 526f 6164 6d61 700a 2d20 5b78 5d20  # Roadmap.- [x] 
+00000eb0: 436c 6561 6e65 7220 6c6f 6773 2061 6e64  Cleaner logs and
+00000ec0: 2065 7863 6570 7469 6f6e 2068 616e 646c   exception handl
+00000ed0: 696e 670a 2d20 5b78 5d20 4465 7065 6e64  ing.- [x] Depend
+00000ee0: 656e 6379 2063 6f6e 6669 6775 7261 7469  ency configurati
+00000ef0: 6f6e 2055 5820 696d 7072 6f76 656d 656e  on UX improvemen
+00000f00: 740a 2d20 5b20 5d20 496d 706f 7274 2073  t.- [ ] Import s
+00000f10: 6b69 6c6c 2072 6570 6f73 6974 6f72 6965  kill repositorie
+00000f20: 7320 666f 7220 7265 7573 696e 6720 736b  s for reusing sk
+00000f30: 696c 6c73 2063 7265 6174 6564 2062 7920  ills created by 
+00000f40: 7573 6572 206f 7220 7072 6573 656e 7420  user or present 
+00000f50: 696e 2073 746f 7265 0a2d 205b 205d 2043  in store.- [ ] C
+00000f60: 7265 6174 6520 616e 6420 6361 6c6c 2064  reate and call d
+00000f70: 6f77 6e73 7472 6561 6d20 6175 746f 2d64  ownstream auto-d
+00000f80: 6570 6c6f 7965 6420 6675 6e63 7469 6f6e  eployed function
+00000f90: 730a 2d20 5b20 5d20 416c 6c6f 7720 6d75  s.- [ ] Allow mu
+00000fa0: 6c74 692d 7072 6f66 696c 6520 616e 6420  lti-profile and 
+00000fb0: 7465 616d 2070 726f 6669 6c65 2061 6363  team profile acc
+00000fc0: 6573 730a                                ess.
```

### Comparing `mayalabs-0.0.8/mayalabs.egg-info/SOURCES.txt` & `mayalabs-0.0.9/mayalabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.8/pyproject.toml` & `mayalabs-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mayalabs"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python SDK for Maya Labs' natural language programming paradigm"
 dependencies = [
     "requests",
     "pydantic",
     "websockets",
     "click",
     "colorama",
```

### Comparing `mayalabs-0.0.8/tests/example_1.py` & `mayalabs-0.0.9/tests/example_1.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.8/tests/example_2.py` & `mayalabs-0.0.9/tests/example_2.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.8/tests/example_3.py` & `mayalabs-0.0.9/tests/example_3.py`

 * *Files identical despite different names*

