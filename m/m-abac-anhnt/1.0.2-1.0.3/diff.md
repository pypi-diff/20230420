# Comparing `tmp/m-abac-anhnt-1.0.2.tar.gz` & `tmp/m-abac-anhnt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abac-anhnt-1.0.2.tar", last modified: Thu Apr 20 09:59:29 2023, max compression
+gzip compressed data, was "m-abac-anhnt-1.0.3.tar", last modified: Thu Apr 20 10:05:14 2023, max compression
```

## Comparing `m-abac-anhnt-1.0.2.tar` & `m-abac-anhnt-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 09:59:29.081699 m-abac-anhnt-1.0.2/
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     2012 2023-04-20 09:59:29.081699 m-abac-anhnt-1.0.2/PKG-INFO
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1115 2023-04-13 06:35:19.000000 m-abac-anhnt-1.0.2/README.md
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 09:59:29.081699 m-abac-anhnt-1.0.2/m_abac_anhnt.egg-info/
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     2012 2023-04-20 09:59:29.000000 m-abac-anhnt-1.0.2/m_abac_anhnt.egg-info/PKG-INFO
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      212 2023-04-20 09:59:29.000000 m-abac-anhnt-1.0.2/m_abac_anhnt.egg-info/SOURCES.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)        1 2023-04-20 09:59:29.000000 m-abac-anhnt-1.0.2/m_abac_anhnt.egg-info/dependency_links.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      100 2023-04-20 09:59:29.000000 m-abac-anhnt-1.0.2/m_abac_anhnt.egg-info/requires.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)        1 2023-04-20 09:59:29.000000 m-abac-anhnt-1.0.2/m_abac_anhnt.egg-info/top_level.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      104 2022-12-15 03:46:40.000000 m-abac-anhnt-1.0.2/pyproject.toml
--rw-rw-r--   0 mobio     (1000) mobio     (1000)       38 2023-04-20 09:59:29.081699 m-abac-anhnt-1.0.2/setup.cfg
--rw-r--r--   0 mobio     (1000) mobio     (1000)     9788 2023-04-20 09:58:40.000000 m-abac-anhnt-1.0.2/setup.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:05:14.506660 m-abac-anhnt-1.0.3/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     2012 2023-04-20 10:05:14.506660 m-abac-anhnt-1.0.3/PKG-INFO
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1115 2023-04-13 06:35:19.000000 m-abac-anhnt-1.0.3/README.md
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:05:14.506660 m-abac-anhnt-1.0.3/m_abac_anhnt.egg-info/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     2012 2023-04-20 10:05:14.000000 m-abac-anhnt-1.0.3/m_abac_anhnt.egg-info/PKG-INFO
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      212 2023-04-20 10:05:14.000000 m-abac-anhnt-1.0.3/m_abac_anhnt.egg-info/SOURCES.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)        1 2023-04-20 10:05:14.000000 m-abac-anhnt-1.0.3/m_abac_anhnt.egg-info/dependency_links.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      100 2023-04-20 10:05:14.000000 m-abac-anhnt-1.0.3/m_abac_anhnt.egg-info/requires.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)        1 2023-04-20 10:05:14.000000 m-abac-anhnt-1.0.3/m_abac_anhnt.egg-info/top_level.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      104 2022-12-15 03:46:40.000000 m-abac-anhnt-1.0.3/pyproject.toml
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)       38 2023-04-20 10:05:14.506660 m-abac-anhnt-1.0.3/setup.cfg
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     9779 2023-04-20 10:05:03.000000 m-abac-anhnt-1.0.3/setup.py
```

### Comparing `m-abac-anhnt-1.0.2/PKG-INFO` & `m-abac-anhnt-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-anhnt
-Version: 1.0.2
+Version: 1.0.3
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
```

### Comparing `m-abac-anhnt-1.0.2/README.md` & `m-abac-anhnt-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.2/m_abac_anhnt.egg-info/PKG-INFO` & `m-abac-anhnt-1.0.3/m_abac_anhnt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-anhnt
-Version: 1.0.2
+Version: 1.0.3
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
```

### Comparing `m-abac-anhnt-1.0.2/setup.py` & `m-abac-anhnt-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.2',  # Required
+    version='1.0.3',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -139,15 +139,15 @@
     #
     # Note that this is a list of additional keywords, separated
     # by commas, to be used to assist searching for the distribution in a
     # larger catalog.
     keywords="mobio, mobio-engine, m-abac",  # Optional
     # When your source code is in a subdirectory under the project root, e.g.
     # `src/`, it is necessary to specify the `package_dir` argument.
-    package_dir={'mobio.libs.abac': 'mobio/libs/abac'},  # Optional
+    package_dir={'mobio.libs.abac': 'm_abac'},  # Optional
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
     # called `my_module.py` to exist:
     #
```

