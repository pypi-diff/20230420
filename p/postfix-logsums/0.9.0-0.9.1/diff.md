# Comparing `tmp/postfix_logsums-0.9.0.tar.gz` & `tmp/postfix_logsums-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postfix_logsums-0.9.0.tar", last modified: Wed Apr 19 16:24:37 2023, max compression
+gzip compressed data, was "postfix_logsums-0.9.1.tar", last modified: Thu Apr 20 07:50:26 2023, max compression
```

## Comparing `postfix_logsums-0.9.0.tar` & `postfix_logsums-0.9.1.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:37.097709 postfix_logsums-0.9.0/
--rw-r--r--   0 root         (0) root         (0)     7652 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2225 2023-04-19 16:24:37.097709 postfix_logsums-0.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      987 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/README.md
--rwxr-xr-x   0 root         (0) root         (0)     1091 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/postfix-logsums
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:37.093709 postfix_logsums-0.9.0/postfix_logsums/
--rw-r--r--   0 root         (0) root         (0)    63893 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/postfix_logsums/__init__.py
--rw-r--r--   0 root         (0) root         (0)    74500 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/postfix_logsums/app.py
--rw-r--r--   0 root         (0) root         (0)     7699 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/postfix_logsums/errors.py
--rw-r--r--   0 root         (0) root         (0)     7965 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/postfix_logsums/results.py
--rw-r--r--   0 root         (0) root         (0)    31716 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/postfix_logsums/stats.py
--rw-r--r--   0 root         (0) root         (0)     2943 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/postfix_logsums/xlate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:37.097709 postfix_logsums-0.9.0/postfix_logsums.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2225 2023-04-19 16:24:37.000000 postfix_logsums-0.9.0/postfix_logsums.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      443 2023-04-19 16:24:37.000000 postfix_logsums-0.9.0/postfix_logsums.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 16:24:37.000000 postfix_logsums-0.9.0/postfix_logsums.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-19 16:24:37.000000 postfix_logsums-0.9.0/postfix_logsums.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1125 2023-04-19 16:24:37.097709 postfix_logsums-0.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4364 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:37.097709 postfix_logsums-0.9.0/test/
--rwxr-xr-x   0 root         (0) root         (0)     7285 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/test/test_00_errors.py
--rwxr-xr-x   0 root         (0) root         (0)    13220 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/test/test_05_stats_collections.py
--rwxr-xr-x   0 root         (0) root         (0)     2411 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/test/test_10_results.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.475744 postfix_logsums-0.9.1/
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-04-20 07:50:26.475744 postfix_logsums-0.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      987 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.471744 postfix_logsums-0.9.1/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.471744 postfix_logsums-0.9.1/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.471744 postfix_logsums-0.9.1/locale/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    20693 2023-04-20 07:50:26.000000 postfix_logsums-0.9.1/locale/de/LC_MESSAGES/postfix_logsums.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.471744 postfix_logsums-0.9.1/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.471744 postfix_logsums-0.9.1/locale/en/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      940 2023-04-20 07:50:26.000000 postfix_logsums-0.9.1/locale/en/LC_MESSAGES/postfix_logsums.mo
+-rwxr-xr-x   0 root         (0) root         (0)     1091 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/postfix-logsums
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.471744 postfix_logsums-0.9.1/postfix_logsums/
+-rw-r--r--   0 root         (0) root         (0)    63893 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/postfix_logsums/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    74500 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/postfix_logsums/app.py
+-rw-r--r--   0 root         (0) root         (0)     7699 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/postfix_logsums/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7965 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/postfix_logsums/results.py
+-rw-r--r--   0 root         (0) root         (0)    31716 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/postfix_logsums/stats.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/postfix_logsums/xlate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.471744 postfix_logsums-0.9.1/postfix_logsums.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-04-20 07:50:26.000000 postfix_logsums-0.9.1/postfix_logsums.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      525 2023-04-20 07:50:26.000000 postfix_logsums-0.9.1/postfix_logsums.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 07:50:26.000000 postfix_logsums-0.9.1/postfix_logsums.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-20 07:50:26.000000 postfix_logsums-0.9.1/postfix_logsums.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-04-20 07:50:26.475744 postfix_logsums-0.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6273 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.475744 postfix_logsums-0.9.1/test/
+-rwxr-xr-x   0 root         (0) root         (0)     7285 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/test/test_00_errors.py
+-rwxr-xr-x   0 root         (0) root         (0)    13220 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/test/test_05_stats_collections.py
+-rwxr-xr-x   0 root         (0) root         (0)     2411 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/test/test_10_results.py
```

### Comparing `postfix_logsums-0.9.0/LICENSE` & `postfix_logsums-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.0/PKG-INFO` & `postfix_logsums-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postfix_logsums
-Version: 0.9.0
+Version: 0.9.1
 Summary: Produce Postfix MTA logfile summary
 Home-page: https://github.com/pixelpark/postfix-logsums
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `postfix_logsums-0.9.0/README.md` & `postfix_logsums-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.0/postfix-logsums` & `postfix_logsums-0.9.1/postfix-logsums`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.0/postfix_logsums/__init__.py` & `postfix_logsums-0.9.1/postfix_logsums/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 from .results import PostfixLogSums
 
 from .stats import MessageStats, MessageStatsPerDay, SmtpdStats
 
 from .xlate import XLATOR
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
 __copyright__ = '(C) 2023 by Frank Brehm, Berlin'
 
 DEFAULT_TERMINAL_WIDTH = 99
 DEFAULT_TERMINAL_HEIGHT = 40
 MAX_TERMINAL_WIDTH = 150
```

### Comparing `postfix_logsums-0.9.0/postfix_logsums/app.py` & `postfix_logsums-0.9.1/postfix_logsums/app.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.0/postfix_logsums/errors.py` & `postfix_logsums-0.9.1/postfix_logsums/errors.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.0/postfix_logsums/results.py` & `postfix_logsums-0.9.1/postfix_logsums/results.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.0/postfix_logsums/stats.py` & `postfix_logsums-0.9.1/postfix_logsums/stats.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.0/postfix_logsums/xlate.py` & `postfix_logsums-0.9.1/postfix_logsums/xlate.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.0/postfix_logsums.egg-info/PKG-INFO` & `postfix_logsums-0.9.1/postfix_logsums.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postfix-logsums
-Version: 0.9.0
+Version: 0.9.1
 Summary: Produce Postfix MTA logfile summary
 Home-page: https://github.com/pixelpark/postfix-logsums
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `postfix_logsums-0.9.0/setup.cfg` & `postfix_logsums-0.9.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 	Topic :: Communications :: Email :: Mail Transport Agents
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: System :: Systems Administration
 
 [options]
 packages = find:
 
+[compile_catalog]
+domain = postfix_logsums
+directory = locale
+statistics = 1
+
 [pep8]
 max-line-length = 99
 
 [flake8]
 max-line-length = 99
 max-complexity = 20
 ignore = E226,E302,E41,E402,W503
```

### Comparing `postfix_logsums-0.9.0/setup.py` & `postfix_logsums-0.9.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,32 +11,41 @@
 
 from __future__ import print_function
 
 import os
 import sys
 import re
 import pprint
+import glob
+import subprocess
 
 from pathlib import Path
 
 # Third party modules
 from setuptools import setup
+from setuptools.command.sdist import sdist
+
+from babel.messages import frontend as babel
 
 # own modules:
 __module_name__ = 'postfix_logsums'
 __setup_script__ = Path(__file__).resolve()
 __base_dir__ = __setup_script__.parent
 __module_dir__ = __base_dir__ / __module_name__
 __init_py__ = __module_dir__ / '__init__.py'
+__share_dir__ = Path(sys.base_prefix) / 'share'
+__locale_dir__ = __share_dir__ / 'locale'
 
 PATHS = {
     '__setup_script__': str(__setup_script__),
     '__base_dir__': str(__base_dir__),
     '__module_dir__': str(__module_dir__),
     '__init_py__': str(__init_py__),
+    '__share_dir__': __share_dir__,
+    '__locale_dir__': __locale_dir__,
 }
 
 def pp(obj):
     """Human friendly output of data structures."""
     pprinter = pprint.PrettyPrinter(indent=4)
     return pprinter.pformat(obj)
 
@@ -156,17 +165,73 @@
 read_requirements()
 
 # -----------------------------------
 __scripts__ = ['postfix-logsums']
 
 
 # -----------------------------------
+PO_FILES = 'locale/*/LC_MESSAGES/*.po'
+__package_data__ = {}
+__data_files__ = []
+
+def create_mo_files():
+    """Compile the translation files."""
+    mo_files = []
+    for po_path in glob.glob(PO_FILES):
+        mo = Path(po_path.replace('.po', '.mo'))
+        if not mo.exists():
+            subprocess.call(['msgfmt', '-o', str(mo), po_path])
+        mo_files.append(mo)
+
+    # print("Found mo files: {}\n".format(pp(mo_files)))
+    return mo_files
+
+
+__pkg_mo_paths__ = create_mo_files()
+__pkg_mo_files__ = []
+for mo_file in __pkg_mo_paths__:
+    __pkg_mo_files__.append(str(mo_file))
+
+__package_data__[''] = __pkg_mo_files__
+# print("Package_data:\n" + pp(__package_data__) + "\n")
+
+
+for mo_file in __pkg_mo_paths__:
+    ltype = mo_file.parent.name
+    lname = mo_file.parent.parent.name
+    ldir = __locale_dir__ / lname / ltype
+    mo_file_rel = str(mo_file).lstrip('/')
+    __data_files__.append((str(ldir), [mo_file_rel]))
+
+# print("Found data files:\n" + pp(__data_files__) + "\n")
+
+
+# -----------------------------------
+class Sdist(sdist):
+    """Custom ``sdist`` command to ensure that mo files are always created."""
+
+    def run(self):
+        self.run_command('compile_catalog')
+        # sdist is an old style class so super cannot be used.
+        sdist.run(self)
+
+
+# -----------------------------------
 setup(
     version=__packet_version__,
     long_description=read(__readme_file__),
     scripts=__scripts__,
     requires=__requirements__,
+    package_data=__package_data__,
+    data_files=__data_files__,
+    cmdclass={
+        'compile_catalog': babel.compile_catalog,
+        'extract_messages': babel.extract_messages,
+        'init_catalog': babel.init_catalog,
+        'update_catalog': babel.update_catalog,
+        'sdist': Sdist,
+    },
 )
 
 
 # =============================================================================
 # vim: fileencoding=utf-8 filetype=python ts=4 et list
```

### Comparing `postfix_logsums-0.9.0/test/test_00_errors.py` & `postfix_logsums-0.9.1/test/test_00_errors.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.0/test/test_05_stats_collections.py` & `postfix_logsums-0.9.1/test/test_05_stats_collections.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.0/test/test_10_results.py` & `postfix_logsums-0.9.1/test/test_10_results.py`

 * *Files identical despite different names*

