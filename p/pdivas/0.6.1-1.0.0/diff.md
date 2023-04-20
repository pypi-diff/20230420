# Comparing `tmp/pdivas-0.6.1.tar.gz` & `tmp/pdivas-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdivas-0.6.1.tar", last modified: Mon Mar 20 09:53:54 2023, max compression
+gzip compressed data, was "dist/pdivas-1.0.0.tar", last modified: Thu Apr 20 09:02:53 2023, max compression
```

## Comparing `pdivas-0.6.1.tar` & `pdivas-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-03-20 09:53:54.524403 pdivas-0.6.1/
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     1088 2023-01-23 08:15:04.000000 pdivas-0.6.1/LICENSE
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)       25 2023-01-22 09:13:56.000000 pdivas-0.6.1/MANIFEST.in
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2253 2023-03-20 09:53:54.522394 pdivas-0.6.1/PKG-INFO
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     1910 2023-03-03 06:46:08.000000 pdivas-0.6.1/README.md
-drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-03-20 09:53:54.378428 pdivas-0.6.1/pdivas/
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)      225 2023-03-03 06:50:54.000000 pdivas-0.6.1/pdivas/__init__.py
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     3833 2023-03-03 06:41:45.000000 pdivas-0.6.1/pdivas/__main__.py
-drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-03-20 09:53:54.484533 pdivas-0.6.1/pdivas/model/
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)  1897567 2023-01-22 05:53:51.000000 pdivas-0.6.1/pdivas/model/PDIVAS.sav
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     4316 2023-01-28 08:26:30.000000 pdivas-0.6.1/pdivas/scoring_to_vcf.py
-drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-03-20 09:53:54.463054 pdivas-0.6.1/pdivas.egg-info/
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2253 2023-03-20 09:53:54.000000 pdivas-0.6.1/pdivas.egg-info/PKG-INFO
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)      324 2023-03-20 09:53:54.000000 pdivas-0.6.1/pdivas.egg-info/SOURCES.txt
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)        1 2023-03-20 09:53:54.000000 pdivas-0.6.1/pdivas.egg-info/dependency_links.txt
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)       49 2023-03-20 09:53:54.000000 pdivas-0.6.1/pdivas.egg-info/entry_points.txt
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)       40 2023-03-20 09:53:54.000000 pdivas-0.6.1/pdivas.egg-info/requires.txt
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)        7 2023-03-20 09:53:54.000000 pdivas-0.6.1/pdivas.egg-info/top_level.txt
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)       44 2023-01-24 02:22:53.000000 pdivas-0.6.1/requirements.txt
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)       38 2023-03-20 09:53:54.525393 pdivas-0.6.1/setup.cfg
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     1654 2023-03-03 06:43:46.000000 pdivas-0.6.1/setup.py
+drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-04-20 09:02:53.000000 pdivas-1.0.0/
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     1088 2023-04-20 06:40:12.000000 pdivas-1.0.0/LICENSE
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)       25 2023-04-20 06:44:18.000000 pdivas-1.0.0/MANIFEST.in
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2233 2023-04-20 09:02:53.000000 pdivas-1.0.0/PKG-INFO
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     1910 2023-04-20 06:40:12.000000 pdivas-1.0.0/README.md
+drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-04-20 09:02:53.000000 pdivas-1.0.0/pdivas/
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)      221 2023-04-20 09:01:00.000000 pdivas-1.0.0/pdivas/__init__.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     7315 2023-04-20 09:00:17.000000 pdivas-1.0.0/pdivas/__main__.py
+drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-04-20 09:02:53.000000 pdivas-1.0.0/pdivas/model/
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)  1897567 2023-04-20 06:40:12.000000 pdivas-1.0.0/pdivas/model/PDIVAS.sav
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     4316 2023-04-20 06:40:12.000000 pdivas-1.0.0/pdivas/scoring_to_vcf.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2111 2023-04-20 08:31:42.000000 pdivas-1.0.0/pdivas/vcf2tsv.py
+drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-04-20 09:02:53.000000 pdivas-1.0.0/pdivas.egg-info/
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2233 2023-04-20 09:02:52.000000 pdivas-1.0.0/pdivas.egg-info/PKG-INFO
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)      342 2023-04-20 09:02:52.000000 pdivas-1.0.0/pdivas.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)        1 2023-04-20 09:02:52.000000 pdivas-1.0.0/pdivas.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)       48 2023-04-20 09:02:52.000000 pdivas-1.0.0/pdivas.egg-info/entry_points.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)       40 2023-04-20 09:02:52.000000 pdivas-1.0.0/pdivas.egg-info/requires.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)        7 2023-04-20 09:02:52.000000 pdivas-1.0.0/pdivas.egg-info/top_level.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)       44 2023-04-20 06:44:18.000000 pdivas-1.0.0/requirements.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)       38 2023-04-20 09:02:53.000000 pdivas-1.0.0/setup.cfg
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     1650 2023-04-20 07:56:35.000000 pdivas-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pdivas-0.6.1/LICENSE` & `pdivas-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdivas-0.6.1/PKG-INFO` & `pdivas-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pdivas
-Version: 0.6.1
+Version: 1.0.0
 Summary: PDIVAS: Pathogenicity predictor for Deep-Intronic Variants causing Aberrant Splicing
 Home-page: https://github.com/shiro-kur/PDIVAS
 Author: Ryo Kurosawa
 Author-email: a0160561@yahoo.co.jp
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PDIVAS : Pathogenicity Predictor for Deep-Intronic Variants causing Aberrant Splicing
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Sumary
@@ -29,9 +28,7 @@
 ## Reference & contact
 bioarxiv?  
 a0160561@yahoo.co.jp (Ryo Kurosawa at Kyoto University)
 
 ## Details
 Please view the detailed usage and methods at https://github.com/shiro-kur/PDIVAS and medRxiv. 
 
-
-
```

### Comparing `pdivas-0.6.1/README.md` & `pdivas-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pdivas-0.6.1/pdivas/model/PDIVAS.sav` & `pdivas-1.0.0/pdivas/model/PDIVAS.sav`

 * *Files identical despite different names*

### Comparing `pdivas-0.6.1/pdivas/scoring_to_vcf.py` & `pdivas-1.0.0/pdivas/scoring_to_vcf.py`

 * *Files identical despite different names*

### Comparing `pdivas-0.6.1/pdivas.egg-info/PKG-INFO` & `pdivas-1.0.0/pdivas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pdivas
-Version: 0.6.1
+Version: 1.0.0
 Summary: PDIVAS: Pathogenicity predictor for Deep-Intronic Variants causing Aberrant Splicing
 Home-page: https://github.com/shiro-kur/PDIVAS
 Author: Ryo Kurosawa
 Author-email: a0160561@yahoo.co.jp
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PDIVAS : Pathogenicity Predictor for Deep-Intronic Variants causing Aberrant Splicing
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Sumary
@@ -29,9 +28,7 @@
 ## Reference & contact
 bioarxiv?  
 a0160561@yahoo.co.jp (Ryo Kurosawa at Kyoto University)
 
 ## Details
 Please view the detailed usage and methods at https://github.com/shiro-kur/PDIVAS and medRxiv. 
 
-
-
```

### Comparing `pdivas-0.6.1/setup.py` & `pdivas-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,9 +42,7 @@
       install_requires=_requirements(),
       package_data={'pdivas': ['model/PDIVAS.sav']},
       entry_points={'console_scripts': ['pdivas=pdivas.__main__:main']},
       test_suite='tests')
       
       
 
-
-
```

