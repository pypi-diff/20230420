# Comparing `tmp/just_update_arch-0.1.0.tar.gz` & `tmp/just_update_arch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "just_update_arch-0.1.0.tar", last modified: Thu Apr 20 13:28:26 2023, max compression
+gzip compressed data, was "just_update_arch-0.1.1.tar", last modified: Thu Apr 20 13:42:16 2023, max compression
```

## Comparing `just_update_arch-0.1.0.tar` & `just_update_arch-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 maeve     (1000) maeve     (1000)        0 2023-04-20 13:28:26.102515 just_update_arch-0.1.0/
--rw-r--r--   0 maeve     (1000) maeve     (1000)    34916 2023-04-20 13:27:29.000000 just_update_arch-0.1.0/LICENSE.md
--rw-r--r--   0 maeve     (1000) maeve     (1000)     1914 2023-04-20 13:28:26.102515 just_update_arch-0.1.0/PKG-INFO
--rw-r--r--   0 maeve     (1000) maeve     (1000)     1562 2023-04-20 13:27:29.000000 just_update_arch-0.1.0/README.md
-drwxr-xr-x   0 maeve     (1000) maeve     (1000)        0 2023-04-20 13:28:26.102515 just_update_arch-0.1.0/just_update_arch/
--rw-r--r--   0 maeve     (1000) maeve     (1000)        0 2023-04-20 13:27:29.000000 just_update_arch-0.1.0/just_update_arch/__init__.py
--rw-r--r--   0 maeve     (1000) maeve     (1000)     2520 2023-04-20 13:27:29.000000 just_update_arch-0.1.0/just_update_arch/cli.py
-drwxr-xr-x   0 maeve     (1000) maeve     (1000)        0 2023-04-20 13:28:26.102515 just_update_arch-0.1.0/just_update_arch.egg-info/
--rw-r--r--   0 maeve     (1000) maeve     (1000)     1914 2023-04-20 13:28:26.000000 just_update_arch-0.1.0/just_update_arch.egg-info/PKG-INFO
--rw-r--r--   0 maeve     (1000) maeve     (1000)      324 2023-04-20 13:28:26.000000 just_update_arch-0.1.0/just_update_arch.egg-info/SOURCES.txt
--rw-r--r--   0 maeve     (1000) maeve     (1000)        1 2023-04-20 13:28:26.000000 just_update_arch-0.1.0/just_update_arch.egg-info/dependency_links.txt
--rw-r--r--   0 maeve     (1000) maeve     (1000)       65 2023-04-20 13:28:26.000000 just_update_arch-0.1.0/just_update_arch.egg-info/entry_points.txt
--rw-r--r--   0 maeve     (1000) maeve     (1000)        9 2023-04-20 13:28:26.000000 just_update_arch-0.1.0/just_update_arch.egg-info/requires.txt
--rw-r--r--   0 maeve     (1000) maeve     (1000)       17 2023-04-20 13:28:26.000000 just_update_arch-0.1.0/just_update_arch.egg-info/top_level.txt
--rw-r--r--   0 maeve     (1000) maeve     (1000)       38 2023-04-20 13:28:26.102515 just_update_arch-0.1.0/setup.cfg
--rw-r--r--   0 maeve     (1000) maeve     (1000)      956 2023-04-20 13:27:29.000000 just_update_arch-0.1.0/setup.py
+drwxr-xr-x   0 maeve     (1000) maeve     (1000)        0 2023-04-20 13:42:16.912688 just_update_arch-0.1.1/
+-rw-r--r--   0 maeve     (1000) maeve     (1000)    34916 2023-04-20 13:27:29.000000 just_update_arch-0.1.1/LICENSE.md
+-rw-r--r--   0 maeve     (1000) maeve     (1000)     1915 2023-04-20 13:42:16.912688 just_update_arch-0.1.1/PKG-INFO
+-rw-r--r--   0 maeve     (1000) maeve     (1000)     1563 2023-04-20 13:38:48.000000 just_update_arch-0.1.1/README.md
+drwxr-xr-x   0 maeve     (1000) maeve     (1000)        0 2023-04-20 13:42:16.912688 just_update_arch-0.1.1/just_update_arch/
+-rw-r--r--   0 maeve     (1000) maeve     (1000)        0 2023-04-20 13:27:29.000000 just_update_arch-0.1.1/just_update_arch/__init__.py
+-rw-r--r--   0 maeve     (1000) maeve     (1000)     2520 2023-04-20 13:27:29.000000 just_update_arch-0.1.1/just_update_arch/cli.py
+drwxr-xr-x   0 maeve     (1000) maeve     (1000)        0 2023-04-20 13:42:16.912688 just_update_arch-0.1.1/just_update_arch.egg-info/
+-rw-r--r--   0 maeve     (1000) maeve     (1000)     1915 2023-04-20 13:42:16.000000 just_update_arch-0.1.1/just_update_arch.egg-info/PKG-INFO
+-rw-r--r--   0 maeve     (1000) maeve     (1000)      324 2023-04-20 13:42:16.000000 just_update_arch-0.1.1/just_update_arch.egg-info/SOURCES.txt
+-rw-r--r--   0 maeve     (1000) maeve     (1000)        1 2023-04-20 13:42:16.000000 just_update_arch-0.1.1/just_update_arch.egg-info/dependency_links.txt
+-rw-r--r--   0 maeve     (1000) maeve     (1000)       65 2023-04-20 13:42:16.000000 just_update_arch-0.1.1/just_update_arch.egg-info/entry_points.txt
+-rw-r--r--   0 maeve     (1000) maeve     (1000)        9 2023-04-20 13:42:16.000000 just_update_arch-0.1.1/just_update_arch.egg-info/requires.txt
+-rw-r--r--   0 maeve     (1000) maeve     (1000)       17 2023-04-20 13:42:16.000000 just_update_arch-0.1.1/just_update_arch.egg-info/top_level.txt
+-rw-r--r--   0 maeve     (1000) maeve     (1000)       38 2023-04-20 13:42:16.912688 just_update_arch-0.1.1/setup.cfg
+-rw-r--r--   0 maeve     (1000) maeve     (1000)      956 2023-04-20 13:40:20.000000 just_update_arch-0.1.1/setup.py
```

### Comparing `just_update_arch-0.1.0/LICENSE.md` & `just_update_arch-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `just_update_arch-0.1.0/PKG-INFO` & `just_update_arch-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: just_update_arch
-Version: 0.1.0
+Version: 0.1.1
 Summary: Updates installed AUR packages.
 Home-page: https://github.com/MolassesLover/JustUpdateArch
 Author: MolassesLover
 Author-email: 60114762+MolassesLover@users.noreply.github.com
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Just Update Arch
 
 [![Ko-Fi](https://img.shields.io/badge/donate-kofi-blue?style=for-the-badge&logo=ko-fi&color=e57578&logoColor=FFFFFF&labelColor=262a35)](https://ko-fi.com/molasses)
 [![Patreon](https://img.shields.io/badge/donate-patreon-blue?style=for-the-badge&logo=patreon&color=e57578&logoColor=FFFFFF&labelColor=262a35)](https://www.patreon.com/molasseslover)
-[![PyPi](https://img.shields.io/badge/install-pypi-blue?style=for-the-badge&logo=python&color=e57578&logoColor=FFFFFF&labelColor=262a35)](https://pypi.org/project/just_update_arch)
+[![PyPi](https://img.shields.io/badge/install-pypi-blue?style=for-the-badge&logo=python&color=e57578&logoColor=FFFFFF&labelColor=262a35)](https://pypi.org/project/just-update-arch/)
 
 Updates packages from the [Arch User Repository](https://aur.archlinux.org/), alongside
 the vanilla arch packages, installed as normal through [`pacman`](https://wiki.archlinux.org/title/pacman).
 
 ## Usage
 
 There is no complexity to this script, all you have to do is run the command:
@@ -32,15 +32,15 @@
 
 You can install it from [GitHub](https://github.com/MolassesLover/JustUpdateArch):
 ```sh
 ➜ pip install git+https://github.com/MolassesLover/JustUpdateArch.git
 ```
 Alternatively, from [PyPi](https://pypi.org/project/just_update_arch):
 ```sh
-➜ pip install just_update_arch
+➜ pip install just-update-arch
 ```
 
 ## License
 All files within this repository are licensed under the
 [GNU General Public License v3.0](`LICENSE.md`).
 
 ## Contributing
```

### Comparing `just_update_arch-0.1.0/README.md` & `just_update_arch-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Just Update Arch
 
 [![Ko-Fi](https://img.shields.io/badge/donate-kofi-blue?style=for-the-badge&logo=ko-fi&color=e57578&logoColor=FFFFFF&labelColor=262a35)](https://ko-fi.com/molasses)
 [![Patreon](https://img.shields.io/badge/donate-patreon-blue?style=for-the-badge&logo=patreon&color=e57578&logoColor=FFFFFF&labelColor=262a35)](https://www.patreon.com/molasseslover)
-[![PyPi](https://img.shields.io/badge/install-pypi-blue?style=for-the-badge&logo=python&color=e57578&logoColor=FFFFFF&labelColor=262a35)](https://pypi.org/project/just_update_arch)
+[![PyPi](https://img.shields.io/badge/install-pypi-blue?style=for-the-badge&logo=python&color=e57578&logoColor=FFFFFF&labelColor=262a35)](https://pypi.org/project/just-update-arch/)
 
 Updates packages from the [Arch User Repository](https://aur.archlinux.org/), alongside
 the vanilla arch packages, installed as normal through [`pacman`](https://wiki.archlinux.org/title/pacman).
 
 ## Usage
 
 There is no complexity to this script, all you have to do is run the command:
@@ -21,15 +21,15 @@
 
 You can install it from [GitHub](https://github.com/MolassesLover/JustUpdateArch):
 ```sh
 ➜ pip install git+https://github.com/MolassesLover/JustUpdateArch.git
 ```
 Alternatively, from [PyPi](https://pypi.org/project/just_update_arch):
 ```sh
-➜ pip install just_update_arch
+➜ pip install just-update-arch
 ```
 
 ## License
 All files within this repository are licensed under the
 [GNU General Public License v3.0](`LICENSE.md`).
 
 ## Contributing
```

### Comparing `just_update_arch-0.1.0/just_update_arch/cli.py` & `just_update_arch-0.1.1/just_update_arch/cli.py`

 * *Files identical despite different names*

### Comparing `just_update_arch-0.1.0/just_update_arch.egg-info/PKG-INFO` & `just_update_arch-0.1.1/just_update_arch.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: just-update-arch
-Version: 0.1.0
+Version: 0.1.1
 Summary: Updates installed AUR packages.
 Home-page: https://github.com/MolassesLover/JustUpdateArch
 Author: MolassesLover
 Author-email: 60114762+MolassesLover@users.noreply.github.com
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Just Update Arch
 
 [![Ko-Fi](https://img.shields.io/badge/donate-kofi-blue?style=for-the-badge&logo=ko-fi&color=e57578&logoColor=FFFFFF&labelColor=262a35)](https://ko-fi.com/molasses)
 [![Patreon](https://img.shields.io/badge/donate-patreon-blue?style=for-the-badge&logo=patreon&color=e57578&logoColor=FFFFFF&labelColor=262a35)](https://www.patreon.com/molasseslover)
-[![PyPi](https://img.shields.io/badge/install-pypi-blue?style=for-the-badge&logo=python&color=e57578&logoColor=FFFFFF&labelColor=262a35)](https://pypi.org/project/just_update_arch)
+[![PyPi](https://img.shields.io/badge/install-pypi-blue?style=for-the-badge&logo=python&color=e57578&logoColor=FFFFFF&labelColor=262a35)](https://pypi.org/project/just-update-arch/)
 
 Updates packages from the [Arch User Repository](https://aur.archlinux.org/), alongside
 the vanilla arch packages, installed as normal through [`pacman`](https://wiki.archlinux.org/title/pacman).
 
 ## Usage
 
 There is no complexity to this script, all you have to do is run the command:
@@ -32,15 +32,15 @@
 
 You can install it from [GitHub](https://github.com/MolassesLover/JustUpdateArch):
 ```sh
 ➜ pip install git+https://github.com/MolassesLover/JustUpdateArch.git
 ```
 Alternatively, from [PyPi](https://pypi.org/project/just_update_arch):
 ```sh
-➜ pip install just_update_arch
+➜ pip install just-update-arch
 ```
 
 ## License
 All files within this repository are licensed under the
 [GNU General Public License v3.0](`LICENSE.md`).
 
 ## Contributing
```

