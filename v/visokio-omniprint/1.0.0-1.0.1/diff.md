# Comparing `tmp/visokio_omniprint-1.0.0.tar.gz` & `tmp/visokio_omniprint-1.0.1.tar.gz`

## Comparing `visokio_omniprint-1.0.0.tar` & `visokio_omniprint-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/scripts/build.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/scripts/test_install.sh
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/scripts/test_upload.sh
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/visokio_omniprint/DriverBase.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/visokio_omniprint/Image.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/visokio_omniprint/ImagesPdf.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/visokio_omniprint/Pdf.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/visokio_omniprint/Tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/visokio_omniprint/__about__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/visokio_omniprint/__init__.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/.gitignore
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/README.md
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/scripts/build.sh
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/scripts/install.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/scripts/test_install.sh
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/scripts/test_upload.sh
+-rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/scripts/upload.sh
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/visokio_omniprint/DriverBase.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/visokio_omniprint/Image.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/visokio_omniprint/ImagesPdf.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/visokio_omniprint/Pdf.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/visokio_omniprint/Tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/visokio_omniprint/__about__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/visokio_omniprint/__init__.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/.gitignore
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/LICENSE
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/README.md
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.1/PKG-INFO
```

### Comparing `visokio_omniprint-1.0.0/visokio_omniprint/DriverBase.py` & `visokio_omniprint-1.0.1/visokio_omniprint/DriverBase.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,19 +27,21 @@
     def create_options(self):
         """
         This function creates a set of options that will be used to configure the ChromeDriver instance.
         """
         webdriver_options = Options()
         webdriver_prefs = {}
         # Add arguments to options
-        webdriver_options.add_argument("--headless")
+        webdriver_options.add_argument("--headless")  # TODO: explore new headless mode - https://developer.chrome.com/articles/new-headless/#:~:text=In%20a%20regular%20headful%20Chrome,number%20from%20the%20WebSocket%20URL.
         webdriver_options.add_argument("--disable-gpu")
         webdriver_options.add_argument("--no-sandbox")
         webdriver_options.add_argument("--disable-dev-shm-usage")
-        webdriver_options.add_argument("--window-size=1920,1080")
+        webdriver_options.add_argument("--window-size=1920,1080")  # TODO: document; why?
+        webdriver_options.add_argument("--ignore-certificate-errors") # Allow self-signed certificates. FIXME: update pypi for this change
+        # TODO: If remote debugging is needed, it can be added here: https://developer.chrome.com/blog/headless-chrome/#debugging-chrome-without-a-browser-ui
         # Add preferences to options
         webdriver_options.experimental_options["prefs"] = webdriver_prefs
         webdriver_prefs["profile.default_content_settings"] = {"images": 2}
         return webdriver_options
 
 
     def get_driver_docker(self, options):
```

### Comparing `visokio_omniprint-1.0.0/visokio_omniprint/ImagesPdf.py` & `visokio_omniprint-1.0.1/visokio_omniprint/ImagesPdf.py`

 * *Files identical despite different names*

### Comparing `visokio_omniprint-1.0.0/visokio_omniprint/Tools.py` & `visokio_omniprint-1.0.1/visokio_omniprint/Tools.py`

 * *Files identical despite different names*

### Comparing `visokio_omniprint-1.0.0/pyproject.toml` & `visokio_omniprint-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "visokio-omniprint"
-version = "1.0.0"
+version = "1.0.1"
 description = "Visokio Omniscope PDF printing library"
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
-  { name = "Visokio", email = "nils@visokio.com" },
+  { name = "Visokio" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -31,17 +31,17 @@
   "tinify",
   "fpdf",
   "urllib3"
 ]
 
 
 [project.urls]
-Documentation = "https://github.com/visokio/omniscope-custom-blocks/visokio-omniprint#readme"
-Issues = "https://github.com/visokio/omniscope-custom-blocks/visokio-omniprint/issues"
-Source = "https://github.com/visokio/omniscope-custom-blocks/visokio-omniprint"
+Documentation = "https://github.com/visokio/omniscope-custom-blocks/tree/master/visokio-omniprint#readme"
+Issues = "https://github.com/visokio/omniscope-custom-blocks/tree/master/visokio-omniprint/issues"
+Source = "https://github.com/visokio/omniscope-custom-blocks/tree/master/visokio-omniprint"
 
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
 ]
```

### Comparing `visokio_omniprint-1.0.0/PKG-INFO` & `visokio_omniprint-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: visokio-omniprint
-Version: 1.0.0
+Version: 1.0.1
 Summary: Visokio Omniscope PDF printing library
-Project-URL: Documentation, https://github.com/visokio/omniscope-custom-blocks/visokio-omniprint#readme
-Project-URL: Issues, https://github.com/visokio/omniscope-custom-blocks/visokio-omniprint/issues
-Project-URL: Source, https://github.com/visokio/omniscope-custom-blocks/visokio-omniprint
-Author-email: Visokio <nils@visokio.com>
+Project-URL: Documentation, https://github.com/visokio/omniscope-custom-blocks/tree/master/visokio-omniprint#readme
+Project-URL: Issues, https://github.com/visokio/omniscope-custom-blocks/tree/master/visokio-omniprint/issues
+Project-URL: Source, https://github.com/visokio/omniscope-custom-blocks/tree/master/visokio-omniprint
+Author: Visokio
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

