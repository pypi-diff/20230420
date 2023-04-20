# Comparing `tmp/mypy-boto3-chime-sdk-media-pipelines-1.26.117.tar.gz` & `tmp/mypy-boto3-chime-sdk-media-pipelines-1.26.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-media-pipelines-1.26.117.tar", last modified: Thu Apr 20 19:33:48 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-media-pipelines-1.26.98.tar", last modified: Thu Mar 23 19:33:04 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.117.tar` & `mypy-boto3-chime-sdk-media-pipelines-1.26.98.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:48.459264 mypy-boto3-chime-sdk-media-pipelines-1.26.117/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 19:32:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18008 2023-04-20 19:33:48.459264 mypy-boto3-chime-sdk-media-pipelines-1.26.117/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16450 2023-04-20 19:32:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:48.451264 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-20 19:32:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 19:32:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-20 19:32:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17691 2023-04-20 19:32:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-04-20 19:32:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-04-20 19:32:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-04-20 19:32:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:32:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38611 2023-04-20 19:32:17.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38566 2023-04-20 19:32:17.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 19:32:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:48.459264 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18008 2023-04-20 19:33:48.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-20 19:33:48.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:33:48.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:33:48.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 19:33:48.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 19:33:48.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:33:48.459264 mypy-boto3-chime-sdk-media-pipelines-1.26.117/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-20 19:32:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.117/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.399627 mypy-boto3-chime-sdk-media-pipelines-1.26.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-03-23 19:33:04.395626 mypy-boto3-chime-sdk-media-pipelines-1.26.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.383626 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17691 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38555 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38510 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.395626 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:04.399627 mypy-boto3-chime-sdk-media-pipelines-1.26.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/setup.py
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.117/LICENSE` & `mypy-boto3-chime-sdk-media-pipelines-1.26.98/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.117/PKG-INFO` & `mypy-boto3-chime-sdk-media-pipelines-1.26.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-media-pipelines
-Version: 1.26.117
-Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.26.117 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.98
+Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.26.98 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-media-pipelines"></a>
 
 # mypy-boto3-chime-sdk-media-pipelines
 
 [![PyPI - mypy-boto3-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.117/README.md` & `mypy-boto3-chime-sdk-media-pipelines-1.26.98/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-chime-sdk-media-pipelines"></a>
 
 # mypy-boto3-chime-sdk-media-pipelines
 
 [![PyPI - mypy-boto3-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/__main__.py` & `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMediaPipelines 1.26.117\nVersion:        "
-        " 1.26.117\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMediaPipelines 1.26.98\nVersion:        "
+        " 1.26.98\nBuilder version: 7.14.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.117")
+    print("1.26.98")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/client.py` & `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/client.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/literals.py` & `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ArtifactsConcatenationStateType",
     "ArtifactsStateType",
     "AudioArtifactsConcatenationStateType",
     "AudioChannelsOptionType",
     "AudioMuxTypeType",
     "CallAnalyticsLanguageCodeType",
@@ -55,15 +54,14 @@
     "VoiceAnalyticsConfigurationStatusType",
     "ChimeSDKMediaPipelinesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ArtifactsConcatenationStateType = Literal["Disabled", "Enabled"]
 ArtifactsStateType = Literal["Disabled", "Enabled"]
 AudioArtifactsConcatenationStateType = Literal["Enabled"]
 AudioChannelsOptionType = Literal["Mono", "Stereo"]
 AudioMuxTypeType = Literal["AudioOnly", "AudioWithActiveSpeakerVideo", "AudioWithCompositedVideo"]
 CallAnalyticsLanguageCodeType = Literal[
     "de-DE", "en-AU", "en-GB", "en-US", "es-US", "fr-CA", "fr-FR", "it-IT", "pt-BR"
@@ -434,15 +432,14 @@
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/literals.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ArtifactsConcatenationStateType",
     "ArtifactsStateType",
     "AudioArtifactsConcatenationStateType",
     "AudioChannelsOptionType",
     "AudioMuxTypeType",
     "CallAnalyticsLanguageCodeType",
@@ -54,14 +55,15 @@
     "VoiceAnalyticsConfigurationStatusType",
     "ChimeSDKMediaPipelinesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 ArtifactsConcatenationStateType = Literal["Disabled", "Enabled"]
 ArtifactsStateType = Literal["Disabled", "Enabled"]
 AudioArtifactsConcatenationStateType = Literal["Enabled"]
 AudioChannelsOptionType = Literal["Mono", "Stereo"]
 AudioMuxTypeType = Literal["AudioOnly", "AudioWithActiveSpeakerVideo", "AudioWithCompositedVideo"]
 CallAnalyticsLanguageCodeType = Literal[
     "de-DE", "en-AU", "en-GB", "en-US", "es-US", "fr-CA", "fr-FR", "it-IT", "pt-BR"
@@ -432,15 +434,14 @@
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/type_defs.py` & `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,15 +549,14 @@
     pass
 
 
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
-        "RecordingFileFormat": RecordingFileFormatType,
     },
     total=False,
 )
 
 SnsTopicSinkConfigurationTypeDef = TypedDict(
     "SnsTopicSinkConfigurationTypeDef",
     {
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -534,15 +534,14 @@
 ):
     pass
 
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
-        "RecordingFileFormat": RecordingFileFormatType,
     },
     total=False,
 )
 
 SnsTopicSinkConfigurationTypeDef = TypedDict(
     "SnsTopicSinkConfigurationTypeDef",
     {
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-media-pipelines
-Version: 1.26.117
-Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.26.117 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.98
+Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.26.98 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-media-pipelines"></a>
 
 # mypy-boto3-chime-sdk-media-pipelines
 
 [![PyPI - mypy-boto3-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.117/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.117/setup.py` & `mypy-boto3-chime-sdk-media-pipelines-1.26.98/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-media-pipelines",
-    version="1.26.117",
+    version="1.26.98",
     packages=["mypy_boto3_chime_sdk_media_pipelines"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMediaPipelines 1.26.117 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ChimeSDKMediaPipelines 1.26.98 service generated with"
+        " mypy-boto3-builder 7.14.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

