# Comparing `tmp/pelican-redirect-url-0.1.0.tar.gz` & `tmp/pelican-redirect-url-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican-redirect-url-0.1.0.tar", last modified: Thu Apr 20 13:51:26 2023, max compression
+gzip compressed data, was "pelican-redirect-url-0.1.1.tar", last modified: Thu Apr 20 13:56:50 2023, max compression
```

## Comparing `pelican-redirect-url-0.1.0.tar` & `pelican-redirect-url-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-20 13:51:25.999963 pelican-redirect-url-0.1.0/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    34523 2023-04-20 13:50:47.000000 pelican-redirect-url-0.1.0/COPYING
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       16 2023-04-20 13:50:47.000000 pelican-redirect-url-0.1.0/MANIFEST.in
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1780 2023-04-20 13:51:25.999963 pelican-redirect-url-0.1.0/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      821 2023-04-20 13:50:47.000000 pelican-redirect-url-0.1.0/README.md
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-20 13:51:25.995963 pelican-redirect-url-0.1.0/pelican/
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-20 13:51:25.995963 pelican-redirect-url-0.1.0/pelican/plugins/
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-20 13:51:25.995963 pelican-redirect-url-0.1.0/pelican/plugins/redirect_url/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      187 2023-04-20 13:50:47.000000 pelican-redirect-url-0.1.0/pelican/plugins/redirect_url/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1931 2023-04-20 13:50:47.000000 pelican-redirect-url-0.1.0/pelican/plugins/redirect_url/redirect_url.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-20 13:51:25.995963 pelican-redirect-url-0.1.0/pelican_redirect_url.egg-info/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1780 2023-04-20 13:51:25.000000 pelican-redirect-url-0.1.0/pelican_redirect_url.egg-info/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      370 2023-04-20 13:51:25.000000 pelican-redirect-url-0.1.0/pelican_redirect_url.egg-info/SOURCES.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2023-04-20 13:51:25.000000 pelican-redirect-url-0.1.0/pelican_redirect_url.egg-info/dependency_links.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       48 2023-04-20 13:51:25.000000 pelican-redirect-url-0.1.0/pelican_redirect_url.egg-info/requires.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        8 2023-04-20 13:51:25.000000 pelican-redirect-url-0.1.0/pelican_redirect_url.egg-info/top_level.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       38 2023-04-20 13:51:25.999963 pelican-redirect-url-0.1.0/setup.cfg
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1637 2023-04-20 13:50:47.000000 pelican-redirect-url-0.1.0/setup.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-20 13:51:25.999963 pelican-redirect-url-0.1.0/tests/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2844 2023-04-20 13:50:47.000000 pelican-redirect-url-0.1.0/tests/test_redirect_url.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-20 13:56:50.210955 pelican-redirect-url-0.1.1/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    34523 2023-04-20 13:50:47.000000 pelican-redirect-url-0.1.1/COPYING
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       16 2023-04-20 13:50:47.000000 pelican-redirect-url-0.1.1/MANIFEST.in
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1779 2023-04-20 13:56:50.210955 pelican-redirect-url-0.1.1/PKG-INFO
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      821 2023-04-20 13:50:47.000000 pelican-redirect-url-0.1.1/README.md
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-20 13:56:50.202955 pelican-redirect-url-0.1.1/pelican/
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-20 13:56:50.206955 pelican-redirect-url-0.1.1/pelican/plugins/
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-20 13:56:50.206955 pelican-redirect-url-0.1.1/pelican/plugins/redirect_url/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      187 2023-04-20 13:50:47.000000 pelican-redirect-url-0.1.1/pelican/plugins/redirect_url/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1931 2023-04-20 13:50:47.000000 pelican-redirect-url-0.1.1/pelican/plugins/redirect_url/redirect_url.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-20 13:56:50.210955 pelican-redirect-url-0.1.1/pelican_redirect_url.egg-info/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1779 2023-04-20 13:56:50.000000 pelican-redirect-url-0.1.1/pelican_redirect_url.egg-info/PKG-INFO
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      370 2023-04-20 13:56:50.000000 pelican-redirect-url-0.1.1/pelican_redirect_url.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2023-04-20 13:56:50.000000 pelican-redirect-url-0.1.1/pelican_redirect_url.egg-info/dependency_links.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       48 2023-04-20 13:56:50.000000 pelican-redirect-url-0.1.1/pelican_redirect_url.egg-info/requires.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        8 2023-04-20 13:56:50.000000 pelican-redirect-url-0.1.1/pelican_redirect_url.egg-info/top_level.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       38 2023-04-20 13:56:50.210955 pelican-redirect-url-0.1.1/setup.cfg
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1636 2023-04-20 13:56:40.000000 pelican-redirect-url-0.1.1/setup.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-20 13:56:50.210955 pelican-redirect-url-0.1.1/tests/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2844 2023-04-20 13:50:47.000000 pelican-redirect-url-0.1.1/tests/test_redirect_url.py
```

### Comparing `pelican-redirect-url-0.1.0/COPYING` & `pelican-redirect-url-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `pelican-redirect-url-0.1.0/PKG-INFO` & `pelican-redirect-url-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pelican-redirect-url
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pelican plugin to redirect to any URL
-Home-page: https://github.com/FriedrichFroebel/pelican-redirect-urls/
+Home-page: https://github.com/FriedrichFroebel/pelican-redirect-url/
 Author: FriedrichFröbel
 License: AGPL-3.0
 Keywords: pelican,plugin,redirect
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
```

### Comparing `pelican-redirect-url-0.1.0/README.md` & `pelican-redirect-url-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pelican-redirect-url-0.1.0/pelican/plugins/redirect_url/redirect_url.py` & `pelican-redirect-url-0.1.1/pelican/plugins/redirect_url/redirect_url.py`

 * *Files identical despite different names*

### Comparing `pelican-redirect-url-0.1.0/pelican_redirect_url.egg-info/PKG-INFO` & `pelican-redirect-url-0.1.1/pelican_redirect_url.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pelican-redirect-url
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pelican plugin to redirect to any URL
-Home-page: https://github.com/FriedrichFroebel/pelican-redirect-urls/
+Home-page: https://github.com/FriedrichFroebel/pelican-redirect-url/
 Author: FriedrichFröbel
 License: AGPL-3.0
 Keywords: pelican,plugin,redirect
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
```

### Comparing `pelican-redirect-url-0.1.0/setup.py` & `pelican-redirect-url-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 ROOT_DIRECTORY = Path(__file__).parent.resolve()
 
 
 setup(
     name="pelican-redirect-url",
     description="Pelican plugin to redirect to any URL",
-    version="0.1.0",
+    version="0.1.1",
     license="AGPL-3.0",
     long_description=(ROOT_DIRECTORY / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     author="FriedrichFröbel",
-    url="https://github.com/FriedrichFroebel/pelican-redirect-urls/",
+    url="https://github.com/FriedrichFroebel/pelican-redirect-url/",
     packages=find_namespace_packages(
         where=".",
         include=[
             "pelican.plugins.redirect_url",
             "pelican.plugins.redirect_url.*",
         ],
     ),
```

### Comparing `pelican-redirect-url-0.1.0/tests/test_redirect_url.py` & `pelican-redirect-url-0.1.1/tests/test_redirect_url.py`

 * *Files identical despite different names*

