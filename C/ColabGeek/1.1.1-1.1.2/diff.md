# Comparing `tmp/ColabGeek-1.1.1.tar.gz` & `tmp/ColabGeek-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ColabGeek-1.1.1.tar", last modified: Tue Apr 18 03:18:11 2023, max compression
+gzip compressed data, was "ColabGeek-1.1.2.tar", last modified: Thu Apr 20 17:18:36 2023, max compression
```

## Comparing `ColabGeek-1.1.1.tar` & `ColabGeek-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 03:18:11.984721 ColabGeek-1.1.1/
--rw-rw-r--   0 root         (0) root         (0)     1067 2023-04-18 03:15:02.000000 ColabGeek-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5602 2023-04-18 03:18:11.984721 ColabGeek-1.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4865 2023-04-18 03:15:02.000000 ColabGeek-1.1.1/README.md
--rw-rw-r--   0 root         (0) root         (0)      939 2023-04-18 03:15:02.000000 ColabGeek-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 03:18:11.984721 ColabGeek-1.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 03:18:11.982721 ColabGeek-1.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 03:18:11.983721 ColabGeek-1.1.1/src/ColabGeek/
--rw-rw-r--   0 root         (0) root         (0)     6993 2023-04-18 03:15:02.000000 ColabGeek-1.1.1/src/ColabGeek/ColabGeek.py
--rw-rw-r--   0 root         (0) root         (0)       24 2023-04-18 03:15:02.000000 ColabGeek-1.1.1/src/ColabGeek/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 03:18:11.984721 ColabGeek-1.1.1/src/ColabGeek/shell_scripts/
--rw-rw-r--   0 root         (0) root         (0)      382 2023-04-18 03:15:02.000000 ColabGeek-1.1.1/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
--rw-rw-r--   0 root         (0) root         (0)     1192 2023-04-18 03:15:02.000000 ColabGeek-1.1.1/src/ColabGeek/shell_scripts/Run_code_server.exp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 03:18:11.983721 ColabGeek-1.1.1/src/ColabGeek.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5602 2023-04-18 03:18:11.000000 ColabGeek-1.1.1/src/ColabGeek.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-04-18 03:18:11.000000 ColabGeek-1.1.1/src/ColabGeek.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 03:18:11.000000 ColabGeek-1.1.1/src/ColabGeek.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-18 03:18:11.000000 ColabGeek-1.1.1/src/ColabGeek.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:36.209597 ColabGeek-1.1.2/
+-rw-rw-r--   0 root         (0) root         (0)     1067 2023-04-20 16:19:47.000000 ColabGeek-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6380 2023-04-20 17:18:36.208597 ColabGeek-1.1.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5643 2023-04-20 17:14:39.000000 ColabGeek-1.1.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)      939 2023-04-20 17:14:39.000000 ColabGeek-1.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 17:18:36.209597 ColabGeek-1.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:36.206596 ColabGeek-1.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:36.207596 ColabGeek-1.1.2/src/ColabGeek/
+-rw-rw-r--   0 root         (0) root         (0)     7849 2023-04-20 17:14:39.000000 ColabGeek-1.1.2/src/ColabGeek/ColabGeek.py
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-04-20 16:19:47.000000 ColabGeek-1.1.2/src/ColabGeek/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:36.208597 ColabGeek-1.1.2/src/ColabGeek/shell_scripts/
+-rw-rw-r--   0 root         (0) root         (0)      382 2023-04-20 16:19:47.000000 ColabGeek-1.1.2/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
+-rw-rw-r--   0 root         (0) root         (0)     1192 2023-04-20 16:19:47.000000 ColabGeek-1.1.2/src/ColabGeek/shell_scripts/Run_code_server.exp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:36.208597 ColabGeek-1.1.2/src/ColabGeek.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6380 2023-04-20 17:18:36.000000 ColabGeek-1.1.2/src/ColabGeek.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-04-20 17:18:36.000000 ColabGeek-1.1.2/src/ColabGeek.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 17:18:36.000000 ColabGeek-1.1.2/src/ColabGeek.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-20 17:18:36.000000 ColabGeek-1.1.2/src/ColabGeek.egg-info/top_level.txt
```

### Comparing `ColabGeek-1.1.1/LICENSE` & `ColabGeek-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.1.1/PKG-INFO` & `ColabGeek-1.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.1.1
+Version: 1.1.2
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ColabGeek
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/yimingsun12138/ColabGeek/blob/main/LICENSE)
+[![PyPI version](https://badge.fury.io/py/ColabGeek.svg)](https://badge.fury.io/py/ColabGeek)
+
 ColabGeek Python package is designed to help run useful tools on Google Colab, including web IDE, port forwarding and so on. It is worth noting that this package is also compatible with other Ubuntu operating system based servers, so try this package on other platforms as well.
 
 ## Installation
 
 ```python
 pip install ColabGeek
 ```
@@ -59,14 +62,27 @@
 # ColabGeek.Install_code_server_extension has the following parameters:
 # - extension The extension id or the path of the VSIX file.
 # - verbose Show the running logs.
 
 main.Install_code_server_extension(extension='ms-python.anaconda-extension-pack')
 ```
 
+You can also config code server through `ColabGeek.Config_code_server` method.
+
+```python
+# ColabGeek.Config_code_server has the following parameters:
+# - property Matching the key in settings.json config file.
+# - value Matching the value in settings.json config file.
+
+main.Config_code_server(property='workbench.colorTheme',value='Default Dark+')
+main.Config_code_server(property='editor.fontSize',value=18)
+main.Config_code_server(property='terminal.integrated.fontSize',value=18)
+main.Config_code_server(property='files.autoSave',value='off')
+```
+
 ### Run Rstudio server
 
 [Rstudio server](https://posit.co/products/open-source/rstudio-server/) is a web IDE for R programming. With Rstudio server, users can run R scripts, create and manage R projects, develop and test code, and share their work with others. Rstudio server also offers powerful features such as syntax highlighting, code completion, debugging and data visualization.
 
 ```python
 # ColabGeek.Run_Rstudio_server has the following parameters:
 # - port The port you want to run Rstudio on, set to None to use the default port.
@@ -112,8 +128,8 @@
 # - encrypt The shadowsocks encrypt method.
 
 main.Run_shadowsocks()
 ```
 
 ## Statement
 
-ColabGeek violated numerous community rules of Google Colab. But still, I developed ColabGeek, because the simple Jupyter interface just does not meet the requirements of many software applications and is not user-friendly for coding in non-Python languages. I recommend all ColabGeek users can purchase Colab Pro or Pro+ to support the excellent services provided by Google. Keep in mind, avoid misuse and Don't Be Evil.
+ColabGeek violated numerous community rules of Google Colab. But still, I developed ColabGeek, because the simple Jupyter interface just does not meet the requirements of many software applications and is not user-friendly for coding in non-Python languages. I recommend all ColabGeek users purchase Colab Pro or Pro+ to support the excellent services provided by Google. Keep in mind, avoid misuse and Don't Be Evil.
```

### Comparing `ColabGeek-1.1.1/README.md` & `ColabGeek-1.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # ColabGeek
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/yimingsun12138/ColabGeek/blob/main/LICENSE)
+[![PyPI version](https://badge.fury.io/py/ColabGeek.svg)](https://badge.fury.io/py/ColabGeek)
+
 ColabGeek Python package is designed to help run useful tools on Google Colab, including web IDE, port forwarding and so on. It is worth noting that this package is also compatible with other Ubuntu operating system based servers, so try this package on other platforms as well.
 
 ## Installation
 
 ```python
 pip install ColabGeek
 ```
@@ -45,14 +48,27 @@
 # ColabGeek.Install_code_server_extension has the following parameters:
 # - extension The extension id or the path of the VSIX file.
 # - verbose Show the running logs.
 
 main.Install_code_server_extension(extension='ms-python.anaconda-extension-pack')
 ```
 
+You can also config code server through `ColabGeek.Config_code_server` method.
+
+```python
+# ColabGeek.Config_code_server has the following parameters:
+# - property Matching the key in settings.json config file.
+# - value Matching the value in settings.json config file.
+
+main.Config_code_server(property='workbench.colorTheme',value='Default Dark+')
+main.Config_code_server(property='editor.fontSize',value=18)
+main.Config_code_server(property='terminal.integrated.fontSize',value=18)
+main.Config_code_server(property='files.autoSave',value='off')
+```
+
 ### Run Rstudio server
 
 [Rstudio server](https://posit.co/products/open-source/rstudio-server/) is a web IDE for R programming. With Rstudio server, users can run R scripts, create and manage R projects, develop and test code, and share their work with others. Rstudio server also offers powerful features such as syntax highlighting, code completion, debugging and data visualization.
 
 ```python
 # ColabGeek.Run_Rstudio_server has the following parameters:
 # - port The port you want to run Rstudio on, set to None to use the default port.
@@ -98,8 +114,8 @@
 # - encrypt The shadowsocks encrypt method.
 
 main.Run_shadowsocks()
 ```
 
 ## Statement
 
-ColabGeek violated numerous community rules of Google Colab. But still, I developed ColabGeek, because the simple Jupyter interface just does not meet the requirements of many software applications and is not user-friendly for coding in non-Python languages. I recommend all ColabGeek users can purchase Colab Pro or Pro+ to support the excellent services provided by Google. Keep in mind, avoid misuse and Don't Be Evil.
+ColabGeek violated numerous community rules of Google Colab. But still, I developed ColabGeek, because the simple Jupyter interface just does not meet the requirements of many software applications and is not user-friendly for coding in non-Python languages. I recommend all ColabGeek users purchase Colab Pro or Pro+ to support the excellent services provided by Google. Keep in mind, avoid misuse and Don't Be Evil.
```

### Comparing `ColabGeek-1.1.1/pyproject.toml` & `ColabGeek-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 "ColabGeek.shell_scripts" = ["*"]
 
 [project]
 name = "ColabGeek"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
     {name = "Yiming Sun",email = "yiming.sun12138@gmail.com"},
 ]
 description = "ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ColabGeek-1.1.1/src/ColabGeek/ColabGeek.py` & `ColabGeek-1.1.2/src/ColabGeek/ColabGeek.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 '''
 import dependent modules.
 '''
 import os
 import sys
 import time
+import json
 
 '''
 define ColabSession class
 '''
 class ColabSession:
     def __init__(self,user,password,sudo = True,port = 8787,mount_GD = False,keep_busy = True):
         self.user = user
@@ -158,14 +159,35 @@
 
     def Install_code_server_extension(self,extension,verbose = True):
         char_cmd = "sudo -u" + " " + str(self.user) + " " + "code-server --install-extension" + " " + str(extension)
         exec_logging = os.popen(char_cmd)
         if verbose:
             exec_logging = ''.join(exec_logging.readlines())
             print(exec_logging)
+
+    def Config_code_server(self,property,value):
+        # check whether settings.json exists
+        file_path = "/home/" + str(self.user) + "/.local/share/code-server/User"
+        char_cmd = "sudo -u" + " " + str(self.user) + " " + "mkdir -p" + " " + file_path
+        os.system(char_cmd)
+        file_path = file_path + "/settings.json"
+        if os.path.exists(file_path):
+            with open(file_path,"r") as json_file:
+                json_setting = json.load(json_file)
+        else:
+            char_cmd = "sudo -u" + " " + str(self.user) + " " + "touch" + " " + file_path
+            os.system(char_cmd)
+            json_setting = {}
+
+        # add property
+        json_setting[str(property)] = value
+
+        # dump settings
+        with open(file_path,"w") as json_file:
+            json.dump(json_setting,json_file,indent=4)
             
     '''
     proxy method
     '''
     # run shadowsocks
     def Run_shadowsocks(self,port = None,password = None,encrypt = 'aes-256-gcm'):
         # check param
```

### Comparing `ColabGeek-1.1.1/src/ColabGeek/shell_scripts/Run_code_server.exp` & `ColabGeek-1.1.2/src/ColabGeek/shell_scripts/Run_code_server.exp`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.1.1/src/ColabGeek.egg-info/PKG-INFO` & `ColabGeek-1.1.2/src/ColabGeek.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.1.1
+Version: 1.1.2
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ColabGeek
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/yimingsun12138/ColabGeek/blob/main/LICENSE)
+[![PyPI version](https://badge.fury.io/py/ColabGeek.svg)](https://badge.fury.io/py/ColabGeek)
+
 ColabGeek Python package is designed to help run useful tools on Google Colab, including web IDE, port forwarding and so on. It is worth noting that this package is also compatible with other Ubuntu operating system based servers, so try this package on other platforms as well.
 
 ## Installation
 
 ```python
 pip install ColabGeek
 ```
@@ -59,14 +62,27 @@
 # ColabGeek.Install_code_server_extension has the following parameters:
 # - extension The extension id or the path of the VSIX file.
 # - verbose Show the running logs.
 
 main.Install_code_server_extension(extension='ms-python.anaconda-extension-pack')
 ```
 
+You can also config code server through `ColabGeek.Config_code_server` method.
+
+```python
+# ColabGeek.Config_code_server has the following parameters:
+# - property Matching the key in settings.json config file.
+# - value Matching the value in settings.json config file.
+
+main.Config_code_server(property='workbench.colorTheme',value='Default Dark+')
+main.Config_code_server(property='editor.fontSize',value=18)
+main.Config_code_server(property='terminal.integrated.fontSize',value=18)
+main.Config_code_server(property='files.autoSave',value='off')
+```
+
 ### Run Rstudio server
 
 [Rstudio server](https://posit.co/products/open-source/rstudio-server/) is a web IDE for R programming. With Rstudio server, users can run R scripts, create and manage R projects, develop and test code, and share their work with others. Rstudio server also offers powerful features such as syntax highlighting, code completion, debugging and data visualization.
 
 ```python
 # ColabGeek.Run_Rstudio_server has the following parameters:
 # - port The port you want to run Rstudio on, set to None to use the default port.
@@ -112,8 +128,8 @@
 # - encrypt The shadowsocks encrypt method.
 
 main.Run_shadowsocks()
 ```
 
 ## Statement
 
-ColabGeek violated numerous community rules of Google Colab. But still, I developed ColabGeek, because the simple Jupyter interface just does not meet the requirements of many software applications and is not user-friendly for coding in non-Python languages. I recommend all ColabGeek users can purchase Colab Pro or Pro+ to support the excellent services provided by Google. Keep in mind, avoid misuse and Don't Be Evil.
+ColabGeek violated numerous community rules of Google Colab. But still, I developed ColabGeek, because the simple Jupyter interface just does not meet the requirements of many software applications and is not user-friendly for coding in non-Python languages. I recommend all ColabGeek users purchase Colab Pro or Pro+ to support the excellent services provided by Google. Keep in mind, avoid misuse and Don't Be Evil.
```

