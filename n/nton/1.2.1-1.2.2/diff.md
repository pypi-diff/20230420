# Comparing `tmp/nton-1.2.1.tar.gz` & `tmp/nton-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nton-1.2.1.tar", max compression
+gzip compressed data, was "nton-1.2.2.tar", max compression
```

## Comparing `nton-1.2.1.tar` & `nton-1.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35823 2023-04-20 07:40:29.665652 nton-1.2.1/LICENSE
--rw-r--r--   0        0        0       23 2023-04-20 07:40:29.665652 nton-1.2.1/nton/__init__.py
--rw-r--r--   0        0        0     5669 2023-04-20 07:40:29.665652 nton-1.2.1/nton/assets/control.nacp.xml
--rw-r--r--   0        0        0    54085 2023-04-20 07:40:29.665652 nton-1.2.1/nton/assets/exefs/main
--rw-r--r--   0        0        0     1016 2023-04-20 07:40:29.681337 nton-1.2.1/nton/assets/exefs/main.npdm
--rw-r--r--   0        0        0      262 2023-04-20 07:40:29.681337 nton-1.2.1/nton/assets/logo/NintendoLogo.png
--rw-r--r--   0        0        0    51019 2023-04-20 07:40:29.681337 nton-1.2.1/nton/assets/logo/StartupMovie.gif
--rw-r--r--   0        0        0     1423 2023-04-20 07:40:29.681337 nton-1.2.1/nton/constants.py
--rw-r--r--   0        0        0    15843 2023-04-20 07:40:29.681337 nton-1.2.1/nton/main.py
--rw-r--r--   0        0        0     3339 2023-04-20 07:40:29.681337 nton-1.2.1/nton/nstool.py
--rw-r--r--   0        0        0    22034 2023-04-20 07:40:29.681337 nton-1.2.1/nton/title_ids.py
--rw-r--r--   0        0        0     1123 2023-04-20 07:40:29.681337 nton-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     8263 2023-04-20 07:40:29.665652 nton-1.2.1/README.md
--rw-r--r--   0        0        0     9575 1970-01-01 00:00:00.000000 nton-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-20 07:48:40.476933 nton-1.2.2/LICENSE
+-rw-r--r--   0        0        0       23 2023-04-20 07:48:40.476933 nton-1.2.2/nton/__init__.py
+-rw-r--r--   0        0        0     5669 2023-04-20 07:48:40.476933 nton-1.2.2/nton/assets/control.nacp.xml
+-rw-r--r--   0        0        0    54085 2023-04-20 07:48:40.476933 nton-1.2.2/nton/assets/exefs/main
+-rw-r--r--   0        0        0     1016 2023-04-20 07:48:40.476933 nton-1.2.2/nton/assets/exefs/main.npdm
+-rw-r--r--   0        0        0      262 2023-04-20 07:48:40.476933 nton-1.2.2/nton/assets/logo/NintendoLogo.png
+-rw-r--r--   0        0        0    51019 2023-04-20 07:48:40.476933 nton-1.2.2/nton/assets/logo/StartupMovie.gif
+-rw-r--r--   0        0        0     1423 2023-04-20 07:48:40.476933 nton-1.2.2/nton/constants.py
+-rw-r--r--   0        0        0    15843 2023-04-20 07:48:40.476933 nton-1.2.2/nton/main.py
+-rw-r--r--   0        0        0     3339 2023-04-20 07:48:40.476933 nton-1.2.2/nton/nstool.py
+-rw-r--r--   0        0        0    22034 2023-04-20 07:48:40.476933 nton-1.2.2/nton/title_ids.py
+-rw-r--r--   0        0        0     1123 2023-04-20 07:48:40.476933 nton-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8263 2023-04-20 07:48:40.476933 nton-1.2.2/README.md
+-rw-r--r--   0        0        0     9626 1970-01-01 00:00:00.000000 nton-1.2.2/PKG-INFO
```

### Comparing `nton-1.2.1/LICENSE` & `nton-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nton-1.2.1/nton/assets/control.nacp.xml` & `nton-1.2.2/nton/assets/control.nacp.xml`

 * *Files identical despite different names*

### Comparing `nton-1.2.1/nton/assets/exefs/main` & `nton-1.2.2/nton/assets/exefs/main`

 * *Files identical despite different names*

### Comparing `nton-1.2.1/nton/assets/exefs/main.npdm` & `nton-1.2.2/nton/assets/exefs/main.npdm`

 * *Files identical despite different names*

### Comparing `nton-1.2.1/nton/assets/logo/StartupMovie.gif` & `nton-1.2.2/nton/assets/logo/StartupMovie.gif`

 * *Files identical despite different names*

### Comparing `nton-1.2.1/nton/constants.py` & `nton-1.2.2/nton/constants.py`

 * *Files identical despite different names*

### Comparing `nton-1.2.1/nton/main.py` & `nton-1.2.2/nton/main.py`

 * *Files identical despite different names*

### Comparing `nton-1.2.1/nton/nstool.py` & `nton-1.2.2/nton/nstool.py`

 * *Files identical despite different names*

### Comparing `nton-1.2.1/nton/title_ids.py` & `nton-1.2.2/nton/title_ids.py`

 * *Files identical despite different names*

### Comparing `nton-1.2.1/pyproject.toml` & `nton-1.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nton"
-version = "1.2.1"
+version = "1.2.2"
 description = "Nintendo Switch NRO to NSP Forwarder."
 authors = ["rlaphoenix <rlaphoenix@pm.me>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/rlaphoenix/nton"
 keywords = ["nintendo", "switch", "homebrew", "forwarder"]
 classifiers = [
@@ -22,15 +22,15 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/rlaphoenix/nton/issues"
 "Forums" = "https://github.com/rlaphoenix/nton/discussions"
 "Changelog" = "https://github.com/rlaphoenix/nton/blob/master/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.11"
+python = ">=3.7,<3.12"
 click = "^8.1.3"
 appdirs = "^1.4.4"
 requests = "^2.28.2"
 jsonpickle = "^3.0.1"
 coloredlogs = "^15.0.1"
 beautifulsoup4 = "^4.12.2"
 lxml = "^4.9.2"
```

### Comparing `nton-1.2.1/README.md` & `nton-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nton-1.2.1/PKG-INFO` & `nton-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: nton
-Version: 1.2.1
+Version: 1.2.2
 Summary: Nintendo Switch NRO to NSP Forwarder.
 Home-page: https://github.com/rlaphoenix/nton
 License: GPL-3.0-only
 Keywords: nintendo,switch,homebrew,forwarder
 Author: rlaphoenix
 Author-email: rlaphoenix@pm.me
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.7,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Utilities
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: jsonpickle (>=3.0.1,<4.0.0)
```

#### html2text {}

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1 Name: nton Version: 1.2.1 Summary: Nintendo Switch NRO to
+Metadata-Version: 2.1 Name: nton Version: 1.2.2 Summary: Nintendo Switch NRO to
 NSP Forwarder. Home-page: https://github.com/rlaphoenix/nton License: GPL-3.0-
 only Keywords: nintendo,switch,homebrew,forwarder Author: rlaphoenix Author-
-email: rlaphoenix@pm.me Requires-Python: >=3.7,<3.11 Classifier: Development
+email: rlaphoenix@pm.me Requires-Python: >=3.7,<3.12 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Games/Entertainment
-Classifier: Topic :: Utilities Requires-Dist: appdirs (>=1.4.4,<2.0.0)
-Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: click
-(>=8.1.3,<9.0.0) Requires-Dist: coloredlogs (>=15.0.1,<16.0.0) Requires-Dist:
-jsonpickle (>=3.0.1,<4.0.0) Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist:
-requests (>=2.28.2,<3.0.0) Project-URL: Bug Tracker, https://github.com/
-rlaphoenix/nton/issues Project-URL: Changelog, https://github.com/rlaphoenix/
-nton/blob/master/CHANGELOG.md Project-URL: Forums, https://github.com/
-rlaphoenix/nton/discussions Project-URL: Repository, https://github.com/
-rlaphoenix/nton Description-Content-Type: text/markdown # NTON [![Build status]
-(https://github.com/rlaphoenix/nton/actions/workflows/ci.yml/badge.svg)](https:
-//github.com/rlaphoenix/nton/actions/workflows/ci.yml) [![PyPI version](https:/
-/img.shields.io/pypi/v/nton)](https://pypi.python.org/pypi/nton) [![Python
-versions](https://img.shields.io/pypi/pyversions/nton)](https://
-pypi.python.org/pypi/nton) [License_(GPLv3)] NTON is a Nintendo Switch NRO to
-NSP Forwarder for firmware 12.0.0 and newer. A forwarder lets you open a
-Homebrew NRO file from your SD card through the Nintendo Switch Home Screen
-instead of the Homebrew Launcher. ![Preview](https://user-
-images.githubusercontent.com/17136956/206882948-4f05cace-16a3-4300-9047-
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Games/Entertainment Classifier: Topic ::
+Utilities Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-Dist: beautifulsoup4
+(>=4.12.2,<5.0.0) Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist:
+coloredlogs (>=15.0.1,<16.0.0) Requires-Dist: jsonpickle (>=3.0.1,<4.0.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist: requests (>=2.28.2,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/rlaphoenix/nton/issues Project-
+URL: Changelog, https://github.com/rlaphoenix/nton/blob/master/CHANGELOG.md
+Project-URL: Forums, https://github.com/rlaphoenix/nton/discussions Project-
+URL: Repository, https://github.com/rlaphoenix/nton Description-Content-Type:
+text/markdown # NTON [![Build status](https://github.com/rlaphoenix/nton/
+actions/workflows/ci.yml/badge.svg)](https://github.com/rlaphoenix/nton/
+actions/workflows/ci.yml) [![PyPI version](https://img.shields.io/pypi/v/nton)]
+(https://pypi.python.org/pypi/nton) [![Python versions](https://img.shields.io/
+pypi/pyversions/nton)](https://pypi.python.org/pypi/nton) [License_(GPLv3)]
+NTON is a Nintendo Switch NRO to NSP Forwarder for firmware 12.0.0 and newer. A
+forwarder lets you open a Homebrew NRO file from your SD card through the
+Nintendo Switch Home Screen instead of the Homebrew Launcher. ![Preview](https:
+//user-images.githubusercontent.com/17136956/206882948-4f05cace-16a3-4300-9047-
 8cba33106a64.jpg) *Forwarders made with NTON.* ## Features - ð¡ï¸ Safety-
 first approach; System/Game Title IDs cannot be used and NRO files are
 validated - ð¹ï¸ Boot right into an Emulated Game with Direct RetroArch Game
 Forwarding - ð¼ï¸ Supports any Image file of any resolution or format for
 the NSP Icon - ð¤ The Title Name, Publisher, Icon, and more are automatically
 extracted from the NRO - ð¥ Supports Video Capture and Screenshots - â
 Currently Supports Firmware 12.0.0 and up - ð§© Plug-and-play installation via
```

