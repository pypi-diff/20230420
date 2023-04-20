# Comparing `tmp/proteinflow-1.2.8.tar.gz` & `tmp/proteinflow-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-1.2.8.tar", last modified: Mon Apr 17 12:02:39 2023, max compression
+gzip compressed data, was "proteinflow-1.2.9.tar", last modified: Mon Apr 17 15:36:40 2023, max compression
```

## Comparing `proteinflow-1.2.8.tar` & `proteinflow-1.2.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:39.255886 proteinflow-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-17 12:02:27.000000 proteinflow-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-04-17 12:02:39.255886 proteinflow-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-17 12:02:27.000000 proteinflow-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:39.255886 proteinflow-1.2.8/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)    75424 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:39.255886 proteinflow-1.2.8/proteinflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/scripts/proteinflow_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:39.255886 proteinflow-1.2.8/proteinflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/async_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/biotite_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/build_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    34257 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/cluster_and_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/filter_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/mmcif_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)    14143 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/process_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-17 12:02:27.000000 proteinflow-1.2.8/proteinflow/utils/split_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:39.255886 proteinflow-1.2.8/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-04-17 12:02:39.000000 proteinflow-1.2.8/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-17 12:02:39.000000 proteinflow-1.2.8/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:02:39.000000 proteinflow-1.2.8/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 12:02:39.000000 proteinflow-1.2.8/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-17 12:02:39.000000 proteinflow-1.2.8/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 12:02:39.000000 proteinflow-1.2.8/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-17 12:02:27.000000 proteinflow-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 12:02:39.255886 proteinflow-1.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:02:39.255886 proteinflow-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-17 12:02:27.000000 proteinflow-1.2.8/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-17 12:02:27.000000 proteinflow-1.2.8/tests/test_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:40.683986 proteinflow-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-17 15:36:28.000000 proteinflow-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-04-17 15:36:40.683986 proteinflow-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-04-17 15:36:28.000000 proteinflow-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:40.679986 proteinflow-1.2.9/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    75424 2023-04-17 15:36:28.000000 proteinflow-1.2.9/proteinflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:40.679986 proteinflow-1.2.9/proteinflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:28.000000 proteinflow-1.2.9/proteinflow/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-17 15:36:28.000000 proteinflow-1.2.9/proteinflow/scripts/proteinflow_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:40.679986 proteinflow-1.2.9/proteinflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:28.000000 proteinflow-1.2.9/proteinflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-17 15:36:28.000000 proteinflow-1.2.9/proteinflow/utils/async_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-17 15:36:28.000000 proteinflow-1.2.9/proteinflow/utils/biotite_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-04-17 15:36:28.000000 proteinflow-1.2.9/proteinflow/utils/build_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34257 2023-04-17 15:36:28.000000 proteinflow-1.2.9/proteinflow/utils/cluster_and_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-17 15:36:28.000000 proteinflow-1.2.9/proteinflow/utils/filter_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-17 15:36:28.000000 proteinflow-1.2.9/proteinflow/utils/mmcif_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14143 2023-04-17 15:36:28.000000 proteinflow-1.2.9/proteinflow/utils/process_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-17 15:36:28.000000 proteinflow-1.2.9/proteinflow/utils/split_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:40.679986 proteinflow-1.2.9/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-04-17 15:36:40.000000 proteinflow-1.2.9/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-17 15:36:40.000000 proteinflow-1.2.9/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:36:40.000000 proteinflow-1.2.9/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 15:36:40.000000 proteinflow-1.2.9/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-17 15:36:40.000000 proteinflow-1.2.9/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 15:36:40.000000 proteinflow-1.2.9/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-17 15:36:28.000000 proteinflow-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:36:40.683986 proteinflow-1.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:40.683986 proteinflow-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-17 15:36:28.000000 proteinflow-1.2.9/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-17 15:36:28.000000 proteinflow-1.2.9/tests/test_generate.py
```

### Comparing `proteinflow-1.2.8/LICENSE` & `proteinflow-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.8/PKG-INFO` & `proteinflow-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.2.8
+Version: 1.2.9
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Elizaveta Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,14 +27,16 @@
 Recommended: create a new `conda` environment and install `proteinflow` with `pip`. 
 ```bash
 conda create --name proteinflow -y
 conda activate proteinflow
 python -m pip install proteinflow
 ```
 
+If you are using `python 3.10` and encountering installation problems, try running `python -m pip install prody==2.4.0` before installing `proteinflow`.
+
 ### Additional requirements
 In most cases, running the commands is enough. However, if you are planning to generate a new dataset, there is a couple additional requirements.
 
 First, you will need to install `mmseqs`. The recommended way is to run the following command in your `conda` environment but there are alternative methods you can see [here](https://github.com/soedinglab/MMseqs2).
 ```bash
 conda install -y -c conda-forge -c bioconda mmseqs2
 ```
```

### Comparing `proteinflow-1.2.8/README.md` & `proteinflow-1.2.9/proteinflow.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: proteinflow
+Version: 1.2.9
+Summary: Versatile pipeline for processing protein structure data for deep learning applications.
+Author-email: Elizaveta Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
+License: BSD-3-Clause
+Keywords: bioinformatics,dataset,protein,PDB,deep learning
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ProteinFlow
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/project/proteinflow/)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/tags)
 ![Generic badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)
@@ -16,14 +27,16 @@
 Recommended: create a new `conda` environment and install `proteinflow` with `pip`. 
 ```bash
 conda create --name proteinflow -y
 conda activate proteinflow
 python -m pip install proteinflow
 ```
 
+If you are using `python 3.10` and encountering installation problems, try running `python -m pip install prody==2.4.0` before installing `proteinflow`.
+
 ### Additional requirements
 In most cases, running the commands is enough. However, if you are planning to generate a new dataset, there is a couple additional requirements.
 
 First, you will need to install `mmseqs`. The recommended way is to run the following command in your `conda` environment but there are alternative methods you can see [here](https://github.com/soedinglab/MMseqs2).
 ```bash
 conda install -y -c conda-forge -c bioconda mmseqs2
 ```
```

### Comparing `proteinflow-1.2.8/proteinflow/__init__.py` & `proteinflow-1.2.9/proteinflow/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.8/proteinflow/scripts/proteinflow_cli.py` & `proteinflow-1.2.9/proteinflow/scripts/proteinflow_cli.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.8/proteinflow/utils/async_download.py` & `proteinflow-1.2.9/proteinflow/utils/async_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.8/proteinflow/utils/biotite_sse.py` & `proteinflow-1.2.9/proteinflow/utils/biotite_sse.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.8/proteinflow/utils/build_pdb.py` & `proteinflow-1.2.9/proteinflow/utils/build_pdb.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.8/proteinflow/utils/cluster_and_partition.py` & `proteinflow-1.2.9/proteinflow/utils/cluster_and_partition.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.8/proteinflow/utils/filter_database.py` & `proteinflow-1.2.9/proteinflow/utils/filter_database.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.8/proteinflow/utils/mmcif_fix.py` & `proteinflow-1.2.9/proteinflow/utils/mmcif_fix.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.8/proteinflow/utils/process_pdb.py` & `proteinflow-1.2.9/proteinflow/utils/process_pdb.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.8/proteinflow/utils/split_dataset.py` & `proteinflow-1.2.9/proteinflow/utils/split_dataset.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.8/proteinflow.egg-info/PKG-INFO` & `proteinflow-1.2.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: proteinflow
-Version: 1.2.8
-Summary: Versatile pipeline for processing protein structure data for deep learning applications.
-Author-email: Elizaveta Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
-License: BSD-3-Clause
-Keywords: bioinformatics,dataset,protein,PDB,deep learning
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ProteinFlow
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/project/proteinflow/)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/tags)
 ![Generic badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)
@@ -27,14 +16,16 @@
 Recommended: create a new `conda` environment and install `proteinflow` with `pip`. 
 ```bash
 conda create --name proteinflow -y
 conda activate proteinflow
 python -m pip install proteinflow
 ```
 
+If you are using `python 3.10` and encountering installation problems, try running `python -m pip install prody==2.4.0` before installing `proteinflow`.
+
 ### Additional requirements
 In most cases, running the commands is enough. However, if you are planning to generate a new dataset, there is a couple additional requirements.
 
 First, you will need to install `mmseqs`. The recommended way is to run the following command in your `conda` environment but there are alternative methods you can see [here](https://github.com/soedinglab/MMseqs2).
 ```bash
 conda install -y -c conda-forge -c bioconda mmseqs2
 ```
```

### Comparing `proteinflow-1.2.8/proteinflow.egg-info/SOURCES.txt` & `proteinflow-1.2.9/proteinflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.8/pyproject.toml` & `proteinflow-1.2.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "1.2.8"
+version = "1.2.9"
 authors = [
     {name = "Elizaveta Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -24,15 +24,14 @@
     "networkx==2.8.8",
     "einops>=0.6.0",
     "pandas>=1.5.2",
     "torch>=1.10.0",
     "biotite==0.35.0",
     "aiobotocore==2.4.2",
     "awscli==1.25.60",
-    "prody>=2.4",
     "rcsbsearch",
     "sidechainnet",
 ]
 keywords = ["bioinformatics", "dataset", "protein", "PDB", "deep learning"]
 
 [project.scripts]
 proteinflow = "proteinflow.scripts.proteinflow_cli:cli"
```

### Comparing `proteinflow-1.2.8/tests/test_download.py` & `proteinflow-1.2.9/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.2.8/tests/test_generate.py` & `proteinflow-1.2.9/tests/test_generate.py`

 * *Files identical despite different names*

