# Comparing `tmp/jupyterlab_h5web-7.1.0.tar.gz` & `tmp/jupyterlab_h5web-7.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/jupyterlab-h5web/jupyterlab-h5web/dist/.tmp-3trg1z60/jupyterlab_h5web-7.1.0.tar", last modified: Tue Apr 18 08:57:37 2023, max compression
+gzip compressed data, was "/home/runner/work/jupyterlab-h5web/jupyterlab-h5web/dist/.tmp-85lrh3j6/jupyterlab_h5web-7.1.1.tar", last modified: Thu Apr 20 12:16:39 2023, max compression
```

## Comparing `jupyterlab_h5web-7.1.0.tar` & `jupyterlab_h5web-7.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/jupyter-config/nb-config/jupyterlab_h5web.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/jupyter-config/server-config/jupyterlab_h5web.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-04-18 08:54:51.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)  1208336 2023-04-18 08:54:51.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-18 08:54:51.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-04-18 08:54:51.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/static/317.7320f9f9a065f27d09c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    39615 2023-04-18 08:54:51.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/static/549.8a4bd7ffba6e2772bada.js
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-04-18 08:54:51.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/static/remoteEntry.fcd5580296bb57fbb2e8.js
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 08:54:33.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    80860 2023-04-18 08:54:51.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:54:22.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/jupyterlab_h5web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/src/H5webApp.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/src/browser.ts
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/src/fileType.ts
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/src/icons.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/src/mimeplugin.tsx
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/src/svg.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/src/widget.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:57:37.000000 jupyterlab_h5web-7.1.0/style/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/style/h5web-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/style/hdf5-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-18 08:52:58.000000 jupyterlab_h5web-7.1.0/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)   296546 2023-04-18 08:53:53.000000 jupyterlab_h5web-7.1.0/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/jupyter-config/nb-config/jupyterlab_h5web.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/jupyter-config/server-config/jupyterlab_h5web.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-04-20 12:13:30.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)  1208336 2023-04-20 12:13:30.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-20 12:13:30.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-04-20 12:13:30.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/317.7320f9f9a065f27d09c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39615 2023-04-20 12:13:30.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/549.8a4bd7ffba6e2772bada.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-04-20 12:13:30.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/remoteEntry.ec65a8378b6cbb458b20.js
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 12:13:07.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80860 2023-04-20 12:13:30.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:12:54.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/H5webApp.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/browser.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/fileType.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/icons.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/mimeplugin.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/svg.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/widget.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/style/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/style/h5web-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/style/hdf5-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)   296546 2023-04-20 12:12:21.000000 jupyterlab_h5web-7.1.1/yarn.lock
```

### Comparing `jupyterlab_h5web-7.1.0/LICENSE.md` & `jupyterlab_h5web-7.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/MANIFEST.in` & `jupyterlab_h5web-7.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/PKG-INFO` & `jupyterlab_h5web-7.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_h5web
-Version: 7.1.0
+Version: 7.1.1
 Summary: A JupyterLab extension to explore and visualize HDF5 file contents.
 Home-page: https://github.com/silx-kit/jupyterlab-h5web
 Author: European Synchrotron Radiation Facility
 Author-email: h5web@esrf.fr
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `jupyterlab_h5web-7.1.0/README.md` & `jupyterlab_h5web-7.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/jupyterlab_h5web/__init__.py` & `jupyterlab_h5web-7.1.1/jupyterlab_h5web/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/jupyterlab_h5web/_version.py` & `jupyterlab_h5web-7.1.1/jupyterlab_h5web/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/jupyterlab_h5web/handlers.py` & `jupyterlab_h5web-7.1.1/jupyterlab_h5web/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,17 +58,18 @@
         assert isinstance(content, ResolvedEntityContent)
         return content.attributes()
 
 
 class DataHandler(ContentHandler):
     def parse_content(self, content):
         selection = self.get_query_argument("selection", None)
+        dtype = self.get_query_argument("dtype", None)
 
         assert isinstance(content, DatasetContent)
-        return content.data(selection)
+        return content.data(selection, dtype=dtype)
 
 
 class MetadataHandler(ContentHandler):
     def parse_content(self, content):
         return content.metadata()
```

### Comparing `jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/package.json` & `jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9731359649122806%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ec65a8378b6cbb458b20.js'}}",*

 * * "'version'": "'7.1.1'"}*

```diff
@@ -45,15 +45,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/silx-kit/jupyterlab-h5web",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.fcd5580296bb57fbb2e8.js",
+            "load": "static/remoteEntry.ec65a8378b6cbb458b20.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_h5web"
                 },
@@ -99,9 +99,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "7.1.0"
+    "version": "7.1.1"
 }
```

### Comparing `jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js` & `jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js.LICENSE.txt` & `jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/static/317.7320f9f9a065f27d09c7.js` & `jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/317.7320f9f9a065f27d09c7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/static/549.8a4bd7ffba6e2772bada.js` & `jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/549.8a4bd7ffba6e2772bada.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/static/remoteEntry.fcd5580296bb57fbb2e8.js` & `jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/remoteEntry.ec65a8378b6cbb458b20.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -112,15 +112,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@h5web/app", "7.1.0", (() => Promise.all([E.e(295), E.e(832)]).then((() => () => E(6295))))), l("jupyterlab-h5web", "7.1.0", (() => Promise.all([E.e(832), E.e(317)]).then((() => () => E(317)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@h5web/app", "7.1.0", (() => Promise.all([E.e(295), E.e(832)]).then((() => () => E(6295))))), l("jupyterlab-h5web", "7.1.1", (() => Promise.all([E.e(832), E.e(317)]).then((() => () => E(317)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_h5web-7.1.0/jupyterlab_h5web/labextension/static/third-party-licenses.json` & `jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/jupyterlab_h5web/widget.py` & `jupyterlab_h5web-7.1.1/jupyterlab_h5web/widget.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/jupyterlab_h5web.egg-info/PKG-INFO` & `jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-h5web
-Version: 7.1.0
+Version: 7.1.1
 Summary: A JupyterLab extension to explore and visualize HDF5 file contents.
 Home-page: https://github.com/silx-kit/jupyterlab-h5web
 Author: European Synchrotron Radiation Facility
 Author-email: h5web@esrf.fr
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `jupyterlab_h5web-7.1.0/jupyterlab_h5web.egg-info/SOURCES.txt` & `jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 jupyterlab_h5web.egg-info/requires.txt
 jupyterlab_h5web.egg-info/top_level.txt
 jupyterlab_h5web/labextension/package.json
 jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js
 jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js.LICENSE.txt
 jupyterlab_h5web/labextension/static/317.7320f9f9a065f27d09c7.js
 jupyterlab_h5web/labextension/static/549.8a4bd7ffba6e2772bada.js
-jupyterlab_h5web/labextension/static/remoteEntry.fcd5580296bb57fbb2e8.js
+jupyterlab_h5web/labextension/static/remoteEntry.ec65a8378b6cbb458b20.js
 jupyterlab_h5web/labextension/static/style.js
 jupyterlab_h5web/labextension/static/third-party-licenses.json
 src/H5webApp.tsx
 src/browser.ts
 src/fileType.ts
 src/icons.ts
 src/index.ts
```

### Comparing `jupyterlab_h5web-7.1.0/package.json` & `jupyterlab_h5web-7.1.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736842105263158%*

 * *Differences: {"'version'": "'7.1.1'"}*

```diff
@@ -94,9 +94,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "7.1.0"
+    "version": "7.1.1"
 }
```

### Comparing `jupyterlab_h5web-7.1.0/pyproject.toml` & `jupyterlab_h5web-7.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/setup.py` & `jupyterlab_h5web-7.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/src/H5webApp.tsx` & `jupyterlab_h5web-7.1.1/src/H5webApp.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/src/browser.ts` & `jupyterlab_h5web-7.1.1/src/browser.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/src/fileType.ts` & `jupyterlab_h5web-7.1.1/src/fileType.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/src/index.ts` & `jupyterlab_h5web-7.1.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/src/mimeplugin.tsx` & `jupyterlab_h5web-7.1.1/src/mimeplugin.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/src/widget.tsx` & `jupyterlab_h5web-7.1.1/src/widget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/style/h5web-icon.svg` & `jupyterlab_h5web-7.1.1/style/h5web-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/style/hdf5-icon.svg` & `jupyterlab_h5web-7.1.1/style/hdf5-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/style/index.css` & `jupyterlab_h5web-7.1.1/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/tsconfig.json` & `jupyterlab_h5web-7.1.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.0/yarn.lock` & `jupyterlab_h5web-7.1.1/yarn.lock`

 * *Files identical despite different names*

