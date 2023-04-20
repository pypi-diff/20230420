# Comparing `tmp/oslili-0.6.tar.gz` & `tmp/oslili-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslili-0.6.tar", last modified: Thu Apr 20 13:06:41 2023, max compression
+gzip compressed data, was "oslili-0.7.tar", last modified: Thu Apr 20 13:08:48 2023, max compression
```

## Comparing `oslili-0.6.tar` & `oslili-0.7.tar`

### file list

```diff
@@ -1,572 +1,572 @@
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:06:41.669622 oslili-0.6/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2023-04-05 07:52:31.000000 oslili-0.6/LICENSE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2023-04-09 07:33:34.000000 oslili-0.6/NOTICE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2983 2023-04-20 13:06:41.669892 oslili-0.6/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2451 2023-04-20 04:48:38.000000 oslili-0.6/README.md
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:06:40.868809 oslili-0.6/oslili/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       77 2023-04-05 07:52:31.000000 oslili-0.6/oslili/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4524 2023-04-13 19:34:09.000000 oslili-0.6/oslili/identifier.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:06:41.668886 oslili-0.6/oslili/spdx/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      643 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/0BSD.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1931 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/389-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2529 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/AAL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      488 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ADSL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4676 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/AFL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4950 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/AFL-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8987 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/AFL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8948 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/AFL-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10334 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/AFL-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15839 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/AGPL-1.0-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15839 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/AGPL-1.0-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    34020 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/AGPL-3.0-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    34020 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/AGPL-3.0-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5642 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/AMDPLPA.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2358 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/AML.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2192 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/AMPAS.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1261 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ANTLR-PD-fallback.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      987 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ANTLR-PD.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      617 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/APAFML.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    46103 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/APL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19644 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/APSL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20151 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/APSL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19800 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/APSL-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20285 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/APSL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      731 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Abstyles.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      236 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/AdaCore-doc.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1776 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Adobe-2006.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1608 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Adobe-Glyph.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      893 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Afmparse.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11604 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Aladdin.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2507 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Apache-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2514 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Apache-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10280 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Apache-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      224 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/App-s2p.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6901 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Arphic-1999.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6060 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Artistic-1.0-Perl.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5184 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Artistic-1.0-cl8.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4854 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Artistic-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8764 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Artistic-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1573 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Autoconf-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1818 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Autoconf-exception-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      266 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Autoconf-exception-generic.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      768 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Autoconf-exception-macro.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1086 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-1-Clause.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2569 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-2-Clause-Patent.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1519 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-2-Clause-Views.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1267 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-2-Clause.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1646 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-3-Clause-Attribution.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1676 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-3-Clause-Clear.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2388 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-3-Clause-LBNL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1624 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-3-Clause-Modification.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1647 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-3-Clause-No-Military-License.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1709 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-3-Clause-No-Nuclear-License-2014.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1693 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-3-Clause-No-Nuclear-License.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1699 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-3-Clause-No-Nuclear-Warranty.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1820 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-3-Clause-Open-MPI.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1460 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-3-Clause.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1048 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-4-Clause-Shortened.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1771 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-4-Clause-UC.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1618 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-4-Clause.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      476 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-4.3RENO.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      781 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-4.3TAHOE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1626 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-Advertising-Acknowledgement.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1679 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-Attribution-HPND-disclaimer.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6244 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-Protection.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1301 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSD-Source-Code.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1338 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BSL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3424 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BUSL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      479 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Baekmuk.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1377 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Bahyph.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      603 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Barr.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      266 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Beerware.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      673 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Bison-exception-2.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    24219 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BitTorrent-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    27782 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BitTorrent-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      572 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Bitstream-Charter.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2318 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Bitstream-Vera.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1552 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/BlueOak-1.0.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      523 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Bootloader-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      647 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Borceux.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1096 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Brian-Gladman-3-Clause.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3451 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/C-UDA-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16125 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CAL-1.0-Combined-Work-Exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16125 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CAL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19046 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CATOSL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11405 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12572 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17126 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-2.5-AU.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12781 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-2.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19189 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-3.0-AT.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19218 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-3.0-DE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17572 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-3.0-IGO.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18371 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-3.0-NL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14654 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-3.0-US.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18666 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17023 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-4.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11902 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13585 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13790 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-2.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20434 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-3.0-DE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19607 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17649 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-4.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11032 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-ND-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12711 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-ND-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12936 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-ND-2.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19469 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-ND-3.0-DE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17672 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-ND-3.0-IGO.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17860 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-ND-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17452 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-ND-4.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13065 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-SA-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15676 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-SA-2.0-DE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18798 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-SA-2.0-FR.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11347 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-SA-2.0-UK.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15177 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-SA-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15386 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-SA-2.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22414 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-SA-3.0-DE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20330 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-SA-3.0-IGO.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21351 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-SA-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19018 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-NC-SA-4.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10488 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-ND-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11696 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-ND-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11921 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-ND-2.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18246 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-ND-3.0-DE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16930 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-ND-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16830 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-ND-4.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12523 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-SA-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10810 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-SA-2.0-UK.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14122 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-SA-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16303 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-SA-2.1-JP.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14331 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-SA-2.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22343 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-SA-3.0-AT.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22421 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-SA-3.0-DE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21305 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-SA-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18375 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-BY-SA-4.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1593 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC-PDDC.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     7048 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CC0-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16514 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CDDL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17390 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CDDL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8592 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CDL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10462 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CDLA-Permissive-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2354 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CDLA-Permissive-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11233 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CDLA-Sharing-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21842 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CECILL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21219 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CECILL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21097 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CECILL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21778 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CECILL-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21393 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CECILL-B.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21863 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CECILL-C.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8114 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CERN-OHL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9168 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CERN-OHL-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8855 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CERN-OHL-P-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13419 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CERN-OHL-S-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14529 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CERN-OHL-W-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1408 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CFITSIO.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2698 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CLISP-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      938 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CMU-Mach.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3923 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CNRI-Jython.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4004 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CNRI-Python-GPL-Compatible.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3381 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CNRI-Python.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1657 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/COIL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    28319 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CPAL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11653 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11649 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CPOL-1.02.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    23381 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CUA-OPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2577 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Caldera.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6389 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ClArtistic.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      919 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Classpath-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      938 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Clips.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15885 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Community-Spec-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6056 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Condor-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      971 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Cornell-Lossless-JPEG.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      480 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Crossword.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      982 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/CrystalStacker.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1078 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Cube.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15238 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/D-FSL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2518 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/DL-DE-BY-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4472 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/DOC.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1512 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/DRL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2280 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/DSDP.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3131 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/DigiRule-FOSS-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      261 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Dotseqn.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2425 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ECL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11111 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ECL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      919 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/EFL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      924 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/EFL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3439 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/EPICS.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11345 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/EPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14020 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/EPL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3199 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/EUDatagrid.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13005 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/EUPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13231 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/EUPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13792 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/EUPL-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3860 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Elastic-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2277 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Entessa.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13958 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ErlPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1367 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Eurosym.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4447 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/FDK-AAC.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1470 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/FLTK-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      225 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/FSFAP.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      198 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/FSFUL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      234 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/FSFULLR.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      544 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/FSFULLRWD.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5979 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/FTL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      245 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Fair.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1344 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Fawkes-Runtime-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      582 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Font-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9771 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Frameworx-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2781 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/FreeBSD-DOC.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17656 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/FreeImage.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      482 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GCC-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3390 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GCC-exception-3.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2983 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GD.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.1-invariants-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.1-invariants-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.1-no-invariants-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.1-no-invariants-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.1-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.1-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.2-invariants-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.2-invariants-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.2-no-invariants-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.2-no-invariants-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.2-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.2-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.3-invariants-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.3-invariants-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.3-no-invariants-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.3-no-invariants-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.3-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GFDL-1.3-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      896 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GL2PS.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      959 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GLWTPL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      379 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GNAT-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12235 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GPL-1.0-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12235 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GPL-1.0-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17337 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GPL-2.0-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17337 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GPL-2.0-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      359 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GPL-3.0-linking-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      531 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GPL-3.0-linking-source-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    34670 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GPL-3.0-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    34670 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GPL-3.0-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2092 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GPL-CC-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      246 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GStreamer-exception-2005.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      462 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/GStreamer-exception-2008.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1352 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Giftware.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12253 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Glide.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      462 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Glulxe.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      707 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Graphics-Gems.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      617 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/HP-1986.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      179 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/HPND-Markus-Kuhn.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      944 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/HPND-export-US.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      891 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/HPND-sell-variant-MIT-disclaimer.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1102 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/HPND-sell-variant.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1173 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/HPND.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1460 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/HTMLTIDY.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      602 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/HaskellReport.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8422 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Hippocratic-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      855 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/IBM-pibs.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1597 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ICU.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2330 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/IEC-Code-Components-EULA.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1640 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/IJG-short.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4244 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/IJG.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9093 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/IPA.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11409 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/IPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      823 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ISC.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12506 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ImageMagick.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2002 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Imlib2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3171 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Info-ZIP.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6132 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Intel-ACPI.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2084 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Intel.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    24344 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Interbase-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3158 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/JPL-image.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2086 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/JPNIC.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1114 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/JSON.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      195 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Jam.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2741 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/JasPer-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      683 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Kazlib.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      299 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/KiCad-libraries-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      296 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Knuth-CTAN.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6972 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LAL-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8264 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LAL-1.3.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    24842 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LGPL-2.0-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    24842 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LGPL-2.0-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    25967 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LGPL-2.1-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    25967 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LGPL-2.1-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1033 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LGPL-3.0-linking-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    42098 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LGPL-3.0-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    42098 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LGPL-3.0-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14556 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LGPLLR.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      919 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LLVM-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2054 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LOOP.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11948 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11824 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LPL-1.02.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8929 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LPPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14026 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LPPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14115 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LPPL-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18012 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LPPL-1.3a.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18575 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LPPL-1.3c.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      240 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LZMA-SDK-9.11-to-9.20.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      582 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LZMA-SDK-9.22.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      522 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LZMA-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      704 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Latex2e.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      734 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Leptonica.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6590 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LiLiQ-P-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8694 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LiLiQ-R-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8338 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/LiLiQ-Rplus-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4218 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Libpng.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      254 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Libtool-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      939 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Linux-OpenIB.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1019 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Linux-man-pages-copyleft.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      638 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Linux-syscall-note.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      915 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MIT-0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1150 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MIT-CMU.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      917 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MIT-Modern-Variant.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1295 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MIT-Wu.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1270 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MIT-advertising.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1668 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MIT-enna.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1105 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MIT-feh.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1121 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MIT-open-group.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1078 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MIT.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1531 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MITNFA.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18272 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    23669 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16727 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MPL-2.0-no-copyleft-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16727 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MPL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2870 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MS-LPL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2663 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MS-PL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3058 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MS-RL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3239 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MTLL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1974 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MakeIndex.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      407 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Martin-Birgmeier.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2193 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Minpack.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      887 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MirOS.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20187 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Motosoto.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8908 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MulanPSL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9233 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/MulanPSL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2040 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Multics.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1459 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Mup.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3792 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NAIST-2003.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13778 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NASA-1.3.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5425 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NBPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5540 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NCGL-UK-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1700 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NCSA.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4703 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NGPL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2977 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NICTA-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1644 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NIST-PD-fallback.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      890 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NIST-PD.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8712 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NLOD-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8810 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NLOD-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      268 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NLPL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    24490 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NOSL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21051 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    28018 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11800 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NPOSL-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3298 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NRL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      528 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NTP-0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      714 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NTP.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1953 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Naumen.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14237 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Net-SNMP.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1881 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/NetCDF.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      510 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Newsletr.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1177 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Nokia-Qt-exception-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21003 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Nokia.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1126 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Noweb.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3434 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/O-UDA-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14012 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OCCT-PL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      663 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OCCT-exception-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11124 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OCLC-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      881 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OCaml-LGPL-linking-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19808 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ODC-By-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    25289 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ODbL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1007 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OFFIS.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3858 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OFL-1.0-RFN.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3858 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OFL-1.0-no-RFN.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3858 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OFL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4016 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OFL-1.1-RFN.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4016 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OFL-1.1-no-RFN.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4016 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OFL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2179 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OGC-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11606 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OGDL-Taiwan-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3679 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OGL-Canada-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6080 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OGL-UK-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5980 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OGL-UK-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6220 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OGL-UK-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5277 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OGTSL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5393 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5396 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5795 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-1.3.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5873 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-1.4.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1977 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-2.0.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1981 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2220 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2241 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-2.2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2267 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-2.2.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2228 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-2.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2265 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-2.3.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2124 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-2.4.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2171 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-2.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2109 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-2.6.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2197 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-2.7.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2195 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OLDAP-2.8.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1689 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OML.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20309 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6148 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OPUBL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19967 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OSET-PL-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8921 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OSL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9663 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OSL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9880 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OSL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9872 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OSL-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10319 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OSL-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1447 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OpenJDK-assembly-exception-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3962 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OpenPBS-2.3.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5309 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/OpenSSL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15485 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/PDDL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2846 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/PHP-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2855 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/PHP-3.01.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      439 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/PS-or-PDF-font-exception-20170817.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2427 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/PSF-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1704 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Parity-6.0.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3524 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Parity-7.0.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1849 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Plexus.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4563 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/PolyForm-Noncommercial-1.0.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4389 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/PolyForm-Small-Business-1.0.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1195 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/PostgreSQL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9916 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Python-2.0.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9411 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Python-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      334 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/QPL-1.0-INRIA-2004-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4641 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/QPL-1.0-INRIA-2004.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4364 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/QPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1304 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Qhull.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      964 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Qt-GPL-exception-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1195 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Qt-LGPL-exception-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1199 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Qwt-exception-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21641 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/RHeCos-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    33931 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/RPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    32009 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/RPL-1.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    30271 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/RPSL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      869 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/RSA-MD.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21050 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/RSCPL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1107 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Rdisc.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2137 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Ruby.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2315 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SAX-PD.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6638 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SCEA.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13553 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SGI-B-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14556 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SGI-B-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1503 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SGI-B-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11386 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SHL-0.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11399 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SHL-0.51.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2776 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SHL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4485 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SHL-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12474 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SISSL-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14496 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SISSL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1122 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SMLNJ.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3177 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SMPPL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21717 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SNIA.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    23398 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3399 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SSH-OpenSSH.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      326 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SSH-short.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    30609 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SSPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      382 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SWI-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2129 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SWL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2133 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Saxpath.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      290 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SchemeReport.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4020 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Sendmail-8.23.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3948 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Sendmail.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2529 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SimPL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4995 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Sleepycat.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      628 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Spencer-86.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      935 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Spencer-94.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1376 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Spencer-99.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22087 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SugarCRM-1.1.3.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      246 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/SunPro.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      355 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Swift-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      515 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Symlinks.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13932 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/TAPR-OHL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2251 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/TCL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      648 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/TCP-wrappers.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2537 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/TMate.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3998 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/TORQUE-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2074 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/TOSL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      233 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/TPDL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    23787 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/TPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      406 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/TTWL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      678 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/TU-Berlin-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1369 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/TU-Berlin-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1948 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/UCAR.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10566 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/UCL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1837 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/UPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2873 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Unicode-DFS-2015.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2858 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Unicode-DFS-2016.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6261 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Unicode-TOU.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3154 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Universal-FOSS-exception-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1211 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Unlicense.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3058 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/VOSTROM.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2065 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/VSL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4525 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Vim.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3116 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/W3C-19980720.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1807 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/W3C-20150513.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2701 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/W3C.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      432 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/WTFPL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20972 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Watcom-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      529 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Wsuipa.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1267 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/WxWindows-exception-3.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1314 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/X11-distribute-modifications-variant.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1338 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/X11.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2398 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/XFree86-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      535 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/XSkat.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      963 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Xerox.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1186 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Xnet.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9010 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/YPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8988 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/YPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2924 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ZPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2275 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ZPL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2100 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/ZPL-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      259 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Zed.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2490 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Zend-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8994 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Zimbra-1.3.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8947 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Zimbra-1.4.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      838 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/Zlib.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      244 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/blessing.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1739 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/bzip2-1.0.6.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      435 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/checkmk.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10571 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/copyleft-next-0.3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10634 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/copyleft-next-0.3.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1043 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/curl.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       88 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/diffmark.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      210 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/dvipdfm.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      575 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/eCos-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4235 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/eGenix.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8198 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/etalab-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1687 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/freertos-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20362 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/gSOAP-1.3b.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      341 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/gnu-javamail-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1407 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/gnuplot.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      605 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/i2p-gpl-java-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3473 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/iMatix.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1550 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/libpng-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1034 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/libselinux-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1139 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/libtiff.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      915 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/libutil-David-Nugent.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      529 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/mif-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      583 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/mpi-permissive.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1424 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/mpich2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      226 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/mplus.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      629 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/openvpn-openssl-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      480 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/psfrag.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1961 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/psutils.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      209 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/snprintf.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      629 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/u-boot-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      568 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/w3m.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      591 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/x11vnc-openssl-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2030 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/xinetd.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      734 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/xlock.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2482 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/xpp.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1133 2023-04-05 07:52:31.000000 oslili-0.6/oslili/spdx/zlib-acknowledgement.txt
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:06:40.874233 oslili-0.6/oslili.egg-info/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2983 2023-04-20 13:06:40.000000 oslili-0.6/oslili.egg-info/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16059 2023-04-20 13:06:40.000000 oslili-0.6/oslili.egg-info/SOURCES.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2023-04-20 13:06:40.000000 oslili-0.6/oslili.egg-info/dependency_links.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       13 2023-04-20 13:06:40.000000 oslili-0.6/oslili.egg-info/requires.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        7 2023-04-20 13:06:40.000000 oslili-0.6/oslili.egg-info/top_level.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       79 2023-04-20 13:06:41.670735 oslili-0.6/setup.cfg
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1064 2023-04-20 13:06:10.000000 oslili-0.6/setup.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:08:48.417288 oslili-0.7/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2023-04-05 07:52:31.000000 oslili-0.7/LICENSE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2023-04-09 07:33:34.000000 oslili-0.7/NOTICE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2972 2023-04-20 13:08:48.417453 oslili-0.7/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2451 2023-04-20 04:48:38.000000 oslili-0.7/README.md
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:08:47.892054 oslili-0.7/oslili/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       77 2023-04-05 07:52:31.000000 oslili-0.7/oslili/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4524 2023-04-13 19:34:09.000000 oslili-0.7/oslili/identifier.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:08:48.416774 oslili-0.7/oslili/spdx/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      643 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/0BSD.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1931 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/389-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2529 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/AAL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      488 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ADSL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4676 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/AFL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4950 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/AFL-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8987 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/AFL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8948 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/AFL-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10334 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/AFL-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15839 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/AGPL-1.0-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15839 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/AGPL-1.0-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    34020 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/AGPL-3.0-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    34020 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/AGPL-3.0-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5642 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/AMDPLPA.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2358 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/AML.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2192 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/AMPAS.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1261 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ANTLR-PD-fallback.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      987 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ANTLR-PD.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      617 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/APAFML.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    46103 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/APL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19644 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/APSL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20151 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/APSL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19800 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/APSL-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20285 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/APSL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      731 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Abstyles.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      236 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/AdaCore-doc.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1776 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Adobe-2006.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1608 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Adobe-Glyph.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      893 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Afmparse.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11604 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Aladdin.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2507 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Apache-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2514 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Apache-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10280 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Apache-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      224 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/App-s2p.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6901 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Arphic-1999.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6060 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Artistic-1.0-Perl.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5184 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Artistic-1.0-cl8.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4854 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Artistic-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8764 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Artistic-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1573 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Autoconf-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1818 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Autoconf-exception-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      266 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Autoconf-exception-generic.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      768 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Autoconf-exception-macro.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1086 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-1-Clause.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2569 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-2-Clause-Patent.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1519 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-2-Clause-Views.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1267 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-2-Clause.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1646 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-3-Clause-Attribution.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1676 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-3-Clause-Clear.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2388 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-3-Clause-LBNL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1624 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-3-Clause-Modification.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1647 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-3-Clause-No-Military-License.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1709 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-3-Clause-No-Nuclear-License-2014.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1693 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-3-Clause-No-Nuclear-License.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1699 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-3-Clause-No-Nuclear-Warranty.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1820 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-3-Clause-Open-MPI.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1460 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-3-Clause.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1048 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-4-Clause-Shortened.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1771 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-4-Clause-UC.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1618 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-4-Clause.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      476 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-4.3RENO.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      781 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-4.3TAHOE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1626 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-Advertising-Acknowledgement.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1679 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-Attribution-HPND-disclaimer.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6244 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-Protection.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1301 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSD-Source-Code.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1338 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BSL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3424 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BUSL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      479 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Baekmuk.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1377 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Bahyph.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      603 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Barr.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      266 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Beerware.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      673 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Bison-exception-2.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    24219 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BitTorrent-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    27782 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BitTorrent-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      572 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Bitstream-Charter.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2318 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Bitstream-Vera.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1552 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/BlueOak-1.0.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      523 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Bootloader-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      647 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Borceux.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1096 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Brian-Gladman-3-Clause.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3451 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/C-UDA-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16125 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CAL-1.0-Combined-Work-Exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16125 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CAL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19046 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CATOSL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11405 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12572 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17126 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-2.5-AU.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12781 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-2.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19189 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-3.0-AT.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19218 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-3.0-DE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17572 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-3.0-IGO.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18371 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-3.0-NL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14654 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-3.0-US.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18666 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17023 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-4.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11902 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13585 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13790 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-2.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20434 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-3.0-DE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19607 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17649 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-4.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11032 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-ND-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12711 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-ND-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12936 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-ND-2.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19469 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-ND-3.0-DE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17672 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-ND-3.0-IGO.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17860 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-ND-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17452 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-ND-4.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13065 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-SA-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15676 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-SA-2.0-DE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18798 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-SA-2.0-FR.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11347 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-SA-2.0-UK.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15177 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-SA-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15386 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-SA-2.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22414 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-SA-3.0-DE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20330 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-SA-3.0-IGO.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21351 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-SA-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19018 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-NC-SA-4.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10488 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-ND-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11696 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-ND-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11921 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-ND-2.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18246 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-ND-3.0-DE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16930 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-ND-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16830 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-ND-4.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12523 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-SA-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10810 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-SA-2.0-UK.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14122 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-SA-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16303 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-SA-2.1-JP.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14331 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-SA-2.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22343 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-SA-3.0-AT.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22421 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-SA-3.0-DE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21305 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-SA-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18375 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-BY-SA-4.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1593 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC-PDDC.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     7048 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CC0-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16514 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CDDL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17390 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CDDL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8592 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CDL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10462 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CDLA-Permissive-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2354 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CDLA-Permissive-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11233 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CDLA-Sharing-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21842 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CECILL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21219 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CECILL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21097 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CECILL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21778 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CECILL-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21393 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CECILL-B.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21863 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CECILL-C.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8114 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CERN-OHL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9168 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CERN-OHL-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8855 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CERN-OHL-P-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13419 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CERN-OHL-S-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14529 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CERN-OHL-W-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1408 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CFITSIO.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2698 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CLISP-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      938 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CMU-Mach.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3923 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CNRI-Jython.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4004 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CNRI-Python-GPL-Compatible.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3381 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CNRI-Python.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1657 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/COIL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    28319 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CPAL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11653 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11649 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CPOL-1.02.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    23381 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CUA-OPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2577 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Caldera.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6389 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ClArtistic.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      919 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Classpath-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      938 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Clips.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15885 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Community-Spec-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6056 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Condor-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      971 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Cornell-Lossless-JPEG.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      480 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Crossword.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      982 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/CrystalStacker.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1078 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Cube.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15238 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/D-FSL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2518 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/DL-DE-BY-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4472 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/DOC.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1512 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/DRL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2280 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/DSDP.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3131 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/DigiRule-FOSS-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      261 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Dotseqn.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2425 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ECL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11111 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ECL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      919 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/EFL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      924 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/EFL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3439 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/EPICS.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11345 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/EPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14020 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/EPL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3199 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/EUDatagrid.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13005 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/EUPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13231 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/EUPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13792 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/EUPL-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3860 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Elastic-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2277 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Entessa.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13958 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ErlPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1367 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Eurosym.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4447 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/FDK-AAC.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1470 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/FLTK-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      225 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/FSFAP.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      198 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/FSFUL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      234 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/FSFULLR.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      544 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/FSFULLRWD.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5979 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/FTL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      245 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Fair.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1344 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Fawkes-Runtime-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      582 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Font-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9771 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Frameworx-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2781 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/FreeBSD-DOC.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17656 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/FreeImage.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      482 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GCC-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3390 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GCC-exception-3.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2983 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GD.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.1-invariants-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.1-invariants-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.1-no-invariants-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.1-no-invariants-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.1-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.1-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.2-invariants-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.2-invariants-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.2-no-invariants-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.2-no-invariants-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.2-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.2-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.3-invariants-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.3-invariants-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.3-no-invariants-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.3-no-invariants-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.3-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GFDL-1.3-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      896 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GL2PS.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      959 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GLWTPL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      379 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GNAT-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12235 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GPL-1.0-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12235 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GPL-1.0-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17337 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GPL-2.0-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17337 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GPL-2.0-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      359 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GPL-3.0-linking-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      531 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GPL-3.0-linking-source-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    34670 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GPL-3.0-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    34670 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GPL-3.0-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2092 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GPL-CC-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      246 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GStreamer-exception-2005.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      462 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/GStreamer-exception-2008.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1352 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Giftware.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12253 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Glide.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      462 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Glulxe.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      707 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Graphics-Gems.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      617 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/HP-1986.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      179 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/HPND-Markus-Kuhn.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      944 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/HPND-export-US.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      891 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/HPND-sell-variant-MIT-disclaimer.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1102 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/HPND-sell-variant.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1173 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/HPND.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1460 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/HTMLTIDY.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      602 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/HaskellReport.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8422 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Hippocratic-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      855 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/IBM-pibs.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1597 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ICU.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2330 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/IEC-Code-Components-EULA.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1640 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/IJG-short.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4244 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/IJG.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9093 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/IPA.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11409 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/IPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      823 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ISC.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12506 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ImageMagick.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2002 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Imlib2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3171 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Info-ZIP.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6132 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Intel-ACPI.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2084 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Intel.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    24344 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Interbase-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3158 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/JPL-image.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2086 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/JPNIC.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1114 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/JSON.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      195 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Jam.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2741 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/JasPer-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      683 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Kazlib.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      299 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/KiCad-libraries-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      296 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Knuth-CTAN.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6972 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LAL-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8264 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LAL-1.3.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    24842 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LGPL-2.0-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    24842 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LGPL-2.0-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    25967 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LGPL-2.1-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    25967 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LGPL-2.1-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1033 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LGPL-3.0-linking-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    42098 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LGPL-3.0-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    42098 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LGPL-3.0-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14556 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LGPLLR.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      919 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LLVM-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2054 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LOOP.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11948 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11824 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LPL-1.02.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8929 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LPPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14026 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LPPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14115 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LPPL-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18012 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LPPL-1.3a.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18575 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LPPL-1.3c.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      240 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LZMA-SDK-9.11-to-9.20.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      582 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LZMA-SDK-9.22.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      522 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LZMA-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      704 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Latex2e.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      734 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Leptonica.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6590 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LiLiQ-P-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8694 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LiLiQ-R-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8338 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/LiLiQ-Rplus-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4218 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Libpng.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      254 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Libtool-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      939 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Linux-OpenIB.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1019 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Linux-man-pages-copyleft.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      638 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Linux-syscall-note.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      915 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MIT-0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1150 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MIT-CMU.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      917 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MIT-Modern-Variant.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1295 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MIT-Wu.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1270 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MIT-advertising.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1668 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MIT-enna.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1105 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MIT-feh.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1121 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MIT-open-group.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1078 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MIT.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1531 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MITNFA.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18272 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    23669 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16727 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MPL-2.0-no-copyleft-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16727 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MPL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2870 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MS-LPL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2663 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MS-PL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3058 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MS-RL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3239 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MTLL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1974 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MakeIndex.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      407 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Martin-Birgmeier.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2193 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Minpack.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      887 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MirOS.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20187 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Motosoto.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8908 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MulanPSL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9233 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/MulanPSL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2040 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Multics.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1459 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Mup.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3792 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NAIST-2003.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13778 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NASA-1.3.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5425 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NBPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5540 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NCGL-UK-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1700 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NCSA.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4703 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NGPL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2977 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NICTA-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1644 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NIST-PD-fallback.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      890 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NIST-PD.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8712 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NLOD-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8810 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NLOD-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      268 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NLPL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    24490 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NOSL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21051 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    28018 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11800 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NPOSL-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3298 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NRL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      528 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NTP-0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      714 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NTP.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1953 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Naumen.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14237 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Net-SNMP.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1881 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/NetCDF.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      510 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Newsletr.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1177 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Nokia-Qt-exception-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21003 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Nokia.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1126 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Noweb.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3434 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/O-UDA-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14012 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OCCT-PL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      663 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OCCT-exception-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11124 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OCLC-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      881 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OCaml-LGPL-linking-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19808 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ODC-By-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    25289 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ODbL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1007 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OFFIS.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3858 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OFL-1.0-RFN.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3858 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OFL-1.0-no-RFN.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3858 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OFL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4016 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OFL-1.1-RFN.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4016 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OFL-1.1-no-RFN.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4016 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OFL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2179 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OGC-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11606 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OGDL-Taiwan-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3679 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OGL-Canada-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6080 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OGL-UK-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5980 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OGL-UK-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6220 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OGL-UK-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5277 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OGTSL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5393 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5396 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5795 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-1.3.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5873 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-1.4.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1977 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-2.0.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1981 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2220 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2241 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-2.2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2267 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-2.2.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2228 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-2.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2265 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-2.3.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2124 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-2.4.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2171 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-2.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2109 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-2.6.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2197 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-2.7.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2195 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OLDAP-2.8.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1689 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OML.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20309 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6148 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OPUBL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19967 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OSET-PL-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8921 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OSL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9663 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OSL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9880 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OSL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9872 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OSL-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10319 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OSL-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1447 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OpenJDK-assembly-exception-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3962 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OpenPBS-2.3.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5309 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/OpenSSL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15485 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/PDDL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2846 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/PHP-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2855 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/PHP-3.01.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      439 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/PS-or-PDF-font-exception-20170817.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2427 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/PSF-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1704 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Parity-6.0.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3524 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Parity-7.0.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1849 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Plexus.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4563 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/PolyForm-Noncommercial-1.0.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4389 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/PolyForm-Small-Business-1.0.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1195 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/PostgreSQL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9916 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Python-2.0.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9411 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Python-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      334 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/QPL-1.0-INRIA-2004-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4641 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/QPL-1.0-INRIA-2004.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4364 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/QPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1304 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Qhull.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      964 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Qt-GPL-exception-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1195 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Qt-LGPL-exception-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1199 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Qwt-exception-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21641 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/RHeCos-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    33931 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/RPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    32009 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/RPL-1.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    30271 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/RPSL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      869 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/RSA-MD.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21050 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/RSCPL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1107 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Rdisc.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2137 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Ruby.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2315 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SAX-PD.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6638 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SCEA.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13553 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SGI-B-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14556 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SGI-B-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1503 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SGI-B-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11386 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SHL-0.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11399 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SHL-0.51.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2776 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SHL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4485 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SHL-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12474 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SISSL-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14496 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SISSL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1122 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SMLNJ.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3177 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SMPPL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21717 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SNIA.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    23398 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3399 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SSH-OpenSSH.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      326 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SSH-short.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    30609 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SSPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      382 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SWI-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2129 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SWL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2133 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Saxpath.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      290 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SchemeReport.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4020 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Sendmail-8.23.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3948 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Sendmail.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2529 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SimPL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4995 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Sleepycat.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      628 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Spencer-86.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      935 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Spencer-94.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1376 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Spencer-99.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22087 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SugarCRM-1.1.3.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      246 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/SunPro.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      355 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Swift-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      515 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Symlinks.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13932 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/TAPR-OHL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2251 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/TCL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      648 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/TCP-wrappers.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2537 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/TMate.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3998 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/TORQUE-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2074 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/TOSL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      233 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/TPDL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    23787 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/TPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      406 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/TTWL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      678 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/TU-Berlin-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1369 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/TU-Berlin-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1948 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/UCAR.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10566 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/UCL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1837 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/UPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2873 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Unicode-DFS-2015.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2858 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Unicode-DFS-2016.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6261 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Unicode-TOU.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3154 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Universal-FOSS-exception-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1211 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Unlicense.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3058 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/VOSTROM.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2065 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/VSL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4525 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Vim.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3116 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/W3C-19980720.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1807 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/W3C-20150513.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2701 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/W3C.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      432 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/WTFPL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20972 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Watcom-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      529 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Wsuipa.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1267 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/WxWindows-exception-3.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1314 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/X11-distribute-modifications-variant.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1338 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/X11.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2398 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/XFree86-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      535 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/XSkat.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      963 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Xerox.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1186 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Xnet.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9010 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/YPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8988 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/YPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2924 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ZPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2275 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ZPL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2100 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/ZPL-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      259 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Zed.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2490 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Zend-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8994 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Zimbra-1.3.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8947 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Zimbra-1.4.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      838 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/Zlib.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      244 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/blessing.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1739 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/bzip2-1.0.6.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      435 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/checkmk.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10571 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/copyleft-next-0.3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10634 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/copyleft-next-0.3.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1043 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/curl.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       88 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/diffmark.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      210 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/dvipdfm.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      575 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/eCos-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4235 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/eGenix.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8198 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/etalab-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1687 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/freertos-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20362 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/gSOAP-1.3b.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      341 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/gnu-javamail-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1407 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/gnuplot.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      605 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/i2p-gpl-java-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3473 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/iMatix.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1550 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/libpng-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1034 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/libselinux-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1139 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/libtiff.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      915 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/libutil-David-Nugent.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      529 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/mif-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      583 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/mpi-permissive.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1424 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/mpich2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      226 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/mplus.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      629 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/openvpn-openssl-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      480 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/psfrag.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1961 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/psutils.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      209 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/snprintf.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      629 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/u-boot-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      568 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/w3m.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      591 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/x11vnc-openssl-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2030 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/xinetd.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      734 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/xlock.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2482 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/xpp.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1133 2023-04-05 07:52:31.000000 oslili-0.7/oslili/spdx/zlib-acknowledgement.txt
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:08:47.896067 oslili-0.7/oslili.egg-info/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2972 2023-04-20 13:08:47.000000 oslili-0.7/oslili.egg-info/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16059 2023-04-20 13:08:47.000000 oslili-0.7/oslili.egg-info/SOURCES.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2023-04-20 13:08:47.000000 oslili-0.7/oslili.egg-info/dependency_links.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       13 2023-04-20 13:08:47.000000 oslili-0.7/oslili.egg-info/requires.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        7 2023-04-20 13:08:47.000000 oslili-0.7/oslili.egg-info/top_level.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       79 2023-04-20 13:08:48.418074 oslili-0.7/setup.cfg
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1053 2023-04-20 13:08:18.000000 oslili-0.7/setup.py
```

### Comparing `oslili-0.6/LICENSE` & `oslili-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oslili-0.6/PKG-INFO` & `oslili-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: oslili
-Version: 0.6
+Version: 0.7
 Summary: Open Source License Identification Library
 Home-page: https://github.com/oscarvalenzuelab/oslili
 Author: Oscar Valenzuela B.
-Author-email: oscar.valenzuela.b@gmail.com
+Author-email: alkamod@gmail.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oslili-0.6/README.md` & `oslili-0.7/README.md`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/identifier.py` & `oslili-0.7/oslili/identifier.py`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/0BSD.txt` & `oslili-0.7/oslili/spdx/0BSD.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/389-exception.txt` & `oslili-0.7/oslili/spdx/389-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/AAL.txt` & `oslili-0.7/oslili/spdx/AAL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/AFL-1.1.txt` & `oslili-0.7/oslili/spdx/AFL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/AFL-1.2.txt` & `oslili-0.7/oslili/spdx/AFL-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/AFL-2.0.txt` & `oslili-0.7/oslili/spdx/AFL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/AFL-2.1.txt` & `oslili-0.7/oslili/spdx/AFL-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/AFL-3.0.txt` & `oslili-0.7/oslili/spdx/AFL-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/AGPL-1.0-only.txt` & `oslili-0.7/oslili/spdx/AGPL-1.0-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/AGPL-1.0-or-later.txt` & `oslili-0.7/oslili/spdx/AGPL-1.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/AGPL-3.0-only.txt` & `oslili-0.7/oslili/spdx/AGPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/AGPL-3.0-or-later.txt` & `oslili-0.7/oslili/spdx/AGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/AMDPLPA.txt` & `oslili-0.7/oslili/spdx/AMDPLPA.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/AML.txt` & `oslili-0.7/oslili/spdx/AML.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/AMPAS.txt` & `oslili-0.7/oslili/spdx/AMPAS.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/ANTLR-PD-fallback.txt` & `oslili-0.7/oslili/spdx/ANTLR-PD-fallback.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/ANTLR-PD.txt` & `oslili-0.7/oslili/spdx/ANTLR-PD.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/APAFML.txt` & `oslili-0.7/oslili/spdx/APAFML.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/APL-1.0.txt` & `oslili-0.7/oslili/spdx/APL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/APSL-1.0.txt` & `oslili-0.7/oslili/spdx/APSL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/APSL-1.1.txt` & `oslili-0.7/oslili/spdx/APSL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/APSL-1.2.txt` & `oslili-0.7/oslili/spdx/APSL-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/APSL-2.0.txt` & `oslili-0.7/oslili/spdx/APSL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Abstyles.txt` & `oslili-0.7/oslili/spdx/Abstyles.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Adobe-2006.txt` & `oslili-0.7/oslili/spdx/Adobe-2006.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Adobe-Glyph.txt` & `oslili-0.7/oslili/spdx/Adobe-Glyph.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Afmparse.txt` & `oslili-0.7/oslili/spdx/Afmparse.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Aladdin.txt` & `oslili-0.7/oslili/spdx/Aladdin.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Apache-1.0.txt` & `oslili-0.7/oslili/spdx/Apache-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Apache-1.1.txt` & `oslili-0.7/oslili/spdx/Apache-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Apache-2.0.txt` & `oslili-0.7/oslili/spdx/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Arphic-1999.txt` & `oslili-0.7/oslili/spdx/Arphic-1999.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Artistic-1.0-Perl.txt` & `oslili-0.7/oslili/spdx/Artistic-1.0-Perl.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Artistic-1.0-cl8.txt` & `oslili-0.7/oslili/spdx/Artistic-1.0-cl8.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Artistic-1.0.txt` & `oslili-0.7/oslili/spdx/Artistic-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Artistic-2.0.txt` & `oslili-0.7/oslili/spdx/Artistic-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Autoconf-exception-2.0.txt` & `oslili-0.7/oslili/spdx/Autoconf-exception-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Autoconf-exception-3.0.txt` & `oslili-0.7/oslili/spdx/Autoconf-exception-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Autoconf-exception-macro.txt` & `oslili-0.7/oslili/spdx/Autoconf-exception-macro.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-1-Clause.txt` & `oslili-0.7/oslili/spdx/BSD-1-Clause.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-2-Clause-Patent.txt` & `oslili-0.7/oslili/spdx/BSD-2-Clause-Patent.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-2-Clause-Views.txt` & `oslili-0.7/oslili/spdx/BSD-2-Clause-Views.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-2-Clause.txt` & `oslili-0.7/oslili/spdx/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-3-Clause-Attribution.txt` & `oslili-0.7/oslili/spdx/BSD-3-Clause-Attribution.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-3-Clause-Clear.txt` & `oslili-0.7/oslili/spdx/BSD-3-Clause-Clear.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-3-Clause-LBNL.txt` & `oslili-0.7/oslili/spdx/BSD-3-Clause-LBNL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-3-Clause-Modification.txt` & `oslili-0.7/oslili/spdx/BSD-3-Clause-Modification.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-3-Clause-No-Military-License.txt` & `oslili-0.7/oslili/spdx/BSD-3-Clause-No-Military-License.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-3-Clause-No-Nuclear-License-2014.txt` & `oslili-0.7/oslili/spdx/BSD-3-Clause-No-Nuclear-License-2014.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-3-Clause-No-Nuclear-License.txt` & `oslili-0.7/oslili/spdx/BSD-3-Clause-No-Nuclear-License.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-3-Clause-No-Nuclear-Warranty.txt` & `oslili-0.7/oslili/spdx/BSD-3-Clause-No-Nuclear-Warranty.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-3-Clause-Open-MPI.txt` & `oslili-0.7/oslili/spdx/BSD-3-Clause-Open-MPI.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-3-Clause.txt` & `oslili-0.7/oslili/spdx/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-4-Clause-Shortened.txt` & `oslili-0.7/oslili/spdx/BSD-4-Clause-Shortened.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-4-Clause-UC.txt` & `oslili-0.7/oslili/spdx/BSD-4-Clause-UC.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-4-Clause.txt` & `oslili-0.7/oslili/spdx/BSD-4-Clause.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-4.3TAHOE.txt` & `oslili-0.7/oslili/spdx/BSD-4.3TAHOE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-Advertising-Acknowledgement.txt` & `oslili-0.7/oslili/spdx/BSD-Advertising-Acknowledgement.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-Attribution-HPND-disclaimer.txt` & `oslili-0.7/oslili/spdx/BSD-Attribution-HPND-disclaimer.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-Protection.txt` & `oslili-0.7/oslili/spdx/BSD-Protection.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSD-Source-Code.txt` & `oslili-0.7/oslili/spdx/BSD-Source-Code.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BSL-1.0.txt` & `oslili-0.7/oslili/spdx/BSL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BUSL-1.1.txt` & `oslili-0.7/oslili/spdx/BUSL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Bahyph.txt` & `oslili-0.7/oslili/spdx/Bahyph.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Barr.txt` & `oslili-0.7/oslili/spdx/Barr.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Bison-exception-2.2.txt` & `oslili-0.7/oslili/spdx/Bison-exception-2.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BitTorrent-1.0.txt` & `oslili-0.7/oslili/spdx/BitTorrent-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BitTorrent-1.1.txt` & `oslili-0.7/oslili/spdx/BitTorrent-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Bitstream-Charter.txt` & `oslili-0.7/oslili/spdx/Bitstream-Charter.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Bitstream-Vera.txt` & `oslili-0.7/oslili/spdx/Bitstream-Vera.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/BlueOak-1.0.0.txt` & `oslili-0.7/oslili/spdx/BlueOak-1.0.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Bootloader-exception.txt` & `oslili-0.7/oslili/spdx/Bootloader-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Borceux.txt` & `oslili-0.7/oslili/spdx/Borceux.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Brian-Gladman-3-Clause.txt` & `oslili-0.7/oslili/spdx/Brian-Gladman-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/C-UDA-1.0.txt` & `oslili-0.7/oslili/spdx/C-UDA-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CAL-1.0-Combined-Work-Exception.txt` & `oslili-0.7/oslili/spdx/CAL-1.0-Combined-Work-Exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CAL-1.0.txt` & `oslili-0.7/oslili/spdx/CAL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CATOSL-1.1.txt` & `oslili-0.7/oslili/spdx/CATOSL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-1.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-2.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-2.5-AU.txt` & `oslili-0.7/oslili/spdx/CC-BY-2.5-AU.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-2.5.txt` & `oslili-0.7/oslili/spdx/CC-BY-2.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-3.0-AT.txt` & `oslili-0.7/oslili/spdx/CC-BY-3.0-AT.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-3.0-DE.txt` & `oslili-0.7/oslili/spdx/CC-BY-3.0-DE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-3.0-IGO.txt` & `oslili-0.7/oslili/spdx/CC-BY-3.0-IGO.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-3.0-NL.txt` & `oslili-0.7/oslili/spdx/CC-BY-3.0-NL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-3.0-US.txt` & `oslili-0.7/oslili/spdx/CC-BY-3.0-US.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-3.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-4.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-1.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-2.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-2.5.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-2.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-3.0-DE.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-3.0-DE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-3.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-4.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-4.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-ND-1.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-ND-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-ND-2.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-ND-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-ND-2.5.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-ND-2.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-ND-3.0-DE.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-ND-3.0-DE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-ND-3.0-IGO.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-ND-3.0-IGO.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-ND-3.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-ND-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-ND-4.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-ND-4.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-SA-1.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-SA-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-SA-2.0-DE.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-SA-2.0-DE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-SA-2.0-FR.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-SA-2.0-FR.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-SA-2.0-UK.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-SA-2.0-UK.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-SA-2.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-SA-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-SA-2.5.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-SA-2.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-SA-3.0-DE.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-SA-3.0-DE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-SA-3.0-IGO.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-SA-3.0-IGO.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-SA-3.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-SA-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-NC-SA-4.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-NC-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-ND-1.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-ND-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-ND-2.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-ND-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-ND-2.5.txt` & `oslili-0.7/oslili/spdx/CC-BY-ND-2.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-ND-3.0-DE.txt` & `oslili-0.7/oslili/spdx/CC-BY-ND-3.0-DE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-ND-3.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-ND-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-ND-4.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-ND-4.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-SA-1.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-SA-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-SA-2.0-UK.txt` & `oslili-0.7/oslili/spdx/CC-BY-SA-2.0-UK.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-SA-2.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-SA-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-SA-2.1-JP.txt` & `oslili-0.7/oslili/spdx/CC-BY-SA-2.1-JP.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-SA-2.5.txt` & `oslili-0.7/oslili/spdx/CC-BY-SA-2.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-SA-3.0-AT.txt` & `oslili-0.7/oslili/spdx/CC-BY-SA-3.0-AT.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-SA-3.0-DE.txt` & `oslili-0.7/oslili/spdx/CC-BY-SA-3.0-DE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-SA-3.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-SA-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-BY-SA-4.0.txt` & `oslili-0.7/oslili/spdx/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC-PDDC.txt` & `oslili-0.7/oslili/spdx/CC-PDDC.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CC0-1.0.txt` & `oslili-0.7/oslili/spdx/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CDDL-1.0.txt` & `oslili-0.7/oslili/spdx/CDDL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CDDL-1.1.txt` & `oslili-0.7/oslili/spdx/CDDL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CDL-1.0.txt` & `oslili-0.7/oslili/spdx/CDL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CDLA-Permissive-1.0.txt` & `oslili-0.7/oslili/spdx/CDLA-Permissive-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CDLA-Permissive-2.0.txt` & `oslili-0.7/oslili/spdx/CDLA-Permissive-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CDLA-Sharing-1.0.txt` & `oslili-0.7/oslili/spdx/CDLA-Sharing-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CECILL-1.0.txt` & `oslili-0.7/oslili/spdx/CECILL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CECILL-1.1.txt` & `oslili-0.7/oslili/spdx/CECILL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CECILL-2.0.txt` & `oslili-0.7/oslili/spdx/CECILL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CECILL-2.1.txt` & `oslili-0.7/oslili/spdx/CECILL-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CECILL-B.txt` & `oslili-0.7/oslili/spdx/CECILL-B.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CECILL-C.txt` & `oslili-0.7/oslili/spdx/CECILL-C.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CERN-OHL-1.1.txt` & `oslili-0.7/oslili/spdx/CERN-OHL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CERN-OHL-1.2.txt` & `oslili-0.7/oslili/spdx/CERN-OHL-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CERN-OHL-P-2.0.txt` & `oslili-0.7/oslili/spdx/CERN-OHL-P-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CERN-OHL-S-2.0.txt` & `oslili-0.7/oslili/spdx/CERN-OHL-S-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CERN-OHL-W-2.0.txt` & `oslili-0.7/oslili/spdx/CERN-OHL-W-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CFITSIO.txt` & `oslili-0.7/oslili/spdx/CFITSIO.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CLISP-exception-2.0.txt` & `oslili-0.7/oslili/spdx/CLISP-exception-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CMU-Mach.txt` & `oslili-0.7/oslili/spdx/CMU-Mach.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CNRI-Jython.txt` & `oslili-0.7/oslili/spdx/CNRI-Jython.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CNRI-Python-GPL-Compatible.txt` & `oslili-0.7/oslili/spdx/CNRI-Python-GPL-Compatible.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CNRI-Python.txt` & `oslili-0.7/oslili/spdx/CNRI-Python.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/COIL-1.0.txt` & `oslili-0.7/oslili/spdx/COIL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CPAL-1.0.txt` & `oslili-0.7/oslili/spdx/CPAL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CPL-1.0.txt` & `oslili-0.7/oslili/spdx/CPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CPOL-1.02.txt` & `oslili-0.7/oslili/spdx/CPOL-1.02.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CUA-OPL-1.0.txt` & `oslili-0.7/oslili/spdx/CUA-OPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Caldera.txt` & `oslili-0.7/oslili/spdx/Caldera.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/ClArtistic.txt` & `oslili-0.7/oslili/spdx/ClArtistic.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Classpath-exception-2.0.txt` & `oslili-0.7/oslili/spdx/Classpath-exception-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Clips.txt` & `oslili-0.7/oslili/spdx/Clips.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Community-Spec-1.0.txt` & `oslili-0.7/oslili/spdx/Community-Spec-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Condor-1.1.txt` & `oslili-0.7/oslili/spdx/Condor-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Cornell-Lossless-JPEG.txt` & `oslili-0.7/oslili/spdx/Cornell-Lossless-JPEG.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/CrystalStacker.txt` & `oslili-0.7/oslili/spdx/CrystalStacker.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Cube.txt` & `oslili-0.7/oslili/spdx/Cube.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/D-FSL-1.0.txt` & `oslili-0.7/oslili/spdx/D-FSL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/DL-DE-BY-2.0.txt` & `oslili-0.7/oslili/spdx/DL-DE-BY-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/DOC.txt` & `oslili-0.7/oslili/spdx/DOC.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/DRL-1.0.txt` & `oslili-0.7/oslili/spdx/DRL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/DSDP.txt` & `oslili-0.7/oslili/spdx/DSDP.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/DigiRule-FOSS-exception.txt` & `oslili-0.7/oslili/spdx/DigiRule-FOSS-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/ECL-1.0.txt` & `oslili-0.7/oslili/spdx/ECL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/ECL-2.0.txt` & `oslili-0.7/oslili/spdx/ECL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/EFL-1.0.txt` & `oslili-0.7/oslili/spdx/EFL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/EFL-2.0.txt` & `oslili-0.7/oslili/spdx/EFL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/EPICS.txt` & `oslili-0.7/oslili/spdx/EPICS.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/EPL-1.0.txt` & `oslili-0.7/oslili/spdx/EPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/EPL-2.0.txt` & `oslili-0.7/oslili/spdx/EPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/EUDatagrid.txt` & `oslili-0.7/oslili/spdx/EUDatagrid.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/EUPL-1.0.txt` & `oslili-0.7/oslili/spdx/EUPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/EUPL-1.1.txt` & `oslili-0.7/oslili/spdx/EUPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/EUPL-1.2.txt` & `oslili-0.7/oslili/spdx/EUPL-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Elastic-2.0.txt` & `oslili-0.7/oslili/spdx/Elastic-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Entessa.txt` & `oslili-0.7/oslili/spdx/Entessa.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/ErlPL-1.1.txt` & `oslili-0.7/oslili/spdx/ErlPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Eurosym.txt` & `oslili-0.7/oslili/spdx/Eurosym.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/FDK-AAC.txt` & `oslili-0.7/oslili/spdx/FDK-AAC.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/FLTK-exception.txt` & `oslili-0.7/oslili/spdx/FLTK-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/FSFULLRWD.txt` & `oslili-0.7/oslili/spdx/FSFULLRWD.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/FTL.txt` & `oslili-0.7/oslili/spdx/FTL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Fawkes-Runtime-exception.txt` & `oslili-0.7/oslili/spdx/Fawkes-Runtime-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Font-exception-2.0.txt` & `oslili-0.7/oslili/spdx/Font-exception-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Frameworx-1.0.txt` & `oslili-0.7/oslili/spdx/Frameworx-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/FreeBSD-DOC.txt` & `oslili-0.7/oslili/spdx/FreeBSD-DOC.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/FreeImage.txt` & `oslili-0.7/oslili/spdx/FreeImage.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GCC-exception-3.1.txt` & `oslili-0.7/oslili/spdx/GCC-exception-3.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GD.txt` & `oslili-0.7/oslili/spdx/GD.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.1-invariants-only.txt` & `oslili-0.7/oslili/spdx/GFDL-1.1-invariants-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.1-invariants-or-later.txt` & `oslili-0.7/oslili/spdx/GFDL-1.1-invariants-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.1-no-invariants-only.txt` & `oslili-0.7/oslili/spdx/GFDL-1.1-no-invariants-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.1-no-invariants-or-later.txt` & `oslili-0.7/oslili/spdx/GFDL-1.1-no-invariants-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.1-only.txt` & `oslili-0.7/oslili/spdx/GFDL-1.1-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.1-or-later.txt` & `oslili-0.7/oslili/spdx/GFDL-1.1-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.2-invariants-only.txt` & `oslili-0.7/oslili/spdx/GFDL-1.2-invariants-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.2-invariants-or-later.txt` & `oslili-0.7/oslili/spdx/GFDL-1.2-invariants-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.2-no-invariants-only.txt` & `oslili-0.7/oslili/spdx/GFDL-1.2-no-invariants-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.2-no-invariants-or-later.txt` & `oslili-0.7/oslili/spdx/GFDL-1.2-no-invariants-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.2-only.txt` & `oslili-0.7/oslili/spdx/GFDL-1.2-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.2-or-later.txt` & `oslili-0.7/oslili/spdx/GFDL-1.2-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.3-invariants-only.txt` & `oslili-0.7/oslili/spdx/GFDL-1.3-invariants-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.3-invariants-or-later.txt` & `oslili-0.7/oslili/spdx/GFDL-1.3-invariants-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.3-no-invariants-only.txt` & `oslili-0.7/oslili/spdx/GFDL-1.3-no-invariants-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.3-no-invariants-or-later.txt` & `oslili-0.7/oslili/spdx/GFDL-1.3-no-invariants-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.3-only.txt` & `oslili-0.7/oslili/spdx/GFDL-1.3-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GFDL-1.3-or-later.txt` & `oslili-0.7/oslili/spdx/GFDL-1.3-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GL2PS.txt` & `oslili-0.7/oslili/spdx/GL2PS.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GLWTPL.txt` & `oslili-0.7/oslili/spdx/GLWTPL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GPL-1.0-only.txt` & `oslili-0.7/oslili/spdx/GPL-1.0-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GPL-1.0-or-later.txt` & `oslili-0.7/oslili/spdx/GPL-1.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GPL-2.0-only.txt` & `oslili-0.7/oslili/spdx/GPL-2.0-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GPL-2.0-or-later.txt` & `oslili-0.7/oslili/spdx/GPL-2.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GPL-3.0-linking-source-exception.txt` & `oslili-0.7/oslili/spdx/GPL-3.0-linking-source-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GPL-3.0-only.txt` & `oslili-0.7/oslili/spdx/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GPL-3.0-or-later.txt` & `oslili-0.7/oslili/spdx/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/GPL-CC-1.0.txt` & `oslili-0.7/oslili/spdx/GPL-CC-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Giftware.txt` & `oslili-0.7/oslili/spdx/Giftware.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Glide.txt` & `oslili-0.7/oslili/spdx/Glide.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Graphics-Gems.txt` & `oslili-0.7/oslili/spdx/Graphics-Gems.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/HP-1986.txt` & `oslili-0.7/oslili/spdx/HP-1986.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/HPND-export-US.txt` & `oslili-0.7/oslili/spdx/HPND-export-US.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/HPND-sell-variant-MIT-disclaimer.txt` & `oslili-0.7/oslili/spdx/HPND-sell-variant-MIT-disclaimer.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/HPND-sell-variant.txt` & `oslili-0.7/oslili/spdx/HPND-sell-variant.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/HPND.txt` & `oslili-0.7/oslili/spdx/HPND.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/HTMLTIDY.txt` & `oslili-0.7/oslili/spdx/HTMLTIDY.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/HaskellReport.txt` & `oslili-0.7/oslili/spdx/HaskellReport.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Hippocratic-2.1.txt` & `oslili-0.7/oslili/spdx/Hippocratic-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/IBM-pibs.txt` & `oslili-0.7/oslili/spdx/IBM-pibs.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/ICU.txt` & `oslili-0.7/oslili/spdx/ICU.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/IEC-Code-Components-EULA.txt` & `oslili-0.7/oslili/spdx/IEC-Code-Components-EULA.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/IJG-short.txt` & `oslili-0.7/oslili/spdx/IJG-short.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/IJG.txt` & `oslili-0.7/oslili/spdx/IJG.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/IPA.txt` & `oslili-0.7/oslili/spdx/IPA.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/IPL-1.0.txt` & `oslili-0.7/oslili/spdx/IPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/ISC.txt` & `oslili-0.7/oslili/spdx/ISC.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/ImageMagick.txt` & `oslili-0.7/oslili/spdx/ImageMagick.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Imlib2.txt` & `oslili-0.7/oslili/spdx/Imlib2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Info-ZIP.txt` & `oslili-0.7/oslili/spdx/Info-ZIP.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Intel-ACPI.txt` & `oslili-0.7/oslili/spdx/Intel-ACPI.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Intel.txt` & `oslili-0.7/oslili/spdx/Intel.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Interbase-1.0.txt` & `oslili-0.7/oslili/spdx/Interbase-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/JPL-image.txt` & `oslili-0.7/oslili/spdx/JPL-image.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/JPNIC.txt` & `oslili-0.7/oslili/spdx/JPNIC.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/JSON.txt` & `oslili-0.7/oslili/spdx/JSON.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/JasPer-2.0.txt` & `oslili-0.7/oslili/spdx/JasPer-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Kazlib.txt` & `oslili-0.7/oslili/spdx/Kazlib.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LAL-1.2.txt` & `oslili-0.7/oslili/spdx/LAL-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LAL-1.3.txt` & `oslili-0.7/oslili/spdx/LAL-1.3.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LGPL-2.0-only.txt` & `oslili-0.7/oslili/spdx/LGPL-2.0-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LGPL-2.0-or-later.txt` & `oslili-0.7/oslili/spdx/LGPL-2.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LGPL-2.1-only.txt` & `oslili-0.7/oslili/spdx/LGPL-2.1-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LGPL-2.1-or-later.txt` & `oslili-0.7/oslili/spdx/LGPL-2.1-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LGPL-3.0-linking-exception.txt` & `oslili-0.7/oslili/spdx/LGPL-3.0-linking-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LGPL-3.0-only.txt` & `oslili-0.7/oslili/spdx/LGPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LGPL-3.0-or-later.txt` & `oslili-0.7/oslili/spdx/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LGPLLR.txt` & `oslili-0.7/oslili/spdx/LGPLLR.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LLVM-exception.txt` & `oslili-0.7/oslili/spdx/LLVM-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LOOP.txt` & `oslili-0.7/oslili/spdx/LOOP.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LPL-1.0.txt` & `oslili-0.7/oslili/spdx/LPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LPL-1.02.txt` & `oslili-0.7/oslili/spdx/LPL-1.02.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LPPL-1.0.txt` & `oslili-0.7/oslili/spdx/LPPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LPPL-1.1.txt` & `oslili-0.7/oslili/spdx/LPPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LPPL-1.2.txt` & `oslili-0.7/oslili/spdx/LPPL-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LPPL-1.3a.txt` & `oslili-0.7/oslili/spdx/LPPL-1.3a.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LPPL-1.3c.txt` & `oslili-0.7/oslili/spdx/LPPL-1.3c.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LZMA-SDK-9.22.txt` & `oslili-0.7/oslili/spdx/LZMA-SDK-9.22.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LZMA-exception.txt` & `oslili-0.7/oslili/spdx/LZMA-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Latex2e.txt` & `oslili-0.7/oslili/spdx/Latex2e.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Leptonica.txt` & `oslili-0.7/oslili/spdx/Leptonica.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LiLiQ-P-1.1.txt` & `oslili-0.7/oslili/spdx/LiLiQ-P-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LiLiQ-R-1.1.txt` & `oslili-0.7/oslili/spdx/LiLiQ-R-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/LiLiQ-Rplus-1.1.txt` & `oslili-0.7/oslili/spdx/LiLiQ-Rplus-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Libpng.txt` & `oslili-0.7/oslili/spdx/Libpng.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Linux-OpenIB.txt` & `oslili-0.7/oslili/spdx/Linux-OpenIB.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Linux-man-pages-copyleft.txt` & `oslili-0.7/oslili/spdx/Linux-man-pages-copyleft.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Linux-syscall-note.txt` & `oslili-0.7/oslili/spdx/Linux-syscall-note.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MIT-0.txt` & `oslili-0.7/oslili/spdx/MIT-0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MIT-CMU.txt` & `oslili-0.7/oslili/spdx/MIT-CMU.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MIT-Modern-Variant.txt` & `oslili-0.7/oslili/spdx/MIT-Modern-Variant.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MIT-Wu.txt` & `oslili-0.7/oslili/spdx/MIT-Wu.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MIT-advertising.txt` & `oslili-0.7/oslili/spdx/MIT-advertising.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MIT-enna.txt` & `oslili-0.7/oslili/spdx/MIT-enna.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MIT-feh.txt` & `oslili-0.7/oslili/spdx/MIT-feh.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MIT-open-group.txt` & `oslili-0.7/oslili/spdx/MIT-open-group.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MIT.txt` & `oslili-0.7/oslili/spdx/MIT.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MITNFA.txt` & `oslili-0.7/oslili/spdx/MITNFA.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MPL-1.0.txt` & `oslili-0.7/oslili/spdx/MPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MPL-1.1.txt` & `oslili-0.7/oslili/spdx/MPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MPL-2.0-no-copyleft-exception.txt` & `oslili-0.7/oslili/spdx/MPL-2.0-no-copyleft-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MPL-2.0.txt` & `oslili-0.7/oslili/spdx/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MS-LPL.txt` & `oslili-0.7/oslili/spdx/MS-LPL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MS-PL.txt` & `oslili-0.7/oslili/spdx/MS-PL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MS-RL.txt` & `oslili-0.7/oslili/spdx/MS-RL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MTLL.txt` & `oslili-0.7/oslili/spdx/MTLL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MakeIndex.txt` & `oslili-0.7/oslili/spdx/MakeIndex.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Minpack.txt` & `oslili-0.7/oslili/spdx/Minpack.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MirOS.txt` & `oslili-0.7/oslili/spdx/MirOS.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Motosoto.txt` & `oslili-0.7/oslili/spdx/Motosoto.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MulanPSL-1.0.txt` & `oslili-0.7/oslili/spdx/MulanPSL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/MulanPSL-2.0.txt` & `oslili-0.7/oslili/spdx/MulanPSL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Multics.txt` & `oslili-0.7/oslili/spdx/Multics.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Mup.txt` & `oslili-0.7/oslili/spdx/Mup.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NAIST-2003.txt` & `oslili-0.7/oslili/spdx/NAIST-2003.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NASA-1.3.txt` & `oslili-0.7/oslili/spdx/NASA-1.3.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NBPL-1.0.txt` & `oslili-0.7/oslili/spdx/NBPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NCGL-UK-2.0.txt` & `oslili-0.7/oslili/spdx/NCGL-UK-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NCSA.txt` & `oslili-0.7/oslili/spdx/NCSA.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NGPL.txt` & `oslili-0.7/oslili/spdx/NGPL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NICTA-1.0.txt` & `oslili-0.7/oslili/spdx/NICTA-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NIST-PD-fallback.txt` & `oslili-0.7/oslili/spdx/NIST-PD-fallback.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NIST-PD.txt` & `oslili-0.7/oslili/spdx/NIST-PD.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NLOD-1.0.txt` & `oslili-0.7/oslili/spdx/NLOD-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NLOD-2.0.txt` & `oslili-0.7/oslili/spdx/NLOD-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NOSL.txt` & `oslili-0.7/oslili/spdx/NOSL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NPL-1.0.txt` & `oslili-0.7/oslili/spdx/NPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NPL-1.1.txt` & `oslili-0.7/oslili/spdx/NPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NPOSL-3.0.txt` & `oslili-0.7/oslili/spdx/NPOSL-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NRL.txt` & `oslili-0.7/oslili/spdx/NRL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NTP-0.txt` & `oslili-0.7/oslili/spdx/NTP-0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NTP.txt` & `oslili-0.7/oslili/spdx/NTP.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Naumen.txt` & `oslili-0.7/oslili/spdx/Naumen.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Net-SNMP.txt` & `oslili-0.7/oslili/spdx/Net-SNMP.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/NetCDF.txt` & `oslili-0.7/oslili/spdx/NetCDF.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Nokia-Qt-exception-1.1.txt` & `oslili-0.7/oslili/spdx/Nokia-Qt-exception-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Nokia.txt` & `oslili-0.7/oslili/spdx/Nokia.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Noweb.txt` & `oslili-0.7/oslili/spdx/Noweb.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/O-UDA-1.0.txt` & `oslili-0.7/oslili/spdx/O-UDA-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OCCT-PL.txt` & `oslili-0.7/oslili/spdx/OCCT-PL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OCCT-exception-1.0.txt` & `oslili-0.7/oslili/spdx/OCCT-exception-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OCLC-2.0.txt` & `oslili-0.7/oslili/spdx/OCLC-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OCaml-LGPL-linking-exception.txt` & `oslili-0.7/oslili/spdx/OCaml-LGPL-linking-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/ODC-By-1.0.txt` & `oslili-0.7/oslili/spdx/ODC-By-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/ODbL-1.0.txt` & `oslili-0.7/oslili/spdx/ODbL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OFFIS.txt` & `oslili-0.7/oslili/spdx/OFFIS.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OFL-1.0-RFN.txt` & `oslili-0.7/oslili/spdx/OFL-1.0-RFN.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OFL-1.0-no-RFN.txt` & `oslili-0.7/oslili/spdx/OFL-1.0-no-RFN.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OFL-1.0.txt` & `oslili-0.7/oslili/spdx/OFL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OFL-1.1-RFN.txt` & `oslili-0.7/oslili/spdx/OFL-1.1-RFN.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OFL-1.1-no-RFN.txt` & `oslili-0.7/oslili/spdx/OFL-1.1-no-RFN.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OFL-1.1.txt` & `oslili-0.7/oslili/spdx/OFL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OGC-1.0.txt` & `oslili-0.7/oslili/spdx/OGC-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OGDL-Taiwan-1.0.txt` & `oslili-0.7/oslili/spdx/OGDL-Taiwan-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OGL-Canada-2.0.txt` & `oslili-0.7/oslili/spdx/OGL-Canada-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OGL-UK-1.0.txt` & `oslili-0.7/oslili/spdx/OGL-UK-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OGL-UK-2.0.txt` & `oslili-0.7/oslili/spdx/OGL-UK-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OGL-UK-3.0.txt` & `oslili-0.7/oslili/spdx/OGL-UK-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OGTSL.txt` & `oslili-0.7/oslili/spdx/OGTSL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-1.1.txt` & `oslili-0.7/oslili/spdx/OLDAP-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-1.2.txt` & `oslili-0.7/oslili/spdx/OLDAP-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-1.3.txt` & `oslili-0.7/oslili/spdx/OLDAP-1.3.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-1.4.txt` & `oslili-0.7/oslili/spdx/OLDAP-1.4.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-2.0.1.txt` & `oslili-0.7/oslili/spdx/OLDAP-2.0.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-2.0.txt` & `oslili-0.7/oslili/spdx/OLDAP-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-2.1.txt` & `oslili-0.7/oslili/spdx/OLDAP-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-2.2.1.txt` & `oslili-0.7/oslili/spdx/OLDAP-2.2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-2.2.2.txt` & `oslili-0.7/oslili/spdx/OLDAP-2.2.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-2.2.txt` & `oslili-0.7/oslili/spdx/OLDAP-2.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-2.3.txt` & `oslili-0.7/oslili/spdx/OLDAP-2.3.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-2.4.txt` & `oslili-0.7/oslili/spdx/OLDAP-2.4.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-2.5.txt` & `oslili-0.7/oslili/spdx/OLDAP-2.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-2.6.txt` & `oslili-0.7/oslili/spdx/OLDAP-2.6.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-2.7.txt` & `oslili-0.7/oslili/spdx/OLDAP-2.7.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OLDAP-2.8.txt` & `oslili-0.7/oslili/spdx/OLDAP-2.8.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OML.txt` & `oslili-0.7/oslili/spdx/OML.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OPL-1.0.txt` & `oslili-0.7/oslili/spdx/OPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OPUBL-1.0.txt` & `oslili-0.7/oslili/spdx/OPUBL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OSET-PL-2.1.txt` & `oslili-0.7/oslili/spdx/OSET-PL-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OSL-1.0.txt` & `oslili-0.7/oslili/spdx/OSL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OSL-1.1.txt` & `oslili-0.7/oslili/spdx/OSL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OSL-2.0.txt` & `oslili-0.7/oslili/spdx/OSL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OSL-2.1.txt` & `oslili-0.7/oslili/spdx/OSL-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OSL-3.0.txt` & `oslili-0.7/oslili/spdx/OSL-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OpenJDK-assembly-exception-1.0.txt` & `oslili-0.7/oslili/spdx/OpenJDK-assembly-exception-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OpenPBS-2.3.txt` & `oslili-0.7/oslili/spdx/OpenPBS-2.3.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/OpenSSL.txt` & `oslili-0.7/oslili/spdx/OpenSSL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/PDDL-1.0.txt` & `oslili-0.7/oslili/spdx/PDDL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/PHP-3.0.txt` & `oslili-0.7/oslili/spdx/PHP-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/PHP-3.01.txt` & `oslili-0.7/oslili/spdx/PHP-3.01.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/PSF-2.0.txt` & `oslili-0.7/oslili/spdx/PSF-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Parity-6.0.0.txt` & `oslili-0.7/oslili/spdx/Parity-6.0.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Parity-7.0.0.txt` & `oslili-0.7/oslili/spdx/Parity-7.0.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Plexus.txt` & `oslili-0.7/oslili/spdx/Plexus.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/PolyForm-Noncommercial-1.0.0.txt` & `oslili-0.7/oslili/spdx/PolyForm-Noncommercial-1.0.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/PolyForm-Small-Business-1.0.0.txt` & `oslili-0.7/oslili/spdx/PolyForm-Small-Business-1.0.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/PostgreSQL.txt` & `oslili-0.7/oslili/spdx/PostgreSQL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Python-2.0.1.txt` & `oslili-0.7/oslili/spdx/Python-2.0.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Python-2.0.txt` & `oslili-0.7/oslili/spdx/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/QPL-1.0-INRIA-2004.txt` & `oslili-0.7/oslili/spdx/QPL-1.0-INRIA-2004.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/QPL-1.0.txt` & `oslili-0.7/oslili/spdx/QPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Qhull.txt` & `oslili-0.7/oslili/spdx/Qhull.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Qt-GPL-exception-1.0.txt` & `oslili-0.7/oslili/spdx/Qt-GPL-exception-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Qt-LGPL-exception-1.1.txt` & `oslili-0.7/oslili/spdx/Qt-LGPL-exception-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Qwt-exception-1.0.txt` & `oslili-0.7/oslili/spdx/Qwt-exception-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/RHeCos-1.1.txt` & `oslili-0.7/oslili/spdx/RHeCos-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/RPL-1.1.txt` & `oslili-0.7/oslili/spdx/RPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/RPL-1.5.txt` & `oslili-0.7/oslili/spdx/RPL-1.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/RPSL-1.0.txt` & `oslili-0.7/oslili/spdx/RPSL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/RSA-MD.txt` & `oslili-0.7/oslili/spdx/RSA-MD.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/RSCPL.txt` & `oslili-0.7/oslili/spdx/RSCPL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Rdisc.txt` & `oslili-0.7/oslili/spdx/Rdisc.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Ruby.txt` & `oslili-0.7/oslili/spdx/Ruby.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SAX-PD.txt` & `oslili-0.7/oslili/spdx/SAX-PD.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SCEA.txt` & `oslili-0.7/oslili/spdx/SCEA.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SGI-B-1.0.txt` & `oslili-0.7/oslili/spdx/SGI-B-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SGI-B-1.1.txt` & `oslili-0.7/oslili/spdx/SGI-B-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SGI-B-2.0.txt` & `oslili-0.7/oslili/spdx/SGI-B-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SHL-0.5.txt` & `oslili-0.7/oslili/spdx/SHL-0.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SHL-0.51.txt` & `oslili-0.7/oslili/spdx/SHL-0.51.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SHL-2.0.txt` & `oslili-0.7/oslili/spdx/SHL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SHL-2.1.txt` & `oslili-0.7/oslili/spdx/SHL-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SISSL-1.2.txt` & `oslili-0.7/oslili/spdx/SISSL-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SISSL.txt` & `oslili-0.7/oslili/spdx/SISSL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SMLNJ.txt` & `oslili-0.7/oslili/spdx/SMLNJ.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SMPPL.txt` & `oslili-0.7/oslili/spdx/SMPPL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SNIA.txt` & `oslili-0.7/oslili/spdx/SNIA.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SPL-1.0.txt` & `oslili-0.7/oslili/spdx/SPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SSH-OpenSSH.txt` & `oslili-0.7/oslili/spdx/SSH-OpenSSH.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SSPL-1.0.txt` & `oslili-0.7/oslili/spdx/SSPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SWL.txt` & `oslili-0.7/oslili/spdx/SWL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Saxpath.txt` & `oslili-0.7/oslili/spdx/Saxpath.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Sendmail-8.23.txt` & `oslili-0.7/oslili/spdx/Sendmail-8.23.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Sendmail.txt` & `oslili-0.7/oslili/spdx/Sendmail.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SimPL-2.0.txt` & `oslili-0.7/oslili/spdx/SimPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Sleepycat.txt` & `oslili-0.7/oslili/spdx/Sleepycat.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Spencer-86.txt` & `oslili-0.7/oslili/spdx/Spencer-86.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Spencer-94.txt` & `oslili-0.7/oslili/spdx/Spencer-94.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Spencer-99.txt` & `oslili-0.7/oslili/spdx/Spencer-99.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/SugarCRM-1.1.3.txt` & `oslili-0.7/oslili/spdx/SugarCRM-1.1.3.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Symlinks.txt` & `oslili-0.7/oslili/spdx/Symlinks.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/TAPR-OHL-1.0.txt` & `oslili-0.7/oslili/spdx/TAPR-OHL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/TCL.txt` & `oslili-0.7/oslili/spdx/TCL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/TCP-wrappers.txt` & `oslili-0.7/oslili/spdx/TCP-wrappers.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/TMate.txt` & `oslili-0.7/oslili/spdx/TMate.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/TORQUE-1.1.txt` & `oslili-0.7/oslili/spdx/TORQUE-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/TOSL.txt` & `oslili-0.7/oslili/spdx/TOSL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/TPL-1.0.txt` & `oslili-0.7/oslili/spdx/TPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/TU-Berlin-1.0.txt` & `oslili-0.7/oslili/spdx/TU-Berlin-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/TU-Berlin-2.0.txt` & `oslili-0.7/oslili/spdx/TU-Berlin-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/UCAR.txt` & `oslili-0.7/oslili/spdx/UCAR.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/UCL-1.0.txt` & `oslili-0.7/oslili/spdx/UCL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/UPL-1.0.txt` & `oslili-0.7/oslili/spdx/UPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Unicode-DFS-2015.txt` & `oslili-0.7/oslili/spdx/Unicode-DFS-2015.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Unicode-DFS-2016.txt` & `oslili-0.7/oslili/spdx/Unicode-DFS-2016.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Unicode-TOU.txt` & `oslili-0.7/oslili/spdx/Unicode-TOU.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Universal-FOSS-exception-1.0.txt` & `oslili-0.7/oslili/spdx/Universal-FOSS-exception-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Unlicense.txt` & `oslili-0.7/oslili/spdx/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/VOSTROM.txt` & `oslili-0.7/oslili/spdx/VOSTROM.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/VSL-1.0.txt` & `oslili-0.7/oslili/spdx/VSL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Vim.txt` & `oslili-0.7/oslili/spdx/Vim.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/W3C-19980720.txt` & `oslili-0.7/oslili/spdx/W3C-19980720.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/W3C-20150513.txt` & `oslili-0.7/oslili/spdx/W3C-20150513.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/W3C.txt` & `oslili-0.7/oslili/spdx/W3C.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Watcom-1.0.txt` & `oslili-0.7/oslili/spdx/Watcom-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Wsuipa.txt` & `oslili-0.7/oslili/spdx/Wsuipa.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/WxWindows-exception-3.1.txt` & `oslili-0.7/oslili/spdx/WxWindows-exception-3.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/X11-distribute-modifications-variant.txt` & `oslili-0.7/oslili/spdx/X11-distribute-modifications-variant.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/X11.txt` & `oslili-0.7/oslili/spdx/X11.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/XFree86-1.1.txt` & `oslili-0.7/oslili/spdx/XFree86-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/XSkat.txt` & `oslili-0.7/oslili/spdx/XSkat.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Xerox.txt` & `oslili-0.7/oslili/spdx/Xerox.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Xnet.txt` & `oslili-0.7/oslili/spdx/Xnet.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/YPL-1.0.txt` & `oslili-0.7/oslili/spdx/YPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/YPL-1.1.txt` & `oslili-0.7/oslili/spdx/YPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/ZPL-1.1.txt` & `oslili-0.7/oslili/spdx/ZPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/ZPL-2.0.txt` & `oslili-0.7/oslili/spdx/ZPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/ZPL-2.1.txt` & `oslili-0.7/oslili/spdx/ZPL-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Zend-2.0.txt` & `oslili-0.7/oslili/spdx/Zend-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Zimbra-1.3.txt` & `oslili-0.7/oslili/spdx/Zimbra-1.3.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Zimbra-1.4.txt` & `oslili-0.7/oslili/spdx/Zimbra-1.4.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/Zlib.txt` & `oslili-0.7/oslili/spdx/Zlib.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/bzip2-1.0.6.txt` & `oslili-0.7/oslili/spdx/bzip2-1.0.6.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/copyleft-next-0.3.0.txt` & `oslili-0.7/oslili/spdx/copyleft-next-0.3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/copyleft-next-0.3.1.txt` & `oslili-0.7/oslili/spdx/copyleft-next-0.3.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/curl.txt` & `oslili-0.7/oslili/spdx/curl.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/eCos-exception-2.0.txt` & `oslili-0.7/oslili/spdx/eCos-exception-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/eGenix.txt` & `oslili-0.7/oslili/spdx/eGenix.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/etalab-2.0.txt` & `oslili-0.7/oslili/spdx/etalab-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/freertos-exception-2.0.txt` & `oslili-0.7/oslili/spdx/freertos-exception-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/gSOAP-1.3b.txt` & `oslili-0.7/oslili/spdx/gSOAP-1.3b.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/gnuplot.txt` & `oslili-0.7/oslili/spdx/gnuplot.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/i2p-gpl-java-exception.txt` & `oslili-0.7/oslili/spdx/i2p-gpl-java-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/iMatix.txt` & `oslili-0.7/oslili/spdx/iMatix.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/libpng-2.0.txt` & `oslili-0.7/oslili/spdx/libpng-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/libselinux-1.0.txt` & `oslili-0.7/oslili/spdx/libselinux-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/libtiff.txt` & `oslili-0.7/oslili/spdx/libtiff.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/libutil-David-Nugent.txt` & `oslili-0.7/oslili/spdx/libutil-David-Nugent.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/mif-exception.txt` & `oslili-0.7/oslili/spdx/mif-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/mpi-permissive.txt` & `oslili-0.7/oslili/spdx/mpi-permissive.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/mpich2.txt` & `oslili-0.7/oslili/spdx/mpich2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/openvpn-openssl-exception.txt` & `oslili-0.7/oslili/spdx/openvpn-openssl-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/psutils.txt` & `oslili-0.7/oslili/spdx/psutils.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/u-boot-exception-2.0.txt` & `oslili-0.7/oslili/spdx/u-boot-exception-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/w3m.txt` & `oslili-0.7/oslili/spdx/w3m.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/x11vnc-openssl-exception.txt` & `oslili-0.7/oslili/spdx/x11vnc-openssl-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/xinetd.txt` & `oslili-0.7/oslili/spdx/xinetd.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/xlock.txt` & `oslili-0.7/oslili/spdx/xlock.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/xpp.txt` & `oslili-0.7/oslili/spdx/xpp.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili/spdx/zlib-acknowledgement.txt` & `oslili-0.7/oslili/spdx/zlib-acknowledgement.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/oslili.egg-info/PKG-INFO` & `oslili-0.7/oslili.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: oslili
-Version: 0.6
+Version: 0.7
 Summary: Open Source License Identification Library
 Home-page: https://github.com/oscarvalenzuelab/oslili
 Author: Oscar Valenzuela B.
-Author-email: oscar.valenzuela.b@gmail.com
+Author-email: alkamod@gmail.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oslili-0.6/oslili.egg-info/SOURCES.txt` & `oslili-0.7/oslili.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.6/setup.py` & `oslili-0.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pathlib
 import sys
 from setuptools import setup, find_packages
 
 
 HERE = pathlib.Path(__file__).parent
-VERSION = '0.6'
+VERSION = '0.7'
 PACKAGE_NAME = 'oslili'
 AUTHOR = 'Oscar Valenzuela B.'
-AUTHOR_EMAIL = 'oscar.valenzuela.b@gmail.com'
+AUTHOR_EMAIL = 'alkamod@gmail.com'
 URL = 'https://github.com/oscarvalenzuelab/oslili'
 LICENSE = 'Apache-2.0'
 DESCRIPTION = 'Open Source License Identification Library'
 LONG_DESCRIPTION = (HERE / "README.md").read_text()
 LONG_DESC_TYPE = "text/markdown"
 
 setup(
```

