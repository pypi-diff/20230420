# Comparing `tmp/eQTac-1.0.6.tar.gz` & `tmp/eQTac-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eQTac-1.0.6.tar", last modified: Thu Apr 20 01:54:27 2023, max compression
+gzip compressed data, was "eQTac-1.0.7.tar", last modified: Thu Apr 20 03:41:28 2023, max compression
```

## Comparing `eQTac-1.0.6.tar` & `eQTac-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 01:54:27.112834 eQTac-1.0.6/
--rw-rw-rw-   0        0        0     1539 2023-04-19 07:30:51.000000 eQTac-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       17 2023-04-19 07:47:38.000000 eQTac-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5926 2023-04-20 01:54:27.110839 eQTac-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5429 2023-04-20 01:48:21.000000 eQTac-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 01:54:26.996147 eQTac-1.0.6/eQTac/
--rw-rw-rw-   0        0        0        0 2023-04-19 08:08:46.000000 eQTac-1.0.6/eQTac/__init__.py
--rw-rw-rw-   0        0        0     1860 2023-04-18 09:28:48.000000 eQTac-1.0.6/eQTac/control_FDR.py
--rw-rw-rw-   0        0        0     4204 2023-04-19 08:46:12.000000 eQTac-1.0.6/eQTac/eQTac_correlation.py
--rw-rw-rw-   0        0        0     2122 2023-04-19 08:47:10.000000 eQTac-1.0.6/eQTac/eQTac_permutation.py
--rw-rw-rw-   0        0        0     2608 2023-04-19 08:48:46.000000 eQTac-1.0.6/eQTac/filter_bkg.py
--rw-rw-rw-   0        0        0     4744 2023-04-17 11:42:17.000000 eQTac-1.0.6/eQTac/generate_PRE.py
--rw-rw-rw-   0        0        0     2594 2023-04-17 11:42:17.000000 eQTac-1.0.6/eQTac/generate_mut_fa.py
--rw-rw-rw-   0        0        0      910 2023-04-17 11:42:17.000000 eQTac-1.0.6/eQTac/generate_snp_dict.py
--rw-rw-rw-   0        0        0     3646 2023-04-19 08:54:46.000000 eQTac-1.0.6/eQTac/geno2score.py
--rw-rw-rw-   0        0        0     2457 2023-04-19 08:55:27.000000 eQTac-1.0.6/eQTac/get_nullseq.py
-drwxrwxrwx   0        0        0        0 2023-04-20 01:54:27.093914 eQTac-1.0.6/eQTac.egg-info/
--rw-rw-rw-   0        0        0     5926 2023-04-20 01:54:26.000000 eQTac-1.0.6/eQTac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-04-20 01:54:26.000000 eQTac-1.0.6/eQTac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 01:54:26.000000 eQTac-1.0.6/eQTac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-04-20 01:54:26.000000 eQTac-1.0.6/eQTac.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 01:54:26.000000 eQTac-1.0.6/eQTac.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 01:54:27.115826 eQTac-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      767 2023-04-20 01:54:17.000000 eQTac-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:41:28.304611 eQTac-1.0.7/
+-rw-rw-rw-   0        0        0     1539 2023-04-19 07:30:51.000000 eQTac-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-04-19 07:47:38.000000 eQTac-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5926 2023-04-20 03:41:28.301618 eQTac-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5429 2023-04-20 02:35:35.000000 eQTac-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 03:41:28.183933 eQTac-1.0.7/eQTac/
+-rw-rw-rw-   0        0        0        0 2023-04-19 08:08:46.000000 eQTac-1.0.7/eQTac/__init__.py
+-rw-rw-rw-   0        0        0     1860 2023-04-18 09:28:48.000000 eQTac-1.0.7/eQTac/control_FDR.py
+-rw-rw-rw-   0        0        0     4204 2023-04-19 08:46:12.000000 eQTac-1.0.7/eQTac/eQTac_correlation.py
+-rw-rw-rw-   0        0        0     2122 2023-04-19 08:47:10.000000 eQTac-1.0.7/eQTac/eQTac_permutation.py
+-rw-rw-rw-   0        0        0     2608 2023-04-19 08:48:46.000000 eQTac-1.0.7/eQTac/filter_bkg.py
+-rw-rw-rw-   0        0        0     4744 2023-04-17 11:42:17.000000 eQTac-1.0.7/eQTac/generate_PRE.py
+-rw-rw-rw-   0        0        0     2594 2023-04-17 11:42:17.000000 eQTac-1.0.7/eQTac/generate_mut_fa.py
+-rw-rw-rw-   0        0        0      910 2023-04-17 11:42:17.000000 eQTac-1.0.7/eQTac/generate_snp_dict.py
+-rw-rw-rw-   0        0        0     3646 2023-04-19 08:54:46.000000 eQTac-1.0.7/eQTac/geno2score.py
+-rw-rw-rw-   0        0        0     2457 2023-04-19 08:55:27.000000 eQTac-1.0.7/eQTac/get_nullseq.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:41:28.284663 eQTac-1.0.7/eQTac.egg-info/
+-rw-rw-rw-   0        0        0     5926 2023-04-20 03:41:27.000000 eQTac-1.0.7/eQTac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-04-20 03:41:28.000000 eQTac-1.0.7/eQTac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 03:41:27.000000 eQTac-1.0.7/eQTac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-04-20 03:41:27.000000 eQTac-1.0.7/eQTac.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 03:41:27.000000 eQTac-1.0.7/eQTac.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 03:41:28.308600 eQTac-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      765 2023-04-20 03:41:19.000000 eQTac-1.0.7/setup.py
```

### Comparing `eQTac-1.0.6/LICENSE` & `eQTac-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.6/PKG-INFO` & `eQTac-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eQTac
-Version: 1.0.6
+Version: 1.0.7
 Summary: The eQTac method.
 Home-page: https://github.com/JFF1594032292/eQTac
 Author: Jiang Feng
 Author-email: 1594032292@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.7
```

### Comparing `eQTac-1.0.6/README.md` & `eQTac-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.6/eQTac/control_FDR.py` & `eQTac-1.0.7/eQTac/control_FDR.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.6/eQTac/eQTac_correlation.py` & `eQTac-1.0.7/eQTac/eQTac_correlation.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.6/eQTac/eQTac_permutation.py` & `eQTac-1.0.7/eQTac/eQTac_permutation.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.6/eQTac/filter_bkg.py` & `eQTac-1.0.7/eQTac/filter_bkg.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.6/eQTac/generate_PRE.py` & `eQTac-1.0.7/eQTac/generate_PRE.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.6/eQTac/generate_mut_fa.py` & `eQTac-1.0.7/eQTac/generate_mut_fa.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.6/eQTac/generate_snp_dict.py` & `eQTac-1.0.7/eQTac/generate_snp_dict.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.6/eQTac/geno2score.py` & `eQTac-1.0.7/eQTac/geno2score.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.6/eQTac/get_nullseq.py` & `eQTac-1.0.7/eQTac/get_nullseq.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.6/eQTac.egg-info/PKG-INFO` & `eQTac-1.0.7/eQTac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eQTac
-Version: 1.0.6
+Version: 1.0.7
 Summary: The eQTac method.
 Home-page: https://github.com/JFF1594032292/eQTac
 Author: Jiang Feng
 Author-email: 1594032292@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.7
```

### Comparing `eQTac-1.0.6/setup.py` & `eQTac-1.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as f1:
     long_description = f1.read()
 
 setuptools.setup(
     name="eQTac",
-    version="1.0.6",
+    version="1.0.7",
     author="Jiang Feng",
     author_email="1594032292@qq.com",
     description="The eQTac method.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JFF1594032292/eQTac",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
     ],
     python_requires='>=3.7',
     install_requires=[
-        'numpy >= 1.22.4',
-        'pandas >= 1.4.3',
-        'pybedtools >= 0.8.2',
-        'pysam >= 0.16.0.1',
+        'numpy >= 1.21.6',
+        'pandas >= 1.2.3',
+        'pybedtools >= 0.8.1',
+        'pysam >= 0.15.3',
         'rpy2 >= 3.4.2',
-        'scipy >= 1.8.1'],
+        'scipy >= 1.7.3'],
 )
```

