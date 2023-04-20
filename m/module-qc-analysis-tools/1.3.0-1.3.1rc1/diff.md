# Comparing `tmp/module_qc_analysis_tools-1.3.0.tar.gz` & `tmp/module_qc_analysis_tools-1.3.1rc1.tar.gz`

## Comparing `module_qc_analysis_tools-1.3.0.tar` & `module_qc_analysis_tools-1.3.1rc1.tar`

### file list

```diff
@@ -1,28 +1,31 @@
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/.flake8
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/.gitmodules
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/tbump.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/_version.py
--rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    17034 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0     9798 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0    22732 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/SLDO.py
--rw-r--r--   0        0        0    11230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/__main__.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/globals.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/main.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/overwrite_config.py
--rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/update_chip_config.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/data/analysis_cuts.json
--rw-r--r--   0        0        0    19622 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/utils/analysis.py
--rw-r--r--   0        0        0    33978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/utils/misc.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/tests/test_cli.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/tests/test_package.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/LICENSE
--rw-r--r--   0        0        0    13096 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/README.md
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/.flake8
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/.gitmodules
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/tbump.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/_version.py
+-rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    17806 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0     9559 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/IV_MEASURE.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
+-rw-r--r--   0        0        0    23808 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/SLDO.py
+-rw-r--r--   0        0        0    11972 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/__main__.py
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/globals.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/main.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/overwrite_config.py
+-rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/update_chip_config.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/data/analysis_cuts.json
+-rw-r--r--   0        0        0    21042 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/utils/analysis.py
+-rw-r--r--   0        0        0    34380 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/utils/misc.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/tests/test_cli.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/tests/test_package.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/LICENSE
+-rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/README.md
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/pyproject.toml
+-rw-r--r--   0        0        0    15226 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/PKG-INFO
```

### Comparing `module_qc_analysis_tools-1.3.0/.gitlab-ci.yml` & `module_qc_analysis_tools-1.3.1rc1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.0/.pre-commit-config.yaml` & `module_qc_analysis_tools-1.3.1rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.0/tbump.toml` & `module_qc_analysis_tools-1.3.1rc1/tbump.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2231 2e33 2e30 220a 0a23 2045  t = "1.3.0"..# E
-00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
-00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
-00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
-00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
-00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
-00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
-00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
-00000090: 3e5c 642b 290a 2020 5c2e 0a20 2028 3f50  >\d+).  \..  (?P
-000000a0: 3c6d 696e 6f72 3e5c 642b 290a 2020 5c2e  <minor>\d+).  \.
-000000b0: 0a20 2028 3f50 3c70 6174 6368 3e5c 642b  .  (?P<patch>\d+
-000000c0: 290a 2020 2872 630a 2020 2020 283f 503c  ).  (rc.    (?P<
-000000d0: 6361 6e64 6964 6174 653e 5c64 2b29 0a20  candidate>\d+). 
-000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
-000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
-00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
-00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
-00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
-00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
-00000140: 6d70 2076 6572 7369 6f6e 3a20 312e 332e  mp version: 1.3.
-00000150: 3020 e286 9220 7b6e 6577 5f76 6572 7369  0 ... {new_versi
-00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
-00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
-00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
-00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
-000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
-000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
-000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
-000001d0: 6174 6820 6f66 2074 6865 2066 696c 652c  ath of the file,
-000001e0: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
-000001f0: 0a23 2074 6275 6d70 2e74 6f6d 6c20 6c6f  .# tbump.toml lo
-00000200: 6361 7469 6f6e 2e0a 5b5b 6669 6c65 5d5d  cation..[[file]]
-00000210: 0a73 7263 203d 2022 7462 756d 702e 746f  .src = "tbump.to
-00000220: 6d6c 220a 2320 5265 7374 7269 6374 2073  ml".# Restrict s
-00000230: 6561 7263 6820 746f 206d 616b 6520 6974  earch to make it
-00000240: 2065 7870 6c69 6369 7420 7768 7920 7462   explicit why tb
-00000250: 756d 702e 746f 6d6c 0a23 2069 7320 6576  ump.toml.# is ev
-00000260: 656e 2069 6e63 6c75 6465 6420 6173 2061  en included as a
-00000270: 2066 696c 6520 746f 2062 756d 702c 2061   file to bump, a
-00000280: 7320 6974 2077 696c 6c20 6765 740a 2320  s it will get.# 
-00000290: 6974 7320 7665 7273 696f 6e2e 6375 7272  its version.curr
-000002a0: 656e 7420 6174 7472 6962 7574 6520 6275  ent attribute bu
-000002b0: 6d70 6564 2061 6e79 7761 792e 0a73 6561  mped anyway..sea
-000002c0: 7263 6820 3d20 2242 756d 7020 7665 7273  rch = "Bump vers
-000002d0: 696f 6e3a 207b 6375 7272 656e 745f 7665  ion: {current_ve
-000002e0: 7273 696f 6e7d 20e2 8692 2022 0a0a 5b5b  rsion} ... "..[[
-000002f0: 6669 6c65 5d5d 0a73 7263 203d 2022 5245  file]].src = "RE
-00000300: 4144 4d45 2e6d 6422 0a0a 5b5b 6669 656c  ADME.md"..[[fiel
-00000310: 645d 5d0a 2320 7468 6520 6e61 6d65 206f  d]].# the name o
-00000320: 6620 7468 6520 6669 656c 640a 6e61 6d65  f the field.name
-00000330: 203d 2022 6361 6e64 6964 6174 6522 0a23   = "candidate".#
-00000340: 2074 6865 2064 6566 6175 6c74 2076 616c   the default val
-00000350: 7565 2074 6f20 7573 652c 2069 6620 7468  ue to use, if th
-00000360: 6572 6520 6973 206e 6f20 6d61 7463 680a  ere is no match.
-00000370: 6465 6661 756c 7420 3d20 2222 0a         default = "".
+00000010: 7420 3d20 2231 2e33 2e31 7263 3122 0a0a  t = "1.3.1rc1"..
+00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
+00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
+00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
+00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
+00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
+00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
+00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
+00000090: 6a6f 723e 5c64 2b29 0a20 205c 2e0a 2020  jor>\d+).  \..  
+000000a0: 283f 503c 6d69 6e6f 723e 5c64 2b29 0a20  (?P<minor>\d+). 
+000000b0: 205c 2e0a 2020 283f 503c 7061 7463 683e   \..  (?P<patch>
+000000c0: 5c64 2b29 0a20 2028 7263 0a20 2020 2028  \d+).  (rc.    (
+000000d0: 3f50 3c63 616e 6469 6461 7465 3e5c 642b  ?P<candidate>\d+
+000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
+000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
+00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
+00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
+00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
+00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
+00000140: 2242 756d 7020 7665 7273 696f 6e3a 2031  "Bump version: 1
+00000150: 2e33 2e31 7263 3120 e286 9220 7b6e 6577  .3.1rc1 ... {new
+00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
+00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
+00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
+00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
+000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
+000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
+000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
+000001d0: 2074 6865 2070 6174 6820 6f66 2074 6865   the path of the
+000001e0: 2066 696c 652c 2072 656c 6174 6976 6520   file, relative 
+000001f0: 746f 2074 6865 0a23 2074 6275 6d70 2e74  to the.# tbump.t
+00000200: 6f6d 6c20 6c6f 6361 7469 6f6e 2e0a 5b5b  oml location..[[
+00000210: 6669 6c65 5d5d 0a73 7263 203d 2022 7462  file]].src = "tb
+00000220: 756d 702e 746f 6d6c 220a 2320 5265 7374  ump.toml".# Rest
+00000230: 7269 6374 2073 6561 7263 6820 746f 206d  rict search to m
+00000240: 616b 6520 6974 2065 7870 6c69 6369 7420  ake it explicit 
+00000250: 7768 7920 7462 756d 702e 746f 6d6c 0a23  why tbump.toml.#
+00000260: 2069 7320 6576 656e 2069 6e63 6c75 6465   is even include
+00000270: 6420 6173 2061 2066 696c 6520 746f 2062  d as a file to b
+00000280: 756d 702c 2061 7320 6974 2077 696c 6c20  ump, as it will 
+00000290: 6765 740a 2320 6974 7320 7665 7273 696f  get.# its versio
+000002a0: 6e2e 6375 7272 656e 7420 6174 7472 6962  n.current attrib
+000002b0: 7574 6520 6275 6d70 6564 2061 6e79 7761  ute bumped anywa
+000002c0: 792e 0a73 6561 7263 6820 3d20 2242 756d  y..search = "Bum
+000002d0: 7020 7665 7273 696f 6e3a 207b 6375 7272  p version: {curr
+000002e0: 656e 745f 7665 7273 696f 6e7d 20e2 8692  ent_version} ...
+000002f0: 2022 0a0a 5b5b 6669 6c65 5d5d 0a73 7263   "..[[file]].src
+00000300: 203d 2022 5245 4144 4d45 2e6d 6422 0a0a   = "README.md"..
+00000310: 5b5b 6669 656c 645d 5d0a 2320 7468 6520  [[field]].# the 
+00000320: 6e61 6d65 206f 6620 7468 6520 6669 656c  name of the fiel
+00000330: 640a 6e61 6d65 203d 2022 6361 6e64 6964  d.name = "candid
+00000340: 6174 6522 0a23 2074 6865 2064 6566 6175  ate".# the defau
+00000350: 6c74 2076 616c 7565 2074 6f20 7573 652c  lt value to use,
+00000360: 2069 6620 7468 6572 6520 6973 206e 6f20   if there is no 
+00000370: 6d61 7463 680a 6465 6661 756c 7420 3d20  match.default = 
+00000380: 2222 0a                                  "".
```

### Comparing `module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,33 @@
 from datetime import datetime
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 import typer
 from module_qc_data_tools import (
+    get_layer_from_sn,
     load_json,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
 from module_qc_analysis_tools import __version__
 from module_qc_analysis_tools.cli.globals import (
     CONTEXT_SETTINGS,
     OPTIONS,
     FitMethod,
     LogLevel,
 )
-from module_qc_analysis_tools.utils.analysis import perform_qc_analysis, submit_results
+from module_qc_analysis_tools.utils.analysis import (
+    check_layer,
+    perform_qc_analysis,
+    submit_results,
+)
 from module_qc_analysis_tools.utils.misc import (
     DataExtractor,
     JsonChecker,
     bcolors,
     get_inputs,
     get_qc_config,
     get_time_stamp,
@@ -37,15 +42,15 @@
 
 
 @app.command()
 def main(
     input_meas: Path = OPTIONS["input_meas"],
     base_output_dir: Path = OPTIONS["output_dir"],
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
-    layer: str = OPTIONS["layer"],
+    input_layer: str = OPTIONS["layer"],
     permodule: bool = OPTIONS["permodule"],
     submit: bool = OPTIONS["submit"],
     site: str = OPTIONS["site"],
     fit_method: FitMethod = OPTIONS["fit_method"],
     verbosity: LogLevel = OPTIONS["verbosity"],
 ):
     log = logging.getLogger(__name__)
@@ -81,18 +86,15 @@
         log.info(f" Loading {filename}")
         meas_timestamp = get_time_stamp(filename)
         inputDFs = load_json(filename)
         log.debug(
             f" There are results from {len(inputDFs)} chip(s) stored in this file"
         )
         for inputDF in inputDFs:
-            qcframe = inputDF.get_results()
-            metadata = qcframe.get_meta_data()
-
-            """ Check file integrity  """
+            """Check file integrity"""
             checker = JsonChecker(inputDF, test_type)
 
             try:
                 checker.check()
             except BaseException as exc:
                 log.exception(exc)
                 log.warning(
@@ -101,14 +103,34 @@
                     + bcolors.ENDC
                 )
                 continue
             else:
                 log.debug(" JsonChecker check passed!")
                 pass
 
+            """  Get info  """
+            qcframe = inputDF.get_results()
+            metadata = qcframe.get_meta_data()
+
+            if input_layer == "Unknown":
+                try:
+                    layer = get_layer_from_sn(metadata.get("ModuleSN"))
+                except Exception:
+                    log.error(bcolors.WARNING + " Something went wrong." + bcolors.ENDC)
+            else:
+                log.warning(
+                    bcolors.WARNING
+                    + " Overwriting default layer config {} with manual input {}!".format(
+                        get_layer_from_sn(metadata.get("ModuleSN")), input_layer
+                    )
+                    + bcolors.ENDC
+                )
+                layer = input_layer
+            check_layer(layer)
+
             try:
                 chipname = metadata.get("Name")
                 log.debug(f" Found chip name = {chipname} from chip config")
             except Exception:
                 log.warning(
                     bcolors.WARNING
                     + "Chip name not found in input from {filename}, skipping."
```

### Comparing `module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py` & `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,34 @@
 import logging
 from datetime import datetime
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 import typer
-from module_qc_data_tools import load_json, outputDataFrame, qcDataFrame, save_dict_list
+from module_qc_data_tools import (
+    get_layer_from_sn,
+    load_json,
+    outputDataFrame,
+    qcDataFrame,
+    save_dict_list,
+)
 
 from module_qc_analysis_tools import __version__
 from module_qc_analysis_tools.cli.globals import (
     CONTEXT_SETTINGS,
     OPTIONS,
     FitMethod,
     LogLevel,
 )
-from module_qc_analysis_tools.utils.analysis import perform_qc_analysis, submit_results
+from module_qc_analysis_tools.utils.analysis import (
+    check_layer,
+    perform_qc_analysis,
+    submit_results,
+)
 from module_qc_analysis_tools.utils.misc import (
     DataExtractor,
     JsonChecker,
     bcolors,
     get_inputs,
     get_qc_config,
     get_time_stamp,
@@ -174,15 +184,15 @@
 
 
 @app.command()
 def main(
     input_meas: Path = OPTIONS["input_meas"],
     base_output_dir: Path = OPTIONS["output_dir"],
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
-    layer: str = OPTIONS["layer"],
+    input_layer: str = OPTIONS["layer"],
     permodule: bool = OPTIONS["permodule"],
     submit: bool = OPTIONS["submit"],
     site: str = OPTIONS["site"],
     fit_method: FitMethod = OPTIONS["fit_method"],
     verbosity: LogLevel = OPTIONS["verbosity"],
 ):
     log.setLevel(verbosity.value)
@@ -226,17 +236,51 @@
         )
 
         chipnames = []
         results = {}
         data = {}
         int_biases = {}
         for inputDF in inputDFs:
+            """Check file integrity"""
+            checker = JsonChecker(inputDF, test_type)
+
+            try:
+                checker.check()
+            except BaseException as exc:
+                log.exception(exc)
+                log.warning(
+                    bcolors.WARNING
+                    + " JsonChecker check not passed, skipping this input."
+                    + bcolors.ENDC
+                )
+                continue
+            else:
+                log.debug(" JsonChecker check passed!")
+                pass
+
+            """ Get info """
             qcframe = inputDF.get_results()
             metadata = qcframe.get_meta_data()
 
+            if input_layer == "Unknown":
+                try:
+                    layer = get_layer_from_sn(metadata.get("ModuleSN"))
+                except Exception:
+                    log.error(bcolors.WARNING + " Something went wrong." + bcolors.ENDC)
+            else:
+                log.warning(
+                    bcolors.WARNING
+                    + " Overwriting default layer config {} with manual input {}!".format(
+                        get_layer_from_sn(metadata.get("ModuleSN")), input_layer
+                    )
+                    + bcolors.ENDC
+                )
+                layer = input_layer
+            check_layer(layer)
+
             # Read chipname from input DF
             try:
                 chipname = metadata.get("Name")
                 chipnames.append(chipname)
                 log.debug(f" Found chip name = {chipname} from chip config")
             except Exception:
                 log.warning(
@@ -257,31 +301,14 @@
                     "MEASUREMENT_VERSION",
                     qcframe.get_properties().get(test_type + "_MEASUREMENT_VERSION"),
                 )
                 data[chipname].add_meta_data("QC_LAYER", layer)
                 data[chipname]._meta_data.update(metadata)
                 int_biases[chipname] = {}
 
-            """ Check file integrity  """
-            checker = JsonChecker(inputDF, test_type)
-
-            try:
-                checker.check()
-            except BaseException as exc:
-                log.exception(exc)
-                log.warning(
-                    bcolors.WARNING
-                    + " JsonChecker check not passed, skipping this input."
-                    + bcolors.ENDC
-                )
-                continue
-            else:
-                log.debug(" JsonChecker check passed!")
-                pass
-
             """  Calculate quanties   """
             # Vmux conversion is embedded.
             extractor = DataExtractor(inputDF, test_type)
             calculated_data = extractor.calculate()
             Vmux_map = getVmuxMap()
             Imux_map = getImuxMap()
 
@@ -330,17 +357,17 @@
                 data[chipname].add_parameter("AR_TEMP_POLY_BOTTOM", EMPTY_VAL)
                 data[chipname].add_parameter("AR_TEMP_NF_TOP", EMPTY_VAL)
                 data[chipname].add_parameter("AR_TEMP_NF_BOTTOM", EMPTY_VAL)
                 data[chipname].add_parameter("AR_RING_OSCILATOR_A", [EMPTY_VAL] * 16)
                 data[chipname].add_parameter("AR_RING_OSCILATOR_B", [EMPTY_VAL] * 16)
                 # Load values to dictionary for QC analysis
                 tmpresults.update({"ChipNTC_vs_ExtExt": AR_TEMP_NTC - AR_TEMP_EXT})
-                tmpresults.update({"ASLO_ChipNTC": AR_TEMP_ASLDO - AR_TEMP_NTC})
-                tmpresults.update({"DSLD_ChipNTC": AR_TEMP_DSLDO - AR_TEMP_NTC})
-                tmpresults.update({"ACB_ChipNTC": AR_TEMP_ACB - AR_TEMP_NTC})
+                tmpresults.update({"ASLDO_vs_ChipNTC": AR_TEMP_ASLDO - AR_TEMP_NTC})
+                tmpresults.update({"DSLDO_vs_ChipNTC": AR_TEMP_DSLDO - AR_TEMP_NTC})
+                tmpresults.update({"ACB_vs_ChipNTC": AR_TEMP_ACB - AR_TEMP_NTC})
 
             elif inputDF._subtestType == "AR_VDD":
                 vdda = calculated_data["VDDA"]["Values"].tolist()
                 vddd = calculated_data["VDDD"]["Values"].tolist()
                 trimA = calculated_data["SldoTrimA"]["Values"].tolist()
                 trimD = calculated_data["SldoTrimD"]["Values"].tolist()
                 # Add parameters for output file
```

### Comparing `module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,29 @@
 import logging
 from datetime import datetime
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 import typer
-from module_qc_data_tools import load_json, outputDataFrame, qcDataFrame, save_dict_list
+from module_qc_data_tools import (
+    get_layer_from_sn,
+    load_json,
+    outputDataFrame,
+    qcDataFrame,
+    save_dict_list,
+)
 
 from module_qc_analysis_tools import __version__
 from module_qc_analysis_tools.cli.globals import CONTEXT_SETTINGS, OPTIONS, LogLevel
-from module_qc_analysis_tools.utils.analysis import perform_qc_analysis, submit_results
+from module_qc_analysis_tools.utils.analysis import (
+    check_layer,
+    perform_qc_analysis,
+    submit_results,
+)
 from module_qc_analysis_tools.utils.misc import (
     DataExtractor,
     JsonChecker,
     bcolors,
     get_inputs,
     get_qc_config,
     get_time_stamp,
@@ -25,15 +35,15 @@
 
 
 @app.command()
 def main(
     input_meas: Path = OPTIONS["input_meas"],
     base_output_dir: Path = OPTIONS["output_dir"],
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
-    layer: str = OPTIONS["layer"],
+    input_layer: str = OPTIONS["layer"],
     permodule: bool = OPTIONS["permodule"],
     submit: bool = OPTIONS["submit"],
     site: str = OPTIONS["site"],
     verbosity: LogLevel = OPTIONS["verbosity"],
 ):
     log = logging.getLogger(__name__)
     log.setLevel(verbosity.value)
@@ -70,18 +80,15 @@
         meas_timestamp = get_time_stamp(filename)
         inputDFs = load_json(filename)
 
         log.debug(
             f" There are results from {len(inputDFs)} chip(s) stored in this file"
         )
         for inputDF in inputDFs:
-            qcframe = inputDF.get_results()
-            metadata = qcframe.get_meta_data()
-
-            """ Check file integrity  """
+            """Check file integrity"""
             checker = JsonChecker(inputDF, f"{test_type}")
 
             try:
                 checker.check()
             except BaseException as exc:
                 log.exception(exc)
                 log.warning(
@@ -90,14 +97,34 @@
                     + bcolors.ENDC
                 )
                 continue
             else:
                 log.debug(" JsonChecker check passed!")
                 pass
 
+            """  Get info  """
+            qcframe = inputDF.get_results()
+            metadata = qcframe.get_meta_data()
+
+            if input_layer == "Unknown":
+                try:
+                    layer = get_layer_from_sn(metadata.get("ModuleSN"))
+                except Exception:
+                    log.error(bcolors.WARNING + " Something went wrong." + bcolors.ENDC)
+            else:
+                log.warning(
+                    bcolors.WARNING
+                    + " Overwriting default layer config {} with manual input {}!".format(
+                        get_layer_from_sn(metadata.get("ModuleSN")), input_layer
+                    )
+                    + bcolors.ENDC
+                )
+                layer = input_layer
+            check_layer(layer)
+
             try:
                 chipname = metadata.get("Name")
                 log.debug(f" Found chip name = {chipname} from chip config")
             except Exception:
                 log.warning(
                     bcolors.WARNING
                     + "Chip name not found in input from {filename}, skipping."
@@ -110,19 +137,35 @@
             extractor = DataExtractor(inputDF, f"{test_type}")
             calculated_data = extractor.calculate()
 
             """        Plotting       """
             CapMeas = calculated_data.get("CapMeas").get("Values")
             CapMeasPar = calculated_data.get("CapMeasPar").get("Values")
             VDDAcapmeas = calculated_data.get("VDDAcapmeas").get("Values")
+            ImuxGnds = calculated_data.get("Imux63").get("Values")
 
             allCpix = []
             for i in range(len(CapMeas)):
-                cmeas = abs(CapMeas[i] / (VDDAcapmeas[i] * 10000000))
-                cpar = abs(CapMeasPar[i] / (VDDAcapmeas[i] * 10000000))
+                cmeas = abs(
+                    CapMeas[i]
+                    / (
+                        (VDDAcapmeas[i] - (extractor.rImux * CapMeas[i] + ImuxGnds[i]))
+                        * 10000000
+                    )
+                )
+                cpar = abs(
+                    CapMeasPar[i]
+                    / (
+                        (
+                            VDDAcapmeas[i]
+                            - (extractor.rImux * CapMeasPar[i] + ImuxGnds[i])
+                        )
+                        * 10000000
+                    )
+                )
                 cpix = ((cmeas - cpar) / 100) - 0.48e-15
                 allCpix += [cpix * 1e15]
 
             avgCpix = sum(allCpix) / len(allCpix)
 
             fig, ax1 = plt.subplots()
             ax1.plot(
```

### Comparing `module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/SLDO.py` & `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/SLDO.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 from datetime import datetime
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 import typer
 from module_qc_data_tools import (
+    get_layer_from_sn,
     load_json,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
 from module_qc_analysis_tools import __version__
 from module_qc_analysis_tools.cli.globals import (
     CONTEXT_SETTINGS,
     OPTIONS,
     FitMethod,
     LogLevel,
 )
 from module_qc_analysis_tools.utils.analysis import (
+    check_layer,
     get_n_chips,
     get_nominal_current,
     get_nominal_RextA,
     get_nominal_RextD,
     get_nominal_Voffs,
     perform_qc_analysis,
     submit_results,
@@ -45,15 +47,15 @@
 
 
 @app.command()
 def main(
     input_meas: Path = OPTIONS["input_meas"],
     base_output_dir: Path = OPTIONS["output_dir"],
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
-    layer: str = OPTIONS["layer"],
+    input_layer: str = OPTIONS["layer"],
     permodule: bool = OPTIONS["permodule"],
     submit: bool = OPTIONS["submit"],
     site: str = OPTIONS["site"],
     nChips: int = OPTIONS["nchips"],
     fit_method: FitMethod = OPTIONS["fit_method"],
     verbosity: LogLevel = OPTIONS["verbosity"],
     lp_enable: bool = OPTIONS["lp_enable"],
@@ -73,20 +75,14 @@
     log.info(" =======================================")
     log.info(" \tPerforming SLDO analysis")
     log.info(" =======================================")
     log.info("")
 
     test_type = Path(__file__).stem
 
-    # SLDO parameters
-    RextA = get_nominal_RextA(layer)
-    RextD = get_nominal_RextD(layer)
-    if nChips == 0:
-        nChips = get_n_chips(layer)
-
     allinputs = get_inputs(input_meas, test_type)
     qc_config = get_qc_config(qc_criteria_path, test_type)
 
     time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
     output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
     output_dir.mkdir(parents=True, exist_ok=False)
 
@@ -98,17 +94,65 @@
         meas_timestamp = get_time_stamp(filename)
         inputDFs = load_json(filename)
 
         log.debug(
             f" There are results from {len(inputDFs)} chip(s) stored in this file"
         )
         for inputDF in inputDFs:
+            """Check file integrity"""
+            checker = JsonChecker(inputDF, test_type)
+
+            try:
+                checker.check()
+            except BaseException as exc:
+                log.exception(exc)
+                log.error(
+                    bcolors.ERROR
+                    + " JsonChecker check not passed, skipping this input."
+                    + bcolors.ENDC
+                )
+                continue
+            else:
+                log.debug(" JsonChecker check passed!")
+                pass
+
+            """  Get info  """
             qcframe = inputDF.get_results()
             metadata = qcframe.get_meta_data()
 
+            if input_layer == "Unknown":
+                try:
+                    layer = get_layer_from_sn(metadata.get("ModuleSN"))
+                except Exception:
+                    log.error(bcolors.WARNING + " Something went wrong." + bcolors.ENDC)
+            else:
+                log.warning(
+                    bcolors.WARNING
+                    + " Overwriting default layer config {} with manual input {}!".format(
+                        get_layer_from_sn(metadata.get("ModuleSN")), input_layer
+                    )
+                    + bcolors.ENDC
+                )
+                layer = input_layer
+            check_layer(layer)
+
+            # SLDO parameters
+            RextA = get_nominal_RextA(layer)
+            RextD = get_nominal_RextD(layer)
+            if nChips == 0:
+                nChips = get_n_chips(layer)
+            else:
+                log.warning(
+                    bcolors.WARNING
+                    + " Overwriting default number of chips ({}) with manual input ({})!".format(
+                        get_n_chips(layer), nChips
+                    )
+                    + bcolors.ENDC
+                )
+
             try:
                 kShuntA = (
                     metadata.get("ChipConfigs")
                     .get("RD53B")
                     .get("Parameter")
                     .get("KShuntA")
                 )
@@ -151,31 +195,14 @@
             R_eff = 1.0 / ((kShuntA / RextA) + (kShuntD / RextD)) / nChips
 
             Vofs = get_nominal_Voffs(layer, lp_enable)
 
             p = np.poly1d([R_eff, Vofs])
             p1 = np.poly1d([R_eff, 0])
 
-            """ Check file integrity  """
-            checker = JsonChecker(inputDF, test_type)
-
-            try:
-                checker.check()
-            except BaseException as exc:
-                log.exception(exc)
-                log.error(
-                    bcolors.ERROR
-                    + " JsonChecker check not passed, skipping this input."
-                    + bcolors.ENDC
-                )
-                continue
-            else:
-                log.debug(" JsonChecker check passed!")
-                pass
-
             """  Calculate quanties   """
             extractor = DataExtractor(inputDF, test_type)
             calculated_data = extractor.calculate()
 
             passes_qc = True
 
             # Plot parameters
```

### Comparing `module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,33 @@
 from datetime import datetime
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 import typer
 from module_qc_data_tools import (
+    get_layer_from_sn,
     load_json,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
 from module_qc_analysis_tools import __version__
 from module_qc_analysis_tools.cli.globals import (
     CONTEXT_SETTINGS,
     OPTIONS,
     FitMethod,
     LogLevel,
 )
-from module_qc_analysis_tools.utils.analysis import perform_qc_analysis, submit_results
+from module_qc_analysis_tools.utils.analysis import (
+    check_layer,
+    perform_qc_analysis,
+    submit_results,
+)
 from module_qc_analysis_tools.utils.misc import (
     DataExtractor,
     JsonChecker,
     bcolors,
     get_inputs,
     get_qc_config,
     get_time_stamp,
@@ -37,15 +42,15 @@
 
 
 @app.command()
 def main(
     input_meas: Path = OPTIONS["input_meas"],
     base_output_dir: Path = OPTIONS["output_dir"],
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
-    layer: str = OPTIONS["layer"],
+    input_layer: str = OPTIONS["layer"],
     permodule: bool = OPTIONS["permodule"],
     submit: bool = OPTIONS["submit"],
     site: str = OPTIONS["site"],
     fit_method: FitMethod = OPTIONS["fit_method"],
     verbosity: LogLevel = OPTIONS["verbosity"],
 ):
     log = logging.getLogger(__name__)
@@ -84,31 +89,15 @@
         meas_timestamp = get_time_stamp(filename)
         inputDFs = load_json(filename)
 
         log.debug(
             f" There are results from {len(inputDFs)} chip(s) stored in this file"
         )
         for inputDF in inputDFs:
-            qcframe = inputDF.get_results()
-            metadata = qcframe.get_meta_data()
-
-            """ Determine test type """
-            try:
-                testname = inputDF._subtestType
-                testprefix = testname.split("_")[0] + "_" + testname.split("_")[1]
-                testsuffix = testname.split(testprefix)[1]
-            except Exception:
-                log.error(
-                    bcolors.ERROR
-                    + f" {filename}.json does not have subtestType, which is needed for VCAL_CALIBRATION analysis, skipping!"
-                    + bcolors.ENDC
-                )
-                continue
-
-            """ Check file integrity  """
+            """Check file integrity"""
             checker = JsonChecker(inputDF, test_type)
 
             try:
                 checker.check()
             except BaseException as exc:
                 log.exception(exc)
                 log.warning(
@@ -117,14 +106,47 @@
                     + bcolors.ENDC
                 )
                 continue
             else:
                 log.debug(" JsonChecker check passed!")
                 pass
 
+            """  Get info  """
+            qcframe = inputDF.get_results()
+            metadata = qcframe.get_meta_data()
+
+            if input_layer == "Unknown":
+                try:
+                    layer = get_layer_from_sn(metadata.get("ModuleSN"))
+                except Exception:
+                    log.error(bcolors.WARNING + " Something went wrong." + bcolors.ENDC)
+            else:
+                log.warning(
+                    bcolors.WARNING
+                    + " Overwriting default layer config {} with manual input {}!".format(
+                        get_layer_from_sn(metadata.get("ModuleSN")), input_layer
+                    )
+                    + bcolors.ENDC
+                )
+                layer = input_layer
+            check_layer(layer)
+
+            """ Determine test type """
+            try:
+                testname = inputDF._subtestType
+                testprefix = testname.split("_")[0] + "_" + testname.split("_")[1]
+                testsuffix = testname.split(testprefix)[1]
+            except Exception:
+                log.error(
+                    bcolors.ERROR
+                    + f" {filename}.json does not have subtestType, which is needed for VCAL_CALIBRATION analysis, skipping!"
+                    + bcolors.ENDC
+                )
+                continue
+
             try:
                 chipname = metadata.get("Name")
                 log.debug(f" Found chip name = {chipname} from chip config")
             except Exception:
                 log.warning(
                     bcolors.WARNING
                     + "Chip name not found in input from {filename}, skipping."
```

### Comparing `module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/globals.py` & `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/globals.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/main.py` & `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,18 +8,21 @@
 import module_qc_analysis_tools
 from module_qc_analysis_tools.cli.ADC_CALIBRATION import main as adc_calibration
 from module_qc_analysis_tools.cli.ANALOG_READBACK import main as analog_readback
 from module_qc_analysis_tools.cli.globals import CONTEXT_SETTINGS
 from module_qc_analysis_tools.cli.INJECTION_CAPACITANCE import (
     main as injection_capacitance,
 )
+from module_qc_analysis_tools.cli.IV_MEASURE import main as iv_measure
+from module_qc_analysis_tools.cli.MASS_MEASUREMENT import main as mass
 from module_qc_analysis_tools.cli.overwrite_config import main as overwrite_config
 from module_qc_analysis_tools.cli.SLDO import main as sldo
 from module_qc_analysis_tools.cli.update_chip_config import main as update_chip_config
 from module_qc_analysis_tools.cli.VCAL_CALIBRATION import main as vcal_calibration
+from module_qc_analysis_tools.cli.VISUAL_INSPECTION import main as visual_inspection
 
 # subcommands
 app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 app_analysis = typer.Typer(context_settings=CONTEXT_SETTINGS)
 app_config = typer.Typer(context_settings=CONTEXT_SETTINGS)
 app.add_typer(app_analysis, name="analysis")
 app.add_typer(app_config, name="config")
@@ -44,12 +47,15 @@
 
 
 app_analysis.command("adc-calibration")(adc_calibration)
 app_analysis.command("analog-readback")(analog_readback)
 app_analysis.command("injection-capacitance")(injection_capacitance)
 app_analysis.command("sldo")(sldo)
 app_analysis.command("vcal-calibration")(vcal_calibration)
+app_analysis.command("mass-measurement")(mass)
+app_analysis.command("iv-measure")(iv_measure)
+app_analysis.command("visual-inspection")(visual_inspection)
 app_config.command("overwrite")(overwrite_config)
 app_config.command("update")(update_chip_config)
 
 # for generating documentation using mkdocs-click
 typer_click_object = typer.main.get_command(app)
```

### Comparing `module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/overwrite_config.py` & `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/overwrite_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/cli/update_chip_config.py` & `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/update_chip_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/data/analysis_cuts.json` & `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/data/analysis_cuts.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7744212962962962%*

 * *Differences: {"'ANALOG_READBACK'": "{'AR_VDDA_VS_TRIM': {replace: OrderedDict([('VDD_TRIM_0', [0.98355, "*

 * *                      "1.1593]), ('VDD_step_size', [0.01665, 0.02035])])}, 'AR_VDDD_VS_TRIM': "*

 * *                      "{replace: OrderedDict([('VDD_TRIM_0', [0.98355, 1.1593]), ('VDD_step_size', "*

 * *                      "[0.01665, 0.02035])])}, 'ASLDO_vs_ChipNTC': [-8, 2], 'DSLDO_vs_ChipNTC': "*

 * *                      "[-8, 2], 'ACB_vs_ChipNTC': [-8, 2], delete: ['ASLO_ChipNTC', "*

 * *                      "'DSLD_ChipNTC', […]*

```diff
@@ -6,15 +6,15 @@
         ],
         "ADC_CALIBRATION_SLOPE": [
             0.15,
             0.224
         ]
     },
     "ANALOG_READBACK": {
-        "ACB_ChipNTC": [
+        "ACB_vs_ChipNTC": [
             -8,
             2
         ],
         "AR_NOMINAL_SETTINGS": {
             "AnaGND30": [
                 0.02,
                 0.025
@@ -128,41 +128,54 @@
                 0.625
             ],
             "VrefOVP": [
                 1.768,
                 2.161
             ]
         },
-        "AR_VDDA_VS_TRIM": [
-            1,
-            1.4
-        ],
-        "AR_VDDD_VS_TRIM": [
-            1,
-            1.4
-        ],
-        "ASLO_ChipNTC": [
+        "AR_VDDA_VS_TRIM": {
+            "VDD_TRIM_0": [
+                0.98355,
+                1.1593
+            ],
+            "VDD_step_size": [
+                0.01665,
+                0.02035
+            ]
+        },
+        "AR_VDDD_VS_TRIM": {
+            "VDD_TRIM_0": [
+                0.98355,
+                1.1593
+            ],
+            "VDD_step_size": [
+                0.01665,
+                0.02035
+            ]
+        },
+        "ASLDO_vs_ChipNTC": [
             -8,
             2
         ],
         "ChipNTC_vs_ExtExt": [
             -2,
             2
         ],
-        "DSLD_ChipNTC": [
+        "DSLDO_vs_ChipNTC": [
             -8,
             2
         ]
     },
     "INJECTION_CAPACITANCE": {
         "INJ_CAPACITANCE": [
             6.74,
             9.0
         ]
     },
+    "MASS_MEASUREMENT": {},
     "SLDO": {
         "SLDO_IINA": {
             "LOne": [
                 0.681,
                 0.735
             ],
             "LTwo": [
@@ -180,16 +193,16 @@
                 0.971
             ],
             "LTwo": [
                 0.846,
                 0.905
             ],
             "LZero": [
-                1.177,
-                1.24
+                0.997,
+                1.06
             ]
         },
         "SLDO_IREF": [
             3.7,
             4.3
         ],
         "SLDO_ISHUNTA": {
```

### Comparing `module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/utils/analysis.py` & `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/utils/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import logging
 import sys
 from pathlib import Path
 
+import numpy as np
+
 from module_qc_analysis_tools.utils.misc import bcolors, getImuxMap, getVmuxMap
 
 log = logging.getLogger(__name__)
 log.setLevel("INFO")
 
 
 def format_text():
@@ -115,20 +117,19 @@
 def get_key(mydict, val):
     for key, value in mydict.items():
         if val == value:
             return key
     return -1
 
 
-def perform_qc_analysis_AR(
+def perform_qc_analysis_AR_NOMINAL_SETTINGS(
     _test_type, qc_config, _layer_name, results, verbosity="INFO"
 ):
     log.setLevel(verbosity)
-    # Basically the same function as perform_qc_analysis
-    # minus all the initial checks which have already been performed.
+    # QC analysis for AR_NOMINAL_SETTINGS
 
     passes_qc_overall = True
     VmuxMap = getVmuxMap()
     ImuxMap = getImuxMap()
     if len(VmuxMap.keys()) + len(ImuxMap.keys()) != len(results):
         log.error(
             bcolors.ERROR
@@ -170,14 +171,53 @@
         else:
             print_output_fail(key, results[index], lower_bound, upper_bound)
         passes_qc_overall = passes_qc_overall and passes_qc_test
 
     return passes_qc_overall
 
 
+def perform_qc_analysis_AR_VDD_Trim(
+    _test_type, qc_config, _layer_name, results, key, verbosity="INFO"
+):
+    log.setLevel(verbosity)
+    # QC analysis for VDDA_VS_TRIM and VDDD_VS_TRIM
+    pass_vdd_vs_trim_test = True
+
+    # Fist VDD value must satisfy requirements
+    tmp_pass_qc = True
+    lower_bound_vdd = qc_config.get("VDD_TRIM_0")[0]
+    upper_bound_vdd = qc_config.get("VDD_TRIM_0")[1]
+    if (results[0] < lower_bound_vdd) or (results[0] > upper_bound_vdd):
+        tmp_pass_qc = False
+    if tmp_pass_qc:
+        print_output_pass(f"{key}_0", results[0], lower_bound_vdd, upper_bound_vdd)
+    else:
+        print_output_fail(f"{key}_0", results[0], lower_bound_vdd, upper_bound_vdd)
+    pass_vdd_vs_trim_test = pass_vdd_vs_trim_test and tmp_pass_qc
+
+    # The trim step size (change in voltage per DAC step) must satisfy requirements
+    VDD_dV_list = np.diff(np.array(results))
+    lower_bound_dv = qc_config.get("VDD_step_size")[0]
+    upper_bound_dv = qc_config.get("VDD_step_size")[1]
+    dV_fail = (VDD_dV_list < lower_bound_dv) | (VDD_dV_list > upper_bound_dv)
+    pass_vdd_vs_trim_test = pass_vdd_vs_trim_test and np.any(dV_fail)
+    for i in range(len(VDD_dV_list)):
+        tmp_pass_qc = not dV_fail[i]
+        if tmp_pass_qc:
+            print_output_pass(
+                f"{key}_{i+1}_STEP_SIZE", VDD_dV_list[i], lower_bound_dv, upper_bound_dv
+            )
+        else:
+            print_output_fail(
+                f"{key}_{i+1}_STEP_SIZE", VDD_dV_list[i], lower_bound_dv, upper_bound_dv
+            )
+
+    return pass_vdd_vs_trim_test
+
+
 def perform_qc_analysis(test_type, qc_config, layer_name, results, verbosity="INFO"):
     log.setLevel(verbosity)
     log.info("")
     log.info("Performing QC analysis!")
     log.info("")
 
     qc_selections = qc_config[test_type]
@@ -201,19 +241,32 @@
                 + bcolors.ENDC
             )
             continue
         check_qc_selections.pop(key)
 
         # Handle AR_NOMINAL_SETTINGS in completely different function, for now...
         if key == "AR_NOMINAL_SETTINGS":
-            passes_qc_test = perform_qc_analysis_AR(
+            passes_qc_test = perform_qc_analysis_AR_NOMINAL_SETTINGS(
+                test_type,
+                qc_selections.get(key),
+                layer_name,
+                results.get(key),
+                verbosity,
+            )
+            passes_qc_overall = passes_qc_overall and passes_qc_test
+            continue
+
+        # Handle AR_VDDA_VS_TRIM and AR_VDD_VS_TRIM separately
+        if ("AR_VDDA_VS_TRIM" in key) or ("AR_VDDD_VS_TRIM" in key):
+            passes_qc_test = perform_qc_analysis_AR_VDD_Trim(
                 test_type,
                 qc_selections.get(key),
                 layer_name,
                 results.get(key),
+                key,
                 verbosity,
             )
             passes_qc_overall = passes_qc_overall and passes_qc_test
             continue
 
         log.debug(f" QC selections for {key}: {qc_selections.get(key)}")
         if type(qc_selections.get(key)) is list:
@@ -235,33 +288,20 @@
                     + bcolors.ENDC
                 )
                 continue
             lower_bound = layer_bounds[0]
             upper_bound = layer_bounds[1]
 
         passes_qc_test = True
-        if ("AR_VDDA_VS_TRIM" in key) or ("AR_VDDD_VS_TRIM" in key):
-            # All values in list must satisfy requirements
-            for elem in results.get(key):
-                tmp_pass_qc = True
-                if (elem < lower_bound) or (elem > upper_bound):
-                    passes_qc_test = False
-                    tmp_pass_qc = False
-                if tmp_pass_qc:
-                    print_output_pass(key, elem, lower_bound, upper_bound)
-                else:
-                    print_output_fail(key, elem, lower_bound, upper_bound)
-
+        if (results.get(key) < lower_bound) or (results.get(key) > upper_bound):
+            passes_qc_test = False
+        if passes_qc_test:
+            print_output_pass(key, results.get(key), lower_bound, upper_bound)
         else:
-            if (results.get(key) < lower_bound) or (results.get(key) > upper_bound):
-                passes_qc_test = False
-            if passes_qc_test:
-                print_output_pass(key, results.get(key), lower_bound, upper_bound)
-            else:
-                print_output_fail(key, results.get(key), lower_bound, upper_bound)
+            print_output_fail(key, results.get(key), lower_bound, upper_bound)
         passes_qc_overall = passes_qc_overall and passes_qc_test
     if len(check_qc_selections) > 0:
         for key in check_qc_selections:
             log.error(
                 bcolors.ERROR
                 + f" Parameter from chip for QC selection of {key} was not passed to analysis - please fix!"
                 + bcolors.ENDC
```

### Comparing `module_qc_analysis_tools-1.3.0/src/module_qc_analysis_tools/utils/misc.py` & `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/utils/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -230,14 +230,26 @@
             log.error(
                 bcolors.ERROR
                 + f"Required testtype of the file '{required_testtype}' is not matched to '{testtype_from_file}' from the file! "
                 + bcolors.ENDC
             )
             raise KeyError()
 
+    def check_metadata(self):
+        required_metadata = ["ModuleSN"]
+        input_metadata = self.qcdataframe.get_identifiers()
+        for key in required_metadata:
+            if input_metadata[key] is None:
+                log.error(
+                    bcolors.ERROR
+                    + f" Metadata not complete: {key} missing"
+                    + bcolors.ENDC
+                )
+                raise KeyError()
+
     def check_keywords_exist(self) -> None:
         for required_keyword in self.required_keywords:
             if required_keyword not in self.qcdataframe._data.keys():
                 log.error(
                     bcolors.ERROR + f"{required_keyword} not found! " + bcolors.ENDC
                 )
                 raise KeyError()
@@ -305,14 +317,15 @@
 
     def check(self) -> None:
         self.check_testtype()
         self.check_keywords_exist()
         self.check_keywords_length()
         self.check_positive_values()
         self.check_parameters_overwritten()
+        self.check_metadata()
 
 
 class DataExtractor(JsonChecker):
     def __init__(self, inputDF, test_type_from_script) -> None:
         super().__init__(inputDF, test_type_from_script)
         qcframe = inputDF.get_results()
         self.df = qcframe._data
@@ -327,185 +340,184 @@
         )
         self.kIshuntA = qcframe._meta_data["ChipConfigs"]["RD53B"]["Parameter"].get(
             "KSenseShuntA", 26000.0
         )
         self.kIshuntD = qcframe._meta_data["ChipConfigs"]["RD53B"]["Parameter"].get(
             "KSenseShuntD", 26000.0
         )
-        self.VmuxGrd = "Vmux30"
-        self.ImuxGrd = "Imux63"
+        self.VmuxGnd = "Vmux30"
+        self.ImuxGnd = "Imux63"
 
     def getQuantity(self, key):
         return getattr(self, key, lambda: False)()
 
     def Vmux0(self):
         return {
             getVmuxMap()[0]: {
                 "X": self.df["Vmux0"]["X"],
                 "Unit": self.df["Vmux0"]["Unit"],
                 "Values": (
-                    self.df["Vmux0"]["Values"] - self.df[self.VmuxGrd]["Values"]
+                    self.df["Vmux0"]["Values"] - self.df[self.VmuxGnd]["Values"]
                 ),
             }
         }
 
     def Vmux2(self):
         return {
             getVmuxMap()[2]: {
                 "X": self.df["Vmux2"]["X"],
                 "Unit": self.df["Vmux2"]["Unit"],
                 "Values": (
-                    self.df["Vmux2"]["Values"] - self.df[self.VmuxGrd]["Values"]
+                    self.df["Vmux2"]["Values"] - self.df[self.VmuxGnd]["Values"]
                 ),
             }
         }
 
     def Vmux3(self):
         return {
             getVmuxMap()[3]: {
                 "X": self.df["Vmux3"]["X"],
                 "Unit": self.df["Vmux3"]["Unit"],
-                "Values": (self.df["Vmux3"]["Values"] - self.df[self.VmuxGrd]["Values"])
+                "Values": (self.df["Vmux3"]["Values"] - self.df[self.VmuxGnd]["Values"])
                 * 2,
             }
         }
 
     def Vmux4(self):
         return {
             getVmuxMap()[4]: {
                 "X": self.df["Vmux4"]["X"],
                 "Unit": self.df["Vmux4"]["Unit"],
-                "Values": (self.df["Vmux4"]["Values"] - self.df[self.VmuxGrd]["Values"])
-                * 2,
+                "Values": self.df["Vmux4"]["Values"] * 2,
             }
         }
 
     def Vmux5(self):
         return {
             getVmuxMap()[5]: {
                 "X": self.df["Vmux5"]["X"],
                 "Unit": self.df["Vmux5"]["Unit"],
-                "Values": self.df["Vmux5"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux5"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux6(self):
         return {
             getVmuxMap()[6]: {
                 "X": self.df["Vmux6"]["X"],
                 "Unit": self.df["Vmux6"]["Unit"],
-                "Values": self.df["Vmux6"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux6"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux7(self):
         return {
             getVmuxMap()[7]: {
                 "X": self.df["Vmux7"]["X"],
                 "Unit": self.df["Vmux7"]["Unit"],
-                "Values": self.df["Vmux7"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux7"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux8(self):
         return {
             getVmuxMap()[8]: {
                 "X": self.df["Vmux8"]["X"],
                 "Unit": self.df["Vmux8"]["Unit"],
-                "Values": self.df["Vmux8"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux8"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux9(self):
         return {
             getVmuxMap()[9]: {
                 "X": self.df["Vmux9"]["X"],
                 "Unit": self.df["Vmux9"]["Unit"],
-                "Values": self.df["Vmux9"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux9"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux10(self):
         return {
             getVmuxMap()[10]: {
                 "X": self.df["Vmux10"]["X"],
                 "Unit": self.df["Vmux10"]["Unit"],
-                "Values": self.df["Vmux10"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux10"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux11(self):
         return {
             getVmuxMap()[11]: {
                 "X": self.df["Vmux11"]["X"],
                 "Unit": self.df["Vmux11"]["Unit"],
-                "Values": self.df["Vmux11"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux11"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux12(self):
         return {
             getVmuxMap()[12]: {
                 "X": self.df["Vmux12"]["X"],
                 "Unit": self.df["Vmux12"]["Unit"],
-                "Values": self.df["Vmux12"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux12"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux13(self):
         return {
             getVmuxMap()[13]: {
                 "X": self.df["Vmux13"]["X"],
                 "Unit": self.df["Vmux13"]["Unit"],
-                "Values": self.df["Vmux13"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux13"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux14(self):
         return {
             getVmuxMap()[14]: {
                 "X": self.df["Vmux14"]["X"],
                 "Unit": self.df["Vmux14"]["Unit"],
-                "Values": self.df["Vmux14"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux14"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux15(self):
         return {
             getVmuxMap()[15]: {
                 "X": self.df["Vmux15"]["X"],
                 "Unit": self.df["Vmux15"]["Unit"],
-                "Values": self.df["Vmux15"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux15"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux16(self):
         return {
             getVmuxMap()[16]: {
                 "X": self.df["Vmux16"]["X"],
                 "Unit": self.df["Vmux16"]["Unit"],
-                "Values": self.df["Vmux16"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux16"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux17(self):
         return {
             getVmuxMap()[17]: {
                 "X": self.df["Vmux17"]["X"],
                 "Unit": self.df["Vmux17"]["Unit"],
-                "Values": self.df["Vmux17"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux17"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux18(self):
         return {
             getVmuxMap()[18]: {
                 "X": self.df["Vmux18"]["X"],
                 "Unit": self.df["Vmux18"]["Unit"],
-                "Values": self.df["Vmux18"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux18"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux30(self):
         return {
             getVmuxMap()[30]: {
                 "X": self.df["Vmux30"]["X"],
@@ -515,450 +527,450 @@
         }
 
     def Vmux31(self):
         return {
             getVmuxMap()[31]: {
                 "X": self.df["Vmux31"]["X"],
                 "Unit": self.df["Vmux31"]["Unit"],
-                "Values": self.df["Vmux31"]["Values"] - self.df[self.VmuxGrd]["Values"],
+                "Values": self.df["Vmux31"]["Values"] - self.df[self.VmuxGnd]["Values"],
             }
         }
 
     def Vmux32(self):
         return {
             getVmuxMap()[32]: {
                 "X": self.df["Vmux32"]["X"],
                 "Unit": self.df["Vmux32"]["Unit"],
                 "Values": (
-                    self.df["Vmux32"]["Values"] - self.df[self.VmuxGrd]["Values"]
+                    self.df["Vmux32"]["Values"] - self.df[self.VmuxGnd]["Values"]
                 )
                 * 3.33,
             }
         }
 
     def Vmux33(self):
         return {
             getVmuxMap()[33]: {
                 "X": self.df["Vmux33"]["X"],
                 "Unit": self.df["Vmux33"]["Unit"],
                 "Values": (
-                    self.df["Vmux33"]["Values"] - self.df[self.VmuxGrd]["Values"]
+                    self.df["Vmux33"]["Values"] - self.df[self.VmuxGnd]["Values"]
                 )
                 * 4,
             }
         }
 
     def Vmux34(self):
         return {
             getVmuxMap()[34]: {
                 "X": self.df["Vmux34"]["X"],
                 "Unit": self.df["Vmux34"]["Unit"],
                 "Values": (
-                    self.df["Vmux34"]["Values"] - self.df[self.VmuxGrd]["Values"]
+                    self.df["Vmux34"]["Values"] - self.df[self.VmuxGnd]["Values"]
                 )
                 * 2,
             }
         }
 
     def Vmux35(self):
         return {
             getVmuxMap()[35]: {
                 "X": self.df["Vmux35"]["X"],
                 "Unit": self.df["Vmux35"]["Unit"],
                 "Values": (
-                    self.df["Vmux35"]["Values"] - self.df[self.VmuxGrd]["Values"]
+                    self.df["Vmux35"]["Values"] - self.df[self.VmuxGnd]["Values"]
                 ),
             }
         }
 
     def Vmux36(self):
         return {
             getVmuxMap()[36]: {
                 "X": self.df["Vmux36"]["X"],
                 "Unit": self.df["Vmux36"]["Unit"],
                 "Values": (
-                    self.df["Vmux36"]["Values"] - self.df[self.VmuxGrd]["Values"]
+                    self.df["Vmux36"]["Values"] - self.df[self.VmuxGnd]["Values"]
                 )
                 * 4,
             }
         }
 
     def Vmux37(self):
         return {
             getVmuxMap()[37]: {
                 "X": self.df["Vmux37"]["X"],
                 "Unit": self.df["Vmux37"]["Unit"],
                 "Values": (
-                    self.df["Vmux37"]["Values"] - self.df[self.VmuxGrd]["Values"]
+                    self.df["Vmux37"]["Values"] - self.df[self.VmuxGnd]["Values"]
                 )
                 * 4,
             }
         }
 
     def Vmux38(self):
         return {
             getVmuxMap()[38]: {
                 "X": self.df["Vmux38"]["X"],
                 "Unit": self.df["Vmux38"]["Unit"],
                 "Values": (
-                    self.df["Vmux38"]["Values"] - self.df[self.VmuxGrd]["Values"]
+                    self.df["Vmux38"]["Values"] - self.df[self.VmuxGnd]["Values"]
                 )
                 * 2,
             }
         }
 
     def Vmux39(self):
         return {
             getVmuxMap()[39]: {
                 "X": self.df["Vmux39"]["X"],
                 "Unit": self.df["Vmux39"]["Unit"],
                 "Values": (
-                    self.df["Vmux39"]["Values"] - self.df[self.VmuxGrd]["Values"]
+                    self.df["Vmux39"]["Values"] - self.df[self.VmuxGnd]["Values"]
                 ),
             }
         }
 
     def Imux0(self):
         return {
             getImuxMap()[0]: {
                 "X": self.df["Imux0"]["X"],
                 "Unit": "A",
-                "Values": (self.df["Imux0"]["Values"] - self.df[self.ImuxGrd]["Values"])
+                "Values": (self.df["Imux0"]["Values"] - self.df[self.ImuxGnd]["Values"])
                 / self.rImux,
             }
         }
 
     def Imux1(self):
         return {
             getImuxMap()[1]: {
                 "X": self.df["Imux1"]["X"],
                 "Unit": "A",
-                "Values": (self.df["Imux1"]["Values"] - self.df[self.ImuxGrd]["Values"])
+                "Values": (self.df["Imux1"]["Values"] - self.df[self.ImuxGnd]["Values"])
                 / self.rImux,
             }
         }
 
     def Imux2(self):
         return {
             getImuxMap()[2]: {
                 "X": self.df["Imux2"]["X"],
                 "Unit": "A",
-                "Values": (self.df["Imux2"]["Values"] - self.df[self.ImuxGrd]["Values"])
+                "Values": (self.df["Imux2"]["Values"] - self.df[self.ImuxGnd]["Values"])
                 / self.rImux,
             }
         }
 
     def Imux3(self):
         return {
             getImuxMap()[3]: {
                 "X": self.df["Imux3"]["X"],
                 "Unit": "A",
-                "Values": (self.df["Imux3"]["Values"] - self.df[self.ImuxGrd]["Values"])
+                "Values": (self.df["Imux3"]["Values"] - self.df[self.ImuxGnd]["Values"])
                 / self.rImux,
             }
         }
 
     def Imux4(self):
         return {
             getImuxMap()[4]: {
                 "X": self.df["Imux4"]["X"],
                 "Unit": "A",
-                "Values": (self.df["Imux4"]["Values"] - self.df[self.ImuxGrd]["Values"])
+                "Values": (self.df["Imux4"]["Values"] - self.df[self.ImuxGnd]["Values"])
                 / self.rImux,
             }
         }
 
     def Imux5(self):
         return {
             getImuxMap()[5]: {
                 "X": self.df["Imux5"]["X"],
                 "Unit": "A",
-                "Values": (self.df["Imux5"]["Values"] - self.df[self.ImuxGrd]["Values"])
+                "Values": (self.df["Imux5"]["Values"] - self.df[self.ImuxGnd]["Values"])
                 / self.rImux,
             }
         }
 
     def Imux6(self):
         return {
             getImuxMap()[6]: {
                 "X": self.df["Imux6"]["X"],
                 "Unit": "A",
-                "Values": (self.df["Imux6"]["Values"] - self.df[self.ImuxGrd]["Values"])
+                "Values": (self.df["Imux6"]["Values"] - self.df[self.ImuxGnd]["Values"])
                 / self.rImux,
             }
         }
 
     def Imux7(self):
         return {
             getImuxMap()[7]: {
                 "X": self.df["Imux7"]["X"],
                 "Unit": "A",
-                "Values": (self.df["Imux7"]["Values"] - self.df[self.ImuxGrd]["Values"])
+                "Values": (self.df["Imux7"]["Values"] - self.df[self.ImuxGnd]["Values"])
                 / self.rImux,
             }
         }
 
     def Imux8(self):
         return {
             getImuxMap()[8]: {
                 "X": self.df["Imux8"]["X"],
                 "Unit": "A",
-                "Values": (self.df["Imux8"]["Values"] - self.df[self.ImuxGrd]["Values"])
+                "Values": (self.df["Imux8"]["Values"] - self.df[self.ImuxGnd]["Values"])
                 / self.rImux,
             }
         }
 
     def Imux9(self):
         return {
             getImuxMap()[9]: {
                 "X": self.df["Imux9"]["X"],
                 "Unit": "A",
-                "Values": (self.df["Imux9"]["Values"] - self.df[self.ImuxGrd]["Values"])
+                "Values": (self.df["Imux9"]["Values"] - self.df[self.ImuxGnd]["Values"])
                 / self.rImux,
             }
         }
 
     def Imux10(self):
         return {
             getImuxMap()[10]: {
                 "X": self.df["Imux10"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux10"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux10"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux11(self):
         return {
             getImuxMap()[11]: {
                 "X": self.df["Imux11"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux11"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux11"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux12(self):
         return {
             getImuxMap()[12]: {
                 "X": self.df["Imux12"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux12"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux12"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux13(self):
         return {
             getImuxMap()[13]: {
                 "X": self.df["Imux13"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux13"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux13"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux14(self):
         return {
             getImuxMap()[14]: {
                 "X": self.df["Imux14"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux14"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux14"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux15(self):
         return {
             getImuxMap()[15]: {
                 "X": self.df["Imux15"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux15"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux15"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux16(self):
         return {
             getImuxMap()[16]: {
                 "X": self.df["Imux16"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux16"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux16"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux17(self):
         return {
             getImuxMap()[17]: {
                 "X": self.df["Imux17"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux17"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux17"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux18(self):
         return {
             getImuxMap()[18]: {
                 "X": self.df["Imux18"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux18"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux18"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux19(self):
         return {
             getImuxMap()[19]: {
                 "X": self.df["Imux15"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux15"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux15"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux20(self):
         return {
             getImuxMap()[20]: {
                 "X": self.df["Imux20"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux20"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux20"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux21(self):
         return {
             getImuxMap()[21]: {
                 "X": self.df["Imux21"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux21"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux21"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux22(self):
         return {
             getImuxMap()[22]: {
                 "X": self.df["Imux22"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux22"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux22"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux23(self):
         return {
             getImuxMap()[23]: {
                 "X": self.df["Imux23"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux23"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux23"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux24(self):
         return {
             getImuxMap()[24]: {
                 "X": self.df["Imux24"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux24"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux24"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux25(self):
         return {
             getImuxMap()[25]: {
                 "X": self.df["Imux25"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux25"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux25"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux,
             }
         }
 
     def Imux28(self):
         return {
             getImuxMap()[28]: {
                 "X": self.df["Imux28"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux28"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux28"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux
                 * self.kIinA,
             }
         }
 
     def Imux29(self):
         return {
             getImuxMap()[29]: {
                 "X": self.df["Imux29"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux29"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux29"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux
                 * self.kIshuntA,
             }
         }
 
     def Imux30(self):
         return {
             getImuxMap()[30]: {
                 "X": self.df["Imux30"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux30"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux30"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux
                 * self.kIinD,
             }
         }
 
     def Imux31(self):
         return {
             getImuxMap()[31]: {
                 "X": self.df["Imux31"]["X"],
                 "Unit": "A",
                 "Values": (
-                    self.df["Imux31"]["Values"] - self.df[self.ImuxGrd]["Values"]
+                    self.df["Imux31"]["Values"] - self.df[self.ImuxGnd]["Values"]
                 )
                 / self.rImux
                 * self.kIshuntD,
             }
         }
 
     def IcoreA(self):
```

### Comparing `module_qc_analysis_tools-1.3.0/tests/test_cli.py` & `module_qc_analysis_tools-1.3.1rc1/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,16 +22,14 @@
     result = runner.invoke(
         app,
         args=[
             "analysis",
             "adc-calibration",
             "-i",
             base_path.joinpath("ADC_CALIBRATION/1000000001//"),
-            "--layer",
-            "L2",
             "-v",
             "DEBUG",
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0, result.stderr
     for chip_id in range(1, 5):
@@ -44,16 +42,14 @@
     result = runner.invoke(
         app,
         args=[
             "analysis",
             "analog-readback",
             "-i",
             base_path.joinpath("ANALOG_READBACK/1000000001//"),
-            "--layer",
-            "L2",
             "-v",
             "DEBUG",
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0, result.stderr
     for chip_id in range(1, 5):
@@ -66,16 +62,14 @@
     result = runner.invoke(
         app,
         args=[
             "analysis",
             "vcal-calibration",
             "-i",
             base_path.joinpath("VCAL_CALIBRATION/1000000001//"),
-            "--layer",
-            "L2",
             "-v",
             "DEBUG",
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0, result.stderr
     for chip_id in range(1, 5):
@@ -88,16 +82,14 @@
     result = runner.invoke(
         app,
         args=[
             "analysis",
             "sldo",
             "-i",
             base_path.joinpath("SLDO/1000000001//"),
-            "--layer",
-            "L2",
             "-v",
             "DEBUG",
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0, result.stderr
     for chip_id in range(1, 5):
@@ -110,16 +102,14 @@
     result = runner.invoke(
         app,
         args=[
             "analysis",
             "injection-capacitance",
             "-i",
             base_path.joinpath("INJECTION_CAPACITANCE/1000000001/"),
-            "--layer",
-            "L2",
             "-v",
             "DEBUG",
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0, result.stderr
     for chip_id in range(1, 5):
```

### Comparing `module_qc_analysis_tools-1.3.0/.gitignore` & `module_qc_analysis_tools-1.3.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.0/LICENSE` & `module_qc_analysis_tools-1.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.0/README.md` & `module_qc_analysis_tools-1.3.1rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-analysis-tools v1.3.0
+# module-qc-analysis-tools v1.3.1rc1
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -49,15 +49,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.0
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc1
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
```

### Comparing `module_qc_analysis_tools-1.3.0/pyproject.toml` & `module_qc_analysis_tools-1.3.1rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 module-qc-analysis-tools = "module_qc_analysis_tools.cli:app"
 "mqat" = "module_qc_analysis_tools.cli:app"
 analysis-ADC-CALIBRATION = "module_qc_analysis_tools.cli.ADC_CALIBRATION:app"
 analysis-ANALOG-READBACK = "module_qc_analysis_tools.cli.ANALOG_READBACK:app"
 analysis-INJECTION-CAPACITANCE = "module_qc_analysis_tools.cli.INJECTION_CAPACITANCE:app"
 analysis-SLDO = "module_qc_analysis_tools.cli.SLDO:app"
 analysis-VCAL-CALIBRATION = "module_qc_analysis_tools.cli.VCAL_CALIBRATION:app"
+analysis-MASS-MEASUREMENT = "module_qc_analysis_tools.cli.MASS_MEASUREMENT:app"
+analysis-IV-MEASURE = "module_qc_analysis_tools.cli.IV_MEASURE:app"
+analysis-VISUAL-INSPECTION = "module_qc_analysis_tools.cli.VISUAL_INSPECTION:app"
 analysis-overwrite-config = "module_qc_analysis_tools.cli.overwrite_config:app"
 analysis-update-chip-config = "module_qc_analysis_tools.cli.update_chip_config:app"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.version.raw-options]
```

### Comparing `module_qc_analysis_tools-1.3.0/PKG-INFO` & `module_qc_analysis_tools-1.3.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-analysis-tools
-Version: 1.3.0
+Version: 1.3.1rc1
 Summary: Module qc analysis tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
@@ -34,15 +34,15 @@
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
 Requires-Dist: matplotlib
 Requires-Dist: module-qc-data-tools>=1.0.3
 Requires-Dist: numpy
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
-# module-qc-analysis-tools v1.3.0
+# module-qc-analysis-tools v1.3.1rc1
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -89,15 +89,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.0
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc1
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
```

