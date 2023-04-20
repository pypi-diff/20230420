# Comparing `tmp/serverjars-api-1.0.1.tar.gz` & `tmp/serverjars-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serverjars-api-1.0.1.tar", last modified: Mon Sep  5 23:34:39 2022, max compression
+gzip compressed data, was "serverjars-api-1.1.0.tar", last modified: Thu Apr 20 20:28:22 2023, max compression
```

## Comparing `serverjars-api-1.0.1.tar` & `serverjars-api-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-09-05 23:34:39.393793 serverjars-api-1.0.1/
--rw-rw-rw-   0        0        0     1077 2022-01-20 21:59:27.000000 serverjars-api-1.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     1648 2022-09-05 23:34:39.393793 serverjars-api-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      947 2022-09-05 22:41:13.000000 serverjars-api-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-09-05 23:34:39.376457 serverjars-api-1.0.1/ServerJars/
--rw-rw-rw-   0        0        0     4103 2022-09-05 23:32:51.000000 serverjars-api-1.0.1/ServerJars/__init__.py
--rw-rw-rw-   0        0        0     1014 2022-09-05 22:47:04.000000 serverjars-api-1.0.1/ServerJars/constants.py
-drwxrwxrwx   0        0        0        0 2022-09-05 23:34:39.393793 serverjars-api-1.0.1/serverjars_api.egg-info/
--rw-rw-rw-   0        0        0     1648 2022-09-05 23:34:39.000000 serverjars-api-1.0.1/serverjars_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2022-09-05 23:34:39.000000 serverjars-api-1.0.1/serverjars_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-05 23:34:39.000000 serverjars-api-1.0.1/serverjars_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-09-05 23:34:39.000000 serverjars-api-1.0.1/serverjars_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-09-05 23:34:39.000000 serverjars-api-1.0.1/serverjars_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2022-09-05 23:34:39.393793 serverjars-api-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1104 2022-09-05 23:33:48.000000 serverjars-api-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:28:22.507393 serverjars-api-1.1.0/
+-rw-rw-rw-   0        0        0     1077 2022-01-20 21:59:27.000000 serverjars-api-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0     1476 2023-04-20 20:28:22.507393 serverjars-api-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      741 2023-04-20 20:20:43.000000 serverjars-api-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 20:28:22.494393 serverjars-api-1.1.0/serverjars/
+-rw-rw-rw-   0        0        0     5593 2023-04-20 20:26:30.000000 serverjars-api-1.1.0/serverjars/__init__.py
+-rw-rw-rw-   0        0        0      580 2023-04-20 19:20:46.000000 serverjars-api-1.1.0/serverjars/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:28:22.506393 serverjars-api-1.1.0/serverjars_api.egg-info/
+-rw-rw-rw-   0        0        0     1476 2023-04-20 20:28:22.000000 serverjars-api-1.1.0/serverjars_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-20 20:28:22.000000 serverjars-api-1.1.0/serverjars_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 20:28:22.000000 serverjars-api-1.1.0/serverjars_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 20:28:22.000000 serverjars-api-1.1.0/serverjars_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 20:28:22.000000 serverjars-api-1.1.0/serverjars_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      114 2023-04-20 20:28:22.510394 serverjars-api-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1147 2023-04-20 20:23:30.000000 serverjars-api-1.1.0/setup.py
```

### Comparing `serverjars-api-1.0.1/LICENSE.md` & `serverjars-api-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `serverjars-api-1.0.1/setup.py` & `serverjars-api-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 with open('README.md') as f:
     long_description = f.read()
 
 required_modules = ["requests"]
 
 setuptools.setup(
     name='serverjars-api',
-    version='1.0.1',
+    version='1.1.0',
     author='Legopitstop',
-    description='The unofficial Python API for ServerJars',
+    description='The unofficial Python wrapper for serverjars.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/legopitstop/serverjars-python-api-wrapper',
     packages=setuptools.find_packages(),
     install_requires=required_modules,
     license='MIT',
-    keywords=['ServerJars', 'API'],
+    keywords=['ServerJars', 'Minecraft', "Servers", "Bedrock", 'API'],
     author_email='officiallegopitstop@gmail.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable', # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Operating System :: Microsoft :: Windows',
```

