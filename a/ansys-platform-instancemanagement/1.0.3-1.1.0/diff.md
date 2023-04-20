# Comparing `tmp/ansys-platform-instancemanagement-1.0.3.tar.gz` & `tmp/ansys-platform-instancemanagement-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-platform-instancemanagement-1.0.3.tar", last modified: Fri Jan 20 16:08:14 2023, max compression
+gzip compressed data, was "ansys-platform-instancemanagement-1.1.0.tar", last modified: Thu Apr 20 10:10:32 2023, max compression
```

## Comparing `ansys-platform-instancemanagement-1.0.3.tar` & `ansys-platform-instancemanagement-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0      233 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/.flake8
--rw-r--r--   0        0        0      516 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/.github/dependabot.yml
--rw-r--r--   0        0        0     2783 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     2999 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/.gitignore
--rw-r--r--   0        0        0      579 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1089 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/LICENSE
--rw-r--r--   0        0        0     5083 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/README.rst
--rwxr-xr-x   0        0        0      753 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/doc/Makefile
--rw-r--r--   0        0        0      970 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/doc/make.bat
--rw-r--r--   0        0        0       22 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/doc/source/CNAME
--rw-r--r--   0        0        0       64 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/doc/source/_static/README.md
--rw-r--r--   0        0        0       50 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/doc/source/_templates/README.md
--rw-r--r--   0        0        0      443 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0       12 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/doc/source/api/.gitignore
--rw-r--r--   0        0        0      592 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/doc/source/api/index.rst
--rwxr-xr-x   0        0        0     2806 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/doc/source/conf.py
--rw-r--r--   0        0        0     2018 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/doc/source/contributing.rst
--rw-r--r--   0        0        0      254 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/doc/source/index.rst
--rw-r--r--   0        0        0     8229 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/doc/source/integration.rst
--rw-r--r--   0        0        0      201 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/protos/README.rst
--rw-r--r--   0        0        0     8485 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/protos/ansys/api/platform/instancemanagement/v1/product_instance_manager.proto
--rw-r--r--   0        0        0     1285 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       24 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/requirements/requirements_build.txt
--rw-r--r--   0        0        0      120 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/requirements/requirements_doc.txt
--rw-r--r--   0        0        0      126 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/requirements/requirements_tests.txt
--rw-r--r--   0        0        0     3259 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/src/ansys/platform/instancemanagement/__init__.py
--rw-r--r--   0        0        0    10229 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/src/ansys/platform/instancemanagement/client.py
--rw-r--r--   0        0        0     4321 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/src/ansys/platform/instancemanagement/definition.py
--rw-r--r--   0        0        0     3574 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/src/ansys/platform/instancemanagement/exceptions.py
--rw-r--r--   0        0        0    10101 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/src/ansys/platform/instancemanagement/instance.py
--rw-r--r--   0        0        0     3157 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/src/ansys/platform/instancemanagement/interceptor.py
--rw-r--r--   0        0        0     2817 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/src/ansys/platform/instancemanagement/service.py
--rw-r--r--   0        0        0     1021 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/tests/conftest.py
--rw-r--r--   0        0        0    16956 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/tests/test_client.py
--rw-r--r--   0        0        0     2561 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/tests/test_definition.py
--rw-r--r--   0        0        0    15439 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/tests/test_instance.py
--rw-r--r--   0        0        0      118 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/tests/test_metadata.py
--rw-r--r--   0        0        0     2424 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/tests/test_service.py
--rw-r--r--   0        0        0     1371 2023-01-20 16:08:03.858656 ansys-platform-instancemanagement-1.0.3/tox.ini
--rw-r--r--   0        0        0     5756 1970-01-01 00:00:00.000000 ansys-platform-instancemanagement-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      233 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/.flake8
+-rw-r--r--   0        0        0      516 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2783 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     3019 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/.gitignore
+-rw-r--r--   0        0        0      579 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1089 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5201 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/README.rst
+-rwxr-xr-x   0        0        0      753 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/Makefile
+-rw-r--r--   0        0        0      970 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/make.bat
+-rw-r--r--   0        0        0       22 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/CNAME
+-rw-r--r--   0        0        0       64 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/_static/README.md
+-rw-r--r--   0        0        0       50 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      451 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0       12 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/api/.gitignore
+-rw-r--r--   0        0        0      592 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/api/index.rst
+-rwxr-xr-x   0        0        0     2806 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/conf.py
+-rw-r--r--   0        0        0     1911 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/contributing.rst
+-rw-r--r--   0        0        0      254 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/index.rst
+-rw-r--r--   0        0        0     8374 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/doc/source/integration.rst
+-rw-r--r--   0        0        0      201 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/protos/README.rst
+-rw-r--r--   0        0        0     8485 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/protos/ansys/api/platform/instancemanagement/v1/product_instance_manager.proto
+-rw-r--r--   0        0        0     1285 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/requirements/requirements_build.txt
+-rw-r--r--   0        0        0      120 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/requirements/requirements_doc.txt
+-rw-r--r--   0        0        0      126 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/requirements/requirements_tests.txt
+-rw-r--r--   0        0        0     3090 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/__init__.py
+-rw-r--r--   0        0        0     9848 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/client.py
+-rw-r--r--   0        0        0     6248 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/configuration.py
+-rw-r--r--   0        0        0     4497 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/definition.py
+-rw-r--r--   0        0        0     3574 2023-04-20 10:10:15.203651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/exceptions.py
+-rw-r--r--   0        0        0    10514 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/instance.py
+-rw-r--r--   0        0        0     3157 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/interceptor.py
+-rw-r--r--   0        0        0     3363 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/service.py
+-rw-r--r--   0        0        0     1021 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0    18868 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tests/test_client.py
+-rw-r--r--   0        0        0     2349 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tests/test_configuration.py
+-rw-r--r--   0        0        0     2804 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tests/test_definition.py
+-rw-r--r--   0        0        0    15486 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tests/test_instance.py
+-rw-r--r--   0        0        0      118 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tests/test_metadata.py
+-rw-r--r--   0        0        0     2424 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tests/test_service.py
+-rw-r--r--   0        0        0     1371 2023-04-20 10:10:15.207651 ansys-platform-instancemanagement-1.1.0/tox.ini
+-rw-r--r--   0        0        0     5874 1970-01-01 00:00:00.000000 ansys-platform-instancemanagement-1.1.0/PKG-INFO
```

### Comparing `ansys-platform-instancemanagement-1.0.3/.github/dependabot.yml` & `ansys-platform-instancemanagement-1.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.0.3/.github/workflows/ci_cd.yml` & `ansys-platform-instancemanagement-1.1.0/.github/workflows/ci_cd.yml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 jobs:
 
   style:
     name: Code style
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.7
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip flit tox
@@ -31,15 +31,15 @@
     strategy:
       matrix:
         os: [windows-latest, ubuntu-latest]
         python-version: ['3.7', '3.8', '3.9', '3.10']
       fail-fast: false
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip flit tox tox-gh-actions
@@ -50,15 +50,15 @@
         if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.10'
         name: 'Upload coverage to Codecov'
 
   docs:
     name: Documentation
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.7
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip flit tox
@@ -73,15 +73,15 @@
 
 
   release:
     name: Build library and publish on tag
     runs-on: ubuntu-latest
     needs: tests
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.7
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip flit
```

### Comparing `ansys-platform-instancemanagement-1.0.3/.gitignore` & `ansys-platform-instancemanagement-1.1.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -154,8 +154,9 @@
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # End of https://www.toptal.com/developers/gitignore/api/python
 
 # VSCode
-.vscode
+.vscode
+/tests/config.json
```

### Comparing `ansys-platform-instancemanagement-1.0.3/.pre-commit-config.yaml` & `ansys-platform-instancemanagement-1.1.0/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   hooks:
   - id: black
     args: [
       src, tests
     ]
 
 - repo: https://github.com/pycqa/isort
-  rev: 5.10.1
+  rev: 5.11.5
   hooks:
   - id: isort
 
 - repo: https://github.com/PyCQA/flake8
   rev: 4.0.1
   hooks:
   - id: flake8
```

### Comparing `ansys-platform-instancemanagement-1.0.3/LICENSE` & `ansys-platform-instancemanagement-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.0.3/README.rst` & `ansys-platform-instancemanagement-1.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -29,34 +29,34 @@
     
 `PyPIM <https://pypim.docs.pyansys.com>`_ exposes a Pythonic interface to
 communicate with the Product Instance Management (PIM) API.
 
 What is the PIM API?
 ============================================
 
-The PIM API is a gRPC API enabling library and application developers to
+The PIM API is a gRPC API, enabling both library and app developers to
 start a product in a remote environment and communicate with its API.
 
 The PIM API is intended to be as simple as possible to be adaptable in a variety of
 network and software infrastructures. Using this API does not require any
 knowledge of its infrastructure. You need only know which product to
 start and which API the product exposes. The PIM API itself exposes very few
 features and assumes that all the configuration is set on a server.
 
 The PIM API is not intended to manage stateless services, to be a job management
 system, or a fully featured service orchestration API. Its purpose is to expose
-a minimum feature set for managing service-oriented applications.
+a minimum feature set for managing service-oriented apps.
 
-Getting Started
+Getting started
 ===============
 To use PyPIM, you must have access to the PIM API.
 
 .. note::
-    The PIM API is a work in progress. Even though the API definition and the
-    PyPIM client are published, the service itself is not publicly exposed.
+   The PIM API is a work in progress. Even though the API definition and the
+   PyPIM client are published, the service itself is not publicly exposed.
 
 PyPIM itself is pure Python and relies on `gRPC`_.
 
 .. _`gRPC`: https://grpc.io/
 
 Installation
 ------------
@@ -67,15 +67,15 @@
 
     pip install ansys-platform-instancemanagement
 
 Configuration
 -------------
 
 By default, PyPIM is configured externally instead of via code. Anywhere in the
-local storage, create a configuration file with the following format:
+local storage, create a configuration file with this format:
 
 .. code-block:: json
 
     {
         "version": 1,
         "pim": {
             "uri": "dns:pim.svc.com:80",
@@ -83,22 +83,22 @@
                 "metadata-info": "value"
             },
             "tls": false
         }
     }
 
 Then, define the environment variable
-``ANSYS_PLATFORM_INSTANCEMANAGEMENT_CONFIG`` to point to this file.
+``ANSYS_PLATFORM_INSTANCEMANAGEMENT_CONFIG`` to point to this configuration file.
 
 Usage
 -----
 PyPIM is a single module called ``ansys.platform.instancemanagement``, shortened
 to ``pypim``.
 
-To start MAPDL and communicate with PyPIM:
+To start MAPDL and communicate with PyPIM, use this code:
 
 .. code-block:: python
     
     import ansys.platform.instancemanagement as pypim
     from ansys.mapdl.core import Mapdl
     
     if pypim.is_configured():
@@ -106,15 +106,15 @@
             with pim.create_instance(product_name="mapdl", product_version="221") as instance:
                 instance.wait_for_ready()
                 channel = instance.build_grpc_channel(options=[("grpc.max_receive_message_length", 8*1024**2)])
                 mapdl = Mapdl(channel=channel)
                 mapdl.prep7()
                 ...
 
-You can also use PyPIM without the ``with`` statement:
+You can also use PyPIM without the ``with`` statement, as shown in this code:
 
 .. code-block:: python
     
     import ansys.platform.instancemanagement as pypim
     from ansys.mapdl.core import Mapdl
     
     if pypim.is_configured():
@@ -127,16 +127,17 @@
         instance.delete()
         pim.close()
 
 Integration
 -----------
 
 PyPIM can be integrated in PyAnsys libraries to transparently switch to a remote
-instance in a suitable environment. This process is described in the
-integration topic.
+instance in a suitable environment. This process is described in `Integration <https://pypim.docs.pyansys.com/integration.html>`_
+in the PyPIM documentation.
 
-For example, starting MAPDL with PyPIM is as simple as:
+For example, starting MAPDL with PyPIM is as simple as using this code:
 
 .. code-block:: python
 
     from ansys.mapdl.core import launch_mapdl    
     mapdl = launch_mapdl()
+
```

### Comparing `ansys-platform-instancemanagement-1.0.3/doc/Makefile` & `ansys-platform-instancemanagement-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.0.3/doc/make.bat` & `ansys-platform-instancemanagement-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.0.3/doc/source/api/index.rst` & `ansys-platform-instancemanagement-1.1.0/doc/source/api/index.rst`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.0.3/doc/source/conf.py` & `ansys-platform-instancemanagement-1.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.0.3/doc/source/contributing.rst` & `ansys-platform-instancemanagement-1.1.0/doc/source/contributing.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,75 @@
-============
-Contributing
-============
+==========
+Contribute
+==========
 
 Overall guidance on contributing to a PyAnsys repository appears in the
 `Contributing`_ topic in the *PyAnsys Developer's Guide*. Ensure that you are
-thoroughly familiar with it and all `Guidelines and Best Practices`_
-before attempting to contribute to PyPIM.
+thoroughly familiar with this guide before attempting to contribute to PyPIM.
  
-.. _`Contributing`: https://dev.docs.pyansys.com/overview/contributing.html
-.. _`Guidelines and Best Practices`: https://dev.docs.pyansys.com/guidelines/index.html
+.. _`Contributing`: https://dev.docs.pyansys.com/how-to/contributing.html
 
 The following contribution information is specific to PyPIM.
 
-Cloning the PyPIM repository
-----------------------------
-Run this code to clone and install the latest version of PyPIM in development mode:
+Clone the PyPIM repository
+--------------------------
+To clone and install the latest version of PyPIM in development mode, run this code:
 
 .. code-block::
     
     git clone https://github.com/pyansys/pypim.git
     cd pypim/
 
-Running tests
--------------
-Test automation relies on `tox`_, which can be installed with:
+Run tests
+---------
+Test automation relies on `tox`_, which can be installed with this command:
 
 .. code-block::
 
     pip install tox
 
 
 Tests are entirely based on mocks and do not require any external software. Run
-the tests with the following code:
+the tests with this command:
 
 .. code-block::
     
     tox -e py
 
+
 .. _`tox`: https://tox.wiki/en/latest/install.html#installation-with-pip
 
-Building the documentation
---------------------------
-You can build PyPIM documentation with:
+Build the documentation
+-----------------------
+You can build PyPIM documentation with this command:
 
 .. code-block::
     
     tox -e doc
 
-Building the package
---------------------
+Build the package
+-----------------
 
-The PyPIM package is built using `flit`.
+The PyPIM package is built using `flit`_.
 
-You can build the package with:
+To build the package, use this command:
 
 .. code-block::
     
     flit build
 
-You can also directly install PyPIM in your current environment with:
+
+You can also directly install PyPIM in your current environment with
+this command:
 
 .. code-block::
     
     flit install
 
+
 .. _`flit`: https://flit.pypa.io/en/latest/#install
 
 Release process
 ---------------
 PyPIM follows the same `branching model`_ as other PyAnsys libraries and the
 same `release procedure`_.
```

### Comparing `ansys-platform-instancemanagement-1.0.3/doc/source/integration.rst` & `ansys-platform-instancemanagement-1.1.0/doc/source/integration.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 ###########
 Integration
 ###########
 
 .. currentmodule:: ansys.platform.instancemanagement
 
-While PyPIM can be used by an application developer, it can also
+While PyPIM can be used by an app developer, it can also
 be used behind the scene by other PyAnsys libraries to manage remote
-instances of the products that they interact with. This enables an application
+instances of the products that they interact with. This enables an app
 developer to write code that works both in an environment configured with PyPIM
 and an environment without such a configuration.
 
-For example, an application developer can write the following code:
+For example, an app developer can write the following code:
 
 .. code:: python
 
    from ansys.mapdl.core import launch_mapdl
 
    mapdl = launch_mapdl()
 
-Instead of:
+The preceding code replaces this much longer code:
 
 .. code:: python
 
    import ansys.platform.instancemanagement as pypim
    from ansys.mapdl.core import launch_mapdl
 
    if pypim.is_configured():
@@ -33,16 +33,16 @@
        channel = instance.build_grpc_channel(
            options=[("grpc.max_receive_message_length", 8 * 1024**2)]
        )
        mapdl = Mapdl(channel=channel)
    else:
        mapdl = launch_mapdl()
 
-This topic provides guidelines for implementing the ``launch_*`` method that
-takes PyPIM into account. Just like the entire PIM API, this topic is targeted
+This page provides guidelines for implementing the ``launch_*`` method that
+takes PyPIM into account. Just like the entire PIM API, this page is targeted
 only toward products that are stateful and require explicit lifecycle
 management.
 
 *****
 Usage
 *****
 
@@ -53,23 +53,23 @@
 must include the following ``require`` string:
 
 ``"ansys-platform-instancemanagement~=1.0"``
 
 Condition for PyPIM usage
 =========================
 
-The condition for using PyPIM transparently is that the user must
+The condition for using PyPIM transparently is that you must
 be able to launch the product in an environment configured with PyPIM
 without specifying launch information. In other words, PyPIM must be
 the default startup method in an environment that is configured with PyPIM.
 
 To integrate PyPIM correctly, you should use either a generic method such as
-``launch_my_product()`` or a constructor that usually starts a local process.
+the ``launch_my_product()`` method or a constructor that usually starts a local process.
 
-For example, with PyMAPDL in an environment configured with PyPIM, the following
+For example, with PyMAPDL in an environment configured with PyPIM, this
 code uses PyPIM:
 
 .. code:: python
 
    from ansys.mapdl.core import launch_mapdl
 
    mapdl = launch_mapdl()
@@ -78,27 +78,27 @@
 
 .. code:: python
 
    from ansys.mapdl.core import launch_mapdl
 
    mapdl = launch_mapdl(exec_file="/usr/bin/mapdl")
 
-Starting a gRPC product
-=======================
+Start a gRPC product
+====================
 
 To use PyPIM, the code flow should first check if PyPIM is configured
-with :func:`is_configured` and then check to ensure that the user has not
-specified how to launch it.
+to use the :func:`is_configured` method and then check to ensure that the caller
+of the ``launch_my_product()`` method has not specified how to launch it.
 
 If both conditions are met:
 
-#. Connect to PyPIM with :func:`connect`
-#. Create an instance with :func:`Client.create_instance`
-#. Wait for the instance to be ready with :func:`Instance.wait_for_ready`
-#. Build a gRPC channel with :func:`Instance.build_grpc_channel`
+#. Connect to PyPIM with the :func:`connect` method.
+#. Create an instance with :func:`Client.create_instance` method.
+#. Wait for the instance to be ready with the :func:`Instance.wait_for_ready` method.
+#. Build a gRPC channel with the :func:`Instance.build_grpc_channel` method.
 
 Typically, the resulting code looks like this:
 
 .. code:: python
 
    import ansys.platform.instancemanagement as pypim
 
@@ -109,29 +109,30 @@
            self.instance.wait_for_ready()
            channel = self.instance.build_grpc_channel()
        else:
            # usual start-up
            self.process = subprocess.run(...)
            channel = grpc.insecure_chanel(...)
 
-When stopping the product, ensure that the remote instance is deleted:
+When stopping the product, use this code to ensure that the remote instance
+is deleted:
 
 .. code:: python
 
    def stop(self):
        if self.instance is not None:
            self.instance.delete()
 
 .. note::
    While it is PyPIM's responsibility to clean up any resource and
    process associated with the product, relevant product-specific cleanup
    can still be performed.
 
-Starting a Non-gRPC product
-===========================
+Start a non-gRPC product
+========================
 
 While the code flow for a non-gRPC product is the same, connection information
 is more specific.
 
 * For a REST-ful product, the base uniform resource identifier (URI) must be
   found under ``instance.services["http"].uri`` and all requests must include the
   headers in ``instance.services["http"].headers``.
@@ -199,22 +200,24 @@
 
         # Mock the general PyPIM connection and configuration check method to expose the mock client.
         mock_connect = create_autospec(pypim.connect, return_value=mock_client)
         mock_is_configured = create_autospec(pypim.is_configured, return_value=True)
         monkeypatch.setattr(pypim, "connect", mock_connect)
         monkeypatch.setattr(pypim, "is_configured", mock_is_configured)
 
+
 This initial setup is faking all the necessary parts of PyPIM. From here,
-calling ``launch_my_product()`` with no parameter is expected to call only the
-mocks, which the test should now do:
+calling the ``launch_my_product()`` method with no parameter is expected
+to call only the mocks, which the test should now do:
 
 .. code:: python
     
     my_product = launch_my_product()
 
+
 After this call, the test is ready to make all the assertions verifying that the PyPIM workflow was applied:
 
 .. code:: python
 
     # The launch method checked if it was in a PyPIM environment
     assert mock_is_configured.called
 
@@ -231,21 +234,24 @@
 
     # It created an gRPC channel from this instance
     assert mock_instance.build_grpc_channel.called
 
     # It connected using the channel created by PyPIM
     assert my_product._channel == pim_channel
 
+
 When stopping the product, the test should also verify that the remote instance is deleted:
 
 .. code:: python
     
     # Stop the product
     my_product.stop()
     
     assert mock_instance.delete.called
 
+
 *******
 Example
 *******
 
-An example of such an integration can be seen `in PyMAPDL <https://github.com/pyansys/pymapdl/pull/1091/files>`_.
+An example of such an integration can be seen in this
+`PyMAPDL pull request <https://github.com/pyansys/pymapdl/pull/1091/files>`_.
```

### Comparing `ansys-platform-instancemanagement-1.0.3/protos/ansys/api/platform/instancemanagement/v1/product_instance_manager.proto` & `ansys-platform-instancemanagement-1.1.0/protos/ansys/api/platform/instancemanagement/v1/product_instance_manager.proto`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.0.3/pyproject.toml` & `ansys-platform-instancemanagement-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-platform-instancemanagement"
-version = "1.0.3"
+version = "1.1.0"
 description = "A Python wrapper for Ansys platform instancemanagement"
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.support@ansys.com"},
 ]
```

### Comparing `ansys-platform-instancemanagement-1.0.3/src/ansys/platform/instancemanagement/__init__.py` & `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,19 @@
     import importlib.metadata as importlib_metadata
 except ModuleNotFoundError:
     import importlib_metadata
 
 import os
 
 from ansys.platform.instancemanagement.client import Client
+from ansys.platform.instancemanagement.configuration import (
+    CONFIGURATION_PATH_ENVIRONMENT_VARIABLE,
+    Configuration,
+    is_configured,
+)
 from ansys.platform.instancemanagement.definition import Definition
 from ansys.platform.instancemanagement.exceptions import (
     InstanceNotFoundError,
     InstanceNotReadyError,
     InvalidConfigurationError,
     NotConfiguredError,
     RemoteError,
@@ -23,41 +28,29 @@
 
 __all__ = [
     "__version__",
     "CONFIGURATION_PATH_ENVIRONMENT_VARIABLE",
     "is_configured",
     "connect",
     "Client",
+    "Configuration",
     "Instance",
     "Service",
     "Definition",
     "InstanceNotFoundError",
     "InvalidConfigurationError",
     "NotConfiguredError",
     "RemoteError",
     "UnsupportedProductError",
     "InstanceNotReadyError",
     "UnsupportedServiceError",
 ]
 
 __version__ = importlib_metadata.version(__name__.replace(".", "-"))
 
-CONFIGURATION_PATH_ENVIRONMENT_VARIABLE = "ANSYS_PLATFORM_INSTANCEMANAGEMENT_CONFIG"
-
-
-def is_configured() -> bool:
-    """Check if the environment is configured to use PyPIM.
-
-    Returns
-    -------
-    bool
-        ``True`` when the environment is configured to use PyPIM, ``False`` otherwise.
-    """
-    return CONFIGURATION_PATH_ENVIRONMENT_VARIABLE in os.environ
-
 
 def connect() -> Client:
     """Create a PyPIM client based on the environment configuration.
 
     Before calling this method, :func:`~is_configured()` should be called to check if
     the environment is configured to use PyPIM.
 
@@ -106,8 +99,10 @@
         >>> import ansys.platform.instancemanagement as pypim
         >>> if pypim.is_configured():
         >>>     with pypim.connect() as client:
         >>>         # use client
     """
     if not is_configured():
         raise NotConfiguredError("The environment is not configured to use PyPIM.")
-    return Client._from_configuration(os.environ[CONFIGURATION_PATH_ENVIRONMENT_VARIABLE])
+    return Client._from_configuration(
+        os.path.expandvars(os.environ[CONFIGURATION_PATH_ENVIRONMENT_VARIABLE])
+    )
```

### Comparing `ansys-platform-instancemanagement-1.0.3/src/ansys/platform/instancemanagement/client.py` & `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Client class module."""
 import contextlib
-import json
 import logging
 from typing import Sequence
 
 from ansys.api.platform.instancemanagement.v1.product_instance_manager_pb2 import (
     GetInstanceRequest,
     ListDefinitionsRequest,
     ListInstancesRequest,
 )
 from ansys.api.platform.instancemanagement.v1.product_instance_manager_pb2_grpc import (
     ProductInstanceManagerStub,
 )
 import grpc
 
+from ansys.platform.instancemanagement.configuration import Configuration
 from ansys.platform.instancemanagement.definition import Definition
 from ansys.platform.instancemanagement.exceptions import (
     InstanceNotFoundError,
-    InvalidConfigurationError,
     RemoteError,
     UnsupportedProductError,
 )
 from ansys.platform.instancemanagement.instance import Instance
 from ansys.platform.instancemanagement.interceptor import header_adder_interceptor
 
 logger = logging.getLogger(__name__)
@@ -30,17 +29,18 @@
 class Client(contextlib.AbstractContextManager):
     """Provides a high-level client object for interacting with the PIM API.
 
     This class exposes the methods of the PIM API.
     """
 
     _channel: grpc.Channel
+    _configuration: Configuration
     _stub: ProductInstanceManagerStub
 
-    def __init__(self, channel: grpc.Channel) -> None:
+    def __init__(self, channel: grpc.Channel, configuration: Configuration = None) -> None:
         """Initialize the client library.
 
         Parameters
         ----------
         channel
             gRPC channel hosting the connection.
 
@@ -50,14 +50,15 @@
             >>> import grpc
             >>> channel = grpc.insecure_channel("127.0.0.0:50001")
             >>> client = pypim.Client(channel)
 
         """
         logger.info("Connecting.")
         self._channel = channel
+        self._configuration = configuration
         self._stub = ProductInstanceManagerStub(self._channel)
 
     def __exit__(self, *_):
         """Close the channel when used in a ``with`` statement."""
         self._channel.close()
 
     def close(self):
@@ -82,56 +83,37 @@
             PyPIM client.
 
         Raises
         ------
         InvalidConfigurationError
             The configuration is not valid.
         """
-        logger.debug("Initializing from %s", config_path)
-
         # Note: At some point, this configuration is likely to become a
         # full-featured object to be shared across the PyPIM class.
         # The configuration is a plain JSON file with the settings for creating
         # the gRPC channel.
 
-        with open(config_path, "r") as f:
-            try:
-                configuration = json.load(f)
-            except json.JSONDecodeError:
-                raise InvalidConfigurationError(config_path, "Invalid json.")
+        configuration = Configuration.from_file(config_path)
 
-        # What follows should likely be done with a schema validation
-        try:
-            version = configuration["version"]
-            if version != 1:
-                raise InvalidConfigurationError(
-                    config_path,
-                    f'Unsupported version "{version}".\
-Consider upgrading ansys-platform-instancemanagement.',
-                )
-
-            pim_configuration = configuration["pim"]
-            tls = pim_configuration["tls"]
-            if tls:
-                raise InvalidConfigurationError(
-                    config_path, f"Secured connection is not yet supported."
-                )
-
-            uri = pim_configuration["uri"]
-            headers = [(key, value) for key, value in pim_configuration["headers"].items()]
-        except KeyError as e:
-            key = e.args[0]
-            raise InvalidConfigurationError(
-                config_path, f"The configuration is missing the entry {key}."
+        if configuration.tls:
+            logger.debug("The connection to the server will use a secure channel.")
+            channel_credentials = grpc.composite_channel_credentials(
+                grpc.ssl_channel_credentials(),
+                grpc.access_token_call_credentials(configuration.access_token),
             )
+            grpc_channel = grpc.secure_channel(configuration.uri, channel_credentials)
+        else:
+            grpc_channel = grpc.insecure_channel(configuration.uri)
 
         channel = grpc.intercept_channel(
-            grpc.insecure_channel(uri), header_adder_interceptor(headers)
+            grpc_channel,
+            header_adder_interceptor(configuration.headers),
         )
-        return Client(channel)
+
+        return Client(channel, configuration)
 
     def list_definitions(
         self,
         product_name: str = None,
         product_version: str = None,
         timeout: float = None,
     ) -> Sequence[Definition]:
@@ -203,15 +185,18 @@
         request = ListInstancesRequest()
 
         try:
             response = self._stub.ListInstances(request, timeout=timeout)
         except grpc.RpcError as exc:
             raise RemoteError(exc, exc.details()) from exc
 
-        return [Instance._from_pim_v1(instance, self._stub) for instance in response.instances]
+        return [
+            Instance._from_pim_v1(instance, self._stub, self._configuration)
+            for instance in response.instances
+        ]
 
     def create_instance(
         self,
         product_name: str,
         product_version: str = None,
         requests_timeout: float = None,
     ) -> Instance:
@@ -260,15 +245,17 @@
         )
 
         if len(definitions) == 0:
             raise UnsupportedProductError(
                 product_name=product_name, product_version=product_version
             )
         definition = definitions[0]
-        return definition.create_instance(timeout=requests_timeout)
+        return definition.create_instance(
+            timeout=requests_timeout, configuration=self._configuration
+        )
 
     def get_instance(self, name: str, timeout: float = None) -> Instance:
         """Get a remote product instance by name.
 
         Parameters
         ----------
         name: str
@@ -295,8 +282,8 @@
         try:
             instance = self._stub.GetInstance(request, timeout=timeout)
         except grpc.RpcError as exc:
             if exc.code() == grpc.StatusCode.NOT_FOUND:
                 raise InstanceNotFoundError(exc, f"The instance {name} does not exist.") from exc
             raise RemoteError(exc, exc.details()) from exc
 
-        return Instance._from_pim_v1(instance, self._stub)
+        return Instance._from_pim_v1(instance, self._stub, self._configuration)
```

### Comparing `ansys-platform-instancemanagement-1.0.3/src/ansys/platform/instancemanagement/definition.py` & `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/definition.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from ansys.api.platform.instancemanagement.v1.product_instance_manager_pb2 import (
     Definition as DefinitionV1,
 )
 from ansys.api.platform.instancemanagement.v1.product_instance_manager_pb2_grpc import (
     ProductInstanceManagerStub,
 )
 
+from ansys.platform.instancemanagement.configuration import Configuration
 from ansys.platform.instancemanagement.instance import Instance
 
 
 class Definition:
     """Provides a definition of a product that can be started using the PIM API.
 
     The definition is a static object describing a product that can be started remotely.
@@ -93,28 +94,32 @@
         """Python-callable description."""
         return (
             f"Definition(name={repr(self.name)}, product_name={repr(self.product_name)},"
             f" product_version={repr(self.product_version)}, available_service_names="
             f"{repr(self.available_service_names)})"
         )
 
-    def create_instance(self, timeout: float = None) -> Instance:
+    def create_instance(
+        self, timeout: float = None, configuration: Configuration = None
+    ) -> Instance:
         """Create a product instance from this definition.
 
         Parameters
         ----------
         timeout : float
             Time in seconds to create the instance. The default is ``None``.
 
         Returns
         -------
         instance
             Product instance.
         """
-        return Instance._create(definition_name=self.name, stub=self._stub, timeout=timeout)
+        return Instance._create(
+            definition_name=self.name, stub=self._stub, timeout=timeout, configuration=configuration
+        )
 
     @staticmethod
     def _from_pim_v1(definition: DefinitionV1, stub: ProductInstanceManagerStub = None):
         """Build a definition from the PIM API v1 protobuf object.
 
         Parameters
         ----------
```

### Comparing `ansys-platform-instancemanagement-1.0.3/src/ansys/platform/instancemanagement/exceptions.py` & `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.0.3/src/ansys/platform/instancemanagement/instance.py` & `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Instance as InstanceV1,
 )
 from ansys.api.platform.instancemanagement.v1.product_instance_manager_pb2_grpc import (
     ProductInstanceManagerStub,
 )
 import grpc
 
+from ansys.platform.instancemanagement.configuration import Configuration
 from ansys.platform.instancemanagement.exceptions import (
     InstanceNotFoundError,
     InstanceNotReadyError,
     RemoteError,
     UnsupportedServiceError,
 )
 from ansys.platform.instancemanagement.service import Service
@@ -35,14 +36,15 @@
 
     This class is a context manager and can be used with the ``with`` statement to
     automatically stop the remote instance when the tasks are finished.
     """
 
     _stub: ProductInstanceManagerStub
 
+    _configuration: Configuration
     _definition_name: str
     _name: str
     _ready: bool
     _status_message: str
     _services: Mapping[str, Service]
 
     @property
@@ -98,14 +100,15 @@
         name: str,
         ready: bool,
         status_message: str,
         services: Mapping[str, Service],
         stub: ProductInstanceManagerStub = None,
     ):
         """Create an Instance."""
+        self._configuration = None
         self._definition_name = definition_name
         self._name = name
         self._ready = ready
         self._status_message = status_message
         self._services = services
         self._stub = stub
         if self.status_message:
@@ -133,30 +136,35 @@
         return (
             f"Instance(name={repr(self.name)}, definition_name={repr(self.definition_name)},"
             f" ready={repr(self.ready)}, status_message={repr(self.status_message)},"
             f" services={repr(self.services)})"
         )
 
     @staticmethod
-    def _create(definition_name: str, stub: ProductInstanceManagerStub, timeout: float = None):
+    def _create(
+        definition_name: str,
+        stub: ProductInstanceManagerStub,
+        timeout: float = None,
+        configuration: Configuration = None,
+    ):
         """Create a product instance from the given definition.
 
         Parameters
         ----------
         timeout : float
             Time in seconds to create the instance. The default is ``None``.
 
         Returns
         -------
         Instance
             Product instance.
         """
         request = CreateInstanceRequest(instance=InstanceV1(definition_name=definition_name))
         instance = stub.CreateInstance(request, timeout=timeout)
-        return Instance._from_pim_v1(instance, stub)
+        return Instance._from_pim_v1(instance, stub, configuration)
 
     def delete(self, timeout: float = None):
         """Delete the remote product instance.
 
         Parameters
         ----------
         timeout : float, optional
@@ -280,30 +288,36 @@
         if not self.ready:
             raise InstanceNotReadyError(self.name)
 
         service = self.services.get(service_name, None)
         if not service:
             raise UnsupportedServiceError(self.name, service_name)
 
-        return service._build_grpc_channel(**kwargs)
+        return service._build_grpc_channel(configuration=self._configuration, **kwargs)
 
     @staticmethod
-    def _from_pim_v1(instance: InstanceV1, stub: ProductInstanceManagerStub = None):
+    def _from_pim_v1(
+        instance: InstanceV1,
+        stub: ProductInstanceManagerStub = None,
+        configuration: Configuration = None,
+    ):
         """Create a PyPIM instance from the raw protobuf message.
 
         Parameters
         ----------
         instance : InstanceV1
             Raw protobuf message from the PIM API.
         stub : ProductInstanceManagerStub, optional
             PIM stub.
         """
-        return Instance(
+        instance = Instance(
             name=instance.name,
             definition_name=instance.definition_name,
             status_message=instance.status_message,
             services={
                 name: Service._from_pim_v1(value) for name, value in instance.services.items()
             },
             ready=instance.ready,
             stub=stub,
         )
+        instance._configuration = configuration
+        return instance
```

### Comparing `ansys-platform-instancemanagement-1.0.3/src/ansys/platform/instancemanagement/interceptor.py` & `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/interceptor.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.0.3/src/ansys/platform/instancemanagement/service.py` & `ansys-platform-instancemanagement-1.1.0/src/ansys/platform/instancemanagement/service.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Mapping
 
 from ansys.api.platform.instancemanagement.v1.product_instance_manager_pb2 import (
     Service as ServiceV1,
 )
 import grpc
 
+from ansys.platform.instancemanagement.configuration import Configuration
 from ansys.platform.instancemanagement.interceptor import header_adder_interceptor
 
 
 class Service:
     """Provides an entry point for communicating with a remote product."""
 
     _uri: str
@@ -51,32 +52,43 @@
 
     def __repr__(self):
         """Python callable representation."""
         return f"Service(uri={repr(self.uri)}, headers={repr(self.headers)})"
 
     def _build_grpc_channel(
         self,
+        configuration: Configuration = None,
         **kwargs,
     ) -> grpc.Channel:
         """Build a gRPC channel communicating with the product instance.
 
         Parameters
         -----------
+        configuration: pim configuration
         kwargs: list, optional
             Named arguments for gRPC construction.
-            They are passed to ``grpc.insecure_channel``.
+            They are passed to ``grpc.secure_channel`` or ``grpc.insecure_channel``.
 
         Returns
         -------
         grpc.Channel
             gRPC channel ready to be used for communicating with the service.
         """
         headers = self.headers.items()
         interceptor = header_adder_interceptor(headers)
-        channel = grpc.insecure_channel(self.uri, **kwargs)
+
+        if configuration is not None and configuration.tls:
+            credentials = grpc.composite_channel_credentials(
+                grpc.ssl_channel_credentials(),
+                grpc.access_token_call_credentials(configuration.access_token),
+            )
+            channel = grpc.secure_channel(self.uri, credentials, **kwargs)
+        else:
+            channel = grpc.insecure_channel(self.uri, **kwargs)
+
         return grpc.intercept_channel(channel, interceptor)
 
     @staticmethod
     def _from_pim_v1(service: ServiceV1):
         """Build a definition from the PIM API v1 protobuf object.
 
         Parameters
```

### Comparing `ansys-platform-instancemanagement-1.0.3/tests/conftest.py` & `ansys-platform-instancemanagement-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.0.3/tests/test_client.py` & `ansys-platform-instancemanagement-1.1.0/tests/test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 
     #  Assert
     # The client got the hardcoded instances
     server_future.result()
     assert instances == expected_instances
 
 
-def test_create_instance(testing_channel):
+def test_create_instance_without_configuration(testing_channel):
     # Arrange
     # A client with two definitions
     client = pypim.Client(testing_channel)
     definitions = [
         pypim.Definition(
             name="definitions/the-good-one",
             product_name="calculator",
@@ -344,15 +344,71 @@
 
     # Assert
     # The method created an instance from the first definition
     client.list_definitions.assert_called()
     client.list_definitions.assert_called_once_with(
         product_name="definitions/the-good-one", product_version=None, timeout=0.32
     )
-    definitions[0].create_instance.assert_called_once_with(timeout=0.32)
+    definitions[0].create_instance.assert_called_once_with(timeout=0.32, configuration=None)
+    definitions[1].create_instance.assert_not_called()
+    assert created_instance == instance
+
+
+def test_create_instance(testing_channel):
+    # Arrange
+    # A client with two definitions
+    configuration = pypim.Configuration(
+        headers=[],
+        tls=False,
+        uri="dns:instancemanagement.example.com:443",
+        access_token="Bearer 007",
+    )
+    client = pypim.Client(testing_channel, configuration)
+
+    definitions = [
+        pypim.Definition(
+            name="definitions/the-good-one",
+            product_name="calculator",
+            product_version="221",
+            available_service_names=["fax"],
+        ),
+        pypim.Definition(
+            name="definitions/the-bad-one",
+            product_name="calculator",
+            product_version="195",
+            available_service_names=["fax"],
+        ),
+    ]
+    instance = pypim.Instance(
+        definition_name="definitions/the-good-one",
+        name="instances/calculator-42",
+        ready=False,
+        status_message="loading...",
+        services={},
+    )
+
+    definitions[0].create_instance = create_autospec(
+        definitions[0].create_instance, return_value=instance
+    )
+    definitions[1].create_instance = create_autospec(definitions[1].create_instance)
+    client.list_definitions = create_autospec(client.list_definitions, return_value=definitions)
+
+    # Act
+    created_instance = client.create_instance(
+        product_name="definitions/the-good-one", requests_timeout=0.32
+    )
+
+    # Assert
+    # The method created an instance from the first definition
+    client.list_definitions.assert_called_once_with(
+        product_name="definitions/the-good-one", product_version=None, timeout=0.32
+    )
+    definitions[0].create_instance.assert_called_once_with(
+        timeout=0.32, configuration=configuration
+    )
     definitions[1].create_instance.assert_not_called()
     assert created_instance == instance
 
 
 def test_unsupported_product(
     testing_channel: grpc_testing.Channel,
 ):
@@ -452,15 +508,15 @@
             r"""{"version": 1, "pim": {"uri": "dns:127.0.0.1:5000",
             "headers": {"token": "007","identity": "james bond"}}}""",
             "tls",
         ),
         (
             r"""{"version": 1, "pim": {"uri": "dns:127.0.0.1:5000", "tls": true,
             "headers": {"token": "007","identity": "james bond"}}}""",
-            "not yet supported",
+            "authorization header with a bearer token is required",
         ),
     ],
 )
 def test_bad_configuration(tmp_path, bad_configuration, message_content):
     config_path = tmp_path / "pim.json"
     with open(config_path, "w") as f:
         f.write(bad_configuration)
```

### Comparing `ansys-platform-instancemanagement-1.0.3/tests/test_definition.py` & `ansys-platform-instancemanagement-1.1.0/tests/test_definition.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,22 +41,28 @@
             name="definitions/my_def",
             product_name="my_product",
             product_version="221",
             available_service_names=["grpc", "http"],
             stub=stub,
         )
 
+        configuration = pypim.Configuration(
+            headers=[],
+            tls=False,
+            uri="dns:instancemanagement.example.com:443",
+            access_token="Bearer 007",
+        )
         # Act
         # Create the instance from the definition
-        definition.create_instance(0.1)
+        definition.create_instance(0.1, configuration)
 
     # Assert
     # The mocked Instance class was correctly called
     mock_instance_create.assert_called_once_with(
-        definition_name="definitions/my_def", timeout=0.1, stub=stub
+        definition_name="definitions/my_def", timeout=0.1, stub=stub, configuration=configuration
     )
 
 
 def test_str():
     definition_str = str(
         pypim.Definition(
             name="definitions/my_def",
```

### Comparing `ansys-platform-instancemanagement-1.0.3/tests/test_instance.py` & `ansys-platform-instancemanagement-1.1.0/tests/test_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,41 +352,43 @@
     assert instance.services == {"http": pb2.Service(uri="http://example.com", headers={})}
 
 
 def test_create_channel():
     # Arrange
     # Two mocked services
     main_service = pypim.Service(uri="dns:example.com", headers={})
+    sidecar_service = pypim.Service(uri="dns:ansysapis.com", headers={})
+
     main_channel = grpc.insecure_channel("dns:example.com")
     main_service._build_grpc_channel = create_autospec(
         main_service._build_grpc_channel, return_value=main_channel
     )
-
-    sidecar_service = pypim.Service(uri="dns:ansysapis.com", headers={})
     sidecar_channel = grpc.insecure_channel("dns:ansysapis.com")
     sidecar_service._build_grpc_channel = create_autospec(
         sidecar_service._build_grpc_channel, return_value=sidecar_channel
     )
 
     # An instance containing these services
     instance = pypim.Instance(
         name="instances/hello-world-32",
         definition_name="definitions/my-def",
         ready=True,
         status_message="Creating...",
         services={"grpc": main_service, "other": sidecar_service},
     )
 
+    # instance._configuration = configuration
     # Act: Create two channels
     channel1 = instance.build_grpc_channel()
     channel2 = instance.build_grpc_channel(service_name="other")
 
     # Assert: The services were called
     main_service._build_grpc_channel.assert_called_once()
     sidecar_service._build_grpc_channel.assert_called_once()
+
     assert channel1 == main_channel
     assert channel2 == sidecar_channel
 
 
 def test_create_channel_not_ready():
     # Arrange
     # An instance that's not ready
```

### Comparing `ansys-platform-instancemanagement-1.0.3/tests/test_service.py` & `ansys-platform-instancemanagement-1.1.0/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.0.3/tox.ini` & `ansys-platform-instancemanagement-1.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys-platform-instancemanagement-1.0.3/PKG-INFO` & `ansys-platform-instancemanagement-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-platform-instancemanagement
-Version: 1.0.3
+Version: 1.1.0
 Summary: A Python wrapper for Ansys platform instancemanagement
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -45,34 +45,34 @@
     
 `PyPIM <https://pypim.docs.pyansys.com>`_ exposes a Pythonic interface to
 communicate with the Product Instance Management (PIM) API.
 
 What is the PIM API?
 ============================================
 
-The PIM API is a gRPC API enabling library and application developers to
+The PIM API is a gRPC API, enabling both library and app developers to
 start a product in a remote environment and communicate with its API.
 
 The PIM API is intended to be as simple as possible to be adaptable in a variety of
 network and software infrastructures. Using this API does not require any
 knowledge of its infrastructure. You need only know which product to
 start and which API the product exposes. The PIM API itself exposes very few
 features and assumes that all the configuration is set on a server.
 
 The PIM API is not intended to manage stateless services, to be a job management
 system, or a fully featured service orchestration API. Its purpose is to expose
-a minimum feature set for managing service-oriented applications.
+a minimum feature set for managing service-oriented apps.
 
-Getting Started
+Getting started
 ===============
 To use PyPIM, you must have access to the PIM API.
 
 .. note::
-    The PIM API is a work in progress. Even though the API definition and the
-    PyPIM client are published, the service itself is not publicly exposed.
+   The PIM API is a work in progress. Even though the API definition and the
+   PyPIM client are published, the service itself is not publicly exposed.
 
 PyPIM itself is pure Python and relies on `gRPC`_.
 
 .. _`gRPC`: https://grpc.io/
 
 Installation
 ------------
@@ -83,15 +83,15 @@
 
     pip install ansys-platform-instancemanagement
 
 Configuration
 -------------
 
 By default, PyPIM is configured externally instead of via code. Anywhere in the
-local storage, create a configuration file with the following format:
+local storage, create a configuration file with this format:
 
 .. code-block:: json
 
     {
         "version": 1,
         "pim": {
             "uri": "dns:pim.svc.com:80",
@@ -99,22 +99,22 @@
                 "metadata-info": "value"
             },
             "tls": false
         }
     }
 
 Then, define the environment variable
-``ANSYS_PLATFORM_INSTANCEMANAGEMENT_CONFIG`` to point to this file.
+``ANSYS_PLATFORM_INSTANCEMANAGEMENT_CONFIG`` to point to this configuration file.
 
 Usage
 -----
 PyPIM is a single module called ``ansys.platform.instancemanagement``, shortened
 to ``pypim``.
 
-To start MAPDL and communicate with PyPIM:
+To start MAPDL and communicate with PyPIM, use this code:
 
 .. code-block:: python
     
     import ansys.platform.instancemanagement as pypim
     from ansys.mapdl.core import Mapdl
     
     if pypim.is_configured():
@@ -122,15 +122,15 @@
             with pim.create_instance(product_name="mapdl", product_version="221") as instance:
                 instance.wait_for_ready()
                 channel = instance.build_grpc_channel(options=[("grpc.max_receive_message_length", 8*1024**2)])
                 mapdl = Mapdl(channel=channel)
                 mapdl.prep7()
                 ...
 
-You can also use PyPIM without the ``with`` statement:
+You can also use PyPIM without the ``with`` statement, as shown in this code:
 
 .. code-block:: python
     
     import ansys.platform.instancemanagement as pypim
     from ansys.mapdl.core import Mapdl
     
     if pypim.is_configured():
@@ -143,17 +143,18 @@
         instance.delete()
         pim.close()
 
 Integration
 -----------
 
 PyPIM can be integrated in PyAnsys libraries to transparently switch to a remote
-instance in a suitable environment. This process is described in the
-integration topic.
+instance in a suitable environment. This process is described in `Integration <https://pypim.docs.pyansys.com/integration.html>`_
+in the PyPIM documentation.
 
-For example, starting MAPDL with PyPIM is as simple as:
+For example, starting MAPDL with PyPIM is as simple as using this code:
 
 .. code-block:: python
 
     from ansys.mapdl.core import launch_mapdl    
     mapdl = launch_mapdl()
 
+
```

