# Comparing `tmp/win23crypt-0.1.3.tar.gz` & `tmp/win23crypt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "win23crypt-0.1.3.tar", last modified: Thu Apr 20 20:44:59 2023, max compression
+gzip compressed data, was "win23crypt-0.1.4.tar", last modified: Thu Apr 20 20:48:50 2023, max compression
```

## Comparing `win23crypt-0.1.3.tar` & `win23crypt-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 20:45:00.000000 win23crypt-0.1.3/
--rw-rw-rw-   0        0        0      145 2023-04-20 20:45:00.000000 win23crypt-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-20 20:45:00.000000 win23crypt-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      215 2023-04-20 20:44:48.000000 win23crypt-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:45:00.000000 win23crypt-0.1.3/win23crypt/
--rw-rw-rw-   0        0        0      101 2023-04-20 19:45:58.000000 win23crypt-0.1.3/win23crypt/__init__.py
--rw-rw-rw-   0        0        0     9524 2023-04-20 20:44:38.000000 win23crypt-0.1.3/win23crypt/hypixel_api.py
--rw-rw-rw-   0        0        0      770 2023-04-20 19:34:26.000000 win23crypt-0.1.3/win23crypt/python_mc.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:45:00.000000 win23crypt-0.1.3/win23crypt.egg-info/
--rw-rw-rw-   0        0        0      145 2023-04-20 20:45:00.000000 win23crypt-0.1.3/win23crypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-04-20 20:45:00.000000 win23crypt-0.1.3/win23crypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 20:45:00.000000 win23crypt-0.1.3/win23crypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-20 20:45:00.000000 win23crypt-0.1.3/win23crypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 20:45:00.000000 win23crypt-0.1.3/win23crypt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 20:48:52.000000 win23crypt-0.1.4/
+-rw-rw-rw-   0        0        0      145 2023-04-20 20:48:52.000000 win23crypt-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-20 20:48:52.000000 win23crypt-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      260 2023-04-20 20:48:44.000000 win23crypt-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:48:52.000000 win23crypt-0.1.4/win23crypt/
+-rw-rw-rw-   0        0        0      101 2023-04-20 19:45:58.000000 win23crypt-0.1.4/win23crypt/__init__.py
+-rw-rw-rw-   0        0        0     9524 2023-04-20 20:44:38.000000 win23crypt-0.1.4/win23crypt/hypixel_api.py
+-rw-rw-rw-   0        0        0      770 2023-04-20 19:34:26.000000 win23crypt-0.1.4/win23crypt/python_mc.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:48:52.000000 win23crypt-0.1.4/win23crypt.egg-info/
+-rw-rw-rw-   0        0        0      145 2023-04-20 20:48:52.000000 win23crypt-0.1.4/win23crypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-04-20 20:48:52.000000 win23crypt-0.1.4/win23crypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 20:48:52.000000 win23crypt-0.1.4/win23crypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-20 20:48:52.000000 win23crypt-0.1.4/win23crypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 20:48:52.000000 win23crypt-0.1.4/win23crypt.egg-info/top_level.txt
```

### Comparing `win23crypt-0.1.3/win23crypt/hypixel_api.py` & `win23crypt-0.1.4/win23crypt/hypixel_api.py`

 * *Files identical despite different names*

### Comparing `win23crypt-0.1.3/win23crypt/python_mc.py` & `win23crypt-0.1.4/win23crypt/python_mc.py`

 * *Files identical despite different names*

