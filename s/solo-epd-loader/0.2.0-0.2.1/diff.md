# Comparing `tmp/solo_epd_loader-0.2.0.tar.gz` & `tmp/solo_epd_loader-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solo_epd_loader-0.2.0.tar", last modified: Thu Apr 20 12:50:56 2023, max compression
+gzip compressed data, was "solo_epd_loader-0.2.1.tar", last modified: Thu Apr 20 13:34:16 2023, max compression
```

## Comparing `solo_epd_loader-0.2.0.tar` & `solo_epd_loader-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 12:50:56.824914 solo_epd_loader-0.2.0/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.0/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.0/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15865 2023-04-20 12:50:56.824914 solo_epd_loader-0.2.0/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    14917 2022-09-21 10:27:58.000000 solo_epd_loader-0.2.0/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.0/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 12:50:56.808914 solo_epd_loader-0.2.0/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.0/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.0/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.0/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.0/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 12:50:56.812914 solo_epd_loader-0.2.0/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.0/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.0/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.0/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.0/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 12:50:56.816913 solo_epd_loader-0.2.0/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.0/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.0/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.0/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2302 2023-04-20 12:50:56.828914 solo_epd_loader-0.2.0/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.0/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 12:50:56.816913 solo_epd_loader-0.2.0/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    37798 2022-11-16 14:15:40.000000 solo_epd_loader-0.2.0/solo_epd_loader/__init__ (STEP UPDATE).py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    44704 2023-04-20 12:40:04.000000 solo_epd_loader-0.2.0/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 12:50:56.824914 solo_epd_loader-0.2.0/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.0/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-04-20 12:50:56.000000 solo_epd_loader-0.2.0/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 12:50:56.824914 solo_epd_loader-0.2.0/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15865 2023-04-20 12:50:56.000000 solo_epd_loader-0.2.0/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      653 2023-04-20 12:50:56.000000 solo_epd_loader-0.2.0/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-04-20 12:50:56.000000 solo_epd_loader-0.2.0/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.0/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      188 2023-04-20 12:50:56.000000 solo_epd_loader-0.2.0/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-04-20 12:50:56.000000 solo_epd_loader-0.2.0/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.0/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 13:34:16.025219 solo_epd_loader-0.2.1/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.1/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.1/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16777 2023-04-20 13:34:16.025219 solo_epd_loader-0.2.1/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15829 2023-04-20 13:32:52.000000 solo_epd_loader-0.2.1/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.1/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 13:34:16.021219 solo_epd_loader-0.2.1/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.1/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.1/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.1/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.1/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 13:34:16.021219 solo_epd_loader-0.2.1/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.1/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.1/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.1/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.1/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 13:34:16.021219 solo_epd_loader-0.2.1/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.1/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.1/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.1/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2302 2023-04-20 13:34:16.025219 solo_epd_loader-0.2.1/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.1/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 13:34:16.025219 solo_epd_loader-0.2.1/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    37798 2022-11-16 14:15:40.000000 solo_epd_loader-0.2.1/solo_epd_loader/__init__ (STEP UPDATE).py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    44704 2023-04-20 12:40:04.000000 solo_epd_loader-0.2.1/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 13:34:16.025219 solo_epd_loader-0.2.1/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.1/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-04-20 13:34:15.000000 solo_epd_loader-0.2.1/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 13:34:16.025219 solo_epd_loader-0.2.1/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16777 2023-04-20 13:34:15.000000 solo_epd_loader-0.2.1/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      653 2023-04-20 13:34:16.000000 solo_epd_loader-0.2.1/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-04-20 13:34:15.000000 solo_epd_loader-0.2.1/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.1/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      188 2023-04-20 13:34:15.000000 solo_epd_loader-0.2.1/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-04-20 13:34:15.000000 solo_epd_loader-0.2.1/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.1/tox.ini
```

### Comparing `solo_epd_loader-0.2.0/LICENSE.rst` & `solo_epd_loader-0.2.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/PKG-INFO` & `solo_epd_loader-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo_epd_loader
-Version: 0.2.0
+Version: 0.2.1
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -44,15 +44,15 @@
 - High Energy Telescope (HET)
 - SupraThermal Electrons and Protons (STEP)
 
 Current caveats:
 
 - Only the standard ``rates`` data products are supported (i.e., no ``burst`` or ``high cadence`` data).
 - Only electrons, protons and alpha particles are processed (i.e., for HET He3, He4, C, N, O, Fe are omitted at the moment).
-- For STEP, the sectored data is not yet available, and data is only available until Oct 2021 due to the change of the data product (will be updated soon).
+- For the old STEP data product (until Oct 22, 2021), the sectored data is not processed (i.e., only averaged data is supported) and electron data needs to be calculated manually.
 - The Suprathermal Ion Spectrograph (SIS) is not yet included. 
 
 Disclaimer
 ----------
 This software is provided "as is", with no guarantee. It is no official data source, and not officially endorsed by the corresponding instrument teams. **Please always refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
 
 Installation
@@ -120,14 +120,26 @@
       MeV)’
    2. Dictionary with energy information for all particles:
 
       -  String with energy channel info
       -  Value of lower energy bin edge in MeV
       -  Value of energy bin width in MeV
 
+SupraThermal Electron Proton (STEP) sensor electron measurements
+----------------------------------------------------------------
+
+Please note that the STEP electron measurements are not directly provided in the publically released data, but need to be calculated from them. This process is not straightforward, and the resulting data is prone to uncertainties (like contamination). **Thus it should only be used scientifically with caution! Please refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
+
+The ``contamination_threshold`` option can be used when calling ``epd_load()`` to mask STEP electron data that probably is contaminated (i.e., it is set to nan) following the equation:
+
+   Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty
+
+The default setting is ``contamination_threshold=2``.
+
+
 Data folder structure
 ---------------------
 
 The ``path`` variable provided to the module should be the base
 directory where the corresponding cdf data files should be placed in
 subdirectories. First subfolder defines the data product ``level``
 (``l2`` or ``low_latency`` at the moment), the next one the
```

### Comparing `solo_epd_loader-0.2.0/README.rst` & `solo_epd_loader-0.2.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 - High Energy Telescope (HET)
 - SupraThermal Electrons and Protons (STEP)
 
 Current caveats:
 
 - Only the standard ``rates`` data products are supported (i.e., no ``burst`` or ``high cadence`` data).
 - Only electrons, protons and alpha particles are processed (i.e., for HET He3, He4, C, N, O, Fe are omitted at the moment).
-- For STEP, the sectored data is not yet available, and data is only available until Oct 2021 due to the change of the data product (will be updated soon).
+- For the old STEP data product (until Oct 22, 2021), the sectored data is not processed (i.e., only averaged data is supported) and electron data needs to be calculated manually.
 - The Suprathermal Ion Spectrograph (SIS) is not yet included. 
 
 Disclaimer
 ----------
 This software is provided "as is", with no guarantee. It is no official data source, and not officially endorsed by the corresponding instrument teams. **Please always refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
 
 Installation
@@ -95,14 +95,26 @@
       MeV)’
    2. Dictionary with energy information for all particles:
 
       -  String with energy channel info
       -  Value of lower energy bin edge in MeV
       -  Value of energy bin width in MeV
 
+SupraThermal Electron Proton (STEP) sensor electron measurements
+----------------------------------------------------------------
+
+Please note that the STEP electron measurements are not directly provided in the publically released data, but need to be calculated from them. This process is not straightforward, and the resulting data is prone to uncertainties (like contamination). **Thus it should only be used scientifically with caution! Please refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
+
+The ``contamination_threshold`` option can be used when calling ``epd_load()`` to mask STEP electron data that probably is contaminated (i.e., it is set to nan) following the equation:
+
+   Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty
+
+The default setting is ``contamination_threshold=2``.
+
+
 Data folder structure
 ---------------------
 
 The ``path`` variable provided to the module should be the base
 directory where the corresponding cdf data files should be placed in
 subdirectories. First subfolder defines the data product ``level``
 (``l2`` or ``low_latency`` at the moment), the next one the
```

### Comparing `solo_epd_loader-0.2.0/code_of_conduct.md` & `solo_epd_loader-0.2.1/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/docs/Makefile` & `solo_epd_loader-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/docs/conf.py` & `solo_epd_loader-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/docs/make.bat` & `solo_epd_loader-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/examples/gh2021_fig_2.png` & `solo_epd_loader-0.2.1/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.2.1/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/gh2021_fig_2.png` & `solo_epd_loader-0.2.1/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/gh2021_fig_2a.png` & `solo_epd_loader-0.2.1/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/licenses/LICENSE.rst` & `solo_epd_loader-0.2.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.2.1/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/setup.cfg` & `solo_epd_loader-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/setup.py` & `solo_epd_loader-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/solo_epd_loader/__init__ (STEP UPDATE).py` & `solo_epd_loader-0.2.1/solo_epd_loader/__init__ (STEP UPDATE).py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/solo_epd_loader/__init__.py` & `solo_epd_loader-0.2.1/solo_epd_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.2.1/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo-epd-loader
-Version: 0.2.0
+Version: 0.2.1
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -44,15 +44,15 @@
 - High Energy Telescope (HET)
 - SupraThermal Electrons and Protons (STEP)
 
 Current caveats:
 
 - Only the standard ``rates`` data products are supported (i.e., no ``burst`` or ``high cadence`` data).
 - Only electrons, protons and alpha particles are processed (i.e., for HET He3, He4, C, N, O, Fe are omitted at the moment).
-- For STEP, the sectored data is not yet available, and data is only available until Oct 2021 due to the change of the data product (will be updated soon).
+- For the old STEP data product (until Oct 22, 2021), the sectored data is not processed (i.e., only averaged data is supported) and electron data needs to be calculated manually.
 - The Suprathermal Ion Spectrograph (SIS) is not yet included. 
 
 Disclaimer
 ----------
 This software is provided "as is", with no guarantee. It is no official data source, and not officially endorsed by the corresponding instrument teams. **Please always refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
 
 Installation
@@ -120,14 +120,26 @@
       MeV)’
    2. Dictionary with energy information for all particles:
 
       -  String with energy channel info
       -  Value of lower energy bin edge in MeV
       -  Value of energy bin width in MeV
 
+SupraThermal Electron Proton (STEP) sensor electron measurements
+----------------------------------------------------------------
+
+Please note that the STEP electron measurements are not directly provided in the publically released data, but need to be calculated from them. This process is not straightforward, and the resulting data is prone to uncertainties (like contamination). **Thus it should only be used scientifically with caution! Please refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
+
+The ``contamination_threshold`` option can be used when calling ``epd_load()`` to mask STEP electron data that probably is contaminated (i.e., it is set to nan) following the equation:
+
+   Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty
+
+The default setting is ``contamination_threshold=2``.
+
+
 Data folder structure
 ---------------------
 
 The ``path`` variable provided to the module should be the base
 directory where the corresponding cdf data files should be placed in
 subdirectories. First subfolder defines the data product ``level``
 (``l2`` or ``low_latency`` at the moment), the next one the
```

### Comparing `solo_epd_loader-0.2.0/solo_epd_loader.egg-info/SOURCES.txt` & `solo_epd_loader-0.2.1/solo_epd_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.0/tox.ini` & `solo_epd_loader-0.2.1/tox.ini`

 * *Files identical despite different names*

