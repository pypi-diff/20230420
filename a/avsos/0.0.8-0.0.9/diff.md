# Comparing `tmp/avsos-0.0.8.tar.gz` & `tmp/avsos-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avsos-0.0.8.tar", last modified: Thu Apr 20 08:47:37 2023, max compression
+gzip compressed data, was "avsos-0.0.9.tar", last modified: Thu Apr 20 09:54:31 2023, max compression
```

## Comparing `avsos-0.0.8.tar` & `avsos-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 08:47:37.283645 avsos-0.0.8/
--rw-r--r--   0 kali      (1000) kali      (1000)       93 2023-04-20 08:47:37.279643 avsos-0.0.8/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     4011 2023-04-20 08:39:37.000000 avsos-0.0.8/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 08:47:37.275641 avsos-0.0.8/avsos/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-17 10:34:17.000000 avsos-0.0.8/avsos/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)      261 2023-04-17 17:22:40.000000 avsos-0.0.8/avsos/config.ini
--rwxrwxr-x   0 kali      (1000) kali      (1000)     1440 2023-04-20 08:08:45.000000 avsos-0.0.8/avsos/config.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     3283 2023-04-20 08:11:09.000000 avsos-0.0.8/avsos/encryption.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)    17394 2023-04-20 00:30:11.000000 avsos-0.0.8/avsos/main.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     5760 2023-04-20 08:28:21.000000 avsos-0.0.8/avsos/osint.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     5584 2023-04-20 00:28:39.000000 avsos-0.0.8/avsos/portscan.py
--rw-rw-rw-   0 kali      (1000) kali      (1000)  1140036 2023-03-22 16:54:30.000000 avsos-0.0.8/avsos/service-names-port-numbers.csv
--rwxrwxr-x   0 kali      (1000) kali      (1000)      353 2023-04-17 10:29:11.000000 avsos-0.0.8/avsos/setup.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)      480 2023-04-17 16:53:14.000000 avsos-0.0.8/avsos/start_zap.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     4077 2023-04-13 00:12:44.000000 avsos-0.0.8/avsos/utils.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     5492 2023-04-20 00:26:38.000000 avsos-0.0.8/avsos/zapscan.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 08:47:37.279643 avsos-0.0.8/avsos.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)       93 2023-04-20 08:47:37.000000 avsos-0.0.8/avsos.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      415 2023-04-20 08:47:37.000000 avsos-0.0.8/avsos.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-20 08:47:37.000000 avsos-0.0.8/avsos.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       42 2023-04-20 08:47:37.000000 avsos-0.0.8/avsos.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      208 2023-04-20 08:47:37.000000 avsos-0.0.8/avsos.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-20 08:47:37.000000 avsos-0.0.8/avsos.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-20 08:47:37.283645 avsos-0.0.8/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      729 2023-04-20 08:47:32.000000 avsos-0.0.8/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 09:54:31.198587 avsos-0.0.9/
+-rw-r--r--   0 kali      (1000) kali      (1000)       93 2023-04-20 09:54:31.198587 avsos-0.0.9/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     4011 2023-04-20 08:39:37.000000 avsos-0.0.9/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 09:54:31.198587 avsos-0.0.9/avsos/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-17 10:34:17.000000 avsos-0.0.9/avsos/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      261 2023-04-17 17:22:40.000000 avsos-0.0.9/avsos/config.ini
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     1440 2023-04-20 08:08:45.000000 avsos-0.0.9/avsos/config.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     3283 2023-04-20 08:11:09.000000 avsos-0.0.9/avsos/encryption.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)    17394 2023-04-20 00:30:11.000000 avsos-0.0.9/avsos/main.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     5760 2023-04-20 08:28:21.000000 avsos-0.0.9/avsos/osint.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     5584 2023-04-20 00:28:39.000000 avsos-0.0.9/avsos/portscan.py
+-rw-rw-rw-   0 kali      (1000) kali      (1000)  1140036 2023-03-22 16:54:30.000000 avsos-0.0.9/avsos/service-names-port-numbers.csv
+-rwxrwxr-x   0 kali      (1000) kali      (1000)      353 2023-04-17 10:29:11.000000 avsos-0.0.9/avsos/setup.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)      480 2023-04-17 16:53:14.000000 avsos-0.0.9/avsos/start_zap.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     4077 2023-04-13 00:12:44.000000 avsos-0.0.9/avsos/utils.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     5492 2023-04-20 00:26:38.000000 avsos-0.0.9/avsos/zapscan.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 09:54:31.198587 avsos-0.0.9/avsos.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)       93 2023-04-20 09:54:30.000000 avsos-0.0.9/avsos.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      415 2023-04-20 09:54:31.000000 avsos-0.0.9/avsos.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-20 09:54:30.000000 avsos-0.0.9/avsos.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       42 2023-04-20 09:54:30.000000 avsos-0.0.9/avsos.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      208 2023-04-20 09:54:30.000000 avsos-0.0.9/avsos.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-20 09:54:30.000000 avsos-0.0.9/avsos.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-20 09:54:31.198587 avsos-0.0.9/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      528 2023-04-20 09:47:01.000000 avsos-0.0.9/setup.py
```

### Comparing `avsos-0.0.8/README.md` & `avsos-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `avsos-0.0.8/avsos/config.py` & `avsos-0.0.9/avsos/config.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.8/avsos/encryption.py` & `avsos-0.0.9/avsos/encryption.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.8/avsos/main.py` & `avsos-0.0.9/avsos/main.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.8/avsos/osint.py` & `avsos-0.0.9/avsos/osint.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.8/avsos/portscan.py` & `avsos-0.0.9/avsos/portscan.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.8/avsos/service-names-port-numbers.csv` & `avsos-0.0.9/avsos/service-names-port-numbers.csv`

 * *Files identical despite different names*

### Comparing `avsos-0.0.8/avsos/utils.py` & `avsos-0.0.9/avsos/utils.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.8/avsos/zapscan.py` & `avsos-0.0.9/avsos/zapscan.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.8/setup.py` & `avsos-0.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
-classifiers = {
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: Linux",
-    }
-    
-"Homepage" == "https://github.com/Tomzy2506/AVSOS"
-
 setup(
     name="avsos",
-    version="0.0.8",
+    version="0.0.9",
     description = "An automated Vulnerability Scanner",
     readme = "README.md",
     packages=find_packages(),
     package_data={
         "avsos": ["config.ini", "service-names-port-numbers.csv"]
     },
     install_requires=required_packages,
```

