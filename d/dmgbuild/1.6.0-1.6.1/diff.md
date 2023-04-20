# Comparing `tmp/dmgbuild-1.6.0.tar.gz` & `tmp/dmgbuild-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmgbuild-1.6.0.tar", last modified: Thu Nov 24 06:18:24 2022, max compression
+gzip compressed data, was "dmgbuild-1.6.1.tar", last modified: Thu Apr 20 12:39:21 2023, max compression
```

## Comparing `dmgbuild-1.6.0.tar` & `dmgbuild-1.6.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2022-11-24 06:18:24.931523 dmgbuild-1.6.0/
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2022-11-24 06:18:24.920493 dmgbuild-1.6.0/.github/
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2022-11-24 06:18:24.924732 dmgbuild-1.6.0/.github/workflows/
--rw-r--r--   0 rkm        (501) staff       (20)     1466 2022-11-24 05:32:37.000000 dmgbuild-1.6.0/.github/workflows/ci.yml
--rw-r--r--   0 rkm        (501) staff       (20)      119 2022-11-24 05:00:55.000000 dmgbuild-1.6.0/.gitignore
--rw-r--r--   0 rkm        (501) staff       (20)      900 2022-11-24 05:32:37.000000 dmgbuild-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0 rkm        (501) staff       (20)      638 2022-11-24 05:32:37.000000 dmgbuild-1.6.0/.readthedocs.yaml
--rw-r--r--   0 rkm        (501) staff       (20)     1100 2022-06-21 01:38:55.000000 dmgbuild-1.6.0/LICENSE
--rw-r--r--   0 rkm        (501) staff       (20)      363 2022-11-24 05:32:37.000000 dmgbuild-1.6.0/MANIFEST.in
--rw-r--r--   0 rkm        (501) staff       (20)     2676 2022-11-24 06:18:24.931647 dmgbuild-1.6.0/PKG-INFO
--rw-r--r--   0 rkm        (501) staff       (20)     1514 2022-11-24 05:01:12.000000 dmgbuild-1.6.0/README.rst
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2022-11-24 06:18:24.926230 dmgbuild-1.6.0/docs/
--rw-r--r--   0 rkm        (501) staff       (20)     6770 2022-06-21 07:53:33.000000 dmgbuild-1.6.0/docs/Makefile
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2022-11-24 06:18:24.926427 dmgbuild-1.6.0/docs/_static/
--rw-r--r--   0 rkm        (501) staff       (20)       26 2022-11-24 05:32:37.000000 dmgbuild-1.6.0/docs/_static/README.rst
--rw-r--r--   0 rkm        (501) staff       (20)     8764 2022-11-24 05:32:37.000000 dmgbuild-1.6.0/docs/conf.py
--rw-r--r--   0 rkm        (501) staff       (20)      221 2022-11-24 05:01:12.000000 dmgbuild-1.6.0/docs/example.rst
--rw-r--r--   0 rkm        (501) staff       (20)     1463 2022-11-24 05:32:37.000000 dmgbuild-1.6.0/docs/index.rst
--rw-r--r--   0 rkm        (501) staff       (20)     6705 2022-06-21 07:53:33.000000 dmgbuild-1.6.0/docs/make.bat
--rw-r--r--   0 rkm        (501) staff       (20)    15833 2022-11-24 06:16:39.000000 dmgbuild-1.6.0/docs/settings.rst
--rw-r--r--   0 rkm        (501) staff       (20)      550 2022-06-21 07:53:33.000000 dmgbuild-1.6.0/docs/usage.rst
--rw-r--r--   0 rkm        (501) staff       (20)      201 2022-11-24 05:32:37.000000 dmgbuild-1.6.0/pyproject.toml
--rw-r--r--   0 rkm        (501) staff       (20)     1701 2022-11-24 06:18:24.932111 dmgbuild-1.6.0/setup.cfg
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2022-11-24 06:18:24.921003 dmgbuild-1.6.0/src/
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2022-11-24 06:18:24.928525 dmgbuild-1.6.0/src/dmgbuild/
--rw-r--r--   0 rkm        (501) staff       (20)       91 2022-11-24 06:17:48.000000 dmgbuild-1.6.0/src/dmgbuild/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     1512 2022-11-24 05:32:37.000000 dmgbuild-1.6.0/src/dmgbuild/__main__.py
--rw-r--r--   0 rkm        (501) staff       (20)     6176 2022-11-24 05:32:37.000000 dmgbuild-1.6.0/src/dmgbuild/badge.py
--rw-r--r--   0 rkm        (501) staff       (20)    12881 2022-11-24 05:32:37.000000 dmgbuild-1.6.0/src/dmgbuild/colors.py
--rw-r--r--   0 rkm        (501) staff       (20)    27986 2022-11-24 05:59:54.000000 dmgbuild-1.6.0/src/dmgbuild/core.py
--rw-r--r--   0 rkm        (501) staff       (20)    10858 2022-11-24 05:32:37.000000 dmgbuild-1.6.0/src/dmgbuild/licensing.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2022-11-24 06:18:24.930580 dmgbuild-1.6.0/src/dmgbuild/resources/
--rw-r--r--   0 rkm        (501) staff       (20)    26264 2022-06-21 07:53:33.000000 dmgbuild-1.6.0/src/dmgbuild/resources/builtin-arrow.tiff
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2022-11-24 06:18:24.930384 dmgbuild-1.6.0/src/dmgbuild.egg-info/
--rw-r--r--   0 rkm        (501) staff       (20)     2676 2022-11-24 06:18:24.000000 dmgbuild-1.6.0/src/dmgbuild.egg-info/PKG-INFO
--rw-r--r--   0 rkm        (501) staff       (20)      804 2022-11-24 06:18:24.000000 dmgbuild-1.6.0/src/dmgbuild.egg-info/SOURCES.txt
--rw-r--r--   0 rkm        (501) staff       (20)        1 2022-11-24 06:18:24.000000 dmgbuild-1.6.0/src/dmgbuild.egg-info/dependency_links.txt
--rw-r--r--   0 rkm        (501) staff       (20)       52 2022-11-24 06:18:24.000000 dmgbuild-1.6.0/src/dmgbuild.egg-info/entry_points.txt
--rw-r--r--   0 rkm        (501) staff       (20)        1 2022-06-21 02:22:32.000000 dmgbuild-1.6.0/src/dmgbuild.egg-info/not-zip-safe
--rw-r--r--   0 rkm        (501) staff       (20)      188 2022-11-24 06:18:24.000000 dmgbuild-1.6.0/src/dmgbuild.egg-info/requires.txt
--rw-r--r--   0 rkm        (501) staff       (20)        9 2022-11-24 06:18:24.000000 dmgbuild-1.6.0/src/dmgbuild.egg-info/top_level.txt
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2022-11-24 06:18:24.930956 dmgbuild-1.6.0/tests/
--rw-r--r--   0 rkm        (501) staff       (20)        0 2022-06-21 01:38:55.000000 dmgbuild-1.6.0/tests/__init__.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2022-11-24 06:18:24.931355 dmgbuild-1.6.0/tests/examples/
--rw-r--r--   0 rkm        (501) staff       (20)      420 2022-11-24 05:59:43.000000 dmgbuild-1.6.0/tests/examples/settings.json
--rw-r--r--   0 rkm        (501) staff       (20)     8434 2022-11-24 05:32:37.000000 dmgbuild-1.6.0/tests/examples/settings.py
--rw-r--r--   0 rkm        (501) staff       (20)      570 2022-11-24 06:16:39.000000 dmgbuild-1.6.0/tests/test_samples.py
--rw-r--r--   0 rkm        (501) staff       (20)      980 2022-11-24 05:32:37.000000 dmgbuild-1.6.0/tox.ini
+drwxr-xr-x   0 rkm        (501) staff       (20)        0 2023-04-20 12:39:21.622618 dmgbuild-1.6.1/
+drwxr-xr-x   0 rkm        (501) staff       (20)        0 2023-04-20 12:39:21.614164 dmgbuild-1.6.1/.github/
+drwxr-xr-x   0 rkm        (501) staff       (20)        0 2023-04-20 12:39:21.617318 dmgbuild-1.6.1/.github/workflows/
+-rw-r--r--   0 rkm        (501) staff       (20)     1466 2022-11-24 05:32:37.000000 dmgbuild-1.6.1/.github/workflows/ci.yml
+-rw-r--r--   0 rkm        (501) staff       (20)      119 2022-11-24 05:00:55.000000 dmgbuild-1.6.1/.gitignore
+-rw-r--r--   0 rkm        (501) staff       (20)      717 2023-04-20 12:37:21.000000 dmgbuild-1.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 rkm        (501) staff       (20)      638 2022-11-24 05:32:37.000000 dmgbuild-1.6.1/.readthedocs.yaml
+-rw-r--r--   0 rkm        (501) staff       (20)     1100 2022-06-21 01:38:55.000000 dmgbuild-1.6.1/LICENSE
+-rw-r--r--   0 rkm        (501) staff       (20)      363 2022-11-24 05:32:37.000000 dmgbuild-1.6.1/MANIFEST.in
+-rw-r--r--   0 rkm        (501) staff       (20)     2676 2023-04-20 12:39:21.622731 dmgbuild-1.6.1/PKG-INFO
+-rw-r--r--   0 rkm        (501) staff       (20)     1514 2022-11-24 05:01:12.000000 dmgbuild-1.6.1/README.rst
+drwxr-xr-x   0 rkm        (501) staff       (20)        0 2023-04-20 12:39:21.618656 dmgbuild-1.6.1/docs/
+-rw-r--r--   0 rkm        (501) staff       (20)     6770 2022-06-21 07:53:33.000000 dmgbuild-1.6.1/docs/Makefile
+drwxr-xr-x   0 rkm        (501) staff       (20)        0 2023-04-20 12:39:21.618853 dmgbuild-1.6.1/docs/_static/
+-rw-r--r--   0 rkm        (501) staff       (20)       26 2022-11-24 05:32:37.000000 dmgbuild-1.6.1/docs/_static/README.rst
+-rw-r--r--   0 rkm        (501) staff       (20)     8764 2022-11-24 05:32:37.000000 dmgbuild-1.6.1/docs/conf.py
+-rw-r--r--   0 rkm        (501) staff       (20)      221 2022-11-24 05:01:12.000000 dmgbuild-1.6.1/docs/example.rst
+-rw-r--r--   0 rkm        (501) staff       (20)     1463 2022-11-24 05:32:37.000000 dmgbuild-1.6.1/docs/index.rst
+-rw-r--r--   0 rkm        (501) staff       (20)     6705 2022-06-21 07:53:33.000000 dmgbuild-1.6.1/docs/make.bat
+-rw-r--r--   0 rkm        (501) staff       (20)    16077 2023-04-20 12:37:21.000000 dmgbuild-1.6.1/docs/settings.rst
+-rw-r--r--   0 rkm        (501) staff       (20)      550 2022-06-21 07:53:33.000000 dmgbuild-1.6.1/docs/usage.rst
+-rw-r--r--   0 rkm        (501) staff       (20)      201 2022-11-24 05:32:37.000000 dmgbuild-1.6.1/pyproject.toml
+-rw-r--r--   0 rkm        (501) staff       (20)     1754 2023-04-20 12:39:21.623225 dmgbuild-1.6.1/setup.cfg
+drwxr-xr-x   0 rkm        (501) staff       (20)        0 2023-04-20 12:39:21.614929 dmgbuild-1.6.1/src/
+drwxr-xr-x   0 rkm        (501) staff       (20)        0 2023-04-20 12:39:21.620089 dmgbuild-1.6.1/src/dmgbuild/
+-rw-r--r--   0 rkm        (501) staff       (20)       91 2023-04-20 12:37:42.000000 dmgbuild-1.6.1/src/dmgbuild/__init__.py
+-rw-r--r--   0 rkm        (501) staff       (20)     1512 2022-11-24 05:32:37.000000 dmgbuild-1.6.1/src/dmgbuild/__main__.py
+-rw-r--r--   0 rkm        (501) staff       (20)     6176 2022-11-24 05:32:37.000000 dmgbuild-1.6.1/src/dmgbuild/badge.py
+-rw-r--r--   0 rkm        (501) staff       (20)    12881 2022-11-24 05:32:37.000000 dmgbuild-1.6.1/src/dmgbuild/colors.py
+-rw-r--r--   0 rkm        (501) staff       (20)    28373 2023-04-20 12:37:21.000000 dmgbuild-1.6.1/src/dmgbuild/core.py
+-rw-r--r--   0 rkm        (501) staff       (20)    10858 2022-11-24 05:32:37.000000 dmgbuild-1.6.1/src/dmgbuild/licensing.py
+drwxr-xr-x   0 rkm        (501) staff       (20)        0 2023-04-20 12:39:21.621661 dmgbuild-1.6.1/src/dmgbuild/resources/
+-rw-r--r--   0 rkm        (501) staff       (20)    26264 2022-06-21 07:53:33.000000 dmgbuild-1.6.1/src/dmgbuild/resources/builtin-arrow.tiff
+drwxr-xr-x   0 rkm        (501) staff       (20)        0 2023-04-20 12:39:21.621466 dmgbuild-1.6.1/src/dmgbuild.egg-info/
+-rw-r--r--   0 rkm        (501) staff       (20)     2676 2023-04-20 12:39:21.000000 dmgbuild-1.6.1/src/dmgbuild.egg-info/PKG-INFO
+-rw-r--r--   0 rkm        (501) staff       (20)      804 2023-04-20 12:39:21.000000 dmgbuild-1.6.1/src/dmgbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 rkm        (501) staff       (20)        1 2023-04-20 12:39:21.000000 dmgbuild-1.6.1/src/dmgbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 rkm        (501) staff       (20)       52 2023-04-20 12:39:21.000000 dmgbuild-1.6.1/src/dmgbuild.egg-info/entry_points.txt
+-rw-r--r--   0 rkm        (501) staff       (20)        1 2022-06-21 02:22:32.000000 dmgbuild-1.6.1/src/dmgbuild.egg-info/not-zip-safe
+-rw-r--r--   0 rkm        (501) staff       (20)      241 2023-04-20 12:39:21.000000 dmgbuild-1.6.1/src/dmgbuild.egg-info/requires.txt
+-rw-r--r--   0 rkm        (501) staff       (20)        9 2023-04-20 12:39:21.000000 dmgbuild-1.6.1/src/dmgbuild.egg-info/top_level.txt
+drwxr-xr-x   0 rkm        (501) staff       (20)        0 2023-04-20 12:39:21.622044 dmgbuild-1.6.1/tests/
+-rw-r--r--   0 rkm        (501) staff       (20)        0 2022-06-21 01:38:55.000000 dmgbuild-1.6.1/tests/__init__.py
+drwxr-xr-x   0 rkm        (501) staff       (20)        0 2023-04-20 12:39:21.622449 dmgbuild-1.6.1/tests/examples/
+-rw-r--r--   0 rkm        (501) staff       (20)      420 2022-11-24 05:59:43.000000 dmgbuild-1.6.1/tests/examples/settings.json
+-rw-r--r--   0 rkm        (501) staff       (20)     8434 2022-11-24 05:32:37.000000 dmgbuild-1.6.1/tests/examples/settings.py
+-rw-r--r--   0 rkm        (501) staff       (20)      570 2023-04-20 12:07:23.000000 dmgbuild-1.6.1/tests/test_samples.py
+-rw-r--r--   0 rkm        (501) staff       (20)      980 2022-11-24 05:32:37.000000 dmgbuild-1.6.1/tox.ini
```

### Comparing `dmgbuild-1.6.0/.github/workflows/ci.yml` & `dmgbuild-1.6.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/.pre-commit-config.yaml` & `dmgbuild-1.6.1/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: check-toml
       - id: check-yaml
       - id: check-case-conflict
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
         additional_dependencies: [toml]
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.2.0
+    rev: v3.3.1
     hooks:
       - id: pyupgrade
         args: [--py37-plus]
-  - repo: https://github.com/myint/docformatter
-    rev: v1.5.0
-    hooks:
-    - id: docformatter
-      args: [--in-place]
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
     - id: black
       language_version: python3
   - repo: https://github.com/PyCQA/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
-        additional_dependencies: [flake8-eradicate==1.4.0]
```

### Comparing `dmgbuild-1.6.0/.readthedocs.yaml` & `dmgbuild-1.6.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/LICENSE` & `dmgbuild-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/PKG-INFO` & `dmgbuild-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmgbuild
-Version: 1.6.0
+Version: 1.6.1
 Summary: macOS command line utility to build disk images
 Home-page: http://alastairs-place.net/projects/dmgbuild
 Author: Alastair Houghton
 Author-email: alastair@alastairs-place.net
 Maintainer: Russell Keith-Magee
 Maintainer-email: russell@keith-magee.com
 License: MIT License
```

### Comparing `dmgbuild-1.6.0/README.rst` & `dmgbuild-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/docs/Makefile` & `dmgbuild-1.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/docs/conf.py` & `dmgbuild-1.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/docs/index.rst` & `dmgbuild-1.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/docs/make.bat` & `dmgbuild-1.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/docs/settings.rst` & `dmgbuild-1.6.1/docs/settings.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
    ====  =========================
    Code  Meaning
    ====  =========================
    UDRO  Read-only
    UDCO  Compressed (ADC)
    UDZO  Compressed (gzip)
    UDBZ  Compressed (bzip2)
+   ULFO  Compressed (lzfse - macOS 10.11+ only)
+   ULMO  Compressed (lzma - macOS 10.15+ only)
    UFBI  Entire device
    IPOD  iPod image
    UDxx  UDIF stub
    UDSB  Sparse bundle
    UDSP  Sparse
    UDRW  Read/write
    UDTO  DVD/CD master
@@ -55,14 +57,19 @@
    ROCo  NDIF Compressed
    Rken  NDIF Compressed (KenCode)
    ====  =========================
 
    For disk images you intend to distribute over the Internet, you
    should probably stick to 'UDZO' and 'UDBZ'.
 
+.. py:data:: filesystem
+
+   Specifies the filesystem for the output disk image.  Must be
+   either 'HFS+' (the default) or 'APFS' (macOS 10.13+ only).
+
 .. py:data:: size
 
    If defined, specifies the size of the filesystem within the image.
    If this is not defined, ``dmgbuild`` will attempt to determine a
    reasonable size for the image.
 
    If you set this, you should set it large enough to hold the files you
@@ -121,18 +128,18 @@
    As an alternative to the above, if you set `badge_icon` to the path
    of an icon file or image, it will be used to badge the system's
    standard external disk icon.  This is a convenient way to construct
    a suitable icon from your application's icon, e.g.::
 
      badge_icon = '/Applications/TextEdit.app/Contents/Resources/Edit.icns'
 
-   The use of badge icons requires that ``dmg_build`` be installed with the
-   ``badge_icons`` extra; i.e., you need to install dmg_build using::
+   The use of badge icons requires that ``dmgbuild`` be installed with the
+   ``badge_icons`` extra; i.e., you need to install dmgbuild using::
 
-      pip install "dmg_build[badge_icons]"
+      pip install "dmgbuild[badge_icons]"
 
 .. py:data:: icon_locations
 
    A dictionary specifying the co-ordinates of items in the root
    directory of the disk image, where the keys are filenames and the
    values are (x, y) tuples. e.g.::
```

### Comparing `dmgbuild-1.6.0/docs/usage.rst` & `dmgbuild-1.6.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/setup.cfg` & `dmgbuild-1.6.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 python_requires = >= 3.7
 include_package_data = True
 package_dir = 
 	= src
 install_requires = 
 	ds_store >= 1.1.0
 	mac_alias >= 2.0.1
+	importlib_resources == 5.9; python_version <= "3.8"
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	dmgbuild = dmgbuild.__main__:main
```

### Comparing `dmgbuild-1.6.0/src/dmgbuild/__main__.py` & `dmgbuild-1.6.1/src/dmgbuild/__main__.py`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/src/dmgbuild/badge.py` & `dmgbuild-1.6.1/src/dmgbuild/badge.py`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/src/dmgbuild/colors.py` & `dmgbuild-1.6.1/src/dmgbuild/colors.py`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/src/dmgbuild/core.py` & `dmgbuild-1.6.1/src/dmgbuild/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 import re
 import shutil
 import subprocess
 import tempfile
 import time
 import tokenize
 
-import pkg_resources
+try:
+    import importlib_resources as resources
+except ImportError:
+    from importlib import resources
+
 from ds_store import DSStore
 from mac_alias import Alias, Bookmark
 
 from . import colors, licensing
 
 try:
     from . import badge
@@ -97,14 +101,15 @@
     pos = wnd.get("position", {"x": 100, "y": 100})
     siz = wnd.get("size", {"width": 640, "height": 480})
     settings["window_rect"] = (
         (pos.get("x", 100), pos.get("y", 100)),
         (siz.get("width", 640), siz.get("height", 480)),
     )
     settings["format"] = json_data.get("format", "UDZO")
+    settings["filesystem"] = json_data.get("filesystem", "HFS+")
     settings["compression_level"] = json_data.get("compression-level", None)
     settings["license"] = json_data.get("license", None)
     files = []
     hide = []
     hide_extensions = []
     symlinks = {}
     icon_locations = {}
@@ -151,14 +156,15 @@
     callback=quiet_callback,
 ):
     options = {
         # Default settings
         "filename": filename,
         "volume_name": volume_name,
         "format": "UDBZ",
+        "filesystem": "HFS+",
         "compression_level": None,
         "size": None,
         "files": [],
         "symlinks": {},
         "hide": [],
         "hide_extensions": [],
         "icon": None,
@@ -456,23 +462,26 @@
     callback(
         {
             "type": "command::start",
             "command": "hdiutil::create",
         }
     )
 
+    filesystem = options["filesystem"].upper()
+    fs_args = "-c c=64,a=16,e=16" if filesystem != "APFS" else ""
+
     ret, output = hdiutil(
         "create",
         "-ov",
         "-volname",
         volume_name,
         "-fs",
-        "HFS+",
+        filesystem,
         "-fsargs",
-        "-c c=64,a=16,e=16",
+        fs_args,
         "-size",
         total_size,
         writableFile.name,
     )
 
     callback(
         {
@@ -607,26 +616,26 @@
                                 'unable to compile combined HiDPI file "%s" got error: %s\noutput: %s'
                                 % (background, str(e), output.read())
                             )
 
                 _, kind = os.path.splitext(background)
                 path_in_image = os.path.join(mount_point, ".background" + kind)
                 shutil.copyfile(background, path_in_image)
-            elif pkg_resources.resource_exists(
-                "dmgbuild", "resources/" + background + ".tiff"
-            ):
-                tiffdata = pkg_resources.resource_string(
-                    "dmgbuild", "resources/" + background + ".tiff"
-                )
-                path_in_image = os.path.join(mount_point, ".background.tiff")
-
-                with open(path_in_image, "wb") as f:
-                    f.write(tiffdata)
             else:
-                raise ValueError('background file "%s" not found' % background)
+                dmg_resources = resources.files("dmgbuild")
+                bg_resource = dmg_resources.joinpath(
+                    "resources/" + background + ".tiff"
+                )
+                if bg_resource.is_file():
+                    path_in_image = os.path.join(mount_point, ".background.tiff")
+                    with bg_resource.open("rb") as in_file:
+                        with open(path_in_image, "wb") as out_file:
+                            out_file.write(in_file.read())
+                else:
+                    raise ValueError('background file "%s" not found' % background)
 
             alias = Alias.for_file(path_in_image)
             background_bmk = Bookmark.for_file(path_in_image)
 
             icvp["backgroundType"] = 2
             icvp["backgroundImageAlias"] = alias.to_bytes()
 
@@ -849,15 +858,15 @@
     callback(
         {
             "type": "operation::start",
             "operation": "dmg::shrink",
         }
     )
 
-    key_prefix = {"UDZO": "zlib", "UDBZ": "bzip2", "ULFO": "lzfse"}
+    key_prefix = {"UDZO": "zlib", "UDBZ": "bzip2", "ULFO": "lzfse", "ULMO": "lzma"}
     compression_level = options["compression_level"]
     if options["format"] in key_prefix and compression_level:
         compression_args = [
             "-imagekey",
             key_prefix[options["format"]] + "-level=" + str(compression_level),
         ]
     else:
@@ -874,15 +883,15 @@
         "convert",
         writableFile.name,
         "-format",
         options["format"],
         "-ov",
         "-o",
         filename,
-        *compression_args
+        *compression_args,
     )
 
     callback(
         {
             "type": "command::finished",
             "command": "hdiutil::convert",
             "ret": ret,
```

### Comparing `dmgbuild-1.6.0/src/dmgbuild/licensing.py` & `dmgbuild-1.6.1/src/dmgbuild/licensing.py`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/src/dmgbuild/resources/builtin-arrow.tiff` & `dmgbuild-1.6.1/src/dmgbuild/resources/builtin-arrow.tiff`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/src/dmgbuild.egg-info/PKG-INFO` & `dmgbuild-1.6.1/src/dmgbuild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmgbuild
-Version: 1.6.0
+Version: 1.6.1
 Summary: macOS command line utility to build disk images
 Home-page: http://alastairs-place.net/projects/dmgbuild
 Author: Alastair Houghton
 Author-email: alastair@alastairs-place.net
 Maintainer: Russell Keith-Magee
 Maintainer-email: russell@keith-magee.com
 License: MIT License
```

### Comparing `dmgbuild-1.6.0/src/dmgbuild.egg-info/SOURCES.txt` & `dmgbuild-1.6.1/src/dmgbuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/tests/examples/settings.py` & `dmgbuild-1.6.1/tests/examples/settings.py`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/tests/test_samples.py` & `dmgbuild-1.6.1/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `dmgbuild-1.6.0/tox.ini` & `dmgbuild-1.6.1/tox.ini`

 * *Files identical despite different names*

