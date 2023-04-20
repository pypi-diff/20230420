# Comparing `tmp/cliffordlayers-0.1.0.tar.gz` & `tmp/cliffordlayers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliffordlayers-0.1.0.tar", last modified: Wed Mar  1 22:02:07 2023, max compression
+gzip compressed data, was "cliffordlayers-0.1.1.tar", last modified: Thu Apr 20 00:36:01 2023, max compression
```

## Comparing `cliffordlayers-0.1.0.tar` & `cliffordlayers-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,50 @@
-drwxrwxr-x   0 jagupt    (1000) jagupt    (1000)        0 2023-03-01 22:02:07.725589 cliffordlayers-0.1.0/
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     1141 2023-03-01 21:56:08.000000 cliffordlayers-0.1.0/LICENSE
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     2694 2023-03-01 22:02:07.725589 cliffordlayers-0.1.0/PKG-INFO
--rwxrwxr-x   0 jagupt    (1000) jagupt    (1000)     1935 2023-03-01 21:56:45.000000 cliffordlayers-0.1.0/README.md
-drwxrwxr-x   0 jagupt    (1000) jagupt    (1000)        0 2023-03-01 22:02:07.721589 cliffordlayers-0.1.0/cliffordlayers.egg-info/
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     2694 2023-03-01 22:02:07.000000 cliffordlayers-0.1.0/cliffordlayers.egg-info/PKG-INFO
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)      545 2023-03-01 22:02:07.000000 cliffordlayers-0.1.0/cliffordlayers.egg-info/SOURCES.txt
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)        1 2023-03-01 22:02:07.000000 cliffordlayers-0.1.0/cliffordlayers.egg-info/dependency_links.txt
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)       13 2023-03-01 22:02:07.000000 cliffordlayers-0.1.0/cliffordlayers.egg-info/requires.txt
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)        1 2023-03-01 22:02:07.000000 cliffordlayers-0.1.0/cliffordlayers.egg-info/top_level.txt
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)       38 2023-03-01 22:02:07.725589 cliffordlayers-0.1.0/setup.cfg
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     1193 2023-03-01 21:56:45.000000 cliffordlayers-0.1.0/setup.py
-drwxrwxr-x   0 jagupt    (1000) jagupt    (1000)        0 2023-03-01 22:02:07.725589 cliffordlayers-0.1.0/tests/
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     4670 2023-03-01 21:56:45.000000 cliffordlayers-0.1.0/tests/test_CliffordNet2d.py
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     1345 2023-03-01 21:56:45.000000 cliffordlayers-0.1.0/tests/test_CliffordNet3d.py
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     5946 2023-03-01 21:56:45.000000 cliffordlayers-0.1.0/tests/test_clifford_batchnorm.py
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     3345 2023-03-01 21:56:45.000000 cliffordlayers-0.1.0/tests/test_clifford_convolution.py
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     2751 2023-03-01 21:56:45.000000 cliffordlayers-0.1.0/tests/test_clifford_convolution_custom.py
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     4750 2023-03-01 21:56:45.000000 cliffordlayers-0.1.0/tests/test_clifford_fourier.py
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)    11196 2023-03-01 21:56:45.000000 cliffordlayers-0.1.0/tests/test_clifford_groupnorm.py
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     1467 2023-03-01 21:56:45.000000 cliffordlayers-0.1.0/tests/test_clifford_kernels.py
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     3869 2023-03-01 21:56:45.000000 cliffordlayers-0.1.0/tests/test_clifford_linear.py
--rw-rw-r--   0 jagupt    (1000) jagupt    (1000)      922 2023-03-01 21:56:45.000000 cliffordlayers-0.1.0/tests/test_clifford_rotation_kernel.py
+drwxrwxr-x   0 jagupt    (1000) jagupt    (1000)        0 2023-04-20 00:36:01.883598 cliffordlayers-0.1.1/
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     1141 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/LICENSE
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     3321 2023-04-20 00:36:01.883598 cliffordlayers-0.1.1/PKG-INFO
+-rwxrwxr-x   0 jagupt    (1000) jagupt    (1000)     2562 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/README.md
+drwxrwxr-x   0 jagupt    (1000) jagupt    (1000)        0 2023-04-20 00:36:01.879598 cliffordlayers-0.1.1/cliffordlayers/
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)        1 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/__init__.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)    11441 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/cliffordkernels.py
+drwxrwxr-x   0 jagupt    (1000) jagupt    (1000)        0 2023-04-20 00:36:01.879598 cliffordlayers-0.1.1/cliffordlayers/models/
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)        0 2023-04-20 00:32:01.000000 cliffordlayers-0.1.1/cliffordlayers/models/__init__.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)    11163 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/models/custom_kernels.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     5083 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/models/custom_layers.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     9782 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/models/models_2d.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     7132 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/models/models_3d.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)      932 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/models/utils.py
+drwxrwxr-x   0 jagupt    (1000) jagupt    (1000)        0 2023-04-20 00:36:01.879598 cliffordlayers-0.1.1/cliffordlayers/nn/
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)        0 2023-04-20 00:31:42.000000 cliffordlayers-0.1.1/cliffordlayers/nn/__init__.py
+drwxrwxr-x   0 jagupt    (1000) jagupt    (1000)        0 2023-04-20 00:36:01.879598 cliffordlayers-0.1.1/cliffordlayers/nn/functional/
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)       74 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/nn/functional/__init__.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     8941 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/nn/functional/batchnorm.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     9064 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/nn/functional/groupnorm.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     3347 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/nn/functional/utils.py
+drwxrwxr-x   0 jagupt    (1000) jagupt    (1000)        0 2023-04-20 00:36:01.883598 cliffordlayers-0.1.1/cliffordlayers/nn/modules/
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)       74 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/nn/modules/__init__.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     9835 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/nn/modules/batchnorm.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)    11563 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/nn/modules/cliffordconv.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)    14866 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/nn/modules/cliffordfourier.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)    14065 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/nn/modules/cliffordfourier_deprecated.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     3151 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/nn/modules/cliffordlinear.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     5968 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/nn/modules/groupnorm.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     1281 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/signature.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)       96 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/cliffordlayers/version.py
+drwxrwxr-x   0 jagupt    (1000) jagupt    (1000)        0 2023-04-20 00:36:01.879598 cliffordlayers-0.1.1/cliffordlayers.egg-info/
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     3321 2023-04-20 00:36:01.000000 cliffordlayers-0.1.1/cliffordlayers.egg-info/PKG-INFO
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     1370 2023-04-20 00:36:01.000000 cliffordlayers-0.1.1/cliffordlayers.egg-info/SOURCES.txt
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)        1 2023-04-20 00:36:01.000000 cliffordlayers-0.1.1/cliffordlayers.egg-info/dependency_links.txt
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)       13 2023-04-20 00:36:01.000000 cliffordlayers-0.1.1/cliffordlayers.egg-info/requires.txt
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)       15 2023-04-20 00:36:01.000000 cliffordlayers-0.1.1/cliffordlayers.egg-info/top_level.txt
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)       38 2023-04-20 00:36:01.883598 cliffordlayers-0.1.1/setup.cfg
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     1267 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/setup.py
+drwxrwxr-x   0 jagupt    (1000) jagupt    (1000)        0 2023-04-20 00:36:01.883598 cliffordlayers-0.1.1/tests/
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     4744 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/tests/test_CliffordNet2d.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     1419 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/tests/test_CliffordNet3d.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     6020 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/tests/test_clifford_batchnorm.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     3419 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/tests/test_clifford_convolution.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     2825 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/tests/test_clifford_convolution_custom.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     4824 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/tests/test_clifford_fourier.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)    11270 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/tests/test_clifford_groupnorm.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     1541 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/tests/test_clifford_kernels.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)     3943 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/tests/test_clifford_linear.py
+-rw-rw-r--   0 jagupt    (1000) jagupt    (1000)      996 2023-04-20 00:31:27.000000 cliffordlayers-0.1.1/tests/test_clifford_rotation_kernel.py
```

### Comparing `cliffordlayers-0.1.0/LICENSE` & `cliffordlayers-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cliffordlayers-0.1.0/PKG-INFO` & `cliffordlayers-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 636c 6966  : 2.1.Name: clif
 00000020: 666f 7264 6c61 7965 7273 0a56 6572 7369  fordlayers.Versi
-00000030: 6f6e 3a20 302e 312e 300a 5375 6d6d 6172  on: 0.1.0.Summar
+00000030: 6f6e 3a20 302e 312e 310a 5375 6d6d 6172  on: 0.1.1.Summar
 00000040: 793a 2041 2050 7954 6f72 6368 206c 6962  y: A PyTorch lib
 00000050: 7261 7279 2066 6f72 2043 6c69 6666 6f72  rary for Cliffor
 00000060: 6420 6c61 7965 7273 0a41 7574 686f 723a  d layers.Author:
 00000070: 204a 6179 6573 6820 4b2e 2047 7570 7461   Jayesh K. Gupta
 00000080: 2c20 4a6f 6861 6e6e 6573 2042 7261 6e64  , Johannes Brand
 00000090: 7374 6574 7465 722c 2044 6176 6964 2052  stetter, David R
 000000a0: 7568 652c 2061 6e64 2063 6f6e 7472 6962  uhe, and contrib
@@ -42,128 +42,167 @@
 00000290: 6961 6c20 496e 7465 6c6c 6967 656e 6365  ial Intelligence
 000002a0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
 000002b0: 3a20 3e3d 332e 360a 4465 7363 7269 7074  : >=3.6.Descript
 000002c0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
 000002d0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
 000002e0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
 000002f0: 4345 4e53 450a 0a0a 2320 436c 6966 666f  CENSE...# Cliffo
-00000300: 7264 204e 6575 7261 6c20 4c61 7965 7273  rd Neural Layers
-00000310: 0a0a 0a0a 3c61 2068 7265 663d 2268 7474  ....<a href="htt
-00000320: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-00000330: 6273 2f32 3230 392e 3034 3933 3422 3e4c  bs/2209.04934">L
-00000340: 696e 6b20 746f 2074 6865 2070 6170 6572  ink to the paper
-00000350: 3c2f 613e 0a0a 4966 2079 6f75 2066 696e  </a>..If you fin
-00000360: 6420 6f75 7220 776f 726b 2061 6e64 2f6f  d our work and/o
-00000370: 7220 6f75 7220 636f 6465 2075 7365 6675  r our code usefu
-00000380: 6c2c 2070 6c65 6173 6520 6369 7465 2075  l, please cite u
-00000390: 7320 7669 613a 0a0a 6060 6062 6962 7465  s via:..```bibte
-000003a0: 780a 4061 7274 6963 6c65 7b62 7261 6e64  x.@article{brand
-000003b0: 7374 6574 7465 7232 3032 3263 6c69 6666  stetter2022cliff
-000003c0: 6f72 642c 0a20 2074 6974 6c65 3d7b 436c  ord,.  title={Cl
-000003d0: 6966 666f 7264 204e 6575 7261 6c20 4c61  ifford Neural La
-000003e0: 7965 7273 2066 6f72 2050 4445 204d 6f64  yers for PDE Mod
-000003f0: 656c 696e 677d 2c0a 2020 6175 7468 6f72  eling},.  author
-00000400: 3d7b 4272 616e 6473 7465 7474 6572 2c20  ={Brandstetter, 
-00000410: 4a6f 6861 6e6e 6573 2061 6e64 2042 6572  Johannes and Ber
-00000420: 672c 2052 6961 6e6e 6520 7661 6e20 6465  g, Rianne van de
-00000430: 6e20 616e 6420 5765 6c6c 696e 672c 204d  n and Welling, M
-00000440: 6178 2061 6e64 2047 7570 7461 2c20 4a61  ax and Gupta, Ja
-00000450: 7965 7368 204b 7d2c 0a20 206a 6f75 726e  yesh K},.  journ
-00000460: 616c 3d7b 6172 5869 7620 7072 6570 7269  al={arXiv prepri
-00000470: 6e74 2061 7258 6976 3a32 3230 392e 3034  nt arXiv:2209.04
-00000480: 3933 347d 2c0a 2020 7965 6172 3d7b 3230  934},.  year={20
-00000490: 3232 7d0a 7d0a 6060 600a 0a23 2320 496e  22}.}.```..## In
-000004a0: 7374 616c 6c61 7469 6f6e 0a0a 6060 6062  stallation..```b
-000004b0: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
-000004c0: 636c 6966 666f 7264 6c61 7965 7273 0a60  cliffordlayers.`
-000004d0: 6060 0a0a 2323 2043 6f6e 7472 6962 7574  ``..## Contribut
-000004e0: 696e 670a 0a54 6869 7320 7072 6f6a 6563  ing..This projec
-000004f0: 7420 7765 6c63 6f6d 6573 2063 6f6e 7472  t welcomes contr
-00000500: 6962 7574 696f 6e73 2061 6e64 2073 7567  ibutions and sug
-00000510: 6765 7374 696f 6e73 2e20 204d 6f73 7420  gestions.  Most 
-00000520: 636f 6e74 7269 6275 7469 6f6e 7320 7265  contributions re
-00000530: 7175 6972 6520 796f 7520 746f 2061 6772  quire you to agr
-00000540: 6565 2074 6f20 610a 436f 6e74 7269 6275  ee to a.Contribu
-00000550: 746f 7220 4c69 6365 6e73 6520 4167 7265  tor License Agre
-00000560: 656d 656e 7420 2843 4c41 2920 6465 636c  ement (CLA) decl
-00000570: 6172 696e 6720 7468 6174 2079 6f75 2068  aring that you h
-00000580: 6176 6520 7468 6520 7269 6768 7420 746f  ave the right to
-00000590: 2c20 616e 6420 6163 7475 616c 6c79 2064  , and actually d
-000005a0: 6f2c 2067 7261 6e74 2075 730a 7468 6520  o, grant us.the 
-000005b0: 7269 6768 7473 2074 6f20 7573 6520 796f  rights to use yo
-000005c0: 7572 2063 6f6e 7472 6962 7574 696f 6e2e  ur contribution.
-000005d0: 2046 6f72 2064 6574 6169 6c73 2c20 7669   For details, vi
-000005e0: 7369 7420 6874 7470 733a 2f2f 636c 612e  sit https://cla.
-000005f0: 6f70 656e 736f 7572 6365 2e6d 6963 726f  opensource.micro
-00000600: 736f 6674 2e63 6f6d 2e0a 0a57 6865 6e20  soft.com...When 
-00000610: 796f 7520 7375 626d 6974 2061 2070 756c  you submit a pul
-00000620: 6c20 7265 7175 6573 742c 2061 2043 4c41  l request, a CLA
-00000630: 2062 6f74 2077 696c 6c20 6175 746f 6d61   bot will automa
-00000640: 7469 6361 6c6c 7920 6465 7465 726d 696e  tically determin
-00000650: 6520 7768 6574 6865 7220 796f 7520 6e65  e whether you ne
-00000660: 6564 2074 6f20 7072 6f76 6964 650a 6120  ed to provide.a 
-00000670: 434c 4120 616e 6420 6465 636f 7261 7465  CLA and decorate
-00000680: 2074 6865 2050 5220 6170 7072 6f70 7269   the PR appropri
-00000690: 6174 656c 7920 2865 2e67 2e2c 2073 7461  ately (e.g., sta
-000006a0: 7475 7320 6368 6563 6b2c 2063 6f6d 6d65  tus check, comme
-000006b0: 6e74 292e 2053 696d 706c 7920 666f 6c6c  nt). Simply foll
-000006c0: 6f77 2074 6865 2069 6e73 7472 7563 7469  ow the instructi
-000006d0: 6f6e 730a 7072 6f76 6964 6564 2062 7920  ons.provided by 
-000006e0: 7468 6520 626f 742e 2059 6f75 2077 696c  the bot. You wil
-000006f0: 6c20 6f6e 6c79 206e 6565 6420 746f 2064  l only need to d
-00000700: 6f20 7468 6973 206f 6e63 6520 6163 726f  o this once acro
-00000710: 7373 2061 6c6c 2072 6570 6f73 2075 7369  ss all repos usi
-00000720: 6e67 206f 7572 2043 4c41 2e0a 0a54 6869  ng our CLA...Thi
-00000730: 7320 7072 6f6a 6563 7420 6861 7320 6164  s project has ad
-00000740: 6f70 7465 6420 7468 6520 5b4d 6963 726f  opted the [Micro
-00000750: 736f 6674 204f 7065 6e20 536f 7572 6365  soft Open Source
-00000760: 2043 6f64 6520 6f66 2043 6f6e 6475 6374   Code of Conduct
-00000770: 5d28 6874 7470 733a 2f2f 6f70 656e 736f  ](https://openso
-00000780: 7572 6365 2e6d 6963 726f 736f 6674 2e63  urce.microsoft.c
-00000790: 6f6d 2f63 6f64 656f 6663 6f6e 6475 6374  om/codeofconduct
-000007a0: 2f29 2e0a 466f 7220 6d6f 7265 2069 6e66  /)..For more inf
-000007b0: 6f72 6d61 7469 6f6e 2073 6565 2074 6865  ormation see the
-000007c0: 205b 436f 6465 206f 6620 436f 6e64 7563   [Code of Conduc
-000007d0: 7420 4641 515d 2868 7474 7073 3a2f 2f6f  t FAQ](https://o
-000007e0: 7065 6e73 6f75 7263 652e 6d69 6372 6f73  pensource.micros
-000007f0: 6f66 742e 636f 6d2f 636f 6465 6f66 636f  oft.com/codeofco
-00000800: 6e64 7563 742f 6661 712f 2920 6f72 0a63  nduct/faq/) or.c
-00000810: 6f6e 7461 6374 205b 6f70 656e 636f 6465  ontact [opencode
-00000820: 406d 6963 726f 736f 6674 2e63 6f6d 5d28  @microsoft.com](
-00000830: 6d61 696c 746f 3a6f 7065 6e63 6f64 6540  mailto:opencode@
-00000840: 6d69 6372 6f73 6f66 742e 636f 6d29 2077  microsoft.com) w
-00000850: 6974 6820 616e 7920 6164 6469 7469 6f6e  ith any addition
-00000860: 616c 2071 7565 7374 696f 6e73 206f 7220  al questions or 
-00000870: 636f 6d6d 656e 7473 2e0a 0a23 2320 5472  comments...## Tr
-00000880: 6164 656d 6172 6b73 0a0a 5468 6973 2070  ademarks..This p
-00000890: 726f 6a65 6374 206d 6179 2063 6f6e 7461  roject may conta
-000008a0: 696e 2074 7261 6465 6d61 726b 7320 6f72  in trademarks or
-000008b0: 206c 6f67 6f73 2066 6f72 2070 726f 6a65   logos for proje
-000008c0: 6374 732c 2070 726f 6475 6374 732c 206f  cts, products, o
-000008d0: 7220 7365 7276 6963 6573 2e20 4175 7468  r services. Auth
-000008e0: 6f72 697a 6564 2075 7365 206f 6620 4d69  orized use of Mi
-000008f0: 6372 6f73 6f66 740a 7472 6164 656d 6172  crosoft.trademar
-00000900: 6b73 206f 7220 6c6f 676f 7320 6973 2073  ks or logos is s
-00000910: 7562 6a65 6374 2074 6f20 616e 6420 6d75  ubject to and mu
-00000920: 7374 2066 6f6c 6c6f 770a 5b4d 6963 726f  st follow.[Micro
-00000930: 736f 6674 2773 2054 7261 6465 6d61 726b  soft's Trademark
-00000940: 2026 2042 7261 6e64 2047 7569 6465 6c69   & Brand Guideli
-00000950: 6e65 735d 2868 7474 7073 3a2f 2f77 7777  nes](https://www
-00000960: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f65  .microsoft.com/e
-00000970: 6e2d 7573 2f6c 6567 616c 2f69 6e74 656c  n-us/legal/intel
-00000980: 6c65 6374 7561 6c70 726f 7065 7274 792f  lectualproperty/
-00000990: 7472 6164 656d 6172 6b73 2f75 7361 6765  trademarks/usage
-000009a0: 2f67 656e 6572 616c 292e 0a55 7365 206f  /general)..Use o
-000009b0: 6620 4d69 6372 6f73 6f66 7420 7472 6164  f Microsoft trad
-000009c0: 656d 6172 6b73 206f 7220 6c6f 676f 7320  emarks or logos 
-000009d0: 696e 206d 6f64 6966 6965 6420 7665 7273  in modified vers
-000009e0: 696f 6e73 206f 6620 7468 6973 2070 726f  ions of this pro
-000009f0: 6a65 6374 206d 7573 7420 6e6f 7420 6361  ject must not ca
-00000a00: 7573 6520 636f 6e66 7573 696f 6e20 6f72  use confusion or
-00000a10: 2069 6d70 6c79 204d 6963 726f 736f 6674   imply Microsoft
-00000a20: 2073 706f 6e73 6f72 7368 6970 2e0a 416e   sponsorship..An
-00000a30: 7920 7573 6520 6f66 2074 6869 7264 2d70  y use of third-p
-00000a40: 6172 7479 2074 7261 6465 6d61 726b 7320  arty trademarks 
-00000a50: 6f72 206c 6f67 6f73 2061 7265 2073 7562  or logos are sub
-00000a60: 6a65 6374 2074 6f20 7468 6f73 6520 7468  ject to those th
-00000a70: 6972 642d 7061 7274 7927 7320 706f 6c69  ird-party's poli
-00000a80: 6369 6573 2e0a                           cies..
+00000300: 7264 204c 6179 6572 730a 0a5b 215b 446f  rd Layers..[![Do
+00000310: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00000320: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000330: 2e69 6f2f 6261 6467 652f 646f 6373 2d70  .io/badge/docs-p
+00000340: 6173 7369 6e67 2d62 7269 6768 7467 7265  assing-brightgre
+00000350: 656e 295d 2868 7474 7073 3a2f 2f6d 6963  en)](https://mic
+00000360: 726f 736f 6674 2e67 6974 6875 622e 696f  rosoft.github.io
+00000370: 2f63 6c69 6666 6f72 646c 6179 6572 7329  /cliffordlayers)
+00000380: 0a0a 466f 7220 6465 7461 696c 7320 6162  ..For details ab
+00000390: 6f75 7420 7573 6167 6520 706c 6561 7365  out usage please
+000003a0: 2073 6565 205b 646f 6375 6d65 6e74 6174   see [documentat
+000003b0: 696f 6e5d 2868 7474 7073 3a2f 2f6d 6963  ion](https://mic
+000003c0: 726f 736f 6674 2e67 6974 6875 622e 696f  rosoft.github.io
+000003d0: 2f63 6c69 6666 6f72 646c 6179 6572 7329  /cliffordlayers)
+000003e0: 2e0a 4966 2079 6f75 2068 6176 6520 616e  ..If you have an
+000003f0: 7920 7175 6573 7469 6f6e 7320 6f72 2073  y questions or s
+00000400: 7567 6765 7374 696f 6e73 2070 6c65 6173  uggestions pleas
+00000410: 6520 6f70 656e 2061 205b 6469 7363 7573  e open a [discus
+00000420: 7369 6f6e 5d28 6874 7470 733a 2f2f 6769  sion](https://gi
+00000430: 7468 7562 2e63 6f6d 2f6d 6963 726f 736f  thub.com/microso
+00000440: 6674 2f63 6c69 6666 6f72 646c 6179 6572  ft/cliffordlayer
+00000450: 732f 6469 7363 7573 7369 6f6e 7329 2e20  s/discussions). 
+00000460: 4966 2079 6f75 206e 6f74 6963 6520 6120  If you notice a 
+00000470: 6275 672c 2070 6c65 6173 6520 6f70 656e  bug, please open
+00000480: 2061 6e20 5b69 7373 7565 5d28 6874 7470   an [issue](http
+00000490: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+000004a0: 6963 726f 736f 6674 2f63 6c69 6666 6f72  icrosoft/cliffor
+000004b0: 646c 6179 6572 732f 6973 7375 6573 292e  dlayers/issues).
+000004c0: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+000004d0: 6e0a 0a60 6060 6261 7368 0a70 6970 2069  n..```bash.pip i
+000004e0: 6e73 7461 6c6c 2063 6c69 6666 6f72 646c  nstall cliffordl
+000004f0: 6179 6572 730a 6060 600a 0a0a 2323 2043  ayers.```...## C
+00000500: 6974 6174 696f 6e0a 0a49 6620 796f 7520  itation..If you 
+00000510: 6669 6e64 206f 7572 2077 6f72 6b20 616e  find our work an
+00000520: 642f 6f72 206f 7572 2063 6f64 6520 7573  d/or our code us
+00000530: 6566 756c 2c20 706c 6561 7365 2063 6974  eful, please cit
+00000540: 6520 7573 2076 6961 3a0a 0a60 6060 6269  e us via:..```bi
+00000550: 6274 6578 0a40 6172 7469 636c 657b 6272  btex.@article{br
+00000560: 616e 6473 7465 7474 6572 3230 3232 636c  andstetter2022cl
+00000570: 6966 666f 7264 2c0a 2020 7469 746c 653d  ifford,.  title=
+00000580: 7b43 6c69 6666 6f72 6420 4e65 7572 616c  {Clifford Neural
+00000590: 204c 6179 6572 7320 666f 7220 5044 4520   Layers for PDE 
+000005a0: 4d6f 6465 6c69 6e67 7d2c 0a20 2061 7574  Modeling},.  aut
+000005b0: 686f 723d 7b42 7261 6e64 7374 6574 7465  hor={Brandstette
+000005c0: 722c 204a 6f68 616e 6e65 7320 616e 6420  r, Johannes and 
+000005d0: 4265 7267 2c20 5269 616e 6e65 2076 616e  Berg, Rianne van
+000005e0: 2064 656e 2061 6e64 2057 656c 6c69 6e67   den and Welling
+000005f0: 2c20 4d61 7820 616e 6420 4775 7074 612c  , Max and Gupta,
+00000600: 204a 6179 6573 6820 4b7d 2c0a 2020 6a6f   Jayesh K},.  jo
+00000610: 7572 6e61 6c3d 7b61 7258 6976 2070 7265  urnal={arXiv pre
+00000620: 7072 696e 7420 6172 5869 763a 3232 3039  print arXiv:2209
+00000630: 2e30 3439 3334 7d2c 0a20 2079 6561 723d  .04934},.  year=
+00000640: 7b32 3032 327d 0a7d 0a0a 4061 7274 6963  {2022}.}..@artic
+00000650: 6c65 7b72 7568 6532 3032 3367 656f 6d65  le{ruhe2023geome
+00000660: 7472 6963 2c0a 2020 7469 746c 653d 7b47  tric,.  title={G
+00000670: 656f 6d65 7472 6963 2043 6c69 6666 6f72  eometric Cliffor
+00000680: 6420 416c 6765 6272 6120 4e65 7477 6f72  d Algebra Networ
+00000690: 6b73 7d2c 0a20 2061 7574 686f 723d 7b52  ks},.  author={R
+000006a0: 7568 652c 2044 6176 6964 2061 6e64 2047  uhe, David and G
+000006b0: 7570 7461 2c20 4a61 7965 7368 204b 2061  upta, Jayesh K a
+000006c0: 6e64 2064 6520 4b65 6e69 6e63 6b2c 2053  nd de Keninck, S
+000006d0: 7465 7665 6e20 616e 6420 5765 6c6c 696e  teven and Wellin
+000006e0: 672c 204d 6178 2061 6e64 2042 7261 6e64  g, Max and Brand
+000006f0: 7374 6574 7465 722c 204a 6f68 616e 6e65  stetter, Johanne
+00000700: 737d 2c0a 2020 6a6f 7572 6e61 6c3d 7b61  s},.  journal={a
+00000710: 7258 6976 2070 7265 7072 696e 7420 6172  rXiv preprint ar
+00000720: 5869 763a 3233 3032 2e30 3635 3934 7d2c  Xiv:2302.06594},
+00000730: 0a20 2079 6561 723d 7b32 3032 337d 0a7d  .  year={2023}.}
+00000740: 0a60 6060 0a0a 0a23 2320 436f 6e74 7269  .```...## Contri
+00000750: 6275 7469 6e67 0a0a 5468 6973 2070 726f  buting..This pro
+00000760: 6a65 6374 2077 656c 636f 6d65 7320 636f  ject welcomes co
+00000770: 6e74 7269 6275 7469 6f6e 7320 616e 6420  ntributions and 
+00000780: 7375 6767 6573 7469 6f6e 732e 2020 4d6f  suggestions.  Mo
+00000790: 7374 2063 6f6e 7472 6962 7574 696f 6e73  st contributions
+000007a0: 2072 6571 7569 7265 2079 6f75 2074 6f20   require you to 
+000007b0: 6167 7265 6520 746f 2061 0a43 6f6e 7472  agree to a.Contr
+000007c0: 6962 7574 6f72 204c 6963 656e 7365 2041  ibutor License A
+000007d0: 6772 6565 6d65 6e74 2028 434c 4129 2064  greement (CLA) d
+000007e0: 6563 6c61 7269 6e67 2074 6861 7420 796f  eclaring that yo
+000007f0: 7520 6861 7665 2074 6865 2072 6967 6874  u have the right
+00000800: 2074 6f2c 2061 6e64 2061 6374 7561 6c6c   to, and actuall
+00000810: 7920 646f 2c20 6772 616e 7420 7573 0a74  y do, grant us.t
+00000820: 6865 2072 6967 6874 7320 746f 2075 7365  he rights to use
+00000830: 2079 6f75 7220 636f 6e74 7269 6275 7469   your contributi
+00000840: 6f6e 2e20 466f 7220 6465 7461 696c 732c  on. For details,
+00000850: 2076 6973 6974 2068 7474 7073 3a2f 2f63   visit https://c
+00000860: 6c61 2e6f 7065 6e73 6f75 7263 652e 6d69  la.opensource.mi
+00000870: 6372 6f73 6f66 742e 636f 6d2e 0a0a 5768  crosoft.com...Wh
+00000880: 656e 2079 6f75 2073 7562 6d69 7420 6120  en you submit a 
+00000890: 7075 6c6c 2072 6571 7565 7374 2c20 6120  pull request, a 
+000008a0: 434c 4120 626f 7420 7769 6c6c 2061 7574  CLA bot will aut
+000008b0: 6f6d 6174 6963 616c 6c79 2064 6574 6572  omatically deter
+000008c0: 6d69 6e65 2077 6865 7468 6572 2079 6f75  mine whether you
+000008d0: 206e 6565 6420 746f 2070 726f 7669 6465   need to provide
+000008e0: 0a61 2043 4c41 2061 6e64 2064 6563 6f72  .a CLA and decor
+000008f0: 6174 6520 7468 6520 5052 2061 7070 726f  ate the PR appro
+00000900: 7072 6961 7465 6c79 2028 652e 672e 2c20  priately (e.g., 
+00000910: 7374 6174 7573 2063 6865 636b 2c20 636f  status check, co
+00000920: 6d6d 656e 7429 2e20 5369 6d70 6c79 2066  mment). Simply f
+00000930: 6f6c 6c6f 7720 7468 6520 696e 7374 7275  ollow the instru
+00000940: 6374 696f 6e73 0a70 726f 7669 6465 6420  ctions.provided 
+00000950: 6279 2074 6865 2062 6f74 2e20 596f 7520  by the bot. You 
+00000960: 7769 6c6c 206f 6e6c 7920 6e65 6564 2074  will only need t
+00000970: 6f20 646f 2074 6869 7320 6f6e 6365 2061  o do this once a
+00000980: 6372 6f73 7320 616c 6c20 7265 706f 7320  cross all repos 
+00000990: 7573 696e 6720 6f75 7220 434c 412e 0a0a  using our CLA...
+000009a0: 5468 6973 2070 726f 6a65 6374 2068 6173  This project has
+000009b0: 2061 646f 7074 6564 2074 6865 205b 4d69   adopted the [Mi
+000009c0: 6372 6f73 6f66 7420 4f70 656e 2053 6f75  crosoft Open Sou
+000009d0: 7263 6520 436f 6465 206f 6620 436f 6e64  rce Code of Cond
+000009e0: 7563 745d 2868 7474 7073 3a2f 2f6f 7065  uct](https://ope
+000009f0: 6e73 6f75 7263 652e 6d69 6372 6f73 6f66  nsource.microsof
+00000a00: 742e 636f 6d2f 636f 6465 6f66 636f 6e64  t.com/codeofcond
+00000a10: 7563 742f 292e 0a46 6f72 206d 6f72 6520  uct/)..For more 
+00000a20: 696e 666f 726d 6174 696f 6e20 7365 6520  information see 
+00000a30: 7468 6520 5b43 6f64 6520 6f66 2043 6f6e  the [Code of Con
+00000a40: 6475 6374 2046 4151 5d28 6874 7470 733a  duct FAQ](https:
+00000a50: 2f2f 6f70 656e 736f 7572 6365 2e6d 6963  //opensource.mic
+00000a60: 726f 736f 6674 2e63 6f6d 2f63 6f64 656f  rosoft.com/codeo
+00000a70: 6663 6f6e 6475 6374 2f66 6171 2f29 206f  fconduct/faq/) o
+00000a80: 720a 636f 6e74 6163 7420 5b6f 7065 6e63  r.contact [openc
+00000a90: 6f64 6540 6d69 6372 6f73 6f66 742e 636f  ode@microsoft.co
+00000aa0: 6d5d 286d 6169 6c74 6f3a 6f70 656e 636f  m](mailto:openco
+00000ab0: 6465 406d 6963 726f 736f 6674 2e63 6f6d  de@microsoft.com
+00000ac0: 2920 7769 7468 2061 6e79 2061 6464 6974  ) with any addit
+00000ad0: 696f 6e61 6c20 7175 6573 7469 6f6e 7320  ional questions 
+00000ae0: 6f72 2063 6f6d 6d65 6e74 732e 0a0a 2323  or comments...##
+00000af0: 2054 7261 6465 6d61 726b 730a 0a54 6869   Trademarks..Thi
+00000b00: 7320 7072 6f6a 6563 7420 6d61 7920 636f  s project may co
+00000b10: 6e74 6169 6e20 7472 6164 656d 6172 6b73  ntain trademarks
+00000b20: 206f 7220 6c6f 676f 7320 666f 7220 7072   or logos for pr
+00000b30: 6f6a 6563 7473 2c20 7072 6f64 7563 7473  ojects, products
+00000b40: 2c20 6f72 2073 6572 7669 6365 732e 2041  , or services. A
+00000b50: 7574 686f 7269 7a65 6420 7573 6520 6f66  uthorized use of
+00000b60: 204d 6963 726f 736f 6674 0a74 7261 6465   Microsoft.trade
+00000b70: 6d61 726b 7320 6f72 206c 6f67 6f73 2069  marks or logos i
+00000b80: 7320 7375 626a 6563 7420 746f 2061 6e64  s subject to and
+00000b90: 206d 7573 7420 666f 6c6c 6f77 0a5b 4d69   must follow.[Mi
+00000ba0: 6372 6f73 6f66 7427 7320 5472 6164 656d  crosoft's Tradem
+00000bb0: 6172 6b20 2620 4272 616e 6420 4775 6964  ark & Brand Guid
+00000bc0: 656c 696e 6573 5d28 6874 7470 733a 2f2f  elines](https://
+00000bd0: 7777 772e 6d69 6372 6f73 6f66 742e 636f  www.microsoft.co
+00000be0: 6d2f 656e 2d75 732f 6c65 6761 6c2f 696e  m/en-us/legal/in
+00000bf0: 7465 6c6c 6563 7475 616c 7072 6f70 6572  tellectualproper
+00000c00: 7479 2f74 7261 6465 6d61 726b 732f 7573  ty/trademarks/us
+00000c10: 6167 652f 6765 6e65 7261 6c29 2e0a 5573  age/general)..Us
+00000c20: 6520 6f66 204d 6963 726f 736f 6674 2074  e of Microsoft t
+00000c30: 7261 6465 6d61 726b 7320 6f72 206c 6f67  rademarks or log
+00000c40: 6f73 2069 6e20 6d6f 6469 6669 6564 2076  os in modified v
+00000c50: 6572 7369 6f6e 7320 6f66 2074 6869 7320  ersions of this 
+00000c60: 7072 6f6a 6563 7420 6d75 7374 206e 6f74  project must not
+00000c70: 2063 6175 7365 2063 6f6e 6675 7369 6f6e   cause confusion
+00000c80: 206f 7220 696d 706c 7920 4d69 6372 6f73   or imply Micros
+00000c90: 6f66 7420 7370 6f6e 736f 7273 6869 702e  oft sponsorship.
+00000ca0: 0a41 6e79 2075 7365 206f 6620 7468 6972  .Any use of thir
+00000cb0: 642d 7061 7274 7920 7472 6164 656d 6172  d-party trademar
+00000cc0: 6b73 206f 7220 6c6f 676f 7320 6172 6520  ks or logos are 
+00000cd0: 7375 626a 6563 7420 746f 2074 686f 7365  subject to those
+00000ce0: 2074 6869 7264 2d70 6172 7479 2773 2070   third-party's p
+00000cf0: 6f6c 6963 6965 732e 0a                   olicies..
```

### Comparing `cliffordlayers-0.1.0/README.md` & `cliffordlayers-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,121 +1,161 @@
-00000000: 0a23 2043 6c69 6666 6f72 6420 4e65 7572  .# Clifford Neur
-00000010: 616c 204c 6179 6572 730a 0a0a 0a3c 6120  al Layers....<a 
-00000020: 6872 6566 3d22 6874 7470 733a 2f2f 6172  href="https://ar
-00000030: 7869 762e 6f72 672f 6162 732f 3232 3039  xiv.org/abs/2209
-00000040: 2e30 3439 3334 223e 4c69 6e6b 2074 6f20  .04934">Link to 
-00000050: 7468 6520 7061 7065 723c 2f61 3e0a 0a49  the paper</a>..I
-00000060: 6620 796f 7520 6669 6e64 206f 7572 2077  f you find our w
-00000070: 6f72 6b20 616e 642f 6f72 206f 7572 2063  ork and/or our c
-00000080: 6f64 6520 7573 6566 756c 2c20 706c 6561  ode useful, plea
-00000090: 7365 2063 6974 6520 7573 2076 6961 3a0a  se cite us via:.
-000000a0: 0a60 6060 6269 6274 6578 0a40 6172 7469  .```bibtex.@arti
-000000b0: 636c 657b 6272 616e 6473 7465 7474 6572  cle{brandstetter
-000000c0: 3230 3232 636c 6966 666f 7264 2c0a 2020  2022clifford,.  
-000000d0: 7469 746c 653d 7b43 6c69 6666 6f72 6420  title={Clifford 
-000000e0: 4e65 7572 616c 204c 6179 6572 7320 666f  Neural Layers fo
-000000f0: 7220 5044 4520 4d6f 6465 6c69 6e67 7d2c  r PDE Modeling},
-00000100: 0a20 2061 7574 686f 723d 7b42 7261 6e64  .  author={Brand
-00000110: 7374 6574 7465 722c 204a 6f68 616e 6e65  stetter, Johanne
-00000120: 7320 616e 6420 4265 7267 2c20 5269 616e  s and Berg, Rian
-00000130: 6e65 2076 616e 2064 656e 2061 6e64 2057  ne van den and W
-00000140: 656c 6c69 6e67 2c20 4d61 7820 616e 6420  elling, Max and 
-00000150: 4775 7074 612c 204a 6179 6573 6820 4b7d  Gupta, Jayesh K}
-00000160: 2c0a 2020 6a6f 7572 6e61 6c3d 7b61 7258  ,.  journal={arX
-00000170: 6976 2070 7265 7072 696e 7420 6172 5869  iv preprint arXi
-00000180: 763a 3232 3039 2e30 3439 3334 7d2c 0a20  v:2209.04934},. 
-00000190: 2079 6561 723d 7b32 3032 327d 0a7d 0a60   year={2022}.}.`
-000001a0: 6060 0a0a 2323 2049 6e73 7461 6c6c 6174  ``..## Installat
-000001b0: 696f 6e0a 0a60 6060 6261 7368 0a70 6970  ion..```bash.pip
-000001c0: 2069 6e73 7461 6c6c 2063 6c69 6666 6f72   install cliffor
-000001d0: 646c 6179 6572 730a 6060 600a 0a23 2320  dlayers.```..## 
-000001e0: 436f 6e74 7269 6275 7469 6e67 0a0a 5468  Contributing..Th
-000001f0: 6973 2070 726f 6a65 6374 2077 656c 636f  is project welco
-00000200: 6d65 7320 636f 6e74 7269 6275 7469 6f6e  mes contribution
-00000210: 7320 616e 6420 7375 6767 6573 7469 6f6e  s and suggestion
-00000220: 732e 2020 4d6f 7374 2063 6f6e 7472 6962  s.  Most contrib
-00000230: 7574 696f 6e73 2072 6571 7569 7265 2079  utions require y
-00000240: 6f75 2074 6f20 6167 7265 6520 746f 2061  ou to agree to a
-00000250: 0a43 6f6e 7472 6962 7574 6f72 204c 6963  .Contributor Lic
-00000260: 656e 7365 2041 6772 6565 6d65 6e74 2028  ense Agreement (
-00000270: 434c 4129 2064 6563 6c61 7269 6e67 2074  CLA) declaring t
-00000280: 6861 7420 796f 7520 6861 7665 2074 6865  hat you have the
-00000290: 2072 6967 6874 2074 6f2c 2061 6e64 2061   right to, and a
-000002a0: 6374 7561 6c6c 7920 646f 2c20 6772 616e  ctually do, gran
-000002b0: 7420 7573 0a74 6865 2072 6967 6874 7320  t us.the rights 
-000002c0: 746f 2075 7365 2079 6f75 7220 636f 6e74  to use your cont
-000002d0: 7269 6275 7469 6f6e 2e20 466f 7220 6465  ribution. For de
-000002e0: 7461 696c 732c 2076 6973 6974 2068 7474  tails, visit htt
-000002f0: 7073 3a2f 2f63 6c61 2e6f 7065 6e73 6f75  ps://cla.opensou
-00000300: 7263 652e 6d69 6372 6f73 6f66 742e 636f  rce.microsoft.co
-00000310: 6d2e 0a0a 5768 656e 2079 6f75 2073 7562  m...When you sub
-00000320: 6d69 7420 6120 7075 6c6c 2072 6571 7565  mit a pull reque
-00000330: 7374 2c20 6120 434c 4120 626f 7420 7769  st, a CLA bot wi
-00000340: 6c6c 2061 7574 6f6d 6174 6963 616c 6c79  ll automatically
-00000350: 2064 6574 6572 6d69 6e65 2077 6865 7468   determine wheth
-00000360: 6572 2079 6f75 206e 6565 6420 746f 2070  er you need to p
-00000370: 726f 7669 6465 0a61 2043 4c41 2061 6e64  rovide.a CLA and
-00000380: 2064 6563 6f72 6174 6520 7468 6520 5052   decorate the PR
-00000390: 2061 7070 726f 7072 6961 7465 6c79 2028   appropriately (
-000003a0: 652e 672e 2c20 7374 6174 7573 2063 6865  e.g., status che
-000003b0: 636b 2c20 636f 6d6d 656e 7429 2e20 5369  ck, comment). Si
-000003c0: 6d70 6c79 2066 6f6c 6c6f 7720 7468 6520  mply follow the 
-000003d0: 696e 7374 7275 6374 696f 6e73 0a70 726f  instructions.pro
-000003e0: 7669 6465 6420 6279 2074 6865 2062 6f74  vided by the bot
-000003f0: 2e20 596f 7520 7769 6c6c 206f 6e6c 7920  . You will only 
-00000400: 6e65 6564 2074 6f20 646f 2074 6869 7320  need to do this 
-00000410: 6f6e 6365 2061 6372 6f73 7320 616c 6c20  once across all 
-00000420: 7265 706f 7320 7573 696e 6720 6f75 7220  repos using our 
-00000430: 434c 412e 0a0a 5468 6973 2070 726f 6a65  CLA...This proje
-00000440: 6374 2068 6173 2061 646f 7074 6564 2074  ct has adopted t
-00000450: 6865 205b 4d69 6372 6f73 6f66 7420 4f70  he [Microsoft Op
-00000460: 656e 2053 6f75 7263 6520 436f 6465 206f  en Source Code o
-00000470: 6620 436f 6e64 7563 745d 2868 7474 7073  f Conduct](https
-00000480: 3a2f 2f6f 7065 6e73 6f75 7263 652e 6d69  ://opensource.mi
-00000490: 6372 6f73 6f66 742e 636f 6d2f 636f 6465  crosoft.com/code
-000004a0: 6f66 636f 6e64 7563 742f 292e 0a46 6f72  ofconduct/)..For
-000004b0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-000004c0: 6e20 7365 6520 7468 6520 5b43 6f64 6520  n see the [Code 
-000004d0: 6f66 2043 6f6e 6475 6374 2046 4151 5d28  of Conduct FAQ](
-000004e0: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
-000004f0: 6365 2e6d 6963 726f 736f 6674 2e63 6f6d  ce.microsoft.com
-00000500: 2f63 6f64 656f 6663 6f6e 6475 6374 2f66  /codeofconduct/f
-00000510: 6171 2f29 206f 720a 636f 6e74 6163 7420  aq/) or.contact 
-00000520: 5b6f 7065 6e63 6f64 6540 6d69 6372 6f73  [opencode@micros
-00000530: 6f66 742e 636f 6d5d 286d 6169 6c74 6f3a  oft.com](mailto:
-00000540: 6f70 656e 636f 6465 406d 6963 726f 736f  opencode@microso
-00000550: 6674 2e63 6f6d 2920 7769 7468 2061 6e79  ft.com) with any
-00000560: 2061 6464 6974 696f 6e61 6c20 7175 6573   additional ques
-00000570: 7469 6f6e 7320 6f72 2063 6f6d 6d65 6e74  tions or comment
-00000580: 732e 0a0a 2323 2054 7261 6465 6d61 726b  s...## Trademark
-00000590: 730a 0a54 6869 7320 7072 6f6a 6563 7420  s..This project 
-000005a0: 6d61 7920 636f 6e74 6169 6e20 7472 6164  may contain trad
-000005b0: 656d 6172 6b73 206f 7220 6c6f 676f 7320  emarks or logos 
-000005c0: 666f 7220 7072 6f6a 6563 7473 2c20 7072  for projects, pr
-000005d0: 6f64 7563 7473 2c20 6f72 2073 6572 7669  oducts, or servi
-000005e0: 6365 732e 2041 7574 686f 7269 7a65 6420  ces. Authorized 
-000005f0: 7573 6520 6f66 204d 6963 726f 736f 6674  use of Microsoft
-00000600: 0a74 7261 6465 6d61 726b 7320 6f72 206c  .trademarks or l
-00000610: 6f67 6f73 2069 7320 7375 626a 6563 7420  ogos is subject 
-00000620: 746f 2061 6e64 206d 7573 7420 666f 6c6c  to and must foll
-00000630: 6f77 0a5b 4d69 6372 6f73 6f66 7427 7320  ow.[Microsoft's 
-00000640: 5472 6164 656d 6172 6b20 2620 4272 616e  Trademark & Bran
-00000650: 6420 4775 6964 656c 696e 6573 5d28 6874  d Guidelines](ht
-00000660: 7470 733a 2f2f 7777 772e 6d69 6372 6f73  tps://www.micros
-00000670: 6f66 742e 636f 6d2f 656e 2d75 732f 6c65  oft.com/en-us/le
-00000680: 6761 6c2f 696e 7465 6c6c 6563 7475 616c  gal/intellectual
-00000690: 7072 6f70 6572 7479 2f74 7261 6465 6d61  property/tradema
-000006a0: 726b 732f 7573 6167 652f 6765 6e65 7261  rks/usage/genera
-000006b0: 6c29 2e0a 5573 6520 6f66 204d 6963 726f  l)..Use of Micro
-000006c0: 736f 6674 2074 7261 6465 6d61 726b 7320  soft trademarks 
-000006d0: 6f72 206c 6f67 6f73 2069 6e20 6d6f 6469  or logos in modi
-000006e0: 6669 6564 2076 6572 7369 6f6e 7320 6f66  fied versions of
-000006f0: 2074 6869 7320 7072 6f6a 6563 7420 6d75   this project mu
-00000700: 7374 206e 6f74 2063 6175 7365 2063 6f6e  st not cause con
-00000710: 6675 7369 6f6e 206f 7220 696d 706c 7920  fusion or imply 
-00000720: 4d69 6372 6f73 6f66 7420 7370 6f6e 736f  Microsoft sponso
-00000730: 7273 6869 702e 0a41 6e79 2075 7365 206f  rship..Any use o
-00000740: 6620 7468 6972 642d 7061 7274 7920 7472  f third-party tr
-00000750: 6164 656d 6172 6b73 206f 7220 6c6f 676f  ademarks or logo
-00000760: 7320 6172 6520 7375 626a 6563 7420 746f  s are subject to
-00000770: 2074 686f 7365 2074 6869 7264 2d70 6172   those third-par
-00000780: 7479 2773 2070 6f6c 6963 6965 732e 0a    ty's policies..
+00000000: 0a23 2043 6c69 6666 6f72 6420 4c61 7965  .# Clifford Laye
+00000010: 7273 0a0a 5b21 5b44 6f63 756d 656e 7461  rs..[![Documenta
+00000020: 7469 6f6e 5d28 6874 7470 733a 2f2f 696d  tion](https://im
+00000030: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000040: 6765 2f64 6f63 732d 7061 7373 696e 672d  ge/docs-passing-
+00000050: 6272 6967 6874 6772 6565 6e29 5d28 6874  brightgreen)](ht
+00000060: 7470 733a 2f2f 6d69 6372 6f73 6f66 742e  tps://microsoft.
+00000070: 6769 7468 7562 2e69 6f2f 636c 6966 666f  github.io/cliffo
+00000080: 7264 6c61 7965 7273 290a 0a46 6f72 2064  rdlayers)..For d
+00000090: 6574 6169 6c73 2061 626f 7574 2075 7361  etails about usa
+000000a0: 6765 2070 6c65 6173 6520 7365 6520 5b64  ge please see [d
+000000b0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+000000c0: 7470 733a 2f2f 6d69 6372 6f73 6f66 742e  tps://microsoft.
+000000d0: 6769 7468 7562 2e69 6f2f 636c 6966 666f  github.io/cliffo
+000000e0: 7264 6c61 7965 7273 292e 0a49 6620 796f  rdlayers)..If yo
+000000f0: 7520 6861 7665 2061 6e79 2071 7565 7374  u have any quest
+00000100: 696f 6e73 206f 7220 7375 6767 6573 7469  ions or suggesti
+00000110: 6f6e 7320 706c 6561 7365 206f 7065 6e20  ons please open 
+00000120: 6120 5b64 6973 6375 7373 696f 6e5d 2868  a [discussion](h
+00000130: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000140: 6d2f 6d69 6372 6f73 6f66 742f 636c 6966  m/microsoft/clif
+00000150: 666f 7264 6c61 7965 7273 2f64 6973 6375  fordlayers/discu
+00000160: 7373 696f 6e73 292e 2049 6620 796f 7520  ssions). If you 
+00000170: 6e6f 7469 6365 2061 2062 7567 2c20 706c  notice a bug, pl
+00000180: 6561 7365 206f 7065 6e20 616e 205b 6973  ease open an [is
+00000190: 7375 655d 2868 7474 7073 3a2f 2f67 6974  sue](https://git
+000001a0: 6875 622e 636f 6d2f 6d69 6372 6f73 6f66  hub.com/microsof
+000001b0: 742f 636c 6966 666f 7264 6c61 7965 7273  t/cliffordlayers
+000001c0: 2f69 7373 7565 7329 2e0a 0a23 2320 496e  /issues)...## In
+000001d0: 7374 616c 6c61 7469 6f6e 0a0a 6060 6062  stallation..```b
+000001e0: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
+000001f0: 636c 6966 666f 7264 6c61 7965 7273 0a60  cliffordlayers.`
+00000200: 6060 0a0a 0a23 2320 4369 7461 7469 6f6e  ``...## Citation
+00000210: 0a0a 4966 2079 6f75 2066 696e 6420 6f75  ..If you find ou
+00000220: 7220 776f 726b 2061 6e64 2f6f 7220 6f75  r work and/or ou
+00000230: 7220 636f 6465 2075 7365 6675 6c2c 2070  r code useful, p
+00000240: 6c65 6173 6520 6369 7465 2075 7320 7669  lease cite us vi
+00000250: 613a 0a0a 6060 6062 6962 7465 780a 4061  a:..```bibtex.@a
+00000260: 7274 6963 6c65 7b62 7261 6e64 7374 6574  rticle{brandstet
+00000270: 7465 7232 3032 3263 6c69 6666 6f72 642c  ter2022clifford,
+00000280: 0a20 2074 6974 6c65 3d7b 436c 6966 666f  .  title={Cliffo
+00000290: 7264 204e 6575 7261 6c20 4c61 7965 7273  rd Neural Layers
+000002a0: 2066 6f72 2050 4445 204d 6f64 656c 696e   for PDE Modelin
+000002b0: 677d 2c0a 2020 6175 7468 6f72 3d7b 4272  g},.  author={Br
+000002c0: 616e 6473 7465 7474 6572 2c20 4a6f 6861  andstetter, Joha
+000002d0: 6e6e 6573 2061 6e64 2042 6572 672c 2052  nnes and Berg, R
+000002e0: 6961 6e6e 6520 7661 6e20 6465 6e20 616e  ianne van den an
+000002f0: 6420 5765 6c6c 696e 672c 204d 6178 2061  d Welling, Max a
+00000300: 6e64 2047 7570 7461 2c20 4a61 7965 7368  nd Gupta, Jayesh
+00000310: 204b 7d2c 0a20 206a 6f75 726e 616c 3d7b   K},.  journal={
+00000320: 6172 5869 7620 7072 6570 7269 6e74 2061  arXiv preprint a
+00000330: 7258 6976 3a32 3230 392e 3034 3933 347d  rXiv:2209.04934}
+00000340: 2c0a 2020 7965 6172 3d7b 3230 3232 7d0a  ,.  year={2022}.
+00000350: 7d0a 0a40 6172 7469 636c 657b 7275 6865  }..@article{ruhe
+00000360: 3230 3233 6765 6f6d 6574 7269 632c 0a20  2023geometric,. 
+00000370: 2074 6974 6c65 3d7b 4765 6f6d 6574 7269   title={Geometri
+00000380: 6320 436c 6966 666f 7264 2041 6c67 6562  c Clifford Algeb
+00000390: 7261 204e 6574 776f 726b 737d 2c0a 2020  ra Networks},.  
+000003a0: 6175 7468 6f72 3d7b 5275 6865 2c20 4461  author={Ruhe, Da
+000003b0: 7669 6420 616e 6420 4775 7074 612c 204a  vid and Gupta, J
+000003c0: 6179 6573 6820 4b20 616e 6420 6465 204b  ayesh K and de K
+000003d0: 656e 696e 636b 2c20 5374 6576 656e 2061  eninck, Steven a
+000003e0: 6e64 2057 656c 6c69 6e67 2c20 4d61 7820  nd Welling, Max 
+000003f0: 616e 6420 4272 616e 6473 7465 7474 6572  and Brandstetter
+00000400: 2c20 4a6f 6861 6e6e 6573 7d2c 0a20 206a  , Johannes},.  j
+00000410: 6f75 726e 616c 3d7b 6172 5869 7620 7072  ournal={arXiv pr
+00000420: 6570 7269 6e74 2061 7258 6976 3a32 3330  eprint arXiv:230
+00000430: 322e 3036 3539 347d 2c0a 2020 7965 6172  2.06594},.  year
+00000440: 3d7b 3230 3233 7d0a 7d0a 6060 600a 0a0a  ={2023}.}.```...
+00000450: 2323 2043 6f6e 7472 6962 7574 696e 670a  ## Contributing.
+00000460: 0a54 6869 7320 7072 6f6a 6563 7420 7765  .This project we
+00000470: 6c63 6f6d 6573 2063 6f6e 7472 6962 7574  lcomes contribut
+00000480: 696f 6e73 2061 6e64 2073 7567 6765 7374  ions and suggest
+00000490: 696f 6e73 2e20 204d 6f73 7420 636f 6e74  ions.  Most cont
+000004a0: 7269 6275 7469 6f6e 7320 7265 7175 6972  ributions requir
+000004b0: 6520 796f 7520 746f 2061 6772 6565 2074  e you to agree t
+000004c0: 6f20 610a 436f 6e74 7269 6275 746f 7220  o a.Contributor 
+000004d0: 4c69 6365 6e73 6520 4167 7265 656d 656e  License Agreemen
+000004e0: 7420 2843 4c41 2920 6465 636c 6172 696e  t (CLA) declarin
+000004f0: 6720 7468 6174 2079 6f75 2068 6176 6520  g that you have 
+00000500: 7468 6520 7269 6768 7420 746f 2c20 616e  the right to, an
+00000510: 6420 6163 7475 616c 6c79 2064 6f2c 2067  d actually do, g
+00000520: 7261 6e74 2075 730a 7468 6520 7269 6768  rant us.the righ
+00000530: 7473 2074 6f20 7573 6520 796f 7572 2063  ts to use your c
+00000540: 6f6e 7472 6962 7574 696f 6e2e 2046 6f72  ontribution. For
+00000550: 2064 6574 6169 6c73 2c20 7669 7369 7420   details, visit 
+00000560: 6874 7470 733a 2f2f 636c 612e 6f70 656e  https://cla.open
+00000570: 736f 7572 6365 2e6d 6963 726f 736f 6674  source.microsoft
+00000580: 2e63 6f6d 2e0a 0a57 6865 6e20 796f 7520  .com...When you 
+00000590: 7375 626d 6974 2061 2070 756c 6c20 7265  submit a pull re
+000005a0: 7175 6573 742c 2061 2043 4c41 2062 6f74  quest, a CLA bot
+000005b0: 2077 696c 6c20 6175 746f 6d61 7469 6361   will automatica
+000005c0: 6c6c 7920 6465 7465 726d 696e 6520 7768  lly determine wh
+000005d0: 6574 6865 7220 796f 7520 6e65 6564 2074  ether you need t
+000005e0: 6f20 7072 6f76 6964 650a 6120 434c 4120  o provide.a CLA 
+000005f0: 616e 6420 6465 636f 7261 7465 2074 6865  and decorate the
+00000600: 2050 5220 6170 7072 6f70 7269 6174 656c   PR appropriatel
+00000610: 7920 2865 2e67 2e2c 2073 7461 7475 7320  y (e.g., status 
+00000620: 6368 6563 6b2c 2063 6f6d 6d65 6e74 292e  check, comment).
+00000630: 2053 696d 706c 7920 666f 6c6c 6f77 2074   Simply follow t
+00000640: 6865 2069 6e73 7472 7563 7469 6f6e 730a  he instructions.
+00000650: 7072 6f76 6964 6564 2062 7920 7468 6520  provided by the 
+00000660: 626f 742e 2059 6f75 2077 696c 6c20 6f6e  bot. You will on
+00000670: 6c79 206e 6565 6420 746f 2064 6f20 7468  ly need to do th
+00000680: 6973 206f 6e63 6520 6163 726f 7373 2061  is once across a
+00000690: 6c6c 2072 6570 6f73 2075 7369 6e67 206f  ll repos using o
+000006a0: 7572 2043 4c41 2e0a 0a54 6869 7320 7072  ur CLA...This pr
+000006b0: 6f6a 6563 7420 6861 7320 6164 6f70 7465  oject has adopte
+000006c0: 6420 7468 6520 5b4d 6963 726f 736f 6674  d the [Microsoft
+000006d0: 204f 7065 6e20 536f 7572 6365 2043 6f64   Open Source Cod
+000006e0: 6520 6f66 2043 6f6e 6475 6374 5d28 6874  e of Conduct](ht
+000006f0: 7470 733a 2f2f 6f70 656e 736f 7572 6365  tps://opensource
+00000700: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f63  .microsoft.com/c
+00000710: 6f64 656f 6663 6f6e 6475 6374 2f29 2e0a  odeofconduct/)..
+00000720: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
+00000730: 7469 6f6e 2073 6565 2074 6865 205b 436f  tion see the [Co
+00000740: 6465 206f 6620 436f 6e64 7563 7420 4641  de of Conduct FA
+00000750: 515d 2868 7474 7073 3a2f 2f6f 7065 6e73  Q](https://opens
+00000760: 6f75 7263 652e 6d69 6372 6f73 6f66 742e  ource.microsoft.
+00000770: 636f 6d2f 636f 6465 6f66 636f 6e64 7563  com/codeofconduc
+00000780: 742f 6661 712f 2920 6f72 0a63 6f6e 7461  t/faq/) or.conta
+00000790: 6374 205b 6f70 656e 636f 6465 406d 6963  ct [opencode@mic
+000007a0: 726f 736f 6674 2e63 6f6d 5d28 6d61 696c  rosoft.com](mail
+000007b0: 746f 3a6f 7065 6e63 6f64 6540 6d69 6372  to:opencode@micr
+000007c0: 6f73 6f66 742e 636f 6d29 2077 6974 6820  osoft.com) with 
+000007d0: 616e 7920 6164 6469 7469 6f6e 616c 2071  any additional q
+000007e0: 7565 7374 696f 6e73 206f 7220 636f 6d6d  uestions or comm
+000007f0: 656e 7473 2e0a 0a23 2320 5472 6164 656d  ents...## Tradem
+00000800: 6172 6b73 0a0a 5468 6973 2070 726f 6a65  arks..This proje
+00000810: 6374 206d 6179 2063 6f6e 7461 696e 2074  ct may contain t
+00000820: 7261 6465 6d61 726b 7320 6f72 206c 6f67  rademarks or log
+00000830: 6f73 2066 6f72 2070 726f 6a65 6374 732c  os for projects,
+00000840: 2070 726f 6475 6374 732c 206f 7220 7365   products, or se
+00000850: 7276 6963 6573 2e20 4175 7468 6f72 697a  rvices. Authoriz
+00000860: 6564 2075 7365 206f 6620 4d69 6372 6f73  ed use of Micros
+00000870: 6f66 740a 7472 6164 656d 6172 6b73 206f  oft.trademarks o
+00000880: 7220 6c6f 676f 7320 6973 2073 7562 6a65  r logos is subje
+00000890: 6374 2074 6f20 616e 6420 6d75 7374 2066  ct to and must f
+000008a0: 6f6c 6c6f 770a 5b4d 6963 726f 736f 6674  ollow.[Microsoft
+000008b0: 2773 2054 7261 6465 6d61 726b 2026 2042  's Trademark & B
+000008c0: 7261 6e64 2047 7569 6465 6c69 6e65 735d  rand Guidelines]
+000008d0: 2868 7474 7073 3a2f 2f77 7777 2e6d 6963  (https://www.mic
+000008e0: 726f 736f 6674 2e63 6f6d 2f65 6e2d 7573  rosoft.com/en-us
+000008f0: 2f6c 6567 616c 2f69 6e74 656c 6c65 6374  /legal/intellect
+00000900: 7561 6c70 726f 7065 7274 792f 7472 6164  ualproperty/trad
+00000910: 656d 6172 6b73 2f75 7361 6765 2f67 656e  emarks/usage/gen
+00000920: 6572 616c 292e 0a55 7365 206f 6620 4d69  eral)..Use of Mi
+00000930: 6372 6f73 6f66 7420 7472 6164 656d 6172  crosoft trademar
+00000940: 6b73 206f 7220 6c6f 676f 7320 696e 206d  ks or logos in m
+00000950: 6f64 6966 6965 6420 7665 7273 696f 6e73  odified versions
+00000960: 206f 6620 7468 6973 2070 726f 6a65 6374   of this project
+00000970: 206d 7573 7420 6e6f 7420 6361 7573 6520   must not cause 
+00000980: 636f 6e66 7573 696f 6e20 6f72 2069 6d70  confusion or imp
+00000990: 6c79 204d 6963 726f 736f 6674 2073 706f  ly Microsoft spo
+000009a0: 6e73 6f72 7368 6970 2e0a 416e 7920 7573  nsorship..Any us
+000009b0: 6520 6f66 2074 6869 7264 2d70 6172 7479  e of third-party
+000009c0: 2074 7261 6465 6d61 726b 7320 6f72 206c   trademarks or l
+000009d0: 6f67 6f73 2061 7265 2073 7562 6a65 6374  ogos are subject
+000009e0: 2074 6f20 7468 6f73 6520 7468 6972 642d   to those third-
+000009f0: 7061 7274 7927 7320 706f 6c69 6369 6573  party's policies
+00000a00: 2e0a                                     ..
```

### Comparing `cliffordlayers-0.1.0/cliffordlayers.egg-info/PKG-INFO` & `cliffordlayers-0.1.1/cliffordlayers.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 636c 6966  : 2.1.Name: clif
 00000020: 666f 7264 6c61 7965 7273 0a56 6572 7369  fordlayers.Versi
-00000030: 6f6e 3a20 302e 312e 300a 5375 6d6d 6172  on: 0.1.0.Summar
+00000030: 6f6e 3a20 302e 312e 310a 5375 6d6d 6172  on: 0.1.1.Summar
 00000040: 793a 2041 2050 7954 6f72 6368 206c 6962  y: A PyTorch lib
 00000050: 7261 7279 2066 6f72 2043 6c69 6666 6f72  rary for Cliffor
 00000060: 6420 6c61 7965 7273 0a41 7574 686f 723a  d layers.Author:
 00000070: 204a 6179 6573 6820 4b2e 2047 7570 7461   Jayesh K. Gupta
 00000080: 2c20 4a6f 6861 6e6e 6573 2042 7261 6e64  , Johannes Brand
 00000090: 7374 6574 7465 722c 2044 6176 6964 2052  stetter, David R
 000000a0: 7568 652c 2061 6e64 2063 6f6e 7472 6962  uhe, and contrib
@@ -42,128 +42,167 @@
 00000290: 6961 6c20 496e 7465 6c6c 6967 656e 6365  ial Intelligence
 000002a0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
 000002b0: 3a20 3e3d 332e 360a 4465 7363 7269 7074  : >=3.6.Descript
 000002c0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
 000002d0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
 000002e0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
 000002f0: 4345 4e53 450a 0a0a 2320 436c 6966 666f  CENSE...# Cliffo
-00000300: 7264 204e 6575 7261 6c20 4c61 7965 7273  rd Neural Layers
-00000310: 0a0a 0a0a 3c61 2068 7265 663d 2268 7474  ....<a href="htt
-00000320: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-00000330: 6273 2f32 3230 392e 3034 3933 3422 3e4c  bs/2209.04934">L
-00000340: 696e 6b20 746f 2074 6865 2070 6170 6572  ink to the paper
-00000350: 3c2f 613e 0a0a 4966 2079 6f75 2066 696e  </a>..If you fin
-00000360: 6420 6f75 7220 776f 726b 2061 6e64 2f6f  d our work and/o
-00000370: 7220 6f75 7220 636f 6465 2075 7365 6675  r our code usefu
-00000380: 6c2c 2070 6c65 6173 6520 6369 7465 2075  l, please cite u
-00000390: 7320 7669 613a 0a0a 6060 6062 6962 7465  s via:..```bibte
-000003a0: 780a 4061 7274 6963 6c65 7b62 7261 6e64  x.@article{brand
-000003b0: 7374 6574 7465 7232 3032 3263 6c69 6666  stetter2022cliff
-000003c0: 6f72 642c 0a20 2074 6974 6c65 3d7b 436c  ord,.  title={Cl
-000003d0: 6966 666f 7264 204e 6575 7261 6c20 4c61  ifford Neural La
-000003e0: 7965 7273 2066 6f72 2050 4445 204d 6f64  yers for PDE Mod
-000003f0: 656c 696e 677d 2c0a 2020 6175 7468 6f72  eling},.  author
-00000400: 3d7b 4272 616e 6473 7465 7474 6572 2c20  ={Brandstetter, 
-00000410: 4a6f 6861 6e6e 6573 2061 6e64 2042 6572  Johannes and Ber
-00000420: 672c 2052 6961 6e6e 6520 7661 6e20 6465  g, Rianne van de
-00000430: 6e20 616e 6420 5765 6c6c 696e 672c 204d  n and Welling, M
-00000440: 6178 2061 6e64 2047 7570 7461 2c20 4a61  ax and Gupta, Ja
-00000450: 7965 7368 204b 7d2c 0a20 206a 6f75 726e  yesh K},.  journ
-00000460: 616c 3d7b 6172 5869 7620 7072 6570 7269  al={arXiv prepri
-00000470: 6e74 2061 7258 6976 3a32 3230 392e 3034  nt arXiv:2209.04
-00000480: 3933 347d 2c0a 2020 7965 6172 3d7b 3230  934},.  year={20
-00000490: 3232 7d0a 7d0a 6060 600a 0a23 2320 496e  22}.}.```..## In
-000004a0: 7374 616c 6c61 7469 6f6e 0a0a 6060 6062  stallation..```b
-000004b0: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
-000004c0: 636c 6966 666f 7264 6c61 7965 7273 0a60  cliffordlayers.`
-000004d0: 6060 0a0a 2323 2043 6f6e 7472 6962 7574  ``..## Contribut
-000004e0: 696e 670a 0a54 6869 7320 7072 6f6a 6563  ing..This projec
-000004f0: 7420 7765 6c63 6f6d 6573 2063 6f6e 7472  t welcomes contr
-00000500: 6962 7574 696f 6e73 2061 6e64 2073 7567  ibutions and sug
-00000510: 6765 7374 696f 6e73 2e20 204d 6f73 7420  gestions.  Most 
-00000520: 636f 6e74 7269 6275 7469 6f6e 7320 7265  contributions re
-00000530: 7175 6972 6520 796f 7520 746f 2061 6772  quire you to agr
-00000540: 6565 2074 6f20 610a 436f 6e74 7269 6275  ee to a.Contribu
-00000550: 746f 7220 4c69 6365 6e73 6520 4167 7265  tor License Agre
-00000560: 656d 656e 7420 2843 4c41 2920 6465 636c  ement (CLA) decl
-00000570: 6172 696e 6720 7468 6174 2079 6f75 2068  aring that you h
-00000580: 6176 6520 7468 6520 7269 6768 7420 746f  ave the right to
-00000590: 2c20 616e 6420 6163 7475 616c 6c79 2064  , and actually d
-000005a0: 6f2c 2067 7261 6e74 2075 730a 7468 6520  o, grant us.the 
-000005b0: 7269 6768 7473 2074 6f20 7573 6520 796f  rights to use yo
-000005c0: 7572 2063 6f6e 7472 6962 7574 696f 6e2e  ur contribution.
-000005d0: 2046 6f72 2064 6574 6169 6c73 2c20 7669   For details, vi
-000005e0: 7369 7420 6874 7470 733a 2f2f 636c 612e  sit https://cla.
-000005f0: 6f70 656e 736f 7572 6365 2e6d 6963 726f  opensource.micro
-00000600: 736f 6674 2e63 6f6d 2e0a 0a57 6865 6e20  soft.com...When 
-00000610: 796f 7520 7375 626d 6974 2061 2070 756c  you submit a pul
-00000620: 6c20 7265 7175 6573 742c 2061 2043 4c41  l request, a CLA
-00000630: 2062 6f74 2077 696c 6c20 6175 746f 6d61   bot will automa
-00000640: 7469 6361 6c6c 7920 6465 7465 726d 696e  tically determin
-00000650: 6520 7768 6574 6865 7220 796f 7520 6e65  e whether you ne
-00000660: 6564 2074 6f20 7072 6f76 6964 650a 6120  ed to provide.a 
-00000670: 434c 4120 616e 6420 6465 636f 7261 7465  CLA and decorate
-00000680: 2074 6865 2050 5220 6170 7072 6f70 7269   the PR appropri
-00000690: 6174 656c 7920 2865 2e67 2e2c 2073 7461  ately (e.g., sta
-000006a0: 7475 7320 6368 6563 6b2c 2063 6f6d 6d65  tus check, comme
-000006b0: 6e74 292e 2053 696d 706c 7920 666f 6c6c  nt). Simply foll
-000006c0: 6f77 2074 6865 2069 6e73 7472 7563 7469  ow the instructi
-000006d0: 6f6e 730a 7072 6f76 6964 6564 2062 7920  ons.provided by 
-000006e0: 7468 6520 626f 742e 2059 6f75 2077 696c  the bot. You wil
-000006f0: 6c20 6f6e 6c79 206e 6565 6420 746f 2064  l only need to d
-00000700: 6f20 7468 6973 206f 6e63 6520 6163 726f  o this once acro
-00000710: 7373 2061 6c6c 2072 6570 6f73 2075 7369  ss all repos usi
-00000720: 6e67 206f 7572 2043 4c41 2e0a 0a54 6869  ng our CLA...Thi
-00000730: 7320 7072 6f6a 6563 7420 6861 7320 6164  s project has ad
-00000740: 6f70 7465 6420 7468 6520 5b4d 6963 726f  opted the [Micro
-00000750: 736f 6674 204f 7065 6e20 536f 7572 6365  soft Open Source
-00000760: 2043 6f64 6520 6f66 2043 6f6e 6475 6374   Code of Conduct
-00000770: 5d28 6874 7470 733a 2f2f 6f70 656e 736f  ](https://openso
-00000780: 7572 6365 2e6d 6963 726f 736f 6674 2e63  urce.microsoft.c
-00000790: 6f6d 2f63 6f64 656f 6663 6f6e 6475 6374  om/codeofconduct
-000007a0: 2f29 2e0a 466f 7220 6d6f 7265 2069 6e66  /)..For more inf
-000007b0: 6f72 6d61 7469 6f6e 2073 6565 2074 6865  ormation see the
-000007c0: 205b 436f 6465 206f 6620 436f 6e64 7563   [Code of Conduc
-000007d0: 7420 4641 515d 2868 7474 7073 3a2f 2f6f  t FAQ](https://o
-000007e0: 7065 6e73 6f75 7263 652e 6d69 6372 6f73  pensource.micros
-000007f0: 6f66 742e 636f 6d2f 636f 6465 6f66 636f  oft.com/codeofco
-00000800: 6e64 7563 742f 6661 712f 2920 6f72 0a63  nduct/faq/) or.c
-00000810: 6f6e 7461 6374 205b 6f70 656e 636f 6465  ontact [opencode
-00000820: 406d 6963 726f 736f 6674 2e63 6f6d 5d28  @microsoft.com](
-00000830: 6d61 696c 746f 3a6f 7065 6e63 6f64 6540  mailto:opencode@
-00000840: 6d69 6372 6f73 6f66 742e 636f 6d29 2077  microsoft.com) w
-00000850: 6974 6820 616e 7920 6164 6469 7469 6f6e  ith any addition
-00000860: 616c 2071 7565 7374 696f 6e73 206f 7220  al questions or 
-00000870: 636f 6d6d 656e 7473 2e0a 0a23 2320 5472  comments...## Tr
-00000880: 6164 656d 6172 6b73 0a0a 5468 6973 2070  ademarks..This p
-00000890: 726f 6a65 6374 206d 6179 2063 6f6e 7461  roject may conta
-000008a0: 696e 2074 7261 6465 6d61 726b 7320 6f72  in trademarks or
-000008b0: 206c 6f67 6f73 2066 6f72 2070 726f 6a65   logos for proje
-000008c0: 6374 732c 2070 726f 6475 6374 732c 206f  cts, products, o
-000008d0: 7220 7365 7276 6963 6573 2e20 4175 7468  r services. Auth
-000008e0: 6f72 697a 6564 2075 7365 206f 6620 4d69  orized use of Mi
-000008f0: 6372 6f73 6f66 740a 7472 6164 656d 6172  crosoft.trademar
-00000900: 6b73 206f 7220 6c6f 676f 7320 6973 2073  ks or logos is s
-00000910: 7562 6a65 6374 2074 6f20 616e 6420 6d75  ubject to and mu
-00000920: 7374 2066 6f6c 6c6f 770a 5b4d 6963 726f  st follow.[Micro
-00000930: 736f 6674 2773 2054 7261 6465 6d61 726b  soft's Trademark
-00000940: 2026 2042 7261 6e64 2047 7569 6465 6c69   & Brand Guideli
-00000950: 6e65 735d 2868 7474 7073 3a2f 2f77 7777  nes](https://www
-00000960: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f65  .microsoft.com/e
-00000970: 6e2d 7573 2f6c 6567 616c 2f69 6e74 656c  n-us/legal/intel
-00000980: 6c65 6374 7561 6c70 726f 7065 7274 792f  lectualproperty/
-00000990: 7472 6164 656d 6172 6b73 2f75 7361 6765  trademarks/usage
-000009a0: 2f67 656e 6572 616c 292e 0a55 7365 206f  /general)..Use o
-000009b0: 6620 4d69 6372 6f73 6f66 7420 7472 6164  f Microsoft trad
-000009c0: 656d 6172 6b73 206f 7220 6c6f 676f 7320  emarks or logos 
-000009d0: 696e 206d 6f64 6966 6965 6420 7665 7273  in modified vers
-000009e0: 696f 6e73 206f 6620 7468 6973 2070 726f  ions of this pro
-000009f0: 6a65 6374 206d 7573 7420 6e6f 7420 6361  ject must not ca
-00000a00: 7573 6520 636f 6e66 7573 696f 6e20 6f72  use confusion or
-00000a10: 2069 6d70 6c79 204d 6963 726f 736f 6674   imply Microsoft
-00000a20: 2073 706f 6e73 6f72 7368 6970 2e0a 416e   sponsorship..An
-00000a30: 7920 7573 6520 6f66 2074 6869 7264 2d70  y use of third-p
-00000a40: 6172 7479 2074 7261 6465 6d61 726b 7320  arty trademarks 
-00000a50: 6f72 206c 6f67 6f73 2061 7265 2073 7562  or logos are sub
-00000a60: 6a65 6374 2074 6f20 7468 6f73 6520 7468  ject to those th
-00000a70: 6972 642d 7061 7274 7927 7320 706f 6c69  ird-party's poli
-00000a80: 6369 6573 2e0a                           cies..
+00000300: 7264 204c 6179 6572 730a 0a5b 215b 446f  rd Layers..[![Do
+00000310: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00000320: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000330: 2e69 6f2f 6261 6467 652f 646f 6373 2d70  .io/badge/docs-p
+00000340: 6173 7369 6e67 2d62 7269 6768 7467 7265  assing-brightgre
+00000350: 656e 295d 2868 7474 7073 3a2f 2f6d 6963  en)](https://mic
+00000360: 726f 736f 6674 2e67 6974 6875 622e 696f  rosoft.github.io
+00000370: 2f63 6c69 6666 6f72 646c 6179 6572 7329  /cliffordlayers)
+00000380: 0a0a 466f 7220 6465 7461 696c 7320 6162  ..For details ab
+00000390: 6f75 7420 7573 6167 6520 706c 6561 7365  out usage please
+000003a0: 2073 6565 205b 646f 6375 6d65 6e74 6174   see [documentat
+000003b0: 696f 6e5d 2868 7474 7073 3a2f 2f6d 6963  ion](https://mic
+000003c0: 726f 736f 6674 2e67 6974 6875 622e 696f  rosoft.github.io
+000003d0: 2f63 6c69 6666 6f72 646c 6179 6572 7329  /cliffordlayers)
+000003e0: 2e0a 4966 2079 6f75 2068 6176 6520 616e  ..If you have an
+000003f0: 7920 7175 6573 7469 6f6e 7320 6f72 2073  y questions or s
+00000400: 7567 6765 7374 696f 6e73 2070 6c65 6173  uggestions pleas
+00000410: 6520 6f70 656e 2061 205b 6469 7363 7573  e open a [discus
+00000420: 7369 6f6e 5d28 6874 7470 733a 2f2f 6769  sion](https://gi
+00000430: 7468 7562 2e63 6f6d 2f6d 6963 726f 736f  thub.com/microso
+00000440: 6674 2f63 6c69 6666 6f72 646c 6179 6572  ft/cliffordlayer
+00000450: 732f 6469 7363 7573 7369 6f6e 7329 2e20  s/discussions). 
+00000460: 4966 2079 6f75 206e 6f74 6963 6520 6120  If you notice a 
+00000470: 6275 672c 2070 6c65 6173 6520 6f70 656e  bug, please open
+00000480: 2061 6e20 5b69 7373 7565 5d28 6874 7470   an [issue](http
+00000490: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+000004a0: 6963 726f 736f 6674 2f63 6c69 6666 6f72  icrosoft/cliffor
+000004b0: 646c 6179 6572 732f 6973 7375 6573 292e  dlayers/issues).
+000004c0: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+000004d0: 6e0a 0a60 6060 6261 7368 0a70 6970 2069  n..```bash.pip i
+000004e0: 6e73 7461 6c6c 2063 6c69 6666 6f72 646c  nstall cliffordl
+000004f0: 6179 6572 730a 6060 600a 0a0a 2323 2043  ayers.```...## C
+00000500: 6974 6174 696f 6e0a 0a49 6620 796f 7520  itation..If you 
+00000510: 6669 6e64 206f 7572 2077 6f72 6b20 616e  find our work an
+00000520: 642f 6f72 206f 7572 2063 6f64 6520 7573  d/or our code us
+00000530: 6566 756c 2c20 706c 6561 7365 2063 6974  eful, please cit
+00000540: 6520 7573 2076 6961 3a0a 0a60 6060 6269  e us via:..```bi
+00000550: 6274 6578 0a40 6172 7469 636c 657b 6272  btex.@article{br
+00000560: 616e 6473 7465 7474 6572 3230 3232 636c  andstetter2022cl
+00000570: 6966 666f 7264 2c0a 2020 7469 746c 653d  ifford,.  title=
+00000580: 7b43 6c69 6666 6f72 6420 4e65 7572 616c  {Clifford Neural
+00000590: 204c 6179 6572 7320 666f 7220 5044 4520   Layers for PDE 
+000005a0: 4d6f 6465 6c69 6e67 7d2c 0a20 2061 7574  Modeling},.  aut
+000005b0: 686f 723d 7b42 7261 6e64 7374 6574 7465  hor={Brandstette
+000005c0: 722c 204a 6f68 616e 6e65 7320 616e 6420  r, Johannes and 
+000005d0: 4265 7267 2c20 5269 616e 6e65 2076 616e  Berg, Rianne van
+000005e0: 2064 656e 2061 6e64 2057 656c 6c69 6e67   den and Welling
+000005f0: 2c20 4d61 7820 616e 6420 4775 7074 612c  , Max and Gupta,
+00000600: 204a 6179 6573 6820 4b7d 2c0a 2020 6a6f   Jayesh K},.  jo
+00000610: 7572 6e61 6c3d 7b61 7258 6976 2070 7265  urnal={arXiv pre
+00000620: 7072 696e 7420 6172 5869 763a 3232 3039  print arXiv:2209
+00000630: 2e30 3439 3334 7d2c 0a20 2079 6561 723d  .04934},.  year=
+00000640: 7b32 3032 327d 0a7d 0a0a 4061 7274 6963  {2022}.}..@artic
+00000650: 6c65 7b72 7568 6532 3032 3367 656f 6d65  le{ruhe2023geome
+00000660: 7472 6963 2c0a 2020 7469 746c 653d 7b47  tric,.  title={G
+00000670: 656f 6d65 7472 6963 2043 6c69 6666 6f72  eometric Cliffor
+00000680: 6420 416c 6765 6272 6120 4e65 7477 6f72  d Algebra Networ
+00000690: 6b73 7d2c 0a20 2061 7574 686f 723d 7b52  ks},.  author={R
+000006a0: 7568 652c 2044 6176 6964 2061 6e64 2047  uhe, David and G
+000006b0: 7570 7461 2c20 4a61 7965 7368 204b 2061  upta, Jayesh K a
+000006c0: 6e64 2064 6520 4b65 6e69 6e63 6b2c 2053  nd de Keninck, S
+000006d0: 7465 7665 6e20 616e 6420 5765 6c6c 696e  teven and Wellin
+000006e0: 672c 204d 6178 2061 6e64 2042 7261 6e64  g, Max and Brand
+000006f0: 7374 6574 7465 722c 204a 6f68 616e 6e65  stetter, Johanne
+00000700: 737d 2c0a 2020 6a6f 7572 6e61 6c3d 7b61  s},.  journal={a
+00000710: 7258 6976 2070 7265 7072 696e 7420 6172  rXiv preprint ar
+00000720: 5869 763a 3233 3032 2e30 3635 3934 7d2c  Xiv:2302.06594},
+00000730: 0a20 2079 6561 723d 7b32 3032 337d 0a7d  .  year={2023}.}
+00000740: 0a60 6060 0a0a 0a23 2320 436f 6e74 7269  .```...## Contri
+00000750: 6275 7469 6e67 0a0a 5468 6973 2070 726f  buting..This pro
+00000760: 6a65 6374 2077 656c 636f 6d65 7320 636f  ject welcomes co
+00000770: 6e74 7269 6275 7469 6f6e 7320 616e 6420  ntributions and 
+00000780: 7375 6767 6573 7469 6f6e 732e 2020 4d6f  suggestions.  Mo
+00000790: 7374 2063 6f6e 7472 6962 7574 696f 6e73  st contributions
+000007a0: 2072 6571 7569 7265 2079 6f75 2074 6f20   require you to 
+000007b0: 6167 7265 6520 746f 2061 0a43 6f6e 7472  agree to a.Contr
+000007c0: 6962 7574 6f72 204c 6963 656e 7365 2041  ibutor License A
+000007d0: 6772 6565 6d65 6e74 2028 434c 4129 2064  greement (CLA) d
+000007e0: 6563 6c61 7269 6e67 2074 6861 7420 796f  eclaring that yo
+000007f0: 7520 6861 7665 2074 6865 2072 6967 6874  u have the right
+00000800: 2074 6f2c 2061 6e64 2061 6374 7561 6c6c   to, and actuall
+00000810: 7920 646f 2c20 6772 616e 7420 7573 0a74  y do, grant us.t
+00000820: 6865 2072 6967 6874 7320 746f 2075 7365  he rights to use
+00000830: 2079 6f75 7220 636f 6e74 7269 6275 7469   your contributi
+00000840: 6f6e 2e20 466f 7220 6465 7461 696c 732c  on. For details,
+00000850: 2076 6973 6974 2068 7474 7073 3a2f 2f63   visit https://c
+00000860: 6c61 2e6f 7065 6e73 6f75 7263 652e 6d69  la.opensource.mi
+00000870: 6372 6f73 6f66 742e 636f 6d2e 0a0a 5768  crosoft.com...Wh
+00000880: 656e 2079 6f75 2073 7562 6d69 7420 6120  en you submit a 
+00000890: 7075 6c6c 2072 6571 7565 7374 2c20 6120  pull request, a 
+000008a0: 434c 4120 626f 7420 7769 6c6c 2061 7574  CLA bot will aut
+000008b0: 6f6d 6174 6963 616c 6c79 2064 6574 6572  omatically deter
+000008c0: 6d69 6e65 2077 6865 7468 6572 2079 6f75  mine whether you
+000008d0: 206e 6565 6420 746f 2070 726f 7669 6465   need to provide
+000008e0: 0a61 2043 4c41 2061 6e64 2064 6563 6f72  .a CLA and decor
+000008f0: 6174 6520 7468 6520 5052 2061 7070 726f  ate the PR appro
+00000900: 7072 6961 7465 6c79 2028 652e 672e 2c20  priately (e.g., 
+00000910: 7374 6174 7573 2063 6865 636b 2c20 636f  status check, co
+00000920: 6d6d 656e 7429 2e20 5369 6d70 6c79 2066  mment). Simply f
+00000930: 6f6c 6c6f 7720 7468 6520 696e 7374 7275  ollow the instru
+00000940: 6374 696f 6e73 0a70 726f 7669 6465 6420  ctions.provided 
+00000950: 6279 2074 6865 2062 6f74 2e20 596f 7520  by the bot. You 
+00000960: 7769 6c6c 206f 6e6c 7920 6e65 6564 2074  will only need t
+00000970: 6f20 646f 2074 6869 7320 6f6e 6365 2061  o do this once a
+00000980: 6372 6f73 7320 616c 6c20 7265 706f 7320  cross all repos 
+00000990: 7573 696e 6720 6f75 7220 434c 412e 0a0a  using our CLA...
+000009a0: 5468 6973 2070 726f 6a65 6374 2068 6173  This project has
+000009b0: 2061 646f 7074 6564 2074 6865 205b 4d69   adopted the [Mi
+000009c0: 6372 6f73 6f66 7420 4f70 656e 2053 6f75  crosoft Open Sou
+000009d0: 7263 6520 436f 6465 206f 6620 436f 6e64  rce Code of Cond
+000009e0: 7563 745d 2868 7474 7073 3a2f 2f6f 7065  uct](https://ope
+000009f0: 6e73 6f75 7263 652e 6d69 6372 6f73 6f66  nsource.microsof
+00000a00: 742e 636f 6d2f 636f 6465 6f66 636f 6e64  t.com/codeofcond
+00000a10: 7563 742f 292e 0a46 6f72 206d 6f72 6520  uct/)..For more 
+00000a20: 696e 666f 726d 6174 696f 6e20 7365 6520  information see 
+00000a30: 7468 6520 5b43 6f64 6520 6f66 2043 6f6e  the [Code of Con
+00000a40: 6475 6374 2046 4151 5d28 6874 7470 733a  duct FAQ](https:
+00000a50: 2f2f 6f70 656e 736f 7572 6365 2e6d 6963  //opensource.mic
+00000a60: 726f 736f 6674 2e63 6f6d 2f63 6f64 656f  rosoft.com/codeo
+00000a70: 6663 6f6e 6475 6374 2f66 6171 2f29 206f  fconduct/faq/) o
+00000a80: 720a 636f 6e74 6163 7420 5b6f 7065 6e63  r.contact [openc
+00000a90: 6f64 6540 6d69 6372 6f73 6f66 742e 636f  ode@microsoft.co
+00000aa0: 6d5d 286d 6169 6c74 6f3a 6f70 656e 636f  m](mailto:openco
+00000ab0: 6465 406d 6963 726f 736f 6674 2e63 6f6d  de@microsoft.com
+00000ac0: 2920 7769 7468 2061 6e79 2061 6464 6974  ) with any addit
+00000ad0: 696f 6e61 6c20 7175 6573 7469 6f6e 7320  ional questions 
+00000ae0: 6f72 2063 6f6d 6d65 6e74 732e 0a0a 2323  or comments...##
+00000af0: 2054 7261 6465 6d61 726b 730a 0a54 6869   Trademarks..Thi
+00000b00: 7320 7072 6f6a 6563 7420 6d61 7920 636f  s project may co
+00000b10: 6e74 6169 6e20 7472 6164 656d 6172 6b73  ntain trademarks
+00000b20: 206f 7220 6c6f 676f 7320 666f 7220 7072   or logos for pr
+00000b30: 6f6a 6563 7473 2c20 7072 6f64 7563 7473  ojects, products
+00000b40: 2c20 6f72 2073 6572 7669 6365 732e 2041  , or services. A
+00000b50: 7574 686f 7269 7a65 6420 7573 6520 6f66  uthorized use of
+00000b60: 204d 6963 726f 736f 6674 0a74 7261 6465   Microsoft.trade
+00000b70: 6d61 726b 7320 6f72 206c 6f67 6f73 2069  marks or logos i
+00000b80: 7320 7375 626a 6563 7420 746f 2061 6e64  s subject to and
+00000b90: 206d 7573 7420 666f 6c6c 6f77 0a5b 4d69   must follow.[Mi
+00000ba0: 6372 6f73 6f66 7427 7320 5472 6164 656d  crosoft's Tradem
+00000bb0: 6172 6b20 2620 4272 616e 6420 4775 6964  ark & Brand Guid
+00000bc0: 656c 696e 6573 5d28 6874 7470 733a 2f2f  elines](https://
+00000bd0: 7777 772e 6d69 6372 6f73 6f66 742e 636f  www.microsoft.co
+00000be0: 6d2f 656e 2d75 732f 6c65 6761 6c2f 696e  m/en-us/legal/in
+00000bf0: 7465 6c6c 6563 7475 616c 7072 6f70 6572  tellectualproper
+00000c00: 7479 2f74 7261 6465 6d61 726b 732f 7573  ty/trademarks/us
+00000c10: 6167 652f 6765 6e65 7261 6c29 2e0a 5573  age/general)..Us
+00000c20: 6520 6f66 204d 6963 726f 736f 6674 2074  e of Microsoft t
+00000c30: 7261 6465 6d61 726b 7320 6f72 206c 6f67  rademarks or log
+00000c40: 6f73 2069 6e20 6d6f 6469 6669 6564 2076  os in modified v
+00000c50: 6572 7369 6f6e 7320 6f66 2074 6869 7320  ersions of this 
+00000c60: 7072 6f6a 6563 7420 6d75 7374 206e 6f74  project must not
+00000c70: 2063 6175 7365 2063 6f6e 6675 7369 6f6e   cause confusion
+00000c80: 206f 7220 696d 706c 7920 4d69 6372 6f73   or imply Micros
+00000c90: 6f66 7420 7370 6f6e 736f 7273 6869 702e  oft sponsorship.
+00000ca0: 0a41 6e79 2075 7365 206f 6620 7468 6972  .Any use of thir
+00000cb0: 642d 7061 7274 7920 7472 6164 656d 6172  d-party trademar
+00000cc0: 6b73 206f 7220 6c6f 676f 7320 6172 6520  ks or logos are 
+00000cd0: 7375 626a 6563 7420 746f 2074 686f 7365  subject to those
+00000ce0: 2074 6869 7264 2d70 6172 7479 2773 2070   third-party's p
+00000cf0: 6f6c 6963 6965 732e 0a                   olicies..
```

### Comparing `cliffordlayers-0.1.0/setup.py` & `cliffordlayers-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+
 import os.path as osp
 
 from setuptools import find_packages, setup
 
 with open("README.md") as fh:
     long_description = fh.read()
```

### Comparing `cliffordlayers-0.1.0/tests/test_CliffordNet2d.py` & `cliffordlayers-0.1.1/tests/test_CliffordNet2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+
 import torch
 import torch.nn.functional as F 
 from cliffordlayers.models.utils import partialclass
 from cliffordlayers.models.models_2d import (
     CliffordNet2d,
     CliffordBasicBlock2d,
     CliffordFourierBasicBlock2d,
```

### Comparing `cliffordlayers-0.1.0/tests/test_CliffordNet3d.py` & `cliffordlayers-0.1.1/tests/test_CliffordNet3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+
 import torch
 import torch.nn.functional as F 
 from cliffordlayers.models.models_3d import (
     CliffordNet3d,
     CliffordFourierBasicBlock3d,
 )
```

### Comparing `cliffordlayers-0.1.0/tests/test_clifford_batchnorm.py` & `cliffordlayers-0.1.1/tests/test_clifford_batchnorm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+
 import torch
 
 from cliffordlayers.nn.functional.batchnorm import (
     clifford_batch_norm,
     complex_batch_norm,
 )
 from cliffordlayers.nn.modules.batchnorm import (
```

### Comparing `cliffordlayers-0.1.0/tests/test_clifford_convolution.py` & `cliffordlayers-0.1.1/tests/test_clifford_convolution.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+
 import torch
 import torch.nn.functional as F
 from cliffordlayers.nn.modules.cliffordconv import (
     CliffordConv1d,
     CliffordConv2d,
     CliffordConv3d,
 )
```

### Comparing `cliffordlayers-0.1.0/tests/test_clifford_convolution_custom.py` & `cliffordlayers-0.1.1/tests/test_clifford_convolution_custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+
 import torch
 from cliffordlayers.models.custom_layers import(
     CliffordConv2dEncoder,
     CliffordConv2dDecoder,
     CliffordConv3dEncoder,
     CliffordConv3dDecoder,
 )
```

### Comparing `cliffordlayers-0.1.0/tests/test_clifford_fourier.py` & `cliffordlayers-0.1.1/tests/test_clifford_fourier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from cliffordlayers.nn.modules.cliffordfourier_deprecated import (
     CliffordSpectralConv2d_deprecated, 
     CliffordSpectralConv3d_deprecated,
 )
```

### Comparing `cliffordlayers-0.1.0/tests/test_clifford_groupnorm.py` & `cliffordlayers-0.1.1/tests/test_clifford_groupnorm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+
 from typing import Tuple
 
 import torch
 
 from cliffordlayers.nn.functional.groupnorm import (
     clifford_group_norm,
     complex_group_norm,
```

### Comparing `cliffordlayers-0.1.0/tests/test_clifford_kernels.py` & `cliffordlayers-0.1.1/tests/test_clifford_kernels.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+
 import torch
 
 from cliffordlayers.cliffordkernels import (
     get_1d_clifford_kernel,
     get_2d_clifford_kernel,
     get_3d_clifford_kernel,
     get_complex_kernel,
```

### Comparing `cliffordlayers-0.1.0/tests/test_clifford_linear.py` & `cliffordlayers-0.1.1/tests/test_clifford_linear.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from cliffordlayers.nn.modules.cliffordconv import (
     CliffordConv1d,
     CliffordConv2d,
     CliffordConv3d,
```

### Comparing `cliffordlayers-0.1.0/tests/test_clifford_rotation_kernel.py` & `cliffordlayers-0.1.1/tests/test_clifford_rotation_kernel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+
 import torch
 
 from cliffordlayers.cliffordkernels import get_2d_clifford_rotation_kernel, get_quaternion_rotation_kernel
 from cliffordlayers.signature import CliffordSignature
 
 
 def test_2d_clifford_rotation_kernel():
```

