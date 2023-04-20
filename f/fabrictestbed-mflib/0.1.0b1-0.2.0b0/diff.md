# Comparing `tmp/fabrictestbed-mflib-0.1.0b1.tar.gz` & `tmp/fabrictestbed-mflib-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-mflib-0.1.0b1.tar", last modified: Fri Apr 14 03:22:48 2023, max compression
+gzip compressed data, was "fabrictestbed-mflib-0.2.0b0.tar", last modified: Thu Apr 20 21:38:11 2023, max compression
```

## Comparing `fabrictestbed-mflib-0.1.0b1.tar` & `fabrictestbed-mflib-0.2.0b0.tar`

### file list

```diff
@@ -1,28 +1,39 @@
--rw-r--r--   0        0        0      647 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.1.0b1/.gitignore
--rw-r--r--   0        0        0      575 2023-03-29 18:17:09.721091 fabrictestbed-mflib-0.1.0b1/.readthedocs.yaml
--rw-r--r--   0        0        0     1071 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.1.0b1/LICENSE
--rw-r--r--   0        0        0       24 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.1.0b1/MANIFEST.in
--rw-r--r--   0        0        0   197131 2023-04-14 03:21:30.723292 fabrictestbed-mflib-0.1.0b1/MFLib.pdf
--rw-r--r--   0        0        0     4071 2023-04-13 20:24:08.607249 fabrictestbed-mflib-0.1.0b1/README.md
--rwxr-xr-x   0        0        0      817 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/create_html_doc.sh
--rwxr-xr-x   0        0        0      687 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/create_pdf_doc.sh
--rwxr-xr-x   0        0        0      668 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/create_release.sh
--rw-r--r--   0        0        0      638 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b1/docs/Makefile
--rw-r--r--   0        0        0      804 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b1/docs/make.bat
--rw-r--r--   0        0        0       55 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/docs/requirements.txt
-lrwxr-xr-x   0        0        0        0 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b1/docs/source/README.md -> ../../README.md
--rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b1/docs/source/_static/placeholder
--rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b1/docs/source/_templates/placeholder
--rw-r--r--   0        0        0     1297 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/docs/source/conf.py
--rw-r--r--   0        0        0      204 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b1/docs/source/core.rst
--rw-r--r--   0        0        0      262 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/docs/source/index.rst
--rw-r--r--   0        0        0      215 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/docs/source/mflib.rst
--rw-r--r--   0        0        0     7308 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b1/mflib/README.md
--rw-r--r--   0        0        0      539 2023-04-14 02:31:14.348369 fabrictestbed-mflib-0.1.0b1/mflib/__init__.py
--rw-r--r--   0        0        0    41757 2023-04-14 02:31:55.528704 fabrictestbed-mflib-0.1.0b1/mflib/core.py
--rw-r--r--   0        0        0    11653 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/mflib/mf_timestamp.py
--rw-r--r--   0        0        0    31859 2023-04-14 02:22:04.816077 fabrictestbed-mflib-0.1.0b1/mflib/mflib.py
--rw-r--r--   0        0        0    27967 2023-02-01 16:43:59.712079 fabrictestbed-mflib-0.1.0b1/mflib/mfvis.py
--rw-r--r--   0        0        0      735 2023-04-13 19:34:14.734792 fabrictestbed-mflib-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0       32 2023-02-01 16:43:59.712079 fabrictestbed-mflib-0.1.0b1/requirements.txt
--rw-r--r--   0        0        0     4581 1970-01-01 00:00:00.000000 fabrictestbed-mflib-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0      647 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.2.0b0/.gitignore
+-rw-r--r--   0        0        0      575 2023-03-29 18:17:09.721091 fabrictestbed-mflib-0.2.0b0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1071 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.2.0b0/LICENSE
+-rw-r--r--   0        0        0       24 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.2.0b0/MANIFEST.in
+-rw-r--r--   0        0        0   668002 2023-04-20 20:16:13.194055 fabrictestbed-mflib-0.2.0b0/MFLib.pdf
+-rw-r--r--   0        0        0     3974 2023-04-17 18:32:21.683648 fabrictestbed-mflib-0.2.0b0/README.md
+-rwxr-xr-x   0        0        0      817 2023-04-17 18:32:21.683648 fabrictestbed-mflib-0.2.0b0/create_html_doc.sh
+-rwxr-xr-x   0        0        0      687 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.2.0b0/create_pdf_doc.sh
+-rwxr-xr-x   0        0        0      668 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.2.0b0/create_release.sh
+-rw-r--r--   0        0        0      638 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.2.0b0/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.2.0b0/docs/make.bat
+-rw-r--r--   0        0        0       55 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.2.0b0/docs/requirements.txt
+lrwxr-xr-x   0        0        0        0 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.2.0b0/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.2.0b0/docs/source/_static/placeholder
+-rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.2.0b0/docs/source/_templates/placeholder
+-rw-r--r--   0        0        0     1297 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.2.0b0/docs/source/conf.py
+-rw-r--r--   0        0        0      204 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.2.0b0/docs/source/core.rst
+-rw-r--r--   0        0        0    42620 2023-04-18 03:41:22.987762 fabrictestbed-mflib-0.2.0b0/docs/source/images/3nodes.png
+-rw-r--r--   0        0        0    71388 2023-04-18 03:41:22.987762 fabrictestbed-mflib-0.2.0b0/docs/source/images/3nodes_add_meas.png
+-rw-r--r--   0        0        0   100374 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/images/3nodes_ini.png
+-rw-r--r--   0        0        0    70104 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/images/3nodes_inst.png
+-rw-r--r--   0        0        0   204495 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/images/keys.png
+-rw-r--r--   0        0        0      310 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/index.rst
+-rw-r--r--   0        0        0       94 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/mf_timestamp.rst
+-rw-r--r--   0        0        0      215 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.2.0b0/docs/source/mflib.rst
+-rw-r--r--   0        0        0     6230 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/overview.md
+-rw-r--r--   0        0        0       58 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/owl.rst
+-rw-r--r--   0        0        0       81 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/owl_data.rst
+-rw-r--r--   0        0        0     7308 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.2.0b0/mflib/README.md
+-rw-r--r--   0        0        0      539 2023-04-20 20:15:41.833758 fabrictestbed-mflib-0.2.0b0/mflib/__init__.py
+-rw-r--r--   0        0        0    47346 2023-04-20 18:51:49.099811 fabrictestbed-mflib-0.2.0b0/mflib/core.py
+-rw-r--r--   0        0        0    17118 2023-04-17 18:32:21.683648 fabrictestbed-mflib-0.2.0b0/mflib/mf_timestamp.py
+-rw-r--r--   0        0        0    31971 2023-04-18 03:40:43.967413 fabrictestbed-mflib-0.2.0b0/mflib/mflib.py
+-rw-r--r--   0        0        0    27967 2023-02-01 16:43:59.712079 fabrictestbed-mflib-0.2.0b0/mflib/mfvis.py
+-rw-r--r--   0        0        0    15650 2023-04-18 01:21:17.807688 fabrictestbed-mflib-0.2.0b0/mflib/owl.py
+-rw-r--r--   0        0        0    11858 2023-04-19 17:56:04.413586 fabrictestbed-mflib-0.2.0b0/mflib/owl_data.py
+-rw-r--r--   0        0        0      735 2023-04-17 18:32:21.683648 fabrictestbed-mflib-0.2.0b0/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-02-01 16:43:59.712079 fabrictestbed-mflib-0.2.0b0/requirements.txt
+-rw-r--r--   0        0        0     4484 1970-01-01 00:00:00.000000 fabrictestbed-mflib-0.2.0b0/PKG-INFO
```

### Comparing `fabrictestbed-mflib-0.1.0b1/.gitignore` & `fabrictestbed-mflib-0.2.0b0/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b1/.readthedocs.yaml` & `fabrictestbed-mflib-0.2.0b0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b1/LICENSE` & `fabrictestbed-mflib-0.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b1/README.md` & `fabrictestbed-mflib-0.2.0b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: fabrictestbed-mflib
+Version: 0.2.0b0
+Summary: FABRIC Measurement Framework Python Client Library - Makes monitoring FABRIC Slice easy.
+Author: Song, Pinyi, Hussam
+Author-email: Carpenter <csacarp0@g.uky.edu>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Project-URL: Homepage, https://github.com/fabric-testbed/mflib
+
 # MFLIB Measurement Framework Library
 
 [![Documentation Status](https://readthedocs.org/projects/fabrictestbed-mflib/badge/?version=latest)](https://fabrictestbed-mflib.readthedocs.io/en/latest/?badge=latest)
 
 Welcome to the FABRIC Measurement Framework Library. MFLib makes it easy to install monitoring systems to a FABRIC experimenter's slice. The monitoring system makes extensive use of industry standards such as Prometheus, Grafana, Elastic Search and Kibana while adding customized monitoring tools and dashboards for quick setup and visualization.
 
 ## Documentation Resources
@@ -12,15 +25,14 @@
 ### FABRIC Learn Site
 [FABRIC Knowledge Base](https://learn.fabric-testbed.net/) 
 
 ### MFLib Python Package Documentation
 Documentation for the package is presented in serveral different forms (and maybe include later in this document):
 * [ReadTheDocs](https://fabrictestbed-mflib.readthedocs.io/en/latest/)
 * [MFLib.pdf](https://github.com/fabric-testbed/mflib/blob/main/MFLib.pdf) in the source code/GitHub.
-* [MFLib HTML Index](https://github.com/fabric-testbed/mflib/blob/main/docs/html/index.html) in the source code/GitHub.
 * Or you may build the documentation from the source code. See Sphinx Documentation later in this document.
 
 ## MFLib Installation
 
 ### Instaling via PIP
 MFLib may be installed using PIP and PyPI [fabrictestbed-mflib](https://pypi.org/project/fabrictestbed-mflib/)
 ```
@@ -50,15 +62,15 @@
 ```
 
 Build the documentation by running the following command from the root directory of the repo.
 ```
 ./create_html_doc.sh
 ```
 
-The completed documentation may be accessed by clicking on `/docs/build/html/index.html`
+The completed documentation may be accessed by clicking on `/docs/build/html/index.html`. Note that the HTML docs are not saved to the repository.
 
 #### Build PDF Document
 Latex must be installed. For Debian use: 
 ```
 sudo apt install texlive-latex-extra 
 sudo apt install latexmk
 
@@ -68,17 +80,15 @@
 ./create_pdf_doc.sh
 ```
 
 ### Distribution Package
 
 MFLib package is created using [Flit](https://flit.pypa.io/en/stable/)
 Be sure to create and commit the PDF documentation to GitHub before building and publishing to PyPi. The MFLib.pdf is included in the distributition.
-```
-python3 -m pip install flit
-```
+
 To build python package for PyPi run  
 ```
 ./create_release.sh
 ```
 
 #### Uploading to PyPI
 
@@ -87,7 +97,8 @@
 flit publish --repository testpypi 
 ```
 Once install is good, upload to PiPy  
 ```
 flit publish
 ```
 Note that Flit places a .pypirc file in your home directory if you do not already have one. Flit may also store your password in the keyring which may break if the password is changed. see [Flit Controlling package uploads](https://flit.pypa.io/en/stable/upload.html). The password can also be added to the .pypirc file. If password contains % signs it will break the .pypirc file.
+
```

### Comparing `fabrictestbed-mflib-0.1.0b1/create_html_doc.sh` & `fabrictestbed-mflib-0.2.0b0/create_html_doc.sh`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b1/create_pdf_doc.sh` & `fabrictestbed-mflib-0.2.0b0/create_pdf_doc.sh`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b1/create_release.sh` & `fabrictestbed-mflib-0.2.0b0/create_release.sh`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b1/docs/Makefile` & `fabrictestbed-mflib-0.2.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b1/docs/make.bat` & `fabrictestbed-mflib-0.2.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b1/docs/source/conf.py` & `fabrictestbed-mflib-0.2.0b0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b1/mflib/README.md` & `fabrictestbed-mflib-0.2.0b0/mflib/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b1/mflib/__init__.py` & `fabrictestbed-mflib-0.2.0b0/mflib/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 FABRIC Measurement Framework Python Client Library - Makes monitoring FABRIC Slice easy.
 """
 # release level is a alpha, b beta, rc candidate, dev development, post post,  or f final
 # (major, minor, micro, release level, release build)
-__version_info__ = [0, 1, 0, "b", 1]
+__version_info__ = [0, 2, 0, "b", 0]
 
 __version__ = f"{__version_info__[0]}.{__version_info__[1]}.{__version_info__[2]}"
 
 if __version_info__[3] != 'f':
     __version__ = f"{__version__}{__version_info__[3]}{__version_info__[4]}"
```

### Comparing `fabrictestbed-mflib-0.1.0b1/mflib/core.py` & `fabrictestbed-mflib-0.2.0b0/mflib/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,31 +24,28 @@
 
 import json
 import traceback
 import os
 
 from fabrictestbed_extensions.fablib.fablib import fablib
 
-# For getting vars to make tunnel
-from fabrictestbed_extensions.fablib.fablib import FablibManager
-
 
 import string
 import random
 
 import logging
 
 
 class Core:
     """
     MFLib core contains the core methods needed to create and interact with the Measurement Framework installed in a slice.
     It is not intended to be used by itself, but rather, it is the base object for creating Measurement Framework Library objects.
     """
 
-    core_class_version = "1.0.37"
+    core_class_version = "1.0.38"
 
     """
     An updatable version for debugging purposes to make sure the correct version of this file is being used. Anyone can update this value as they see fit.
     Should always be increasing.
 
     Returns:
         String: Version.sub-version.build
@@ -302,51 +299,23 @@
         Args:
             local_port (String): local port ie port on users machine
             remote_port (String): remote port ie port on Measurement Node
 
         Returns:
             String : SSH command string or error string.
         """
+        # These values from fabric_ssh_tunnel_tools.tgz obtained by user when configuring Fabric environment
+        private_key_file = "slice_key"
+        ssh_config = "ssh_config"
+
         slice_username = self.slice_username
         meas_node_ip = self.meas_node_ip
 
-        # User has setup an ssh config file
-        extra_fm = FablibManager()
-        errmsg = ""
-        ssh_config = ""
-        private_key_file = ""
-
-        extra_fm_vars = extra_fm.read_fabric_rc(extra_fm.default_fabric_rc)
-        if extra_fm_vars:
-            if "FABRIC_ALT_COPY_SSH_CONFIG" in extra_fm_vars:
-                ssh_config = extra_fm_vars["FABRIC_ALT_COPY_SSH_CONFIG"]
-            else:
-                #errmsg += "FABRIC_ALT_COPY_SSH_CONFIG not found in fabric_rc file. "
-                ssh_config = "~/fabric_tunnel_config/tunnel_ssh_config"
-
-            if "FABRIC_ALT_COPY_SLICE_PRIVATE_KEY_FILE" in extra_fm_vars:
-                private_key_file = extra_fm_vars[
-                    "FABRIC_ALT_COPY_SLICE_PRIVATE_KEY_FILE"
-                ]
-            else:
-                #errmsg += "FABRIC_ALT_COPY_SLICE_PRIVATE_KEY_FILE not found in fabric_rc file. "
-                private_key_file = "~/fabric_tunnel_config/slice_key"
-
-        if errmsg:
-            self.core_logger.error(
-                f"It appears you have not added alternate ssh config or slice key file locations to the fabric_rc file. {errmsg} "
-            )
-            return (
-                "It appears you have not added alternate ssh config or slice key file locations to the fabric_rc file. "
-                + errmsg
-            )
-        else:
-            # return f'ssh -L 10010:localhost:443 -F {extra_fm_vars["FABRIC_ALT_SSH_CONFIG"]} -i {extra_fm_vars["FABRIC_ALT_SLICE_PRIVATE_KEY_FILE"]} {self.slice_username}@{self.meas_node_ip}'
-            tunnel_cmd = f"ssh -L {local_port}:localhost:{remote_port} -F {ssh_config} -i {private_key_file} {slice_username}@{meas_node_ip}"
-            return tunnel_cmd
+        tunnel_cmd = f"ssh -L {local_port}:localhost:{remote_port} -F {ssh_config} -i {private_key_file} {slice_username}@{meas_node_ip}"
+        return tunnel_cmd
 
     """
     The git branch to be used for cloning the MeasurementFramework branch to the Measusrement Node.
     """
 
     def __init__(
         self,
@@ -436,14 +405,19 @@
 
         Args:
             service (String): The name of the service.
             data (JSON Serializable Object): Data to be passed to a JSON file place in the service's meas node directory.
         Returns:
             dict: Dictionary of info results.
         """
+        # Ensure service inputted is valid
+        if service not in self._get_service_list():
+            print("You must specify a valid service")
+            return {"success": False}
+
         self.core_logger.info(f"Run info for {service}")
         self.core_logger.debug(f"Data is {data}.")
         return self._run_on_meas_node(service, "info", data)
 
     def start(self, services=[]):
         """
         Restarts a stopped service using existing configs on meas node.
@@ -498,14 +472,27 @@
                 {
                     "service": service,
                     "results": self._run_on_meas_node(service, "remove"),
                 }
             )
 
     # Utility Methods
+    
+    def _get_service_list(self):
+        """
+        Gets a list of all currently existing services
+        :return: all currently existing services
+        :rtype: List
+        """
+        service_list = []
+        stdout, stderr = self.meas_node.execute(f"ls {self.services_directory}", quiet=True)
+        for item in stdout.split('\n'):
+            if item != "common" and item != "":
+                service_list.append(item)
+        return service_list
 
     def _upload_mfuser_keys(self, private_filename=None, public_filename=None):
         """
         Uploads the mfuser keys to the default user for easy access later.
 
         """
         if private_filename is None:
@@ -707,15 +694,14 @@
         :type files: List
         :raises: Exception: for misc failures....
         :return: ?
         :rtype: ?
         """
         letters = string.ascii_letters
 
-        # TODO could add option to upload a directory of files using fablib.upload_directory
         try:
             for file in files:
                 # Set src/dst filenames
                 # file is local path
                 local_file_path = file
                 filename = os.path.basename(file)
                 final_remote_file_path = os.path.join(
@@ -738,16 +724,62 @@
         except Exception as e:
             print(f"Service File Upload Failed: {e}")
             self.core_logger.exception("Upload service files failed")
             if stdout:
                 self.core_logger.debug(f"STDOUT: {stdout}")
             if stderr:
                 self.core_logger.debug(f"STDERR: {stderr}")
-            return False
-        return True
+            return {"success": False, "message": f"Service file upload failed: {e}"}
+        return {"success": True, "message": f"Service file {filename} uploaded successfully."}
+
+    def _upload_service_directory(self, service, local_directory_path, force=False):
+        """
+        Uploads the given local directory to the given service's directory on the meas node.
+        :param service: Service name for which the files are being upload to the meas node.
+        :type service: String
+        :param local_directory_path: List of file paths on local machine.
+        :type local_directory_path: String
+        :param force: Whether to overwrite existing directory, if it exists.
+        :type force: Bool
+        :raises: Exception: for misc failures....
+        :return: ?
+        :rtype: ?
+        """
+
+        local_directory_path = os.path.normpath(local_directory_path)
+        if not os.path.dirname(local_directory_path):
+            return {"success": False, "message": "The local directory does not exist."}
+        local_directory_name = os.path.basename(local_directory_path)
+
+        # Create a tmp spot for directory
+        letters = string.ascii_letters
+        rand_dir_name = "mf_dir_" + "".join(random.choice(letters) for i in range(10))
+        tmp_remote_directory_path = os.path.join("/tmp", rand_dir_name)
+
+        final_remote_directory_path = os.path.join(self.services_directory, service, "files")
+        
+        stdout, stderr = self.meas_node.execute(f"if test -d {final_remote_directory_path}/{local_directory_name}; then echo 'Directory exists'; else echo 'does not exist'; fi", quiet=True)
+        if "Directory exists" in stdout:
+            if force:
+                stdout, stderr = self.meas_node.execute(f"sudo rm -rf {final_remote_directory_path}/{local_directory_name}")
+            else:
+                return {"success": False, "message": "The selected directory already exists. Run command with force=True to overwrite it."}
+        
+        try:
+            # upload directory
+            self.meas_node.upload_directory(local_directory_path, tmp_remote_directory_path)
+            cmd = f"sudo mv -f {tmp_remote_directory_path}/{local_directory_name} {final_remote_directory_path};  sudo chown mfuser:mfuser {final_remote_directory_path}; sudo rm -rf {tmp_remote_directory_path}"
+            stdout, stderr = self.meas_node.execute(cmd)
+
+        except Exception as e:
+            self.core_logger.exception("Upload service directory failed")
+            if stdout: self.core_logger.debug(f"STDOUT: {stdout}")
+            if stderr: self.core_logger.debug(f"STDERR: {stderr}")
+            return {"success": False, "message": f"Service Directory Upload Failed: {e}"}
+        return {"success": True, "message": f"Service Directory {local_directory_name} uploaded successfully."}
 
     def _run_service_command(self, service, command):
         """
         Runs the given comand for the given service on the meas node.
 
         Args:
             service(String): Service name for which the command is being run on the meas node.
@@ -825,19 +857,18 @@
         # TODO figure out how to name/where to put file locally
         try:
             # local_file_path = os.path.join(self.local_slice_directory, service, filename)
             remote_file_path = os.path.join(self.services_directory, service, filename)
             file_attributes = self.meas_node.download_file(
                 local_file_path, remote_file_path
             )  # , retry=3, retry_interval=10):
-            return {"success": True, "filename": local_file_path}
+            return {"success": True, "message": "uploaded " + filename + " successfully."}
         except Exception as e:
-            print(f"Download service file Fail: {e}")
             self.core_logger.exception()
-            return {"success": False}
+            return {"success": False, "message": f"Download service file Fail: {e}"}
 
     def _clone_mf_repo(self):
         """
         Clones the MeasurementFramework  git repository to /home/mfuser/mf_git on the meas node.
         """
         msg = f"Cloning Measurement Framework Repository from github.com..."
         self.core_logger.debug(msg)
@@ -922,19 +953,22 @@
 
         Args:
             force(Boolean): If downloaded file already exists locally, it will not be downloaded unless force is True. .
         Returns:
             Dictionary: Bootstrap dict if any type of bootstraping has occured, Empty dict otherwise.
         """
         if force or not os.path.exists(self.bootstrap_status_file):
-            if not self._download_bootstrap_status():
-                # print("Bootstrap file was not downloaded. Bootstrap most likely has not been done.")
-                return {}
+            download_success, download_msg = self._download_bootstrap_status()
+            if not download_success:
+                return {"msg", download_msg }
 
         if os.path.exists(self.bootstrap_status_file):
+            if os.stat(self.bootstrap_status_file).st_size == 0:
+                return {}
+                # workaround download creating empty file if file not found
             with open(self.bootstrap_status_file) as bsf:
                 try:
                     bootstrap_dict = json.load(bsf)
                     # print(bootstrap_dict)
                     if bootstrap_dict:
                         return bootstrap_dict
                     else:
@@ -981,23 +1015,27 @@
             # print(local_file_path)
             # print(remote_file_path)
             file_attributes = self.meas_node.download_file(
                 local_file_path, remote_file_path, retry=1
             )  # , retry=3, retry_interval=10): # note retry is really tries
             # print(file_attributes)
 
-            return True
+            return True, ""
         except FileNotFoundError:
             pass
             # Most likely the file does not exist because it has not yet been created. So we will ignore this exception.
+            self.core_logger.warning("Bootstrap file not found on Measure Node")
+            return True, "File not found"
         except Exception as e:
-            print("Bootstrap download has failed.")
-            print(f"Fail: {e}")
-            return False
-        return False
+            msg = f"Bootstrap download has failed. Fail: {e}"
+            #print("Bootstrap download has failed.")
+            #print(f"Fail: {e}")
+            #return {"msg":msg, "success":False}
+            return False, msg
+        #return {}
 
     def get_mfuser_private_key(self, force=True):
         """
         Downloads the mfuser private key. Default setting of force will always download the most recent file from the meas node. The downloaded file will be stored locally for future reference at self.local_mfuser_private_key_filename.
 
 
         Args:
@@ -1069,14 +1107,19 @@
         :param service: The name of the service.
         :type service: String
         :param method: The method name such as create, update, info, start, stop, remove.
         :type method: String
         :return: Writes file to local storage and returns text of the log file.
         :rtype: String
         """
+        # Ensure service inputted is valid
+        if service not in self._get_service_list():
+            print("You must specify a valid service")
+            return {"success": False}
+
         try:
             local_file_path = os.path.join(self.local_slice_directory, f"{method}.log")
             remote_file_path = os.path.join(
                 "/", "home", "mfuser", "services", service, "log", f"{method}.log"
             )
             # print(local_file_path)
             # print(remote_file_path)
@@ -1089,7 +1132,81 @@
                 log_text = f.read()
                 return local_file_path, log_text
 
         except Exception as e:
             print("Service log download has failed.")
             print(f"Downloading service log file has Failed. It may not exist: {e}")
             return "", ""
+
+    def download_service_file(self, service, filename, local_file_path=""):
+        """
+        Downloads service files from the meas node and places them in the local storage directory.
+        Denies the user from downloading files anywhere outside the service directory
+        :param service: Service name
+        :type service: String
+        :param filename: The filename to download from the meas node.
+        :param local_file_path: Optional filename for local saved file.
+        :type local_file_path: String
+        """
+        # Ensure service inputted is valid
+        if service not in self._get_service_list():
+            print("You must specify a valid service")
+            return {"success": False}
+
+        # Ensure remote file path will be within the service directory.
+        if ".." in filename:
+            print("Error: Remote file must be within the service directory.")
+            return {"success": False}
+
+        # Call the internal download service file function
+        output = self._download_service_file(service, filename, local_file_path)
+        print(output)
+        return output
+
+    def upload_service_files(self, service, files):
+        """
+        Uploads the given local files to the given service's directory on the meas node.
+        Denies the user from uploading files anywhere outside the service directory
+        :param service: Service name for which the files are being upload to the meas node.
+        :type service: String
+        :param files: List of file paths on local machine.
+        :type files: List
+        :raises: Exception: for misc failures....
+        :return: ?
+        :rtype: ?
+        """
+
+        # Ensure service inputted is valid
+        if service not in self._get_service_list():
+            output = {"success": False, "message": "You must specify a valid service"}
+            print(output)
+            return output
+
+        # Call the internal upload service file function
+        output = self._upload_service_files(service, files)
+        print(output)
+        return output
+
+    def upload_service_directory(self, service, local_directory_path, force=False):
+        """
+        Uploads the given local directory to the given service's directory on the meas node.
+        :param service: Service name for which the files are being upload to the meas node.
+        :type service: String
+        :param local_directory_path: Directory path on local machine.
+        :type local_directory_path: String
+        :param force: Whether to overwrite existing directory, if it exists.
+        :type force: Bool
+        :raises: Exception: for misc failures....
+        :return: ?
+        :rtype: ?
+        """
+
+        # Ensure service inputted is valid
+        if service not in self._get_service_list():
+            output = {"success": False, "message": "You must specify a valid service"}
+            print(output)
+            return output
+
+        # Call the internal upload service directory function
+        output = self._upload_service_directory(service, local_directory_path, force)
+        print(output)
+        return output
```

### Comparing `fabrictestbed-mflib-0.1.0b1/mflib/mflib.py` & `fabrictestbed-mflib-0.2.0b0/mflib/mflib.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,17 @@
             f"Found meas node as {self.meas_node.get_name()} at {self.meas_node.get_management_ip()}"
         )
         self.mflib_logger.info(
             f"Found meas node as {self.meas_node.get_name()} at {self.meas_node.get_management_ip()}"
         )
 
         bss = self.get_bootstrap_status()
+        if "msg" in bss:
+            print(f"Bootstrap Download failed {bss['msg']}")
+            return False 
         if bss:
             # print("Bootstrap status is")
             # print(bss)
             self.mflib_logger.info("Bootstrap status is")
             self.mflib_logger.info(bss)
         else:
             print("Bootstrap status not found. Will now start bootstrap process...")
```

### Comparing `fabrictestbed-mflib-0.1.0b1/mflib/mfvis.py` & `fabrictestbed-mflib-0.2.0b0/mflib/mfvis.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b1/pyproject.toml` & `fabrictestbed-mflib-0.2.0b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b1/PKG-INFO` & `fabrictestbed-mflib-0.2.0b0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: fabrictestbed-mflib
-Version: 0.1.0b1
-Summary: FABRIC Measurement Framework Python Client Library - Makes monitoring FABRIC Slice easy.
-Author: Song, Pinyi, Hussam
-Author-email: Carpenter <csacarp0@g.uky.edu>
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Project-URL: Homepage, https://github.com/fabric-testbed/mflib
-
 # MFLIB Measurement Framework Library
 
 [![Documentation Status](https://readthedocs.org/projects/fabrictestbed-mflib/badge/?version=latest)](https://fabrictestbed-mflib.readthedocs.io/en/latest/?badge=latest)
 
 Welcome to the FABRIC Measurement Framework Library. MFLib makes it easy to install monitoring systems to a FABRIC experimenter's slice. The monitoring system makes extensive use of industry standards such as Prometheus, Grafana, Elastic Search and Kibana while adding customized monitoring tools and dashboards for quick setup and visualization.
 
 ## Documentation Resources
@@ -25,15 +12,14 @@
 ### FABRIC Learn Site
 [FABRIC Knowledge Base](https://learn.fabric-testbed.net/) 
 
 ### MFLib Python Package Documentation
 Documentation for the package is presented in serveral different forms (and maybe include later in this document):
 * [ReadTheDocs](https://fabrictestbed-mflib.readthedocs.io/en/latest/)
 * [MFLib.pdf](https://github.com/fabric-testbed/mflib/blob/main/MFLib.pdf) in the source code/GitHub.
-* [MFLib HTML Index](https://github.com/fabric-testbed/mflib/blob/main/docs/html/index.html) in the source code/GitHub.
 * Or you may build the documentation from the source code. See Sphinx Documentation later in this document.
 
 ## MFLib Installation
 
 ### Instaling via PIP
 MFLib may be installed using PIP and PyPI [fabrictestbed-mflib](https://pypi.org/project/fabrictestbed-mflib/)
 ```
@@ -63,15 +49,15 @@
 ```
 
 Build the documentation by running the following command from the root directory of the repo.
 ```
 ./create_html_doc.sh
 ```
 
-The completed documentation may be accessed by clicking on `/docs/build/html/index.html`
+The completed documentation may be accessed by clicking on `/docs/build/html/index.html`. Note that the HTML docs are not saved to the repository.
 
 #### Build PDF Document
 Latex must be installed. For Debian use: 
 ```
 sudo apt install texlive-latex-extra 
 sudo apt install latexmk
 
@@ -81,17 +67,15 @@
 ./create_pdf_doc.sh
 ```
 
 ### Distribution Package
 
 MFLib package is created using [Flit](https://flit.pypa.io/en/stable/)
 Be sure to create and commit the PDF documentation to GitHub before building and publishing to PyPi. The MFLib.pdf is included in the distributition.
-```
-python3 -m pip install flit
-```
+
 To build python package for PyPi run  
 ```
 ./create_release.sh
 ```
 
 #### Uploading to PyPI
 
@@ -100,8 +84,7 @@
 flit publish --repository testpypi 
 ```
 Once install is good, upload to PiPy  
 ```
 flit publish
 ```
 Note that Flit places a .pypirc file in your home directory if you do not already have one. Flit may also store your password in the keyring which may break if the password is changed. see [Flit Controlling package uploads](https://flit.pypa.io/en/stable/upload.html). The password can also be added to the .pypirc file. If password contains % signs it will break the .pypirc file.
-
```

