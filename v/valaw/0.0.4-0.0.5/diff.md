# Comparing `tmp/valaw-0.0.4.tar.gz` & `tmp/valaw-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valaw-0.0.4.tar", last modified: Sat Apr 15 04:08:19 2023, max compression
+gzip compressed data, was "valaw-0.0.5.tar", last modified: Thu Apr 20 20:05:12 2023, max compression
```

## Comparing `valaw-0.0.4.tar` & `valaw-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 04:08:19.275044 valaw-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-04-13 23:03:00.000000 valaw-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1895 2023-04-15 04:08:19.275044 valaw-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2023-04-15 03:19:54.000000 valaw-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-15 04:08:19.276044 valaw-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1143 2023-04-15 03:57:53.000000 valaw-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 04:08:19.256621 valaw-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 04:08:19.262786 valaw-0.0.4/src/valaw/
--rw-rw-rw-   0        0        0       73 2023-04-13 23:03:00.000000 valaw-0.0.4/src/valaw/__init__.py
--rw-rw-rw-   0        0        0    13440 2023-04-15 03:43:20.000000 valaw-0.0.4/src/valaw/client.py
-drwxrwxrwx   0        0        0        0 2023-04-15 04:08:19.274044 valaw-0.0.4/src/valaw.egg-info/
--rw-rw-rw-   0        0        0     1895 2023-04-15 04:08:19.000000 valaw-0.0.4/src/valaw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-04-15 04:08:19.000000 valaw-0.0.4/src/valaw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 04:08:19.000000 valaw-0.0.4/src/valaw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-15 04:08:19.000000 valaw-0.0.4/src/valaw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-15 04:08:19.000000 valaw-0.0.4/src/valaw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 20:05:12.618703 valaw-0.0.5/
+-rw-rw-rw-   0        0        0     1090 2023-04-04 04:45:45.000000 valaw-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2306 2023-04-20 20:05:12.610672 valaw-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1623 2023-04-20 18:57:49.000000 valaw-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 20:05:12.618703 valaw-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1143 2023-04-20 19:36:11.000000 valaw-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:05:12.472818 valaw-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 20:05:12.521143 valaw-0.0.5/src/valaw/
+-rw-rw-rw-   0        0        0       73 2023-04-04 05:08:42.000000 valaw-0.0.5/src/valaw/__init__.py
+-rw-rw-rw-   0        0        0    13699 2023-04-20 19:46:04.000000 valaw-0.0.5/src/valaw/client.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:05:12.610672 valaw-0.0.5/src/valaw.egg-info/
+-rw-rw-rw-   0        0        0     2306 2023-04-20 20:05:12.000000 valaw-0.0.5/src/valaw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-04-20 20:05:12.000000 valaw-0.0.5/src/valaw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 20:05:12.000000 valaw-0.0.5/src/valaw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-20 20:05:12.000000 valaw-0.0.5/src/valaw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 20:05:12.000000 valaw-0.0.5/src/valaw.egg-info/top_level.txt
```

### Comparing `valaw-0.0.4/LICENSE` & `valaw-0.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `valaw-0.0.4/PKG-INFO` & `valaw-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2076 616c  : 2.1..Name: val
 00000020: 6177 0d0a 5665 7273 696f 6e3a 2030 2e30  aw..Version: 0.0
-00000030: 2e34 0d0a 5375 6d6d 6172 793a 2041 6e20  .4..Summary: An 
+00000030: 2e35 0d0a 5375 6d6d 6172 793a 2041 6e20  .5..Summary: An 
 00000040: 6173 796e 6368 726f 6e6f 7573 2041 5049  asynchronous API
 00000050: 2077 7261 7070 6572 2066 6f72 2056 414c   wrapper for VAL
 00000060: 4f52 414e 5427 7320 4150 490d 0a48 6f6d  ORANT's API..Hom
 00000070: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
 00000080: 6769 7468 7562 2e63 6f6d 2f4a 6574 3631  github.com/Jet61
 00000090: 322f 7661 6c61 770d 0a41 7574 686f 723a  2/valaw..Author:
 000000a0: 204a 6574 3631 320d 0a50 726f 6a65 6374   Jet612..Project
@@ -36,84 +36,110 @@
 00000230: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
 00000240: 6520 3a3a 2044 6576 656c 6f70 6572 730d  e :: Developers.
 00000250: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
 00000260: 3a20 3e3d 332e 380d 0a44 6573 6372 6970  : >=3.8..Descrip
 00000270: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
 00000280: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
 00000290: 0d0a 4c69 6365 6e73 652d 4669 6c65 3a20  ..License-File: 
-000002a0: 4c49 4345 4e53 450d 0a0d 0a3c 696d 6720  LICENSE....<img 
-000002b0: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-000002c0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-000002d0: 6e74 2e63 6f6d 2f4a 6574 3631 322f 7661  nt.com/Jet612/va
-000002e0: 6c61 772f 6d61 696e 2f61 7373 6574 732f  law/main/assets/
-000002f0: 6261 6e6e 6572 2e70 6e67 223e 0d0a 0d0a  banner.png">....
-00000300: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000310: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000320: 742f 7661 6c61 772f 223e 3c69 6d67 2073  t/valaw/"><img s
-00000330: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000340: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000350: 762f 7661 6c61 773f 7374 796c 653d 666f  v/valaw?style=fo
-00000360: 722d 7468 652d 6261 6467 6522 3e0d 0a3c  r-the-badge">..<
-00000370: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000380: 6769 7468 7562 2e63 6f6d 2f4a 6574 3631  github.com/Jet61
-00000390: 322f 7661 6c61 772f 6973 7375 6573 223e  2/valaw/issues">
-000003a0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000003b0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000003c0: 2f67 6974 6875 622f 6973 7375 6573 2f6a  /github/issues/j
-000003d0: 6574 3631 322f 7661 6c61 773f 7374 796c  et612/valaw?styl
-000003e0: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
-000003f0: 3e0d 0a3c 6120 6872 6566 3d22 6874 7470  >..<a href="http
-00000400: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000410: 6a65 6374 2f76 616c 6177 2f22 3e3c 696d  ject/valaw/"><im
-00000420: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-00000430: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000440: 7069 2f64 6d2f 7661 6c61 773f 7374 796c  pi/dm/valaw?styl
-00000450: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
-00000460: 3e0d 0a3c 6120 6872 6566 3d22 6874 7470  >..<a href="http
-00000470: 733a 2f2f 7777 772e 7079 7468 6f6e 2e6f  s://www.python.o
-00000480: 7267 2f22 3e3c 696d 6720 7372 633d 2268  rg/"><img src="h
-00000490: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000004a0: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
-000004b0: 7369 6f6e 732f 7661 6c61 773f 7374 796c  sions/valaw?styl
-000004c0: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
-000004d0: 3e0d 0a3c 6120 6872 6566 3d22 6874 7470  >..<a href="http
-000004e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4a  s://github.com/J
-000004f0: 6574 3631 322f 7661 6c61 772f 6772 6170  et612/valaw/grap
-00000500: 6873 2f63 6f6e 7472 6962 7574 6f72 7322  hs/contributors"
-00000510: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00000520: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000530: 6f2f 6769 7468 7562 2f63 6f6e 7472 6962  o/github/contrib
-00000540: 7574 6f72 732f 6a65 7436 3132 2f76 616c  utors/jet612/val
-00000550: 6177 3f73 7479 6c65 3d66 6f72 2d74 6865  aw?style=for-the
-00000560: 2d62 6164 6765 223e 0d0a 0d0a 7661 6c61  -badge">....vala
-00000570: 7720 6973 2061 6e20 6173 796e 6368 726f  w is an asynchro
-00000580: 6e6f 7573 2041 5049 2077 7261 7070 6572  nous API wrapper
-00000590: 2066 6f72 2056 414c 4f52 414e 5427 7320   for VALORANT's 
-000005a0: 4150 492e 0d0a 0d0a 2320 446f 6375 6d65  API.....# Docume
-000005b0: 6e74 6174 696f 6e0d 0a54 6865 2064 6f63  ntation..The doc
-000005c0: 756d 656e 7461 7469 6f6e 2066 6f72 2074  umentation for t
-000005d0: 6869 7320 7772 6170 7065 7220 6361 6e20  his wrapper can 
-000005e0: 6265 2066 6f75 6e64 205b 6865 7265 5d28  be found [here](
-000005f0: 6874 7470 733a 2f2f 7661 6c61 772e 7265  https://valaw.re
-00000600: 6164 7468 6564 6f63 732e 696f 2f29 2e0d  adthedocs.io/)..
-00000610: 0a0d 0a23 2051 7569 636b 204c 696e 6b73  ...# Quick Links
-00000620: 0d0a 2d20 5b44 6973 636f 7264 5d28 6874  ..- [Discord](ht
-00000630: 7470 733a 2f2f 6469 7363 6f72 642e 6767  tps://discord.gg
-00000640: 2f6d 5658 7076 756e 4262 4629 0d0a 2d20  /mVXpvunBbF)..- 
-00000650: 5b50 7950 495d 2868 7474 7073 3a2f 2f70  [PyPI](https://p
-00000660: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000670: 7661 6c61 772f 290d 0a2d 205b 4769 7448  valaw/)..- [GitH
-00000680: 7562 5d28 6874 7470 733a 2f2f 6769 7468  ub](https://gith
-00000690: 7562 2e63 6f6d 2f4a 6574 3631 322f 7661  ub.com/Jet612/va
-000006a0: 6c61 7729 0d0a 2d20 5b44 6f63 756d 656e  law)..- [Documen
-000006b0: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
-000006c0: 7661 6c61 772e 7265 6164 7468 6564 6f63  valaw.readthedoc
-000006d0: 732e 696f 2f29 0d0a 0d0a 5468 6973 2070  s.io/)....This p
-000006e0: 726f 6a65 6374 2069 7320 6f77 6e65 6420  roject is owned 
-000006f0: 616e 6420 6d61 696e 7461 696e 6564 2062  and maintained b
-00000700: 7920 4a65 7436 3132 2c20 6f74 6865 7220  y Jet612, other 
-00000710: 636f 6e74 7269 6275 746f 7273 2063 616e  contributors can
-00000720: 2062 6520 666f 756e 6420 5b68 6572 655d   be found [here]
-00000730: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000740: 636f 6d2f 4a65 7436 3132 2f76 616c 6177  com/Jet612/valaw
-00000750: 2f67 7261 7068 732f 636f 6e74 7269 6275  /graphs/contribu
-00000760: 746f 7273 290d 0a                        tors)..
+000002a0: 4c49 4345 4e53 450d 0a0d 0a21 5b56 616c  LICENSE....![Val
+000002b0: 6177 2042 616e 6e65 725d 2868 7474 7073  aw Banner](https
+000002c0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+000002d0: 7263 6f6e 7465 6e74 2e63 6f6d 2f4a 6574  rcontent.com/Jet
+000002e0: 3631 322f 7661 6c61 772f 6d61 696e 2f61  612/valaw/main/a
+000002f0: 7373 6574 732f 6261 6e6e 6572 2e70 6e67  ssets/banner.png
+00000300: 290d 0a0d 0a0d 0a5b 215b 5079 5049 2056  )......[![PyPI V
+00000310: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
+00000320: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000330: 7970 692f 762f 7661 6c61 773f 7374 796c  ypi/v/valaw?styl
+00000340: 653d 666f 722d 7468 652d 6261 6467 6529  e=for-the-badge)
+00000350: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
+00000360: 7267 2f70 726f 6a65 6374 2f76 616c 6177  rg/project/valaw
+00000370: 2f29 0d0a 5b21 5b47 6974 4875 6220 4973  /)..[![GitHub Is
+00000380: 7375 6573 5d28 6874 7470 733a 2f2f 696d  sues](https://im
+00000390: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+000003a0: 6875 622f 6973 7375 6573 2f6a 6574 3631  hub/issues/jet61
+000003b0: 322f 7661 6c61 773f 7374 796c 653d 666f  2/valaw?style=fo
+000003c0: 722d 7468 652d 6261 6467 6529 5d28 6874  r-the-badge)](ht
+000003d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000003e0: 2f4a 6574 3631 322f 7661 6c61 772f 6973  /Jet612/valaw/is
+000003f0: 7375 6573 290d 0a5b 215b 5079 5049 2044  sues)..[![PyPI D
+00000400: 6f77 6e6c 6f61 6473 5d28 6874 7470 733a  ownloads](https:
+00000410: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000420: 2f70 7970 692f 646d 2f76 616c 6177 3f73  /pypi/dm/valaw?s
+00000430: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
+00000440: 6765 295d 2868 7474 7073 3a2f 2f70 7970  ge)](https://pyp
+00000450: 692e 6f72 672f 7072 6f6a 6563 742f 7661  i.org/project/va
+00000460: 6c61 772f 290d 0a5b 215b 5079 7468 6f6e  law/)..[![Python
+00000470: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
+00000480: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000490: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
+000004a0: 2f76 616c 6177 3f73 7479 6c65 3d66 6f72  /valaw?style=for
+000004b0: 2d74 6865 2d62 6164 6765 295d 2868 7474  -the-badge)](htt
+000004c0: 7073 3a2f 2f77 7777 2e70 7974 686f 6e2e  ps://www.python.
+000004d0: 6f72 672f 290d 0a5b 215b 4769 7448 7562  org/)..[![GitHub
+000004e0: 2043 6f6e 7472 6962 7574 6f72 735d 2868   Contributors](h
+000004f0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000500: 6473 2e69 6f2f 6769 7468 7562 2f63 6f6e  ds.io/github/con
+00000510: 7472 6962 7574 6f72 732f 6a65 7436 3132  tributors/jet612
+00000520: 2f76 616c 6177 3f73 7479 6c65 3d66 6f72  /valaw?style=for
+00000530: 2d74 6865 2d62 6164 6765 295d 2868 7474  -the-badge)](htt
+00000540: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000550: 4a65 7436 3132 2f76 616c 6177 2f67 7261  Jet612/valaw/gra
+00000560: 7068 732f 636f 6e74 7269 6275 746f 7273  phs/contributors
+00000570: 290d 0a0d 0a0d 0a76 616c 6177 2069 7320  )......valaw is 
+00000580: 616e 2061 7379 6e63 6872 6f6e 6f75 7320  an asynchronous 
+00000590: 4150 4920 7772 6170 7065 7220 666f 7220  API wrapper for 
+000005a0: 5641 4c4f 5241 4e54 2773 2041 5049 2e0d  VALORANT's API..
+000005b0: 0a0d 0a23 2044 6f63 756d 656e 7461 7469  ...# Documentati
+000005c0: 6f6e 0d0a 5468 6520 646f 6375 6d65 6e74  on..The document
+000005d0: 6174 696f 6e20 666f 7220 7468 6973 2077  ation for this w
+000005e0: 7261 7070 6572 2063 616e 2062 6520 666f  rapper can be fo
+000005f0: 756e 6420 5b68 6572 655d 2868 7474 7073  und [here](https
+00000600: 3a2f 2f76 616c 6177 2e72 6561 6474 6865  ://valaw.readthe
+00000610: 646f 6373 2e69 6f2f 292e 2052 6561 6420  docs.io/). Read 
+00000620: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
+00000630: 6e20 746f 206c 6561 726e 2068 6f77 2074  n to learn how t
+00000640: 6f20 6765 7420 7374 6172 7465 6420 7769  o get started wi
+00000650: 7468 2076 616c 6177 2e0d 0a54 6865 2064  th valaw...The d
+00000660: 6f63 756d 656e 7461 7469 6f6e 2061 6c73  ocumentation als
+00000670: 6f20 6861 7320 6120 6c69 7374 206f 6620  o has a list of 
+00000680: 616c 6c20 7468 6520 656e 6470 6f69 6e74  all the endpoint
+00000690: 7320 616e 6420 6578 616d 706c 6573 206f  s and examples o
+000006a0: 6e20 686f 7720 746f 2075 7365 2074 6865  n how to use the
+000006b0: 6d2e 0d0a 0d0a 2320 4865 6c70 2f53 7570  m.....# Help/Sup
+000006c0: 706f 7274 0d0a 4966 2079 6f75 206e 6565  port..If you nee
+000006d0: 6420 6865 6c70 2f73 7570 706f 7274 2077  d help/support w
+000006e0: 6974 6820 7661 6c61 772c 2079 6f75 2063  ith valaw, you c
+000006f0: 616e 206a 6f69 6e20 7468 6520 5b44 6973  an join the [Dis
+00000700: 636f 7264 2053 6572 7665 725d 2868 7474  cord Server](htt
+00000710: 7073 3a2f 2f64 6973 636f 7264 2e67 672f  ps://discord.gg/
+00000720: 6d56 5870 7675 6e42 6246 292e 2049 6620  mVXpvunBbF). If 
+00000730: 796f 7520 6861 7665 2069 6e63 6f75 6e74  you have incount
+00000740: 6572 6564 2061 2062 7567 2c20 796f 7520  ered a bug, you 
+00000750: 6361 6e20 616c 736f 206f 7065 6e20 616e  can also open an
+00000760: 2069 7373 7565 206f 6e20 7468 6520 5b47   issue on the [G
+00000770: 6974 4875 6220 7265 706f 7369 746f 7279  itHub repository
+00000780: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000790: 2e63 6f6d 2f4a 6574 3631 322f 7661 6c61  .com/Jet612/vala
+000007a0: 772f 6973 7375 6573 292e 0d0a 0d0a 2320  w/issues).....# 
+000007b0: 5175 6963 6b20 4c69 6e6b 730d 0a2d 205b  Quick Links..- [
+000007c0: 4469 7363 6f72 645d 2868 7474 7073 3a2f  Discord](https:/
+000007d0: 2f64 6973 636f 7264 2e67 672f 6d56 5870  /discord.gg/mVXp
+000007e0: 7675 6e42 6246 290d 0a2d 205b 5079 5049  vunBbF)..- [PyPI
+000007f0: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
+00000800: 7267 2f70 726f 6a65 6374 2f76 616c 6177  rg/project/valaw
+00000810: 2f29 0d0a 2d20 5b47 6974 4875 625d 2868  /)..- [GitHub](h
+00000820: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000830: 6d2f 4a65 7436 3132 2f76 616c 6177 290d  m/Jet612/valaw).
+00000840: 0a2d 205b 446f 6375 6d65 6e74 6174 696f  .- [Documentatio
+00000850: 6e5d 2868 7474 7073 3a2f 2f76 616c 6177  n](https://valaw
+00000860: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000870: 290d 0a0d 0a54 6869 7320 7072 6f6a 6563  )....This projec
+00000880: 7420 6973 206f 776e 6564 2061 6e64 206d  t is owned and m
+00000890: 6169 6e74 6169 6e65 6420 6279 204a 6574  aintained by Jet
+000008a0: 3631 322c 206f 7468 6572 2063 6f6e 7472  612, other contr
+000008b0: 6962 7574 6f72 7320 6361 6e20 6265 2066  ibutors can be f
+000008c0: 6f75 6e64 205b 6865 7265 5d28 6874 7470  ound [here](http
+000008d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4a  s://github.com/J
+000008e0: 6574 3631 322f 7661 6c61 772f 6772 6170  et612/valaw/grap
+000008f0: 6873 2f63 6f6e 7472 6962 7574 6f72 7329  hs/contributors)
+00000900: 0d0a                                     ..
```

### Comparing `valaw-0.0.4/setup.py` & `valaw-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_namespace_packages
 
 with open("README.md", "r") as readme:
     long_desc = readme.read()
 
 setup(
     name="valaw",
-    version="0.0.4",
+    version="0.0.5",
     author="Jet612",
     description="An asynchronous API wrapper for VALORANT's API",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/Jet612/valaw",
     project_urls={
         "Documentation": "https://valaw.readthedocs.io",
```

### Comparing `valaw-0.0.4/src/valaw/client.py` & `valaw-0.0.5/src/valaw/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,24 +12,26 @@
 class Exceptions:
     class InvalidCluster(ValueError):
         """Invalid Cluster."""
     class InvalidRegion(ValueError):
         """Invalid Region."""
 
 ### Content Verify ###
-async def verify_content(response):
+async def verify_content(response: aiohttp.ClientResponse):
     """
     Helper function to verify response content-type & deal
     with the response appropriately 
     """
     content_type = response.headers.get("Content-Type")
-    if content_type == "application/json; charset=utf-8" or content_type == "application/json":
+    print(content_type)
+    if content_type == "application/json; charset=utf-8" or content_type == "application/json" or content_type == "application/json;charset=utf-8":
         return await response.json()
-    elif content_type == "text/plain; charset=utf-8" or content_type == "text/plain":
+    elif content_type == "text/plain; charset=utf-8" or content_type == "text/plain" or content_type == "text/plain; charset=utf-8":
         return json.loads(await response.text())
+    return response
 
 ### Client ###
 class Client:
     def __init__(self, token: str, cluster: str):
         """Initialize the client."""
 
         # Checking if the arguments are valid
@@ -67,15 +69,15 @@
                 "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36",
                 "Accept-Language": "en-US,en;q=0.9",
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token
             }
             async with session.get(f"https://{cluster}.api.riotgames.com/riot/account/v1/accounts/by-puuid/{puuid}", headers=headers) as resp:
-                return await verify_content(resp)
+                return await verify_content(response=resp)
             
     async def GET_getByRiotId(self, gameName: str, tagLine: str, cluster: str = None) -> dict:
         """Get account by Riot ID."""
 
         if cluster != None:
             if cluster.lower() not in clusters:
                 raise Exceptions.InvalidCluster(f"Invalid cluster, valid clusters are: {clusters}.")
@@ -87,15 +89,15 @@
                 "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36",
                 "Accept-Language": "en-US,en;q=0.9",
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token
             }
             async with session.get(f"https://{cluster}.api.riotgames.com/riot/account/v1/accounts/by-riot-id/{gameName}/{tagLine}", headers=headers) as resp:
-                return await verify_content(resp)
+                return await verify_content(response=resp)
             
     async def GET_getByAccessToken(self, authorization: str, cluster: str = None) -> dict:
         """Get account by access token."""
 
         if cluster != None:
             if cluster.lower() not in clusters:
                 raise Exceptions.InvalidCluster(f"Invalid cluster, valid clusters are: {clusters}.")
@@ -108,15 +110,15 @@
                 "Accept-Language": "en-US,en;q=0.9",
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token,
                 "Authorization": authorization
             }
             async with session.get(f"https://{cluster}.api.riotgames.com/riot/account/v1/accounts/me", headers=headers) as resp:
-                return await verify_content(resp)
+                return await verify_content(response=resp)
             
     async def GET_getActiveShard(self, puuid: str, cluster: str = None) -> dict:
         """Get active shard for a player."""
 
         if cluster != None:
             if cluster.lower() not in clusters:
                 raise Exceptions.InvalidCluster(f"Invalid cluster, valid clusters are: {clusters}.")
@@ -128,15 +130,15 @@
                 "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36",
                 "Accept-Language": "en-US,en;q=0.9",
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token
             }
             async with session.get(f"https://{cluster}.api.riotgames.com/riot/account/v1/active-shards/by-game/val/by-puuid/{puuid}", headers=headers) as resp:
-                return await verify_content(resp)
+                return await verify_content(response=resp)
 
     ######################
     ### VAL-CONTENT-V1 ###
     ######################
 
     async def GET_getContent(self, region: str, locale: str = "") -> dict:
         """Get content optionally filtered by locale. A locale is recommended to be used for faster response times."""
@@ -154,15 +156,15 @@
                 "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36",
                 "Accept-Language": "en-US,en;q=0.9",
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token
             }
             async with session.get(f"https://{region}.api.riotgames.com/val/content/v1/contents{locale}", headers=headers) as resp:
-                return await verify_content(resp)
+                return await verify_content(response=resp)
 
     ####################
     ### VAL-MATCH-V1 ###
     #################### 
 
     async def GET_getMatch(self, matchId: str, region: str) -> dict:
         """Get match by id."""
@@ -175,15 +177,15 @@
                 "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36",
                 "Accept-Language": "en-US,en;q=0.9",
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token
             }
             async with session.get(f"https://{region}.api.riotgames.com/val/match/v1/matches/{matchId}", headers=headers) as resp:
-                return await verify_content(resp)
+                return await verify_content(response=resp)
             
     async def GET_getMatchlist(self, puuid: str, region: str) -> dict:
         """Get matchlist for games played by puuid."""
 
         if region.lower() not in regions:
             raise Exceptions.InvalidRegion(f"Invalid region, valid regions are: {regions}.")
 
@@ -192,15 +194,15 @@
                 "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36",
                 "Accept-Language": "en-US,en;q=0.9",
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token
             }
             async with session.get(f"https://{region}.api.riotgames.com/val/match/v1/matchlists/by-puuid/{puuid}", headers=headers) as resp:
-                return await verify_content(resp)
+                return await verify_content(response=resp)
             
     async def GET_getRecent(self, queue: str, region: str) -> dict:
         """
         Get recent matches.
 
         Returns a list of match ids that have completed 
         in the last 10 minutes for live regions and 12 hours 
@@ -222,15 +224,15 @@
                 "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36",
                 "Accept-Language": "en-US,en;q=0.9",
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token
             }
             async with session.get(f"https://{region}.api.riotgames.com/val/match/v1/recent-matches/by-queue/{queue}", headers=headers) as resp:
-                return await verify_content(resp)
+                return await verify_content(response=resp)
     
     #####################
     ### VAL-RANKED-V1 ###
     #####################
 
     async def GET_getLeaderboard(self, actId: str, region: str, size: int = 200, startIndex: int = 0) -> dict:
         """Get leaderboard for the competitive queue"""
@@ -246,15 +248,15 @@
                 "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36",
                 "Accept-Language": "en-US,en;q=0.9",
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token
             }
             async with session.get(f"https://{region}.api.riotgames.com/val/ranked/v1/leaderboards/by-act/{actId}?size={size}&startIndex={startIndex}", headers=headers) as resp:
-                return await verify_content(resp)
+                return await verify_content(response=resp)
 
     #####################
     ### VAL-STATUS-V1 ###
     #####################
 
     async def GET_getPlatformData(self, region: str) -> dict:
         """Get VALORANT status for the given platform."""
@@ -267,8 +269,8 @@
                 "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36",
                 "Accept-Language": "en-US,en;q=0.9",
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token
             }
             async with session.get(f"https://{region}.api.riotgames.com/val/status/v1/platform-data", headers=headers) as resp:
-                return await verify_content(resp)
+                return await verify_content(response=resp)
```

### Comparing `valaw-0.0.4/src/valaw.egg-info/PKG-INFO` & `valaw-0.0.5/src/valaw.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2076 616c  : 2.1..Name: val
 00000020: 6177 0d0a 5665 7273 696f 6e3a 2030 2e30  aw..Version: 0.0
-00000030: 2e34 0d0a 5375 6d6d 6172 793a 2041 6e20  .4..Summary: An 
+00000030: 2e35 0d0a 5375 6d6d 6172 793a 2041 6e20  .5..Summary: An 
 00000040: 6173 796e 6368 726f 6e6f 7573 2041 5049  asynchronous API
 00000050: 2077 7261 7070 6572 2066 6f72 2056 414c   wrapper for VAL
 00000060: 4f52 414e 5427 7320 4150 490d 0a48 6f6d  ORANT's API..Hom
 00000070: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
 00000080: 6769 7468 7562 2e63 6f6d 2f4a 6574 3631  github.com/Jet61
 00000090: 322f 7661 6c61 770d 0a41 7574 686f 723a  2/valaw..Author:
 000000a0: 204a 6574 3631 320d 0a50 726f 6a65 6374   Jet612..Project
@@ -36,84 +36,110 @@
 00000230: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
 00000240: 6520 3a3a 2044 6576 656c 6f70 6572 730d  e :: Developers.
 00000250: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
 00000260: 3a20 3e3d 332e 380d 0a44 6573 6372 6970  : >=3.8..Descrip
 00000270: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
 00000280: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
 00000290: 0d0a 4c69 6365 6e73 652d 4669 6c65 3a20  ..License-File: 
-000002a0: 4c49 4345 4e53 450d 0a0d 0a3c 696d 6720  LICENSE....<img 
-000002b0: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-000002c0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-000002d0: 6e74 2e63 6f6d 2f4a 6574 3631 322f 7661  nt.com/Jet612/va
-000002e0: 6c61 772f 6d61 696e 2f61 7373 6574 732f  law/main/assets/
-000002f0: 6261 6e6e 6572 2e70 6e67 223e 0d0a 0d0a  banner.png">....
-00000300: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000310: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000320: 742f 7661 6c61 772f 223e 3c69 6d67 2073  t/valaw/"><img s
-00000330: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000340: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000350: 762f 7661 6c61 773f 7374 796c 653d 666f  v/valaw?style=fo
-00000360: 722d 7468 652d 6261 6467 6522 3e0d 0a3c  r-the-badge">..<
-00000370: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000380: 6769 7468 7562 2e63 6f6d 2f4a 6574 3631  github.com/Jet61
-00000390: 322f 7661 6c61 772f 6973 7375 6573 223e  2/valaw/issues">
-000003a0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000003b0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000003c0: 2f67 6974 6875 622f 6973 7375 6573 2f6a  /github/issues/j
-000003d0: 6574 3631 322f 7661 6c61 773f 7374 796c  et612/valaw?styl
-000003e0: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
-000003f0: 3e0d 0a3c 6120 6872 6566 3d22 6874 7470  >..<a href="http
-00000400: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000410: 6a65 6374 2f76 616c 6177 2f22 3e3c 696d  ject/valaw/"><im
-00000420: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-00000430: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000440: 7069 2f64 6d2f 7661 6c61 773f 7374 796c  pi/dm/valaw?styl
-00000450: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
-00000460: 3e0d 0a3c 6120 6872 6566 3d22 6874 7470  >..<a href="http
-00000470: 733a 2f2f 7777 772e 7079 7468 6f6e 2e6f  s://www.python.o
-00000480: 7267 2f22 3e3c 696d 6720 7372 633d 2268  rg/"><img src="h
-00000490: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000004a0: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
-000004b0: 7369 6f6e 732f 7661 6c61 773f 7374 796c  sions/valaw?styl
-000004c0: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
-000004d0: 3e0d 0a3c 6120 6872 6566 3d22 6874 7470  >..<a href="http
-000004e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4a  s://github.com/J
-000004f0: 6574 3631 322f 7661 6c61 772f 6772 6170  et612/valaw/grap
-00000500: 6873 2f63 6f6e 7472 6962 7574 6f72 7322  hs/contributors"
-00000510: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00000520: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000530: 6f2f 6769 7468 7562 2f63 6f6e 7472 6962  o/github/contrib
-00000540: 7574 6f72 732f 6a65 7436 3132 2f76 616c  utors/jet612/val
-00000550: 6177 3f73 7479 6c65 3d66 6f72 2d74 6865  aw?style=for-the
-00000560: 2d62 6164 6765 223e 0d0a 0d0a 7661 6c61  -badge">....vala
-00000570: 7720 6973 2061 6e20 6173 796e 6368 726f  w is an asynchro
-00000580: 6e6f 7573 2041 5049 2077 7261 7070 6572  nous API wrapper
-00000590: 2066 6f72 2056 414c 4f52 414e 5427 7320   for VALORANT's 
-000005a0: 4150 492e 0d0a 0d0a 2320 446f 6375 6d65  API.....# Docume
-000005b0: 6e74 6174 696f 6e0d 0a54 6865 2064 6f63  ntation..The doc
-000005c0: 756d 656e 7461 7469 6f6e 2066 6f72 2074  umentation for t
-000005d0: 6869 7320 7772 6170 7065 7220 6361 6e20  his wrapper can 
-000005e0: 6265 2066 6f75 6e64 205b 6865 7265 5d28  be found [here](
-000005f0: 6874 7470 733a 2f2f 7661 6c61 772e 7265  https://valaw.re
-00000600: 6164 7468 6564 6f63 732e 696f 2f29 2e0d  adthedocs.io/)..
-00000610: 0a0d 0a23 2051 7569 636b 204c 696e 6b73  ...# Quick Links
-00000620: 0d0a 2d20 5b44 6973 636f 7264 5d28 6874  ..- [Discord](ht
-00000630: 7470 733a 2f2f 6469 7363 6f72 642e 6767  tps://discord.gg
-00000640: 2f6d 5658 7076 756e 4262 4629 0d0a 2d20  /mVXpvunBbF)..- 
-00000650: 5b50 7950 495d 2868 7474 7073 3a2f 2f70  [PyPI](https://p
-00000660: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000670: 7661 6c61 772f 290d 0a2d 205b 4769 7448  valaw/)..- [GitH
-00000680: 7562 5d28 6874 7470 733a 2f2f 6769 7468  ub](https://gith
-00000690: 7562 2e63 6f6d 2f4a 6574 3631 322f 7661  ub.com/Jet612/va
-000006a0: 6c61 7729 0d0a 2d20 5b44 6f63 756d 656e  law)..- [Documen
-000006b0: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
-000006c0: 7661 6c61 772e 7265 6164 7468 6564 6f63  valaw.readthedoc
-000006d0: 732e 696f 2f29 0d0a 0d0a 5468 6973 2070  s.io/)....This p
-000006e0: 726f 6a65 6374 2069 7320 6f77 6e65 6420  roject is owned 
-000006f0: 616e 6420 6d61 696e 7461 696e 6564 2062  and maintained b
-00000700: 7920 4a65 7436 3132 2c20 6f74 6865 7220  y Jet612, other 
-00000710: 636f 6e74 7269 6275 746f 7273 2063 616e  contributors can
-00000720: 2062 6520 666f 756e 6420 5b68 6572 655d   be found [here]
-00000730: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000740: 636f 6d2f 4a65 7436 3132 2f76 616c 6177  com/Jet612/valaw
-00000750: 2f67 7261 7068 732f 636f 6e74 7269 6275  /graphs/contribu
-00000760: 746f 7273 290d 0a                        tors)..
+000002a0: 4c49 4345 4e53 450d 0a0d 0a21 5b56 616c  LICENSE....![Val
+000002b0: 6177 2042 616e 6e65 725d 2868 7474 7073  aw Banner](https
+000002c0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+000002d0: 7263 6f6e 7465 6e74 2e63 6f6d 2f4a 6574  rcontent.com/Jet
+000002e0: 3631 322f 7661 6c61 772f 6d61 696e 2f61  612/valaw/main/a
+000002f0: 7373 6574 732f 6261 6e6e 6572 2e70 6e67  ssets/banner.png
+00000300: 290d 0a0d 0a0d 0a5b 215b 5079 5049 2056  )......[![PyPI V
+00000310: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
+00000320: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000330: 7970 692f 762f 7661 6c61 773f 7374 796c  ypi/v/valaw?styl
+00000340: 653d 666f 722d 7468 652d 6261 6467 6529  e=for-the-badge)
+00000350: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
+00000360: 7267 2f70 726f 6a65 6374 2f76 616c 6177  rg/project/valaw
+00000370: 2f29 0d0a 5b21 5b47 6974 4875 6220 4973  /)..[![GitHub Is
+00000380: 7375 6573 5d28 6874 7470 733a 2f2f 696d  sues](https://im
+00000390: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+000003a0: 6875 622f 6973 7375 6573 2f6a 6574 3631  hub/issues/jet61
+000003b0: 322f 7661 6c61 773f 7374 796c 653d 666f  2/valaw?style=fo
+000003c0: 722d 7468 652d 6261 6467 6529 5d28 6874  r-the-badge)](ht
+000003d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000003e0: 2f4a 6574 3631 322f 7661 6c61 772f 6973  /Jet612/valaw/is
+000003f0: 7375 6573 290d 0a5b 215b 5079 5049 2044  sues)..[![PyPI D
+00000400: 6f77 6e6c 6f61 6473 5d28 6874 7470 733a  ownloads](https:
+00000410: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000420: 2f70 7970 692f 646d 2f76 616c 6177 3f73  /pypi/dm/valaw?s
+00000430: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
+00000440: 6765 295d 2868 7474 7073 3a2f 2f70 7970  ge)](https://pyp
+00000450: 692e 6f72 672f 7072 6f6a 6563 742f 7661  i.org/project/va
+00000460: 6c61 772f 290d 0a5b 215b 5079 7468 6f6e  law/)..[![Python
+00000470: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
+00000480: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000490: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
+000004a0: 2f76 616c 6177 3f73 7479 6c65 3d66 6f72  /valaw?style=for
+000004b0: 2d74 6865 2d62 6164 6765 295d 2868 7474  -the-badge)](htt
+000004c0: 7073 3a2f 2f77 7777 2e70 7974 686f 6e2e  ps://www.python.
+000004d0: 6f72 672f 290d 0a5b 215b 4769 7448 7562  org/)..[![GitHub
+000004e0: 2043 6f6e 7472 6962 7574 6f72 735d 2868   Contributors](h
+000004f0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000500: 6473 2e69 6f2f 6769 7468 7562 2f63 6f6e  ds.io/github/con
+00000510: 7472 6962 7574 6f72 732f 6a65 7436 3132  tributors/jet612
+00000520: 2f76 616c 6177 3f73 7479 6c65 3d66 6f72  /valaw?style=for
+00000530: 2d74 6865 2d62 6164 6765 295d 2868 7474  -the-badge)](htt
+00000540: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000550: 4a65 7436 3132 2f76 616c 6177 2f67 7261  Jet612/valaw/gra
+00000560: 7068 732f 636f 6e74 7269 6275 746f 7273  phs/contributors
+00000570: 290d 0a0d 0a0d 0a76 616c 6177 2069 7320  )......valaw is 
+00000580: 616e 2061 7379 6e63 6872 6f6e 6f75 7320  an asynchronous 
+00000590: 4150 4920 7772 6170 7065 7220 666f 7220  API wrapper for 
+000005a0: 5641 4c4f 5241 4e54 2773 2041 5049 2e0d  VALORANT's API..
+000005b0: 0a0d 0a23 2044 6f63 756d 656e 7461 7469  ...# Documentati
+000005c0: 6f6e 0d0a 5468 6520 646f 6375 6d65 6e74  on..The document
+000005d0: 6174 696f 6e20 666f 7220 7468 6973 2077  ation for this w
+000005e0: 7261 7070 6572 2063 616e 2062 6520 666f  rapper can be fo
+000005f0: 756e 6420 5b68 6572 655d 2868 7474 7073  und [here](https
+00000600: 3a2f 2f76 616c 6177 2e72 6561 6474 6865  ://valaw.readthe
+00000610: 646f 6373 2e69 6f2f 292e 2052 6561 6420  docs.io/). Read 
+00000620: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
+00000630: 6e20 746f 206c 6561 726e 2068 6f77 2074  n to learn how t
+00000640: 6f20 6765 7420 7374 6172 7465 6420 7769  o get started wi
+00000650: 7468 2076 616c 6177 2e0d 0a54 6865 2064  th valaw...The d
+00000660: 6f63 756d 656e 7461 7469 6f6e 2061 6c73  ocumentation als
+00000670: 6f20 6861 7320 6120 6c69 7374 206f 6620  o has a list of 
+00000680: 616c 6c20 7468 6520 656e 6470 6f69 6e74  all the endpoint
+00000690: 7320 616e 6420 6578 616d 706c 6573 206f  s and examples o
+000006a0: 6e20 686f 7720 746f 2075 7365 2074 6865  n how to use the
+000006b0: 6d2e 0d0a 0d0a 2320 4865 6c70 2f53 7570  m.....# Help/Sup
+000006c0: 706f 7274 0d0a 4966 2079 6f75 206e 6565  port..If you nee
+000006d0: 6420 6865 6c70 2f73 7570 706f 7274 2077  d help/support w
+000006e0: 6974 6820 7661 6c61 772c 2079 6f75 2063  ith valaw, you c
+000006f0: 616e 206a 6f69 6e20 7468 6520 5b44 6973  an join the [Dis
+00000700: 636f 7264 2053 6572 7665 725d 2868 7474  cord Server](htt
+00000710: 7073 3a2f 2f64 6973 636f 7264 2e67 672f  ps://discord.gg/
+00000720: 6d56 5870 7675 6e42 6246 292e 2049 6620  mVXpvunBbF). If 
+00000730: 796f 7520 6861 7665 2069 6e63 6f75 6e74  you have incount
+00000740: 6572 6564 2061 2062 7567 2c20 796f 7520  ered a bug, you 
+00000750: 6361 6e20 616c 736f 206f 7065 6e20 616e  can also open an
+00000760: 2069 7373 7565 206f 6e20 7468 6520 5b47   issue on the [G
+00000770: 6974 4875 6220 7265 706f 7369 746f 7279  itHub repository
+00000780: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000790: 2e63 6f6d 2f4a 6574 3631 322f 7661 6c61  .com/Jet612/vala
+000007a0: 772f 6973 7375 6573 292e 0d0a 0d0a 2320  w/issues).....# 
+000007b0: 5175 6963 6b20 4c69 6e6b 730d 0a2d 205b  Quick Links..- [
+000007c0: 4469 7363 6f72 645d 2868 7474 7073 3a2f  Discord](https:/
+000007d0: 2f64 6973 636f 7264 2e67 672f 6d56 5870  /discord.gg/mVXp
+000007e0: 7675 6e42 6246 290d 0a2d 205b 5079 5049  vunBbF)..- [PyPI
+000007f0: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
+00000800: 7267 2f70 726f 6a65 6374 2f76 616c 6177  rg/project/valaw
+00000810: 2f29 0d0a 2d20 5b47 6974 4875 625d 2868  /)..- [GitHub](h
+00000820: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000830: 6d2f 4a65 7436 3132 2f76 616c 6177 290d  m/Jet612/valaw).
+00000840: 0a2d 205b 446f 6375 6d65 6e74 6174 696f  .- [Documentatio
+00000850: 6e5d 2868 7474 7073 3a2f 2f76 616c 6177  n](https://valaw
+00000860: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000870: 290d 0a0d 0a54 6869 7320 7072 6f6a 6563  )....This projec
+00000880: 7420 6973 206f 776e 6564 2061 6e64 206d  t is owned and m
+00000890: 6169 6e74 6169 6e65 6420 6279 204a 6574  aintained by Jet
+000008a0: 3631 322c 206f 7468 6572 2063 6f6e 7472  612, other contr
+000008b0: 6962 7574 6f72 7320 6361 6e20 6265 2066  ibutors can be f
+000008c0: 6f75 6e64 205b 6865 7265 5d28 6874 7470  ound [here](http
+000008d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4a  s://github.com/J
+000008e0: 6574 3631 322f 7661 6c61 772f 6772 6170  et612/valaw/grap
+000008f0: 6873 2f63 6f6e 7472 6962 7574 6f72 7329  hs/contributors)
+00000900: 0d0a                                     ..
```

