# Comparing `tmp/solo_epd_loader-0.1.8.tar.gz` & `tmp/solo_epd_loader-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solo_epd_loader-0.1.8.tar", last modified: Wed Mar 30 13:44:17 2022, max compression
+gzip compressed data, was "solo_epd_loader-0.2.0.tar", last modified: Thu Apr 20 12:50:56 2023, max compression
```

## Comparing `solo_epd_loader-0.1.8.tar` & `solo_epd_loader-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2022-03-30 13:44:17.412502 solo_epd_loader-0.1.8/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.1.8/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.1.8/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15474 2022-03-30 13:44:17.412502 solo_epd_loader-0.1.8/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    14506 2022-03-29 15:30:34.000000 solo_epd_loader-0.1.8/README.rst
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2022-03-30 13:44:17.408501 solo_epd_loader-0.1.8/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.1.8/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.1.8/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.1.8/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.1.8/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2022-03-30 13:44:17.408501 solo_epd_loader-0.1.8/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.1.8/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.1.8/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.1.8/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.1.8/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2022-03-30 13:44:17.412502 solo_epd_loader-0.1.8/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.1.8/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.1.8/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.1.8/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2205 2022-03-30 13:44:17.412502 solo_epd_loader-0.1.8/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.1.8/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2022-03-30 13:44:17.412502 solo_epd_loader-0.1.8/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    36335 2022-03-30 13:35:34.000000 solo_epd_loader-0.1.8/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2022-03-30 13:44:17.412502 solo_epd_loader-0.1.8/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.1.8/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2022-03-30 13:44:16.000000 solo_epd_loader-0.1.8/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2022-03-30 13:44:17.412502 solo_epd_loader-0.1.8/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15474 2022-03-30 13:44:16.000000 solo_epd_loader-0.1.8/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      592 2022-03-30 13:44:17.000000 solo_epd_loader-0.1.8/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-03-30 13:44:16.000000 solo_epd_loader-0.1.8/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.1.8/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      153 2022-03-30 13:44:17.000000 solo_epd_loader-0.1.8/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2022-03-30 13:44:17.000000 solo_epd_loader-0.1.8/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1304 2022-03-14 11:22:31.000000 solo_epd_loader-0.1.8/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 12:50:56.824914 solo_epd_loader-0.2.0/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.0/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.0/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15865 2023-04-20 12:50:56.824914 solo_epd_loader-0.2.0/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    14917 2022-09-21 10:27:58.000000 solo_epd_loader-0.2.0/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.0/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 12:50:56.808914 solo_epd_loader-0.2.0/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.0/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.0/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.0/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.0/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 12:50:56.812914 solo_epd_loader-0.2.0/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.0/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.0/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.0/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.0/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 12:50:56.816913 solo_epd_loader-0.2.0/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.0/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.0/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.0/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2302 2023-04-20 12:50:56.828914 solo_epd_loader-0.2.0/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.0/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 12:50:56.816913 solo_epd_loader-0.2.0/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    37798 2022-11-16 14:15:40.000000 solo_epd_loader-0.2.0/solo_epd_loader/__init__ (STEP UPDATE).py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    44704 2023-04-20 12:40:04.000000 solo_epd_loader-0.2.0/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 12:50:56.824914 solo_epd_loader-0.2.0/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.0/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-04-20 12:50:56.000000 solo_epd_loader-0.2.0/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-04-20 12:50:56.824914 solo_epd_loader-0.2.0/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15865 2023-04-20 12:50:56.000000 solo_epd_loader-0.2.0/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      653 2023-04-20 12:50:56.000000 solo_epd_loader-0.2.0/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-04-20 12:50:56.000000 solo_epd_loader-0.2.0/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.0/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      188 2023-04-20 12:50:56.000000 solo_epd_loader-0.2.0/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-04-20 12:50:56.000000 solo_epd_loader-0.2.0/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.0/tox.ini
```

### Comparing `solo_epd_loader-0.1.8/LICENSE.rst` & `solo_epd_loader-0.2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.1.8/PKG-INFO` & `solo_epd_loader-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: solo_epd_loader
-Version: 0.1.8
+Version: 0.2.0
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -23,38 +22,42 @@
 Provides-Extra: test
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
 solo-epd-loader
 ===============
 
-|pypi Version| |conda version| |license| |python version|
+|pypi Version| |conda version| |license| |python version| |zenodo doi|
 
 .. |pypi Version| image:: https://img.shields.io/pypi/v/solo-epd-loader?style=flat&logo=pypi
    :target: https://pypi.org/project/solo-epd-loader/
 .. |conda version| image:: https://img.shields.io/conda/vn/conda-forge/solo-epd-loader?style=flat&logo=anaconda
    :target: https://anaconda.org/conda-forge/solo-epd-loader/
 .. |license| image:: https://img.shields.io/conda/l/conda-forge/solo-epd-loader?style=flat
    :target: https://github.com/jgieseler/solo-epd-loader/blob/main/LICENSE.rst
 .. |python version| image:: https://img.shields.io/pypi/pyversions/solo-epd-loader?style=flat&logo=python
+.. |zenodo doi| image:: https://zenodo.org/badge/446889843.svg
+   :target: https://zenodo.org/badge/latestdoi/446889843
 
 Python data loader for Solar Orbiter's (SolO) `Energetic Particle Detector (EPD) <http://espada.uah.es/epd/>`_. At the moment provides level 2 (l2) and low latency (ll) data (`more details on data levels here <http://espada.uah.es/epd/EPD_data_overview.php>`_) obtained through CDF files from ESA's `Solar Orbiter Archive (SOAR) <http://soar.esac.esa.int/soar>`_ for the following sensors:
 
 - Electron Proton Telescope (EPT)
 - High Energy Telescope (HET)
 - SupraThermal Electrons and Protons (STEP)
 
 Current caveats:
 
 - Only the standard ``rates`` data products are supported (i.e., no ``burst`` or ``high cadence`` data).
 - Only electrons, protons and alpha particles are processed (i.e., for HET He3, He4, C, N, O, Fe are omitted at the moment).
-- For STEP, the sectored data is not yet available.
+- For STEP, the sectored data is not yet available, and data is only available until Oct 2021 due to the change of the data product (will be updated soon).
 - The Suprathermal Ion Spectrograph (SIS) is not yet included. 
 
-**Please always refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
+Disclaimer
+----------
+This software is provided "as is", with no guarantee. It is no official data source, and not officially endorsed by the corresponding instrument teams. **Please always refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
 
 Installation
 ------------
 
 solo_epd_loader requires python >= 3.6.
 
 It can be installed either from `PyPI <https://pypi.org/project/solo-epd-loader/>`_ using:
@@ -361,9 +364,7 @@
 which is licensed under the BSD 3-clause license. See the licenses folder for
 more information.
 
 Acknowledgements
 ----------------
 
 The development of this software has received funding from the European Union's Horizon 2020 research and innovation programme under grant agreement No 101004159 (SERPENTINE).
-
-
```

### Comparing `solo_epd_loader-0.1.8/README.rst` & `solo_epd_loader-0.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 solo-epd-loader
 ===============
 
-|pypi Version| |conda version| |license| |python version|
+|pypi Version| |conda version| |license| |python version| |zenodo doi|
 
 .. |pypi Version| image:: https://img.shields.io/pypi/v/solo-epd-loader?style=flat&logo=pypi
    :target: https://pypi.org/project/solo-epd-loader/
 .. |conda version| image:: https://img.shields.io/conda/vn/conda-forge/solo-epd-loader?style=flat&logo=anaconda
    :target: https://anaconda.org/conda-forge/solo-epd-loader/
 .. |license| image:: https://img.shields.io/conda/l/conda-forge/solo-epd-loader?style=flat
    :target: https://github.com/jgieseler/solo-epd-loader/blob/main/LICENSE.rst
 .. |python version| image:: https://img.shields.io/pypi/pyversions/solo-epd-loader?style=flat&logo=python
+.. |zenodo doi| image:: https://zenodo.org/badge/446889843.svg
+   :target: https://zenodo.org/badge/latestdoi/446889843
 
 Python data loader for Solar Orbiter's (SolO) `Energetic Particle Detector (EPD) <http://espada.uah.es/epd/>`_. At the moment provides level 2 (l2) and low latency (ll) data (`more details on data levels here <http://espada.uah.es/epd/EPD_data_overview.php>`_) obtained through CDF files from ESA's `Solar Orbiter Archive (SOAR) <http://soar.esac.esa.int/soar>`_ for the following sensors:
 
 - Electron Proton Telescope (EPT)
 - High Energy Telescope (HET)
 - SupraThermal Electrons and Protons (STEP)
 
 Current caveats:
 
 - Only the standard ``rates`` data products are supported (i.e., no ``burst`` or ``high cadence`` data).
 - Only electrons, protons and alpha particles are processed (i.e., for HET He3, He4, C, N, O, Fe are omitted at the moment).
-- For STEP, the sectored data is not yet available.
+- For STEP, the sectored data is not yet available, and data is only available until Oct 2021 due to the change of the data product (will be updated soon).
 - The Suprathermal Ion Spectrograph (SIS) is not yet included. 
 
-**Please always refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
+Disclaimer
+----------
+This software is provided "as is", with no guarantee. It is no official data source, and not officially endorsed by the corresponding instrument teams. **Please always refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
 
 Installation
 ------------
 
 solo_epd_loader requires python >= 3.6.
 
 It can be installed either from `PyPI <https://pypi.org/project/solo-epd-loader/>`_ using:
```

### Comparing `solo_epd_loader-0.1.8/docs/Makefile` & `solo_epd_loader-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.1.8/docs/conf.py` & `solo_epd_loader-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.1.8/docs/make.bat` & `solo_epd_loader-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.1.8/examples/gh2021_fig_2.png` & `solo_epd_loader-0.2.0/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.1.8/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.2.0/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.1.8/gh2021_fig_2.png` & `solo_epd_loader-0.2.0/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.1.8/gh2021_fig_2a.png` & `solo_epd_loader-0.2.0/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.1.8/licenses/LICENSE.rst` & `solo_epd_loader-0.2.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.1.8/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.2.0/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.1.8/setup.cfg` & `solo_epd_loader-0.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -23,23 +23,28 @@
 [options]
 zip_safe = False
 packages = find:
 include_package_data = True
 python_requires = >=3.6
 setup_requires = setuptools_scm
 install_requires = 
+	astropy
+	bs4
 	cdflib
+	datetime
+	drms
 	h5netcdf
+	lxml
 	matplotlib
 	numpy
 	pandas
 	requests
-	astropy
+	sunpy>=4.1.0
 	tqdm
-	sunpy
+	zeep
 
 [options.extras_require]
 all = 
 test = 
 	pytest
 	pytest-doctestplus
 	pytest-cov
@@ -48,14 +53,19 @@
 	sphinx-automodapi
 
 [tool:pytest]
 testpaths = "solo_epd_loader" "docs"
 doctest_plus = enabled
 text_file_format = rst
 addopts = --doctest-rst
+python_files = 
+	test_*.py
+	*_test.py
+	test.py
+	tests.py
 
 [coverage:run]
 omit = 
 	solo_epd_loader/__init*
 	solo_epd_loader/conftest.py
 	solo_epd_loader/*setup_package*
 	solo_epd_loader/tests/*
```

### Comparing `solo_epd_loader-0.1.8/setup.py` & `solo_epd_loader-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.1.8/solo_epd_loader/__init__.py` & `solo_epd_loader-0.2.0/solo_epd_loader/__init__ (STEP UPDATE).py`

 * *Files 4% similar despite different names*

```diff
@@ -207,18 +207,23 @@
     if level == 'll':
         l_str = 'LL02'
         t_str = 'T??????-????????T??????'
     if level == 'l2':
         l_str = 'L2'
         t_str = ''
 
+    if startdate <= 20211022:
+        product = 'rates'
+    if startdate > 20211022:
+        product = 'main'
+
     filelist = []
     for i in range(startdate, enddate+1):
         filelist = filelist + \
-            glob.glob(path+'solo_'+l_str+'_epd-'+sensor+'-rates_' +
+            glob.glob(path+'solo_'+l_str+'_epd-'+sensor+'-'+product+'_' +
                       str(i) + t_str + '_V*.cdf')
 
     if filenames_only:
         filelist = [os.path.basename(x) for x in filelist]
 
     return filelist
 
@@ -286,18 +291,22 @@
                         'step')
     """
 
     # try loading tqdm for download progress display
     tqdm_available, download_url = _load_tqdm(verbose=True)
 
     if sensor.lower() == 'step':
+        if date <= 20211022:
+            product = 'rates'
+        if date > 20211022:
+            product = 'main'
         url = 'http://soar.esac.esa.int/soar-sl-tap/data?' + \
-            'retrieval_type=LAST_PRODUCT&data_item_id=solo_L2_epd-' + \
-            sensor.lower()+'-rates_'+str(date) + \
-            '&product_type=SCIENCE'
+              'retrieval_type=LAST_PRODUCT&data_item_id=solo_L2_epd-' + \
+              sensor.lower()+'-'+product+'_'+str(date) + \
+              '&product_type=SCIENCE'
     else:
         url = 'http://soar.esac.esa.int/soar-sl-tap/data?' + \
             'retrieval_type=LAST_PRODUCT&data_item_id=solo_L2_epd-' + \
             sensor.lower()+'-'+viewing.lower()+'-rates_'+str(date) + \
             '&product_type=SCIENCE'
 
     # Get filename from url
@@ -384,16 +393,20 @@
     # only use data level wanted; i.e., 'LL' or 'L2'
     df = df[df['processing_level'] == p_level]
 
     # list filenames for given telescope (e.g., 'HET')
     # filelist = df['filename'][df['sensor'] == sensor.upper()].sort_values()
     filelist = [s for s in df['file_name'].values if sensor.lower() in s]
 
-    # list filenames for 'rates' type (i.e., remove 'hcad')
-    filelist = [s for s in filelist if "rates" in s]
+    if sensor.lower() == 'step' and startdate > 20211022:
+        # list filenames for 'main' type (i.e., remove 'hcad')
+        filelist = [s for s in filelist if "main" in s]
+    else:
+        # list filenames for 'rates' type (i.e., remove 'hcad')
+        filelist = [s for s in filelist if "rates" in s]
 
     # filelist.sort()
     if len(filelist) == 0:
         print('No corresponding data found at SOAR!')
     return filelist
 
 
@@ -444,17 +457,17 @@
         e.g. 20210415
     enddate : (datetime or int), optional
         Provides end date. Either a datetime object (e.g., dt.date(2021,12,31)
         or dt.datetime(2021,4,15)). Or a combined integer yyyymmdd with year
         (yyyy), month (mm) and day (dd) with empty positions filled with zeros,
         e.g. 20210415
         (if no enddate is given, 'enddate = startdate' will be set)
-    viewing : {'sun', 'asun', 'north', 'south' or None}, optional
-        Viewing direction of sensor. Needed for 'ept' or 'het'; for 'step'
-        shoule be None. By default None
+    viewing : {'sun', 'asun', 'north', 'south', 'omni' or None}, optional
+        Viewing direction of sensor (omni equals mean of four viewing directions).
+        Needed for 'ept' or 'het'; for 'step' shoule be None. By default None
     path : str, optional
         User-specified directory in which Solar Orbiter data is/should be
         organized; e.g. '/home/userxyz/solo/data/', by default None
     autodownload : bool, optional
         If True, will try to download missing data files from SOAR, by default
         False.
 
@@ -519,14 +532,19 @@
     if sensor.lower() == 'ept' or sensor.lower() == 'het':
         if viewing is None:
             raise Exception("EPT and HET need a telescope 'viewing' " +
                             "direction! No data read!")
             df_epd_p = []
             df_epd_e = []
             energies_dict = []
+        elif viewing == 'omni':
+            for view in ['sun', 'asun', 'north', 'south']:
+                exec(f"df_epd_p_{view}, df_epd_e{view}, energies_dict = \
+                     _read_epd_cdf(sensor, view, level, startdate, enddate, path, autodownload)")
+                exec(f"ept_e_{view} = ept_e_{view}.add_prefix('{view}_'.capitalize())")
         else:
             df_epd_p, df_epd_e, energies_dict = \
                 _read_epd_cdf(sensor, viewing, level, startdate, enddate, path,
                               autodownload)
         return df_epd_p, df_epd_e, energies_dict
 
 
@@ -580,16 +598,15 @@
     filelist = _get_epd_filelist(sensor.lower(), level.lower(), startdate,
                                  enddate, path=path)[viewing.lower()]
 
     # check for duplicate files with different version numbers and remove them
     filelist = _check_duplicates(filelist, verbose=True)
 
     if len(filelist) == 0:
-        raise Exception('WARNING: No corresponding data files found! ' +
-                        'Try different settings, path or autodownload.')
+        warnings.warn('WARNING: No corresponding data files found! Try different settings, path or autodownload.')
         df_epd_p = []
         df_epd_e = []
         energies_dict = []
     else:
 
         """ <-- get column names of dataframe """
         if sensor.lower() == 'ept':
@@ -754,16 +771,16 @@
 
         # manual replace FILLVALUES in dataframes with np.nan
         # t_cdf_file.varattsget("Ion_Flux")["FILLVAL"][0] = -1e+31
         # same for l2 & ll and het & ept and e, p/ion, alpha
         # remove this (i.e. following two lines) when sunpy's read_cdf is updated,
         # and FILLVAL will be replaced directly, see
         # https://github.com/sunpy/sunpy/issues/5908
-        df_epd_p = df_epd_p.replace(-1e+31, np.nan)
-        df_epd_e = df_epd_e.replace(-1e+31, np.nan)
+        df_epd_p = df_epd_p.replace(np.float32(-1e+31), np.nan)
+        df_epd_e = df_epd_e.replace(np.float32(-1e+31), np.nan)
 
         energies_dict = {protons+"_Bins_Text":
                          t_cdf_file.varget(protons+'_Bins_Text'),
                          protons+"_Bins_Low_Energy":
                          t_cdf_file.varget(protons+'_Bins_Low_Energy'),
                          protons+"_Bins_Width":
                          t_cdf_file.varget(protons+'_Bins_Width'),
@@ -791,16 +808,15 @@
     Careful if adding more species - they might have different EPOCH
     dependencies and cannot easily be put in the same dataframe!
     '''
 
     return df_epd_p, df_epd_e, energies_dict
 
 
-def _read_step_cdf(level, startdate, enddate=None, path=None,
-                   autodownload=False):
+def _read_step_cdf(level, startdate, enddate=None, path=None, autodownload=False):
     """
     INPUT:
         level: 'll' or 'l2' (string)
         startdate,
         enddate:    YYYYMMDD, e.g., 20210415 (integer)
                     (if no enddate is given, 'enddate = startdate' will be set)
         path: directory in which Solar Orbiter data is/should be organized;
@@ -829,91 +845,101 @@
     # add a OS-specific '/' to end end of 'path'
     path = f'{path}{os.sep}'
 
     # if no 'enddate' is given, get data only for single day of 'startdate'
     if enddate is None:
         enddate = startdate
 
-    # if True, check online available files and download if not locally present
-    if autodownload:
-        _autodownload_cdf(startdate, enddate, sensor.lower(), level.lower(),
-                          path)
-
-    # get list of local files for date range
-    filelist = _get_step_filelist(level.lower(), startdate, enddate, path=path)
-
-    # check for duplicate files with different version numbers and remove them
-    filelist = _check_duplicates(filelist, verbose=True)
-
-    if len(filelist) == 0:
-        raise Exception('WARNING: No corresponding data files found! ' +
-                        'Try different settings, path or autodownload.')
+    # check if Oct 22 2021 is within time interval; at that date the data product changed!
+    if startdate <= 20211022:
+        product = 'rates'
+    if startdate > 20211022:
+        product = 'main'
+    if startdate < 20211022 and enddate > 20211022:
+        warnings.warn('WARNING: During the selected time range the STEP data product changed (on Oct 22 2021)! Please adjust time range and run again.')
         datadf = []
         energies_dict = []
     else:
-        all_cdf = []
-        for file in filelist:
-            all_cdf.append(cdflib.CDF(file))
-
-        if level == 'l2':
-            param_list = ['Integral_Flux', 'Magnet_Flux', 'Integral_Rate',
-                          'Magnet_Rate', 'Magnet_Uncertainty',
-                          'Integral_Uncertainty']
-            # set up the dictionary:
-            energies_dict = \
-                {"Bins_Text": all_cdf[0].varget('Bins_Text'),
-                 "Bins_Low_Energy": all_cdf[0].varget('Bins_Low_Energy'),
-                 "Bins_Width": all_cdf[0].varget('Bins_Width'),
-                 "Sector_Bins_Text": all_cdf[0].varget('Sector_Bins_Text'),
-                 "Sector_Bins_Low_Energy": all_cdf[0].varget('Sector_Bins_Low_Energy'),
-                 "Sector_Bins_Width": all_cdf[0].varget('Sector_Bins_Width')
-                 }
-        if level == 'll':
-            param_list = ['Integral_Flux', 'Ion_Flux', 'Integral_Flux_Sigma',
-                          'Ion_Flux_Sigma']
-            # set up the dictionary:
-            energies_dict = \
-                {"Integral_Bins_Text": all_cdf[0].varget('Integral_Bins_Text'),
-                 "Integral_Bins_Low_Energy": all_cdf[0].varget('Integral_Bins_Low_Energy'),
-                 "Integral_Bins_Width": all_cdf[0].varget('Integral_Bins_Width'),
-                 "Ion_Bins_Text": all_cdf[0].varget('Ion_Bins_Text'),
-                 "Ion_Bins_Low_Energy": all_cdf[0].varget('Ion_Bins_Low_Energy'),
-                 "Ion_Bins_Width": all_cdf[0].varget('Ion_Bins_Width')
-                 }
-
-        df_list = []
-        for cdffile in all_cdf:
-            col_list = []
-            for key in param_list:
-                try:
-                    t_df = pd.DataFrame(cdffile[key], index=cdffile['EPOCH'])
 
-                    # Replace FILLVAL dynamically for each element of param_list
-                    fillval = cdffile.varattsget(key)["FILLVAL"]
-                    t_df = t_df.replace(fillval, np.nan)
-
-                    col_list.append(t_df)
-                except TypeError:
-                    print(' ')
-                    print("WARNING: Gap in dataframe due to missing cdf file.")
-                    break
-            try:
-                temp_df = pd.concat(col_list, axis=1, keys=param_list)
-                df_list.append(temp_df)
-            except ValueError:
-                continue
-        datadf = pd.concat(df_list)
-
-        # transform the index of the dataframe into pd_datetime
-        # notice the transform alldata.index -> np.int_ so that encode()
-        # understands the format
-        datetimes = cdflib.cdfepoch.encode(np.int_(datadf.index))
-        datadf.index = pd.to_datetime(datetimes)
-
-        datadf.index.names = ['Time']
-
-    '''
-    Careful if adding more species - they might have different EPOCH
-    dependencies and cannot easily be put in the same dataframe!
-    '''
+        # if True, check online available files and download if not locally present
+        if autodownload:
+            _autodownload_cdf(startdate, enddate, sensor.lower(), level.lower(), path)
+
+        # get list of local files for date range
+        filelist = _get_step_filelist(level.lower(), startdate, enddate, path=path)
+
+        # check for duplicate files with different version numbers and remove them
+        filelist = _check_duplicates(filelist, verbose=True)
+
+        if len(filelist) == 0:
+            warnings.warn('WARNING: No corresponding data files found! Try different settings, path or autodownload.')
+            datadf = []
+            energies_dict = []
+        else:
+            all_cdf = []
+            for file in filelist:
+                all_cdf.append(cdflib.CDF(file))
+
+            # if product == 'rates':
+            # if product = 'main':
+
+            if level == 'l2':
+                param_list = ['Integral_Flux', 'Magnet_Flux', 'Integral_Rate',
+                              'Magnet_Rate', 'Magnet_Uncertainty',
+                              'Integral_Uncertainty']
+                # set up the dictionary:
+                energies_dict = \
+                    {"Bins_Text": all_cdf[0].varget('Bins_Text'),
+                     "Bins_Low_Energy": all_cdf[0].varget('Bins_Low_Energy'),
+                     "Bins_Width": all_cdf[0].varget('Bins_Width'),
+                     "Sector_Bins_Text": all_cdf[0].varget('Sector_Bins_Text'),
+                     "Sector_Bins_Low_Energy": all_cdf[0].varget('Sector_Bins_Low_Energy'),
+                     "Sector_Bins_Width": all_cdf[0].varget('Sector_Bins_Width')
+                     }
+            if level == 'll':
+                param_list = ['Integral_Flux', 'Ion_Flux', 'Integral_Flux_Sigma',
+                              'Ion_Flux_Sigma']
+                # set up the dictionary:
+                energies_dict = \
+                    {"Integral_Bins_Text": all_cdf[0].varget('Integral_Bins_Text'),
+                     "Integral_Bins_Low_Energy": all_cdf[0].varget('Integral_Bins_Low_Energy'),
+                     "Integral_Bins_Width": all_cdf[0].varget('Integral_Bins_Width'),
+                     "Ion_Bins_Text": all_cdf[0].varget('Ion_Bins_Text'),
+                     "Ion_Bins_Low_Energy": all_cdf[0].varget('Ion_Bins_Low_Energy'),
+                     "Ion_Bins_Width": all_cdf[0].varget('Ion_Bins_Width')
+                     }
+
+            df_list = []
+            for cdffile in all_cdf:
+                col_list = []
+                for key in param_list:
+                    try:
+                        t_df = pd.DataFrame(cdffile[key], index=cdffile['EPOCH'])
+
+                        # Replace FILLVAL dynamically for each element of param_list
+                        fillval = cdffile.varattsget(key)["FILLVAL"]
+                        t_df = t_df.replace(fillval, np.nan)
+
+                        col_list.append(t_df)
+                    except TypeError:
+                        print(' ')
+                        print("WARNING: Gap in dataframe due to missing cdf file.")
+                        break
+                try:
+                    temp_df = pd.concat(col_list, axis=1, keys=param_list)
+                    df_list.append(temp_df)
+                except ValueError:
+                    continue
+            datadf = pd.concat(df_list)
+
+            # transform the index of the dataframe into pd_datetime
+            datetimes = cdflib.cdfepoch.encode(datadf.index.values)
+            datadf.index = pd.to_datetime(datetimes)
+
+            datadf.index.names = ['Time']
+
+        '''
+        Careful if adding more species - they might have different EPOCH
+        dependencies and cannot easily be put in the same dataframe!
+        '''
 
     return datadf, energies_dict
```

### Comparing `solo_epd_loader-0.1.8/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.2.0/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: solo-epd-loader
-Version: 0.1.8
+Version: 0.2.0
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -23,38 +22,42 @@
 Provides-Extra: test
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
 solo-epd-loader
 ===============
 
-|pypi Version| |conda version| |license| |python version|
+|pypi Version| |conda version| |license| |python version| |zenodo doi|
 
 .. |pypi Version| image:: https://img.shields.io/pypi/v/solo-epd-loader?style=flat&logo=pypi
    :target: https://pypi.org/project/solo-epd-loader/
 .. |conda version| image:: https://img.shields.io/conda/vn/conda-forge/solo-epd-loader?style=flat&logo=anaconda
    :target: https://anaconda.org/conda-forge/solo-epd-loader/
 .. |license| image:: https://img.shields.io/conda/l/conda-forge/solo-epd-loader?style=flat
    :target: https://github.com/jgieseler/solo-epd-loader/blob/main/LICENSE.rst
 .. |python version| image:: https://img.shields.io/pypi/pyversions/solo-epd-loader?style=flat&logo=python
+.. |zenodo doi| image:: https://zenodo.org/badge/446889843.svg
+   :target: https://zenodo.org/badge/latestdoi/446889843
 
 Python data loader for Solar Orbiter's (SolO) `Energetic Particle Detector (EPD) <http://espada.uah.es/epd/>`_. At the moment provides level 2 (l2) and low latency (ll) data (`more details on data levels here <http://espada.uah.es/epd/EPD_data_overview.php>`_) obtained through CDF files from ESA's `Solar Orbiter Archive (SOAR) <http://soar.esac.esa.int/soar>`_ for the following sensors:
 
 - Electron Proton Telescope (EPT)
 - High Energy Telescope (HET)
 - SupraThermal Electrons and Protons (STEP)
 
 Current caveats:
 
 - Only the standard ``rates`` data products are supported (i.e., no ``burst`` or ``high cadence`` data).
 - Only electrons, protons and alpha particles are processed (i.e., for HET He3, He4, C, N, O, Fe are omitted at the moment).
-- For STEP, the sectored data is not yet available.
+- For STEP, the sectored data is not yet available, and data is only available until Oct 2021 due to the change of the data product (will be updated soon).
 - The Suprathermal Ion Spectrograph (SIS) is not yet included. 
 
-**Please always refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
+Disclaimer
+----------
+This software is provided "as is", with no guarantee. It is no official data source, and not officially endorsed by the corresponding instrument teams. **Please always refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
 
 Installation
 ------------
 
 solo_epd_loader requires python >= 3.6.
 
 It can be installed either from `PyPI <https://pypi.org/project/solo-epd-loader/>`_ using:
@@ -361,9 +364,7 @@
 which is licensed under the BSD 3-clause license. See the licenses folder for
 more information.
 
 Acknowledgements
 ----------------
 
 The development of this software has received funding from the European Union's Horizon 2020 research and innovation programme under grant agreement No 101004159 (SERPENTINE).
-
-
```

### Comparing `solo_epd_loader-0.1.8/solo_epd_loader.egg-info/SOURCES.txt` & `solo_epd_loader-0.2.0/solo_epd_loader.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 LICENSE.rst
 MANIFEST.in
 README.rst
+code_of_conduct.md
 gh2021_fig_2.png
 gh2021_fig_2a.png
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 examples/gh2021_fig_2.png
 examples/ws2021_fig_2d.png
 licenses/LICENSE.rst
 licenses/TEMPLATE_LICENSE.rst
+solo_epd_loader/__init__ (STEP UPDATE).py
 solo_epd_loader/__init__.py
 solo_epd_loader/version.py
 solo_epd_loader.egg-info/PKG-INFO
 solo_epd_loader.egg-info/SOURCES.txt
 solo_epd_loader.egg-info/dependency_links.txt
 solo_epd_loader.egg-info/not-zip-safe
 solo_epd_loader.egg-info/requires.txt
```

### Comparing `solo_epd_loader-0.1.8/tox.ini` & `solo_epd_loader-0.2.0/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 envlist =
-    py{36,37,38}-test
+    py{37,38,39,310}-test
     build_docs
     codestyle
 isolated_build = true
 # This is included for testing of the template. You can remove it safely.
 skip_missing_interpreters = True
 
 [testenv]
```

