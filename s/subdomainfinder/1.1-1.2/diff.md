# Comparing `tmp/subdomainfinder-1.1.tar.gz` & `tmp/subdomainfinder-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subdomainfinder-1.1.tar", last modified: Wed Apr 19 20:10:26 2023, max compression
+gzip compressed data, was "subdomainfinder-1.2.tar", last modified: Thu Apr 20 20:54:37 2023, max compression
```

## Comparing `subdomainfinder-1.1.tar` & `subdomainfinder-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwx------   0 u0_a189  (10189) u0_a189  (10189)        0 2023-04-19 20:10:26.751889 subdomainfinder-1.1/
--rw-------   0 u0_a189  (10189) u0_a189  (10189)     1792 2023-04-19 20:10:26.751889 subdomainfinder-1.1/PKG-INFO
--rw-------   0 u0_a189  (10189) u0_a189  (10189)      984 2023-04-19 19:02:43.000000 subdomainfinder-1.1/README.md
--rw-------   0 u0_a189  (10189) u0_a189  (10189)       38 2023-04-19 20:10:26.751889 subdomainfinder-1.1/setup.cfg
--rw-------   0 u0_a189  (10189) u0_a189  (10189)     1217 2023-04-19 20:10:09.000000 subdomainfinder-1.1/setup.py
-drwx------   0 u0_a189  (10189) u0_a189  (10189)        0 2023-04-19 20:10:26.748556 subdomainfinder-1.1/subdomainfinder/
--rw-------   0 u0_a189  (10189) u0_a189  (10189)     6137 2023-04-19 20:07:30.000000 subdomainfinder-1.1/subdomainfinder/__init__.py
--rw-------   0 u0_a189  (10189) u0_a189  (10189)       89 2023-04-19 20:09:04.000000 subdomainfinder-1.1/subdomainfinder/__main__.py
-drwx------   0 u0_a189  (10189) u0_a189  (10189)        0 2023-04-19 20:10:26.751889 subdomainfinder-1.1/subdomainfinder.egg-info/
--rw-------   0 u0_a189  (10189) u0_a189  (10189)     1792 2023-04-19 20:10:26.000000 subdomainfinder-1.1/subdomainfinder.egg-info/PKG-INFO
--rw-------   0 u0_a189  (10189) u0_a189  (10189)      310 2023-04-19 20:10:26.000000 subdomainfinder-1.1/subdomainfinder.egg-info/SOURCES.txt
--rw-------   0 u0_a189  (10189) u0_a189  (10189)        1 2023-04-19 20:10:26.000000 subdomainfinder-1.1/subdomainfinder.egg-info/dependency_links.txt
--rw-------   0 u0_a189  (10189) u0_a189  (10189)       67 2023-04-19 20:10:26.000000 subdomainfinder-1.1/subdomainfinder.egg-info/entry_points.txt
--rw-------   0 u0_a189  (10189) u0_a189  (10189)       14 2023-04-19 20:10:26.000000 subdomainfinder-1.1/subdomainfinder.egg-info/requires.txt
--rw-------   0 u0_a189  (10189) u0_a189  (10189)       26 2023-04-19 20:10:26.000000 subdomainfinder-1.1/subdomainfinder.egg-info/top_level.txt
+drwx------   0 u0_a189  (10189) u0_a189  (10189)        0 2023-04-20 20:54:37.757597 subdomainfinder-1.2/
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)     1788 2023-04-20 20:54:37.757597 subdomainfinder-1.2/PKG-INFO
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)      984 2023-04-19 19:02:43.000000 subdomainfinder-1.2/README.md
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)       38 2023-04-20 20:54:37.760930 subdomainfinder-1.2/setup.cfg
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)     1256 2023-04-20 20:48:24.000000 subdomainfinder-1.2/setup.py
+drwx------   0 u0_a189  (10189) u0_a189  (10189)        0 2023-04-20 20:54:37.757597 subdomainfinder-1.2/subdomainfinder/
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)     6211 2023-04-20 20:51:07.000000 subdomainfinder-1.2/subdomainfinder/__init__.py
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)       89 2023-04-19 20:09:04.000000 subdomainfinder-1.2/subdomainfinder/__main__.py
+drwx------   0 u0_a189  (10189) u0_a189  (10189)        0 2023-04-20 20:54:37.757597 subdomainfinder-1.2/subdomainfinder.egg-info/
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)     1788 2023-04-20 20:54:37.000000 subdomainfinder-1.2/subdomainfinder.egg-info/PKG-INFO
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)      310 2023-04-20 20:54:37.000000 subdomainfinder-1.2/subdomainfinder.egg-info/SOURCES.txt
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)        1 2023-04-20 20:54:37.000000 subdomainfinder-1.2/subdomainfinder.egg-info/dependency_links.txt
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)       67 2023-04-20 20:54:37.000000 subdomainfinder-1.2/subdomainfinder.egg-info/entry_points.txt
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)       14 2023-04-20 20:54:37.000000 subdomainfinder-1.2/subdomainfinder.egg-info/requires.txt
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)       26 2023-04-20 20:54:37.000000 subdomainfinder-1.2/subdomainfinder.egg-info/top_level.txt
```

### Comparing `subdomainfinder-1.1/PKG-INFO` & `subdomainfinder-1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: subdomainfinder
-Version: 1.1
+Version: 1.2
 Summary: A python based tool for finding subdomains of a domain.
 Home-page: https://github.com/ankushbhagatofficial/subdomain-finder
 Author: Ankush Bhagat
 Author-email: <ankushbhagatofficial@gmail.com>
-License: UNKNOWN
+License: MIT
 Description: 
         <h1 align="center">subdomainfinder</h1>
         
         <p align="center">
         A program to find subdomain of any domain.
         </p>
```

### Comparing `subdomainfinder-1.1/README.md` & `subdomainfinder-1.2/README.md`

 * *Files identical despite different names*

### Comparing `subdomainfinder-1.1/setup.py` & `subdomainfinder-1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "PYPIREADME.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1'
+VERSION = '1.2'
 DESCRIPTION = 'A python based tool for finding subdomains of a domain.'
 
 # Setting up
 setup(
     name='subdomainfinder',
     version=VERSION,
+    platform='all',
     author='Ankush Bhagat',
     author_email="<ankushbhagatofficial@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
+    license='MIT',
     url='https://github.com/ankushbhagatofficial/subdomain-finder',
     packages=find_packages(),
     py_modules=['subfinder'],
     install_requires=[
         'requests',
         'rich'
     ],
```

### Comparing `subdomainfinder-1.1/subdomainfinder/__init__.py` & `subdomainfinder-1.2/subdomainfinder/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import requests
 import json
-import os, sys, signal
+import os, sys, signal, platform
 import time
 import logging
 from rich.progress import Progress, SpinnerColumn, TimeElapsedColumn
 from rich.logging import RichHandler
 from rich.console import Console
 from rich.align import Align
 from rich.panel import Panel
 from rich.syntax import Syntax
 from rich.traceback import install
 install()
 
+mysys = platform.uname()
+
 # Define a signal handler for SIGTSTP and SIGTSTP
 def signal_handler(signal, frame):
 #    print("Program exit.")
     sys.stdout.write('\rProgram exit.                           ')
     sys.stdout.flush()
     print()
     sys.exit()
 
-signal.signal(signal.SIGTSTP, signal_handler)
-signal.signal(signal.SIGINT, signal_handler)
+if not mysys.system == "Windows":
+    signal.signal(signal.SIGTSTP, signal_handler)
 
+signal.signal(signal.SIGINT, signal_handler)
 
 FORMAT = "%(message)s"
 logging.basicConfig(
     level="NOTSET", format=FORMAT, datefmt="[%X]", handlers=[RichHandler()]
 )
 
 log = logging.getLogger("rich")
```

### Comparing `subdomainfinder-1.1/subdomainfinder.egg-info/PKG-INFO` & `subdomainfinder-1.2/subdomainfinder.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: subdomainfinder
-Version: 1.1
+Version: 1.2
 Summary: A python based tool for finding subdomains of a domain.
 Home-page: https://github.com/ankushbhagatofficial/subdomain-finder
 Author: Ankush Bhagat
 Author-email: <ankushbhagatofficial@gmail.com>
-License: UNKNOWN
+License: MIT
 Description: 
         <h1 align="center">subdomainfinder</h1>
         
         <p align="center">
         A program to find subdomain of any domain.
         </p>
```

