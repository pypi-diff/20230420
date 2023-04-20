# Comparing `tmp/uberduck-0.0.3.tar.gz` & `tmp/uberduck-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uberduck-0.0.3.tar", last modified: Fri Dec 23 09:59:40 2022, max compression
+gzip compressed data, was "uberduck-0.0.4.tar", last modified: Thu Apr 20 09:27:30 2023, max compression
```

## Comparing `uberduck-0.0.3.tar` & `uberduck-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nimboss    (501) staff       (20)        0 2022-12-23 09:59:40.386470 uberduck-0.0.3/
--rw-r--r--   0 nimboss    (501) staff       (20)     1056 2022-03-09 10:12:26.000000 uberduck-0.0.3/LICENSE
--rw-r--r--   0 nimboss    (501) staff       (20)     5480 2022-12-23 09:59:40.386083 uberduck-0.0.3/PKG-INFO
--rw-r--r--   0 nimboss    (501) staff       (20)     3213 2022-06-27 13:35:50.000000 uberduck-0.0.3/README.md
--rw-r--r--   0 nimboss    (501) staff       (20)       38 2022-12-23 09:59:40.386809 uberduck-0.0.3/setup.cfg
--rw-r--r--   0 nimboss    (501) staff       (20)     2829 2022-12-23 09:59:01.000000 uberduck-0.0.3/setup.py
-drwxr-xr-x   0 nimboss    (501) staff       (20)        0 2022-12-23 09:59:40.380150 uberduck-0.0.3/uberduck/
--rw-r--r--   0 nimboss    (501) staff       (20)     1781 2022-12-23 09:57:26.000000 uberduck-0.0.3/uberduck/__init__.py
--rw-r--r--   0 nimboss    (501) staff       (20)     7009 2022-06-27 13:31:37.000000 uberduck-0.0.3/uberduck/classes.py
--rw-r--r--   0 nimboss    (501) staff       (20)    13171 2022-03-10 05:52:01.000000 uberduck-0.0.3/uberduck/main.py
-drwxr-xr-x   0 nimboss    (501) staff       (20)        0 2022-12-23 09:59:40.385333 uberduck-0.0.3/uberduck.egg-info/
--rw-r--r--   0 nimboss    (501) staff       (20)     5480 2022-12-23 09:59:40.000000 uberduck-0.0.3/uberduck.egg-info/PKG-INFO
--rw-r--r--   0 nimboss    (501) staff       (20)      243 2022-12-23 09:59:40.000000 uberduck-0.0.3/uberduck.egg-info/SOURCES.txt
--rw-r--r--   0 nimboss    (501) staff       (20)        1 2022-12-23 09:59:40.000000 uberduck-0.0.3/uberduck.egg-info/dependency_links.txt
--rw-r--r--   0 nimboss    (501) staff       (20)       31 2022-12-23 09:59:40.000000 uberduck-0.0.3/uberduck.egg-info/requires.txt
--rw-r--r--   0 nimboss    (501) staff       (20)        9 2022-12-23 09:59:40.000000 uberduck-0.0.3/uberduck.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 09:27:30.526666 uberduck-0.0.4/
+-rw-rw-rw-   0        0        0     1056 2022-03-09 10:12:26.000000 uberduck-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5846 2023-04-20 09:27:30.525667 uberduck-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3455 2023-04-20 09:20:50.000000 uberduck-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 09:27:30.526666 uberduck-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2839 2022-12-25 04:32:37.000000 uberduck-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 09:27:30.462836 uberduck-0.0.4/uberduck/
+-rw-rw-rw-   0        0        0     1781 2023-04-17 12:29:41.000000 uberduck-0.0.4/uberduck/__init__.py
+-rw-rw-rw-   0        0        0     9038 2023-04-20 09:16:22.000000 uberduck-0.0.4/uberduck/classes.py
+-rw-rw-rw-   0        0        0    13171 2022-03-10 05:52:01.000000 uberduck-0.0.4/uberduck/main.py
+drwxrwxrwx   0        0        0        0 2023-04-20 09:27:30.521710 uberduck-0.0.4/uberduck.egg-info/
+-rw-rw-rw-   0        0        0     5846 2023-04-20 09:27:29.000000 uberduck-0.0.4/uberduck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-04-20 09:27:29.000000 uberduck-0.0.4/uberduck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 09:27:29.000000 uberduck-0.0.4/uberduck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-20 09:27:29.000000 uberduck-0.0.4/uberduck.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 09:27:29.000000 uberduck-0.0.4/uberduck.egg-info/top_level.txt
```

### Comparing `uberduck-0.0.3/LICENSE` & `uberduck-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uberduck-0.0.3/PKG-INFO` & `uberduck-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-Metadata-Version: 2.1
-Name: uberduck
-Version: 0.0.3
-Summary: A synchronous and asynchronous API wrapper for the UberDuck text-to-speech service (https://uberduck.ai) with 100% coverage and top-notch utilities.
-Home-page: https://github.com/ImNimboss/uberduck
-Author: ImNimboss
-Author-email: nim@nimboss.me
-License: MIT
-Project-URL: Documentation, https://github.com/ImNimboss/uberduck/tree/main/Documentation
-Project-URL: Issue Tracker, https://github.com/ImNimboss/uberduck/issues
-Project-URL: Source, https://github.com/ImNimboss/uberduck
-Project-URL: Funding, https://patreon.com/nimboss
-Project-URL: API Credits, https://uberduck.ai
-Project-URL: Creator, https://nimboss.me
-Project-URL: Discord, https://discord.gg/FcxqdJ7AQq
-Project-URL: Repository, https://github.com/ImNimboss/uberduck
-Keywords: uberduck,wrapper,api,text-to-speech,async,famous,tts,texttospeech,AI,api-wrapper,api-key,api-secret
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Artistic Software
-Classifier: Topic :: Games/Entertainment
-Classifier: Topic :: Internet
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: Multimedia :: Sound/Audio :: Players
-Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/ImNimboss/uberduck/main/.github/assets/uberduck-logo.png" alt="Uberduck Logo">
-</p>
-
-# Uberduck
-
-<a href="https://pypi.org/project/uberduck" target="_blank" rel="noopener noreferrer">
-    <img src="https://img.shields.io/pypi/v/uberduck.svg?color=9cf&logo=pypi" alt="PyPI Uberduck version number">
-    <img src="https://img.shields.io/pypi/dm/uberduck?color=9cf&logo=pypi" alt="PyPI downloads per month">
-    <img src="https://img.shields.io/pypi/pyversions/uberduck.svg?color=9cf&logo=pypi" alt="PyPI supported Python versions">
-</a>
-<a href="https://github.com/ImNimboss/uberduck/issues" target="_blank" rel="noopener noreferrer">
-    <img src="https://img.shields.io/github/issues/ImNimboss/uberduck?color=9cf&logo=github" alt="Number of open GitHub issues">
-</a>
-<a href="https://github.com/ImNimboss/uberduck/contributors" target="_blank" rel="noopener noreferrer">
-    <img src="https://img.shields.io/github/contributors/ImNimboss/uberduck?color=9cf&logo=github" alt="Number of contributors">
-</a>
-<a href="https://discord.gg/FcxqdJ7AQq" target="_blank" rel="noopener noreferrer">
-    <img src="https://img.shields.io/discord/930791886522810399?color=9cf&logo=discord&label=discord" alt="Discord server">
-</a>
-
-## Description
-
-A synchronous and asynchronous API wrapper for the [UberDuck](https://uberduck.ai) text-to-speech service with 100% coverage and top-notch utilities.
-
-## Main features
-
-- [x] - Synchronous support
-- [x] - Asynchronous support
-- [x] - Object-oriented
-- [x] - Easy to use
-- [x] - Utilities like file-saving, audio-playing etc. packed all in one
-- [x] - Very adjustable/configurable
-- [x] - Regularly maintained
-- [x] - Makes the hard tasks of polling and asynchronous operations easy
-
-## Links
-
-* [Documentation](https://github.com/ImNimboss/uberduck/tree/main/Documentation)
-* [PyPI](https://pypi.org/project/uberduck)
-* [Issue Tracking](https://github.com/ImNimboss/uberduck/issues)
-* [Discord server](https://discord.gg/FcxqdJ7AQq)
-* [Uberduck main site](https://uberduck.ai)
-
-
-## Installation and upgrades
-
-```
-pip install uberduck
-```
-for the stable version (recommended).
-
-```
-pip install -U uberduck
-```
-to update your stable version.
-
-```
-pip install git+https://github.com/ImNimboss/uberduck
-```
-to install it straight off of GitHub (you need git installed for this).
-
-```
-pip install -U git+https://github.com/ImNimboss/uberduck
-```
-to upgrade your version that you got from GitHub.
-
-## How to use
-
-Check [Documentation/Basics.md](https://github.com/ImNimboss/uberduck/blob/master/Documentation/Basics.md).
-
-## Examples
-
-Check [Documentation/Examples.md](https://github.com/ImNimboss/uberduck/blob/master/Documentation/Examples.md).
-
-## Some credits
-
-The idea to implement logging in this library came from [discord.py](https://github.com/Rapptz/discord.py).
-
-The idea to use the `polling` library came from [CupOfGeo/UberDuckAPI](https://github.com/CupOfGeo/UberDuckAPI), another uberduck.ai API wrapper.
-
-## Changelog
-
-* `v0.0.1` - Initial release.
-* `v0.0.2` - Fixed `get_voices()` and `get_voices_async()` by updating the `Voice` class to be compatible with the new voice data available from the API.
-
+Metadata-Version: 2.1
+Name: uberduck
+Version: 0.0.4
+Summary: A synchronous and asynchronous API wrapper for the UberDuck text-to-speech service (https://uberduck.ai) with 100% coverage and top-notch utilities.
+Home-page: https://github.com/ImNimboss/uberduck
+Author: ImNimboss
+Author-email: nimit.grover24@gmail.com
+License: MIT
+Project-URL: Documentation, https://github.com/ImNimboss/uberduck/tree/main/Documentation
+Project-URL: Issue Tracker, https://github.com/ImNimboss/uberduck/issues
+Project-URL: Source, https://github.com/ImNimboss/uberduck
+Project-URL: Funding, https://patreon.com/nimboss
+Project-URL: API Credits, https://uberduck.ai
+Project-URL: Creator, https://nimboss.me
+Project-URL: Discord, https://discord.gg/FcxqdJ7AQq
+Project-URL: Repository, https://github.com/ImNimboss/uberduck
+Keywords: uberduck,wrapper,api,text-to-speech,async,famous,tts,texttospeech,AI,api-wrapper,api-key,api-secret
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Artistic Software
+Classifier: Topic :: Games/Entertainment
+Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Sound/Audio :: Players
+Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/ImNimboss/uberduck/main/.github/assets/uberduck-logo.png" alt="Uberduck Logo">
+</p>
+
+# Uberduck
+
+<a href="https://pypi.org/project/uberduck" target="_blank" rel="noopener noreferrer">
+    <img src="https://img.shields.io/pypi/v/uberduck.svg?color=9cf&logo=pypi" alt="PyPI Uberduck version number">
+    <img src="https://img.shields.io/pypi/dm/uberduck?color=9cf&logo=pypi" alt="PyPI downloads per month">
+    <img src="https://img.shields.io/pypi/pyversions/uberduck.svg?color=9cf&logo=pypi" alt="PyPI supported Python versions">
+</a>
+<a href="https://github.com/ImNimboss/uberduck/issues" target="_blank" rel="noopener noreferrer">
+    <img src="https://img.shields.io/github/issues/ImNimboss/uberduck?color=9cf&logo=github" alt="Number of open GitHub issues">
+</a>
+<a href="https://github.com/ImNimboss/uberduck/contributors" target="_blank" rel="noopener noreferrer">
+    <img src="https://img.shields.io/github/contributors/ImNimboss/uberduck?color=9cf&logo=github" alt="Number of contributors">
+</a>
+<a href="https://discord.gg/FcxqdJ7AQq" target="_blank" rel="noopener noreferrer">
+    <img src="https://img.shields.io/discord/930791886522810399?color=9cf&logo=discord&label=discord" alt="Discord server">
+</a>
+
+## Description
+
+A synchronous and asynchronous API wrapper for the [UberDuck](https://uberduck.ai) text-to-speech service with 100% coverage and top-notch utilities.
+
+## Main features
+
+- [x] - Synchronous support
+- [x] - Asynchronous support
+- [x] - Object-oriented
+- [x] - Easy to use
+- [x] - Utilities like file-saving, audio-playing etc. packed all in one
+- [x] - Very adjustable/configurable
+- [x] - Regularly maintained
+- [x] - Makes the hard tasks of polling and asynchronous operations easy
+
+## Links
+
+* [Documentation](https://github.com/ImNimboss/uberduck/tree/main/Documentation)
+* [PyPI](https://pypi.org/project/uberduck)
+* [Issue Tracking](https://github.com/ImNimboss/uberduck/issues)
+* [Discord server](https://discord.gg/FcxqdJ7AQq)
+* [Uberduck main site](https://uberduck.ai)
+
+
+## Installation and upgrades
+
+```
+pip install uberduck
+```
+for the stable version (recommended).
+
+```
+pip install -U uberduck
+```
+to update your stable version.
+
+```
+pip install git+https://github.com/ImNimboss/uberduck
+```
+to install it straight off of GitHub (you need git installed for this).
+
+```
+pip install -U git+https://github.com/ImNimboss/uberduck
+```
+to upgrade your version that you got from GitHub.
+
+## How to use
+
+Check [Documentation/Basics.md](https://github.com/ImNimboss/uberduck/blob/master/Documentation/Basics.md).
+
+## Examples
+
+Check [Documentation/Examples.md](https://github.com/ImNimboss/uberduck/blob/master/Documentation/Examples.md).
+
+## Some credits
+
+The idea to implement logging in this library came from [discord.py](https://github.com/Rapptz/discord.py).
+
+The idea to use the `polling` library came from [CupOfGeo/UberDuckAPI](https://github.com/CupOfGeo/UberDuckAPI), another uberduck.ai API wrapper.
+
+## Changelog
+
+* `v0.0.1` - Initial release.
+* `v0.0.2` - Fixed `get_voices()` and `get_voices_async()` by updating the `Voice` class to be compatible with the new voice data available from the API.
+* `v0.0.3` - Moved `README.md` from `.github` to root folder due to compatibility issues with other software
+* `v0.0.4` - Added attributes `added_at`, `is_primary`, `hifi_gan_vocoder`, `ml_model_id`, `speaker_id`, `language` to `Voice` class
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: uberduck Version: 0.0.3 Summary: A synchronous and
+Metadata-Version: 2.1 Name: uberduck Version: 0.0.4 Summary: A synchronous and
 asynchronous API wrapper for the UberDuck text-to-speech service (https://
 uberduck.ai) with 100% coverage and top-notch utilities. Home-page: https://
-github.com/ImNimboss/uberduck Author: ImNimboss Author-email: nim@nimboss.me
-License: MIT Project-URL: Documentation, https://github.com/ImNimboss/uberduck/
-tree/main/Documentation Project-URL: Issue Tracker, https://github.com/
-ImNimboss/uberduck/issues Project-URL: Source, https://github.com/ImNimboss/
-uberduck Project-URL: Funding, https://patreon.com/nimboss Project-URL: API
-Credits, https://uberduck.ai Project-URL: Creator, https://nimboss.me Project-
-URL: Discord, https://discord.gg/FcxqdJ7AQq Project-URL: Repository, https://
-github.com/ImNimboss/uberduck Keywords: uberduck,wrapper,api,text-to-
-speech,async,famous,tts,texttospeech,AI,api-wrapper,api-key,api-secret
-Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
-:: MIT License Classifier: Natural Language :: English Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+github.com/ImNimboss/uberduck Author: ImNimboss Author-email:
+nimit.grover24@gmail.com License: MIT Project-URL: Documentation, https://
+github.com/ImNimboss/uberduck/tree/main/Documentation Project-URL: Issue
+Tracker, https://github.com/ImNimboss/uberduck/issues Project-URL: Source,
+https://github.com/ImNimboss/uberduck Project-URL: Funding, https://
+patreon.com/nimboss Project-URL: API Credits, https://uberduck.ai Project-URL:
+Creator, https://nimboss.me Project-URL: Discord, https://discord.gg/FcxqdJ7AQq
+Project-URL: Repository, https://github.com/ImNimboss/uberduck Keywords:
+uberduck,wrapper,api,text-to-speech,async,famous,tts,texttospeech,AI,api-
+wrapper,api-key,api-secret Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: MIT License Classifier: Natural Language :: English Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Topic :: Artistic Software Classifier:
 Topic :: Games/Entertainment Classifier: Topic :: Internet Classifier: Topic ::
 Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic
 Content Classifier: Topic :: Multimedia :: Sound/Audio Classifier: Topic ::
@@ -52,8 +52,11 @@
 [Documentation/Examples.md](https://github.com/ImNimboss/uberduck/blob/master/
 Documentation/Examples.md). ## Some credits The idea to implement logging in
 this library came from [discord.py](https://github.com/Rapptz/discord.py). The
 idea to use the `polling` library came from [CupOfGeo/UberDuckAPI](https://
 github.com/CupOfGeo/UberDuckAPI), another uberduck.ai API wrapper. ## Changelog
 * `v0.0.1` - Initial release. * `v0.0.2` - Fixed `get_voices()` and
 `get_voices_async()` by updating the `Voice` class to be compatible with the
-new voice data available from the API.
+new voice data available from the API. * `v0.0.3` - Moved `README.md` from
+`.github` to root folder due to compatibility issues with other software *
+`v0.0.4` - Added attributes `added_at`, `is_primary`, `hifi_gan_vocoder`,
+`ml_model_id`, `speaker_id`, `language` to `Voice` class
```

### Comparing `uberduck-0.0.3/README.md` & `uberduck-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -78,8 +78,10 @@
 The idea to implement logging in this library came from [discord.py](https://github.com/Rapptz/discord.py).
 
 The idea to use the `polling` library came from [CupOfGeo/UberDuckAPI](https://github.com/CupOfGeo/UberDuckAPI), another uberduck.ai API wrapper.
 
 ## Changelog
 
 * `v0.0.1` - Initial release.
-* `v0.0.2` - Fixed `get_voices()` and `get_voices_async()` by updating the `Voice` class to be compatible with the new voice data available from the API.
+* `v0.0.2` - Fixed `get_voices()` and `get_voices_async()` by updating the `Voice` class to be compatible with the new voice data available from the API.
+* `v0.0.3` - Moved `README.md` from `.github` to root folder due to compatibility issues with other software
+* `v0.0.4` - Added attributes `added_at`, `is_primary`, `hifi_gan_vocoder`, `ml_model_id`, `speaker_id`, `language` to `Voice` class
```

#### html2text {}

```diff
@@ -22,8 +22,11 @@
 [Documentation/Examples.md](https://github.com/ImNimboss/uberduck/blob/master/
 Documentation/Examples.md). ## Some credits The idea to implement logging in
 this library came from [discord.py](https://github.com/Rapptz/discord.py). The
 idea to use the `polling` library came from [CupOfGeo/UberDuckAPI](https://
 github.com/CupOfGeo/UberDuckAPI), another uberduck.ai API wrapper. ## Changelog
 * `v0.0.1` - Initial release. * `v0.0.2` - Fixed `get_voices()` and
 `get_voices_async()` by updating the `Voice` class to be compatible with the
-new voice data available from the API.
+new voice data available from the API. * `v0.0.3` - Moved `README.md` from
+`.github` to root folder due to compatibility issues with other software *
+`v0.0.4` - Added attributes `added_at`, `is_primary`, `hifi_gan_vocoder`,
+`ml_model_id`, `speaker_id`, `language` to `Voice` class
```

### Comparing `uberduck-0.0.3/setup.py` & `uberduck-0.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 setup(
     name = 'uberduck',
     version = version,
     description = 'A synchronous and asynchronous API wrapper for the UberDuck text-to-speech service (https://uberduck.ai) with 100% coverage and top-notch utilities.',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     author = 'ImNimboss',
-    author_email = 'nim@nimboss.me',
+    author_email = 'nimit.grover24@gmail.com',
     url = 'https://github.com/ImNimboss/uberduck',
     license = 'MIT',
     packages = ['uberduck'],
     keywords = [
         'uberduck', 'wrapper', 'api', 'text-to-speech', 'async', 'famous',
         'tts', 'texttospeech', 'AI', 'api-wrapper', 'api-key', 'api-secret'
     ],
```

### Comparing `uberduck-0.0.3/uberduck/__init__.py` & `uberduck-0.0.4/uberduck/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 from uberduck.main import UberDuck, get_voices, get_voices_async
 from uberduck.classes import *
 import logging as _logging
 
 __author__: str = 'ImNimboss'
 __license__: str = 'MIT'
-__version__: str = '0.0.3'
+__version__: str = '0.0.4'
 GITHUB: str = 'https://github.com/ImNimboss/uberduck'
 ISSUE_TRACKER: str = 'https://github.com/ImNimboss/uberduck/issues'
 DOCUMENTATION: str = 'https://github.com/ImNimboss/uberduck/tree/main/Documentation'
 SPONSOR: str = 'https://patreon.com/ImNimboss'
 API_CREDITS: str = 'https://uberduck.ai'
 
 _logging.getLogger(__name__).addHandler(_logging.NullHandler())
```

### Comparing `uberduck-0.0.3/uberduck/classes.py` & `uberduck-0.0.4/uberduck/classes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,131 +1,151 @@
-"""
-Copyright 2022-present ImNimboss
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
-from typing import List
-
-class Membership:
-    """
-    This is a model class Membership that represents the membership attribute of a voice.
-    
-    Attributes:
-        `name (str)`: The name of the membership.
-        `id (int)`: The ID of the membership.
-
-    Magic methods:
-        `__str__`: Returns a string representation of the Membership object in the format `Membership: Name - {name}, ID - {id}`.
-        `__repr__`: Returns a string representation of the Membership object in the format `<Membership name='{name}' id={id}>`.
-
-    This class is read-only.
-    """
-    def __init__(self, name: str = None, id: int = None):
-        self.name = name
-        self.id = id
-
-    def __str__(self):
-        return f'Membership: Name - {self.name}, ID - {self.id}'
-
-    def __repr__(self):
-        return f'<Membership name=\'{self.name}>\' id={self.id}>'
-
-class Voice:
-    """
-    This is a model class Voice that represents a voice.
-
-    Attributes:
-        `architecture (str)`: The architecture of the voice i.e. the engine that was used to make the voice.
-        `category (str)`: The category of the voice i.e. where it's from (WWE, SpongeBob etc).
-        `contributors (list)`: The contributors' names of the voice.
-        `controls (bool)`: Whether the voice has controls.
-        `display_name (str)`: The display name of the voice i.e. a better formatted name to show to general users.
-        `is_active (bool)`: Whether the voice is active.
-        `model_id (str)`: The model ID of the voice. This is not a unique identification, the name is.
-        `memberships (list)`: The memberships of the voice.
-        `is_private (bool)`: Whether the voice is private.
-        `name (str)`: The name of the voice i.e. the name you pass to the API in order for it to recognize which voice you want.
-        `symbol_set (str)`: The symbol set of the voice.
-        `voicemodel_uuid (str)`: The voice model's UUID.
-
-    Magic methods:
-        `__str__`: Returns a string representation of the Voice object in the format `Voice: Architecture - {architecture}, Category - {category}, Controls - {controls}, Display Name - {display_name}, Name - {name}, Model ID - {model_id}, Memberships - {memberships}, Is Private - {is_private}, Contributors - {contributors}`.
-        `__repr__`: Returns a string representation of the Voice object in the format `<Voice architecture='{architecture}' category='{category}' controls='{controls}' display_name='{display_name}' name='{name}' model_id='{model_id}' memberships='{memberships}' is_private='{is_private}' contributors='{contributors}'>`.
-    
-    This class is read-only.
-    """
-    def __init__(
-        self,
-        architecture: str,
-        category: str,
-        contributors: List[str],
-        controls: bool,
-        display_name: str,
-        is_active: bool,
-        model_id: str,
-        memberships: list,
-        is_private: bool,
-        name: str,
-        symbol_set: str,
-        voicemodel_uuid: str
-    ) -> None:
-        self.architecture = architecture
-        self.category = category
-        self.contributors = contributors
-        self.controls = controls
-        self.display_name = display_name
-        self.is_active = is_active
-        self.model_id = model_id
-        self.memberships = memberships
-        if self.memberships:
-            self.memberships: List[Membership] = [Membership(*memberships)]
-        self.is_private = is_private
-        self.name = name
-        self.symbol_set = symbol_set
-        self.voicemodel_uuid = voicemodel_uuid
-
-    def __str__(self):
-        return f'Voice: Architecture - {self.architecture}, Category - {self.category}, Contributors - {self.contributors}, Controls - {self.controls}, Display Name - {self.display_name}, Is Active - {self.is_active},  Model ID - {self.model_id}, Memberships - {self.memberships}, Is Private - {self.is_private}, Name - {self.name}, Symbol Set - {self.symbol_set}, Voice model UUID - {self.voicemodel_uuid}'
-
-    def __repr__(self):
-        return f'<Voice architecture=\'{self.architecture}\' category=\'{self.category}\' contributors=\'{self.contributors}\' controls=\'{self.controls}\' display_name=\'{self.display_name}\' is_active=\'{self.is_active}\' model_id=\'{self.model_id}\' memberships=\'{self.memberships}\' is_private=\'{self.is_private}\' name=\'{self.name}\' symbol_set=\'{self.symbol_set}\' voicemodel_uuid=\'{self.voicemodel_uuid}\'>'
-
-class UberduckException(Exception):
-    """
-    Base class for all exceptions raised by Uberduck. This exception could be used to catch any exceptions thrown by this library.
-    """
-    pass
-
-class InvalidVoice(UberduckException):
-    """
-    Raised when an invalid voice is specified. See all the voices from `uberduck.get_voices()`, `uberduck.get_voices_async()` or [uberduck.ai/quack-help](https://uberduck.ai/quack-help).
-    """
-    def __init__(self, voice: str) -> None:
-        self.voice = voice
-        super().__init__(f'Invalid voice: {voice}.')
-
-class Unauthorized(UberduckException):
-    """
-    Exception raised when your API key is invalid or your API secret is invalid. Get an API key and secret from [uberduck.ai/account/manage](https://uberduck.ai/account/manage).
-    """
-    def __init__(self) -> None:
-        super().__init__('Invalid API credentials. Please check your api key and/or api secret.')
-
-class Ratelimited(UberduckException):
-    """
-    Exception raised when you are being ratelimited from the API.
-    """
-    def __init__(self) -> None:
-        super().__init__('You are being ratelimited from the API. Please try again later.')
-
-class HTTPException(UberduckException):
-    """
-    Exception raised when the HTTP request fails due to an unknown cause.
-    """
-    def __init__(self, status_code: int, detail) -> None:
-        self.status_code = status_code
-        self.detail = detail
+"""
+Copyright 2022-present ImNimboss
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+"""
+from typing import List, Optional
+from datetime import datetime as dt
+
+class Membership:
+    """
+    This is a model class Membership that represents the membership attribute of a voice.
+    
+    Attributes:
+        `name (str)`: The name of the membership.
+        `id (int)`: The ID of the membership.
+
+    Magic methods:
+        `__str__`: Returns a string representation of the Membership object in the format `Membership: Name - {name}, ID - {id}`.
+        `__repr__`: Returns a string representation of the Membership object in the format `<Membership name='{name}' id={id}>`.
+
+    This class is read-only.
+    """
+    def __init__(self, name: str = None, id: int = None):
+        self.name = name
+        self.id = id
+
+    def __str__(self):
+        return f'Membership: Name - {self.name}, ID - {self.id}'
+
+    def __repr__(self):
+        return f'<Membership name=\'{self.name}>\' id={self.id}>'
+
+class Voice:
+    """
+    This is a model class Voice that represents a voice.
+
+    Attributes:
+        `architecture (str)`: The architecture of the voice i.e. the engine that was used to make the voice.
+        `category (str)`: The category of the voice i.e. where it's from (WWE, SpongeBob etc).
+        `contributors (list)`: The contributors' names of the voice.
+        `controls (bool)`: Whether the voice has controls.
+        `display_name (str)`: The display name of the voice i.e. a better formatted name to show to general users.
+        `is_active (bool)`: Whether the voice is active.
+        `model_id (str)`: The model ID of the voice. This is not a unique identification, the name is.
+        `memberships (list)`: The memberships of the voice.
+        `is_private (bool)`: Whether the voice is private.
+        `name (str)`: The name of the voice i.e. the name you pass to the API in order for it to recognize which voice you want.
+        `symbol_set (str)`: The symbol set of the voice.
+        `voicemodel_uuid (str)`: The voice model's UUID.
+        `added_at (datetime)`: The date and time the model was added at.
+        `is_primary: (bool)`: Whether the voice is added to the Uberduck.ai site.
+        `hifi_gan_vocoder: (str)`: The HIFI-gan vocoder used to improve the voice.
+        `ml_model_id: (int)`: The ID of the machine learning model.
+        `speaker_id: (int)`: The ID of the person doing the voice.
+        `language: (str)`: The language the voice was trained for.
+
+    Magic methods:
+        `__str__`: Returns a string representation of the Voice object in the format `Voice: Architecture - {architecture}, Category - {category}, Contributors - {contributors}, Controls - {controls}, Display Name - {display_name}, Is Active - {is_active},  Model ID - {model_id}, Memberships - {memberships}, Is Private - {is_private}, Name - {name}, Symbol Set - {symbol_set}, Voice model UUID - {voicemodel_uuid}, Added At - {added_at}, Is Primary - {is_primary}, Hifi Gan Vocoder - {hifi_gan_vocoder}, ML Model ID - {ml_model_id}, Speaker ID - {speaker_id}, Language {language}`.
+        `__repr__`: Returns a string representation of the Voice object in the format `<Voice architecture='{architecture}' category='{category}' contributors='{contributors}' controls='{controls}' display_name='{display_name}' is_active='{is_active}' model_id='{model_id}' memberships='{memberships}' is_private='{is_private}' name='{name}' symbol_set='{symbol_set}' voicemodel_uuid='{voicemodel_uuid}' added_at='{added_at}' is_primary='{is_primary}' hifi_gan_vocoder='{hifi_gan_vocoder}' ml_model_id='{ml_model_id}' speaker_id='{speaker_id}' language='{language}'>`.
+
+    This class is read-only.
+    """
+    def __init__(
+        self,
+        architecture: str,
+        category: str,
+        contributors: List[str],
+        controls: bool,
+        display_name: str,
+        is_active: bool,
+        model_id: str,
+        memberships: list,
+        is_private: bool,
+        name: str,
+        symbol_set: str,
+        voicemodel_uuid: str,
+        added_at: float,
+        is_primary: bool,
+        hifi_gan_vocoder: str,
+        ml_model_id: int,
+        speaker_id: Optional[int],
+        language: str
+    ) -> None:
+        self.architecture = architecture
+        self.category = category
+        self.contributors = contributors
+        self.controls = controls
+        self.display_name = display_name
+        self.is_active = is_active
+        self.model_id = model_id
+        self.memberships = memberships
+        if self.memberships:
+            self.memberships: List[Membership] = [Membership(*memberships)]
+        self.is_private = is_private
+        self.name = name
+        self.symbol_set = symbol_set
+        self.voicemodel_uuid = voicemodel_uuid
+        self.added_at: dt = dt.fromtimestamp(added_at)
+        self.is_primary = is_primary
+        self.hifi_gan_vocoder = hifi_gan_vocoder
+        self.ml_model_id = ml_model_id
+        self.speaker_id = speaker_id
+        self.language = language
+
+    def __str__(self):
+        time = self.added_at.strftime('%a, %B %d %Y, %I:%M:%S %p UTC')
+        return f'Voice: Architecture - {self.architecture}, Category - {self.category}, Contributors - {self.contributors}, Controls - {self.controls}, Display Name - {self.display_name}, Is Active - {self.is_active},  Model ID - {self.model_id}, Memberships - {self.memberships}, Is Private - {self.is_private}, Name - {self.name}, Symbol Set - {self.symbol_set}, Voice model UUID - {self.voicemodel_uuid}, Added At - {time}, Is Primary - {self.is_primary}, Hifi Gan Vocoder - {self.hifi_gan_vocoder}, ML Model ID - {self.ml_model_id}, Speaker ID - {self.speaker_id}, Language {self.language}'
+
+    def __repr__(self):
+        return f'<Voice architecture=\'{self.architecture}\' category=\'{self.category}\' contributors=\'{self.contributors}\' controls=\'{self.controls}\' display_name=\'{self.display_name}\' is_active=\'{self.is_active}\' model_id=\'{self.model_id}\' memberships=\'{self.memberships}\' is_private=\'{self.is_private}\' name=\'{self.name}\' symbol_set=\'{self.symbol_set}\' voicemodel_uuid=\'{self.voicemodel_uuid}\' added_at=\'{dt.timestamp(self.added_at)}\' is_primary=\'{self.is_primary}\' hifi_gan_vocoder=\'{self.hifi_gan_vocoder}\' ml_model_id=\'{self.ml_model_id}\' speaker_id=\'{self.speaker_id}\' language=\'{self.language}\'>'
+
+class UberduckException(Exception):
+    """
+    Base class for all exceptions raised by Uberduck. This exception could be used to catch any exceptions thrown by this library.
+    """
+    pass
+
+class InvalidVoice(UberduckException):
+    """
+    Raised when an invalid voice is specified. See all the voices from `uberduck.get_voices()`, `uberduck.get_voices_async()` or [uberduck.ai/quack-help](https://uberduck.ai/quack-help).
+    """
+    def __init__(self, voice: str) -> None:
+        self.voice = voice
+        super().__init__(f'Invalid voice: {voice}.')
+
+class Unauthorized(UberduckException):
+    """
+    Exception raised when your API key is invalid or your API secret is invalid. Get an API key and secret from [uberduck.ai/account/manage](https://uberduck.ai/account/manage).
+    """
+    def __init__(self) -> None:
+        super().__init__('Invalid API credentials. Please check your api key and/or api secret.')
+
+class Ratelimited(UberduckException):
+    """
+    Exception raised when you are being ratelimited from the API.
+    """
+    def __init__(self) -> None:
+        super().__init__('You are being ratelimited from the API. Please try again later.')
+
+class HTTPException(UberduckException):
+    """
+    Exception raised when the HTTP request fails due to an unknown cause.
+    """
+    def __init__(self, status_code: int, detail) -> None:
+        self.status_code = status_code
+        self.detail = detail
         super().__init__(f'Unexpected HTTP response with status code {status_code} and detail {detail}.')
```

### Comparing `uberduck-0.0.3/uberduck/main.py` & `uberduck-0.0.4/uberduck/main.py`

 * *Files identical despite different names*

### Comparing `uberduck-0.0.3/uberduck.egg-info/PKG-INFO` & `uberduck-0.0.4/uberduck.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-Metadata-Version: 2.1
-Name: uberduck
-Version: 0.0.3
-Summary: A synchronous and asynchronous API wrapper for the UberDuck text-to-speech service (https://uberduck.ai) with 100% coverage and top-notch utilities.
-Home-page: https://github.com/ImNimboss/uberduck
-Author: ImNimboss
-Author-email: nim@nimboss.me
-License: MIT
-Project-URL: Documentation, https://github.com/ImNimboss/uberduck/tree/main/Documentation
-Project-URL: Issue Tracker, https://github.com/ImNimboss/uberduck/issues
-Project-URL: Source, https://github.com/ImNimboss/uberduck
-Project-URL: Funding, https://patreon.com/nimboss
-Project-URL: API Credits, https://uberduck.ai
-Project-URL: Creator, https://nimboss.me
-Project-URL: Discord, https://discord.gg/FcxqdJ7AQq
-Project-URL: Repository, https://github.com/ImNimboss/uberduck
-Keywords: uberduck,wrapper,api,text-to-speech,async,famous,tts,texttospeech,AI,api-wrapper,api-key,api-secret
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Artistic Software
-Classifier: Topic :: Games/Entertainment
-Classifier: Topic :: Internet
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: Multimedia :: Sound/Audio :: Players
-Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/ImNimboss/uberduck/main/.github/assets/uberduck-logo.png" alt="Uberduck Logo">
-</p>
-
-# Uberduck
-
-<a href="https://pypi.org/project/uberduck" target="_blank" rel="noopener noreferrer">
-    <img src="https://img.shields.io/pypi/v/uberduck.svg?color=9cf&logo=pypi" alt="PyPI Uberduck version number">
-    <img src="https://img.shields.io/pypi/dm/uberduck?color=9cf&logo=pypi" alt="PyPI downloads per month">
-    <img src="https://img.shields.io/pypi/pyversions/uberduck.svg?color=9cf&logo=pypi" alt="PyPI supported Python versions">
-</a>
-<a href="https://github.com/ImNimboss/uberduck/issues" target="_blank" rel="noopener noreferrer">
-    <img src="https://img.shields.io/github/issues/ImNimboss/uberduck?color=9cf&logo=github" alt="Number of open GitHub issues">
-</a>
-<a href="https://github.com/ImNimboss/uberduck/contributors" target="_blank" rel="noopener noreferrer">
-    <img src="https://img.shields.io/github/contributors/ImNimboss/uberduck?color=9cf&logo=github" alt="Number of contributors">
-</a>
-<a href="https://discord.gg/FcxqdJ7AQq" target="_blank" rel="noopener noreferrer">
-    <img src="https://img.shields.io/discord/930791886522810399?color=9cf&logo=discord&label=discord" alt="Discord server">
-</a>
-
-## Description
-
-A synchronous and asynchronous API wrapper for the [UberDuck](https://uberduck.ai) text-to-speech service with 100% coverage and top-notch utilities.
-
-## Main features
-
-- [x] - Synchronous support
-- [x] - Asynchronous support
-- [x] - Object-oriented
-- [x] - Easy to use
-- [x] - Utilities like file-saving, audio-playing etc. packed all in one
-- [x] - Very adjustable/configurable
-- [x] - Regularly maintained
-- [x] - Makes the hard tasks of polling and asynchronous operations easy
-
-## Links
-
-* [Documentation](https://github.com/ImNimboss/uberduck/tree/main/Documentation)
-* [PyPI](https://pypi.org/project/uberduck)
-* [Issue Tracking](https://github.com/ImNimboss/uberduck/issues)
-* [Discord server](https://discord.gg/FcxqdJ7AQq)
-* [Uberduck main site](https://uberduck.ai)
-
-
-## Installation and upgrades
-
-```
-pip install uberduck
-```
-for the stable version (recommended).
-
-```
-pip install -U uberduck
-```
-to update your stable version.
-
-```
-pip install git+https://github.com/ImNimboss/uberduck
-```
-to install it straight off of GitHub (you need git installed for this).
-
-```
-pip install -U git+https://github.com/ImNimboss/uberduck
-```
-to upgrade your version that you got from GitHub.
-
-## How to use
-
-Check [Documentation/Basics.md](https://github.com/ImNimboss/uberduck/blob/master/Documentation/Basics.md).
-
-## Examples
-
-Check [Documentation/Examples.md](https://github.com/ImNimboss/uberduck/blob/master/Documentation/Examples.md).
-
-## Some credits
-
-The idea to implement logging in this library came from [discord.py](https://github.com/Rapptz/discord.py).
-
-The idea to use the `polling` library came from [CupOfGeo/UberDuckAPI](https://github.com/CupOfGeo/UberDuckAPI), another uberduck.ai API wrapper.
-
-## Changelog
-
-* `v0.0.1` - Initial release.
-* `v0.0.2` - Fixed `get_voices()` and `get_voices_async()` by updating the `Voice` class to be compatible with the new voice data available from the API.
-
+Metadata-Version: 2.1
+Name: uberduck
+Version: 0.0.4
+Summary: A synchronous and asynchronous API wrapper for the UberDuck text-to-speech service (https://uberduck.ai) with 100% coverage and top-notch utilities.
+Home-page: https://github.com/ImNimboss/uberduck
+Author: ImNimboss
+Author-email: nimit.grover24@gmail.com
+License: MIT
+Project-URL: Documentation, https://github.com/ImNimboss/uberduck/tree/main/Documentation
+Project-URL: Issue Tracker, https://github.com/ImNimboss/uberduck/issues
+Project-URL: Source, https://github.com/ImNimboss/uberduck
+Project-URL: Funding, https://patreon.com/nimboss
+Project-URL: API Credits, https://uberduck.ai
+Project-URL: Creator, https://nimboss.me
+Project-URL: Discord, https://discord.gg/FcxqdJ7AQq
+Project-URL: Repository, https://github.com/ImNimboss/uberduck
+Keywords: uberduck,wrapper,api,text-to-speech,async,famous,tts,texttospeech,AI,api-wrapper,api-key,api-secret
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Artistic Software
+Classifier: Topic :: Games/Entertainment
+Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Sound/Audio :: Players
+Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/ImNimboss/uberduck/main/.github/assets/uberduck-logo.png" alt="Uberduck Logo">
+</p>
+
+# Uberduck
+
+<a href="https://pypi.org/project/uberduck" target="_blank" rel="noopener noreferrer">
+    <img src="https://img.shields.io/pypi/v/uberduck.svg?color=9cf&logo=pypi" alt="PyPI Uberduck version number">
+    <img src="https://img.shields.io/pypi/dm/uberduck?color=9cf&logo=pypi" alt="PyPI downloads per month">
+    <img src="https://img.shields.io/pypi/pyversions/uberduck.svg?color=9cf&logo=pypi" alt="PyPI supported Python versions">
+</a>
+<a href="https://github.com/ImNimboss/uberduck/issues" target="_blank" rel="noopener noreferrer">
+    <img src="https://img.shields.io/github/issues/ImNimboss/uberduck?color=9cf&logo=github" alt="Number of open GitHub issues">
+</a>
+<a href="https://github.com/ImNimboss/uberduck/contributors" target="_blank" rel="noopener noreferrer">
+    <img src="https://img.shields.io/github/contributors/ImNimboss/uberduck?color=9cf&logo=github" alt="Number of contributors">
+</a>
+<a href="https://discord.gg/FcxqdJ7AQq" target="_blank" rel="noopener noreferrer">
+    <img src="https://img.shields.io/discord/930791886522810399?color=9cf&logo=discord&label=discord" alt="Discord server">
+</a>
+
+## Description
+
+A synchronous and asynchronous API wrapper for the [UberDuck](https://uberduck.ai) text-to-speech service with 100% coverage and top-notch utilities.
+
+## Main features
+
+- [x] - Synchronous support
+- [x] - Asynchronous support
+- [x] - Object-oriented
+- [x] - Easy to use
+- [x] - Utilities like file-saving, audio-playing etc. packed all in one
+- [x] - Very adjustable/configurable
+- [x] - Regularly maintained
+- [x] - Makes the hard tasks of polling and asynchronous operations easy
+
+## Links
+
+* [Documentation](https://github.com/ImNimboss/uberduck/tree/main/Documentation)
+* [PyPI](https://pypi.org/project/uberduck)
+* [Issue Tracking](https://github.com/ImNimboss/uberduck/issues)
+* [Discord server](https://discord.gg/FcxqdJ7AQq)
+* [Uberduck main site](https://uberduck.ai)
+
+
+## Installation and upgrades
+
+```
+pip install uberduck
+```
+for the stable version (recommended).
+
+```
+pip install -U uberduck
+```
+to update your stable version.
+
+```
+pip install git+https://github.com/ImNimboss/uberduck
+```
+to install it straight off of GitHub (you need git installed for this).
+
+```
+pip install -U git+https://github.com/ImNimboss/uberduck
+```
+to upgrade your version that you got from GitHub.
+
+## How to use
+
+Check [Documentation/Basics.md](https://github.com/ImNimboss/uberduck/blob/master/Documentation/Basics.md).
+
+## Examples
+
+Check [Documentation/Examples.md](https://github.com/ImNimboss/uberduck/blob/master/Documentation/Examples.md).
+
+## Some credits
+
+The idea to implement logging in this library came from [discord.py](https://github.com/Rapptz/discord.py).
+
+The idea to use the `polling` library came from [CupOfGeo/UberDuckAPI](https://github.com/CupOfGeo/UberDuckAPI), another uberduck.ai API wrapper.
+
+## Changelog
+
+* `v0.0.1` - Initial release.
+* `v0.0.2` - Fixed `get_voices()` and `get_voices_async()` by updating the `Voice` class to be compatible with the new voice data available from the API.
+* `v0.0.3` - Moved `README.md` from `.github` to root folder due to compatibility issues with other software
+* `v0.0.4` - Added attributes `added_at`, `is_primary`, `hifi_gan_vocoder`, `ml_model_id`, `speaker_id`, `language` to `Voice` class
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: uberduck Version: 0.0.3 Summary: A synchronous and
+Metadata-Version: 2.1 Name: uberduck Version: 0.0.4 Summary: A synchronous and
 asynchronous API wrapper for the UberDuck text-to-speech service (https://
 uberduck.ai) with 100% coverage and top-notch utilities. Home-page: https://
-github.com/ImNimboss/uberduck Author: ImNimboss Author-email: nim@nimboss.me
-License: MIT Project-URL: Documentation, https://github.com/ImNimboss/uberduck/
-tree/main/Documentation Project-URL: Issue Tracker, https://github.com/
-ImNimboss/uberduck/issues Project-URL: Source, https://github.com/ImNimboss/
-uberduck Project-URL: Funding, https://patreon.com/nimboss Project-URL: API
-Credits, https://uberduck.ai Project-URL: Creator, https://nimboss.me Project-
-URL: Discord, https://discord.gg/FcxqdJ7AQq Project-URL: Repository, https://
-github.com/ImNimboss/uberduck Keywords: uberduck,wrapper,api,text-to-
-speech,async,famous,tts,texttospeech,AI,api-wrapper,api-key,api-secret
-Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
-:: MIT License Classifier: Natural Language :: English Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+github.com/ImNimboss/uberduck Author: ImNimboss Author-email:
+nimit.grover24@gmail.com License: MIT Project-URL: Documentation, https://
+github.com/ImNimboss/uberduck/tree/main/Documentation Project-URL: Issue
+Tracker, https://github.com/ImNimboss/uberduck/issues Project-URL: Source,
+https://github.com/ImNimboss/uberduck Project-URL: Funding, https://
+patreon.com/nimboss Project-URL: API Credits, https://uberduck.ai Project-URL:
+Creator, https://nimboss.me Project-URL: Discord, https://discord.gg/FcxqdJ7AQq
+Project-URL: Repository, https://github.com/ImNimboss/uberduck Keywords:
+uberduck,wrapper,api,text-to-speech,async,famous,tts,texttospeech,AI,api-
+wrapper,api-key,api-secret Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: MIT License Classifier: Natural Language :: English Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Topic :: Artistic Software Classifier:
 Topic :: Games/Entertainment Classifier: Topic :: Internet Classifier: Topic ::
 Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic
 Content Classifier: Topic :: Multimedia :: Sound/Audio Classifier: Topic ::
@@ -52,8 +52,11 @@
 [Documentation/Examples.md](https://github.com/ImNimboss/uberduck/blob/master/
 Documentation/Examples.md). ## Some credits The idea to implement logging in
 this library came from [discord.py](https://github.com/Rapptz/discord.py). The
 idea to use the `polling` library came from [CupOfGeo/UberDuckAPI](https://
 github.com/CupOfGeo/UberDuckAPI), another uberduck.ai API wrapper. ## Changelog
 * `v0.0.1` - Initial release. * `v0.0.2` - Fixed `get_voices()` and
 `get_voices_async()` by updating the `Voice` class to be compatible with the
-new voice data available from the API.
+new voice data available from the API. * `v0.0.3` - Moved `README.md` from
+`.github` to root folder due to compatibility issues with other software *
+`v0.0.4` - Added attributes `added_at`, `is_primary`, `hifi_gan_vocoder`,
+`ml_model_id`, `speaker_id`, `language` to `Voice` class
```

