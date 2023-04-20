# Comparing `tmp/UniverseLists-0.2.tar.gz` & `tmp/UniverseLists-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniverseLists-0.2.tar", last modified: Thu Apr 20 16:13:19 2023, max compression
+gzip compressed data, was "UniverseLists-0.3.tar", last modified: Thu Apr 20 16:27:37 2023, max compression
```

## Comparing `UniverseLists-0.2.tar` & `UniverseLists-0.3.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 16:13:19.448789 UniverseLists-0.2/
--rw-rw-rw-   0        0        0      491 2023-04-20 16:13:19.447195 UniverseLists-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-20 16:09:42.000000 UniverseLists-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 16:13:19.445192 UniverseLists-0.2/UniverseLists.egg-info/
--rw-rw-rw-   0        0        0      491 2023-04-20 16:13:19.000000 UniverseLists-0.2/UniverseLists.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-04-20 16:13:19.000000 UniverseLists-0.2/UniverseLists.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 16:13:19.000000 UniverseLists-0.2/UniverseLists.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 16:13:19.000000 UniverseLists-0.2/UniverseLists.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      523 2023-04-20 16:06:56.000000 UniverseLists-0.2/autoposter.py
--rw-rw-rw-   0        0        0       42 2023-04-20 16:13:19.449708 UniverseLists-0.2/setup.cfg
--rw-rw-rw-   0        0        0      370 2023-04-20 16:13:05.000000 UniverseLists-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:27:37.509887 UniverseLists-0.3/
+-rw-rw-rw-   0        0        0     1085 2023-04-20 16:27:02.000000 UniverseLists-0.3/LICENSE
+-rw-rw-rw-   0        0        0      899 2023-04-20 16:27:37.509383 UniverseLists-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-20 16:09:42.000000 UniverseLists-0.3/README.md
+-rw-rw-rw-   0        0        0      666 2023-04-20 16:26:53.000000 UniverseLists-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 16:27:37.510890 UniverseLists-0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 16:27:37.473363 UniverseLists-0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 16:27:37.487139 UniverseLists-0.3/src/UniverseLists/
+-rw-rw-rw-   0        0        0        0 2023-04-20 16:23:55.000000 UniverseLists-0.3/src/UniverseLists/__init__.py
+-rw-rw-rw-   0        0        0      523 2023-04-20 16:06:56.000000 UniverseLists-0.3/src/UniverseLists/autoposter.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:27:37.505879 UniverseLists-0.3/src/UniverseLists.egg-info/
+-rw-rw-rw-   0        0        0      899 2023-04-20 16:27:37.000000 UniverseLists-0.3/src/UniverseLists.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-04-20 16:27:37.000000 UniverseLists-0.3/src/UniverseLists.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 16:27:37.000000 UniverseLists-0.3/src/UniverseLists.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-20 16:27:37.000000 UniverseLists-0.3/src/UniverseLists.egg-info/top_level.txt
```

### Comparing `UniverseLists-0.2/autoposter.py` & `UniverseLists-0.3/src/UniverseLists/autoposter.py`

 * *Files identical despite different names*

